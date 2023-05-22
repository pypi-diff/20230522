# Comparing `tmp/anoncreds-0.1.0.dev16.tar.gz` & `tmp/anoncreds-0.1.0.dev17-py3-none-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoncreds-0.1.0.dev16.tar", last modified: Wed May 17 14:20:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

