# Comparing `tmp/scar-4.3.0.tar.gz` & `tmp/scar-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scar-4.3.0.tar", last modified: Tue Feb 15 15:23:08 2022, max compression
+gzip compressed data, was "scar-4.3.1.tar", last modified: Mon May 22 11:11:50 2023, max compression
```

## Comparing `scar-4.3.0.tar` & `scar-4.3.1.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.553083 scar-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     5457 2022-02-15 15:23:08.553083 scar-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-02-15 15:22:47.000000 scar-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.541083 scar-4.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.545083 scar-4.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     4773 2022-02-15 15:22:47.000000 scar-4.3.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.541083 scar-4.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.541083 scar-4.3.0/examples/mask-detector-workflow/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.541083 scar-4.3.0/examples/mask-detector-workflow/blurry-faces/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.545083 scar-4.3.0/examples/mask-detector-workflow/blurry-faces/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2022-02-15 15:22:47.000000 scar-4.3.0/examples/mask-detector-workflow/blurry-faces/src/DetectorAPI.py
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-02-15 15:22:47.000000 scar-4.3.0/examples/mask-detector-workflow/blurry-faces/src/auto_blur_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3656 2022-02-15 15:22:47.000000 scar-4.3.0/examples/mask-detector-workflow/blurry-faces/src/auto_blur_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-02-15 15:22:47.000000 scar-4.3.0/examples/mask-detector-workflow/blurry-faces/src/manual_blur_image.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.545083 scar-4.3.0/examples/mask-detector-workflow/mask-detector/
--rw-r--r--   0 runner    (1001) docker     (121)     5370 2022-02-15 15:22:47.000000 scar-4.3.0/examples/mask-detector-workflow/mask-detector/mask-detector-image.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.545083 scar-4.3.0/scar/
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-02-15 15:22:47.000000 scar-4.3.0/scar/cmdtemplate.py
--rw-r--r--   0 runner    (1001) docker     (121)    10040 2022-02-15 15:22:47.000000 scar-4.3.0/scar/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.545083 scar-4.3.0/scar/http/
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-02-15 15:22:47.000000 scar-4.3.0/scar/http/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2022-02-15 15:22:47.000000 scar-4.3.0/scar/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.545083 scar-4.3.0/scar/parser/
--rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-02-15 15:22:47.000000 scar-4.3.0/scar/parser/cfgfile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.545083 scar-4.3.0/scar/parser/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     8428 2022-02-15 15:22:47.000000 scar-4.3.0/scar/parser/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6750 2022-02-15 15:22:47.000000 scar-4.3.0/scar/parser/cli/parents.py
--rw-r--r--   0 runner    (1001) docker     (121)     7741 2022-02-15 15:22:47.000000 scar-4.3.0/scar/parser/cli/subparsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-02-15 15:22:47.000000 scar-4.3.0/scar/parser/fdl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.541083 scar-4.3.0/scar/providers/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.549083 scar-4.3.0/scar/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4128 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (121)    11497 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/batchfunction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.549083 scar-4.3.0/scar/providers/aws/clients/
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4184 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (121)     3950 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/batchfunction.py
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/cloudwatchlogs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/ec2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/ecr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/iam.py
--rw-r--r--   0 runner    (1001) docker     (121)     6490 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/lambdafunction.py
--rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/resourcegroups.py
--rw-r--r--   0 runner    (1001) docker     (121)     4167 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/clients/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     5388 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/cloudwatchlogs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7673 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/containerimage.py
--rw-r--r--   0 runner    (1001) docker     (121)    20767 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/ecr.py
--rw-r--r--   0 runner    (1001) docker     (121)     6519 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/functioncode.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/iam.py
--rw-r--r--   0 runner    (1001) docker     (121)    17735 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/lambdafunction.py
--rw-r--r--   0 runner    (1001) docker     (121)     6104 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/lambdalayers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6628 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/launchtemplates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/resourcegroups.py
--rw-r--r--   0 runner    (1001) docker     (121)    11205 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6679 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/udocker.py
--rw-r--r--   0 runner    (1001) docker     (121)     6302 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/aws/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.549083 scar-4.3.0/scar/providers/oscar/
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/oscar/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4606 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/oscar/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-02-15 15:22:47.000000 scar-4.3.0/scar/providers/oscar/response.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2551 2022-02-15 15:22:47.000000 scar-4.3.0/scar/scarcli.py
--rw-r--r--   0 runner    (1001) docker     (121)    21230 2022-02-15 15:22:47.000000 scar-4.3.0/scar/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-02-15 15:22:47.000000 scar-4.3.0/scar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.545083 scar-4.3.0/scar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5457 2022-02-15 15:23:08.000000 scar-4.3.0/scar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-02-15 15:23:08.000000 scar-4.3.0/scar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 15:23:08.000000 scar-4.3.0/scar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-02-15 15:23:08.000000 scar-4.3.0/scar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-15 15:23:08.000000 scar-4.3.0/scar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-02-15 15:23:08.000000 scar-4.3.0/scar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-15 15:23:08.553083 scar-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-02-15 15:22:47.000000 scar-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.549083 scar-4.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 15:22:47.000000 scar-4.3.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.549083 scar-4.3.0/test/functional/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 15:22:47.000000 scar-4.3.0/test/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6362 2022-02-15 15:22:47.000000 scar-4.3.0/test/functional/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.549083 scar-4.3.0/test/functional/parser/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 15:22:47.000000 scar-4.3.0/test/functional/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-02-15 15:22:47.000000 scar-4.3.0/test/functional/parser/fdl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.549083 scar-4.3.0/test/unit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.549083 scar-4.3.0/test/unit/aws/
--rw-r--r--   0 runner    (1001) docker     (121)     3694 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/aws/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (121)     8762 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/aws/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2749 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/aws/test_cloudwatchlogs.py
--rw-r--r--   0 runner    (1001) docker     (121)    20009 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/aws/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/aws/test_ecr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/aws/test_iam.py
--rw-r--r--   0 runner    (1001) docker     (121)    16168 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/aws/test_lambdafunction.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/aws/test_resourcegroups.py
--rw-r--r--   0 runner    (1001) docker     (121)     6052 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/aws/test_s3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:23:08.553083 scar-4.3.0/test/unit/oscar/
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/oscar/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3567 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/oscar/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-02-15 15:22:47.000000 scar-4.3.0/test/unit/test_scarcli.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:50.004145 scar-4.3.1/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)    11357 2022-11-09 10:57:03.000000 scar-4.3.1/LICENSE
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     5522 2023-05-22 11:11:50.004145 scar-4.3.1/PKG-INFO
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     5047 2022-11-09 11:46:01.000000 scar-4.3.1/README.md
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.984146 scar-4.3.1/docs/
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.988146 scar-4.3.1/docs/source/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     4773 2022-11-09 10:57:03.000000 scar-4.3.1/docs/source/conf.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.984146 scar-4.3.1/examples/
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.984146 scar-4.3.1/examples/mask-detector-workflow/
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.984146 scar-4.3.1/examples/mask-detector-workflow/blurry-faces/
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.988146 scar-4.3.1/examples/mask-detector-workflow/blurry-faces/src/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2691 2022-11-09 10:57:03.000000 scar-4.3.1/examples/mask-detector-workflow/blurry-faces/src/DetectorAPI.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     3111 2022-11-09 10:57:03.000000 scar-4.3.1/examples/mask-detector-workflow/blurry-faces/src/auto_blur_image.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     3656 2022-11-09 10:57:03.000000 scar-4.3.1/examples/mask-detector-workflow/blurry-faces/src/auto_blur_video.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2676 2022-11-09 10:57:03.000000 scar-4.3.1/examples/mask-detector-workflow/blurry-faces/src/manual_blur_image.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.988146 scar-4.3.1/examples/mask-detector-workflow/mask-detector/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     5370 2022-11-09 10:57:03.000000 scar-4.3.1/examples/mask-detector-workflow/mask-detector/mask-detector-image.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.988146 scar-4.3.1/scar/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     1410 2022-11-09 10:57:03.000000 scar-4.3.1/scar/cmdtemplate.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)    10040 2022-11-09 10:57:03.000000 scar-4.3.1/scar/exceptions.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.992146 scar-4.3.1/scar/http/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     1382 2022-11-09 10:57:03.000000 scar-4.3.1/scar/http/request.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2843 2022-11-09 10:57:03.000000 scar-4.3.1/scar/logger.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.992146 scar-4.3.1/scar/parser/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     9366 2022-11-09 10:57:03.000000 scar-4.3.1/scar/parser/cfgfile.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.992146 scar-4.3.1/scar/parser/cli/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     8673 2022-11-09 10:57:03.000000 scar-4.3.1/scar/parser/cli/__init__.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     6750 2022-11-09 10:57:03.000000 scar-4.3.1/scar/parser/cli/parents.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     7741 2022-11-09 10:57:03.000000 scar-4.3.1/scar/parser/cli/subparsers.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2109 2022-11-09 10:57:03.000000 scar-4.3.1/scar/parser/fdl.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.984146 scar-4.3.1/scar/providers/
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.996146 scar-4.3.1/scar/providers/aws/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2456 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/__init__.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     4128 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/apigateway.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)    11498 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/batchfunction.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.996146 scar-4.3.1/scar/providers/aws/clients/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     1857 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/__init__.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     4184 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/apigateway.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     3950 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/batchfunction.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2851 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/cloudwatchlogs.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2515 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/ec2.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2488 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/ecr.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2092 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/iam.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     6490 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/lambdafunction.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2318 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/resourcegroups.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     4167 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/clients/s3.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     5372 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/cloudwatchlogs.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     7683 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/containerimage.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)    20767 2022-11-14 12:42:22.000000 scar-4.3.1/scar/providers/aws/controller.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     1954 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/ecr.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     6499 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/functioncode.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)      912 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/iam.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)    17809 2023-05-22 10:59:52.000000 scar-4.3.1/scar/providers/aws/lambdafunction.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     6104 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/lambdalayers.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     6628 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/launchtemplates.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     1835 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/resourcegroups.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)    11205 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/response.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     6679 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/s3.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     3338 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/udocker.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     6302 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/aws/validators.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.996146 scar-4.3.1/scar/providers/oscar/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     3941 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/oscar/client.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     4579 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/oscar/controller.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     3116 2022-11-09 10:57:03.000000 scar-4.3.1/scar/providers/oscar/response.py
+-rwxrwxr-x   0 micafer   (1000) micafer   (1000)     2545 2022-11-09 10:57:03.000000 scar-4.3.1/scar/scarcli.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)    21227 2022-11-09 10:57:03.000000 scar-4.3.1/scar/utils.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)      600 2023-05-22 11:11:25.000000 scar-4.3.1/scar/version.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.992146 scar-4.3.1/scar.egg-info/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     5522 2023-05-22 11:11:49.000000 scar-4.3.1/scar.egg-info/PKG-INFO
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2363 2023-05-22 11:11:49.000000 scar-4.3.1/scar.egg-info/SOURCES.txt
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)        1 2023-05-22 11:11:49.000000 scar-4.3.1/scar.egg-info/dependency_links.txt
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)       44 2023-05-22 11:11:49.000000 scar-4.3.1/scar.egg-info/entry_points.txt
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)       88 2023-05-22 11:11:49.000000 scar-4.3.1/scar.egg-info/requires.txt
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)       24 2023-05-22 11:11:49.000000 scar-4.3.1/scar.egg-info/top_level.txt
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)       38 2023-05-22 11:11:50.004145 scar-4.3.1/setup.cfg
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     1834 2022-11-09 10:57:03.000000 scar-4.3.1/setup.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:49.996146 scar-4.3.1/test/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)        0 2022-11-09 10:57:03.000000 scar-4.3.1/test/__init__.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:50.000146 scar-4.3.1/test/functional/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)        0 2022-11-09 10:57:03.000000 scar-4.3.1/test/functional/__init__.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     6204 2022-11-09 10:57:03.000000 scar-4.3.1/test/functional/aws.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:50.000146 scar-4.3.1/test/functional/parser/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)        0 2022-11-09 10:57:03.000000 scar-4.3.1/test/functional/parser/__init__.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2182 2022-11-09 10:57:03.000000 scar-4.3.1/test/functional/parser/fdl.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:50.000146 scar-4.3.1/test/unit/
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:50.000146 scar-4.3.1/test/unit/aws/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     3684 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/aws/test_apigateway.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     8762 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/aws/test_batch.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2749 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/aws/test_cloudwatchlogs.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)    20009 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/aws/test_controller.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     3341 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/aws/test_ecr.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     1510 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/aws/test_iam.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)    16180 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/aws/test_lambdafunction.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     1547 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/aws/test_resourcegroups.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     6061 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/aws/test_s3.py
+drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-05-22 11:11:50.000146 scar-4.3.1/test/unit/oscar/
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     4624 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/oscar/test_client.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     3563 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/oscar/test_controller.py
+-rw-rw-r--   0 micafer   (1000) micafer   (1000)     2151 2022-11-09 10:57:03.000000 scar-4.3.1/test/unit/test_scarcli.py
```

### Comparing `scar-4.3.0/PKG-INFO` & `scar-4.3.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,58 @@
-Metadata-Version: 2.1
-Name: scar
-Version: 4.3.0
-Summary: CLI for deploying serverless infrastructures on multiple cloud environments
-Home-page: https://github.com/grycap/scar
-Author: GRyCAP - Universitat Politecnica de Valencia
-Author-email: products@grycap.upv.es
-License: Apache 2.0
-Description: # SCAR - Serverless Container-aware ARchitectures
-        
-        [![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
-        [![Build Status](https://jenkins.i3m.upv.es/buildStatus/icon?job=grycap/scar)](https://jenkins.i3m.upv.es/job/grycap/job/scar/)
-        [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1968/badge)](https://bestpractices.coreinfrastructure.org/projects/1968)
-        
-        # ![SCAR](scar-logo.png)
-        
-        SCAR is a framework to transparently execute containers out of Docker images in AWS Lambda, in order to run applications (see examples for [ImageMagick](examples/imagemagick/README.md), [FFmpeg](examples/ffmpeg/README.md) and [AWS CLI](examples/aws-cli/README.md), as well as deep learning frameworks such as [Theano](examples/theano/README.md) and [Darknet](examples/darknet/README.md)) and code in virtually any programming language (see examples for [Ruby](examples/ruby), [R](examples/r), [Erlang](examples/erlang) and [Elixir](examples/elixir)) on AWS Lambda.
-        
-        SCAR provides the benefits of AWS Lambda with the execution environment you decide, provided as a Docker image available in Docker Hub. It is probably the easiest, most convenient approach to run generic applications on AWS Lambda, as well as code in your favourite programming language, not only in those languages supported by AWS Lambda.
-        
-        SCAR also supports a High Throughput Computing [Programming Model](https://scar.readthedocs.io/en/latest/prog_model.html) to create highly-parallel event-driven file-processing serverless applications that execute on customized runtime environments provided by Docker containers run on AWS Lambda. The development of SCAR has been published in the [Future Generation Computer Systems](https://www.journals.elsevier.com/future-generation-computer-systems) scientific journal.
-        
-        SCAR is integrated with API Gateway in order to expose an application via a highly-available HTTP-based REST API that supports both synchronous and asynchronous invocations. It is also integrated with AWS Batch. This way, AWS Lambda can be used to acommodate the execution of large bursts of short requests while long-running executions are delegated to AWS Batch.
-        
-        SCAR allows to create serverless workflows by combining functions that run on either AWS Batch or AWS Lambda which produce output files that trigger the execution of functions that, again, run on either AWS Batch or AWS Lambda, using the very same Docker images, thus effectively creating highly-scalable cross-services serverless workflows.
-        
-        <a name="toc"></a>
-        **Related resources**:  
-          [Scientific Paper](http://linkinghub.elsevier.com/retrieve/pii/S0167739X17316485) ([pre-print](http://www.grycap.upv.es/gmolto/publications/preprints/Perez2018scc.pdf)).
-        
-        ## Update 3.0.0
-        
-        Since version 3.0.0 SCAR creates a lambda layer called 'faas-supervisor' that includes the core functionality for the lambda containers.
-        This layer allows to deploy new functions faster. The layer is created once (the first time that a function is created or after a layer update) and then it's linked to all the other functions.
-        
-        If a new version of the supervisor is released (e.g. when a new feature is added or a bug is found) the functions can be updated with the command `scar update -a -sl`.
-        
-        To check the supervisor layer version that your function is using you only have to do an ls like `scar ls`
-        
-        ## Documentation
-        
-        SCAR documentation can be found in [readthedocs](http://scar.readthedocs.io/en/latest/).
-        
-        Also the examples have extra information that is usefull to execute them.
-        
-        ## Licensing
-        
-        SCAR is licensed under the Apache License, Version 2.0. See
-        [LICENSE](https://github.com/grycap/scar/blob/master/LICENSE) for the full
-        license text.
-        
-        <a id="furtherinfo"></a>
-        ## Further information
-        
-        There is further information on the architecture of SCAR and use cases in the scientific publication ["Serverless computing for container-based architectures"](http://linkinghub.elsevier.com/retrieve/pii/S0167739X17316485) (pre-print available [here](http://www.grycap.upv.es/gmolto/publications/preprints/Perez2018scc.pdf)), included in the Future Generation Computer Systems journal. Please acknowledge the use of SCAR by including the following cite:
-        
-        ```
-        A. Pérez, G. Moltó, M. Caballer, and A. Calatrava, “Serverless computing for container-based architectures,” Futur. Gener. Comput. Syst., vol. 83, pp. 50–59, Jun. 2018.
-        ```
-        
-        <a id="acknowledgements"></a>
-        ## Acknowledgements
-        
-        * [udocker](https://github.com/indigo-dc/udocker)
-        
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
+# SCAR - Serverless Container-aware ARchitectures
+
+[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
+[![test](https://github.com/grycap/scar/actions/workflows/main.yaml/badge.svg)](https://github.com/grycap/scar/actions/workflows/main.yaml)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/54fa508a76fa4001843abad945c127c9)](https://www.codacy.com/gh/grycap/scar/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=grycap/scar&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/54fa508a76fa4001843abad945c127c9)](https://www.codacy.com/gh/grycap/scar/dashboard?utm_source=github.com&utm_medium=referral&utm_content=grycap/scar&utm_campaign=Badge_Coverage)
+[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1968/badge)](https://bestpractices.coreinfrastructure.org/projects/1968)
+
+## ![SCAR](scar-logo.png)
+
+SCAR is a framework to transparently execute containers out of Docker images in AWS Lambda, in order to run applications (see examples for [ImageMagick](examples/imagemagick/README.md), [FFmpeg](examples/ffmpeg/README.md) and [AWS CLI](examples/aws-cli/README.md), as well as deep learning frameworks such as [Theano](examples/theano/README.md) and [Darknet](examples/darknet/README.md)) and code in virtually any programming language (see examples for [Ruby](examples/ruby), [R](examples/r), [Erlang](examples/erlang) and [Elixir](examples/elixir)) on AWS Lambda.
+
+SCAR provides the benefits of AWS Lambda with the execution environment you decide, provided as a Docker image available in Docker Hub. It is probably the easiest, most convenient approach to run generic applications on AWS Lambda, as well as code in your favourite programming language, not only in those languages supported by AWS Lambda.
+
+SCAR also supports a High Throughput Computing [Programming Model](https://scar.readthedocs.io/en/latest/prog_model.html) to create highly-parallel event-driven file-processing serverless applications that execute on customized runtime environments provided by Docker containers run on AWS Lambda. The development of SCAR has been published in the [Future Generation Computer Systems](https://www.journals.elsevier.com/future-generation-computer-systems) scientific journal.
+
+SCAR is integrated with API Gateway in order to expose an application via a highly-available HTTP-based REST API that supports both synchronous and asynchronous invocations. It is also integrated with AWS Batch. This way, AWS Lambda can be used to acommodate the execution of large bursts of short requests while long-running executions are delegated to AWS Batch.
+
+SCAR allows to create serverless workflows by combining functions that run on either AWS Batch or AWS Lambda which produce output files that trigger the execution of functions that, again, run on either AWS Batch or AWS Lambda, using the very same Docker images, thus effectively creating highly-scalable cross-services serverless workflows.
+
+<a name="toc"></a>
+**Related resources**:  
+  [Scientific Paper](http://linkinghub.elsevier.com/retrieve/pii/S0167739X17316485) ([pre-print](http://www.grycap.upv.es/gmolto/publications/preprints/Perez2018scc.pdf)).
+
+## Update 3.0.0
+
+Since version 3.0.0 SCAR creates a lambda layer called 'faas-supervisor' that includes the core functionality for the lambda containers.
+This layer allows to deploy new functions faster. The layer is created once (the first time that a function is created or after a layer update) and then it's linked to all the other functions.
+
+If a new version of the supervisor is released (e.g. when a new feature is added or a bug is found) the functions can be updated with the command `scar update -a -sl`.
+
+To check the supervisor layer version that your function is using you only have to do an ls like `scar ls`
+
+## Documentation
+
+SCAR documentation can be found in [readthedocs](http://scar.readthedocs.io/en/latest/).
+
+Also the examples have extra information that is usefull to execute them.
+
+## Licensing
+
+SCAR is licensed under the Apache License, Version 2.0. See
+[LICENSE](https://github.com/grycap/scar/blob/master/LICENSE) for the full
+license text.
+
+<a id="furtherinfo"></a>
+## Further information
+
+There is further information on the architecture of SCAR and use cases in the scientific publication ["Serverless computing for container-based architectures"](http://linkinghub.elsevier.com/retrieve/pii/S0167739X17316485) (pre-print available [here](http://www.grycap.upv.es/gmolto/publications/preprints/Perez2018scc.pdf)), included in the Future Generation Computer Systems journal. Please acknowledge the use of SCAR by including the following cite:
+
+```
+A. Pérez, G. Moltó, M. Caballer, and A. Calatrava, “Serverless computing for container-based architectures,” Futur. Gener. Comput. Syst., vol. 83, pp. 50–59, Jun. 2018.
+```
+
+<a id="acknowledgements"></a>
+## Acknowledgements
+
+*  [udocker](https://github.com/indigo-dc/udocker)
```

### Comparing `scar-4.3.0/README.md` & `scar-4.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,30 @@
+Metadata-Version: 2.1
+Name: scar
+Version: 4.3.1
+Summary: CLI for deploying serverless infrastructures on multiple cloud environments
+Home-page: https://github.com/grycap/scar
+Author: GRyCAP - Universitat Politecnica de Valencia
+Author-email: products@grycap.upv.es
+License: Apache 2.0
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SCAR - Serverless Container-aware ARchitectures
 
 [![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
-[![Build Status](https://jenkins.i3m.upv.es/buildStatus/icon?job=grycap/scar)](https://jenkins.i3m.upv.es/job/grycap/job/scar/)
+[![test](https://github.com/grycap/scar/actions/workflows/main.yaml/badge.svg)](https://github.com/grycap/scar/actions/workflows/main.yaml)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/54fa508a76fa4001843abad945c127c9)](https://www.codacy.com/gh/grycap/scar/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=grycap/scar&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/54fa508a76fa4001843abad945c127c9)](https://www.codacy.com/gh/grycap/scar/dashboard?utm_source=github.com&utm_medium=referral&utm_content=grycap/scar&utm_campaign=Badge_Coverage)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1968/badge)](https://bestpractices.coreinfrastructure.org/projects/1968)
 
-# ![SCAR](scar-logo.png)
+## ![SCAR](scar-logo.png)
 
 SCAR is a framework to transparently execute containers out of Docker images in AWS Lambda, in order to run applications (see examples for [ImageMagick](examples/imagemagick/README.md), [FFmpeg](examples/ffmpeg/README.md) and [AWS CLI](examples/aws-cli/README.md), as well as deep learning frameworks such as [Theano](examples/theano/README.md) and [Darknet](examples/darknet/README.md)) and code in virtually any programming language (see examples for [Ruby](examples/ruby), [R](examples/r), [Erlang](examples/erlang) and [Elixir](examples/elixir)) on AWS Lambda.
 
 SCAR provides the benefits of AWS Lambda with the execution environment you decide, provided as a Docker image available in Docker Hub. It is probably the easiest, most convenient approach to run generic applications on AWS Lambda, as well as code in your favourite programming language, not only in those languages supported by AWS Lambda.
 
 SCAR also supports a High Throughput Computing [Programming Model](https://scar.readthedocs.io/en/latest/prog_model.html) to create highly-parallel event-driven file-processing serverless applications that execute on customized runtime environments provided by Docker containers run on AWS Lambda. The development of SCAR has been published in the [Future Generation Computer Systems](https://www.journals.elsevier.com/future-generation-computer-systems) scientific journal.
 
@@ -49,8 +65,10 @@
 ```
 A. Pérez, G. Moltó, M. Caballer, and A. Calatrava, “Serverless computing for container-based architectures,” Futur. Gener. Comput. Syst., vol. 83, pp. 50–59, Jun. 2018.
 ```
 
 <a id="acknowledgements"></a>
 ## Acknowledgements
 
-* [udocker](https://github.com/indigo-dc/udocker)
+*  [udocker](https://github.com/indigo-dc/udocker)
+
+
```

### Comparing `scar-4.3.0/docs/source/conf.py` & `scar-4.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/examples/mask-detector-workflow/blurry-faces/src/DetectorAPI.py` & `scar-4.3.1/examples/mask-detector-workflow/blurry-faces/src/DetectorAPI.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/examples/mask-detector-workflow/blurry-faces/src/auto_blur_image.py` & `scar-4.3.1/examples/mask-detector-workflow/blurry-faces/src/auto_blur_image.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/examples/mask-detector-workflow/blurry-faces/src/auto_blur_video.py` & `scar-4.3.1/examples/mask-detector-workflow/blurry-faces/src/auto_blur_video.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/examples/mask-detector-workflow/blurry-faces/src/manual_blur_image.py` & `scar-4.3.1/examples/mask-detector-workflow/blurry-faces/src/manual_blur_image.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/examples/mask-detector-workflow/mask-detector/mask-detector-image.py` & `scar-4.3.1/examples/mask-detector-workflow/mask-detector/mask-detector-image.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/cmdtemplate.py` & `scar-4.3.1/scar/cmdtemplate.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,29 +19,29 @@
     INIT = "init"
     INVOKE = "invoke"
     RUN = "run"
     LS = "ls"
     RM = "rm"
     LOG = "log"
     PUT = "put"
-    GET = "get"  
+    GET = "get"
 
 class Commands(metaclass=abc.ABCMeta):
-    ''' All the different cloud provider controllers must inherit 
+    ''' All the different cloud provider controllers must inherit
     from this class to ensure that the commands are defined consistently'''
 
     @abc.abstractmethod
     def init(self):
         pass
 
-    @abc.abstractmethod    
+    @abc.abstractmethod
     def invoke(self):
         pass
 
-    @abc.abstractmethod    
+    @abc.abstractmethod
     def run(self):
         pass
 
     @abc.abstractmethod    
     def ls(self):
         pass
 
@@ -55,8 +55,8 @@
 
     @abc.abstractmethod
     def put(self):
         pass
 
     @abc.abstractmethod
     def get(self):
-        pass    
+        pass
```

### Comparing `scar-4.3.0/scar/exceptions.py` & `scar-4.3.1/scar/exceptions.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/http/request.py` & `scar-4.3.1/scar/http/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import requests
 
 def call_http_endpoint(url, **kwargs):
-    """
-    Does a 'GET' or 'PUT' request if the parameter 'data' exists or not respectively
+    """Does a 'GET' or 'PUT' request if the parameter 'data' exists or not respectively
 
-    :param url: URL for the request.        
+    :param url: URL for the request.
     :param data: (optional) Dictionary (will be form-encoded), bytes, or file-like object to send in the body of the request.
     :param headers: (optional) Dictionary of HTTP Headers to send with the request.
     :param parameters: (optional) Dictionary or bytes to be sent in the query string.
     """
     if ('data' in kwargs and kwargs['data']) or ('json' in kwargs and kwargs['json']):
         response = requests.post(url, **kwargs)
     else:
```

### Comparing `scar-4.3.0/scar/logger.py` & `scar-4.3.1/scar/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 loglevel = logging.INFO
 FORMAT = '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 logging.basicConfig(filename=log_file_path, level=loglevel, format=FORMAT)
 
 def init_execution_trace():
     logging.info('----------------------------------------------------')
     logging.info('SCAR execution started')
-    
+
 def end_execution_trace():
     logging.info('SCAR execution finished')
-    logging.info('----------------------------------------------------')     
-        
+    logging.info('----------------------------------------------------')
+
 def end_execution_trace_with_errors():
     logging.info('SCAR execution finished with errors')
     logging.info('----------------------------------------------------')
 
 def debug(cli_msg, log_msg=None):
     if loglevel == logging.DEBUG:
         print(cli_msg)
@@ -60,17 +60,17 @@
 def error(cli_msg, log_msg=None):
     if log_msg:
         print(log_msg)
         logging.error(log_msg)
     else:
         print(cli_msg)
         logging.error(cli_msg)
-        
+
 def exception(msg):
-    logging.exception(msg)        
+    logging.exception(msg)
 
 def log_exception(error_msg, exception):
     error(error_msg, error_msg + ": {0}".format(exception))
 
 def print_json(value):
     print(json.dumps(value))
 
@@ -80,8 +80,8 @@
 
 def warning_json(cli_msg, log_msg=None):
     print_json(cli_msg)
     logging.warning(log_msg) if log_msg else logging.warning(cli_msg)
 
 def error_json(cli_msg, log_msg=None):
     print_json(cli_msg)
-    logging.error(log_msg) if log_msg else logging.error(cli_msg)          
+    logging.error(log_msg) if log_msg else logging.error(cli_msg)
```

### Comparing `scar-4.3.0/scar/parser/cfgfile.py` & `scar-4.3.1/scar/parser/cfgfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,31 +61,31 @@
                 "Variables": {
                     "UDOCKER_BIN" : "/opt/udocker/bin/",
                     "UDOCKER_LIB" : "/opt/udocker/lib/",
                     "UDOCKER_DIR" : "/tmp/shared/udocker",
                     "UDOCKER_EXEC": "/opt/udocker/udocker.py"}},
             "deployment": {
                 "max_payload_size": 52428800,
-                "max_s3_payload_size": 262144000           
+                "max_s3_payload_size": 262144000
             },
             "container": {
                 "environment" : {
                     "Variables" : {}},
                 "timeout_threshold": 10
             },
             # Must be a Github tag or "latest"
             "supervisor": {
                 "version": "latest",
                 'layer_name' : "faas-supervisor",
-                'license_info' : 'Apache 2.0'                
+                'license_info' : 'Apache 2.0'
             }
         },
         "s3": {
             "boto_profile": "default",
-            "region": "us-east-1",            
+            "region": "us-east-1",
             "event" : {
                 "Records": [{
                     "eventSource": "aws:s3",
                     "s3" : {
                         "bucket" : {
                             "name": "{bucket_name}",
                             "arn": "arn:aws:s3:::{bucket_name}"
@@ -95,15 +95,15 @@
                         }
                     }
                 }]
             }
         },
         "api_gateway": {
             "boto_profile": "default",
-            "region": "us-east-1",            
+            "region": "us-east-1",
             "endpoint": "https://{api_id}.execute-api.{api_region}.amazonaws.com/{stage_name}/launch",
             'request_parameters': {"integration.request.header.X-Amz-Invocation-Type":
                                    "method.request.header.X-Amz-Invocation-Type"},
             # ANY, DELETE, GET, HEAD, OPTIONS, PATCH, POST, PUT
             'http_method': "ANY",
             "method" : {
                 # NONE, AWS_IAM, CUSTOM, COGNITO_USER_POOLS
@@ -112,15 +112,15 @@
             },
             "integration": {
                 # 'HTTP'|'AWS'|'MOCK'|'HTTP_PROXY'|'AWS_PROXY'
                 'type': "AWS_PROXY",
                 'integrationHttpMethod' : "POST",
                 'uri' : "arn:aws:apigateway:{api_region}:lambda:path/2015-03-31/functions/arn:aws:lambda:{lambda_region}:{account_id}:function:{function_name}/invocations",
                 'requestParameters' : {"integration.request.header.X-Amz-Invocation-Type":
-                                       "method.request.header.X-Amz-Invocation-Type"}            
+                                       "method.request.header.X-Amz-Invocation-Type"}
             },
             'path_part': "{proxy+}",
             'stage_name': "scar",
             # Used to add invocation permissions to lambda
             'service_id': 'apigateway.amazonaws.com',
             'source_arn_testing': 'arn:aws:execute-api:{api_region}:{account_id}:{api_id}/*',
             'source_arn_invocation': 'arn:aws:execute-api:{api_region}:{account_id}:{api_id}/{stage_name}/ANY'
@@ -152,15 +152,15 @@
                 "min_v_cpus": 0,
                 "max_v_cpus": 2,
                 "subnets": [],
                 "instance_types": ["m3.medium"],
                 "launch_template_name": "faas-supervisor",
                 "instance_role": "arn:aws:iam::{account_id}:instance-profile/ecsInstanceRole"
             },
-            "service_role": "arn:aws:iam::{account_id}:role/service-role/AWSBatchServiceRole"            
+            "service_role": "arn:aws:iam::{account_id}:role/service-role/AWSBatchServiceRole"
         }
     }
 }
 
 
 class ConfigFileParser():
     """Class to manage the SCAR configuration file creation, update and load."""
```

### Comparing `scar-4.3.0/scar/parser/cli/__init__.py` & `scar-4.3.1/scar/parser/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Module with methods and classes in charge
 of parsing the SCAR CLI commands."""
 
 import argparse
 import sys
-from typing import Dict, List
+from typing import Dict
 from scar.parser.cli.subparsers import Subparsers
-from scar.parser.cli.parents import *
-from scar.utils import DataTypesUtils, StrUtils, FileUtils
+from scar.parser.cli.parents import (create_exec_parser,
+                                     create_function_definition_parser,
+                                     create_output_parser,
+                                     create_profile_parser,
+                                     create_storage_parser)
+from scar.utils import DataTypesUtils, FileUtils
 from scar.cmdtemplate import CallType
 import scar.exceptions as excp
 import scar.logger as logger
 import scar.version as version
 
 
 def _parse_aws_args(cmd_args: Dict) -> Dict:
@@ -79,23 +83,23 @@
         # These variables define the udocker container environment variables
         for env_var in lambda_args["environment_variables"]:
             key_val = env_var.split("=")
             # Add an specific prefix to be able to find the container variables defined by the user
             lambda_env_vars['container']['environment']['Variables'][f'{key_val[0]}'] = key_val[1]
         del(lambda_args['environment_variables'])
     if "extra_payload" in lambda_args:
-        lambda_env_vars['container']['extra_payload'] = f"/var/task"
+        lambda_env_vars['container']['extra_payload'] = "/var/task"
     if "init_script" in lambda_args:
         lambda_env_vars['container']['init_script'] = f"/var/task/{FileUtils.get_file_name(lambda_args['init_script'])}"
     if "image" in lambda_args:
         lambda_env_vars['container']['image'] = lambda_args.get('image')
         del(lambda_args['image'])
     if "image_file" in lambda_args:
         lambda_env_vars['container']['image_file'] = lambda_args.get('image_file')
-        del(lambda_args['image_file'])        
+        del(lambda_args['image_file'])
 
     if "lambda_environment" in lambda_args:
         # These variables define the lambda environment variables
         for env_var in lambda_args["lambda_environment"]:
             key_val = env_var.split("=")
             lambda_env_vars['environment']['Variables'][f'{key_val[0]}'] = key_val[1]
         del(lambda_args['lambda_environment'])
```

### Comparing `scar-4.3.0/scar/parser/cli/parents.py` & `scar-4.3.1/scar/parser/cli/parents.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/parser/cli/subparsers.py` & `scar-4.3.1/scar/parser/cli/subparsers.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/parser/fdl.py` & `scar-4.3.1/scar/parser/fdl.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/__init__.py` & `scar-4.3.1/scar/providers/aws/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,14 @@
         self.properties = {}
         if resource_info:
             region = resource_info.get('region')
             if region:
                 self.properties['client'] = {'region_name': region}
             session = resource_info.get('boto_profile')
             if session:
-                self.properties['session'] = {'profile_name': session}        
+                self.properties['session'] = {'profile_name': session}
 
     @lazy_property
     def client(self):
         """Returns the required boto client based on the implementing class name."""
         client = self._CLIENTS[self.__class__.__name__.upper()](self.properties)
         return client
```

### Comparing `scar-4.3.0/scar/providers/aws/apigateway.py` & `scar-4.3.1/scar/providers/aws/apigateway.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/batchfunction.py` & `scar-4.3.1/scar/providers/aws/batchfunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
                     'value': '1',
                     'type': 'GPU'
                 }
             ]
         return job_def_args
 
     def _get_node_properties_multi_node_args(self):
-        targetNodes = self.batch.get('multi_node_parallel').get('number_nodes') - 1
+        #targetNodes = self.batch.get('multi_node_parallel').get('number_nodes') - 1
         job_def_args = {
             "numNodes": int(self.batch.get('multi_node_parallel').get('number_nodes')),
             "mainNode": int(self.batch.get('multi_node_parallel').get('main_node_index')),
             "nodeRangeProperties": [
                 {
                 "targetNodes": "0:", #+ str(targetNodes),
                 "container": self._get_container_properties_single_node_args()
```

### Comparing `scar-4.3.0/scar/providers/aws/clients/__init__.py` & `scar-4.3.1/scar/providers/aws/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/clients/apigateway.py` & `scar-4.3.1/scar/providers/aws/clients/apigateway.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/clients/batchfunction.py` & `scar-4.3.1/scar/providers/aws/clients/batchfunction.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/clients/cloudwatchlogs.py` & `scar-4.3.1/scar/providers/aws/clients/cloudwatchlogs.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/clients/ec2.py` & `scar-4.3.1/scar/providers/aws/clients/ec2.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/clients/ecr.py` & `scar-4.3.1/scar/providers/aws/clients/ecr.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/clients/iam.py` & `scar-4.3.1/scar/providers/aws/clients/iam.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/clients/lambdafunction.py` & `scar-4.3.1/scar/providers/aws/clients/lambdafunction.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/clients/resourcegroups.py` & `scar-4.3.1/scar/providers/aws/clients/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/clients/s3.py` & `scar-4.3.1/scar/providers/aws/clients/s3.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/cloudwatchlogs.py` & `scar-4.3.1/scar/providers/aws/cloudwatchlogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     data = [(event.get('message', ''), event.get('timestamp', '')) for event in log_events]
     sorted_data = sorted(data, key=lambda time: time[1])
     return "".join([sdata[0] for sdata in sorted_data])
 
 
 class CloudWatchLogs(GenericClient):
     """Manages the AWS CloudWatch Logs functionality"""
-    
+
     def __init__(self, resources_info: Dict):
         super().__init__(resources_info.get('cloudwatch'))
         self.resources_info = resources_info
         self.cloudwatch = resources_info.get('cloudwatch')
 
     def get_log_group_name(self, function_name: str=None) -> str:
         """Returns the log group matching the
@@ -75,15 +75,15 @@
                 kwargs["logStreamNames"] = [self.cloudwatch.get("log_stream_name")]
             function_logs = _parse_events_in_message(self.client.get_log_events(**kwargs))
             if self.cloudwatch.get("request_id", False):
                 function_logs = self._parse_logs_with_requestid(function_logs)
         except ClientError as cerr:
             logger.warning("Error getting the function logs: %s" % cerr)
         return function_logs
-            
+
     def _get_batch_job_log(self, jobs_info: List) -> str:
         """Returns Batch logs for an specific job."""
         batch_logs = ""
         if jobs_info:
             job = jobs_info[0]
             batch_logs += f"Batch job status: {job.get('status', '')}\n"
             kwargs = {'logGroupName': "/aws/batch/job"}
```

### Comparing `scar-4.3.0/scar/providers/aws/containerimage.py` & `scar-4.3.1/scar/providers/aws/containerimage.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,16 +109,16 @@
         dockerfile += 'WORKDIR ${FUNCTION_DIR}\n'
         dockerfile += 'ENV PATH="${FUNCTION_DIR}:${PATH}"\n'
         # Add PYTHONIOENCODING to avoid UnicodeEncodeError as sugested in:
         # https://github.com/aws/aws-lambda-python-runtime-interface-client/issues/19
         dockerfile += 'ENV PYTHONIOENCODING="utf8"\n'
 
         # Add user environment variables
-        vars = lambda_info.get('container').get('environment').get('Variables', {})
-        for key, value in vars.items():
+        variables = lambda_info.get('container').get('environment').get('Variables', {})
+        for key, value in variables.items():
             dockerfile += 'ENV %s="%s"\n' % (key, value)
 
         dockerfile += 'CMD [ "supervisor" ]\n'
         dockerfile += 'ADD supervisor ${FUNCTION_DIR}\n'
         dockerfile += 'COPY function_config.yaml ${FUNCTION_DIR}\n'
         init_script_path = lambda_info.get('init_script')
         if init_script_path:
```

### Comparing `scar-4.3.0/scar/providers/aws/controller.py` & `scar-4.3.1/scar/providers/aws/controller.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/ecr.py` & `scar-4.3.1/scar/providers/aws/ecr.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from typing import Dict
 from scar.providers.aws import GenericClient
 
 
 class ECR(GenericClient):
     """Manages the AWS ElasticContainerRegistry functionality"""
-    
+
     def __init__(self, resources_info: Dict):
         super().__init__()
         self.resources_info = resources_info
 
     def get_authorization_token(self) -> str:
         """Retrieves an authorization token."""
         return self.client.get_authorization_token()
```

### Comparing `scar-4.3.0/scar/providers/aws/functioncode.py` & `scar-4.3.1/scar/providers/aws/functioncode.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from _ast import Or
 """Module with methods and classes to create the function deployment package."""
 
 from typing import Dict
 from zipfile import ZipFile
 import ntpath
 from scar.providers.aws.udocker import Udocker
 from scar.providers.aws.validators import AWSValidator
```

### Comparing `scar-4.3.0/scar/providers/aws/iam.py` & `scar-4.3.1/scar/providers/aws/iam.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/lambdafunction.py` & `scar-4.3.1/scar/providers/aws/lambdafunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     def __init__(self, resources_info: Dict) -> None:
         super().__init__(resources_info.get('lambda', {}))
         self.resources_info = resources_info
         self.function = resources_info.get('lambda', {})
         self.supervisor_version = resources_info.get('lambda').get('supervisor').get('version')
         if (self.function.get('runtime') == "image" and
+                self.supervisor_version != "latest" and
                 StrUtils.compare_versions(self.supervisor_version, "1.5.0b3") < 0):
             # In case of using image runtime
             # it must be 1.5.0-beta3 version or higher
             raise Exception("Supervisor version must be 1.5.0 or higher for image runtime.")
 
     def _get_creations_args(self, zip_payload_path: str, supervisor_zip_path: str) -> Dict:
         args = {'FunctionName': self.function.get('name'),
@@ -315,15 +316,15 @@
     def get_api_gateway_id(self):
         env_vars = self._get_function_environment_variables()
         return env_vars['Variables'].get('API_GATEWAY_ID', '')
 
     def _get_api_gateway_url(self):
         api_id = self.get_api_gateway_id()
         if not api_id:
-            raise excp.ApiEndpointNotFoundError(self.function.get('name'))
+            raise excp.ApiEndpointNotFoundError(function_name=self.function.get('name'))
         return self.resources_info.get('api_gateway').get('endpoint').format(api_id=api_id,
                                                                              api_region=self.resources_info.get('api_gateway').get('region'),
                                                                              stage_name=self.resources_info.get('api_gateway').get('stage_name'))
 
     def call_http_endpoint(self):
         invoke_args = {'headers': {'X-Amz-Invocation-Type': 'Event'} if self.is_asynchronous() else {}}
         self._set_invoke_args(invoke_args)
@@ -336,15 +337,15 @@
         if self.resources_info.get('api_gateway').get('parameters', False):
             invoke_args['params'] = self._parse_http_parameters(self.resources_info.get('api_gateway').get('parameters'))
         if self.resources_info.get('api_gateway').get('json_data', False):
             invoke_args['data'] = self._parse_http_parameters(self.resources_info.get('api_gateway').get('json_data'))
             invoke_args['headers'].update({'Content-Type': 'application/json'})
 
     def _parse_http_parameters(self, parameters):
-        return parameters if type(parameters) is dict else json.loads(parameters)
+        return parameters if isinstance(parameters, dict) else json.loads(parameters)
 
     @excp.exception(logger)
     def _get_b64encoded_binary_data(self):
         data_path = self.resources_info.get('api_gateway').get('data_binary')
         AWSValidator.validate_http_payload_size(data_path, self.is_asynchronous())
         with open(data_path, 'rb') as data_file:
             return base64.b64encode(data_file.read())
```

### Comparing `scar-4.3.0/scar/providers/aws/lambdalayers.py` & `scar-4.3.1/scar/providers/aws/lambdalayers.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/launchtemplates.py` & `scar-4.3.1/scar/providers/aws/launchtemplates.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/resourcegroups.py` & `scar-4.3.1/scar/providers/aws/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/response.py` & `scar-4.3.1/scar/providers/aws/response.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/s3.py` & `scar-4.3.1/scar/providers/aws/s3.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/udocker.py` & `scar-4.3.1/scar/providers/aws/udocker.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/aws/validators.py` & `scar-4.3.1/scar/providers/aws/validators.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/scar/providers/oscar/client.py` & `scar-4.3.1/scar/providers/oscar/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Module with the class implementing the low-level functions to 
+"""Module with the class implementing the low-level functions to
 communicate with an OSCAR cluster."""
 
 from typing import Dict, List
 import scar.logger as logger
 import scar.exceptions as excp
 import requests
 
@@ -31,27 +31,27 @@
         error_msg = 'Bad Request'
     elif res.status_code == 401:
         error_msg = 'Invalid Credentials'
     elif res.status_code == 404:
         error_msg = 'The Service doesn\'t exist'
     elif res.status_code == 500:
         error_msg = 'Internal Server Error'
-    return error_msg    
+    return error_msg
 
 
 class OSCARClient():
     _SERVICES_PATH = '/system/services'
 
     def __init__(self, credentials_info: Dict, cluster_id: str):
         self.cluster_id = cluster_id
         self.endpoint = credentials_info['endpoint']
         self.auth_user = credentials_info['auth_user']
         self.auth_password = credentials_info['auth_password']
         self.ssl_verify = credentials_info['ssl_verify']
-        
+
     def create_service(self, **kwargs: Dict) -> Dict:
         """Creates a new OSCAR service."""
         logger.debug('Creating OSCAR service.')
         res = requests.post(
             f'{self.endpoint}{self._SERVICES_PATH}',
             auth=(self.auth_user, self.auth_password),
             verify=self.ssl_verify,
```

### Comparing `scar-4.3.0/scar/providers/oscar/controller.py` & `scar-4.3.1/scar/providers/oscar/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Module with class and methods used to manage the OSCAR provider."""
 
 from typing import Dict
 from copy import deepcopy
-from scar.utils import StrUtils, FileUtils, SupervisorUtils
+from scar.utils import FileUtils
 from scar.providers.oscar.client import OSCARClient
 from scar.providers.aws.controller import add_output
 import scar.exceptions as excp
 import scar.logger as logger
 import scar.providers.oscar.response as response_parser
```

### Comparing `scar-4.3.0/scar/providers/oscar/response.py` & `scar-4.3.1/scar/providers/oscar/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Module with the class implementing the low-level functions to 
+"""Module with the class implementing the low-level functions to
 communicate with an OSCAR cluster."""
 
 from typing import Dict, List
 from tabulate import tabulate
 from scar.providers.aws.response import OutputType
 import scar.logger as logger
-from scar.utils import StrUtils
 
 
 def parse_ls_response(oscar_resources: List, endpoint: str, cluster_id: str, output_type: int) -> None:
     oscar_output = 'Services'
     result = []
     text_message = f'\nOSCAR SERVICES - CLUSTER "{cluster_id}" ({endpoint}):\n'
     for resources_info in oscar_resources:
```

### Comparing `scar-4.3.0/scar/scarcli.py` & `scar-4.3.1/scar/scarcli.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         # Default provider
         # If more providers, analyze the arguments and build the required one
         AWS(func_call)
         # Build the OSCAR controller only with 'init', 'rm' and 'ls' commands
         if func_call in ['init', 'rm', 'ls']:
             OSCAR(func_call)
         logger.end_execution_trace()
-    except Exception as excp:
-        print(excp)
-        logger.exception(excp)
+    except Exception as ex:
+        print(ex)
+        logger.exception(ex)
         logger.end_execution_trace_with_errors()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `scar-4.3.0/scar/utils.py` & `scar-4.3.1/scar/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,27 +35,28 @@
 from scar.exceptions import GitHubTagNotFoundError, YamlFileNotFoundError
 
 COMMANDS = ['scar-config']
 
 
 def lazy_property(func):
     # Skipped type hinting: https://github.com/python/mypy/issues/3157
-    """ A decorator that makes a property lazy-evaluated."""
+    """A decorator that makes a property lazy-evaluated."""
     attr_name = '_lazy_' + func.__name__
 
     @property
     def _lazy_property(self):
         if not hasattr(self, attr_name):
             setattr(self, attr_name, func(self))
         return getattr(self, attr_name)
 
     return _lazy_property
 
 
 class SysUtils:
+
     """Common methods for system management."""
 
     @staticmethod
     def is_variable_in_environment(variable: str) -> bool:
         """Checks if a variable is in the system environment."""
         return variable in os.environ
 
@@ -95,20 +96,22 @@
     def finish_scar_execution() -> None:
         """Finishes the program execution."""
         logger.end_execution_trace()
         sys.exit(0)
 
 
 class DataTypesUtils:
+
     """Common methods for data types management."""
 
     @staticmethod
     def merge_dicts(dict1: Dict, dict2: Dict) -> Dict:
         """Merge 'dict1' and 'dict2' dicts into 'dict1'.
-        'dict2' has precedence over 'dict1'."""
+        'dict2' has precedence over 'dict1'.
+        """
         for key, val in dict2.items():
             if val is not None:
                 if isinstance(val, dict) and key in dict1:
                     dict1[key] = DataTypesUtils.merge_dicts(dict1[key], val)
                 elif isinstance(val, list) and key in dict1:
                     dict1[key] += val
                 else:
@@ -136,44 +139,43 @@
         if not elements:
             yield []
         for i in range(0, len(elements), chunk_size):
             yield elements[i:i + chunk_size]
 
     @staticmethod
     def parse_arg_list(arg_keys: List, cmd_args: Dict) -> Dict:
-        """Parse an argument dictionary filtering by the names
-        specified in a list."""
+        """Parse an argument dictionary filtering by the names specified in a list."""
         result = {}
         for key in arg_keys:
             if isinstance(key, tuple):
                 if key[0] in cmd_args and cmd_args[key[0]]:
                     result[key[1]] = cmd_args[key[0]]
             else:
                 if key in cmd_args and cmd_args[key]:
                     result[key] = cmd_args[key]
         return result
 
 
 class FileUtils:
+
     """Common methods for file and directory management."""
 
     @staticmethod
     def copy_file(source: str, dest: str) -> None:
         """Copy file to specified destination."""
         shutil.copy(source, dest)
 
     @staticmethod
     def copy_dir(source: str, dest: str) -> None:
         """Copy directory to specified destination."""
         dir_util.copy_tree(source, dest)
 
     @staticmethod
     def create_folder(folder_name):
-        """Creates a system folder.
-        Does nothing if the folder exists."""
+        """Creates a system folder. Does nothing if the folder exists."""
         os.makedirs(folder_name, exist_ok=True)
 
     @staticmethod
     def get_scar_root_path() -> str:
         """Returns the root path of the project."""
         return os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
@@ -320,14 +322,15 @@
     @staticmethod
     def extract_zip_from_url(url: str, dest_path: str) -> None:
         with ZipFile(BytesIO(url)) as thezip:
             thezip.extractall(dest_path)
 
 
 class StrUtils:
+
     """Common methods for string management."""
 
     @staticmethod
     def decode_base64(value: Union[bytes, str]) -> bytes:
         """Decode a Base64 encoded bytes-like object or
         ASCII string and return the decoded bytes"""
         return base64.b64decode(value)
@@ -386,14 +389,15 @@
             res = -1
         elif version.parse(ver1) > version.parse(ver2):
             res = 1
         return res
 
 
 class GitHubUtils:
+
     """Common methods for GitHub API Queries.
     https://developer.github.com/v3/repos/releases/"""
 
     @staticmethod
     def get_latest_release(user: str, project: str) -> str:
         """Get the tag of the latest release in a repository."""
         url = f'https://api.github.com/repos/{user}/{project}/releases/latest'
@@ -450,14 +454,15 @@
             response = json.loads(request.get_file(repo_url))
             if isinstance(response, dict):
                 source_url = response.get('zipball_url')
         return source_url
 
 
 class SupervisorUtils:
+
     """Common methods for FaaS Supervisor management.
     https://github.com/grycap/faas-supervisor/"""
 
     _SUPERVISOR_GITHUB_REPO = 'faas-supervisor'
     _SUPERVISOR_GITHUB_USER = 'grycap'
     _SUPERVISOR_GITHUB_ASSET_NAME = 'supervisor'
     _SUPERVISOR_CACHE_DIR = '/var/tmp/cache/scar'
@@ -518,15 +523,15 @@
 
     @classmethod
     def is_supervisor_asset_cached(cls, asset_name: str, supervisor_version: str) -> Tuple[bool, str]:
         """Check if specified supervisor asset is cached."""
         supervisor_path = FileUtils.join_paths(cls._SUPERVISOR_CACHE_DIR, supervisor_version)
         supervisor_zip_path = FileUtils.join_paths(supervisor_path, asset_name)
         try:
-            # The file must exist and be more that 1MB 
+            # The file must exist and be more that 1MB
             if os.path.isfile(supervisor_zip_path) and os.path.getsize(supervisor_zip_path) > 1048576:
                 return True, supervisor_zip_path
             elif not os.path.exists(supervisor_path):
                 os.makedirs(supervisor_path)
         except Exception as ex:
             logger.warning('Error checking asset file in cache: %s' % ex)
         return False, supervisor_zip_path
```

### Comparing `scar-4.3.0/scar/version.py` & `scar-4.3.1/scar/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '4.3.0'
+__version__ = '4.3.1'
```

### Comparing `scar-4.3.0/scar.egg-info/SOURCES.txt` & `scar-4.3.1/scar.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 docs/source/conf.py
 examples/mask-detector-workflow/blurry-faces/src/DetectorAPI.py
 examples/mask-detector-workflow/blurry-faces/src/auto_blur_image.py
 examples/mask-detector-workflow/blurry-faces/src/auto_blur_video.py
 examples/mask-detector-workflow/blurry-faces/src/manual_blur_image.py
```

### Comparing `scar-4.3.0/setup.py` & `scar-4.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, find_namespace_packages
+from scar.version import __version__
+
 
 # Load readme
 with open('README.md', mode='r', encoding='utf-8') as f:
     readme = f.read()
 
-# Load version
-with open('scar/version.py', mode='r', encoding='utf-8')  as f:
-    exec(f.read())
-
 setup(name='scar',
       version=__version__,
       description='CLI for deploying serverless infrastructures on multiple cloud environments',
       long_description=readme,
-      long_description_content_type='text/markdown',      
+      long_description_content_type='text/markdown',
       url='https://github.com/grycap/scar',
       author='GRyCAP - Universitat Politecnica de Valencia',
       author_email='products@grycap.upv.es',
       license='Apache 2.0',
       packages=find_namespace_packages(),
       install_requires=['setuptools >= 40.8.0',
                         'boto3',
@@ -46,9 +44,9 @@
       entry_points={
           'console_scripts': [
               'scar=scar.scarcli:main'
           ]
       },
       classifiers=['Programming Language :: Python :: 3',
                    'License :: OSI Approved :: Apache Software License'
-      ]      
+      ]
     )
```

### Comparing `scar-4.3.0/test/functional/aws.py` & `scar-4.3.1/test/functional/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,104 +14,105 @@
 
 import json
 import os
 import subprocess
 import unittest
 
 class AwsTest(unittest.TestCase):
-    
+
     scar_base_path = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
     scar_bin = ["scar"]
-    
+
     def tearDown(self):
         self.execute_command(self.get_cmd(["rm","-a"]))
-    
-    def execute_command(self, cmd):
+
+    @staticmethod
+    def execute_command(cmd):
         return subprocess.check_output(cmd).decode("utf-8")
-    
+
     def get_cmd(self, extra_args):
         return self.scar_bin + extra_args
-    
+
     def create_function(self, function_name):
         cmd = self.get_cmd(["init","-n", function_name, "-i", "centos:7"])
         cmd_out = self.execute_command(cmd)
         self.assertTrue("Packing udocker files" in cmd_out)
         self.assertTrue("Creating function package." in cmd_out)
         self.assertTrue("Function '{0}' successfully created.".format(function_name) in cmd_out)
         self.assertTrue("Log group '/aws/lambda/{0}' successfully created.".format(function_name) in cmd_out)
-     
+
     def test_empty_ls_table(self):
         cmd = self.get_cmd(["ls"])
         cmd_out = self.execute_command(cmd)
         self.assertEqual(cmd_out, 'NAME    MEMORY    TIME    IMAGE_ID    API_URL\n------  --------  ------  ----------  ---------\n')
-          
+
         cmd = self.get_cmd(["ls", "-j"])
         cmd_out = self.execute_command(cmd)
         self.assertEqual(json.loads(cmd_out), {"Functions": []})
-          
+
         cmd = self.get_cmd(["ls", "-v"])
         cmd_out = self.execute_command(cmd)
-        self.assertEqual(json.loads(cmd_out), {"Functions": []})                 
-                  
+        self.assertEqual(json.loads(cmd_out), {"Functions": []})
+
     def test_init_ls_run_rm_function(self):
         func_name = "scar-test-init-ls-run-rm"
         self.create_function(func_name)
-         
+
         cmd = self.get_cmd(["ls"])
         cmd_out = self.execute_command(cmd)
         self.assertTrue("NAME                        MEMORY    TIME  IMAGE_ID    API_URL" in cmd_out)
         self.assertTrue("------------------------  --------  ------  ----------  ---------" in cmd_out)
-        self.assertTrue("{0}       512     300  centos:7    -".format(func_name) in cmd_out)        
-        
+        self.assertTrue("{0}       512     300  centos:7    -".format(func_name) in cmd_out)
+
         cmd = self.get_cmd(["run", "-n", func_name])
         cmd_out = self.execute_command(cmd)
         self.assertTrue("Request Id:" in cmd_out)
         self.assertTrue("Log Group Name: /aws/lambda/{0}".format(func_name) in cmd_out)
         self.assertTrue("Log Stream Name:" in cmd_out)
-                 
+
         cmd = self.get_cmd(["rm","-n", func_name])
         cmd_out = self.execute_command(cmd)
         self.assertTrue("Log group '/aws/lambda/{0}' successfully deleted".format(func_name) in cmd_out)
         self.assertTrue("Function '{0}' successfully deleted".format(func_name) in cmd_out)
-         
+
     def test_init_ls_rm_function_json(self):
         func_name = "scar-test-init-ls-rm-json"
         self.create_function(func_name)
-        
+
         cmd = self.get_cmd(["ls", "-j"])
         cmd_out = self.execute_command(cmd)
         self.assertEqual(json.loads(cmd_out),
                          {"Functions": [{"Name": func_name,
                                          "Memory": 512,
                                          "Timeout": 300,
                                          "Image_id": "centos:7",
                                          "Api_gateway": "-"}]
                          })
-          
+
         cmd = self.get_cmd(["rm","-n", func_name, "-j"])
         cmd_out = self.execute_command(cmd)
         cw_out, lambda_out, _ = cmd_out.split("\n")
         self.assertTrue(json.loads(cw_out)['CloudWatchOutput']['HTTPStatusCode'], 200)
         self.assertTrue(json.loads(lambda_out)['LambdaOutput']['HTTPStatusCode'], 204)
-         
+
     def test_init_ls_rm_simple_function_verbose(self):
         func_name = "scar-test-init-ls-rm-verbose"
         self.create_function(func_name)
         cmd = self.scar_bin + ["ls", "-v"]
         cmd_out = self.execute_command(cmd)
         output = json.loads(cmd_out)
         self.assertTrue(output['Functions'][0]['FunctionName'], "scar-func-test")
         self.assertTrue(output['Functions'][0]['Handler'], "scar-func-test.lambda_handler")
 
         cmd = self.scar_bin + ["rm","-n", func_name, "-v"]
         cmd_out = self.execute_command(cmd)
         cw_out,lambda_out,_ = cmd_out.split("\n")
         self.assertTrue(json.loads(cw_out)['CloudWatchOutput']['ResponseMetadata']['HTTPStatusCode'], 200)
         self.assertTrue(json.loads(lambda_out)['LambdaOutput']['ResponseMetadata']['HTTPStatusCode'], 204)
-        
+
     def test_init_ls_rm_several_functions(self):
         function_names = ["scar-test-init-ls-rm-mult", "scar-test-init-ls-rm-mult-1", "scar-test-init-ls-rm-mult-2"]
         for function_name in function_names:
             self.create_function(function_name)
 
         cmd = self.get_cmd(["ls"])
         cmd_out = self.execute_command(cmd)
@@ -125,8 +126,7 @@
         cmd_out = self.execute_command(cmd)
         for function_name in function_names:
             self.assertTrue("Log group '/aws/lambda/{0}' successfully deleted".format(function_name) in cmd_out)
             self.assertTrue("Function '{0}' successfully deleted".format(function_name) in cmd_out)
 
 if __name__ == '__main__':
     unittest.main()
-
```

### Comparing `scar-4.3.0/test/functional/parser/fdl.py` & `scar-4.3.1/test/functional/parser/fdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,12 +41,12 @@
         result = FDLParser().parse_yaml('fdl.yaml')
         self.assertEqual(len(result), 2)
         for function in result:
             self.assertTrue(('name' in function) and ('env_vars' in function))
             if function['name'] == 'function1':
                 self.assertEqual(len(function['env_vars'].items()), 8)
             elif function['name'] == 'function2':
-                self.assertEqual(len(function['env_vars'].items()), 5)                
+                self.assertEqual(len(function['env_vars'].items()), 5)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `scar-4.3.0/test/unit/aws/test_apigateway.py` & `scar-4.3.1/test/unit/aws/test_apigateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 import sys
-import os
 from mock import MagicMock
 from mock import patch
 
 sys.path.append("..")
 sys.path.append(".")
 sys.path.append("../..")
```

### Comparing `scar-4.3.0/test/unit/aws/test_batch.py` & `scar-4.3.1/test/unit/aws/test_batch.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/test/unit/aws/test_cloudwatchlogs.py` & `scar-4.3.1/test/unit/aws/test_cloudwatchlogs.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/test/unit/aws/test_controller.py` & `scar-4.3.1/test/unit/aws/test_controller.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/test/unit/aws/test_ecr.py` & `scar-4.3.1/test/unit/aws/test_ecr.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,20 @@
         os.environ["AWS_DEFAULT_REGION"] = "us-east-1"
         unittest.TestCase.__init__(self, *args)
 
     def test_init(self):
         ecr = ECR({})
         self.assertEqual(type(ecr.client.client).__name__, "ECR")
 
-    def _init_mocks(self, call_list):
+    @staticmethod
+    def _init_mocks(call_list):
         session = MagicMock(['client'])
         client = MagicMock(call_list)
         session.client.return_value = client
-        return session   
+        return session
 
     @patch('boto3.Session')
     def test_get_authorization_token(self, boto_session):
         boto_session.return_value = self._init_mocks(['get_authorization_token'])
         ecr = ECR({})
         token = "QVdTOnRva2Vu"
         ecr.client.client.get_authorization_token.return_value = {'authorizationData': [{'authorizationToken': token}]}
```

### Comparing `scar-4.3.0/test/unit/aws/test_iam.py` & `scar-4.3.1/test/unit/aws/test_iam.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/test/unit/aws/test_lambdafunction.py` & `scar-4.3.1/test/unit/aws/test_lambdafunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 class TestLambda(unittest.TestCase):
 
     def __init__(self, *args):
         os.environ["AWS_DEFAULT_REGION"] = "us-east-1"
         unittest.TestCase.__init__(self, *args)
 
-    def _init_mocks(self, call_list):
+    @staticmethod
+    def _init_mocks(call_list):
         session = MagicMock(['client'])
         client = MagicMock(call_list)
         session.client.return_value = client
 
         resource_info = {'lambda': {'name': 'fname',
                                     'runtime': 'python3.7',
                                     'timeout': 300,
```

### Comparing `scar-4.3.0/test/unit/aws/test_resourcegroups.py` & `scar-4.3.1/test/unit/aws/test_resourcegroups.py`

 * *Files identical despite different names*

### Comparing `scar-4.3.0/test/unit/aws/test_s3.py` & `scar-4.3.1/test/unit/aws/test_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,20 @@
     def __init__(self, *args):
         unittest.TestCase.__init__(self, *args)
 
     def test_init(self):
         s3 = S3({})
         self.assertEqual(type(s3.client.client).__name__, "S3")
 
-    def _init_mocks(self, call_list):
+    @staticmethod
+    def _init_mocks(call_list):
         session = MagicMock(['client'])
         client = MagicMock(call_list)
         session.client.return_value = client
-        return session   
+        return session
 
     @patch('boto3.Session')
     def test_create_bucket(self, boto_session):
         boto_session.return_value = self._init_mocks(['get_bucket_location', 'create_bucket'])
         s3 = S3({})
         s3.client.client.get_bucket_location.side_effect = ClientError({'Error': {'Code': 'NoSuchBucket'}}, 'op')
         s3.client.client.create_bucket.return_value = {}
```

### Comparing `scar-4.3.0/test/unit/oscar/test_client.py` & `scar-4.3.1/test/unit/oscar/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 import sys
-import os
 from mock import MagicMock
 from mock import patch
 
 sys.path.append("..")
 sys.path.append(".")
 sys.path.append("../..")
```

### Comparing `scar-4.3.0/test/unit/oscar/test_controller.py` & `scar-4.3.1/test/unit/oscar/test_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         tmpfile.close()
         load_tmp_config_file.return_value = {"functions": {"oscar": [{"my_oscar": {"name": "oname",
                                                                                    "script": tmpfile.name}}]}}
         ocli = MagicMock(['create_service'])
         oscar_client.return_value = ocli
 
         OSCAR('init')
-    
+
         os.unlink(tmpfile.name)
         res = {'name': 'oname', 'script': 'Hello world!',
                'cluster_id': 'my_oscar', 'storage_providers': {}}
         self.assertEqual(ocli.create_service.call_args_list[0][1], res)
 
     @patch('scar.providers.oscar.controller.OSCARClient')
     @patch('scar.providers.aws.controller.FileUtils.load_tmp_config_file')
```

### Comparing `scar-4.3.0/test/unit/test_scarcli.py` & `scar-4.3.1/test/unit/test_scarcli.py`

 * *Files identical despite different names*

