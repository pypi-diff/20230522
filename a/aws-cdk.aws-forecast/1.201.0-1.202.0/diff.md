# Comparing `tmp/aws-cdk.aws-forecast-1.201.0.tar.gz` & `tmp/aws_cdk.aws_forecast-1.202.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src536437278/src/packages/@aws-cdk/aws-forecast/dist/python/aws-cdk.aws-forecast-1.201.0.tar", last modified: Wed May 10 17:09:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

