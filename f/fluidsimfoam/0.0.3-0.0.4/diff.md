# Comparing `tmp/fluidsimfoam-0.0.3.tar.gz` & `tmp/fluidsimfoam-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidsimfoam-0.0.3.tar", max compression
+gzip compressed data, was "fluidsimfoam-0.0.4.tar", max compression
```

## Comparing `fluidsimfoam-0.0.3.tar` & `fluidsimfoam-0.0.4.tar`

### file list

```diff
@@ -1,53 +1,60 @@
--rw-r--r--   0        0        0     1521 2023-03-02 21:01:46.291446 fluidsimfoam-0.0.3/LICENSE
--rw-r--r--   0        0        0     3951 2023-05-09 12:08:00.518116 fluidsimfoam-0.0.3/README.md
--rw-r--r--   0        0        0     1429 2023-05-09 13:09:30.236813 fluidsimfoam-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1807 2023-05-09 13:05:24.334349 fluidsimfoam-0.0.3/src/fluidsimfoam/__init__.py
--rw-r--r--   0        0        0     2195 2023-05-09 12:44:19.739747 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__init__.py
--rw-r--r--   0        0        0     2527 2023-05-09 12:44:22.103389 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    15511 2023-05-09 12:46:11.206907 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc
--rw-r--r--   0        0        0     2205 2023-05-09 12:43:04.211446 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc
--rw-r--r--   0        0        0     6100 2023-05-08 19:53:29.031102 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc
--rw-r--r--   0        0        0     2752 2023-05-08 19:53:29.031102 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc
--rw-r--r--   0        0        0     1844 2023-05-05 07:20:02.628943 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc
--rw-r--r--   0        0        0     5356 2023-05-09 12:43:04.227444 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc
--rw-r--r--   0        0        0    10473 2023-05-09 12:43:04.027476 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0        0        0     1082 2023-05-03 21:01:43.908143 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc
--rw-r--r--   0        0        0    15046 2023-05-09 12:44:45.871789 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/ast.py
--rw-r--r--   0        0        0     1080 2023-04-23 15:48:42.099657 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE
--rw-r--r--   0        0        0    13459 2023-05-05 07:30:16.059861 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py
--rw-r--r--   0        0        0    14477 2023-05-05 07:30:22.743807 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2344 2023-05-05 07:26:24.618314 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc
--rw-r--r--   0        0        0     3085 2023-05-05 07:26:24.622314 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc
--rw-r--r--   0        0        0     1810 2023-04-24 21:00:31.761612 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/edges.py
--rw-r--r--   0        0        0     3426 2023-04-24 20:58:16.942659 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/grading.py
--rw-r--r--   0        0        0     2135 2023-05-09 12:38:35.919916 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/constant_files.py
--rw-r--r--   0        0        0     5743 2023-05-08 19:04:20.598143 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/fields.py
--rw-r--r--   0        0        0     2414 2023-05-08 19:04:20.598143 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/fv_schemes.py
--rw-r--r--   0        0        0     5070 2023-05-09 12:42:19.787198 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/generators.py
--rw-r--r--   0        0        0     1918 2023-04-18 19:23:17.863337 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/grammar.lark
--rw-r--r--   0        0        0     2335 2023-04-18 19:23:17.863337 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/grammar_advanced.lark
--rw-r--r--   0        0        0     9522 2023-05-09 12:42:41.039310 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/parser.py
--rw-r--r--   0        0        0      973 2023-05-03 19:26:40.332634 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/polymesh.py
--rw-r--r--   0        0        0     1399 2023-05-09 12:54:58.927322 fluidsimfoam-0.0.3/src/fluidsimfoam/info.py
--rw-r--r--   0        0        0      124 2023-05-09 13:01:28.476575 fluidsimfoam-0.0.3/src/fluidsimfoam/init_fields.py
--rw-r--r--   0        0        0      747 2023-05-09 13:00:38.420124 fluidsimfoam-0.0.3/src/fluidsimfoam/log.py
--rw-r--r--   0        0        0      334 2023-05-09 12:56:28.245852 fluidsimfoam-0.0.3/src/fluidsimfoam/make.py
--rw-r--r--   0        0        0     1185 2023-05-09 12:57:19.118180 fluidsimfoam-0.0.3/src/fluidsimfoam/next_fluidsim_core.py
--rw-r--r--   0        0        0     1321 2023-05-09 12:57:49.645576 fluidsimfoam-0.0.3/src/fluidsimfoam/operators.py
--rw-r--r--   0        0        0      137 2023-05-09 12:48:51.690704 fluidsimfoam-0.0.3/src/fluidsimfoam/output/__init__.py
--rw-r--r--   0        0        0      314 2023-05-09 12:51:06.198419 fluidsimfoam-0.0.3/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7626 2023-05-09 09:32:45.016908 fluidsimfoam-0.0.3/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     9206 2023-05-09 09:29:43.622730 fluidsimfoam-0.0.3/src/fluidsimfoam/output/base.py
--rw-r--r--   0        0        0     1303 2023-05-09 12:58:11.670255 fluidsimfoam-0.0.3/src/fluidsimfoam/params.py
--rw-r--r--   0        0        0      573 2023-05-09 13:02:35.270502 fluidsimfoam-0.0.3/src/fluidsimfoam/resources/__init__.py
--rw-r--r--   0        0        0      955 2023-05-09 13:02:39.537858 fluidsimfoam-0.0.3/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2765 2023-05-09 13:04:52.906067 fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__init__.py
--rw-r--r--   0        0        0     2620 2023-05-09 13:05:27.378825 fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1779 2023-05-09 12:51:06.182422 fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1857 2023-05-09 12:49:41.227234 fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/base.py
--rw-r--r--   0        0        0      714 2023-05-09 12:58:59.894982 fluidsimfoam-0.0.3/src/fluidsimfoam/tasks.py
--rw-r--r--   0        0        0       76 2023-05-09 12:51:03.050894 fluidsimfoam-0.0.3/src/fluidsimfoam/util/__init__.py
--rw-r--r--   0        0        0      238 2023-05-09 12:51:06.202419 fluidsimfoam-0.0.3/src/fluidsimfoam/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1145 2023-03-09 20:43:42.785643 fluidsimfoam-0.0.3/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
--rw-r--r--   0        0        0      861 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.3/src/fluidsimfoam/util/console.py
--rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-03-02 21:01:46.291446 fluidsimfoam-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4133 2023-05-12 11:29:14.677721 fluidsimfoam-0.0.4/README.md
+-rw-r--r--   0        0        0     1996 2023-05-22 20:03:53.584389 fluidsimfoam-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1966 2023-05-16 18:45:49.936442 fluidsimfoam-0.0.4/src/fluidsimfoam/__init__.py
+-rw-r--r--   0        0        0     3247 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__init__.py
+-rw-r--r--   0        0        0     3512 2023-05-22 18:59:45.209791 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    16673 2023-05-22 18:59:45.213791 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc
+-rw-r--r--   0        0        0     1795 2023-05-22 18:59:45.381794 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc
+-rw-r--r--   0        0        0     6520 2023-05-22 18:59:45.385794 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc
+-rw-r--r--   0        0        0     5005 2023-05-22 18:59:45.385794 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/fv_options.cpython-310.pyc
+-rw-r--r--   0        0        0     2752 2023-05-08 19:53:29.031102 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc
+-rw-r--r--   0        0        0     1844 2023-05-05 07:20:02.628943 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5361 2023-05-16 20:16:40.470447 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc
+-rw-r--r--   0        0        0    10473 2023-05-09 12:43:04.027476 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     1082 2023-05-03 21:01:43.908143 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc
+-rw-r--r--   0        0        0    16524 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/ast.py
+-rw-r--r--   0        0        0     1080 2023-04-23 15:48:42.099657 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE
+-rw-r--r--   0        0        0    14466 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py
+-rw-r--r--   0        0        0    15603 2023-05-22 18:59:45.381794 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2344 2023-05-05 07:26:24.618314 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc
+-rw-r--r--   0        0        0     3085 2023-05-05 07:26:24.622314 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc
+-rw-r--r--   0        0        0     1810 2023-04-24 21:00:31.761612 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/edges.py
+-rw-r--r--   0        0        0     3426 2023-04-24 20:58:16.942659 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/grading.py
+-rw-r--r--   0        0        0     1752 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/constant_files.py
+-rw-r--r--   0        0        0     6033 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/fields.py
+-rw-r--r--   0        0        0     6107 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/fv_options.py
+-rw-r--r--   0        0        0     2414 2023-05-08 19:04:20.598143 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/fv_schemes.py
+-rw-r--r--   0        0        0     5076 2023-05-16 18:45:49.936442 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/generators.py
+-rw-r--r--   0        0        0     1916 2023-05-16 18:45:49.936442 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/grammar.lark
+-rw-r--r--   0        0        0     2337 2023-05-16 18:45:49.940441 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/grammar_advanced.lark
+-rw-r--r--   0        0        0     9522 2023-05-09 12:42:41.039310 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/parser.py
+-rw-r--r--   0        0        0      973 2023-05-03 19:26:40.332634 fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/polymesh.py
+-rw-r--r--   0        0        0     1400 2023-05-09 20:05:14.235128 fluidsimfoam-0.0.4/src/fluidsimfoam/info.py
+-rw-r--r--   0        0        0      124 2023-05-09 13:01:28.476575 fluidsimfoam-0.0.4/src/fluidsimfoam/init_fields.py
+-rw-r--r--   0        0        0      747 2023-05-09 13:00:38.420124 fluidsimfoam-0.0.4/src/fluidsimfoam/log.py
+-rw-r--r--   0        0        0      608 2023-05-11 19:44:39.696948 fluidsimfoam-0.0.4/src/fluidsimfoam/make.py
+-rw-r--r--   0        0        0     1185 2023-05-09 12:57:19.118180 fluidsimfoam-0.0.4/src/fluidsimfoam/next_fluidsim_core.py
+-rw-r--r--   0        0        0     1210 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.4/src/fluidsimfoam/operators.py
+-rw-r--r--   0        0        0      154 2023-05-12 15:24:49.346320 fluidsimfoam-0.0.4/src/fluidsimfoam/output/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-12 15:24:54.098078 fluidsimfoam-0.0.4/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7823 2023-05-16 20:16:40.466447 fluidsimfoam-0.0.4/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1607 2023-05-12 15:28:21.593481 fluidsimfoam-0.0.4/src/fluidsimfoam/output/__pycache__/fields.cpython-310.pyc
+-rw-r--r--   0        0        0     5156 2023-05-16 20:16:40.490446 fluidsimfoam-0.0.4/src/fluidsimfoam/output/__pycache__/log.cpython-310.pyc
+-rw-r--r--   0        0        0     9574 2023-05-16 18:45:49.940441 fluidsimfoam-0.0.4/src/fluidsimfoam/output/base.py
+-rw-r--r--   0        0        0      958 2023-05-12 15:28:18.250001 fluidsimfoam-0.0.4/src/fluidsimfoam/output/fields.py
+-rw-r--r--   0        0        0     6370 2023-05-16 18:45:49.940441 fluidsimfoam-0.0.4/src/fluidsimfoam/output/log.py
+-rw-r--r--   0        0        0     2886 2023-05-22 18:56:58.339368 fluidsimfoam-0.0.4/src/fluidsimfoam/params.py
+-rw-r--r--   0        0        0      573 2023-05-09 13:02:35.270502 fluidsimfoam-0.0.4/src/fluidsimfoam/resources/__init__.py
+-rw-r--r--   0        0        0      955 2023-05-09 13:02:39.537858 fluidsimfoam-0.0.4/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2765 2023-05-09 13:04:52.906067 fluidsimfoam-0.0.4/src/fluidsimfoam/solvers/__init__.py
+-rw-r--r--   0        0        0     2620 2023-05-09 13:05:27.378825 fluidsimfoam-0.0.4/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2748 2023-05-11 19:45:07.074828 fluidsimfoam-0.0.4/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2908 2023-05-11 19:44:39.696948 fluidsimfoam-0.0.4/src/fluidsimfoam/solvers/base.py
+-rw-r--r--   0        0        0     2247 2023-05-22 18:56:58.339368 fluidsimfoam-0.0.4/src/fluidsimfoam/tasks.py
+-rw-r--r--   0        0        0     1611 2023-05-22 18:56:58.339368 fluidsimfoam-0.0.4/src/fluidsimfoam/testing.py
+-rw-r--r--   0        0        0       77 2023-05-09 20:05:14.251128 fluidsimfoam-0.0.4/src/fluidsimfoam/util/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-09 20:27:04.597492 fluidsimfoam-0.0.4/src/fluidsimfoam/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1145 2023-03-09 20:43:42.785643 fluidsimfoam-0.0.4/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
+-rw-r--r--   0        0        0      861 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.4/src/fluidsimfoam/util/console.py
+-rw-r--r--   0        0        0     5430 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.4/PKG-INFO
```

### Comparing `fluidsimfoam-0.0.3/LICENSE` & `fluidsimfoam-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/README.md` & `fluidsimfoam-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPI](https://img.shields.io/pypi/v/fluidsimfoam)](https://pypi.org/project/fluidsimfoam/)
 [![Documentation Status](https://readthedocs.org/projects/fluidsimfoam/badge/?version=latest)](https://fluidsimfoam.readthedocs.io/en/latest/?badge=latest)
 
 Python framework for [OpenFOAM]
 
 </div>
 
-<!-- badges -->
+<!-- start-intro -->
 
 [OpenFOAM] is a very popular open-source C++ CFD framework. Working with [OpenFOAM]
 implies writting and modifying a lot of input files describing a simulation.
 The method described in the official [OpenFOAM] documentations is to copy an
 existing simulation directory and to modify the input files by hand.
 Fluidsimfoam is a Python package designed to improve the life of [OpenFOAM]
 users.
@@ -41,31 +41,52 @@
 equivalent of [Snek5000], our Fluidsim framework for [Nek5000]. Looking at the
 [Snek5000] tutorials should give a good idea of what Fluidsimfoam will soon
 allow.
 
 For our examples, we currently target OpenFOAM v2206 but it should be possible
 to write Fluidsimfoam solvers targeting any recent OpenFOAM versions.
 
+[fluiddyn]: https://fluiddyn.readthedocs.io
+[fluidsim]: https://fluidsim.readthedocs.io
+[fluidfoam]: https://fluidfoam.readthedocs.io
+[fluidsimfoam-tgv]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-tgv
+[fluidsimfoam-cbox]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-cbox
+[fluidsimfoam-sed]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-sed
+[openfoam]: https://openfoam.org/
+[nek5000]: https://nek5000.mcs.anl.gov/
+[snek5000]: https://snek5000.readthedocs.io
+
+<!-- end-intro -->
+
 See more in [Fluidsimfoam documentation](https://fluidsimfoam.readthedocs.org).
 
 ## Install
 
+<!-- start-install -->
+
 Currently, it still makes sense to install Fluidsimfoam like we, the
 fluidsimfoam developers, install it, i.e. in a dedicated controlled virtual
 environment created by [Poetry]. After installing [Poetry] (for example with
 something like `pip install poetry`), the following commands should install and
 activate the virtual environment:
 
 ```sh
 hg clone https://foss.heptapod.net/fluiddyn/fluidsimfoam
 cd fluidsimfoam
 poetry install
 poetry shell
 ```
 
+For better user experience with Matplotlib figures, you can also install with
+`poetry install --extra qt`.
+
+[Poetry]: https://python-poetry.org/docs/
+
+<!-- end-install -->
+
 ## Related projects
 
 - [Fluidfoam] Another [Fluiddyn] package (like Fluidsimfoam) to use/plot OpenFOAM
   data. Will be used by Fluidsimfoam.
 
 - [PyFoam] ([PyPI package](https://pypi.org/project/PyFoam/),
   [hg repo](http://hg.code.sf.net/p/openfoam-extend/PyFoam)) Python utilities for
@@ -73,19 +94,9 @@
 
 - [PythonFlu] ([wiki](https://openfoamwiki.net/index.php/Contrib_pythonFlu))
 
 - [Swak4Foam] Popular set of utilities for OpenFOAM. Can be used in
   Fluidsimfoam solvers.
 
 [PyFoam]: https://openfoamwiki.net/index.php/Contrib/PyFoam
-[fluiddyn]: https://fluiddyn.readthedocs.io
-[fluidsim]: https://fluidsim.readthedocs.io
-[fluidfoam]: https://fluidfoam.readthedocs.io
-[fluidsimfoam-tgv]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-tgv
-[fluidsimfoam-cbox]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-cbox
-[fluidsimfoam-sed]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-sed
-[openfoam]: https://openfoam.org/
-[nek5000]: https://nek5000.mcs.anl.gov/
-[snek5000]: https://snek5000.readthedocs.io
 [PythonFlu]: http://pythonflu.wikidot.com/
 [Swak4Foam]: https://openfoamwiki.net/index.php/Contrib/swak4Foam
-[Poetry]: https://python-poetry.org/docs/
```

### Comparing `fluidsimfoam-0.0.3/pyproject.toml` & `fluidsimfoam-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluidsimfoam"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python framework for OpenFOAM"
 authors = ["pierre.augier <pierre.augier@univ-grenoble-alpes.fr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -13,20 +13,31 @@
 fluiddyn = "^0.5.2"
 ipython = "^8.11.0"
 pandas = "^1.5.3"
 jinja2 = "^3.1.2"
 lark = "^1.1.5"
 rich = "^13.3.3"
 invoke = "^2.0.0"
+PySide6 = {version = "^6.5.0", optional = true, python = ">=3.9,<3.12"}
+jupyterlab = {version = "^3.6.3", optional = true}
+jupyterlab_myst = {version = "^1.1.3", optional = true}
+jupytext = {version = "^1.14.5", optional = true}
+mdformat-myst = {version = "^0.1.4", optional = true}
+
+[tool.poetry.extras]
+qt = ["PySide6"]
+jupyter = ["jupyterlab", "jupyterlab_myst", "jupytext", "mdformat-myst"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 fluidsimfoam-tgv = { path = "./doc/examples/fluidsimfoam-tgv/", develop = true }
 fluidsimfoam-cbox = { path = "./doc/examples/fluidsimfoam-cbox/", develop = true }
 fluidsimfoam-sed = { path = "./doc/examples/fluidsimfoam-sed/", develop = true }
+fluidsimfoam-cavity = { path = "./doc/examples/fluidsimfoam-cavity/", develop = true }
+fluidsimfoam-phill = { path = "./doc/examples/fluidsimfoam-phill/", develop = true }
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/__init__.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,21 @@
 
    info
    make
    init_fields
    operators
    log
    tasks
+   testing
+   params
    next_fluidsim_core
 
 """
 import importlib.metadata
+import sys
 
 from fluidsimfoam.params import Parameters
 
 from .next_fluidsim_core import path_try_from_fluidsim_path
 
 __version__ = importlib.metadata.version(__package__ or __name__)
 __all__ = ["load", "load_simul", "load_params"]
@@ -82,7 +85,13 @@
 
     """
     path_dir = path_try_from_fluidsim_path(path_dir)
     return Parameters(path_file=path_dir / "params_simul.xml")
 
 
 load = load_simul
+
+
+if any("pytest" in part for part in sys.argv):
+    import pytest
+
+    pytest.register_assert_rewrite("fluidsimfoam.testing")
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 12:44:19 2023 UTC, .py size: 2195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,158 +1,220 @@
-00000000: 6f0d 0d0a 0000 0000 2340 5a64 9308 0000  o.......#@Zd....
+00000000: 6f0d 0d0a 0000 0000 faba 6b64 af0c 0000  o.........kd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0011 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
+00000020: 0011 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
-00000040: 0100 6403 6404 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
-00000050: 6d07 5a07 6d08 5a08 0100 6403 6405 6c09  m.Z.m.Z...d.d.l.
-00000060: 6d0a 5a0a 6d0b 5a0b 0100 6700 6406 a201  m.Z.m.Z...g.d...
-00000070: 5a0c 4700 6407 6408 8400 6408 6502 8303  Z.G.d.d...d.e...
-00000080: 5a0d 6409 5a0e 650e 6403 640a 8502 1900  Z.d.Z.e.d.d.....
-00000090: 5a0e 650f 640b 640c 6401 640d 640e 640f  Z.e.d.d.d.d.d.d.
-000000a0: 6410 6411 6401 6412 6413 6414 6415 6413  d.d.d.d.d.d.d.d.
-000000b0: 6416 6417 8d0f 5a10 6403 6418 6c11 6d12  d.d...Z.d.d.l.m.
-000000c0: 5a12 6d13 5a13 0100 6403 6419 6c14 6d15  Z.m.Z...d.d.l.m.
-000000d0: 5a15 0100 6403 641a 6c16 6d17 5a17 6d18  Z...d.d.l.m.Z.m.
-000000e0: 5a18 6d19 5a19 0100 6403 641b 6c1a 6d1b  Z.m.Z...d.d.l.m.
-000000f0: 5a1b 0100 641c 5300 291d 7af9 4f70 656e  Z...d.S.).z.Open
-00000100: 464f 414d 2069 6e70 7574 2066 696c 6573  FOAM input files
-00000110: 0a0a 2e2e 2072 7562 7269 633a 3a20 4153  .... rubric:: AS
-00000120: 5420 616e 6420 7061 7273 6572 0a0a 2e2e  T and parser....
-00000130: 2061 7574 6f73 756d 6d61 7279 3a3a 0a20   autosummary::. 
-00000140: 2020 3a74 6f63 7472 6565 3a0a 0a20 2020    :toctree:..   
-00000150: 2061 7374 0a20 2020 2067 656e 6572 6174   ast.    generat
-00000160: 6f72 730a 2020 2020 7061 7273 6572 0a0a  ors.    parser..
-00000170: 2e2e 2072 7562 7269 633a 3a20 4865 6c70  .. rubric:: Help
-00000180: 6572 2074 6f20 6372 6561 7465 2069 6e70  er to create inp
-00000190: 7574 2066 696c 6573 0a0a 2e2e 2061 7574  ut files.... aut
-000001a0: 6f73 756d 6d61 7279 3a3a 0a20 2020 3a74  osummary::.   :t
-000001b0: 6f63 7472 6565 3a0a 0a20 2020 2062 6c6f  octree:..    blo
-000001c0: 636b 6d65 7368 0a20 2020 2066 6965 6c64  ckmesh.    field
-000001d0: 730a 2020 2020 6676 5f73 6368 656d 6573  s.    fv_schemes
-000001e0: 0a20 2020 2063 6f6e 7374 616e 745f 6669  .    constant_fi
-000001f0: 6c65 730a 0ae9 0000 0000 2902 da03 4142  les.......)...AB
-00000200: 43da 0e61 6273 7472 6163 746d 6574 686f  C..abstractmetho
-00000210: 64e9 0100 0000 2904 da04 4469 6374 da0d  d.....)...Dict..
-00000220: 466f 616d 496e 7075 7446 696c 65da 044c  FoamInputFile..L
-00000230: 6973 74da 0556 616c 7565 2902 da04 6475  ist..Value)...du
-00000240: 6d70 da05 7061 7273 6529 0e72 0a00 0000  mp..parse).r....
-00000250: 7209 0000 0072 0600 0000 da0e 4445 4641  r....r......DEFA
-00000260: 554c 545f 4845 4144 4552 7205 0000 0072  ULT_HEADERr....r
-00000270: 0700 0000 7208 0000 00da 0d42 6c6f 636b  ....r......Block
-00000280: 4d65 7368 4469 6374 da0e 566f 6c53 6361  MeshDict..VolSca
-00000290: 6c61 7246 6965 6c64 da0e 566f 6c56 6563  larField..VolVec
-000002a0: 746f 7246 6965 6c64 da0f 4676 5363 6865  torField..FvSche
-000002b0: 6d65 7348 656c 7065 72da 0656 6572 7465  mesHelper..Verte
-000002c0: 78da 0f72 6561 645f 6669 656c 645f 6669  x..read_field_fi
-000002d0: 6c65 da0a 4669 6c65 4865 6c70 6572 6300  le..FileHelperc.
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000002f0: 0000 0040 0000 0073 2800 0000 6500 5a01  ...@...s(...e.Z.
-00000300: 6400 5a02 6401 5a03 6504 6402 6403 8400  d.Z.d.Z.e.d.d...
-00000310: 8301 5a05 6504 6404 6405 8400 8301 5a06  ..Z.e.d.d.....Z.
-00000320: 6406 5300 2907 7212 0000 007a 2341 6273  d.S.).r....z#Abs
-00000330: 7472 6163 7420 636c 6173 7320 666f 7220  tract class for 
-00000340: 2248 656c 7065 7222 206f 626a 6563 7473  "Helper" objects
-00000350: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000360: 0001 0000 0043 0000 00f3 0400 0000 6401  .....C........d.
-00000370: 5300 2902 7a1a 436f 6d70 6c65 7465 2074  S.).z.Complete t
-00000380: 6865 2070 6172 616d 7320 6f62 6a65 6374  he params object
-00000390: 4ea9 00a9 02da 0473 656c 66da 0670 6172  N......self..par
-000003a0: 616d 7372 1400 0000 7214 0000 00fa 4b2f  amsr....r.....K/
-000003b0: 686f 6d65 2f70 6965 7272 652f 4465 762f  home/pierre/Dev/
-000003c0: 666c 7569 6473 696d 666f 616d 2f73 7263  fluidsimfoam/src
-000003d0: 2f66 6c75 6964 7369 6d66 6f61 6d2f 666f  /fluidsimfoam/fo
-000003e0: 616d 5f69 6e70 7574 5f66 696c 6573 2f5f  am_input_files/_
-000003f0: 5f69 6e69 745f 5f2e 7079 da0f 636f 6d70  _init__.py..comp
-00000400: 6c65 7465 5f70 6172 616d 7331 0000 00f3  lete_params1....
-00000410: 0200 0000 0400 7a1a 4669 6c65 4865 6c70  ......z.FileHelp
-00000420: 6572 2e63 6f6d 706c 6574 655f 7061 7261  er.complete_para
-00000430: 6d73 6302 0000 0000 0000 0000 0000 0002  msc.............
-00000440: 0000 0001 0000 0043 0000 0072 1300 0000  .......C...r....
-00000450: 2902 7a24 4d61 6b65 2074 6865 2041 5354  ).z$Make the AST
-00000460: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
-00000470: 6f20 6120 6669 6c65 4e72 1400 0000 7215  o a fileNr....r.
-00000480: 0000 0072 1400 0000 7214 0000 0072 1800  ...r....r....r..
-00000490: 0000 da09 6d61 6b65 5f74 7265 6535 0000  ....make_tree5..
-000004a0: 0072 1a00 0000 7a14 4669 6c65 4865 6c70  .r....z.FileHelp
-000004b0: 6572 2e6d 616b 655f 7472 6565 4e29 07da  er.make_treeN)..
-000004c0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000004d0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000004e0: 655f 5fda 075f 5f64 6f63 5f5f 7203 0000  e__..__doc__r...
-000004f0: 0072 1900 0000 721b 0000 0072 1400 0000  .r....r....r....
-00000500: 7214 0000 0072 1400 0000 7218 0000 0072  r....r....r....r
-00000510: 1200 0000 2f00 0000 730c 0000 0008 0004  ..../...s.......
-00000520: 0102 010a 0102 030e 0172 1200 0000 6131  .........r....a1
-00000530: 0200 000a 2f2a 2d2d 2d2d 2d2d 2d2d 2d2d  ..../*----------
-00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000550: 2d2d 2d2d 2d2d 2a2d 2043 2b2b 202d 2a2d  ------*- C++ -*-
-00000560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000580: 2d2a 5c0a 7c20 3d3d 3d3d 3d3d 3d3d 3d20  -*\.| ========= 
-00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000005b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005d0: 2020 7c0a 7c20 5c5c 2020 2020 2020 2f20    |.| \\      / 
-000005e0: 2046 2069 656c 6420 2020 2020 2020 2020   F ield         
-000005f0: 7c20 4f70 656e 464f 414d 3a20 5468 6520  | OpenFOAM: The 
-00000600: 4f70 656e 2053 6f75 7263 6520 4346 4420  Open Source CFD 
-00000610: 546f 6f6c 626f 7820 2020 2020 2020 2020  Toolbox         
-00000620: 2020 7c0a 7c20 205c 5c20 2020 202f 2020    |.|  \\    /  
-00000630: 204f 2070 6572 6174 696f 6e20 2020 2020   O peration     
-00000640: 7c20 5665 7273 696f 6e3a 2020 7632 3230  | Version:  v220
-00000650: 3620 2020 2020 2020 2020 2020 2020 2020  6               
-00000660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000670: 2020 7c0a 7c20 2020 5c5c 2020 2f20 2020    |.|   \\  /   
-00000680: 2041 206e 6420 2020 2020 2020 2020 2020   A nd           
-00000690: 7c20 5765 6273 6974 653a 2020 7777 772e  | Website:  www.
-000006a0: 6f70 656e 666f 616d 2e63 6f6d 2020 2020  openfoam.com    
-000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006c0: 2020 7c0a 7c20 2020 205c 5c2f 2020 2020    |.|    \\/    
-000006d0: 204d 2061 6e69 7075 6c61 7469 6f6e 2020   M anipulation  
-000006e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000710: 2020 7c0a 5c2a 2d2d 2d2d 2d2d 2d2d 2d2d    |.\*----------
-00000720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000760: 2d2a 2f0a e9ff ffff ff5a 0769 636f 466f  -*/......Z.icoFo
-00000770: 616d da09 7374 6172 7454 696d 65da 0765  am..startTime..e
-00000780: 6e64 5469 6d65 6700 0000 0000 00e0 3f67  ndTimeg.......?g
-00000790: 7b14 ae47 e17a 743f 5a08 7469 6d65 5374  {..G.zt?Z.timeSt
-000007a0: 6570 e914 0000 00da 0561 7363 6969 e906  ep.......ascii..
-000007b0: 0000 00da 036f 6666 da07 6765 6e65 7261  .....off..genera
-000007c0: 6cda 0474 7275 6529 0fda 0b61 7070 6c69  l..true)...appli
-000007d0: 6361 7469 6f6e 5a09 7374 6172 7446 726f  cationZ.startFro
-000007e0: 6d72 2100 0000 5a06 7374 6f70 4174 7222  mr!...Z.stopAtr"
-000007f0: 0000 005a 0664 656c 7461 545a 0c77 7269  ...Z.deltaTZ.wri
-00000800: 7465 436f 6e74 726f 6c5a 0d77 7269 7465  teControlZ.write
-00000810: 496e 7465 7276 616c 5a0a 7075 7267 6557  IntervalZ.purgeW
-00000820: 7269 7465 5a0b 7772 6974 6546 6f72 6d61  riteZ.writeForma
-00000830: 745a 0e77 7269 7465 5072 6563 6973 696f  tZ.writePrecisio
-00000840: 6e5a 1077 7269 7465 436f 6d70 7265 7373  nZ.writeCompress
-00000850: 696f 6e5a 0a74 696d 6546 6f72 6d61 745a  ionZ.timeFormatZ
-00000860: 0d74 696d 6550 7265 6369 7369 6f6e 5a11  .timePrecisionZ.
-00000870: 7275 6e54 696d 654d 6f64 6966 6961 626c  runTimeModifiabl
-00000880: 6529 0272 0c00 0000 7210 0000 0029 01da  e).r....r....)..
-00000890: 1243 6f6e 7374 616e 7446 696c 6548 656c  .ConstantFileHel
-000008a0: 7065 7229 0372 0d00 0000 720e 0000 0072  per).r....r....r
-000008b0: 1100 0000 2901 720f 0000 004e 291c 721f  ....).r....N).r.
-000008c0: 0000 00da 0361 6263 7202 0000 0072 0300  .....abcr....r..
-000008d0: 0000 da03 6173 7472 0500 0000 7206 0000  ....astr....r...
-000008e0: 0072 0700 0000 7208 0000 00da 0670 6172  .r....r......par
-000008f0: 7365 7272 0900 0000 720a 0000 00da 075f  serr....r......_
-00000900: 5f61 6c6c 5f5f 7212 0000 0072 0b00 0000  _all__r....r....
-00000910: da04 6469 6374 5a14 4445 4641 554c 545f  ..dictZ.DEFAULT_
-00000920: 434f 4e54 524f 4c5f 4449 4354 5a09 626c  CONTROL_DICTZ.bl
-00000930: 6f63 6b6d 6573 6872 0c00 0000 7210 0000  ockmeshr....r...
-00000940: 005a 0e63 6f6e 7374 616e 745f 6669 6c65  .Z.constant_file
-00000950: 7372 2a00 0000 da06 6669 656c 6473 720d  sr*.....fieldsr.
-00000960: 0000 0072 0e00 0000 7211 0000 005a 0a66  ...r....r....Z.f
-00000970: 765f 7363 6865 6d65 7372 0f00 0000 7214  v_schemesr....r.
-00000980: 0000 0072 1400 0000 7214 0000 0072 1800  ...r....r....r..
-00000990: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000009a0: 733a 0000 0004 0010 1718 0210 0108 0210  s:..............
-000009b0: 1204 0b0c 0a02 0302 0102 0102 0102 0102  ................
-000009c0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-000009d0: 0102 0102 0106 f110 120c 0114 0110 01    ...............
+00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6404  ..d.d.l.m.Z...d.
+00000050: 6405 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
+00000060: 6d0a 5a0a 6d0b 5a0b 0100 6404 6406 6c0c  m.Z.m.Z...d.d.l.
+00000070: 6d0d 5a0d 6d0e 5a0e 0100 6700 6407 a201  m.Z.m.Z...g.d...
+00000080: 5a0f 6408 6409 8400 5a10 640a 640b 8400  Z.d.d...Z.d.d...
+00000090: 5a11 6425 640d 640e 8401 5a12 4700 640f  Z.d%d.d...Z.G.d.
+000000a0: 6410 8400 6410 6502 8303 5a13 6411 5a14  d...d.e...Z.d.Z.
+000000b0: 6514 6404 6412 8502 1900 5a14 6515 6413  e.d.d.....Z.e.d.
+000000c0: 6414 6401 6415 6416 6417 6418 6419 6401  d.d.d.d.d.d.d.d.
+000000d0: 641a 641b 641c 641d 641b 641e 641f 8d0f  d.d.d.d.d.d.d...
+000000e0: 5a16 6404 6420 6c17 6d18 5a18 6d19 5a19  Z.d.d l.m.Z.m.Z.
+000000f0: 6d1a 5a1a 0100 6404 6421 6c1b 6d1c 5a1c  m.Z...d.d!l.m.Z.
+00000100: 0100 6404 6422 6c1d 6d1e 5a1e 6d1f 5a1f  ..d.d"l.m.Z.m.Z.
+00000110: 6d20 5a20 0100 6404 6423 6c21 6d22 5a22  m Z ..d.d#l!m"Z"
+00000120: 0100 6404 6424 6c23 6d24 5a24 0100 640c  ..d.d$l#m$Z$..d.
+00000130: 5300 2926 6108 0100 004f 7065 6e46 4f41  S.)&a....OpenFOA
+00000140: 4d20 696e 7075 7420 6669 6c65 730a 0a2e  M input files...
+00000150: 2e20 7275 6272 6963 3a3a 2041 5354 2061  . rubric:: AST a
+00000160: 6e64 2070 6172 7365 720a 0a2e 2e20 6175  nd parser.... au
+00000170: 746f 7375 6d6d 6172 793a 3a0a 2020 203a  tosummary::.   :
+00000180: 746f 6374 7265 653a 0a0a 2020 2020 6173  toctree:..    as
+00000190: 740a 2020 2020 6765 6e65 7261 746f 7273  t.    generators
+000001a0: 0a20 2020 2070 6172 7365 720a 0a2e 2e20  .    parser.... 
+000001b0: 7275 6272 6963 3a3a 2048 656c 7065 7220  rubric:: Helper 
+000001c0: 746f 2063 7265 6174 6520 696e 7075 7420  to create input 
+000001d0: 6669 6c65 730a 0a2e 2e20 6175 746f 7375  files.... autosu
+000001e0: 6d6d 6172 793a 3a0a 2020 203a 746f 6374  mmary::.   :toct
+000001f0: 7265 653a 0a0a 2020 2020 626c 6f63 6b6d  ree:..    blockm
+00000200: 6573 680a 2020 2020 6669 656c 6473 0a20  esh.    fields. 
+00000210: 2020 2066 765f 7363 6865 6d65 730a 2020     fv_schemes.  
+00000220: 2020 636f 6e73 7461 6e74 5f66 696c 6573    constant_files
+00000230: 0a20 2020 2066 765f 6f70 7469 6f6e 730a  .    fv_options.
+00000240: 0ae9 0000 0000 2902 da03 4142 43da 0e61  ......)...ABC..a
+00000250: 6273 7472 6163 746d 6574 686f 6429 01da  bstractmethod)..
+00000260: 0a75 6e64 6572 7363 6f72 65e9 0100 0000  .underscore.....
+00000270: 2905 da04 4469 6374 da0c 4469 6d65 6e73  )...Dict..Dimens
+00000280: 696f 6e53 6574 da0d 466f 616d 496e 7075  ionSet..FoamInpu
+00000290: 7446 696c 65da 044c 6973 74da 0556 616c  tFile..List..Val
+000002a0: 7565 2902 da04 6475 6d70 da05 7061 7273  ue)...dump..pars
+000002b0: 6529 1272 0c00 0000 720b 0000 0072 0800  e).r....r....r..
+000002c0: 0000 da0e 4445 4641 554c 545f 4845 4144  ....DEFAULT_HEAD
+000002d0: 4552 7206 0000 0072 0900 0000 720a 0000  ERr....r....r...
+000002e0: 00da 0d42 6c6f 636b 4d65 7368 4469 6374  ...BlockMeshDict
+000002f0: da0e 566f 6c53 6361 6c61 7246 6965 6c64  ..VolScalarField
+00000300: da0e 566f 6c56 6563 746f 7246 6965 6c64  ..VolVectorField
+00000310: da0f 4676 5363 6865 6d65 7348 656c 7065  ..FvSchemesHelpe
+00000320: 72da 0656 6572 7465 78da 0f72 6561 645f  r..Vertex..read_
+00000330: 6669 656c 645f 6669 6c65 da0a 4669 6c65  field_file..File
+00000340: 4865 6c70 6572 da12 436f 6e73 7461 6e74  Helper..Constant
+00000350: 4669 6c65 4865 6c70 6572 da18 426c 6f63  FileHelper..Bloc
+00000360: 6b4d 6573 6844 6963 7452 6563 7469 6c69  kMeshDictRectili
+00000370: 6e65 6172 da0f 4676 4f70 7469 6f6e 7348  near..FvOptionsH
+00000380: 656c 7065 7272 0700 0000 6301 0000 0000  elperr....c.....
+00000390: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+000003a0: 0000 0073 1000 0000 7400 7c00 8301 a001  ...s....t.|.....
+000003b0: 6401 6402 a102 5300 2903 4eda 012e da01  d.d...S.).N.....
+000003c0: 5f29 0272 0400 0000 da07 7265 706c 6163  _).r......replac
+000003d0: 6529 01da 046e 616d 65a9 0072 1c00 0000  e)...name..r....
+000003e0: fa4b 2f68 6f6d 652f 7069 6572 7265 2f44  .K/home/pierre/D
+000003f0: 6576 2f66 6c75 6964 7369 6d66 6f61 6d2f  ev/fluidsimfoam/
+00000400: 7372 632f 666c 7569 6473 696d 666f 616d  src/fluidsimfoam
+00000410: 2f66 6f61 6d5f 696e 7075 745f 6669 6c65  /foam_input_file
+00000420: 732f 5f5f 696e 6974 5f5f 2e70 79da 0b5f  s/__init__.py.._
+00000430: 6173 5f70 795f 6e61 6d65 3600 0000 7302  as_py_name6...s.
+00000440: 0000 0010 0172 1e00 0000 6302 0000 0000  .....r....c.....
+00000450: 0000 0000 0000 0006 0000 000a 0000 0043  ...............C
+00000460: 0000 0073 6000 0000 7c00 a000 a100 4400  ...s`...|.....D.
+00000470: 5d29 5c02 7d02 7d03 7401 7c02 8301 7d04  ])\.}.}.t.|...}.
+00000480: 7a06 7c01 7c04 1900 7d05 5700 6e0b 0400  z.|.|...}.W.n...
+00000490: 7402 7403 6602 791d 0100 0100 0100 5900  t.t.f.y.......Y.
+000004a0: 7104 7700 7404 7c03 7405 8302 7229 7406  q.w.t.|.t...r)t.
+000004b0: 7c03 7c05 8302 0100 7104 7c05 7c00 7c02  |.|.....q.|.|.|.
+000004c0: 3c00 7104 6400 5300 a901 4e29 07da 0569  <.q.d.S...N)...i
+000004d0: 7465 6d73 7204 0000 00da 084b 6579 4572  temsr......KeyEr
+000004e0: 726f 72da 0e41 7474 7269 6275 7465 4572  ror..AttributeEr
+000004f0: 726f 72da 0a69 7369 6e73 7461 6e63 65da  ror..isinstance.
+00000500: 0464 6963 74da 185f 7570 6461 7465 5f64  .dict.._update_d
+00000510: 6963 745f 7769 7468 5f70 6172 616d 7329  ict_with_params)
+00000520: 06da 0464 6174 615a 0b70 6172 616d 735f  ...dataZ.params_
+00000530: 6461 7461 da03 6b65 79da 0576 616c 7565  data..key..value
+00000540: 721b 0000 005a 0b70 6172 616d 5f76 616c  r....Z.param_val
+00000550: 7565 721c 0000 0072 1c00 0000 721d 0000  uer....r....r...
+00000560: 0072 2500 0000 3a00 0000 7316 0000 0010  .r%...:...s.....
+00000570: 0108 0102 020c 0110 0104 0102 ff0a 030c  ................
+00000580: 010a 0204 f572 2500 0000 4e63 0400 0000  .....r%...Nc....
+00000590: 0000 0000 0000 0000 0700 0000 0500 0000  ................
+000005a0: 4300 0000 7354 0000 0074 007c 0183 017d  C...sT...t.|...}
+000005b0: 017c 006a 017c 017c 0364 018d 027d 047c  .|.j.|.|.d...}.|
+000005c0: 02a0 02a1 0044 005d 185c 027d 057d 0674  .....D.].\.}.}.t
+000005d0: 037c 0674 0483 0272 1f74 057c 047c 057c  .|.t...r.t.|.|.|
+000005e0: 0683 0301 0071 0f7c 04a0 0674 007c 0583  .....q.|...t.|..
+000005f0: 017c 06a1 0201 0071 0f64 0053 0029 024e  .|.....q.d.S.).N
+00000600: 2901 da03 646f 6329 0772 1e00 0000 da0a  )...doc).r......
+00000610: 5f73 6574 5f63 6869 6c64 7220 0000 0072  _set_childr ...r
+00000620: 2300 0000 7224 0000 00da 155f 636f 6d70  #...r$....._comp
+00000630: 6c65 7465 5f70 6172 616d 735f 6469 6374  lete_params_dict
+00000640: da0b 5f73 6574 5f61 7474 7269 6229 07da  .._set_attrib)..
+00000650: 0973 7562 7061 7261 6d73 721b 0000 00da  .subparamsr.....
+00000660: 0764 6566 6175 6c74 7229 0000 005a 0c73  .defaultr)...Z.s
+00000670: 7562 7375 6270 6172 616d 7372 2700 0000  ubsubparamsr'...
+00000680: 7228 0000 0072 1c00 0000 721c 0000 0072  r(...r....r....r
+00000690: 1d00 0000 722b 0000 0049 0000 0073 1000  ....r+...I...s..
+000006a0: 0000 0801 0e01 1002 0a01 0c01 0201 1202  ................
+000006b0: 04fb 722b 0000 0063 0000 0000 0000 0000  ..r+...c........
+000006c0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+000006d0: 7328 0000 0065 005a 0164 005a 0264 015a  s(...e.Z.d.Z.d.Z
+000006e0: 0365 0464 0264 0384 0083 015a 0565 0464  .e.d.d.....Z.e.d
+000006f0: 0464 0584 0083 015a 0664 0653 0029 0772  .d.....Z.d.S.).r
+00000700: 1400 0000 7a23 4162 7374 7261 6374 2063  ....z#Abstract c
+00000710: 6c61 7373 2066 6f72 2022 4865 6c70 6572  lass for "Helper
+00000720: 2220 6f62 6a65 6374 7363 0200 0000 0000  " objectsc......
+00000730: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+00000740: 0000 f304 0000 0064 0153 0029 027a 1a43  .......d.S.).z.C
+00000750: 6f6d 706c 6574 6520 7468 6520 7061 7261  omplete the para
+00000760: 6d73 206f 626a 6563 744e 721c 0000 00a9  ms objectNr.....
+00000770: 02da 0473 656c 66da 0670 6172 616d 7372  ...self..paramsr
+00000780: 1c00 0000 721c 0000 0072 1d00 0000 da0f  ....r....r......
+00000790: 636f 6d70 6c65 7465 5f70 6172 616d 7358  complete_paramsX
+000007a0: 0000 00f3 0200 0000 0400 7a1a 4669 6c65  ..........z.File
+000007b0: 4865 6c70 6572 2e63 6f6d 706c 6574 655f  Helper.complete_
+000007c0: 7061 7261 6d73 6302 0000 0000 0000 0000  paramsc.........
+000007d0: 0000 0002 0000 0001 0000 0043 0000 0072  ...........C...r
+000007e0: 2f00 0000 2902 7a24 4d61 6b65 2074 6865  /...).z$Make the
+000007f0: 2041 5354 2063 6f72 7265 7370 6f6e 6469   AST correspondi
+00000800: 6e67 2074 6f20 6120 6669 6c65 4e72 1c00  ng to a fileNr..
+00000810: 0000 7230 0000 0072 1c00 0000 721c 0000  ..r0...r....r...
+00000820: 0072 1d00 0000 da09 6d61 6b65 5f74 7265  .r......make_tre
+00000830: 655c 0000 0072 3400 0000 7a14 4669 6c65  e\...r4...z.File
+00000840: 4865 6c70 6572 2e6d 616b 655f 7472 6565  Helper.make_tree
+00000850: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000860: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000870: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000880: 7203 0000 0072 3300 0000 7235 0000 0072  r....r3...r5...r
+00000890: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
+000008a0: 0000 0072 1400 0000 5500 0000 730c 0000  ...r....U...s...
+000008b0: 0008 0004 0102 020a 0102 030e 0172 1400  .............r..
+000008c0: 0000 6131 0200 000a 2f2a 2d2d 2d2d 2d2d  ..a1..../*------
+000008d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2a2d 2043 2b2b  ----------*- C++
+000008f0: 202d 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   -*-------------
+00000900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000910: 2d2d 2d2d 2d2a 5c0a 7c20 3d3d 3d3d 3d3d  -----*\.| ======
+00000920: 3d3d 3d20 2020 2020 2020 2020 2020 2020  ===             
+00000930: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000960: 2020 2020 2020 7c0a 7c20 5c5c 2020 2020        |.| \\    
+00000970: 2020 2f20 2046 2069 656c 6420 2020 2020    /  F ield     
+00000980: 2020 2020 7c20 4f70 656e 464f 414d 3a20      | OpenFOAM: 
+00000990: 5468 6520 4f70 656e 2053 6f75 7263 6520  The Open Source 
+000009a0: 4346 4420 546f 6f6c 626f 7820 2020 2020  CFD Toolbox     
+000009b0: 2020 2020 2020 7c0a 7c20 205c 5c20 2020        |.|  \\   
+000009c0: 202f 2020 204f 2070 6572 6174 696f 6e20   /   O peration 
+000009d0: 2020 2020 7c20 5665 7273 696f 6e3a 2020      | Version:  
+000009e0: 7632 3230 3620 2020 2020 2020 2020 2020  v2206           
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 2020 2020 2020 7c0a 7c20 2020 5c5c 2020        |.|   \\  
+00000a10: 2f20 2020 2041 206e 6420 2020 2020 2020  /    A nd       
+00000a20: 2020 2020 7c20 5765 6273 6974 653a 2020      | Website:  
+00000a30: 7777 772e 6f70 656e 666f 616d 2e63 6f6d  www.openfoam.com
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2020 2020 2020 7c0a 7c20 2020 205c 5c2f        |.|    \\/
+00000a60: 2020 2020 204d 2061 6e69 7075 6c61 7469       M anipulati
+00000a70: 6f6e 2020 7c20 2020 2020 2020 2020 2020  on  |           
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 7c0a 5c2a 2d2d 2d2d 2d2d        |.\*------
+00000ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000af0: 2d2d 2d2d 2d2a 2f0a e9ff ffff ff5a 0769  -----*/......Z.i
+00000b00: 636f 466f 616d da09 7374 6172 7454 696d  coFoam..startTim
+00000b10: 65da 0765 6e64 5469 6d65 6700 0000 0000  e..endTimeg.....
+00000b20: 00e0 3f67 7b14 ae47 e17a 743f 5a08 7469  ..?g{..G.zt?Z.ti
+00000b30: 6d65 5374 6570 e914 0000 00da 0561 7363  meStep.......asc
+00000b40: 6969 e906 0000 00da 036f 6666 da07 6765  ii.......off..ge
+00000b50: 6e65 7261 6cda 0474 7275 6529 0fda 0b61  neral..true)...a
+00000b60: 7070 6c69 6361 7469 6f6e 5a09 7374 6172  pplicationZ.star
+00000b70: 7446 726f 6d72 3b00 0000 5a06 7374 6f70  tFromr;...Z.stop
+00000b80: 4174 723c 0000 005a 0664 656c 7461 545a  Atr<...Z.deltaTZ
+00000b90: 0c77 7269 7465 436f 6e74 726f 6c5a 0d77  .writeControlZ.w
+00000ba0: 7269 7465 496e 7465 7276 616c 5a0a 7075  riteIntervalZ.pu
+00000bb0: 7267 6557 7269 7465 5a0b 7772 6974 6546  rgeWriteZ.writeF
+00000bc0: 6f72 6d61 745a 0e77 7269 7465 5072 6563  ormatZ.writePrec
+00000bd0: 6973 696f 6e5a 1077 7269 7465 436f 6d70  isionZ.writeComp
+00000be0: 7265 7373 696f 6e5a 0a74 696d 6546 6f72  ressionZ.timeFor
+00000bf0: 6d61 745a 0d74 696d 6550 7265 6369 7369  matZ.timePrecisi
+00000c00: 6f6e 5a11 7275 6e54 696d 654d 6f64 6966  onZ.runTimeModif
+00000c10: 6961 626c 6529 0372 0e00 0000 7216 0000  iable).r....r...
+00000c20: 0072 1200 0000 2901 7215 0000 0029 0372  .r....).r....).r
+00000c30: 0f00 0000 7210 0000 0072 1300 0000 2901  ....r....r....).
+00000c40: 7217 0000 0029 0172 1100 0000 721f 0000  r....).r....r...
+00000c50: 0029 2572 3900 0000 da03 6162 6372 0200  .)%r9.....abcr..
+00000c60: 0000 7203 0000 005a 0a69 6e66 6c65 6374  ..r....Z.inflect
+00000c70: 696f 6e72 0400 0000 da03 6173 7472 0600  ionr......astr..
+00000c80: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00000c90: 0072 0a00 0000 da06 7061 7273 6572 720b  .r......parserr.
+00000ca0: 0000 0072 0c00 0000 da07 5f5f 616c 6c5f  ...r......__all_
+00000cb0: 5f72 1e00 0000 7225 0000 0072 2b00 0000  _r....r%...r+...
+00000cc0: 7214 0000 0072 0d00 0000 7224 0000 005a  r....r....r$...Z
+00000cd0: 1444 4546 4155 4c54 5f43 4f4e 5452 4f4c  .DEFAULT_CONTROL
+00000ce0: 5f44 4943 545a 0962 6c6f 636b 6d65 7368  _DICTZ.blockmesh
+00000cf0: 720e 0000 0072 1600 0000 7212 0000 005a  r....r....r....Z
+00000d00: 0e63 6f6e 7374 616e 745f 6669 6c65 7372  .constant_filesr
+00000d10: 1500 0000 da06 6669 656c 6473 720f 0000  ......fieldsr...
+00000d20: 0072 1000 0000 7213 0000 005a 0a66 765f  .r....r....Z.fv_
+00000d30: 6f70 7469 6f6e 7372 1700 0000 5a0a 6676  optionsr....Z.fv
+00000d40: 5f73 6368 656d 6573 7211 0000 0072 1c00  _schemesr....r..
+00000d50: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000d60: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000d70: 4400 0000 0400 1018 0c02 1c02 1001 0802  D...............
+00000d80: 0816 0804 0a0f 100c 040c 0c0a 0203 0201  ................
+00000d90: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000da0: 0201 0201 0201 0201 0201 0201 06f1 1412  ................
+00000db0: 0c01 1401 0c01 1001                      ........
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 12:44:45 2023 UTC, .py size: 15046 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,970 +1,1043 @@
-00000000: 6f0d 0d0a 0000 0000 3d40 5a64 c63a 0000  o.......=@Zd.:..
+00000000: 6f0d 0d0a 0000 0000 faba 6b64 8c40 0000  o.........kd.@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 8601 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 8e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
-00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
-00000080: 6d0e 5a0e 0100 6700 6409 a201 5a0f 640a  m.Z...g.d...Z.d.
-00000090: 640b 8400 5a10 640c 640d 8400 5a11 642e  d...Z.d.d...Z.d.
-000000a0: 640f 6410 8401 5a12 4700 6411 6412 8400  d.d...Z.G.d.d...
-000000b0: 6412 8302 5a13 4700 6413 6414 8400 6414  d...Z.G.d.d...d.
-000000c0: 6503 8303 5a14 4700 6415 6416 8400 6416  e...Z.G.d.d...d.
-000000d0: 6513 6514 8304 5a15 6506 4700 6417 6418  e.e...Z.e.G.d.d.
-000000e0: 8400 6418 8302 8301 5a16 4700 6419 641a  ..d.....Z.G.d.d.
-000000f0: 8400 641a 6516 8303 5a17 6506 4700 641b  ..d.e...Z.e.G.d.
-00000100: 641c 8400 641c 6513 8303 8301 5a18 4700  d...d.e.....Z.G.
-00000110: 641d 641e 8400 641e 6519 6513 8304 5a1a  d.d...d.e.e...Z.
-00000120: 4700 641f 6420 8400 6420 651b 6513 6514  G.d.d ..d e.e.e.
-00000130: 8305 5a1c 4700 6421 6422 8400 6422 6519  ..Z.G.d!d"..d"e.
-00000140: 6513 8304 5a1d 4700 6423 6424 8400 6424  e...Z.G.d#d$..d$
-00000150: 651c 8303 5a1e 6425 6426 8400 5a1f 6427  e...Z.d%d&..Z.d'
-00000160: 4400 5d0c 5a20 6521 651e 650e 6520 8301  D.].Z e!e.e.e ..
-00000170: 651f 6520 8301 8303 0100 719a 4700 6428  e.e ......q.G.d(
-00000180: 6429 8400 6429 6513 8303 5a22 6506 4700  d)..d)e...Z"e.G.
-00000190: 642a 642b 8400 642b 6513 8303 8301 5a23  d*d+..d+e.....Z#
-000001a0: 4700 642c 642d 8400 642d 6513 8303 5a24  G.d,d-..d-e...Z$
-000001b0: 6402 5300 292f 7a2e 4162 7374 7261 6374  d.S.)/z.Abstract
-000001c0: 2053 796e 7461 7820 5472 6565 7320 666f   Syntax Trees fo
-000001d0: 7220 4f70 656e 464f 414d 2069 6e70 7574  r OpenFOAM input
-000001e0: 2066 696c 6573 e900 0000 004e 2902 da03   files.....N)...
-000001f0: 4142 43da 0e61 6273 7472 6163 746d 6574  ABC..abstractmet
-00000200: 686f 6429 01da 0964 6174 6163 6c61 7373  hod)...dataclass
-00000210: 2901 da06 4e75 6d62 6572 2901 da06 6465  )...Number)...de
-00000220: 6465 6e74 2901 da08 4f70 7469 6f6e 616c  dent)...Optional
-00000230: 2901 da0a 756e 6465 7273 636f 7265 2907  )...underscore).
-00000240: da02 6b67 da01 6dda 0173 da01 4b5a 046b  ..kg..m..s..KZ.k
-00000250: 6d6f 6cda 0141 da02 6364 6301 0000 0000  mol..A..cdc.....
-00000260: 0000 0000 0000 0009 0000 0008 0000 0043  ...............C
-00000270: 0000 0073 d600 0000 6401 6701 6402 1400  ...s....d.g.d...
-00000280: 7d01 6403 7d02 7c00 7269 7a0a 7400 a001  }.d.}.|.riz.t...
-00000290: 6404 7c00 a102 a002 a100 7d03 5700 6e0f  d.|.......}.W.n.
-000002a0: 0400 7403 7922 0100 0100 0100 7c00 7d04  ..t.y"......|.}.
-000002b0: 6405 7d00 6406 7d05 5900 6e19 7700 7c00  d.}.d.}.Y.n.w.|.
-000002c0: 7c03 1900 7d05 7c05 6407 7600 732d 4a00  |...}.|.d.v.s-J.
-000002d0: 8201 7c00 6400 7c03 8502 1900 7d04 7c00  ..|.d.|.....}.|.
-000002e0: 7c03 6403 1700 6400 8502 1900 7d00 6408  |.d...d.....}.d.
-000002f0: 7c04 7600 724b 7c04 a004 6408 a101 5c02  |.v.rK|...d...\.
-00000300: 7d06 7d07 7405 7c07 8301 7d07 6e05 7c04  }.}.t.|...}.n.|.
-00000310: 6403 0202 7d06 7d07 7c06 6409 6b03 725f  d...}.}.|.d.k.r_
-00000320: 7406 a007 7c06 a101 7d08 7c02 7c07 1400  t...|...}.|.|...
-00000330: 7c01 7c08 3c00 7c05 6406 6b02 7265 6403  |.|.<.|.d.k.red.
-00000340: 6e01 640a 7d02 7c00 7309 7c01 5300 290b  n.d.}.|.s.|.S.).
-00000350: 4e72 0100 0000 e907 0000 00e9 0100 0000  Nr..............
-00000360: 7a04 5b2f 2e5d da00 da01 2e7a 022f 2efa  z.[/.].....z./..
-00000370: 015e da01 31e9 ffff ffff 2908 da02 7265  .^..1.....)...re
-00000380: da06 7365 6172 6368 da05 7374 6172 74da  ..search..start.
-00000390: 0e41 7474 7269 6275 7465 4572 726f 72da  .AttributeError.
-000003a0: 0573 706c 6974 da03 696e 74da 0773 796d  .split..int..sym
-000003b0: 626f 6c73 da05 696e 6465 7829 09da 0575  bols..index)...u
-000003c0: 6e69 7473 da06 7265 7375 6c74 da04 7369  nits..result..si
-000003d0: 676e 721d 0000 005a 0875 6e69 745f 616c  gnr....Z.unit_al
-000003e0: 6c5a 096e 6578 745f 6f70 6572 da09 756e  lZ.next_oper..un
-000003f0: 6974 5f6e 616d 655a 0a75 6e69 745f 7661  it_nameZ.unit_va
-00000400: 6c75 655a 0a75 6e69 745f 696e 6465 78a9  lueZ.unit_index.
-00000410: 0072 2200 0000 fa46 2f68 6f6d 652f 7069  .r"....F/home/pi
-00000420: 6572 7265 2f44 6576 2f66 6c75 6964 7369  erre/Dev/fluidsi
-00000430: 6d66 6f61 6d2f 7372 632f 666c 7569 6473  mfoam/src/fluids
-00000440: 696d 666f 616d 2f66 6f61 6d5f 696e 7075  imfoam/foam_inpu
-00000450: 745f 6669 6c65 732f 6173 742e 7079 da0e  t_files/ast.py..
-00000460: 7374 7232 666f 616d 5f75 6e69 7473 0f00  str2foam_units..
-00000470: 0000 7330 0000 000a 0104 0104 0102 0114  ..s0............
-00000480: 010c 0104 0104 0108 0102 fd08 050c 010c  ................
-00000490: 0110 0108 010e 010a 010a 0208 010a 010c  ................
-000004a0: 0110 0104 ec04 1572 2400 0000 6301 0000  .......r$...c...
-000004b0: 0000 0000 0000 0000 0005 0000 0008 0000  ................
-000004c0: 0043 0000 0073 a800 0000 6700 7d01 7400  .C...s....g.}.t.
-000004d0: 7401 7c00 8302 4400 5d2f 5c02 7d02 7d03  t.|...D.]/\.}.}.
-000004e0: 7c03 6401 6b02 7210 7107 7c03 6401 6b04  |.d.k.r.q.|.d.k.
-000004f0: 7216 6402 6e01 6403 7d04 7402 7c03 8301  r.d.n.d.}.t.|...
-00000500: 6404 6b02 7228 7c01 a003 7c04 9b00 7c02  d.k.r(|...|...|.
-00000510: 9b00 9d02 a101 0100 7107 7c01 a003 7c04  ........q.|...|.
-00000520: 9b00 7c02 9b00 6405 7402 7c03 8301 9b00  ..|...d.t.|.....
-00000530: 9d04 a101 0100 7107 6406 a004 7c01 a101  ......q.d...|...
-00000540: 7d01 7c01 a005 6402 a101 7249 7c01 6404  }.|...d...rI|.d.
-00000550: 6400 8502 1900 7d01 7c01 5300 7c01 a005  d.....}.|.S.|...
-00000560: 6403 a101 7252 6407 7c01 1700 7d01 7c01  d...rRd.|...}.|.
-00000570: 5300 2908 4e72 0100 0000 7212 0000 00fa  S.).Nr....r.....
-00000580: 012f 7210 0000 0072 1300 0000 7211 0000  ./r....r....r...
-00000590: 0072 1400 0000 2906 da03 7a69 7072 1c00  .r....)...zipr..
-000005a0: 0000 da03 6162 73da 0661 7070 656e 64da  ....abs..append.
-000005b0: 046a 6f69 6eda 0a73 7461 7274 7377 6974  .join..startswit
-000005c0: 6829 05da 0a66 6f61 6d5f 756e 6974 7372  h)...foam_unitsr
-000005d0: 1f00 0000 da06 7379 6d62 6f6c da08 6578  ......symbol..ex
-000005e0: 706f 6e65 6e74 da08 6f70 6572 6174 6f72  ponent..operator
-000005f0: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
-00000600: 0e66 6f61 6d5f 756e 6974 7332 7374 722a  .foam_units2str*
-00000610: 0000 0073 1e00 0000 0401 1201 0801 0201  ...s............
-00000620: 1001 0c01 1401 1e02 0a01 0a01 0c01 0403  ................
-00000630: 0afe 0801 0401 722f 0000 00e9 1400 0000  ......r/........
-00000640: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00000650: 0008 0000 0043 0000 0073 4400 0000 7a10  .....C...sD...z.
-00000660: 7400 7c01 7401 6401 6402 8400 7c00 a002  t.|.t.d.d...|...
-00000670: a100 4400 8301 8301 8302 7d01 5700 6e0b  ..D.......}.W.n.
-00000680: 0400 7403 791b 0100 0100 0100 6403 7d01  ..t.y.......d.}.
-00000690: 5900 6e01 7700 6404 7d02 7c01 7c02 1700  Y.n.w.d.}.|.|...
-000006a0: 5300 2905 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-000006b0: 0000 0300 0000 0500 0000 7300 0000 732a  ..........s...s*
-000006c0: 0000 0081 007c 005d 105c 027d 017d 0274  .....|.].\.}.}.t
-000006d0: 007c 0274 0174 0266 0283 0273 0274 037c  .|.t.t.f...s.t.|
-000006e0: 0183 0156 0001 0071 0264 0053 00a9 014e  ...V...q.d.S...N
-000006f0: 2904 da0a 6973 696e 7374 616e 6365 da04  )...isinstance..
-00000700: 4469 6374 da04 4c69 7374 da03 6c65 6e29  Dict..List..len)
-00000710: 03da 022e 30da 036b 6579 da05 7661 6c75  ....0..key..valu
-00000720: 6572 2200 0000 7222 0000 0072 2300 0000  er"...r"...r#...
-00000730: da09 3c67 656e 6578 7072 3e40 0000 0073  ..<genexpr>@...s
-00000740: 0e00 0000 0280 0400 0602 0c01 02fd 0601  ................
-00000750: 0aff 7a2b 5f63 6f6d 7075 7465 5f73 7061  ..z+_compute_spa
-00000760: 6365 735f 746f 5f61 6c69 676e 2e3c 6c6f  ces_to_align.<lo
-00000770: 6361 6c73 3e2e 3c67 656e 6578 7072 3e72  cals>.<genexpr>r
-00000780: 0100 0000 e904 0000 0029 04da 036d 696e  .........)...min
-00000790: da03 6d61 78da 0569 7465 6d73 da0a 5661  ..max..items..Va
-000007a0: 6c75 6545 7272 6f72 2903 da04 6461 7461  lueError)...data
-000007b0: da0a 6d61 785f 6c65 6e67 7468 5a0d 6465  ..max_lengthZ.de
-000007c0: 6661 756c 745f 7370 6163 6572 2200 0000  fault_spacer"...
-000007d0: 7222 0000 0072 2300 0000 da18 5f63 6f6d  r"...r#....._com
-000007e0: 7075 7465 5f73 7061 6365 735f 746f 5f61  pute_spaces_to_a
-000007f0: 6c69 676e 3c00 0000 7318 0000 0002 0102  lign<...s.......
-00000800: 0102 0108 0106 0206 fe08 fe0c 0808 0102  ................
-00000810: ff04 0308 0172 4100 0000 6300 0000 0000  .....rA...c.....
-00000820: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-00000830: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000840: 6401 6402 8400 5a03 6403 5300 2904 da04  d.d...Z.d.S.)...
-00000850: 4e6f 6465 6302 0000 0000 0000 0000 0000  Nodec...........
-00000860: 0002 0000 0003 0000 0043 0000 0073 2000  .........C...s .
-00000870: 0000 7400 7c01 8301 7400 7c00 8301 7500  ..t.|...t.|...u.
-00000880: 720e 7c00 6a01 7c01 6a01 6b02 5300 6401  r.|.j.|.j.k.S.d.
-00000890: 5300 2902 4e46 2902 da04 7479 7065 da08  S.).NF)...type..
-000008a0: 5f5f 6469 6374 5f5f 2902 da04 7365 6c66  __dict__)...self
-000008b0: da05 6f74 6865 7272 2200 0000 7222 0000  ..otherr"...r"..
-000008c0: 0072 2300 0000 da06 5f5f 6571 5f5f 4e00  .r#.....__eq__N.
-000008d0: 0000 7306 0000 0010 010c 0104 017a 0b4e  ..s..........z.N
-000008e0: 6f64 652e 5f5f 6571 5f5f 4e29 04da 085f  ode.__eq__N)..._
-000008f0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000900: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000910: 5f72 4700 0000 7222 0000 0072 2200 0000  _rG...r"...r"...
-00000920: 7222 0000 0072 2300 0000 7242 0000 004d  r"...r#...rB...M
-00000930: 0000 0073 0400 0000 0800 0c01 7242 0000  ...s........rB..
-00000940: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000950: 0000 0800 0000 4000 0000 7350 0000 0065  ......@...sP...e
-00000960: 005a 0164 005a 0209 0109 0209 0164 0e64  .Z.d.Z.......d.d
-00000970: 0365 0364 0465 0465 0319 0064 0565 0465  .e.d.e.e...d.e.e
-00000980: 0319 0066 0664 0664 0784 055a 0564 0864  ...f.d.d...Z.d.d
-00000990: 0984 005a 0664 0f64 0a64 0b84 015a 0765  ...Z.d.d.d...Z.e
-000009a0: 0864 0c64 0d84 0083 015a 0964 0153 0029  .d.d.....Z.d.S.)
-000009b0: 10da 0e4e 6f64 654c 696b 6550 7944 6963  ...NodeLikePyDic
-000009c0: 744e 4672 3f00 0000 da0a 6469 6d65 6e73  tNFr?.....dimens
-000009d0: 696f 6e73 da08 636f 6d6d 656e 7473 6305  ions..commentsc.
-000009e0: 0000 0000 0000 0000 0000 000b 0000 0007  ................
-000009f0: 0000 0043 0000 0073 fa00 0000 7c02 6400  ...C...s....|.d.
-00000a00: 7500 7206 6900 7d02 7c04 6400 7500 720c  u.r.i.}.|.d.u.r.
-00000a10: 6900 7d04 7c01 a000 a100 4400 5d6a 5c02  i.}.|.....D.]j\.
-00000a20: 7d05 7d06 7401 7c06 7402 6400 8301 7403  }.}.t.|.t.d...t.
-00000a30: 6602 8302 7224 7c00 a004 7c05 7c06 a102  f...r$|...|.|...
-00000a40: 0100 7110 7401 7c06 7405 7406 6602 8302  ..q.t.|.t.t.f...
-00000a50: 724d 7c03 6401 7500 7236 7c00 a004 7c05  rM|.d.u.r6|...|.
-00000a60: 7c06 a102 0100 7110 7c02 a007 7c05 7c03  |.....q.|...|.|.
-00000a70: a102 7d07 7401 7c06 7406 8302 7245 7408  ..}.t.|.t...rEt.
-00000a80: 7c06 8301 7d06 7c00 a009 7c05 7c06 7c07  |...}.|...|.|.|.
-00000a90: a103 0100 7110 7401 7c06 740a 8302 7275  ....q.t.|.t...ru
-00000aa0: 7c02 a007 7c05 6400 a102 7d08 7c04 a007  |...|.d...}.|...
-00000ab0: 7c05 6400 a102 7d09 740b 6900 7c05 7c09  |.d...}.t.i.|.|.
-00000ac0: 6402 8d03 7d0a 7c0a 6a0c 7c06 7c08 7c03  d...}.|.j.|.|.|.
-00000ad0: 7c09 6403 8d04 0100 7c00 a00d 7c05 7c0a  |.d.....|...|.|.
-00000ae0: a102 0100 7110 740e 7402 7c06 8301 8301  ....q.t.t.|.....
-00000af0: 8201 6400 5300 2904 4e46 2902 da04 6e61  ..d.S.).NF)...na
-00000b00: 6d65 724d 0000 0029 0372 4c00 0000 da11  merM...).rL.....
-00000b10: 6465 6661 756c 745f 6469 6d65 6e73 696f  default_dimensio
-00000b20: 6e72 4d00 0000 290f 723d 0000 0072 3200  nrM...).r=...r2.
-00000b30: 0000 7243 0000 00da 0373 7472 da09 7365  ..rC.....str..se
-00000b40: 745f 6368 696c 6472 0500 0000 da04 6c69  t_childr......li
-00000b50: 7374 da03 6765 7472 3400 0000 da09 7365  st..getr4.....se
-00000b60: 745f 7661 6c75 65da 0464 6963 7472 3300  t_value..dictr3.
-00000b70: 0000 da14 696e 6974 5f66 726f 6d5f 7079  ....init_from_py
-00000b80: 5f6f 626a 6563 7473 da09 5f73 6574 5f69  _objects.._set_i
-00000b90: 7465 6dda 134e 6f74 496d 706c 656d 656e  tem..NotImplemen
-00000ba0: 7465 6445 7272 6f72 290b 7245 0000 0072  tedError).rE...r
-00000bb0: 3f00 0000 724c 0000 0072 4f00 0000 724d  ?...rL...rO...rM
-00000bc0: 0000 0072 3700 0000 7238 0000 00da 0964  ...r7...r8.....d
-00000bd0: 696d 656e 7369 6f6e 5a0f 6469 6d65 6e73  imensionZ.dimens
-00000be0: 696f 6e73 5f64 6963 745a 0d63 6f6d 6d65  ions_dictZ.comme
-00000bf0: 6e74 735f 6469 6374 da03 6f62 6a72 2200  nts_dict..objr".
-00000c00: 0000 7222 0000 0072 2300 0000 7256 0000  ..r"...r#...rV..
-00000c10: 0055 0000 0073 3600 0000 0807 0401 0801  .U...s6.........
-00000c20: 0401 1001 1201 0e01 0e01 0801 0e01 0c02  ................
-00000c30: 0a01 0801 1001 0a01 0c01 0c01 0e01 0401  ................
-00000c40: 0201 0201 0201 0201 06fc 0e06 0c02 04e9  ................
-00000c50: 7a23 4e6f 6465 4c69 6b65 5079 4469 6374  z#NodeLikePyDict
-00000c60: 2e69 6e69 745f 6672 6f6d 5f70 795f 6f62  .init_from_py_ob
-00000c70: 6a65 6374 7363 0300 0000 0000 0000 0000  jectsc..........
-00000c80: 0000 0300 0000 0500 0000 4300 0000 735a  ..........C...sZ
-00000c90: 0000 0074 007c 0274 0164 0083 0174 0274  ...t.|.t.d...t.t
-00000ca0: 0366 0383 0272 0b6e 1a74 007c 0274 0483  .f...r.n.t.|.t..
-00000cb0: 0272 1774 057c 027c 0164 018d 027d 026e  .r.t.|.|.d...}.n
-00000cc0: 0e74 007c 0274 0683 0272 2374 077c 027c  .t.|.t...r#t.|.|
-00000cd0: 0164 018d 027d 026e 0274 0882 017c 00a0  .d...}.n.t...|..
-00000ce0: 097c 017c 02a1 0201 0064 0053 0029 024e  .|.|.....d.S.).N
-00000cf0: a901 724e 0000 0029 0a72 3200 0000 7243  ..rN...).r2...rC
-00000d00: 0000 0072 5000 0000 7205 0000 0072 5500  ...rP...r....rU.
-00000d10: 0000 7233 0000 0072 5200 0000 7234 0000  ..r3...rR...r4..
-00000d20: 0072 5800 0000 7257 0000 0029 0372 4500  .rX...rW...).rE.
-00000d30: 0000 7237 0000 00da 0563 6869 6c64 7222  ..r7.....childr"
-00000d40: 0000 0072 2200 0000 7223 0000 0072 5100  ...r"...r#...rQ.
-00000d50: 0000 7900 0000 7310 0000 0014 0102 010a  ..y...s.........
-00000d60: 010e 010a 010e 0104 0210 017a 184e 6f64  ...........z.Nod
-00000d70: 654c 696b 6550 7944 6963 742e 7365 745f  eLikePyDict.set_
-00000d80: 6368 696c 6463 0400 0000 0000 0000 0000  childc..........
-00000d90: 0000 0400 0000 0500 0000 4300 0000 7330  ..........C...s0
-00000da0: 0000 0074 007c 0274 0183 0273 097c 0364  ...t.|.t...s.|.d
-00000db0: 0075 0172 1074 027c 027c 017c 0364 018d  .u.r.t.|.|.|.d..
-00000dc0: 037d 027c 00a0 037c 017c 02a1 0201 0064  .}.|...|.|.....d
-00000dd0: 0053 0029 024e 2901 7259 0000 0029 0472  .S.).N).rY...).r
-00000de0: 3200 0000 7205 0000 00da 0556 616c 7565  2...r......Value
-00000df0: 7257 0000 0029 0472 4500 0000 724e 0000  rW...).rE...rN..
-00000e00: 0072 3800 0000 7259 0000 0072 2200 0000  .r8...rY...r"...
-00000e10: 7222 0000 0072 2300 0000 7254 0000 0084  r"...r#...rT....
-00000e20: 0000 0073 0600 0000 1201 0e01 1001 7a18  ...s..........z.
-00000e30: 4e6f 6465 4c69 6b65 5079 4469 6374 2e73  NodeLikePyDict.s
-00000e40: 6574 5f76 616c 7565 6303 0000 0000 0000  et_valuec.......
-00000e50: 0000 0000 0003 0000 0001 0000 0043 0000  .............C..
-00000e60: 0073 0400 0000 6401 5300 2902 7a0b 5365  .s....d.S.).z.Se
-00000e70: 7420 616e 2069 7465 6d4e 7222 0000 00a9  t an itemNr"....
-00000e80: 0372 4500 0000 7237 0000 0072 3800 0000  .rE...r7...r8...
-00000e90: 7222 0000 0072 2200 0000 7223 0000 0072  r"...r"...r#...r
-00000ea0: 5700 0000 8900 0000 7302 0000 0004 007a  W.......s......z
-00000eb0: 184e 6f64 654c 696b 6550 7944 6963 742e  .NodeLikePyDict.
-00000ec0: 5f73 6574 5f69 7465 6d29 034e 464e 7231  _set_item).NFNr1
-00000ed0: 0000 0029 0a72 4800 0000 7249 0000 0072  ...).rH...rI...r
-00000ee0: 4a00 0000 7255 0000 0072 0700 0000 7256  J...rU...r....rV
-00000ef0: 0000 0072 5100 0000 7254 0000 0072 0300  ...rQ...rT...r..
-00000f00: 0000 7257 0000 0072 2200 0000 7222 0000  ..rW...r"...r"..
-00000f10: 0072 2200 0000 7223 0000 0072 4b00 0000  .r"...r#...rK...
-00000f20: 5400 0000 731e 0000 0008 0002 0402 0102  T...s...........
-00000f30: 0104 fb02 0202 fe06 0302 fd06 050a fb08  ................
-00000f40: 240a 0b02 050e 0172 4b00 0000 6300 0000  $......rK...c...
-00000f50: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000f60: 0040 0000 0073 3600 0000 6500 5a01 6400  .@...s6...e.Z.d.
-00000f70: 5a02 640c 6402 6403 8401 5a03 6404 6405  Z.d.d.d...Z.d.d.
-00000f80: 8400 5a04 6406 6407 8400 5a05 6408 6409  ..Z.d.d...Z.d.d.
-00000f90: 8400 5a06 640a 640b 8400 5a07 6401 5300  ..Z.d.d...Z.d.S.
-00000fa0: 290d da0d 466f 616d 496e 7075 7446 696c  )...FoamInputFil
-00000fb0: 654e 6305 0000 0000 0000 0000 0000 0005  eNc.............
-00000fc0: 0000 0002 0000 0043 0000 0073 2e00 0000  .......C...s....
-00000fd0: 7c01 7c00 5f00 7c02 6400 7500 7209 6900  |.|._.|.d.u.r.i.
-00000fe0: 7d02 7c02 7c00 5f01 7c03 7c00 5f02 7c04  }.|.|._.|.|._.|.
-00000ff0: 7c00 5f03 6400 7c00 5f04 6400 5300 7231  |._.d.|._.d.S.r1
-00001000: 0000 0029 05da 0469 6e66 6fda 0863 6869  ...)...info..chi
-00001010: 6c64 7265 6eda 0668 6561 6465 7272 4d00  ldren..headerrM.
-00001020: 0000 da04 7061 7468 2905 7245 0000 0072  ....path).rE...r
-00001030: 6000 0000 7261 0000 0072 6200 0000 724d  `...ra...rb...rM
-00001040: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00001050: 0000 da08 5f5f 696e 6974 5f5f 8f00 0000  ....__init__....
-00001060: 730e 0000 0006 0108 0104 0106 0106 0106  s...............
-00001070: 010a 017a 1646 6f61 6d49 6e70 7574 4669  ...z.FoamInputFi
-00001080: 6c65 2e5f 5f69 6e69 745f 5f63 0100 0000  le.__init__c....
-00001090: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-000010a0: 4300 0000 7342 0000 0064 0167 017d 017c  C...sB...d.g.}.|
-000010b0: 006a 0064 0075 0172 127c 01a0 0164 027c  .j.d.u.r.|...d.|
-000010c0: 006a 009b 0064 039d 03a1 0101 007c 01a0  .j...d.......|..
-000010d0: 0164 047c 006a 029b 0064 059d 03a1 0101  .d.|.j...d......
-000010e0: 0064 06a0 037c 01a1 0153 0029 074e 7a0b  .d...|...S.).Nz.
-000010f0: 496e 7075 7446 696c 6528 0a7a 0569 6e66  InputFile(.z.inf
-00001100: 6f3d 7a02 2c0a 7a09 6368 696c 6472 656e  o=z.,.z.children
-00001110: 3d7a 020a 2972 1100 0000 2904 7260 0000  =z..)r....).r`..
-00001120: 0072 2800 0000 7261 0000 0072 2900 0000  .r(...ra...r)...
-00001130: 2902 7245 0000 00da 0374 6d70 7222 0000  ).rE.....tmpr"..
-00001140: 0072 2200 0000 7223 0000 00da 085f 5f72  .r"...r#.....__r
-00001150: 6570 725f 5f98 0000 0073 0a00 0000 0601  epr__....s......
-00001160: 0a01 1401 1401 0a01 7a16 466f 616d 496e  ........z.FoamIn
-00001170: 7075 7446 696c 652e 5f5f 7265 7072 5f5f  putFile.__repr__
-00001180: 6301 0000 0000 0000 0000 0000 000b 0000  c...............
-00001190: 0008 0000 0043 0000 0073 a201 0000 6700  .....C...s....g.
-000011a0: 7d01 7c00 6a00 6400 7501 7236 6401 6701  }.|.j.d.u.r6d.g.
-000011b0: 7d02 7c00 6a00 a001 a100 4400 5d19 5c02  }.|.j.....D.].\.
-000011c0: 7d03 7d04 6402 7402 7c03 8301 1800 6403  }.}.d.t.|.....d.
-000011d0: 1400 7d05 7c02 a003 6404 7c03 9b00 7c05  ..}.|...d.|...|.
-000011e0: 9b00 7c04 9b00 6405 9d05 a101 0100 710f  ..|...d.......q.
-000011f0: 7c02 a003 6406 a101 0100 7c01 a003 6407  |...d.....|...d.
-00001200: a004 7c02 a101 a101 0100 7405 7c00 6a06  ..|.......t.|.j.
-00001210: 6408 6409 8d02 7d06 7c00 6a06 a001 a100  d.d...}.|.j.....
-00001220: 4400 5d71 5c02 7d03 7d04 7407 7c04 640a  D.]q\.}.}.t.|.d.
-00001230: 8302 725d 7c04 a008 a100 7d07 7c03 6400  ..r]|.....}.|.d.
-00001240: 7500 725c 7409 7c04 740a 8302 725c 7c07  u.r\t.|.t...r\|.
-00001250: 6405 3700 7d07 6e2f 7c04 6400 7500 7265  d.7.}.n/|.d.u.re
-00001260: 7c03 9b00 7d07 6e27 7407 7c04 640b 8302  |...}.n't.|.d...
-00001270: 726f 7c04 a00b a100 7d08 6e02 7c04 7d08  ro|.....}.n.|.}.
-00001280: 7c08 640c 6b02 7278 640c 7d05 6e0b 740c  |.d.k.rxd.}.n.t.
-00001290: 640d 7c06 7402 7c03 8301 1800 8302 6403  d.|.t.|.......d.
-000012a0: 1400 7d05 7c03 9b00 7c05 9b00 7c08 9b00  ..}.|...|...|...
-000012b0: 6405 9d04 7d07 7c00 6a0d 6400 7501 72ae  d...}.|.j.d.u.r.
-000012c0: 7c03 7c00 6a0d 7600 72ae 7c00 6a0d 7c03  |.|.j.v.r.|.j.|.
-000012d0: 1900 7d09 7409 7c09 740e 8302 72ae 640e  ..}.t.|.t...r.d.
-000012e0: 7c09 a00f 6407 640f a102 1700 7d09 7c09  |...d.d.....}.|.
-000012f0: 6407 1700 7c07 1700 7d07 7c01 a003 7c07  d...|...}.|...|.
-00001300: a101 0100 7142 6410 a004 7c01 a101 7d0a  ....qBd...|...}.
-00001310: 7c00 6a10 6400 7501 72c5 7c00 6a10 6407  |.j.d.u.r.|.j.d.
-00001320: 1700 7c0a 1700 7d0a 7c0a 6411 1900 6407  ..|...}.|.d...d.
-00001330: 6b03 72cf 7c0a 6407 3700 7d0a 7c0a 5300  k.r.|.d.7.}.|.S.
-00001340: 2912 4e7a 0a46 6f61 6d46 696c 650a 7be9  ).Nz.FoamFile.{.
-00001350: 0c00 0000 da01 20fa 0420 2020 20fa 013b  ...... ..    ..;
-00001360: da01 7dda 010a e90e 0000 0029 0172 4000  ..}........).r@.
-00001370: 0000 da04 6475 6d70 da17 6475 6d70 5f77  ....dump..dump_w
-00001380: 6974 686f 7574 5f61 7373 6967 6e6d 656e  ithout_assignmen
-00001390: 7472 1100 0000 e902 0000 007a 032f 2f20  tr.........z.// 
-000013a0: 7a04 0a2f 2f20 7a02 0a0a 7215 0000 0029  z..// z...r....)
-000013b0: 1172 6000 0000 723d 0000 0072 3500 0000  .r`...r=...r5...
-000013c0: 7228 0000 0072 2900 0000 7241 0000 0072  r(...r)...rA...r
-000013d0: 6100 0000 da07 6861 7361 7474 7272 6e00  a.....hasattrrn.
-000013e0: 0000 7232 0000 0072 3400 0000 726f 0000  ..r2...r4...ro..
-000013f0: 0072 3c00 0000 724d 0000 0072 5000 0000  .r<...rM...rP...
-00001400: da07 7265 706c 6163 6572 6200 0000 290b  ..replacerb...).
-00001410: 7245 0000 0072 6500 0000 5a04 746d 7031  rE...re...Z.tmp1
-00001420: 7237 0000 00da 046e 6f64 6572 0b00 0000  r7.....noder....
-00001430: da0a 6e75 6d5f 7370 6163 6573 da09 636f  ..num_spaces..co
-00001440: 6465 5f6e 6f64 655a 0b6e 6f64 655f 6475  de_nodeZ.node_du
-00001450: 6d70 6564 da07 636f 6d6d 656e 7472 1f00  mped..commentr..
-00001460: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00001470: 0072 6e00 0000 9f00 0000 7348 0000 0004  .rn.......sH....
-00001480: 010a 0106 0112 0110 011c 010a 0110 010e  ................
-00001490: 0212 010a 0108 0112 0208 0102 8008 0108  ................
-000014a0: 010a 020a 0104 0208 0106 0116 0212 0114  ................
-000014b0: 010a 010a 0110 010c 010c 010a 010a 010e  ................
-000014c0: 010c 0108 0104 017a 1246 6f61 6d49 6e70  .......z.FoamInp
-000014d0: 7574 4669 6c65 2e64 756d 7063 0100 0000  utFile.dumpc....
-000014e0: 0000 0000 0000 0000 0200 0000 0800 0000  ................
-000014f0: 4300 0000 7352 0000 007c 006a 0064 0075  C...sR...|.j.d.u
-00001500: 0072 0974 0164 0183 0182 0174 027c 006a  .r.t.d.....t.|.j
-00001510: 0064 0283 028f 107d 017c 01a0 037c 00a0  .d.....}.|...|..
-00001520: 04a1 00a1 0101 0057 0064 0004 0004 0083  .......W.d......
-00001530: 0301 0064 0053 0031 0073 2277 0101 0001  ...d.S.1.s"w....
-00001540: 0001 0059 0001 0064 0053 0029 034e 7a11  ...Y...d.S.).Nz.
-00001550: 7365 6c66 2e70 6174 6820 6973 204e 6f6e  self.path is Non
-00001560: 65da 0177 2905 7263 0000 0072 3e00 0000  e..w).rc...r>...
-00001570: da04 6f70 656e da05 7772 6974 6572 6e00  ..open..writern.
-00001580: 0000 2902 7245 0000 00da 0466 696c 6572  ..).rE.....filer
-00001590: 2200 0000 7222 0000 0072 2300 0000 da09  "...r"...r#.....
-000015a0: 6f76 6572 7772 6974 65c9 0000 0073 0a00  overwrite....s..
-000015b0: 0000 0a01 0801 0e01 1001 22ff 7a17 466f  ..........".z.Fo
-000015c0: 616d 496e 7075 7446 696c 652e 6f76 6572  amInputFile.over
-000015d0: 7772 6974 6563 0300 0000 0000 0000 0000  writec..........
-000015e0: 0000 0300 0000 0300 0000 4300 0000 730e  ..........C...s.
-000015f0: 0000 007c 027c 006a 007c 013c 0064 0053  ...|.|.j.|.<.d.S
-00001600: 0072 3100 0000 2901 7261 0000 0072 5e00  .r1...).ra...r^.
-00001610: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00001620: 0072 5700 0000 cf00 0000 f302 0000 000e  .rW.............
-00001630: 017a 1746 6f61 6d49 6e70 7574 4669 6c65  .z.FoamInputFile
-00001640: 2e5f 7365 745f 6974 656d a903 4e4e 4e29  ._set_item..NNN)
-00001650: 0872 4800 0000 7249 0000 0072 4a00 0000  .rH...rI...rJ...
-00001660: 7264 0000 0072 6600 0000 726e 0000 0072  rd...rf...rn...r
-00001670: 7b00 0000 7257 0000 0072 2200 0000 7222  {...rW...r"...r"
-00001680: 0000 0072 2200 0000 7223 0000 0072 5f00  ...r"...r#...r_.
-00001690: 0000 8e00 0000 730c 0000 0008 000a 0108  ......s.........
-000016a0: 0908 0708 2a0c 0672 5f00 0000 6300 0000  ....*..r_...c...
-000016b0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-000016c0: 0040 0000 0073 2800 0000 6500 5a01 6400  .@...s(...e.Z.d.
-000016d0: 5a02 5500 6503 6504 6401 3c00 6505 6504  Z.U.e.e.d.<.e.e.
-000016e0: 6402 3c00 6407 6404 6405 8401 5a06 6406  d.<.d.d.d...Z.d.
-000016f0: 5300 2908 da0a 4173 7369 676e 6d65 6e74  S.)...Assignment
-00001700: 724e 0000 0072 3800 0000 7201 0000 0063  rN...r8...r....c
-00001710: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00001720: 0500 0000 4300 0000 7334 0000 0074 007c  ....C...s4...t.|
-00001730: 006a 0164 0183 0272 0c7c 006a 01a0 027c  .j.d...r.|.j...|
-00001740: 01a1 0153 007c 0164 0214 007c 006a 039b  ...S.|.d...|.j..
-00001750: 0064 037c 006a 019b 0064 049d 0417 0053  .d.|.j...d.....S
-00001760: 00a9 054e 726e 0000 0072 6800 0000 fa02  ...Nrn...rh.....
-00001770: 2020 726a 0000 0029 0472 7100 0000 7238    rj...).rq...r8
-00001780: 0000 0072 6e00 0000 724e 0000 00a9 0272  ...rn...rN.....r
-00001790: 4500 0000 da06 696e 6465 6e74 7222 0000  E.....indentr"..
-000017a0: 0072 2200 0000 7223 0000 0072 6e00 0000  .r"...r#...rn...
-000017b0: d800 0000 7306 0000 000c 010c 011c 027a  ....s..........z
-000017c0: 0f41 7373 6967 6e6d 656e 742e 6475 6d70  .Assignment.dump
-000017d0: 4ea9 0172 0100 0000 2907 7248 0000 0072  N..r....).rH...r
-000017e0: 4900 0000 724a 0000 0072 5000 0000 da0f  I...rJ...rP.....
-000017f0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fda  __annotations__.
-00001800: 066f 626a 6563 7472 6e00 0000 7222 0000  .objectrn...r"..
-00001810: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
-00001820: 727e 0000 00d3 0000 0073 0800 0000 0a00  r~.......s......
-00001830: 0802 0801 0e02 727e 0000 0063 0000 0000  ......r~...c....
-00001840: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00001850: 0000 0000 7326 0000 0065 005a 0164 005a  ....s&...e.Z.d.Z
-00001860: 0287 0066 0164 0164 0284 085a 0364 0664  ...f.d.d...Z.d.d
-00001870: 0464 0584 015a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
-00001880: 07da 1256 6172 6961 626c 6541 7373 6967  ...VariableAssig
-00001890: 6e6d 656e 7463 0100 0000 0000 0000 0000  nmentc..........
-000018a0: 0000 0200 0000 0200 0000 0300 0000 730e  ..............s.
-000018b0: 0000 0074 0083 00a0 01a1 007d 017c 0153  ...t.......}.|.S
-000018c0: 0072 3100 0000 a902 da05 7375 7065 7272  .r1.......superr
-000018d0: 6600 0000 2902 7245 0000 0072 0b00 0000  f...).rE...r....
-000018e0: a901 da09 5f5f 636c 6173 735f 5f72 2200  ....__class__r".
-000018f0: 0000 7223 0000 0072 6600 0000 e000 0000  ..r#...rf.......
-00001900: 7304 0000 000a 0104 017a 1b56 6172 6961  s........z.Varia
-00001910: 626c 6541 7373 6967 6e6d 656e 742e 5f5f  bleAssignment.__
-00001920: 7265 7072 5f5f 7201 0000 0063 0200 0000  repr__r....c....
-00001930: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00001940: 4300 0000 734a 0000 0074 007c 006a 0164  C...sJ...t.|.j.d
-00001950: 0183 0272 177c 0164 0214 007c 006a 029b  ...r.|.d...|.j..
-00001960: 0064 037c 006a 01a0 037c 01a1 019b 0064  .d.|.j...|.....d
-00001970: 049d 0417 0053 007c 0164 0214 007c 006a  .....S.|.d...|.j
-00001980: 029b 0064 037c 006a 019b 0064 049d 0417  ...d.|.j...d....
-00001990: 0053 0072 7f00 0000 2904 7271 0000 0072  .S.r....).rq...r
-000019a0: 3800 0000 724e 0000 0072 6e00 0000 7281  8...rN...rn...r.
-000019b0: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-000019c0: 0000 726e 0000 00e4 0000 0073 0600 0000  ..rn.......s....
-000019d0: 0c01 2201 1c02 7a17 5661 7269 6162 6c65  .."...z.Variable
-000019e0: 4173 7369 676e 6d65 6e74 2e64 756d 7072  Assignment.dumpr
-000019f0: 8300 0000 2906 7248 0000 0072 4900 0000  ....).rH...rI...
-00001a00: 724a 0000 0072 6600 0000 726e 0000 00da  rJ...rf...rn....
-00001a10: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7222  .__classcell__r"
-00001a20: 0000 0072 2200 0000 7289 0000 0072 2300  ...r"...r....r#.
-00001a30: 0000 7286 0000 00df 0000 0073 0600 0000  ..r........s....
-00001a40: 0800 0c01 1204 7286 0000 0063 0000 0000  ......r....c....
-00001a50: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00001a60: 4000 0000 f328 0000 0065 005a 0164 005a  @....(...e.Z.d.Z
-00001a70: 0264 0964 0264 0384 015a 0364 0464 0584  .d.d.d...Z.d.d..
-00001a80: 005a 0464 0a64 0764 0884 015a 0564 0153  .Z.d.d.d...Z.d.S
-00001a90: 0029 0b72 5d00 0000 4e63 0400 0000 0000  .).r]...Nc......
-00001aa0: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
-00001ab0: 0000 732c 0000 007c 017c 005f 007c 027c  ..s,...|.|._.|.|
-00001ac0: 005f 0174 027c 0374 0374 0466 0283 0272  ._.t.|.t.t.f...r
-00001ad0: 1174 057c 0383 017d 037c 037c 005f 0664  .t.|...}.|.|._.d
-00001ae0: 0053 0072 3100 0000 2907 7238 0000 0072  .S.r1...).r8...r
-00001af0: 4e00 0000 7232 0000 0072 5200 0000 da05  N...r2...rR.....
-00001b00: 7475 706c 6572 2f00 0000 7259 0000 0029  tupler/...rY...)
-00001b10: 0472 4500 0000 7238 0000 0072 4e00 0000  .rE...r8...rN...
-00001b20: 7259 0000 0072 2200 0000 7222 0000 0072  rY...r"...r"...r
-00001b30: 2300 0000 7264 0000 00ed 0000 0073 0a00  #...rd.......s..
-00001b40: 0000 0601 0601 0e01 0801 0a01 7a0e 5661  ............z.Va
-00001b50: 6c75 652e 5f5f 696e 6974 5f5f 6301 0000  lue.__init__c...
-00001b60: 0000 0000 0000 0000 0001 0000 0007 0000  ................
-00001b70: 0043 0000 0073 9400 0000 7c00 6a00 6400  .C...s....|.j.d.
-00001b80: 7501 7219 7c00 6a01 6400 7501 7219 6401  u.r.|.j.d.u.r.d.
-00001b90: 7c00 6a02 9b00 6402 7c00 6a01 9b00 6403  |.j...d.|.j...d.
-00001ba0: 7c00 6a00 9b00 6404 9d07 5300 7c00 6a00  |.j...d...S.|.j.
-00001bb0: 6400 7500 722e 7c00 6a01 6400 7501 722e  d.u.r.|.j.d.u.r.
-00001bc0: 6401 7c00 6a02 9b00 6402 7c00 6a01 9b00  d.|.j...d.|.j...
-00001bd0: 6404 9d05 5300 7c00 6a00 6400 7501 7243  d...S.|.j.d.u.rC
-00001be0: 7c00 6a01 6400 7500 7243 6401 7c00 6a02  |.j.d.u.rCd.|.j.
-00001bf0: 9b00 6405 7c00 6a00 9b00 6404 9d05 5300  ..d.|.j...d...S.
-00001c00: 6401 7c00 6a02 9b00 6406 9d03 5300 2907  d.|.j...d...S.).
-00001c10: 4e7a 0656 616c 7565 287a 082c 206e 616d  Nz.Value(z., nam
-00001c20: 653d 227a 0e22 2c20 6469 6d65 6e73 696f  e="z.", dimensio
-00001c30: 6e3d 227a 0222 297a 0d2c 2064 696d 656e  n="z.")z., dimen
-00001c40: 7369 6f6e 3d22 fa01 2929 0372 5900 0000  sion="..)).rY...
-00001c50: 724e 0000 0072 3800 0000 a901 7245 0000  rN...r8.....rE..
-00001c60: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
-00001c70: 7266 0000 00f4 0000 0073 0e00 0000 1401  rf.......s......
-00001c80: 1e01 1401 1601 1401 1601 0e02 7a0e 5661  ............z.Va
-00001c90: 6c75 652e 5f5f 7265 7072 5f5f 7201 0000  lue.__repr__r...
-00001ca0: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
-00001cb0: 0000 0500 0000 4300 0000 73ce 0000 007c  ......C...s....|
-00001cc0: 006a 0064 0075 0172 1474 017c 006a 0083  .j.d.u.r.t.|.j..
-00001cd0: 017d 0264 01a0 0264 0264 0384 007c 0244  .}.d...d.d...|.D
-00001ce0: 0083 01a1 017d 0374 037c 006a 0474 0583  .....}.t.|.j.t..
-00001cf0: 0272 2674 067c 006a 0464 0483 0272 267c  .r&t.|.j.d...r&|
-00001d00: 006a 04a0 07a1 007d 046e 0574 087c 006a  .j.....}.n.t.|.j
-00001d10: 0483 017d 047c 006a 0064 0075 0172 407c  ...}.|.j.d.u.r@|
-00001d20: 006a 0964 0075 0172 407c 006a 099b 0064  .j.d.u.r@|.j...d
-00001d30: 057c 039b 0064 067c 049b 009d 0553 007c  .|...d.|.....S.|
-00001d40: 006a 0064 0075 0072 527c 006a 0964 0075  .j.d.u.rR|.j.d.u
-00001d50: 0172 527c 006a 099b 0064 017c 049b 009d  .rR|.j...d.|....
-00001d60: 0353 007c 006a 0064 0075 0172 647c 006a  .S.|.j.d.u.rd|.j
-00001d70: 0964 0075 0072 6464 077c 039b 0064 067c  .d.u.rdd.|...d.|
-00001d80: 049b 009d 0453 007c 049b 0053 0029 084e  .....S.|...S.).N
-00001d90: 7268 0000 0063 0100 0000 0000 0000 0000  rh...c..........
-00001da0: 0000 0200 0000 0300 0000 7300 0000 f318  ..........s.....
-00001db0: 0000 0081 007c 005d 077d 0174 007c 0183  .....|.].}.t.|..
-00001dc0: 0156 0001 0071 0264 0053 0072 3100 0000  .V...q.d.S.r1...
-00001dd0: a901 7250 0000 00a9 0272 3600 0000 da06  ..rP.....r6.....
-00001de0: 6e75 6d62 6572 7222 0000 0072 2200 0000  numberr"...r"...
-00001df0: 7223 0000 0072 3900 0000 0101 0000 f304  r#...r9.........
-00001e00: 0000 0002 8016 007a 3056 616c 7565 2e64  .......z0Value.d
-00001e10: 756d 705f 7769 7468 6f75 745f 6173 7369  ump_without_assi
-00001e20: 676e 6d65 6e74 2e3c 6c6f 6361 6c73 3e2e  gnment.<locals>.
-00001e30: 3c67 656e 6578 7072 3e72 6e00 0000 7a02  <genexpr>rn...z.
-00001e40: 205b 7a02 5d20 fa01 5b29 0a72 5900 0000   [z.] ..[).rY...
-00001e50: 7224 0000 0072 2900 0000 7232 0000 0072  r$...r)...r2...r
-00001e60: 3800 0000 7242 0000 0072 7100 0000 726e  8...rB...rq...rn
-00001e70: 0000 0072 5000 0000 724e 0000 0029 0572  ...rP...rN...).r
-00001e80: 4500 0000 7282 0000 005a 0e64 696d 656e  E...r....Z.dimen
-00001e90: 7369 6f6e 5f6c 6973 745a 1064 696d 656e  sion_listZ.dimen
-00001ea0: 7369 6f6e 5f64 756d 7065 645a 0c76 616c  sion_dumpedZ.val
-00001eb0: 7565 5f64 756d 7065 6472 2200 0000 7222  ue_dumpedr"...r"
-00001ec0: 0000 0072 2300 0000 726f 0000 00fe 0000  ...r#...ro......
-00001ed0: 0073 1a00 0000 0a01 0a01 1401 1802 0c01  .s..............
-00001ee0: 0a02 1402 1601 1401 1001 1401 1001 0602  ................
-00001ef0: 7a1d 5661 6c75 652e 6475 6d70 5f77 6974  z.Value.dump_wit
-00001f00: 686f 7574 5f61 7373 6967 6e6d 656e 74a9  hout_assignment.
-00001f10: 024e 4e72 8300 0000 2906 7248 0000 0072  .NNr....).rH...r
-00001f20: 4900 0000 724a 0000 0072 6400 0000 7266  I...rJ...rd...rf
-00001f30: 0000 0072 6f00 0000 7222 0000 0072 2200  ...ro...r"...r".
-00001f40: 0000 7222 0000 0072 2300 0000 725d 0000  ..r"...r#...r]..
-00001f50: 00eb 0000 0073 0800 0000 0800 0a02 0807  .....s..........
-00001f60: 0e0a 725d 0000 0063 0000 0000 0000 0000  ..r]...c........
-00001f70: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00001f80: 732e 0000 0065 005a 0164 005a 0287 0066  s....e.Z.d.Z...f
-00001f90: 0164 0164 0284 085a 0364 0364 0484 005a  .d.d...Z.d.d...Z
-00001fa0: 0464 0864 0664 0784 015a 0587 0004 005a  .d.d.d...Z.....Z
-00001fb0: 0653 0029 09da 0c44 696d 656e 7369 6f6e  .S.)...Dimension
-00001fc0: 5365 7463 0200 0000 0000 0000 0000 0000  Setc............
-00001fd0: 0200 0000 0300 0000 0300 0000 732a 0000  ............s*..
-00001fe0: 0074 0064 0164 0284 007c 0144 0083 0183  .t.d.d...|.D....
-00001ff0: 0173 0d74 0164 0383 0182 0174 0283 00a0  .s.t.d.....t....
-00002000: 037c 01a1 0101 0064 0053 0029 044e 6301  .|.....d.S.).Nc.
-00002010: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00002020: 0000 0073 0000 0073 1a00 0000 8100 7c00  ...s...s......|.
-00002030: 5d08 7d01 7400 7c01 7401 8302 5600 0100  ].}.t.|.t...V...
-00002040: 7102 6400 5300 7231 0000 0029 0272 3200  q.d.S.r1...).r2.
-00002050: 0000 721b 0000 0029 0272 3600 0000 da04  ..r....).r6.....
-00002060: 656c 656d 7222 0000 0072 2200 0000 7223  elemr"...r"...r#
-00002070: 0000 0072 3900 0000 1401 0000 f304 0000  ...r9...........
-00002080: 0002 8018 007a 2844 696d 656e 7369 6f6e  .....z(Dimension
-00002090: 5365 742e 5f5f 696e 6974 5f5f 2e3c 6c6f  Set.__init__.<lo
-000020a0: 6361 6c73 3e2e 3c67 656e 6578 7072 3e7a  cals>.<genexpr>z
-000020b0: 1342 6164 207b 666f 616d 5f75 6e69 7473  .Bad {foam_units
-000020c0: 203d 207d 2904 da03 616c 6c72 3e00 0000   = })...allr>...
-000020d0: 7288 0000 0072 6400 0000 2902 7245 0000  r....rd...).rE..
-000020e0: 0072 2b00 0000 7289 0000 0072 2200 0000  .r+...r....r"...
-000020f0: 7223 0000 0072 6400 0000 1301 0000 7306  r#...rd.......s.
-00002100: 0000 0012 0108 0110 017a 1544 696d 656e  .........z.Dimen
-00002110: 7369 6f6e 5365 742e 5f5f 696e 6974 5f5f  sionSet.__init__
-00002120: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00002130: 0002 0000 0043 0000 0073 0800 0000 7400  .....C...s....t.
-00002140: 7c00 8301 5300 7231 0000 0029 0172 2f00  |...S.r1...).r/.
-00002150: 0000 728f 0000 0072 2200 0000 7222 0000  ..r....r"...r"..
-00002160: 0072 2300 0000 7266 0000 0018 0100 00f3  .r#...rf........
-00002170: 0200 0000 0801 7a15 4469 6d65 6e73 696f  ......z.Dimensio
-00002180: 6e53 6574 2e5f 5f72 6570 725f 5f72 0100  nSet.__repr__r..
-00002190: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-000021a0: 0000 0005 0000 0043 0000 0073 1c00 0000  .......C...s....
-000021b0: 6401 6402 a000 6403 6404 8400 7c00 4400  d.d...d.d...|.D.
-000021c0: 8301 a101 1700 6405 1700 5300 2906 4e72  ......d...S.).Nr
-000021d0: 9500 0000 7268 0000 0063 0100 0000 0000  ....rh...c......
-000021e0: 0000 0000 0000 0200 0000 0300 0000 7300  ..............s.
-000021f0: 0000 7290 0000 0072 3100 0000 7291 0000  ..r....r1...r...
-00002200: 0072 9200 0000 7222 0000 0072 2200 0000  .r....r"...r"...
-00002210: 7223 0000 0072 3900 0000 1c01 0000 7294  r#...r9.......r.
-00002220: 0000 007a 3744 696d 656e 7369 6f6e 5365  ...z7DimensionSe
-00002230: 742e 6475 6d70 5f77 6974 686f 7574 5f61  t.dump_without_a
-00002240: 7373 6967 6e6d 656e 742e 3c6c 6f63 616c  ssignment.<local
-00002250: 733e 2e3c 6765 6e65 7870 723e fa01 5da9  s>.<genexpr>..].
-00002260: 0172 2900 0000 7281 0000 0072 2200 0000  .r)...r....r"...
-00002270: 7222 0000 0072 2300 0000 726f 0000 001b  r"...r#...ro....
-00002280: 0100 00f3 0200 0000 1c01 7a24 4469 6d65  ..........z$Dime
-00002290: 6e73 696f 6e53 6574 2e64 756d 705f 7769  nsionSet.dump_wi
-000022a0: 7468 6f75 745f 6173 7369 676e 6d65 6e74  thout_assignment
-000022b0: 7283 0000 0029 0772 4800 0000 7249 0000  r....).rH...rI..
-000022c0: 0072 4a00 0000 7264 0000 0072 6600 0000  .rJ...rd...rf...
-000022d0: 726f 0000 0072 8b00 0000 7222 0000 0072  ro...r....r"...r
-000022e0: 2200 0000 7289 0000 0072 2300 0000 7297  "...r....r#...r.
-000022f0: 0000 0012 0100 0073 0800 0000 0800 0c01  .......s........
-00002300: 0805 1203 7297 0000 0063 0000 0000 0000  ....r....c......
-00002310: 0000 0000 0000 0000 0000 0400 0000 0000  ................
-00002320: 0000 7344 0000 0065 005a 0164 005a 0264  ..sD...e.Z.d.Z.d
-00002330: 0d87 0066 0164 0264 0384 095a 0364 0464  ...f.d.d...Z.d.d
-00002340: 0584 005a 0487 0066 0164 0664 0784 085a  ...Z...f.d.d...Z
-00002350: 0564 0e64 0964 0a84 015a 0664 0b64 0c84  .d.d.d...Z.d.d..
-00002360: 005a 0787 0004 005a 0853 0029 0f72 3300  .Z.....Z.S.).r3.
-00002370: 0000 4e63 0500 0000 0000 0000 0000 0000  ..Nc............
-00002380: 0500 0000 0400 0000 0300 0000 7328 0000  ............s(..
-00002390: 007c 027c 005f 007c 037c 005f 017c 047c  .|.|._.|.|._.|.|
-000023a0: 005f 0274 0383 006a 0464 0169 007c 01a4  ._.t...j.d.i.|..
-000023b0: 018e 0101 0064 0053 0029 024e 7222 0000  .....d.S.).Nr"..
-000023c0: 0029 05da 055f 6e61 6d65 da0a 5f64 6972  .)..._name.._dir
-000023d0: 6563 7469 7665 724d 0000 0072 8800 0000  ectiverM...r....
-000023e0: 7264 0000 0029 0572 4500 0000 723f 0000  rd...).rE...r?..
-000023f0: 0072 4e00 0000 da09 6469 7265 6374 6976  .rN.....directiv
-00002400: 6572 4d00 0000 7289 0000 0072 2200 0000  erM...r....r"...
-00002410: 7223 0000 0072 6400 0000 2001 0000 7308  r#...rd... ...s.
-00002420: 0000 0006 0106 0106 0116 017a 0d44 6963  ...........z.Dic
-00002430: 742e 5f5f 696e 6974 5f5f 6301 0000 0000  t.__init__c.....
-00002440: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00002450: 0000 00f3 0600 0000 7c00 6a00 5300 7231  ........|.j.S.r1
-00002460: 0000 00a9 0172 9f00 0000 728f 0000 0072  .....r....r....r
-00002470: 2200 0000 7222 0000 0072 2300 0000 da08  "...r"...r#.....
-00002480: 6765 745f 6e61 6d65 2601 0000 f302 0000  get_name&.......
-00002490: 0006 017a 0d44 6963 742e 6765 745f 6e61  ...z.Dict.get_na
-000024a0: 6d65 6301 0000 0000 0000 0000 0000 0001  mec.............
-000024b0: 0000 0002 0000 0003 0000 00f3 0a00 0000  ................
-000024c0: 7400 8300 a001 a100 5300 7231 0000 0072  t.......S.r1...r
-000024d0: 8700 0000 728f 0000 0072 8900 0000 7222  ....r....r....r"
-000024e0: 0000 0072 2300 0000 7266 0000 0029 0100  ...r#...rf...)..
-000024f0: 00f3 0200 0000 0a01 7a0d 4469 6374 2e5f  ........z.Dict._
-00002500: 5f72 6570 725f 5f72 0100 0000 6302 0000  _repr__r....c...
-00002510: 0000 0000 0000 0000 000b 0000 0009 0000  ................
-00002520: 0043 0000 0073 5401 0000 6700 7d02 7c01  .C...sT...g.}.|.
-00002530: 6401 1400 7d03 7c00 6a00 6400 7501 7228  d...}.|.j.d.u.r(
-00002540: 7c03 7c00 6a00 1700 7d04 7c00 6a01 6400  |.|.j...}.|.j.d.
-00002550: 7501 721c 7c04 6402 7c00 6a01 1700 3700  u.r.|.d.|.j...7.
-00002560: 7d04 7c02 a002 7c04 6403 7c03 9b00 9d02  }.|...|.d.|.....
-00002570: 1700 6404 1700 a101 0100 7403 7c00 8301  ..d.......t.|...
-00002580: 7d05 7c00 a004 a100 4400 5d60 5c02 7d06  }.|.....D.]`\.}.
-00002590: 7d07 7c00 6a05 6400 7501 7253 7c06 7c00  }.|.j.d.u.rS|.|.
-000025a0: 6a05 7600 7253 7c00 6a05 7c06 1900 7d08  j.v.rS|.j.|...}.
-000025b0: 7406 7c08 7407 8302 7253 7c02 a002 6405  t.|.t...rS|...d.
-000025c0: 7c08 a008 6403 6406 a102 1700 a101 0100  |...d.d.........
-000025d0: 7409 7c07 6407 8302 7263 7c02 a002 7c07  t.|.d...rc|...|.
-000025e0: a00a 7c01 6408 1700 a101 a101 0100 7130  ..|.d.........q0
-000025f0: 7409 7c07 6409 8302 726d 7c07 a00b a100  t.|.d...rm|.....
-00002600: 7d09 6e02 7c07 7d09 7c07 640a 6b02 7276  }.n.|.}.|.d.k.rv
-00002610: 640a 7d0a 6e0b 740c 640b 7c05 740d 7c06  d.}.n.t.d.|.t.|.
-00002620: 8301 1800 8302 6401 1400 7d0a 7c02 a002  ......d...}.|...
-00002630: 7c03 640c 7c06 9b00 7c0a 9b00 7c09 9b00  |.d.|...|...|...
-00002640: 640d 9d05 1700 a101 0100 7130 7c02 a002  d.........q0|...
-00002650: 7c03 640e 1700 a101 0100 7406 7c00 740e  |.d.......t.|.t.
-00002660: 8302 72a5 7c02 640f 0500 1900 640d 3700  ..r.|.d.....d.7.
-00002670: 0300 3c00 6403 a00f 7c02 a101 5300 2910  ..<.d...|...S.).
-00002680: 4e72 6800 0000 7280 0000 0072 6c00 0000  Nrh...r....rl...
-00002690: da01 7b7a 0720 2020 202f 2f20 7a08 0a20  ..{z.    // z.. 
-000026a0: 2020 202f 2f20 726e 0000 0072 3a00 0000     // rn...r:...
-000026b0: 726f 0000 0072 1100 0000 7270 0000 0072  ro...r....rp...r
-000026c0: 6900 0000 726a 0000 0072 6b00 0000 7215  i...rj...rk...r.
-000026d0: 0000 0029 1072 9f00 0000 72a0 0000 0072  ...).r....r....r
-000026e0: 2800 0000 7241 0000 0072 3d00 0000 724d  (...rA...r=...rM
-000026f0: 0000 0072 3200 0000 7250 0000 0072 7200  ...r2...rP...rr.
-00002700: 0000 7271 0000 0072 6e00 0000 726f 0000  ..rq...rn...ro..
-00002710: 0072 3c00 0000 7235 0000 00da 0a43 6f64  .r<...r5.....Cod
-00002720: 6553 7472 6561 6d72 2900 0000 290b 7245  eStreamr)...).rE
-00002730: 0000 0072 8200 0000 7265 0000 00da 0b69  ...r....re.....i
-00002740: 6e64 656e 7461 7469 6f6e da04 6c69 6e65  ndentation..line
-00002750: 7274 0000 0072 3700 0000 7273 0000 0072  rt...r7...rs...r
-00002760: 7600 0000 7275 0000 0072 0b00 0000 7222  v...ru...r....r"
-00002770: 0000 0072 2200 0000 7223 0000 0072 6e00  ...r"...r#...rn.
-00002780: 0000 2c01 0000 7334 0000 0004 0108 010a  ..,...s4........
-00002790: 010a 010a 010e 0118 0108 0210 0114 010a  ................
-000027a0: 010a 0116 010a 0216 010a 020a 0104 0208  ................
-000027b0: 0106 0116 0220 010e 010a 0310 010a 027a  ..... .........z
-000027c0: 0944 6963 742e 6475 6d70 6303 0000 0000  .Dict.dumpc.....
-000027d0: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-000027e0: 0000 0073 0c00 0000 7c02 7c00 7c01 3c00  ...s....|.|.|.<.
-000027f0: 6400 5300 7231 0000 0072 2200 0000 725e  d.S.r1...r"...r^
-00002800: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00002810: 0000 7257 0000 0050 0100 0073 0200 0000  ..rW...P...s....
-00002820: 0c01 7a0e 4469 6374 2e5f 7365 745f 6974  ..z.Dict._set_it
-00002830: 656d 727d 0000 0072 8300 0000 2909 7248  emr}...r....).rH
-00002840: 0000 0072 4900 0000 724a 0000 0072 6400  ...rI...rJ...rd.
-00002850: 0000 72a4 0000 0072 6600 0000 726e 0000  ..r....rf...rn..
-00002860: 0072 5700 0000 728b 0000 0072 2200 0000  .rW...r....r"...
-00002870: 7222 0000 0072 8900 0000 7223 0000 0072  r"...r....r#...r
-00002880: 3300 0000 1f01 0000 730c 0000 0008 000e  3.......s.......
-00002890: 0108 060c 030a 0310 2472 3300 0000 6300  ........$r3...c.
-000028a0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-000028b0: 0000 0000 0000 0073 5a00 0000 6500 5a01  .......sZ...e.Z.
-000028c0: 6400 5a02 6401 5a03 6412 8700 6601 6403  d.Z.d.Z.d...f.d.
-000028d0: 6404 8409 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
-000028e0: 6408 8400 5a06 8700 6601 6409 640a 8408  d...Z...f.d.d...
-000028f0: 5a07 640b 640c 8400 5a08 6413 640e 640f  Z.d.d...Z.d.d.d.
-00002900: 8401 5a09 6413 6410 6411 8401 5a0a 8700  ..Z.d.d.d...Z...
-00002910: 0400 5a0b 5300 2914 7234 0000 007a 1b52  ..Z.S.).r4...z.R
-00002920: 6570 7265 7365 6e74 7320 616e 204f 7065  epresents an Ope
-00002930: 6e46 6f61 6d20 6c69 7374 4e63 0300 0000  nFoam listNc....
-00002940: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00002950: 0300 0000 7316 0000 007c 027c 005f 0074  ....s....|.|._.t
-00002960: 0183 00a0 027c 01a1 0101 0064 0053 0072  .....|.....d.S.r
-00002970: 3100 0000 2903 729f 0000 0072 8800 0000  1...).r....r....
-00002980: 7264 0000 0029 0372 4500 0000 da08 6974  rd...).rE.....it
-00002990: 6572 6162 6c65 724e 0000 0072 8900 0000  erablerN...r....
-000029a0: 7222 0000 0072 2300 0000 7264 0000 0057  r"...r#...rd...W
-000029b0: 0100 0073 0400 0000 0601 1001 7a0d 4c69  ...s........z.Li
-000029c0: 7374 2e5f 5f69 6e69 745f 5f63 0100 0000  st.__init__c....
-000029d0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-000029e0: 4300 0000 72a2 0000 0072 3100 0000 72a3  C...r....r1...r.
-000029f0: 0000 0072 8f00 0000 7222 0000 0072 2200  ...r....r"...r".
-00002a00: 0000 7223 0000 0072 a400 0000 5b01 0000  ..r#...r....[...
-00002a10: 72a5 0000 007a 0d4c 6973 742e 6765 745f  r....z.List.get_
-00002a20: 6e61 6d65 6302 0000 0000 0000 0000 0000  namec...........
-00002a30: 0002 0000 0003 0000 0043 0000 0073 4800  .........C...sH.
-00002a40: 0000 7c00 6a00 6400 7500 720a 7c01 7c00  ..|.j.d.u.r.|.|.
-00002a50: 5f00 6400 5300 7401 7c00 6a00 7402 8302  _.d.S.t.|.j.t...
-00002a60: 7221 7c00 6a00 7c01 6b03 721f 7c01 6401  r!|.j.|.k.r.|.d.
-00002a70: 1700 7c00 6a00 1700 7c00 5f00 6400 5300  ..|.j...|._.d.S.
-00002a80: 6400 5300 7403 8300 8201 2902 4e72 6800  d.S.t.....).Nrh.
-00002a90: 0000 2904 729f 0000 0072 3200 0000 7250  ..).r....r2...rP
-00002aa0: 0000 00da 0c52 756e 7469 6d65 4572 726f  .....RuntimeErro
-00002ab0: 7229 0272 4500 0000 724e 0000 0072 2200  r).rE...rN...r".
-00002ac0: 0000 7222 0000 0072 2300 0000 da08 6164  ..r"...r#.....ad
-00002ad0: 645f 6e61 6d65 5e01 0000 730e 0000 000a  d_name^...s.....
-00002ae0: 010a 010c 010a 0114 0104 ff06 037a 0d4c  .............z.L
-00002af0: 6973 742e 6164 645f 6e61 6d65 6301 0000  ist.add_namec...
-00002b00: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00002b10: 0003 0000 0072 a600 0000 7231 0000 0072  .....r....r1...r
-00002b20: 8700 0000 728f 0000 0072 8900 0000 7222  ....r....r....r"
-00002b30: 0000 0072 2300 0000 7266 0000 0067 0100  ...r#...rf...g..
-00002b40: 0072 a700 0000 7a0d 4c69 7374 2e5f 5f72  .r....z.List.__r
-00002b50: 6570 725f 5f63 0200 0000 0000 0000 0000  epr__c..........
-00002b60: 0000 0200 0000 0300 0000 0300 0000 7314  ..............s.
-00002b70: 0000 0087 0087 0166 0264 0164 0284 0888  .......f.d.d....
-00002b80: 0144 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
-00002b90: 0000 0000 0000 0002 0000 0006 0000 0013  ................
-00002ba0: 0000 0073 1800 0000 6700 7c00 5d08 7d01  ...s....g.|.].}.
-00002bb0: 8801 a000 7c01 8800 a102 9102 7102 5300  ....|.......q.S.
-00002bc0: 7222 0000 00a9 01da 0a5f 6475 6d70 5f69  r"......._dump_i
-00002bd0: 7465 6d29 0272 3600 0000 da04 6974 656d  tem).r6.....item
-00002be0: a902 7282 0000 0072 4500 0000 7222 0000  ..r....rE...r"..
-00002bf0: 0072 2300 0000 da0a 3c6c 6973 7463 6f6d  .r#.....<listcom
-00002c00: 703e 6b01 0000 7302 0000 0018 007a 2b4c  p>k...s......z+L
-00002c10: 6973 742e 5f6d 616b 655f 6c69 7374 5f73  ist._make_list_s
-00002c20: 7472 696e 6773 2e3c 6c6f 6361 6c73 3e2e  trings.<locals>.
-00002c30: 3c6c 6973 7463 6f6d 703e 7222 0000 0072  <listcomp>r"...r
-00002c40: 8100 0000 7222 0000 0072 b200 0000 7223  ....r"...r....r#
-00002c50: 0000 00da 125f 6d61 6b65 5f6c 6973 745f  ....._make_list_
-00002c60: 7374 7269 6e67 736a 0100 0073 0200 0000  stringsj...s....
-00002c70: 1401 7a17 4c69 7374 2e5f 6d61 6b65 5f6c  ..z.List._make_l
-00002c80: 6973 745f 7374 7269 6e67 7372 0100 0000  ist_stringsr....
-00002c90: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00002ca0: 0004 0000 0043 0000 0073 3200 0000 7400  .....C...s2...t.
-00002cb0: 7c01 7401 7402 6602 8302 7211 7403 7c01  |.t.t.f...r.t.|.
-00002cc0: 6401 8302 7211 7c01 a004 7c02 a101 5300  d...r.|...|...S.
-00002cd0: 7c02 6402 1400 7405 7c01 8301 1700 5300  |.d...t.|.....S.
-00002ce0: 2903 4e72 6e00 0000 7268 0000 0029 0672  ).Nrn...rh...).r
-00002cf0: 3200 0000 7242 0000 0072 7e00 0000 7271  2...rB...r~...rq
-00002d00: 0000 0072 6e00 0000 7250 0000 0029 0372  ...rn...rP...).r
-00002d10: 4500 0000 72b1 0000 0072 8200 0000 7222  E...r....r....r"
-00002d20: 0000 0072 2200 0000 7223 0000 0072 b000  ...r"...r#...r..
-00002d30: 0000 6d01 0000 7306 0000 0018 010a 0110  ..m...s.........
-00002d40: 027a 0f4c 6973 742e 5f64 756d 705f 6974  .z.List._dump_it
-00002d50: 656d 6302 0000 0000 0000 0000 0000 0009  emc.............
-00002d60: 0000 0008 0000 0003 0000 0073 3c01 0000  ...........s<...
-00002d70: 6700 7d02 8800 6401 1400 7d03 8801 6a00  g.}...d...}...j.
-00002d80: 6400 7500 721f 7c02 a001 8801 6a02 6402  d.u.r.|.....j.d.
-00002d90: 6403 8d01 a101 0100 7c03 6404 1700 6401  d.......|.d...d.
-00002da0: a003 7c02 a101 1700 6405 1700 5300 7c02  ..|.....d...S.|.
-00002db0: a004 7c03 8801 6a00 1700 6406 7c03 9b00  ..|...j...d.|...
-00002dc0: 9d02 1700 6404 1700 a101 0100 6407 6408  ....d.......d.d.
-00002dd0: 6409 9c02 7d04 8801 6a00 7c04 a005 a100  d...}...j.|.....
-00002de0: 7601 7248 7c02 a004 6406 a003 8801 a002  v.rH|...d.......
-00002df0: 8800 640a 1700 a101 a101 a101 0100 6e4a  ..d...........nJ
-00002e00: 8801 7292 7c04 8801 6a00 1900 7d05 8801  ..r.|...j...}...
-00002e10: 6402 1900 7c05 6b02 7359 7406 8801 8301  d...|.k.sYt.....
-00002e20: 8201 6700 7d06 6400 7d07 8801 4400 5d18  ..g.}.d.}...D.].
-00002e30: 7d08 7c08 7c05 6b02 7272 7c07 6400 7501  }.|.|.k.rr|.d.u.
-00002e40: 726e 7c06 a004 7c07 a101 0100 7c08 6701  rn|...|.....|.g.
-00002e50: 7d07 715f 7c07 a004 7c08 a101 0100 715f  }.q_|...|.....q_
-00002e60: 7c06 a004 7c07 a101 0100 8701 6601 640b  |...|.......f.d.
-00002e70: 640c 8408 7c06 4400 8301 7d06 7c02 a001  d...|.D...}.|...
-00002e80: 8700 6601 640d 640e 8408 7c06 4400 8301  ..f.d.d...|.D...
-00002e90: a101 0100 7c02 a004 7c03 640f 1700 a101  ....|...|.d.....
-00002ea0: 0100 6406 a003 7c02 a101 5300 2910 4e72  ..d...|...S.).Nr
-00002eb0: 6800 0000 7201 0000 00a9 0172 8200 0000  h...r......r....
-00002ec0: fa01 2872 8e00 0000 726c 0000 00da 0368  ..(r....rl.....h
-00002ed0: 6578 5a06 7370 6c69 6e65 2902 da06 626c  exZ.spline)...bl
-00002ee0: 6f63 6b73 da05 6564 6765 7372 3a00 0000  ocks..edgesr:...
-00002ef0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002f00: 0007 0000 0013 0000 0073 2400 0000 6700  .........s$...g.
-00002f10: 7c00 5d0e 7d01 6400 a000 8700 6601 6401  |.].}.d.....f.d.
-00002f20: 6402 8408 7c01 4400 8301 a101 9102 7102  d...|.D.......q.
-00002f30: 5300 2903 7268 0000 0063 0100 0000 0000  S.).rh...c......
-00002f40: 0000 0000 0000 0200 0000 0400 0000 3300  ..............3.
-00002f50: 0000 731a 0000 0081 007c 005d 087d 0188  ..s......|.].}..
-00002f60: 00a0 007c 01a1 0156 0001 0071 0264 0053  ...|...V...q.d.S
-00002f70: 0072 3100 0000 72af 0000 0029 0272 3600  .r1...r....).r6.
-00002f80: 0000 5a05 5f69 7465 6d72 8f00 0000 7222  ..Z._itemr....r"
-00002f90: 0000 0072 2300 0000 7239 0000 008d 0100  ...r#...r9......
-00002fa0: 0072 9900 0000 7a27 4c69 7374 2e64 756d  .r....z'List.dum
-00002fb0: 702e 3c6c 6f63 616c 733e 2e3c 6c69 7374  p.<locals>.<list
-00002fc0: 636f 6d70 3e2e 3c67 656e 6578 7072 3e72  comp>.<genexpr>r
-00002fd0: 9d00 0000 2902 7236 0000 00da 0a69 7465  ....).r6.....ite
-00002fe0: 6d73 5f6c 696e 6572 8f00 0000 7222 0000  ms_liner....r"..
-00002ff0: 0072 2300 0000 72b3 0000 008c 0100 0073  .r#...r........s
-00003000: 0800 0000 0600 0202 16ff 06ff 7a1d 4c69  ............z.Li
-00003010: 7374 2e64 756d 702e 3c6c 6f63 616c 733e  st.dump.<locals>
-00003020: 2e3c 6c69 7374 636f 6d70 3e63 0100 0000  .<listcomp>c....
-00003030: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00003040: 3300 0000 7320 0000 0081 007c 005d 0b7d  3...s .....|.].}
-00003050: 0188 0064 0017 0064 0114 007c 0117 0056  ...d...d...|...V
-00003060: 0001 0071 0264 0253 0029 0372 3a00 0000  ...q.d.S.).r:...
-00003070: 7268 0000 004e 7222 0000 0029 0272 3600  rh...Nr"...).r6.
-00003080: 0000 72ab 0000 0072 b500 0000 7222 0000  ..r....r....r"..
-00003090: 0072 2300 0000 7239 0000 0090 0100 0073  .r#...r9.......s
-000030a0: 0400 0000 0280 1e00 7a1c 4c69 7374 2e64  ........z.List.d
-000030b0: 756d 702e 3c6c 6f63 616c 733e 2e3c 6765  ump.<locals>.<ge
-000030c0: 6e65 7870 723e 7a02 293b 2907 729f 0000  nexpr>z.);).r...
-000030d0: 00da 0665 7874 656e 6472 b400 0000 7229  ...extendr....r)
-000030e0: 0000 0072 2800 0000 da04 6b65 7973 723e  ...r(.....keysr>
-000030f0: 0000 0029 0972 4500 0000 7282 0000 0072  ...).rE...r....r
-00003100: 6500 0000 72aa 0000 00da 0c73 7065 6369  e...r......speci
-00003110: 616c 5f6b 6579 735a 0b73 7065 6369 616c  al_keysZ.special
-00003120: 5f6b 6579 da05 6c69 6e65 7372 ba00 0000  _key..linesr....
-00003130: 72b1 0000 0072 2200 0000 72b2 0000 0072  r....r"...r....r
-00003140: 2300 0000 726e 0000 0073 0100 0073 3800  #...rn...s...s8.
-00003150: 0000 0401 0801 0a01 1201 1601 1e02 0a01  ................
-00003160: 0e01 1c01 0401 0a01 0c01 0801 0401 0401  ................
-00003170: 0801 0801 0801 0a01 0801 0c02 0a01 0a01  ................
-00003180: 0202 06fe 1804 0e01 0a01 7a09 4c69 7374  ..........z.List
-00003190: 2e64 756d 7072 9600 0000 7283 0000 0029  .dumpr....r....)
-000031a0: 0c72 4800 0000 7249 0000 0072 4a00 0000  .rH...rI...rJ...
-000031b0: da07 5f5f 646f 635f 5f72 6400 0000 72a4  ..__doc__rd...r.
-000031c0: 0000 0072 ae00 0000 7266 0000 0072 b400  ...r....rf...r..
-000031d0: 0000 72b0 0000 0072 6e00 0000 728b 0000  ..r....rn...r...
-000031e0: 0072 2200 0000 7222 0000 0072 8900 0000  .r"...r"...r....
-000031f0: 7223 0000 0072 3400 0000 5401 0000 7312  r#...r4...T...s.
-00003200: 0000 0008 0004 010e 0208 0408 030c 0908  ................
-00003210: 030a 0312 0672 3400 0000 6300 0000 0000  .....r4...c.....
-00003220: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00003230: 0000 0073 1000 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00003240: 6401 5a03 6402 5300 2903 72a9 0000 007a  d.Z.d.S.).r....z
-00003250: 2241 2064 6963 7469 6f6e 6e61 7279 2074  "A dictionnary t
-00003260: 6f20 7374 6f72 6520 2363 6f64 6553 7472  o store #codeStr
-00003270: 6561 6d4e 2904 7248 0000 0072 4900 0000  eamN).rH...rI...
-00003280: 724a 0000 0072 bf00 0000 7222 0000 0072  rJ...r....r"...r
-00003290: 2200 0000 7222 0000 0072 2300 0000 72a9  "...r"...r#...r.
-000032a0: 0000 0095 0100 0073 0400 0000 0800 0801  .......s........
-000032b0: 72a9 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000032c0: 0000 0300 0000 0300 0000 0300 0000 7322  ..............s"
-000032d0: 0000 0087 0066 0164 0164 0284 087d 0187  .....f.d.d...}..
-000032e0: 0066 0164 0364 0484 087d 0274 007c 017c  .f.d.d...}.t.|.|
-000032f0: 0283 0253 0029 054e 6301 0000 0000 0000  ...S.).Nc.......
-00003300: 0000 0000 0001 0000 0002 0000 0013 0000  ................
-00003310: 0073 0a00 0000 7c00 8800 1900 6a00 5300  .s....|.....j.S.
-00003320: 7231 0000 00a9 01da 0463 6f64 6572 8f00  r1.......coder..
-00003330: 0000 725b 0000 0072 2200 0000 7223 0000  ..r[...r"...r#..
-00003340: 0072 5300 0000 9a01 0000 72a7 0000 007a  .rS.......r....z
-00003350: 185f 6d61 6b65 5f61 6c69 6173 2e3c 6c6f  ._make_alias.<lo
-00003360: 6361 6c73 3e2e 6765 7463 0200 0000 0000  cals>.getc......
-00003370: 0000 0000 0000 0200 0000 0300 0000 1300  ................
-00003380: 0000 730e 0000 007c 017c 0088 0019 005f  ..s....|.|....._
-00003390: 0064 0053 0072 3100 0000 72c0 0000 0029  .d.S.r1...r....)
-000033a0: 02da 055f 7365 6c66 7238 0000 0072 5b00  ..._selfr8...r[.
-000033b0: 0000 7222 0000 0072 2300 0000 da03 7365  ..r"...r#.....se
-000033c0: 749d 0100 0072 7c00 0000 7a18 5f6d 616b  t....r|...z._mak
-000033d0: 655f 616c 6961 732e 3c6c 6f63 616c 733e  e_alias.<locals>
-000033e0: 2e73 6574 2901 da08 7072 6f70 6572 7479  .set)...property
-000033f0: 2903 724e 0000 0072 5300 0000 72c3 0000  ).rN...rS...r...
-00003400: 0072 2200 0000 725b 0000 0072 2300 0000  .r"...r[...r#...
-00003410: da0b 5f6d 616b 655f 616c 6961 7399 0100  .._make_alias...
-00003420: 0073 0600 0000 0c01 0c03 0a03 72c5 0000  .s..........r...
-00003430: 0029 045a 0b63 6f64 6549 6e63 6c75 6465  .).Z.codeInclude
-00003440: 5a0b 636f 6465 4f70 7469 6f6e 735a 0863  Z.codeOptionsZ.c
-00003450: 6f64 654c 6962 7372 c100 0000 6300 0000  odeLibsr....c...
-00003460: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00003470: 0040 0000 0072 8c00 0000 290b da04 436f  .@...r....)...Co
-00003480: 6465 4e63 0400 0000 0000 0000 0000 0000  deNc............
-00003490: 0400 0000 0200 0000 4300 0000 731a 0000  ........C...s...
-000034a0: 007c 017c 005f 0074 017c 0283 017c 005f  .|.|._.t.|...|._
-000034b0: 027c 037c 005f 0364 0053 0072 3100 0000  .|.|._.d.S.r1...
-000034c0: 2904 724e 0000 0072 0600 0000 72c1 0000  ).rN...r....r...
-000034d0: 0072 a100 0000 2904 7245 0000 0072 4e00  .r....).rE...rN.
-000034e0: 0000 72c1 0000 0072 a100 0000 7222 0000  ..r....r....r"..
-000034f0: 0072 2200 0000 7223 0000 0072 6400 0000  .r"...r#...rd...
-00003500: a801 0000 7306 0000 0006 010a 010a 017a  ....s..........z
-00003510: 0d43 6f64 652e 5f5f 696e 6974 5f5f 6301  .Code.__init__c.
-00003520: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-00003530: 0000 0043 0000 0073 3e00 0000 7c00 6a00  ...C...s>...|.j.
-00003540: 6400 7500 7210 6401 7c00 6a01 6400 6402  d.u.r.d.|.j.d.d.
-00003550: 8502 1900 9b00 6403 9d03 5300 6401 7c00  ......d...S.d.|.
-00003560: 6a01 6400 6402 8502 1900 9b00 6404 7c00  j.d.d.......d.|.
-00003570: 6a00 9b00 6405 9d05 5300 2906 4e7a 0643  j...d...S.).Nz.C
-00003580: 6f64 6528 2272 3000 0000 7a07 5b2e 2e2e  ode("r0...z.[...
-00003590: 5d22 297a 125b 2e2e 2e5d 222c 2064 6972  ]")z.[...]", dir
-000035a0: 6563 7469 7665 3d72 8e00 0000 2902 72a1  ective=r....).r.
-000035b0: 0000 0072 c100 0000 728f 0000 0072 2200  ...r....r....r".
-000035c0: 0000 7222 0000 0072 2300 0000 7266 0000  ..r"...r#...rf..
-000035d0: 00ad 0100 0073 0600 0000 0a01 1601 1e01  .....s..........
-000035e0: 7a0d 436f 6465 2e5f 5f72 6570 725f 5f72  z.Code.__repr__r
-000035f0: 0100 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00003600: 0007 0000 0005 0000 0043 0000 0073 8a00  .........C...s..
-00003610: 0000 6700 7d02 7c01 6401 1400 7d03 7c01  ..g.}.|.d...}.|.
-00003620: 6402 1700 6401 1400 7d04 7c03 7c00 6a00  d...d...}.|.|.j.
-00003630: 1700 7d05 7c00 6a01 6400 7501 721d 7c05  ..}.|.j.d.u.r.|.
-00003640: 6401 7c00 6a01 1700 3700 7d05 7c02 a002  d.|.j...7.}.|...
-00003650: 7c05 6403 7c03 9b00 9d02 1700 6404 1700  |.d.|.......d...
-00003660: a101 0100 7c00 6a03 a004 6403 a101 4400  ....|.j...d...D.
-00003670: 5d09 7d06 7c02 a002 7c04 7c06 1700 a101  ].}.|...|.|.....
-00003680: 0100 712f 7c02 a002 7c03 6405 1700 a101  ..q/|...|.d.....
-00003690: 0100 6403 a005 7c02 a101 5300 2906 4e72  ..d...|...S.).Nr
-000036a0: 6800 0000 723a 0000 0072 6c00 0000 7a02  h...r:...rl...z.
-000036b0: 237b 7a03 237d 3b29 0672 4e00 0000 72a1  #{z.#};).rN...r.
-000036c0: 0000 0072 2800 0000 72c1 0000 0072 1a00  ...r(...r....r..
-000036d0: 0000 7229 0000 0029 0772 4500 0000 7282  ..r)...).rE...r.
-000036e0: 0000 0072 6500 0000 72aa 0000 005a 0c69  ...re...r....Z.i
-000036f0: 6e64 656e 7461 7469 6f6e 3472 1800 0000  ndentation4r....
-00003700: 72ab 0000 0072 2200 0000 7222 0000 0072  r....r"...r"...r
-00003710: 2300 0000 726e 0000 00b2 0100 0073 1600  #...rn.......s..
-00003720: 0000 0401 0801 0c01 0a01 0a01 0e01 1801  ................
-00003730: 1001 1001 0e01 0a01 7a09 436f 6465 2e64  ........z.Code.d
-00003740: 756d 7072 3100 0000 7283 0000 00a9 0672  umpr1...r......r
-00003750: 4800 0000 7249 0000 0072 4a00 0000 7264  H...rI...rJ...rd
-00003760: 0000 0072 6600 0000 726e 0000 0072 2200  ...rf...rn...r".
-00003770: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00003780: 0072 c600 0000 a701 0000 7308 0000 0008  .r........s.....
-00003790: 000a 0108 050e 0572 c600 0000 6300 0000  .......r....c...
-000037a0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-000037b0: 0040 0000 0072 8c00 0000 290b da04 4e61  .@...r....)...Na
-000037c0: 6d65 4e63 0300 0000 0000 0000 0000 0000  meNc............
-000037d0: 0300 0000 0200 0000 4300 0000 f310 0000  ........C.......
-000037e0: 007c 017c 005f 007c 027c 005f 0164 0053  .|.|._.|.|._.d.S
-000037f0: 0072 3100 0000 2902 724e 0000 0072 3800  .r1...).rN...r8.
-00003800: 0000 2903 7245 0000 0072 4e00 0000 7238  ..).rE...rN...r8
-00003810: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00003820: 0000 7264 0000 00c2 0100 00f3 0400 0000  ..rd............
-00003830: 0601 0a01 7a0d 4e61 6d65 2e5f 5f69 6e69  ....z.Name.__ini
-00003840: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00003850: 0100 0000 0300 0000 4300 0000 730e 0000  ........C...s...
-00003860: 0064 017c 006a 009b 0064 029d 0353 0029  .d.|.j...d...S.)
-00003870: 034e 7a05 4e61 6d65 2872 8e00 0000 725b  .Nz.Name(r....r[
-00003880: 0000 0072 8f00 0000 7222 0000 0072 2200  ...r....r"...r".
-00003890: 0000 7223 0000 0072 6600 0000 c601 0000  ..r#...rf.......
-000038a0: 727c 0000 007a 0d4e 616d 652e 5f5f 7265  r|...z.Name.__re
-000038b0: 7072 5f5f 7201 0000 0063 0200 0000 0000  pr__r....c......
-000038c0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-000038d0: 0000 7308 0000 007c 006a 009b 0053 0072  ..s....|.j...S.r
-000038e0: 3100 0000 725b 0000 0072 8100 0000 7222  1...r[...r....r"
-000038f0: 0000 0072 2200 0000 7223 0000 0072 6e00  ...r"...r#...rn.
-00003900: 0000 c901 0000 729b 0000 007a 094e 616d  ......r....z.Nam
-00003910: 652e 6475 6d70 7231 0000 0072 8300 0000  e.dumpr1...r....
-00003920: 72c7 0000 0072 2200 0000 7222 0000 0072  r....r"...r"...r
-00003930: 2200 0000 7223 0000 0072 c800 0000 c001  "...r#...r......
-00003940: 0000 7308 0000 0008 000a 0208 040e 0372  ..s............r
-00003950: c800 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00003960: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
-00003970: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
-00003980: 5a03 6403 6404 8400 5a04 6409 6406 6407  Z.d.d...Z.d.d.d.
-00003990: 8401 5a05 6408 5300 290a da09 4469 7265  ..Z.d.S.)...Dire
-000039a0: 6374 6976 6563 0300 0000 0000 0000 0000  ctivec..........
-000039b0: 0000 0300 0000 0200 0000 4300 0000 72c9  ..........C...r.
-000039c0: 0000 0072 3100 0000 a902 72a1 0000 00da  ...r1.....r.....
-000039d0: 0763 6f6e 7465 6e74 2903 7245 0000 0072  .content).rE...r
-000039e0: a100 0000 72cd 0000 0072 2200 0000 7222  ....r....r"...r"
-000039f0: 0000 0072 2300 0000 7264 0000 00ce 0100  ...r#...rd......
-00003a00: 0072 ca00 0000 7a12 4469 7265 6374 6976  .r....z.Directiv
-00003a10: 652e 5f5f 696e 6974 5f5f 6301 0000 0000  e.__init__c.....
-00003a20: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00003a30: 0000 0073 1200 0000 7c00 6a00 9b00 6401  ...s....|.j...d.
-00003a40: 7c00 6a01 9b00 9d03 5300 2902 4e72 8000  |.j.....S.).Nr..
-00003a50: 0000 72cc 0000 0072 8f00 0000 7222 0000  ..r....r....r"..
-00003a60: 0072 2200 0000 7223 0000 0072 6600 0000  .r"...r#...rf...
-00003a70: d201 0000 7302 0000 0012 017a 1244 6972  ....s......z.Dir
-00003a80: 6563 7469 7665 2e5f 5f72 6570 725f 5f72  ective.__repr__r
-00003a90: 0100 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00003aa0: 0002 0000 0005 0000 0043 0000 0073 1c00  .........C...s..
-00003ab0: 0000 7c01 6401 1400 7c00 6a00 9b00 6402  ..|.d...|.j...d.
-00003ac0: 7c00 6a01 9b00 6403 9d04 1700 5300 2904  |.j...d.....S.).
-00003ad0: 4e72 6800 0000 7280 0000 0072 6a00 0000  Nrh...r....rj...
-00003ae0: 72cc 0000 0072 8100 0000 7222 0000 0072  r....r....r"...r
-00003af0: 2200 0000 7223 0000 0072 6e00 0000 d501  "...r#...rn.....
-00003b00: 0000 729e 0000 007a 0e44 6972 6563 7469  ..r....z.Directi
-00003b10: 7665 2e64 756d 704e 7283 0000 0072 c700  ve.dumpNr....r..
-00003b20: 0000 7222 0000 0072 2200 0000 7222 0000  ..r"...r"...r"..
-00003b30: 0072 2300 0000 72cb 0000 00cd 0100 0073  .r#...r........s
-00003b40: 0800 0000 0800 0801 0804 0e03 72cb 0000  ............r...
-00003b50: 0029 0172 3000 0000 2925 72bf 0000 0072  .).r0...)%r....r
-00003b60: 1600 0000 da03 6162 6372 0200 0000 7203  ......abcr....r.
-00003b70: 0000 00da 0b64 6174 6163 6c61 7373 6573  .....dataclasses
-00003b80: 7204 0000 00da 076e 756d 6265 7273 7205  r......numbersr.
-00003b90: 0000 00da 0874 6578 7477 7261 7072 0600  .....textwrapr..
-00003ba0: 0000 da06 7479 7069 6e67 7207 0000 005a  ....typingr....Z
-00003bb0: 0a69 6e66 6c65 6374 696f 6e72 0800 0000  .inflectionr....
-00003bc0: 721c 0000 0072 2400 0000 722f 0000 0072  r....r$...r/...r
-00003bd0: 4100 0000 7242 0000 0072 4b00 0000 725f  A...rB...rK...r_
-00003be0: 0000 0072 7e00 0000 7286 0000 0072 5d00  ...r~...r....r].
-00003bf0: 0000 7252 0000 0072 9700 0000 7255 0000  ..rR...r....rU..
-00003c00: 0072 3300 0000 7234 0000 0072 a900 0000  .r3...r4...r....
-00003c10: 72c5 0000 0072 9f00 0000 da07 7365 7461  r....r......seta
-00003c20: 7474 7272 c600 0000 72c8 0000 0072 cb00  ttrr....r....r..
-00003c30: 0000 7222 0000 0072 2200 0000 7222 0000  ..r"...r"...r"..
-00003c40: 0072 2300 0000 da08 3c6d 6f64 756c 653e  .r#.....<module>
-00003c50: 0100 0000 733e 0000 0004 0008 0210 010c  ....s>..........
-00003c60: 010c 010c 010c 010c 0208 0208 0308 1b0a  ................
-00003c70: 120e 1110 0712 3a02 4510 0110 0b02 0c12  ......:.E.......
-00003c80: 0112 2614 0d12 3510 4108 0408 0a16 0110  ..&...5.A.......
-00003c90: 0302 1912 0114 0c                        .......
+00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6402 6c0d  d.l.m.Z...d.d.l.
+00000080: 5a0e 6401 6408 6c0f 6d10 5a10 0100 6700  Z.d.d.l.m.Z...g.
+00000090: 6409 a201 5a11 640a 640b 8400 5a12 640c  d...Z.d.d...Z.d.
+000000a0: 640d 8400 5a13 642e 640f 6410 8401 5a14  d...Z.d.d.d...Z.
+000000b0: 4700 6411 6412 8400 6412 8302 5a15 4700  G.d.d...d...Z.G.
+000000c0: 6413 6414 8400 6414 6503 8303 5a16 4700  d.d...d.e...Z.G.
+000000d0: 6415 6416 8400 6416 6515 6516 8304 5a17  d.d...d.e.e...Z.
+000000e0: 6506 4700 6417 6418 8400 6418 8302 8301  e.G.d.d...d.....
+000000f0: 5a18 4700 6419 641a 8400 641a 6518 8303  Z.G.d.d...d.e...
+00000100: 5a19 6506 4700 641b 641c 8400 641c 6515  Z.e.G.d.d...d.e.
+00000110: 8303 8301 5a1a 4700 641d 641e 8400 641e  ....Z.G.d.d...d.
+00000120: 651b 6515 8304 5a1c 4700 641f 6420 8400  e.e...Z.G.d.d ..
+00000130: 6420 651d 6515 6516 8305 5a1e 4700 6421  d e.e.e...Z.G.d!
+00000140: 6422 8400 6422 651b 6515 8304 5a1f 4700  d"..d"e.e...Z.G.
+00000150: 6423 6424 8400 6424 651e 8303 5a20 6425  d#d$..d$e...Z d%
+00000160: 6426 8400 5a21 6427 4400 5d0c 5a22 6523  d&..Z!d'D.].Z"e#
+00000170: 6520 6510 6522 8301 6521 6522 8301 8303  e e.e"..e!e"....
+00000180: 0100 719e 4700 6428 6429 8400 6429 6515  ..q.G.d(d)..d)e.
+00000190: 8303 5a24 6506 4700 642a 642b 8400 642b  ..Z$e.G.d*d+..d+
+000001a0: 6515 8303 8301 5a25 4700 642c 642d 8400  e.....Z%G.d,d-..
+000001b0: 642d 6515 8303 5a26 6402 5300 292f 7a2e  d-e...Z&d.S.)/z.
+000001c0: 4162 7374 7261 6374 2053 796e 7461 7820  Abstract Syntax 
+000001d0: 5472 6565 7320 666f 7220 4f70 656e 464f  Trees for OpenFO
+000001e0: 414d 2069 6e70 7574 2066 696c 6573 e900  AM input files..
+000001f0: 0000 004e 2902 da03 4142 43da 0e61 6273  ...N)...ABC..abs
+00000200: 7472 6163 746d 6574 686f 6429 01da 0964  tractmethod)...d
+00000210: 6174 6163 6c61 7373 2901 da06 4e75 6d62  ataclass)...Numb
+00000220: 6572 2901 da06 6465 6465 6e74 2901 da08  er)...dedent)...
+00000230: 4f70 7469 6f6e 616c 2901 da0a 756e 6465  Optional)...unde
+00000240: 7273 636f 7265 2907 5a02 6b67 da01 6dda  rscore).Z.kg..m.
+00000250: 0173 da01 4b5a 046b 6d6f 6cda 0141 da02  .s..KZ.kmol..A..
+00000260: 6364 6301 0000 0000 0000 0000 0000 0009  cdc.............
+00000270: 0000 0008 0000 0043 0000 0073 d600 0000  .......C...s....
+00000280: 6401 6701 6402 1400 7d01 6403 7d02 7c00  d.g.d...}.d.}.|.
+00000290: 7269 7a0a 7400 a001 6404 7c00 a102 a002  riz.t...d.|.....
+000002a0: a100 7d03 5700 6e0f 0400 7403 7922 0100  ..}.W.n...t.y"..
+000002b0: 0100 0100 7c00 7d04 6405 7d00 6406 7d05  ....|.}.d.}.d.}.
+000002c0: 5900 6e19 7700 7c00 7c03 1900 7d05 7c05  Y.n.w.|.|...}.|.
+000002d0: 6407 7600 732d 4a00 8201 7c00 6400 7c03  d.v.s-J...|.d.|.
+000002e0: 8502 1900 7d04 7c00 7c03 6403 1700 6400  ....}.|.|.d...d.
+000002f0: 8502 1900 7d00 6408 7c04 7600 724b 7c04  ....}.d.|.v.rK|.
+00000300: a004 6408 a101 5c02 7d06 7d07 7405 7c07  ..d...\.}.}.t.|.
+00000310: 8301 7d07 6e05 7c04 6403 0202 7d06 7d07  ..}.n.|.d...}.}.
+00000320: 7c06 6409 6b03 725f 7406 a007 7c06 a101  |.d.k.r_t...|...
+00000330: 7d08 7c02 7c07 1400 7c01 7c08 3c00 7c05  }.|.|...|.|.<.|.
+00000340: 6406 6b02 7265 6403 6e01 640a 7d02 7c00  d.k.red.n.d.}.|.
+00000350: 7309 7c01 5300 290b 4e72 0100 0000 e907  s.|.S.).Nr......
+00000360: 0000 00e9 0100 0000 7a04 5b2f 2e5d da00  ........z.[/.]..
+00000370: da01 2e7a 022f 2efa 015e da01 31e9 ffff  ...z./...^..1...
+00000380: ffff 2908 da02 7265 da06 7365 6172 6368  ..)...re..search
+00000390: da05 7374 6172 74da 0e41 7474 7269 6275  ..start..Attribu
+000003a0: 7465 4572 726f 72da 0573 706c 6974 da03  teError..split..
+000003b0: 696e 74da 0773 796d 626f 6c73 da05 696e  int..symbols..in
+000003c0: 6465 7829 09da 0575 6e69 7473 da06 7265  dex)...units..re
+000003d0: 7375 6c74 da04 7369 676e 721c 0000 005a  sult..signr....Z
+000003e0: 0875 6e69 745f 616c 6c5a 096e 6578 745f  .unit_allZ.next_
+000003f0: 6f70 6572 da09 756e 6974 5f6e 616d 655a  oper..unit_nameZ
+00000400: 0a75 6e69 745f 7661 6c75 655a 0a75 6e69  .unit_valueZ.uni
+00000410: 745f 696e 6465 78a9 0072 2100 0000 fa46  t_index..r!....F
+00000420: 2f68 6f6d 652f 7069 6572 7265 2f44 6576  /home/pierre/Dev
+00000430: 2f66 6c75 6964 7369 6d66 6f61 6d2f 7372  /fluidsimfoam/sr
+00000440: 632f 666c 7569 6473 696d 666f 616d 2f66  c/fluidsimfoam/f
+00000450: 6f61 6d5f 696e 7075 745f 6669 6c65 732f  oam_input_files/
+00000460: 6173 742e 7079 da0e 7374 7232 666f 616d  ast.py..str2foam
+00000470: 5f75 6e69 7473 1000 0000 7330 0000 000a  _units....s0....
+00000480: 0104 0104 0102 0114 010c 0104 0104 0108  ................
+00000490: 0102 fd08 050c 010c 0110 0108 010e 010a  ................
+000004a0: 010a 0208 010a 010c 0110 0104 ec04 1572  ...............r
+000004b0: 2300 0000 6301 0000 0000 0000 0000 0000  #...c...........
+000004c0: 0005 0000 0008 0000 0043 0000 0073 a800  .........C...s..
+000004d0: 0000 6700 7d01 7400 7401 7c00 8302 4400  ..g.}.t.t.|...D.
+000004e0: 5d2f 5c02 7d02 7d03 7c03 6401 6b02 7210  ]/\.}.}.|.d.k.r.
+000004f0: 7107 7c03 6401 6b04 7216 6402 6e01 6403  q.|.d.k.r.d.n.d.
+00000500: 7d04 7402 7c03 8301 6404 6b02 7228 7c01  }.t.|...d.k.r(|.
+00000510: a003 7c04 9b00 7c02 9b00 9d02 a101 0100  ..|...|.........
+00000520: 7107 7c01 a003 7c04 9b00 7c02 9b00 6405  q.|...|...|...d.
+00000530: 7402 7c03 8301 9b00 9d04 a101 0100 7107  t.|...........q.
+00000540: 6406 a004 7c01 a101 7d01 7c01 a005 6402  d...|...}.|...d.
+00000550: a101 7249 7c01 6404 6400 8502 1900 7d01  ..rI|.d.d.....}.
+00000560: 7c01 5300 7c01 a005 6403 a101 7252 6407  |.S.|...d...rRd.
+00000570: 7c01 1700 7d01 7c01 5300 2908 4e72 0100  |...}.|.S.).Nr..
+00000580: 0000 7211 0000 00fa 012f 720f 0000 0072  ..r....../r....r
+00000590: 1200 0000 7210 0000 0072 1300 0000 2906  ....r....r....).
+000005a0: da03 7a69 7072 1b00 0000 da03 6162 73da  ..zipr......abs.
+000005b0: 0661 7070 656e 64da 046a 6f69 6eda 0a73  .append..join..s
+000005c0: 7461 7274 7377 6974 6829 05da 0a66 6f61  tartswith)...foa
+000005d0: 6d5f 756e 6974 7372 1e00 0000 da06 7379  m_unitsr......sy
+000005e0: 6d62 6f6c da08 6578 706f 6e65 6e74 da08  mbol..exponent..
+000005f0: 6f70 6572 6174 6f72 7221 0000 0072 2100  operatorr!...r!.
+00000600: 0000 7222 0000 00da 0e66 6f61 6d5f 756e  ..r".....foam_un
+00000610: 6974 7332 7374 722b 0000 0073 1e00 0000  its2str+...s....
+00000620: 0401 1201 0801 0201 1001 0c01 1401 1e02  ................
+00000630: 0a01 0a01 0c01 0403 0afe 0801 0401 722e  ..............r.
+00000640: 0000 00e9 1400 0000 6302 0000 0000 0000  ........c.......
+00000650: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
+00000660: 0073 4400 0000 7a10 7400 7c01 7401 6401  .sD...z.t.|.t.d.
+00000670: 6402 8400 7c00 a002 a100 4400 8301 8301  d...|.....D.....
+00000680: 8302 7d01 5700 6e0b 0400 7403 791b 0100  ..}.W.n...t.y...
+00000690: 0100 0100 6403 7d01 5900 6e01 7700 6404  ....d.}.Y.n.w.d.
+000006a0: 7d02 7c01 7c02 1700 5300 2905 4e63 0100  }.|.|...S.).Nc..
+000006b0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+000006c0: 0000 7300 0000 732a 0000 0081 007c 005d  ..s...s*.....|.]
+000006d0: 105c 027d 017d 0274 007c 0274 0174 0266  .\.}.}.t.|.t.t.f
+000006e0: 0283 0273 0274 037c 0183 0156 0001 0071  ...s.t.|...V...q
+000006f0: 0264 0053 00a9 014e 2904 da0a 6973 696e  .d.S...N)...isin
+00000700: 7374 616e 6365 da04 4469 6374 da04 4c69  stance..Dict..Li
+00000710: 7374 da03 6c65 6e29 03da 022e 30da 036b  st..len)....0..k
+00000720: 6579 da05 7661 6c75 6572 2100 0000 7221  ey..valuer!...r!
+00000730: 0000 0072 2200 0000 da09 3c67 656e 6578  ...r".....<genex
+00000740: 7072 3e41 0000 0073 0e00 0000 0280 0400  pr>A...s........
+00000750: 0602 0c01 02fd 0601 0aff 7a2b 5f63 6f6d  ..........z+_com
+00000760: 7075 7465 5f73 7061 6365 735f 746f 5f61  pute_spaces_to_a
+00000770: 6c69 676e 2e3c 6c6f 6361 6c73 3e2e 3c67  lign.<locals>.<g
+00000780: 656e 6578 7072 3e72 0100 0000 e904 0000  enexpr>r........
+00000790: 0029 04da 036d 696e da03 6d61 78da 0569  .)...min..max..i
+000007a0: 7465 6d73 da0a 5661 6c75 6545 7272 6f72  tems..ValueError
+000007b0: 2903 da04 6461 7461 da0a 6d61 785f 6c65  )...data..max_le
+000007c0: 6e67 7468 5a0d 6465 6661 756c 745f 7370  ngthZ.default_sp
+000007d0: 6163 6572 2100 0000 7221 0000 0072 2200  acer!...r!...r".
+000007e0: 0000 da18 5f63 6f6d 7075 7465 5f73 7061  ...._compute_spa
+000007f0: 6365 735f 746f 5f61 6c69 676e 3d00 0000  ces_to_align=...
+00000800: 7318 0000 0002 0102 0102 0108 0106 0206  s...............
+00000810: fe08 fe0c 0808 0102 ff04 0308 0172 4000  .............r@.
+00000820: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000830: 0000 0002 0000 0040 0000 0073 1400 0000  .......@...s....
+00000840: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
+00000850: 6403 5300 2904 da04 4e6f 6465 6302 0000  d.S.)...Nodec...
+00000860: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00000870: 0043 0000 0073 2000 0000 7400 7c01 8301  .C...s ...t.|...
+00000880: 7400 7c00 8301 7500 720e 7c00 6a01 7c01  t.|...u.r.|.j.|.
+00000890: 6a01 6b02 5300 6401 5300 2902 4e46 2902  j.k.S.d.S.).NF).
+000008a0: da04 7479 7065 da08 5f5f 6469 6374 5f5f  ..type..__dict__
+000008b0: 2902 da04 7365 6c66 da05 6f74 6865 7272  )...self..otherr
+000008c0: 2100 0000 7221 0000 0072 2200 0000 da06  !...r!...r".....
+000008d0: 5f5f 6571 5f5f 4f00 0000 7306 0000 0010  __eq__O...s.....
+000008e0: 010c 0104 017a 0b4e 6f64 652e 5f5f 6571  .....z.Node.__eq
+000008f0: 5f5f 4e29 04da 085f 5f6e 616d 655f 5fda  __N)...__name__.
+00000900: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000910: 7561 6c6e 616d 655f 5f72 4600 0000 7221  ualname__rF...r!
+00000920: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00000930: 0000 7241 0000 004e 0000 0073 0400 0000  ..rA...N...s....
+00000940: 0800 0c01 7241 0000 0063 0000 0000 0000  ....rA...c......
+00000950: 0000 0000 0000 0000 0000 0800 0000 4000  ..............@.
+00000960: 0000 7350 0000 0065 005a 0164 005a 0209  ..sP...e.Z.d.Z..
+00000970: 0109 0209 0164 0e64 0365 0364 0465 0465  .....d.d.e.d.e.e
+00000980: 0319 0064 0565 0465 0319 0066 0664 0664  ...d.e.e...f.d.d
+00000990: 0784 055a 0564 0864 0984 005a 0664 0f64  ...Z.d.d...Z.d.d
+000009a0: 0a64 0b84 015a 0765 0864 0c64 0d84 0083  .d...Z.e.d.d....
+000009b0: 015a 0964 0153 0029 10da 0e4e 6f64 654c  .Z.d.S.)...NodeL
+000009c0: 696b 6550 7944 6963 744e 4672 3e00 0000  ikePyDictNFr>...
+000009d0: da0a 6469 6d65 6e73 696f 6e73 da08 636f  ..dimensions..co
+000009e0: 6d6d 656e 7473 6305 0000 0000 0000 0000  mmentsc.........
+000009f0: 0000 000b 0000 0007 0000 0043 0000 0073  ...........C...s
+00000a00: fa00 0000 7c02 6400 7500 7206 6900 7d02  ....|.d.u.r.i.}.
+00000a10: 7c04 6400 7500 720c 6900 7d04 7c01 a000  |.d.u.r.i.}.|...
+00000a20: a100 4400 5d6a 5c02 7d05 7d06 7401 7c06  ..D.]j\.}.}.t.|.
+00000a30: 7402 6400 8301 7403 6602 8302 7224 7c00  t.d...t.f...r$|.
+00000a40: a004 7c05 7c06 a102 0100 7110 7401 7c06  ..|.|.....q.t.|.
+00000a50: 7405 7406 6602 8302 724d 7c03 6401 7500  t.t.f...rM|.d.u.
+00000a60: 7236 7c00 a004 7c05 7c06 a102 0100 7110  r6|...|.|.....q.
+00000a70: 7c02 a007 7c05 7c03 a102 7d07 7401 7c06  |...|.|...}.t.|.
+00000a80: 7406 8302 7245 7408 7c06 8301 7d06 7c00  t...rEt.|...}.|.
+00000a90: a009 7c05 7c06 7c07 a103 0100 7110 7401  ..|.|.|.....q.t.
+00000aa0: 7c06 740a 8302 7275 7c02 a007 7c05 6400  |.t...ru|...|.d.
+00000ab0: a102 7d08 7c04 a007 7c05 6400 a102 7d09  ..}.|...|.d...}.
+00000ac0: 740b 6900 7c05 7c09 6402 8d03 7d0a 7c0a  t.i.|.|.d...}.|.
+00000ad0: 6a0c 7c06 7c08 7c03 7c09 6403 8d04 0100  j.|.|.|.|.d.....
+00000ae0: 7c00 a00d 7c05 7c0a a102 0100 7110 740e  |...|.|.....q.t.
+00000af0: 7402 7c06 8301 8301 8201 6400 5300 2904  t.|.......d.S.).
+00000b00: 4e46 2902 da04 6e61 6d65 724c 0000 0029  NF)...namerL...)
+00000b10: 0372 4b00 0000 da11 6465 6661 756c 745f  .rK.....default_
+00000b20: 6469 6d65 6e73 696f 6e72 4c00 0000 290f  dimensionrL...).
+00000b30: 723c 0000 0072 3100 0000 7242 0000 00da  r<...r1...rB....
+00000b40: 0373 7472 da09 7365 745f 6368 696c 6472  .str..set_childr
+00000b50: 0500 0000 da04 6c69 7374 da03 6765 7472  ......list..getr
+00000b60: 3300 0000 da09 7365 745f 7661 6c75 65da  3.....set_value.
+00000b70: 0464 6963 7472 3200 0000 da14 696e 6974  .dictr2.....init
+00000b80: 5f66 726f 6d5f 7079 5f6f 626a 6563 7473  _from_py_objects
+00000b90: da09 5f73 6574 5f69 7465 6dda 134e 6f74  .._set_item..Not
+00000ba0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00000bb0: 290b 7244 0000 0072 3e00 0000 724b 0000  ).rD...r>...rK..
+00000bc0: 0072 4e00 0000 724c 0000 0072 3600 0000  .rN...rL...r6...
+00000bd0: 7237 0000 00da 0964 696d 656e 7369 6f6e  r7.....dimension
+00000be0: 5a0f 6469 6d65 6e73 696f 6e73 5f64 6963  Z.dimensions_dic
+00000bf0: 745a 0d63 6f6d 6d65 6e74 735f 6469 6374  tZ.comments_dict
+00000c00: da03 6f62 6a72 2100 0000 7221 0000 0072  ..objr!...r!...r
+00000c10: 2200 0000 7255 0000 0056 0000 0073 3600  "...rU...V...s6.
+00000c20: 0000 0807 0401 0801 0401 1001 1201 0e01  ................
+00000c30: 0e01 0801 0e01 0c02 0a01 0801 1001 0a01  ................
+00000c40: 0c01 0c01 0e01 0401 0201 0201 0201 0201  ................
+00000c50: 06fc 0e06 0c02 04e9 7a23 4e6f 6465 4c69  ........z#NodeLi
+00000c60: 6b65 5079 4469 6374 2e69 6e69 745f 6672  kePyDict.init_fr
+00000c70: 6f6d 5f70 795f 6f62 6a65 6374 7363 0300  om_py_objectsc..
+00000c80: 0000 0000 0000 0000 0000 0600 0000 0600  ................
+00000c90: 0000 4300 0000 733a 0100 0074 007c 0274  ..C...s:...t.|.t
+00000ca0: 0183 0272 227c 0272 2274 007c 0264 0119  ...r"|.r"t.|.d..
+00000cb0: 0074 0183 0272 227c 0264 0119 0072 2274  .t...r"|.d...r"t
+00000cc0: 0264 0264 0384 007c 0264 0119 0044 0083  .d.d...|.d...D..
+00000cd0: 0183 0172 2274 03a0 047c 02a1 017d 0274  ...r"t...|...}.t
+00000ce0: 007c 0274 0564 0083 0174 0674 0774 0866  .|.t.d...t.t.t.f
+00000cf0: 0483 0272 2e6e 6774 007c 0274 0983 0272  ...r.ngt.|.t...r
+00000d00: 3a74 0a7c 027c 0164 048d 027d 026e 5b74  :t.|.|.d...}.n[t
+00000d10: 007c 0274 0183 0272 4674 0b7c 027c 0164  .|.t...rFt.|.|.d
+00000d20: 048d 027d 026e 4f74 007c 0274 036a 0c83  ...}.nOt.|.t.j..
+00000d30: 0272 897c 026a 0d7d 037c 026a 0e7d 047c  .r.|.j.}.|.j.}.|
+00000d40: 02a0 0fa1 0001 0064 007d 057c 0464 056b  .......d.}.|.d.k
+00000d50: 0272 787c 0364 0619 0064 076b 0272 6564  .rx|.d...d.k.red
+00000d60: 087d 056e 0b7c 0364 0619 0064 096b 0272  .}.n.|.d...d.k.r
+00000d70: 6e64 0a7d 056e 0274 1082 0164 0b64 0c84  nd.}.n.t...d.d..
+00000d80: 007c 0244 0083 017d 026e 097c 0464 066b  .|.D...}.n.|.d.k
+00000d90: 0272 7f64 0d7d 056e 0274 1082 0174 0b7c  .r.d.}.n.t...t.|
+00000da0: 027c 017c 0564 0e8d 037d 026e 0c74 007c  .|.|.d...}.n.t.|
+00000db0: 0274 1183 0272 8f6e 0674 1074 057c 0283  .t...r.n.t.t.|..
+00000dc0: 0183 0182 017c 00a0 127c 017c 02a1 0201  .....|...|.|....
+00000dd0: 0064 0053 0029 0f4e 7201 0000 0063 0100  .d.S.).Nr....c..
+00000de0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000df0: 0000 7300 0000 f31a 0000 0081 007c 005d  ..s..........|.]
+00000e00: 087d 0174 007c 0174 0183 0256 0001 0071  .}.t.|.t...V...q
+00000e10: 0264 0053 0072 3000 0000 2902 7231 0000  .d.S.r0...).r1..
+00000e20: 0072 0500 0000 2902 7235 0000 00da 016e  .r....).r5.....n
+00000e30: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
+00000e40: 3800 0000 8000 0000 f304 0000 0002 8018  8...............
+00000e50: 007a 2b4e 6f64 654c 696b 6550 7944 6963  .z+NodeLikePyDic
+00000e60: 742e 7365 745f 6368 696c 642e 3c6c 6f63  t.set_child.<loc
+00000e70: 616c 733e 2e3c 6765 6e65 7870 723e a901  als>.<genexpr>..
+00000e80: 724d 0000 00e9 0200 0000 720f 0000 00e9  rM........r.....
+00000e90: 0900 0000 da06 7465 6e73 6f72 e903 0000  ......tensor....
+00000ea0: 00da 0676 6563 746f 7263 0100 0000 0000  ...vectorc......
+00000eb0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
+00000ec0: 0000 7314 0000 0067 007c 005d 067d 0174  ..s....g.|.].}.t
+00000ed0: 007c 0183 0191 0271 0253 0072 2100 0000  .|.....q.S.r!...
+00000ee0: 2901 7233 0000 0029 0272 3500 0000 da08  ).r3...).r5.....
+00000ef0: 7365 7175 656e 6365 7221 0000 0072 2100  sequencer!...r!.
+00000f00: 0000 7222 0000 00da 0a3c 6c69 7374 636f  ..r".....<listco
+00000f10: 6d70 3e96 0000 0073 0200 0000 1400 7a2c  mp>....s......z,
+00000f20: 4e6f 6465 4c69 6b65 5079 4469 6374 2e73  NodeLikePyDict.s
+00000f30: 6574 5f63 6869 6c64 2e3c 6c6f 6361 6c73  et_child.<locals
+00000f40: 3e2e 3c6c 6973 7463 6f6d 703e da06 7363  >.<listcomp>..sc
+00000f50: 616c 6172 2902 724d 0000 00da 0564 7479  alar).rM.....dty
+00000f60: 7065 2913 7231 0000 0072 5100 0000 da03  pe).r1...rQ.....
+00000f70: 616c 6cda 026e 70da 0561 7272 6179 7242  all..np..arrayrB
+00000f80: 0000 0072 4f00 0000 7205 0000 00da 0c44  ...rO...r......D
+00000f90: 696d 656e 7369 6f6e 5365 7472 5400 0000  imensionSetrT...
+00000fa0: 7232 0000 0072 3300 0000 da07 6e64 6172  r2...r3.....ndar
+00000fb0: 7261 79da 0573 6861 7065 da04 6e64 696d  ray..shape..ndim
+00000fc0: da06 746f 6c69 7374 7257 0000 0072 4100  ..tolistrW...rA.
+00000fd0: 0000 7256 0000 0029 0672 4400 0000 7236  ..rV...).rD...r6
+00000fe0: 0000 00da 0563 6869 6c64 726c 0000 0072  .....childrl...r
+00000ff0: 6d00 0000 7266 0000 0072 2100 0000 7221  m...rf...r!...r!
+00001000: 0000 0072 2200 0000 7250 0000 007a 0000  ...r"...rP...z..
+00001010: 0073 4a00 0000 0802 02ff 0202 02fe 0c03  .sJ.............
+00001020: 02fd 0604 02fc 1405 02fb 0a07 1602 0201  ................
+00001030: 0a01 0e01 0a01 0e01 0c01 0601 0601 0801  ................
+00001040: 0401 0801 0c01 0601 0c01 0601 0402 1001  ................
+00001050: 0801 0601 0402 1001 0a01 0201 0c02 1001  ................
+00001060: 7a18 4e6f 6465 4c69 6b65 5079 4469 6374  z.NodeLikePyDict
+00001070: 2e73 6574 5f63 6869 6c64 6304 0000 0000  .set_childc.....
+00001080: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
+00001090: 0000 0073 3000 0000 7400 7c02 7401 8302  ...s0...t.|.t...
+000010a0: 7309 7c03 6400 7501 7210 7402 7c02 7c01  s.|.d.u.r.t.|.|.
+000010b0: 7c03 6401 8d03 7d02 7c00 a003 7c01 7c02  |.d...}.|...|.|.
+000010c0: a102 0100 6400 5300 2902 4e29 0172 5800  ....d.S.).N).rX.
+000010d0: 0000 2904 7231 0000 0072 0500 0000 da05  ..).r1...r......
+000010e0: 5661 6c75 6572 5600 0000 2904 7244 0000  ValuerV...).rD..
+000010f0: 0072 4d00 0000 7237 0000 0072 5800 0000  .rM...r7...rX...
+00001100: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
+00001110: 5300 0000 a200 0000 7306 0000 0012 010e  S.......s.......
+00001120: 0110 017a 184e 6f64 654c 696b 6550 7944  ...z.NodeLikePyD
+00001130: 6963 742e 7365 745f 7661 6c75 6563 0300  ict.set_valuec..
+00001140: 0000 0000 0000 0000 0000 0300 0000 0100  ................
+00001150: 0000 4300 0000 7304 0000 0064 0153 0029  ..C...s....d.S.)
+00001160: 027a 0b53 6574 2061 6e20 6974 656d 4e72  .z.Set an itemNr
+00001170: 2100 0000 a903 7244 0000 0072 3600 0000  !.....rD...r6...
+00001180: 7237 0000 0072 2100 0000 7221 0000 0072  r7...r!...r!...r
+00001190: 2200 0000 7256 0000 00a7 0000 0073 0200  "...rV.......s..
+000011a0: 0000 0400 7a18 4e6f 6465 4c69 6b65 5079  ....z.NodeLikePy
+000011b0: 4469 6374 2e5f 7365 745f 6974 656d 2903  Dict._set_item).
+000011c0: 4e46 4e72 3000 0000 290a 7247 0000 0072  NFNr0...).rG...r
+000011d0: 4800 0000 7249 0000 0072 5400 0000 7207  H...rI...rT...r.
+000011e0: 0000 0072 5500 0000 7250 0000 0072 5300  ...rU...rP...rS.
+000011f0: 0000 7203 0000 0072 5600 0000 7221 0000  ..r....rV...r!..
+00001200: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+00001210: 724a 0000 0055 0000 0073 1e00 0000 0800  rJ...U...s......
+00001220: 0204 0201 0201 04fb 0202 02fe 0603 02fd  ................
+00001230: 0605 0afb 0824 0a28 0205 0e01 724a 0000  .....$.(....rJ..
+00001240: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001250: 0000 0300 0000 4000 0000 7346 0000 0065  ......@...sF...e
+00001260: 005a 0164 005a 0264 1064 0264 0384 015a  .Z.d.Z.d.d.d...Z
+00001270: 0364 0464 0584 005a 0464 0664 0784 005a  .d.d...Z.d.d...Z
+00001280: 0564 0864 0984 005a 0664 0a64 0b84 005a  .d.d...Z.d.d...Z
+00001290: 0764 0c64 0d84 005a 0864 0e64 0f84 005a  .d.d...Z.d.d...Z
+000012a0: 0964 0153 0029 11da 0d46 6f61 6d49 6e70  .d.S.)...FoamInp
+000012b0: 7574 4669 6c65 4e63 0500 0000 0000 0000  utFileNc........
+000012c0: 0000 0000 0500 0000 0200 0000 4300 0000  ............C...
+000012d0: 732e 0000 007c 017c 005f 007c 0264 0075  s....|.|._.|.d.u
+000012e0: 0072 0969 007d 027c 027c 005f 017c 037c  .r.i.}.|.|._.|.|
+000012f0: 005f 027c 047c 005f 0364 007c 005f 0464  ._.|.|._.d.|._.d
+00001300: 0053 0072 3000 0000 2905 da04 696e 666f  .S.r0...)...info
+00001310: da08 6368 696c 6472 656e da06 6865 6164  ..children..head
+00001320: 6572 724c 0000 00da 0470 6174 6829 0572  errL.....path).r
+00001330: 4400 0000 7273 0000 0072 7400 0000 7275  D...rs...rt...ru
+00001340: 0000 0072 4c00 0000 7221 0000 0072 2100  ...rL...r!...r!.
+00001350: 0000 7222 0000 00da 085f 5f69 6e69 745f  ..r".....__init_
+00001360: 5fad 0000 0073 0e00 0000 0601 0801 0401  _....s..........
+00001370: 0601 0601 0601 0a01 7a16 466f 616d 496e  ........z.FoamIn
+00001380: 7075 7446 696c 652e 5f5f 696e 6974 5f5f  putFile.__init__
+00001390: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000013a0: 0005 0000 0043 0000 0073 4200 0000 6401  .....C...sB...d.
+000013b0: 6701 7d01 7c00 6a00 6400 7501 7212 7c01  g.}.|.j.d.u.r.|.
+000013c0: a001 6402 7c00 6a00 9b00 6403 9d03 a101  ..d.|.j...d.....
+000013d0: 0100 7c01 a001 6404 7c00 6a02 9b00 6405  ..|...d.|.j...d.
+000013e0: 9d03 a101 0100 6406 a003 7c01 a101 5300  ......d...|...S.
+000013f0: 2907 4e7a 0b49 6e70 7574 4669 6c65 280a  ).Nz.InputFile(.
+00001400: 7a05 696e 666f 3d7a 022c 0a7a 0963 6869  z.info=z.,.z.chi
+00001410: 6c64 7265 6e3d 7a02 0a29 7210 0000 0029  ldren=z..)r....)
+00001420: 0472 7300 0000 7227 0000 0072 7400 0000  .rs...r'...rt...
+00001430: 7228 0000 0029 0272 4400 0000 da03 746d  r(...).rD.....tm
+00001440: 7072 2100 0000 7221 0000 0072 2200 0000  pr!...r!...r"...
+00001450: da08 5f5f 7265 7072 5f5f b600 0000 730a  ..__repr__....s.
+00001460: 0000 0006 010a 0114 0114 010a 017a 1646  .............z.F
+00001470: 6f61 6d49 6e70 7574 4669 6c65 2e5f 5f72  oamInputFile.__r
+00001480: 6570 725f 5f63 0100 0000 0000 0000 0000  epr__c..........
+00001490: 0000 0b00 0000 0800 0000 4300 0000 73a2  ..........C...s.
+000014a0: 0100 0067 007d 017c 006a 0064 0075 0172  ...g.}.|.j.d.u.r
+000014b0: 3664 0167 017d 027c 006a 00a0 01a1 0044  6d.g.}.|.j.....D
+000014c0: 005d 195c 027d 037d 0464 0274 027c 0383  .].\.}.}.d.t.|..
+000014d0: 0118 0064 0314 007d 057c 02a0 0364 047c  ...d...}.|...d.|
+000014e0: 039b 007c 059b 007c 049b 0064 059d 05a1  ...|...|...d....
+000014f0: 0101 0071 0f7c 02a0 0364 06a1 0101 007c  ...q.|...d.....|
+00001500: 01a0 0364 07a0 047c 02a1 01a1 0101 0074  ...d...|.......t
+00001510: 057c 006a 0664 0864 098d 027d 067c 006a  .|.j.d.d...}.|.j
+00001520: 06a0 01a1 0044 005d 715c 027d 037d 0474  .....D.]q\.}.}.t
+00001530: 077c 0464 0a83 0272 5d7c 04a0 08a1 007d  .|.d...r]|.....}
+00001540: 077c 0364 0075 0072 5c74 097c 0474 0a83  .|.d.u.r\t.|.t..
+00001550: 0272 5c7c 0764 0537 007d 076e 2f7c 0464  .r\|.d.7.}.n/|.d
+00001560: 0075 0072 657c 039b 007d 076e 2774 077c  .u.re|...}.n't.|
+00001570: 0464 0b83 0272 6f7c 04a0 0ba1 007d 086e  .d...ro|.....}.n
+00001580: 027c 047d 087c 0864 0c6b 0272 7864 0c7d  .|.}.|.d.k.rxd.}
+00001590: 056e 0b74 0c64 0d7c 0674 027c 0383 0118  .n.t.d.|.t.|....
+000015a0: 0083 0264 0314 007d 057c 039b 007c 059b  ...d...}.|...|..
+000015b0: 007c 089b 0064 059d 047d 077c 006a 0d64  .|...d...}.|.j.d
+000015c0: 0075 0172 ae7c 037c 006a 0d76 0072 ae7c  .u.r.|.|.j.v.r.|
+000015d0: 006a 0d7c 0319 007d 0974 097c 0974 0e83  .j.|...}.t.|.t..
+000015e0: 0272 ae64 0e7c 09a0 0f64 0764 0fa1 0217  .r.d.|...d.d....
+000015f0: 007d 097c 0964 0717 007c 0717 007d 077c  .}.|.d...|...}.|
+00001600: 01a0 037c 07a1 0101 0071 4264 10a0 047c  ...|.....qBd...|
+00001610: 01a1 017d 0a7c 006a 1064 0075 0172 c57c  ...}.|.j.d.u.r.|
+00001620: 006a 1064 0717 007c 0a17 007d 0a7c 0a64  .j.d...|...}.|.d
+00001630: 1119 0064 076b 0372 cf7c 0a64 0737 007d  ...d.k.r.|.d.7.}
+00001640: 0a7c 0a53 0029 124e 7a0a 466f 616d 4669  .|.S.).Nz.FoamFi
+00001650: 6c65 0a7b e90c 0000 00fa 0120 fa04 2020  le.{....... ..  
+00001660: 2020 fa01 3bda 017d da01 0ae9 0e00 0000    ..;..}........
+00001670: 2901 723f 0000 00da 0464 756d 70da 1764  ).r?.....dump..d
+00001680: 756d 705f 7769 7468 6f75 745f 6173 7369  ump_without_assi
+00001690: 676e 6d65 6e74 7210 0000 0072 5e00 0000  gnmentr....r^...
+000016a0: 7a03 2f2f 207a 040a 2f2f 207a 020a 0a72  z.// z..// z...r
+000016b0: 1400 0000 2911 7273 0000 0072 3c00 0000  ....).rs...r<...
+000016c0: 7234 0000 0072 2700 0000 7228 0000 0072  r4...r'...r(...r
+000016d0: 4000 0000 7274 0000 00da 0768 6173 6174  @...rt.....hasat
+000016e0: 7472 7281 0000 0072 3100 0000 7233 0000  trr....r1...r3..
+000016f0: 0072 8200 0000 723b 0000 0072 4c00 0000  .r....r;...rL...
+00001700: 724f 0000 00da 0772 6570 6c61 6365 7275  rO.....replaceru
+00001710: 0000 0029 0b72 4400 0000 7278 0000 005a  ...).rD...rx...Z
+00001720: 0474 6d70 3172 3600 0000 da04 6e6f 6465  .tmp1r6.....node
+00001730: 720a 0000 00da 0a6e 756d 5f73 7061 6365  r......num_space
+00001740: 73da 0963 6f64 655f 6e6f 6465 5a0b 6e6f  s..code_nodeZ.no
+00001750: 6465 5f64 756d 7065 64da 0763 6f6d 6d65  de_dumped..comme
+00001760: 6e74 721e 0000 0072 2100 0000 7221 0000  ntr....r!...r!..
+00001770: 0072 2200 0000 7281 0000 00bd 0000 0073  .r"...r........s
+00001780: 4800 0000 0401 0a01 0601 1201 1001 1c01  H...............
+00001790: 0a01 1001 0e02 1201 0a01 0801 1202 0801  ................
+000017a0: 0280 0801 0801 0a02 0a01 0402 0801 0601  ................
+000017b0: 1602 1201 1401 0a01 0a01 1001 0c01 0c01  ................
+000017c0: 0a01 0a01 0e01 0c01 0801 0401 7a12 466f  ............z.Fo
+000017d0: 616d 496e 7075 7446 696c 652e 6475 6d70  amInputFile.dump
+000017e0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000017f0: 0008 0000 0043 0000 0073 5200 0000 7c00  .....C...sR...|.
+00001800: 6a00 6400 7500 7209 7401 6401 8301 8201  j.d.u.r.t.d.....
+00001810: 7402 7c00 6a00 6402 8302 8f10 7d01 7c01  t.|.j.d.....}.|.
+00001820: a003 7c00 a004 a100 a101 0100 5700 6400  ..|.........W.d.
+00001830: 0400 0400 8303 0100 6400 5300 3100 7322  ........d.S.1.s"
+00001840: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
+00001850: 2903 4e7a 1173 656c 662e 7061 7468 2069  ).Nz.self.path i
+00001860: 7320 4e6f 6e65 da01 7729 0572 7600 0000  s None..w).rv...
+00001870: 723d 0000 00da 046f 7065 6eda 0577 7269  r=.....open..wri
+00001880: 7465 7281 0000 0029 0272 4400 0000 da04  ter....).rD.....
+00001890: 6669 6c65 7221 0000 0072 2100 0000 7222  filer!...r!...r"
+000018a0: 0000 00da 096f 7665 7277 7269 7465 e700  .....overwrite..
+000018b0: 0000 730a 0000 000a 0108 010e 0110 0122  ..s............"
+000018c0: ff7a 1746 6f61 6d49 6e70 7574 4669 6c65  .z.FoamInputFile
+000018d0: 2e6f 7665 7277 7269 7465 6303 0000 0000  .overwritec.....
+000018e0: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
+000018f0: 0000 00f3 0e00 0000 7c02 7c00 6a00 7c01  ........|.|.j.|.
+00001900: 3c00 6400 5300 7230 0000 00a9 0172 7400  <.d.S.r0.....rt.
+00001910: 0000 7271 0000 0072 2100 0000 7221 0000  ..rq...r!...r!..
+00001920: 0072 2200 0000 7256 0000 00ed 0000 00f3  .r"...rV........
+00001930: 0200 0000 0e01 7a17 466f 616d 496e 7075  ......z.FoamInpu
+00001940: 7446 696c 652e 5f73 6574 5f69 7465 6d63  tFile._set_itemc
+00001950: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00001960: 0300 0000 4300 0000 728e 0000 0072 3000  ....C...r....r0.
+00001970: 0000 728f 0000 0029 0372 4400 0000 7236  ..r....).rD...r6
+00001980: 0000 00da 0469 7465 6d72 2100 0000 7221  .....itemr!...r!
+00001990: 0000 0072 2200 0000 da0b 5f5f 7365 7469  ...r".....__seti
+000019a0: 7465 6d5f 5ff0 0000 0072 9000 0000 7a19  tem__....r....z.
+000019b0: 466f 616d 496e 7075 7446 696c 652e 5f5f  FoamInputFile.__
+000019c0: 7365 7469 7465 6d5f 5f63 0200 0000 0000  setitem__c......
+000019d0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+000019e0: 0000 730a 0000 007c 006a 007c 0119 0053  ..s....|.j.|...S
+000019f0: 0072 3000 0000 728f 0000 0029 0272 4400  .r0...r....).rD.
+00001a00: 0000 7236 0000 0072 2100 0000 7221 0000  ..r6...r!...r!..
+00001a10: 0072 2200 0000 da0b 5f5f 6765 7469 7465  .r".....__getite
+00001a20: 6d5f 5ff3 0000 00f3 0200 0000 0a01 7a19  m__...........z.
+00001a30: 466f 616d 496e 7075 7446 696c 652e 5f5f  FoamInputFile.__
+00001a40: 6765 7469 7465 6d5f 5fa9 034e 4e4e 290a  getitem__..NNN).
+00001a50: 7247 0000 0072 4800 0000 7249 0000 0072  rG...rH...rI...r
+00001a60: 7700 0000 7279 0000 0072 8100 0000 728d  w...ry...r....r.
+00001a70: 0000 0072 5600 0000 7292 0000 0072 9300  ...rV...r....r..
+00001a80: 0000 7221 0000 0072 2100 0000 7221 0000  ..r!...r!...r!..
+00001a90: 0072 2200 0000 7272 0000 00ac 0000 0073  .r"...rr.......s
+00001aa0: 1000 0000 0800 0a01 0809 0807 082a 0806  .............*..
+00001ab0: 0803 0c03 7272 0000 0063 0000 0000 0000  ....rr...c......
+00001ac0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00001ad0: 0000 7328 0000 0065 005a 0164 005a 0255  ..s(...e.Z.d.Z.U
+00001ae0: 0065 0365 0464 013c 0065 0565 0464 023c  .e.e.d.<.e.e.d.<
+00001af0: 0064 0764 0464 0584 015a 0664 0653 0029  .d.d.d...Z.d.S.)
+00001b00: 08da 0a41 7373 6967 6e6d 656e 7472 4d00  ...AssignmentrM.
+00001b10: 0000 7237 0000 0072 0100 0000 6302 0000  ..r7...r....c...
+00001b20: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00001b30: 0043 0000 0073 3400 0000 7400 7c00 6a01  .C...s4...t.|.j.
+00001b40: 6401 8302 720c 7c00 6a01 a002 7c01 a101  d...r.|.j...|...
+00001b50: 5300 7c01 6402 1400 7c00 6a03 9b00 6403  S.|.d...|.j...d.
+00001b60: 7c00 6a01 9b00 6404 9d04 1700 5300 a905  |.j...d.....S...
+00001b70: 4e72 8100 0000 727b 0000 00fa 0220 2072  Nr....r{.....  r
+00001b80: 7d00 0000 2904 7283 0000 0072 3700 0000  }...).r....r7...
+00001b90: 7281 0000 0072 4d00 0000 a902 7244 0000  r....rM.....rD..
+00001ba0: 00da 0669 6e64 656e 7472 2100 0000 7221  ...indentr!...r!
+00001bb0: 0000 0072 2200 0000 7281 0000 00fc 0000  ...r"...r.......
+00001bc0: 0073 0600 0000 0c01 0c01 1c02 7a0f 4173  .s..........z.As
+00001bd0: 7369 676e 6d65 6e74 2e64 756d 704e a901  signment.dumpN..
+00001be0: 7201 0000 0029 0772 4700 0000 7248 0000  r....).rG...rH..
+00001bf0: 0072 4900 0000 724f 0000 00da 0f5f 5f61  .rI...rO.....__a
+00001c00: 6e6e 6f74 6174 696f 6e73 5f5f da06 6f62  nnotations__..ob
+00001c10: 6a65 6374 7281 0000 0072 2100 0000 7221  jectr....r!...r!
+00001c20: 0000 0072 2100 0000 7222 0000 0072 9600  ...r!...r"...r..
+00001c30: 0000 f700 0000 7308 0000 000a 0008 0208  ......s.........
+00001c40: 010e 0272 9600 0000 6300 0000 0000 0000  ...r....c.......
+00001c50: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00001c60: 0073 2600 0000 6500 5a01 6400 5a02 8700  .s&...e.Z.d.Z...
+00001c70: 6601 6401 6402 8408 5a03 6406 6404 6405  f.d.d...Z.d.d.d.
+00001c80: 8401 5a04 8700 0400 5a05 5300 2907 da12  ..Z.....Z.S.)...
+00001c90: 5661 7269 6162 6c65 4173 7369 676e 6d65  VariableAssignme
+00001ca0: 6e74 6301 0000 0000 0000 0000 0000 0002  ntc.............
+00001cb0: 0000 0002 0000 0003 0000 0073 0e00 0000  ...........s....
+00001cc0: 7400 8300 a001 a100 7d01 7c01 5300 7230  t.......}.|.S.r0
+00001cd0: 0000 00a9 02da 0573 7570 6572 7279 0000  .......superry..
+00001ce0: 0029 0272 4400 0000 720a 0000 00a9 01da  .).rD...r.......
+00001cf0: 095f 5f63 6c61 7373 5f5f 7221 0000 0072  .__class__r!...r
+00001d00: 2200 0000 7279 0000 0004 0100 0073 0400  "...ry.......s..
+00001d10: 0000 0a01 0401 7a1b 5661 7269 6162 6c65  ......z.Variable
+00001d20: 4173 7369 676e 6d65 6e74 2e5f 5f72 6570  Assignment.__rep
+00001d30: 725f 5f72 0100 0000 6302 0000 0000 0000  r__r....c.......
+00001d40: 0000 0000 0002 0000 0006 0000 0043 0000  .............C..
+00001d50: 0073 4a00 0000 7400 7c00 6a01 6401 8302  .sJ...t.|.j.d...
+00001d60: 7217 7c01 6402 1400 7c00 6a02 9b00 6403  r.|.d...|.j...d.
+00001d70: 7c00 6a01 a003 7c01 a101 9b00 6404 9d04  |.j...|.....d...
+00001d80: 1700 5300 7c01 6402 1400 7c00 6a02 9b00  ..S.|.d...|.j...
+00001d90: 6403 7c00 6a01 9b00 6404 9d04 1700 5300  d.|.j...d.....S.
+00001da0: 7297 0000 0029 0472 8300 0000 7237 0000  r....).r....r7..
+00001db0: 0072 4d00 0000 7281 0000 0072 9900 0000  .rM...r....r....
+00001dc0: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
+00001dd0: 8100 0000 0801 0000 7306 0000 000c 0122  ........s......"
+00001de0: 011c 027a 1756 6172 6961 626c 6541 7373  ...z.VariableAss
+00001df0: 6967 6e6d 656e 742e 6475 6d70 729b 0000  ignment.dumpr...
+00001e00: 0029 0672 4700 0000 7248 0000 0072 4900  .).rG...rH...rI.
+00001e10: 0000 7279 0000 0072 8100 0000 da0d 5f5f  ..ry...r......__
+00001e20: 636c 6173 7363 656c 6c5f 5f72 2100 0000  classcell__r!...
+00001e30: 7221 0000 0072 a100 0000 7222 0000 0072  r!...r....r"...r
+00001e40: 9e00 0000 0301 0000 7306 0000 0008 000c  ........s.......
+00001e50: 0112 0472 9e00 0000 6300 0000 0000 0000  ...r....c.......
+00001e60: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00001e70: 00f3 2800 0000 6500 5a01 6400 5a02 6409  ..(...e.Z.d.Z.d.
+00001e80: 6402 6403 8401 5a03 6404 6405 8400 5a04  d.d...Z.d.d...Z.
+00001e90: 640a 6407 6408 8401 5a05 6401 5300 290b  d.d.d...Z.d.S.).
+00001ea0: 7270 0000 004e 6304 0000 0000 0000 0000  rp...Nc.........
+00001eb0: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
+00001ec0: 2c00 0000 7c01 7c00 5f00 7c02 7c00 5f01  ,...|.|._.|.|._.
+00001ed0: 7402 7c03 7403 7404 6602 8302 7211 7405  t.|.t.t.f...r.t.
+00001ee0: 7c03 8301 7d03 7c03 7c00 5f06 6400 5300  |...}.|.|._.d.S.
+00001ef0: 7230 0000 0029 0772 3700 0000 724d 0000  r0...).r7...rM..
+00001f00: 0072 3100 0000 7251 0000 00da 0574 7570  .r1...rQ.....tup
+00001f10: 6c65 722e 0000 0072 5800 0000 2904 7244  ler....rX...).rD
+00001f20: 0000 0072 3700 0000 724d 0000 0072 5800  ...r7...rM...rX.
+00001f30: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00001f40: 0072 7700 0000 1101 0000 730a 0000 0006  .rw.......s.....
+00001f50: 0106 010e 0108 010a 017a 0e56 616c 7565  .........z.Value
+00001f60: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00001f70: 0000 0000 0000 0100 0000 0700 0000 4300  ..............C.
+00001f80: 0000 7394 0000 007c 006a 0064 0075 0172  ..s....|.j.d.u.r
+00001f90: 197c 006a 0164 0075 0172 1964 017c 006a  .|.j.d.u.r.d.|.j
+00001fa0: 029b 0064 027c 006a 019b 0064 037c 006a  ...d.|.j...d.|.j
+00001fb0: 009b 0064 049d 0753 007c 006a 0064 0075  ...d...S.|.j.d.u
+00001fc0: 0072 2e7c 006a 0164 0075 0172 2e64 017c  .r.|.j.d.u.r.d.|
+00001fd0: 006a 029b 0064 027c 006a 019b 0064 049d  .j...d.|.j...d..
+00001fe0: 0553 007c 006a 0064 0075 0172 437c 006a  .S.|.j.d.u.rC|.j
+00001ff0: 0164 0075 0072 4364 017c 006a 029b 0064  .d.u.rCd.|.j...d
+00002000: 057c 006a 009b 0064 049d 0553 0064 017c  .|.j...d...S.d.|
+00002010: 006a 029b 0064 069d 0353 0029 074e 7a06  .j...d...S.).Nz.
+00002020: 5661 6c75 6528 7a08 2c20 6e61 6d65 3d22  Value(z., name="
+00002030: 7a0e 222c 2064 696d 656e 7369 6f6e 3d22  z.", dimension="
+00002040: 7a02 2229 7a0d 2c20 6469 6d65 6e73 696f  z.")z., dimensio
+00002050: 6e3d 22fa 0129 2903 7258 0000 0072 4d00  n="..)).rX...rM.
+00002060: 0000 7237 0000 00a9 0172 4400 0000 7221  ..r7.....rD...r!
+00002070: 0000 0072 2100 0000 7222 0000 0072 7900  ...r!...r"...ry.
+00002080: 0000 1801 0000 730e 0000 0014 011e 0114  ......s.........
+00002090: 0116 0114 0116 010e 027a 0e56 616c 7565  .........z.Value
+000020a0: 2e5f 5f72 6570 725f 5f72 0100 0000 6302  .__repr__r....c.
+000020b0: 0000 0000 0000 0000 0000 0005 0000 0005  ................
+000020c0: 0000 0043 0000 0073 ce00 0000 7c00 6a00  ...C...s....|.j.
+000020d0: 6400 7501 7214 7401 7c00 6a00 8301 7d02  d.u.r.t.|.j...}.
+000020e0: 6401 a002 6402 6403 8400 7c02 4400 8301  d...d.d...|.D...
+000020f0: a101 7d03 7403 7c00 6a04 7405 8302 7226  ..}.t.|.j.t...r&
+00002100: 7406 7c00 6a04 6404 8302 7226 7c00 6a04  t.|.j.d...r&|.j.
+00002110: a007 a100 7d04 6e05 7408 7c00 6a04 8301  ....}.n.t.|.j...
+00002120: 7d04 7c00 6a00 6400 7501 7240 7c00 6a09  }.|.j.d.u.r@|.j.
+00002130: 6400 7501 7240 7c00 6a09 9b00 6405 7c03  d.u.r@|.j...d.|.
+00002140: 9b00 6406 7c04 9b00 9d05 5300 7c00 6a00  ..d.|.....S.|.j.
+00002150: 6400 7500 7252 7c00 6a09 6400 7501 7252  d.u.rR|.j.d.u.rR
+00002160: 7c00 6a09 9b00 6401 7c04 9b00 9d03 5300  |.j...d.|.....S.
+00002170: 7c00 6a00 6400 7501 7264 7c00 6a09 6400  |.j.d.u.rd|.j.d.
+00002180: 7500 7264 6407 7c03 9b00 6406 7c04 9b00  u.rdd.|...d.|...
+00002190: 9d04 5300 7c04 9b00 5300 2908 4e72 7b00  ..S.|...S.).Nr{.
+000021a0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+000021b0: 0000 0003 0000 0073 0000 00f3 1800 0000  .......s........
+000021c0: 8100 7c00 5d07 7d01 7400 7c01 8301 5600  ..|.].}.t.|...V.
+000021d0: 0100 7102 6400 5300 7230 0000 00a9 0172  ..q.d.S.r0.....r
+000021e0: 4f00 0000 a902 7235 0000 00da 066e 756d  O.....r5.....num
+000021f0: 6265 7272 2100 0000 7221 0000 0072 2200  berr!...r!...r".
+00002200: 0000 7238 0000 0025 0100 00f3 0400 0000  ..r8...%........
+00002210: 0280 1600 7a30 5661 6c75 652e 6475 6d70  ....z0Value.dump
+00002220: 5f77 6974 686f 7574 5f61 7373 6967 6e6d  _without_assignm
+00002230: 656e 742e 3c6c 6f63 616c 733e 2e3c 6765  ent.<locals>.<ge
+00002240: 6e65 7870 723e 7281 0000 007a 0220 5b7a  nexpr>r....z. [z
+00002250: 025d 20fa 015b 290a 7258 0000 0072 2300  .] ..[).rX...r#.
+00002260: 0000 7228 0000 0072 3100 0000 7237 0000  ..r(...r1...r7..
+00002270: 0072 4100 0000 7283 0000 0072 8100 0000  .rA...r....r....
+00002280: 724f 0000 0072 4d00 0000 2905 7244 0000  rO...rM...).rD..
+00002290: 0072 9a00 0000 5a0e 6469 6d65 6e73 696f  .r....Z.dimensio
+000022a0: 6e5f 6c69 7374 5a10 6469 6d65 6e73 696f  n_listZ.dimensio
+000022b0: 6e5f 6475 6d70 6564 5a0c 7661 6c75 655f  n_dumpedZ.value_
+000022c0: 6475 6d70 6564 7221 0000 0072 2100 0000  dumpedr!...r!...
+000022d0: 7222 0000 0072 8200 0000 2201 0000 731a  r"...r...."...s.
+000022e0: 0000 000a 010a 0114 0118 020c 010a 0214  ................
+000022f0: 0216 0114 0110 0114 0110 0106 027a 1d56  .............z.V
+00002300: 616c 7565 2e64 756d 705f 7769 7468 6f75  alue.dump_withou
+00002310: 745f 6173 7369 676e 6d65 6e74 2902 4e4e  t_assignment).NN
+00002320: 729b 0000 0029 0672 4700 0000 7248 0000  r....).rG...rH..
+00002330: 0072 4900 0000 7277 0000 0072 7900 0000  .rI...rw...ry...
+00002340: 7282 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
+00002350: 2100 0000 7222 0000 0072 7000 0000 0f01  !...r"...rp.....
+00002360: 0000 7308 0000 0008 000a 0208 070e 0a72  ..s............r
+00002370: 7000 0000 6300 0000 0000 0000 0000 0000  p...c...........
+00002380: 0000 0000 0003 0000 0000 0000 0073 2e00  .............s..
+00002390: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
+000023a0: 6402 8408 5a03 6403 6404 8400 5a04 6408  d...Z.d.d...Z.d.
+000023b0: 6406 6407 8401 5a05 8700 0400 5a06 5300  d.d...Z.....Z.S.
+000023c0: 2909 726a 0000 0063 0200 0000 0000 0000  ).rj...c........
+000023d0: 0000 0000 0200 0000 0300 0000 0300 0000  ................
+000023e0: 733c 0000 0074 007c 0174 0183 0272 0974  s<...t.|.t...r.t
+000023f0: 027c 0183 017d 0174 0364 0164 0284 007c  .|...}.t.d.d...|
+00002400: 0144 0083 0183 0173 1674 0464 0383 0182  .D.....s.t.d....
+00002410: 0174 0583 00a0 067c 01a1 0101 0064 0053  .t.....|.....d.S
+00002420: 0029 044e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00002430: 0002 0000 0004 0000 0073 0000 0072 5a00  .........s...rZ.
+00002440: 0000 7230 0000 0029 0272 3100 0000 721a  ..r0...).r1...r.
+00002450: 0000 0029 0272 3500 0000 da04 656c 656d  ...).r5.....elem
+00002460: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
+00002470: 3800 0000 3a01 0000 725c 0000 007a 2844  8...:...r\...z(D
+00002480: 696d 656e 7369 6f6e 5365 742e 5f5f 696e  imensionSet.__in
+00002490: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c67  it__.<locals>.<g
+000024a0: 656e 6578 7072 3e7a 1342 6164 207b 666f  enexpr>z.Bad {fo
+000024b0: 616d 5f75 6e69 7473 203d 207d 2907 7231  am_units = }).r1
+000024c0: 0000 0072 4f00 0000 7223 0000 0072 6700  ...rO...r#...rg.
+000024d0: 0000 723d 0000 0072 a000 0000 7277 0000  ..r=...r....rw..
+000024e0: 0029 0272 4400 0000 722a 0000 0072 a100  .).rD...r*...r..
+000024f0: 0000 7221 0000 0072 2200 0000 7277 0000  ..r!...r"...rw..
+00002500: 0037 0100 0073 0a00 0000 0a01 0801 1201  .7...s..........
+00002510: 0801 1001 7a15 4469 6d65 6e73 696f 6e53  ....z.DimensionS
+00002520: 6574 2e5f 5f69 6e69 745f 5f63 0100 0000  et.__init__c....
+00002530: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00002540: 4300 0000 7308 0000 0074 007c 0083 0153  C...s....t.|...S
+00002550: 0072 3000 0000 2901 722e 0000 0072 a700  .r0...).r....r..
+00002560: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00002570: 0072 7900 0000 3e01 0000 f302 0000 0008  .ry...>.........
+00002580: 017a 1544 696d 656e 7369 6f6e 5365 742e  .z.DimensionSet.
+00002590: 5f5f 7265 7072 5f5f 7201 0000 0063 0200  __repr__r....c..
+000025a0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+000025b0: 0000 4300 0000 731c 0000 0064 0164 02a0  ..C...s....d.d..
+000025c0: 0064 0364 0484 007c 0044 0083 01a1 0117  .d.d...|.D......
+000025d0: 0064 0517 0053 0029 064e 72ad 0000 0072  .d...S.).Nr....r
+000025e0: 7b00 0000 6301 0000 0000 0000 0000 0000  {...c...........
+000025f0: 0002 0000 0003 0000 0073 0000 0072 a800  .........s...r..
+00002600: 0000 7230 0000 0072 a900 0000 72aa 0000  ..r0...r....r...
+00002610: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+00002620: 7238 0000 0042 0100 0072 ac00 0000 7a37  r8...B...r....z7
+00002630: 4469 6d65 6e73 696f 6e53 6574 2e64 756d  DimensionSet.dum
+00002640: 705f 7769 7468 6f75 745f 6173 7369 676e  p_without_assign
+00002650: 6d65 6e74 2e3c 6c6f 6361 6c73 3e2e 3c67  ment.<locals>.<g
+00002660: 656e 6578 7072 3efa 015d a901 7228 0000  enexpr>..]..r(..
+00002670: 0072 9900 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00002680: 7222 0000 0072 8200 0000 4101 0000 f302  r"...r....A.....
+00002690: 0000 001c 017a 2444 696d 656e 7369 6f6e  .....z$Dimension
+000026a0: 5365 742e 6475 6d70 5f77 6974 686f 7574  Set.dump_without
+000026b0: 5f61 7373 6967 6e6d 656e 7472 9b00 0000  _assignmentr....
+000026c0: 2907 7247 0000 0072 4800 0000 7249 0000  ).rG...rH...rI..
+000026d0: 0072 7700 0000 7279 0000 0072 8200 0000  .rw...ry...r....
+000026e0: 72a3 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
+000026f0: a100 0000 7222 0000 0072 6a00 0000 3601  ....r"...rj...6.
+00002700: 0000 7308 0000 0008 000c 0108 0712 0372  ..s............r
+00002710: 6a00 0000 6300 0000 0000 0000 0000 0000  j...c...........
+00002720: 0000 0000 0004 0000 0000 0000 0073 4400  .............sD.
+00002730: 0000 6500 5a01 6400 5a02 640d 8700 6601  ..e.Z.d.Z.d...f.
+00002740: 6402 6403 8409 5a03 6404 6405 8400 5a04  d.d...Z.d.d...Z.
+00002750: 8700 6601 6406 6407 8408 5a05 640e 6409  ..f.d.d...Z.d.d.
+00002760: 640a 8401 5a06 640b 640c 8400 5a07 8700  d...Z.d.d...Z...
+00002770: 0400 5a08 5300 290f 7232 0000 004e 6305  ..Z.S.).r2...Nc.
+00002780: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00002790: 0000 0003 0000 0073 2800 0000 7c02 7c00  .......s(...|.|.
+000027a0: 5f00 7c03 7c00 5f01 7c04 7c00 5f02 7403  _.|.|._.|.|._.t.
+000027b0: 8300 6a04 6401 6900 7c01 a401 8e01 0100  ..j.d.i.|.......
+000027c0: 6400 5300 2902 4e72 2100 0000 2905 da05  d.S.).Nr!...)...
+000027d0: 5f6e 616d 65da 0a5f 6469 7265 6374 6976  _name.._directiv
+000027e0: 6572 4c00 0000 72a0 0000 0072 7700 0000  erL...r....rw...
+000027f0: 2905 7244 0000 0072 3e00 0000 724d 0000  ).rD...r>...rM..
+00002800: 00da 0964 6972 6563 7469 7665 724c 0000  ...directiverL..
+00002810: 0072 a100 0000 7221 0000 0072 2200 0000  .r....r!...r"...
+00002820: 7277 0000 0046 0100 0073 0800 0000 0601  rw...F...s......
+00002830: 0601 0601 1601 7a0d 4469 6374 2e5f 5f69  ......z.Dict.__i
+00002840: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00002850: 0000 0100 0000 0100 0000 4300 0000 f306  ..........C.....
+00002860: 0000 007c 006a 0053 0072 3000 0000 a901  ...|.j.S.r0.....
+00002870: 72b3 0000 0072 a700 0000 7221 0000 0072  r....r....r!...r
+00002880: 2100 0000 7222 0000 00da 0867 6574 5f6e  !...r".....get_n
+00002890: 616d 654c 0100 00f3 0200 0000 0601 7a0d  ameL..........z.
+000028a0: 4469 6374 2e67 6574 5f6e 616d 6563 0100  Dict.get_namec..
+000028b0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000028c0: 0000 0300 0000 f30a 0000 0074 0083 00a0  ...........t....
+000028d0: 01a1 0053 0072 3000 0000 729f 0000 0072  ...S.r0...r....r
+000028e0: a700 0000 72a1 0000 0072 2100 0000 7222  ....r....r!...r"
+000028f0: 0000 0072 7900 0000 4f01 0000 7294 0000  ...ry...O...r...
+00002900: 007a 0d44 6963 742e 5f5f 7265 7072 5f5f  .z.Dict.__repr__
+00002910: 7201 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00002920: 0000 0b00 0000 0900 0000 4300 0000 7354  ..........C...sT
+00002930: 0100 0067 007d 027c 0164 0114 007d 037c  ...g.}.|.d...}.|
+00002940: 006a 0064 0075 0172 287c 037c 006a 0017  .j.d.u.r(|.|.j..
+00002950: 007d 047c 006a 0164 0075 0172 1c7c 0464  .}.|.j.d.u.r.|.d
+00002960: 027c 006a 0117 0037 007d 047c 02a0 027c  .|.j...7.}.|...|
+00002970: 0464 037c 039b 009d 0217 0064 0417 00a1  .d.|.......d....
+00002980: 0101 0074 037c 0083 017d 057c 00a0 04a1  ...t.|...}.|....
+00002990: 0044 005d 605c 027d 067d 077c 006a 0564  .D.]`\.}.}.|.j.d
+000029a0: 0075 0172 537c 067c 006a 0576 0072 537c  .u.rS|.|.j.v.rS|
+000029b0: 006a 057c 0619 007d 0874 067c 0874 0783  .j.|...}.t.|.t..
+000029c0: 0272 537c 02a0 0264 057c 08a0 0864 0364  .rS|...d.|...d.d
+000029d0: 06a1 0217 00a1 0101 0074 097c 0764 0783  .........t.|.d..
+000029e0: 0272 637c 02a0 027c 07a0 0a7c 0164 0817  .rc|...|...|.d..
+000029f0: 00a1 01a1 0101 0071 3074 097c 0764 0983  .......q0t.|.d..
+00002a00: 0272 6d7c 07a0 0ba1 007d 096e 027c 077d  .rm|.....}.n.|.}
+00002a10: 097c 0764 0a6b 0272 7664 0a7d 0a6e 0b74  .|.d.k.rvd.}.n.t
+00002a20: 0c64 0b7c 0574 0d7c 0683 0118 0083 0264  .d.|.t.|.......d
+00002a30: 0114 007d 0a7c 02a0 027c 0364 0c7c 069b  ...}.|...|.d.|..
+00002a40: 007c 0a9b 007c 099b 0064 0d9d 0517 00a1  .|...|...d......
+00002a50: 0101 0071 307c 02a0 027c 0364 0e17 00a1  ...q0|...|.d....
+00002a60: 0101 0074 067c 0074 0e83 0272 a57c 0264  ...t.|.t...r.|.d
+00002a70: 0f05 0019 0064 0d37 0003 003c 0064 03a0  .....d.7...<.d..
+00002a80: 0f7c 02a1 0153 0029 104e 727b 0000 0072  .|...S.).Nr{...r
+00002a90: 9800 0000 727f 0000 00da 017b 7a07 2020  ....r......{z.  
+00002aa0: 2020 2f2f 207a 080a 2020 2020 2f2f 2072    // z..    // r
+00002ab0: 8100 0000 7239 0000 0072 8200 0000 7210  ....r9...r....r.
+00002ac0: 0000 0072 5e00 0000 727c 0000 0072 7d00  ...r^...r|...r}.
+00002ad0: 0000 727e 0000 0072 1400 0000 2910 72b3  ..r~...r....).r.
+00002ae0: 0000 0072 b400 0000 7227 0000 0072 4000  ...r....r'...r@.
+00002af0: 0000 723c 0000 0072 4c00 0000 7231 0000  ..r<...rL...r1..
+00002b00: 0072 4f00 0000 7284 0000 0072 8300 0000  .rO...r....r....
+00002b10: 7281 0000 0072 8200 0000 723b 0000 0072  r....r....r;...r
+00002b20: 3400 0000 da0a 436f 6465 5374 7265 616d  4.....CodeStream
+00002b30: 7228 0000 0029 0b72 4400 0000 729a 0000  r(...).rD...r...
+00002b40: 0072 7800 0000 da0b 696e 6465 6e74 6174  .rx.....indentat
+00002b50: 696f 6eda 046c 696e 6572 8600 0000 7236  ion..liner....r6
+00002b60: 0000 0072 8500 0000 7288 0000 0072 8700  ...r....r....r..
+00002b70: 0000 720a 0000 0072 2100 0000 7221 0000  ..r....r!...r!..
+00002b80: 0072 2200 0000 7281 0000 0052 0100 0073  .r"...r....R...s
+00002b90: 3400 0000 0401 0801 0a01 0a01 0a01 0e01  4...............
+00002ba0: 1801 0802 1001 1401 0a01 0a01 1601 0a02  ................
+00002bb0: 1601 0a02 0a01 0402 0801 0601 1602 2001  .............. .
+00002bc0: 0e01 0a03 1001 0a02 7a09 4469 6374 2e64  ........z.Dict.d
+00002bd0: 756d 7063 0300 0000 0000 0000 0000 0000  umpc............
+00002be0: 0300 0000 0300 0000 4300 0000 730c 0000  ........C...s...
+00002bf0: 007c 027c 007c 013c 0064 0053 0072 3000  .|.|.|.<.d.S.r0.
+00002c00: 0000 7221 0000 0072 7100 0000 7221 0000  ..r!...rq...r!..
+00002c10: 0072 2100 0000 7222 0000 0072 5600 0000  .r!...r"...rV...
+00002c20: 7601 0000 7302 0000 000c 017a 0e44 6963  v...s......z.Dic
+00002c30: 742e 5f73 6574 5f69 7465 6d72 9500 0000  t._set_itemr....
+00002c40: 729b 0000 0029 0972 4700 0000 7248 0000  r....).rG...rH..
+00002c50: 0072 4900 0000 7277 0000 0072 b800 0000  .rI...rw...r....
+00002c60: 7279 0000 0072 8100 0000 7256 0000 0072  ry...r....rV...r
+00002c70: a300 0000 7221 0000 0072 2100 0000 72a1  ....r!...r!...r.
+00002c80: 0000 0072 2200 0000 7232 0000 0045 0100  ...r"...r2...E..
+00002c90: 0073 0c00 0000 0800 0e01 0806 0c03 0a03  .s..............
+00002ca0: 1024 7232 0000 0063 0000 0000 0000 0000  .$r2...c........
+00002cb0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+00002cc0: 735a 0000 0065 005a 0164 005a 0264 015a  sZ...e.Z.d.Z.d.Z
+00002cd0: 0364 1287 0066 0164 0364 0484 095a 0464  .d...f.d.d...Z.d
+00002ce0: 0564 0684 005a 0564 0764 0884 005a 0687  .d...Z.d.d...Z..
+00002cf0: 0066 0164 0964 0a84 085a 0764 0b64 0c84  .f.d.d...Z.d.d..
+00002d00: 005a 0864 1364 0e64 0f84 015a 0964 1364  .Z.d.d.d...Z.d.d
+00002d10: 1064 1184 015a 0a87 0004 005a 0b53 0029  .d...Z.....Z.S.)
+00002d20: 1472 3300 0000 7a1b 5265 7072 6573 656e  .r3...z.Represen
+00002d30: 7473 2061 6e20 4f70 656e 466f 616d 206c  ts an OpenFoam l
+00002d40: 6973 744e 6304 0000 0000 0000 0000 0000  istNc...........
+00002d50: 0004 0000 0003 0000 0003 0000 0073 1c00  .............s..
+00002d60: 0000 7c02 7c00 5f00 7c03 7c00 5f01 7402  ..|.|._.|.|._.t.
+00002d70: 8300 a003 7c01 a101 0100 6400 5300 7230  ....|.....d.S.r0
+00002d80: 0000 0029 0472 b300 0000 da06 5f64 7479  ...).r......_dty
+00002d90: 7065 72a0 0000 0072 7700 0000 2904 7244  per....rw...).rD
+00002da0: 0000 00da 0869 7465 7261 626c 6572 4d00  .....iterablerM.
+00002db0: 0000 7266 0000 0072 a100 0000 7221 0000  ..rf...r....r!..
+00002dc0: 0072 2200 0000 7277 0000 007d 0100 0073  .r"...rw...}...s
+00002dd0: 0600 0000 0601 0601 1001 7a0d 4c69 7374  ..........z.List
+00002de0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00002df0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00002e00: 0000 72b6 0000 0072 3000 0000 72b7 0000  ..r....r0...r...
+00002e10: 0072 a700 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00002e20: 7222 0000 0072 b800 0000 8201 0000 72b9  r"...r........r.
+00002e30: 0000 007a 0d4c 6973 742e 6765 745f 6e61  ...z.List.get_na
+00002e40: 6d65 6302 0000 0000 0000 0000 0000 0002  mec.............
+00002e50: 0000 0003 0000 0043 0000 0073 4800 0000  .......C...sH...
+00002e60: 7c00 6a00 6400 7500 720a 7c01 7c00 5f00  |.j.d.u.r.|.|._.
+00002e70: 6400 5300 7401 7c00 6a00 7402 8302 7221  d.S.t.|.j.t...r!
+00002e80: 7c00 6a00 7c01 6b03 721f 7c01 6401 1700  |.j.|.k.r.|.d...
+00002e90: 7c00 6a00 1700 7c00 5f00 6400 5300 6400  |.j...|._.d.S.d.
+00002ea0: 5300 7403 8300 8201 2902 4e72 7b00 0000  S.t.....).Nr{...
+00002eb0: 2904 72b3 0000 0072 3100 0000 724f 0000  ).r....r1...rO..
+00002ec0: 00da 0c52 756e 7469 6d65 4572 726f 7229  ...RuntimeError)
+00002ed0: 0272 4400 0000 724d 0000 0072 2100 0000  .rD...rM...r!...
+00002ee0: 7221 0000 0072 2200 0000 da08 6164 645f  r!...r".....add_
+00002ef0: 6e61 6d65 8501 0000 730e 0000 000a 010a  name....s.......
+00002f00: 010c 010a 0114 0104 ff06 037a 0d4c 6973  ...........z.Lis
+00002f10: 742e 6164 645f 6e61 6d65 6301 0000 0000  t.add_namec.....
+00002f20: 0000 0000 0000 0001 0000 0002 0000 0003  ................
+00002f30: 0000 0072 ba00 0000 7230 0000 0072 9f00  ...r....r0...r..
+00002f40: 0000 72a7 0000 0072 a100 0000 7221 0000  ..r....r....r!..
+00002f50: 0072 2200 0000 7279 0000 008e 0100 0072  .r"...ry.......r
+00002f60: 9400 0000 7a0d 4c69 7374 2e5f 5f72 6570  ....z.List.__rep
+00002f70: 725f 5f63 0200 0000 0000 0000 0000 0000  r__c............
+00002f80: 0200 0000 0300 0000 0300 0000 7314 0000  ............s...
+00002f90: 0087 0087 0166 0264 0164 0284 0888 0144  .....f.d.d.....D
+00002fa0: 0083 0153 0029 034e 6301 0000 0000 0000  ...S.).Nc.......
+00002fb0: 0000 0000 0002 0000 0006 0000 0013 0000  ................
+00002fc0: 0073 1800 0000 6700 7c00 5d08 7d01 8801  .s....g.|.].}...
+00002fd0: a000 7c01 8800 a102 9102 7102 5300 7221  ..|.......q.S.r!
+00002fe0: 0000 00a9 01da 0a5f 6475 6d70 5f69 7465  ......._dump_ite
+00002ff0: 6d29 0272 3500 0000 7291 0000 00a9 0272  m).r5...r......r
+00003000: 9a00 0000 7244 0000 0072 2100 0000 7222  ....rD...r!...r"
+00003010: 0000 0072 6400 0000 9201 0000 7302 0000  ...rd.......s...
+00003020: 0018 007a 2b4c 6973 742e 5f6d 616b 655f  ...z+List._make_
+00003030: 6c69 7374 5f73 7472 696e 6773 2e3c 6c6f  list_strings.<lo
+00003040: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00003050: 7221 0000 0072 9900 0000 7221 0000 0072  r!...r....r!...r
+00003060: c500 0000 7222 0000 00da 125f 6d61 6b65  ....r"....._make
+00003070: 5f6c 6973 745f 7374 7269 6e67 7391 0100  _list_strings...
+00003080: 0073 0200 0000 1401 7a17 4c69 7374 2e5f  .s......z.List._
+00003090: 6d61 6b65 5f6c 6973 745f 7374 7269 6e67  make_list_string
+000030a0: 7372 0100 0000 6303 0000 0000 0000 0000  sr....c.........
+000030b0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+000030c0: 3200 0000 7400 7c01 7401 7402 6602 8302  2...t.|.t.t.f...
+000030d0: 7211 7403 7c01 6401 8302 7211 7c01 a004  r.t.|.d...r.|...
+000030e0: 7c02 a101 5300 7c02 6402 1400 7405 7c01  |...S.|.d...t.|.
+000030f0: 8301 1700 5300 2903 4e72 8100 0000 727b  ....S.).Nr....r{
+00003100: 0000 0029 0672 3100 0000 7241 0000 0072  ...).r1...rA...r
+00003110: 9600 0000 7283 0000 0072 8100 0000 724f  ....r....r....rO
+00003120: 0000 0029 0372 4400 0000 7291 0000 0072  ...).rD...r....r
+00003130: 9a00 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
+00003140: 0000 0072 c400 0000 9401 0000 7306 0000  ...r........s...
+00003150: 0018 010a 0110 027a 0f4c 6973 742e 5f64  .......z.List._d
+00003160: 756d 705f 6974 656d 6302 0000 0000 0000  ump_itemc.......
+00003170: 0000 0000 000a 0000 0008 0000 0003 0000  ................
+00003180: 0073 6801 0000 6700 7d02 8800 6401 1400  .sh...g.}...d...
+00003190: 7d03 8801 6a00 6400 7500 721f 7c02 a001  }...j.d.u.r.|...
+000031a0: 8801 6a02 6402 6403 8d01 a101 0100 7c03  ..j.d.d.......|.
+000031b0: 6404 1700 6401 a003 7c02 a101 1700 6405  d...d...|.....d.
+000031c0: 1700 5300 8801 6a00 7d04 8801 6a04 6400  ..S...j.}...j.d.
+000031d0: 7501 7236 7c04 6406 8801 6a04 9b00 6407  u.r6|.d...j...d.
+000031e0: 7c03 9b00 7405 8801 8301 9b00 9d05 3700  |...t.........7.
+000031f0: 7d04 7c02 a006 7c03 7c04 1700 6408 7c03  }.|...|.|...d.|.
+00003200: 9b00 9d02 1700 6404 1700 a101 0100 6409  ......d.......d.
+00003210: 640a 640b 9c02 7d05 8801 6a00 7c05 a007  d.d...}...j.|...
+00003220: a100 7601 725e 7c02 a006 6408 a003 8801  ..v.r^|...d.....
+00003230: a002 8800 640c 1700 a101 a101 a101 0100  ....d...........
+00003240: 6e4a 8801 72a8 7c05 8801 6a00 1900 7d06  nJ..r.|...j...}.
+00003250: 8801 6402 1900 7c06 6b02 736f 7408 8801  ..d...|.k.sot...
+00003260: 8301 8201 6700 7d07 6400 7d08 8801 4400  ....g.}.d.}...D.
+00003270: 5d18 7d09 7c09 7c06 6b02 7288 7c08 6400  ].}.|.|.k.r.|.d.
+00003280: 7501 7284 7c07 a006 7c08 a101 0100 7c09  u.r.|...|.....|.
+00003290: 6701 7d08 7175 7c08 a006 7c09 a101 0100  g.}.qu|...|.....
+000032a0: 7175 7c07 a006 7c08 a101 0100 8701 6601  qu|...|.......f.
+000032b0: 640d 640e 8408 7c07 4400 8301 7d07 7c02  d.d...|.D...}.|.
+000032c0: a001 8700 6601 640f 6410 8408 7c07 4400  ....f.d.d...|.D.
+000032d0: 8301 a101 0100 7c02 a006 7c03 6411 1700  ......|...|.d...
+000032e0: a101 0100 6408 a003 7c02 a101 5300 2912  ....d...|...S.).
+000032f0: 4e72 7b00 0000 7201 0000 00a9 0172 9a00  Nr{...r......r..
+00003300: 0000 fa01 2872 a600 0000 7a13 2020 206e  ....(r....z.   n
+00003310: 6f6e 756e 6966 6f72 6d20 4c69 7374 3c7a  onuniform List<z
+00003320: 023e 0a72 7f00 0000 da03 6865 785a 0673  .>.r......hexZ.s
+00003330: 706c 696e 6529 02da 0662 6c6f 636b 73da  pline)...blocks.
+00003340: 0565 6467 6573 7239 0000 0063 0100 0000  .edgesr9...c....
+00003350: 0000 0000 0000 0000 0200 0000 0700 0000  ................
+00003360: 1300 0000 7324 0000 0067 007c 005d 0e7d  ....s$...g.|.].}
+00003370: 0164 00a0 0087 0066 0164 0164 0284 087c  .d.....f.d.d...|
+00003380: 0144 0083 01a1 0191 0271 0253 0029 0372  .D.......q.S.).r
+00003390: 7b00 0000 6301 0000 0000 0000 0000 0000  {...c...........
+000033a0: 0002 0000 0004 0000 0033 0000 0073 1a00  .........3...s..
+000033b0: 0000 8100 7c00 5d08 7d01 8800 a000 7c01  ....|.].}.....|.
+000033c0: a101 5600 0100 7102 6400 5300 7230 0000  ..V...q.d.S.r0..
+000033d0: 0072 c300 0000 2902 7235 0000 005a 055f  .r....).r5...Z._
+000033e0: 6974 656d 72a7 0000 0072 2100 0000 7222  itemr....r!...r"
+000033f0: 0000 0072 3800 0000 bb01 0000 725c 0000  ...r8.......r\..
+00003400: 007a 274c 6973 742e 6475 6d70 2e3c 6c6f  .z'List.dump.<lo
+00003410: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00003420: 2e3c 6765 6e65 7870 723e 72b1 0000 0029  .<genexpr>r....)
+00003430: 0272 3500 0000 da0a 6974 656d 735f 6c69  .r5.....items_li
+00003440: 6e65 72a7 0000 0072 2100 0000 7222 0000  ner....r!...r"..
+00003450: 0072 6400 0000 ba01 0000 7308 0000 0006  .rd.......s.....
+00003460: 0002 0216 ff06 ff7a 1d4c 6973 742e 6475  .......z.List.du
+00003470: 6d70 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  mp.<locals>.<lis
+00003480: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
+00003490: 0000 0002 0000 0003 0000 0033 0000 0073  ...........3...s
+000034a0: 2000 0000 8100 7c00 5d0b 7d01 8800 6400   .....|.].}...d.
+000034b0: 1700 6401 1400 7c01 1700 5600 0100 7102  ..d...|...V...q.
+000034c0: 6402 5300 2903 7239 0000 0072 7b00 0000  d.S.).r9...r{...
+000034d0: 4e72 2100 0000 2902 7235 0000 0072 be00  Nr!...).r5...r..
+000034e0: 0000 72c7 0000 0072 2100 0000 7222 0000  ..r....r!...r"..
+000034f0: 0072 3800 0000 be01 0000 7304 0000 0002  .r8.......s.....
+00003500: 801e 007a 1c4c 6973 742e 6475 6d70 2e3c  ...z.List.dump.<
+00003510: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
+00003520: 3e7a 0229 3b29 0972 b300 0000 da06 6578  >z.);).r......ex
+00003530: 7465 6e64 72c6 0000 0072 2800 0000 72bf  tendr....r(...r.
+00003540: 0000 0072 3400 0000 7227 0000 00da 046b  ...r4...r'.....k
+00003550: 6579 7372 3d00 0000 290a 7244 0000 0072  eysr=...).rD...r
+00003560: 9a00 0000 7278 0000 0072 bd00 0000 7275  ....rx...r....ru
+00003570: 0000 005a 0c73 7065 6369 616c 5f6b 6579  ...Z.special_key
+00003580: 735a 0b73 7065 6369 616c 5f6b 6579 da05  sZ.special_key..
+00003590: 6c69 6e65 7372 cc00 0000 7291 0000 0072  linesr....r....r
+000035a0: 2100 0000 72c5 0000 0072 2200 0000 7281  !...r....r"...r.
+000035b0: 0000 009a 0100 0073 4a00 0000 0401 0801  .......sJ.......
+000035c0: 0a01 1201 1601 0602 0a01 0201 0a01 0201  ................
+000035d0: 02ff 0601 04ff 04ff 1c05 0a01 0e01 1c01  ................
+000035e0: 0401 0a01 0c01 0801 0401 0401 0801 0801  ................
+000035f0: 0801 0a01 0801 0c02 0a01 0a01 0202 06fe  ................
+00003600: 1804 0e01 0a01 7a09 4c69 7374 2e64 756d  ......z.List.dum
+00003610: 7072 9500 0000 729b 0000 0029 0c72 4700  pr....r....).rG.
+00003620: 0000 7248 0000 0072 4900 0000 da07 5f5f  ..rH...rI.....__
+00003630: 646f 635f 5f72 7700 0000 72b8 0000 0072  doc__rw...r....r
+00003640: c200 0000 7279 0000 0072 c600 0000 72c4  ....ry...r....r.
+00003650: 0000 0072 8100 0000 72a3 0000 0072 2100  ...r....r....r!.
+00003660: 0000 7221 0000 0072 a100 0000 7222 0000  ..r!...r....r"..
+00003670: 0072 3300 0000 7a01 0000 7312 0000 0008  .r3...z...s.....
+00003680: 0004 010e 0208 0508 030c 0908 030a 0312  ................
+00003690: 0672 3300 0000 6300 0000 0000 0000 0000  .r3...c.........
+000036a0: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+000036b0: 1000 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+000036c0: 6402 5300 2903 72bc 0000 007a 2241 2064  d.S.).r....z"A d
+000036d0: 6963 7469 6f6e 6e61 7279 2074 6f20 7374  ictionnary to st
+000036e0: 6f72 6520 2363 6f64 6553 7472 6561 6d4e  ore #codeStreamN
+000036f0: 2904 7247 0000 0072 4800 0000 7249 0000  ).rG...rH...rI..
+00003700: 0072 d000 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00003710: 7221 0000 0072 2200 0000 72bc 0000 00c3  r!...r"...r.....
+00003720: 0100 0073 0400 0000 0800 0801 72bc 0000  ...s........r...
+00003730: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+00003740: 0000 0300 0000 0300 0000 7322 0000 0087  ..........s"....
+00003750: 0066 0164 0164 0284 087d 0187 0066 0164  .f.d.d...}...f.d
+00003760: 0364 0484 087d 0274 007c 017c 0283 0253  .d...}.t.|.|...S
+00003770: 0029 054e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00003780: 0001 0000 0002 0000 0013 0000 0073 0a00  .............s..
+00003790: 0000 7c00 8800 1900 6a00 5300 7230 0000  ..|.....j.S.r0..
+000037a0: 00a9 01da 0463 6f64 6572 a700 0000 725d  .....coder....r]
+000037b0: 0000 0072 2100 0000 7222 0000 0072 5200  ...r!...r"...rR.
+000037c0: 0000 c801 0000 7294 0000 007a 185f 6d61  ......r....z._ma
+000037d0: 6b65 5f61 6c69 6173 2e3c 6c6f 6361 6c73  ke_alias.<locals
+000037e0: 3e2e 6765 7463 0200 0000 0000 0000 0000  >.getc..........
+000037f0: 0000 0200 0000 0300 0000 1300 0000 730e  ..............s.
+00003800: 0000 007c 017c 0088 0019 005f 0064 0053  ...|.|....._.d.S
+00003810: 0072 3000 0000 72d1 0000 0029 02da 055f  .r0...r....)..._
+00003820: 7365 6c66 7237 0000 0072 5d00 0000 7221  selfr7...r]...r!
+00003830: 0000 0072 2200 0000 da03 7365 74cb 0100  ...r".....set...
+00003840: 0072 9000 0000 7a18 5f6d 616b 655f 616c  .r....z._make_al
+00003850: 6961 732e 3c6c 6f63 616c 733e 2e73 6574  ias.<locals>.set
+00003860: 2901 da08 7072 6f70 6572 7479 2903 724d  )...property).rM
+00003870: 0000 0072 5200 0000 72d4 0000 0072 2100  ...rR...r....r!.
+00003880: 0000 725d 0000 0072 2200 0000 da0b 5f6d  ..r]...r"....._m
+00003890: 616b 655f 616c 6961 73c7 0100 0073 0600  ake_alias....s..
+000038a0: 0000 0c01 0c03 0a03 72d6 0000 0029 045a  ........r....).Z
+000038b0: 0b63 6f64 6549 6e63 6c75 6465 5a0b 636f  .codeIncludeZ.co
+000038c0: 6465 4f70 7469 6f6e 735a 0863 6f64 654c  deOptionsZ.codeL
+000038d0: 6962 7372 d200 0000 6300 0000 0000 0000  ibsr....c.......
+000038e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000038f0: 0072 a400 0000 290b da04 436f 6465 4e63  .r....)...CodeNc
+00003900: 0400 0000 0000 0000 0000 0000 0400 0000  ................
+00003910: 0200 0000 4300 0000 731a 0000 007c 017c  ....C...s....|.|
+00003920: 005f 0074 017c 0283 017c 005f 027c 037c  ._.t.|...|._.|.|
+00003930: 005f 0364 0053 0072 3000 0000 2904 724d  ._.d.S.r0...).rM
+00003940: 0000 0072 0600 0000 72d2 0000 0072 b500  ...r....r....r..
+00003950: 0000 2904 7244 0000 0072 4d00 0000 72d2  ..).rD...rM...r.
+00003960: 0000 0072 b500 0000 7221 0000 0072 2100  ...r....r!...r!.
+00003970: 0000 7222 0000 0072 7700 0000 d601 0000  ..r"...rw.......
+00003980: 7306 0000 0006 010a 010a 017a 0d43 6f64  s..........z.Cod
+00003990: 652e 5f5f 696e 6974 5f5f 6301 0000 0000  e.__init__c.....
+000039a0: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+000039b0: 0000 0073 3e00 0000 7c00 6a00 6400 7500  ...s>...|.j.d.u.
+000039c0: 7210 6401 7c00 6a01 6400 6402 8502 1900  r.d.|.j.d.d.....
+000039d0: 9b00 6403 9d03 5300 6401 7c00 6a01 6400  ..d...S.d.|.j.d.
+000039e0: 6402 8502 1900 9b00 6404 7c00 6a00 9b00  d.......d.|.j...
+000039f0: 6405 9d05 5300 2906 4e7a 0643 6f64 6528  d...S.).Nz.Code(
+00003a00: 2272 2f00 0000 7a07 5b2e 2e2e 5d22 297a  "r/...z.[...]")z
+00003a10: 125b 2e2e 2e5d 222c 2064 6972 6563 7469  .[...]", directi
+00003a20: 7665 3d72 a600 0000 2902 72b5 0000 0072  ve=r....).r....r
+00003a30: d200 0000 72a7 0000 0072 2100 0000 7221  ....r....r!...r!
+00003a40: 0000 0072 2200 0000 7279 0000 00db 0100  ...r"...ry......
+00003a50: 0073 0600 0000 0a01 1601 1e01 7a0d 436f  .s..........z.Co
+00003a60: 6465 2e5f 5f72 6570 725f 5f72 0100 0000  de.__repr__r....
+00003a70: 6302 0000 0000 0000 0000 0000 0007 0000  c...............
+00003a80: 0005 0000 0043 0000 0073 8a00 0000 6700  .....C...s....g.
+00003a90: 7d02 7c01 6401 1400 7d03 7c01 6402 1700  }.|.d...}.|.d...
+00003aa0: 6401 1400 7d04 7c03 7c00 6a00 1700 7d05  d...}.|.|.j...}.
+00003ab0: 7c00 6a01 6400 7501 721d 7c05 6401 7c00  |.j.d.u.r.|.d.|.
+00003ac0: 6a01 1700 3700 7d05 7c02 a002 7c05 6403  j...7.}.|...|.d.
+00003ad0: 7c03 9b00 9d02 1700 6404 1700 a101 0100  |.......d.......
+00003ae0: 7c00 6a03 a004 6403 a101 4400 5d09 7d06  |.j...d...D.].}.
+00003af0: 7c02 a002 7c04 7c06 1700 a101 0100 712f  |...|.|.......q/
+00003b00: 7c02 a002 7c03 6405 1700 a101 0100 6403  |...|.d.......d.
+00003b10: a005 7c02 a101 5300 2906 4e72 7b00 0000  ..|...S.).Nr{...
+00003b20: 7239 0000 0072 7f00 0000 7a02 237b 7a03  r9...r....z.#{z.
+00003b30: 237d 3b29 0672 4d00 0000 72b5 0000 0072  #};).rM...r....r
+00003b40: 2700 0000 72d2 0000 0072 1900 0000 7228  '...r....r....r(
+00003b50: 0000 0029 0772 4400 0000 729a 0000 0072  ...).rD...r....r
+00003b60: 7800 0000 72bd 0000 005a 0c69 6e64 656e  x...r....Z.inden
+00003b70: 7461 7469 6f6e 3472 1700 0000 72be 0000  tation4r....r...
+00003b80: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+00003b90: 7281 0000 00e0 0100 0073 1600 0000 0401  r........s......
+00003ba0: 0801 0c01 0a01 0a01 0e01 1801 1001 1001  ................
+00003bb0: 0e01 0a01 7a09 436f 6465 2e64 756d 7072  ....z.Code.dumpr
+00003bc0: 3000 0000 729b 0000 00a9 0672 4700 0000  0...r......rG...
+00003bd0: 7248 0000 0072 4900 0000 7277 0000 0072  rH...rI...rw...r
+00003be0: 7900 0000 7281 0000 0072 2100 0000 7221  y...r....r!...r!
+00003bf0: 0000 0072 2100 0000 7222 0000 0072 d700  ...r!...r"...r..
+00003c00: 0000 d501 0000 7308 0000 0008 000a 0108  ......s.........
+00003c10: 050e 0572 d700 0000 6300 0000 0000 0000  ...r....c.......
+00003c20: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00003c30: 0072 a400 0000 290b da04 4e61 6d65 4e63  .r....)...NameNc
+00003c40: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00003c50: 0200 0000 4300 0000 f310 0000 007c 017c  ....C........|.|
+00003c60: 005f 007c 027c 005f 0164 0053 0072 3000  ._.|.|._.d.S.r0.
+00003c70: 0000 2902 724d 0000 0072 3700 0000 2903  ..).rM...r7...).
+00003c80: 7244 0000 0072 4d00 0000 7237 0000 0072  rD...rM...r7...r
+00003c90: 2100 0000 7221 0000 0072 2200 0000 7277  !...r!...r"...rw
+00003ca0: 0000 00f0 0100 00f3 0400 0000 0601 0a01  ................
+00003cb0: 7a0d 4e61 6d65 2e5f 5f69 6e69 745f 5f63  z.Name.__init__c
+00003cc0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00003cd0: 0300 0000 4300 0000 730e 0000 0064 017c  ....C...s....d.|
+00003ce0: 006a 009b 0064 029d 0353 0029 034e 7a05  .j...d...S.).Nz.
+00003cf0: 4e61 6d65 2872 a600 0000 725d 0000 0072  Name(r....r]...r
+00003d00: a700 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
+00003d10: 0000 0072 7900 0000 f401 0000 7290 0000  ...ry.......r...
+00003d20: 007a 0d4e 616d 652e 5f5f 7265 7072 5f5f  .z.Name.__repr__
+00003d30: 7201 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00003d40: 0000 0200 0000 0100 0000 4300 0000 7308  ..........C...s.
+00003d50: 0000 007c 006a 009b 0053 0072 3000 0000  ...|.j...S.r0...
+00003d60: 725d 0000 0072 9900 0000 7221 0000 0072  r]...r....r!...r
+00003d70: 2100 0000 7222 0000 0072 8100 0000 f701  !...r"...r......
+00003d80: 0000 72af 0000 007a 094e 616d 652e 6475  ..r....z.Name.du
+00003d90: 6d70 7230 0000 0072 9b00 0000 72d8 0000  mpr0...r....r...
+00003da0: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
+00003db0: 7222 0000 0072 d900 0000 ee01 0000 7308  r"...r........s.
+00003dc0: 0000 0008 000a 0208 040e 0372 d900 0000  ...........r....
+00003dd0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00003de0: 0003 0000 0040 0000 0073 2600 0000 6500  .....@...s&...e.
+00003df0: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
+00003e00: 6404 8400 5a04 6409 6406 6407 8401 5a05  d...Z.d.d.d...Z.
+00003e10: 6408 5300 290a da09 4469 7265 6374 6976  d.S.)...Directiv
+00003e20: 6563 0300 0000 0000 0000 0000 0000 0300  ec..............
+00003e30: 0000 0200 0000 4300 0000 72da 0000 0072  ......C...r....r
+00003e40: 3000 0000 a902 72b5 0000 00da 0763 6f6e  0.....r......con
+00003e50: 7465 6e74 2903 7244 0000 0072 b500 0000  tent).rD...r....
+00003e60: 72de 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
+00003e70: 2200 0000 7277 0000 00fc 0100 0072 db00  "...rw.......r..
+00003e80: 0000 7a12 4469 7265 6374 6976 652e 5f5f  ..z.Directive.__
+00003e90: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00003ea0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00003eb0: 1200 0000 7c00 6a00 9b00 6401 7c00 6a01  ....|.j...d.|.j.
+00003ec0: 9b00 9d03 5300 2902 4e72 9800 0000 72dd  ....S.).Nr....r.
+00003ed0: 0000 0072 a700 0000 7221 0000 0072 2100  ...r....r!...r!.
+00003ee0: 0000 7222 0000 0072 7900 0000 0002 0000  ..r"...ry.......
+00003ef0: 7302 0000 0012 017a 1244 6972 6563 7469  s......z.Directi
+00003f00: 7665 2e5f 5f72 6570 725f 5f72 0100 0000  ve.__repr__r....
+00003f10: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00003f20: 0005 0000 0043 0000 0073 1c00 0000 7c01  .....C...s....|.
+00003f30: 6401 1400 7c00 6a00 9b00 6402 7c00 6a01  d...|.j...d.|.j.
+00003f40: 9b00 6403 9d04 1700 5300 2904 4e72 7b00  ..d.....S.).Nr{.
+00003f50: 0000 7298 0000 0072 7d00 0000 72dd 0000  ..r....r}...r...
+00003f60: 0072 9900 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00003f70: 7222 0000 0072 8100 0000 0302 0000 72b2  r"...r........r.
+00003f80: 0000 007a 0e44 6972 6563 7469 7665 2e64  ...z.Directive.d
+00003f90: 756d 704e 729b 0000 0072 d800 0000 7221  umpNr....r....r!
+00003fa0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00003fb0: 0000 72dc 0000 00fb 0100 0073 0800 0000  ..r........s....
+00003fc0: 0800 0801 0804 0e03 72dc 0000 0029 0172  ........r....).r
+00003fd0: 2f00 0000 2927 72d0 0000 0072 1500 0000  /...)'r....r....
+00003fe0: da03 6162 6372 0200 0000 7203 0000 00da  ..abcr....r.....
+00003ff0: 0b64 6174 6163 6c61 7373 6573 7204 0000  .dataclassesr...
+00004000: 00da 076e 756d 6265 7273 7205 0000 00da  ...numbersr.....
+00004010: 0874 6578 7477 7261 7072 0600 0000 da06  .textwrapr......
+00004020: 7479 7069 6e67 7207 0000 00da 056e 756d  typingr......num
+00004030: 7079 7268 0000 00da 0a69 6e66 6c65 6374  pyrh.....inflect
+00004040: 696f 6e72 0800 0000 721b 0000 0072 2300  ionr....r....r#.
+00004050: 0000 722e 0000 0072 4000 0000 7241 0000  ..r....r@...rA..
+00004060: 0072 4a00 0000 7272 0000 0072 9600 0000  .rJ...rr...r....
+00004070: 729e 0000 0072 7000 0000 7251 0000 0072  r....rp...rQ...r
+00004080: 6a00 0000 7254 0000 0072 3200 0000 7233  j...rT...r2...r3
+00004090: 0000 0072 bc00 0000 72d6 0000 0072 b300  ...r....r....r..
+000040a0: 0000 da07 7365 7461 7474 7272 d700 0000  ....setattrr....
+000040b0: 72d9 0000 0072 dc00 0000 7221 0000 0072  r....r....r!...r
+000040c0: 2100 0000 7221 0000 0072 2200 0000 da08  !...r!...r".....
+000040d0: 3c6d 6f64 756c 653e 0100 0000 7340 0000  <module>....s@..
+000040e0: 0004 0008 0210 010c 010c 010c 010c 0108  ................
+000040f0: 020c 0108 0208 0308 1b0a 120e 1110 0712  ................
+00004100: 5702 4b10 0110 0b02 0c12 0112 2614 0f12  W.K.........&...
+00004110: 3510 4908 0408 0a16 0110 0302 1912 0114  5.I.............
+00004120: 0c                                       .
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 19:04:20 2023 UTC, .py size: 5743 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,382 +1,408 @@
-00000000: 6f0d 0d0a 0000 0000 b447 5964 6f16 0000  o........GYdo...
+00000000: 6f0d 0d0a 0000 0000 faba 6b64 9117 0000  o.........kd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6402 6c0b 5a0c 6401 6407 6c0d 6d0e 5a0e  d.l.Z.d.d.l.m.Z.
 00000080: 0100 6401 6408 6c0f 6d10 5a10 6d11 5a11  ..d.d.l.m.Z.m.Z.
 00000090: 6d12 5a12 6d13 5a13 6d14 5a14 6d15 5a15  m.Z.m.Z.m.Z.m.Z.
-000000a0: 6d16 5a16 6d17 5a17 0100 6409 5a18 640a  m.Z.m.Z...d.Z.d.
-000000b0: 5a19 640b 5a1a 4700 640c 640d 8400 640d  Z.d.Z.G.d.d...d.
-000000c0: 6503 8303 5a1b 4700 640e 640f 8400 640f  e...Z.G.d.d...d.
-000000d0: 651b 8303 5a1c 4700 6410 6411 8400 6411  e...Z.G.d.d...d.
-000000e0: 651b 8303 5a1d 651c 651d 6412 9c02 5a1e  e...Z.e.e.d...Z.
-000000f0: 6413 6414 8400 5a1f 6402 5300 2915 7a1e  d.d...Z.d.S.).z.
-00000100: 4865 6c70 6572 2074 6f20 6372 6561 7465  Helper to create
-00000110: 2066 6965 6c64 2066 696c 6573 0a0a e900   field files....
-00000120: 0000 004e 2902 da03 4142 43da 0e61 6273  ...N)...ABC..abs
-00000130: 7472 6163 746d 6574 686f 6429 01da 0853  tractmethod)...S
-00000140: 7472 696e 6749 4f29 01da 064e 756d 6265  tringIO)...Numbe
-00000150: 7229 01da 0450 6174 6829 01da 0570 6172  r)...Path)...par
-00000160: 7365 2908 da04 436f 6465 da0a 436f 6465  se)...Code..Code
-00000170: 5374 7265 616d da04 4469 6374 da0c 4469  Stream..Dict..Di
-00000180: 6d65 6e73 696f 6e53 6574 da0d 466f 616d  mensionSet..Foam
-00000190: 496e 7075 7446 696c 65da 044c 6973 74da  InputFile..List.
-000001a0: 0556 616c 7565 da0e 7374 7232 666f 616d  .Value..str2foam
-000001b0: 5f75 6e69 7473 7a12 2369 6e63 6c75 6465  _unitsz.#include
-000001c0: 2022 6676 4346 442e 4822 7a46 2d49 2428   "fvCFD.H"zF-I$(
-000001d0: 4c49 425f 5352 4329 2f66 696e 6974 6556  LIB_SRC)/finiteV
-000001e0: 6f6c 756d 652f 6c6e 496e 636c 7564 6520  olume/lnInclude 
-000001f0: 5c0a 2d49 2428 4c49 425f 5352 4329 2f6d  \.-I$(LIB_SRC)/m
-00000200: 6573 6854 6f6f 6c73 2f6c 6e49 6e63 6c75  eshTools/lnInclu
-00000210: 6465 7a1c 2d6c 6d65 7368 546f 6f6c 7320  dez.-lmeshTools 
-00000220: 5c0a 2d6c 6669 6e69 7465 566f 6c75 6d65  \.-lfiniteVolume
-00000230: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000240: 0004 0000 0040 0000 0073 8e00 0000 6500  .....@...s....e.
-00000250: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
-00000260: 6505 6402 6503 6602 6403 6404 8404 8301  e.d.e.f.d.d.....
-00000270: 5a06 6505 6405 6503 7017 6507 6602 6406  Z.e.d.e.p.e.f.d.
-00000280: 6407 8404 8301 5a08 6419 6409 640a 8401  d.....Z.d.d.d...
-00000290: 5a09 640b 640c 8400 5a0a 640d 640e 8400  Z.d.d...Z.d.d...
-000002a0: 5a0b 650c 640f 6410 8400 8301 5a0d 650e  Z.e.d.d.....Z.e.
-000002b0: 650f 6510 6603 6411 6412 8401 5a11 6419  e.e.f.d.d...Z.d.
-000002c0: 6413 6414 8401 5a12 6415 6416 8400 5a13  d.d...Z.d.d...Z.
-000002d0: 6417 6418 8400 5a14 6408 5300 291a da08  d.d...Z.d.S.)...
-000002e0: 4669 656c 6441 4243 da03 636c 73da 0463  FieldABC..cls..c
-000002f0: 6f64 6563 0200 0000 0000 0000 0000 0000  odec............
-00000300: 0a00 0000 0600 0000 4300 0000 73c4 0000  ........C...s...
-00000310: 0064 017c 0176 0172 0f74 007c 0183 017d  .d.|.v.r.t.|...}
-00000320: 027c 0064 0064 007c 0264 028d 0353 007c  .|.d.d.|.d...S.|
-00000330: 01a0 0164 01a1 017d 037c 01a0 0264 037c  ...d...}.|...d.|
-00000340: 03a1 027d 047c 01a0 0164 047c 037c 04a1  ...}.|...d.|.|..
-00000350: 037d 057c 01a0 0264 057c 037c 04a1 037d  .}.|...d.|.|...}
-00000360: 067c 0164 007c 0385 0219 0064 0617 007c  .|.d.|.....d...|
-00000370: 017c 0464 0085 0219 0017 007d 0774 007c  .|.d.......}.t.|
-00000380: 0783 017d 027c 017c 0564 0717 007c 0685  ...}.|.|.d...|..
-00000390: 0219 00a0 03a1 007d 087c 08a0 0464 04a1  .......}.|...d..
-000003a0: 0172 5074 05a0 0664 0864 097c 08a1 037d  .rPt...d.d.|...}
-000003b0: 0874 07a0 0874 097c 0883 01a1 017d 097c  .t...t.|.....}.|
-000003c0: 097c 025f 0a7c 0064 0964 097c 027c 0964  .|._.|.d.d.|.|.d
-000003d0: 0a8d 0453 0029 0b4e 5a0a 6e6f 6e75 6e69  ...S.).NZ.nonuni
-000003e0: 666f 726d 2901 da04 7472 6565 da0d 626f  form)...tree..bo
-000003f0: 756e 6461 7279 4669 656c 64fa 0128 fa01  undaryField..(..
-00000400: 297a 033b 0a0a e901 0000 007a 045b 2829  )z.;.......z.[()
-00000410: 5dda 0029 0272 1300 0000 da06 7661 6c75  ]..).r......valu
-00000420: 6573 290b 7207 0000 00da 0569 6e64 6578  es).r......index
-00000430: da06 7269 6e64 6578 da05 7374 7269 70da  ..rindex..strip.
-00000440: 0a73 7461 7274 7377 6974 68da 0272 65da  .startswith..re.
-00000450: 0373 7562 da02 6e70 da07 6c6f 6164 7478  .sub..np..loadtx
-00000460: 7472 0400 0000 da04 6461 7461 290a 7211  tr......data).r.
-00000470: 0000 0072 1200 0000 7213 0000 005a 1069  ...r....r....Z.i
-00000480: 6e64 6578 5f6e 6f6e 756e 6966 6f72 6d5a  ndex_nonuniformZ
-00000490: 1369 6e64 6578 5f62 6f75 6e64 6172 7946  .index_boundaryF
-000004a0: 6965 6c64 5a11 696e 6465 785f 6f70 656e  ieldZ.index_open
-000004b0: 696e 675f 7061 725a 1169 6e64 6578 5f63  ing_parZ.index_c
-000004c0: 6c6f 7369 6e67 5f70 6172 5a0d 636f 6465  losing_parZ.code
-000004d0: 5f74 6f5f 7061 7273 655a 0963 6f64 655f  _to_parseZ.code_
-000004e0: 6461 7461 7222 0000 00a9 0072 2300 0000  datar".....r#...
-000004f0: fa49 2f68 6f6d 652f 7069 6572 7265 2f44  .I/home/pierre/D
-00000500: 6576 2f66 6c75 6964 7369 6d66 6f61 6d2f  ev/fluidsimfoam/
-00000510: 7372 632f 666c 7569 6473 696d 666f 616d  src/fluidsimfoam
-00000520: 2f66 6f61 6d5f 696e 7075 745f 6669 6c65  /foam_input_file
-00000530: 732f 6669 656c 6473 2e70 79da 0966 726f  s/fields.py..fro
-00000540: 6d5f 636f 6465 2300 0000 7324 0000 0008  m_code#...s$....
-00000550: 0208 010e 010a 020c 010e 0104 0106 0104  ................
-00000560: ff1a 0502 ff08 0414 010a 020e 010e 0206  ................
-00000570: 0210 017a 1246 6965 6c64 4142 432e 6672  ...z.FieldABC.fr
-00000580: 6f6d 5f63 6f64 65da 0470 6174 6863 0200  om_code..pathc..
-00000590: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-000005a0: 0000 4300 0000 7320 0000 0074 007c 0183  ..C...s ...t.|..
-000005b0: 017d 017c 00a0 017c 01a0 02a1 00a1 017d  .}.|...|.......}
-000005c0: 027c 017c 025f 037c 0253 00a9 014e 2904  .|.|._.|.S...N).
-000005d0: 7206 0000 0072 2500 0000 da09 7265 6164  r....r%.....read
-000005e0: 5f74 6578 7472 2600 0000 2903 7211 0000  _textr&...).r...
-000005f0: 0072 2600 0000 da05 6669 656c 6472 2300  .r&.....fieldr#.
-00000600: 0000 7223 0000 0072 2400 0000 da09 6672  ..r#...r$.....fr
-00000610: 6f6d 5f70 6174 683f 0000 0073 0800 0000  om_path?...s....
-00000620: 0802 0e01 0601 0401 7a12 4669 656c 6441  ........z.FieldA
-00000630: 4243 2e66 726f 6d5f 7061 7468 4e63 0500  BC.from_pathNc..
-00000640: 0000 0000 0000 0000 0000 0600 0000 0500  ................
-00000650: 0000 4300 0000 7374 0000 007c 0364 0075  ..C...st...|.d.u
-00000660: 0172 087c 037c 005f 006e 2464 0164 027c  .r.|.|._.n$d.d.|
-00000670: 006a 017c 0164 039c 047d 0574 027c 0274  .j.|.d...}.t.|.t
-00000680: 0383 0273 1b74 0374 047c 0283 0183 017d  ...s.t.t.|.....}
-00000690: 0274 057c 057c 0264 0064 049c 0264 058d  .t.|.|.d.d...d..
-000006a0: 027c 005f 007c 006a 00a0 0664 0669 00a1  .|._.|.j...d.i..
-000006b0: 0201 007c 0464 0075 0172 357c 00a0 077c  ...|.d.u.r5|...|
-000006c0: 04a1 0101 0064 007c 005f 0864 0053 0029  .....d.|._.d.S.)
-000006d0: 074e 7a03 322e 30da 0561 7363 6969 2904  .Nz.2.0..ascii).
-000006e0: da07 7665 7273 696f 6eda 0666 6f72 6d61  ..version..forma
-000006f0: 74da 0563 6c61 7373 da06 6f62 6a65 6374  t..class..object
-00000700: 2902 da0a 6469 6d65 6e73 696f 6e73 da0d  )...dimensions..
-00000710: 696e 7465 726e 616c 4669 656c 6429 01da  internalField)..
-00000720: 0863 6869 6c64 7265 6e72 1400 0000 2909  .childrenr....).
-00000730: 7213 0000 0072 1100 0000 da0a 6973 696e  r....r......isin
-00000740: 7374 616e 6365 720b 0000 0072 0f00 0000  stancer....r....
-00000750: 720c 0000 00da 0973 6574 5f63 6869 6c64  r......set_child
-00000760: da0a 7365 745f 7661 6c75 6573 7226 0000  ..set_valuesr&..
-00000770: 0029 06da 0473 656c 66da 046e 616d 65da  .)...self..name.
-00000780: 0964 696d 656e 7369 6f6e 7213 0000 0072  .dimensionr....r
-00000790: 1900 0000 da04 696e 666f 7223 0000 0072  ......infor#...r
-000007a0: 2300 0000 7224 0000 00da 085f 5f69 6e69  #...r$.....__ini
-000007b0: 745f 5f46 0000 0073 2000 0000 0801 0801  t__F...s .......
-000007c0: 0203 0201 0401 0201 06fc 0a07 0c01 0202  ................
-000007d0: 0a01 08ff 0e04 0802 0a01 0a02 7a11 4669  ............z.Fi
-000007e0: 656c 6441 4243 2e5f 5f69 6e69 745f 5f63  eldABC.__init__c
-000007f0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000800: 0200 0000 4300 0000 730a 0000 007c 006a  ....C...s....|.j
-00000810: 00a0 01a1 0053 0072 2700 0000 2902 7213  .....S.r'...).r.
-00000820: 0000 00da 0464 756d 70a9 0172 3600 0000  .....dump..r6...
-00000830: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
-00000840: 3b00 0000 5f00 0000 7302 0000 000a 017a  ;..._...s......z
-00000850: 0d46 6965 6c64 4142 432e 6475 6d70 6301  .FieldABC.dumpc.
-00000860: 0000 0000 0000 0000 0000 0002 0000 0008  ................
-00000870: 0000 0043 0000 0073 5200 0000 7c00 6a00  ...C...sR...|.j.
-00000880: 6400 7500 7209 7401 6401 8301 8201 7402  d.u.r.t.d.....t.
-00000890: 7c00 6a00 6402 8302 8f10 7d01 7c01 a003  |.j.d.....}.|...
-000008a0: 7c00 a004 a100 a101 0100 5700 6400 0400  |.........W.d...
-000008b0: 0400 8303 0100 6400 5300 3100 7322 7701  ......d.S.1.s"w.
-000008c0: 0100 0100 0100 5900 0100 6400 5300 2903  ......Y...d.S.).
-000008d0: 4e7a 1173 656c 662e 7061 7468 2069 7320  Nz.self.path is 
-000008e0: 4e6f 6e65 da01 7729 0572 2600 0000 da0a  None..w).r&.....
-000008f0: 5661 6c75 6545 7272 6f72 da04 6f70 656e  ValueError..open
-00000900: da05 7772 6974 6572 3b00 0000 2902 7236  ..writer;...).r6
-00000910: 0000 00da 0466 696c 6572 2300 0000 7223  .....filer#...r#
-00000920: 0000 0072 2400 0000 da09 6f76 6572 7772  ...r$.....overwr
-00000930: 6974 6562 0000 0073 0a00 0000 0a01 0801  iteb...s........
-00000940: 0e01 1001 22ff 7a12 4669 656c 6441 4243  ....".z.FieldABC
-00000950: 2e6f 7665 7277 7269 7465 6302 0000 0000  .overwritec.....
-00000960: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
-00000970: 0000 0073 0400 0000 6401 5300 2902 7a1f  ...s....d.S.).z.
-00000980: 5365 7420 696e 7465 726e 616c 4669 656c  Set internalFiel
-00000990: 6420 7769 7468 2076 616c 7565 2873 294e  d with value(s)N
-000009a0: 7223 0000 0029 0272 3600 0000 7219 0000  r#...).r6...r...
-000009b0: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-000009c0: 7235 0000 0068 0000 0073 0200 0000 0400  r5...h...s......
-000009d0: 7a13 4669 656c 6441 4243 2e73 6574 5f76  z.FieldABC.set_v
-000009e0: 616c 7565 7363 0500 0000 0000 0000 0000  aluesc..........
-000009f0: 0000 0600 0000 0500 0000 4300 0000 733a  ..........C...s:
-00000a00: 0000 007c 027c 037c 047c 0164 019c 047d  ...|.|.|.|.d...}
-00000a10: 0564 0264 0384 007c 05a0 00a1 0044 0083  .d.d...|.....D..
-00000a20: 017d 0574 017c 0564 0464 0564 068d 037c  .}.t.|.d.d.d...|
-00000a30: 006a 026a 0364 043c 0064 0053 0029 074e  .j.j.d.<.d.S.).N
-00000a40: 2904 da0b 636f 6465 496e 636c 7564 65da  )...codeInclude.
-00000a50: 0b63 6f64 654f 7074 696f 6e73 da08 636f  .codeOptions..co
-00000a60: 6465 4c69 6273 7212 0000 0063 0100 0000  deLibsr....c....
-00000a70: 0000 0000 0000 0000 0300 0000 0700 0000  ................
-00000a80: 5300 0000 7320 0000 0069 007c 005d 0c5c  S...s ...i.|.].\
-00000a90: 027d 017d 027c 0174 007c 017c 02a0 01a1  .}.}.|.t.|.|....
-00000aa0: 0083 0293 0271 0253 0072 2300 0000 2902  .....q.S.r#...).
-00000ab0: 7208 0000 0072 1c00 0000 2903 da02 2e30  r....r....)....0
-00000ac0: da03 6b65 79da 0576 616c 7565 7223 0000  ..key..valuer#..
-00000ad0: 0072 2300 0000 7224 0000 00da 0a3c 6469  .r#...r$.....<di
-00000ae0: 6374 636f 6d70 3e79 0000 0073 0200 0000  ctcomp>y...s....
-00000af0: 2000 7a2b 4669 656c 6441 4243 2e73 6574   .z+FieldABC.set
-00000b00: 5f63 6f64 6573 7472 6561 6d2e 3c6c 6f63  _codestream.<loc
-00000b10: 616c 733e 2e3c 6469 6374 636f 6d70 3e72  als>.<dictcomp>r
-00000b20: 3100 0000 7a0b 2363 6f64 6553 7472 6561  1...z.#codeStrea
-00000b30: 6d29 0272 3700 0000 da09 6469 7265 6374  m).r7.....direct
-00000b40: 6976 6529 04da 0569 7465 6d73 7209 0000  ive)...itemsr...
-00000b50: 0072 1300 0000 7232 0000 0029 0672 3600  .r....r2...).r6.
-00000b60: 0000 7212 0000 00da 0769 6e63 6c75 6465  ..r......include
-00000b70: da07 6f70 7469 6f6e 735a 046c 6962 7372  ..optionsZ.libsr
-00000b80: 2200 0000 7223 0000 0072 2300 0000 7224  "...r#...r#...r$
-00000b90: 0000 00da 0e73 6574 5f63 6f64 6573 7472  .....set_codestr
-00000ba0: 6561 6d6c 0000 0073 1200 0000 0208 0201  eaml...s........
-00000bb0: 0201 0201 06fc 1206 0201 0601 12ff 7a17  ..............z.
-00000bc0: 4669 656c 6441 4243 2e73 6574 5f63 6f64  FieldABC.set_cod
-00000bd0: 6573 7472 6561 6d63 0500 0000 0000 0000  estreamc........
-00000be0: 0000 0000 0700 0000 0400 0000 4300 0000  ............C...
-00000bf0: 7348 0000 007c 006a 006a 0164 0119 007d  sH...|.j.j.d...}
-00000c00: 0564 027c 0269 017d 067c 0364 0075 0172  .d.|.i.}.|.d.u.r
-00000c10: 127c 037c 0664 033c 007c 0464 0075 0172  .|.|.d.<.|.d.u.r
-00000c20: 1a7c 047c 0664 043c 0074 027c 067c 0164  .|.|.d.<.t.|.|.d
-00000c30: 058d 027c 057c 013c 0064 0053 0029 064e  ...|.|.<.d.S.).N
-00000c40: 7214 0000 00da 0474 7970 6572 4800 0000  r......typerH...
-00000c50: da08 6772 6164 6965 6e74 a901 7237 0000  ..gradient..r7..
-00000c60: 0029 0372 1300 0000 7232 0000 0072 0a00  .).r....r2...r..
-00000c70: 0000 2907 7236 0000 0072 3700 0000 da05  ..).r6...r7.....
-00000c80: 7479 7065 5f72 4800 0000 7250 0000 00da  type_rH...rP....
-00000c90: 0a62 6f75 6e64 6172 6965 7372 2200 0000  .boundariesr"...
-00000ca0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
-00000cb0: 0c73 6574 5f62 6f75 6e64 6172 797e 0000  .set_boundary~..
-00000cc0: 0073 0e00 0000 0c01 0801 0801 0801 0801  .s..............
-00000cd0: 0801 1401 7a15 4669 656c 6441 4243 2e73  ....z.FieldABC.s
-00000ce0: 6574 5f62 6f75 6e64 6172 7963 0200 0000  et_boundaryc....
-00000cf0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000d00: 4300 0000 7310 0000 007c 017c 006a 006a  C...s....|.|.j.j
-00000d10: 0164 013c 0064 0053 0029 024e 722f 0000  .d.<.d.S.).Nr/..
-00000d20: 0029 0272 1300 0000 7239 0000 0029 0272  .).r....r9...).r
-00000d30: 3600 0000 7237 0000 0072 2300 0000 7223  6...r7...r#...r#
-00000d40: 0000 0072 2400 0000 da08 7365 745f 6e61  ...r$.....set_na
-00000d50: 6d65 8700 0000 7302 0000 0010 017a 1146  me....s......z.F
-00000d60: 6965 6c64 4142 432e 7365 745f 6e61 6d65  ieldABC.set_name
-00000d70: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000d80: 0004 0000 0043 0000 0073 1200 0000 7400  .....C...s....t.
-00000d90: a001 7c00 6a02 6a03 6401 1900 a101 5300  ..|.j.j.d.....S.
-00000da0: 2902 4e72 3100 0000 2904 7220 0000 00da  ).Nr1...).r ....
-00000db0: 0561 7272 6179 7213 0000 0072 3200 0000  .arrayr....r2...
-00000dc0: 723c 0000 0072 2300 0000 7223 0000 0072  r<...r#...r#...r
-00000dd0: 2400 0000 da09 6765 745f 6172 7261 798a  $.....get_array.
-00000de0: 0000 0073 0200 0000 1201 7a12 4669 656c  ...s......z.Fiel
-00000df0: 6441 4243 2e67 6574 5f61 7272 6179 a902  dABC.get_array..
-00000e00: 4e4e 2915 da08 5f5f 6e61 6d65 5f5f da0a  NN)...__name__..
-00000e10: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000e20: 616c 6e61 6d65 5f5f da03 7374 72da 0f5f  alname__..str.._
-00000e30: 5f61 6e6e 6f74 6174 696f 6e73 5f5f da0b  _annotations__..
-00000e40: 636c 6173 736d 6574 686f 6472 2500 0000  classmethodr%...
-00000e50: 7206 0000 0072 2a00 0000 723a 0000 0072  r....r*...r:...r
-00000e60: 3b00 0000 7242 0000 0072 0300 0000 7235  ;...rB...r....r5
-00000e70: 0000 00da 1444 4546 4155 4c54 5f43 4f44  .....DEFAULT_COD
-00000e80: 455f 494e 434c 5544 45da 1444 4546 4155  E_INCLUDE..DEFAU
-00000e90: 4c54 5f43 4f44 455f 4f50 5449 4f4e 53da  LT_CODE_OPTIONS.
-00000ea0: 1144 4546 4155 4c54 5f43 4f44 455f 4c49  .DEFAULT_CODE_LI
-00000eb0: 4253 724e 0000 0072 5400 0000 7255 0000  BSrN...rT...rU..
-00000ec0: 0072 5700 0000 7223 0000 0072 2300 0000  .rW...r#...r#...
-00000ed0: 7223 0000 0072 2400 0000 7210 0000 0020  r#...r$...r.... 
-00000ee0: 0000 0073 2400 0000 0a00 0801 0202 1001  ...s$...........
-00000ef0: 021b 1401 0a06 0819 0803 0206 0a01 0206  ................
-00000f00: 0201 0201 0afb 0a12 0809 0c03 7210 0000  ............r...
-00000f10: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000f20: 0000 0200 0000 4000 0000 7318 0000 0065  ......@...s....e
-00000f30: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
-00000f40: 005a 0464 0453 0029 05da 0e56 6f6c 5363  .Z.d.S.)...VolSc
-00000f50: 616c 6172 4669 656c 64da 0e76 6f6c 5363  alarField..volSc
-00000f60: 616c 6172 4669 656c 6463 0200 0000 0000  alarFieldc......
-00000f70: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00000f80: 0000 7342 0000 0074 007c 0174 0183 0272  ..sB...t.|.t...r
-00000f90: 0c74 027c 0164 0164 028d 027d 026e 0d74  .t.|.d.d...}.n.t
-00000fa0: 0374 047c 0183 0164 0374 057c 0183 019b  .t.|...d.t.|....
-00000fb0: 009d 0264 028d 027d 027c 027c 006a 066a  ...d...}.|.|.j.j
-00000fc0: 0764 043c 0064 0053 0029 054e da07 756e  .d.<.d.S.).N..un
-00000fd0: 6966 6f72 6d72 5100 0000 7a26 696e 7465  iformrQ...z&inte
-00000fe0: 726e 616c 4669 656c 6420 6e6f 6e75 6e69  rnalField nonuni
-00000ff0: 666f 726d 0a4c 6973 743c 7363 616c 6172  form.List<scalar
-00001000: 3e0a 7231 0000 0029 0872 3300 0000 7205  >.r1...).r3...r.
-00001010: 0000 0072 0e00 0000 720d 0000 00da 046c  ...r....r......l
-00001020: 6973 74da 036c 656e 7213 0000 0072 3200  ist..lenr....r2.
-00001030: 0000 2903 7236 0000 0072 1900 0000 7248  ..).r6...r....rH
-00001040: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-00001050: 0000 7235 0000 0091 0000 0073 0e00 0000  ..r5.......s....
-00001060: 0a01 0e01 0202 0601 0c01 06fe 1004 7a19  ..............z.
-00001070: 566f 6c53 6361 6c61 7246 6965 6c64 2e73  VolScalarField.s
-00001080: 6574 5f76 616c 7565 734e a905 7259 0000  et_valuesN..rY..
-00001090: 0072 5a00 0000 725b 0000 0072 1100 0000  .rZ...r[...r....
-000010a0: 7235 0000 0072 2300 0000 7223 0000 0072  r5...r#...r#...r
-000010b0: 2300 0000 7224 0000 0072 6200 0000 8e00  #...r$...rb.....
-000010c0: 0000 7306 0000 0008 0004 010c 0272 6200  ..s..........rb.
-000010d0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000010e0: 0000 0003 0000 0040 0000 0073 1a00 0000  .......@...s....
-000010f0: 6500 5a01 6400 5a02 6401 5a03 6405 6403  e.Z.d.Z.d.Z.d.d.
-00001100: 6404 8401 5a04 6402 5300 2906 da0e 566f  d...Z.d.S.)...Vo
-00001110: 6c56 6563 746f 7246 6965 6c64 da0e 766f  lVectorField..vo
-00001120: 6c56 6563 746f 7246 6965 6c64 4e63 0400  lVectorFieldNc..
-00001130: 0000 0000 0000 0000 0000 0700 0000 0600  ................
-00001140: 0000 4300 0000 7300 0100 007c 0264 0075  ..C...s....|.d.u
-00001150: 0172 347c 0364 0075 0072 0a74 0082 0174  .r4|.d.u.r.t...t
-00001160: 017c 0174 026a 0383 0273 1274 0082 017c  .|.t.j...s.t...|
-00001170: 016a 0464 016b 0373 277c 016a 057c 026a  .j.d.k.s'|.j.|.j
-00001180: 0504 0003 006b 0372 257c 036a 056b 0372  .....k.r%|.j.k.r
-00001190: 2974 0082 0101 006e 0274 0082 017c 017d  )t.....n.t...|.}
-000011a0: 0474 02a0 067c 047c 027c 0367 03a1 016a  .t...|.|.|.g...j
-000011b0: 077d 0174 017c 0174 026a 0383 0272 487c  .}.t.|.t.j...rH|
-000011c0: 016a 0464 026b 0372 4174 0082 0164 0364  .j.d.k.rAt...d.d
-000011d0: 0484 007c 0144 0083 017d 0174 087c 0183  ...|.D...}.t.|..
-000011e0: 017d 057c 0564 056b 0272 6a74 017c 0164  .}.|.d.k.rjt.|.d
-000011f0: 0619 0074 0983 0272 6a74 0a64 0764 08a0  ...t...rjt.d.d..
-00001200: 0b64 0964 0a84 007c 0144 0083 01a1 0117  .d.d...|.D......
-00001210: 0064 0b17 0064 0c64 0d8d 027d 066e 0e74  .d...d.d...}.n.t
-00001220: 0c64 0e64 0484 007c 0144 0083 0164 0f7c  .d.d...|.D...d.|
-00001230: 059b 009d 0264 0d8d 027d 067c 067c 006a  .....d...}.|.|.j
-00001240: 0d6a 0e64 103c 0064 0053 0029 114e 7217  .j.d.<.d.S.).Nr.
-00001250: 0000 00e9 0200 0000 6301 0000 0000 0000  ........c.......
-00001260: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00001270: 00f3 1400 0000 6700 7c00 5d06 7d01 7400  ......g.|.].}.t.
-00001280: 7c01 8301 9102 7102 5300 7223 0000 0029  |.....q.S.r#...)
-00001290: 0172 6500 0000 2902 7246 0000 00da 0361  .re...).rF.....a
-000012a0: 7272 7223 0000 0072 2300 0000 7224 0000  rrr#...r#...r$..
-000012b0: 00da 0a3c 6c69 7374 636f 6d70 3ead 0000  ...<listcomp>...
-000012c0: 00f3 0200 0000 1400 7a2d 566f 6c56 6563  ........z-VolVec
-000012d0: 746f 7246 6965 6c64 2e73 6574 5f76 616c  torField.set_val
-000012e0: 7565 732e 3c6c 6f63 616c 733e 2e3c 6c69  ues.<locals>.<li
-000012f0: 7374 636f 6d70 3ee9 0300 0000 7201 0000  stcomp>.....r...
-00001300: 0072 1500 0000 da01 2063 0100 0000 0000  .r...... c......
-00001310: 0000 0000 0000 0200 0000 0300 0000 7300  ..............s.
-00001320: 0000 7318 0000 0081 007c 005d 077d 0174  ..s......|.].}.t
-00001330: 007c 0183 0156 0001 0071 0264 0053 0072  .|...V...q.d.S.r
-00001340: 2700 0000 2901 725c 0000 00a9 0272 4600  '...).r\.....rF.
-00001350: 0000 7248 0000 0072 2300 0000 7223 0000  ..rH...r#...r#..
-00001360: 0072 2400 0000 da09 3c67 656e 6578 7072  .r$.....<genexpr
-00001370: 3eb2 0000 0073 0400 0000 0280 1600 7a2c  >....s........z,
-00001380: 566f 6c56 6563 746f 7246 6965 6c64 2e73  VolVectorField.s
-00001390: 6574 5f76 616c 7565 732e 3c6c 6f63 616c  et_values.<local
-000013a0: 733e 2e3c 6765 6e65 7870 723e 7216 0000  s>.<genexpr>r...
-000013b0: 0072 6400 0000 7251 0000 0063 0100 0000  .rd...rQ...c....
-000013c0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000013d0: 5300 0000 726b 0000 0072 2300 0000 2901  S...rk...r#...).
-000013e0: 720d 0000 0072 7100 0000 7223 0000 0072  r....rq...r#...r
-000013f0: 2300 0000 7224 0000 0072 6d00 0000 b700  #...r$...rm.....
-00001400: 0000 726e 0000 007a 2669 6e74 6572 6e61  ..rn...z&interna
-00001410: 6c46 6965 6c64 206e 6f6e 756e 6966 6f72  lField nonunifor
-00001420: 6d0a 4c69 7374 3c76 6563 746f 723e 0a72  m.List<vector>.r
-00001430: 3100 0000 290f 723e 0000 0072 3300 0000  1...).r>...r3...
-00001440: 7220 0000 00da 076e 6461 7272 6179 da04  r .....ndarray..
-00001450: 6e64 696d da04 7369 7a65 da05 7374 6163  ndim..size..stac
-00001460: 6bda 0154 7266 0000 0072 0500 0000 720e  k..Trf...r....r.
-00001470: 0000 00da 046a 6f69 6e72 0d00 0000 7213  .....joinr....r.
-00001480: 0000 0072 3200 0000 2907 7236 0000 0072  ...r2...).r6...r
-00001490: 1900 0000 5a02 7679 5a02 767a 5a02 7678  ....Z.vyZ.vzZ.vx
-000014a0: 5a06 6e5f 656c 656d 7248 0000 0072 2300  Z.n_elemrH...r#.
-000014b0: 0000 7223 0000 0072 2400 0000 7235 0000  ..r#...r$...r5..
-000014c0: 009f 0000 0073 3400 0000 0801 0801 0401  .....s4.........
-000014d0: 0c01 0401 2201 0401 04ff 0401 0401 1201  ...."...........
-000014e0: 0c02 0a01 0401 0e01 0802 1601 0201 1a01  ................
-000014f0: 0201 08fe 0205 0c01 0801 06fe 1004 7a19  ..............z.
-00001500: 566f 6c56 6563 746f 7246 6965 6c64 2e73  VolVectorField.s
-00001510: 6574 5f76 616c 7565 7372 5800 0000 7267  et_valuesrX...rg
-00001520: 0000 0072 2300 0000 7223 0000 0072 2300  ...r#...r#...r#.
-00001530: 0000 7224 0000 0072 6800 0000 9c00 0000  ..r$...rh.......
-00001540: 7306 0000 0008 0004 010e 0272 6800 0000  s..........rh...
-00001550: 2902 7263 0000 0072 6900 0000 6301 0000  ).rc...ri...c...
-00001560: 0000 0000 0000 0000 0004 0000 0008 0000  ................
-00001570: 0043 0000 0073 8000 0000 6400 7d01 7400  .C...s....d.}.t.
-00001580: 7c00 6401 8302 8f22 7d02 7c02 4400 5d17  |.d...."}.|.D.].
-00001590: 7d03 7c03 a001 a100 7d03 7c03 a002 6402  }.|.....}.|...d.
-000015a0: a101 7221 7c03 a003 a100 6403 1900 6400  ..r!|.....d...d.
-000015b0: 6403 8502 1900 7d01 0100 6e01 710a 5700  d.....}...n.q.W.
-000015c0: 6400 0400 0400 8303 0100 6e08 3100 732c  d.........n.1.s,
-000015d0: 7701 0100 0100 0100 5900 0100 7c01 6400  w.......Y...|.d.
-000015e0: 7500 7237 7404 8201 7405 7c01 1900 7d01  u.r7t...t.|...}.
-000015f0: 7c01 a006 7c00 a101 5300 2904 4eda 0172  |...|...S.).N..r
-00001600: 7a06 636c 6173 7320 e9ff ffff ff29 0772  z.class .....).r
-00001610: 3f00 0000 721c 0000 0072 1d00 0000 da05  ?...r....r......
-00001620: 7370 6c69 74da 0c52 756e 7469 6d65 4572  split..RuntimeEr
-00001630: 726f 72da 0763 6c61 7373 6573 722a 0000  ror..classesr*..
-00001640: 0029 0472 2600 0000 7211 0000 0072 4100  .).r&...r....rA.
-00001650: 0000 da04 6c69 6e65 7223 0000 0072 2300  ....liner#...r#.
-00001660: 0000 7224 0000 00da 0f72 6561 645f 6669  ..r$.....read_fi
-00001670: 656c 645f 6669 6c65 c000 0000 731c 0000  eld_file....s...
-00001680: 0004 010c 0108 0108 010a 0114 0104 0102  ................
-00001690: fe02 801c fd08 0704 0108 020a 0272 7f00  .............r..
-000016a0: 0000 2920 da07 5f5f 646f 635f 5f72 1e00  ..) ..__doc__r..
-000016b0: 0000 da03 6162 6372 0200 0000 7203 0000  ....abcr....r...
-000016c0: 00da 0269 6f72 0400 0000 da07 6e75 6d62  ...ior......numb
-000016d0: 6572 7372 0500 0000 da07 7061 7468 6c69  ersr......pathli
-000016e0: 6272 0600 0000 da05 6e75 6d70 7972 2000  br......numpyr .
-000016f0: 0000 5a1d 666c 7569 6473 696d 666f 616d  ..Z.fluidsimfoam
-00001700: 2e66 6f61 6d5f 696e 7075 745f 6669 6c65  .foam_input_file
-00001710: 7372 0700 0000 da21 666c 7569 6473 696d  sr.....!fluidsim
-00001720: 666f 616d 2e66 6f61 6d5f 696e 7075 745f  foam.foam_input_
-00001730: 6669 6c65 732e 6173 7472 0800 0000 7209  files.astr....r.
-00001740: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
-00001750: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00001760: 0072 5f00 0000 7260 0000 0072 6100 0000  .r_...r`...ra...
-00001770: 7210 0000 0072 6200 0000 7268 0000 0072  r....rb...rh...r
-00001780: 7d00 0000 727f 0000 0072 2300 0000 7223  }...r....r#...r#
-00001790: 0000 0072 2300 0000 7224 0000 00da 083c  ...r#...r$.....<
-000017a0: 6d6f 6475 6c65 3e01 0000 0073 2400 0000  module>....s$...
-000017b0: 0400 0804 1001 0c01 0c01 0c01 0802 0c02  ................
-000017c0: 2801 040b 0202 02ff 0403 1003 106e 100e  (............n..
-000017d0: 0a21 0c03                                .!..
+000000a0: 6d16 5a16 0100 6409 5a17 640a 5a18 640b  m.Z...d.Z.d.Z.d.
+000000b0: 5a19 4700 640c 640d 8400 640d 6503 8303  Z.G.d.d...d.e...
+000000c0: 5a1a 4700 640e 640f 8400 640f 651a 8303  Z.G.d.d...d.e...
+000000d0: 5a1b 4700 6410 6411 8400 6411 651a 8303  Z.G.d.d...d.e...
+000000e0: 5a1c 4700 6412 6413 8400 6413 651a 8303  Z.G.d.d...d.e...
+000000f0: 5a1d 6414 6415 8400 651b 651c 651d 6603  Z.d.d...e.e.e.f.
+00000100: 4400 8301 5a1e 6416 6417 8400 5a1f 6402  D...Z.d.d...Z.d.
+00000110: 5300 2918 7a1e 4865 6c70 6572 2074 6f20  S.).z.Helper to 
+00000120: 6372 6561 7465 2066 6965 6c64 2066 696c  create field fil
+00000130: 6573 0a0a e900 0000 004e 2902 da03 4142  es.......N)...AB
+00000140: 43da 0e61 6273 7472 6163 746d 6574 686f  C..abstractmetho
+00000150: 6429 01da 0853 7472 696e 6749 4f29 01da  d)...StringIO)..
+00000160: 064e 756d 6265 7229 01da 0450 6174 6829  .Number)...Path)
+00000170: 01da 0570 6172 7365 2907 da04 436f 6465  ...parse)...Code
+00000180: da0a 436f 6465 5374 7265 616d da04 4469  ..CodeStream..Di
+00000190: 6374 da0c 4469 6d65 6e73 696f 6e53 6574  ct..DimensionSet
+000001a0: da0d 466f 616d 496e 7075 7446 696c 65da  ..FoamInputFile.
+000001b0: 044c 6973 74da 0556 616c 7565 7a12 2369  .List..Valuez.#i
+000001c0: 6e63 6c75 6465 2022 6676 4346 442e 4822  nclude "fvCFD.H"
+000001d0: 7a46 2d49 2428 4c49 425f 5352 4329 2f66  zF-I$(LIB_SRC)/f
+000001e0: 696e 6974 6556 6f6c 756d 652f 6c6e 496e  initeVolume/lnIn
+000001f0: 636c 7564 6520 5c0a 2d49 2428 4c49 425f  clude \.-I$(LIB_
+00000200: 5352 4329 2f6d 6573 6854 6f6f 6c73 2f6c  SRC)/meshTools/l
+00000210: 6e49 6e63 6c75 6465 7a1c 2d6c 6d65 7368  nIncludez.-lmesh
+00000220: 546f 6f6c 7320 5c0a 2d6c 6669 6e69 7465  Tools \.-lfinite
+00000230: 566f 6c75 6d65 6300 0000 0000 0000 0000  Volumec.........
+00000240: 0000 0000 0000 0005 0000 0040 0000 0073  ...........@...s
+00000250: 9200 0000 6500 5a01 6400 5a02 5500 6503  ....e.Z.d.Z.U.e.
+00000260: 6504 6401 3c00 6505 641a 6403 6503 6602  e.d.<.e.d.d.e.f.
+00000270: 6404 6405 8405 8301 5a06 6505 641a 6406  d.d.....Z.e.d.d.
+00000280: 6503 7019 6507 6602 6407 6408 8405 8301  e.p.e.f.d.d.....
+00000290: 5a08 641b 640a 640b 8401 5a09 640c 640d  Z.d.d.d...Z.d.d.
+000002a0: 8400 5a0a 640e 640f 8400 5a0b 650c 6410  ..Z.d.d...Z.e.d.
+000002b0: 6411 8400 8301 5a0d 650e 650f 6510 6603  d.....Z.e.e.e.f.
+000002c0: 6412 6413 8401 5a11 641b 6414 6415 8401  d.d...Z.d.d.d...
+000002d0: 5a12 6416 6417 8400 5a13 6418 6419 8400  Z.d.d...Z.d.d...
+000002e0: 5a14 6409 5300 291c da08 4669 656c 6441  Z.d.S.)...FieldA
+000002f0: 4243 da03 636c 7346 da04 636f 6465 6303  BC..clsF..codec.
+00000300: 0000 0000 0000 0000 0000 000b 0000 0006  ................
+00000310: 0000 0043 0000 0073 d000 0000 6401 7c01  ...C...s....d.|.
+00000320: 7601 720f 7400 7c01 8301 7d03 7c00 6400  v.r.t.|...}.|.d.
+00000330: 6400 7c03 6402 8d03 5300 7c01 a001 6401  d.|.d...S.|...d.
+00000340: a101 7d04 7c01 a002 6403 7c04 a102 7d05  ..}.|...d.|...}.
+00000350: 7c01 a001 6404 7c04 7c05 a103 7d06 7c01  |...d.|.|...}.|.
+00000360: a002 6405 7c04 7c05 a103 7d07 7c01 6400  ..d.|.|...}.|.d.
+00000370: 7c04 8502 1900 6406 1700 7d08 7c02 733c  |.....d...}.|.s<
+00000380: 7c08 6407 7c01 7c05 6400 8502 1900 1700  |.d.|.|.d.......
+00000390: 3700 7d08 7400 7c08 8301 7d03 7c01 7c06  7.}.t.|...}.|.|.
+000003a0: 6408 1700 7c07 8502 1900 a003 a100 7d09  d...|.........}.
+000003b0: 7c09 a004 6404 a101 7256 7405 a006 6409  |...d...rVt...d.
+000003c0: 640a 7c09 a103 7d09 7407 a008 7409 7c09  d.|...}.t...t.|.
+000003d0: 8301 a101 7d0a 7c0a 7c03 5f0a 7c00 640a  ....}.|.|._.|.d.
+000003e0: 640a 7c03 7c0a 640b 8d04 5300 290c 4e5a  d.|.|.d...S.).NZ
+000003f0: 0a6e 6f6e 756e 6966 6f72 6d29 01da 0474  .nonuniform)...t
+00000400: 7265 65da 0d62 6f75 6e64 6172 7946 6965  ree..boundaryFie
+00000410: 6c64 fa01 28fa 0129 7a02 3b0a da01 0ae9  ld..(..)z.;.....
+00000420: 0100 0000 7a04 5b28 295d da00 2902 7212  ....z.[()]..).r.
+00000430: 0000 00da 0676 616c 7565 7329 0b72 0700  .....values).r..
+00000440: 0000 da05 696e 6465 78da 0672 696e 6465  ....index..rinde
+00000450: 78da 0573 7472 6970 da0a 7374 6172 7473  x..strip..starts
+00000460: 7769 7468 da02 7265 da03 7375 62da 026e  with..re..sub..n
+00000470: 70da 076c 6f61 6474 7874 7204 0000 00da  p..loadtxtr.....
+00000480: 0464 6174 6129 0b72 1000 0000 7211 0000  .data).r....r...
+00000490: 00da 1373 6b69 705f 626f 756e 6461 7279  ...skip_boundary
+000004a0: 5f66 6965 6c64 7212 0000 005a 1069 6e64  _fieldr....Z.ind
+000004b0: 6578 5f6e 6f6e 756e 6966 6f72 6d5a 1369  ex_nonuniformZ.i
+000004c0: 6e64 6578 5f62 6f75 6e64 6172 7946 6965  ndex_boundaryFie
+000004d0: 6c64 5a11 696e 6465 785f 6f70 656e 696e  ldZ.index_openin
+000004e0: 675f 7061 725a 1169 6e64 6578 5f63 6c6f  g_parZ.index_clo
+000004f0: 7369 6e67 5f70 6172 5a0d 636f 6465 5f74  sing_parZ.code_t
+00000500: 6f5f 7061 7273 655a 0963 6f64 655f 6461  o_parseZ.code_da
+00000510: 7461 7222 0000 00a9 0072 2400 0000 fa49  tar".....r$....I
+00000520: 2f68 6f6d 652f 7069 6572 7265 2f44 6576  /home/pierre/Dev
+00000530: 2f66 6c75 6964 7369 6d66 6f61 6d2f 7372  /fluidsimfoam/sr
+00000540: 632f 666c 7569 6473 696d 666f 616d 2f66  c/fluidsimfoam/f
+00000550: 6f61 6d5f 696e 7075 745f 6669 6c65 732f  oam_input_files/
+00000560: 6669 656c 6473 2e70 79da 0966 726f 6d5f  fields.py..from_
+00000570: 636f 6465 2200 0000 7326 0000 0008 0208  code"...s&......
+00000580: 010e 010a 020c 010e 0104 0106 0104 ff10  ................
+00000590: 0404 0114 0108 0214 010a 020e 010e 0206  ................
+000005a0: 0210 017a 1246 6965 6c64 4142 432e 6672  ...z.FieldABC.fr
+000005b0: 6f6d 5f63 6f64 65da 0470 6174 6863 0300  om_code..pathc..
+000005c0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+000005d0: 0000 4300 0000 7324 0000 0074 007c 0183  ..C...s$...t.|..
+000005e0: 017d 017c 006a 017c 01a0 02a1 007c 0264  .}.|.j.|.....|.d
+000005f0: 018d 027d 037c 017c 035f 037c 0353 0029  ...}.|.|._.|.S.)
+00000600: 024e 2901 7223 0000 0029 0472 0600 0000  .N).r#...).r....
+00000610: 7226 0000 00da 0972 6561 645f 7465 7874  r&.....read_text
+00000620: 7227 0000 0029 0472 1000 0000 7227 0000  r'...).r....r'..
+00000630: 0072 2300 0000 da05 6669 656c 6472 2400  .r#.....fieldr$.
+00000640: 0000 7224 0000 0072 2500 0000 da09 6672  ..r$...r%.....fr
+00000650: 6f6d 5f70 6174 683e 0000 0073 0c00 0000  om_path>...s....
+00000660: 0802 0401 0801 06ff 0603 0401 7a12 4669  ............z.Fi
+00000670: 656c 6441 4243 2e66 726f 6d5f 7061 7468  eldABC.from_path
+00000680: 4e63 0500 0000 0000 0000 0000 0000 0600  Nc..............
+00000690: 0000 0500 0000 4300 0000 7370 0000 007c  ......C...sp...|
+000006a0: 0364 0075 0172 087c 037c 005f 006e 2264  .d.u.r.|.|._.n"d
+000006b0: 0164 027c 006a 017c 0164 039c 047d 0574  .d.|.j.|.d...}.t
+000006c0: 027c 0274 0383 0273 1974 037c 0283 017d  .|.t...s.t.|...}
+000006d0: 0274 047c 057c 0264 0064 049c 0264 058d  .t.|.|.d.d...d..
+000006e0: 027c 005f 007c 006a 00a0 0564 0669 00a1  .|._.|.j...d.i..
+000006f0: 0201 007c 0464 0075 0172 337c 00a0 067c  ...|.d.u.r3|...|
+00000700: 04a1 0101 0064 007c 005f 0764 0053 0029  .....d.|._.d.S.)
+00000710: 074e 7a03 322e 30da 0561 7363 6969 2904  .Nz.2.0..ascii).
+00000720: da07 7665 7273 696f 6eda 0666 6f72 6d61  ..version..forma
+00000730: 74da 0563 6c61 7373 da06 6f62 6a65 6374  t..class..object
+00000740: 2902 da0a 6469 6d65 6e73 696f 6e73 da0d  )...dimensions..
+00000750: 696e 7465 726e 616c 4669 656c 6429 01da  internalField)..
+00000760: 0863 6869 6c64 7265 6e72 1300 0000 2908  .childrenr....).
+00000770: 7212 0000 0072 1000 0000 da0a 6973 696e  r....r......isin
+00000780: 7374 616e 6365 720b 0000 0072 0c00 0000  stancer....r....
+00000790: da09 7365 745f 6368 696c 64da 0a73 6574  ..set_child..set
+000007a0: 5f76 616c 7565 7372 2700 0000 2906 da04  _valuesr'...)...
+000007b0: 7365 6c66 da04 6e61 6d65 da09 6469 6d65  self..name..dime
+000007c0: 6e73 696f 6e72 1200 0000 7219 0000 00da  nsionr....r.....
+000007d0: 0469 6e66 6f72 2400 0000 7224 0000 0072  .infor$...r$...r
+000007e0: 2500 0000 da08 5f5f 696e 6974 5f5f 4700  %.....__init__G.
+000007f0: 0000 7320 0000 0008 0108 0102 0302 0104  ..s ............
+00000800: 0102 0106 fc0a 0708 0102 020a 0108 ff0e  ................
+00000810: 0408 020a 010a 027a 1146 6965 6c64 4142  .......z.FieldAB
+00000820: 432e 5f5f 696e 6974 5f5f 6301 0000 0000  C.__init__c.....
+00000830: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00000840: 0000 0073 0a00 0000 7c00 6a00 a001 a100  ...s....|.j.....
+00000850: 5300 a901 4e29 0272 1200 0000 da04 6475  S...N).r......du
+00000860: 6d70 a901 7236 0000 0072 2400 0000 7224  mp..r6...r$...r$
+00000870: 0000 0072 2500 0000 723c 0000 0060 0000  ...r%...r<...`..
+00000880: 0073 0200 0000 0a01 7a0d 4669 656c 6441  .s......z.FieldA
+00000890: 4243 2e64 756d 7063 0100 0000 0000 0000  BC.dumpc........
+000008a0: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
+000008b0: 7352 0000 007c 006a 0064 0075 0072 0974  sR...|.j.d.u.r.t
+000008c0: 0164 0183 0182 0174 027c 006a 0064 0283  .d.....t.|.j.d..
+000008d0: 028f 107d 017c 01a0 037c 00a0 04a1 00a1  ...}.|...|......
+000008e0: 0101 0057 0064 0004 0004 0083 0301 0064  ...W.d.........d
+000008f0: 0053 0031 0073 2277 0101 0001 0001 0059  .S.1.s"w.......Y
+00000900: 0001 0064 0053 0029 034e 7a11 7365 6c66  ...d.S.).Nz.self
+00000910: 2e70 6174 6820 6973 204e 6f6e 65da 0177  .path is None..w
+00000920: 2905 7227 0000 00da 0a56 616c 7565 4572  ).r'.....ValueEr
+00000930: 726f 72da 046f 7065 6eda 0577 7269 7465  ror..open..write
+00000940: 723c 0000 0029 0272 3600 0000 da04 6669  r<...).r6.....fi
+00000950: 6c65 7224 0000 0072 2400 0000 7225 0000  ler$...r$...r%..
+00000960: 00da 096f 7665 7277 7269 7465 6300 0000  ...overwritec...
+00000970: 730a 0000 000a 0108 010e 0110 0122 ff7a  s............".z
+00000980: 1246 6965 6c64 4142 432e 6f76 6572 7772  .FieldABC.overwr
+00000990: 6974 6563 0200 0000 0000 0000 0000 0000  itec............
+000009a0: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000009b0: 0064 0153 0029 027a 1f53 6574 2069 6e74  .d.S.).z.Set int
+000009c0: 6572 6e61 6c46 6965 6c64 2077 6974 6820  ernalField with 
+000009d0: 7661 6c75 6528 7329 4e72 2400 0000 a902  value(s)Nr$.....
+000009e0: 7236 0000 0072 1900 0000 7224 0000 0072  r6...r....r$...r
+000009f0: 2400 0000 7225 0000 0072 3500 0000 6900  $...r%...r5...i.
+00000a00: 0000 7302 0000 0004 007a 1346 6965 6c64  ..s......z.Field
+00000a10: 4142 432e 7365 745f 7661 6c75 6573 6305  ABC.set_valuesc.
+00000a20: 0000 0000 0000 0000 0000 0006 0000 0005  ................
+00000a30: 0000 0043 0000 0073 3a00 0000 7c02 7c03  ...C...s:...|.|.
+00000a40: 7c04 7c01 6401 9c04 7d05 6402 6403 8400  |.|.d...}.d.d...
+00000a50: 7c05 a000 a100 4400 8301 7d05 7401 7c05  |.....D...}.t.|.
+00000a60: 6404 6405 6406 8d03 7c00 6a02 6a03 6404  d.d.d...|.j.j.d.
+00000a70: 3c00 6400 5300 2907 4e29 04da 0b63 6f64  <.d.S.).N)...cod
+00000a80: 6549 6e63 6c75 6465 da0b 636f 6465 4f70  eInclude..codeOp
+00000a90: 7469 6f6e 73da 0863 6f64 654c 6962 7372  tions..codeLibsr
+00000aa0: 1100 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000ab0: 0003 0000 0007 0000 0053 0000 0073 2000  .........S...s .
+00000ac0: 0000 6900 7c00 5d0c 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
+00000ad0: 7400 7c01 7c02 a001 a100 8302 9302 7102  t.|.|.........q.
+00000ae0: 5300 7224 0000 0029 0272 0800 0000 721c  S.r$...).r....r.
+00000af0: 0000 0029 03da 022e 30da 036b 6579 da05  ...)....0..key..
+00000b00: 7661 6c75 6572 2400 0000 7224 0000 0072  valuer$...r$...r
+00000b10: 2500 0000 da0a 3c64 6963 7463 6f6d 703e  %.....<dictcomp>
+00000b20: 7a00 0000 7302 0000 0020 007a 2b46 6965  z...s.... .z+Fie
+00000b30: 6c64 4142 432e 7365 745f 636f 6465 7374  ldABC.set_codest
+00000b40: 7265 616d 2e3c 6c6f 6361 6c73 3e2e 3c64  ream.<locals>.<d
+00000b50: 6963 7463 6f6d 703e 7231 0000 007a 0b23  ictcomp>r1...z.#
+00000b60: 636f 6465 5374 7265 616d 2902 7237 0000  codeStream).r7..
+00000b70: 00da 0964 6972 6563 7469 7665 2904 da05  ...directive)...
+00000b80: 6974 656d 7372 0900 0000 7212 0000 0072  itemsr....r....r
+00000b90: 3200 0000 2906 7236 0000 0072 1100 0000  2...).r6...r....
+00000ba0: da07 696e 636c 7564 65da 076f 7074 696f  ..include..optio
+00000bb0: 6e73 5a04 6c69 6273 7222 0000 0072 2400  nsZ.libsr"...r$.
+00000bc0: 0000 7224 0000 0072 2500 0000 da0e 7365  ..r$...r%.....se
+00000bd0: 745f 636f 6465 7374 7265 616d 6d00 0000  t_codestreamm...
+00000be0: 7312 0000 0002 0802 0102 0102 0106 fc12  s...............
+00000bf0: 0602 0106 0112 ff7a 1746 6965 6c64 4142  .......z.FieldAB
+00000c00: 432e 7365 745f 636f 6465 7374 7265 616d  C.set_codestream
+00000c10: 6305 0000 0000 0000 0000 0000 0007 0000  c...............
+00000c20: 0004 0000 0043 0000 0073 4800 0000 7c00  .....C...sH...|.
+00000c30: 6a00 6a01 6401 1900 7d05 6402 7c02 6901  j.j.d...}.d.|.i.
+00000c40: 7d06 7c03 6400 7501 7212 7c03 7c06 6403  }.|.d.u.r.|.|.d.
+00000c50: 3c00 7c04 6400 7501 721a 7c04 7c06 6404  <.|.d.u.r.|.|.d.
+00000c60: 3c00 7402 7c06 7c01 6405 8d02 7c05 7c01  <.t.|.|.d...|.|.
+00000c70: 3c00 6400 5300 2906 4e72 1300 0000 da04  <.d.S.).Nr......
+00000c80: 7479 7065 724a 0000 00da 0867 7261 6469  typerJ.....gradi
+00000c90: 656e 74a9 0172 3700 0000 2903 7212 0000  ent..r7...).r...
+00000ca0: 0072 3200 0000 720a 0000 0029 0772 3600  .r2...r....).r6.
+00000cb0: 0000 7237 0000 00da 0574 7970 655f 724a  ..r7.....type_rJ
+00000cc0: 0000 0072 5200 0000 da0a 626f 756e 6461  ...rR.....bounda
+00000cd0: 7269 6573 7222 0000 0072 2400 0000 7224  riesr"...r$...r$
+00000ce0: 0000 0072 2500 0000 da0c 7365 745f 626f  ...r%.....set_bo
+00000cf0: 756e 6461 7279 7f00 0000 730e 0000 000c  undary....s.....
+00000d00: 0108 0108 0108 0108 0108 0114 017a 1546  .............z.F
+00000d10: 6965 6c64 4142 432e 7365 745f 626f 756e  ieldABC.set_boun
+00000d20: 6461 7279 6302 0000 0000 0000 0000 0000  daryc...........
+00000d30: 0002 0000 0003 0000 0043 0000 0073 1000  .........C...s..
+00000d40: 0000 7c01 7c00 6a00 6a01 6401 3c00 6400  ..|.|.j.j.d.<.d.
+00000d50: 5300 2902 4e72 2f00 0000 2902 7212 0000  S.).Nr/...).r...
+00000d60: 0072 3900 0000 2902 7236 0000 0072 3700  .r9...).r6...r7.
+00000d70: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+00000d80: 00da 0873 6574 5f6e 616d 6588 0000 0073  ...set_name....s
+00000d90: 0200 0000 1001 7a11 4669 656c 6441 4243  ......z.FieldABC
+00000da0: 2e73 6574 5f6e 616d 6563 0100 0000 0000  .set_namec......
+00000db0: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00000dc0: 0000 7312 0000 0074 00a0 017c 006a 026a  ..s....t...|.j.j
+00000dd0: 0364 0119 00a1 0153 0029 024e 7231 0000  .d.....S.).Nr1..
+00000de0: 0029 0472 2000 0000 da05 6172 7261 7972  .).r .....arrayr
+00000df0: 1200 0000 7232 0000 0072 3d00 0000 7224  ....r2...r=...r$
+00000e00: 0000 0072 2400 0000 7225 0000 00da 0967  ...r$...r%.....g
+00000e10: 6574 5f61 7272 6179 8b00 0000 7302 0000  et_array....s...
+00000e20: 0012 017a 1246 6965 6c64 4142 432e 6765  ...z.FieldABC.ge
+00000e30: 745f 6172 7261 7929 0146 a902 4e4e 2915  t_array).F..NN).
+00000e40: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000e50: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000e60: 6d65 5f5f da03 7374 72da 0f5f 5f61 6e6e  me__..str..__ann
+00000e70: 6f74 6174 696f 6e73 5f5f da0b 636c 6173  otations__..clas
+00000e80: 736d 6574 686f 6472 2600 0000 7206 0000  smethodr&...r...
+00000e90: 0072 2a00 0000 723a 0000 0072 3c00 0000  .r*...r:...r<...
+00000ea0: 7243 0000 0072 0300 0000 7235 0000 00da  rC...r....r5....
+00000eb0: 1444 4546 4155 4c54 5f43 4f44 455f 494e  .DEFAULT_CODE_IN
+00000ec0: 434c 5544 45da 1444 4546 4155 4c54 5f43  CLUDE..DEFAULT_C
+00000ed0: 4f44 455f 4f50 5449 4f4e 53da 1144 4546  ODE_OPTIONS..DEF
+00000ee0: 4155 4c54 5f43 4f44 455f 4c49 4253 7250  AULT_CODE_LIBSrP
+00000ef0: 0000 0072 5600 0000 7257 0000 0072 5900  ...rV...rW...rY.
+00000f00: 0000 7224 0000 0072 2400 0000 7224 0000  ..r$...r$...r$..
+00000f10: 0072 2500 0000 720f 0000 001f 0000 0073  .r%...r........s
+00000f20: 2400 0000 0a00 0801 0202 1201 021b 1601  $...............
+00000f30: 0a08 0819 0803 0206 0a01 0206 0201 0201  ................
+00000f40: 0afb 0a12 0809 0c03 720f 0000 0063 0000  ........r....c..
+00000f50: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+00000f60: 0000 4000 0000 f318 0000 0065 005a 0164  ..@........e.Z.d
+00000f70: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
+00000f80: 0453 0029 05da 0e56 6f6c 5363 616c 6172  .S.)...VolScalar
+00000f90: 4669 656c 645a 0e76 6f6c 5363 616c 6172  FieldZ.volScalar
+00000fa0: 4669 656c 6463 0200 0000 0000 0000 0000  Fieldc..........
+00000fb0: 0000 0300 0000 0500 0000 4300 0000 7342  ..........C...sB
+00000fc0: 0000 0074 007c 0174 0183 0272 0c74 027c  ...t.|.t...r.t.|
+00000fd0: 0164 0164 028d 027d 026e 0d74 0374 047c  .d.d...}.n.t.t.|
+00000fe0: 0183 0164 0374 057c 0183 019b 009d 0264  ...d.t.|.......d
+00000ff0: 028d 027d 027c 027c 006a 066a 0764 043c  ...}.|.|.j.j.d.<
+00001000: 0064 0053 0029 054e da07 756e 6966 6f72  .d.S.).N..unifor
+00001010: 6d72 5300 0000 7a26 696e 7465 726e 616c  mrS...z&internal
+00001020: 4669 656c 6420 6e6f 6e75 6e69 666f 726d  Field nonuniform
+00001030: 0a4c 6973 743c 7363 616c 6172 3e0a 7231  .List<scalar>.r1
+00001040: 0000 0029 0872 3300 0000 7205 0000 0072  ...).r3...r....r
+00001050: 0e00 0000 720d 0000 00da 046c 6973 74da  ....r......list.
+00001060: 036c 656e 7212 0000 0072 3200 0000 2903  .lenr....r2...).
+00001070: 7236 0000 0072 1900 0000 724a 0000 0072  r6...r....rJ...r
+00001080: 2400 0000 7224 0000 0072 2500 0000 7235  $...r$...r%...r5
+00001090: 0000 0092 0000 0073 0e00 0000 0a01 0e01  .......s........
+000010a0: 0202 0601 0c01 06fe 1004 7a19 566f 6c53  ..........z.VolS
+000010b0: 6361 6c61 7246 6965 6c64 2e73 6574 5f76  calarField.set_v
+000010c0: 616c 7565 734e a905 725b 0000 0072 5c00  aluesN..r[...r\.
+000010d0: 0000 725d 0000 0072 1000 0000 7235 0000  ..r]...r....r5..
+000010e0: 0072 2400 0000 7224 0000 0072 2400 0000  .r$...r$...r$...
+000010f0: 7225 0000 0072 6500 0000 8f00 0000 f306  r%...re.........
+00001100: 0000 0008 0004 010c 0272 6500 0000 6300  .........re...c.
+00001110: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00001120: 0000 0040 0000 0073 2200 0000 6500 5a01  ...@...s"...e.Z.
+00001130: 6400 5a02 6401 5a03 6407 6403 6404 8401  d.Z.d.Z.d.d.d...
+00001140: 5a04 6405 6406 8400 5a05 6402 5300 2908  Z.d.d...Z.d.S.).
+00001150: da0e 566f 6c56 6563 746f 7246 6965 6c64  ..VolVectorField
+00001160: 5a0e 766f 6c56 6563 746f 7246 6965 6c64  Z.volVectorField
+00001170: 4e63 0400 0000 0000 0000 0000 0000 0700  Nc..............
+00001180: 0000 0600 0000 4300 0000 73c2 0000 007c  ......C...s....|
+00001190: 0264 0075 0172 347c 0364 0075 0072 0a74  .d.u.r4|.d.u.r.t
+000011a0: 0082 0174 017c 0174 026a 0383 0273 1274  ...t.|.t.j...s.t
+000011b0: 0082 017c 016a 0464 016b 0373 277c 016a  ...|.j.d.k.s'|.j
+000011c0: 057c 026a 0504 0003 006b 0372 257c 036a  .|.j.....k.r%|.j
+000011d0: 056b 0372 2974 0082 0101 006e 0274 0082  .k.r)t.....n.t..
+000011e0: 017c 017d 0474 02a0 067c 047c 027c 0367  .|.}.t...|.|.|.g
+000011f0: 03a1 016a 077d 0174 087c 0183 017d 057c  ...j.}.t.|...}.|
+00001200: 0564 026b 0272 5674 017c 0164 0319 0074  .d.k.rVt.|.d...t
+00001210: 0983 0272 5674 0a64 0464 05a0 0b64 0664  ...rVt.d.d...d.d
+00001220: 0784 007c 0144 0083 01a1 0117 0064 0817  ...|.D.......d..
+00001230: 0064 0964 0a8d 027d 066e 027c 017d 067c  .d.d...}.n.|.}.|
+00001240: 006a 0ca0 0d64 0b7c 06a1 0201 0064 0053  .j...d.|.....d.S
+00001250: 0029 0c4e 7217 0000 00e9 0300 0000 7201  .).Nr.........r.
+00001260: 0000 0072 1400 0000 da01 2063 0100 0000  ...r...... c....
+00001270: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001280: 7300 0000 7318 0000 0081 007c 005d 077d  s...s......|.].}
+00001290: 0174 007c 0183 0156 0001 0071 0264 0053  .t.|...V...q.d.S
+000012a0: 0072 3b00 0000 2901 725e 0000 0029 0272  .r;...).r^...).r
+000012b0: 4800 0000 724a 0000 0072 2400 0000 7224  H...rJ...r$...r$
+000012c0: 0000 0072 2500 0000 da09 3c67 656e 6578  ...r%.....<genex
+000012d0: 7072 3eae 0000 0073 0400 0000 0280 1600  pr>....s........
+000012e0: 7a2c 566f 6c56 6563 746f 7246 6965 6c64  z,VolVectorField
+000012f0: 2e73 6574 5f76 616c 7565 732e 3c6c 6f63  .set_values.<loc
+00001300: 616c 733e 2e3c 6765 6e65 7870 723e 7215  als>.<genexpr>r.
+00001310: 0000 0072 6600 0000 7253 0000 0072 3100  ...rf...rS...r1.
+00001320: 0000 290e 723f 0000 0072 3300 0000 7220  ..).r?...r3...r 
+00001330: 0000 00da 076e 6461 7272 6179 da04 6e64  .....ndarray..nd
+00001340: 696d da04 7369 7a65 da05 7374 6163 6bda  im..size..stack.
+00001350: 0154 7268 0000 0072 0500 0000 720e 0000  .Trh...r....r...
+00001360: 00da 046a 6f69 6e72 1200 0000 7234 0000  ...joinr....r4..
+00001370: 0029 0772 3600 0000 7219 0000 005a 0276  .).r6...r....Z.v
+00001380: 795a 0276 7a5a 0276 785a 066e 5f65 6c65  yZ.vzZ.vxZ.n_ele
+00001390: 6d72 4a00 0000 7224 0000 0072 2400 0000  mrJ...r$...r$...
+000013a0: 7225 0000 0072 3500 0000 a000 0000 7326  r%...r5.......s&
+000013b0: 0000 0008 0108 0104 010c 0104 0122 0104  ............."..
+000013c0: 0104 ff04 0104 0112 0108 0216 0102 011a  ................
+000013d0: 0102 0108 fe04 0512 017a 1956 6f6c 5665  .........z.VolVe
+000013e0: 6374 6f72 4669 656c 642e 7365 745f 7661  ctorField.set_va
+000013f0: 6c75 6573 6301 0000 0000 0000 0000 0000  luesc...........
+00001400: 0002 0000 0005 0000 0043 0000 0073 3600  .........C...s6.
+00001410: 0000 7c00 a000 a100 7d01 7c01 6400 6400  ..|.....}.|.d.d.
+00001420: 8502 6401 6602 1900 7c01 6400 6400 8502  ..d.f...|.d.d...
+00001430: 6402 6602 1900 7c01 6400 6400 8502 6403  d.f...|.d.d...d.
+00001440: 6602 1900 6603 5300 2904 4e72 0100 0000  f...f.S.).Nr....
+00001450: 7217 0000 00e9 0200 0000 2901 7259 0000  r.........).rY..
+00001460: 0029 0272 3600 0000 da03 6172 7272 2400  .).r6.....arrr$.
+00001470: 0000 7224 0000 0072 2500 0000 da0e 6765  ..r$...r%.....ge
+00001480: 745f 636f 6d70 6f6e 656e 7473 b500 0000  t_components....
+00001490: 7304 0000 0008 012e 017a 1d56 6f6c 5665  s........z.VolVe
+000014a0: 6374 6f72 4669 656c 642e 6765 745f 636f  ctorField.get_co
+000014b0: 6d70 6f6e 656e 7473 725a 0000 0029 0672  mponentsrZ...).r
+000014c0: 5b00 0000 725c 0000 0072 5d00 0000 7210  [...r\...r]...r.
+000014d0: 0000 0072 3500 0000 7277 0000 0072 2400  ...r5...rw...r$.
+000014e0: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+000014f0: 0072 6b00 0000 9d00 0000 7308 0000 0008  .rk.......s.....
+00001500: 0004 010a 020c 1572 6b00 0000 6300 0000  .......rk...c...
+00001510: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00001520: 0040 0000 0072 6400 0000 2905 da0e 566f  .@...rd...)...Vo
+00001530: 6c54 656e 736f 7246 6965 6c64 5a0e 766f  lTensorFieldZ.vo
+00001540: 6c54 656e 736f 7246 6965 6c64 6302 0000  lTensorFieldc...
+00001550: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00001560: 0043 0000 0073 3000 0000 7400 7c01 7401  .C...s0...t.|.t.
+00001570: 6a02 8302 720b 7c01 6a03 6401 6b03 720f  j...r.|.j.d.k.r.
+00001580: 7404 6402 8301 8201 7c00 6a05 a006 6403  t.d.....|.j...d.
+00001590: 7c01 a102 0100 6400 5300 2904 4e72 7500  |.....d.S.).Nru.
+000015a0: 0000 7a36 6e6f 7420 6973 696e 7374 616e  ..z6not isinstan
+000015b0: 6365 2876 616c 7565 732c 206e 702e 6e64  ce(values, np.nd
+000015c0: 6172 7261 7929 206f 7220 7661 6c75 6573  array) or values
+000015d0: 2e6e 6469 6d20 213d 2032 7231 0000 0029  .ndim != 2r1...)
+000015e0: 0772 3300 0000 7220 0000 0072 6f00 0000  .r3...r ...ro...
+000015f0: 7270 0000 00da 134e 6f74 496d 706c 656d  rp.....NotImplem
+00001600: 656e 7465 6445 7272 6f72 7212 0000 0072  entedErrorr....r
+00001610: 3400 0000 7244 0000 0072 2400 0000 7224  4...rD...r$...r$
+00001620: 0000 0072 2500 0000 7235 0000 00bd 0000  ...r%...r5......
+00001630: 0073 0a00 0000 1601 0201 0201 04ff 1204  .s..............
+00001640: 7a19 566f 6c54 656e 736f 7246 6965 6c64  z.VolTensorField
+00001650: 2e73 6574 5f76 616c 7565 734e 7269 0000  .set_valuesNri..
+00001660: 0072 2400 0000 7224 0000 0072 2400 0000  .r$...r$...r$...
+00001670: 7225 0000 0072 7800 0000 ba00 0000 726a  r%...rx.......rj
+00001680: 0000 0072 7800 0000 6301 0000 0000 0000  ...rx...c.......
+00001690: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+000016a0: 0073 1400 0000 6900 7c00 5d06 7d01 7c01  .s....i.|.].}.|.
+000016b0: 6a00 7c01 9302 7102 5300 7224 0000 0029  j.|...q.S.r$...)
+000016c0: 0172 1000 0000 2902 7248 0000 0072 1000  .r....).rH...r..
+000016d0: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+000016e0: 0072 4b00 0000 c600 0000 7306 0000 0006  .rK.......s.....
+000016f0: 0008 0106 ff72 4b00 0000 6301 0000 0000  .....rK...c.....
+00001700: 0000 0000 0000 0004 0000 0008 0000 0043  ...............C
+00001710: 0000 0073 8000 0000 6400 7d01 7400 7c00  ...s....d.}.t.|.
+00001720: 6401 8302 8f22 7d02 7c02 4400 5d17 7d03  d...."}.|.D.].}.
+00001730: 7c03 a001 a100 7d03 7c03 a002 6402 a101  |.....}.|...d...
+00001740: 7221 7c03 a003 a100 6403 1900 6400 6403  r!|.....d...d.d.
+00001750: 8502 1900 7d01 0100 6e01 710a 5700 6400  ....}...n.q.W.d.
+00001760: 0400 0400 8303 0100 6e08 3100 732c 7701  ........n.1.s,w.
+00001770: 0100 0100 0100 5900 0100 7c01 6400 7500  ......Y...|.d.u.
+00001780: 7237 7404 8201 7405 7c01 1900 7d01 7c01  r7t...t.|...}.|.
+00001790: a006 7c00 a101 5300 2904 4eda 0172 7a06  ..|...S.).N..rz.
+000017a0: 636c 6173 7320 e9ff ffff ff29 0772 4000  class .....).r@.
+000017b0: 0000 721c 0000 0072 1d00 0000 da05 7370  ..r....r......sp
+000017c0: 6c69 74da 0c52 756e 7469 6d65 4572 726f  lit..RuntimeErro
+000017d0: 72da 0763 6c61 7373 6573 722a 0000 0029  r..classesr*...)
+000017e0: 0472 2700 0000 7210 0000 0072 4200 0000  .r'...r....rB...
+000017f0: da04 6c69 6e65 7224 0000 0072 2400 0000  ..liner$...r$...
+00001800: 7225 0000 00da 0f72 6561 645f 6669 656c  r%.....read_fiel
+00001810: 645f 6669 6c65 cb00 0000 731c 0000 0004  d_file....s.....
+00001820: 010c 0108 0108 010a 0114 0104 0102 fe02  ................
+00001830: 801c fd08 0704 0108 020a 0272 8000 0000  ...........r....
+00001840: 2920 da07 5f5f 646f 635f 5f72 1e00 0000  ) ..__doc__r....
+00001850: da03 6162 6372 0200 0000 7203 0000 00da  ..abcr....r.....
+00001860: 0269 6f72 0400 0000 da07 6e75 6d62 6572  .ior......number
+00001870: 7372 0500 0000 da07 7061 7468 6c69 6272  sr......pathlibr
+00001880: 0600 0000 da05 6e75 6d70 7972 2000 0000  ......numpyr ...
+00001890: 5a1d 666c 7569 6473 696d 666f 616d 2e66  Z.fluidsimfoam.f
+000018a0: 6f61 6d5f 696e 7075 745f 6669 6c65 7372  oam_input_filesr
+000018b0: 0700 0000 5a21 666c 7569 6473 696d 666f  ....Z!fluidsimfo
+000018c0: 616d 2e66 6f61 6d5f 696e 7075 745f 6669  am.foam_input_fi
+000018d0: 6c65 732e 6173 7472 0800 0000 7209 0000  les.astr....r...
+000018e0: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+000018f0: 720d 0000 0072 0e00 0000 7261 0000 0072  r....r....ra...r
+00001900: 6200 0000 7263 0000 0072 0f00 0000 7265  b...rc...r....re
+00001910: 0000 0072 6b00 0000 7278 0000 0072 7e00  ...rk...rx...r~.
+00001920: 0000 7280 0000 0072 2400 0000 7224 0000  ..r....r$...r$..
+00001930: 0072 2400 0000 7225 0000 00da 083c 6d6f  .r$...r%.....<mo
+00001940: 6475 6c65 3e01 0000 0073 2a00 0000 0400  dule>....s*.....
+00001950: 0804 1001 0c01 0c01 0c01 0802 0c02 2401  ..............$.
+00001960: 040a 0202 02ff 0403 1003 1070 100e 101d  ...........p....
+00001970: 060c 0801 06ff 0c05                      ........
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 12:42:19 2023 UTC, .py size: 5070 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ab3f 5a64 ce13 0000  o........?Zd....
+00000000: 6f0d 0d0a 0000 0000 5dcf 6364 d413 0000  o.......].cd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 5a08 6401 6406 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
@@ -35,163 +35,163 @@
 00000220: 027c 016a 0383 0183 017d 0274 047c 026a  .|.j.....}.t.|.j
 00000230: 0583 01a0 06a1 006a 0764 011b 007c 005f  .......j.d...|._
 00000240: 0874 09a0 0a74 09a0 0b7c 026a 0c64 01a1  .t...t...|.j.d..
 00000250: 0274 09a0 0b64 0264 03a1 0267 02a1 017d  .t...d.d...g...}
 00000260: 0374 096a 0d7c 0374 096a 0e64 0464 058d  .t.j.|.t.j.d.d..
 00000270: 037c 005f 0f64 0053 0029 064e da09 7465  .|._.d.S.).N..te
 00000280: 6d70 6c61 7465 73da 0c66 6c75 6964 7369  mplates..fluidsi
-00000290: 6d66 6f61 6dda 0972 6573 6f75 7263 6573  mfoam..resources
+00000290: 6d66 6f61 6d5a 0972 6573 6f75 7263 6573  mfoamZ.resources
 000002a0: 5429 03da 066c 6f61 6465 72da 0975 6e64  T)...loader..und
-000002b0: 6566 696e 6564 da15 6b65 6570 5f74 7261  efined..keep_tra
+000002b0: 6566 696e 6564 5a15 6b65 6570 5f74 7261  efinedZ.keep_tra
 000002c0: 696c 696e 675f 6e65 776c 696e 6529 10da  iling_newline)..
 000002d0: 066f 7574 7075 7472 0400 0000 da04 7479  .outputr......ty
 000002e0: 7065 da03 7369 6d72 0500 0000 da08 5f5f  pe..simr......__
 000002f0: 6669 6c65 5f5f da08 6162 736f 6c75 7465  file__..absolute
 00000300: da06 7061 7265 6e74 da0d 7465 6d70 6c61  ..parent..templa
-00000310: 7465 735f 6469 72da 066a 696e 6a61 32da  tes_dir..jinja2.
-00000320: 0c43 686f 6963 654c 6f61 6465 72da 0d50  .ChoiceLoader..P
+00000310: 7465 735f 6469 72da 066a 696e 6a61 325a  tes_dir..jinja2Z
+00000320: 0c43 686f 6963 654c 6f61 6465 725a 0d50  .ChoiceLoaderZ.P
 00000330: 6163 6b61 6765 4c6f 6164 6572 da0b 5f5f  ackageLoader..__
-00000340: 7061 636b 6167 655f 5fda 0b45 6e76 6972  package__..Envir
-00000350: 6f6e 6d65 6e74 da0f 5374 7269 6374 556e  onment..StrictUn
+00000340: 7061 636b 6167 655f 5f5a 0b45 6e76 6972  package__Z.Envir
+00000350: 6f6e 6d65 6e74 5a0f 5374 7269 6374 556e  onmentZ.StrictUn
 00000360: 6465 6669 6e65 64da 096a 696e 6a61 5f65  defined..jinja_e
-00000370: 6e76 2904 da04 7365 6c66 7213 0000 00da  nv)...selfr.....
-00000380: 036d 6f64 7210 0000 00a9 0072 2300 0000  .modr......r#...
+00000370: 6e76 2904 da04 7365 6c66 7211 0000 00da  nv)...selfr.....
+00000380: 036d 6f64 720f 0000 00a9 0072 1d00 0000  .modr......r....
 00000390: fa4d 2f68 6f6d 652f 7069 6572 7265 2f44  .M/home/pierre/D
 000003a0: 6576 2f66 6c75 6964 7369 6d66 6f61 6d2f  ev/fluidsimfoam/
 000003b0: 7372 632f 666c 7569 6473 696d 666f 616d  src/fluidsimfoam
 000003c0: 2f66 6f61 6d5f 696e 7075 745f 6669 6c65  /foam_input_file
 000003d0: 732f 6765 6e65 7261 746f 7273 2e70 79da  s/generators.py.
 000003e0: 085f 5f69 6e69 745f 5f11 0000 0073 1a00  .__init__....s..
 000003f0: 0000 0601 0e01 1601 0402 0c02 0a01 02fe  ................
 00000400: 04ff 0407 0201 0401 0201 0cfd 7a13 496e  ............z.In
 00000410: 7075 7446 696c 6573 2e5f 5f69 6e69 745f  putFiles.__init_
 00000420: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
 00000430: 0000 0300 0000 4300 0000 730c 0000 007c  ......C...s....|
 00000440: 006a 00a0 017c 01a1 0153 00a9 014e 2902  .j...|...S...N).
-00000450: 7220 0000 00da 0c67 6574 5f74 656d 706c  r .....get_templ
-00000460: 6174 6529 0272 2100 0000 da0d 7465 6d70  ate).r!.....temp
-00000470: 6c61 7465 5f6e 616d 6572 2300 0000 7223  late_namer#...r#
-00000480: 0000 0072 2400 0000 7227 0000 0023 0000  ...r$...r'...#..
+00000450: 721a 0000 00da 0c67 6574 5f74 656d 706c  r......get_templ
+00000460: 6174 6529 0272 1b00 0000 da0d 7465 6d70  ate).r......temp
+00000470: 6c61 7465 5f6e 616d 6572 1d00 0000 721d  late_namer....r.
+00000480: 0000 0072 1e00 0000 7221 0000 0023 0000  ...r....r!...#..
 00000490: 00f3 0200 0000 0c01 7a17 496e 7075 7446  ........z.InputF
 000004a0: 696c 6573 2e67 6574 5f74 656d 706c 6174  iles.get_templat
 000004b0: 654e 2906 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
 000004c0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 000004d0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-000004e0: 5f72 2500 0000 7227 0000 0072 2300 0000  _r%...r'...r#...
-000004f0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
+000004e0: 5f72 1f00 0000 7221 0000 0072 1d00 0000  _r....r!...r....
+000004f0: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
 00000500: 0c00 0000 0e00 0000 7308 0000 0008 0004  ........s.......
 00000510: 0108 020c 1272 0c00 0000 6300 0000 0000  .....r....c.....
 00000520: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
 00000530: 0000 0073 4400 0000 6500 5a01 6400 5a02  ...sD...e.Z.d.Z.
 00000540: 5500 6503 6504 6401 3c00 6402 6403 8400  U.e.e.d.<.d.d...
 00000550: 5a05 640d 6405 6406 8401 5a06 6507 6407  Z.d.d.d...Z.e.d.
 00000560: 6408 8400 8301 5a08 6409 640a 8400 5a09  d.....Z.d.d...Z.
 00000570: 640b 640c 8400 5a0a 6404 5300 290e da10  d.d...Z.d.S.)...
 00000580: 4669 6c65 4765 6e65 7261 746f 7241 4243  FileGeneratorABC
 00000590: da08 7265 6c5f 7061 7468 6302 0000 0000  ..rel_pathc.....
 000005a0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
 000005b0: 0000 0073 1200 0000 7c01 7c00 5f00 7c01  ...s....|.|._.|.
-000005c0: 6a01 7c00 5f01 6400 5300 7226 0000 0029  j.|._.d.S.r&...)
-000005d0: 0272 1300 0000 da0b 696e 7075 745f 6669  .r......input_fi
-000005e0: 6c65 73a9 0272 2100 0000 7213 0000 0072  les..r!...r....r
-000005f0: 2300 0000 7223 0000 0072 2400 0000 7225  #...r#...r$...r%
+000005c0: 6a01 7c00 5f01 6400 5300 7220 0000 0029  j.|._.d.S.r ...)
+000005d0: 0272 1100 0000 da0b 696e 7075 745f 6669  .r......input_fi
+000005e0: 6c65 73a9 0272 1b00 0000 7211 0000 0072  les..r....r....r
+000005f0: 1d00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
 00000600: 0000 002a 0000 0073 0400 0000 0601 0c01  ...*...s........
 00000610: 7a19 4669 6c65 4765 6e65 7261 746f 7241  z.FileGeneratorA
 00000620: 4243 2e5f 5f69 6e69 745f 5f4e 6302 0000  BC.__init__Nc...
 00000630: 0000 0000 0000 0000 0003 0000 0008 0000  ................
 00000640: 0043 0000 0073 5c00 0000 7c01 6401 7500  .C...s\...|.d.u.
 00000650: 7209 7c00 6a00 6a01 6a02 7d01 7403 7c00  r.|.j.j.j.}.t.|.
 00000660: 6a00 6a04 7c00 6a05 1b00 6402 8302 8f11  j.j.|.j...d.....
 00000670: 7d02 7c02 a006 7c00 a007 7c01 a101 a101  }.|...|...|.....
 00000680: 0100 5700 6401 0400 0400 8303 0100 6401  ..W.d.........d.
 00000690: 5300 3100 7327 7701 0100 0100 0100 5900  S.1.s'w.......Y.
 000006a0: 0100 6401 5300 2903 7a11 4765 6e65 7261  ..d.S.).z.Genera
 000006b0: 7465 2074 6865 2066 696c 654e da01 7729  te the fileN..w)
-000006c0: 0872 1300 0000 7215 0000 00da 0670 6172  .r....r......par
+000006c0: 0872 1100 0000 7213 0000 00da 0670 6172  .r....r......par
 000006d0: 616d 73da 046f 7065 6eda 0870 6174 685f  ams..open..path_
-000006e0: 7275 6e72 2f00 0000 da05 7772 6974 65da  runr/.....write.
+000006e0: 7275 6e72 2900 0000 da05 7772 6974 65da  runr).....write.
 000006f0: 0d67 656e 6572 6174 655f 636f 6465 2903  .generate_code).
-00000700: 7221 0000 0072 3300 0000 da04 6669 6c65  r!...r3.....file
-00000710: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
+00000700: 721b 0000 0072 2d00 0000 da04 6669 6c65  r....r-.....file
+00000710: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
 00000720: 0d67 656e 6572 6174 655f 6669 6c65 2e00  .generate_file..
 00000730: 0000 730a 0000 0008 020a 0116 0112 0122  ..s............"
 00000740: ff7a 1e46 696c 6547 656e 6572 6174 6f72  .z.FileGenerator
 00000750: 4142 432e 6765 6e65 7261 7465 5f66 696c  ABC.generate_fil
 00000760: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
 00000770: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
 00000780: 0153 0029 027a 1d47 656e 6572 6174 6520  .S.).z.Generate 
 00000790: 7468 6520 636f 6465 206f 6620 7468 6520  the code of the 
-000007a0: 6669 6c65 4e72 2300 0000 a901 7221 0000  fileNr#.....r!..
-000007b0: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-000007c0: 7237 0000 0035 0000 0073 0200 0000 0400  r7...5...s......
+000007a0: 6669 6c65 4e72 1d00 0000 a901 721b 0000  fileNr......r...
+000007b0: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+000007c0: 7231 0000 0035 0000 0073 0200 0000 0400  r1...5...s......
 000007d0: 7a1e 4669 6c65 4765 6e65 7261 746f 7241  z.FileGeneratorA
 000007e0: 4243 2e67 656e 6572 6174 655f 636f 6465  BC.generate_code
 000007f0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
 00000800: 0004 0000 0003 0000 0073 4200 0000 8800  .........sB.....
 00000810: 6a00 6a01 8800 6a02 1b00 7d01 7403 8700  j.j...j...}.t...
 00000820: 6601 6401 6402 8408 6403 4400 8301 8301  f.d.d...d.D.....
 00000830: 721d 7404 7c01 a005 a100 8301 7d02 7c01  r.t.|.......}.|.
 00000840: 7c02 5f06 7c02 5300 7407 7c01 8301 5300  |._.|.S.t.|...S.
 00000850: 2904 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
 00000860: 0200 0000 0400 0000 3300 0000 731c 0000  ........3...s...
 00000870: 0081 007c 005d 097d 0188 006a 00a0 017c  ...|.].}...j...|
-00000880: 01a1 0156 0001 0071 0264 0053 0072 2600  ...V...q.d.S.r&.
-00000890: 0000 2902 722f 0000 00da 0a73 7461 7274  ..).r/.....start
+00000880: 01a1 0156 0001 0071 0264 0053 0072 2000  ...V...q.d.S.r .
+00000890: 0000 2902 7229 0000 00da 0a73 7461 7274  ..).r).....start
 000008a0: 7377 6974 6829 02da 022e 30da 0573 7461  swith)....0..sta
-000008b0: 7274 723a 0000 0072 2300 0000 7224 0000  rtr:...r#...r$..
+000008b0: 7274 7234 0000 0072 1d00 0000 721e 0000  rtr4...r....r...
 000008c0: 00da 093c 6765 6e65 7870 723e 3b00 0000  ...<genexpr>;...
 000008d0: 7308 0000 0002 8004 000c 010a ff7a 2846  s............z(F
 000008e0: 696c 6547 656e 6572 6174 6f72 4142 432e  ileGeneratorABC.
 000008f0: 7265 6164 2e3c 6c6f 6361 6c73 3e2e 3c67  read.<locals>.<g
 00000900: 656e 6578 7072 3e29 02da 0673 7973 7465  enexpr>)...syste
-00000910: 6dda 0863 6f6e 7374 616e 7429 0872 1300  m..constant).r..
-00000920: 0000 7235 0000 0072 2f00 0000 da03 616e  ..r5...r/.....an
+00000910: 6dda 0863 6f6e 7374 616e 7429 0872 1100  m..constant).r..
+00000920: 0000 722f 0000 0072 2900 0000 da03 616e  ..r/...r).....an
 00000930: 7972 0a00 0000 da09 7265 6164 5f74 6578  yr......read_tex
-00000940: 74da 0470 6174 6872 0b00 0000 2903 7221  t..pathr....).r!
-00000950: 0000 0072 4300 0000 da04 7472 6565 7223  ...rC.....treer#
-00000960: 0000 0072 3a00 0000 7224 0000 00da 0472  ...r:...r$.....r
+00000940: 74da 0470 6174 6872 0b00 0000 2903 721b  t..pathr....).r.
+00000950: 0000 0072 3d00 0000 da04 7472 6565 721d  ...r=.....treer.
+00000960: 0000 0072 3400 0000 721e 0000 00da 0472  ...r4...r......r
 00000970: 6561 6439 0000 0073 1000 0000 0e01 0c01  ead9...s........
 00000980: 0201 08ff 0c03 0601 0401 0802 7a15 4669  ............z.Fi
 00000990: 6c65 4765 6e65 7261 746f 7241 4243 2e72  leGeneratorABC.r
 000009a0: 6561 6463 0200 0000 0000 0000 0000 0000  eadc............
 000009b0: 0300 0000 0800 0000 4300 0000 7348 0000  ........C...sH..
 000009c0: 0074 007c 006a 016a 027c 006a 031b 0064  .t.|.j.j.|.j...d
 000009d0: 0183 028f 107d 027c 02a0 047c 01a0 05a1  .....}.|...|....
 000009e0: 00a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
 000009f0: 0064 0053 0031 0073 1d77 0101 0001 0001  .d.S.1.s.w......
-00000a00: 0059 0001 0064 0053 0029 024e 7232 0000  .Y...d.S.).Nr2..
-00000a10: 0029 0672 3400 0000 7213 0000 0072 3500  .).r4...r....r5.
-00000a20: 0000 722f 0000 0072 3600 0000 da04 6475  ..r/...r6.....du
-00000a30: 6d70 2903 7221 0000 005a 0864 756d 7061  mp).r!...Z.dumpa
-00000a40: 626c 6572 3800 0000 7223 0000 0072 2300  bler8...r#...r#.
-00000a50: 0000 7224 0000 00da 096f 7665 7277 7269  ..r$.....overwri
+00000a00: 0059 0001 0064 0053 0029 024e 722c 0000  .Y...d.S.).Nr,..
+00000a10: 0029 0672 2e00 0000 7211 0000 0072 2f00  .).r....r....r/.
+00000a20: 0000 7229 0000 0072 3000 0000 da04 6475  ..r)...r0.....du
+00000a30: 6d70 2903 721b 0000 005a 0864 756d 7061  mp).r....Z.dumpa
+00000a40: 626c 6572 3200 0000 721d 0000 0072 1d00  bler2...r....r..
+00000a50: 0000 721e 0000 00da 096f 7665 7277 7269  ..r......overwri
 00000a60: 7465 4400 0000 7306 0000 0016 0110 0122  teD...s........"
 00000a70: ff7a 1a46 696c 6547 656e 6572 6174 6f72  .z.FileGenerator
-00000a80: 4142 432e 6f76 6572 7772 6974 6572 2600  ABC.overwriter&.
-00000a90: 0000 290b 722a 0000 0072 2b00 0000 722c  ..).r*...r+...r,
+00000a80: 4142 432e 6f76 6572 7772 6974 6572 2000  ABC.overwriter .
+00000a90: 0000 290b 7224 0000 0072 2500 0000 7226  ..).r$...r%...r&
 00000aa0: 0000 00da 0373 7472 da0f 5f5f 616e 6e6f  .....str..__anno
-00000ab0: 7461 7469 6f6e 735f 5f72 2500 0000 7239  tations__r%...r9
-00000ac0: 0000 0072 0300 0000 7237 0000 0072 4500  ...r....r7...rE.
-00000ad0: 0000 7247 0000 0072 2300 0000 7223 0000  ..rG...r#...r#..
-00000ae0: 0072 2300 0000 7224 0000 0072 2e00 0000  .r#...r$...r....
+00000ab0: 7461 7469 6f6e 735f 5f72 1f00 0000 7233  tations__r....r3
+00000ac0: 0000 0072 0300 0000 7231 0000 0072 3f00  ...r....r1...r?.
+00000ad0: 0000 7241 0000 0072 1d00 0000 721d 0000  ..rA...r....r...
+00000ae0: 0072 1d00 0000 721e 0000 0072 2800 0000  .r....r....r(...
 00000af0: 2700 0000 7310 0000 000a 0008 0108 020a  '...s...........
-00000b00: 0402 070a 0108 030c 0b72 2e00 0000 6300  .........r....c.
+00000b00: 0402 070a 0108 030c 0b72 2800 0000 6300  .........r(...c.
 00000b10: 0000 0000 0000 0000 0000 0000 0000 0003  ................
 00000b20: 0000 0000 0000 0073 3c00 0000 6500 5a01  .......s<...e.Z.
 00000b30: 6400 5a02 5500 6503 6504 6401 3c00 8700  d.Z.U.e.e.d.<...
 00000b40: 6601 6402 6403 8408 5a05 6409 6405 6406  f.d.d...Z.d.d.d.
 00000b50: 8401 5a06 6507 6407 6408 8400 8301 5a08  ..Z.e.d.d.....Z.
 00000b60: 8700 0400 5a09 5300 290a da0d 4669 6c65  ....Z.S.)...File
-00000b70: 4765 6e65 7261 746f 7272 2800 0000 6302  Generatorr(...c.
+00000b70: 4765 6e65 7261 746f 7272 2200 0000 6302  Generatorr"...c.
 00000b80: 0000 0000 0000 0000 0000 0002 0000 0003  ................
 00000b90: 0000 0003 0000 0073 1000 0000 7400 8300  .......s....t...
-00000ba0: a001 7c01 a101 0100 6400 5300 7226 0000  ..|.....d.S.r&..
-00000bb0: 0029 02da 0573 7570 6572 7225 0000 0072  .)...superr%...r
-00000bc0: 3100 0000 a901 da09 5f5f 636c 6173 735f  1.......__class_
-00000bd0: 5f72 2300 0000 7224 0000 0072 2500 0000  _r#...r$...r%...
+00000ba0: a001 7c01 a101 0100 6400 5300 7220 0000  ..|.....d.S.r ..
+00000bb0: 0029 02da 0573 7570 6572 721f 0000 0072  .)...superr....r
+00000bc0: 2b00 0000 a901 da09 5f5f 636c 6173 735f  +.......__class_
+00000bd0: 5f72 1d00 0000 721e 0000 0072 1f00 0000  _r....r....r....
 00000be0: 4c00 0000 7302 0000 0010 017a 1646 696c  L...s......z.Fil
 00000bf0: 6547 656e 6572 6174 6f72 2e5f 5f69 6e69  eGenerator.__ini
 00000c00: 745f 5f4e 6302 0000 0000 0000 0000 0000  t__Nc...........
 00000c10: 0005 0000 0008 0000 0003 0000 0073 2c01  .............s,.
 00000c20: 0000 7c01 6401 7500 7209 7c00 6a00 6a01  ..|.d.u.r.|.j.j.
 00000c30: 6a02 7d01 7a0b 7403 7c00 6a00 6402 7c00  j.}.z.t.|.j.d.|.
 00000c40: 6a04 1700 8302 7d02 5700 6e0b 0400 7405  j.....}.W.n...t.
@@ -207,129 +207,130 @@
 00000ce0: 7266 8700 6601 6405 6406 8408 7d02 7c02  rf..f.d.d...}.|.
 00000cf0: 6401 7500 7277 7c00 6a09 a00a 7c00 6a0b  d.u.rw|.j...|.j.
 00000d00: a101 7d04 7c04 6a0c 7c01 6407 8d01 5300  ..}.|.j.|.d...S.
 00000d10: 7c00 6a09 6a0d 7c00 6a0b 1b00 a00e a100  |.j.j.|.j.......
 00000d20: 7292 740f 6408 7c00 6a10 9b00 6409 7c00  r.t.d.|.j...d.|.
 00000d30: 6a09 6a0d 9b00 640a 7c00 6a04 9b00 640b  j.j...d.|.j...d.
 00000d40: 9d07 8301 8201 7c02 7c01 8301 5300 290c  ......|.|...S.).
-00000d50: 7a95 4765 6e65 7261 7465 2074 6865 2063  z.Generate the c
+00000d50: 7a96 4765 6e65 7261 7465 2074 6865 2063  z.Generate the c
 00000d60: 6f64 6520 6f66 2074 6865 2066 696c 6520  ode of the file 
 00000d70: 6672 6f6d 202e 2e2e 0a0a 2020 2020 2020  from .....      
 00000d80: 2020 2d20 6120 6d65 7468 6f64 206e 616d    - a method nam
 00000d90: 6564 206c 696b 6520 6073 696d 2e6f 7574  ed like `sim.out
-00000da0: 7075 742e 6d61 6b65 5f63 6f64 655f 626c  put.make_code_bl
-00000db0: 6f63 6b5f 6d65 7368 5f64 6963 7460 2c0a  ock_mesh_dict`,.
-00000dc0: 2020 2020 2020 2020 2d20 6f72 2061 204a          - or a J
-00000dd0: 696e 6a61 2074 656d 706c 6174 652e 0a20  inja template.. 
-00000de0: 2020 2020 2020 204e 5a0a 6d61 6b65 5f63         NZ.make_c
-00000df0: 6f64 655f 5a0a 6d61 6b65 5f74 7265 655f  ode_Z.make_tree_
-00000e00: da07 6865 6c70 6572 5f63 0100 0000 0000  ..helper_c......
-00000e10: 0000 0000 0000 0100 0000 0200 0000 1300  ................
-00000e20: 0000 730c 0000 0088 007c 0083 01a0 00a1  ..s......|......
-00000e30: 0053 0072 2600 0000 2901 7246 0000 0029  .S.r&...).rF...)
-00000e40: 015a 0770 6172 616d 735f a901 da09 6d61  .Z.params_....ma
-00000e50: 6b65 5f74 7265 6572 2300 0000 7224 0000  ke_treer#...r$..
-00000e60: 00da 096d 616b 655f 636f 6465 6e00 0000  ...make_coden...
-00000e70: 7229 0000 007a 2e46 696c 6547 656e 6572  r)...z.FileGener
-00000e80: 6174 6f72 2e67 656e 6572 6174 655f 636f  ator.generate_co
-00000e90: 6465 2e3c 6c6f 6361 6c73 3e2e 6d61 6b65  de.<locals>.make
-00000ea0: 5f63 6f64 6529 0172 3300 0000 7a3b 466c  _code).r3...z;Fl
-00000eb0: 7569 6473 696d 666f 616d 2073 6f6c 7665  uidsimfoam solve
-00000ec0: 7220 6973 7375 653a 2032 2063 6f6e 6375  r issue: 2 concu
-00000ed0: 7272 656e 7420 6d65 7468 6f64 7320 746f  rrent methods to
-00000ee0: 2070 726f 6475 6365 207a 103a 0a2d 2074   produce z.:.- t
-00000ef0: 656d 706c 6174 6520 696e 207a 1e2c 0a2d  emplate in z.,.-
-00000f00: 2066 756e 6374 696f 6e20 6f75 7470 7574   function output
-00000f10: 2e6d 616b 655f 636f 6465 5f7a 3d2e 0a52  .make_code_z=..R
-00000f20: 656d 6f76 6520 7468 6520 6669 6c65 206f  emove the file o
-00000f30: 7220 7468 6520 6675 6e63 7469 6f6e 2028  r the function (
-00000f40: 6f72 206d 616b 6520 6974 2065 7175 616c  or make it equal
-00000f50: 2074 6f20 4e6f 6e65 292e 2911 7213 0000   to None).).r...
-00000f60: 0072 1500 0000 7233 0000 00da 0767 6574  .r....r3.....get
-00000f70: 6174 7472 da05 5f6e 616d 65da 0e41 7474  attr.._name..Att
-00000f80: 7269 6275 7465 4572 726f 72da 0a69 7369  ributeError..isi
-00000f90: 6e73 7461 6e63 6572 0900 0000 7250 0000  nstancer....rP..
-00000fa0: 0072 3000 0000 7227 0000 0072 2800 0000  .r0...r'...r(...
-00000fb0: da06 7265 6e64 6572 7219 0000 00da 0665  ..renderr......e
-00000fc0: 7869 7374 73da 0c52 756e 7469 6d65 4572  xists..RuntimeEr
-00000fd0: 726f 7272 2f00 0000 2905 7221 0000 0072  rorr/...).r!...r
-00000fe0: 3300 0000 7251 0000 00da 0668 656c 7065  3...rQ.....helpe
-00000ff0: 72da 0874 656d 706c 6174 6572 2300 0000  r..templater#...
-00001000: 724f 0000 0072 2400 0000 7237 0000 004f  rO...r$...r7...O
-00001010: 0000 0073 4a00 0000 0806 0a01 0202 1601  ...sJ...........
-00001020: 0c01 0801 02ff 0803 0201 1601 0c01 0801  ................
-00001030: 02ff 0803 0201 1601 0c01 0401 02ff 0a03  ................
-00001040: 0601 0802 0c02 0803 0e01 0c01 1202 0201  ................
-00001050: 0201 0401 04ff 0602 04fe 0403 06fd 04ff  ................
-00001060: 0808 7a1b 4669 6c65 4765 6e65 7261 746f  ..z.FileGenerato
-00001070: 722e 6765 6e65 7261 7465 5f63 6f64 6563  r.generate_codec
-00001080: 0300 0000 0000 0000 0000 0000 0600 0000  ................
-00001090: 0800 0000 4300 0000 739a 0000 0074 007c  ....C...s....t.|
-000010a0: 026a 016a 026a 037c 026a 016a 026a 0483  .j.j.j.|.j.j.j..
-000010b0: 027d 037a 0a74 057c 0364 017c 006a 0617  .}.z.t.|.d.|.j..
-000010c0: 0083 027d 0457 006e 0b04 0074 0779 2001  ...}.W.n...t.y .
-000010d0: 0001 0001 0064 007d 0459 006e 0177 007c  .....d.}.Y.n.w.|
-000010e0: 0464 0075 0072 417a 0a74 057c 0364 027c  .d.u.rAz.t.|.d.|
-000010f0: 006a 0617 0083 027d 0557 006e 0904 0074  .j.....}.W.n...t
-00001100: 0779 3801 0001 0001 0059 006e 0977 0074  .y8......Y.n.w.t
-00001110: 087c 0574 0983 0272 417c 056a 0a7d 047c  .|.t...rA|.j.}.|
-00001120: 0464 0075 0172 4b7c 047c 0183 0101 0064  .d.u.rK|.|.....d
-00001130: 0053 0064 0053 0029 034e 5a11 5f63 6f6d  .S.d.S.).NZ._com
-00001140: 706c 6574 655f 7061 7261 6d73 5f72 4e00  plete_params_rN.
-00001150: 0000 290b 7208 0000 00da 0763 6c61 7373  ..).r......class
-00001160: 6573 da06 4f75 7470 7574 da0b 6d6f 6475  es..Output..modu
-00001170: 6c65 5f6e 616d 65da 0a63 6c61 7373 5f6e  le_name..class_n
-00001180: 616d 6572 5200 0000 7253 0000 0072 5400  amerR...rS...rT.
-00001190: 0000 7255 0000 0072 0900 0000 da0f 636f  ..rU...r......co
-000011a0: 6d70 6c65 7465 5f70 6172 616d 7329 06da  mplete_params)..
-000011b0: 0363 6c73 7233 0000 00da 0b69 6e66 6f5f  .clsr3.....info_
-000011c0: 736f 6c76 6572 5a0a 6f75 7470 7574 5f63  solverZ.output_c
-000011d0: 6c73 725f 0000 0072 5900 0000 7223 0000  lsr_...rY...r#..
-000011e0: 0072 2300 0000 7224 0000 00da 1d5f 636f  .r#...r$....._co
-000011f0: 6d70 6c65 7465 5f70 6172 616d 735f 7769  mplete_params_wi
-00001200: 7468 5f64 6566 6175 6c74 8000 0000 7328  th_default....s(
-00001210: 0000 0002 0208 0108 0104 fe02 0414 010c  ................
-00001220: 0108 0102 ff08 0302 0114 010c 0104 0102  ................
-00001230: ff0a 0306 0108 020c 0104 ff7a 2b46 696c  ...........z+Fil
-00001240: 6547 656e 6572 6174 6f72 2e5f 636f 6d70  eGenerator._comp
-00001250: 6c65 7465 5f70 6172 616d 735f 7769 7468  lete_params_with
-00001260: 5f64 6566 6175 6c74 7226 0000 0029 0a72  _defaultr&...).r
-00001270: 2a00 0000 722b 0000 0072 2c00 0000 7248  *...r+...r,...rH
-00001280: 0000 0072 4900 0000 7225 0000 0072 3700  ...rI...r%...r7.
-00001290: 0000 da0b 636c 6173 736d 6574 686f 6472  ....classmethodr
-000012a0: 6200 0000 da0d 5f5f 636c 6173 7363 656c  b.....__classcel
-000012b0: 6c5f 5f72 2300 0000 7223 0000 0072 4c00  l__r#...r#...rL.
-000012c0: 0000 7224 0000 0072 4a00 0000 4900 0000  ..r$...rJ...I...
-000012d0: 730c 0000 000a 0008 010c 020a 0302 3112  s.............1.
-000012e0: 0172 4a00 0000 da01 3063 0200 0000 0000  .rJ.....0c......
-000012f0: 0000 0000 0000 0300 0000 0b00 0000 4300  ..............C.
-00001300: 0000 7342 0000 0064 0174 007c 0083 019b  ..sB...d.t.|....
-00001310: 009d 027d 0274 017c 0274 0266 017c 017c  ...}.t.|.t.f.|.|
-00001320: 019b 0064 027c 009b 009d 037c 009b 0064  ...d.|.....|...d
-00001330: 039d 0274 037c 00a0 0464 0464 05a1 0283  ...t.|...d.d....
-00001340: 0164 069c 0483 0353 0029 074e 724a 0000  .d.....S.).NrJ..
-00001350: 00fa 012f 7a06 2e6a 696e 6a61 da01 2eda  .../z..jinja....
-00001360: 015f 2904 da08 6469 725f 6e61 6d65 722f  ._)...dir_namer/
-00001370: 0000 0072 2800 0000 7253 0000 0029 0572  ...r(...rS...).r
-00001380: 0600 0000 7214 0000 0072 4a00 0000 7207  ....r....rJ...r.
-00001390: 0000 00da 0772 6570 6c61 6365 2903 da09  .....replace)...
-000013a0: 6669 6c65 5f6e 616d 6572 6900 0000 da08  file_nameri.....
-000013b0: 636c 735f 6e61 6d65 7223 0000 0072 2300  cls_namer#...r#.
-000013c0: 0000 7224 0000 00da 186e 6577 5f66 696c  ..r$.....new_fil
-000013d0: 655f 6765 6e65 7261 746f 725f 636c 6173  e_generator_clas
-000013e0: 7398 0000 0073 1400 0000 0e01 0201 0201  s....s..........
-000013f0: 0401 0202 0c01 0801 0e01 04fc 04fd 726d  ..............rm
-00001400: 0000 0029 0172 6500 0000 2916 722d 0000  ...).re...).r-..
-00001410: 00da 0361 6263 7202 0000 0072 0300 0000  ...abcr....r....
-00001420: da07 696e 7370 6563 7472 0400 0000 da07  ..inspectr......
-00001430: 7061 7468 6c69 6272 0500 0000 721a 0000  pathlibr....r...
-00001440: 00da 0a69 6e66 6c65 6374 696f 6e72 0600  ...inflectionr..
-00001450: 0000 7207 0000 00da 0d66 6c75 6964 6479  ..r......fluiddy
-00001460: 6e2e 7574 696c 7208 0000 00da 1d66 6c75  n.utilr......flu
-00001470: 6964 7369 6d66 6f61 6d2e 666f 616d 5f69  idsimfoam.foam_i
-00001480: 6e70 7574 5f66 696c 6573 7209 0000 0072  nput_filesr....r
-00001490: 0a00 0000 720b 0000 0072 0c00 0000 722e  ....r....r....r.
-000014a0: 0000 0072 4a00 0000 726d 0000 0072 2300  ...rJ...rm...r#.
-000014b0: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
-000014c0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000014d0: 1800 0000 0400 1002 0c01 0c01 0802 1001  ................
-000014e0: 0c02 1401 0e03 1019 1022 0e4f            .........".O
+00000da0: 7075 742e 5f6d 616b 655f 636f 6465 5f62  put._make_code_b
+00000db0: 6c6f 636b 5f6d 6573 685f 6469 6374 602c  lock_mesh_dict`,
+00000dc0: 0a20 2020 2020 2020 202d 206f 7220 6120  .        - or a 
+00000dd0: 4a69 6e6a 6120 7465 6d70 6c61 7465 2e0a  Jinja template..
+00000de0: 2020 2020 2020 2020 4e5a 0b5f 6d61 6b65          NZ._make
+00000df0: 5f63 6f64 655f 5a0b 5f6d 616b 655f 7472  _code_Z._make_tr
+00000e00: 6565 5fda 085f 6865 6c70 6572 5f63 0100  ee_.._helper_c..
+00000e10: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000e20: 0000 1300 0000 730c 0000 0088 007c 0083  ......s......|..
+00000e30: 01a0 00a1 0053 0072 2000 0000 2901 7240  .....S.r ...).r@
+00000e40: 0000 0029 015a 0770 6172 616d 735f a901  ...).Z.params_..
+00000e50: da09 6d61 6b65 5f74 7265 6572 1d00 0000  ..make_treer....
+00000e60: 721e 0000 00da 096d 616b 655f 636f 6465  r......make_code
+00000e70: 6e00 0000 7223 0000 007a 2e46 696c 6547  n...r#...z.FileG
+00000e80: 656e 6572 6174 6f72 2e67 656e 6572 6174  enerator.generat
+00000e90: 655f 636f 6465 2e3c 6c6f 6361 6c73 3e2e  e_code.<locals>.
+00000ea0: 6d61 6b65 5f63 6f64 6529 0172 2d00 0000  make_code).r-...
+00000eb0: 7a3b 466c 7569 6473 696d 666f 616d 2073  z;Fluidsimfoam s
+00000ec0: 6f6c 7665 7220 6973 7375 653a 2032 2063  olver issue: 2 c
+00000ed0: 6f6e 6375 7272 656e 7420 6d65 7468 6f64  oncurrent method
+00000ee0: 7320 746f 2070 726f 6475 6365 207a 103a  s to produce z.:
+00000ef0: 0a2d 2074 656d 706c 6174 6520 696e 207a  .- template in z
+00000f00: 1f2c 0a2d 2066 756e 6374 696f 6e20 6f75  .,.- function ou
+00000f10: 7470 7574 2e5f 6d61 6b65 5f63 6f64 655f  tput._make_code_
+00000f20: 7a3d 2e0a 5265 6d6f 7665 2074 6865 2066  z=..Remove the f
+00000f30: 696c 6520 6f72 2074 6865 2066 756e 6374  ile or the funct
+00000f40: 696f 6e20 286f 7220 6d61 6b65 2069 7420  ion (or make it 
+00000f50: 6571 7561 6c20 746f 204e 6f6e 6529 2e29  equal to None).)
+00000f60: 1172 1100 0000 7213 0000 0072 2d00 0000  .r....r....r-...
+00000f70: da07 6765 7461 7474 72da 055f 6e61 6d65  ..getattr.._name
+00000f80: da0e 4174 7472 6962 7574 6545 7272 6f72  ..AttributeError
+00000f90: da0a 6973 696e 7374 616e 6365 7209 0000  ..isinstancer...
+00000fa0: 0072 4a00 0000 722a 0000 0072 2100 0000  .rJ...r*...r!...
+00000fb0: 7222 0000 00da 0672 656e 6465 7272 1700  r".....renderr..
+00000fc0: 0000 da06 6578 6973 7473 da0c 5275 6e74  ....exists..Runt
+00000fd0: 696d 6545 7272 6f72 7229 0000 0029 0572  imeErrorr)...).r
+00000fe0: 1b00 0000 722d 0000 0072 4b00 0000 da06  ....r-...rK.....
+00000ff0: 6865 6c70 6572 da08 7465 6d70 6c61 7465  helper..template
+00001000: 721d 0000 0072 4900 0000 721e 0000 0072  r....rI...r....r
+00001010: 3100 0000 4f00 0000 734a 0000 0008 060a  1...O...sJ......
+00001020: 0102 0216 010c 0108 0102 ff08 0302 0116  ................
+00001030: 010c 0108 0102 ff08 0302 0116 010c 0104  ................
+00001040: 0102 ff0a 0306 0108 020c 0208 030e 010c  ................
+00001050: 0112 0202 0102 0104 0104 ff06 0204 fe04  ................
+00001060: 0306 fd04 ff08 087a 1b46 696c 6547 656e  .......z.FileGen
+00001070: 6572 6174 6f72 2e67 656e 6572 6174 655f  erator.generate_
+00001080: 636f 6465 6303 0000 0000 0000 0000 0000  codec...........
+00001090: 0006 0000 0008 0000 0043 0000 0073 9a00  .........C...s..
+000010a0: 0000 7400 7c02 6a01 6a02 6a03 7c02 6a01  ..t.|.j.j.j.|.j.
+000010b0: 6a02 6a04 8302 7d03 7a0a 7405 7c03 6401  j.j...}.z.t.|.d.
+000010c0: 7c00 6a06 1700 8302 7d04 5700 6e0b 0400  |.j.....}.W.n...
+000010d0: 7407 7920 0100 0100 0100 6400 7d04 5900  t.y ......d.}.Y.
+000010e0: 6e01 7700 7c04 6400 7500 7241 7a0a 7405  n.w.|.d.u.rAz.t.
+000010f0: 7c03 6402 7c00 6a06 1700 8302 7d05 5700  |.d.|.j.....}.W.
+00001100: 6e09 0400 7407 7938 0100 0100 0100 5900  n...t.y8......Y.
+00001110: 6e09 7700 7408 7c05 7409 8302 7241 7c05  n.w.t.|.t...rA|.
+00001120: 6a0a 7d04 7c04 6400 7501 724b 7c04 7c01  j.}.|.d.u.rK|.|.
+00001130: 8301 0100 6400 5300 6400 5300 2903 4e5a  ....d.S.d.S.).NZ
+00001140: 115f 636f 6d70 6c65 7465 5f70 6172 616d  ._complete_param
+00001150: 735f 7248 0000 0029 0b72 0800 0000 da07  s_rH...).r......
+00001160: 636c 6173 7365 73da 064f 7574 7075 74da  classes..Output.
+00001170: 0b6d 6f64 756c 655f 6e61 6d65 da0a 636c  .module_name..cl
+00001180: 6173 735f 6e61 6d65 724c 0000 0072 4d00  ass_namerL...rM.
+00001190: 0000 724e 0000 0072 4f00 0000 7209 0000  ..rN...rO...r...
+000011a0: 00da 0f63 6f6d 706c 6574 655f 7061 7261  ...complete_para
+000011b0: 6d73 2906 da03 636c 7372 2d00 0000 da0b  ms)...clsr-.....
+000011c0: 696e 666f 5f73 6f6c 7665 725a 0a6f 7574  info_solverZ.out
+000011d0: 7075 745f 636c 7372 5900 0000 7253 0000  put_clsrY...rS..
+000011e0: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+000011f0: da1d 5f63 6f6d 706c 6574 655f 7061 7261  .._complete_para
+00001200: 6d73 5f77 6974 685f 6465 6661 756c 7480  ms_with_default.
+00001210: 0000 0073 2800 0000 0202 0801 0801 04fe  ...s(...........
+00001220: 0204 1401 0c01 0801 02ff 0803 0201 1401  ................
+00001230: 0c01 0401 02ff 0a03 0601 0802 0c01 04ff  ................
+00001240: 7a2b 4669 6c65 4765 6e65 7261 746f 722e  z+FileGenerator.
+00001250: 5f63 6f6d 706c 6574 655f 7061 7261 6d73  _complete_params
+00001260: 5f77 6974 685f 6465 6661 756c 7472 2000  _with_defaultr .
+00001270: 0000 290a 7224 0000 0072 2500 0000 7226  ..).r$...r%...r&
+00001280: 0000 0072 4200 0000 7243 0000 0072 1f00  ...rB...rC...r..
+00001290: 0000 7231 0000 00da 0b63 6c61 7373 6d65  ..r1.....classme
+000012a0: 7468 6f64 725c 0000 00da 0d5f 5f63 6c61  thodr\.....__cla
+000012b0: 7373 6365 6c6c 5f5f 721d 0000 0072 1d00  sscell__r....r..
+000012c0: 0000 7246 0000 0072 1e00 0000 7244 0000  ..rF...r....rD..
+000012d0: 0049 0000 0073 0c00 0000 0a00 0801 0c02  .I...s..........
+000012e0: 0a03 0231 1201 7244 0000 00da 0130 6302  ...1..rD.....0c.
+000012f0: 0000 0000 0000 0000 0000 0003 0000 000b  ................
+00001300: 0000 0043 0000 0073 4200 0000 6401 7400  ...C...sB...d.t.
+00001310: 7c00 8301 9b00 9d02 7d02 7401 7c02 7402  |.......}.t.|.t.
+00001320: 6601 7c01 7c01 9b00 6402 7c00 9b00 9d03  f.|.|...d.|.....
+00001330: 7c00 9b00 6403 9d02 7403 7c00 a004 6404  |...d...t.|...d.
+00001340: 6405 a102 8301 6406 9c04 8303 5300 2907  d.....d.....S.).
+00001350: 4e72 4400 0000 fa01 2f7a 062e 6a69 6e6a  NrD...../z..jinj
+00001360: 61da 012e da01 5f29 04da 0864 6972 5f6e  a....._)...dir_n
+00001370: 616d 6572 2900 0000 7222 0000 0072 4d00  amer)...r"...rM.
+00001380: 0000 2905 7206 0000 0072 1200 0000 7244  ..).r....r....rD
+00001390: 0000 0072 0700 0000 da07 7265 706c 6163  ...r......replac
+000013a0: 6529 03da 0966 696c 655f 6e61 6d65 7263  e)...file_namerc
+000013b0: 0000 00da 0863 6c73 5f6e 616d 6572 1d00  .....cls_namer..
+000013c0: 0000 721d 0000 0072 1e00 0000 da18 6e65  ..r....r......ne
+000013d0: 775f 6669 6c65 5f67 656e 6572 6174 6f72  w_file_generator
+000013e0: 5f63 6c61 7373 9800 0000 7314 0000 000e  _class....s.....
+000013f0: 0102 0102 0104 0102 020c 0108 010e 0104  ................
+00001400: fc04 fd72 6700 0000 2901 725f 0000 0029  ...rg...).r_...)
+00001410: 1672 2700 0000 da03 6162 6372 0200 0000  .r'.....abcr....
+00001420: 7203 0000 00da 0769 6e73 7065 6374 7204  r......inspectr.
+00001430: 0000 00da 0770 6174 686c 6962 7205 0000  .....pathlibr...
+00001440: 0072 1800 0000 da0a 696e 666c 6563 7469  .r......inflecti
+00001450: 6f6e 7206 0000 0072 0700 0000 da0d 666c  onr....r......fl
+00001460: 7569 6464 796e 2e75 7469 6c72 0800 0000  uiddyn.utilr....
+00001470: da1d 666c 7569 6473 696d 666f 616d 2e66  ..fluidsimfoam.f
+00001480: 6f61 6d5f 696e 7075 745f 6669 6c65 7372  oam_input_filesr
+00001490: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
+000014a0: 0000 0072 2800 0000 7244 0000 0072 6700  ...r(...rD...rg.
+000014b0: 0000 721d 0000 0072 1d00 0000 721d 0000  ..r....r....r...
+000014c0: 0072 1e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000014d0: 0100 0000 7318 0000 0004 0010 020c 010c  ....s...........
+000014e0: 0108 0210 010c 0214 010e 0310 1910 220e  ..............".
+000014f0: 4f                                       O
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/ast.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/ast.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from numbers import Number
 from textwrap import dedent
 from typing import Optional
 
+import numpy as np
 from inflection import underscore
 
 symbols = ["kg", "m", "s", "K", "kmol", "A", "cd"]
 
 
 def str2foam_units(units):
     result = [0] * 7
@@ -115,22 +116,51 @@
                     comments=comments_dict,
                 )
                 self._set_item(key, obj)
             else:
                 raise NotImplementedError(type(value))
 
     def set_child(self, key, child):
-        if isinstance(child, (type(None), str, Number)):
+        if (
+            isinstance(child, list)
+            and child
+            and isinstance(child[0], list)
+            and child[0]
+            and all(isinstance(n, Number) for n in child[0])
+        ):
+            child = np.array(child)
+
+        if isinstance(child, (type(None), str, Number, DimensionSet)):
             pass
         elif isinstance(child, dict):
             child = Dict(child, name=key)
         elif isinstance(child, list):
             child = List(child, name=key)
+        elif isinstance(child, np.ndarray):
+            shape = child.shape
+            ndim = child.ndim
+            child.tolist()
+            dtype = None
+            if ndim == 2:
+                if shape[1] == 9:
+                    dtype = "tensor"
+                elif shape[1] == 3:
+                    dtype = "vector"
+                else:
+                    raise NotImplementedError
+                child = [List(sequence) for sequence in child]
+            elif ndim == 1:
+                dtype = "scalar"
+            else:
+                raise NotImplementedError
+            child = List(child, name=key, dtype=dtype)
+        elif isinstance(child, Node):
+            pass
         else:
-            raise NotImplementedError
+            raise NotImplementedError(type(child))
         self._set_item(key, child)
 
     def set_value(self, name, value, dimension=None):
         if isinstance(value, Number) or dimension is not None:
             value = Value(value, name, dimension=dimension)
         self._set_item(name, value)
 
@@ -203,14 +233,20 @@
             raise ValueError("self.path is None")
         with open(self.path, "w") as file:
             file.write(self.dump())
 
     def _set_item(self, key, value):
         self.children[key] = value
 
+    def __setitem__(self, key, item):
+        self.children[key] = item
+
+    def __getitem__(self, key):
+        return self.children[key]
+
 
 @dataclass
 class Assignment:
     name: str
     value: object
 
     def dump(self, indent=0):
@@ -269,14 +305,16 @@
             return f"[{dimension_dumped}] {value_dumped}"
         else:
             return f"{value_dumped}"
 
 
 class DimensionSet(list, Node):
     def __init__(self, foam_units):
+        if isinstance(foam_units, str):
+            foam_units = str2foam_units(foam_units)
         if not all(isinstance(elem, int) for elem in foam_units):
             raise ValueError("Bad {foam_units = }")
         super().__init__(foam_units)
 
     def __repr__(self):
         return foam_units2str(self)
 
@@ -336,16 +374,17 @@
     def _set_item(self, key, value):
         self[key] = value
 
 
 class List(list, Node):
     """Represents an OpenFoam list"""
 
-    def __init__(self, iterable=None, name=None):
+    def __init__(self, iterable=None, name=None, dtype=None):
         self._name = name
+        self._dtype = dtype
         super().__init__(iterable)
 
     def get_name(self):
         return self._name
 
     def add_name(self, name):
         if self._name is None:
@@ -371,15 +410,22 @@
     def dump(self, indent=0):
         tmp = []
         indentation = indent * " "
         if self._name is None:
             tmp.extend(self._make_list_strings(indent=0))
             return indentation + "(" + " ".join(tmp) + ")"
         else:
-            tmp.append(indentation + self._name + f"\n{indentation}" + "(")
+            header = self._name
+            if self._dtype is not None:
+                header += (
+                    f"   nonuniform List<{self._dtype}>\n"
+                    f"{indentation}{len(self)}"
+                )
+
+            tmp.append(indentation + header + f"\n{indentation}" + "(")
             special_keys = {"blocks": "hex", "edges": "spline"}
             if self._name not in special_keys.keys():
                 tmp.append("\n".join(self._make_list_strings(indent + 4)))
             elif self:
                 special_key = special_keys[self._name]
                 if not self[0] == special_key:
                     raise ValueError(self)
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,15 @@
         # for blocks, edges, boundaries
         self.index = index
 
     def format(self):
         comment = f"{self.index} {self.name}"
         if len(self.alias) > 1:
             comment += " : " + " ".join(sorted(self.alias))
-        return (
-            f"( {self.x:18.15g} {self.y:18.15g} {self.z:18.15g} )  // {comment}"
-        )
+        return f"( {self.x: .15g} {self.y: .15g} {self.z: .15g} )  // {comment}"
 
     def __lt__(self, rhs):
         return (self.z, self.y, self.x) < (rhs.z, rhs.y, rhs.x)
 
     def __eq__(self, rhs):
         return (self.z, self.y, self.x) == (rhs.z, rhs.y, rhs.x)
 
@@ -110,15 +108,15 @@
             f"{self.grading.format()}  // {self.name} ({comment})"
         )
 
     def face(self, index, name=None):
         """Generate Face object
         index is number or keyword to identify the face of Hex
             0 = 'w' = 'xm' = '-100' = (0 4 7 3)
-            1 = 'e' = 'xp' = '100' = (1 2 5 6)
+            1 = 'e' = 'xp' = '100' = (1 2 6 5)
             2 = 's' = 'ym' = '0-10' = (0 1 5 4)
             3 = 'n' = 'yp' = '010' = (2 3 7 6)
             4 = 'b' = 'zm' = '00-1' = (0 3 2 1) = "bottom"
             5 = 't' = 'zp' = '001' = (4 5 6 7) = "top"
         name is given to Face instance. If omitted, name is automatically
             genaratied like ('f-' + self.name + '-w')
         """
@@ -148,29 +146,26 @@
             (0, 4, 7, 3),
             (1, 2, 6, 5),
             (0, 1, 5, 4),
             (2, 3, 7, 6),
             (0, 3, 2, 1),
             (4, 5, 6, 7),
         ]
-        index_to_defaultsuffix = [
-            "f-{}-w",
-            "f-{}-n",
-            "f-{}-s",
-            "f-{}-n",
-            "f-{}-b",
-            "f-{}-t",
-        ]
+        index_to_defaultsuffix = "wesnbt"
 
         if isinstance(index, str):
             index = kw_to_index[index]
 
         vnames = tuple([self.vnames[i] for i in index_to_vertex[index]])
         if name is None:
-            name = index_to_defaultsuffix[index].format(self.name)
+            parts = ["f"]
+            if self.name:
+                parts.append(self.name)
+            parts.append(index_to_defaultsuffix[index])
+            name = "-".join(parts)
         return Face(vnames, name)
 
 
 class Boundary:
     def __init__(self, type_, name, faces=None, neighbour=None):
         """initialize boundary
         type_ is type keyword (wall, patch, empty, ..)
@@ -200,16 +195,16 @@
         if self.neighbour is None:
             tmp.append("{\n" + f"    type {self.type_};\n    faces\n    (")
         else:
             tmp.append(
                 "{\n"
                 + f"    type {self.type_};\n    neighbourPatch  {self.neighbour};\n    faces\n    ("
             )
-        for f in self.faces:
-            tmp.append(f"        {f.format(vertices)}")
+        for face in self.faces:
+            tmp.append(f"        {face.format(vertices)}")
         tmp.append("    );\n}")
         return "\n".join(tmp)
 
 
 class BlockMeshDict:
     def __init__(self):
         self.convert_to_meters = 1.0
@@ -285,15 +280,19 @@
             groups.append(list(g))
         for group in groups:
             if len(group) == 1:
                 continue
             names = [v[0] for v in group]
             self.reduce_vertex(*names)
 
-    def add_hexblock(self, vnames, cells, name, grading=SimpleGrading(1, 1, 1)):
+    def add_hexblock(
+        self, vnames, cells, name=None, grading=SimpleGrading(1, 1, 1)
+    ):
+        if name is None:
+            name = f"b{len(self.blocks)}"
         b = HexBlock(vnames, cells, name, grading)
         self.blocks[name] = b
         return b
 
     def add_arcedge(self, vnames, name, inter_vertex):
         e = ArcEdge(vnames, name, inter_vertex)
         self.edges[name] = e
@@ -306,14 +305,24 @@
 
     def add_boundary(self, type_, name, faces=None, neighbour=None):
         b = Boundary(type_, name, faces, neighbour)
         self.boundaries[name] = b
         return b
 
     def add_cyclic_boundaries(self, name0, name1, faces0, faces1):
+        """Add 2 cyclic boundaries
+
+        Example
+        -------
+
+        2 cyclic boundaries can be created as follow::
+
+          add_cyclic_boundaries("outlet", "inlet", b0.face("e"), b0.face("w"))
+
+        """
         b0 = self.add_boundary("cyclic", name0, faces0, neighbour=name1)
         b1 = self.add_boundary("cyclic", name1, faces1, neighbour=name0)
         return b0, b1
 
     def assign_vertexid(self, sort=True):
         """1. create list of Vertex which are referred by blocks only.
         2. sort vertex according to (x, y, z)
@@ -386,18 +395,21 @@
             indent = " " * 4
             s = b.format(self.vertices).replace("\n", "\n" + indent)
             tmp.append(indent + s)
         tmp.append(");")
         return "\n".join(tmp)
 
     def format_mergepatchpairs_section(self):
-        return """\
-mergePatchPairs
-(
-);"""
+        # not yet implemented
+        return ""
+
+    #         return """\
+    # mergePatchPairs
+    # (
+    # );"""
 
     def format(self, header=DEFAULT_HEADER, sort_vortices=True):
         self.assign_vertexid(sort=sort_vortices)
         template = Template(
             r"""$header
 FoamFile
 {
@@ -413,23 +425,45 @@
 $vertices
 
 $blocks
 
 $edges
 
 $boundary
-
 $mergepatchpairs
-
 // ************************************************************************* //
 """
         )
 
         return template.substitute(
             header=header,
             metricconvert=str(self.convert_to_meters),
             vertices=self.format_vertices_section(),
             edges=self.format_edges_section(),
             blocks=self.format_blocks_section(),
             boundary=self.format_boundary_section(),
             mergepatchpairs=self.format_mergepatchpairs_section(),
         )
+
+
+class BlockMeshDictRectilinear(BlockMeshDict):
+    def __init__(self, lx, ly, lz, nx, ny, nz, scale):
+        super().__init__()
+
+        self.set_scale(scale)
+
+        basevs = [
+            Vertex(0, 0, 0, "v0"),
+            Vertex(lx, 0, 0, "v1"),
+            Vertex(lx, ly, 0, "v2"),
+            Vertex(0, ly, 0, "v3"),
+        ]
+
+        for v in basevs:
+            self.add_vertex(v.x, v.y, 0, v.name + "-bot")
+            self.add_vertex(v.x, v.y, lz, v.name + "-top")
+
+        vertex_names = [
+            f"v{index}{post}" for post in ("-bot", "-top") for index in range(4)
+        ]
+
+        self.block = self.add_hexblock(vertex_names, (nx, ny, nz), name="")
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May  5 07:30:16 2023 UTC, .py size: 13459 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,905 +1,976 @@
-00000000: 6f0d 0d0a 0000 0000 88b0 5464 9334 0000  o.........Td.4..
+00000000: 6f0d 0d0a 0000 0000 faba 6b64 8238 0000  o.........kd.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6406 6407 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6406 6408 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6700  m.Z.m.Z.m.Z...g.
 00000080: 6409 a201 5a0f 4700 640a 640b 8400 640b  d...Z.G.d.d...d.
 00000090: 8302 5a10 4700 640c 640d 8400 640d 8302  ..Z.G.d.d...d...
 000000a0: 5a11 4700 640e 640f 8400 640f 8302 5a12  Z.G.d.d...d...Z.
 000000b0: 4700 6410 6411 8400 6411 8302 5a13 4700  G.d.d...d...Z.G.
 000000c0: 6412 6413 8400 6413 8302 5a14 4700 6414  d.d...d...Z.G.d.
-000000d0: 6415 8400 6415 8302 5a15 6416 5300 2917  d...d...Z.d.S.).
-000000e0: 6120 0100 0048 656c 7065 7220 746f 2063  a ...Helper to c
-000000f0: 7265 6174 6520 626c 6f63 6b4d 6573 6844  reate blockMeshD
-00000100: 6963 7420 6669 6c65 730a 0a54 616b 656e  ict files..Taken
-00000110: 2066 726f 6d20 6874 7470 733a 2f2f 6769   from https://gi
-00000120: 7468 7562 2e63 6f6d 2f74 616b 6161 6b69  thub.com/takaaki
-00000130: 616f 6b69 2f6f 6662 6c6f 636b 6d65 7368  aoki/ofblockmesh
-00000140: 6469 6374 6865 6c70 6572 2028 4769 7420  dicthelper (Git 
-00000150: 636f 6d6d 6974 0a35 3835 3839 6631 2920  commit.58589f1) 
-00000160: 616e 6420 6d6f 6469 6669 6564 2061 7320  and modified as 
-00000170: 666f 6c6c 6f77 3a0a 0a2d 2060 6070 7975  follow:..- ``pyu
-00000180: 7067 7261 6465 205f 5f69 6e69 745f 5f2e  pgrade __init__.
-00000190: 7079 202d 2d70 7933 392d 706c 7573 6060  py --py39-plus``
-000001a0: 0a2d 2074 6573 7465 6420 2831 3030 2520  .- tested (100% 
-000001b0: 636f 7665 7261 6765 2920 616e 6420 7265  coverage) and re
-000001c0: 7072 6f64 7563 6962 6c65 2028 7365 7473  producible (sets
-000001d0: 2073 6f72 7465 6429 0a2d 2072 6566 6163   sorted).- refac
-000001e0: 746f 720a 2d20 7375 7070 6f72 7420 666f  tor.- support fo
-000001f0: 7220 6379 636c 6963 2062 6f75 6e64 6172  r cyclic boundar
-00000200: 6965 730a 0ae9 0000 0000 2901 da07 6772  ies.......)...gr
-00000210: 6f75 7062 7929 01da 0854 656d 706c 6174  oupby)...Templat
-00000220: 65e9 0200 0000 2901 da0e 4445 4641 554c  e.....)...DEFAUL
-00000230: 545f 4845 4144 4552 e901 0000 0029 02da  T_HEADER.....)..
-00000240: 0741 7263 4564 6765 da0a 5370 6c69 6e65  .ArcEdge..Spline
-00000250: 4564 6765 2904 da0b 4564 6765 4772 6164  Edge)...EdgeGrad
-00000260: 696e 67da 0747 7261 6469 6e67 da0d 5369  ing..Grading..Si
-00000270: 6d70 6c65 4772 6164 696e 67da 1453 696d  mpleGrading..Sim
-00000280: 706c 6547 7261 6469 6e67 456c 656d 656e  pleGradingElemen
-00000290: 7429 0672 0a00 0000 720c 0000 0072 0b00  t).r....r....r..
-000002a0: 0000 7209 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000002b0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000002c0: 0000 0300 0000 4000 0000 7336 0000 0065  ......@...s6...e
-000002d0: 005a 0164 005a 0264 0c64 0264 0384 015a  .Z.d.Z.d.d.d...Z
-000002e0: 0364 0464 0584 005a 0464 0664 0784 005a  .d.d...Z.d.d...Z
-000002f0: 0564 0864 0984 005a 0664 0a64 0b84 005a  .d.d...Z.d.d...Z
-00000300: 0764 0153 0029 0dda 0656 6572 7465 784e  .d.S.)...VertexN
-00000310: 6306 0000 0000 0000 0000 0000 0006 0000  c...............
-00000320: 0002 0000 0043 0000 0073 2a00 0000 7c01  .....C...s*...|.
-00000330: 7c00 5f00 7c02 7c00 5f01 7c03 7c00 5f02  |._.|.|._.|.|._.
-00000340: 7c04 7c00 5f03 7c04 6801 7c00 5f04 7c05  |.|._.|.h.|._.|.
-00000350: 7c00 5f05 6400 5300 a901 4e29 06da 0178  |._.d.S...N)...x
-00000360: da01 79da 017a da04 6e61 6d65 da05 616c  ..y..z..name..al
-00000370: 6961 73da 0569 6e64 6578 2906 da04 7365  ias..index)...se
-00000380: 6c66 720f 0000 0072 1000 0000 7211 0000  lfr....r....r...
-00000390: 0072 1200 0000 7214 0000 00a9 0072 1600  .r....r......r..
-000003a0: 0000 fa55 2f68 6f6d 652f 7069 6572 7265  ...U/home/pierre
-000003b0: 2f44 6576 2f66 6c75 6964 7369 6d66 6f61  /Dev/fluidsimfoa
-000003c0: 6d2f 7372 632f 666c 7569 6473 696d 666f  m/src/fluidsimfo
-000003d0: 616d 2f66 6f61 6d5f 696e 7075 745f 6669  am/foam_input_fi
-000003e0: 6c65 732f 626c 6f63 6b6d 6573 682f 5f5f  les/blockmesh/__
-000003f0: 696e 6974 5f5f 2e70 79da 085f 5f69 6e69  init__.py..__ini
-00000400: 745f 5f1f 0000 0073 0c00 0000 0601 0601  t__....s........
-00000410: 0601 0601 0801 0a04 7a0f 5665 7274 6578  ........z.Vertex
-00000420: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000430: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
-00000440: 0000 7360 0000 007c 006a 009b 0064 017c  ..s`...|.j...d.|
-00000450: 006a 019b 009d 037d 0174 027c 006a 0383  .j.....}.t.|.j..
-00000460: 0164 026b 0472 1c7c 0164 0364 01a0 0474  .d.k.r.|.d.d...t
-00000470: 057c 006a 0383 01a1 0117 0037 007d 0164  .|.j.......7.}.d
-00000480: 047c 006a 0664 059b 0464 017c 006a 0764  .|.j.d...d.|.j.d
-00000490: 059b 0464 017c 006a 0864 059b 0464 067c  ...d.|.j.d...d.|
-000004a0: 019b 009d 0853 0029 074e da01 2072 0600  .....S.).N.. r..
-000004b0: 0000 7a03 203a 20fa 0228 20fa 0631 382e  ..z. : ..( ..18.
-000004c0: 3135 677a 0720 2920 202f 2f20 2909 7214  15gz. )  // ).r.
-000004d0: 0000 0072 1200 0000 da03 6c65 6e72 1300  ...r......lenr..
-000004e0: 0000 da04 6a6f 696e da06 736f 7274 6564  ....join..sorted
-000004f0: 720f 0000 0072 1000 0000 7211 0000 0029  r....r....r....)
-00000500: 0272 1500 0000 da07 636f 6d6d 656e 7472  .r......commentr
-00000510: 1600 0000 7216 0000 0072 1700 0000 da06  ....r....r......
-00000520: 666f 726d 6174 2a00 0000 730a 0000 0012  format*...s.....
-00000530: 010e 0118 0126 0202 ff7a 0d56 6572 7465  .....&...z.Verte
-00000540: 782e 666f 726d 6174 6302 0000 0000 0000  x.formatc.......
-00000550: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000560: 0073 2000 0000 7c00 6a00 7c00 6a01 7c00  .s ...|.j.|.j.|.
-00000570: 6a02 6603 7c01 6a00 7c01 6a01 7c01 6a02  j.f.|.j.|.j.|.j.
-00000580: 6603 6b00 5300 720e 0000 00a9 0372 1100  f.k.S.r......r..
-00000590: 0000 7210 0000 0072 0f00 0000 a902 7215  ..r....r......r.
-000005a0: 0000 00da 0372 6873 7216 0000 0072 1600  .....rhsr....r..
-000005b0: 0000 7217 0000 00da 065f 5f6c 745f 5f32  ..r......__lt__2
-000005c0: 0000 00f3 0200 0000 2001 7a0d 5665 7274  ........ .z.Vert
-000005d0: 6578 2e5f 5f6c 745f 5f63 0200 0000 0000  ex.__lt__c......
-000005e0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-000005f0: 0000 7320 0000 007c 006a 007c 006a 017c  ..s ...|.j.|.j.|
-00000600: 006a 0266 037c 016a 007c 016a 017c 016a  .j.f.|.j.|.j.|.j
-00000610: 0266 036b 0253 0072 0e00 0000 7221 0000  .f.k.S.r....r!..
-00000620: 0072 2200 0000 7216 0000 0072 1600 0000  .r"...r....r....
-00000630: 7217 0000 00da 065f 5f65 715f 5f35 0000  r......__eq__5..
-00000640: 0072 2500 0000 7a0d 5665 7274 6578 2e5f  .r%...z.Vertex._
-00000650: 5f65 715f 5f63 0100 0000 0000 0000 0000  _eq__c..........
-00000660: 0000 0100 0000 0400 0000 4300 0000 7314  ..........C...s.
-00000670: 0000 0074 007c 006a 017c 006a 027c 006a  ...t.|.j.|.j.|.j
-00000680: 0366 0383 0153 0072 0e00 0000 2904 da04  .f...S.r....)...
-00000690: 6861 7368 7211 0000 0072 1000 0000 720f  hashr....r....r.
-000006a0: 0000 00a9 0172 1500 0000 7216 0000 0072  .....r....r....r
-000006b0: 1600 0000 7217 0000 00da 085f 5f68 6173  ....r......__has
-000006c0: 685f 5f38 0000 0073 0200 0000 1401 7a0f  h__8...s......z.
-000006d0: 5665 7274 6578 2e5f 5f68 6173 685f 5f72  Vertex.__hash__r
-000006e0: 0e00 0000 2908 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
-000006f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000700: 7175 616c 6e61 6d65 5f5f 7218 0000 0072  qualname__r....r
-00000710: 2000 0000 7224 0000 0072 2600 0000 7229   ...r$...r&...r)
-00000720: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
-00000730: 0000 7217 0000 0072 0d00 0000 1e00 0000  ..r....r........
-00000740: 730c 0000 0008 000a 0108 0b08 0808 030c  s...............
-00000750: 0372 0d00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000760: 0000 0000 0000 0002 0000 0040 0000 00f3  ...........@....
-00000770: 1c00 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
-00000780: 8400 5a03 6403 6404 8400 5a04 6405 5300  ..Z.d.d...Z.d.S.
-00000790: 2906 da05 506f 696e 7463 0400 0000 0000  )...Pointc......
-000007a0: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
-000007b0: 0000 7316 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
-000007c0: 005f 017c 037c 005f 0264 0053 0072 0e00  ._.|.|._.d.S.r..
-000007d0: 0000 a903 720f 0000 0072 1000 0000 7211  ....r....r....r.
-000007e0: 0000 0029 0472 1500 0000 720f 0000 0072  ...).r....r....r
-000007f0: 1000 0000 7211 0000 0072 1600 0000 7216  ....r....r....r.
-00000800: 0000 0072 1700 0000 7218 0000 003d 0000  ...r....r....=..
-00000810: 0073 0600 0000 0601 0601 0a01 7a0e 506f  .s..........z.Po
-00000820: 696e 742e 5f5f 696e 6974 5f5f 6301 0000  int.__init__c...
-00000830: 0000 0000 0000 0000 0001 0000 0007 0000  ................
-00000840: 0043 0000 0073 2400 0000 6401 7c00 6a00  .C...s$...d.|.j.
-00000850: 6402 9b04 6403 7c00 6a01 6402 9b04 6403  d...d.|.j.d...d.
-00000860: 7c00 6a02 6402 9b04 6404 9d07 5300 2905  |.j.d...d...S.).
-00000870: 4e72 1a00 0000 721b 0000 0072 1900 0000  Nr....r....r....
-00000880: 7a02 2029 722f 0000 0072 2800 0000 7216  z. )r/...r(...r.
-00000890: 0000 0072 1600 0000 7217 0000 0072 2000  ...r....r....r .
-000008a0: 0000 4200 0000 7302 0000 0024 017a 0c50  ..B...s....$.z.P
-000008b0: 6f69 6e74 2e66 6f72 6d61 744e a905 722a  oint.formatN..r*
-000008c0: 0000 0072 2b00 0000 722c 0000 0072 1800  ...r+...r,...r..
-000008d0: 0000 7220 0000 0072 1600 0000 7216 0000  ..r ...r....r...
-000008e0: 0072 1600 0000 7217 0000 0072 2e00 0000  .r....r....r....
-000008f0: 3c00 0000 7306 0000 0008 0008 010c 0572  <...s..........r
-00000900: 2e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000910: 0000 0000 0002 0000 0040 0000 0072 2d00  .........@...r-.
-00000920: 0000 2906 da04 4661 6365 6303 0000 0000  ..)...Facec.....
-00000930: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-00000940: 0000 0073 1000 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
-00000950: 7c00 5f01 6401 5300 2902 7a38 0a20 2020  |._.d.S.).z8.   
-00000960: 2020 2020 2076 6e61 6d65 2069 7320 6c69       vname is li
-00000970: 7374 206f 7220 7475 706c 6520 6f66 2076  st or tuple of v
-00000980: 6572 7465 7820 6e61 6d65 730a 2020 2020  ertex names.    
-00000990: 2020 2020 4e29 02da 0676 6e61 6d65 7372      N)...vnamesr
-000009a0: 1200 0000 2903 7215 0000 0072 3200 0000  ....).r....r2...
-000009b0: 7212 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-000009c0: 1700 0000 7218 0000 0047 0000 0073 0400  ....r....G...s..
-000009d0: 0000 0604 0a01 7a0d 4661 6365 2e5f 5f69  ......z.Face.__i
-000009e0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
-000009f0: 0000 0400 0000 0700 0000 0300 0000 7346  ..............sF
-00000a00: 0000 0064 01a0 0087 0066 0164 0264 0384  ...d.....f.d.d..
-00000a10: 087c 006a 0144 0083 01a1 017d 0264 01a0  .|.j.D.....}.d..
-00000a20: 007c 006a 01a1 017d 0364 047c 0264 059b  .|.j...}.d.|.d..
-00000a30: 0464 067c 006a 0264 059b 0464 077c 0364  .d.|.j.d...d.|.d
-00000a40: 059b 0464 089d 0753 0029 09fa 4b46 6f72  ...d...S.)..KFor
-00000a50: 6d61 7420 696e 7374 616e 6365 2074 6f20  mat instance to 
-00000a60: 6475 6d70 0a20 2020 2020 2020 2076 6572  dump.        ver
-00000a70: 7469 6365 7320 6973 2064 6963 7420 6f66  tices is dict of
-00000a80: 206e 616d 6520 746f 2056 6572 7465 780a   name to Vertex.
-00000a90: 2020 2020 2020 2020 7219 0000 0063 0100          r....c..
-00000aa0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000ab0: 0000 3300 0000 f31e 0000 0081 007c 005d  ..3..........|.]
-00000ac0: 0a7d 0174 0088 007c 0119 006a 0183 0156  .}.t...|...j...V
-00000ad0: 0001 0071 0264 0053 0072 0e00 0000 a902  ...q.d.S.r......
-00000ae0: da03 7374 7272 1400 0000 a902 da02 2e30  ..strr.........0
-00000af0: da02 766e a901 da08 7665 7274 6963 6573  ..vn....vertices
-00000b00: 7216 0000 0072 1700 0000 da09 3c67 656e  r....r......<gen
-00000b10: 6578 7072 3e52 0000 00f3 0400 0000 0280  expr>R..........
-00000b20: 1c00 7a1e 4661 6365 2e66 6f72 6d61 742e  ..z.Face.format.
-00000b30: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
-00000b40: 723e fa01 28da 0173 7a06 2920 202f 2f20  r>..(..sz.)  // 
-00000b50: fa02 2028 fa01 2929 0372 1d00 0000 7232  .. (..)).r....r2
-00000b60: 0000 0072 1200 0000 a904 7215 0000 0072  ...r......r....r
-00000b70: 3b00 0000 7214 0000 0072 1f00 0000 7216  ;...r....r....r.
-00000b80: 0000 0072 3a00 0000 7217 0000 0072 2000  ...r:...r....r .
-00000b90: 0000 4e00 0000 7306 0000 001a 040c 0120  ..N...s........ 
-00000ba0: 017a 0b46 6163 652e 666f 726d 6174 4e72  .z.Face.formatNr
-00000bb0: 3000 0000 7216 0000 0072 1600 0000 7216  0...r....r....r.
-00000bc0: 0000 0072 1700 0000 7231 0000 0046 0000  ...r....r1...F..
-00000bd0: 0073 0600 0000 0800 0801 0c07 7231 0000  .s..........r1..
-00000be0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000bf0: 0000 0400 0000 4000 0000 7332 0000 0065  ......@...s2...e
-00000c00: 005a 0164 005a 0265 0364 0164 0164 0183  .Z.d.Z.e.d.d.d..
-00000c10: 0366 0164 0264 0384 015a 0464 0464 0584  .f.d.d...Z.d.d..
-00000c20: 005a 0564 0964 0764 0884 015a 0664 0653  .Z.d.d.d...Z.d.S
-00000c30: 0029 0ada 0848 6578 426c 6f63 6b72 0600  .)...HexBlockr..
-00000c40: 0000 6305 0000 0000 0000 0000 0000 0005  ..c.............
-00000c50: 0000 0002 0000 0043 0000 0073 1c00 0000  .......C...s....
-00000c60: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
-00000c70: 5f02 7c04 7c00 5f03 6401 5300 2902 612e  _.|.|._.d.S.).a.
-00000c80: 0100 0049 6e69 7469 616c 697a 6520 4865  ...Initialize He
-00000c90: 7842 6c6f 636b 2069 6e73 7461 6e63 650a  xBlock instance.
-00000ca0: 2020 2020 2020 2020 766e 616d 6573 2069          vnames i
-00000cb0: 7320 7468 6520 7665 7274 6578 206e 616d  s the vertex nam
-00000cc0: 6573 2069 6e20 6f72 6465 7220 6465 7363  es in order desc
-00000cd0: 7269 7665 6420 696e 0a20 2020 2020 2020  rived in.       
-00000ce0: 2020 2020 2068 7474 703a 2f2f 7777 772e       http://www.
-00000cf0: 6f70 656e 666f 616d 2e6f 7267 2f64 6f63  openfoam.org/doc
-00000d00: 732f 7573 6572 2f6d 6573 682d 6465 7363  s/user/mesh-desc
-00000d10: 7269 7074 696f 6e2e 7068 700a 2020 2020  ription.php.    
-00000d20: 2020 2020 6365 6c6c 7320 6973 206e 756d      cells is num
-00000d30: 6265 7220 6f66 2063 656c 6c73 2064 6576  ber of cells dev
-00000d40: 6965 6420 696e 746f 2069 6e20 6561 6368  ied into in each
-00000d50: 2064 6972 6563 7469 6f6e 0a20 2020 2020   direction.     
-00000d60: 2020 206e 616d 6520 6973 2074 6865 2075     name is the u
-00000d70: 6e69 7120 6e61 6d65 206f 6620 7468 6520  niq name of the 
-00000d80: 626c 6f63 6b0a 2020 2020 2020 2020 6772  block.        gr
-00000d90: 6164 696e 6720 6973 2067 7261 6469 6e67  ading is grading
-00000da0: 206d 6574 686f 642e 0a20 2020 2020 2020   method..       
-00000db0: 204e 2904 7232 0000 00da 0563 656c 6c73   N).r2.....cells
-00000dc0: 7212 0000 00da 0767 7261 6469 6e67 2905  r......grading).
-00000dd0: 7215 0000 0072 3200 0000 7244 0000 0072  r....r2...rD...r
-00000de0: 1200 0000 7245 0000 0072 1600 0000 7216  ....rE...r....r.
-00000df0: 0000 0072 1700 0000 7218 0000 0058 0000  ...r....r....X..
-00000e00: 0073 0800 0000 0608 0601 0601 0a01 7a11  .s............z.
-00000e10: 4865 7842 6c6f 636b 2e5f 5f69 6e69 745f  HexBlock.__init_
-00000e20: 5f63 0200 0000 0000 0000 0000 0000 0400  _c..............
-00000e30: 0000 1100 0000 0300 0000 737e 0000 0064  ..........s~...d
-00000e40: 01a0 0087 0066 0164 0264 0384 087c 006a  .....f.d.d...|.j
-00000e50: 0144 0083 01a1 017d 0264 01a0 007c 006a  .D.....}.d...|.j
-00000e60: 01a1 017d 0364 047c 029b 0064 057c 006a  ...}.d.|...d.|.j
-00000e70: 029b 0064 067c 006a 0364 0719 0064 089b  ...d.|.j.d...d..
-00000e80: 0464 017c 006a 0364 0919 0064 089b 0464  .d.|.j.d...d...d
-00000e90: 017c 006a 0364 0a19 0064 089b 0464 057c  .|.j.d...d...d.|
-00000ea0: 006a 04a0 05a1 009b 0064 0b7c 006a 029b  .j.......d.|.j..
-00000eb0: 0064 067c 039b 0064 0c9d 1153 0029 0d72  .d.|...d...S.).r
-00000ec0: 3300 0000 7219 0000 0063 0100 0000 0000  3...r....c......
-00000ed0: 0000 0000 0000 0200 0000 0400 0000 3300  ..............3.
-00000ee0: 0000 7234 0000 0072 0e00 0000 7235 0000  ..r4...r....r5..
-00000ef0: 0072 3700 0000 723a 0000 0072 1600 0000  .r7...r:...r....
-00000f00: 7217 0000 0072 3c00 0000 6900 0000 723d  r....r<...i...r=
-00000f10: 0000 007a 2248 6578 426c 6f63 6b2e 666f  ...z"HexBlock.fo
-00000f20: 726d 6174 2e3c 6c6f 6361 6c73 3e2e 3c67  rmat.<locals>.<g
-00000f30: 656e 6578 7072 3e7a 0568 6578 2028 7a02  enexpr>z.hex (z.
-00000f40: 2920 7240 0000 0072 0100 0000 da01 6472  ) r@...r......dr
-00000f50: 0600 0000 7204 0000 007a 0520 202f 2f20  ....r....z.  // 
-00000f60: 7241 0000 0029 0672 1d00 0000 7232 0000  rA...).r....r2..
-00000f70: 0072 1200 0000 7244 0000 0072 4500 0000  .r....rD...rE...
-00000f80: 7220 0000 0072 4200 0000 7216 0000 0072  r ...rB...r....r
-00000f90: 3a00 0000 7217 0000 0072 2000 0000 6500  :...r....r ...e.
-00000fa0: 0000 7320 0000 001a 040c 0110 020a 0104  ..s ............
-00000fb0: ff0a 0104 ff0a 0104 ff08 0204 fe04 0204  ................
-00000fc0: fe02 0206 fe02 ff7a 0f48 6578 426c 6f63  .......z.HexBloc
-00000fd0: 6b2e 666f 726d 6174 4e63 0300 0000 0000  k.formatNc......
-00000fe0: 0000 0000 0000 0700 0000 0500 0000 0300  ................
-00000ff0: 0000 73d4 0000 0069 0064 0164 0293 0164  ..s....i.d.d...d
-00001000: 0364 0293 0164 0464 0293 0164 0564 0693  .d...d.d...d.d..
-00001010: 0164 0764 0693 0164 0864 0693 0164 0964  .d.d...d.d...d.d
-00001020: 0a93 0164 0b64 0a93 0164 0c64 0a93 0164  ...d.d...d.d...d
-00001030: 0d64 0e93 0164 0f64 0e93 0164 1064 0e93  .d...d.d...d.d..
-00001040: 0164 1164 1293 0164 1364 1293 0164 1464  .d.d...d.d...d.d
-00001050: 1293 0164 1564 1293 0164 1664 1793 0164  ...d.d...d.d...d
-00001060: 1764 1764 1764 189c 03a5 017d 0367 0064  .d.d.d.....}.g.d
-00001070: 19a2 017d 0467 0064 1aa2 017d 0574 007c  ...}.g.d...}.t.|
-00001080: 0174 0183 0272 4c7c 037c 0119 007d 0174  .t...rL|.|...}.t
-00001090: 0287 0066 0164 1b64 1c84 087c 047c 0119  ...f.d.d...|.|..
-000010a0: 0044 0083 0183 017d 067c 0264 1d75 0072  .D.....}.|.d.u.r
-000010b0: 657c 057c 0119 00a0 0388 006a 04a1 017d  e|.|.......j...}
-000010c0: 0274 057c 067c 0283 0253 0029 1e61 0c02  .t.|.|...S.).a..
-000010d0: 0000 4765 6e65 7261 7465 2046 6163 6520  ..Generate Face 
-000010e0: 6f62 6a65 6374 0a20 2020 2020 2020 2069  object.        i
-000010f0: 6e64 6578 2069 7320 6e75 6d62 6572 206f  ndex is number o
-00001100: 7220 6b65 7977 6f72 6420 746f 2069 6465  r keyword to ide
-00001110: 6e74 6966 7920 7468 6520 6661 6365 206f  ntify the face o
-00001120: 6620 4865 780a 2020 2020 2020 2020 2020  f Hex.          
-00001130: 2020 3020 3d20 2777 2720 3d20 2778 6d27    0 = 'w' = 'xm'
-00001140: 203d 2027 2d31 3030 2720 3d20 2830 2034   = '-100' = (0 4
-00001150: 2037 2033 290a 2020 2020 2020 2020 2020   7 3).          
-00001160: 2020 3120 3d20 2765 2720 3d20 2778 7027    1 = 'e' = 'xp'
-00001170: 203d 2027 3130 3027 203d 2028 3120 3220   = '100' = (1 2 
-00001180: 3520 3629 0a20 2020 2020 2020 2020 2020  5 6).           
-00001190: 2032 203d 2027 7327 203d 2027 796d 2720   2 = 's' = 'ym' 
-000011a0: 3d20 2730 2d31 3027 203d 2028 3020 3120  = '0-10' = (0 1 
-000011b0: 3520 3429 0a20 2020 2020 2020 2020 2020  5 4).           
-000011c0: 2033 203d 2027 6e27 203d 2027 7970 2720   3 = 'n' = 'yp' 
-000011d0: 3d20 2730 3130 2720 3d20 2832 2033 2037  = '010' = (2 3 7
-000011e0: 2036 290a 2020 2020 2020 2020 2020 2020   6).            
-000011f0: 3420 3d20 2762 2720 3d20 277a 6d27 203d  4 = 'b' = 'zm' =
-00001200: 2027 3030 2d31 2720 3d20 2830 2033 2032   '00-1' = (0 3 2
-00001210: 2031 2920 3d20 2262 6f74 746f 6d22 0a20   1) = "bottom". 
-00001220: 2020 2020 2020 2020 2020 2035 203d 2027             5 = '
-00001230: 7427 203d 2027 7a70 2720 3d20 2730 3031  t' = 'zp' = '001
-00001240: 2720 3d20 2834 2035 2036 2037 2920 3d20  ' = (4 5 6 7) = 
-00001250: 2274 6f70 220a 2020 2020 2020 2020 6e61  "top".        na
-00001260: 6d65 2069 7320 6769 7665 6e20 746f 2046  me is given to F
-00001270: 6163 6520 696e 7374 616e 6365 2e20 4966  ace instance. If
-00001280: 206f 6d69 7474 6564 2c20 6e61 6d65 2069   omitted, name i
-00001290: 7320 6175 746f 6d61 7469 6361 6c6c 790a  s automatically.
-000012a0: 2020 2020 2020 2020 2020 2020 6765 6e61              gena
-000012b0: 7261 7469 6564 206c 696b 6520 2827 662d  ratied like ('f-
-000012c0: 2720 2b20 7365 6c66 2e6e 616d 6520 2b20  ' + self.name + 
-000012d0: 272d 7727 290a 2020 2020 2020 2020 da01  '-w').        ..
-000012e0: 7772 0100 0000 da02 786d 7a04 2d31 3030  wr......xmz.-100
-000012f0: da01 6572 0600 0000 da02 7870 da03 3130  ..er......xp..10
-00001300: 3072 3f00 0000 7204 0000 00da 0279 6d7a  0r?...r......ymz
-00001310: 0430 2d31 30da 016e e903 0000 00da 0279  .0-10..n.......y
-00001320: 705a 0330 3130 da01 62e9 0400 0000 da06  pZ.010..b.......
-00001330: 626f 7474 6f6d da02 7a6d 7a04 3030 2d31  bottom..zmz.00-1
-00001340: da01 74e9 0500 0000 2903 da03 746f 70da  ..t.....)...top.
-00001350: 027a 705a 0330 3031 2906 2904 7201 0000  .zpZ.001).).r...
-00001360: 0072 5100 0000 e907 0000 0072 4e00 0000  .rQ........rN...
-00001370: 2904 7206 0000 0072 0400 0000 e906 0000  ).r....r........
-00001380: 0072 5500 0000 2904 7201 0000 0072 0600  .rU...).r....r..
-00001390: 0000 7255 0000 0072 5100 0000 2904 7204  ..rU...rQ...).r.
-000013a0: 0000 0072 4e00 0000 7258 0000 0072 5900  ...rN...rX...rY.
-000013b0: 0000 2904 7201 0000 0072 4e00 0000 7204  ..).r....rN...r.
-000013c0: 0000 0072 0600 0000 2904 7251 0000 0072  ...r....).rQ...r
-000013d0: 5500 0000 7259 0000 0072 5800 0000 2906  U...rY...rX...).
-000013e0: 7a06 662d 7b7d 2d77 fa06 662d 7b7d 2d6e  z.f-{}-w..f-{}-n
-000013f0: 7a06 662d 7b7d 2d73 725a 0000 007a 0666  z.f-{}-srZ...z.f
-00001400: 2d7b 7d2d 627a 0666 2d7b 7d2d 7463 0100  -{}-bz.f-{}-tc..
-00001410: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001420: 0000 1300 0000 7316 0000 0067 007c 005d  ......s....g.|.]
-00001430: 077d 0188 006a 007c 0119 0091 0271 0253  .}...j.|.....q.S
-00001440: 0072 1600 0000 2901 7232 0000 0029 0272  .r....).r2...).r
-00001450: 3800 0000 da01 6972 2800 0000 7216 0000  8.....ir(...r...
-00001460: 0072 1700 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00001470: 703e a700 0000 7302 0000 0016 007a 2148  p>....s......z!H
-00001480: 6578 426c 6f63 6b2e 6661 6365 2e3c 6c6f  exBlock.face.<lo
-00001490: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000014a0: 4e29 06da 0a69 7369 6e73 7461 6e63 6572  N)...isinstancer
-000014b0: 3600 0000 da05 7475 706c 6572 2000 0000  6.....tupler ...
-000014c0: 7212 0000 0072 3100 0000 2907 7215 0000  r....r1...).r...
-000014d0: 0072 1400 0000 7212 0000 005a 0b6b 775f  .r....r....Z.kw_
-000014e0: 746f 5f69 6e64 6578 5a0f 696e 6465 785f  to_indexZ.index_
-000014f0: 746f 5f76 6572 7465 785a 1669 6e64 6578  to_vertexZ.index
-00001500: 5f74 6f5f 6465 6661 756c 7473 7566 6669  _to_defaultsuffi
-00001510: 7872 3200 0000 7216 0000 0072 2800 0000  xr2...r....r(...
-00001520: 7217 0000 00da 0466 6163 6571 0000 0073  r......faceq...s
-00001530: 5e00 0000 020c 0401 02ff 0402 02fe 0403  ^...............
-00001540: 02fd 0404 02fc 0405 02fb 0406 02fa 0407  ................
-00001550: 02f9 0408 02f8 0409 02f7 040a 02f6 040b  ................
-00001560: 02f5 040c 02f4 040d 02f3 040e 02f2 040f  ................
-00001570: 02f1 0410 02f0 0411 02ef 0212 0201 0201  ................
-00001580: 08ec 0816 0808 0a09 0801 1a02 0801 1001  ................
-00001590: 0a01 7a0d 4865 7842 6c6f 636b 2e66 6163  ..z.HexBlock.fac
-000015a0: 6572 0e00 0000 2907 722a 0000 0072 2b00  er....).r*...r+.
-000015b0: 0000 722c 0000 0072 0b00 0000 7218 0000  ..r,...r....r...
-000015c0: 0072 2000 0000 725f 0000 0072 1600 0000  .r ...r_...r....
-000015d0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-000015e0: 4300 0000 5700 0000 7308 0000 0008 0014  C...W...s.......
-000015f0: 0108 0d0e 0c72 4300 0000 6300 0000 0000  .....rC...c.....
-00001600: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00001610: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
-00001620: 6408 6402 6403 8401 5a03 6404 6405 8400  d.d.d...Z.d.d...
-00001630: 5a04 6406 6407 8400 5a05 6401 5300 2909  Z.d.d...Z.d.S.).
-00001640: da08 426f 756e 6461 7279 4e63 0500 0000  ..BoundaryNc....
-00001650: 0000 0000 0000 0000 0500 0000 0300 0000  ................
-00001660: 4300 0000 733a 0000 007c 017c 005f 007c  C...s:...|.|._.|
-00001670: 027c 005f 017c 0364 0175 0072 0d67 007d  .|._.|.d.u.r.g.}
-00001680: 036e 0874 027c 0374 0383 0272 157c 0367  .n.t.|.t...r.|.g
-00001690: 017d 037c 037c 005f 047c 047c 005f 0564  .}.|.|._.|.|._.d
-000016a0: 0153 0029 027a c469 6e69 7469 616c 697a  .S.).z.initializ
-000016b0: 6520 626f 756e 6461 7279 0a20 2020 2020  e boundary.     
-000016c0: 2020 2074 7970 655f 2069 7320 7479 7065     type_ is type
-000016d0: 206b 6579 776f 7264 2028 7761 6c6c 2c20   keyword (wall, 
-000016e0: 7061 7463 682c 2065 6d70 7479 2c20 2e2e  patch, empty, ..
-000016f0: 290a 2020 2020 2020 2020 6e61 6d65 2069  ).        name i
-00001700: 7320 6e61 7665 206f 6620 626f 756e 6461  s nave of bounda
-00001710: 7279 2065 6d65 6c6d 656e 740a 2020 2020  ry emelment.    
-00001720: 2020 2020 6661 6365 7320 6973 2066 6163      faces is fac
-00001730: 6573 2077 6869 6368 2061 7265 2061 7070  es which are app
-00001740: 6c69 6564 2077 6974 6820 7468 6973 2062  lied with this b
-00001750: 6f75 6e64 6172 7920 636f 6e64 6974 696f  oundary conditio
-00001760: 6e73 0a20 2020 2020 2020 204e 2906 da05  ns.        N)...
-00001770: 7479 7065 5f72 1200 0000 725d 0000 0072  type_r....r]...r
-00001780: 3100 0000 da05 6661 6365 73da 096e 6569  1.....faces..nei
-00001790: 6768 626f 7572 2905 7215 0000 0072 6100  ghbour).r....ra.
-000017a0: 0000 7212 0000 0072 6200 0000 7263 0000  ..r....rb...rc..
-000017b0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-000017c0: 7218 0000 00ae 0000 0073 1000 0000 0606  r........s......
-000017d0: 0601 0801 0601 0a01 0601 0601 0a01 7a11  ..............z.
-000017e0: 426f 756e 6461 7279 2e5f 5f69 6e69 745f  Boundary.__init_
-000017f0: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
-00001800: 0000 0300 0000 4300 0000 7310 0000 007c  ......C...s....|
-00001810: 006a 00a0 017c 01a1 0101 0064 0153 0029  .j...|.....d.S.)
-00001820: 027a 5161 6464 2066 6163 6520 696e 7374  .zQadd face inst
-00001830: 616e 6365 0a20 2020 2020 2020 2066 6163  ance.        fac
-00001840: 6520 6973 2061 2046 6163 6520 696e 7374  e is a Face inst
-00001850: 616e 6365 2028 6e6f 7420 6e61 6d65 2920  ance (not name) 
-00001860: 746f 2062 6520 6164 6465 640a 2020 2020  to be added.    
-00001870: 2020 2020 4e29 0272 6200 0000 da06 6170      N).rb.....ap
-00001880: 7065 6e64 2902 7215 0000 0072 5f00 0000  pend).r....r_...
-00001890: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-000018a0: 0861 6464 5f66 6163 65bd 0000 0073 0200  .add_face....s..
-000018b0: 0000 1004 7a11 426f 756e 6461 7279 2e61  ....z.Boundary.a
-000018c0: 6464 5f66 6163 6563 0200 0000 0000 0000  dd_facec........
-000018d0: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
-000018e0: 7382 0000 007c 006a 0067 017d 027c 006a  s....|.j.g.}.|.j
-000018f0: 0164 0175 0072 167c 02a0 0264 0264 037c  .d.u.r.|...d.d.|
-00001900: 006a 039b 0064 049d 0317 00a1 0101 006e  .j...d.........n
-00001910: 107c 02a0 0264 0264 037c 006a 039b 0064  .|...d.d.|.j...d
-00001920: 057c 006a 019b 0064 049d 0517 00a1 0101  .|.j...d........
-00001930: 007c 006a 0444 005d 0d7d 037c 02a0 0264  .|.j.D.].}.|...d
-00001940: 067c 03a0 057c 01a1 019b 009d 02a1 0101  .|...|..........
-00001950: 0071 297c 02a0 0264 07a1 0101 0064 08a0  .q)|...d.....d..
-00001960: 067c 02a1 0153 0029 0972 3300 0000 4e7a  .|...S.).r3...Nz
-00001970: 027b 0a7a 0920 2020 2074 7970 6520 7a11  .{.z.    type z.
-00001980: 3b0a 2020 2020 6661 6365 730a 2020 2020  ;.    faces.    
-00001990: 287a 163b 0a20 2020 206e 6569 6768 626f  (z.;.    neighbo
-000019a0: 7572 5061 7463 6820 207a 0820 2020 2020  urPatch  z.     
-000019b0: 2020 207a 0820 2020 2029 3b0a 7dda 010a     z.    );.}...
-000019c0: 2907 7212 0000 0072 6300 0000 7264 0000  ).r....rc...rd..
-000019d0: 0072 6100 0000 7262 0000 0072 2000 0000  .ra...rb...r ...
-000019e0: 721d 0000 0029 0472 1500 0000 723b 0000  r....).r....r;..
-000019f0: 00da 0374 6d70 da01 6672 1600 0000 7216  ...tmp..fr....r.
-00001a00: 0000 0072 1700 0000 7220 0000 00c3 0000  ...r....r ......
-00001a10: 0073 1800 0000 0804 0a01 1a01 0402 0201  .s..............
-00001a20: 1401 02ff 04ff 0a04 1801 0a01 0a01 7a0f  ..............z.
-00001a30: 426f 756e 6461 7279 2e66 6f72 6d61 74a9  Boundary.format.
-00001a40: 024e 4e29 0672 2a00 0000 722b 0000 0072  .NN).r*...r+...r
-00001a50: 2c00 0000 7218 0000 0072 6500 0000 7220  ,...r....re...r 
-00001a60: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
-00001a70: 0000 7217 0000 0072 6000 0000 ad00 0000  ..r....r`.......
-00001a80: 7308 0000 0008 000a 0108 0f0c 0672 6000  s............r`.
-00001a90: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001aa0: 0000 0004 0000 0040 0000 0073 bc00 0000  .......@...s....
-00001ab0: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
-00001ac0: 6403 6404 8400 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
-00001ad0: 642a 6408 6409 8401 5a06 640a 640b 8400  d*d.d...Z.d.d...
-00001ae0: 5a07 640c 640d 8400 5a08 640e 640f 8400  Z.d.d...Z.d.d...
-00001af0: 5a09 650a 6410 6410 6410 8303 6601 6411  Z.e.d.d.d...f.d.
-00001b00: 6412 8401 5a0b 6413 6414 8400 5a0c 6415  d...Z.d.d...Z.d.
-00001b10: 6416 8400 5a0d 642b 6417 6418 8401 5a0e  d...Z.d+d.d...Z.
-00001b20: 6419 641a 8400 5a0f 642c 641c 641d 8401  d.d...Z.d,d.d...
-00001b30: 5a10 641e 641f 8400 5a11 6420 6421 8400  Z.d.d...Z.d d!..
-00001b40: 5a12 6422 6423 8400 5a13 6424 6425 8400  Z.d"d#..Z.d$d%..
-00001b50: 5a14 6426 6427 8400 5a15 6516 641b 6602  Z.d&d'..Z.e.d.f.
-00001b60: 6428 6429 8401 5a17 6407 5300 292d da0d  d(d)..Z.d.S.)-..
-00001b70: 426c 6f63 6b4d 6573 6844 6963 7463 0100  BlockMeshDictc..
-00001b80: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00001b90: 0000 4300 0000 7328 0000 0064 017c 005f  ..C...s(...d.|._
-00001ba0: 0069 007c 005f 0169 007c 005f 0269 007c  .i.|._.i.|._.i.|
-00001bb0: 005f 0369 007c 005f 0464 007c 005f 0564  ._.i.|._.d.|._.d
-00001bc0: 0053 0029 024e 6700 0000 0000 00f0 3f29  .S.).Ng.......?)
-00001bd0: 06da 1163 6f6e 7665 7274 5f74 6f5f 6d65  ...convert_to_me
-00001be0: 7465 7273 723b 0000 00da 0662 6c6f 636b  tersr;.....block
-00001bf0: 73da 0565 6467 6573 da0a 626f 756e 6461  s..edges..bounda
-00001c00: 7269 6573 da16 5f76 6572 7469 6365 735f  ries.._vertices_
-00001c10: 696e 5f62 6c6f 636b 6d65 7368 7228 0000  in_blockmeshr(..
-00001c20: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00001c30: 7218 0000 00d6 0000 0073 0c00 0000 0601  r........s......
-00001c40: 0601 0601 0601 0601 0a01 7a16 426c 6f63  ..........z.Bloc
-00001c50: 6b4d 6573 6844 6963 742e 5f5f 696e 6974  kMeshDict.__init
-00001c60: 5f5f 6302 0000 0000 0000 0000 0000 0003  __c.............
-00001c70: 0000 0009 0000 0043 0000 0073 2400 0000  .......C...s$...
-00001c80: 6401 6402 6403 6404 6405 6406 6407 6407  d.d.d.d.d.d.d.d.
-00001c90: 6408 9c08 7d02 7c02 7c01 1900 7c00 5f00  d...}.|.|...|._.
-00001ca0: 6409 5300 290a 7a22 7365 7420 7365 6c66  d.S.).z"set self
-00001cb0: 2e63 6f6d 7665 7274 5f74 6f5f 6d65 7465  .comvert_to_mete
-00001cc0: 7273 2062 7920 776f 7264 69e8 0300 0072  rs by wordi....r
-00001cd0: 0600 0000 677b 14ae 47e1 7a84 3f67 fca9  ....g{..G.z.?g..
-00001ce0: f1d2 4d62 503f 678d edb5 a0f7 c6b0 3e67  ..MbP?g.......>g
-00001cf0: 95d6 26e8 0b2e 113e 67bb bdd7 d9df 7cdb  ..&....>g.....|.
-00001d00: 3d29 08da 026b 6dda 016d da02 636d da02  =)...km..m..cm..
-00001d10: 6d6d da02 756d da02 6e6d da01 415a 0841  mm..um..nm..AZ.A
-00001d20: 6e67 7374 726f 6d4e a901 726b 0000 0029  ngstromN..rk...)
-00001d30: 0372 1500 0000 da06 6d65 7472 6963 5a17  .r......metricZ.
-00001d40: 6d65 7472 6963 7379 6d5f 746f 5f63 6f6e  metricsym_to_con
-00001d50: 7665 7273 696f 6e72 1600 0000 7216 0000  versionr....r...
-00001d60: 0072 1700 0000 da0a 7365 745f 6d65 7472  .r......set_metr
-00001d70: 6963 de00 0000 7314 0000 0002 0302 0102  ic....s.........
-00001d80: 0102 0102 0102 0102 0102 0106 f80e 0a7a  ...............z
-00001d90: 1842 6c6f 636b 4d65 7368 4469 6374 2e73  .BlockMeshDict.s
-00001da0: 6574 5f6d 6574 7269 6363 0200 0000 0000  et_metricc......
-00001db0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00001dc0: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
-00001dd0: 0072 0e00 0000 7277 0000 0029 0272 1500  .r....rw...).r..
-00001de0: 0000 da05 7363 616c 6572 1600 0000 7216  ....scaler....r.
-00001df0: 0000 0072 1700 0000 da09 7365 745f 7363  ...r......set_sc
-00001e00: 616c 65ec 0000 0073 0200 0000 0a01 7a17  ale....s......z.
-00001e10: 426c 6f63 6b4d 6573 6844 6963 742e 7365  BlockMeshDict.se
-00001e20: 745f 7363 616c 654e 6305 0000 0000 0000  t_scaleNc.......
-00001e30: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
-00001e40: 0073 5800 0000 7400 7c01 7401 8302 721b  .sX...t.|.t...r.
-00001e50: 7402 6401 6402 8400 7c02 7c03 7c04 6603  t.d.d...|.|.|.f.
-00001e60: 4400 8301 8301 7215 7403 6403 8301 8201  D.....r.t.d.....
-00001e70: 7c01 7d05 7c05 6a04 7d04 6e07 7401 7c01  |.}.|.j.}.n.t.|.
-00001e80: 7c02 7c03 7c04 8304 7d05 7c05 7c00 6a05  |.|.|...}.|.|.j.
-00001e90: 7c04 3c00 7c00 6a05 7c04 1900 5300 2904  |.<.|.j.|...S.).
-00001ea0: 7ab2 6164 6420 7665 7274 6578 2062 7920  z.add vertex by 
-00001eb0: 636f 6f72 6469 6e61 7465 2061 6e64 2075  coordinate and u
-00001ec0: 6e69 7120 6e61 6d65 0a20 2020 2020 2020  niq name.       
-00001ed0: 2078 2079 207a 2069 7320 636f 6f72 6469   x y z is coordi
-00001ee0: 6e61 7465 7320 6f66 2076 6572 7465 780a  nates of vertex.
-00001ef0: 2020 2020 2020 2020 6e61 6d65 2069 7320          name is 
-00001f00: 756e 6971 206e 616d 6520 746f 2072 6566  uniq name to ref
-00001f10: 6572 2074 6865 2076 6572 7465 780a 2020  er the vertex.  
-00001f20: 2020 2020 2020 7265 7475 726e 7320 5665        returns Ve
-00001f30: 7274 6578 206f 626a 6563 7420 7768 6963  rtex object whic
-00001f40: 6920 6973 2061 6464 6564 2e0a 2020 2020  i is added..    
-00001f50: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-00001f60: 0002 0000 0003 0000 0073 0000 0073 1800  .........s...s..
-00001f70: 0000 8100 7c00 5d07 7d01 7c01 6400 7501  ....|.].}.|.d.u.
-00001f80: 5600 0100 7102 6400 5300 720e 0000 0072  V...q.d.S.r....r
-00001f90: 1600 0000 2902 7238 0000 00da 0361 7267  ....).r8.....arg
-00001fa0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00001fb0: 3c00 0000 f600 0000 7304 0000 0002 8016  <.......s.......
-00001fc0: 007a 2b42 6c6f 636b 4d65 7368 4469 6374  .z+BlockMeshDict
-00001fd0: 2e61 6464 5f76 6572 7465 782e 3c6c 6f63  .add_vertex.<loc
-00001fe0: 616c 733e 2e3c 6765 6e65 7870 723e 7a40  als>.<genexpr>z@
-00001ff0: 7820 6973 2061 2056 6572 7465 7820 616e  x is a Vertex an
-00002000: 6420 6061 6e79 2861 7267 2069 7320 6e6f  d `any(arg is no
-00002010: 7420 4e6f 6e65 2066 6f72 2061 7267 2069  t None for arg i
-00002020: 6e20 2879 2c20 7a2c 206e 616d 6529 2960  n (y, z, name))`
-00002030: 2906 725d 0000 0072 0d00 0000 da03 616e  ).r]...r......an
-00002040: 79da 0a56 616c 7565 4572 726f 7272 1200  y..ValueErrorr..
-00002050: 0000 723b 0000 0029 0672 1500 0000 720f  ..r;...).r....r.
-00002060: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-00002070: 0000 5a06 7665 7274 6578 7216 0000 0072  ..Z.vertexr....r
-00002080: 1600 0000 7217 0000 00da 0a61 6464 5f76  ....r......add_v
-00002090: 6572 7465 78ef 0000 0073 1400 0000 0a06  ertex....s......
-000020a0: 1801 0201 0201 04ff 0404 0801 0e02 0a01  ................
-000020b0: 0a01 7a18 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
-000020c0: 742e 6164 645f 7665 7274 6578 6302 0000  t.add_vertexc...
-000020d0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-000020e0: 0043 0000 0073 0c00 0000 7c00 6a00 7c01  .C...s....|.j.|.
-000020f0: 3d00 6401 5300 2902 7a1f 6465 6c20 6e61  =.d.S.).z.del na
-00002100: 6d65 206b 6579 2066 726f 6d20 7365 6c66  me key from self
-00002110: 2e76 6572 7469 6365 734e 723a 0000 0029  .verticesNr:...)
-00002120: 0272 1500 0000 7212 0000 0072 1600 0000  .r....r....r....
-00002130: 7216 0000 0072 1700 0000 da0a 6465 6c5f  r....r......del_
-00002140: 7665 7274 6578 0201 0000 7302 0000 000c  vertex....s.....
-00002150: 027a 1842 6c6f 636b 4d65 7368 4469 6374  .z.BlockMeshDict
-00002160: 2e64 656c 5f76 6572 7465 7863 0200 0000  .del_vertexc....
-00002170: 0000 0000 0000 0000 0600 0000 0400 0000  ................
-00002180: 4700 0000 733a 0000 007c 006a 007c 0119  G...s:...|.j.|..
-00002190: 007d 037c 0244 005d 137d 047c 006a 007c  .}.|.D.].}.|.j.|
-000021a0: 0419 007d 057c 036a 01a0 027c 056a 01a1  ...}.|.j...|.j..
-000021b0: 0101 007c 037c 006a 007c 043c 0071 0764  ...|.|.j.|.<.q.d
-000021c0: 0153 0029 027a e274 7265 6174 206e 616d  .S.).z.treat nam
-000021d0: 6531 2c20 6e61 6d65 322c 202e 2e2e 2061  e1, name2, ... a
-000021e0: 7320 7361 6d65 2070 6f69 6e74 2e0a 0a20  s same point... 
-000021f0: 2020 2020 2020 206e 616d 6532 2e61 6c69         name2.ali
-00002200: 6173 2c20 6e61 6d65 332e 616c 6961 732c  as, name3.alias,
-00002210: 202e 2e2e 2061 7265 206d 6572 6765 6420   ... are merged 
-00002220: 7769 7468 206e 616d 6531 2e61 6c69 6173  with name1.alias
-00002230: 0a20 2020 2020 2020 2074 6865 206b 6579  .        the key
-00002240: 206e 616d 6532 2c20 6e61 6d65 332c 202e   name2, name3, .
-00002250: 2e2e 2069 6e20 7365 6c66 2e76 6572 7469  .. in self.verti
-00002260: 6365 7320 6172 6520 6b65 7074 2061 6e64  ces are kept and
-00002270: 206d 6170 7065 6420 746f 0a20 2020 2020   mapped to.     
-00002280: 2020 2073 616d 6520 5665 7274 6578 2069     same Vertex i
-00002290: 6e73 7461 6e63 6520 6173 206e 616d 6531  nstance as name1
-000022a0: 0a20 2020 2020 2020 204e 2903 723b 0000  .        N).r;..
-000022b0: 0072 1300 0000 da06 7570 6461 7465 2906  .r......update).
-000022c0: 7215 0000 00da 056e 616d 6531 da05 6e61  r......name1..na
-000022d0: 6d65 73da 0176 724d 0000 0072 4700 0000  mes..vrM...rG...
-000022e0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-000022f0: 0d72 6564 7563 655f 7665 7274 6578 0601  .reduce_vertex..
-00002300: 0000 730c 0000 000a 0708 010a 010e 010c  ..s.............
-00002310: 0204 fc7a 1b42 6c6f 636b 4d65 7368 4469  ...z.BlockMeshDi
-00002320: 6374 2e72 6564 7563 655f 7665 7274 6578  ct.reduce_vertex
-00002330: 6301 0000 0000 0000 0000 0000 0007 0000  c...............
-00002340: 0005 0000 0043 0000 0073 7800 0000 7400  .....C...sx...t.
-00002350: 7401 7c00 6a02 a003 a100 8301 6401 6402  t.|.j.......d.d.
-00002360: 8400 6403 8d02 7d01 6700 7d02 7404 7c01  ..d...}.g.}.t.|.
-00002370: 6404 6402 8400 8302 4400 5d0b 5c02 7d03  d.d.....D.].\.}.
-00002380: 7d04 7c02 a005 7401 7c04 8301 a101 0100  }.|...t.|.......
-00002390: 7116 7c02 4400 5d15 7d05 7406 7c05 8301  q.|.D.].}.t.|...
-000023a0: 6405 6b02 722d 7124 6406 6407 8400 7c05  d.k.r-q$d.d...|.
-000023b0: 4400 8301 7d06 7c00 6a07 7c06 8e00 0100  D...}.|.j.|.....
-000023c0: 7124 6408 5300 2909 7a39 6361 6c6c 2072  q$d.S.).z9call r
-000023d0: 6564 7563 655f 7665 7274 6578 206f 6e20  educe_vertex on 
-000023e0: 616c 6c20 7665 7274 6963 6573 2077 6974  all vertices wit
-000023f0: 6820 6964 656e 7469 6361 6c20 7661 6c75  h identical valu
-00002400: 6573 2e63 0100 0000 0000 0000 0000 0000  es.c............
-00002410: 0100 0000 0300 0000 5300 0000 f30c 0000  ........S.......
-00002420: 0074 007c 0064 0119 0083 0153 00a9 024e  .t.|.d.....S...N
-00002430: 7206 0000 00a9 0172 2700 0000 a901 7284  r......r'.....r.
-00002440: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00002450: 0000 da08 3c6c 616d 6264 613e 1901 0000  ....<lambda>....
-00002460: f302 0000 000c 007a 2e42 6c6f 636b 4d65  .......z.BlockMe
-00002470: 7368 4469 6374 2e6d 6572 6765 5f76 6572  shDict.merge_ver
-00002480: 7469 6365 732e 3c6c 6f63 616c 733e 2e3c  tices.<locals>.<
-00002490: 6c61 6d62 6461 3e29 01da 036b 6579 6301  lambda>)...keyc.
-000024a0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-000024b0: 0000 0053 0000 0072 8600 0000 7287 0000  ...S...r....r...
-000024c0: 0072 8800 0000 7289 0000 0072 1600 0000  .r....r....r....
-000024d0: 7216 0000 0072 1700 0000 728a 0000 001c  r....r....r.....
-000024e0: 0100 0072 8b00 0000 7206 0000 0063 0100  ...r....r....c..
-000024f0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00002500: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
-00002510: 067d 017c 0164 0019 0091 0271 0253 0029  .}.|.d.....q.S.)
-00002520: 0172 0100 0000 7216 0000 0029 0272 3800  .r....r....).r8.
-00002530: 0000 7284 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00002540: 0072 1700 0000 725c 0000 0021 0100 0073  .r....r\...!...s
-00002550: 0200 0000 1400 7a30 426c 6f63 6b4d 6573  ......z0BlockMes
-00002560: 6844 6963 742e 6d65 7267 655f 7665 7274  hDict.merge_vert
-00002570: 6963 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  ices.<locals>.<l
-00002580: 6973 7463 6f6d 703e 4e29 0872 1e00 0000  istcomp>N).r....
-00002590: da04 6c69 7374 723b 0000 00da 0569 7465  ..listr;.....ite
-000025a0: 6d73 7202 0000 0072 6400 0000 721c 0000  msr....rd...r...
-000025b0: 0072 8500 0000 2907 7215 0000 005a 0f73  .r....).r....Z.s
-000025c0: 6f72 7465 645f 7665 7274 6963 6573 da06  orted_vertices..
-000025d0: 6772 6f75 7073 da01 6bda 0167 da05 6772  groups..k..g..gr
-000025e0: 6f75 7072 8300 0000 7216 0000 0072 1600  oupr....r....r..
-000025f0: 0000 7217 0000 00da 0e6d 6572 6765 5f76  ..r......merge_v
-00002600: 6572 7469 6365 7314 0100 0073 1800 0000  ertices....s....
-00002610: 0204 1201 06ff 0403 1601 1001 0801 0c01  ................
-00002620: 0201 0e01 0c01 04fc 7a1c 426c 6f63 6b4d  ........z.BlockM
-00002630: 6573 6844 6963 742e 6d65 7267 655f 7665  eshDict.merge_ve
-00002640: 7274 6963 6573 7206 0000 0063 0500 0000  rticesr....c....
-00002650: 0000 0000 0000 0000 0600 0000 0500 0000  ................
-00002660: 4300 0000 731c 0000 0074 007c 017c 027c  C...s....t.|.|.|
-00002670: 037c 0483 047d 057c 057c 006a 017c 033c  .|...}.|.|.j.|.<
-00002680: 007c 0553 0072 0e00 0000 2902 7243 0000  .|.S.r....).rC..
-00002690: 0072 6c00 0000 2906 7215 0000 0072 3200  .rl...).r....r2.
-000026a0: 0000 7244 0000 0072 1200 0000 7245 0000  ..rD...r....rE..
-000026b0: 0072 5000 0000 7216 0000 0072 1600 0000  .rP...r....r....
-000026c0: 7217 0000 00da 0c61 6464 5f68 6578 626c  r......add_hexbl
-000026d0: 6f63 6b24 0100 00f3 0600 0000 0e01 0a01  ock$............
-000026e0: 0401 7a1a 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
-000026f0: 742e 6164 645f 6865 7862 6c6f 636b 6304  t.add_hexblockc.
-00002700: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00002710: 0000 0043 0000 00f3 1a00 0000 7400 7c01  ...C........t.|.
-00002720: 7c02 7c03 8303 7d04 7c04 7c00 6a01 7c02  |.|...}.|.|.j.|.
-00002730: 3c00 7c04 5300 720e 0000 0029 0272 0700  <.|.S.r....).r..
-00002740: 0000 726d 0000 0029 0572 1500 0000 7232  ..rm...).r....r2
-00002750: 0000 0072 1200 0000 5a0c 696e 7465 725f  ...r....Z.inter_
-00002760: 7665 7274 6578 7249 0000 0072 1600 0000  vertexrI...r....
-00002770: 7216 0000 0072 1700 0000 da0b 6164 645f  r....r......add_
-00002780: 6172 6365 6467 6529 0100 00f3 0600 0000  arcedge)........
-00002790: 0c01 0a01 0401 7a19 426c 6f63 6b4d 6573  ......z.BlockMes
-000027a0: 6844 6963 742e 6164 645f 6172 6365 6467  hDict.add_arcedg
-000027b0: 6563 0400 0000 0000 0000 0000 0000 0500  ec..............
-000027c0: 0000 0400 0000 4300 0000 7296 0000 0072  ......C...r....r
-000027d0: 0e00 0000 2902 7208 0000 0072 6d00 0000  ....).r....rm...
-000027e0: 2905 7215 0000 0072 3200 0000 7212 0000  ).r....r2...r...
-000027f0: 00da 0670 6f69 6e74 7372 4900 0000 7216  ...pointsrI...r.
-00002800: 0000 0072 1600 0000 7217 0000 00da 0e61  ...r....r......a
-00002810: 6464 5f73 706c 696e 6565 6467 652e 0100  dd_splineedge...
-00002820: 0072 9800 0000 7a1c 426c 6f63 6b4d 6573  .r....z.BlockMes
-00002830: 6844 6963 742e 6164 645f 7370 6c69 6e65  hDict.add_spline
-00002840: 6564 6765 6305 0000 0000 0000 0000 0000  edgec...........
-00002850: 0006 0000 0005 0000 0043 0000 0073 1c00  .........C...s..
-00002860: 0000 7400 7c01 7c02 7c03 7c04 8304 7d05  ..t.|.|.|.|...}.
-00002870: 7c05 7c00 6a01 7c02 3c00 7c05 5300 720e  |.|.j.|.<.|.S.r.
-00002880: 0000 0029 0272 6000 0000 726e 0000 0029  ...).r`...rn...)
-00002890: 0672 1500 0000 7261 0000 0072 1200 0000  .r....ra...r....
-000028a0: 7262 0000 0072 6300 0000 7250 0000 0072  rb...rc...rP...r
-000028b0: 1600 0000 7216 0000 0072 1700 0000 da0c  ....r....r......
-000028c0: 6164 645f 626f 756e 6461 7279 3301 0000  add_boundary3...
-000028d0: 7295 0000 007a 1a42 6c6f 636b 4d65 7368  r....z.BlockMesh
-000028e0: 4469 6374 2e61 6464 5f62 6f75 6e64 6172  Dict.add_boundar
-000028f0: 7963 0500 0000 0000 0000 0000 0000 0700  yc..............
-00002900: 0000 0600 0000 4300 0000 732c 0000 007c  ......C...s,...|
-00002910: 006a 0064 017c 017c 037c 0264 028d 047d  .j.d.|.|.|.d...}
-00002920: 057c 006a 0064 017c 027c 047c 0164 028d  .|.j.d.|.|.|.d..
-00002930: 047d 067c 057c 0666 0253 0029 034e da06  .}.|.|.f.S.).N..
-00002940: 6379 636c 6963 2901 7263 0000 0029 0172  cyclic).rc...).r
-00002950: 9b00 0000 2907 7215 0000 005a 056e 616d  ....).r....Z.nam
-00002960: 6530 7282 0000 005a 0666 6163 6573 305a  e0r....Z.faces0Z
-00002970: 0666 6163 6573 31da 0262 30da 0262 3172  .faces1..b0..b1r
-00002980: 1600 0000 7216 0000 0072 1700 0000 da15  ....r....r......
-00002990: 6164 645f 6379 636c 6963 5f62 6f75 6e64  add_cyclic_bound
-000029a0: 6172 6965 7338 0100 0073 0600 0000 1201  aries8...s......
-000029b0: 1201 0801 7a23 426c 6f63 6b4d 6573 6844  ....z#BlockMeshD
-000029c0: 6963 742e 6164 645f 6379 636c 6963 5f62  ict.add_cyclic_b
-000029d0: 6f75 6e64 6172 6965 7354 6302 0000 0000  oundariesTc.....
-000029e0: 0000 0000 0000 0008 0000 0005 0000 0043  ...............C
-000029f0: 0000 0073 ba00 0000 7400 8300 7d02 6700  ...s....t...}.g.
-00002a00: 7c00 5f01 7c00 6a02 a003 a100 4400 5d1e  |._.|.j.....D.].
-00002a10: 7d03 7c03 6a04 4400 5d18 7d04 7c00 6a05  }.|.j.D.].}.|.j.
-00002a20: 7c04 1900 7d05 7c05 6a06 7c02 7601 7228  |...}.|.j.|.v.r(
-00002a30: 7c02 a007 7c05 6a06 a101 0100 7c00 6a01  |...|.j.....|.j.
-00002a40: a008 7c05 a101 0100 7110 710b 7c01 6401  ..|.....q.q.|.d.
-00002a50: 6b02 7246 6700 7c00 5f01 7c00 6a05 a009  k.rFg.|._.|.j...
-00002a60: a100 4400 5d0e 5c02 7d06 7d05 7c06 7c02  ..D.].\.}.}.|.|.
-00002a70: 7600 7244 7c00 6a01 a008 7c05 a101 0100  v.rD|.j...|.....
-00002a80: 7136 6e08 7c01 724e 740a 7c00 6a01 8301  q6n.|.rNt.|.j...
-00002a90: 7c00 5f01 740b 7c00 6a01 8301 4400 5d07  |._.t.|.j...D.].
-00002aa0: 5c02 7d07 7d05 7c07 7c05 5f0c 7153 6402  \.}.}.|.|._.qSd.
-00002ab0: 5300 2903 7ae3 312e 2063 7265 6174 6520  S.).z.1. create 
-00002ac0: 6c69 7374 206f 6620 5665 7274 6578 2077  list of Vertex w
-00002ad0: 6869 6368 2061 7265 2072 6566 6572 7265  hich are referre
-00002ae0: 6420 6279 2062 6c6f 636b 7320 6f6e 6c79  d by blocks only
-00002af0: 2e0a 2020 2020 2020 2020 322e 2073 6f72  ..        2. sor
-00002b00: 7420 7665 7274 6578 2061 6363 6f72 6469  t vertex accordi
-00002b10: 6e67 2074 6f20 2878 2c20 792c 207a 290a  ng to (x, y, z).
-00002b20: 2020 2020 2020 2020 332e 2061 7373 6967          3. assig
-00002b30: 6e20 7365 7175 656e 6365 206e 756d 6265  n sequence numbe
-00002b40: 7220 666f 7220 6561 6368 2056 6572 7465  r for each Verte
-00002b50: 780a 2020 2020 2020 2020 342e 2073 6f72  x.        4. sor
-00002b60: 7465 6420 6c69 7374 2069 7320 7361 7665  ted list is save
-00002b70: 6420 6173 2073 656c 662e 5f76 6572 7469  d as self._verti
-00002b80: 6365 735f 696e 5f62 6c6f 636b 6d65 7368  ces_in_blockmesh
-00002b90: 0a20 2020 2020 2020 205a 0861 735f 6164  .        Z.as_ad
-00002ba0: 6465 644e 290d da03 7365 7472 6f00 0000  dedN)...setro...
-00002bb0: 726c 0000 00da 0676 616c 7565 7372 3200  rl.....valuesr2.
-00002bc0: 0000 723b 0000 0072 1200 0000 da03 6164  ..r;...r......ad
-00002bd0: 6472 6400 0000 728e 0000 0072 1e00 0000  drd...r....r....
-00002be0: da09 656e 756d 6572 6174 6572 1400 0000  ..enumerater....
-00002bf0: 2908 7215 0000 00da 0473 6f72 745a 0b76  ).r......sortZ.v
-00002c00: 6e61 6d65 735f 6b65 7074 7250 0000 0072  names_keptrP...r
-00002c10: 4d00 0000 7284 0000 00da 0576 6e61 6d65  M...r......vname
-00002c20: 725b 0000 0072 1600 0000 7216 0000 0072  r[...r....r....r
-00002c30: 1700 0000 da0f 6173 7369 676e 5f76 6572  ......assign_ver
-00002c40: 7465 7869 643d 0100 0073 2c00 0000 0607  texid=...s,.....
-00002c50: 0601 0e01 0a01 0a01 0a01 0c01 0c01 0280  ................
-00002c60: 02fc 0805 0601 1201 0801 0c01 0280 02fe  ................
-00002c70: 0403 0c01 1201 0801 04ff 7a1d 426c 6f63  ..........z.Bloc
-00002c80: 6b4d 6573 6844 6963 742e 6173 7369 676e  kMeshDict.assign
-00002c90: 5f76 6572 7465 7869 6463 0100 0000 0000  _vertexidc......
-00002ca0: 0000 0000 0000 0300 0000 0600 0000 4300  ..............C.
-00002cb0: 0000 7338 0000 0064 0167 017d 017c 006a  ..s8...d.g.}.|.j
-00002cc0: 0044 005d 0b7d 027c 01a0 0164 027c 02a0  .D.].}.|...d.|..
-00002cd0: 02a1 0017 00a1 0101 0071 067c 01a0 0164  .........q.|...d
-00002ce0: 03a1 0101 0064 04a0 037c 01a1 0153 0029  .....d...|...S.)
-00002cf0: 057a ec66 6f72 6d61 7420 7665 7274 6963  .z.format vertic
-00002d00: 6573 2073 6563 7469 6f6e 2e0a 2020 2020  es section..    
-00002d10: 2020 2020 6173 7369 676e 5f76 6572 7465      assign_verte
-00002d20: 7869 6428 2920 7368 6f75 6c64 2062 6520  xid() should be 
-00002d30: 6361 6c6c 6564 2062 6566 6f72 6520 7468  called before th
-00002d40: 6973 206d 6574 686f 642c 2062 6563 6175  is method, becau
-00002d50: 7365 0a20 2020 2020 2020 2073 656c 662e  se.        self.
-00002d60: 5f76 6572 7469 6365 735f 696e 5f62 6c6f  _vertices_in_blo
-00002d70: 636b 6d65 7368 2073 686f 756c 6420 6265  ckmesh should be
-00002d80: 2061 7661 696c 6162 6c65 2061 6e64 0a20   available and. 
-00002d90: 2020 2020 2020 206d 656d 6265 7273 206f         members o
-00002da0: 6620 7365 6c66 2e5f 7665 7274 6963 6573  f self._vertices
-00002db0: 5f69 6e5f 626c 6f63 6b6d 6573 6820 7368  _in_blockmesh sh
-00002dc0: 6f75 6c64 2068 6176 6520 7661 6c69 6420  ould have valid 
-00002dd0: 696e 6465 782e 0a20 2020 2020 2020 207a  index..        z
-00002de0: 0a76 6572 7469 6365 730a 28fa 0420 2020  .vertices.(..   
-00002df0: 20fa 0229 3b72 6600 0000 2904 726f 0000   ..);rf...).ro..
-00002e00: 0072 6400 0000 7220 0000 0072 1d00 0000  .rd...r ...r....
-00002e10: 2903 7215 0000 0072 6700 0000 7284 0000  ).r....rg...r...
-00002e20: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00002e30: da17 666f 726d 6174 5f76 6572 7469 6365  ..format_vertice
-00002e40: 735f 7365 6374 696f 6e56 0100 0073 0a00  s_sectionV...s..
-00002e50: 0000 0606 0a01 1401 0a01 0a01 7a25 426c  ............z%Bl
-00002e60: 6f63 6b4d 6573 6844 6963 742e 666f 726d  ockMeshDict.form
-00002e70: 6174 5f76 6572 7469 6365 735f 7365 6374  at_vertices_sect
-00002e80: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
-00002e90: 0300 0000 0700 0000 4300 0000 f340 0000  ........C....@..
-00002ea0: 0064 0167 017d 017c 006a 00a0 01a1 0044  .d.g.}.|.j.....D
-00002eb0: 005d 0d7d 027c 01a0 0264 027c 02a0 037c  .].}.|...d.|...|
-00002ec0: 006a 04a1 0117 00a1 0101 0071 087c 01a0  .j.........q.|..
-00002ed0: 0264 03a1 0101 0064 04a0 057c 01a1 0153  .d.....d...|...S
-00002ee0: 0029 057a a266 6f72 6d61 7420 626c 6f63  .).z.format bloc
-00002ef0: 6b73 2073 6563 7469 6f6e 2e0a 2020 2020  ks section..    
-00002f00: 2020 2020 6173 7369 676e 5f76 6572 7465      assign_verte
-00002f10: 7869 6428 2920 7368 6f75 6c64 2062 6520  xid() should be 
-00002f20: 6361 6c6c 6564 2062 6566 6f72 6520 7468  called before th
-00002f30: 6973 206d 6574 686f 642c 2062 6563 6175  is method, becau
-00002f40: 7365 0a20 2020 2020 2020 2076 6572 7469  se.        verti
-00002f50: 6365 7320 7265 6665 7265 6420 6279 2062  ces refered by b
-00002f60: 6c6f 636b 7320 7368 6f75 6c64 2068 6176  locks should hav
-00002f70: 6520 7661 6c69 6420 696e 6465 782e 0a20  e valid index.. 
-00002f80: 2020 2020 2020 207a 0862 6c6f 636b 730a         z.blocks.
-00002f90: 2872 a700 0000 72a8 0000 0072 6600 0000  (r....r....rf...
-00002fa0: 2906 726c 0000 0072 a100 0000 7264 0000  ).rl...r....rd..
-00002fb0: 0072 2000 0000 723b 0000 0072 1d00 0000  .r ...r;...r....
-00002fc0: 2903 7215 0000 0072 6700 0000 7250 0000  ).r....rg...rP..
-00002fd0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00002fe0: da15 666f 726d 6174 5f62 6c6f 636b 735f  ..format_blocks_
-00002ff0: 7365 6374 696f 6e62 0100 0073 0a00 0000  sectionb...s....
-00003000: 0605 0e01 1801 0a01 0a01 7a23 426c 6f63  ..........z#Bloc
-00003010: 6b4d 6573 6844 6963 742e 666f 726d 6174  kMeshDict.format
-00003020: 5f62 6c6f 636b 735f 7365 6374 696f 6e63  _blocks_sectionc
-00003030: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00003040: 0700 0000 4300 0000 72aa 0000 0029 057a  ....C...r....).z
-00003050: a166 6f72 6d61 7420 6564 6765 7320 7365  .format edges se
-00003060: 6374 696f 6e2e 0a20 2020 2020 2020 2061  ction..        a
-00003070: 7373 6967 6e5f 7665 7274 6578 6964 2829  ssign_vertexid()
-00003080: 2073 686f 756c 6420 6265 2063 616c 6c65   should be calle
-00003090: 6420 6265 666f 7265 2074 6869 7320 6d65  d before this me
-000030a0: 7468 6f64 2c20 6265 6361 7573 650a 2020  thod, because.  
-000030b0: 2020 2020 2020 7665 7274 6963 6573 2072        vertices r
-000030c0: 6566 6572 6564 2062 7920 626c 6f63 6b73  efered by blocks
-000030d0: 2073 686f 756c 6420 6861 7665 2076 616c   should have val
-000030e0: 6964 2069 6e64 6578 2e0a 2020 2020 2020  id index..      
-000030f0: 2020 7a07 6564 6765 730a 2872 a700 0000    z.edges.(r....
-00003100: 72a8 0000 0072 6600 0000 2906 726d 0000  r....rf...).rm..
-00003110: 0072 a100 0000 7264 0000 0072 2000 0000  .r....rd...r ...
-00003120: 723b 0000 0072 1d00 0000 2903 7215 0000  r;...r....).r...
-00003130: 0072 6700 0000 7249 0000 0072 1600 0000  .rg...rI...r....
-00003140: 7216 0000 0072 1700 0000 da14 666f 726d  r....r......form
-00003150: 6174 5f65 6467 6573 5f73 6563 7469 6f6e  at_edges_section
-00003160: 6d01 0000 730a 0000 0006 060e 0118 010a  m...s...........
-00003170: 010a 017a 2242 6c6f 636b 4d65 7368 4469  ...z"BlockMeshDi
-00003180: 6374 2e66 6f72 6d61 745f 6564 6765 735f  ct.format_edges_
-00003190: 7365 6374 696f 6e63 0100 0000 0000 0000  sectionc........
-000031a0: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
-000031b0: 7354 0000 0064 0167 017d 017c 006a 00a0  sT...d.g.}.|.j..
-000031c0: 01a1 0044 005d 177d 0264 027d 037c 02a0  ...D.].}.d.}.|..
-000031d0: 027c 006a 03a1 01a0 0464 0364 037c 0317  .|.j.....d.d.|..
-000031e0: 00a1 027d 047c 01a0 057c 037c 0417 00a1  ...}.|...|.|....
-000031f0: 0101 0071 087c 01a0 0564 04a1 0101 0064  ...q.|...d.....d
-00003200: 03a0 067c 01a1 0153 0029 057a a366 6f72  ...|...S.).z.for
-00003210: 6d61 7420 626f 756e 6461 7279 2073 6563  mat boundary sec
-00003220: 7469 6f6e 2e0a 2020 2020 2020 2020 6173  tion..        as
-00003230: 7369 676e 5f76 6572 7465 7869 6428 2920  sign_vertexid() 
-00003240: 7368 6f75 6c64 2062 6520 6361 6c6c 6564  should be called
-00003250: 2062 6566 6f72 6520 7468 6973 206d 6574   before this met
-00003260: 686f 642c 2062 6563 6175 7365 0a20 2020  hod, because.   
-00003270: 2020 2020 2076 6572 7469 6365 7320 7265       vertices re
-00003280: 6665 7265 6420 6279 2066 6163 6573 2073  fered by faces s
-00003290: 686f 756c 6420 6861 7665 2076 616c 6964  hould have valid
-000032a0: 2069 6e64 6578 2e0a 2020 2020 2020 2020   index..        
-000032b0: 7a0a 626f 756e 6461 7279 0a28 72a7 0000  z.boundary.(r...
-000032c0: 0072 6600 0000 72a8 0000 0029 0772 6e00  .rf...r....).rn.
-000032d0: 0000 72a1 0000 0072 2000 0000 723b 0000  ..r....r ...r;..
-000032e0: 00da 0772 6570 6c61 6365 7264 0000 0072  ...replacerd...r
-000032f0: 1d00 0000 2905 7215 0000 0072 6700 0000  ....).r....rg...
-00003300: 7250 0000 00da 0669 6e64 656e 7472 3f00  rP.....indentr?.
-00003310: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00003320: 00da 1766 6f72 6d61 745f 626f 756e 6461  ...format_bounda
-00003330: 7279 5f73 6563 7469 6f6e 7901 0000 730e  ry_sectiony...s.
-00003340: 0000 0006 060e 0104 0218 0110 010a 010a  ................
-00003350: 017a 2542 6c6f 636b 4d65 7368 4469 6374  .z%BlockMeshDict
-00003360: 2e66 6f72 6d61 745f 626f 756e 6461 7279  .format_boundary
-00003370: 5f73 6563 7469 6f6e 6301 0000 0000 0000  _sectionc.......
-00003380: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00003390: 0073 0400 0000 6401 5300 2902 4e7a 146d  .s....d.S.).Nz.m
-000033a0: 6572 6765 5061 7463 6850 6169 7273 0a28  ergePatchPairs.(
-000033b0: 0a29 3b72 1600 0000 7228 0000 0072 1600  .);r....r(...r..
-000033c0: 0000 7216 0000 0072 1700 0000 da1e 666f  ..r....r......fo
-000033d0: 726d 6174 5f6d 6572 6765 7061 7463 6870  rmat_mergepatchp
-000033e0: 6169 7273 5f73 6563 7469 6f6e 8801 0000  airs_section....
-000033f0: 7302 0000 0004 017a 2c42 6c6f 636b 4d65  s......z,BlockMe
-00003400: 7368 4469 6374 2e66 6f72 6d61 745f 6d65  shDict.format_me
-00003410: 7267 6570 6174 6368 7061 6972 735f 7365  rgepatchpairs_se
-00003420: 6374 696f 6e63 0300 0000 0000 0000 0000  ctionc..........
-00003430: 0000 0400 0000 0900 0000 4300 0000 7346  ..........C...sF
-00003440: 0000 007c 006a 007c 0264 018d 0101 0074  ...|.j.|.d.....t
-00003450: 0164 0283 017d 037c 036a 027c 0174 037c  .d...}.|.j.|.t.|
-00003460: 006a 0483 017c 00a0 05a1 007c 00a0 06a1  .j...|.....|....
-00003470: 007c 00a0 07a1 007c 00a0 08a1 007c 00a0  .|.....|.....|..
-00003480: 09a1 0064 038d 0753 0029 044e 2901 72a4  ...d...S.).N).r.
-00003490: 0000 0061 6f01 0000 2468 6561 6465 720a  ...ao...$header.
-000034a0: 466f 616d 4669 6c65 0a7b 0a20 2020 2076  FoamFile.{.    v
-000034b0: 6572 7369 6f6e 2020 2020 2032 2e30 3b0a  ersion     2.0;.
-000034c0: 2020 2020 666f 726d 6174 2020 2020 2020      format      
-000034d0: 6173 6369 693b 0a20 2020 2063 6c61 7373  ascii;.    class
-000034e0: 2020 2020 2020 2064 6963 7469 6f6e 6172         dictionar
-000034f0: 793b 0a20 2020 206f 626a 6563 7420 2020  y;.    object   
-00003500: 2020 2062 6c6f 636b 4d65 7368 4469 6374     blockMeshDict
-00003510: 3b0a 7d0a 2f2f 202a 202a 202a 202a 202a  ;.}.// * * * * *
-00003520: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-00003530: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-00003540: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-00003550: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-00003560: 202f 2f0a 0a73 6361 6c65 2020 2024 6d65   //..scale   $me
-00003570: 7472 6963 636f 6e76 6572 743b 0a0a 2476  tricconvert;..$v
-00003580: 6572 7469 6365 730a 0a24 626c 6f63 6b73  ertices..$blocks
-00003590: 0a0a 2465 6467 6573 0a0a 2462 6f75 6e64  ..$edges..$bound
-000035a0: 6172 790a 0a24 6d65 7267 6570 6174 6368  ary..$mergepatch
-000035b0: 7061 6972 730a 0a2f 2f20 2a2a 2a2a 2a2a  pairs..// ******
-000035c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-000035d0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-000035e0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-000035f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00003600: 2a2a 2a20 2f2f 0a29 07da 0668 6561 6465  *** //.)...heade
-00003610: 725a 0d6d 6574 7269 6363 6f6e 7665 7274  rZ.metricconvert
-00003620: 723b 0000 0072 6d00 0000 726c 0000 00da  r;...rm...rl....
-00003630: 0862 6f75 6e64 6172 795a 0f6d 6572 6765  .boundaryZ.merge
-00003640: 7061 7463 6870 6169 7273 290a 72a6 0000  patchpairs).r...
-00003650: 0072 0300 0000 da0a 7375 6273 7469 7475  .r......substitu
-00003660: 7465 7236 0000 0072 6b00 0000 72a9 0000  ter6...rk...r...
-00003670: 0072 ac00 0000 72ab 0000 0072 af00 0000  .r....r....r....
-00003680: 72b0 0000 0029 0472 1500 0000 72b1 0000  r....).r....r...
-00003690: 005a 0d73 6f72 745f 766f 7274 6963 6573  .Z.sort_vortices
-000036a0: da08 7465 6d70 6c61 7465 7216 0000 0072  ..templater....r
-000036b0: 1600 0000 7217 0000 0072 2000 0000 8e01  ....r....r .....
-000036c0: 0000 731a 0000 000c 0102 0102 0104 ff04  ..s.............
-000036d0: 1b02 0108 0106 0106 0106 0106 0106 0106  ................
-000036e0: f97a 1442 6c6f 636b 4d65 7368 4469 6374  .z.BlockMeshDict
-000036f0: 2e66 6f72 6d61 7429 034e 4e4e 7269 0000  .format).NNNri..
-00003700: 0029 0154 2918 722a 0000 0072 2b00 0000  .).T).r*...r+...
-00003710: 722c 0000 0072 1800 0000 7279 0000 0072  r,...r....ry...r
-00003720: 7b00 0000 727f 0000 0072 8000 0000 7285  {...r....r....r.
-00003730: 0000 0072 9300 0000 720b 0000 0072 9400  ...r....r....r..
-00003740: 0000 7297 0000 0072 9a00 0000 729b 0000  ..r....r....r...
-00003750: 0072 9f00 0000 72a6 0000 0072 a900 0000  .r....r....r....
-00003760: 72ab 0000 0072 ac00 0000 72af 0000 0072  r....r....r....r
-00003770: b000 0000 7205 0000 0072 2000 0000 7216  ....r....r ...r.
-00003780: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00003790: 0000 726a 0000 00d5 0000 0073 2800 0000  ..rj.......s(...
-000037a0: 0800 0801 0808 080e 0a03 0813 0804 080e  ................
-000037b0: 1410 0805 0805 0a05 0805 0a05 0819 080c  ................
-000037c0: 080b 080c 080f 1206 726a 0000 004e 2916  ........rj...N).
-000037d0: da07 5f5f 646f 635f 5fda 0969 7465 7274  ..__doc__..itert
-000037e0: 6f6f 6c73 7202 0000 00da 0673 7472 696e  oolsr......strin
-000037f0: 6772 0300 0000 da00 7205 0000 0072 6d00  gr......r....rm.
-00003800: 0000 7207 0000 0072 0800 0000 7245 0000  ..r....r....rE..
-00003810: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00003820: 720c 0000 00da 075f 5f61 6c6c 5f5f 720d  r......__all__r.
-00003830: 0000 0072 2e00 0000 7231 0000 0072 4300  ...r....r1...rC.
-00003840: 0000 7260 0000 0072 6a00 0000 7216 0000  ..r`...rj...r...
-00003850: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00003860: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
-00003870: 0000 0004 000c 0c0c 010c 0210 0118 0108  ................
-00003880: 020e 0a0e 1e0e 0a0e 110e 5612 28         ..........V.(
+000000d0: 6415 8400 6415 8302 5a15 4700 6416 6417  d...d...Z.G.d.d.
+000000e0: 8400 6417 6515 8303 5a16 6418 5300 2919  ..d.e...Z.d.S.).
+000000f0: 6120 0100 0048 656c 7065 7220 746f 2063  a ...Helper to c
+00000100: 7265 6174 6520 626c 6f63 6b4d 6573 6844  reate blockMeshD
+00000110: 6963 7420 6669 6c65 730a 0a54 616b 656e  ict files..Taken
+00000120: 2066 726f 6d20 6874 7470 733a 2f2f 6769   from https://gi
+00000130: 7468 7562 2e63 6f6d 2f74 616b 6161 6b69  thub.com/takaaki
+00000140: 616f 6b69 2f6f 6662 6c6f 636b 6d65 7368  aoki/ofblockmesh
+00000150: 6469 6374 6865 6c70 6572 2028 4769 7420  dicthelper (Git 
+00000160: 636f 6d6d 6974 0a35 3835 3839 6631 2920  commit.58589f1) 
+00000170: 616e 6420 6d6f 6469 6669 6564 2061 7320  and modified as 
+00000180: 666f 6c6c 6f77 3a0a 0a2d 2060 6070 7975  follow:..- ``pyu
+00000190: 7067 7261 6465 205f 5f69 6e69 745f 5f2e  pgrade __init__.
+000001a0: 7079 202d 2d70 7933 392d 706c 7573 6060  py --py39-plus``
+000001b0: 0a2d 2074 6573 7465 6420 2831 3030 2520  .- tested (100% 
+000001c0: 636f 7665 7261 6765 2920 616e 6420 7265  coverage) and re
+000001d0: 7072 6f64 7563 6962 6c65 2028 7365 7473  producible (sets
+000001e0: 2073 6f72 7465 6429 0a2d 2072 6566 6163   sorted).- refac
+000001f0: 746f 720a 2d20 7375 7070 6f72 7420 666f  tor.- support fo
+00000200: 7220 6379 636c 6963 2062 6f75 6e64 6172  r cyclic boundar
+00000210: 6965 730a 0ae9 0000 0000 2901 da07 6772  ies.......)...gr
+00000220: 6f75 7062 7929 01da 0854 656d 706c 6174  oupby)...Templat
+00000230: 65e9 0200 0000 2901 da0e 4445 4641 554c  e.....)...DEFAUL
+00000240: 545f 4845 4144 4552 e901 0000 0029 02da  T_HEADER.....)..
+00000250: 0741 7263 4564 6765 da0a 5370 6c69 6e65  .ArcEdge..Spline
+00000260: 4564 6765 2904 da0b 4564 6765 4772 6164  Edge)...EdgeGrad
+00000270: 696e 67da 0747 7261 6469 6e67 da0d 5369  ing..Grading..Si
+00000280: 6d70 6c65 4772 6164 696e 67da 1453 696d  mpleGrading..Sim
+00000290: 706c 6547 7261 6469 6e67 456c 656d 656e  pleGradingElemen
+000002a0: 7429 0672 0a00 0000 720c 0000 0072 0b00  t).r....r....r..
+000002b0: 0000 7209 0000 0072 0700 0000 7208 0000  ..r....r....r...
+000002c0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000002d0: 0000 0300 0000 4000 0000 7336 0000 0065  ......@...s6...e
+000002e0: 005a 0164 005a 0264 0c64 0264 0384 015a  .Z.d.Z.d.d.d...Z
+000002f0: 0364 0464 0584 005a 0464 0664 0784 005a  .d.d...Z.d.d...Z
+00000300: 0564 0864 0984 005a 0664 0a64 0b84 005a  .d.d...Z.d.d...Z
+00000310: 0764 0153 0029 0dda 0656 6572 7465 784e  .d.S.)...VertexN
+00000320: 6306 0000 0000 0000 0000 0000 0006 0000  c...............
+00000330: 0002 0000 0043 0000 0073 2a00 0000 7c01  .....C...s*...|.
+00000340: 7c00 5f00 7c02 7c00 5f01 7c03 7c00 5f02  |._.|.|._.|.|._.
+00000350: 7c04 7c00 5f03 7c04 6801 7c00 5f04 7c05  |.|._.|.h.|._.|.
+00000360: 7c00 5f05 6400 5300 a901 4e29 06da 0178  |._.d.S...N)...x
+00000370: da01 79da 017a da04 6e61 6d65 da05 616c  ..y..z..name..al
+00000380: 6961 73da 0569 6e64 6578 2906 da04 7365  ias..index)...se
+00000390: 6c66 720f 0000 0072 1000 0000 7211 0000  lfr....r....r...
+000003a0: 0072 1200 0000 7214 0000 00a9 0072 1600  .r....r......r..
+000003b0: 0000 fa55 2f68 6f6d 652f 7069 6572 7265  ...U/home/pierre
+000003c0: 2f44 6576 2f66 6c75 6964 7369 6d66 6f61  /Dev/fluidsimfoa
+000003d0: 6d2f 7372 632f 666c 7569 6473 696d 666f  m/src/fluidsimfo
+000003e0: 616d 2f66 6f61 6d5f 696e 7075 745f 6669  am/foam_input_fi
+000003f0: 6c65 732f 626c 6f63 6b6d 6573 682f 5f5f  les/blockmesh/__
+00000400: 696e 6974 5f5f 2e70 79da 085f 5f69 6e69  init__.py..__ini
+00000410: 745f 5f1f 0000 0073 0c00 0000 0601 0601  t__....s........
+00000420: 0601 0601 0801 0a04 7a0f 5665 7274 6578  ........z.Vertex
+00000430: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00000440: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
+00000450: 0000 7360 0000 007c 006a 009b 0064 017c  ..s`...|.j...d.|
+00000460: 006a 019b 009d 037d 0174 027c 006a 0383  .j.....}.t.|.j..
+00000470: 0164 026b 0472 1c7c 0164 0364 01a0 0474  .d.k.r.|.d.d...t
+00000480: 057c 006a 0383 01a1 0117 0037 007d 0164  .|.j.......7.}.d
+00000490: 047c 006a 0664 059b 0464 017c 006a 0764  .|.j.d...d.|.j.d
+000004a0: 059b 0464 017c 006a 0864 059b 0464 067c  ...d.|.j.d...d.|
+000004b0: 019b 009d 0853 0029 074e da01 2072 0600  .....S.).N.. r..
+000004c0: 0000 7a03 203a 20fa 0228 207a 0520 2e31  ..z. : ..( z. .1
+000004d0: 3567 7a07 2029 2020 2f2f 2029 0972 1400  5gz. )  // ).r..
+000004e0: 0000 7212 0000 00da 036c 656e 7213 0000  ..r......lenr...
+000004f0: 00da 046a 6f69 6eda 0673 6f72 7465 6472  ...join..sortedr
+00000500: 0f00 0000 7210 0000 0072 1100 0000 2902  ....r....r....).
+00000510: 7215 0000 00da 0763 6f6d 6d65 6e74 7216  r......commentr.
+00000520: 0000 0072 1600 0000 7217 0000 00da 0666  ...r....r......f
+00000530: 6f72 6d61 742a 0000 0073 0800 0000 1201  ormat*...s......
+00000540: 0e01 1801 2801 7a0d 5665 7274 6578 2e66  ....(.z.Vertex.f
+00000550: 6f72 6d61 7463 0200 0000 0000 0000 0000  ormatc..........
+00000560: 0000 0200 0000 0400 0000 4300 0000 7320  ..........C...s 
+00000570: 0000 007c 006a 007c 006a 017c 006a 0266  ...|.j.|.j.|.j.f
+00000580: 037c 016a 007c 016a 017c 016a 0266 036b  .|.j.|.j.|.j.f.k
+00000590: 0053 0072 0e00 0000 a903 7211 0000 0072  .S.r......r....r
+000005a0: 1000 0000 720f 0000 00a9 0272 1500 0000  ....r......r....
+000005b0: da03 7268 7372 1600 0000 7216 0000 0072  ..rhsr....r....r
+000005c0: 1700 0000 da06 5f5f 6c74 5f5f 3000 0000  ......__lt__0...
+000005d0: f302 0000 0020 017a 0d56 6572 7465 782e  ..... .z.Vertex.
+000005e0: 5f5f 6c74 5f5f 6302 0000 0000 0000 0000  __lt__c.........
+000005f0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000600: 2000 0000 7c00 6a00 7c00 6a01 7c00 6a02   ...|.j.|.j.|.j.
+00000610: 6603 7c01 6a00 7c01 6a01 7c01 6a02 6603  f.|.j.|.j.|.j.f.
+00000620: 6b02 5300 720e 0000 0072 2000 0000 7221  k.S.r....r ...r!
+00000630: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000640: 0000 da06 5f5f 6571 5f5f 3300 0000 7224  ....__eq__3...r$
+00000650: 0000 007a 0d56 6572 7465 782e 5f5f 6571  ...z.Vertex.__eq
+00000660: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00000670: 0000 0004 0000 0043 0000 0073 1400 0000  .......C...s....
+00000680: 7400 7c00 6a01 7c00 6a02 7c00 6a03 6603  t.|.j.|.j.|.j.f.
+00000690: 8301 5300 720e 0000 0029 04da 0468 6173  ..S.r....)...has
+000006a0: 6872 1100 0000 7210 0000 0072 0f00 0000  hr....r....r....
+000006b0: a901 7215 0000 0072 1600 0000 7216 0000  ..r....r....r...
+000006c0: 0072 1700 0000 da08 5f5f 6861 7368 5f5f  .r......__hash__
+000006d0: 3600 0000 7302 0000 0014 017a 0f56 6572  6...s......z.Ver
+000006e0: 7465 782e 5f5f 6861 7368 5f5f 720e 0000  tex.__hash__r...
+000006f0: 0029 08da 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
+00000700: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000710: 6c6e 616d 655f 5f72 1800 0000 721f 0000  lname__r....r...
+00000720: 0072 2300 0000 7225 0000 0072 2800 0000  .r#...r%...r(...
+00000730: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+00000740: 1700 0000 720d 0000 001e 0000 0073 0c00  ....r........s..
+00000750: 0000 0800 0a01 080b 0806 0803 0c03 720d  ..............r.
+00000760: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000770: 0000 0000 0200 0000 4000 0000 f31c 0000  ........@.......
+00000780: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00000790: 0364 0364 0484 005a 0464 0553 0029 06da  .d.d...Z.d.S.)..
+000007a0: 0550 6f69 6e74 6304 0000 0000 0000 0000  .Pointc.........
+000007b0: 0000 0004 0000 0002 0000 0043 0000 0073  ...........C...s
+000007c0: 1600 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
+000007d0: 7c03 7c00 5f02 6400 5300 720e 0000 00a9  |.|._.d.S.r.....
+000007e0: 0372 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+000007f0: 2904 7215 0000 0072 0f00 0000 7210 0000  ).r....r....r...
+00000800: 0072 1100 0000 7216 0000 0072 1600 0000  .r....r....r....
+00000810: 7217 0000 0072 1800 0000 3b00 0000 7306  r....r....;...s.
+00000820: 0000 0006 0106 010a 017a 0e50 6f69 6e74  .........z.Point
+00000830: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00000840: 0000 0000 0000 0100 0000 0700 0000 4300  ..............C.
+00000850: 0000 7324 0000 0064 017c 006a 0064 029b  ..s$...d.|.j.d..
+00000860: 0464 037c 006a 0164 029b 0464 037c 006a  .d.|.j.d...d.|.j
+00000870: 0264 029b 0464 049d 0753 0029 054e 721a  .d...d...S.).Nr.
+00000880: 0000 007a 0631 382e 3135 6772 1900 0000  ...z.18.15gr....
+00000890: 7a02 2029 722e 0000 0072 2700 0000 7216  z. )r....r'...r.
+000008a0: 0000 0072 1600 0000 7217 0000 0072 1f00  ...r....r....r..
+000008b0: 0000 4000 0000 7302 0000 0024 017a 0c50  ..@...s....$.z.P
+000008c0: 6f69 6e74 2e66 6f72 6d61 744e a905 7229  oint.formatN..r)
+000008d0: 0000 0072 2a00 0000 722b 0000 0072 1800  ...r*...r+...r..
+000008e0: 0000 721f 0000 0072 1600 0000 7216 0000  ..r....r....r...
+000008f0: 0072 1600 0000 7217 0000 0072 2d00 0000  .r....r....r-...
+00000900: 3a00 0000 7306 0000 0008 0008 010c 0572  :...s..........r
+00000910: 2d00 0000 6300 0000 0000 0000 0000 0000  -...c...........
+00000920: 0000 0000 0002 0000 0040 0000 0072 2c00  .........@...r,.
+00000930: 0000 2906 da04 4661 6365 6303 0000 0000  ..)...Facec.....
+00000940: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
+00000950: 0000 0073 1000 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
+00000960: 7c00 5f01 6401 5300 2902 7a38 0a20 2020  |._.d.S.).z8.   
+00000970: 2020 2020 2076 6e61 6d65 2069 7320 6c69       vname is li
+00000980: 7374 206f 7220 7475 706c 6520 6f66 2076  st or tuple of v
+00000990: 6572 7465 7820 6e61 6d65 730a 2020 2020  ertex names.    
+000009a0: 2020 2020 4e29 02da 0676 6e61 6d65 7372      N)...vnamesr
+000009b0: 1200 0000 2903 7215 0000 0072 3100 0000  ....).r....r1...
+000009c0: 7212 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+000009d0: 1700 0000 7218 0000 0045 0000 0073 0400  ....r....E...s..
+000009e0: 0000 0604 0a01 7a0d 4661 6365 2e5f 5f69  ......z.Face.__i
+000009f0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
+00000a00: 0000 0400 0000 0700 0000 0300 0000 7346  ..............sF
+00000a10: 0000 0064 01a0 0087 0066 0164 0264 0384  ...d.....f.d.d..
+00000a20: 087c 006a 0144 0083 01a1 017d 0264 01a0  .|.j.D.....}.d..
+00000a30: 007c 006a 01a1 017d 0364 047c 0264 059b  .|.j...}.d.|.d..
+00000a40: 0464 067c 006a 0264 059b 0464 077c 0364  .d.|.j.d...d.|.d
+00000a50: 059b 0464 089d 0753 0029 09fa 4b46 6f72  ...d...S.)..KFor
+00000a60: 6d61 7420 696e 7374 616e 6365 2074 6f20  mat instance to 
+00000a70: 6475 6d70 0a20 2020 2020 2020 2076 6572  dump.        ver
+00000a80: 7469 6365 7320 6973 2064 6963 7420 6f66  tices is dict of
+00000a90: 206e 616d 6520 746f 2056 6572 7465 780a   name to Vertex.
+00000aa0: 2020 2020 2020 2020 7219 0000 0063 0100          r....c..
+00000ab0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000ac0: 0000 3300 0000 f31e 0000 0081 007c 005d  ..3..........|.]
+00000ad0: 0a7d 0174 0088 007c 0119 006a 0183 0156  .}.t...|...j...V
+00000ae0: 0001 0071 0264 0053 0072 0e00 0000 a902  ...q.d.S.r......
+00000af0: da03 7374 7272 1400 0000 a902 da02 2e30  ..strr.........0
+00000b00: da02 766e a901 da08 7665 7274 6963 6573  ..vn....vertices
+00000b10: 7216 0000 0072 1700 0000 da09 3c67 656e  r....r......<gen
+00000b20: 6578 7072 3e50 0000 00f3 0400 0000 0280  expr>P..........
+00000b30: 1c00 7a1e 4661 6365 2e66 6f72 6d61 742e  ..z.Face.format.
+00000b40: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00000b50: 723e fa01 28da 0173 7a06 2920 202f 2f20  r>..(..sz.)  // 
+00000b60: fa02 2028 fa01 2929 0372 1c00 0000 7231  .. (..)).r....r1
+00000b70: 0000 0072 1200 0000 a904 7215 0000 0072  ...r......r....r
+00000b80: 3a00 0000 7214 0000 0072 1e00 0000 7216  :...r....r....r.
+00000b90: 0000 0072 3900 0000 7217 0000 0072 1f00  ...r9...r....r..
+00000ba0: 0000 4c00 0000 7306 0000 001a 040c 0120  ..L...s........ 
+00000bb0: 017a 0b46 6163 652e 666f 726d 6174 4e72  .z.Face.formatNr
+00000bc0: 2f00 0000 7216 0000 0072 1600 0000 7216  /...r....r....r.
+00000bd0: 0000 0072 1700 0000 7230 0000 0044 0000  ...r....r0...D..
+00000be0: 0073 0600 0000 0800 0801 0c07 7230 0000  .s..........r0..
+00000bf0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000c00: 0000 0400 0000 4000 0000 7332 0000 0065  ......@...s2...e
+00000c10: 005a 0164 005a 0265 0364 0164 0164 0183  .Z.d.Z.e.d.d.d..
+00000c20: 0366 0164 0264 0384 015a 0464 0464 0584  .f.d.d...Z.d.d..
+00000c30: 005a 0564 0964 0764 0884 015a 0664 0653  .Z.d.d.d...Z.d.S
+00000c40: 0029 0ada 0848 6578 426c 6f63 6b72 0600  .)...HexBlockr..
+00000c50: 0000 6305 0000 0000 0000 0000 0000 0005  ..c.............
+00000c60: 0000 0002 0000 0043 0000 0073 1c00 0000  .......C...s....
+00000c70: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
+00000c80: 5f02 7c04 7c00 5f03 6401 5300 2902 612e  _.|.|._.d.S.).a.
+00000c90: 0100 0049 6e69 7469 616c 697a 6520 4865  ...Initialize He
+00000ca0: 7842 6c6f 636b 2069 6e73 7461 6e63 650a  xBlock instance.
+00000cb0: 2020 2020 2020 2020 766e 616d 6573 2069          vnames i
+00000cc0: 7320 7468 6520 7665 7274 6578 206e 616d  s the vertex nam
+00000cd0: 6573 2069 6e20 6f72 6465 7220 6465 7363  es in order desc
+00000ce0: 7269 7665 6420 696e 0a20 2020 2020 2020  rived in.       
+00000cf0: 2020 2020 2068 7474 703a 2f2f 7777 772e       http://www.
+00000d00: 6f70 656e 666f 616d 2e6f 7267 2f64 6f63  openfoam.org/doc
+00000d10: 732f 7573 6572 2f6d 6573 682d 6465 7363  s/user/mesh-desc
+00000d20: 7269 7074 696f 6e2e 7068 700a 2020 2020  ription.php.    
+00000d30: 2020 2020 6365 6c6c 7320 6973 206e 756d      cells is num
+00000d40: 6265 7220 6f66 2063 656c 6c73 2064 6576  ber of cells dev
+00000d50: 6965 6420 696e 746f 2069 6e20 6561 6368  ied into in each
+00000d60: 2064 6972 6563 7469 6f6e 0a20 2020 2020   direction.     
+00000d70: 2020 206e 616d 6520 6973 2074 6865 2075     name is the u
+00000d80: 6e69 7120 6e61 6d65 206f 6620 7468 6520  niq name of the 
+00000d90: 626c 6f63 6b0a 2020 2020 2020 2020 6772  block.        gr
+00000da0: 6164 696e 6720 6973 2067 7261 6469 6e67  ading is grading
+00000db0: 206d 6574 686f 642e 0a20 2020 2020 2020   method..       
+00000dc0: 204e 2904 7231 0000 00da 0563 656c 6c73   N).r1.....cells
+00000dd0: 7212 0000 00da 0767 7261 6469 6e67 2905  r......grading).
+00000de0: 7215 0000 0072 3100 0000 7243 0000 0072  r....r1...rC...r
+00000df0: 1200 0000 7244 0000 0072 1600 0000 7216  ....rD...r....r.
+00000e00: 0000 0072 1700 0000 7218 0000 0056 0000  ...r....r....V..
+00000e10: 0073 0800 0000 0608 0601 0601 0a01 7a11  .s............z.
+00000e20: 4865 7842 6c6f 636b 2e5f 5f69 6e69 745f  HexBlock.__init_
+00000e30: 5f63 0200 0000 0000 0000 0000 0000 0400  _c..............
+00000e40: 0000 1100 0000 0300 0000 737e 0000 0064  ..........s~...d
+00000e50: 01a0 0087 0066 0164 0264 0384 087c 006a  .....f.d.d...|.j
+00000e60: 0144 0083 01a1 017d 0264 01a0 007c 006a  .D.....}.d...|.j
+00000e70: 01a1 017d 0364 047c 029b 0064 057c 006a  ...}.d.|...d.|.j
+00000e80: 029b 0064 067c 006a 0364 0719 0064 089b  ...d.|.j.d...d..
+00000e90: 0464 017c 006a 0364 0919 0064 089b 0464  .d.|.j.d...d...d
+00000ea0: 017c 006a 0364 0a19 0064 089b 0464 057c  .|.j.d...d...d.|
+00000eb0: 006a 04a0 05a1 009b 0064 0b7c 006a 029b  .j.......d.|.j..
+00000ec0: 0064 067c 039b 0064 0c9d 1153 0029 0d72  .d.|...d...S.).r
+00000ed0: 3200 0000 7219 0000 0063 0100 0000 0000  2...r....c......
+00000ee0: 0000 0000 0000 0200 0000 0400 0000 3300  ..............3.
+00000ef0: 0000 7233 0000 0072 0e00 0000 7234 0000  ..r3...r....r4..
+00000f00: 0072 3600 0000 7239 0000 0072 1600 0000  .r6...r9...r....
+00000f10: 7217 0000 0072 3b00 0000 6700 0000 723c  r....r;...g...r<
+00000f20: 0000 007a 2248 6578 426c 6f63 6b2e 666f  ...z"HexBlock.fo
+00000f30: 726d 6174 2e3c 6c6f 6361 6c73 3e2e 3c67  rmat.<locals>.<g
+00000f40: 656e 6578 7072 3e7a 0568 6578 2028 7a02  enexpr>z.hex (z.
+00000f50: 2920 723f 0000 0072 0100 0000 da01 6472  ) r?...r......dr
+00000f60: 0600 0000 7204 0000 007a 0520 202f 2f20  ....r....z.  // 
+00000f70: 7240 0000 0029 0672 1c00 0000 7231 0000  r@...).r....r1..
+00000f80: 0072 1200 0000 7243 0000 0072 4400 0000  .r....rC...rD...
+00000f90: 721f 0000 0072 4100 0000 7216 0000 0072  r....rA...r....r
+00000fa0: 3900 0000 7217 0000 0072 1f00 0000 6300  9...r....r....c.
+00000fb0: 0000 7320 0000 001a 040c 0110 020a 0104  ..s ............
+00000fc0: ff0a 0104 ff0a 0104 ff08 0204 fe04 0204  ................
+00000fd0: fe02 0206 fe02 ff7a 0f48 6578 426c 6f63  .......z.HexBloc
+00000fe0: 6b2e 666f 726d 6174 4e63 0300 0000 0000  k.formatNc......
+00000ff0: 0000 0000 0000 0800 0000 0500 0000 0300  ................
+00001000: 0000 73f0 0000 0069 0064 0164 0293 0164  ..s....i.d.d...d
+00001010: 0364 0293 0164 0464 0293 0164 0564 0693  .d...d.d...d.d..
+00001020: 0164 0764 0693 0164 0864 0693 0164 0964  .d.d...d.d...d.d
+00001030: 0a93 0164 0b64 0a93 0164 0c64 0a93 0164  ...d.d...d.d...d
+00001040: 0d64 0e93 0164 0f64 0e93 0164 1064 0e93  .d...d.d...d.d..
+00001050: 0164 1164 1293 0164 1364 1293 0164 1464  .d.d...d.d...d.d
+00001060: 1293 0164 1564 1293 0164 1664 1793 0164  ...d.d...d.d...d
+00001070: 1764 1764 1764 189c 03a5 017d 0367 0064  .d.d.d.....}.g.d
+00001080: 19a2 017d 0464 1a7d 0574 007c 0174 0183  ...}.d.}.t.|.t..
+00001090: 0272 4a7c 037c 0119 007d 0174 0287 0066  .rJ|.|...}.t...f
+000010a0: 0164 1b64 1c84 087c 047c 0119 0044 0083  .d.d...|.|...D..
+000010b0: 0183 017d 067c 0264 1d75 0072 7364 1e67  ...}.|.d.u.rsd.g
+000010c0: 017d 0788 006a 0372 677c 07a0 0488 006a  .}...j.rg|.....j
+000010d0: 03a1 0101 007c 07a0 047c 057c 0119 00a1  .....|...|.|....
+000010e0: 0101 0064 1fa0 057c 07a1 017d 0274 067c  ...d...|...}.t.|
+000010f0: 067c 0283 0253 0029 2061 0c02 0000 4765  .|...S.) a....Ge
+00001100: 6e65 7261 7465 2046 6163 6520 6f62 6a65  nerate Face obje
+00001110: 6374 0a20 2020 2020 2020 2069 6e64 6578  ct.        index
+00001120: 2069 7320 6e75 6d62 6572 206f 7220 6b65   is number or ke
+00001130: 7977 6f72 6420 746f 2069 6465 6e74 6966  yword to identif
+00001140: 7920 7468 6520 6661 6365 206f 6620 4865  y the face of He
+00001150: 780a 2020 2020 2020 2020 2020 2020 3020  x.            0 
+00001160: 3d20 2777 2720 3d20 2778 6d27 203d 2027  = 'w' = 'xm' = '
+00001170: 2d31 3030 2720 3d20 2830 2034 2037 2033  -100' = (0 4 7 3
+00001180: 290a 2020 2020 2020 2020 2020 2020 3120  ).            1 
+00001190: 3d20 2765 2720 3d20 2778 7027 203d 2027  = 'e' = 'xp' = '
+000011a0: 3130 3027 203d 2028 3120 3220 3620 3529  100' = (1 2 6 5)
+000011b0: 0a20 2020 2020 2020 2020 2020 2032 203d  .            2 =
+000011c0: 2027 7327 203d 2027 796d 2720 3d20 2730   's' = 'ym' = '0
+000011d0: 2d31 3027 203d 2028 3020 3120 3520 3429  -10' = (0 1 5 4)
+000011e0: 0a20 2020 2020 2020 2020 2020 2033 203d  .            3 =
+000011f0: 2027 6e27 203d 2027 7970 2720 3d20 2730   'n' = 'yp' = '0
+00001200: 3130 2720 3d20 2832 2033 2037 2036 290a  10' = (2 3 7 6).
+00001210: 2020 2020 2020 2020 2020 2020 3420 3d20              4 = 
+00001220: 2762 2720 3d20 277a 6d27 203d 2027 3030  'b' = 'zm' = '00
+00001230: 2d31 2720 3d20 2830 2033 2032 2031 2920  -1' = (0 3 2 1) 
+00001240: 3d20 2262 6f74 746f 6d22 0a20 2020 2020  = "bottom".     
+00001250: 2020 2020 2020 2035 203d 2027 7427 203d         5 = 't' =
+00001260: 2027 7a70 2720 3d20 2730 3031 2720 3d20   'zp' = '001' = 
+00001270: 2834 2035 2036 2037 2920 3d20 2274 6f70  (4 5 6 7) = "top
+00001280: 220a 2020 2020 2020 2020 6e61 6d65 2069  ".        name i
+00001290: 7320 6769 7665 6e20 746f 2046 6163 6520  s given to Face 
+000012a0: 696e 7374 616e 6365 2e20 4966 206f 6d69  instance. If omi
+000012b0: 7474 6564 2c20 6e61 6d65 2069 7320 6175  tted, name is au
+000012c0: 746f 6d61 7469 6361 6c6c 790a 2020 2020  tomatically.    
+000012d0: 2020 2020 2020 2020 6765 6e61 7261 7469          genarati
+000012e0: 6564 206c 696b 6520 2827 662d 2720 2b20  ed like ('f-' + 
+000012f0: 7365 6c66 2e6e 616d 6520 2b20 272d 7727  self.name + '-w'
+00001300: 290a 2020 2020 2020 2020 da01 7772 0100  ).        ..wr..
+00001310: 0000 da02 786d 7a04 2d31 3030 da01 6572  ....xmz.-100..er
+00001320: 0600 0000 da02 7870 da03 3130 3072 3e00  ......xp..100r>.
+00001330: 0000 7204 0000 00da 0279 6d7a 0430 2d31  ..r......ymz.0-1
+00001340: 30da 016e e903 0000 005a 0279 705a 0330  0..n.....Z.ypZ.0
+00001350: 3130 da01 62e9 0400 0000 da06 626f 7474  10..b.......bott
+00001360: 6f6d 5a02 7a6d 7a04 3030 2d31 da01 74e9  omZ.zmz.00-1..t.
+00001370: 0500 0000 2903 da03 746f 705a 027a 705a  ....)...topZ.zpZ
+00001380: 0330 3031 2906 2904 7201 0000 0072 4f00  .001).).r....rO.
+00001390: 0000 e907 0000 0072 4d00 0000 2904 7206  .......rM...).r.
+000013a0: 0000 0072 0400 0000 e906 0000 0072 5200  ...r.........rR.
+000013b0: 0000 2904 7201 0000 0072 0600 0000 7252  ..).r....r....rR
+000013c0: 0000 0072 4f00 0000 2904 7204 0000 0072  ...rO...).r....r
+000013d0: 4d00 0000 7254 0000 0072 5500 0000 2904  M...rT...rU...).
+000013e0: 7201 0000 0072 4d00 0000 7204 0000 0072  r....rM...r....r
+000013f0: 0600 0000 2904 724f 0000 0072 5200 0000  ....).rO...rR...
+00001400: 7255 0000 0072 5400 0000 5a06 7765 736e  rU...rT...Z.wesn
+00001410: 6274 6301 0000 0000 0000 0000 0000 0002  btc.............
+00001420: 0000 0004 0000 0013 0000 0073 1600 0000  ...........s....
+00001430: 6700 7c00 5d07 7d01 8800 6a00 7c01 1900  g.|.].}...j.|...
+00001440: 9102 7102 5300 7216 0000 0029 0172 3100  ..q.S.r....).r1.
+00001450: 0000 2902 7237 0000 00da 0169 7227 0000  ..).r7.....ir'..
+00001460: 0072 1600 0000 7217 0000 00da 0a3c 6c69  .r....r......<li
+00001470: 7374 636f 6d70 3e9e 0000 0073 0200 0000  stcomp>....s....
+00001480: 1600 7a21 4865 7842 6c6f 636b 2e66 6163  ..z!HexBlock.fac
+00001490: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
+000014a0: 636f 6d70 3e4e da01 66fa 012d 2907 da0a  comp>N..f..-)...
+000014b0: 6973 696e 7374 616e 6365 7235 0000 00da  isinstancer5....
+000014c0: 0574 7570 6c65 7212 0000 00da 0661 7070  .tupler......app
+000014d0: 656e 6472 1c00 0000 7230 0000 0029 0872  endr....r0...).r
+000014e0: 1500 0000 7214 0000 0072 1200 0000 5a0b  ....r....r....Z.
+000014f0: 6b77 5f74 6f5f 696e 6465 785a 0f69 6e64  kw_to_indexZ.ind
+00001500: 6578 5f74 6f5f 7665 7274 6578 5a16 696e  ex_to_vertexZ.in
+00001510: 6465 785f 746f 5f64 6566 6175 6c74 7375  dex_to_defaultsu
+00001520: 6666 6978 7231 0000 00da 0570 6172 7473  ffixr1.....parts
+00001530: 7216 0000 0072 2700 0000 7217 0000 00da  r....r'...r.....
+00001540: 0466 6163 656f 0000 0073 6600 0000 020c  .faceo...sf.....
+00001550: 0401 02ff 0402 02fe 0403 02fd 0404 02fc  ................
+00001560: 0405 02fb 0406 02fa 0407 02f9 0408 02f8  ................
+00001570: 0409 02f7 040a 02f6 040b 02f5 040c 02f4  ................
+00001580: 040d 02f3 040e 02f2 040f 02f1 0410 02f0  ................
+00001590: 0411 02ef 0212 0201 0201 08ec 0816 0408  ................
+000015a0: 0a02 0801 1a02 0801 0601 0601 0c01 0e01  ................
+000015b0: 0a01 0a01 7a0d 4865 7842 6c6f 636b 2e66  ....z.HexBlock.f
+000015c0: 6163 6572 0e00 0000 2907 7229 0000 0072  acer....).r)...r
+000015d0: 2a00 0000 722b 0000 0072 0b00 0000 7218  *...r+...r....r.
+000015e0: 0000 0072 1f00 0000 725e 0000 0072 1600  ...r....r^...r..
+000015f0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001600: 0072 4200 0000 5500 0000 7308 0000 0008  .rB...U...s.....
+00001610: 0014 0108 0d0e 0c72 4200 0000 6300 0000  .......rB...c...
+00001620: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00001630: 0040 0000 0073 2600 0000 6500 5a01 6400  .@...s&...e.Z.d.
+00001640: 5a02 6408 6402 6403 8401 5a03 6404 6405  Z.d.d.d...Z.d.d.
+00001650: 8400 5a04 6406 6407 8400 5a05 6401 5300  ..Z.d.d...Z.d.S.
+00001660: 2909 da08 426f 756e 6461 7279 4e63 0500  )...BoundaryNc..
+00001670: 0000 0000 0000 0000 0000 0500 0000 0300  ................
+00001680: 0000 4300 0000 733a 0000 007c 017c 005f  ..C...s:...|.|._
+00001690: 007c 027c 005f 017c 0364 0175 0072 0d67  .|.|._.|.d.u.r.g
+000016a0: 007d 036e 0874 027c 0374 0383 0272 157c  .}.n.t.|.t...r.|
+000016b0: 0367 017d 037c 037c 005f 047c 047c 005f  .g.}.|.|._.|.|._
+000016c0: 0564 0153 0029 027a c469 6e69 7469 616c  .d.S.).z.initial
+000016d0: 697a 6520 626f 756e 6461 7279 0a20 2020  ize boundary.   
+000016e0: 2020 2020 2074 7970 655f 2069 7320 7479       type_ is ty
+000016f0: 7065 206b 6579 776f 7264 2028 7761 6c6c  pe keyword (wall
+00001700: 2c20 7061 7463 682c 2065 6d70 7479 2c20  , patch, empty, 
+00001710: 2e2e 290a 2020 2020 2020 2020 6e61 6d65  ..).        name
+00001720: 2069 7320 6e61 7665 206f 6620 626f 756e   is nave of boun
+00001730: 6461 7279 2065 6d65 6c6d 656e 740a 2020  dary emelment.  
+00001740: 2020 2020 2020 6661 6365 7320 6973 2066        faces is f
+00001750: 6163 6573 2077 6869 6368 2061 7265 2061  aces which are a
+00001760: 7070 6c69 6564 2077 6974 6820 7468 6973  pplied with this
+00001770: 2062 6f75 6e64 6172 7920 636f 6e64 6974   boundary condit
+00001780: 696f 6e73 0a20 2020 2020 2020 204e 2906  ions.        N).
+00001790: da05 7479 7065 5f72 1200 0000 725a 0000  ..type_r....rZ..
+000017a0: 0072 3000 0000 da05 6661 6365 73da 096e  .r0.....faces..n
+000017b0: 6569 6768 626f 7572 2905 7215 0000 0072  eighbour).r....r
+000017c0: 6000 0000 7212 0000 0072 6100 0000 7262  `...r....ra...rb
+000017d0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000017e0: 0000 7218 0000 00a9 0000 0073 1000 0000  ..r........s....
+000017f0: 0606 0601 0801 0601 0a01 0601 0601 0a01  ................
+00001800: 7a11 426f 756e 6461 7279 2e5f 5f69 6e69  z.Boundary.__ini
+00001810: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+00001820: 0200 0000 0300 0000 4300 0000 7310 0000  ........C...s...
+00001830: 007c 006a 00a0 017c 01a1 0101 0064 0153  .|.j...|.....d.S
+00001840: 0029 027a 5161 6464 2066 6163 6520 696e  .).zQadd face in
+00001850: 7374 616e 6365 0a20 2020 2020 2020 2066  stance.        f
+00001860: 6163 6520 6973 2061 2046 6163 6520 696e  ace is a Face in
+00001870: 7374 616e 6365 2028 6e6f 7420 6e61 6d65  stance (not name
+00001880: 2920 746f 2062 6520 6164 6465 640a 2020  ) to be added.  
+00001890: 2020 2020 2020 4e29 0272 6100 0000 725c        N).ra...r\
+000018a0: 0000 0029 0272 1500 0000 725e 0000 0072  ...).r....r^...r
+000018b0: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
+000018c0: 6164 645f 6661 6365 b800 0000 7302 0000  add_face....s...
+000018d0: 0010 047a 1142 6f75 6e64 6172 792e 6164  ...z.Boundary.ad
+000018e0: 645f 6661 6365 6302 0000 0000 0000 0000  d_facec.........
+000018f0: 0000 0004 0000 0008 0000 0043 0000 0073  ...........C...s
+00001900: 8200 0000 7c00 6a00 6701 7d02 7c00 6a01  ....|.j.g.}.|.j.
+00001910: 6401 7500 7216 7c02 a002 6402 6403 7c00  d.u.r.|...d.d.|.
+00001920: 6a03 9b00 6404 9d03 1700 a101 0100 6e10  j...d.........n.
+00001930: 7c02 a002 6402 6403 7c00 6a03 9b00 6405  |...d.d.|.j...d.
+00001940: 7c00 6a01 9b00 6404 9d05 1700 a101 0100  |.j...d.........
+00001950: 7c00 6a04 4400 5d0d 7d03 7c02 a002 6406  |.j.D.].}.|...d.
+00001960: 7c03 a005 7c01 a101 9b00 9d02 a101 0100  |...|...........
+00001970: 7129 7c02 a002 6407 a101 0100 6408 a006  q)|...d.....d...
+00001980: 7c02 a101 5300 2909 7232 0000 004e 7a02  |...S.).r2...Nz.
+00001990: 7b0a 7a09 2020 2020 7479 7065 207a 113b  {.z.    type z.;
+000019a0: 0a20 2020 2066 6163 6573 0a20 2020 2028  .    faces.    (
+000019b0: 7a16 3b0a 2020 2020 6e65 6967 6862 6f75  z.;.    neighbou
+000019c0: 7250 6174 6368 2020 7a08 2020 2020 2020  rPatch  z.      
+000019d0: 2020 7a08 2020 2020 293b 0a7d da01 0a29    z.    );.}...)
+000019e0: 0772 1200 0000 7262 0000 0072 5c00 0000  .r....rb...r\...
+000019f0: 7260 0000 0072 6100 0000 721f 0000 0072  r`...ra...r....r
+00001a00: 1c00 0000 2904 7215 0000 0072 3a00 0000  ....).r....r:...
+00001a10: da03 746d 7072 5e00 0000 7216 0000 0072  ..tmpr^...r....r
+00001a20: 1600 0000 7217 0000 0072 1f00 0000 be00  ....r....r......
+00001a30: 0000 7318 0000 0008 040a 011a 0104 0202  ..s.............
+00001a40: 0114 0102 ff04 ff0a 0418 010a 010a 017a  ...............z
+00001a50: 0f42 6f75 6e64 6172 792e 666f 726d 6174  .Boundary.format
+00001a60: a902 4e4e 2906 7229 0000 0072 2a00 0000  ..NN).r)...r*...
+00001a70: 722b 0000 0072 1800 0000 7263 0000 0072  r+...r....rc...r
+00001a80: 1f00 0000 7216 0000 0072 1600 0000 7216  ....r....r....r.
+00001a90: 0000 0072 1700 0000 725f 0000 00a8 0000  ...r....r_......
+00001aa0: 0073 0800 0000 0800 0a01 080f 0c06 725f  .s............r_
+00001ab0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001ac0: 0000 0000 0500 0000 4000 0000 73be 0000  ........@...s...
+00001ad0: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00001ae0: 0364 0364 0484 005a 0464 0564 0684 005a  .d.d...Z.d.d...Z
+00001af0: 0564 2a64 0864 0984 015a 0664 0a64 0b84  .d*d.d...Z.d.d..
+00001b00: 005a 0764 0c64 0d84 005a 0864 0e64 0f84  .Z.d.d...Z.d.d..
+00001b10: 005a 0964 0765 0a64 1064 1064 1083 0366  .Z.d.e.d.d.d...f
+00001b20: 0264 1164 1284 015a 0b64 1364 1484 005a  .d.d...Z.d.d...Z
+00001b30: 0c64 1564 1684 005a 0d64 2b64 1764 1884  .d.d...Z.d+d.d..
+00001b40: 015a 0e64 1964 1a84 005a 0f64 2c64 1c64  .Z.d.d...Z.d,d.d
+00001b50: 1d84 015a 1064 1e64 1f84 005a 1164 2064  ...Z.d.d...Z.d d
+00001b60: 2184 005a 1264 2264 2384 005a 1364 2464  !..Z.d"d#..Z.d$d
+00001b70: 2584 005a 1464 2664 2784 005a 1565 1664  %..Z.d&d'..Z.e.d
+00001b80: 1b66 0264 2864 2984 015a 1764 0753 0029  .f.d(d)..Z.d.S.)
+00001b90: 2dda 0d42 6c6f 636b 4d65 7368 4469 6374  -..BlockMeshDict
+00001ba0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001bb0: 0002 0000 0043 0000 0073 2800 0000 6401  .....C...s(...d.
+00001bc0: 7c00 5f00 6900 7c00 5f01 6900 7c00 5f02  |._.i.|._.i.|._.
+00001bd0: 6900 7c00 5f03 6900 7c00 5f04 6400 7c00  i.|._.i.|._.d.|.
+00001be0: 5f05 6400 5300 2902 4e67 0000 0000 0000  _.d.S.).Ng......
+00001bf0: f03f 2906 da11 636f 6e76 6572 745f 746f  .?)...convert_to
+00001c00: 5f6d 6574 6572 7372 3a00 0000 da06 626c  _metersr:.....bl
+00001c10: 6f63 6b73 da05 6564 6765 73da 0a62 6f75  ocks..edges..bou
+00001c20: 6e64 6172 6965 73da 165f 7665 7274 6963  ndaries.._vertic
+00001c30: 6573 5f69 6e5f 626c 6f63 6b6d 6573 6872  es_in_blockmeshr
+00001c40: 2700 0000 7216 0000 0072 1600 0000 7217  '...r....r....r.
+00001c50: 0000 0072 1800 0000 d100 0000 730c 0000  ...r........s...
+00001c60: 0006 0106 0106 0106 0106 010a 017a 1642  .............z.B
+00001c70: 6c6f 636b 4d65 7368 4469 6374 2e5f 5f69  lockMeshDict.__i
+00001c80: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
+00001c90: 0000 0300 0000 0900 0000 4300 0000 7324  ..........C...s$
+00001ca0: 0000 0064 0164 0264 0364 0464 0564 0664  ...d.d.d.d.d.d.d
+00001cb0: 0764 0764 089c 087d 027c 027c 0119 007c  .d.d...}.|.|...|
+00001cc0: 005f 0064 0953 0029 0a7a 2273 6574 2073  ._.d.S.).z"set s
+00001cd0: 656c 662e 636f 6d76 6572 745f 746f 5f6d  elf.comvert_to_m
+00001ce0: 6574 6572 7320 6279 2077 6f72 6469 e803  eters by wordi..
+00001cf0: 0000 7206 0000 0067 7b14 ae47 e17a 843f  ..r....g{..G.z.?
+00001d00: 67fc a9f1 d24d 6250 3f67 8ded b5a0 f7c6  g....MbP?g......
+00001d10: b03e 6795 d626 e80b 2e11 3e67 bbbd d7d9  .>g..&....>g....
+00001d20: df7c db3d 2908 5a02 6b6d da01 6dda 0263  .|.=).Z.km..m..c
+00001d30: 6dda 026d 6dda 0275 6dda 026e 6dda 0141  m..mm..um..nm..A
+00001d40: 5a08 416e 6773 7472 6f6d 4ea9 0172 6800  Z.AngstromN..rh.
+00001d50: 0000 2903 7215 0000 005a 066d 6574 7269  ..).r....Z.metri
+00001d60: 635a 176d 6574 7269 6373 796d 5f74 6f5f  cZ.metricsym_to_
+00001d70: 636f 6e76 6572 7369 6f6e 7216 0000 0072  conversionr....r
+00001d80: 1600 0000 7217 0000 00da 0a73 6574 5f6d  ....r......set_m
+00001d90: 6574 7269 63d9 0000 0073 1400 0000 0203  etric....s......
+00001da0: 0201 0201 0201 0201 0201 0201 0201 06f8  ................
+00001db0: 0e0a 7a18 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
+00001dc0: 742e 7365 745f 6d65 7472 6963 6302 0000  t.set_metricc...
+00001dd0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00001de0: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+00001df0: 6400 5300 720e 0000 0072 7300 0000 2902  d.S.r....rs...).
+00001e00: 7215 0000 00da 0573 6361 6c65 7216 0000  r......scaler...
+00001e10: 0072 1600 0000 7217 0000 00da 0973 6574  .r....r......set
+00001e20: 5f73 6361 6c65 e700 0000 7302 0000 000a  _scale....s.....
+00001e30: 017a 1742 6c6f 636b 4d65 7368 4469 6374  .z.BlockMeshDict
+00001e40: 2e73 6574 5f73 6361 6c65 4e63 0500 0000  .set_scaleNc....
+00001e50: 0000 0000 0000 0000 0600 0000 0500 0000  ................
+00001e60: 4300 0000 7358 0000 0074 007c 0174 0183  C...sX...t.|.t..
+00001e70: 0272 1b74 0264 0164 0284 007c 027c 037c  .r.t.d.d...|.|.|
+00001e80: 0466 0344 0083 0183 0172 1574 0364 0383  .f.D.....r.t.d..
+00001e90: 0182 017c 017d 057c 056a 047d 046e 0774  ...|.}.|.j.}.n.t
+00001ea0: 017c 017c 027c 037c 0483 047d 057c 057c  .|.|.|.|...}.|.|
+00001eb0: 006a 057c 043c 007c 006a 057c 0419 0053  .j.|.<.|.j.|...S
+00001ec0: 0029 047a b261 6464 2076 6572 7465 7820  .).z.add vertex 
+00001ed0: 6279 2063 6f6f 7264 696e 6174 6520 616e  by coordinate an
+00001ee0: 6420 756e 6971 206e 616d 650a 2020 2020  d uniq name.    
+00001ef0: 2020 2020 7820 7920 7a20 6973 2063 6f6f      x y z is coo
+00001f00: 7264 696e 6174 6573 206f 6620 7665 7274  rdinates of vert
+00001f10: 6578 0a20 2020 2020 2020 206e 616d 6520  ex.        name 
+00001f20: 6973 2075 6e69 7120 6e61 6d65 2074 6f20  is uniq name to 
+00001f30: 7265 6665 7220 7468 6520 7665 7274 6578  refer the vertex
+00001f40: 0a20 2020 2020 2020 2072 6574 7572 6e73  .        returns
+00001f50: 2056 6572 7465 7820 6f62 6a65 6374 2077   Vertex object w
+00001f60: 6869 6369 2069 7320 6164 6465 642e 0a20  hici is added.. 
+00001f70: 2020 2020 2020 2063 0100 0000 0000 0000         c........
+00001f80: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
+00001f90: 7318 0000 0081 007c 005d 077d 017c 0164  s......|.].}.|.d
+00001fa0: 0075 0156 0001 0071 0264 0053 0072 0e00  .u.V...q.d.S.r..
+00001fb0: 0000 7216 0000 0029 0272 3700 0000 da03  ..r....).r7.....
+00001fc0: 6172 6772 1600 0000 7216 0000 0072 1700  argr....r....r..
+00001fd0: 0000 723b 0000 00f1 0000 0073 0400 0000  ..r;.......s....
+00001fe0: 0280 1600 7a2b 426c 6f63 6b4d 6573 6844  ....z+BlockMeshD
+00001ff0: 6963 742e 6164 645f 7665 7274 6578 2e3c  ict.add_vertex.<
+00002000: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
+00002010: 3e7a 4078 2069 7320 6120 5665 7274 6578  >z@x is a Vertex
+00002020: 2061 6e64 2060 616e 7928 6172 6720 6973   and `any(arg is
+00002030: 206e 6f74 204e 6f6e 6520 666f 7220 6172   not None for ar
+00002040: 6720 696e 2028 792c 207a 2c20 6e61 6d65  g in (y, z, name
+00002050: 2929 6029 0672 5a00 0000 720d 0000 00da  ))`).rZ...r.....
+00002060: 0361 6e79 da0a 5661 6c75 6545 7272 6f72  .any..ValueError
+00002070: 7212 0000 0072 3a00 0000 2906 7215 0000  r....r:...).r...
+00002080: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00002090: 7212 0000 005a 0676 6572 7465 7872 1600  r....Z.vertexr..
+000020a0: 0000 7216 0000 0072 1700 0000 da0a 6164  ..r....r......ad
+000020b0: 645f 7665 7274 6578 ea00 0000 7314 0000  d_vertex....s...
+000020c0: 000a 0618 0102 0102 0104 ff04 0408 010e  ................
+000020d0: 020a 010a 017a 1842 6c6f 636b 4d65 7368  .....z.BlockMesh
+000020e0: 4469 6374 2e61 6464 5f76 6572 7465 7863  Dict.add_vertexc
+000020f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00002100: 0200 0000 4300 0000 730c 0000 007c 006a  ....C...s....|.j
+00002110: 007c 013d 0064 0153 0029 027a 1f64 656c  .|.=.d.S.).z.del
+00002120: 206e 616d 6520 6b65 7920 6672 6f6d 2073   name key from s
+00002130: 656c 662e 7665 7274 6963 6573 4e72 3900  elf.verticesNr9.
+00002140: 0000 2902 7215 0000 0072 1200 0000 7216  ..).r....r....r.
+00002150: 0000 0072 1600 0000 7217 0000 00da 0a64  ...r....r......d
+00002160: 656c 5f76 6572 7465 78fd 0000 0073 0200  el_vertex....s..
+00002170: 0000 0c02 7a18 426c 6f63 6b4d 6573 6844  ....z.BlockMeshD
+00002180: 6963 742e 6465 6c5f 7665 7274 6578 6302  ict.del_vertexc.
+00002190: 0000 0000 0000 0000 0000 0006 0000 0004  ................
+000021a0: 0000 0047 0000 0073 3a00 0000 7c00 6a00  ...G...s:...|.j.
+000021b0: 7c01 1900 7d03 7c02 4400 5d13 7d04 7c00  |...}.|.D.].}.|.
+000021c0: 6a00 7c04 1900 7d05 7c03 6a01 a002 7c05  j.|...}.|.j...|.
+000021d0: 6a01 a101 0100 7c03 7c00 6a00 7c04 3c00  j.....|.|.j.|.<.
+000021e0: 7107 6401 5300 2902 7ae2 7472 6561 7420  q.d.S.).z.treat 
+000021f0: 6e61 6d65 312c 206e 616d 6532 2c20 2e2e  name1, name2, ..
+00002200: 2e20 6173 2073 616d 6520 706f 696e 742e  . as same point.
+00002210: 0a0a 2020 2020 2020 2020 6e61 6d65 322e  ..        name2.
+00002220: 616c 6961 732c 206e 616d 6533 2e61 6c69  alias, name3.ali
+00002230: 6173 2c20 2e2e 2e20 6172 6520 6d65 7267  as, ... are merg
+00002240: 6564 2077 6974 6820 6e61 6d65 312e 616c  ed with name1.al
+00002250: 6961 730a 2020 2020 2020 2020 7468 6520  ias.        the 
+00002260: 6b65 7920 6e61 6d65 322c 206e 616d 6533  key name2, name3
+00002270: 2c20 2e2e 2e20 696e 2073 656c 662e 7665  , ... in self.ve
+00002280: 7274 6963 6573 2061 7265 206b 6570 7420  rtices are kept 
+00002290: 616e 6420 6d61 7070 6564 2074 6f0a 2020  and mapped to.  
+000022a0: 2020 2020 2020 7361 6d65 2056 6572 7465        same Verte
+000022b0: 7820 696e 7374 616e 6365 2061 7320 6e61  x instance as na
+000022c0: 6d65 310a 2020 2020 2020 2020 4e29 0372  me1.        N).r
+000022d0: 3a00 0000 7213 0000 00da 0675 7064 6174  :...r......updat
+000022e0: 6529 0672 1500 0000 da05 6e61 6d65 31da  e).r......name1.
+000022f0: 056e 616d 6573 da01 7672 4c00 0000 7246  .names..vrL...rF
+00002300: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00002310: 0000 da0d 7265 6475 6365 5f76 6572 7465  ....reduce_verte
+00002320: 7801 0100 0073 0c00 0000 0a07 0801 0a01  x....s..........
+00002330: 0e01 0c02 04fc 7a1b 426c 6f63 6b4d 6573  ......z.BlockMes
+00002340: 6844 6963 742e 7265 6475 6365 5f76 6572  hDict.reduce_ver
+00002350: 7465 7863 0100 0000 0000 0000 0000 0000  texc............
+00002360: 0700 0000 0500 0000 4300 0000 7378 0000  ........C...sx..
+00002370: 0074 0074 017c 006a 02a0 03a1 0083 0164  .t.t.|.j.......d
+00002380: 0164 0284 0064 038d 027d 0167 007d 0274  .d...d...}.g.}.t
+00002390: 047c 0164 0464 0284 0083 0244 005d 0b5c  .|.d.d.....D.].\
+000023a0: 027d 037d 047c 02a0 0574 017c 0483 01a1  .}.}.|...t.|....
+000023b0: 0101 0071 167c 0244 005d 157d 0574 067c  ...q.|.D.].}.t.|
+000023c0: 0583 0164 056b 0272 2d71 2464 0664 0784  ...d.k.r-q$d.d..
+000023d0: 007c 0544 0083 017d 067c 006a 077c 068e  .|.D...}.|.j.|..
+000023e0: 0001 0071 2464 0853 0029 097a 3963 616c  ...q$d.S.).z9cal
+000023f0: 6c20 7265 6475 6365 5f76 6572 7465 7820  l reduce_vertex 
+00002400: 6f6e 2061 6c6c 2076 6572 7469 6365 7320  on all vertices 
+00002410: 7769 7468 2069 6465 6e74 6963 616c 2076  with identical v
+00002420: 616c 7565 732e 6301 0000 0000 0000 0000  alues.c.........
+00002430: 0000 0001 0000 0003 0000 0053 0000 00f3  ...........S....
+00002440: 0c00 0000 7400 7c00 6401 1900 8301 5300  ....t.|.d.....S.
+00002450: a902 4e72 0600 0000 a901 7226 0000 00a9  ..Nr......r&....
+00002460: 0172 7f00 0000 7216 0000 0072 1600 0000  .r....r....r....
+00002470: 7217 0000 00da 083c 6c61 6d62 6461 3e14  r......<lambda>.
+00002480: 0100 00f3 0200 0000 0c00 7a2e 426c 6f63  ..........z.Bloc
+00002490: 6b4d 6573 6844 6963 742e 6d65 7267 655f  kMeshDict.merge_
+000024a0: 7665 7274 6963 6573 2e3c 6c6f 6361 6c73  vertices.<locals
+000024b0: 3e2e 3c6c 616d 6264 613e 2901 da03 6b65  >.<lambda>)...ke
+000024c0: 7963 0100 0000 0000 0000 0000 0000 0100  yc..............
+000024d0: 0000 0300 0000 5300 0000 7281 0000 0072  ......S...r....r
+000024e0: 8200 0000 7283 0000 0072 8400 0000 7216  ....r....r....r.
+000024f0: 0000 0072 1600 0000 7217 0000 0072 8500  ...r....r....r..
+00002500: 0000 1701 0000 7286 0000 0072 0600 0000  ......r....r....
+00002510: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002520: 0004 0000 0053 0000 0073 1400 0000 6700  .....S...s....g.
+00002530: 7c00 5d06 7d01 7c01 6400 1900 9102 7102  |.].}.|.d.....q.
+00002540: 5300 2901 7201 0000 0072 1600 0000 2902  S.).r....r....).
+00002550: 7237 0000 0072 7f00 0000 7216 0000 0072  r7...r....r....r
+00002560: 1600 0000 7217 0000 0072 5700 0000 1c01  ....r....rW.....
+00002570: 0000 7302 0000 0014 007a 3042 6c6f 636b  ..s......z0Block
+00002580: 4d65 7368 4469 6374 2e6d 6572 6765 5f76  MeshDict.merge_v
+00002590: 6572 7469 6365 732e 3c6c 6f63 616c 733e  ertices.<locals>
+000025a0: 2e3c 6c69 7374 636f 6d70 3e4e 2908 721d  .<listcomp>N).r.
+000025b0: 0000 00da 046c 6973 7472 3a00 0000 da05  .....listr:.....
+000025c0: 6974 656d 7372 0200 0000 725c 0000 0072  itemsr....r\...r
+000025d0: 1b00 0000 7280 0000 0029 0772 1500 0000  ....r....).r....
+000025e0: 5a0f 736f 7274 6564 5f76 6572 7469 6365  Z.sorted_vertice
+000025f0: 73da 0667 726f 7570 73da 016b da01 67da  s..groups..k..g.
+00002600: 0567 726f 7570 727e 0000 0072 1600 0000  .groupr~...r....
+00002610: 7216 0000 0072 1700 0000 da0e 6d65 7267  r....r......merg
+00002620: 655f 7665 7274 6963 6573 0f01 0000 7318  e_vertices....s.
+00002630: 0000 0002 0412 0106 ff04 0316 0110 0108  ................
+00002640: 010c 0102 010e 010c 0104 fc7a 1c42 6c6f  ...........z.Blo
+00002650: 636b 4d65 7368 4469 6374 2e6d 6572 6765  ckMeshDict.merge
+00002660: 5f76 6572 7469 6365 7372 0600 0000 6305  _verticesr....c.
+00002670: 0000 0000 0000 0000 0000 0006 0000 0005  ................
+00002680: 0000 0043 0000 0073 3400 0000 7c03 6400  ...C...s4...|.d.
+00002690: 7500 720c 6401 7400 7c00 6a01 8301 9b00  u.r.d.t.|.j.....
+000026a0: 9d02 7d03 7402 7c01 7c02 7c03 7c04 8304  ..}.t.|.|.|.|...
+000026b0: 7d05 7c05 7c00 6a01 7c03 3c00 7c05 5300  }.|.|.j.|.<.|.S.
+000026c0: 2902 4e72 4e00 0000 2903 721b 0000 0072  ).NrN...).r....r
+000026d0: 6900 0000 7242 0000 0029 0672 1500 0000  i...rB...).r....
+000026e0: 7231 0000 0072 4300 0000 7212 0000 0072  r1...rC...r....r
+000026f0: 4400 0000 724e 0000 0072 1600 0000 7216  D...rN...r....r.
+00002700: 0000 0072 1700 0000 da0c 6164 645f 6865  ...r......add_he
+00002710: 7862 6c6f 636b 1f01 0000 730a 0000 0008  xblock....s.....
+00002720: 0310 010e 010a 0104 017a 1a42 6c6f 636b  .........z.Block
+00002730: 4d65 7368 4469 6374 2e61 6464 5f68 6578  MeshDict.add_hex
+00002740: 626c 6f63 6b63 0400 0000 0000 0000 0000  blockc..........
+00002750: 0000 0500 0000 0400 0000 4300 0000 f31a  ..........C.....
+00002760: 0000 0074 007c 017c 027c 0383 037d 047c  ...t.|.|.|...}.|
+00002770: 047c 006a 017c 023c 007c 0453 0072 0e00  .|.j.|.<.|.S.r..
+00002780: 0000 2902 7207 0000 0072 6a00 0000 2905  ..).r....rj...).
+00002790: 7215 0000 0072 3100 0000 7212 0000 005a  r....r1...r....Z
+000027a0: 0c69 6e74 6572 5f76 6572 7465 7872 4800  .inter_vertexrH.
+000027b0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+000027c0: 00da 0b61 6464 5f61 7263 6564 6765 2801  ...add_arcedge(.
+000027d0: 0000 f306 0000 000c 010a 0104 017a 1942  .............z.B
+000027e0: 6c6f 636b 4d65 7368 4469 6374 2e61 6464  lockMeshDict.add
+000027f0: 5f61 7263 6564 6765 6304 0000 0000 0000  _arcedgec.......
+00002800: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
+00002810: 0072 9000 0000 720e 0000 0029 0272 0800  .r....r....).r..
+00002820: 0000 726a 0000 0029 0572 1500 0000 7231  ..rj...).r....r1
+00002830: 0000 0072 1200 0000 da06 706f 696e 7473  ...r......points
+00002840: 7248 0000 0072 1600 0000 7216 0000 0072  rH...r....r....r
+00002850: 1700 0000 da0e 6164 645f 7370 6c69 6e65  ......add_spline
+00002860: 6564 6765 2d01 0000 7292 0000 007a 1c42  edge-...r....z.B
+00002870: 6c6f 636b 4d65 7368 4469 6374 2e61 6464  lockMeshDict.add
+00002880: 5f73 706c 696e 6565 6467 6563 0500 0000  _splineedgec....
+00002890: 0000 0000 0000 0000 0600 0000 0500 0000  ................
+000028a0: 4300 0000 731c 0000 0074 007c 017c 027c  C...s....t.|.|.|
+000028b0: 037c 0483 047d 057c 057c 006a 017c 023c  .|...}.|.|.j.|.<
+000028c0: 007c 0553 0072 0e00 0000 2902 725f 0000  .|.S.r....).r_..
+000028d0: 0072 6b00 0000 2906 7215 0000 0072 6000  .rk...).r....r`.
+000028e0: 0000 7212 0000 0072 6100 0000 7262 0000  ..r....ra...rb..
+000028f0: 0072 4e00 0000 7216 0000 0072 1600 0000  .rN...r....r....
+00002900: 7217 0000 00da 0c61 6464 5f62 6f75 6e64  r......add_bound
+00002910: 6172 7932 0100 0073 0600 0000 0e01 0a01  ary2...s........
+00002920: 0401 7a1a 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
+00002930: 742e 6164 645f 626f 756e 6461 7279 6305  t.add_boundaryc.
+00002940: 0000 0000 0000 0000 0000 0007 0000 0006  ................
+00002950: 0000 0043 0000 0073 2c00 0000 7c00 6a00  ...C...s,...|.j.
+00002960: 6401 7c01 7c03 7c02 6402 8d04 7d05 7c00  d.|.|.|.d...}.|.
+00002970: 6a00 6401 7c02 7c04 7c01 6402 8d04 7d06  j.d.|.|.|.d...}.
+00002980: 7c05 7c06 6602 5300 2903 7aca 4164 6420  |.|.f.S.).z.Add 
+00002990: 3220 6379 636c 6963 2062 6f75 6e64 6172  2 cyclic boundar
+000029a0: 6965 730a 0a20 2020 2020 2020 2045 7861  ies..        Exa
+000029b0: 6d70 6c65 0a20 2020 2020 2020 202d 2d2d  mple.        ---
+000029c0: 2d2d 2d2d 0a0a 2020 2020 2020 2020 3220  ----..        2 
+000029d0: 6379 636c 6963 2062 6f75 6e64 6172 6965  cyclic boundarie
+000029e0: 7320 6361 6e20 6265 2063 7265 6174 6564  s can be created
+000029f0: 2061 7320 666f 6c6c 6f77 3a3a 0a0a 2020   as follow::..  
+00002a00: 2020 2020 2020 2020 6164 645f 6379 636c          add_cycl
+00002a10: 6963 5f62 6f75 6e64 6172 6965 7328 226f  ic_boundaries("o
+00002a20: 7574 6c65 7422 2c20 2269 6e6c 6574 222c  utlet", "inlet",
+00002a30: 2062 302e 6661 6365 2822 6522 292c 2062   b0.face("e"), b
+00002a40: 302e 6661 6365 2822 7722 2929 0a0a 2020  0.face("w"))..  
+00002a50: 2020 2020 2020 5a06 6379 636c 6963 2901        Z.cyclic).
+00002a60: 7262 0000 0029 0172 9500 0000 2907 7215  rb...).r....).r.
+00002a70: 0000 005a 056e 616d 6530 727d 0000 005a  ...Z.name0r}...Z
+00002a80: 0666 6163 6573 305a 0666 6163 6573 31da  .faces0Z.faces1.
+00002a90: 0262 30da 0262 3172 1600 0000 7216 0000  .b0..b1r....r...
+00002aa0: 0072 1700 0000 da15 6164 645f 6379 636c  .r......add_cycl
+00002ab0: 6963 5f62 6f75 6e64 6172 6965 7337 0100  ic_boundaries7..
+00002ac0: 0073 0600 0000 120b 1201 0801 7a23 426c  .s..........z#Bl
+00002ad0: 6f63 6b4d 6573 6844 6963 742e 6164 645f  ockMeshDict.add_
+00002ae0: 6379 636c 6963 5f62 6f75 6e64 6172 6965  cyclic_boundarie
+00002af0: 7354 6302 0000 0000 0000 0000 0000 0008  sTc.............
+00002b00: 0000 0005 0000 0043 0000 0073 ba00 0000  .......C...s....
+00002b10: 7400 8300 7d02 6700 7c00 5f01 7c00 6a02  t...}.g.|._.|.j.
+00002b20: a003 a100 4400 5d1e 7d03 7c03 6a04 4400  ....D.].}.|.j.D.
+00002b30: 5d18 7d04 7c00 6a05 7c04 1900 7d05 7c05  ].}.|.j.|...}.|.
+00002b40: 6a06 7c02 7601 7228 7c02 a007 7c05 6a06  j.|.v.r(|...|.j.
+00002b50: a101 0100 7c00 6a01 a008 7c05 a101 0100  ....|.j...|.....
+00002b60: 7110 710b 7c01 6401 6b02 7246 6700 7c00  q.q.|.d.k.rFg.|.
+00002b70: 5f01 7c00 6a05 a009 a100 4400 5d0e 5c02  _.|.j.....D.].\.
+00002b80: 7d06 7d05 7c06 7c02 7600 7244 7c00 6a01  }.}.|.|.v.rD|.j.
+00002b90: a008 7c05 a101 0100 7136 6e08 7c01 724e  ..|.....q6n.|.rN
+00002ba0: 740a 7c00 6a01 8301 7c00 5f01 740b 7c00  t.|.j...|._.t.|.
+00002bb0: 6a01 8301 4400 5d07 5c02 7d07 7d05 7c07  j...D.].\.}.}.|.
+00002bc0: 7c05 5f0c 7153 6402 5300 2903 7ae3 312e  |._.qSd.S.).z.1.
+00002bd0: 2063 7265 6174 6520 6c69 7374 206f 6620   create list of 
+00002be0: 5665 7274 6578 2077 6869 6368 2061 7265  Vertex which are
+00002bf0: 2072 6566 6572 7265 6420 6279 2062 6c6f   referred by blo
+00002c00: 636b 7320 6f6e 6c79 2e0a 2020 2020 2020  cks only..      
+00002c10: 2020 322e 2073 6f72 7420 7665 7274 6578    2. sort vertex
+00002c20: 2061 6363 6f72 6469 6e67 2074 6f20 2878   according to (x
+00002c30: 2c20 792c 207a 290a 2020 2020 2020 2020  , y, z).        
+00002c40: 332e 2061 7373 6967 6e20 7365 7175 656e  3. assign sequen
+00002c50: 6365 206e 756d 6265 7220 666f 7220 6561  ce number for ea
+00002c60: 6368 2056 6572 7465 780a 2020 2020 2020  ch Vertex.      
+00002c70: 2020 342e 2073 6f72 7465 6420 6c69 7374    4. sorted list
+00002c80: 2069 7320 7361 7665 6420 6173 2073 656c   is saved as sel
+00002c90: 662e 5f76 6572 7469 6365 735f 696e 5f62  f._vertices_in_b
+00002ca0: 6c6f 636b 6d65 7368 0a20 2020 2020 2020  lockmesh.       
+00002cb0: 205a 0861 735f 6164 6465 644e 290d da03   Z.as_addedN)...
+00002cc0: 7365 7472 6c00 0000 7269 0000 00da 0676  setrl...ri.....v
+00002cd0: 616c 7565 7372 3100 0000 723a 0000 0072  aluesr1...r:...r
+00002ce0: 1200 0000 da03 6164 6472 5c00 0000 7289  ......addr\...r.
+00002cf0: 0000 0072 1d00 0000 da09 656e 756d 6572  ...r......enumer
+00002d00: 6174 6572 1400 0000 2908 7215 0000 00da  ater....).r.....
+00002d10: 0473 6f72 745a 0b76 6e61 6d65 735f 6b65  .sortZ.vnames_ke
+00002d20: 7074 724e 0000 0072 4c00 0000 727f 0000  ptrN...rL...r...
+00002d30: 00da 0576 6e61 6d65 7256 0000 0072 1600  ...vnamerV...r..
+00002d40: 0000 7216 0000 0072 1700 0000 da0f 6173  ..r....r......as
+00002d50: 7369 676e 5f76 6572 7465 7869 6446 0100  sign_vertexidF..
+00002d60: 0073 2c00 0000 0607 0601 0e01 0a01 0a01  .s,.............
+00002d70: 0a01 0c01 0c01 0280 02fc 0805 0601 1201  ................
+00002d80: 0801 0c01 0280 02fe 0403 0c01 1201 0801  ................
+00002d90: 04ff 7a1d 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
+00002da0: 742e 6173 7369 676e 5f76 6572 7465 7869  t.assign_vertexi
+00002db0: 6463 0100 0000 0000 0000 0000 0000 0300  dc..............
+00002dc0: 0000 0600 0000 4300 0000 7338 0000 0064  ......C...s8...d
+00002dd0: 0167 017d 017c 006a 0044 005d 0b7d 027c  .g.}.|.j.D.].}.|
+00002de0: 01a0 0164 027c 02a0 02a1 0017 00a1 0101  ...d.|..........
+00002df0: 0071 067c 01a0 0164 03a1 0101 0064 04a0  .q.|...d.....d..
+00002e00: 037c 01a1 0153 0029 057a ec66 6f72 6d61  .|...S.).z.forma
+00002e10: 7420 7665 7274 6963 6573 2073 6563 7469  t vertices secti
+00002e20: 6f6e 2e0a 2020 2020 2020 2020 6173 7369  on..        assi
+00002e30: 676e 5f76 6572 7465 7869 6428 2920 7368  gn_vertexid() sh
+00002e40: 6f75 6c64 2062 6520 6361 6c6c 6564 2062  ould be called b
+00002e50: 6566 6f72 6520 7468 6973 206d 6574 686f  efore this metho
+00002e60: 642c 2062 6563 6175 7365 0a20 2020 2020  d, because.     
+00002e70: 2020 2073 656c 662e 5f76 6572 7469 6365     self._vertice
+00002e80: 735f 696e 5f62 6c6f 636b 6d65 7368 2073  s_in_blockmesh s
+00002e90: 686f 756c 6420 6265 2061 7661 696c 6162  hould be availab
+00002ea0: 6c65 2061 6e64 0a20 2020 2020 2020 206d  le and.        m
+00002eb0: 656d 6265 7273 206f 6620 7365 6c66 2e5f  embers of self._
+00002ec0: 7665 7274 6963 6573 5f69 6e5f 626c 6f63  vertices_in_bloc
+00002ed0: 6b6d 6573 6820 7368 6f75 6c64 2068 6176  kmesh should hav
+00002ee0: 6520 7661 6c69 6420 696e 6465 782e 0a20  e valid index.. 
+00002ef0: 2020 2020 2020 207a 0a76 6572 7469 6365         z.vertice
+00002f00: 730a 28fa 0420 2020 20fa 0229 3b72 6400  s.(..    ..);rd.
+00002f10: 0000 2904 726c 0000 0072 5c00 0000 721f  ..).rl...r\...r.
+00002f20: 0000 0072 1c00 0000 2903 7215 0000 0072  ...r....).r....r
+00002f30: 6500 0000 727f 0000 0072 1600 0000 7216  e...r....r....r.
+00002f40: 0000 0072 1700 0000 da17 666f 726d 6174  ...r......format
+00002f50: 5f76 6572 7469 6365 735f 7365 6374 696f  _vertices_sectio
+00002f60: 6e5f 0100 0073 0a00 0000 0606 0a01 1401  n_...s..........
+00002f70: 0a01 0a01 7a25 426c 6f63 6b4d 6573 6844  ....z%BlockMeshD
+00002f80: 6963 742e 666f 726d 6174 5f76 6572 7469  ict.format_verti
+00002f90: 6365 735f 7365 6374 696f 6e63 0100 0000  ces_sectionc....
+00002fa0: 0000 0000 0000 0000 0300 0000 0700 0000  ................
+00002fb0: 4300 0000 f340 0000 0064 0167 017d 017c  C....@...d.g.}.|
+00002fc0: 006a 00a0 01a1 0044 005d 0d7d 027c 01a0  .j.....D.].}.|..
+00002fd0: 0264 027c 02a0 037c 006a 04a1 0117 00a1  .d.|...|.j......
+00002fe0: 0101 0071 087c 01a0 0264 03a1 0101 0064  ...q.|...d.....d
+00002ff0: 04a0 057c 01a1 0153 0029 057a a266 6f72  ...|...S.).z.for
+00003000: 6d61 7420 626c 6f63 6b73 2073 6563 7469  mat blocks secti
+00003010: 6f6e 2e0a 2020 2020 2020 2020 6173 7369  on..        assi
+00003020: 676e 5f76 6572 7465 7869 6428 2920 7368  gn_vertexid() sh
+00003030: 6f75 6c64 2062 6520 6361 6c6c 6564 2062  ould be called b
+00003040: 6566 6f72 6520 7468 6973 206d 6574 686f  efore this metho
+00003050: 642c 2062 6563 6175 7365 0a20 2020 2020  d, because.     
+00003060: 2020 2076 6572 7469 6365 7320 7265 6665     vertices refe
+00003070: 7265 6420 6279 2062 6c6f 636b 7320 7368  red by blocks sh
+00003080: 6f75 6c64 2068 6176 6520 7661 6c69 6420  ould have valid 
+00003090: 696e 6465 782e 0a20 2020 2020 2020 207a  index..        z
+000030a0: 0862 6c6f 636b 730a 2872 a000 0000 72a1  .blocks.(r....r.
+000030b0: 0000 0072 6400 0000 2906 7269 0000 0072  ...rd...).ri...r
+000030c0: 9a00 0000 725c 0000 0072 1f00 0000 723a  ....r\...r....r:
+000030d0: 0000 0072 1c00 0000 2903 7215 0000 0072  ...r....).r....r
+000030e0: 6500 0000 724e 0000 0072 1600 0000 7216  e...rN...r....r.
+000030f0: 0000 0072 1700 0000 da15 666f 726d 6174  ...r......format
+00003100: 5f62 6c6f 636b 735f 7365 6374 696f 6e6b  _blocks_sectionk
+00003110: 0100 0073 0a00 0000 0605 0e01 1801 0a01  ...s............
+00003120: 0a01 7a23 426c 6f63 6b4d 6573 6844 6963  ..z#BlockMeshDic
+00003130: 742e 666f 726d 6174 5f62 6c6f 636b 735f  t.format_blocks_
+00003140: 7365 6374 696f 6e63 0100 0000 0000 0000  sectionc........
+00003150: 0000 0000 0300 0000 0700 0000 4300 0000  ............C...
+00003160: 72a3 0000 0029 057a a166 6f72 6d61 7420  r....).z.format 
+00003170: 6564 6765 7320 7365 6374 696f 6e2e 0a20  edges section.. 
+00003180: 2020 2020 2020 2061 7373 6967 6e5f 7665         assign_ve
+00003190: 7274 6578 6964 2829 2073 686f 756c 6420  rtexid() should 
+000031a0: 6265 2063 616c 6c65 6420 6265 666f 7265  be called before
+000031b0: 2074 6869 7320 6d65 7468 6f64 2c20 6265   this method, be
+000031c0: 6361 7573 650a 2020 2020 2020 2020 7665  cause.        ve
+000031d0: 7274 6963 6573 2072 6566 6572 6564 2062  rtices refered b
+000031e0: 7920 626c 6f63 6b73 2073 686f 756c 6420  y blocks should 
+000031f0: 6861 7665 2076 616c 6964 2069 6e64 6578  have valid index
+00003200: 2e0a 2020 2020 2020 2020 7a07 6564 6765  ..        z.edge
+00003210: 730a 2872 a000 0000 72a1 0000 0072 6400  s.(r....r....rd.
+00003220: 0000 2906 726a 0000 0072 9a00 0000 725c  ..).rj...r....r\
+00003230: 0000 0072 1f00 0000 723a 0000 0072 1c00  ...r....r:...r..
+00003240: 0000 2903 7215 0000 0072 6500 0000 7248  ..).r....re...rH
+00003250: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00003260: 0000 da14 666f 726d 6174 5f65 6467 6573  ....format_edges
+00003270: 5f73 6563 7469 6f6e 7601 0000 730a 0000  _sectionv...s...
+00003280: 0006 060e 0118 010a 010a 017a 2242 6c6f  ...........z"Blo
+00003290: 636b 4d65 7368 4469 6374 2e66 6f72 6d61  ckMeshDict.forma
+000032a0: 745f 6564 6765 735f 7365 6374 696f 6e63  t_edges_sectionc
+000032b0: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+000032c0: 0600 0000 4300 0000 7354 0000 0064 0167  ....C...sT...d.g
+000032d0: 017d 017c 006a 00a0 01a1 0044 005d 177d  .}.|.j.....D.].}
+000032e0: 0264 027d 037c 02a0 027c 006a 03a1 01a0  .d.}.|...|.j....
+000032f0: 0464 0364 037c 0317 00a1 027d 047c 01a0  .d.d.|.....}.|..
+00003300: 057c 037c 0417 00a1 0101 0071 087c 01a0  .|.|.......q.|..
+00003310: 0564 04a1 0101 0064 03a0 067c 01a1 0153  .d.....d...|...S
+00003320: 0029 057a a366 6f72 6d61 7420 626f 756e  .).z.format boun
+00003330: 6461 7279 2073 6563 7469 6f6e 2e0a 2020  dary section..  
+00003340: 2020 2020 2020 6173 7369 676e 5f76 6572        assign_ver
+00003350: 7465 7869 6428 2920 7368 6f75 6c64 2062  texid() should b
+00003360: 6520 6361 6c6c 6564 2062 6566 6f72 6520  e called before 
+00003370: 7468 6973 206d 6574 686f 642c 2062 6563  this method, bec
+00003380: 6175 7365 0a20 2020 2020 2020 2076 6572  ause.        ver
+00003390: 7469 6365 7320 7265 6665 7265 6420 6279  tices refered by
+000033a0: 2066 6163 6573 2073 686f 756c 6420 6861   faces should ha
+000033b0: 7665 2076 616c 6964 2069 6e64 6578 2e0a  ve valid index..
+000033c0: 2020 2020 2020 2020 7a0a 626f 756e 6461          z.bounda
+000033d0: 7279 0a28 72a0 0000 0072 6400 0000 72a1  ry.(r....rd...r.
+000033e0: 0000 0029 0772 6b00 0000 729a 0000 0072  ...).rk...r....r
+000033f0: 1f00 0000 723a 0000 00da 0772 6570 6c61  ....r:.....repla
+00003400: 6365 725c 0000 0072 1c00 0000 2905 7215  cer\...r....).r.
+00003410: 0000 0072 6500 0000 724e 0000 00da 0669  ...re...rN.....i
+00003420: 6e64 656e 7472 3e00 0000 7216 0000 0072  ndentr>...r....r
+00003430: 1600 0000 7217 0000 00da 1766 6f72 6d61  ....r......forma
+00003440: 745f 626f 756e 6461 7279 5f73 6563 7469  t_boundary_secti
+00003450: 6f6e 8201 0000 730e 0000 0006 060e 0104  on....s.........
+00003460: 0218 0110 010a 010a 017a 2542 6c6f 636b  .........z%Block
+00003470: 4d65 7368 4469 6374 2e66 6f72 6d61 745f  MeshDict.format_
+00003480: 626f 756e 6461 7279 5f73 6563 7469 6f6e  boundary_section
+00003490: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000034a0: 0001 0000 0043 0000 0073 0400 0000 6401  .....C...s....d.
+000034b0: 5300 2902 4eda 0072 1600 0000 7227 0000  S.).N..r....r'..
+000034c0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+000034d0: da1e 666f 726d 6174 5f6d 6572 6765 7061  ..format_mergepa
+000034e0: 7463 6870 6169 7273 5f73 6563 7469 6f6e  tchpairs_section
+000034f0: 9101 0000 7302 0000 0004 027a 2c42 6c6f  ....s......z,Blo
+00003500: 636b 4d65 7368 4469 6374 2e66 6f72 6d61  ckMeshDict.forma
+00003510: 745f 6d65 7267 6570 6174 6368 7061 6972  t_mergepatchpair
+00003520: 735f 7365 6374 696f 6e63 0300 0000 0000  s_sectionc......
+00003530: 0000 0000 0000 0400 0000 0900 0000 4300  ..............C.
+00003540: 0000 7346 0000 007c 006a 007c 0264 018d  ..sF...|.j.|.d..
+00003550: 0101 0074 0164 0283 017d 037c 036a 027c  ...t.d...}.|.j.|
+00003560: 0174 037c 006a 0483 017c 00a0 05a1 007c  .t.|.j...|.....|
+00003570: 00a0 06a1 007c 00a0 07a1 007c 00a0 08a1  .....|.....|....
+00003580: 007c 00a0 09a1 0064 038d 0753 0029 044e  .|.....d...S.).N
+00003590: 2901 729d 0000 0061 6d01 0000 2468 6561  ).r....am...$hea
+000035a0: 6465 720a 466f 616d 4669 6c65 0a7b 0a20  der.FoamFile.{. 
+000035b0: 2020 2076 6572 7369 6f6e 2020 2020 2032     version     2
+000035c0: 2e30 3b0a 2020 2020 666f 726d 6174 2020  .0;.    format  
+000035d0: 2020 2020 6173 6369 693b 0a20 2020 2063      ascii;.    c
+000035e0: 6c61 7373 2020 2020 2020 2064 6963 7469  lass       dicti
+000035f0: 6f6e 6172 793b 0a20 2020 206f 626a 6563  onary;.    objec
+00003600: 7420 2020 2020 2062 6c6f 636b 4d65 7368  t      blockMesh
+00003610: 4469 6374 3b0a 7d0a 2f2f 202a 202a 202a  Dict;.}.// * * *
+00003620: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
+00003630: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
+00003640: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
+00003650: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
+00003660: 202a 202a 202f 2f0a 0a73 6361 6c65 2020   * * //..scale  
+00003670: 2024 6d65 7472 6963 636f 6e76 6572 743b   $metricconvert;
+00003680: 0a0a 2476 6572 7469 6365 730a 0a24 626c  ..$vertices..$bl
+00003690: 6f63 6b73 0a0a 2465 6467 6573 0a0a 2462  ocks..$edges..$b
+000036a0: 6f75 6e64 6172 790a 246d 6572 6765 7061  oundary.$mergepa
+000036b0: 7463 6870 6169 7273 0a2f 2f20 2a2a 2a2a  tchpairs.// ****
+000036c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000036d0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000036e0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000036f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00003700: 2a2a 2a2a 2a20 2f2f 0a29 07da 0668 6561  ***** //.)...hea
+00003710: 6465 725a 0d6d 6574 7269 6363 6f6e 7665  derZ.metricconve
+00003720: 7274 723a 0000 0072 6a00 0000 7269 0000  rtr:...rj...ri..
+00003730: 00da 0862 6f75 6e64 6172 795a 0f6d 6572  ...boundaryZ.mer
+00003740: 6765 7061 7463 6870 6169 7273 290a 729f  gepatchpairs).r.
+00003750: 0000 0072 0300 0000 da0a 7375 6273 7469  ...r......substi
+00003760: 7475 7465 7235 0000 0072 6800 0000 72a2  tuter5...rh...r.
+00003770: 0000 0072 a500 0000 72a4 0000 0072 a800  ...r....r....r..
+00003780: 0000 72aa 0000 0029 0472 1500 0000 72ab  ..r....).r....r.
+00003790: 0000 005a 0d73 6f72 745f 766f 7274 6963  ...Z.sort_vortic
+000037a0: 6573 da08 7465 6d70 6c61 7465 7216 0000  es..templater...
+000037b0: 0072 1600 0000 7217 0000 0072 1f00 0000  .r....r....r....
+000037c0: 9a01 0000 731a 0000 000c 0102 0102 0104  ....s...........
+000037d0: ff04 1902 0108 0106 0106 0106 0106 0106  ................
+000037e0: 0106 f97a 1442 6c6f 636b 4d65 7368 4469  ...z.BlockMeshDi
+000037f0: 6374 2e66 6f72 6d61 7429 034e 4e4e 7266  ct.format).NNNrf
+00003800: 0000 0029 0154 2918 7229 0000 0072 2a00  ...).T).r)...r*.
+00003810: 0000 722b 0000 0072 1800 0000 7274 0000  ..r+...r....rt..
+00003820: 0072 7600 0000 727a 0000 0072 7b00 0000  .rv...rz...r{...
+00003830: 7280 0000 0072 8e00 0000 720b 0000 0072  r....r....r....r
+00003840: 8f00 0000 7291 0000 0072 9400 0000 7295  ....r....r....r.
+00003850: 0000 0072 9800 0000 729f 0000 0072 a200  ...r....r....r..
+00003860: 0000 72a4 0000 0072 a500 0000 72a8 0000  ..r....r....r...
+00003870: 0072 aa00 0000 7205 0000 0072 1f00 0000  .r....r....r....
+00003880: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+00003890: 1700 0000 7267 0000 00d0 0000 0073 2a00  ....rg.......s*.
+000038a0: 0000 0800 0801 0808 080e 0a03 0813 0804  ................
+000038b0: 080e 0c11 0aff 0809 0805 0a05 0805 0a0f  ................
+000038c0: 0819 080c 080b 080c 080f 1209 7267 0000  ............rg..
+000038d0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000038e0: 0000 0300 0000 0000 0000 731c 0000 0065  ..........s....e
+000038f0: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
+00003900: 085a 0387 0004 005a 0453 0029 03da 1842  .Z.....Z.S.)...B
+00003910: 6c6f 636b 4d65 7368 4469 6374 5265 6374  lockMeshDictRect
+00003920: 696c 696e 6561 7263 0800 0000 0000 0000  ilinearc........
+00003930: 0000 0000 0b00 0000 0800 0000 0300 0000  ................
+00003940: 73b0 0000 0074 0083 00a0 01a1 0001 007c  s....t.........|
+00003950: 00a0 027c 07a1 0101 0074 0364 0164 0164  ...|.....t.d.d.d
+00003960: 0164 0283 0474 037c 0164 0164 0164 0383  .d...t.|.d.d.d..
+00003970: 0474 037c 017c 0264 0164 0483 0474 0364  .t.|.|.d.d...t.d
+00003980: 017c 0264 0164 0583 0467 047d 087c 0844  .|.d.d...g.}.|.D
+00003990: 005d 1c7d 097c 00a0 047c 096a 057c 096a  .].}.|...|.j.|.j
+000039a0: 0664 017c 096a 0764 0617 00a1 0401 007c  .d.|.j.d.......|
+000039b0: 00a0 047c 096a 057c 096a 067c 037c 096a  ...|.j.|.j.|.|.j
+000039c0: 0764 0717 00a1 0401 0071 2664 0864 0984  .d.......q&d.d..
+000039d0: 0064 0a44 0083 017d 0a7c 006a 087c 0a7c  .d.D...}.|.j.|.|
+000039e0: 047c 057c 0666 0364 0b64 0c8d 037c 005f  .|.|.f.d.d...|._
+000039f0: 0964 0053 0029 0d4e 7201 0000 005a 0276  .d.S.).Nr....Z.v
+00003a00: 30da 0276 31da 0276 325a 0276 33fa 042d  0..v1..v2Z.v3..-
+00003a10: 626f 74fa 042d 746f 7063 0100 0000 0000  bot..-topc......
+00003a20: 0000 0000 0000 0300 0000 0600 0000 5300  ..............S.
+00003a30: 0000 7328 0000 0067 007c 005d 107d 0174  ..s(...g.|.].}.t
+00003a40: 0064 0083 0144 005d 097d 0264 017c 029b  .d...D.].}.d.|..
+00003a50: 007c 019b 009d 0391 0371 0871 0253 0029  .|.......q.q.S.)
+00003a60: 0272 4f00 0000 727f 0000 0029 01da 0572  .rO...r....)...r
+00003a70: 616e 6765 2903 7237 0000 00da 0470 6f73  ange).r7.....pos
+00003a80: 7472 1400 0000 7216 0000 0072 1600 0000  tr....r....r....
+00003a90: 7217 0000 0072 5700 0000 d101 0000 730a  r....rW.......s.
+00003aa0: 0000 0006 0008 0104 ff0e 0108 ff7a 3542  .............z5B
+00003ab0: 6c6f 636b 4d65 7368 4469 6374 5265 6374  lockMeshDictRect
+00003ac0: 696c 696e 6561 722e 5f5f 696e 6974 5f5f  ilinear.__init__
+00003ad0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00003ae0: 6f6d 703e 2902 72b2 0000 0072 b300 0000  omp>).r....r....
+00003af0: 72a9 0000 0029 0172 1200 0000 290a da05  r....).r....)...
+00003b00: 7375 7065 7272 1800 0000 7276 0000 0072  superr....rv...r
+00003b10: 0d00 0000 727a 0000 0072 0f00 0000 7210  ....rz...r....r.
+00003b20: 0000 0072 1200 0000 728f 0000 00da 0562  ...r....r......b
+00003b30: 6c6f 636b 290b 7215 0000 00da 026c 785a  lock).r......lxZ
+00003b40: 026c 795a 026c 7ada 026e 78da 026e 795a  .lyZ.lz..nx..nyZ
+00003b50: 026e 7a72 7500 0000 5a06 6261 7365 7673  .nzru...Z.basevs
+00003b60: 727f 0000 005a 0c76 6572 7465 785f 6e61  r....Z.vertex_na
+00003b70: 6d65 73a9 01da 095f 5f63 6c61 7373 5f5f  mes....__class__
+00003b80: 7216 0000 0072 1700 0000 7218 0000 00c1  r....r....r.....
+00003b90: 0100 0073 1c00 0000 0a01 0a02 0c03 0c01  ...s............
+00003ba0: 0c01 0c01 04fc 0807 1a01 1c01 0602 0201  ................
+00003bb0: 06ff 1c04 7a21 426c 6f63 6b4d 6573 6844  ....z!BlockMeshD
+00003bc0: 6963 7452 6563 7469 6c69 6e65 6172 2e5f  ictRectilinear._
+00003bd0: 5f69 6e69 745f 5f29 0572 2900 0000 722a  _init__).r)...r*
+00003be0: 0000 0072 2b00 0000 7218 0000 00da 0d5f  ...r+...r......_
+00003bf0: 5f63 6c61 7373 6365 6c6c 5f5f 7216 0000  _classcell__r...
+00003c00: 0072 1600 0000 72bb 0000 0072 1700 0000  .r....r....r....
+00003c10: 72af 0000 00c0 0100 0073 0400 0000 0800  r........s......
+00003c20: 1401 72af 0000 004e 2917 da07 5f5f 646f  ..r....N)...__do
+00003c30: 635f 5fda 0969 7465 7274 6f6f 6c73 7202  c__..itertoolsr.
+00003c40: 0000 00da 0673 7472 696e 6772 0300 0000  .....stringr....
+00003c50: 72a9 0000 0072 0500 0000 726a 0000 0072  r....r....rj...r
+00003c60: 0700 0000 7208 0000 0072 4400 0000 7209  ....r....rD...r.
+00003c70: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
+00003c80: 0000 da07 5f5f 616c 6c5f 5f72 0d00 0000  ....__all__r....
+00003c90: 722d 0000 0072 3000 0000 7242 0000 0072  r-...r0...rB...r
+00003ca0: 5f00 0000 7267 0000 0072 af00 0000 7216  _...rg...r....r.
+00003cb0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00003cc0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00003cd0: 731e 0000 0004 000c 0c0c 010c 0210 0118  s...............
+00003ce0: 0108 020e 0a0e 1c0e 0a0e 110e 530e 2800  ............S.(.
+00003cf0: 7f14 71                                  ..q
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/edges.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/edges.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/grading.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/blockmesh/grading.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/fields.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,59 +15,60 @@
     Code,
     CodeStream,
     Dict,
     DimensionSet,
     FoamInputFile,
     List,
     Value,
-    str2foam_units,
 )
 
 DEFAULT_CODE_INCLUDE = '#include "fvCFD.H"'
 DEFAULT_CODE_OPTIONS = (
     "-I$(LIB_SRC)/finiteVolume/lnInclude \\\n-I$(LIB_SRC)/meshTools/lnInclude"
 )
 DEFAULT_CODE_LIBS = "-lmeshTools \\\n-lfiniteVolume"
 
 
 class FieldABC(ABC):
     cls: str
 
     @classmethod
-    def from_code(cls, code: str):
+    def from_code(cls, code: str, skip_boundary_field=False):
         if "nonuniform" not in code:
             tree = parse(code)
             return cls(None, None, tree=tree)
 
         index_nonuniform = code.index("nonuniform")
         index_boundaryField = code.rindex("boundaryField", index_nonuniform)
         index_opening_par = code.index("(", index_nonuniform, index_boundaryField)
         index_closing_par = code.rindex(
             ")", index_nonuniform, index_boundaryField
         )
 
-        code_to_parse = (
-            code[:index_nonuniform] + ";\n\n" + code[index_boundaryField:]
-        )
+        code_to_parse = code[:index_nonuniform] + ";\n"
+        if not skip_boundary_field:
+            code_to_parse += "\n" + code[index_boundaryField:]
 
         tree = parse(code_to_parse)
         code_data = code[index_opening_par + 1 : index_closing_par].strip()
 
         if code_data.startswith("("):
             code_data = re.sub("[()]", "", code_data)
 
         data = np.loadtxt(StringIO(code_data))
 
         tree.data = data
         return cls("", "", tree=tree, values=data)
 
     @classmethod
-    def from_path(cls, path: str or Path):
+    def from_path(cls, path: str or Path, skip_boundary_field=False):
         path = Path(path)
-        field = cls.from_code(path.read_text())
+        field = cls.from_code(
+            path.read_text(), skip_boundary_field=skip_boundary_field
+        )
         field.path = path
         return field
 
     def __init__(self, name, dimension, tree=None, values=None):
         if tree is not None:
             self.tree = tree
         else:
@@ -75,15 +76,15 @@
                 "version": "2.0",
                 "format": "ascii",
                 "class": self.cls,
                 "object": name,
             }
 
             if not isinstance(dimension, DimensionSet):
-                dimension = DimensionSet(str2foam_units(dimension))
+                dimension = DimensionSet(dimension)
 
             self.tree = FoamInputFile(
                 info, children={"dimensions": dimension, "internalField": None}
             )
 
             self.tree.set_child("boundaryField", {})
 
@@ -163,34 +164,44 @@
             if not isinstance(values, np.ndarray):
                 raise ValueError
             if values.ndim != 1 or values.size != vy.size != vz.size:
                 raise ValueError
             vx = values
             values = np.stack([vx, vy, vz]).T
 
-        if isinstance(values, np.ndarray):
-            if values.ndim != 2:
-                raise ValueError
-            values = [list(arr) for arr in values]
-
         n_elem = len(values)
         if n_elem == 3 and isinstance(values[0], Number):
             value = Value(
                 "(" + " ".join(str(value) for value in values) + ")",
                 name="uniform",
             )
         else:
-            value = List(
-                [List(value) for value in values],
-                name=f"internalField nonuniform\nList<vector>\n{n_elem}",
+            value = values
+        self.tree.set_child("internalField", value)
+
+    def get_components(self):
+        arr = self.get_array()
+        return arr[:, 0], arr[:, 1], arr[:, 2]
+
+
+class VolTensorField(FieldABC):
+    cls = "volTensorField"
+
+    def set_values(self, values):
+        if not isinstance(values, np.ndarray) or values.ndim != 2:
+            raise NotImplementedError(
+                "not isinstance(values, np.ndarray) or values.ndim != 2"
             )
-        self.tree.children["internalField"] = value
+
+        self.tree.set_child("internalField", values)
 
 
-classes = {"volScalarField": VolScalarField, "volVectorField": VolVectorField}
+classes = {
+    cls.cls: cls for cls in (VolScalarField, VolVectorField, VolTensorField)
+}
 
 
 def read_field_file(path):
     cls = None
     with open(path, "r") as file:
         for line in file:
             line = line.strip()
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/fv_schemes.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/fv_schemes.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/generators.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,34 +75,34 @@
 
     def __init__(self, output):
         super().__init__(output)
 
     def generate_code(self, params=None):
         """Generate the code of the file from ...
 
-        - a method named like `sim.output.make_code_block_mesh_dict`,
+        - a method named like `sim.output._make_code_block_mesh_dict`,
         - or a Jinja template.
         """
         if params is None:
             params = self.output.sim.params
 
         try:
-            make_code = getattr(self.output, "make_code_" + self._name)
+            make_code = getattr(self.output, "_make_code_" + self._name)
         except AttributeError:
             make_code = None
 
         if make_code is None:
             try:
-                make_tree = getattr(self.output, "make_tree_" + self._name)
+                make_tree = getattr(self.output, "_make_tree_" + self._name)
             except AttributeError:
                 make_tree = None
 
             if make_tree is None:
                 try:
-                    helper = getattr(self.output, "helper_" + self._name)
+                    helper = getattr(self.output, "_helper_" + self._name)
                 except AttributeError:
                     pass
                 else:
                     if isinstance(helper, FileHelper):
                         make_tree = helper.make_tree
 
             if make_tree is not None:
@@ -115,15 +115,15 @@
             return template.render(params=params)
 
         if (self.input_files.templates_dir / self.template_name).exists():
             raise RuntimeError(
                 "Fluidsimfoam solver issue: "
                 f"2 concurrent methods to produce {self.rel_path}:\n"
                 f"- template in {self.input_files.templates_dir},\n"
-                f"- function output.make_code_{self._name}.\n"
+                f"- function output._make_code_{self._name}.\n"
                 "Remove the file or the function (or make it equal to None)."
             )
 
         return make_code(params)
 
     @classmethod
     def _complete_params_with_default(cls, params, info_solver):
@@ -134,15 +134,15 @@
         try:
             complete_params = getattr(output_cls, "_complete_params_" + cls._name)
         except AttributeError:
             complete_params = None
 
         if complete_params is None:
             try:
-                helper = getattr(output_cls, "helper_" + cls._name)
+                helper = getattr(output_cls, "_helper_" + cls._name)
             except AttributeError:
                 pass
             else:
                 if isinstance(helper, FileHelper):
                     complete_params = helper.complete_params
 
         if complete_params is not None:
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/grammar.lark` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/grammar.lark`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 DOUBLE_NAME.1 : /[a-zA-Z_][a-zA-Z_\d]*[:\.-][:]?[a-zA-Z_\d\.]+/
 
 _list_name: CNAME|ESCAPED_STRING|DOUBLE_NAME|SIGNED_NUMBER
 _dict_name: CNAME|ESCAPED_STRING|DOUBLE_NAME|EQKEY
 _var_name : CNAME|ESCAPED_STRING|DOUBLE_NAME|EQKEY
 
 LIST_TYPE.2 : /List<[\w]+>/
-list_info : _list_name [CNAME] [ NEWLINE LIST_TYPE ] [NEWLINE SIGNED_NUMBER]
+list_info : _list_name [CNAME] [NEWLINE LIST_TYPE] [NEWLINE SIGNED_NUMBER]
 
 directive: /#[a-zA-Z]+/ | /#[a-zA-Z]+{[^}]*}/
 dimension_set : "[" (SIGNED_NUMBER)+ "]"
 _dataentry : DOUBLE_NAME | CNAME | list | ESCAPED_STRING | MACRO | directive
     | SIGNED_NUMBER | dimension_set | EQKEY
 
 list : "(" (_dataentry|NEWLINE|dict_assignment)* ")"
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/grammar_advanced.lark` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/grammar_advanced.lark`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 TRIPLE_NAME.3 :  /[a-zA-Z][a-zA-Z\d]*[:\-][a-zA-Z\d\._]+[:\-][a-zA-Z\d\._]/
 
 _list_name: CNAME|ESCAPED_STRING|DOUBLE_NAME|MACRO|SIGNED_NUMBER|EQKEY|directive
 _dict_name: CNAME|ESCAPED_STRING|DOUBLE_NAME|EQKEY|TRIPLE_NAME|list
 _var_name : CNAME|ESCAPED_STRING|DOUBLE_NAME|MACRO|EQKEY
 
 LIST_TYPE.2 : /List<[\w]+>/
-list_info : _list_name [CNAME] [NEWLINE LIST_TYPE] [NEWLINE SIGNED_NUMBER]
+list_info : _list_name [CNAME] [NEWLINE] [LIST_TYPE] [NEWLINE SIGNED_NUMBER]
 
 directive: /#[a-zA-Z]+/ | /#[a-zA-Z]+{[^}]*}/
 dimension_set : "[" (SIGNED_NUMBER)+ "]"
 _dataentry : DOUBLE_NAME | CNAME | list | ESCAPED_STRING | MACRO | directive
     | SIGNED_NUMBER | dimension_set | EQKEY
 list : "(" (_dataentry|NEWLINE|dict_assignment)* ")"
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/parser.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/parser.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/polymesh.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/foam_input_files/polymesh.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/info.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Base class for ``Simul.InfoSolver``"""
 
 from fluidsim_core.info import InfoSolverCore
 
 
 class InfoSolver(InfoSolverCore):
     """Contains the information on which classes are used in a solver"""
+
     def _init_root(self):
         super()._init_root()
 
         self.classes._set_child(
             "Output",
             attribs={
                 "module_name": "fluidsimfoam.output",
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/log.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/log.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/next_fluidsim_core.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/next_fluidsim_core.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/operators.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/operators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 """Base class for the ``sim.oper`` object"""
 
 import shutil
-from subprocess import run
+from subprocess import PIPE, run
 
-from fluidsimfoam.foam_input_files.fields import VolScalarField
+from fluidsimfoam.foam_input_files.fields import VolVectorField
 
 
 class Operators:
     def __init__(self, sim):
         self.sim = sim
 
         if hasattr(sim.output.input_files, "block_mesh_dict"):
             assert (sim.output.path_run / "system/blockMeshDict").exists()
 
     def get_cells_coords(self):
-        path_cx = self.sim.path_run / "0/Cx"
+        path_c = self.sim.path_run / "0/C"
 
-        if not path_cx.exists():
+        if not path_c.exists():
             path_polymesh = self.sim.path_run / "constant/polyMesh/points"
 
             if not path_polymesh.exists():
-                self.sim.make.exec("polymesh")
+                self.sim.make.exec("polymesh", stdout=PIPE)
 
             if not path_polymesh.exists():
                 raise RuntimeError(f"{path_polymesh} does not exists")
 
             path_postProcess = shutil.which("postProcess")
 
             if path_postProcess is None:
                 raise RuntimeError("OpenFOAM not available")
 
             run(
                 ["postProcess", "-func", "writeCellCentres"],
                 cwd=self.sim.path_run,
+                stdout=PIPE,
             )
 
-        def get_arr(path):
-            field = VolScalarField.from_path(path)
-            return field.get_array()
-
-        path_cy = path_cx.with_name("Cy")
-        path_cz = path_cx.with_name("Cz")
-
-        return get_arr(path_cx), get_arr(path_cy), get_arr(path_cz)
+        field = VolVectorField.from_path(path_c, skip_boundary_field=True)
+        return field.get_components()
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 09:29:43 2023 UTC, .py size: 9206 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,477 +1,489 @@
-00000000: 6f0d 0d0a 0000 0000 8712 5a64 f623 0000  o.........Zd.#..
+00000000: 6f0d 0d0a 0000 0000 5dcf 6364 6625 0000  o.......].cdf%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
-00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6407 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6408 6c0f 6d10 5a10 6d11 5a11 6d12 5a12  d.l.m.Z.m.Z.m.Z.
-000000a0: 6d13 5a13 0100 6400 6409 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
-000000b0: 6d16 5a16 0100 6400 640a 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
-000000c0: 0100 6400 640b 6c19 6d1a 5a1a 0100 4700  ..d.d.l.m.Z...G.
-000000d0: 640c 640d 8400 640d 650c 8303 5a1b 6401  d.d...d.e...Z.d.
-000000e0: 5300 290e e900 0000 004e 2901 da04 5061  S.)......N)...Pa
-000000f0: 7468 a901 da0a 756e 6465 7273 636f 7265  th....underscore
-00000100: 2901 da11 7374 646f 7574 5f72 6564 6972  )...stdout_redir
-00000110: 6563 7465 6429 01da 036d 7069 2901 da0a  ected)...mpi)...
-00000120: 4f75 7470 7574 436f 7265 2901 da14 6974  OutputCore)...it
-00000130: 6572 5f63 6f6d 706c 6574 655f 7061 7261  er_complete_para
-00000140: 6d73 2904 da14 4445 4641 554c 545f 434f  ms)...DEFAULT_CO
-00000150: 4e54 524f 4c5f 4449 4354 da0e 4445 4641  NTROL_DICT..DEFA
-00000160: 554c 545f 4845 4144 4552 da12 436f 6e73  ULT_HEADER..Cons
-00000170: 7461 6e74 4669 6c65 4865 6c70 6572 da0d  tantFileHelper..
-00000180: 466f 616d 496e 7075 7446 696c 6529 02da  FoamInputFile)..
-00000190: 0a49 6e70 7574 4669 6c65 73da 186e 6577  .InputFiles..new
-000001a0: 5f66 696c 655f 6765 6e65 7261 746f 725f  _file_generator_
-000001b0: 636c 6173 7329 01da 066c 6f67 6765 7229  class)...logger)
-000001c0: 01da 1267 6574 5f73 6f6c 7665 725f 7061  ...get_solver_pa
-000001d0: 636b 6167 6563 0000 0000 0000 0000 0000  ckagec..........
-000001e0: 0000 0000 0000 0400 0000 0000 0000 73c0  ..............s.
-000001f0: 0000 0065 005a 0164 005a 0264 0164 0267  ...e.Z.d.Z.d.d.g
-00000200: 025a 0364 0364 0467 025a 0467 0064 05a2  .Z.d.d.g.Z.g.d..
-00000210: 015a 0565 065a 0765 0864 0464 0664 0769  .Z.e.Z.e.d.d.d.i
-00000220: 0183 025a 0965 0a64 0864 0984 0083 015a  ...Z.e.d.d.....Z
-00000230: 0b65 0a64 0a64 0b84 0083 015a 0c65 0a64  .e.d.d.....Z.e.d
-00000240: 0c64 0d84 0083 015a 0d65 0a64 0e64 0f84  .d.....Z.e.d.d..
-00000250: 0083 015a 0e64 2187 0066 0164 1164 1284  ...Z.d!..f.d.d..
-00000260: 095a 0f65 0a64 1364 1484 0083 015a 1087  .Z.e.d.d.....Z..
-00000270: 0066 0164 1564 1684 085a 1164 1764 1884  .f.d.d...Z.d.d..
-00000280: 005a 1265 0a64 1964 1a84 0083 015a 1364  .Z.e.d.d.....Z.d
-00000290: 1b64 1c84 005a 1464 1d64 1e84 005a 1565  .d...Z.d.d...Z.e
-000002a0: 0a64 1f64 2084 0083 015a 1687 0004 005a  .d.d ....Z.....Z
-000002b0: 1753 0029 22da 064f 7574 7075 74da 0170  .S.)"..Output..p
-000002c0: da01 55da 1374 7261 6e73 706f 7274 5072  ..U..transportPr
-000002d0: 6f70 6572 7469 6573 da14 7475 7262 756c  operties..turbul
-000002e0: 656e 6365 5072 6f70 6572 7469 6573 2903  enceProperties).
-000002f0: da0b 636f 6e74 726f 6c44 6963 74da 0966  ..controlDict..f
-00000300: 7653 6368 656d 6573 5a0a 6676 536f 6c75  vSchemesZ.fvSolu
-00000310: 7469 6f6e da0e 7369 6d75 6c61 7469 6f6e  tion..simulation
-00000320: 5479 7065 da07 6c61 6d69 6e61 7263 0200  Type..laminarc..
-00000330: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00000340: 0000 4300 0000 7328 0000 007c 016a 006a  ..C...s(...|.j.j
-00000350: 01a0 0264 01a1 017d 027c 00a0 037c 02a1  ...d...}.|...|..
-00000360: 0101 007c 016a 006a 01a0 04a1 0001 0064  ...|.j.j.......d
-00000370: 0253 0029 037a 6643 6f6d 706c 6574 6520  .S.).zfComplete 
-00000380: 7468 6520 696e 666f 5f73 6f6c 7665 7220  the info_solver 
-00000390: 696e 7374 616e 6365 2077 6974 6820 6368  instance with ch
-000003a0: 696c 6420 636c 6173 7320 6465 7461 696c  ild class detail
-000003b0: 7320 286d 6f64 756c 650a 2020 2020 2020  s (module.      
-000003c0: 2020 616e 6420 636c 6173 7320 6e61 6d65    and class name
-000003d0: 7329 2e0a 0a20 2020 2020 2020 20da 0763  s)...        ..c
-000003e0: 6c61 7373 6573 4e29 0572 1a00 0000 7211  lassesN).r....r.
-000003f0: 0000 00da 0a5f 7365 745f 6368 696c 64da  ....._set_child.
-00000400: 185f 7365 745f 696e 666f 5f73 6f6c 7665  ._set_info_solve
-00000410: 725f 636c 6173 7365 73da 1563 6f6d 706c  r_classes..compl
-00000420: 6574 655f 7769 7468 5f63 6c61 7373 6573  ete_with_classes
-00000430: 2903 da03 636c 73da 0b69 6e66 6f5f 736f  )...cls..info_so
-00000440: 6c76 6572 721a 0000 00a9 0072 2000 0000  lverr......r ...
-00000450: fa3d 2f68 6f6d 652f 7069 6572 7265 2f44  .=/home/pierre/D
-00000460: 6576 2f66 6c75 6964 7369 6d66 6f61 6d2f  ev/fluidsimfoam/
-00000470: 7372 632f 666c 7569 6473 696d 666f 616d  src/fluidsimfoam
-00000480: 2f6f 7574 7075 742f 6261 7365 2e70 79da  /output/base.py.
-00000490: 155f 636f 6d70 6c65 7465 5f69 6e66 6f5f  ._complete_info_
-000004a0: 736f 6c76 6572 2400 0000 7306 0000 000e  solver$...s.....
-000004b0: 060a 0110 027a 1c4f 7574 7075 742e 5f63  .....z.Output._c
-000004c0: 6f6d 706c 6574 655f 696e 666f 5f73 6f6c  omplete_info_sol
-000004d0: 7665 7263 0200 0000 0000 0000 0000 0000  verc............
-000004e0: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
-000004f0: 0064 0153 0029 027a 2e53 6574 2074 6865  .d.S.).z.Set the
-00000500: 2063 6c61 7373 6573 2066 6f72 2069 6e66   classes for inf
-00000510: 6f5f 736f 6c76 6572 2e63 6c61 7373 6573  o_solver.classes
-00000520: 2e4f 7574 7075 744e 7220 0000 0029 0272  .OutputNr ...).r
-00000530: 1e00 0000 721a 0000 0072 2000 0000 7220  ....r....r ...r 
-00000540: 0000 0072 2100 0000 721c 0000 002f 0000  ...r!...r..../..
-00000550: 0073 0200 0000 0400 7a1f 4f75 7470 7574  .s......z.Output
-00000560: 2e5f 7365 745f 696e 666f 5f73 6f6c 7665  ._set_info_solve
-00000570: 725f 636c 6173 7365 7363 0100 0000 0000  r_classesc......
-00000580: 0000 0000 0000 0400 0000 0700 0000 4300  ..............C.
-00000590: 0000 7362 0000 0069 0004 007d 017c 005f  ..sb...i...}.|._
-000005a0: 007c 006a 0144 005d 0c7d 0274 027c 0283  .|.j.D.].}.t.|..
-000005b0: 017c 017c 02a0 0364 0164 02a1 023c 0071  .|.|...d.d...<.q
-000005c0: 087c 006a 0444 005d 097d 0374 027c 0364  .|.j.D.].}.t.|.d
-000005d0: 0383 027c 017c 033c 0071 187c 006a 0544  ...|.|.<.q.|.j.D
-000005e0: 005d 097d 0374 027c 0364 0483 027c 017c  .].}.t.|.d...|.|
-000005f0: 033c 0071 2564 0053 0029 054e da01 2eda  .<.q%d.S.).N....
-00000600: 015f da08 636f 6e73 7461 6e74 da06 7379  ._..constant..sy
-00000610: 7374 656d 2906 da18 5f66 696c 655f 6765  stem)..._file_ge
-00000620: 6e65 7261 746f 7273 5f63 6c61 7373 6573  nerators_classes
-00000630: da0e 7661 7269 6162 6c65 5f6e 616d 6573  ..variable_names
-00000640: 720e 0000 00da 0772 6570 6c61 6365 da14  r......replace..
-00000650: 636f 6e73 7461 6e74 5f66 696c 6573 5f6e  constant_files_n
-00000660: 616d 6573 da12 7379 7374 656d 5f66 696c  ames..system_fil
-00000670: 6573 5f6e 616d 6573 2904 721e 0000 0072  es_names).r....r
-00000680: 1a00 0000 5a0d 7661 7269 6162 6c65 5f6e  ....Z.variable_n
-00000690: 616d 65da 0966 696c 655f 6e61 6d65 7220  ame..file_namer 
-000006a0: 0000 0072 2000 0000 7221 0000 00da 1e5f  ...r ...r!....._
-000006b0: 7365 7475 705f 6669 6c65 5f67 656e 6572  setup_file_gener
-000006c0: 6174 6f72 735f 636c 6173 7365 7333 0000  ators_classes3..
-000006d0: 0073 1400 0000 0a02 0a01 0201 0201 12ff  .s..............
-000006e0: 0a04 1001 0a02 1001 04ff 7a25 4f75 7470  ..........z%Outp
-000006f0: 7574 2e5f 7365 7475 705f 6669 6c65 5f67  ut._setup_file_g
-00000700: 656e 6572 6174 6f72 735f 636c 6173 7365  enerators_classe
-00000710: 7363 0300 0000 0000 0000 0000 0000 0400  sc..............
-00000720: 0000 0600 0000 4300 0000 7372 0000 007c  ......C...sr...|
-00000730: 00a0 00a1 0001 0074 017c 017c 027c 006a  .......t.|.|.|.j
-00000740: 02a0 03a1 0083 0301 007c 01a0 0474 0564  .........|...t.d
-00000750: 0164 0264 038d 02a1 0101 007c 016a 0664  .d.d.......|.j.d
-00000760: 0464 0164 0564 069c 0264 078d 0201 007c  .d.d.d...d.....|
-00000770: 016a 07a0 0874 09a0 0a64 08a1 01a1 0101  .j...t...d......
-00000780: 007c 026a 0b6a 0ca0 0da1 007d 0374 017c  .|.j.j.....}.t.|
-00000790: 017c 027c 03a0 03a1 0083 0301 0064 0953  .|.|.........d.S
-000007a0: 0029 0a7a 3e54 6869 7320 7374 6174 6963  .).z>This static
-000007b0: 206d 6574 686f 6420 6973 2075 7365 6420   method is used 
-000007c0: 746f 2063 6f6d 706c 6574 6520 7468 6520  to complete the 
-000007d0: 2a70 6172 616d 732a 2063 6f6e 7461 696e  *params* contain
-000007e0: 6572 2e54 da03 7275 6e29 02da 0f4e 4557  er.T..run)...NEW
-000007f0: 5f44 4952 5f52 4553 554c 5453 5a13 7368  _DIR_RESULTSZ.sh
-00000800: 6f72 745f 6e61 6d65 5f74 7970 655f 7275  ort_name_type_ru
-00000810: 6eda 066f 7574 7075 74da 0029 02da 0b48  n..output..)...H
-00000820: 4153 5f54 4f5f 5341 5645 da0d 7375 625f  AS_TO_SAVE..sub_
-00000830: 6469 7265 6374 6f72 7929 01da 0761 7474  directory)...att
-00000840: 7269 6273 612e 0100 000a 2020 2020 2d20  ribsa.....    - 
-00000850: 6060 4841 535f 544f 5f53 4156 4560 603a  ``HAS_TO_SAVE``:
-00000860: 2062 6f6f 6c20 2864 6566 6175 6c74 3a20   bool (default: 
-00000870: 5472 7565 2920 4966 2046 616c 7365 2c20  True) If False, 
-00000880: 6e6f 7468 696e 6720 6e65 7720 6973 2073  nothing new is s
-00000890: 6176 6564 2069 6e0a 2020 2020 2020 7468  aved in.      th
-000008a0: 6520 6469 7265 6374 6f72 7920 6f66 2074  e directory of t
-000008b0: 6865 2073 696d 756c 6174 696f 6e2e 0a20  he simulation.. 
-000008c0: 2020 202d 2060 6073 7562 5f64 6972 6563     - ``sub_direc
-000008d0: 746f 7279 6060 3a20 7374 7220 2864 6566  tory``: str (def
-000008e0: 6175 6c74 3a20 2222 2920 4120 6e61 6d65  ault: "") A name
-000008f0: 206f 6620 6120 7375 622d 6469 7265 6374   of a sub-direct
-00000900: 6f72 7920 2872 656c 6174 6976 650a 2020  ory (relative.  
-00000910: 2020 2020 746f 2024 464c 5549 4444 594e      to $FLUIDDYN
-00000920: 5f50 4154 485f 5343 5241 5443 4829 2077  _PATH_SCRATCH) w
-00000930: 6865 7265 696e 2074 6865 2064 6972 6563  herein the direc
-00000940: 746f 7279 206f 6620 7468 6520 7369 6d75  tory of the simu
-00000950: 6c61 7469 6f6e 0a20 2020 2020 2028 6060  lation.      (``
-00000960: 7061 7468 5f72 756e 6060 2920 6973 2073  path_run``) is s
-00000970: 6176 6564 2e0a 0a4e 290e 722d 0000 0072  aved...N).r-...r
-00000980: 0800 0000 7227 0000 00da 0676 616c 7565  ....r'.....value
-00000990: 73da 0c5f 7365 745f 6174 7472 6962 73da  s.._set_attribs.
-000009a0: 0464 6963 7472 1b00 0000 7230 0000 00da  .dictr....r0....
-000009b0: 085f 7365 745f 646f 63da 0874 6578 7477  ._set_doc..textw
-000009c0: 7261 70da 0664 6564 656e 7472 1a00 0000  rap..dedentr....
-000009d0: 7211 0000 00da 0e69 6d70 6f72 745f 636c  r......import_cl
-000009e0: 6173 7365 7329 0472 1e00 0000 da06 7061  asses).r......pa
-000009f0: 7261 6d73 721f 0000 00da 0c64 6963 745f  ramsr......dict_
-00000a00: 636c 6173 7365 7372 2000 0000 7220 0000  classesr ...r ..
-00000a10: 0072 2100 0000 da1d 5f63 6f6d 706c 6574  .r!....._complet
-00000a20: 655f 7061 7261 6d73 5f77 6974 685f 6465  e_params_with_de
-00000a30: 6661 756c 7441 0000 0073 1e00 0000 0804  faultA...s......
-00000a40: 0201 0c01 04ff 1205 0401 0a01 06ff 0603  ................
-00000a50: 0401 0201 02ff 04ff 0c0d 1401 7a24 4f75  ............z$Ou
-00000a60: 7470 7574 2e5f 636f 6d70 6c65 7465 5f70  tput._complete_p
-00000a70: 6172 616d 735f 7769 7468 5f64 6566 6175  arams_with_defau
-00000a80: 6c74 4e63 0300 0000 0000 0000 0000 0000  ltNc............
-00000a90: 0b00 0000 0800 0000 0300 0000 733c 0200  ............s<..
-00000aa0: 007c 017c 005f 007a 087c 016a 016a 026a  .|.|._.z.|.j.j.j
-00000ab0: 037c 005f 0457 006e 0904 0074 0579 1401  .|._.W.n...t.y..
-00000ac0: 0001 0001 0059 006e 0777 0074 067c 006a  .....Y.n.w.t.|.j
-00000ad0: 0483 017c 005f 077c 00a0 08a1 007c 005f  ...|._.|.....|._
-00000ae0: 097c 0172 2e7c 016a 0a6a 0b7c 005f 0a74  .|.r.|.j.j.|._.t
-00000af0: 0c83 00a0 0d7c 01a1 0101 006e 0f7c 0272  .....|.....n.|.r
-00000b00: 357c 026a 0b7c 005f 0a6e 0864 007c 005f  5|.j.|._.n.d.|._
-00000b10: 0a74 0ea0 0f64 01a1 0101 007c 0173 4164  .t...d.....|.sAd
-00000b20: 0053 0074 107c 006a 1183 017c 005f 1174  .S.t.|.j...|._.t
-00000b30: 127c 0083 017c 005f 137c 016a 016a 026a  .|...|._.|.j.j.j
-00000b40: 146a 15a0 16a1 007d 037c 03a0 17a1 0044  .j.....}.|.....D
-00000b50: 005d 265c 027d 047d 0574 187c 007c 0583  .]&\.}.}.t.|.|..
-00000b60: 0272 6271 5874 197c 0483 017d 067c 006a  .rbqXt.|...}.|.j
-00000b70: 0004 006a 1a64 02a0 1b64 037c 069b 0064  ...j.d...d.|...d
-00000b80: 049d 037c 05a1 0237 0002 005f 1a74 1c7c  ...|...7..._.t.|
-00000b90: 007c 067c 057c 0083 0183 0301 0071 5874  .|.|.|.......qXt
-00000ba0: 1d7c 0064 0583 0273 887c 00a0 1ea1 0001  .|.d...s.|......
-00000bb0: 0069 007d 077c 006a 1fa0 17a1 0044 005d  .i.}.|.j.....D.]
-00000bc0: 255c 027d 047d 0574 197c 0483 017d 067c  %\.}.}.t.|...}.|
-00000bd0: 056a 207c 0776 0172 a37c 0467 017c 077c  .j |.v.r.|.g.|.|
-00000be0: 056a 203c 006e 087c 077c 056a 2019 00a0  .j <.n.|.|.j ...
-00000bf0: 217c 04a1 0101 0074 1c7c 006a 137c 067c  !|.....t.|.j.|.|
-00000c00: 057c 0083 0183 0301 0071 8f7c 0772 dc7c  .|.......q.|.r.|
-00000c10: 006a 0004 006a 1a64 0637 0002 005f 1a7c  .j...j.d.7..._.|
-00000c20: 07a0 17a1 0044 005d 185c 027d 087d 097c  .....D.].\.}.}.|
-00000c30: 006a 0004 006a 1a64 077c 0864 0817 0064  .j...j.d.|.d...d
-00000c40: 099b 0464 0aa0 227c 09a1 019b 0064 0b9d  ...d.."|.....d..
-00000c50: 0437 0002 005f 1a71 c374 236a 2464 0c6b  .7..._.q.t#j$d.k
-00000c60: 0272 e97c 006a 2572 e97c 006a 006a 0a6a  .r.|.j%r.|.j.j.j
-00000c70: 2673 eb64 0053 007c 006a 1164 0d1b 00a0  &s.d.S.|.j.d....
-00000c80: 27a1 0001 007c 006a 1164 0e1b 00a0 27a1  '....|.j.d....'.
-00000c90: 0001 007c 006a 1164 0f1b 00a0 27a1 0001  ...|.j.d....'...
-00000ca0: 0074 287c 006a 1383 01a0 29a1 0044 005d  .t(|.j....)..D.]
-00000cb0: 147d 0a74 1d7c 0a64 1083 0290 0172 1a7c  .}.t.|.d.....r.|
-00000cc0: 0a6a 2aa0 2b64 0da1 0190 0172 1a7c 0aa0  .j*.+d.....r.|..
-00000cd0: 2ca1 0001 0090 0171 0764 0053 0029 114e  ,......q.d.S.).N
-00000ce0: 7a45 496e 6974 6961 6c69 7a69 6e67 204f  zEInitializing O
-00000cf0: 7574 7075 7420 636c 6173 7320 7769 7468  utput class with
-00000d00: 6f75 7420 7369 6d20 6f72 2070 6172 616d  out sim or param
-00000d10: 7320 6d69 6768 7420 6c65 6164 2074 6f20  s might lead to 
-00000d20: 6572 726f 7273 2e7a 097b 3a32 3873 7d7b  errors.z.{:28s}{
-00000d30: 7d0a 7a0b 7369 6d2e 6f75 7470 7574 2e7a  }.z.sim.output.z
-00000d40: 023a 2072 2700 0000 7a0d 696e 7075 745f  .: r'...z.input_
-00000d50: 6669 6c65 733a 0a7a 0720 202d 2069 6e20  files:.z.  - in 
-00000d60: fa01 3a5a 0331 3273 da01 20da 010a 7201  ..:Z.12s.. ...r.
-00000d70: 0000 0072 2600 0000 da01 3072 2500 0000  ...r&.....0r%...
-00000d80: da0d 6765 6e65 7261 7465 5f66 696c 6529  ..generate_file)
-00000d90: 2dda 0373 696d da04 696e 666f da06 736f  -..sim..info..so
-00000da0: 6c76 6572 da0a 7368 6f72 745f 6e61 6d65  lver..short_name
-00000db0: da0b 6e61 6d65 5f73 6f6c 7665 72da 0e41  ..name_solver..A
-00000dc0: 7474 7269 6275 7465 4572 726f 7272 1000  ttributeErrorr..
-00000dd0: 0000 da07 7061 636b 6167 65da 1767 6574  ....package..get
-00000de0: 5f70 6174 685f 736f 6c76 6572 5f70 6163  _path_solver_pac
-00000df0: 6b61 6765 5a13 7061 7468 5f73 6f6c 7665  kageZ.path_solve
-00000e00: 725f 7061 636b 6167 6572 3c00 0000 7230  r_packager<...r0
-00000e10: 0000 00da 0573 7570 6572 da08 5f5f 696e  .....super..__in
-00000e20: 6974 5f5f 720f 0000 00da 0777 6172 6e69  it__r......warni
-00000e30: 6e67 7202 0000 00da 0870 6174 685f 7275  ngr......path_ru
-00000e40: 6e72 0d00 0000 da0b 696e 7075 745f 6669  nr......input_fi
-00000e50: 6c65 7372 1a00 0000 7211 0000 0072 3b00  lesr....r....r;.
-00000e60: 0000 da05 6974 656d 73da 0a69 7369 6e73  ....items..isins
-00000e70: 7461 6e63 6572 0400 0000 da11 5f6f 626a  tancer......_obj
-00000e80: 6563 7473 5f74 6f5f 7072 696e 74da 0666  ects_to_print..f
-00000e90: 6f72 6d61 74da 0773 6574 6174 7472 da07  ormat..setattr..
-00000ea0: 6861 7361 7474 7272 2d00 0000 7227 0000  hasattrr-...r'..
-00000eb0: 00da 0864 6972 5f6e 616d 65da 0661 7070  ...dir_name..app
-00000ec0: 656e 64da 046a 6f69 6e72 0600 0000 da04  end..joinr......
-00000ed0: 7261 6e6b da0c 5f68 6173 5f74 6f5f 7361  rank.._has_to_sa
-00000ee0: 7665 722f 0000 00da 056d 6b64 6972 da04  ver/.....mkdir..
-00000ef0: 7661 7273 7235 0000 00da 0872 656c 5f70  varsr5.....rel_p
-00000f00: 6174 68da 0a73 7461 7274 7377 6974 6872  ath..startswithr
-00000f10: 4300 0000 290b da04 7365 6c66 7244 0000  C...)...selfrD..
-00000f20: 0072 3c00 0000 723d 0000 00da 0863 6c73  .r<...r=.....cls
-00000f30: 5f6e 616d 65da 0543 6c61 7373 da08 6f62  _name..Class..ob
-00000f40: 6a5f 6e61 6d65 5a13 666f 725f 7374 725f  j_nameZ.for_str_
-00000f50: 696e 7075 745f 6669 6c65 7372 5700 0000  input_filesrW...
-00000f60: 7250 0000 00da 0e66 696c 655f 6765 6e65  rP.....file_gene
-00000f70: 7261 746f 72a9 01da 095f 5f63 6c61 7373  rator....__class
-00000f80: 5f5f 7220 0000 0072 2100 0000 724d 0000  __r ...r!...rM..
-00000f90: 005f 0000 0073 8000 0000 0601 0201 1001  ._...s..........
-00000fa0: 0c01 0401 02ff 0c03 0a02 0402 0a02 0e01  ................
-00000fb0: 0401 0a02 0602 0401 0201 04ff 0404 0401  ................
-00000fc0: 0c02 0a02 1002 1001 0a01 0201 0801 0c01  ................
-00000fd0: 0c01 08ff 1203 0a02 0801 0401 1201 0801  ................
-00000fe0: 0a02 0e01 1002 1401 0402 1001 1001 0801  ................
-00000ff0: 1a01 08ff 0805 02ff 0402 02fe 0803 02fd  ................
-00001000: 0405 0e02 0e01 0e01 1202 0201 0401 06ff  ................
-00001010: 0a02 04fe 0803 0480 04fc 7a0f 4f75 7470  ..........z.Outp
-00001020: 7574 2e5f 5f69 6e69 745f 5f63 0100 0000  ut.__init__c....
-00001030: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00001040: 4300 0000 7312 0000 0074 0074 01a0 027c  C...s....t.t...|
-00001050: 00a1 016a 0383 016a 0453 0029 017a 2847  ...j...j.S.).z(G
-00001060: 6574 2074 6865 2070 6174 6820 746f 7761  et the path towa
-00001070: 7264 7320 7468 6520 736f 6c76 6572 2070  rds the solver p
-00001080: 6163 6b61 6765 2e29 0572 0200 0000 da07  ackage.).r......
-00001090: 696e 7370 6563 74da 0967 6574 6d6f 6475  inspect..getmodu
-000010a0: 6c65 da08 5f5f 6669 6c65 5f5f da06 7061  le..__file__..pa
-000010b0: 7265 6e74 2901 721e 0000 0072 2000 0000  rent).r....r ...
-000010c0: 7220 0000 0072 2100 0000 724b 0000 00ac  r ...r!...rK....
-000010d0: 0000 0073 0200 0000 1203 7a1e 4f75 7470  ...s......z.Outp
-000010e0: 7574 2e67 6574 5f70 6174 685f 736f 6c76  ut.get_path_solv
-000010f0: 6572 5f70 6163 6b61 6765 6301 0000 0000  er_packagec.....
-00001100: 0000 0000 0000 0005 0000 0008 0000 0003  ................
-00001110: 0000 0073 c800 0000 7400 6a01 6401 6b02  ...s....t.j.d.k.
-00001120: 720d 7402 6402 7c00 6a03 9b00 9d02 8301  r.t.d.|.j.......
-00001130: 0100 7404 8300 8f0d 0100 7405 8300 a006  ..t.......t.....
-00001140: a100 0100 5700 6403 0400 0400 8303 0100  ....W.d.........
-00001150: 6e08 3100 7320 7701 0100 0100 0100 5900  n.1.s w.......Y.
-00001160: 0100 7407 a008 7c00 6a09 6a0a a101 0100  ..t...|.j.j.....
-00001170: 7400 6a01 6401 6b02 723d 7c00 6a0b 723d  t.j.d.k.r=|.j.r=
-00001180: 7c00 6a09 6a0c 6a0d 723d 7c00 a00e a100  |.j.j.j.r=|.....
-00001190: 0100 740f 7c00 6a03 8301 7d01 7c01 6404  ..t.|.j...}.|.d.
-000011a0: 1b00 7d02 7c02 6a10 6405 6406 8d01 0100  ..}.|.j.d.d.....
-000011b0: 6407 4400 5d13 7d03 7c02 7c03 1b00 7d04  d.D.].}.|.|...}.
-000011c0: 7c04 a011 a100 7259 714e 7412 a013 7c01  |.....rYqNt...|.
-000011d0: 7c03 1b00 7c04 a102 0100 714e 6403 5300  |...|.....qNd.S.
-000011e0: 2908 7a21 4c6f 6773 2069 6e66 6f20 6f6e  ).z!Logs info on
-000011f0: 2069 6e73 7461 6e74 6961 7465 6420 636c   instantiated cl
-00001200: 6173 7365 7372 0100 0000 7a0a 7061 7468  assesr....z.path
-00001210: 5f72 756e 3a20 4e7a 0e2e 6461 7461 5f66  _run: Nz..data_f
-00001220: 6c75 6964 7369 6d54 2901 da08 6578 6973  luidsimT)...exis
-00001230: 745f 6f6b 2902 7a0f 696e 666f 5f73 6f6c  t_ok).z.info_sol
-00001240: 7665 722e 786d 6c7a 1070 6172 616d 735f  ver.xmlz.params_
-00001250: 7369 6d75 6c2e 786d 6c29 1472 0600 0000  simul.xml).r....
-00001260: 725a 0000 00da 0570 7269 6e74 724f 0000  rZ.....printrO..
-00001270: 0072 0500 0000 724c 0000 00da 0970 6f73  .r....rL.....pos
-00001280: 745f 696e 6974 720f 0000 0072 4500 0000  t_initr....rE...
-00001290: 7244 0000 0072 5300 0000 725b 0000 0072  rD...rS...r[...r
-000012a0: 3c00 0000 722f 0000 00da 2870 6f73 745f  <...r/....(post_
-000012b0: 696e 6974 5f63 7265 6174 655f 6164 6469  init_create_addi
-000012c0: 7469 6f6e 616c 5f73 6f75 7263 655f 6669  tional_source_fi
-000012d0: 6c65 7372 0200 0000 725c 0000 00da 0665  lesr....r\.....e
-000012e0: 7869 7374 73da 0673 6875 7469 6cda 0463  xists..shutil..c
-000012f0: 6f70 7929 0572 6000 0000 724f 0000 005a  opy).r`...rO...Z
-00001300: 1270 6174 685f 696e 666f 5f66 6c75 6964  .path_info_fluid
-00001310: 7369 6d72 2c00 0000 5a08 7061 7468 5f6e  simr,...Z.path_n
-00001320: 6577 7265 0000 0072 2000 0000 7221 0000  ewre...r ...r!..
-00001330: 0072 6d00 0000 b100 0000 732c 0000 000a  .rm.......s,....
-00001340: 0310 0108 030c 011c ff0e 0308 0402 ff04  ................
-00001350: 0202 fe08 0302 fd08 050a 0308 010c 0108  ................
-00001360: 0108 0108 0102 0112 0104 fc7a 104f 7574  ...........z.Out
-00001370: 7075 742e 706f 7374 5f69 6e69 7463 0100  put.post_initc..
-00001380: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00001390: 0000 4300 0000 736c 0000 007c 006a 006a  ..C...sl...|.j.j
-000013a0: 0164 011b 007d 017c 01a0 02a1 0073 1374  .d...}.|.....s.t
-000013b0: 0364 027c 006a 006a 019b 009d 0283 0182  .d.|.j.j........
-000013c0: 0174 04a0 057c 017c 006a 066a 07a1 0201  .t...|.|.j.j....
-000013d0: 0074 087c 006a 0083 01a0 09a1 0044 005d  .t.|.j.......D.]
-000013e0: 117d 0274 0a7c 0264 0383 0272 337c 026a  .}.t.|.d...r3|.j
-000013f0: 0ba0 0c64 04a1 0173 337c 02a0 0da1 0001  ...d...s3|......
-00001400: 0071 2264 0553 0029 067a 2443 7265 6174  .q"d.S.).z$Creat
-00001410: 6520 7468 6520 6669 6c65 7320 6672 6f6d  e the files from
-00001420: 2074 6865 6972 2074 656d 706c 6174 657a   their templatez
-00001430: 0874 6173 6b73 2e70 797a 2974 6173 6b73  .tasks.pyz)tasks
-00001440: 2e70 7920 6d69 7373 696e 6720 696e 2073  .py missing in s
-00001450: 6f6c 7665 7220 7465 6d70 6c61 7465 735f  olver templates_
-00001460: 6469 7220 7243 0000 0072 2600 0000 4e29  dir rC...r&...N)
-00001470: 0e72 5000 0000 5a0d 7465 6d70 6c61 7465  .rP...Z.template
-00001480: 735f 6469 7272 6f00 0000 da0c 5275 6e74  s_dirro.....Runt
-00001490: 696d 6545 7272 6f72 7270 0000 0072 7100  imeErrorrp...rq.
-000014a0: 0000 7244 0000 0072 4f00 0000 725d 0000  ..rD...rO...r]..
-000014b0: 0072 3500 0000 7256 0000 0072 5e00 0000  .r5...rV...r^...
-000014c0: 725f 0000 0072 4300 0000 2903 7260 0000  r_...rC...).r`..
-000014d0: 005a 0d70 6174 685f 7461 736b 735f 7079  .Z.path_tasks_py
-000014e0: 7264 0000 0072 2000 0000 7220 0000 0072  rd...r ...r ...r
-000014f0: 2100 0000 726e 0000 00cf 0000 0073 2200  !...rn.......s".
-00001500: 0000 0c02 0801 0201 0201 0601 04ff 04ff  ................
-00001510: 1004 1202 0201 0401 04ff 0a02 02fe 0804  ................
-00001520: 0280 04fb 7a2f 4f75 7470 7574 2e70 6f73  ....z/Output.pos
-00001530: 745f 696e 6974 5f63 7265 6174 655f 6164  t_init_create_ad
-00001540: 6469 7469 6f6e 616c 5f73 6f75 7263 655f  ditional_source_
-00001550: 6669 6c65 7363 0200 0000 0000 0000 0000  filesc..........
-00001560: 0000 0300 0000 0500 0000 4300 0000 7328  ..........C...s(
-00001570: 0000 0064 0164 0284 007c 006a 00a0 01a1  ...d.d...|.j....
-00001580: 0044 0083 017d 027c 016a 0264 037c 0264  .D...}.|.j.d.|.d
-00001590: 0464 058d 0301 0064 0053 0029 064e 6301  .d.....d.S.).Nc.
-000015a0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000015b0: 0000 0053 0000 0073 1a00 0000 6900 7c00  ...S...s....i.|.
-000015c0: 5d09 5c02 7d01 7d02 7400 7c01 8301 7c02  ].\.}.}.t.|...|.
-000015d0: 9302 7102 5300 7220 0000 0072 0300 0000  ..q.S.r ...r....
-000015e0: 2903 da02 2e30 da03 6b65 79da 0576 616c  )....0..key..val
-000015f0: 7565 7220 0000 0072 2000 0000 7221 0000  uer ...r ...r!..
-00001600: 00da 0a3c 6469 6374 636f 6d70 3ee2 0000  ...<dictcomp>...
-00001610: 0073 0800 0000 0600 0602 08ff 06ff 7a38  .s............z8
-00001620: 4f75 7470 7574 2e5f 636f 6d70 6c65 7465  Output._complete
-00001630: 5f70 6172 616d 735f 636f 6e74 726f 6c5f  _params_control_
-00001640: 6469 6374 2e3c 6c6f 6361 6c73 3e2e 3c64  dict.<locals>.<d
-00001650: 6963 7463 6f6d 703e da0c 636f 6e74 726f  ictcomp>..contro
-00001660: 6c5f 6469 6374 7a3d 5365 6520 6874 7470  l_dictz=See http
-00001670: 733a 2f2f 646f 632e 6366 642e 6469 7265  s://doc.cfd.dire
-00001680: 6374 2f6f 7065 6e66 6f61 6d2f 7573 6572  ct/openfoam/user
-00001690: 2d67 7569 6465 2d76 362f 636f 6e74 726f  -guide-v6/contro
-000016a0: 6c64 6963 74a9 0272 3400 0000 da03 646f  ldict..r4.....do
-000016b0: 6329 03da 1b64 6566 6175 6c74 5f63 6f6e  c)...default_con
-000016c0: 7472 6f6c 5f64 6963 745f 7061 7261 6d73  trol_dict_params
-000016d0: 7251 0000 0072 1b00 0000 2903 721e 0000  rQ...r....).r...
-000016e0: 0072 3c00 0000 7234 0000 0072 2000 0000  .r<...r4...r ...
-000016f0: 7220 0000 0072 2100 0000 da1d 5f63 6f6d  r ...r!....._com
-00001700: 706c 6574 655f 7061 7261 6d73 5f63 6f6e  plete_params_con
-00001710: 7472 6f6c 5f64 6963 74e0 0000 0073 1000  trol_dict....s..
-00001720: 0000 0602 0802 06fe 0405 0201 0201 0201  ................
-00001730: 0afd 7a24 4f75 7470 7574 2e5f 636f 6d70  ..z$Output._comp
-00001740: 6c65 7465 5f70 6172 616d 735f 636f 6e74  lete_params_cont
-00001750: 726f 6c5f 6469 6374 6302 0000 0000 0000  rol_dictc.......
-00001760: 0000 0000 0004 0000 0007 0000 0003 0000  ................
-00001770: 0073 3600 0000 8700 6601 6401 6402 8408  .s6.....f.d.d...
-00001780: 7c00 6a00 a001 a100 4400 8301 7d02 7402  |.j.....D...}.t.
-00001790: 6403 6404 6405 6406 6407 6408 9c05 7c02  d.d.d.d.d.d...|.
-000017a0: 7403 6409 8d03 7d03 7c03 5300 290a 4e63  t.d...}.|.S.).Nc
-000017b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000017c0: 0600 0000 1300 0000 731c 0000 0069 007c  ........s....i.|
-000017d0: 005d 0a7d 017c 0188 006a 0074 017c 0183  .].}.|...j.t.|..
-000017e0: 0119 0093 0271 0253 0072 2000 0000 2902  .....q.S.r ...).
-000017f0: 7277 0000 0072 0400 0000 2902 7273 0000  rw...r....).rs..
-00001800: 0072 7400 0000 a901 723c 0000 0072 2000  .rt.....r<...r .
-00001810: 0000 7221 0000 0072 7600 0000 ee00 0000  ..r!...rv.......
-00001820: 7308 0000 0006 0002 020e ff06 ff7a 314f  s............z1O
-00001830: 7574 7075 742e 6d61 6b65 5f74 7265 655f  utput.make_tree_
-00001840: 636f 6e74 726f 6c5f 6469 6374 2e3c 6c6f  control_dict.<lo
-00001850: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-00001860: 7a03 322e 30da 0561 7363 6969 da0a 6469  z.2.0..ascii..di
-00001870: 6374 696f 6e61 7279 7a08 2273 7973 7465  ctionaryz."syste
-00001880: 6d22 7216 0000 0029 05da 0776 6572 7369  m"r....)...versi
-00001890: 6f6e 7254 0000 00da 0563 6c61 7373 da08  onrT.....class..
-000018a0: 6c6f 6361 7469 6f6e da06 6f62 6a65 6374  location..object
-000018b0: 2903 7245 0000 00da 0863 6869 6c64 7265  ).rE.....childre
-000018c0: 6eda 0668 6561 6465 7229 0472 7a00 0000  n..header).rz...
-000018d0: da04 6b65 7973 720c 0000 0072 0a00 0000  ..keysr....r....
-000018e0: 2904 7260 0000 0072 3c00 0000 7283 0000  ).r`...r<...r...
-000018f0: 00da 0474 7265 6572 2000 0000 727c 0000  ...treer ...r|..
-00001900: 0072 2100 0000 da16 6d61 6b65 5f74 7265  .r!.....make_tre
-00001910: 655f 636f 6e74 726f 6c5f 6469 6374 ed00  e_control_dict..
-00001920: 0000 731c 0000 000a 0108 0206 fe02 0502  ..s.............
-00001930: 0202 0102 0102 0102 0104 fb02 0702 0106  ................
-00001940: f704 0b7a 1d4f 7574 7075 742e 6d61 6b65  ...z.Output.make
-00001950: 5f74 7265 655f 636f 6e74 726f 6c5f 6469  _tree_control_di
-00001960: 6374 6302 0000 0000 0000 0000 0000 0003  ctc.............
-00001970: 0000 0003 0000 0043 0000 0073 1200 0000  .......C...s....
-00001980: 7c00 a000 7c01 a101 7d02 7c02 a001 a100  |...|...}.|.....
-00001990: 5300 2901 4e29 0272 8700 0000 da04 6475  S.).N).r......du
-000019a0: 6d70 2903 7260 0000 0072 3c00 0000 7286  mp).r`...r<...r.
-000019b0: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-000019c0: 0000 da16 6d61 6b65 5f63 6f64 655f 636f  ....make_code_co
-000019d0: 6e74 726f 6c5f 6469 6374 0001 0000 7304  ntrol_dict....s.
-000019e0: 0000 000a 0108 017a 1d4f 7574 7075 742e  .......z.Output.
-000019f0: 6d61 6b65 5f63 6f64 655f 636f 6e74 726f  make_code_contro
-00001a00: 6c5f 6469 6374 6302 0000 0000 0000 0000  l_dictc.........
-00001a10: 0000 0003 0000 0009 0000 0043 0000 0073  ...........C...s
-00001a20: 2a00 0000 6401 6401 6401 6402 6402 6402  *...d.d.d.d.d.d.
-00001a30: 6403 6400 6404 9c08 7d02 7c01 6a00 6405  d.d.d...}.|.j.d.
-00001a40: 7c02 6406 6407 8d03 0100 6400 5300 2908  |.d.d.....d.S.).
-00001a50: 4ee9 2800 0000 6700 0000 0000 00f0 3fda  N.(...g.......?.
-00001a60: 016d 2908 da02 6e78 da02 6e79 da02 6e7a  .m)...nx..ny..nz
-00001a70: da02 6c78 da02 6c79 da02 6c7a da06 6d65  ..lx..ly..lz..me
-00001a80: 7472 6963 da05 7363 616c 65da 0f62 6c6f  tric..scale..blo
-00001a90: 636b 5f6d 6573 685f 6469 6374 da04 544f  ck_mesh_dict..TO
-00001aa0: 444f 7278 0000 0029 0172 1b00 0000 2903  DOrx...).r....).
-00001ab0: 721e 0000 0072 3c00 0000 da07 6465 6661  r....r<.....defa
-00001ac0: 756c 7472 2000 0000 7220 0000 0072 2100  ultr ...r ...r!.
-00001ad0: 0000 da20 5f63 6f6d 706c 6574 655f 7061  ... _complete_pa
-00001ae0: 7261 6d73 5f62 6c6f 636b 5f6d 6573 685f  rams_block_mesh_
-00001af0: 6469 6374 0401 0000 731c 0000 0002 0302  dict....s.......
-00001b00: 0102 0102 0102 0102 0102 0102 0106 f804  ................
-00001b10: 0b02 0102 0102 010a fd7a 274f 7574 7075  .........z'Outpu
-00001b20: 742e 5f63 6f6d 706c 6574 655f 7061 7261  t._complete_para
-00001b30: 6d73 5f62 6c6f 636b 5f6d 6573 685f 6469  ms_block_mesh_di
-00001b40: 6374 2902 4e4e 2918 da08 5f5f 6e61 6d65  ct).NN)...__name
-00001b50: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001b60: 5f5f 7175 616c 6e61 6d65 5f5f 7228 0000  __qualname__r(..
-00001b70: 0072 2a00 0000 722b 0000 0072 0900 0000  .r*...r+...r....
-00001b80: 727a 0000 0072 0b00 0000 da1c 6865 6c70  rz...r......help
-00001b90: 6572 5f74 7572 6275 6c65 6e63 655f 7072  er_turbulence_pr
-00001ba0: 6f70 6572 7469 6573 da0b 636c 6173 736d  operties..classm
-00001bb0: 6574 686f 6472 2200 0000 721c 0000 0072  ethodr"...r....r
-00001bc0: 2d00 0000 723e 0000 0072 4d00 0000 724b  -...r>...rM...rK
-00001bd0: 0000 0072 6d00 0000 726e 0000 0072 7b00  ...rm...rn...r{.
-00001be0: 0000 7287 0000 0072 8900 0000 7297 0000  ..r....r....r...
-00001bf0: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00001c00: 7220 0000 0072 2000 0000 7265 0000 0072  r ...r ...re...r
-00001c10: 2100 0000 7211 0000 001a 0000 0073 3600  !...r........s6.
-00001c20: 0000 0800 0801 0801 0801 0401 0202 0801  ................
-00001c30: 04ff 0204 0a01 020a 0a01 0203 0a01 020d  ................
-00001c40: 0a01 0e1d 024d 0a01 0c04 081e 0211 0a01  .....M..........
-00001c50: 080c 0813 0204 1201 7211 0000 0029 1c72  ........r....).r
-00001c60: 6700 0000 7270 0000 0072 3900 0000 da07  g...rp...r9.....
-00001c70: 7061 7468 6c69 6272 0200 0000 da0a 696e  pathlibr......in
-00001c80: 666c 6563 7469 6f6e 7204 0000 005a 0b66  flectionr....Z.f
-00001c90: 6c75 6964 6479 6e2e 696f 7205 0000 005a  luiddyn.ior....Z
-00001ca0: 0d66 6c75 6964 6479 6e2e 7574 696c 7206  .fluiddyn.utilr.
-00001cb0: 0000 005a 1466 6c75 6964 7369 6d5f 636f  ...Z.fluidsim_co
-00001cc0: 7265 2e6f 7574 7075 7472 0700 0000 da14  re.outputr......
-00001cd0: 666c 7569 6473 696d 5f63 6f72 652e 7061  fluidsim_core.pa
-00001ce0: 7261 6d73 7208 0000 00da 1d66 6c75 6964  ramsr......fluid
-00001cf0: 7369 6d66 6f61 6d2e 666f 616d 5f69 6e70  simfoam.foam_inp
-00001d00: 7574 5f66 696c 6573 7209 0000 0072 0a00  ut_filesr....r..
-00001d10: 0000 720b 0000 0072 0c00 0000 5a28 666c  ..r....r....Z(fl
-00001d20: 7569 6473 696d 666f 616d 2e66 6f61 6d5f  uidsimfoam.foam_
-00001d30: 696e 7075 745f 6669 6c65 732e 6765 6e65  input_files.gene
-00001d40: 7261 746f 7273 720d 0000 0072 0e00 0000  ratorsr....r....
-00001d50: 5a10 666c 7569 6473 696d 666f 616d 2e6c  Z.fluidsimfoam.l
-00001d60: 6f67 720f 0000 00da 1466 6c75 6964 7369  ogr......fluidsi
-00001d70: 6d66 6f61 6d2e 736f 6c76 6572 7372 1000  mfoam.solversr..
-00001d80: 0000 7211 0000 0072 2000 0000 7220 0000  ..r....r ...r ..
-00001d90: 0072 2000 0000 7221 0000 00da 083c 6d6f  .r ...r!.....<mo
-00001da0: 6475 6c65 3e01 0000 0073 1c00 0000 0800  dule>....s......
-00001db0: 0801 0801 0c01 0c02 0c02 0c01 0c01 0c01  ................
-00001dc0: 1801 1006 0c04 0c01 1403                 ..........
+00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
+00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6401 6405 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
+00000070: 6406 6c0a 6d0b 5a0b 0100 6401 6407 6c0c  d.l.m.Z...d.d.l.
+00000080: 6d0d 5a0d 0100 6401 6408 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
+00000090: 0100 6401 6409 6c10 6d11 5a11 6d12 5a12  ..d.d.l.m.Z.m.Z.
+000000a0: 6d13 5a13 6d14 5a14 0100 6401 640a 6c15  m.Z.m.Z...d.d.l.
+000000b0: 6d16 5a16 6d17 5a17 0100 6401 640b 6c18  m.Z.m.Z...d.d.l.
+000000c0: 6d19 5a19 0100 6401 640c 6c1a 6d1b 5a1b  m.Z...d.d.l.m.Z.
+000000d0: 0100 4700 640d 640e 8400 640e 650d 8303  ..G.d.d...d.e...
+000000e0: 5a1c 6402 5300 290f 7a11 4261 7365 206f  Z.d.S.).z.Base o
+000000f0: 7574 7075 7420 636c 6173 73e9 0000 0000  utput class.....
+00000100: 4e29 01da 0450 6174 68a9 01da 0a75 6e64  N)...Path....und
+00000110: 6572 7363 6f72 6529 01da 1173 7464 6f75  erscore)...stdou
+00000120: 745f 7265 6469 7265 6374 6564 2901 da03  t_redirected)...
+00000130: 6d70 6929 01da 0a4f 7574 7075 7443 6f72  mpi)...OutputCor
+00000140: 6529 01da 1469 7465 725f 636f 6d70 6c65  e)...iter_comple
+00000150: 7465 5f70 6172 616d 7329 04da 1444 4546  te_params)...DEF
+00000160: 4155 4c54 5f43 4f4e 5452 4f4c 5f44 4943  AULT_CONTROL_DIC
+00000170: 54da 0e44 4546 4155 4c54 5f48 4541 4445  T..DEFAULT_HEADE
+00000180: 52da 1243 6f6e 7374 616e 7446 696c 6548  R..ConstantFileH
+00000190: 656c 7065 72da 0d46 6f61 6d49 6e70 7574  elper..FoamInput
+000001a0: 4669 6c65 2902 da0a 496e 7075 7446 696c  File)...InputFil
+000001b0: 6573 da18 6e65 775f 6669 6c65 5f67 656e  es..new_file_gen
+000001c0: 6572 6174 6f72 5f63 6c61 7373 2901 da06  erator_class)...
+000001d0: 6c6f 6767 6572 2901 da12 6765 745f 736f  logger)...get_so
+000001e0: 6c76 6572 5f70 6163 6b61 6765 6300 0000  lver_packagec...
+000001f0: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+00000200: 0000 0000 0073 c000 0000 6500 5a01 6400  .....s....e.Z.d.
+00000210: 5a02 6401 6402 6702 5a03 6403 6404 6702  Z.d.d.g.Z.d.d.g.
+00000220: 5a04 6700 6405 a201 5a05 6506 5a07 6508  Z.g.d...Z.e.Z.e.
+00000230: 6404 6406 6407 6901 8302 5a09 650a 6408  d.d.d.i...Z.e.d.
+00000240: 6409 8400 8301 5a0b 650a 640a 640b 8400  d.....Z.e.d.d...
+00000250: 8301 5a0c 650a 640c 640d 8400 8301 5a0d  ..Z.e.d.d.....Z.
+00000260: 650a 640e 640f 8400 8301 5a0e 6421 8700  e.d.d.....Z.d!..
+00000270: 6601 6411 6412 8409 5a0f 650a 6413 6414  f.d.d...Z.e.d.d.
+00000280: 8400 8301 5a10 8700 6601 6415 6416 8408  ....Z...f.d.d...
+00000290: 5a11 6417 6418 8400 5a12 650a 6419 641a  Z.d.d...Z.e.d.d.
+000002a0: 8400 8301 5a13 641b 641c 8400 5a14 641d  ....Z.d.d...Z.d.
+000002b0: 641e 8400 5a15 650a 641f 6420 8400 8301  d...Z.e.d.d ....
+000002c0: 5a16 8700 0400 5a17 5300 2922 da06 4f75  Z.....Z.S.)"..Ou
+000002d0: 7470 7574 da01 70da 0155 da13 7472 616e  tput..p..U..tran
+000002e0: 7370 6f72 7450 726f 7065 7274 6965 73da  sportProperties.
+000002f0: 1474 7572 6275 6c65 6e63 6550 726f 7065  .turbulencePrope
+00000300: 7274 6965 7329 03da 0b63 6f6e 7472 6f6c  rties)...control
+00000310: 4469 6374 da09 6676 5363 6865 6d65 73da  Dict..fvSchemes.
+00000320: 0a66 7653 6f6c 7574 696f 6eda 0e73 696d  .fvSolution..sim
+00000330: 756c 6174 696f 6e54 7970 65da 076c 616d  ulationType..lam
+00000340: 696e 6172 6302 0000 0000 0000 0000 0000  inarc...........
+00000350: 0003 0000 0003 0000 0043 0000 0073 2800  .........C...s(.
+00000360: 0000 7c01 6a00 6a01 a002 6401 a101 7d02  ..|.j.j...d...}.
+00000370: 7c00 a003 7c02 a101 0100 7c01 6a00 6a01  |...|.....|.j.j.
+00000380: a004 a100 0100 6402 5300 2903 7a66 436f  ......d.S.).zfCo
+00000390: 6d70 6c65 7465 2074 6865 2069 6e66 6f5f  mplete the info_
+000003a0: 736f 6c76 6572 2069 6e73 7461 6e63 6520  solver instance 
+000003b0: 7769 7468 2063 6869 6c64 2063 6c61 7373  with child class
+000003c0: 2064 6574 6169 6c73 2028 6d6f 6475 6c65   details (module
+000003d0: 0a20 2020 2020 2020 2061 6e64 2063 6c61  .        and cla
+000003e0: 7373 206e 616d 6573 292e 0a0a 2020 2020  ss names)...    
+000003f0: 2020 2020 da07 636c 6173 7365 734e 2905      ..classesN).
+00000400: 721b 0000 0072 1100 0000 da0a 5f73 6574  r....r......_set
+00000410: 5f63 6869 6c64 da18 5f73 6574 5f69 6e66  _child.._set_inf
+00000420: 6f5f 736f 6c76 6572 5f63 6c61 7373 6573  o_solver_classes
+00000430: da15 636f 6d70 6c65 7465 5f77 6974 685f  ..complete_with_
+00000440: 636c 6173 7365 7329 03da 0363 6c73 da0b  classes)...cls..
+00000450: 696e 666f 5f73 6f6c 7665 7272 1b00 0000  info_solverr....
+00000460: a900 7221 0000 00fa 3d2f 686f 6d65 2f70  ..r!....=/home/p
+00000470: 6965 7272 652f 4465 762f 666c 7569 6473  ierre/Dev/fluids
+00000480: 696d 666f 616d 2f73 7263 2f66 6c75 6964  imfoam/src/fluid
+00000490: 7369 6d66 6f61 6d2f 6f75 7470 7574 2f62  simfoam/output/b
+000004a0: 6173 652e 7079 da15 5f63 6f6d 706c 6574  ase.py.._complet
+000004b0: 655f 696e 666f 5f73 6f6c 7665 7226 0000  e_info_solver&..
+000004c0: 0073 0600 0000 0e06 0a01 1002 7a1c 4f75  .s..........z.Ou
+000004d0: 7470 7574 2e5f 636f 6d70 6c65 7465 5f69  tput._complete_i
+000004e0: 6e66 6f5f 736f 6c76 6572 6302 0000 0000  nfo_solverc.....
+000004f0: 0000 0000 0000 0002 0000 0007 0000 0043  ...............C
+00000500: 0000 0073 2c00 0000 7c01 a000 6401 7401  ...s,...|...d.t.
+00000510: 6402 6401 6403 8d02 a102 0100 7c01 a000  d.d.d.......|...
+00000520: 6404 7401 6405 6404 6403 8d02 a102 0100  d.t.d.d.d.......
+00000530: 6406 5300 2907 7a2e 5365 7420 7468 6520  d.S.).z.Set the 
+00000540: 636c 6173 7365 7320 666f 7220 696e 666f  classes for info
+00000550: 5f73 6f6c 7665 722e 636c 6173 7365 732e  _solver.classes.
+00000560: 4f75 7470 7574 5a03 4c6f 677a 1766 6c75  OutputZ.Logz.flu
+00000570: 6964 7369 6d66 6f61 6d2e 6f75 7470 7574  idsimfoam.output
+00000580: 2e6c 6f67 2902 da0b 6d6f 6475 6c65 5f6e  .log)...module_n
+00000590: 616d 65da 0a63 6c61 7373 5f6e 616d 655a  ame..class_nameZ
+000005a0: 0646 6965 6c64 737a 1a66 6c75 6964 7369  .Fieldsz.fluidsi
+000005b0: 6d66 6f61 6d2e 6f75 7470 7574 2e66 6965  mfoam.output.fie
+000005c0: 6c64 734e 2902 721c 0000 00da 0464 6963  ldsN).r......dic
+000005d0: 7429 0272 1f00 0000 721b 0000 0072 2100  t).r....r....r!.
+000005e0: 0000 7221 0000 0072 2200 0000 721d 0000  ..r!...r"...r...
+000005f0: 0031 0000 0073 1c00 0000 0403 0201 0201  .1...s..........
+00000600: 0201 0201 04fe 04fe 0408 0201 0201 0201  ................
+00000610: 0201 04fe 08fe 7a1f 4f75 7470 7574 2e5f  ......z.Output._
+00000620: 7365 745f 696e 666f 5f73 6f6c 7665 725f  set_info_solver_
+00000630: 636c 6173 7365 7363 0100 0000 0000 0000  classesc........
+00000640: 0000 0000 0400 0000 0700 0000 4300 0000  ............C...
+00000650: 7362 0000 0069 0004 007d 017c 005f 007c  sb...i...}.|._.|
+00000660: 006a 0144 005d 0c7d 0274 027c 0283 017c  .j.D.].}.t.|...|
+00000670: 017c 02a0 0364 0164 02a1 023c 0071 087c  .|...d.d...<.q.|
+00000680: 006a 0444 005d 097d 0374 027c 0364 0383  .j.D.].}.t.|.d..
+00000690: 027c 017c 033c 0071 187c 006a 0544 005d  .|.|.<.q.|.j.D.]
+000006a0: 097d 0374 027c 0364 0483 027c 017c 033c  .}.t.|.d...|.|.<
+000006b0: 0071 2564 0053 0029 054e da01 2eda 015f  .q%d.S.).N....._
+000006c0: da08 636f 6e73 7461 6e74 da06 7379 7374  ..constant..syst
+000006d0: 656d 2906 da18 5f66 696c 655f 6765 6e65  em)..._file_gene
+000006e0: 7261 746f 7273 5f63 6c61 7373 6573 da0e  rators_classes..
+000006f0: 6e61 6d65 5f76 6172 6961 626c 6573 720e  name_variablesr.
+00000700: 0000 00da 0772 6570 6c61 6365 da13 6e61  .....replace..na
+00000710: 6d65 5f63 6f6e 7374 616e 745f 6669 6c65  me_constant_file
+00000720: 73da 116e 616d 655f 7379 7374 656d 5f66  s..name_system_f
+00000730: 696c 6573 2904 721f 0000 0072 1b00 0000  iles).r....r....
+00000740: 5a0d 7661 7269 6162 6c65 5f6e 616d 65da  Z.variable_name.
+00000750: 0966 696c 655f 6e61 6d65 7221 0000 0072  .file_namer!...r
+00000760: 2100 0000 7222 0000 00da 1e5f 7365 7475  !...r"....._setu
+00000770: 705f 6669 6c65 5f67 656e 6572 6174 6f72  p_file_generator
+00000780: 735f 636c 6173 7365 7344 0000 0073 1400  s_classesD...s..
+00000790: 0000 0a02 0a01 0201 0201 12ff 0a04 1001  ................
+000007a0: 0a02 1001 04ff 7a25 4f75 7470 7574 2e5f  ......z%Output._
+000007b0: 7365 7475 705f 6669 6c65 5f67 656e 6572  setup_file_gener
+000007c0: 6174 6f72 735f 636c 6173 7365 7363 0300  ators_classesc..
+000007d0: 0000 0000 0000 0000 0000 0400 0000 0600  ................
+000007e0: 0000 4300 0000 7372 0000 007c 00a0 00a1  ..C...sr...|....
+000007f0: 0001 0074 017c 017c 027c 006a 02a0 03a1  ...t.|.|.|.j....
+00000800: 0083 0301 007c 01a0 0474 0564 0164 0264  .....|...t.d.d.d
+00000810: 038d 02a1 0101 007c 016a 0664 0464 0164  .......|.j.d.d.d
+00000820: 0564 069c 0264 078d 0201 007c 016a 07a0  .d...d.....|.j..
+00000830: 0874 09a0 0a64 08a1 01a1 0101 007c 026a  .t...d.......|.j
+00000840: 0b6a 0ca0 0da1 007d 0374 017c 017c 027c  .j.....}.t.|.|.|
+00000850: 03a0 03a1 0083 0301 0064 0953 0029 0a7a  .........d.S.).z
+00000860: 3e54 6869 7320 7374 6174 6963 206d 6574  >This static met
+00000870: 686f 6420 6973 2075 7365 6420 746f 2063  hod is used to c
+00000880: 6f6d 706c 6574 6520 7468 6520 2a70 6172  omplete the *par
+00000890: 616d 732a 2063 6f6e 7461 696e 6572 2e54  ams* container.T
+000008a0: da03 7275 6e29 02da 0f4e 4557 5f44 4952  ..run)...NEW_DIR
+000008b0: 5f52 4553 554c 5453 5a13 7368 6f72 745f  _RESULTSZ.short_
+000008c0: 6e61 6d65 5f74 7970 655f 7275 6eda 066f  name_type_run..o
+000008d0: 7574 7075 74da 0029 02da 0b48 4153 5f54  utput..)...HAS_T
+000008e0: 4f5f 5341 5645 da0d 7375 625f 6469 7265  O_SAVE..sub_dire
+000008f0: 6374 6f72 7929 01da 0761 7474 7269 6273  ctory)...attribs
+00000900: 612e 0100 000a 2020 2020 2d20 6060 4841  a.....    - ``HA
+00000910: 535f 544f 5f53 4156 4560 603a 2062 6f6f  S_TO_SAVE``: boo
+00000920: 6c20 2864 6566 6175 6c74 3a20 5472 7565  l (default: True
+00000930: 2920 4966 2046 616c 7365 2c20 6e6f 7468  ) If False, noth
+00000940: 696e 6720 6e65 7720 6973 2073 6176 6564  ing new is saved
+00000950: 2069 6e0a 2020 2020 2020 7468 6520 6469   in.      the di
+00000960: 7265 6374 6f72 7920 6f66 2074 6865 2073  rectory of the s
+00000970: 696d 756c 6174 696f 6e2e 0a20 2020 202d  imulation..    -
+00000980: 2060 6073 7562 5f64 6972 6563 746f 7279   ``sub_directory
+00000990: 6060 3a20 7374 7220 2864 6566 6175 6c74  ``: str (default
+000009a0: 3a20 2222 2920 4120 6e61 6d65 206f 6620  : "") A name of 
+000009b0: 6120 7375 622d 6469 7265 6374 6f72 7920  a sub-directory 
+000009c0: 2872 656c 6174 6976 650a 2020 2020 2020  (relative.      
+000009d0: 746f 2024 464c 5549 4444 594e 5f50 4154  to $FLUIDDYN_PAT
+000009e0: 485f 5343 5241 5443 4829 2077 6865 7265  H_SCRATCH) where
+000009f0: 696e 2074 6865 2064 6972 6563 746f 7279  in the directory
+00000a00: 206f 6620 7468 6520 7369 6d75 6c61 7469   of the simulati
+00000a10: 6f6e 0a20 2020 2020 2028 6060 7061 7468  on.      (``path
+00000a20: 5f72 756e 6060 2920 6973 2073 6176 6564  _run``) is saved
+00000a30: 2e0a 0a4e 290e 7231 0000 0072 0800 0000  ...N).r1...r....
+00000a40: 722b 0000 00da 0676 616c 7565 73da 0c5f  r+.....values.._
+00000a50: 7365 745f 6174 7472 6962 7372 2600 0000  set_attribsr&...
+00000a60: 721c 0000 0072 3400 0000 da08 5f73 6574  r....r4....._set
+00000a70: 5f64 6f63 da08 7465 7874 7772 6170 da06  _doc..textwrap..
+00000a80: 6465 6465 6e74 721b 0000 0072 1100 0000  dedentr....r....
+00000a90: da0e 696d 706f 7274 5f63 6c61 7373 6573  ..import_classes
+00000aa0: 2904 721f 0000 00da 0670 6172 616d 7372  ).r......paramsr
+00000ab0: 2000 0000 da0c 6469 6374 5f63 6c61 7373   .....dict_class
+00000ac0: 6573 7221 0000 0072 2100 0000 7222 0000  esr!...r!...r"..
+00000ad0: 00da 1d5f 636f 6d70 6c65 7465 5f70 6172  ..._complete_par
+00000ae0: 616d 735f 7769 7468 5f64 6566 6175 6c74  ams_with_default
+00000af0: 5200 0000 731e 0000 0008 0402 010c 0104  R...s...........
+00000b00: ff12 0504 010a 0106 ff06 0304 0102 0102  ................
+00000b10: ff04 ff0c 0d14 017a 244f 7574 7075 742e  .......z$Output.
+00000b20: 5f63 6f6d 706c 6574 655f 7061 7261 6d73  _complete_params
+00000b30: 5f77 6974 685f 6465 6661 756c 744e 6303  _with_defaultNc.
+00000b40: 0000 0000 0000 0000 0000 000b 0000 0008  ................
+00000b50: 0000 0003 0000 0073 3c02 0000 7c01 7c00  .......s<...|.|.
+00000b60: 5f00 7a08 7c01 6a01 6a02 6a03 7c00 5f04  _.z.|.j.j.j.|._.
+00000b70: 5700 6e09 0400 7405 7914 0100 0100 0100  W.n...t.y.......
+00000b80: 5900 6e07 7700 7406 7c00 6a04 8301 7c00  Y.n.w.t.|.j...|.
+00000b90: 5f07 7c00 a008 a100 7c00 5f09 7c01 722e  _.|.....|._.|.r.
+00000ba0: 7c01 6a0a 6a0b 7c00 5f0a 740c 8300 a00d  |.j.j.|._.t.....
+00000bb0: 7c01 a101 0100 6e0f 7c02 7235 7c02 6a0b  |.....n.|.r5|.j.
+00000bc0: 7c00 5f0a 6e08 6400 7c00 5f0a 740e a00f  |._.n.d.|._.t...
+00000bd0: 6401 a101 0100 7c01 7341 6400 5300 7410  d.....|.sAd.S.t.
+00000be0: 7c00 6a11 8301 7c00 5f11 7412 7c00 8301  |.j...|._.t.|...
+00000bf0: 7c00 5f13 7c01 6a01 6a02 6a14 6a15 a016  |._.|.j.j.j.j...
+00000c00: a100 7d03 7c03 a017 a100 4400 5d26 5c02  ..}.|.....D.]&\.
+00000c10: 7d04 7d05 7418 7c00 7c05 8302 7262 7158  }.}.t.|.|...rbqX
+00000c20: 7419 7c04 8301 7d06 7c00 6a00 0400 6a1a  t.|...}.|.j...j.
+00000c30: 6402 a01b 6403 7c06 9b00 6404 9d03 7c05  d...d.|...d...|.
+00000c40: a102 3700 0200 5f1a 741c 7c00 7c06 7c05  ..7..._.t.|.|.|.
+00000c50: 7c00 8301 8303 0100 7158 741d 7c00 6405  |.......qXt.|.d.
+00000c60: 8302 7388 7c00 a01e a100 0100 6900 7d07  ..s.|.......i.}.
+00000c70: 7c00 6a1f a017 a100 4400 5d25 5c02 7d04  |.j.....D.]%\.}.
+00000c80: 7d05 7419 7c04 8301 7d06 7c05 6a20 7c07  }.t.|...}.|.j |.
+00000c90: 7601 72a3 7c04 6701 7c07 7c05 6a20 3c00  v.r.|.g.|.|.j <.
+00000ca0: 6e08 7c07 7c05 6a20 1900 a021 7c04 a101  n.|.|.j ...!|...
+00000cb0: 0100 741c 7c00 6a13 7c06 7c05 7c00 8301  ..t.|.j.|.|.|...
+00000cc0: 8303 0100 718f 7c07 72dc 7c00 6a00 0400  ....q.|.r.|.j...
+00000cd0: 6a1a 6406 3700 0200 5f1a 7c07 a017 a100  j.d.7..._.|.....
+00000ce0: 4400 5d18 5c02 7d08 7d09 7c00 6a00 0400  D.].\.}.}.|.j...
+00000cf0: 6a1a 6407 7c08 6408 1700 6409 9b04 640a  j.d.|.d...d...d.
+00000d00: a022 7c09 a101 9b00 640b 9d04 3700 0200  ."|.....d...7...
+00000d10: 5f1a 71c3 7423 6a24 640c 6b02 72e9 7c00  _.q.t#j$d.k.r.|.
+00000d20: 6a25 72e9 7c00 6a00 6a0a 6a26 73eb 6400  j%r.|.j.j.j&s.d.
+00000d30: 5300 7c00 6a11 640d 1b00 a027 a100 0100  S.|.j.d....'....
+00000d40: 7c00 6a11 640e 1b00 a027 a100 0100 7c00  |.j.d....'....|.
+00000d50: 6a11 640f 1b00 a027 a100 0100 7428 7c00  j.d....'....t(|.
+00000d60: 6a13 8301 a029 a100 4400 5d14 7d0a 741d  j....)..D.].}.t.
+00000d70: 7c0a 6410 8302 9001 721a 7c0a 6a2a a02b  |.d.....r.|.j*.+
+00000d80: 640d a101 9001 721a 7c0a a02c a100 0100  d.....r.|..,....
+00000d90: 9001 7107 6400 5300 2911 4e7a 4549 6e69  ..q.d.S.).NzEIni
+00000da0: 7469 616c 697a 696e 6720 4f75 7470 7574  tializing Output
+00000db0: 2063 6c61 7373 2077 6974 686f 7574 2073   class without s
+00000dc0: 696d 206f 7220 7061 7261 6d73 206d 6967  im or params mig
+00000dd0: 6874 206c 6561 6420 746f 2065 7272 6f72  ht lead to error
+00000de0: 732e 7a09 7b3a 3238 737d 7b7d 0a7a 0b73  s.z.{:28s}{}.z.s
+00000df0: 696d 2e6f 7574 7075 742e 7a02 3a20 722b  im.output.z.: r+
+00000e00: 0000 007a 0d69 6e70 7574 5f66 696c 6573  ...z.input_files
+00000e10: 3a0a 7a07 2020 2d20 696e 20fa 013a 5a03  :.z.  - in ..:Z.
+00000e20: 3132 73da 0120 da01 0a72 0100 0000 722a  12s.. ...r....r*
+00000e30: 0000 00da 0130 7229 0000 00da 0d67 656e  .....0r).....gen
+00000e40: 6572 6174 655f 6669 6c65 292d da03 7369  erate_file)-..si
+00000e50: 6dda 0469 6e66 6fda 0673 6f6c 7665 72da  m..info..solver.
+00000e60: 0a73 686f 7274 5f6e 616d 65da 0b6e 616d  .short_name..nam
+00000e70: 655f 736f 6c76 6572 da0e 4174 7472 6962  e_solver..Attrib
+00000e80: 7574 6545 7272 6f72 7210 0000 00da 0770  uteErrorr......p
+00000e90: 6163 6b61 6765 da17 6765 745f 7061 7468  ackage..get_path
+00000ea0: 5f73 6f6c 7665 725f 7061 636b 6167 655a  _solver_packageZ
+00000eb0: 1370 6174 685f 736f 6c76 6572 5f70 6163  .path_solver_pac
+00000ec0: 6b61 6765 723f 0000 0072 3400 0000 da05  kager?...r4.....
+00000ed0: 7375 7065 72da 085f 5f69 6e69 745f 5f72  super..__init__r
+00000ee0: 0f00 0000 da07 7761 726e 696e 6772 0200  ......warningr..
+00000ef0: 0000 da08 7061 7468 5f72 756e 720d 0000  ....path_runr...
+00000f00: 00da 0b69 6e70 7574 5f66 696c 6573 721b  ...input_filesr.
+00000f10: 0000 0072 1100 0000 723e 0000 00da 0569  ...r....r>.....i
+00000f20: 7465 6d73 da0a 6973 696e 7374 616e 6365  tems..isinstance
+00000f30: 7204 0000 00da 115f 6f62 6a65 6374 735f  r......_objects_
+00000f40: 746f 5f70 7269 6e74 da06 666f 726d 6174  to_print..format
+00000f50: da07 7365 7461 7474 72da 0768 6173 6174  ..setattr..hasat
+00000f60: 7472 7231 0000 0072 2b00 0000 da08 6469  trr1...r+.....di
+00000f70: 725f 6e61 6d65 da06 6170 7065 6e64 da04  r_name..append..
+00000f80: 6a6f 696e 7206 0000 00da 0472 616e 6bda  joinr......rank.
+00000f90: 0c5f 6861 735f 746f 5f73 6176 6572 3300  ._has_to_saver3.
+00000fa0: 0000 da05 6d6b 6469 72da 0476 6172 7372  ....mkdir..varsr
+00000fb0: 3900 0000 da08 7265 6c5f 7061 7468 da0a  9.....rel_path..
+00000fc0: 7374 6172 7473 7769 7468 7246 0000 0029  startswithrF...)
+00000fd0: 0bda 0473 656c 6672 4700 0000 723f 0000  ...selfrG...r?..
+00000fe0: 0072 4000 0000 da08 636c 735f 6e61 6d65  .r@.....cls_name
+00000ff0: da05 436c 6173 73da 086f 626a 5f6e 616d  ..Class..obj_nam
+00001000: 655a 1366 6f72 5f73 7472 5f69 6e70 7574  eZ.for_str_input
+00001010: 5f66 696c 6573 725a 0000 0072 5300 0000  _filesrZ...rS...
+00001020: da0e 6669 6c65 5f67 656e 6572 6174 6f72  ..file_generator
+00001030: a901 da09 5f5f 636c 6173 735f 5f72 2100  ....__class__r!.
+00001040: 0000 7222 0000 0072 5000 0000 7000 0000  ..r"...rP...p...
+00001050: 7380 0000 0006 0102 0110 010c 0104 0102  s...............
+00001060: ff0c 030a 0204 020a 020e 0104 010a 0206  ................
+00001070: 0204 0102 0104 ff04 0404 010c 020a 0210  ................
+00001080: 0210 010a 0102 0108 010c 010c 0108 ff12  ................
+00001090: 030a 0208 0104 0112 0108 010a 020e 0110  ................
+000010a0: 0214 0104 0210 0110 0108 011a 0108 ff08  ................
+000010b0: 0502 ff04 0202 fe08 0302 fd04 050e 020e  ................
+000010c0: 010e 0112 0202 0104 0106 ff0a 0204 fe08  ................
+000010d0: 0304 8004 fc7a 0f4f 7574 7075 742e 5f5f  .....z.Output.__
+000010e0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+000010f0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00001100: 1200 0000 7400 7401 a002 7c00 a101 6a03  ....t.t...|...j.
+00001110: 8301 6a04 5300 2901 7a28 4765 7420 7468  ..j.S.).z(Get th
+00001120: 6520 7061 7468 2074 6f77 6172 6473 2074  e path towards t
+00001130: 6865 2073 6f6c 7665 7220 7061 636b 6167  he solver packag
+00001140: 652e 2905 7202 0000 00da 0769 6e73 7065  e.).r......inspe
+00001150: 6374 da09 6765 746d 6f64 756c 65da 085f  ct..getmodule.._
+00001160: 5f66 696c 655f 5fda 0670 6172 656e 7429  _file__..parent)
+00001170: 0172 1f00 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00001180: 7222 0000 0072 4e00 0000 bd00 0000 7302  r"...rN.......s.
+00001190: 0000 0012 037a 1e4f 7574 7075 742e 6765  .....z.Output.ge
+000011a0: 745f 7061 7468 5f73 6f6c 7665 725f 7061  t_path_solver_pa
+000011b0: 636b 6167 6563 0100 0000 0000 0000 0000  ckagec..........
+000011c0: 0000 0500 0000 0800 0000 0300 0000 73c8  ..............s.
+000011d0: 0000 0074 006a 0164 016b 0272 0d74 0264  ...t.j.d.k.r.t.d
+000011e0: 027c 006a 039b 009d 0283 0101 0074 0483  .|.j.........t..
+000011f0: 008f 0d01 0074 0583 00a0 06a1 0001 0057  .....t.........W
+00001200: 0064 0304 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00001210: 2077 0101 0001 0001 0059 0001 0074 07a0   w.......Y...t..
+00001220: 087c 006a 096a 0aa1 0101 0074 006a 0164  .|.j.j.....t.j.d
+00001230: 016b 0272 3d7c 006a 0b72 3d7c 006a 096a  .k.r=|.j.r=|.j.j
+00001240: 0c6a 0d72 3d7c 00a0 0ea1 0001 0074 0f7c  .j.r=|.......t.|
+00001250: 006a 0383 017d 017c 0164 041b 007d 027c  .j...}.|.d...}.|
+00001260: 026a 1064 0564 068d 0101 0064 0744 005d  .j.d.d.....d.D.]
+00001270: 137d 037c 027c 031b 007d 047c 04a0 11a1  .}.|.|...}.|....
+00001280: 0072 5971 4e74 12a0 137c 017c 031b 007c  .rYqNt...|.|...|
+00001290: 04a1 0201 0071 4e64 0353 0029 087a 214c  .....qNd.S.).z!L
+000012a0: 6f67 7320 696e 666f 206f 6e20 696e 7374  ogs info on inst
+000012b0: 616e 7469 6174 6564 2063 6c61 7373 6573  antiated classes
+000012c0: 7201 0000 007a 0a70 6174 685f 7275 6e3a  r....z.path_run:
+000012d0: 204e 7a0e 2e64 6174 615f 666c 7569 6473   Nz..data_fluids
+000012e0: 696d 5429 01da 0865 7869 7374 5f6f 6b29  imT)...exist_ok)
+000012f0: 027a 0f69 6e66 6f5f 736f 6c76 6572 2e78  .z.info_solver.x
+00001300: 6d6c 7a10 7061 7261 6d73 5f73 696d 756c  mlz.params_simul
+00001310: 2e78 6d6c 2914 7206 0000 0072 5d00 0000  .xml).r....r]...
+00001320: da05 7072 696e 7472 5200 0000 7205 0000  ..printrR...r...
+00001330: 0072 4f00 0000 da09 706f 7374 5f69 6e69  .rO.....post_ini
+00001340: 7472 0f00 0000 7248 0000 0072 4700 0000  tr....rH...rG...
+00001350: 7256 0000 0072 5e00 0000 723f 0000 0072  rV...r^...r?...r
+00001360: 3300 0000 da29 5f70 6f73 745f 696e 6974  3....)_post_init
+00001370: 5f63 7265 6174 655f 6164 6469 7469 6f6e  _create_addition
+00001380: 616c 5f73 6f75 7263 655f 6669 6c65 7372  al_source_filesr
+00001390: 0200 0000 725f 0000 00da 0665 7869 7374  ....r_.....exist
+000013a0: 73da 0673 6875 7469 6cda 0463 6f70 7929  s..shutil..copy)
+000013b0: 0572 6300 0000 7252 0000 005a 1270 6174  .rc...rR...Z.pat
+000013c0: 685f 696e 666f 5f66 6c75 6964 7369 6d72  h_info_fluidsimr
+000013d0: 3000 0000 5a08 7061 7468 5f6e 6577 7268  0...Z.path_newrh
+000013e0: 0000 0072 2100 0000 7222 0000 0072 7000  ...r!...r"...rp.
+000013f0: 0000 c200 0000 732c 0000 000a 0310 0108  ......s,........
+00001400: 030c 011c ff0e 0308 0402 ff04 0202 fe08  ................
+00001410: 0302 fd08 050a 0308 010c 0108 0108 0108  ................
+00001420: 0102 0112 0104 fc7a 104f 7574 7075 742e  .......z.Output.
+00001430: 706f 7374 5f69 6e69 7463 0100 0000 0000  post_initc......
+00001440: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+00001450: 0000 736c 0000 007c 006a 006a 0164 011b  ..sl...|.j.j.d..
+00001460: 007d 017c 01a0 02a1 0073 1374 0364 027c  .}.|.....s.t.d.|
+00001470: 006a 006a 019b 009d 0283 0182 0174 04a0  .j.j.........t..
+00001480: 057c 017c 006a 066a 07a1 0201 0074 087c  .|.|.j.j.....t.|
+00001490: 006a 0083 01a0 09a1 0044 005d 117d 0274  .j.......D.].}.t
+000014a0: 0a7c 0264 0383 0272 337c 026a 0ba0 0c64  .|.d...r3|.j...d
+000014b0: 04a1 0173 337c 02a0 0da1 0001 0071 2264  ...s3|.......q"d
+000014c0: 0553 0029 067a 2443 7265 6174 6520 7468  .S.).z$Create th
+000014d0: 6520 6669 6c65 7320 6672 6f6d 2074 6865  e files from the
+000014e0: 6972 2074 656d 706c 6174 657a 0874 6173  ir templatez.tas
+000014f0: 6b73 2e70 797a 2974 6173 6b73 2e70 7920  ks.pyz)tasks.py 
+00001500: 6d69 7373 696e 6720 696e 2073 6f6c 7665  missing in solve
+00001510: 7220 7465 6d70 6c61 7465 735f 6469 7220  r templates_dir 
+00001520: 7246 0000 0072 2a00 0000 4e29 0e72 5300  rF...r*...N).rS.
+00001530: 0000 5a0d 7465 6d70 6c61 7465 735f 6469  ..Z.templates_di
+00001540: 7272 7200 0000 da0c 5275 6e74 696d 6545  rrr.....RuntimeE
+00001550: 7272 6f72 7273 0000 0072 7400 0000 7247  rrorrs...rt...rG
+00001560: 0000 0072 5200 0000 7260 0000 0072 3900  ...rR...r`...r9.
+00001570: 0000 7259 0000 0072 6100 0000 7262 0000  ..rY...ra...rb..
+00001580: 0072 4600 0000 2903 7263 0000 005a 0d70  .rF...).rc...Z.p
+00001590: 6174 685f 7461 736b 735f 7079 7267 0000  ath_tasks_pyrg..
+000015a0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+000015b0: 7271 0000 00e0 0000 0073 2200 0000 0c02  rq.......s".....
+000015c0: 0801 0201 0201 0601 04ff 04ff 1004 1202  ................
+000015d0: 0201 0401 04ff 0a02 02fe 0804 0280 04fb  ................
+000015e0: 7a30 4f75 7470 7574 2e5f 706f 7374 5f69  z0Output._post_i
+000015f0: 6e69 745f 6372 6561 7465 5f61 6464 6974  nit_create_addit
+00001600: 696f 6e61 6c5f 736f 7572 6365 5f66 696c  ional_source_fil
+00001610: 6573 6302 0000 0000 0000 0000 0000 0003  esc.............
+00001620: 0000 0005 0000 0043 0000 0073 2800 0000  .......C...s(...
+00001630: 6401 6402 8400 7c00 6a00 a001 a100 4400  d.d...|.j.....D.
+00001640: 8301 7d02 7c01 6a02 6403 7c02 6404 6405  ..}.|.j.d.|.d.d.
+00001650: 8d03 0100 6400 5300 2906 4e63 0100 0000  ....d.S.).Nc....
+00001660: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00001670: 5300 0000 731a 0000 0069 007c 005d 095c  S...s....i.|.].\
+00001680: 027d 017d 0274 007c 0183 017c 0293 0271  .}.}.t.|...|...q
+00001690: 0253 0072 2100 0000 7203 0000 0029 03da  .S.r!...r....)..
+000016a0: 022e 30da 036b 6579 da05 7661 6c75 6572  ..0..key..valuer
+000016b0: 2100 0000 7221 0000 0072 2200 0000 da0a  !...r!...r".....
+000016c0: 3c64 6963 7463 6f6d 703e f300 0000 7308  <dictcomp>....s.
+000016d0: 0000 0006 0006 0208 ff06 ff7a 384f 7574  ...........z8Out
+000016e0: 7075 742e 5f63 6f6d 706c 6574 655f 7061  put._complete_pa
+000016f0: 7261 6d73 5f63 6f6e 7472 6f6c 5f64 6963  rams_control_dic
+00001700: 742e 3c6c 6f63 616c 733e 2e3c 6469 6374  t.<locals>.<dict
+00001710: 636f 6d70 3eda 0c63 6f6e 7472 6f6c 5f64  comp>..control_d
+00001720: 6963 747a 3d53 6565 2068 7474 7073 3a2f  ictz=See https:/
+00001730: 2f64 6f63 2e63 6664 2e64 6972 6563 742f  /doc.cfd.direct/
+00001740: 6f70 656e 666f 616d 2f75 7365 722d 6775  openfoam/user-gu
+00001750: 6964 652d 7636 2f63 6f6e 7472 6f6c 6469  ide-v6/controldi
+00001760: 6374 a902 7238 0000 00da 0364 6f63 2903  ct..r8.....doc).
+00001770: da1c 5f64 6566 6175 6c74 5f63 6f6e 7472  .._default_contr
+00001780: 6f6c 5f64 6963 745f 7061 7261 6d73 7254  ol_dict_paramsrT
+00001790: 0000 0072 1c00 0000 2903 721f 0000 0072  ...r....).r....r
+000017a0: 3f00 0000 7238 0000 0072 2100 0000 7221  ?...r8...r!...r!
+000017b0: 0000 0072 2200 0000 da1d 5f63 6f6d 706c  ...r"....._compl
+000017c0: 6574 655f 7061 7261 6d73 5f63 6f6e 7472  ete_params_contr
+000017d0: 6f6c 5f64 6963 74f1 0000 0073 1000 0000  ol_dict....s....
+000017e0: 0602 0802 06fe 0405 0201 0201 0201 0afd  ................
+000017f0: 7a24 4f75 7470 7574 2e5f 636f 6d70 6c65  z$Output._comple
+00001800: 7465 5f70 6172 616d 735f 636f 6e74 726f  te_params_contro
+00001810: 6c5f 6469 6374 6302 0000 0000 0000 0000  l_dictc.........
+00001820: 0000 0004 0000 0007 0000 0003 0000 0073  ...............s
+00001830: 3600 0000 8700 6601 6401 6402 8408 7c00  6.....f.d.d...|.
+00001840: 6a00 a001 a100 4400 8301 7d02 7402 6403  j.....D...}.t.d.
+00001850: 6404 6405 6406 6407 6408 9c05 7c02 7403  d.d.d.d.d...|.t.
+00001860: 6409 8d03 7d03 7c03 5300 290a 4e63 0100  d...}.|.S.).Nc..
+00001870: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00001880: 0000 1300 0000 731c 0000 0069 007c 005d  ......s....i.|.]
+00001890: 0a7d 017c 0188 006a 0074 017c 0183 0119  .}.|...j.t.|....
+000018a0: 0093 0271 0253 0072 2100 0000 2902 727a  ...q.S.r!...).rz
+000018b0: 0000 0072 0400 0000 2902 7276 0000 0072  ...r....).rv...r
+000018c0: 7700 0000 a901 723f 0000 0072 2100 0000  w.....r?...r!...
+000018d0: 7222 0000 0072 7900 0000 ff00 0000 7308  r"...ry.......s.
+000018e0: 0000 0006 0002 020e ff06 ff7a 324f 7574  ...........z2Out
+000018f0: 7075 742e 5f6d 616b 655f 7472 6565 5f63  put._make_tree_c
+00001900: 6f6e 7472 6f6c 5f64 6963 742e 3c6c 6f63  ontrol_dict.<loc
+00001910: 616c 733e 2e3c 6469 6374 636f 6d70 3e7a  als>.<dictcomp>z
+00001920: 0332 2e30 da05 6173 6369 69da 0a64 6963  .2.0..ascii..dic
+00001930: 7469 6f6e 6172 797a 0822 7379 7374 656d  tionaryz."system
+00001940: 2272 1600 0000 2905 da07 7665 7273 696f  "r....)...versio
+00001950: 6e72 5700 0000 da05 636c 6173 73da 086c  nrW.....class..l
+00001960: 6f63 6174 696f 6eda 066f 626a 6563 7429  ocation..object)
+00001970: 0372 4800 0000 da08 6368 696c 6472 656e  .rH.....children
+00001980: da06 6865 6164 6572 2904 727d 0000 00da  ..header).r}....
+00001990: 046b 6579 7372 0c00 0000 720a 0000 0029  .keysr....r....)
+000019a0: 0472 6300 0000 723f 0000 0072 8600 0000  .rc...r?...r....
+000019b0: da04 7472 6565 7221 0000 0072 7f00 0000  ..treer!...r....
+000019c0: 7222 0000 00da 175f 6d61 6b65 5f74 7265  r"....._make_tre
+000019d0: 655f 636f 6e74 726f 6c5f 6469 6374 fe00  e_control_dict..
+000019e0: 0000 731c 0000 000a 0108 0206 fe02 0502  ..s.............
+000019f0: 0202 0102 0102 0102 0104 fb02 0702 0106  ................
+00001a00: f704 0b7a 1e4f 7574 7075 742e 5f6d 616b  ...z.Output._mak
+00001a10: 655f 7472 6565 5f63 6f6e 7472 6f6c 5f64  e_tree_control_d
+00001a20: 6963 7463 0200 0000 0000 0000 0000 0000  ictc............
+00001a30: 0300 0000 0300 0000 4300 0000 7312 0000  ........C...s...
+00001a40: 007c 00a0 007c 01a1 017d 027c 02a0 01a1  .|...|...}.|....
+00001a50: 0053 0029 014e 2902 728a 0000 00da 0464  .S.).N).r......d
+00001a60: 756d 7029 0372 6300 0000 723f 0000 0072  ump).rc...r?...r
+00001a70: 8900 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
+00001a80: 0000 00da 175f 6d61 6b65 5f63 6f64 655f  ....._make_code_
+00001a90: 636f 6e74 726f 6c5f 6469 6374 1101 0000  control_dict....
+00001aa0: 7304 0000 000a 0108 017a 1e4f 7574 7075  s........z.Outpu
+00001ab0: 742e 5f6d 616b 655f 636f 6465 5f63 6f6e  t._make_code_con
+00001ac0: 7472 6f6c 5f64 6963 7463 0200 0000 0000  trol_dictc......
+00001ad0: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
+00001ae0: 0000 7328 0000 0064 0164 0164 0164 0264  ..s(...d.d.d.d.d
+00001af0: 0264 0264 0364 049c 077d 027c 016a 0064  .d.d.d...}.|.j.d
+00001b00: 057c 0264 0664 078d 0301 0064 0053 0029  .|.d.d.....d.S.)
+00001b10: 084e e928 0000 0067 0000 0000 0000 f03f  .N.(...g.......?
+00001b20: e901 0000 0029 07da 026e 78da 026e 79da  .....)...nx..ny.
+00001b30: 026e 7ada 026c 78da 026c 79da 026c 7ada  .nz..lx..ly..lz.
+00001b40: 0573 6361 6c65 da0f 626c 6f63 6b5f 6d65  .scale..block_me
+00001b50: 7368 5f64 6963 74da 0454 4f44 4f72 7b00  sh_dict..TODOr{.
+00001b60: 0000 2901 721c 0000 0029 0372 1f00 0000  ..).r....).r....
+00001b70: 723f 0000 00da 0764 6566 6175 6c74 7221  r?.....defaultr!
+00001b80: 0000 0072 2100 0000 7222 0000 00da 205f  ...r!...r".... _
+00001b90: 636f 6d70 6c65 7465 5f70 6172 616d 735f  complete_params_
+00001ba0: 626c 6f63 6b5f 6d65 7368 5f64 6963 7415  block_mesh_dict.
+00001bb0: 0100 0073 1a00 0000 0203 0201 0201 0201  ...s............
+00001bc0: 0201 0201 0201 06f9 040a 0201 0201 0201  ................
+00001bd0: 0afd 7a27 4f75 7470 7574 2e5f 636f 6d70  ..z'Output._comp
+00001be0: 6c65 7465 5f70 6172 616d 735f 626c 6f63  lete_params_bloc
+00001bf0: 6b5f 6d65 7368 5f64 6963 7429 024e 4e29  k_mesh_dict).NN)
+00001c00: 18da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00001c10: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00001c20: 616d 655f 5f72 2c00 0000 722e 0000 0072  ame__r,...r....r
+00001c30: 2f00 0000 7209 0000 0072 7d00 0000 720b  /...r....r}...r.
+00001c40: 0000 00da 1d5f 6865 6c70 6572 5f74 7572  ....._helper_tur
+00001c50: 6275 6c65 6e63 655f 7072 6f70 6572 7469  bulence_properti
+00001c60: 6573 da0b 636c 6173 736d 6574 686f 6472  es..classmethodr
+00001c70: 2300 0000 721d 0000 0072 3100 0000 7241  #...r....r1...rA
+00001c80: 0000 0072 5000 0000 724e 0000 0072 7000  ...rP...rN...rp.
+00001c90: 0000 7271 0000 0072 7e00 0000 728a 0000  ..rq...r~...r...
+00001ca0: 0072 8c00 0000 7299 0000 00da 0d5f 5f63  .r....r......__c
+00001cb0: 6c61 7373 6365 6c6c 5f5f 7221 0000 0072  lasscell__r!...r
+00001cc0: 2100 0000 7268 0000 0072 2200 0000 7211  !...rh...r"...r.
+00001cd0: 0000 001c 0000 0073 3600 0000 0800 0801  .......s6.......
+00001ce0: 0801 0801 0401 0202 0801 04ff 0204 0a01  ................
+00001cf0: 020a 0a01 0212 0a01 020d 0a01 0e1d 024d  ...............M
+00001d00: 0a01 0c04 081e 0211 0a01 080c 0813 0204  ................
+00001d10: 1201 7211 0000 0029 1dda 075f 5f64 6f63  ..r....)...__doc
+00001d20: 5f5f 726a 0000 0072 7300 0000 723c 0000  __rj...rs...r<..
+00001d30: 00da 0770 6174 686c 6962 7202 0000 00da  ...pathlibr.....
+00001d40: 0a69 6e66 6c65 6374 696f 6e72 0400 0000  .inflectionr....
+00001d50: 5a0b 666c 7569 6464 796e 2e69 6f72 0500  Z.fluiddyn.ior..
+00001d60: 0000 5a0d 666c 7569 6464 796e 2e75 7469  ..Z.fluiddyn.uti
+00001d70: 6c72 0600 0000 5a14 666c 7569 6473 696d  lr....Z.fluidsim
+00001d80: 5f63 6f72 652e 6f75 7470 7574 7207 0000  _core.outputr...
+00001d90: 00da 1466 6c75 6964 7369 6d5f 636f 7265  ...fluidsim_core
+00001da0: 2e70 6172 616d 7372 0800 0000 da1d 666c  .paramsr......fl
+00001db0: 7569 6473 696d 666f 616d 2e66 6f61 6d5f  uidsimfoam.foam_
+00001dc0: 696e 7075 745f 6669 6c65 7372 0900 0000  input_filesr....
+00001dd0: 720a 0000 0072 0b00 0000 720c 0000 005a  r....r....r....Z
+00001de0: 2866 6c75 6964 7369 6d66 6f61 6d2e 666f  (fluidsimfoam.fo
+00001df0: 616d 5f69 6e70 7574 5f66 696c 6573 2e67  am_input_files.g
+00001e00: 656e 6572 6174 6f72 7372 0d00 0000 720e  eneratorsr....r.
+00001e10: 0000 005a 1066 6c75 6964 7369 6d66 6f61  ...Z.fluidsimfoa
+00001e20: 6d2e 6c6f 6772 0f00 0000 da14 666c 7569  m.logr......flui
+00001e30: 6473 696d 666f 616d 2e73 6f6c 7665 7273  dsimfoam.solvers
+00001e40: 7210 0000 0072 1100 0000 7221 0000 0072  r....r....r!...r
+00001e50: 2100 0000 7221 0000 0072 2200 0000 da08  !...r!...r".....
+00001e60: 3c6d 6f64 756c 653e 0100 0000 731e 0000  <module>....s...
+00001e70: 0004 0008 0208 0108 010c 010c 020c 020c  ................
+00001e80: 010c 010c 0118 0110 060c 040c 0114 03    ...............
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/output/base.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/output/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Base output class"""
+
 import inspect
 import shutil
 import textwrap
 from pathlib import Path
 
 from inflection import underscore
 
@@ -20,20 +22,20 @@
     new_file_generator_class,
 )
 from fluidsimfoam.log import logger
 from fluidsimfoam.solvers import get_solver_package
 
 
 class Output(OutputCore):
-    variable_names = ["p", "U"]
-    constant_files_names = ["transportProperties", "turbulenceProperties"]
-    system_files_names = ["controlDict", "fvSchemes", "fvSolution"]
-    default_control_dict_params = DEFAULT_CONTROL_DICT
+    name_variables = ["p", "U"]
+    name_constant_files = ["transportProperties", "turbulenceProperties"]
+    name_system_files = ["controlDict", "fvSchemes", "fvSolution"]
+    _default_control_dict_params = DEFAULT_CONTROL_DICT
 
-    helper_turbulence_properties = ConstantFileHelper(
+    _helper_turbulence_properties = ConstantFileHelper(
         "turbulenceProperties", {"simulationType": "laminar"}
     )
 
     @classmethod
     def _complete_info_solver(cls, info_solver):
         """Complete the info_solver instance with child class details (module
         and class names).
@@ -43,27 +45,42 @@
         cls._set_info_solver_classes(classes)
         # iteratively call _complete_info_solver of the above classes
         info_solver.classes.Output.complete_with_classes()
 
     @classmethod
     def _set_info_solver_classes(cls, classes):
         """Set the classes for info_solver.classes.Output"""
+        classes._set_child(
+            "Log",
+            dict(
+                module_name="fluidsimfoam.output.log",
+                class_name="Log",
+            ),
+        )
+
+        classes._set_child(
+            "Fields",
+            dict(
+                module_name="fluidsimfoam.output.fields",
+                class_name="Fields",
+            ),
+        )
 
     @classmethod
     def _setup_file_generators_classes(cls):
         classes = cls._file_generators_classes = {}
-        for variable_name in cls.variable_names:
+        for variable_name in cls.name_variables:
             classes[variable_name.replace(".", "_")] = new_file_generator_class(
                 variable_name
             )
 
-        for file_name in cls.constant_files_names:
+        for file_name in cls.name_constant_files:
             classes[file_name] = new_file_generator_class(file_name, "constant")
 
-        for file_name in cls.system_files_names:
+        for file_name in cls.name_system_files:
             classes[file_name] = new_file_generator_class(file_name, "system")
 
     @classmethod
     def _complete_params_with_default(cls, params, info_solver):
         """This static method is used to complete the *params* container."""
 
         cls._setup_file_generators_classes()
@@ -188,27 +205,27 @@
 
         # Write input files of the simulation
         if (
             mpi.rank == 0
             and self._has_to_save
             and self.sim.params.NEW_DIR_RESULTS
         ):
-            self.post_init_create_additional_source_files()
+            self._post_init_create_additional_source_files()
 
         # OpenFOAM cleanup removes .xml files!
         path_run = Path(self.path_run)
         path_info_fluidsim = path_run / ".data_fluidsim"
         path_info_fluidsim.mkdir(exist_ok=True)
         for file_name in ("info_solver.xml", "params_simul.xml"):
             path_new = path_info_fluidsim / file_name
             if path_new.exists():
                 continue
             shutil.copy(path_run / file_name, path_new)
 
-    def post_init_create_additional_source_files(self):
+    def _post_init_create_additional_source_files(self):
         """Create the files from their template"""
         path_tasks_py = self.input_files.templates_dir / "tasks.py"
         if not path_tasks_py.exists():
             raise RuntimeError(
                 "tasks.py missing in solver templates_dir "
                 f"{self.input_files.templates_dir}"
             )
@@ -221,27 +238,27 @@
                 # system files are already generated
                 file_generator.generate_file()
 
     @classmethod
     def _complete_params_control_dict(cls, params):
         attribs = {
             underscore(key): value
-            for key, value in cls.default_control_dict_params.items()
+            for key, value in cls._default_control_dict_params.items()
         }
 
         params._set_child(
             "control_dict",
             attribs=attribs,
             doc="""See https://doc.cfd.direct/openfoam/user-guide-v6/controldict""",
         )
 
-    def make_tree_control_dict(self, params):
+    def _make_tree_control_dict(self, params):
         children = {
             key: params.control_dict[underscore(key)]
-            for key in self.default_control_dict_params.keys()
+            for key in self._default_control_dict_params.keys()
         }
 
         tree = FoamInputFile(
             info={
                 "version": "2.0",
                 "format": "ascii",
                 "class": "dictionary",
@@ -249,29 +266,28 @@
                 "object": "controlDict",
             },
             children=children,
             header=DEFAULT_HEADER,
         )
         return tree
 
-    def make_code_control_dict(self, params):
-        tree = self.make_tree_control_dict(params)
+    def _make_code_control_dict(self, params):
+        tree = self._make_tree_control_dict(params)
         return tree.dump()
 
     @classmethod
     def _complete_params_block_mesh_dict(cls, params):
         default = {
             "nx": 40,
             "ny": 40,
             "nz": 40,
             "lx": 1.0,
             "ly": 1.0,
             "lz": 1.0,
-            "metric": "m",
-            "scale": None,
+            "scale": 1,
         }
 
         params._set_child(
             "block_mesh_dict",
             attribs=default,
             doc="""TODO""",
         )
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/resources/__init__.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__init__.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/base.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/solvers/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Base class for the ``sim`` object"""
 
 from pathlib import Path
+from time import sleep, time
 
 from inflection import underscore
 
 from fluiddyn.util import mpi  # noqa: F401
 from fluidsim_core.solver import SimulCore
 from fluidsimfoam.log import logger
 from fluidsimfoam.params import Parameters
@@ -54,7 +55,38 @@
             self.output.post_init()
         else:
             self.path_run = None
             if mpi.rank == 0:
                 logger.warning("No output class initialized!")
 
         self.input_files = self.output.input_files
+
+    def stop_time_loop(self, stop_at="writeNow", verbose=True):
+        if verbose:
+            print("Telling OpenFOAM to stop... (overwrite controlDict file)")
+            t_stop = time()
+        ctr_dict = self.input_files.control_dict.read()
+        ctr_dict["stopAt"] = stop_at
+        ctr_dict.overwrite()
+
+        process = self.make.process
+
+        if process is None:
+            return
+
+        while process.poll() is None:
+            # touch needed (strange OpenFOAM bug?)
+            (self.path_run / "system/controlDict").touch()
+            sleep(0.05)
+            if verbose:
+                saved_directories = sorted(
+                    path.name
+                    for path in self.path_run.glob("*")
+                    if path.name[0].isdigit()
+                )
+                print(f"\rsaved times {saved_directories}", end="")
+
+        if verbose:
+            print(
+                f"\nSimulation stopped {time() - t_stop:.2f} s "
+                f"after `stopAt = {stop_at}`"
+            )
```

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc` & `fluidsimfoam-0.0.4/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/src/fluidsimfoam/util/console.py` & `fluidsimfoam-0.0.4/src/fluidsimfoam/util/console.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.3/PKG-INFO` & `fluidsimfoam-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: fluidsimfoam
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python framework for OpenFOAM
 License: BSD-3-Clause
 Author: pierre.augier
 Author-email: pierre.augier@univ-grenoble-alpes.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: jupyter
+Provides-Extra: qt
+Requires-Dist: PySide6 (>=6.5.0,<7.0.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "qt")
 Requires-Dist: fluiddyn (>=0.5.2,<0.6.0)
 Requires-Dist: fluidsim-core (>=0.7.2,<0.8.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: invoke (>=2.0.0,<3.0.0)
 Requires-Dist: ipython (>=8.11.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: jupyterlab (>=3.6.3,<4.0.0) ; extra == "jupyter"
+Requires-Dist: jupyterlab_myst (>=1.1.3,<2.0.0) ; extra == "jupyter"
+Requires-Dist: jupytext (>=1.14.5,<2.0.0) ; extra == "jupyter"
 Requires-Dist: lark (>=1.1.5,<2.0.0)
+Requires-Dist: mdformat-myst (>=0.1.4,<0.2.0) ; extra == "jupyter"
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # Fluidsimfoam
@@ -29,15 +36,15 @@
 [![PyPI](https://img.shields.io/pypi/v/fluidsimfoam)](https://pypi.org/project/fluidsimfoam/)
 [![Documentation Status](https://readthedocs.org/projects/fluidsimfoam/badge/?version=latest)](https://fluidsimfoam.readthedocs.io/en/latest/?badge=latest)
 
 Python framework for [OpenFOAM]
 
 </div>
 
-<!-- badges -->
+<!-- start-intro -->
 
 [OpenFOAM] is a very popular open-source C++ CFD framework. Working with [OpenFOAM]
 implies writting and modifying a lot of input files describing a simulation.
 The method described in the official [OpenFOAM] documentations is to copy an
 existing simulation directory and to modify the input files by hand.
 Fluidsimfoam is a Python package designed to improve the life of [OpenFOAM]
 users.
@@ -65,31 +72,52 @@
 equivalent of [Snek5000], our Fluidsim framework for [Nek5000]. Looking at the
 [Snek5000] tutorials should give a good idea of what Fluidsimfoam will soon
 allow.
 
 For our examples, we currently target OpenFOAM v2206 but it should be possible
 to write Fluidsimfoam solvers targeting any recent OpenFOAM versions.
 
+[fluiddyn]: https://fluiddyn.readthedocs.io
+[fluidsim]: https://fluidsim.readthedocs.io
+[fluidfoam]: https://fluidfoam.readthedocs.io
+[fluidsimfoam-tgv]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-tgv
+[fluidsimfoam-cbox]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-cbox
+[fluidsimfoam-sed]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-sed
+[openfoam]: https://openfoam.org/
+[nek5000]: https://nek5000.mcs.anl.gov/
+[snek5000]: https://snek5000.readthedocs.io
+
+<!-- end-intro -->
+
 See more in [Fluidsimfoam documentation](https://fluidsimfoam.readthedocs.org).
 
 ## Install
 
+<!-- start-install -->
+
 Currently, it still makes sense to install Fluidsimfoam like we, the
 fluidsimfoam developers, install it, i.e. in a dedicated controlled virtual
 environment created by [Poetry]. After installing [Poetry] (for example with
 something like `pip install poetry`), the following commands should install and
 activate the virtual environment:
 
 ```sh
 hg clone https://foss.heptapod.net/fluiddyn/fluidsimfoam
 cd fluidsimfoam
 poetry install
 poetry shell
 ```
 
+For better user experience with Matplotlib figures, you can also install with
+`poetry install --extra qt`.
+
+[Poetry]: https://python-poetry.org/docs/
+
+<!-- end-install -->
+
 ## Related projects
 
 - [Fluidfoam] Another [Fluiddyn] package (like Fluidsimfoam) to use/plot OpenFOAM
   data. Will be used by Fluidsimfoam.
 
 - [PyFoam] ([PyPI package](https://pypi.org/project/PyFoam/),
   [hg repo](http://hg.code.sf.net/p/openfoam-extend/PyFoam)) Python utilities for
@@ -97,19 +125,10 @@
 
 - [PythonFlu] ([wiki](https://openfoamwiki.net/index.php/Contrib_pythonFlu))
 
 - [Swak4Foam] Popular set of utilities for OpenFOAM. Can be used in
   Fluidsimfoam solvers.
 
 [PyFoam]: https://openfoamwiki.net/index.php/Contrib/PyFoam
-[fluiddyn]: https://fluiddyn.readthedocs.io
-[fluidsim]: https://fluidsim.readthedocs.io
-[fluidfoam]: https://fluidfoam.readthedocs.io
-[fluidsimfoam-tgv]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-tgv
-[fluidsimfoam-cbox]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-cbox
-[fluidsimfoam-sed]: https://foss.heptapod.net/fluiddyn/fluidsimfoam/-/tree/branch/default/doc/examples/fluidsimfoam-sed
-[openfoam]: https://openfoam.org/
-[nek5000]: https://nek5000.mcs.anl.gov/
-[snek5000]: https://snek5000.readthedocs.io
 [PythonFlu]: http://pythonflu.wikidot.com/
 [Swak4Foam]: https://openfoamwiki.net/index.php/Contrib/swak4Foam
-[Poetry]: https://python-poetry.org/docs/
+
```

