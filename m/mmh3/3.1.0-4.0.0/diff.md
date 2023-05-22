# Comparing `tmp/mmh3-3.1.0.tar.gz` & `tmp/mmh3-4.0.0-cp310-cp310-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmh3-3.1.0.tar", last modified: Fri Mar 24 14:14:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

