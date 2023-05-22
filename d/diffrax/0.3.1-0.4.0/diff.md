# Comparing `tmp/diffrax-0.3.1.tar.gz` & `tmp/diffrax-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffrax-0.3.1.tar", last modified: Thu Feb 23 02:28:06 2023, max compression
+gzip compressed data, was "diffrax-0.4.0.tar", last modified: Mon May 22 14:23:00 2023, max compression
```

## Comparing `diffrax-0.3.1.tar` & `diffrax-0.4.0.tar`

### file list

```diff
@@ -1,85 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 02:28:06.079354 diffrax-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-23 02:28:01.000000 diffrax-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 02:28:01.000000 diffrax-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-02-23 02:28:06.079354 diffrax-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-02-23 02:28:01.000000 diffrax-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 02:28:06.071354 diffrax-0.3.1/diffrax/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    27144 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/autocitation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 02:28:06.071354 diffrax-0.3.1/diffrax/brownian/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/brownian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/brownian/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/brownian/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/brownian/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    27468 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/global_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/local_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 02:28:06.071354 diffrax-0.3.1/diffrax/nonlinear_solver/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/nonlinear_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/nonlinear_solver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/nonlinear_solver/newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/saveat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 02:28:06.075354 diffrax-0.3.1/diffrax/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/bosh3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/dopri5.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/dopri8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/euler_heun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/heun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/implicit_euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/kvaerno3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/kvaerno4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/kvaerno5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/leapfrog_midpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/midpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/milstein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/ralston.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/reversible_heun.py
--rw-r--r--   0 runner    (1001) docker     (123)    32814 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/runge_kutta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/semi_implicit_euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/solver/tsit5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 02:28:06.075354 diffrax-0.3.1/diffrax/step_size_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/step_size_controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27884 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/step_size_controller/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/step_size_controller/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/step_size_controller/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-02-23 02:28:01.000000 diffrax-0.3.1/diffrax/term.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 02:28:06.071354 diffrax-0.3.1/diffrax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-02-23 02:28:05.000000 diffrax-0.3.1/diffrax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-23 02:28:06.000000 diffrax-0.3.1/diffrax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 02:28:05.000000 diffrax-0.3.1/diffrax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 02:28:05.000000 diffrax-0.3.1/diffrax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-23 02:28:05.000000 diffrax-0.3.1/diffrax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-23 02:28:05.000000 diffrax-0.3.1/diffrax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 02:28:06.079354 diffrax-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-02-23 02:28:01.000000 diffrax-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 02:28:06.075354 diffrax-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_adaptive_stepsize_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_brownian.py
--rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_detest.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_global_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_local_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_newton_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_saveat_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_step_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-02-23 02:28:01.000000 diffrax-0.3.1/test/test_vmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.527938 diffrax-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 14:22:55.000000 diffrax-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 14:22:55.000000 diffrax-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-22 14:23:00.527938 diffrax-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-22 14:22:55.000000 diffrax-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.519939 diffrax-0.4.0/diffrax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27893 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/autocitation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.519939 diffrax-0.4.0/diffrax/brownian/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/brownian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/brownian/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/brownian/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/brownian/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/global_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31501 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/local_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.523939 diffrax-0.4.0/diffrax/nonlinear_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/nonlinear_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/nonlinear_solver/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/nonlinear_solver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/nonlinear_solver/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/saveat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.523939 diffrax-0.4.0/diffrax/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/bosh3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/dopri5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/dopri8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/euler_heun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/heun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/implicit_euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kencarp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kencarp4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kencarp5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kvaerno3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kvaerno4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kvaerno5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/leapfrog_midpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/midpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/milstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/ralston.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/reversible_heun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45338 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/runge_kutta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/semi_implicit_euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/sil3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/tsit5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.523939 diffrax-0.4.0/diffrax/step_size_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/step_size_controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28338 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/step_size_controller/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/step_size_controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/step_size_controller/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/term.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.519939 diffrax-0.4.0/diffrax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:23:00.527938 diffrax-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-22 14:22:56.000000 diffrax-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.523939 diffrax-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_adaptive_stepsize_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_brownian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_detest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_global_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_local_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_newton_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_saveat_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_step_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_vmap.py
```

### Comparing `diffrax-0.3.1/LICENSE` & `diffrax-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/PKG-INFO` & `diffrax-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,95 @@
 Metadata-Version: 2.1
 Name: diffrax
-Version: 0.3.1
+Version: 0.4.0
 Summary: GPU+autodiff-capable ODE/SDE/CDE solvers written in JAX.
 Home-page: https://github.com/patrick-kidger/diffrax
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
-Description: <h1 align='center'>Diffrax</h1>
-        <h2 align='center'>Numerical differential equation solvers in JAX. Autodifferentiable and GPU-capable.</h2>
-        
-        Diffrax is a [JAX](https://github.com/google/jax)-based library providing numerical differential equation solvers.
-        
-        Features include:
-        
-        - ODE/SDE/CDE (ordinary/stochastic/controlled) solvers;
-        - lots of different solvers (including `Tsit5`, `Dopri8`, symplectic solvers, implicit solvers);
-        - vmappable _everything_ (including the region of integration);
-        - using a PyTree as the state;
-        - dense solutions;
-        - multiple adjoint methods for backpropagation;
-        - support for neural differential equations.
-        
-        _From a technical point of view, the internal structure of the library is pretty cool -- all kinds of equations (ODEs, SDEs, CDEs) are solved in a unified way (rather than being treated separately), producing a small tightly-written library._
-        
-        ## Installation
-        
-        ```
-        pip install diffrax
-        ```
-        
-        Requires Python 3.8+, JAX 0.4.3+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.0+.
-        
-        ## Documentation
-        
-        Available at [https://docs.kidger.site/diffrax](https://docs.kidger.site/diffrax).
-        
-        ## Quick example
-        
-        ```python
-        from diffrax import diffeqsolve, ODETerm, Dopri5
-        import jax.numpy as jnp
-        
-        def f(t, y, args):
-            return -y
-        
-        term = ODETerm(f)
-        solver = Dopri5()
-        y0 = jnp.array([2., 3.])
-        solution = diffeqsolve(term, solver, t0=0, t1=1, dt0=0.1, y0=y0)
-        ```
-        
-        Here, `Dopri5` refers to the Dormand--Prince 5(4) numerical differential equation solver, which is a standard choice for many problems.
-        
-        ## Citation
-        
-        If you found this library useful in academic research, please cite: [(arXiv link)](https://arxiv.org/abs/2202.02435)
-        
-        ```bibtex
-        @phdthesis{kidger2021on,
-            title={{O}n {N}eural {D}ifferential {E}quations},
-            author={Patrick Kidger},
-            year={2021},
-            school={University of Oxford},
-        }
-        ```
-        
-        (Also consider starring the project on GitHub.)
-        
-        ## See also
-        
-        Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
-        
-        Type annotations and runtime checking for PyTrees and shape/dtype of JAX arrays: [jaxtyping](https://github.com/google/jaxtyping).
-        
-        Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
-        
-        SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: ~=3.8
+Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align='center'>Diffrax</h1>
+<h2 align='center'>Numerical differential equation solvers in JAX. Autodifferentiable and GPU-capable.</h2>
+
+Diffrax is a [JAX](https://github.com/google/jax)-based library providing numerical differential equation solvers.
+
+Features include:
+
+- ODE/SDE/CDE (ordinary/stochastic/controlled) solvers;
+- lots of different solvers (including `Tsit5`, `Dopri8`, symplectic solvers, implicit solvers);
+- vmappable _everything_ (including the region of integration);
+- using a PyTree as the state;
+- dense solutions;
+- multiple adjoint methods for backpropagation;
+- support for neural differential equations.
+
+_From a technical point of view, the internal structure of the library is pretty cool -- all kinds of equations (ODEs, SDEs, CDEs) are solved in a unified way (rather than being treated separately), producing a small tightly-written library._
+
+## Installation
+
+```
+pip install diffrax
+```
+
+Requires Python 3.9+, JAX 0.4.4+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.4+.
+
+## Documentation
+
+Available at [https://docs.kidger.site/diffrax](https://docs.kidger.site/diffrax).
+
+## Quick example
+
+```python
+from diffrax import diffeqsolve, ODETerm, Dopri5
+import jax.numpy as jnp
+
+def f(t, y, args):
+    return -y
+
+term = ODETerm(f)
+solver = Dopri5()
+y0 = jnp.array([2., 3.])
+solution = diffeqsolve(term, solver, t0=0, t1=1, dt0=0.1, y0=y0)
+```
+
+Here, `Dopri5` refers to the Dormand--Prince 5(4) numerical differential equation solver, which is a standard choice for many problems.
+
+## Citation
+
+If you found this library useful in academic research, please cite: [(arXiv link)](https://arxiv.org/abs/2202.02435)
+
+```bibtex
+@phdthesis{kidger2021on,
+    title={{O}n {N}eural {D}ifferential {E}quations},
+    author={Patrick Kidger},
+    year={2021},
+    school={University of Oxford},
+}
+```
+
+(Also consider starring the project on GitHub.)
+
+## See also
+
+Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
+
+Type annotations and runtime checking for PyTrees and shape/dtype of JAX arrays: [jaxtyping](https://github.com/google/jaxtyping).
+
+Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
+
+SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
```

### Comparing `diffrax-0.3.1/README.md` & `diffrax-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ## Installation
 
 ```
 pip install diffrax
 ```
 
-Requires Python 3.8+, JAX 0.4.3+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.0+.
+Requires Python 3.9+, JAX 0.4.4+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.4+.
 
 ## Documentation
 
 Available at [https://docs.kidger.site/diffrax](https://docs.kidger.site/diffrax).
 
 ## Quick example
```

### Comparing `diffrax-0.3.1/diffrax/__init__.py` & `diffrax-0.4.0/diffrax/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     FourthOrderPolynomialInterpolation,
     LocalLinearInterpolation,
     ThirdOrderHermitePolynomialInterpolation,
 )
 from .misc import adjoint_rms_seminorm
 from .nonlinear_solver import (
     AbstractNonlinearSolver,
+    AffineNonlinearSolver,
     NewtonNonlinearSolver,
     NonlinearSolution,
 )
 from .path import AbstractPath
 from .saveat import SaveAt, SubSaveAt
 from .solution import is_event, is_okay, is_successful, RESULTS, Solution
 from .solver import (
@@ -56,22 +57,27 @@
     Dopri8,
     Euler,
     EulerHeun,
     HalfSolver,
     Heun,
     ImplicitEuler,
     ItoMilstein,
+    KenCarp3,
+    KenCarp4,
+    KenCarp5,
     Kvaerno3,
     Kvaerno4,
     Kvaerno5,
     LeapfrogMidpoint,
     Midpoint,
+    MultiButcherTableau,
     Ralston,
     ReversibleHeun,
     SemiImplicitEuler,
+    Sil3,
     StratonovichMilstein,
     Tsit5,
 )
 from .step_size_controller import (
     AbstractAdaptiveStepSizeController,
     AbstractStepSizeController,
     ConstantStepSize,
@@ -83,8 +89,8 @@
     ControlTerm,
     MultiTerm,
     ODETerm,
     WeaklyDiagonalControlTerm,
 )
 
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
```

### Comparing `diffrax-0.3.1/diffrax/ad.py` & `diffrax-0.4.0/diffrax/ad.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/adjoint.py` & `diffrax-0.4.0/diffrax/adjoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from equinox.internal import ω
 
 from .ad import implicit_jvp
 from .heuristics import is_sde, is_unsafe_sde
 from .saveat import save_y, SaveAt, SubSaveAt
-from .solver import AbstractItoSolver, AbstractStratonovichSolver
+from .solver import AbstractItoSolver, AbstractRungeKutta, AbstractStratonovichSolver
 from .term import AbstractTerm, AdjointTerm
 
 
 def _is_none(x):
     return x is None
 
 
@@ -328,14 +328,15 @@
     So unless you need forward-mode autodifferentiation then
     [`diffrax.RecursiveCheckpointAdjoint`][] should be preferred.
     """
 
     def loop(
         self,
         *,
+        solver,
         max_steps,
         terms,
         throw,
         passed_solver_state,
         passed_controller_state,
         **kwargs,
     ):
@@ -358,18 +359,23 @@
                 "number of steps, or switch to "
                 "`adjoint=RecursiveCheckpointAdjoint(checkpoints=...)`, with an "
                 "explicitly specified number of checkpoints."
             )
         else:
             kind = "bounded"
             msg = None
+        # Support forward-mode autodiff.
+        # TODO: remove this hack once we can JVP through custom_vjps.
+        if isinstance(solver, AbstractRungeKutta) and solver.scan_kind is None:
+            solver = eqx.tree_at(lambda s: s.scan_kind, solver, "bounded")
         inner_while_loop = ft.partial(_inner_loop, kind=kind)
         outer_while_loop = ft.partial(_outer_loop, kind=kind)
         final_state = self._loop(
             **kwargs,
+            solver=solver,
             max_steps=max_steps,
             terms=terms,
             inner_while_loop=inner_while_loop,
             outer_while_loop=outer_while_loop,
         )
         if msg is not None:
             final_state = eqxi.nondifferentiable_backward(
@@ -531,14 +537,16 @@
     del y__args__terms
     diff_args = eqx.filter(args, eqx.is_inexact_array)
     diff_terms = eqx.filter(terms, eqx.is_inexact_array)
     zeros_like_y = jtu.tree_map(jnp.zeros_like, y)
     zeros_like_diff_args = jtu.tree_map(jnp.zeros_like, diff_args)
     zeros_like_diff_terms = jtu.tree_map(jnp.zeros_like, diff_terms)
     del diff_args, diff_terms
+    # TODO: have this look inside MultiTerms? Need to think about the math. i.e.:
+    # is_leaf=lambda x: isinstance(x, AbstractTerm) and not isinstance(x, MultiTerm)
     adjoint_terms = jtu.tree_map(
         AdjointTerm, terms, is_leaf=lambda x: isinstance(x, AbstractTerm)
     )
     diffeqsolve = self._diffeqsolve
     kwargs = dict(
         args=args,
         adjoint=self,
@@ -758,14 +766,19 @@
             elif not isinstance(solver, AbstractStratonovichSolver):
                 warnings.warn(
                     f"{solver.__class__.__name__} is not marked as converging to "
                     "either the Itô or the Stratonovich solution. Note that "
                     "`BacksolveAdjoint` will only produce the correct solution for "
                     "Stratonovich SDEs."
                 )
+        if jtu.tree_structure(solver.term_structure) != jtu.tree_structure(0):
+            raise NotImplementedError(
+                "`diffrax.BacksolveAdjoint` is only compatible with solvers that take "
+                "a single term."
+            )
 
         y = init_state.y
         init_state = eqx.tree_at(lambda s: s.y, init_state, object())
         init_state = _nondiff_solver_controller_state(
             self, init_state, passed_solver_state, passed_controller_state
         )
```

### Comparing `diffrax-0.3.1/diffrax/autocitation.py` & `diffrax-0.4.0/diffrax/autocitation.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/brownian/base.py` & `diffrax-0.4.0/diffrax/brownian/base.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/brownian/path.py` & `diffrax-0.4.0/diffrax/brownian/path.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/brownian/tree.py` & `diffrax-0.4.0/diffrax/brownian/tree.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/custom_types.py` & `diffrax-0.4.0/diffrax/custom_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import typing
-from typing import Dict, Generic, Tuple, TypeVar, Union
+from typing import Any, Dict, Generic, Tuple, TypeVar, Union
 
+import equinox.internal as eqxi
 import jax.tree_util as jtu
 
 
 # Custom flag we set when generating documentation.
 # We do a lot of custom hackery in here to produce nice-looking docs.
 if getattr(typing, "GENERATING_DOCUMENTATION", False):
 
@@ -125,7 +126,8 @@
     Scalar = Union[int, float, Array[()]]
 
     Int = Union[int, Array[(), int]]
     Bool = Union[bool, Array[(), bool]]
 
 DenseInfo = Dict[str, PyTree[Array]]
 DenseInfos = Dict[str, PyTree[Array["times", ...]]]  # noqa: F821
+sentinel: Any = eqxi.doc_repr(object(), "sentinel")
```

### Comparing `diffrax-0.3.1/diffrax/event.py` & `diffrax-0.4.0/diffrax/event.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/global_interpolation.py` & `diffrax-0.4.0/diffrax/global_interpolation.py`

 * *Files 3% similar despite different names*

```diff
@@ -314,48 +314,40 @@
     @eqx.filter_jit
     def evaluate(
         self, t0: Scalar, t1: Optional[Scalar] = None, left: bool = True
     ) -> PyTree:
         if t1 is not None:
             return self.evaluate(t1, left=left) - self.evaluate(t0, left=left)
         t = t0 * self.direction
-        ts_0 = self.ts[0]
-        ts_1 = self.ts[self.ts_size - 1]
-        pred = (self.ts_size > 1) & (t >= ts_0) & (t <= ts_1)
-        eval_fn = ft.partial(self.__class__._evaluate, t=t, left=left)
-        nan_fn = self.__class__._nan
-        # Use cond to avoid generating nans unless we have to.
-        out = lax.cond(pred, eval_fn, nan_fn, self)
+        t_bounded = self._nan_if_out_of_bounds(t)
+        out = self._get_local_interpolation(t_bounded, left).evaluate(
+            t_bounded, left=left
+        )
         keep = ft.partial(jnp.where, (t == self.t0_if_trivial) & (self.ts_size == 1))
         return jtu.tree_map(keep, self.y0_if_trivial, out)
 
     @eqx.filter_jit
     def derivative(self, t: Scalar, left: bool = True) -> PyTree:
         t = t * self.direction
+        t = self._nan_if_out_of_bounds(t)
+        out = self._get_local_interpolation(t, left).derivative(t, left=left)
+        return (self.direction * out**ω).ω
+
+    def _nan_if_out_of_bounds(self, t):
         # Note that len(self.ts) == max_steps + 1 > 0 so the indexing is always valid,
         # even if we throw it away because self.ts_size == 0.
         ts_0 = self.ts[0]
         ts_1 = self.ts[self.ts_size - 1]
-        pred = (self.ts_size > 1) & (t >= ts_0) & (t <= ts_1)
-        deriv_fn = ft.partial(self.__class__._derivative, t=t, left=left)
-        nan_fn = self.__class__._nan
-        # Use cond to avoid generating nans unless we have to.
-        return lax.cond(pred, deriv_fn, nan_fn, self)
-
-    def _evaluate(self, t, left):
-        return self._get_local_interpolation(t, left).evaluate(t, left=left)
-
-    def _derivative(self, t, left):
-        out = self._get_local_interpolation(t, left).derivative(t, left=left)
-        return (self.direction * out**ω).ω
-
-    def _nan(self):
-        return jtu.tree_map(
-            ft.partial(jnp.full_like, fill_value=jnp.nan), self.y0_if_trivial
-        )
+        out_of_bounds = (self.ts_size <= 1) | (t < ts_0) | (t > ts_1)
+        make_nans = lambda t: jnp.where(out_of_bounds, jnp.nan, t)
+        identity = lambda t: t
+        # Avoid making NaNs unless we have to, by using a cond.
+        # (For the sake of JAX_DEBUG_NANS.)
+        t = lax.cond(eqxi.unvmap_any(out_of_bounds), make_nans, identity, t)
+        return t
 
     @property
     def t0(self):
         # Note that len(self.ts) == max_steps + 1 > 0 so the indexing is always valid,
         # even if we throw it away because self.ts_size == 0.
         ts_0 = jnp.where(self.ts_size == 1, self.t0_if_trivial, self.ts[0])
         return ts_0 * self.direction
```

### Comparing `diffrax-0.3.1/diffrax/heuristics.py` & `diffrax-0.4.0/diffrax/heuristics.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/integrate.py` & `diffrax-0.4.0/diffrax/integrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 import functools as ft
 import typing
 import warnings
-from typing import Any, Callable, Optional
+from typing import Any, Callable, get_args, get_origin, Optional, Tuple
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 
 from .adjoint import AbstractAdjoint, DirectAdjoint, RecursiveCheckpointAdjoint
 from .custom_types import Array, Bool, Int, PyTree, Scalar
 from .event import AbstractDiscreteTerminatingEvent
 from .global_interpolation import DenseInterpolation
 from .heuristics import is_sde, is_unsafe_sde
 from .saveat import SaveAt, SubSaveAt
 from .solution import is_okay, is_successful, RESULTS, Solution
-from .solver import AbstractItoSolver, AbstractSolver, AbstractStratonovichSolver, Euler
+from .solver import (
+    AbstractItoSolver,
+    AbstractSolver,
+    AbstractStratonovichSolver,
+    Euler,
+    EulerHeun,
+    ItoMilstein,
+    StratonovichMilstein,
+)
 from .step_size_controller import (
     AbstractAdaptiveStepSizeController,
     AbstractStepSizeController,
     ConstantStepSize,
     PIDController,
     StepTo,
 )
-from .term import AbstractTerm, WrapTerm
+from .term import AbstractTerm, MultiTerm, ODETerm, WrapTerm
 
 
 class SaveState(eqx.Module):
     saveat_ts_index: Int
     ts: Array["times"]  # noqa: F821
     ys: PyTree[Array["times", ...]]  # noqa: F821
     save_index: Int
@@ -53,14 +61,36 @@
     dense_save_index: Int
 
 
 def _is_none(x):
     return x is None
 
 
+def _term_compatible(terms, term_structure):
+    def _check(term_cls, term):
+        if get_origin(term_cls) is MultiTerm:
+            if isinstance(term, MultiTerm):
+                [_tmp] = get_args(term_cls)
+                assert get_origin(_tmp) in (tuple, Tuple), "Malformed term_structure"
+                if not _term_compatible(term.terms, get_args(_tmp)):
+                    raise ValueError
+            else:
+                raise ValueError
+        else:
+            if not isinstance(term, term_cls):
+                raise ValueError
+
+    try:
+        jtu.tree_map(_check, term_structure, terms)
+    except ValueError:
+        # ValueError may also arise from mismatched tree structures
+        return False
+    return True
+
+
 def _is_subsaveat(x: Any) -> bool:
     return isinstance(x, SubSaveAt)
 
 
 def _inner_buffers(save_state):
     assert type(save_state) is SaveState
     return save_state.ts, save_state.ys
@@ -537,27 +567,33 @@
             f"t0 with value {t0} and type {type(t0)}, "
             f"dt0 with value {dt0} and type {type(dt0)}"
         )
         with jax.ensure_compile_time_eval():
             pred = (t1 - t0) * dt0 < 0
         dt0 = eqxi.error_if(dt0, pred, msg)
 
+    # Backward compatibility
+    if isinstance(
+        solver, (EulerHeun, ItoMilstein, StratonovichMilstein)
+    ) and _term_compatible(terms, (ODETerm, AbstractTerm)):
+        warnings.warn(
+            "Passing `terms=(ODETerm(...), SomeOtherTerm(...))` to "
+            f"{solver.__class__.__name__} is deprecated in favour of "
+            "`terms=MultiTerm(ODETerm(...), SomeOtherTerm(...))`. This means that "
+            "the same terms can now be passed used for both general and SDE-specific "
+            "solvers!"
+        )
+        terms = MultiTerm(*terms)
+
     # Error checking
-    term_leaves, term_structure = jtu.tree_flatten(
-        terms, is_leaf=lambda x: isinstance(x, AbstractTerm)
-    )
-    term_leaves2, term_structure2 = jtu.tree_flatten(solver.term_structure)
-    if term_structure != term_structure2 or any(
-        not isinstance(x, y) for x, y in zip(term_leaves, term_leaves2)
-    ):
+    if not _term_compatible(terms, solver.term_structure):
         raise ValueError(
             "`terms` must be a PyTree of `AbstractTerms` (such as `ODETerm`), with "
             f"structure {solver.term_structure}"
         )
-    del term_leaves, term_structure, term_leaves2, term_structure2
 
     if is_sde(terms):
         if not isinstance(solver, (AbstractItoSolver, AbstractStratonovichSolver)):
             warnings.warn(
                 f"`{type(solver).__name__}` is not marked as converging to either the "
                 "Itô or the Stratonovich solution."
             )
@@ -623,18 +659,24 @@
     t1 = t1 * direction
     if dt0 is not None:
         dt0 = dt0 * direction
     saveat = eqx.tree_at(
         _get_subsaveat_ts, saveat, replace_fn=lambda ts: ts * direction
     )
     stepsize_controller = stepsize_controller.wrap(direction)
+
+    def _wrap(term):
+        assert isinstance(term, AbstractTerm)
+        assert not isinstance(term, MultiTerm)
+        return WrapTerm(term, direction)
+
     terms = jtu.tree_map(
-        lambda t: WrapTerm(t, direction),
+        _wrap,
         terms,
-        is_leaf=lambda x: isinstance(x, AbstractTerm),
+        is_leaf=lambda x: isinstance(x, AbstractTerm) and not isinstance(x, MultiTerm),
     )
 
     # Stepsize controller gets an opportunity to modify the solver.
     # Note that at this point the solver could be anything so we must check any
     # abstract base classes of the solver before this.
     solver = stepsize_controller.wrap_solver(solver)
```

### Comparing `diffrax-0.3.1/diffrax/local_interpolation.py` & `diffrax-0.4.0/diffrax/local_interpolation.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,37 +37,37 @@
     coeffs: PyTree[Array[4, "dims":...]]  # noqa: F821
 
     def __init__(
         self,
         *,
         y0: PyTree[Array["dims":...]],  # noqa: F821
         y1: PyTree[Array["dims":...]],  # noqa: F821
-        f0: PyTree[Array["dims":...]],  # noqa: F821
-        f1: PyTree[Array["dims":...]],  # noqa: F821
+        k0: PyTree[Array["dims":...]],  # noqa: F821
+        k1: PyTree[Array["dims":...]],  # noqa: F821
         **kwargs
     ):
         super().__init__(**kwargs)
 
-        def _calculate(_y0, _y1, _f0, _f1):
-            _a = _f0 + _f1 + 2 * _y0 - 2 * _y1
-            _b = -2 * _f0 - _f1 - 3 * _y0 + 3 * _y1
-            return jnp.stack([_a, _b, _f0, _y0])
+        def _calculate(_y0, _y1, _k0, _k1):
+            _a = _k0 + _k1 + 2 * _y0 - 2 * _y1
+            _b = -2 * _k0 - _k1 - 3 * _y0 + 3 * _y1
+            return jnp.stack([_a, _b, _k0, _y0])
 
-        self.coeffs = jtu.tree_map(_calculate, y0, y1, f0, f1)
+        self.coeffs = jtu.tree_map(_calculate, y0, y1, k0, k1)
 
     @classmethod
     def from_k(
         cls,
         *,
         y0: PyTree[Array["dims":...]],  # noqa: F821
         y1: PyTree[Array["dims":...]],  # noqa: F821
         k: PyTree[Array["order", "dims":...]],  # noqa: F821
         **kwargs
     ):
-        return cls(y0=y0, y1=y1, f0=ω(k)[0].ω, f1=ω(k)[-1].ω, **kwargs)
+        return cls(y0=y0, y1=y1, k0=ω(k)[0].ω, k1=ω(k)[-1].ω, **kwargs)
 
     def evaluate(
         self, t0: Scalar, t1: Optional[Scalar] = None, left: bool = True
     ) -> PyTree:
         del left
         if t1 is not None:
             return self.evaluate(t1) - self.evaluate(t0)
```

### Comparing `diffrax-0.3.1/diffrax/misc.py` & `diffrax-0.4.0/diffrax/misc.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/nonlinear_solver/base.py` & `diffrax-0.4.0/diffrax/nonlinear_solver/base.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/nonlinear_solver/newton.py` & `diffrax-0.4.0/diffrax/nonlinear_solver/newton.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/path.py` & `diffrax-0.4.0/diffrax/path.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/saveat.py` & `diffrax-0.4.0/diffrax/saveat.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     using `t0`, `t1`, `ts` or `steps`. Defaults to `fn(t, y, args) -> y`, so that the
     evolving solution is saved. For example this can be useful to save only statistics
     of your solution, so as to reduce memory usage.
 
 - `subs`: Some PyTree of [`diffrax.SubSaveAt`][], which allows for finer-grained control
     over what is saved. Each `SubSaveAt` specifies a combination of a function `fn` and
     some times `t0`, `t1`, `ts`, `steps` at which to evaluate it. `sol.ts` and `sol.ys`
-    will then by PyTrees of the same structure as `subs`, with each leaf of the PyTree
+    will then be PyTrees of the same structure as `subs`, with each leaf of the PyTree
     saving what the corresponding `SubSaveAt` specifies. The arguments
     `SaveAt(t0=..., t1=..., ts=..., steps=..., fn=...)` are actually just a convenience
     for passing a single `SubSaveAt` as
     `SaveAt(subs=SubSaveAt(t0=..., t1=..., ts=..., steps=..., fn=...))`. This
     functionality can be useful when you need different functions of the output saved
     at different times; see the examples below.
```

### Comparing `diffrax-0.3.1/diffrax/solution.py` & `diffrax-0.4.0/diffrax/solution.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/solver/__init__.py` & `diffrax-0.4.0/diffrax/solver/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from .bosh3 import Bosh3
 from .dopri5 import Dopri5
 from .dopri8 import Dopri8
 from .euler import Euler
 from .euler_heun import EulerHeun
 from .heun import Heun
 from .implicit_euler import ImplicitEuler
+from .kencarp3 import KenCarp3
+from .kencarp4 import KenCarp4
+from .kencarp5 import KenCarp5
 from .kvaerno3 import Kvaerno3
 from .kvaerno4 import Kvaerno4
 from .kvaerno5 import Kvaerno5
 from .leapfrog_midpoint import LeapfrogMidpoint
 from .midpoint import Midpoint
 from .milstein import ItoMilstein, StratonovichMilstein
 from .ralston import Ralston
@@ -26,10 +29,12 @@
     AbstractDIRK,
     AbstractERK,
     AbstractESDIRK,
     AbstractRungeKutta,
     AbstractSDIRK,
     ButcherTableau,
     CalculateJacobian,
+    MultiButcherTableau,
 )
 from .semi_implicit_euler import SemiImplicitEuler
+from .sil3 import Sil3
 from .tsit5 import Tsit5
```

### Comparing `diffrax-0.3.1/diffrax/solver/base.py` & `diffrax-0.4.0/diffrax/solver/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import abc
 from typing import Callable, Optional, Tuple, Type, TypeVar
 
 import equinox as eqx
+import equinox.internal as eqxi
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
+from jaxtyping import PyTree
 
-from ..custom_types import Bool, DenseInfo, PyTree, Scalar
+from ..custom_types import Bool, DenseInfo, Scalar
 from ..heuristics import is_sde
 from ..local_interpolation import AbstractLocalInterpolation
 from ..nonlinear_solver import AbstractNonlinearSolver, NewtonNonlinearSolver
 from ..solution import RESULTS
 from ..term import AbstractTerm
 
 
@@ -37,24 +39,18 @@
 class AbstractSolver(eqx.Module, metaclass=_MetaAbstractSolver):
     """Abstract base class for all differential equation solvers.
 
     Subclasses should have a class-level attribute `terms`, specifying the PyTree
     structure of `terms` in `diffeqsolve(terms, ...)`.
     """
 
-    @property
-    @abc.abstractmethod
-    def term_structure(self) -> PyTree[Type[AbstractTerm]]:
-        """What PyTree structure `terms` should have when used with this solver."""
-
-    # On the type: frequently just Type[AbstractLocalInterpolation]
-    @property
-    @abc.abstractmethod
-    def interpolation_cls(self) -> Callable[..., AbstractLocalInterpolation]:
-        """How to interpolate the solution in between steps."""
+    # What PyTree structure `terms` should have when used with this solver.
+    term_structure: eqxi.AbstractClassVar[PyTree[Type[AbstractTerm]]]
+    # How to interpolate the solution in between steps.
+    interpolation_cls: eqxi.AbstractClassVar[Callable[..., AbstractLocalInterpolation]]
 
     def order(self, terms: PyTree[AbstractTerm]) -> Optional[int]:
         """Order of the solver for solving ODEs."""
         return None
 
     def strong_order(self, terms: PyTree[AbstractTerm]) -> Optional[Scalar]:
         """Strong order of the solver for solving SDEs."""
@@ -81,14 +77,15 @@
             order = self.strong_order(terms)
             if order is not None:
                 order = order + 0.5
             return order
         else:
             return self.order(terms)
 
+    @abc.abstractmethod
     def init(
         self,
         terms: PyTree[AbstractTerm],
         t0: Scalar,
         t1: Scalar,
         y0: PyTree,
         args: PyTree,
@@ -97,15 +94,14 @@
 
         **Arguments** as [`diffrax.diffeqsolve`][].
 
         **Returns:**
 
         The initial solver state, which should be used the first time `step` is called.
         """
-        return None
 
     @abc.abstractmethod
     def step(
         self,
         terms: PyTree[AbstractTerm],
         t0: Scalar,
         t1: Scalar,
```

### Comparing `diffrax-0.3.1/diffrax/solver/bosh3.py` & `diffrax-0.4.0/diffrax/solver/bosh3.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 )
 
 
 class Bosh3(AbstractERK):
     """Bogacki--Shampine's 3/2 method.
 
     3rd order explicit Runge--Kutta method. Has an embedded 2nd order method for
-    adaptive step sizing.
+    adaptive step sizing. Uses 4 stages with FSAL. Uses 3rd order Hermite
+    interpolation for dense/ts output.
 
     Also sometimes known as "Ralston's third order method".
     """
 
     tableau = _bosh3_tableau
     interpolation_cls = ThirdOrderHermitePolynomialInterpolation.from_k
```

### Comparing `diffrax-0.3.1/diffrax/solver/dopri5.py` & `diffrax-0.4.0/diffrax/solver/dopri5.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # https://www.sciencedirect.com/science/article/pii/0898122196001411
 # ("An Efficient Runge--Kutta (4, 5) pair", Bogacki and Shampine 1996)
 # Which they claim is slightly more efficient than the one we have here.
 class Dopri5(AbstractERK):
     r"""Dormand-Prince's 5/4 method.
 
     5th order Runge--Kutta method. Has an embedded 4th order method for adaptive step
-    sizing.
+    sizing. Uses 7 stages with FSAL. Uses 5th order interpolation for dense/ts output.
 
     ??? cite "Reference"
 
         The original reference for Dormand--Prince's 5(4) method is:
 
         ```bibtex
         @article{dormand1980family,
```

### Comparing `diffrax-0.3.1/diffrax/solver/dopri8.py` & `diffrax-0.4.0/diffrax/solver/dopri8.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         return (self.y0**ω + vector_tree_dot(coeffs, self.k) ** ω).ω
 
 
 class Dopri8(AbstractERK):
     """Dormand--Prince's 8/7 method.
 
     8th order Runge--Kutta method. Has an embedded 7th order method for adaptive step
-    sizing.
+    sizing. Uses 14 stages with FSAL. Uses 8th order interpolation for dense/ts output.
 
     ??? cite "References"
 
         Coefficients from:
         ```bibtex
         @article{prince1981high,
             author={Prince, P. J and Dormand, J. R.},
```

### Comparing `diffrax-0.3.1/diffrax/solver/euler.py` & `diffrax-0.4.0/diffrax/solver/euler.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,28 +12,39 @@
 _ErrorEstimate = None
 _SolverState = None
 
 
 class Euler(AbstractItoSolver):
     """Euler's method.
 
-    1st order explicit Runge--Kutta method. Does not support adaptive step sizing.
+    1st order explicit Runge--Kutta method. Does not support adaptive step sizing. Uses
+    1 stage. Uses 1st order local linear interpolation for dense/ts output.
 
     When used to solve SDEs, converges to the Itô solution.
     """
 
     term_structure = AbstractTerm
     interpolation_cls = LocalLinearInterpolation
 
     def order(self, terms):
         return 1
 
     def strong_order(self, terms):
         return 0.5
 
+    def init(
+        self,
+        terms: AbstractTerm,
+        t0: Scalar,
+        t1: Scalar,
+        y0: PyTree,
+        args: PyTree,
+    ) -> _SolverState:
+        return None
+
     def step(
         self,
         terms: AbstractTerm,
         t0: Scalar,
         t1: Scalar,
         y0: PyTree,
         args: PyTree,
```

### Comparing `diffrax-0.3.1/diffrax/solver/euler_heun.py` & `diffrax-0.4.0/diffrax/solver/euler_heun.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,65 @@
 from typing import Tuple
 
 from equinox.internal import ω
 
 from ..custom_types import Bool, DenseInfo, PyTree, Scalar
 from ..local_interpolation import LocalLinearInterpolation
 from ..solution import RESULTS
-from ..term import AbstractTerm, ODETerm
+from ..term import AbstractTerm, MultiTerm, ODETerm
 from .base import AbstractStratonovichSolver
 
 
 _ErrorEstimate = None
 _SolverState = None
 
 
 class EulerHeun(AbstractStratonovichSolver):
     """Euler-Heun method.
 
+    Uses a 1st order local linear interpolation scheme for dense/ts output.
+
+    This should be called with `terms=MultiTerm(drift_term, diffusion_term)`, where the
+    drift is an `ODETerm`.
+
     Used to solve SDEs, and converges to the Stratonovich solution.
     """
 
-    term_structure = (ODETerm, AbstractTerm)
+    term_structure = MultiTerm[Tuple[ODETerm, AbstractTerm]]
     interpolation_cls = LocalLinearInterpolation
 
     def order(self, terms):
         return 1
 
     def strong_order(self, terms):
         return 0.5
 
+    def init(
+        self,
+        terms: MultiTerm[Tuple[ODETerm, AbstractTerm]],
+        t0: Scalar,
+        t1: Scalar,
+        y0: PyTree,
+        args: PyTree,
+    ) -> _SolverState:
+        return None
+
     def step(
         self,
-        terms: Tuple[ODETerm, AbstractTerm],
+        terms: MultiTerm[Tuple[ODETerm, AbstractTerm]],
         t0: Scalar,
         t1: Scalar,
         y0: PyTree,
         args: PyTree,
         solver_state: _SolverState,
         made_jump: Bool,
     ) -> Tuple[PyTree, _ErrorEstimate, DenseInfo, _SolverState, RESULTS]:
         del solver_state, made_jump
 
-        drift, diffusion = terms
+        drift, diffusion = terms.terms
         dt = drift.contr(t0, t1)
         dW = diffusion.contr(t0, t1)
 
         f0 = drift.vf_prod(t0, y0, args, dt)
         g0 = diffusion.vf_prod(t0, y0, args, dW)
 
         y_prime = (y0**ω + g0**ω).ω
@@ -53,14 +68,14 @@
         y1 = (y0**ω + f0**ω + 0.5 * (g0**ω + g_prime**ω)).ω
 
         dense_info = dict(y0=y0, y1=y1)
         return y1, None, dense_info, None, RESULTS.successful
 
     def func(
         self,
-        terms: Tuple[AbstractTerm, AbstractTerm],
+        terms: MultiTerm[Tuple[AbstractTerm, AbstractTerm]],
         t0: Scalar,
         y0: PyTree,
         args: PyTree,
     ) -> PyTree:
-        drift, diffusion = terms
+        drift, diffusion = terms.terms
         return drift.vf(t0, y0, args), diffusion.vf(t0, y0, args)
```

### Comparing `diffrax-0.3.1/diffrax/solver/heun.py` & `diffrax-0.4.0/diffrax/solver/heun.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 )
 
 
 class Heun(AbstractERK, AbstractStratonovichSolver):
     """Heun's method.
 
     2nd order explicit Runge--Kutta method. Has an embedded Euler method for adaptive
-    step sizing.
+    step sizing. Uses 2 stages. Uses 2nd-order Hermite interpolation for dense/ts
+    output.
 
     Also sometimes known as either the "improved Euler method", "modified Euler method"
     or "explicit trapezoidal rule".
 
     Should not be confused with Heun's third order method, which is a different (higher
     order) method occasionally also just referred to as "Heun's method".
```

### Comparing `diffrax-0.3.1/diffrax/solver/implicit_euler.py` & `diffrax-0.4.0/diffrax/solver/semi_implicit_euler.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,64 +2,74 @@
 
 from equinox.internal import ω
 
 from ..custom_types import Bool, DenseInfo, PyTree, Scalar
 from ..local_interpolation import LocalLinearInterpolation
 from ..solution import RESULTS
 from ..term import AbstractTerm
-from .base import AbstractImplicitSolver
+from .base import AbstractSolver
 
 
 _ErrorEstimate = None
 _SolverState = None
 
 
-def _implicit_relation(z1, nonlinear_solve_args):
-    vf_prod, t1, y0, args, control = nonlinear_solve_args
-    diff = (vf_prod(t1, (y0**ω + z1**ω).ω, args, control) ** ω - z1**ω).ω
-    return diff
+class SemiImplicitEuler(AbstractSolver):
+    """Semi-implicit Euler's method.
 
-
-class ImplicitEuler(AbstractImplicitSolver):
-    r"""Implicit Euler method.
-
-    A-B-L stable 1st order SDIRK method. Does not support adaptive step sizing.
+    Symplectic method. Does not support adaptive step sizing. Uses 1st order local
+    linear interpolation for dense/ts output.
     """
 
-    term_structure = AbstractTerm
+    term_structure = (AbstractTerm, AbstractTerm)
     interpolation_cls = LocalLinearInterpolation
 
     def order(self, terms):
         return 1
 
-    def step(
+    def init(
         self,
-        terms: AbstractTerm,
+        terms: Tuple[AbstractTerm, AbstractTerm],
         t0: Scalar,
         t1: Scalar,
         y0: PyTree,
         args: PyTree,
+    ) -> _SolverState:
+        return None
+
+    def step(
+        self,
+        terms: Tuple[AbstractTerm, AbstractTerm],
+        t0: Scalar,
+        t1: Scalar,
+        y0: Tuple[PyTree, PyTree],
+        args: PyTree,
         solver_state: _SolverState,
         made_jump: Bool,
-    ) -> Tuple[PyTree, _ErrorEstimate, DenseInfo, _SolverState, RESULTS]:
+    ) -> Tuple[Tuple[PyTree, PyTree], _ErrorEstimate, DenseInfo, _SolverState, RESULTS]:
         del solver_state, made_jump
-        control = terms.contr(t0, t1)
-        pred = terms.vf_prod(t0, y0, args, control)
-        jac = self.nonlinear_solver.jac(
-            _implicit_relation, pred, (terms.vf_prod, t1, y0, args, control)
-        )
-        nonlinear_sol = self.nonlinear_solver(
-            _implicit_relation, pred, (terms.vf_prod, t1, y0, args, control), jac
-        )
-        z1 = nonlinear_sol.root
-        y1 = (y0**ω + z1**ω).ω
+
+        term_1, term_2 = terms
+        y0_1, y0_2 = y0
+
+        control1 = term_1.contr(t0, t1)
+        control2 = term_2.contr(t0, t1)
+        y1_1 = (y0_1**ω + term_1.vf_prod(t0, y0_2, args, control1) ** ω).ω
+        y1_2 = (y0_2**ω + term_2.vf_prod(t0, y1_1, args, control2) ** ω).ω
+
+        y1 = (y1_1, y1_2)
         dense_info = dict(y0=y0, y1=y1)
-        return y1, None, dense_info, None, nonlinear_sol.result
+        return y1, None, dense_info, None, RESULTS.successful
 
     def func(
         self,
-        terms: AbstractTerm,
+        terms: Tuple[AbstractTerm, AbstractTerm],
         t0: Scalar,
-        y0: PyTree,
+        y0: Tuple[PyTree, PyTree],
         args: PyTree,
-    ) -> PyTree:
-        return terms.vf(t0, y0, args)
+    ) -> Tuple[PyTree, PyTree]:
+
+        term_1, term_2 = terms
+        y0_1, y0_2 = y0
+        f1 = term_1.func(t0, y0_2, args)
+        f2 = term_2.func(t0, y0_1, args)
+        return (f1, f2)
```

### Comparing `diffrax-0.3.1/diffrax/solver/kvaerno3.py` & `diffrax-0.4.0/diffrax/solver/kvaerno3.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 )
 
 
 class Kvaerno3(AbstractESDIRK):
     r"""Kvaerno's 3/2 method.
 
     A-L stable stiffly accurate 3rd order ESDIRK method. Has an embedded 2nd order
-    method for adaptive step sizing. Uses 4 stages.
+    method for adaptive step sizing. Uses 4 stages with FSAL. Uses 3rd order Hermite
+    interpolation for dense/ts output.
 
     ??? cite "Reference"
 
         ```bibtex
         @article{kvaerno2004singly,
           title={Singly diagonally implicit Runge--Kutta methods with an explicit first
                  stage},
```

### Comparing `diffrax-0.3.1/diffrax/solver/kvaerno4.py` & `diffrax-0.4.0/diffrax/solver/kvaerno4.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,16 @@
 )
 
 
 class Kvaerno4(AbstractESDIRK):
     r"""Kvaerno's 4/3 method.
 
     A-L stable stiffly accurate 4th order ESDIRK method. Has an embedded 3rd order
-    method for adaptive step sizing. Uses 5 stages.
+    method for adaptive step sizing. Uses 5 stages with FSAL. Uses 3rd order Hermite
+    interpolation for dense/ts output.
 
     When solving an ODE over the interval $[t_0, t_1]$, note that this method will make
     some evaluations slightly past $t_1$.
 
     ??? cite "Reference"
 
         ```bibtex
```

### Comparing `diffrax-0.3.1/diffrax/solver/kvaerno5.py` & `diffrax-0.4.0/diffrax/solver/kvaerno5.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 )
 
 
 class Kvaerno5(AbstractESDIRK):
     r"""Kvaerno's 5/4 method.
 
     A-L stable stiffly accurate 5th order ESDIRK method. Has an embedded 4th order
-    method for adaptive step sizing. Uses 7 stages.
+    method for adaptive step sizing. Uses 7 stages with FSAL. Uses 3rd order Hermite
+    interpolation for dense/ts output.
 
     When solving an ODE over the interval $[t_0, t_1]$, note that this method will make
     some evaluations slightly past $t_1$.
 
     ??? cite "Reference"
 
         ```bibtex
```

### Comparing `diffrax-0.3.1/diffrax/solver/leapfrog_midpoint.py` & `diffrax-0.4.0/diffrax/solver/leapfrog_midpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 _SolverState = Tuple[Scalar, PyTree]
 
 
 # TODO: support arbitrary linear multistep methods
 class LeapfrogMidpoint(AbstractSolver):
     r"""Leapfrog/midpoint method.
 
-    2nd order linear multistep method.
+    2nd order linear multistep method. Uses 1st order local linear interpolation for
+    dense/ts output.
 
     Note that this is referred to as the "leapfrog/midpoint method" as this is the name
     used by Shampine in the reference below. It should not be confused with any of the
     many other "leapfrog methods" (there are several), or with the "midpoint method"
     (which is usually taken to refer to the explicit Runge--Kutta method
     [`diffrax.Midpoint`][]).
```

### Comparing `diffrax-0.3.1/diffrax/solver/midpoint.py` & `diffrax-0.4.0/diffrax/solver/midpoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 )
 
 
 class Midpoint(AbstractERK, AbstractStratonovichSolver):
     """Midpoint method.
 
     2nd order explicit Runge--Kutta method. Has an embedded Euler method for adaptive
-    step sizing.
+    step sizing. Uses 2 stages. Uses 2nd order Hermite interpolation for dense/ts
+    output.
 
     Also sometimes known as the "modified Euler method".
 
     When used to solve SDEs, converges to the Stratonovich solution.
     """
 
     tableau = _midpoint_tableau
```

### Comparing `diffrax-0.3.1/diffrax/solver/milstein.py` & `diffrax-0.4.0/diffrax/solver/milstein.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from equinox.internal import ω
 
 from ..custom_types import Bool, DenseInfo, PyTree, Scalar
 from ..local_interpolation import LocalLinearInterpolation
 from ..solution import RESULTS
-from ..term import AbstractTerm, ODETerm
+from ..term import AbstractTerm, MultiTerm, ODETerm
 from .base import AbstractItoSolver, AbstractStratonovichSolver
 
 
 _ErrorEstimate = None
 _SolverState = None
 
 
@@ -24,43 +24,57 @@
 # correction term.)
 #
 
 
 class StratonovichMilstein(AbstractStratonovichSolver):
     r"""Milstein's method; Stratonovich version.
 
-    Used to solve SDEs, and converges to the Stratonovich solution.
+    Used to solve SDEs, and converges to the Stratonovich solution. Uses local linear
+    interpolation for dense/ts output.
+
+    This should be called with `terms=MultiTerm(drift_term, diffusion_term)`, where the
+    drift is an `ODETerm`.
 
     !!! warning
 
         Requires [commutative noise](https://docs.kidger.site/diffrax/usage/how-to-choose-a-solver/#stochastic-differential-equations).
         Note that this commutativity condition is not checked.
     """  # noqa: E501
 
-    term_structure = (ODETerm, AbstractTerm)
+    term_structure = MultiTerm[Tuple[ODETerm, AbstractTerm]]
     interpolation_cls = LocalLinearInterpolation
 
     def order(self, terms):
         raise ValueError("`StratonovichMilstein` should not used to solve ODEs.")
 
     def strong_order(self, terms):
         return 1  # assuming commutative noise
 
+    def init(
+        self,
+        terms: MultiTerm[Tuple[ODETerm, AbstractTerm]],
+        t0: Scalar,
+        t1: Scalar,
+        y0: PyTree,
+        args: PyTree,
+    ) -> _SolverState:
+        return None
+
     def step(
         self,
-        terms: Tuple[AbstractTerm, AbstractTerm],
+        terms: MultiTerm[Tuple[ODETerm, AbstractTerm]],
         t0: Scalar,
         t1: Scalar,
         y0: PyTree,
         args: PyTree,
         solver_state: _SolverState,
         made_jump: Bool,
     ) -> Tuple[PyTree, _ErrorEstimate, DenseInfo, _SolverState, RESULTS]:
         del solver_state, made_jump
-        drift, diffusion = terms
+        drift, diffusion = terms.terms
         dt = drift.contr(t0, t1)
         dw = diffusion.contr(t0, t1)
 
         f0_prod = drift.vf_prod(t0, y0, args, dt)
         g0_prod = diffusion.vf_prod(t0, y0, args, dw)
 
         def _to_jvp(_y0):
@@ -70,55 +84,69 @@
         y1 = (y0**ω + f0_prod**ω + g0_prod**ω + 0.5 * v0_prod**ω).ω
 
         dense_info = dict(y0=y0, y1=y1)
         return y1, None, dense_info, None, RESULTS.successful
 
     def func(
         self,
-        terms: Tuple[AbstractTerm, AbstractTerm],
+        terms: MultiTerm[Tuple[AbstractTerm, AbstractTerm]],
         t0: Scalar,
         y0: PyTree,
         args: PyTree,
     ) -> PyTree:
-        drift, diffusion = terms
+        drift, diffusion = terms.terms
         return drift.vf(t0, y0, args), diffusion.vf(t0, y0, args)
 
 
 class ItoMilstein(AbstractItoSolver):
     r"""Milstein's method; Itô version.
 
-    Used to solve SDEs, and converges to the Itô solution.
+    Used to solve SDEs, and converges to the Itô solution. Uses local linear
+    interpolation for dense/ts output.
+
+    This should be called with `terms=MultiTerm(drift_term, diffusion_term)`, where the
+    drift is an `ODETerm`.
 
     !!! warning
 
         Requires [commutative noise](https://docs.kidger.site/diffrax/usage/how-to-choose-a-solver/#stochastic-differential-equations).
         Note that this commutativity condition is not checked.
     """  # noqa: E501
 
-    term_structure = (ODETerm, AbstractTerm)
+    term_structure = MultiTerm[Tuple[ODETerm, AbstractTerm]]
     interpolation_cls = LocalLinearInterpolation
 
     def order(self, terms):
         raise ValueError("`StratonovichMilstein` should not used to solve ODEs.")
 
     def strong_order(self, terms):
         return 1  # assuming commutative noise
 
+    def init(
+        self,
+        terms: MultiTerm[Tuple[ODETerm, AbstractTerm]],
+        t0: Scalar,
+        t1: Scalar,
+        y0: PyTree,
+        args: PyTree,
+    ) -> _SolverState:
+        return None
+
     def step(
         self,
-        terms: Tuple[AbstractTerm, AbstractTerm],
+        terms: MultiTerm[Tuple[ODETerm, AbstractTerm]],
         t0: Scalar,
         t1: Scalar,
         y0: PyTree,
         args: PyTree,
         solver_state: _SolverState,
         made_jump: Bool,
     ) -> Tuple[PyTree, _ErrorEstimate, DenseInfo, _SolverState, RESULTS]:
         del solver_state, made_jump
-        drift, diffusion = terms
+        drift, diffusion = terms.terms
         Δt = drift.contr(t0, t1)
         Δw = diffusion.contr(t0, t1)
 
         #
         # So this is a bit involved, largely because of the generality that the rest of
         # the library supports. (In particular arbitrary PyTrees, and arbitrary (linear)
         # `AbstractTerm.prod`)
@@ -322,14 +350,14 @@
         #
 
         dense_info = dict(y0=y0, y1=y1)
         return y1, None, dense_info, None, RESULTS.successful
 
     def func(
         self,
-        terms: Tuple[AbstractTerm, AbstractTerm],
+        terms: MultiTerm[Tuple[AbstractTerm, AbstractTerm]],
         t0: Scalar,
         y0: PyTree,
         args: PyTree,
     ) -> PyTree:
         drift, diffusion = terms
         return drift.vf(t0, y0, args), diffusion.vf(t0, y0, args)
```

### Comparing `diffrax-0.3.1/diffrax/solver/ralston.py` & `diffrax-0.4.0/diffrax/solver/ralston.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 )
 
 
 class Ralston(AbstractERK, AbstractStratonovichSolver):
     """Ralston's method.
 
     2nd order explicit Runge--Kutta method. Has an embedded Euler method for adaptive
-    step sizing.
+    step sizing. Uses 2 stages. Uses 2nd order Hermite interpolation for dense output.
 
     When used to solve SDEs, converges to the Stratonovich solution.
     """
 
     tableau = _ralston_tableau
     interpolation_cls = ThirdOrderHermitePolynomialInterpolation.from_k
```

### Comparing `diffrax-0.3.1/diffrax/solver/reversible_heun.py` & `diffrax-0.4.0/diffrax/solver/reversible_heun.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _SolverState = Tuple[PyTree, PyTree]
 
 
 class ReversibleHeun(AbstractAdaptiveSolver, AbstractStratonovichSolver):
     """Reversible Heun method.
 
     Algebraically reversible 2nd order method. Has an embedded 1st order method for
-    adaptive step sizing.
+    adaptive step sizing. Uses 1st order local linear interpolation for dense/ts output.
 
     When used to solve SDEs, converges to the Stratonovich solution.
 
     ??? cite "Reference"
 
         ```bibtex
         @article{kidger2021efficient,
```

### Comparing `diffrax-0.3.1/diffrax/solver/tsit5.py` & `diffrax-0.4.0/diffrax/solver/tsit5.py`

 * *Files 11% similar despite different names*

```diff
@@ -94,17 +94,22 @@
         ]
     ),
 )
 
 
 class _Tsit5Interpolation(AbstractLocalInterpolation):
     y0: PyTree[Array[...]]
-    y1: PyTree[Array[...]]  # Unused, just here for API compatibility
     k: PyTree[Array["order":7, ...]]  # noqa: F821
 
+    def __init__(self, *, y0, y1, k, **kwargs):
+        del y1  # exists for API compatibility
+        super().__init__(**kwargs)
+        self.y0 = y0
+        self.k = k
+
     def evaluate(
         self, t0: Scalar, t1: Optional[Scalar] = None, left: bool = True
     ) -> PyTree:  # noqa: F821
         del left
         if t1 is not None:
             return self.evaluate(t1) - self.evaluate(t0)
 
@@ -143,15 +148,16 @@
         ).ω
 
 
 class Tsit5(AbstractERK):
     r"""Tsitouras' 5/4 method.
 
     5th order explicit Runge--Kutta method. Has an embedded 4th order method for
-    adaptive step sizing.
+    adaptive step sizing. Uses 7 stages with FSAL. Uses 5th order interpolation
+    for dense/ts output.
 
     ??? cite "Reference"
 
         ```bibtex
         @article{tsitouras2011runge,
           title={Runge--Kutta pairs of order 5 (4) satisfying only the first column
                  simplifying assumption},
```

### Comparing `diffrax-0.3.1/diffrax/step_size_controller/adaptive.py` & `diffrax-0.4.0/diffrax/step_size_controller/adaptive.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,41 +17,50 @@
 
 
 def _select_initial_step(
     terms: PyTree[AbstractTerm],
     t0: Scalar,
     y0: PyTree,
     args: PyTree,
-    func: Callable[[Scalar, PyTree, PyTree], PyTree],
+    func: Callable[[PyTree[AbstractTerm], Scalar, PyTree, PyTree], PyTree],
     error_order: Scalar,
     rtol: Scalar,
     atol: Scalar,
     norm: Callable[[PyTree], Scalar],
 ) -> Scalar:
-    f0 = func(terms, t0, y0, args)
-    scale = (atol + ω(y0).call(jnp.abs) * rtol).ω
-    d0 = norm((y0**ω / scale**ω).ω)
-    d1 = norm((f0**ω / scale**ω).ω)
+    def fn(carry):
+        t, y, _h0, _d1, _f, _ = carry
+        f = func(terms, t, y, args)
+        return t, y, _h0, _d1, _f, f
+
+    def intermediate(carry):
+        _, _, _, _, _, f0 = carry
+        d0 = norm((y0**ω / scale**ω).ω)
+        d1 = norm((f0**ω / scale**ω).ω)
+        _cond = (d0 < 1e-5) | (d1 < 1e-5)
+        _d1 = jnp.where(_cond, 1, d1)
+        h0 = jnp.where(_cond, 1e-6, 0.01 * (d0 / _d1))
+        t1 = t0 + h0
+        y1 = (y0**ω + h0 * f0**ω).ω
+        return t1, y1, h0, d1, f0, f0
 
-    _cond = (d0 < 1e-5) | (d1 < 1e-5)
-    _d1 = jnp.where(_cond, 1, d1)
-    h0 = jnp.where(_cond, 1e-6, 0.01 * (d0 / _d1))
-
-    t1 = t0 + h0
-    y1 = (y0**ω + h0 * f0**ω).ω
-    f1 = func(terms, t1, y1, args)
+    scale = (atol + ω(y0).call(jnp.abs) * rtol).ω
+    dummy_h = t0
+    dummy_d = eqxi.eval_empty(norm, y0)
+    dummy_f = eqxi.eval_empty(lambda: func(terms, t0, y0, args))
+    _, _, h0, d1, f0, f1 = eqxi.scan_trick(
+        fn, [intermediate], (t0, y0, dummy_h, dummy_d, dummy_f, dummy_f)
+    )
     d2 = norm(((f1**ω - f0**ω) / scale**ω).ω) / h0
-
     max_d = jnp.maximum(d1, d2)
     h1 = jnp.where(
         max_d <= 1e-15,
         jnp.maximum(1e-6, h0 * 1e-3),
         (0.01 / max_d) ** (1 / error_order),
     )
-
     return jnp.minimum(100 * h0, h1)
 
 
 _ControllerState = Tuple[Bool, Bool, Scalar, Scalar, Scalar]
 
 
 _gendocs = getattr(typing, "GENERATING_DOCUMENTATION", False)
```

### Comparing `diffrax-0.3.1/diffrax/step_size_controller/base.py` & `diffrax-0.4.0/diffrax/step_size_controller/base.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/step_size_controller/constant.py` & `diffrax-0.4.0/diffrax/step_size_controller/constant.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/diffrax/term.py` & `diffrax-0.4.0/diffrax/term.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 import operator
-from typing import Callable, Tuple
+from typing import Callable, Generic, Tuple, TypeVar
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 from equinox.internal import ω
@@ -309,15 +309,18 @@
         return self.control_term.vf_prod(t, y, args, control)
 
 
 def _sum(*x):
     return sum(x[1:], x[0])
 
 
-class MultiTerm(AbstractTerm):
+_Terms = TypeVar("_Terms", bound=Tuple[AbstractTerm, ...])
+
+
+class MultiTerm(AbstractTerm, Generic[_Terms]):
     r"""Accumulates multiple terms into a single term.
 
     Consider the SDE
 
     $\mathrm{d}y(t) = f(t, y(t))\mathrm{d}t + g(t, y(t))\mathrm{d}w(t)$
 
     This has two terms on the right hand side. It may be represented with a single
@@ -328,17 +331,17 @@
     whose vector field -- control interaction is a dot product.
 
     `MultiTerm` performs this transform. For simplicitly most differential equation
     solvers (at least those built-in to Diffrax) accept just a single term, so this
     transform is a necessary part of e.g. solving an SDE with both drift and diffusion.
     """
 
-    terms: Tuple[AbstractTerm, ...]
+    terms: _Terms
 
-    def __init__(self, *terms):
+    def __init__(self, *terms: AbstractTerm):
         """**Arguments:**
 
         - `*terms`: Any number of [`diffrax.AbstractTerm`][]s to combine.
         """
         self.terms = terms
 
     def vf(self, t: Scalar, y: PyTree, args: PyTree) -> Tuple[PyTree, ...]:
@@ -350,14 +353,32 @@
     def prod(self, vf: Tuple[PyTree, ...], control: Tuple[PyTree, ...]) -> PyTree:
         out = [
             term.prod(vf_, control_)
             for term, vf_, control_ in zip(self.terms, vf, control)
         ]
         return jtu.tree_map(_sum, *out)
 
+    def vf_prod(
+        self, t: Scalar, y: PyTree, args: PyTree, control: Tuple[PyTree, ...]
+    ) -> PyTree:
+        out = [
+            term.vf_prod(t, y, args, control_)
+            for term, control_ in zip(self.terms, control)
+        ]
+        return jtu.tree_map(_sum, *out)
+
+    def is_vf_expensive(
+        self,
+        t0: Scalar,
+        t1: Scalar,
+        y: Tuple[PyTree, PyTree, PyTree, PyTree],
+        args: PyTree,
+    ) -> bool:
+        return any(term.is_vf_expensive(t0, t1, y, args) for term in self.terms)
+
 
 class WrapTerm(AbstractTerm):
     term: AbstractTerm
     direction: Scalar
 
     def vf(self, t: Scalar, y: PyTree, args: PyTree) -> PyTree:
         t = t * self.direction
@@ -367,14 +388,27 @@
         _t0 = jnp.where(self.direction == 1, t0, -t1)
         _t1 = jnp.where(self.direction == 1, t1, -t0)
         return (self.direction * self.term.contr(_t0, _t1) ** ω).ω
 
     def prod(self, vf: PyTree, control: PyTree) -> PyTree:
         return self.term.prod(vf, control)
 
+    def vf_prod(self, t: Scalar, y: PyTree, args: PyTree, control: PyTree) -> PyTree:
+        t = t * self.direction
+        return self.term.vf_prod(t, y, args, control)
+
+    def is_vf_expensive(
+        self,
+        t0: Scalar,
+        t1: Scalar,
+        y: Tuple[PyTree, PyTree, PyTree, PyTree],
+        args: PyTree,
+    ) -> bool:
+        return self.term.is_vf_expensive(t0, t1, y, args)
+
 
 class AdjointTerm(AbstractTerm):
     term: AbstractTerm
 
     def is_vf_expensive(
         self,
         t0: Scalar,
```

### Comparing `diffrax-0.3.1/diffrax.egg-info/PKG-INFO` & `diffrax-0.4.0/diffrax.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,95 @@
 Metadata-Version: 2.1
 Name: diffrax
-Version: 0.3.1
+Version: 0.4.0
 Summary: GPU+autodiff-capable ODE/SDE/CDE solvers written in JAX.
 Home-page: https://github.com/patrick-kidger/diffrax
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
-Description: <h1 align='center'>Diffrax</h1>
-        <h2 align='center'>Numerical differential equation solvers in JAX. Autodifferentiable and GPU-capable.</h2>
-        
-        Diffrax is a [JAX](https://github.com/google/jax)-based library providing numerical differential equation solvers.
-        
-        Features include:
-        
-        - ODE/SDE/CDE (ordinary/stochastic/controlled) solvers;
-        - lots of different solvers (including `Tsit5`, `Dopri8`, symplectic solvers, implicit solvers);
-        - vmappable _everything_ (including the region of integration);
-        - using a PyTree as the state;
-        - dense solutions;
-        - multiple adjoint methods for backpropagation;
-        - support for neural differential equations.
-        
-        _From a technical point of view, the internal structure of the library is pretty cool -- all kinds of equations (ODEs, SDEs, CDEs) are solved in a unified way (rather than being treated separately), producing a small tightly-written library._
-        
-        ## Installation
-        
-        ```
-        pip install diffrax
-        ```
-        
-        Requires Python 3.8+, JAX 0.4.3+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.0+.
-        
-        ## Documentation
-        
-        Available at [https://docs.kidger.site/diffrax](https://docs.kidger.site/diffrax).
-        
-        ## Quick example
-        
-        ```python
-        from diffrax import diffeqsolve, ODETerm, Dopri5
-        import jax.numpy as jnp
-        
-        def f(t, y, args):
-            return -y
-        
-        term = ODETerm(f)
-        solver = Dopri5()
-        y0 = jnp.array([2., 3.])
-        solution = diffeqsolve(term, solver, t0=0, t1=1, dt0=0.1, y0=y0)
-        ```
-        
-        Here, `Dopri5` refers to the Dormand--Prince 5(4) numerical differential equation solver, which is a standard choice for many problems.
-        
-        ## Citation
-        
-        If you found this library useful in academic research, please cite: [(arXiv link)](https://arxiv.org/abs/2202.02435)
-        
-        ```bibtex
-        @phdthesis{kidger2021on,
-            title={{O}n {N}eural {D}ifferential {E}quations},
-            author={Patrick Kidger},
-            year={2021},
-            school={University of Oxford},
-        }
-        ```
-        
-        (Also consider starring the project on GitHub.)
-        
-        ## See also
-        
-        Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
-        
-        Type annotations and runtime checking for PyTrees and shape/dtype of JAX arrays: [jaxtyping](https://github.com/google/jaxtyping).
-        
-        Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
-        
-        SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: ~=3.8
+Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align='center'>Diffrax</h1>
+<h2 align='center'>Numerical differential equation solvers in JAX. Autodifferentiable and GPU-capable.</h2>
+
+Diffrax is a [JAX](https://github.com/google/jax)-based library providing numerical differential equation solvers.
+
+Features include:
+
+- ODE/SDE/CDE (ordinary/stochastic/controlled) solvers;
+- lots of different solvers (including `Tsit5`, `Dopri8`, symplectic solvers, implicit solvers);
+- vmappable _everything_ (including the region of integration);
+- using a PyTree as the state;
+- dense solutions;
+- multiple adjoint methods for backpropagation;
+- support for neural differential equations.
+
+_From a technical point of view, the internal structure of the library is pretty cool -- all kinds of equations (ODEs, SDEs, CDEs) are solved in a unified way (rather than being treated separately), producing a small tightly-written library._
+
+## Installation
+
+```
+pip install diffrax
+```
+
+Requires Python 3.9+, JAX 0.4.4+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.4+.
+
+## Documentation
+
+Available at [https://docs.kidger.site/diffrax](https://docs.kidger.site/diffrax).
+
+## Quick example
+
+```python
+from diffrax import diffeqsolve, ODETerm, Dopri5
+import jax.numpy as jnp
+
+def f(t, y, args):
+    return -y
+
+term = ODETerm(f)
+solver = Dopri5()
+y0 = jnp.array([2., 3.])
+solution = diffeqsolve(term, solver, t0=0, t1=1, dt0=0.1, y0=y0)
+```
+
+Here, `Dopri5` refers to the Dormand--Prince 5(4) numerical differential equation solver, which is a standard choice for many problems.
+
+## Citation
+
+If you found this library useful in academic research, please cite: [(arXiv link)](https://arxiv.org/abs/2202.02435)
+
+```bibtex
+@phdthesis{kidger2021on,
+    title={{O}n {N}eural {D}ifferential {E}quations},
+    author={Patrick Kidger},
+    year={2021},
+    school={University of Oxford},
+}
+```
+
+(Also consider starring the project on GitHub.)
+
+## See also
+
+Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
+
+Type annotations and runtime checking for PyTrees and shape/dtype of JAX arrays: [jaxtyping](https://github.com/google/jaxtyping).
+
+Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
+
+SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
```

### Comparing `diffrax-0.3.1/diffrax.egg-info/SOURCES.txt` & `diffrax-0.4.0/diffrax.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,35 +24,40 @@
 diffrax.egg-info/requires.txt
 diffrax.egg-info/top_level.txt
 diffrax/brownian/__init__.py
 diffrax/brownian/base.py
 diffrax/brownian/path.py
 diffrax/brownian/tree.py
 diffrax/nonlinear_solver/__init__.py
+diffrax/nonlinear_solver/affine.py
 diffrax/nonlinear_solver/base.py
 diffrax/nonlinear_solver/newton.py
 diffrax/solver/__init__.py
 diffrax/solver/base.py
 diffrax/solver/bosh3.py
 diffrax/solver/dopri5.py
 diffrax/solver/dopri8.py
 diffrax/solver/euler.py
 diffrax/solver/euler_heun.py
 diffrax/solver/heun.py
 diffrax/solver/implicit_euler.py
+diffrax/solver/kencarp3.py
+diffrax/solver/kencarp4.py
+diffrax/solver/kencarp5.py
 diffrax/solver/kvaerno3.py
 diffrax/solver/kvaerno4.py
 diffrax/solver/kvaerno5.py
 diffrax/solver/leapfrog_midpoint.py
 diffrax/solver/midpoint.py
 diffrax/solver/milstein.py
 diffrax/solver/ralston.py
 diffrax/solver/reversible_heun.py
 diffrax/solver/runge_kutta.py
 diffrax/solver/semi_implicit_euler.py
+diffrax/solver/sil3.py
 diffrax/solver/tsit5.py
 diffrax/step_size_controller/__init__.py
 diffrax/step_size_controller/adaptive.py
 diffrax/step_size_controller/base.py
 diffrax/step_size_controller/constant.py
 test/__init__.py
 test/conftest.py
```

### Comparing `diffrax-0.3.1/setup.py` & `diffrax-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 
-python_requires = "~=3.8"
+python_requires = "~=3.9"
 
-install_requires = ["jax>=0.4.3", "equinox>=0.10.0"]
+install_requires = ["jax>=0.4.3", "equinox>=0.10.4"]
 
 setuptools.setup(
     name=name,
     version=version,
     author=author,
     author_email=author_email,
     maintainer=author,
```

### Comparing `diffrax-0.3.1/test/conftest.py` & `diffrax-0.4.0/test/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,11 +35,12 @@
             if module_name.startswith("jax"):
                 if module_name not in ["jax.interpreters.partial_eval"]:
                     for obj_name in dir(module):
                         obj = getattr(module, obj_name)
                         if hasattr(obj, "cache_clear"):
                             try:
                                 print(f"Clearing {obj}")
-                                obj.cache_clear()
+                                if "Weakref" not in type(obj).__name__:
+                                    obj.cache_clear()
                             except Exception:
                                 pass
         gc.collect()
```

### Comparing `diffrax-0.3.1/test/test_adaptive_stepsize_controller.py` & `diffrax-0.4.0/test/test_adaptive_stepsize_controller.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/test/test_adjoint.py` & `diffrax-0.4.0/test/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/test/test_brownian.py` & `diffrax-0.4.0/test/test_brownian.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/test/test_detest.py` & `diffrax-0.4.0/test/test_detest.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/test/test_event.py` & `diffrax-0.4.0/test/test_event.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/test/test_global_interpolation.py` & `diffrax-0.4.0/test/test_global_interpolation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import functools as ft
 import operator
+from typing import Tuple
 
 import diffrax
 import jax
 import jax.numpy as jnp
 import jax.random as jrandom
 import jax.tree_util as jtu
 import pytest
 
-from .helpers import all_ode_solvers, implicit_tol, shaped_allclose
+from .helpers import all_ode_solvers, all_split_solvers, implicit_tol, shaped_allclose
 
 
 @pytest.mark.parametrize("mode", ["linear", "linear2", "cubic"])
 @pytest.mark.parametrize("unsqueeze", [True, False])
 def test_interpolation_coeffs(mode, unsqueeze):
     # Data is linear so both linear and cubic interpolation should produce the same
     # results where there is missing data.
@@ -311,16 +312,26 @@
 
                     jtu.tree_map(_test, firstderiv, derivs, y0, y1)
 
 
 def _test_dense_interpolation(solver, key, t1):
     y0 = jrandom.uniform(key, (), minval=0.4, maxval=2)
     dt0 = t1 / 1e3
+    if (
+        solver.term_structure
+        == diffrax.MultiTerm[Tuple[diffrax.AbstractTerm, diffrax.AbstractTerm]]
+    ):
+        term = diffrax.MultiTerm(
+            diffrax.ODETerm(lambda t, y, args: -0.7 * y),
+            diffrax.ODETerm(lambda t, y, args: -0.3 * y),
+        )
+    else:
+        term = diffrax.ODETerm(lambda t, y, args: -y)
     sol = diffrax.diffeqsolve(
-        diffrax.ODETerm(lambda t, y, args: -y),
+        term,
         solver=solver,
         t0=0,
         t1=t1,
         dt0=dt0,
         y0=y0,
         saveat=diffrax.SaveAt(dense=True),
     )
@@ -330,15 +341,15 @@
 
     derivs = jax.vmap(sol.derivative)(points)
     true_derivs = -true_vals
 
     return vals, true_vals, derivs, true_derivs
 
 
-@pytest.mark.parametrize("solver", all_ode_solvers)
+@pytest.mark.parametrize("solver", all_ode_solvers + all_split_solvers)
 def test_dense_interpolation(solver, getkey):
     solver = implicit_tol(solver)
     key = jrandom.PRNGKey(5678)
     vals, true_vals, derivs, true_derivs = _test_dense_interpolation(solver, key, 1)
     assert jnp.array_equal(vals[0], true_vals[0])
     val_tol = {
         diffrax.Euler: 1e-3,
@@ -356,15 +367,15 @@
     }.get(type(solver), 1e-6)
     assert shaped_allclose(derivs, true_derivs, atol=deriv_tol, rtol=deriv_tol)
 
 
 # When vmap'ing then it can happen that some batch elements take more steps to solve
 # than others. This means some padding is used to make things line up; here we test
 # that all of this works as intended.
-@pytest.mark.parametrize("solver", all_ode_solvers)
+@pytest.mark.parametrize("solver", all_ode_solvers + all_split_solvers)
 def test_dense_interpolation_vmap(solver, getkey):
     solver = implicit_tol(solver)
     key = jrandom.PRNGKey(5678)
     _test_dense = ft.partial(_test_dense_interpolation, solver, key)
     _test_dense_vmap = jax.vmap(_test_dense)
     vals, true_vals, derivs, true_derivs = _test_dense_vmap(jnp.array([0.5, 1.0]))
     assert jnp.array_equal(vals[:, 0], true_vals[:, 0])
```

### Comparing `diffrax-0.3.1/test/test_integrate.py` & `diffrax-0.4.0/test/test_integrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import math
 import operator
+from typing import Tuple
 
 import diffrax
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.random as jrandom
 import jax.tree_util as jtu
 import pytest
 import scipy.stats
 from equinox.internal import ω
 
 from .helpers import (
     all_ode_solvers,
+    all_split_solvers,
     implicit_tol,
     random_pytree,
     shaped_allclose,
     treedefs,
 )
 
 
@@ -111,26 +113,40 @@
         else:
             raise
     y1 = sol.ys
     true_y1 = jtu.tree_map(lambda x: (x * math.exp(-1))[None], y0)
     assert shaped_allclose(y1, true_y1, atol=1e-2, rtol=1e-2)
 
 
-@pytest.mark.parametrize("solver", all_ode_solvers)
+@pytest.mark.parametrize("solver", all_ode_solvers + all_split_solvers)
 def test_ode_order(solver):
     solver = implicit_tol(solver)
     key = jrandom.PRNGKey(5678)
     akey, ykey = jrandom.split(key, 2)
 
     A = jrandom.normal(akey, (10, 10), dtype=jnp.float64) * 0.5
 
-    def f(t, y, args):
-        return A @ y
+    if (
+        solver.term_structure
+        == diffrax.MultiTerm[Tuple[diffrax.AbstractTerm, diffrax.AbstractTerm]]
+    ):
+
+        def f1(t, y, args):
+            return 0.3 * A @ y
+
+        def f2(t, y, args):
+            return 0.7 * A @ y
+
+        term = diffrax.MultiTerm(diffrax.ODETerm(f1), diffrax.ODETerm(f2))
+    else:
+
+        def f(t, y, args):
+            return A @ y
 
-    term = diffrax.ODETerm(f)
+        term = diffrax.ODETerm(f)
     t0 = 0
     t1 = 4
     y0 = jrandom.normal(ykey, (10,), dtype=jnp.float64)
 
     true_yT = jax.scipy.linalg.expm((t1 - t0) * A) @ y0
     exponents = []
     errors = []
```

### Comparing `diffrax-0.3.1/test/test_interpolation.py` & `diffrax-0.4.0/test/test_interpolation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import diffrax
 import jax
 import jax.numpy as jnp
 import jax.random as jrandom
 
-from .helpers import all_ode_solvers, implicit_tol, shaped_allclose
+from .helpers import all_ode_solvers, all_split_solvers, implicit_tol, shaped_allclose
 
 
 def _test_path_derivative(path, name):
     for percentage in (0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0):
         t = path.t0 + percentage * (path.t1 - path.t0)
         _, x = jax.jvp(path.evaluate, (t,), (jnp.ones_like(t),))
         y = path.derivative(t)
@@ -62,14 +62,32 @@
             solver,
             0,
             1,
             0.01,
             y0,
             saveat=diffrax.SaveAt(dense=True, t1=True),
         )
+        y1 = solution.ys[-1]
+        paths.append((solution, type(solver).__name__, y0, y1))
+
+    for solver in all_split_solvers:
+        solver = implicit_tol(solver)
+        y0 = jrandom.normal(getkey(), (3,))
+        solution = diffrax.diffeqsolve(
+            diffrax.MultiTerm(
+                diffrax.ODETerm(lambda t, y, p: -0.7 * y),
+                diffrax.ODETerm(lambda t, y, p: -0.3 * y),
+            ),
+            solver,
+            0,
+            1,
+            0.01,
+            y0,
+            saveat=diffrax.SaveAt(dense=True, t1=True),
+        )
         y1 = solution.ys[-1]
         paths.append((solution, type(solver).__name__, y0, y1))
 
     # actually do tests
 
     for path, name, y0, y1 in paths:
         _test_path_derivative(path, name)
```

### Comparing `diffrax-0.3.1/test/test_local_interpolation.py` & `diffrax-0.4.0/test/test_local_interpolation.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 def test_local_linear_interpolation():
     t0 = 2.0
     t1 = 3.3
     t0_ = 2.8
     t1_ = 2.9
     for y0 in (2.1, jnp.array(2.1), jnp.array([2.1, 3.1])):
         for y1 in (2.2, jnp.array(2.2), jnp.array([2.2, 3.2])):
-            interp = diffrax.local_interpolation.LocalLinearInterpolation(
-                t0=t0, t1=t1, y0=y0, y1=y1
-            )
+            interp = diffrax.LocalLinearInterpolation(t0=t0, t1=t1, y0=y0, y1=y1)
 
             # evaluate position
             pred = interp.evaluate(t0_)
             true = y0 + (y1 - y0) * (t0_ - t0) / (t1 - t0)
             assert shaped_allclose(pred, true)
 
             _, pred = jax.jvp(interp.evaluate, (t0_,), (jnp.ones_like(t0_),))
@@ -32,16 +30,31 @@
 
             _, pred = jax.jvp(
                 interp.evaluate, (t0_, t1_), (jnp.ones_like(t0_), jnp.ones_like(t1_))
             )
             assert shaped_allclose(pred, jnp.zeros_like(pred))
 
             # evaluate over zero-length interval. Note t1=t0.
-            interp = diffrax.local_interpolation.LocalLinearInterpolation(
-                t0=t0, t1=t0, y0=y0, y1=y1
-            )
+            interp = diffrax.LocalLinearInterpolation(t0=t0, t1=t0, y0=y0, y1=y1)
             pred = interp.evaluate(t0)
             true, _ = jnp.broadcast_arrays(y0, y1)
             assert shaped_allclose(pred, true)
 
             _, pred = jax.jvp(interp.evaluate, (t0,), (jnp.ones_like(t0),))
             assert shaped_allclose(pred, jnp.zeros_like(pred))
+
+
+def test_third_order_hermite():
+    t0 = 2.0
+    t1 = 3.9
+
+    def y(t):
+        return 0.4 + 0.7 * t - 1.1 * t**2 + 0.4 * t**3
+
+    y0, f0 = jax.jvp(y, (t0,), (1.0,))
+    y1, f1 = jax.jvp(y, (t1,), (1.0,))
+    k0 = f0 * (t1 - t0)
+    k1 = f1 * (t1 - t0)
+    interp = diffrax.ThirdOrderHermitePolynomialInterpolation(
+        t0=t0, t1=t1, y0=y0, y1=y1, k0=k0, k1=k1
+    )
+    assert shaped_allclose(interp.evaluate(2.6), y(2.6))
```

### Comparing `diffrax-0.3.1/test/test_newton_solver.py` & `diffrax-0.4.0/test/test_newton_solver.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/test/test_saveat_solution.py` & `diffrax-0.4.0/test/test_saveat_solution.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/test/test_step_to.py` & `diffrax-0.4.0/test/test_step_to.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/test/test_term.py` & `diffrax-0.4.0/test/test_term.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.3.1/test/test_vmap.py` & `diffrax-0.4.0/test/test_vmap.py`

 * *Files identical despite different names*

