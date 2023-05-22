# Comparing `tmp/boto3_extensions-0.8.0.tar.gz` & `tmp/boto3_extensions-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/boto3_extensions-0.8.0.tar", last modified: Tue Jan  2 23:35:30 2018, max compression
+gzip compressed data, was "dist/boto3_extensions-0.9.0.tar", last modified: Mon Jan  8 00:32:01 2018, max compression
```

## Comparing `boto3_extensions-0.8.0.tar` & `boto3_extensions-0.9.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/acm/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/acm/2015-12-08/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      129 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/acm/2015-12-08/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     3341 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/acm/2015-12-08/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/autoscaling/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/autoscaling/2011-01-01/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      246 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/autoscaling/2011-01-01/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     2177 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/autoscaling/2011-01-01/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudformation/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudformation/2010-05-15/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      191 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudformation/2010-05-15/arns-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudfront/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudfront/2017-03-25/
--rw-r--r--   0 aposney   (1000) aposney   (1000)       64 2017-12-27 23:14:09.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudfront/2017-03-25/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1177 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudfront/2017-03-25/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudtrail/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudtrail/2013-11-01/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      118 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudtrail/2013-11-01/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     5784 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudtrail/2013-11-01/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudwatch/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudwatch/2010-08-01/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      136 2017-12-27 23:14:25.000000 boto3_extensions-0.8.0/boto3_extensions/data/cloudwatch/2010-08-01/arns-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cur/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/cur/2017-01-06/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      189 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/cur/2017-01-06/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1018 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/cur/2017-01-06/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/datapipeline/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/datapipeline/2012-10-29/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      176 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/datapipeline/2012-10-29/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1359 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/datapipeline/2012-10-29/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/directconnect/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/directconnect/2012-10-25/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      345 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/directconnect/2012-10-25/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1782 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/directconnect/2012-10-25/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/dynamodb/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/dynamodb/2012-08-10/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      118 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/dynamodb/2012-08-10/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     4475 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/dynamodb/2012-08-10/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/ec2/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/ec2/2016-11-15/
--rw-r--r--   0 aposney   (1000) aposney   (1000)     3625 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/ec2/2016-11-15/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)    88198 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/ec2/2016-11-15/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/elasticache/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/elasticache/2015-02-02/
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1526 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/elasticache/2015-02-02/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)    14072 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/elasticache/2015-02-02/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/elb/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/elb/2012-06-01/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      212 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/elb/2012-06-01/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1809 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/elb/2012-06-01/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/elbv2/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/elbv2/2015-12-01/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      147 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/elbv2/2015-12-01/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1710 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/elbv2/2015-12-01/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/emr/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/emr/2009-03-31/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      174 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/emr/2009-03-31/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1077 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/emr/2009-03-31/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/glacier/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/glacier/2012-06-01/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      195 2017-12-27 23:14:25.000000 boto3_extensions-0.8.0/boto3_extensions/data/glacier/2012-06-01/arns-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/glue/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/glue/2017-03-31/
--rw-r--r--   0 aposney   (1000) aposney   (1000)     2061 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/glue/2017-03-31/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/health/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/health/2016-08-04/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      145 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/health/2016-08-04/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     2972 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/health/2016-08-04/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/iam/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/iam/2010-05-08/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      718 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/iam/2010-05-08/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)    52525 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/iam/2010-05-08/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/kinesis/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/kinesis/2013-12-02/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      119 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/kinesis/2013-12-02/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)      737 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/kinesis/2013-12-02/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/lambda/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/lambda/2015-03-31/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      124 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/lambda/2015-03-31/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     4754 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/lambda/2015-03-31/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/opsworks/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/opsworks/2013-02-18/
--rw-r--r--   0 aposney   (1000) aposney   (1000)       98 2017-12-27 23:14:25.000000 boto3_extensions-0.8.0/boto3_extensions/data/opsworks/2013-02-18/arns-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/pricing/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/pricing/2017-10-15/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      184 2017-12-21 02:44:07.000000 boto3_extensions-0.8.0/boto3_extensions/data/pricing/2017-10-15/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1092 2017-12-21 02:44:07.000000 boto3_extensions-0.8.0/boto3_extensions/data/pricing/2017-10-15/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/rds/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/rds/2014-10-31/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      187 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/rds/2014-10-31/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     1625 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/rds/2014-10-31/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/redshift/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/redshift/2012-12-01/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      638 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/redshift/2012-12-01/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     5162 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/redshift/2012-12-01/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/route53/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/route53/2013-04-01/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      302 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/route53/2013-04-01/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     3580 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/route53/2013-04-01/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/s3/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/s3/2006-03-01/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      756 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/s3/2006-03-01/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)    36305 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/s3/2006-03-01/resources-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/sns/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/sns/2010-03-31/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      140 2017-12-27 23:14:25.000000 boto3_extensions-0.8.0/boto3_extensions/data/sns/2010-03-31/arns-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/sqs/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/sqs/2012-11-05/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      156 2017-12-27 23:14:25.000000 boto3_extensions-0.8.0/boto3_extensions/data/sqs/2012-11-05/arns-1.json
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/support/
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions/data/support/2013-04-15/
--rw-r--r--   0 aposney   (1000) aposney   (1000)      344 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/support/2013-04-15/arns-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     6079 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/data/support/2013-04-15/resources-1.json
--rw-r--r--   0 aposney   (1000) aposney   (1000)     2588 2018-01-02 23:26:37.000000 boto3_extensions-0.8.0/boto3_extensions/__init__.py
--rw-r--r--   0 aposney   (1000) aposney   (1000)     6530 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/arn_patch.py
--rw-r--r--   0 aposney   (1000) aposney   (1000)       51 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/boto3_extensions/exceptions.py
-drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions.egg-info/
--rw-r--r--   0 aposney   (1000) aposney   (1000)     4096 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions.egg-info/PKG-INFO
--rw-r--r--   0 aposney   (1000) aposney   (1000)     3239 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 aposney   (1000) aposney   (1000)        1 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 aposney   (1000) aposney   (1000)       30 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions.egg-info/requires.txt
--rw-r--r--   0 aposney   (1000) aposney   (1000)       17 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/boto3_extensions.egg-info/top_level.txt
--rw-r--r--   0 aposney   (1000) aposney   (1000)       41 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/MANIFEST.in
--rw-r--r--   0 aposney   (1000) aposney   (1000)     2984 2017-10-23 01:33:47.000000 boto3_extensions-0.8.0/README.rst
--rw-r--r--   0 aposney   (1000) aposney   (1000)       67 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/setup.cfg
--rw-r--r--   0 aposney   (1000) aposney   (1000)      638 2018-01-02 23:35:00.000000 boto3_extensions-0.8.0/setup.py
--rw-r--r--   0 aposney   (1000) aposney   (1000)     4096 2018-01-02 23:35:30.000000 boto3_extensions-0.8.0/PKG-INFO
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/acm/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/acm/2015-12-08/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      129 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/acm/2015-12-08/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     3341 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/acm/2015-12-08/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/autoscaling/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/autoscaling/2011-01-01/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      246 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/autoscaling/2011-01-01/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     2177 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/autoscaling/2011-01-01/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudformation/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudformation/2010-05-15/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      191 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudformation/2010-05-15/arns-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudfront/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudfront/2017-03-25/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)       64 2017-12-27 23:14:09.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudfront/2017-03-25/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1177 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudfront/2017-03-25/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudtrail/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudtrail/2013-11-01/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      118 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudtrail/2013-11-01/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     5784 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudtrail/2013-11-01/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudwatch/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudwatch/2010-08-01/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      136 2017-12-27 23:14:25.000000 boto3_extensions-0.9.0/boto3_extensions/data/cloudwatch/2010-08-01/arns-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cur/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/cur/2017-01-06/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      189 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/cur/2017-01-06/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1018 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/cur/2017-01-06/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/datapipeline/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/datapipeline/2012-10-29/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      176 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/datapipeline/2012-10-29/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1359 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/datapipeline/2012-10-29/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/directconnect/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/directconnect/2012-10-25/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      345 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/directconnect/2012-10-25/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1782 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/directconnect/2012-10-25/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/dynamodb/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/dynamodb/2012-08-10/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      118 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/dynamodb/2012-08-10/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     4475 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/dynamodb/2012-08-10/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/ec2/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/ec2/2016-11-15/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     3625 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/ec2/2016-11-15/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)    88198 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/ec2/2016-11-15/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/elasticache/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/elasticache/2015-02-02/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1526 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/elasticache/2015-02-02/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)    14072 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/elasticache/2015-02-02/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/elb/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/elb/2012-06-01/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      212 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/elb/2012-06-01/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1809 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/elb/2012-06-01/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/elbv2/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/elbv2/2015-12-01/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      147 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/elbv2/2015-12-01/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1710 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/elbv2/2015-12-01/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/emr/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/emr/2009-03-31/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      174 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/emr/2009-03-31/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1077 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/emr/2009-03-31/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/glacier/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/glacier/2012-06-01/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      195 2017-12-27 23:14:25.000000 boto3_extensions-0.9.0/boto3_extensions/data/glacier/2012-06-01/arns-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/glue/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/glue/2017-03-31/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     2061 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/glue/2017-03-31/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/health/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/health/2016-08-04/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      145 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/health/2016-08-04/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     2972 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/health/2016-08-04/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/iam/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/iam/2010-05-08/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      718 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/iam/2010-05-08/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)    52525 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/iam/2010-05-08/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/kinesis/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/kinesis/2013-12-02/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      119 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/kinesis/2013-12-02/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      737 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/kinesis/2013-12-02/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/lambda/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/lambda/2015-03-31/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      124 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/lambda/2015-03-31/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     4754 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/lambda/2015-03-31/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/opsworks/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/opsworks/2013-02-18/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)       98 2017-12-27 23:14:25.000000 boto3_extensions-0.9.0/boto3_extensions/data/opsworks/2013-02-18/arns-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/pricing/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/pricing/2017-10-15/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      184 2017-12-21 02:44:07.000000 boto3_extensions-0.9.0/boto3_extensions/data/pricing/2017-10-15/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1092 2017-12-21 02:44:07.000000 boto3_extensions-0.9.0/boto3_extensions/data/pricing/2017-10-15/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/rds/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/rds/2014-10-31/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      187 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/rds/2014-10-31/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     1625 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/rds/2014-10-31/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/redshift/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/redshift/2012-12-01/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      638 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/redshift/2012-12-01/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     5162 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/redshift/2012-12-01/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/route53/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/route53/2013-04-01/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      302 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/route53/2013-04-01/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     3580 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/route53/2013-04-01/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/s3/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/s3/2006-03-01/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      756 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/s3/2006-03-01/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)    36305 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/s3/2006-03-01/resources-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/sns/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/sns/2010-03-31/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      140 2017-12-27 23:14:25.000000 boto3_extensions-0.9.0/boto3_extensions/data/sns/2010-03-31/arns-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/sqs/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/sqs/2012-11-05/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      156 2017-12-27 23:14:25.000000 boto3_extensions-0.9.0/boto3_extensions/data/sqs/2012-11-05/arns-1.json
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/support/
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions/data/support/2013-04-15/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      344 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/support/2013-04-15/arns-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     6079 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/data/support/2013-04-15/resources-1.json
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     2696 2018-01-08 00:28:44.000000 boto3_extensions-0.9.0/boto3_extensions/__init__.py
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     9197 2018-01-08 00:27:28.000000 boto3_extensions-0.9.0/boto3_extensions/arn_patch.py
+-rw-r--r--   0 aposney   (1000) aposney   (1000)       51 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/boto3_extensions/exceptions.py
+drwxr-xr-x   0 aposney   (1000) aposney   (1000)        0 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions.egg-info/
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     4096 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     3239 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 aposney   (1000) aposney   (1000)        1 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 aposney   (1000) aposney   (1000)       30 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions.egg-info/requires.txt
+-rw-r--r--   0 aposney   (1000) aposney   (1000)       17 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/boto3_extensions.egg-info/top_level.txt
+-rw-r--r--   0 aposney   (1000) aposney   (1000)       41 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/MANIFEST.in
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     2984 2017-10-23 01:33:47.000000 boto3_extensions-0.9.0/README.rst
+-rw-r--r--   0 aposney   (1000) aposney   (1000)       67 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/setup.cfg
+-rw-r--r--   0 aposney   (1000) aposney   (1000)      638 2018-01-08 00:30:28.000000 boto3_extensions-0.9.0/setup.py
+-rw-r--r--   0 aposney   (1000) aposney   (1000)     4096 2018-01-08 00:32:01.000000 boto3_extensions-0.9.0/PKG-INFO
```

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/acm/2015-12-08/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/acm/2015-12-08/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/autoscaling/2011-01-01/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/autoscaling/2011-01-01/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/cloudfront/2017-03-25/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/cloudfront/2017-03-25/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/cloudtrail/2013-11-01/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/cloudtrail/2013-11-01/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/cur/2017-01-06/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/cur/2017-01-06/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/datapipeline/2012-10-29/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/datapipeline/2012-10-29/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/directconnect/2012-10-25/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/directconnect/2012-10-25/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/dynamodb/2012-08-10/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/dynamodb/2012-08-10/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/ec2/2016-11-15/arns-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/ec2/2016-11-15/arns-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/ec2/2016-11-15/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/ec2/2016-11-15/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/elasticache/2015-02-02/arns-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/elasticache/2015-02-02/arns-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/elasticache/2015-02-02/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/elasticache/2015-02-02/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/elb/2012-06-01/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/elb/2012-06-01/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/elbv2/2015-12-01/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/elbv2/2015-12-01/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/emr/2009-03-31/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/emr/2009-03-31/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/glue/2017-03-31/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/glue/2017-03-31/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/health/2016-08-04/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/health/2016-08-04/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/iam/2010-05-08/arns-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/iam/2010-05-08/arns-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/iam/2010-05-08/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/iam/2010-05-08/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/kinesis/2013-12-02/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/kinesis/2013-12-02/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/lambda/2015-03-31/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/lambda/2015-03-31/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/pricing/2017-10-15/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/pricing/2017-10-15/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/rds/2014-10-31/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/rds/2014-10-31/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/redshift/2012-12-01/arns-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/redshift/2012-12-01/arns-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/redshift/2012-12-01/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/redshift/2012-12-01/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/route53/2013-04-01/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/route53/2013-04-01/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/s3/2006-03-01/arns-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/s3/2006-03-01/arns-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/s3/2006-03-01/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/s3/2006-03-01/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/data/support/2013-04-15/resources-1.json` & `boto3_extensions-0.9.0/boto3_extensions/data/support/2013-04-15/resources-1.json`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/boto3_extensions/__init__.py` & `boto3_extensions-0.9.0/boto3_extensions/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import boto3
 import botocore.session
 import logging
 from logging import NullHandler
 from boto3_extensions.arn_patch import patch_session, \
                                    patch_service_context, \
                                    patch_resource_factory, \
-                                   patch_resource_meta
+                                   patch_resource_meta, \
+                                   patch_create_request_parameters
 from os import environ, path
 from imp import reload
 
 logging.getLogger(__name__).addHandler(NullHandler())
 _logger = logging.getLogger(__name__)
 
 dir_path = path.dirname(path.realpath(__file__))
@@ -21,14 +22,15 @@
     """
     Patch boto3 to support ARNs for all resources
     """
     patch_session()
     patch_service_context()
     patch_resource_factory()
     patch_resource_meta()
+    patch_create_request_parameters()
     _logger.info('Patched Boto3 with arn support')
 
 
 def get_role_session(role_arn,
                      role_session_name=None,
                      base_session=None,
                      **kwargs):
```

### Comparing `boto3_extensions-0.8.0/boto3_extensions.egg-info/PKG-INFO` & `boto3_extensions-0.9.0/boto3_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: boto3-extensions
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extensions to the AWS SDK for Python
 Home-page: https://bitbucket.org/atlassian/boto3_extensions/
 Author: Atlassian
 Author-email: UNKNOWN
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description: ================
```

### Comparing `boto3_extensions-0.8.0/boto3_extensions.egg-info/SOURCES.txt` & `boto3_extensions-0.9.0/boto3_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/README.rst` & `boto3_extensions-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `boto3_extensions-0.8.0/setup.py` & `boto3_extensions-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from setuptools import find_packages
 
 long_description = open('README.rst').read()
 
-VERSION = '0.8.0'
+VERSION = '0.9.0'
 requires = [
     'boto3>=1.4.7',
     'botocore>=1.7.40'
 ]
 
 setup(
     name='boto3_extensions',
```

### Comparing `boto3_extensions-0.8.0/PKG-INFO` & `boto3_extensions-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: boto3_extensions
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extensions to the AWS SDK for Python
 Home-page: https://bitbucket.org/atlassian/boto3_extensions/
 Author: Atlassian
 Author-email: UNKNOWN
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description: ================
```

