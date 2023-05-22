# Comparing `tmp/adnbidder-1.0.2.tar.gz` & `tmp/adnbidder-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adnbidder-1.0.2.tar", last modified: Mon May 22 03:05:13 2023, max compression
+gzip compressed data, was "adnbidder-1.0.3.tar", last modified: Mon May 22 14:04:45 2023, max compression
```

## Comparing `adnbidder-1.0.2.tar` & `adnbidder-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:05:13.364913 adnbidder-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-22 03:04:59.000000 adnbidder-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-22 03:05:13.364913 adnbidder-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-22 03:04:59.000000 adnbidder-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:05:13.364913 adnbidder-1.0.2/adnbidder/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 03:04:59.000000 adnbidder-1.0.2/adnbidder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-22 03:04:59.000000 adnbidder-1.0.2/adnbidder/bidder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:05:13.364913 adnbidder-1.0.2/adnbidder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 03:05:13.364913 adnbidder-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 03:04:59.000000 adnbidder-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:04:44.996782 adnbidder-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-22 14:04:28.000000 adnbidder-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-22 14:04:44.992782 adnbidder-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-22 14:04:28.000000 adnbidder-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:04:44.992782 adnbidder-1.0.3/adnbidder/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 14:04:28.000000 adnbidder-1.0.3/adnbidder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-05-22 14:04:28.000000 adnbidder-1.0.3/adnbidder/bidder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:04:44.992782 adnbidder-1.0.3/adnbidder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-22 14:04:44.000000 adnbidder-1.0.3/adnbidder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 14:04:44.000000 adnbidder-1.0.3/adnbidder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:04:44.000000 adnbidder-1.0.3/adnbidder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 14:04:44.000000 adnbidder-1.0.3/adnbidder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 14:04:44.000000 adnbidder-1.0.3/adnbidder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:04:44.996782 adnbidder-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 14:04:28.000000 adnbidder-1.0.3/setup.py
```

### Comparing `adnbidder-1.0.2/LICENSE.txt` & `adnbidder-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adnbidder-1.0.2/README.md` & `adnbidder-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `adnbidder-1.0.2/adnbidder/bidder.py` & `adnbidder-1.0.3/adnbidder/bidder.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 
 class BidUpdate:
     """
     Object to hold a bid update request
     """
     def __init__(self,
                  line_item_id,
-                 site_id,
-                 upper_bid_cpm,
+                 site_id=None,
+                 upper_bid_cpm=None,
                  lower_bid_cpm=None,
-                 lower_bids_percent=0):
+                 lower_bids_percent=0,
+                 pause=None,
+                 resume=None):
         """
         Initialise the bid update
         :param line_item_id: line item identifier
         :param site_id: site identifier
         :param upper_bid_cpm: the highest bid to use
         :param lower_bid_cpm: the lowest bid to use
         :param lower_bids_percent: the percentage of bids that should use the low bid amount
@@ -32,20 +34,32 @@
         self.site_id = site_id
         if lower_bid_cpm is None:
             self.lower_bid_cpm = upper_bid_cpm
         else:
             self.lower_bid_cpm = lower_bid_cpm
         self.upper_bid_cpm = upper_bid_cpm
         self.lower_bids_percent = lower_bids_percent
+        self.pause = pause
+        self.resume = resume
 
     def to_payload(self) -> dict:
         """
         Converts this object into a dict as expected by the Adnuntius API
         :return:
         """
+        if self.pause is not None and self.pause:
+            return {
+                'id': self.line_item_id,
+                'pause': True
+            }
+        if self.resume is not None and self.resume:
+            return {
+                'id': self.line_item_id,
+                'resume': True
+            }
         return {
             'id': self.line_item_id,
             'site': self.site_id,
             'lowerCpm': self.lower_bid_cpm,
             'upperCpm': self.upper_bid_cpm,
             'lowBidPercent': self.lower_bids_percent,
         }
```

### Comparing `adnbidder-1.0.2/setup.py` & `adnbidder-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
     name="adnbidder",
-    version="1.0.2",
+    version="1.0.3",
     description="A simple client for controlling bidding in the Adnuntius platform",
     long_description="A simple client for controlling bidding in the Adnuntius platform",
     url="https://github.com/Adnuntius/adnuntius-bidder",
     author="Adnuntius",
     author_email="tech@adnuntius.com",
     license="MIT",
     classifiers=[
```

