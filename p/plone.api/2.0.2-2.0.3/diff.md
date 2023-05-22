# Comparing `tmp/plone.api-2.0.2.tar.gz` & `tmp/plone.api-2.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.api-2.0.2.tar", last modified: Thu Apr 13 22:55:19 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

