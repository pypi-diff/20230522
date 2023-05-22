# Comparing `tmp/aping_cli-0.1.0-py3-none-any.whl.zip` & `tmp/aping_cli-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,12 @@
-Zip file size: 4211 bytes, number of entries: 7
+Zip file size: 6503 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx     3316 b- defN 23-May-13 23:31 aping.py
--rw-rw-r--  2.0 unx     1056 b- defN 23-May-13 23:40 aping_cli-0.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2140 b- defN 23-May-13 23:40 aping_cli-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-13 23:40 aping_cli-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       38 b- defN 23-May-13 23:40 aping_cli-0.1.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-May-13 23:40 aping_cli-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      557 b- defN 23-May-13 23:40 aping_cli-0.1.0.dist-info/RECORD
-7 files, 7205 bytes uncompressed, 3219 bytes compressed:  55.3%
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-21 17:18 aping/__init__.py
+-rw-rw-r--  2.0 unx     2720 b- defN 23-May-22 12:44 aping/main.py
+-rw-rw-r--  2.0 unx     1647 b- defN 23-May-22 12:43 aping/ping.py
+-rw-rw-r--  2.0 unx     1056 b- defN 23-May-22 12:48 aping_cli-0.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2638 b- defN 23-May-22 12:48 aping_cli-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 12:48 aping_cli-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       43 b- defN 23-May-22 12:48 aping_cli-0.2.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-22 12:48 aping_cli-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      768 b- defN 23-May-22 12:48 aping_cli-0.2.0.dist-info/RECORD
+10 files, 12286 bytes uncompressed, 5197 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -1,22 +1,31 @@
 Filename: aping.py
 Comment: 
 
-Filename: aping_cli-0.1.0.dist-info/LICENSE
+Filename: aping/__init__.py
 Comment: 
 
-Filename: aping_cli-0.1.0.dist-info/METADATA
+Filename: aping/main.py
 Comment: 
 
-Filename: aping_cli-0.1.0.dist-info/WHEEL
+Filename: aping/ping.py
 Comment: 
 
-Filename: aping_cli-0.1.0.dist-info/entry_points.txt
+Filename: aping_cli-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: aping_cli-0.1.0.dist-info/top_level.txt
+Filename: aping_cli-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: aping_cli-0.1.0.dist-info/RECORD
+Filename: aping_cli-0.2.0.dist-info/WHEEL
+Comment: 
+
+Filename: aping_cli-0.2.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: aping_cli-0.2.0.dist-info/top_level.txt
+Comment: 
+
+Filename: aping_cli-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `aping_cli-0.1.0.dist-info/LICENSE` & `aping_cli-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aping_cli-0.1.0.dist-info/METADATA` & `aping_cli-0.2.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aping-cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool to ping multiple hosts at once and export results as Prometheus metrics.
 Home-page: https://github.com/alexpizarroj/aping
 Author: Alex Pizarro
 Author-email: alex.pizarro.j@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,20 @@
 
 # aping
 
 A tool to ping multiple hosts at once and export results as Prometheus metrics.
 
 Relies on https://github.com/romana/multi-ping/ (see https://stackoverflow.com/a/45746002).
 
+## Installation
+
+```shell
+pip install aping-cli
+```
+
 ## Usage
 
 To run the tool, type:
 
 ```shell
 aping "google-dns-1=8.8.8.8" "google-dns-2=8.8.4.4"
 ```
@@ -40,14 +46,22 @@
 Prometheus metrics server available at http://127.0.0.1:8000
 google-dns-1 (8.8.8.8): 100.78ms, google-dns-2 (8.8.4.4): 100.78ms
 google-dns-1 (8.8.8.8): 123.73ms, google-dns-2 (8.8.4.4): 122.97ms
 google-dns-1 (8.8.8.8): 111.99ms, google-dns-2 (8.8.4.4): 112.96ms
 google-dns-1 (8.8.8.8): 112.76ms, google-dns-2 (8.8.4.4): 113.86ms
 ```
 
+In Linux/MacOS environments, ICMP packets can only be sent by processes with root
+privileges (this is a requirement of the `multi-ping` package, which `aping` uses).
+In those cases, the recommended invocation command would be:
+
+```shell
+sudo -E "$(which aping)" "google-dns-1=8.8.8.8" "google-dns-2=8.8.4.4"
+```
+
 ## Contributing
 
 ### Local development
 
 How to set up a local environment:
 
 ```shell
@@ -64,14 +78,15 @@
 ## Resources
 
 Grafana:
 
 - Default username and password are both `admin`.
 - https://grafana.com/tutorials/grafana-fundamentals/
 - https://grafana.com/docs/grafana/latest/getting-started/build-first-dashboard/
+- https://grafana.com/docs/grafana/latest/setup-grafana/configure-docker/#run-grafana-container-with-persistent-storage-recommended
 
 Prometheus:
 
 - https://prometheus.io/docs/concepts/metric_types/
 - https://prometheus.io/docs/practices/histograms/
 - https://github.com/prometheus/client_python
 - https://prometheus.io/docs/prometheus/latest/getting_started/
```

