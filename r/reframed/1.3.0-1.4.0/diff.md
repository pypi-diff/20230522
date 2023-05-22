# Comparing `tmp/reframed-1.3.0.tar.gz` & `tmp/reframed-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reframed-1.3.0.tar", last modified: Mon Mar  6 13:15:06 2023, max compression
+gzip compressed data, was "reframed-1.4.0.tar", last modified: Mon May 22 07:19:57 2023, max compression
```

## Comparing `reframed-1.3.0.tar` & `reframed-1.4.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.139932 reframed-1.3.0/
--rw-r--r--   0 daniel     (501) staff       (20)      586 2021-02-26 10:14:55.000000 reframed-1.3.0/LICENSE
--rw-r--r--   0 daniel     (501) staff       (20)      242 2021-02-26 10:14:55.000000 reframed-1.3.0/MANIFEST.in
--rw-r--r--   0 daniel     (501) staff       (20)     4751 2023-03-06 13:15:06.140009 reframed-1.3.0/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)     4080 2021-02-26 10:14:55.000000 reframed-1.3.0/README.rst
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.132713 reframed-1.3.0/docs/
--rw-r--r--   0 daniel     (501) staff       (20)      609 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/Makefile
--rw-r--r--   0 daniel     (501) staff       (20)     2413 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/basics.rst
--rwxr-xr-x   0 daniel     (501) staff       (20)     4939 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/conf.py
--rw-r--r--   0 daniel     (501) staff       (20)      680 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/index.rst
--rw-r--r--   0 daniel     (501) staff       (20)      733 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/installation.rst
--rw-r--r--   0 daniel     (501) staff       (20)     1454 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/interfaces.rst
--rw-r--r--   0 daniel     (501) staff       (20)      770 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/make.bat
--rw-r--r--   0 daniel     (501) staff       (20)       61 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/modules.rst
--rw-r--r--   0 daniel     (501) staff       (20)     1367 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/reframed.cobra.rst
--rw-r--r--   0 daniel     (501) staff       (20)      720 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/reframed.community.rst
--rw-r--r--   0 daniel     (501) staff       (20)     1146 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/reframed.core.rst
--rw-r--r--   0 daniel     (501) staff       (20)      532 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/reframed.external.rst
--rw-r--r--   0 daniel     (501) staff       (20)      466 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/reframed.io.rst
--rw-r--r--   0 daniel     (501) staff       (20)      309 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/reframed.rst
--rw-r--r--   0 daniel     (501) staff       (20)     1078 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/reframed.solvers.rst
--rw-r--r--   0 daniel     (501) staff       (20)     2528 2021-02-26 10:14:55.000000 reframed-1.3.0/docs/simulation.rst
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.132834 reframed-1.3.0/reframed/
--rw-r--r--   0 daniel     (501) staff       (20)     1223 2023-03-06 13:13:56.000000 reframed-1.3.0/reframed/__init__.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.134366 reframed-1.3.0/reframed/alpha/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/alpha/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1741 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/alpha/fluxutils.py
--rw-r--r--   0 daniel     (501) staff       (20)     2726 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/alpha/gapMake.py
--rw-r--r--   0 daniel     (501) staff       (20)     5546 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/alpha/geneswitch.py
--rw-r--r--   0 daniel     (501) staff       (20)     2757 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/alpha/plotting.py
--rw-r--r--   0 daniel     (501) staff       (20)     3125 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/alpha/sampling.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.135570 reframed-1.3.0/reframed/cobra/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/cobra/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1055 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/cobra/auxotrophy.py
--rw-r--r--   0 daniel     (501) staff       (20)     4708 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/cobra/ensemble.py
--rw-r--r--   0 daniel     (501) staff       (20)     6529 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/cobra/knockout.py
--rw-r--r--   0 daniel     (501) staff       (20)     8541 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/cobra/medium.py
--rw-r--r--   0 daniel     (501) staff       (20)     3668 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/cobra/plotting.py
--rw-r--r--   0 daniel     (501) staff       (20)    15515 2023-03-02 10:28:10.000000 reframed-1.3.0/reframed/cobra/simulation.py
--rw-r--r--   0 daniel     (501) staff       (20)    15733 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/cobra/thermodynamics.py
--rw-r--r--   0 daniel     (501) staff       (20)    13014 2023-03-01 08:54:38.000000 reframed-1.3.0/reframed/cobra/transcriptomics.py
--rw-r--r--   0 daniel     (501) staff       (20)     3575 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/cobra/variability.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.136363 reframed-1.3.0/reframed/community/
--rw-r--r--   0 daniel     (501) staff       (20)     5573 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/community/SteadyCom.py
--rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/community/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     5344 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/community/model.py
--rw-r--r--   0 daniel     (501) staff       (20)     8416 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/community/simulation.py
--rw-r--r--   0 daniel     (501) staff       (20)    12030 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/community/simulation_old.py
--rw-r--r--   0 daniel     (501) staff       (20)     6973 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/community/solution.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.137216 reframed-1.3.0/reframed/core/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/core/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    13066 2021-06-30 13:01:24.000000 reframed-1.3.0/reframed/core/cbmodel.py
--rw-r--r--   0 daniel     (501) staff       (20)     2744 2021-03-05 13:40:40.000000 reframed-1.3.0/reframed/core/elements.py
--rw-r--r--   0 daniel     (501) staff       (20)     6872 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/core/environment.py
--rw-r--r--   0 daniel     (501) staff       (20)    19257 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/core/model.py
--rw-r--r--   0 daniel     (501) staff       (20)     3162 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/core/parser.py
--rw-r--r--   0 daniel     (501) staff       (20)    13416 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/core/transformation.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.137560 reframed-1.3.0/reframed/external/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/external/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     2688 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/external/cobrapy.py
--rw-r--r--   0 daniel     (501) staff       (20)     1427 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/external/escher.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.137902 reframed-1.3.0/reframed/io/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/io/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1240 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/io/cache.py
--rw-r--r--   0 daniel     (501) staff       (20)    27774 2021-06-30 13:59:55.000000 reframed-1.3.0/reframed/io/sbml.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.138817 reframed-1.3.0/reframed/solvers/
--rw-r--r--   0 daniel     (501) staff       (20)     1515 2023-02-14 14:34:59.000000 reframed-1.3.0/reframed/solvers/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    18519 2023-03-01 08:55:45.000000 reframed-1.3.0/reframed/solvers/cplex_solver.py
--rw-r--r--   0 daniel     (501) staff       (20)    12407 2023-03-01 08:55:23.000000 reframed-1.3.0/reframed/solvers/gurobi_solver.py
--rw-r--r--   0 daniel     (501) staff       (20)    10543 2023-03-01 08:55:29.000000 reframed-1.3.0/reframed/solvers/optlang_solver.py
--rw-r--r--   0 daniel     (501) staff       (20)     9475 2023-03-02 12:53:09.000000 reframed-1.3.0/reframed/solvers/pulp_solver.py
--rw-r--r--   0 daniel     (501) staff       (20)     7073 2021-02-26 10:14:55.000000 reframed-1.3.0/reframed/solvers/solution.py
--rw-r--r--   0 daniel     (501) staff       (20)     7117 2023-03-01 09:57:54.000000 reframed-1.3.0/reframed/solvers/solver.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.133589 reframed-1.3.0/reframed.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)     4751 2023-03-06 13:15:06.000000 reframed-1.3.0/reframed.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)     1934 2023-03-06 13:15:06.000000 reframed-1.3.0/reframed.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-03-06 13:15:06.000000 reframed-1.3.0/reframed.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-03-06 13:15:06.000000 reframed-1.3.0/reframed.egg-info/not-zip-safe
--rw-r--r--   0 daniel     (501) staff       (20)       33 2023-03-06 13:15:06.000000 reframed-1.3.0/reframed.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)       15 2023-03-06 13:15:06.000000 reframed-1.3.0/reframed.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)       67 2023-03-06 13:15:06.140270 reframed-1.3.0/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)     1273 2023-03-06 13:13:45.000000 reframed-1.3.0/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.139068 reframed-1.3.0/tests/
--rw-r--r--   0 daniel     (501) staff       (20)       63 2021-02-26 10:14:55.000000 reframed-1.3.0/tests/__init__.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-06 13:15:06.139810 reframed-1.3.0/tests/data/
--rw-r--r--   0 daniel     (501) staff       (20)    40216 2021-02-26 10:14:55.000000 reframed-1.3.0/tests/data/e_coli_core.xml.gz
--rw-r--r--   0 daniel     (501) staff       (20)   470620 2021-02-26 10:14:55.000000 reframed-1.3.0/tests/data/iML1515.xml.gz
--rw-r--r--   0 daniel     (501) staff       (20)     5431 2023-03-01 09:00:19.000000 reframed-1.3.0/tests/data/model_cobra.xml.gz
--rw-r--r--   0 daniel     (501) staff       (20)     5861 2023-03-01 09:00:23.000000 reframed-1.3.0/tests/data/model_fbc2.xml.gz
--rw-r--r--   0 daniel     (501) staff       (20)     5229 2021-02-26 10:14:55.000000 reframed-1.3.0/tests/test_reframed.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.916307 reframed-1.4.0/
+-rw-r--r--   0 daniel     (501) staff       (20)      586 2021-02-26 10:14:55.000000 reframed-1.4.0/LICENSE
+-rw-r--r--   0 daniel     (501) staff       (20)      242 2021-02-26 10:14:55.000000 reframed-1.4.0/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)     4760 2023-05-22 07:19:57.916423 reframed-1.4.0/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     4089 2023-05-22 07:16:53.000000 reframed-1.4.0/README.rst
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.907098 reframed-1.4.0/docs/
+-rw-r--r--   0 daniel     (501) staff       (20)      609 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/Makefile
+-rw-r--r--   0 daniel     (501) staff       (20)     2413 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/basics.rst
+-rwxr-xr-x   0 daniel     (501) staff       (20)     4939 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/conf.py
+-rw-r--r--   0 daniel     (501) staff       (20)      680 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/index.rst
+-rw-r--r--   0 daniel     (501) staff       (20)      733 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/installation.rst
+-rw-r--r--   0 daniel     (501) staff       (20)     1454 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/interfaces.rst
+-rw-r--r--   0 daniel     (501) staff       (20)      770 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/make.bat
+-rw-r--r--   0 daniel     (501) staff       (20)       61 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/modules.rst
+-rw-r--r--   0 daniel     (501) staff       (20)     1367 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/reframed.cobra.rst
+-rw-r--r--   0 daniel     (501) staff       (20)      720 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/reframed.community.rst
+-rw-r--r--   0 daniel     (501) staff       (20)     1146 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/reframed.core.rst
+-rw-r--r--   0 daniel     (501) staff       (20)      532 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/reframed.external.rst
+-rw-r--r--   0 daniel     (501) staff       (20)      466 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/reframed.io.rst
+-rw-r--r--   0 daniel     (501) staff       (20)      309 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/reframed.rst
+-rw-r--r--   0 daniel     (501) staff       (20)     1078 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/reframed.solvers.rst
+-rw-r--r--   0 daniel     (501) staff       (20)     2528 2021-02-26 10:14:55.000000 reframed-1.4.0/docs/simulation.rst
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.907275 reframed-1.4.0/reframed/
+-rw-r--r--   0 daniel     (501) staff       (20)     1223 2023-05-22 07:17:05.000000 reframed-1.4.0/reframed/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.908933 reframed-1.4.0/reframed/alpha/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/alpha/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1741 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/alpha/fluxutils.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2726 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/alpha/gapMake.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5546 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/alpha/geneswitch.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2757 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/alpha/plotting.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3125 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/alpha/sampling.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.910291 reframed-1.4.0/reframed/cobra/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/cobra/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1055 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/cobra/auxotrophy.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4708 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/cobra/ensemble.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6529 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/cobra/knockout.py
+-rw-r--r--   0 daniel     (501) staff       (20)     8541 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/cobra/medium.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3668 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/cobra/plotting.py
+-rw-r--r--   0 daniel     (501) staff       (20)    15515 2023-03-02 10:28:10.000000 reframed-1.4.0/reframed/cobra/simulation.py
+-rw-r--r--   0 daniel     (501) staff       (20)    15733 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/cobra/thermodynamics.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13014 2023-03-01 08:54:38.000000 reframed-1.4.0/reframed/cobra/transcriptomics.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3575 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/cobra/variability.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.911103 reframed-1.4.0/reframed/community/
+-rw-r--r--   0 daniel     (501) staff       (20)     5573 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/community/SteadyCom.py
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/community/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5344 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/community/model.py
+-rw-r--r--   0 daniel     (501) staff       (20)     8416 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/community/simulation.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12030 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/community/simulation_old.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6973 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/community/solution.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.912253 reframed-1.4.0/reframed/core/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/core/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13066 2021-06-30 13:01:24.000000 reframed-1.4.0/reframed/core/cbmodel.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2744 2021-03-05 13:40:40.000000 reframed-1.4.0/reframed/core/elements.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6872 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/core/environment.py
+-rw-r--r--   0 daniel     (501) staff       (20)    19257 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/core/model.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3162 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/core/parser.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13416 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/core/transformation.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.912691 reframed-1.4.0/reframed/external/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/external/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2688 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/external/cobrapy.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1427 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/external/escher.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.913123 reframed-1.4.0/reframed/io/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/io/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1240 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/io/cache.py
+-rw-r--r--   0 daniel     (501) staff       (20)    27774 2021-06-30 13:59:55.000000 reframed-1.4.0/reframed/io/sbml.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.914172 reframed-1.4.0/reframed/solvers/
+-rw-r--r--   0 daniel     (501) staff       (20)     1951 2023-04-24 09:26:55.000000 reframed-1.4.0/reframed/solvers/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    19012 2023-05-22 07:14:54.000000 reframed-1.4.0/reframed/solvers/cplex_solver.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12467 2023-04-25 08:53:36.000000 reframed-1.4.0/reframed/solvers/gurobi_solver.py
+-rw-r--r--   0 daniel     (501) staff       (20)    10543 2023-03-01 08:55:29.000000 reframed-1.4.0/reframed/solvers/optlang_solver.py
+-rw-r--r--   0 daniel     (501) staff       (20)    10248 2023-05-22 07:14:34.000000 reframed-1.4.0/reframed/solvers/pulp_solver.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7073 2021-02-26 10:14:55.000000 reframed-1.4.0/reframed/solvers/solution.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7117 2023-04-25 08:54:23.000000 reframed-1.4.0/reframed/solvers/solver.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.908125 reframed-1.4.0/reframed.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     4760 2023-05-22 07:19:57.000000 reframed-1.4.0/reframed.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     1934 2023-05-22 07:19:57.000000 reframed-1.4.0/reframed.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-22 07:19:57.000000 reframed-1.4.0/reframed.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-22 07:19:57.000000 reframed-1.4.0/reframed.egg-info/not-zip-safe
+-rw-r--r--   0 daniel     (501) staff       (20)       33 2023-05-22 07:19:57.000000 reframed-1.4.0/reframed.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       15 2023-05-22 07:19:57.000000 reframed-1.4.0/reframed.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       67 2023-05-22 07:19:57.916742 reframed-1.4.0/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)     1273 2023-05-22 07:15:27.000000 reframed-1.4.0/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.914427 reframed-1.4.0/tests/
+-rw-r--r--   0 daniel     (501) staff       (20)       63 2021-02-26 10:14:55.000000 reframed-1.4.0/tests/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 07:19:57.916136 reframed-1.4.0/tests/data/
+-rw-r--r--   0 daniel     (501) staff       (20)    40216 2021-02-26 10:14:55.000000 reframed-1.4.0/tests/data/e_coli_core.xml.gz
+-rw-r--r--   0 daniel     (501) staff       (20)   470620 2021-02-26 10:14:55.000000 reframed-1.4.0/tests/data/iML1515.xml.gz
+-rw-r--r--   0 daniel     (501) staff       (20)     5431 2023-05-22 07:18:58.000000 reframed-1.4.0/tests/data/model_cobra.xml.gz
+-rw-r--r--   0 daniel     (501) staff       (20)     5861 2023-05-22 07:19:01.000000 reframed-1.4.0/tests/data/model_fbc2.xml.gz
+-rw-r--r--   0 daniel     (501) staff       (20)     5229 2021-02-26 10:14:55.000000 reframed-1.4.0/tests/test_reframed.py
```

### Comparing `reframed-1.3.0/LICENSE` & `reframed-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/PKG-INFO` & `reframed-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reframed
-Version: 1.3.0
+Version: 1.4.0
 Summary: metabolic modeling package
 Home-page: https://github.com/cdanielmachado/reframed
 Author: Daniel Machado
 Author-email: cdanielmachado@gmail.com
 License: Apache Software License 2.0
 Keywords: reframed
 Classifier: License :: OSI Approved :: Apache Software License
@@ -79,14 +79,13 @@
 +-----------------------+-----------------------+-----------------------+
 | SteadyCom             | Community simulation  | (Chan et al, 2017)    |
 +-----------------------+-----------------------+-----------------------+
 
 Credits and License
 -------------------
 
-Developed by Daniel Machado at the European Molecular Biology Laboratory
-(2019).
+Developed by Daniel Machado at the Norwegian University of Science and Technology (NTNU).
 
 **ReFramed** is a refactored version of the
 `framed <https://github.com/cdanielmachado/framed>`__ library.
 
 Released under an Apache License.
```

### Comparing `reframed-1.3.0/README.rst` & `reframed-1.4.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,13 @@
 +-----------------------+-----------------------+-----------------------+
 | SteadyCom             | Community simulation  | (Chan et al, 2017)    |
 +-----------------------+-----------------------+-----------------------+
 
 Credits and License
 -------------------
 
-Developed by Daniel Machado at the European Molecular Biology Laboratory
-(2019).
+Developed by Daniel Machado at the Norwegian University of Science and Technology (NTNU).
 
 **ReFramed** is a refactored version of the
 `framed <https://github.com/cdanielmachado/framed>`__ library.
 
 Released under an Apache License.
```

### Comparing `reframed-1.3.0/docs/Makefile` & `reframed-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/basics.rst` & `reframed-1.4.0/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/conf.py` & `reframed-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/index.rst` & `reframed-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/installation.rst` & `reframed-1.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/interfaces.rst` & `reframed-1.4.0/docs/interfaces.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/make.bat` & `reframed-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/reframed.cobra.rst` & `reframed-1.4.0/docs/reframed.cobra.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/reframed.community.rst` & `reframed-1.4.0/docs/reframed.community.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/reframed.core.rst` & `reframed-1.4.0/docs/reframed.core.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/reframed.external.rst` & `reframed-1.4.0/docs/reframed.external.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/reframed.solvers.rst` & `reframed-1.4.0/docs/reframed.solvers.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/docs/simulation.rst` & `reframed-1.4.0/docs/simulation.rst`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/__init__.py` & `reframed-1.4.0/reframed/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for ReFramed."""
 
 __author__ = "Daniel Machado"
 __email__ = 'cdanielmachado@gmail.com'
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 
 
 from .core.model import Model, Metabolite, Compartment, Reaction, ReactionType
 from .core.cbmodel import CBReaction, Gene, Protein, GPRAssociation, CBModel
 from .core.environment import Environment
 from .core.transformation import make_irreversible, simplify, gpr_transform
```

### Comparing `reframed-1.3.0/reframed/alpha/fluxutils.py` & `reframed-1.4.0/reframed/alpha/fluxutils.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/alpha/gapMake.py` & `reframed-1.4.0/reframed/alpha/gapMake.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/alpha/geneswitch.py` & `reframed-1.4.0/reframed/alpha/geneswitch.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/alpha/plotting.py` & `reframed-1.4.0/reframed/alpha/plotting.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/alpha/sampling.py` & `reframed-1.4.0/reframed/alpha/sampling.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/cobra/auxotrophy.py` & `reframed-1.4.0/reframed/cobra/auxotrophy.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/cobra/ensemble.py` & `reframed-1.4.0/reframed/cobra/ensemble.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/cobra/knockout.py` & `reframed-1.4.0/reframed/cobra/knockout.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/cobra/medium.py` & `reframed-1.4.0/reframed/cobra/medium.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/cobra/plotting.py` & `reframed-1.4.0/reframed/cobra/plotting.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/cobra/simulation.py` & `reframed-1.4.0/reframed/cobra/simulation.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/cobra/thermodynamics.py` & `reframed-1.4.0/reframed/cobra/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/cobra/transcriptomics.py` & `reframed-1.4.0/reframed/cobra/transcriptomics.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/cobra/variability.py` & `reframed-1.4.0/reframed/cobra/variability.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/community/SteadyCom.py` & `reframed-1.4.0/reframed/community/SteadyCom.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/community/model.py` & `reframed-1.4.0/reframed/community/model.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/community/simulation.py` & `reframed-1.4.0/reframed/community/simulation.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/community/simulation_old.py` & `reframed-1.4.0/reframed/community/simulation_old.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/community/solution.py` & `reframed-1.4.0/reframed/community/solution.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/core/cbmodel.py` & `reframed-1.4.0/reframed/core/cbmodel.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/core/elements.py` & `reframed-1.4.0/reframed/core/elements.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/core/environment.py` & `reframed-1.4.0/reframed/core/environment.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/core/model.py` & `reframed-1.4.0/reframed/core/model.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/core/parser.py` & `reframed-1.4.0/reframed/core/parser.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/core/transformation.py` & `reframed-1.4.0/reframed/core/transformation.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/external/cobrapy.py` & `reframed-1.4.0/reframed/external/cobrapy.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/external/escher.py` & `reframed-1.4.0/reframed/external/escher.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/io/cache.py` & `reframed-1.4.0/reframed/io/cache.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/io/sbml.py` & `reframed-1.4.0/reframed/io/sbml.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/solvers/__init__.py` & `reframed-1.4.0/reframed/solvers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from .solver import Parameter
-
 solvers = dict()
 
 try:
     from .gurobi_solver import GurobiSolver
     solvers['gurobi'] = GurobiSolver
 except ImportError:
     pass
@@ -17,26 +15,50 @@
 
 try:
     from .optlang_solver import OptLangSolver
     solvers['optlang'] = OptLangSolver
 except ImportError:
     pass
 
+try:
+    from .pulp_solver import SCIP_Solver
+    solvers['scip'] = SCIP_Solver
+except ImportError:
+    pass
+
+try:
+    from .pulp_solver import HiGHS_Solver
+    solvers['highs'] = HiGHS_Solver
+except ImportError:
+    pass
+
+try:
+    from .pulp_solver import PulpCplex
+    solvers['pulp_cplex'] = PulpCplex
+except ImportError:
+    pass
+
+try:
+    from .pulp_solver import PulpGurobi
+    solvers['pulp_gurobi'] = PulpGurobi
+except ImportError:
+    pass
+
 
 default_solver = None
 
 
 def get_default_solver():
 
     global default_solver
 
     if default_solver:
         return default_solver
 
-    solver_order = ['cplex', 'gurobi', 'optlang']
+    solver_order = ['gurobi', 'cplex', 'highs', 'scip', 'optlang']
 
     for solver in solver_order:
         if solver in list(solvers.keys()):
             default_solver = solver
             break
 
     if not default_solver:
```

### Comparing `reframed-1.3.0/reframed/solvers/cplex_solver.py` & `reframed-1.4.0/reframed/solvers/cplex_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -287,28 +287,30 @@
         table = model.metabolite_reaction_lookup()
         lhs = list(table.values())
         senses = ['='] * len(constr_ids)
         rhs = [0] * len(constr_ids)
         self.add_constraints(constr_ids, lhs, senses, rhs)
 
     def solve(self, linear=None, quadratic=None, minimize=None, model=None, constraints=None, get_values=True,
-              shadow_prices=False, reduced_costs=False, pool_size=0, pool_gap=None):
+              shadow_prices=False, reduced_costs=False, pool_size=0, pool_gap=None, emphasis=None, timelimit=None):
         """ Solve the optimization problem.
 
         Arguments:
             linear (str or dict): linear coefficients (or a single variable to optimize)
             quadratic (dict): quadratic objective (optional)
             minimize (bool): solve a minimization problem (default: True)
             model (CBModel): model (optional, leave blank to reuse previous model structure)
             constraints (dict): additional constraints (optional)
             get_values (bool or list): set to false for speedup if you only care about the objective value (default: True)
             shadow_prices (bool): return shadow prices if available (default: False)
             reduced_costs (bool): return reduced costs if available (default: False)
             pool_size (int): calculate solution pool of given size (only for MILP problems)
             pool_gap (float): maximum relative gap for solutions in pool (optional)
+            emphasis (int): MIP emphasis switch. Controls trade-offs between speed, feasibility, optimality, and moving bounds in MIP  (default: Balance optimality and feasibility)
+            timelimit (int): Sets the maximum time, in seconds, for a call to an optimizer (default: no limit)
 
         Returns:
             Solution: solution
         """
 
         if model:
             self.build_problem(model)
@@ -319,15 +321,18 @@
             changed_lb, changed_ub = self.temporary_bounds(constraints)
 
         self.set_objective(linear, quadratic, minimize)
 
         # run the optimization
 
         if pool_size <= 1:
-
+            
+            if emphasis: problem.parameters.emphasis.mip.set(emphasis)
+            if timelimit: problem.parameters.timelimit.set(timelimit)
+                
             problem.solve()
 
             status = self.status_mapping.get(problem.solution.get_status(), Status.UNKNOWN)
             message = str(problem.solution.get_status_string())
 
             if status == Status.OPTIMAL:
                 fobj = problem.solution.get_objective_value()
```

### Comparing `reframed-1.3.0/reframed/solvers/gurobi_solver.py` & `reframed-1.4.0/reframed/solvers/gurobi_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,16 @@
                     old_constraints[r_id] = (lpvar.lb, lpvar.ub)
                     lpvar.lb = infinity_fix(lb)
                     lpvar.ub = infinity_fix(ub)
                 else:
                     warn(f"Constrained variable '{r_id}' not previously declared")
             problem.update()
 
-        self.set_objective(linear, quadratic, minimize)
+        if linear is not None or quadratic is not None:
+            self.set_objective(linear, quadratic, minimize)
 
         # run the optimization
         if pool_size <= 1:
 
             problem.optimize()
 
             status = status_mapping.get(problem.status, Status.UNKNOWN)
```

### Comparing `reframed-1.3.0/reframed/solvers/optlang_solver.py` & `reframed-1.4.0/reframed/solvers/optlang_solver.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/solvers/pulp_solver.py` & `reframed-1.4.0/reframed/solvers/pulp_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,23 @@
         self.problem = LpProblem()
         self.variables = {}
         self.constraints = {}
 
         if interface is None:
             self.interface = LpSolverDefault
         else:
-            self.interface = getSolver(interface)
+            self.interface = getSolver(interface, msg=False)
 
-#        self.set_parameters(default_parameters)
-#        self.set_logging(False)
+            # if interface == 'HiGHS_CMD':
+            #     self.interface = getSolver(interface, timeLimit=3600)
+
+            # if interface == 'SCIP_CMD':
+            #     self.interface = getSolver(interface, timeLimit=3600, options=["set presolving maxrounds 0"])
+
+    #    self.set_parameters(default_parameters)
 
         if model:
             self.build_problem(model)
 
     def add_variable(self, var_id, lb=-inf, ub=inf, vartype=VarType.CONTINUOUS, update=True):
         """ Add a variable to the current problem.
 
@@ -169,17 +174,18 @@
             Setting the objective is optional. It can also be passed directly when calling **solve**.
 
         """
 
         if quadratic is not None:
             raise Exception('PuLP wrapper does not support quadratic objectives.')
         
-        objective = lpSum([coeff * self.variables[var_id] for var_id, coeff in linear.items() if coeff != 0])
-        self.problem.setObjective(objective)
-        self.problem.sense = LpMinimize if minimize else LpMaximize
+        if linear is not None:
+            objective = lpSum([coeff * self.variables[var_id] for var_id, coeff in linear.items() if coeff != 0])
+            self.problem.setObjective(objective)
+            self.problem.sense = LpMinimize if minimize else LpMaximize
 
     def build_problem(self, model):
         """ Create problem structure for a given model.
 
         Arguments:
             model : CBModel
         """
@@ -279,8 +285,25 @@
         Arguments:
             filename (str): file path
         """
 
         self.problem.writeLP(filename)
 
 
+class SCIP_Solver(PuLPSolver):
+    def __init__(self, model=None):
+        PuLPSolver.__init__(self, model, 'SCIP_CMD')
+
+
+class HiGHS_Solver(PuLPSolver):
+    def __init__(self, model=None):
+        PuLPSolver.__init__(self, model, 'HiGHS_CMD')
+
+
+class PulpCplex(PuLPSolver):
+    def __init__(self, model=None):
+        PuLPSolver.__init__(self, model, 'CPLEX_PY')
+
 
+class PulpGurobi(PuLPSolver):
+    def __init__(self, model=None):
+        PuLPSolver.__init__(self, model, 'GUROBI')
```

### Comparing `reframed-1.3.0/reframed/solvers/solution.py` & `reframed-1.4.0/reframed/solvers/solution.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed/solvers/solver.py` & `reframed-1.4.0/reframed/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/reframed.egg-info/PKG-INFO` & `reframed-1.4.0/reframed.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reframed
-Version: 1.3.0
+Version: 1.4.0
 Summary: metabolic modeling package
 Home-page: https://github.com/cdanielmachado/reframed
 Author: Daniel Machado
 Author-email: cdanielmachado@gmail.com
 License: Apache Software License 2.0
 Keywords: reframed
 Classifier: License :: OSI Approved :: Apache Software License
@@ -79,14 +79,13 @@
 +-----------------------+-----------------------+-----------------------+
 | SteadyCom             | Community simulation  | (Chan et al, 2017)    |
 +-----------------------+-----------------------+-----------------------+
 
 Credits and License
 -------------------
 
-Developed by Daniel Machado at the European Molecular Biology Laboratory
-(2019).
+Developed by Daniel Machado at the Norwegian University of Science and Technology (NTNU).
 
 **ReFramed** is a refactored version of the
 `framed <https://github.com/cdanielmachado/framed>`__ library.
 
 Released under an Apache License.
```

### Comparing `reframed-1.3.0/reframed.egg-info/SOURCES.txt` & `reframed-1.4.0/reframed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/setup.py` & `reframed-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     keywords='reframed',
     name='reframed',
     packages=find_packages(),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/cdanielmachado/reframed',
-    version='1.3.0',
+    version='1.4.0',
     zip_safe=False,
 )
```

### Comparing `reframed-1.3.0/tests/data/e_coli_core.xml.gz` & `reframed-1.4.0/tests/data/e_coli_core.xml.gz`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/tests/data/iML1515.xml.gz` & `reframed-1.4.0/tests/data/iML1515.xml.gz`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/tests/data/model_cobra.xml.gz` & `reframed-1.4.0/tests/data/model_cobra.xml.gz`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/tests/data/model_fbc2.xml.gz` & `reframed-1.4.0/tests/data/model_fbc2.xml.gz`

 * *Files identical despite different names*

### Comparing `reframed-1.3.0/tests/test_reframed.py` & `reframed-1.4.0/tests/test_reframed.py`

 * *Files identical despite different names*

