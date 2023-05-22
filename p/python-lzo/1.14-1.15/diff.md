# Comparing `tmp/python-lzo-1.14.tar.gz` & `tmp/python_lzo-1.15-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lzo-1.14.tar", last modified: Sun Dec 26 07:54:18 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

