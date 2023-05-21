# Comparing `tmp/reteps-ctfcli-0.0.12.tar.gz` & `tmp/reteps_ctfcli-0.0.13-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reteps-ctfcli-0.0.12.tar", last modified: Wed Nov 30 19:10:02 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

