# Comparing `tmp/cosapp-0.14.0.tar.gz` & `tmp/cosapp-0.14.0.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosapp-0.14.0.tar", last modified: Wed May 17 16:52:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

