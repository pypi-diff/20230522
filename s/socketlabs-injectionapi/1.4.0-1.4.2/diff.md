# Comparing `tmp/socketlabs_injectionapi-1.4.0.tar.gz` & `tmp/socketlabs_injectionapi-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketlabs_injectionapi-1.4.0.tar", last modified: Tue Jan 17 16:16:08 2023, max compression
+gzip compressed data, was "socketlabs_injectionapi-1.4.2.tar", last modified: Mon May 22 19:15:56 2023, max compression
```

## Comparing `socketlabs_injectionapi-1.4.0.tar` & `socketlabs_injectionapi-1.4.2.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 16:16:08.853658 socketlabs_injectionapi-1.4.0/
--rw-rw-rw-   0        0        0     2324 2020-07-30 21:06:54.000000 socketlabs_injectionapi-1.4.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1086 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/LICENSE.md
--rw-rw-rw-   0        0        0      109 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    14506 2023-01-17 16:16:08.852662 socketlabs_injectionapi-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    13415 2023-01-12 14:39:04.000000 socketlabs_injectionapi-1.4.0/README.md
--rw-rw-rw-   0        0        0      369 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/app.json
--rw-rw-rw-   0        0        0       42 2023-01-17 16:16:08.853658 socketlabs_injectionapi-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1520 2023-01-17 16:15:51.000000 socketlabs_injectionapi-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-17 16:16:08.630763 socketlabs_injectionapi-1.4.0/socketlabs/
--rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-17 16:16:08.677825 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/
--rw-rw-rw-   0        0        0      142 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/__imports__.py
--rw-rw-rw-   0        0        0       84 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/__init__.py
--rw-rw-rw-   0        0        0     2856 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/addressresult.py
-drwxrwxrwx   0        0        0        0 2023-01-17 16:16:08.716820 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/
--rw-rw-rw-   0        0        0        2 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/__init__.py
--rw-rw-rw-   0        0        0      730 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/httpendpoint.py
--rw-rw-rw-   0        0        0     5655 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/httprequest.py
--rw-rw-rw-   0        0        0     9700 2023-01-17 16:13:27.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/injectionrequestfactory.py
--rw-rw-rw-   0        0        0     3763 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/injectionresponseparser.py
--rw-rw-rw-   0        0        0     2944 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/retryhandler.py
--rw-rw-rw-   0        0        0    12976 2023-01-12 14:19:37.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/sendvalidator.py
-drwxrwxrwx   0        0        0        0 2023-01-17 16:16:08.776755 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/
--rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/__init__.py
--rw-rw-rw-   0        0        0     1955 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/addressjson.py
--rw-rw-rw-   0        0        0     3541 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/attachmentjson.py
--rw-rw-rw-   0        0        0     1570 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/customheaderjson.py
--rw-rw-rw-   0        0        0     1868 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/injectionrequest.py
--rw-rw-rw-   0        0        0     2776 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/injectionresponsedto.py
--rw-rw-rw-   0        0        0     2801 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/mergedatajson.py
--rw-rw-rw-   0        0        0     1560 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/mergefieldjson.py
--rw-rw-rw-   0        0        0    13585 2023-01-12 17:31:50.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/messagejson.py
--rw-rw-rw-   0        0        0     2306 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/messageresultdto.py
--rw-rw-rw-   0        0        0     1479 2023-01-16 15:09:36.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/metadatajson.py
--rw-rw-rw-   0        0        0     1756 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/stringextension.py
-drwxrwxrwx   0        0        0        0 2023-01-17 16:16:08.832784 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/
--rw-rw-rw-   0        0        0      304 2023-01-12 14:30:01.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/__imports__.py
--rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/__init__.py
--rw-rw-rw-   0        0        0     7486 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/attachment.py
--rw-rw-rw-   0        0        0    15482 2023-01-12 15:08:54.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/basicmessage.py
--rw-rw-rw-   0        0        0    14105 2023-01-12 15:26:17.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/bulkmessage.py
--rw-rw-rw-   0        0        0     3277 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/bulkrecipient.py
--rw-rw-rw-   0        0        0     1991 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/customheader.py
--rw-rw-rw-   0        0        0     2168 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/emailaddress.py
--rw-rw-rw-   0        0        0     6322 2020-07-30 21:06:54.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/messagebase.py
--rw-rw-rw-   0        0        0     1936 2023-01-16 15:10:41.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/metadata.py
--rw-rw-rw-   0        0        0     1364 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/proxy.py
--rw-rw-rw-   0        0        0     1594 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/retrysettings.py
--rw-rw-rw-   0        0        0     4248 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/sendresponse.py
--rw-rw-rw-   0        0        0     7080 2023-01-12 14:17:46.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/sendresult.py
--rw-rw-rw-   0        0        0    10045 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/socketlabsclient.py
--rw-rw-rw-   0        0        0       80 2023-01-12 14:44:09.000000 socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/version.py
-drwxrwxrwx   0        0        0        0 2023-01-17 16:16:08.850698 socketlabs_injectionapi-1.4.0/socketlabs_injectionapi.egg-info/
--rw-rw-rw-   0        0        0    14506 2023-01-17 16:16:08.000000 socketlabs_injectionapi-1.4.0/socketlabs_injectionapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2141 2023-01-17 16:16:08.000000 socketlabs_injectionapi-1.4.0/socketlabs_injectionapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-17 16:16:08.000000 socketlabs_injectionapi-1.4.0/socketlabs_injectionapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-01-17 16:16:08.000000 socketlabs_injectionapi-1.4.0/socketlabs_injectionapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:56.993897 socketlabs_injectionapi-1.4.2/
+-rw-rw-rw-   0        0        0     2324 2020-07-30 21:06:54.000000 socketlabs_injectionapi-1.4.2/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1086 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/LICENSE.md
+-rw-rw-rw-   0        0        0      109 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    14553 2023-05-22 19:15:56.992939 socketlabs_injectionapi-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13462 2023-05-22 19:06:11.000000 socketlabs_injectionapi-1.4.2/README.md
+-rw-rw-rw-   0        0        0      369 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/app.json
+-rw-rw-rw-   0        0        0       42 2023-05-22 19:15:56.993897 socketlabs_injectionapi-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1520 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:56.777422 socketlabs_injectionapi-1.4.2/socketlabs/
+-rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:56.822143 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/
+-rw-rw-rw-   0        0        0      142 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/__imports__.py
+-rw-rw-rw-   0        0        0       84 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/__init__.py
+-rw-rw-rw-   0        0        0     2856 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/addressresult.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:56.857883 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/
+-rw-rw-rw-   0        0        0        2 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/__init__.py
+-rw-rw-rw-   0        0        0     1552 2023-05-22 19:06:05.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/apikeyparser.py
+-rw-rw-rw-   0        0        0     1669 2023-05-22 19:11:14.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/apikeyparseresult.py
+-rw-rw-rw-   0        0        0      730 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/httpendpoint.py
+-rw-rw-rw-   0        0        0     5953 2023-05-22 19:06:08.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/httprequest.py
+-rw-rw-rw-   0        0        0     9700 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/injectionrequestfactory.py
+-rw-rw-rw-   0        0        0     3769 2023-05-22 19:06:08.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/injectionresponseparser.py
+-rw-rw-rw-   0        0        0     2944 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/retryhandler.py
+-rw-rw-rw-   0        0        0    12976 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/sendvalidator.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:56.926340 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/
+-rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/__init__.py
+-rw-rw-rw-   0        0        0     1955 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/addressjson.py
+-rw-rw-rw-   0        0        0     3541 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/attachmentjson.py
+-rw-rw-rw-   0        0        0     1570 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/customheaderjson.py
+-rw-rw-rw-   0        0        0     1868 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/injectionrequest.py
+-rw-rw-rw-   0        0        0     2776 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/injectionresponsedto.py
+-rw-rw-rw-   0        0        0     2801 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/mergedatajson.py
+-rw-rw-rw-   0        0        0     1560 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/mergefieldjson.py
+-rw-rw-rw-   0        0        0    13585 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/messagejson.py
+-rw-rw-rw-   0        0        0     2306 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/messageresultdto.py
+-rw-rw-rw-   0        0        0     1479 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/metadatajson.py
+-rw-rw-rw-   0        0        0     1756 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/stringextension.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:56.967895 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/
+-rw-rw-rw-   0        0        0      304 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/__imports__.py
+-rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/__init__.py
+-rw-rw-rw-   0        0        0     7486 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/attachment.py
+-rw-rw-rw-   0        0        0    15482 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/basicmessage.py
+-rw-rw-rw-   0        0        0    14105 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/bulkmessage.py
+-rw-rw-rw-   0        0        0     3277 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/bulkrecipient.py
+-rw-rw-rw-   0        0        0     1991 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/customheader.py
+-rw-rw-rw-   0        0        0     2168 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/emailaddress.py
+-rw-rw-rw-   0        0        0     6322 2020-07-30 21:06:54.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/messagebase.py
+-rw-rw-rw-   0        0        0     1936 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/metadata.py
+-rw-rw-rw-   0        0        0     1364 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/proxy.py
+-rw-rw-rw-   0        0        0     1594 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/retrysettings.py
+-rw-rw-rw-   0        0        0     4248 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/sendresponse.py
+-rw-rw-rw-   0        0        0     7080 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/sendresult.py
+-rw-rw-rw-   0        0        0    10977 2023-05-22 19:06:05.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/socketlabsclient.py
+-rw-rw-rw-   0        0        0       80 2023-05-22 19:06:28.000000 socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/version.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:56.991896 socketlabs_injectionapi-1.4.2/socketlabs_injectionapi.egg-info/
+-rw-rw-rw-   0        0        0    14553 2023-05-22 19:15:56.000000 socketlabs_injectionapi-1.4.2/socketlabs_injectionapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2236 2023-05-22 19:15:56.000000 socketlabs_injectionapi-1.4.2/socketlabs_injectionapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 19:15:56.000000 socketlabs_injectionapi-1.4.2/socketlabs_injectionapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 19:15:56.000000 socketlabs_injectionapi-1.4.2/socketlabs_injectionapi.egg-info/top_level.txt
```

### Comparing `socketlabs_injectionapi-1.4.0/CONTRIBUTING.md` & `socketlabs_injectionapi-1.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/LICENSE.md` & `socketlabs_injectionapi-1.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/PKG-INFO` & `socketlabs_injectionapi-1.4.2/socketlabs_injectionapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: socketlabs_injectionapi
-Version: 1.4.0
+Name: socketlabs-injectionapi
+Version: 1.4.2
 Summary: SocketLabs Email Delivery Python client library
 Home-page: https://github.com/socketlabs/socketlabs-python
 Author: David Schrenker, Matt Reibach, Ryan Lydzinski, Praneeth Chandra
 Author-email: support@socketlabs.com
 License: MIT
 Project-URL: Organization, https://github.com/socketlabs
 Project-URL: Bug Reports, https://github.com/socketlabs/socketlabs-python/issues
@@ -49,15 +49,15 @@
 ```
 pip install socketlabs-injectionapi
 ```
 ### From a local archive using pip
 
 You can just download the package and install from a local archive file.
 
-> [socketlabs_injectionapi-1.4.0.tar.gz](https://github.com/socketlabs/socketlabs-python/releases/download/socketlabs_injectionapi-1.4.0.tar.gz)
+> [socketlabs_injectionapi-1.4.2.tar.gz](https://github.com/socketlabs/socketlabs-python/releases/download/1.4.2/socketlabs_injectionapi-1.4.2.tar.gz)
 
 ```
 pip install <path>/socketlabs_injectionapi-1.4.0.tar.gz
 ```
 
 ### From git using pip
 ```
@@ -236,14 +236,15 @@
 
 ### [Bulk send with Amp ](https://github.com/socketlabs/socketlabs-python/blob/main/python-examples/bulk/bulk_send_with_amp_body.py)
 This example demonstrates how to send a bulk message with an AMP Html body.
 For more information about AMP please see [AMP Project](https://amp.dev/documentation/)
 
 <a name="version"></a>
 # Version
+* 1.4.2 - Adding API Key Authorization 
 * 1.4.0 - Adding Metadata and Tags
 * 1.2.1 - Adding optional retry logic for Http requests. If configured, the request will retry when certain 500 errors occur (500, 502, 503, 504)
 * 1.1.1 - Adding request timeout value on the client for Http requests
 * 1.1.0 - Adds Amp Html Support
 * 1.0.0 - Initial Release
 
 <a name="license" id="license"></a>
```

### Comparing `socketlabs_injectionapi-1.4.0/README.md` & `socketlabs_injectionapi-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 pip install socketlabs-injectionapi
 ```
 ### From a local archive using pip
 
 You can just download the package and install from a local archive file.
 
-> [socketlabs_injectionapi-1.4.0.tar.gz](https://github.com/socketlabs/socketlabs-python/releases/download/socketlabs_injectionapi-1.4.0.tar.gz)
+> [socketlabs_injectionapi-1.4.2.tar.gz](https://github.com/socketlabs/socketlabs-python/releases/download/1.4.2/socketlabs_injectionapi-1.4.2.tar.gz)
 
 ```
 pip install <path>/socketlabs_injectionapi-1.4.0.tar.gz
 ```
 
 ### From git using pip
 ```
@@ -213,14 +213,15 @@
 
 ### [Bulk send with Amp ](https://github.com/socketlabs/socketlabs-python/blob/main/python-examples/bulk/bulk_send_with_amp_body.py)
 This example demonstrates how to send a bulk message with an AMP Html body.
 For more information about AMP please see [AMP Project](https://amp.dev/documentation/)
 
 <a name="version"></a>
 # Version
+* 1.4.2 - Adding API Key Authorization 
 * 1.4.0 - Adding Metadata and Tags
 * 1.2.1 - Adding optional retry logic for Http requests. If configured, the request will retry when certain 500 errors occur (500, 502, 503, 504)
 * 1.1.1 - Adding request timeout value on the client for Http requests
 * 1.1.0 - Adds Amp Html Support
 * 1.0.0 - Initial Release
 
 <a name="license" id="license"></a>
```

### Comparing `socketlabs_injectionapi-1.4.0/setup.py` & `socketlabs_injectionapi-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/addressresult.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/addressresult.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/httpendpoint.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/httpendpoint.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/httprequest.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/httprequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 import queue
 from enum import Enum
 
 from ..version import __version__
 from ..proxy import Proxy
 
+from .stringextension import StringExtension
 from .httpendpoint import HttpEndpoint
 from .injectionresponseparser import InjectionResponseParser
 from .serialization.injectionrequest import InjectionRequest
 
 
 class HttpRequest(object):
     """
@@ -24,26 +25,34 @@
         Enumeration of HTTP Request Methods
         """
         GET = 0
         POST = 1
         PUT = 2
         DELETE = 3
 
-    def __init__(self, method: HttpRequestMethod, endpoint: HttpEndpoint, timeout: int):
+    def __init__(self, method: HttpRequestMethod, endpoint: HttpEndpoint, timeout: int, authentication: str):
         """
         Creates a new instance of the HTTP Request class
         :param method: the HTTP request method
         :type method: HttpRequestMethod
         :param endpoint: the Http endpoint for the HTTP request
         :type endpoint: HttpEndpoint
         """
         self._request_method = method
         self._endpoint = endpoint
         self._http_proxy = None
         self._timeout = timeout
+        self._authentication = authentication
+        self._headers = {
+            'User-Agent': self.__user_agent,
+            'Content-Type': 'application/json; charset=utf-8',
+            'Accept': 'application/json',
+        }
+        if not StringExtension.is_none_or_white_space(authentication):
+            self._headers["Authorization"] = "Bearer " + authentication
 
     @property
     def __user_agent(self):
         """
         The User-Agent request header added to the Injection API Http request.
         Used to identify the source of the request.
         :return the SocketLabs User-Agent
@@ -104,15 +113,15 @@
         :param on_success_callback: the callback method for success
         :type on_success_callback: method
         :param on_error_callback: the callback method for error
         :type on_error_callback: method
         """
 
         try:
-
+            print (request)
             th = threading.Thread(target=self.__queue_request,
                                   kwargs={
                                       "request": request,
                                       "on_success_callback": on_success_callback,
                                       "on_error_callback": on_error_callback
                                   })
             th.start()
@@ -139,25 +148,20 @@
         """
         Send the HTTP Request
         :param request: the injection request to send
         :type request: InjectionRequest
         :return the injection response received from the request
         :rtype InjectionResponse
         """
-        headers = {
-            'User-Agent': self.__user_agent,
-            'Content-Type': 'application/json; charset=utf-8',
-            'Accept': 'application/json',
-        }
 
         json_body = json.dumps(request.to_json())
 
         try:
             connection = self.__get_connection()
-            connection.request("POST", self._endpoint.url, json_body, headers)
+            connection.request("POST", self._endpoint.url, json_body, self._headers)
             response = connection.getresponse()
 
         except Exception as e:
             raise e
 
         return response
```

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/injectionrequestfactory.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/injectionrequestfactory.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/injectionresponseparser.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/injectionresponseparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         resp_dto._error_code = dct['ErrorCode']
 
     if 'TransactionReceipt' in dct:
         resp_dto._transaction_receipt = dct['TransactionReceipt']
 
     if 'MessageResults' in dct:
         resp_dto.message_results = []
-        for item in dct['MessageResults']:
+        for item in dct['MessageResults'] or []:
             message_dto = MessageResultDto()
             if 'Index' in item:
                 message_dto.index = item['Index']
             if 'AddressResults' in item:
                 message_dto.address_results = str(item['AddressResults'])
             if 'ErrorCode' in item:
                 message_dto.error_code = item['ErrorCode']
```

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/retryhandler.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/retryhandler.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/sendvalidator.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/sendvalidator.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/addressjson.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/addressjson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/attachmentjson.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/attachmentjson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/customheaderjson.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/customheaderjson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/injectionrequest.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/injectionrequest.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/injectionresponsedto.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/injectionresponsedto.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/mergedatajson.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/mergedatajson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/mergefieldjson.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/mergefieldjson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/messagejson.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/messagejson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/messageresultdto.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/messageresultdto.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/serialization/metadatajson.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/serialization/metadatajson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/core/stringextension.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/core/stringextension.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/attachment.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/attachment.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/basicmessage.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/basicmessage.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/bulkmessage.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/bulkmessage.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/bulkrecipient.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/bulkrecipient.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/customheader.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/customheader.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/emailaddress.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/emailaddress.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/messagebase.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/messagebase.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/message/metadata.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/message/metadata.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/proxy.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/proxy.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/retrysettings.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/retrysettings.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/sendresponse.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/sendresponse.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/sendresult.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/sendresult.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs/injectionapi/socketlabsclient.py` & `socketlabs_injectionapi-1.4.2/socketlabs/injectionapi/socketlabsclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from .core.sendvalidator import SendValidator
 from .core.retryhandler import RetryHandler
 from .retrysettings import RetrySettings
 from .message.basicmessage import BasicMessage
 from .message.bulkmessage import BulkMessage
 from .proxy import Proxy
 from .sendresult import SendResult
+from .core.apikeyparser import ApiKeyParser
+from .core.apikeyparseresult import ApiKeyParseResult
 
 
 class SocketLabsClient(object):
     """
     SocketLabsClient is a wrapper for the SocketLabs Injection API that makes
     it easy to send messages and parse responses.
     """
@@ -77,21 +79,23 @@
     def number_of_retries(self):
         return self._number_of_retries
     
     @number_of_retries.setter
     def number_of_retries(self, retries: int):
         self._number_of_retries = retries
 
-    def __build_http_request(self):
+    def __build_http_request(self, authentication: str):
         """
         Build the HttpRequest. Will add the proxy, if set
+        :param authentication: the API key to include as a bearer token
+        :type authentication: object
         :return the HttpRequest object to use for the request
         :rtype HttpRequest
         """
-        req = HttpRequest(HttpRequest.HttpRequestMethod.POST, self.__endpoint, self.request_timeout)
+        req = HttpRequest(HttpRequest.HttpRequestMethod.POST, self.__endpoint, self.request_timeout, authentication)
         if self._http_proxy is not None:
             req.proxy = self._http_proxy
         return req
 
     def send(self, message):
         """
         Sends a BasicMessage message and returns the response from the Injection API.
@@ -115,18 +119,27 @@
         :return the SendResponse from the request
         :rtype SendResponse
         """
         resp = self.__validate_basic_message(message)
         if not resp.result == SendResult.Success:
             return resp
 
+        api_key_parser = ApiKeyParser()
+        parse_result = api_key_parser.parse(self._api_key)
+
         req_factory = InjectionRequestFactory(self._server_id, self._api_key)
+        http_request = self.__build_http_request("")
+
+        if parse_result == ApiKeyParseResult.Success:
+            req_factory = InjectionRequestFactory(self._server_id, "")
+            http_request = self.__build_http_request(self._api_key)
+
         body = req_factory.generate_request(message)
 
-        retry_handler = RetryHandler(self.__build_http_request(), RetrySettings(self.number_of_retries))
+        retry_handler = RetryHandler(http_request, RetrySettings(self.number_of_retries))
         response = retry_handler.send(body)
 
         data = response.read().decode("utf-8")
         response_code = response.status
         result = InjectionResponseParser.parse(data, response_code)
 
         return result
@@ -139,18 +152,27 @@
         :return the SendResponse from the request
         :rtype SendResponse
         """
         resp = self.__validate_bulk_message(message)
         if not resp.result == SendResult.Success:
             return resp
 
+        api_key_parser = ApiKeyParser()
+        parse_result = api_key_parser.parse(self._api_key)
+
         req_factory = InjectionRequestFactory(self._server_id, self._api_key)
+        http_request = self.__build_http_request("")
+
+        if parse_result == ApiKeyParseResult.Success:
+            req_factory = InjectionRequestFactory(self._server_id, "")
+            http_request = self.__build_http_request(self._api_key)
+
         body = req_factory.generate_request(message)
 
-        retry_handler = RetryHandler(self.__build_http_request(), RetrySettings(self.number_of_retries))
+        retry_handler = RetryHandler(http_request, RetrySettings(self.number_of_retries))
         response = retry_handler.send(body)
 
         data = response.read().decode("utf-8")
         response_code = response.status
         result = InjectionResponseParser.parse(data, response_code)
 
         return result
```

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs_injectionapi.egg-info/PKG-INFO` & `socketlabs_injectionapi-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: socketlabs-injectionapi
-Version: 1.4.0
+Name: socketlabs_injectionapi
+Version: 1.4.2
 Summary: SocketLabs Email Delivery Python client library
 Home-page: https://github.com/socketlabs/socketlabs-python
 Author: David Schrenker, Matt Reibach, Ryan Lydzinski, Praneeth Chandra
 Author-email: support@socketlabs.com
 License: MIT
 Project-URL: Organization, https://github.com/socketlabs
 Project-URL: Bug Reports, https://github.com/socketlabs/socketlabs-python/issues
@@ -49,15 +49,15 @@
 ```
 pip install socketlabs-injectionapi
 ```
 ### From a local archive using pip
 
 You can just download the package and install from a local archive file.
 
-> [socketlabs_injectionapi-1.4.0.tar.gz](https://github.com/socketlabs/socketlabs-python/releases/download/socketlabs_injectionapi-1.4.0.tar.gz)
+> [socketlabs_injectionapi-1.4.2.tar.gz](https://github.com/socketlabs/socketlabs-python/releases/download/1.4.2/socketlabs_injectionapi-1.4.2.tar.gz)
 
 ```
 pip install <path>/socketlabs_injectionapi-1.4.0.tar.gz
 ```
 
 ### From git using pip
 ```
@@ -236,14 +236,15 @@
 
 ### [Bulk send with Amp ](https://github.com/socketlabs/socketlabs-python/blob/main/python-examples/bulk/bulk_send_with_amp_body.py)
 This example demonstrates how to send a bulk message with an AMP Html body.
 For more information about AMP please see [AMP Project](https://amp.dev/documentation/)
 
 <a name="version"></a>
 # Version
+* 1.4.2 - Adding API Key Authorization 
 * 1.4.0 - Adding Metadata and Tags
 * 1.2.1 - Adding optional retry logic for Http requests. If configured, the request will retry when certain 500 errors occur (500, 502, 503, 504)
 * 1.1.1 - Adding request timeout value on the client for Http requests
 * 1.1.0 - Adds Amp Html Support
 * 1.0.0 - Initial Release
 
 <a name="license" id="license"></a>
```

### Comparing `socketlabs_injectionapi-1.4.0/socketlabs_injectionapi.egg-info/SOURCES.txt` & `socketlabs_injectionapi-1.4.2/socketlabs_injectionapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 socketlabs/injectionapi/proxy.py
 socketlabs/injectionapi/retrysettings.py
 socketlabs/injectionapi/sendresponse.py
 socketlabs/injectionapi/sendresult.py
 socketlabs/injectionapi/socketlabsclient.py
 socketlabs/injectionapi/version.py
 socketlabs/injectionapi/core/__init__.py
+socketlabs/injectionapi/core/apikeyparser.py
+socketlabs/injectionapi/core/apikeyparseresult.py
 socketlabs/injectionapi/core/httpendpoint.py
 socketlabs/injectionapi/core/httprequest.py
 socketlabs/injectionapi/core/injectionrequestfactory.py
 socketlabs/injectionapi/core/injectionresponseparser.py
 socketlabs/injectionapi/core/retryhandler.py
 socketlabs/injectionapi/core/sendvalidator.py
 socketlabs/injectionapi/core/stringextension.py
```

