# Comparing `tmp/cerbeyra-api-1.0b0.tar.gz` & `tmp/cerbeyra-api-1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbeyra-api-1.0b0.tar", last modified: Fri Feb  3 14:45:07 2023, max compression
+gzip compressed data, was "cerbeyra-api-1.1b1.tar", last modified: Mon May 22 16:26:14 2023, max compression
```

## Comparing `cerbeyra-api-1.0b0.tar` & `cerbeyra-api-1.1b1.tar`

### file list

```diff
@@ -1,46 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 14:45:07.247517 cerbeyra-api-1.0b0/
--rw-rw-rw-   0        0        0    35821 2023-02-02 16:28:06.000000 cerbeyra-api-1.0b0/LICENSE
--rw-rw-rw-   0        0        0     8504 2023-02-03 14:45:07.248517 cerbeyra-api-1.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     8036 2023-02-03 14:42:31.000000 cerbeyra-api-1.0b0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-03 14:45:06.985915 cerbeyra-api-1.0b0/cerbeyra/
--rw-rw-rw-   0        0        0       85 2023-02-02 16:44:13.000000 cerbeyra-api-1.0b0/cerbeyra/__init__.py
--rw-rw-rw-   0        0        0     1985 2023-02-03 13:15:44.000000 cerbeyra-api-1.0b0/cerbeyra/apis.py
--rw-rw-rw-   0        0        0     6326 2023-02-03 09:29:09.000000 cerbeyra-api-1.0b0/cerbeyra/base.py
--rw-rw-rw-   0        0        0     1570 2023-02-02 16:22:07.000000 cerbeyra-api-1.0b0/cerbeyra/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-03 14:45:06.996622 cerbeyra-api-1.0b0/cerbeyra/src/
--rw-rw-rw-   0        0        0        0 2023-02-02 16:22:07.000000 cerbeyra-api-1.0b0/cerbeyra/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-03 14:45:07.027748 cerbeyra-api-1.0b0/cerbeyra/src/cerbeyra_client/
--rw-rw-rw-   0        0        0       73 2023-02-02 16:44:13.000000 cerbeyra-api-1.0b0/cerbeyra/src/cerbeyra_client/__init__.py
--rw-rw-rw-   0        0        0     4084 2023-02-02 16:44:13.000000 cerbeyra-api-1.0b0/cerbeyra/src/cerbeyra_client/cerbeyra_client.py
--rw-rw-rw-   0        0        0      887 2023-02-02 16:22:18.000000 cerbeyra-api-1.0b0/cerbeyra/src/cerbeyra_client/token.py
-drwxrwxrwx   0        0        0        0 2023-02-03 14:45:07.116029 cerbeyra-api-1.0b0/cerbeyra/src/dto/
--rw-rw-rw-   0        0        0      299 2023-02-02 16:44:13.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-02-03 13:13:53.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/cerbeyra_index.py
--rw-rw-rw-   0        0        0      481 2023-02-03 08:57:49.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/client.py
-drwxrwxrwx   0        0        0        0 2023-02-03 14:45:07.143607 cerbeyra-api-1.0b0/cerbeyra/src/dto/commons/
--rw-rw-rw-   0        0        0      110 2023-02-02 16:44:13.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/commons/__init__.py
--rw-rw-rw-   0        0        0      570 2023-02-02 16:22:18.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/commons/va_item.py
--rw-rw-rw-   0        0        0     3791 2023-02-03 08:51:29.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/commons/va_report.py
-drwxrwxrwx   0        0        0        0 2023-02-03 14:45:07.154821 cerbeyra-api-1.0b0/cerbeyra/src/dto/factories/
--rw-rw-rw-   0        0        0        0 2023-02-02 16:22:07.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/factories/__init__.py
--rw-rw-rw-   0        0        0     3212 2023-02-03 13:17:30.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/factories/factories.py
--rw-rw-rw-   0        0        0     2165 2023-02-03 13:02:58.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/network_report.py
--rw-rw-rw-   0        0        0      660 2023-02-03 09:09:43.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/probe.py
--rw-rw-rw-   0        0        0      704 2023-02-03 09:08:34.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/sensor.py
--rw-rw-rw-   0        0        0      283 2023-02-03 13:16:18.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/ubiqum_index.py
--rw-rw-rw-   0        0        0     2167 2023-02-02 16:44:13.000000 cerbeyra-api-1.0b0/cerbeyra/src/dto/web_report.py
--rw-rw-rw-   0        0        0     2752 2023-02-03 13:10:07.000000 cerbeyra-api-1.0b0/cerbeyra/src/types.py
--rw-rw-rw-   0        0        0      299 2023-02-02 16:22:07.000000 cerbeyra-api-1.0b0/cerbeyra/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-03 14:45:07.216552 cerbeyra-api-1.0b0/cerbeyra_api.egg-info/
--rw-rw-rw-   0        0        0     8504 2023-02-03 14:45:06.000000 cerbeyra-api-1.0b0/cerbeyra_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      996 2023-02-03 14:45:06.000000 cerbeyra-api-1.0b0/cerbeyra_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 14:45:06.000000 cerbeyra-api-1.0b0/cerbeyra_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-02-03 14:45:06.000000 cerbeyra-api-1.0b0/cerbeyra_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-03 14:45:06.000000 cerbeyra-api-1.0b0/cerbeyra_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-03 14:45:05.000000 cerbeyra-api-1.0b0/cerbeyra_api.egg-info/zip-safe
--rw-rw-rw-   0        0        0      564 2023-02-03 14:44:25.000000 cerbeyra-api-1.0b0/pyproject.toml
--rw-rw-rw-   0        0        0      182 2023-02-03 14:45:07.257588 cerbeyra-api-1.0b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-03 14:45:07.240428 cerbeyra-api-1.0b0/test/
--rw-rw-rw-   0        0        0     1745 2023-02-03 09:28:44.000000 cerbeyra-api-1.0b0/test/test.py
--rw-rw-rw-   0        0        0     2281 2023-02-03 13:13:53.000000 cerbeyra-api-1.0b0/test/test2.py
--rw-rw-rw-   0        0        0     1255 2023-02-03 13:22:45.000000 cerbeyra-api-1.0b0/test/test3.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.828089 cerbeyra-api-1.1b1/
+-rw-rw-rw-   0        0        0    35148 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/LICENSE
+-rw-rw-rw-   0        0        0    23317 2023-05-22 16:26:14.829088 cerbeyra-api-1.1b1/PKG-INFO
+-rw-rw-rw-   0        0        0    21896 2023-05-22 16:25:39.000000 cerbeyra-api-1.1b1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.465235 cerbeyra-api-1.1b1/cerbeyra/
+-rw-rw-rw-   0        0        0       49 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/__init__.py
+-rw-rw-rw-   0        0        0     1840 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/apis.py
+-rw-rw-rw-   0        0        0     1514 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.482293 cerbeyra-api-1.1b1/cerbeyra/src/
+-rw-rw-rw-   0        0        0       38 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/__init__.py
+-rw-rw-rw-   0        0        0      133 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/base.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.502973 cerbeyra-api-1.1b1/cerbeyra/src/cerbeyra_client/
+-rw-rw-rw-   0        0        0       72 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/cerbeyra_client/__init__.py
+-rw-rw-rw-   0        0        0     4408 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/cerbeyra_client/cerbeyra_client.py
+-rw-rw-rw-   0        0        0      854 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/cerbeyra_client/token.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.622261 cerbeyra-api-1.1b1/cerbeyra/src/dto/
+-rw-rw-rw-   0        0        0      333 2023-05-22 16:11:52.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/__init__.py
+-rw-rw-rw-   0        0        0      449 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/asset.py
+-rw-rw-rw-   0        0        0     1378 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/cerbeyra_index.py
+-rw-rw-rw-   0        0        0      704 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/client.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.655958 cerbeyra-api-1.1b1/cerbeyra/src/dto/collections/
+-rw-rw-rw-   0        0        0      356 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/collections/__init__.py
+-rw-rw-rw-   0        0        0     1381 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/collections/asset_collection.py
+-rw-rw-rw-   0        0        0     2226 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/collections/host_collection.py
+-rw-rw-rw-   0        0        0     2046 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/collections/result_collection.py
+-rw-rw-rw-   0        0        0     2008 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/collections/vuln_collection.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.693930 cerbeyra-api-1.1b1/cerbeyra/src/dto/commons/
+-rw-rw-rw-   0        0        0      108 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/commons/__init__.py
+-rw-rw-rw-   0        0        0     1729 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/commons/collection.py
+-rw-rw-rw-   0        0        0      465 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/commons/item.py
+-rw-rw-rw-   0        0        0      553 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/commons/va_item.py
+-rw-rw-rw-   0        0        0     3683 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/commons/va_report.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.700940 cerbeyra-api-1.1b1/cerbeyra/src/dto/factories/
+-rw-rw-rw-   0        0        0        0 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/factories/__init__.py
+-rw-rw-rw-   0        0        0     5691 2023-05-22 16:10:18.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/factories/factories.py
+-rw-rw-rw-   0        0        0      478 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/host.py
+-rw-rw-rw-   0        0        0      927 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/network_host_vuln.py
+-rw-rw-rw-   0        0        0     2103 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/network_report.py
+-rw-rw-rw-   0        0        0      981 2023-05-22 08:12:35.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/probe.py
+-rw-rw-rw-   0        0        0     1176 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/scan_results.py
+-rw-rw-rw-   0        0        0     1040 2023-05-22 08:12:41.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/sensor.py
+-rw-rw-rw-   0        0        0      734 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/technical_info.py
+-rw-rw-rw-   0        0        0      839 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/web_host_vuln.py
+-rw-rw-rw-   0        0        0     2100 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/dto/web_report.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.764033 cerbeyra-api-1.1b1/cerbeyra/src/services/
+-rw-rw-rw-   0        0        0      360 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/services/__init__.py
+-rw-rw-rw-   0        0        0     1930 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/services/assets.py
+-rw-rw-rw-   0        0        0     1147 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/services/base.py
+-rw-rw-rw-   0        0        0     2333 2023-05-22 08:05:12.000000 cerbeyra-api-1.1b1/cerbeyra/src/services/iot.py
+-rw-rw-rw-   0        0        0     1193 2023-05-22 16:12:12.000000 cerbeyra-api-1.1b1/cerbeyra/src/services/overall.py
+-rw-rw-rw-   0        0        0      754 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/services/partners.py
+-rw-rw-rw-   0        0        0     3444 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/services/reports.py
+-rw-rw-rw-   0        0        0     3139 2023-05-22 15:49:35.000000 cerbeyra-api-1.1b1/cerbeyra/src/services/scans.py
+-rw-rw-rw-   0        0        0     3128 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/services/vulnerabilities.py
+-rw-rw-rw-   0        0        0     1698 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/src/types.py
+-rw-rw-rw-   0        0        0      289 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/cerbeyra/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.810217 cerbeyra-api-1.1b1/cerbeyra_api.egg-info/
+-rw-rw-rw-   0        0        0    23317 2023-05-22 16:26:14.000000 cerbeyra-api-1.1b1/cerbeyra_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1754 2023-05-22 16:26:14.000000 cerbeyra-api-1.1b1/cerbeyra_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:26:14.000000 cerbeyra-api-1.1b1/cerbeyra_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-22 16:26:14.000000 cerbeyra-api-1.1b1/cerbeyra_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 16:26:14.000000 cerbeyra-api-1.1b1/cerbeyra_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-22 16:26:13.000000 cerbeyra-api-1.1b1/cerbeyra_api.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      910 2023-05-22 16:06:02.000000 cerbeyra-api-1.1b1/pyproject.toml
+-rw-rw-rw-   0        0        0      182 2023-05-22 16:26:14.837464 cerbeyra-api-1.1b1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:14.822093 cerbeyra-api-1.1b1/test/
+-rw-rw-rw-   0        0        0     2069 2023-05-22 07:53:56.000000 cerbeyra-api-1.1b1/test/test.py
+-rw-rw-rw-   0        0        0     1013 2023-05-22 16:09:40.000000 cerbeyra-api-1.1b1/test/test_local.py
```

### Comparing `cerbeyra-api-1.0b0/LICENSE` & `cerbeyra-api-1.1b1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `cerbeyra-api-1.0b0/cerbeyra/apis.py` & `cerbeyra-api-1.1b1/cerbeyra/apis.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,47 @@
-from cerbeyra import BaseApi
-from cerbeyra.src.dto.ubiqum_index import UbiqumIndex
-
-
-class CerbeyraApi(BaseApi):
-    """
-    Encloses a set of functions to make it easier getting resources through the Cerbeyra's APIs.
-    It wraps CerbeyraClient.
-    """
-
-    def __init__(self, username: str, password: str, auto_reconnect=False):
-        """
-        Builds a CerbeyraClient object to be used for negotiating with Cerbeyra.
-
-        :param username: the email for authentication.
-        :param password: the password for authentication.
-        :param auto_reconnect: a boolean indicating whether auto reconnection is needed after token expiration.
-        """
-
-        super().__init__(username, password, "https://areaclienti.cerbeyra.com", auto_reconnect=auto_reconnect)
-
-
-class UbiqumApi(BaseApi):
-    """
-    Encloses a set of functions to make it easier getting resources through the Ubiqum's APIs.
-    It wraps CerbeyraClient.
-    """
-
-    def __init__(self, username: str, password: str, auto_reconnect=False):
-        """
-        Builds a CerbeyraClient object to be used for negotiating with Ubiqum.
-
-        :param username: the email for authentication.
-        :param password: the password for authentication.
-        :param auto_reconnect: a boolean indicating whether auto reconnection is needed after token expiration.
-        """
-
-        super().__init__(username, password, "https://areaclienti.ubiqum.ch", auto_reconnect=auto_reconnect)
-
-    def get_ubiqum_index(self, client_id: int = None):
-        """
-        Gets a CerbeyraIndex object. If client_id is specified, then returns the cerbeyra index of specific clients.
-        Otherwise, returns the cerbeyra index of the logged user.
-
-        :param client_id: the unique identifier of a client.
-        :return: a Cerbeyra Index object.
-        """
-        ci = super().get_cerbeyra_index(client_id=client_id)
-        return UbiqumIndex.build_from_index(ci)
+from cerbeyra.src import BaseApi
+
+
+class CerbeyraApi(BaseApi):
+    """
+    Encloses a set of functions to make it easier getting resources through the Cerbeyra's APIs.
+    It wraps CerbeyraClient.
+    """
+
+    def __init__(self, username: str, password: str, auto_reconnect=False):
+        """
+        Builds a CerbeyraClient object to be used for negotiating with Cerbeyra.
+
+        :param username: the email for authentication.
+        :param password: the password for authentication.
+        :param auto_reconnect: a boolean indicating whether auto reconnection is needed after token expiration.
+        """
+
+        super().__init__(username, password, "https://areaclienti.cerbeyra.com", auto_reconnect=auto_reconnect)
+
+
+class UbiqumApi(BaseApi):
+    """
+    Encloses a set of functions to make it easier getting resources through the Ubiqum's APIs.
+    It wraps CerbeyraClient.
+    """
+
+    def __init__(self, username: str, password: str, auto_reconnect=False):
+        """
+        Builds a CerbeyraClient object to be used for negotiating with Ubiqum.
+
+        :param username: the email for authentication.
+        :param password: the password for authentication.
+        :param auto_reconnect: a boolean indicating whether auto reconnection is needed after token expiration.
+        """
+
+        super().__init__(username, password, "https://areaclienti.ubiqum.ch", auto_reconnect=auto_reconnect)
+
+    def get_ubiqum_index(self, client_id: int = None):
+        """
+        Gets a CerbeyraIndex object. If client_id is specified, then returns the cerbeyra index of specific clients.
+        Otherwise, returns the cerbeyra index of the logged user.
+
+        :param client_id: the unique identifier of a client.
+        :return: a Cerbeyra Index object.
+        """
+        return super().get_cerbeyra_index(client_id=client_id)
```

### Comparing `cerbeyra-api-1.0b0/cerbeyra/exceptions.py` & `cerbeyra-api-1.1b1/cerbeyra/exceptions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-class APIException(Exception):
-    """
-    Raised when something goes wrong during an API response handling.
-    """
-    message: str = "Generic HTTP Api Error"
-    code: int = 500
-
-    def __init__(self, status_code: int = None, message: str = None):
-        if message:
-            self.message = message
-        if status_code:
-            self.code = status_code
-
-    def __str__(self):
-        return f'The API request ended with an error (status code={str(self.code)}): {self.message})'
-
-
-class InvalidCredentialsException(APIException):
-    code = 401
-
-
-class ExpiredTokenException(APIException):
-    code = 401
-
-
-def raise_exception_from_response(response):
-    if response.status_code == UnauthenticatedApiException.code:
-        raise UnauthenticatedApiException()
-    if response.status_code == UnauthorizedApiException.code:
-        raise UnauthorizedApiException()
-    if response.status_code == NotFoundApiException.code:
-        raise NotFoundApiException()
-    if response.status_code == RateLimitExceededException.code:
-        raise RateLimitExceededException()
-    try:
-        msg = response.json()['error']
-        raise APIException(response.status_code, msg)
-    except KeyError:
-        pass
-    raise APIException(response.status_code)
-
-
-class UnauthenticatedApiException(APIException):
-    code = 401
-
-
-class UnauthorizedApiException(APIException):
-    code = 403
-
-
-class NotFoundApiException(APIException):
-    code = 404
-
-
-class RateLimitExceededException(APIException):
-    code = 429
+class APIException(Exception):
+    """
+    Raised when something goes wrong during an API response handling.
+    """
+    message: str = "Generic HTTP Api Error"
+    code: int = 500
+
+    def __init__(self, status_code: int = None, message: str = None):
+        if message:
+            self.message = message
+        if status_code:
+            self.code = status_code
+
+    def __str__(self):
+        return f'The API request ended with an error (status code={str(self.code)}): {self.message})'
+
+
+class InvalidCredentialsException(APIException):
+    code = 401
+
+
+class ExpiredTokenException(APIException):
+    code = 401
+
+
+def raise_exception_from_response(response):
+    if response.status_code == UnauthenticatedApiException.code:
+        raise UnauthenticatedApiException()
+    if response.status_code == UnauthorizedApiException.code:
+        raise UnauthorizedApiException()
+    if response.status_code == NotFoundApiException.code:
+        raise NotFoundApiException()
+    if response.status_code == RateLimitExceededException.code:
+        raise RateLimitExceededException()
+    try:
+        msg = response.json()['error']
+        raise APIException(response.status_code, msg)
+    except KeyError:
+        pass
+    raise APIException(response.status_code)
+
+
+class UnauthenticatedApiException(APIException):
+    code = 401
+
+
+class UnauthorizedApiException(APIException):
+    code = 403
+
+
+class NotFoundApiException(APIException):
+    code = 404
+
+
+class RateLimitExceededException(APIException):
+    code = 429
```

### Comparing `cerbeyra-api-1.0b0/cerbeyra/src/cerbeyra_client/cerbeyra_client.py` & `cerbeyra-api-1.1b1/cerbeyra/src/cerbeyra_client/cerbeyra_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,104 @@
-from enum import Enum
-
-import requests
-
-from cerbeyra.exceptions import raise_exception_from_response, InvalidCredentialsException, ExpiredTokenException
-from cerbeyra.src.cerbeyra_client.token import build_token_from_response, Token
-from cerbeyra.src.types import APIurls
-
-
-class _ApiRequestMethod(Enum):
-    GET = 'get'
-    POST = 'post'
-
-
-class CerbeyraClient:
-    """
-    A high-level representation of a session with the Cerbeyra platform. It provides an easy interface to simplify
-    the authentication process and takes care of sending HTTP request and getting responses.
-    """
-    def __init__(self, username: str, password: str, endpoint: str, auto_reconnect=False):
-        """
-        Creates a new CerbeyraClient.
-
-        :param username: the email to be used for authentication.
-        :param password: the password to be used for authentication.
-        :param endpoint: the endpoint exposing Cerbeyra's API.
-        :param auto_reconnect: a boolean indicating whether auto reconnection is needed after token expiration.
-        """
-        self.username = username
-        self.password = password
-        if endpoint.endswith('/'):
-            endpoint = endpoint[:-1]
-        self.endpoint = endpoint
-        self.auto_reconnect = auto_reconnect
-        self.__token: Token | None = None
-
-    def login(self):
-        """
-        Requests an access token. The token will be automatically used for API calls when needed.
-        If credentials are invalid, then raises an InvalidCredentialsExceptions.
-        """
-        if self.__token:
-            if self.__token.is_valid():
-                return
-            elif not self.auto_reconnect:
-                raise ExpiredTokenException()
-        uri = f"{self.endpoint}{APIurls.login.value}"
-
-        res = requests.post(uri, params=dict(email=self.username, password=self.password))
-        if res.ok:
-            self.__token = build_token_from_response(res.json())
-            print(f'Successfully connected to {self.endpoint}')
-            return
-        raise InvalidCredentialsException()
-
-    def get(self, api: str, params: dict = None, stream=False):
-        """
-        Sends an HTTP GET request to an API's endpoint. If params is specified, then the corresponding key-value
-        pairs will be used to for constructing the URL's query string. Additionally, the stream parameter can be
-        set to request the raw socket response. It is built on top of the requests library.
-
-        :param api: the API endpoint.
-        :param params: key-value pairs to be added at the URL's query string.
-        :param stream: a boolean indicating whether request row socket response.
-        :return: a request.models.Response object.
-        """
-        return self.request('get', api, params=params, stream=stream)
-
-    def post(self, api: str, params: dict = None, stream=False):
-        """
-        Sends an HTTP POST request to an API's endpoint. If params is specified, then the corresponding key-value
-        pairs will be used to for constructing the URL's query string. Additionally, the stream parameter can be
-        set to request the raw socket response. It is built on top of the requests library.
-
-        :param api: the API endpoint.
-        :param params: key-value pairs to be added at the URL's query string.
-        :param stream: a boolean indicating whether request row socket response.
-        :return: a request.models.Response object.
-        """
-        return self.request('post', api, params=params, stream=stream)
-
-    def request(self, method: str, api: str, params: dict = None, stream=False):
-        assert _ApiRequestMethod(method)
-        self.login()
-
-        uri = f"{self.endpoint}{api}"
-        headers = {'Authorization': self.__token.get_authorization_header()}
-        response = requests.request(str(method), uri, headers=headers, params=params, stream=stream)
-        if response.ok:
-            return response
-
-        return raise_exception_from_response(response)
+from enum import Enum
+
+import requests
+
+from cerbeyra.exceptions import raise_exception_from_response, InvalidCredentialsException, ExpiredTokenException
+from cerbeyra.src.cerbeyra_client.token import build_token_from_response, Token
+
+
+class _ApiRequestMethod(Enum):
+    GET = 'get'
+    POST = 'post'
+
+
+class CerbeyraClient:
+    __login_uri = 'login'
+
+    """
+    A high-level representation of a session with the Cerbeyra platform. It provides an easy interface to simplify
+    the authentication process and takes care of sending HTTP request and getting responses.
+    """
+
+    def __init__(self, username: str, password: str, endpoint: str, auto_reconnect=False, base_uri: str = '/api/'):
+        """
+        Creates a new CerbeyraClient.
+
+        :param username: the email to be used for authentication.
+        :param password: the password to be used for authentication.
+        :param endpoint: the endpoint exposing Cerbeyra's API.
+        :param auto_reconnect: a boolean indicating whether auto reconnection is needed after token expiration.
+        :param base_uri: str
+        """
+        self.username = username
+        self.password = password
+        if endpoint.endswith('/'):
+            endpoint = endpoint[:-1]
+        endpoint += base_uri
+        self.endpoint = endpoint
+        self.auto_reconnect = auto_reconnect
+        self.__token: Token | None = None
+
+    def login(self):
+        """
+        Requests an access token. The token will be automatically used for API calls when needed.
+        If credentials are invalid, then raises an InvalidCredentialsExceptions.
+        """
+        if self.__token:
+            if self.__token.is_valid():
+                return
+            elif not self.auto_reconnect:
+                raise ExpiredTokenException()
+        uri = f"{self.endpoint}{self.__login_uri}"
+
+        res = requests.post(uri, params=dict(email=self.username, password=self.password))
+        if res.ok:
+            self.__token = build_token_from_response(res.json())
+            print(f'Successfully connected to {self.endpoint}')
+            return
+        raise InvalidCredentialsException()
+
+    def get(self, api: str, params: dict = None, stream=False, client_id=None):
+        """
+        Sends an HTTP GET request to an API's endpoint. If params is specified, then the corresponding key-value
+        pairs will be used to for constructing the URL's query string. Additionally, the stream parameter can be
+        set to request the raw socket response. It is built on top of the requests library.
+
+        :param client_id:
+        :param api: the API endpoint.
+        :param params: key-value pairs to be added at the URL's query string.
+        :param stream: a boolean indicating whether request row socket response.
+        :return: a request.models.Response object.
+        """
+        return self.request('get', api, params=params, stream=stream, client_id=client_id)
+
+    def post(self, api: str, params: dict = None, stream=False, client_id=None):
+        """
+        Sends an HTTP POST request to an API's endpoint. If params is specified, then the corresponding key-value
+        pairs will be used to for constructing the URL's query string. Additionally, the stream parameter can be
+        set to request the raw socket response. It is built on top of the requests library.
+
+        :param client_id:
+        :param api: the API endpoint.
+        :param params: key-value pairs to be added at the URL's query string.
+        :param stream: a boolean indicating whether request row socket response.
+        :return: a request.models.Response object.
+        """
+        return self.request('post', api, params=params, stream=stream, client_id=client_id)
+
+    def request(self, method: str, api: str, params: dict = None, stream=False, client_id=None):
+        assert _ApiRequestMethod(method)
+        self.login()
+        uri = self.__build_uri(api, client_id)
+        headers = {'Authorization': self.__token.get_authorization_header()}
+        response = requests.request(str(method), uri, headers=headers, params=params, stream=stream)
+        if response.ok:
+            return response
+
+        return raise_exception_from_response(response)
+
+    def __build_uri(self, api, client_id=None):
+        uri = f"{self.endpoint}"
+        if client_id is not None:
+            uri += f"clients/{client_id}/"
+        uri += api
+        return uri
```

### Comparing `cerbeyra-api-1.0b0/cerbeyra/src/cerbeyra_client/token.py` & `cerbeyra-api-1.1b1/cerbeyra/src/cerbeyra_client/token.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from datetime import datetime, timedelta
-
-
-class Token:
-    """
-    Defines a Token object.
-    """
-
-    def __init__(self, token: str, expire_time: float):
-        self.token = token
-        self.expire_on = datetime.now() + timedelta(seconds=expire_time)
-
-    def get_authorization_header(self):
-        """
-        Builds the header which is needed to access Cerbeyra's resources.
-
-        :return: a dictionary containing the header.
-        """
-        if self.token:
-            return f'Bearer {self.token}'
-        return None
-
-    def is_valid(self):
-        if self.token is None:
-            return False
-        if self.expire_on < datetime.now():
-            self.token = None
-            return False
-        return True
-
-
-def build_token_from_response(res_json) -> Token:
-    return Token(res_json['access_token'], res_json['expires_in'])
+from datetime import datetime, timedelta
+
+
+class Token:
+    """
+    Defines a Token object.
+    """
+
+    def __init__(self, token: str, expire_time: float):
+        self.token = token
+        self.expire_on = datetime.now() + timedelta(seconds=expire_time)
+
+    def get_authorization_header(self):
+        """
+        Builds the header which is needed to access Cerbeyra's resources.
+
+        :return: a dictionary containing the header.
+        """
+        if self.token:
+            return f'Bearer {self.token}'
+        return None
+
+    def is_valid(self):
+        if self.token is None:
+            return False
+        if self.expire_on < datetime.now():
+            self.token = None
+            return False
+        return True
+
+
+def build_token_from_response(res_json) -> Token:
+    return Token(res_json['access_token'], res_json['expires_in'])
```

### Comparing `cerbeyra-api-1.0b0/cerbeyra/src/dto/cerbeyra_index.py` & `cerbeyra-api-1.1b1/cerbeyra/src/dto/cerbeyra_index.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-from dataclasses import dataclass
-
-
-@dataclass
-class CerbeyraIndex:
-    index: str
-    risk_level: str
-    explain: dict
-
-    __ci_order = ['A+++', 'A++', 'A+', 'A', 'B', 'C', 'D', 'E', 'F', 'G']
-
-    def __str__(self):
-        """
-        Defines the string representation for the CerbeyraIndex object.
-
-        :return: the string representation.
-        """
-        return self.index
-
-    def __eq__(self, other):
-        """
-        Makes it possible to verify the equality of two CerbeyraIndex object (based on the cerbeyra_index attribute).
-
-        :param other: another CerbeyraIndex object
-        :return: a boolean
-        """
-        return self.index == other.index
-
-    def __gt__(self, other):
-        """
-        Makes it possible to verify whether a CerbeyraIndex object is greater than another
-        (based on the cerbeyra_index attribute).
-
-        :param other: another CerbeyraIndex object
-        :return: a boolean
-        """
-        obj_index = self.__ci_order.index(self.index)
-        other_index = self.__ci_order.index(other.index)
-        return obj_index < other_index
+from dataclasses import dataclass, fields
+
+
+@dataclass(kw_only=True)
+class CerbeyraIndex:
+    index: str
+    risk_level: str
+    explain: dict
+
+    __ci_order = ['A+++', 'A++', 'A+', 'A', 'B', 'C', 'D', 'E', 'F', 'G']
+
+    def __init__(self, **kwargs):
+        [setattr(self, k, v) for k, v in kwargs.items() if k in self.fields]
+
+    def __str__(self):
+        """
+        Defines the string representation for the CerbeyraIndex object.
+
+        :return: the string representation.
+        """
+        return f"<Index ({self.index}) risk={self.risk_level}>"
+
+    def __eq__(self, other):
+        """
+        Makes it possible to verify the equality of two CerbeyraIndex object (based on the cerbeyra_index attribute).
+
+        :param other: another CerbeyraIndex object
+        :return: a boolean
+        """
+        return self.index == other.index
+
+    def __gt__(self, other):
+        """
+        Makes it possible to verify whether a CerbeyraIndex object is greater than another
+        (based on the cerbeyra_index attribute).
+
+        :param other: another CerbeyraIndex object
+        :return: a boolean
+        """
+        obj_index = self.__ci_order.index(self.index)
+        other_index = self.__ci_order.index(other.index)
+        return obj_index < other_index
+
+    @property
+    def fields(self) -> list[str]:
+        return [field.name for field in fields(self)]
```

### Comparing `cerbeyra-api-1.0b0/cerbeyra/src/dto/commons/va_item.py` & `cerbeyra-api-1.1b1/cerbeyra/src/dto/commons/va_item.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-class VAItem(dict):
-    """
-    Extends dict to represent a Vulnerability Assessment item.
-    Both Network and Web report consist of VAItem.
-    """
-    def get_field(self, name: str) -> str | None:
-        """
-        Gets the field value for a specific report's field name. In case the field name is not
-        among the available keys, raises a KeyError.
-
-        :param name: the field name to retrieve.
-        :return: a report field value.
-        """
-        try:
-            return self[name]
-        except KeyError:
-            return None
+class VAItem(dict):
+    """
+    Extends dict to represent a Vulnerability Assessment item.
+    Both Network and Web report consist of VAItem.
+    """
+    def get_field(self, name: str) -> str | None:
+        """
+        Gets the field value for a specific report's field name. In case the field name is not
+        among the available keys, raises a KeyError.
+
+        :param name: the field name to retrieve.
+        :return: a report field value.
+        """
+        try:
+            return self[name]
+        except KeyError:
+            return None
```

### Comparing `cerbeyra-api-1.0b0/cerbeyra/src/dto/commons/va_report.py` & `cerbeyra-api-1.1b1/cerbeyra/src/dto/commons/va_report.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,106 @@
-import csv
-import uuid
-import shutil
-import openpyxl
-from typing import Generator, Any, Set, List, Dict
-
-from cerbeyra.src.dto.commons.va_item import VAItem
-from cerbeyra.src.dto.factories.factories import VaItemFactory
-
-
-class VAReport:
-    """
-    This super class defines a vulnerability assessment report object.
-    """
-
-    def __init__(self, csv_file_path: str, queried_fields: list):
-        self.csv_file_path = csv_file_path
-        self.queried_fields = queried_fields
-
-    def iterate_entries(self) -> Generator[VAItem, Any, None]:
-        """
-        Reads the report file specified in 'csv_file_path' and returns a generator over report entries.
-
-        :return: a Generator of VaItem objects.
-        """
-        idx_entry = 0
-        with open(self.csv_file_path, 'r') as f:
-            report_entries = csv.reader(f, delimiter=',')
-            for entry in report_entries:
-                if idx_entry > 0:
-                    yield VaItemFactory.build_from_row(self.queried_fields, entry)
-                idx_entry += 1
-
-    def _get_distinct_field(self, field: str) -> Set[str]:
-        """
-        Gets a set of items belonging to specific fields.
-
-        :param field: the queried report field.
-        :return: a set of value associated to the queried field.
-        """
-        return set(self._get_field(field))
-
-    def _get_field(self, field: str) -> List[str]:
-        """
-        Gets a list of all items belonging to specific fields.
-
-        :param field: the queried fields.
-        :return: a list of report values.
-        """
-        return [item.get_field(field) for item in self.iterate_entries()]
-
-    def _group_by_field(self, field: str) -> Dict[str, List[VAItem]]:
-        """
-        Groups the report items by specific field.
-
-        :param field: the queried field.
-        :return: a dictionary containing the grouped items.
-        """
-        grouped_by_entries = dict()
-        for item in self.iterate_entries():
-            field_value = item.get_field(field)
-            if field_value not in grouped_by_entries.keys():
-                grouped_by_entries[field_value] = list()
-            grouped_by_entries[field_value].append(item)
-        return grouped_by_entries
-
-    def _count_by_field(self, field: str) -> Dict[str, int]:
-        """
-        Counts report items by specific field.
-
-        :param field: the queried field.
-        :return: a dictionary containing the counts.
-        """
-        grouped_entries = self._group_by_field(field)
-        return {k: len(v) for k, v in grouped_entries.items()}
-
-    def save_csv(self, path=None):
-        """
-        Saves report as .csv file. If the saving path is not specified, then a universally unique identifier
-        will be used as file name.
-
-        :param path: the file saving location.
-        """
-        if not path:
-            path = f"{uuid.uuid4()}.csv"
-        shutil.copy(self.csv_file_path, path)
-
-    def save_xls(self, path=None):
-        """
-        Saves report as .xlsx file. If the saving path is not specified, then a universally unique identifier
-        will be used as file name.
-
-        :param path: the file saving location.
-        """
-        if not path:
-            path = f"{uuid.uuid4()}.xlsx"
-        work_book = openpyxl.Workbook()
-        work_sheet = work_book.active
-        work_sheet.append(self.queried_fields)
-        with open(self.csv_file_path, 'r') as f:
-            report_entries = csv.reader(f, delimiter=',')
-            idx_entry = 0
-            for entry in report_entries:
-                if idx_entry > 0:
-                    work_sheet.append(entry)
-                idx_entry += 1
-            work_book.save(path)
+import csv
+import uuid
+import shutil
+import openpyxl
+from typing import Generator, Any, Set, List, Dict
+from cerbeyra.src.dto.commons.va_item import VAItem
+from cerbeyra.src.dto.factories.factories import VaItemFactory
+
+
+class VAReport:
+    """
+    This super class defines a vulnerability assessment report object.
+    """
+
+    def __init__(self, csv_file_path: str, queried_fields: list):
+        self.csv_file_path = csv_file_path
+        self.queried_fields = queried_fields
+
+    def iterate_entries(self) -> Generator[VAItem, Any, None]:
+        """
+        Reads the report file specified in 'csv_file_path' and returns a generator over report entries.
+
+        :return: a Generator of VaItem objects.
+        """
+        idx_entry = 0
+        with open(self.csv_file_path, 'r') as f:
+            report_entries = csv.reader(f, delimiter=',')
+            for entry in report_entries:
+                if idx_entry > 0:
+                    yield VaItemFactory.build_from_row(self.queried_fields, entry)
+                idx_entry += 1
+
+    def _get_distinct_field(self, field: str) -> Set[str]:
+        """
+        Gets a set of items belonging to specific fields.
+
+        :param field: the queried report field.
+        :return: a set of value associated to the queried field.
+        """
+        return set(self._get_field(field))
+
+    def _get_field(self, field: str) -> List[str]:
+        """
+        Gets a list of all items belonging to specific fields.
+
+        :param field: the queried fields.
+        :return: a list of report values.
+        """
+        return [item.get_field(field) for item in self.iterate_entries()]
+
+    def _group_by_field(self, field: str) -> Dict[str, List[VAItem]]:
+        """
+        Groups the report items by specific field.
+
+        :param field: the queried field.
+        :return: a dictionary containing the grouped items.
+        """
+        grouped_by_entries = dict()
+        for item in self.iterate_entries():
+            field_value = item.get_field(field)
+            if field_value not in grouped_by_entries.keys():
+                grouped_by_entries[field_value] = list()
+            grouped_by_entries[field_value].append(item)
+        return grouped_by_entries
+
+    def _count_by_field(self, field: str) -> Dict[str, int]:
+        """
+        Counts report items by specific field.
+
+        :param field: the queried field.
+        :return: a dictionary containing the counts.
+        """
+        grouped_entries = self._group_by_field(field)
+        return {k: len(v) for k, v in grouped_entries.items()}
+
+    def save_csv(self, path=None):
+        """
+        Saves report as .csv file. If the saving path is not specified, then a universally unique identifier
+        will be used as file name.
+
+        :param path: the file saving location.
+        """
+        if not path:
+            path = f"{uuid.uuid4()}.csv"
+        shutil.copy(self.csv_file_path, path)
+
+    def save_xls(self, path=None):
+        """
+        Saves report as .xlsx file. If the saving path is not specified, then a universally unique identifier
+        will be used as file name.
+
+        :param path: the file saving location.
+        """
+        if not path:
+            path = f"{uuid.uuid4()}.xlsx"
+        work_book = openpyxl.Workbook()
+        work_sheet = work_book.active
+        work_sheet.append(self.queried_fields)
+        with open(self.csv_file_path, 'r') as f:
+            report_entries = csv.reader(f, delimiter=',')
+            idx_entry = 0
+            for entry in report_entries:
+                if idx_entry > 0:
+                    work_sheet.append(entry)
+                idx_entry += 1
+            work_book.save(path)
```

### Comparing `cerbeyra-api-1.0b0/cerbeyra/src/dto/network_report.py` & `cerbeyra-api-1.1b1/cerbeyra/src/dto/web_report.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,67 @@
-from typing import Set, Dict, List
-from cerbeyra.src.dto.commons import VAReport, VAItem
-from cerbeyra.src.types import NetworkReportFields
-
-
-class NetworkReport(VAReport):
-    """
-    Defines a NetworkReport object. Contains a set of functions to easily manipulate report entries.
-    It consists of a VAItems list.
-    """
-
-    def __init__(self, csv_file_path, queried_fields):
-        """
-        Makes a NetworkReport object from the corresponding csv file.
-
-        :param csv_file_path: a reference for the csv file location.
-        :param queried_fields: the list of requested network report fields (through URL params).
-        """
-        super().__init__(csv_file_path, queried_fields)
-        self.__check_fields()
-
-    def group_by_threat(self) -> Dict[str, List[VAItem]]:
-        """
-        Groups the report items by threat.
-
-        :return: a dictionary containing the grouped VAItems.
-        """
-        if NetworkReportFields.threat.value not in self.queried_fields:
-            return dict()
-        return super()._group_by_field(field=NetworkReportFields.threat.value)
-
-    def get_distinct_hosts(self) -> Set[str]:
-        """
-        Gets the set of scanned host.
-
-        :return: a set of host.
-        """
-        if NetworkReportFields.host.value not in self.queried_fields:
-            return set()
-        return super()._get_distinct_field(NetworkReportFields.host.value)
-
-    def count_by_threat(self) -> Dict[str, int]:
-        """
-        Counts report items by threat.
-
-        :return: a dictionary containing item counts per threat level.
-        """
-        if NetworkReportFields.threat.value not in self.queried_fields:
-            return dict()
-        return super()._count_by_field(NetworkReportFields.threat.value)
-
-    def __check_fields(self):
-        """
-        Checks whether the queried fields correspond to NetworkReport items.
-
-        :return: None
-        """
-        for queried_field in self.queried_fields:
-            try:
-                NetworkReportFields(queried_field)
-            except ValueError:
-                raise AttributeError
+from typing import Set, Dict, List
+
+from cerbeyra.src.dto.commons import VAReport, VAItem
+from cerbeyra.src.types import WebReportFields
+
+
+class WebReport(VAReport):
+    """
+    Defines a WebReport object. Contains a set of functions to easily manipulate report entries.
+    It consists of a VAItems list.
+    """
+
+    def __init__(self, csv_file_path, queried_fields):
+        super().__init__(csv_file_path, queried_fields)
+        self.__check_fields()
+
+    def group_by_threat(self) -> Dict[str, List[VAItem]]:
+        """
+        Groups the report items by threat.
+
+        :return: a dictionary containing the grouped VAItems.
+        """
+        if WebReportFields.threat.value not in self.queried_fields:
+            return dict()
+        return super()._group_by_field(field=WebReportFields.threat.value)
+
+    def get_distinct_hosts(self) -> Set[str]:
+        """
+        Gets the set of scanned host.
+
+        :return: a set of host.
+        """
+        if WebReportFields.host.value not in self.queried_fields:
+            return set()
+        return super()._get_distinct_field(WebReportFields.host.value)
+
+    def get_distinct_urls(self) -> Set[str]:
+        """
+        Gets the set of scanned urls.
+
+        :return: a set of urls.
+        """
+        if WebReportFields.url.value not in self.queried_fields:
+            return set()
+        return super()._get_distinct_field(WebReportFields.url.value)
+
+    def count_by_threat(self) -> Dict[str, int]:
+        """
+        Counts report items by threat.
+
+        :return: a dictionary containing item counts per threat level.
+        """
+        if WebReportFields.threat.value not in self.queried_fields:
+            return dict()
+        return super()._count_by_field(WebReportFields.threat.value)
+
+    def __check_fields(self):
+        """
+        Checks whether the queried fields correspond to WebReport items.
+
+        :return: None
+        """
+        for queried_field in self.queried_fields:
+            try:
+                WebReportFields(queried_field)
+            except ValueError:
+                raise AttributeError
```

### Comparing `cerbeyra-api-1.0b0/cerbeyra/src/dto/sensor.py` & `cerbeyra-api-1.1b1/cerbeyra/src/dto/probe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-from dataclasses import dataclass
-from cerbeyra.src.dto.client import Client
-from cerbeyra.src.types import IoTStatus
-
-
-@dataclass
-class Sensor:
-    name: str
-    probe_gateway: str
-    status: IoTStatus
-    alarm: str
-    last_update: str
-    client: Client
-    thresholds: list = None
-
-    def __post_init__(self):
-        if self.status is not None:
-            self.status = IoTStatus(self.status)
-
-    def __str__(self):
-        """
-        Defines the string representation for a sensor object containing its name and status.
-
-        :return: the string representation.
-        """
-        return f'[{self.name}] {self.name}: {self.status.value} - Client: {self.client}'
+from dataclasses import dataclass, fields
+from cerbeyra.src.dto.client import Client
+from cerbeyra.src.types import IoTStatus
+
+
+@dataclass(kw_only=True)
+class Probe:
+    name: str
+    probe_id: str
+    status: IoTStatus
+    last_update: str
+    client: Client = None
+
+    def __init__(self, **kwargs):
+        [setattr(self, k, v) for k, v in kwargs.items() if k in self.fields]
+        if self.status is not None:
+            self.status = IoTStatus(self.status)
+
+    def __str__(self):
+        """
+        Defines the string representation for a probe object containing its probe_id and status.
+
+        :return: the string representation.
+        """
+        if self.client:
+            return f'<Probe [{self.probe_id}] {self.name}: {self.status.value} - Client={self.client}>'
+        else:
+            return f'<Probe [{self.probe_id}] {self.name}: {self.status.value}>'
+
+    @property
+    def fields(self) -> list[str]:
+        return [field.name for field in fields(self)]
```

