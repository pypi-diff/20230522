# Comparing `tmp/sparkverse-0.0.2.tar.gz` & `tmp/sparkverse-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkverse-0.0.2.tar", last modified: Mon May  8 19:09:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

