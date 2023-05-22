# Comparing `tmp/cdk-opinionated-constructs-2.1.2.tar.gz` & `tmp/cdk-opinionated-constructs-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-opinionated-constructs-2.1.2.tar", last modified: Fri May 19 08:50:02 2023, max compression
+gzip compressed data, was "cdk-opinionated-constructs-2.1.3.tar", last modified: Mon May 22 07:45:48 2023, max compression
```

## Comparing `cdk-opinionated-constructs-2.1.2.tar` & `cdk-opinionated-constructs-2.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:50:02.713373 cdk-opinionated-constructs-2.1.2/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.1.2/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-05-19 08:50:02.713463 cdk-opinionated-constructs-2.1.2/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    27443 2023-04-18 12:21:33.000000 cdk-opinionated-constructs-2.1.2/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:50:02.602388 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/nlb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/rds_instance.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3325 2023-05-19 08:49:32.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/s3.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/sns.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    11940 2022-12-03 22:01:00.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:50:02.713035 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-05-19 08:50:02.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-05-19 08:50:02.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-05-19 08:50:02.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       89 2023-05-19 08:50:02.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-05-19 08:50:02.000000 cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-05-19 08:50:02.714335 cdk-opinionated-constructs-2.1.2/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      761 2023-05-19 08:49:43.000000 cdk-opinionated-constructs-2.1.2/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:50:02.604121 cdk-opinionated-constructs-2.1.2/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.2/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1781 2023-04-20 10:28:48.000000 cdk-opinionated-constructs-2.1.2/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:50:02.639791 cdk-opinionated-constructs-2.1.2/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.2/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.2/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.2/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3241 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.2/test/stacks/lmb_docker_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.1.2/test/stacks/lmb_monitoring_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2810 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.2/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.2/test/stacks/nlb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.2/test/stacks/rds_mysql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.2/test/stacks/rds_postgresql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.2/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.2/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.2/test/stacks/wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:50:02.648244 cdk-opinionated-constructs-2.1.2/test/unit/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.2/test/unit/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.2/test/unit/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.2/test/unit/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.2/test/unit/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      852 2023-05-19 08:46:19.000000 cdk-opinionated-constructs-2.1.2/test/unit/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.2/test/unit/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.2/test/unit/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.593133 cdk-opinionated-constructs-2.1.3/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.1.3/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-05-22 07:45:48.593237 cdk-opinionated-constructs-2.1.3/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    27443 2023-04-18 12:21:33.000000 cdk-opinionated-constructs-2.1.3/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.504099 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/nlb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/rds_instance.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3325 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/s3.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/sns.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    12369 2023-05-22 07:42:39.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.592880 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       89 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-05-22 07:45:48.593990 cdk-opinionated-constructs-2.1.3/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      761 2023-05-22 07:43:04.000000 cdk-opinionated-constructs-2.1.3/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.509090 cdk-opinionated-constructs-2.1.3/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.3/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1781 2023-04-20 10:28:48.000000 cdk-opinionated-constructs-2.1.3/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.538517 cdk-opinionated-constructs-2.1.3/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.3/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.3/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3241 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.3/test/stacks/lmb_docker_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.1.3/test/stacks/lmb_monitoring_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2810 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.3/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/test/stacks/nlb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.3/test/stacks/rds_mysql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.3/test/stacks/rds_postgresql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.3/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.587443 cdk-opinionated-constructs-2.1.3/test/unit/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      852 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_wafv2_stack.py
```

### Comparing `cdk-opinionated-constructs-2.1.2/LICENSE` & `cdk-opinionated-constructs-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/README.md` & `cdk-opinionated-constructs-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/alb.py` & `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/alb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/ecr.py` & `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/ecr.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/lmb.py` & `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/lmb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/nlb.py` & `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/nlb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/rds_instance.py` & `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/rds_instance.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/s3.py` & `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/s3.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/sns.py` & `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/sns.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs/wafv2.py` & `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/wafv2.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,166 @@
 class WAFv2(Construct):
     """Implement a v2 WAF where logs are sent to the AWS CloudWatch logs."""
 
     # pylint: disable=W0235
     def __init__(self, scope: Construct, construct_id: str) -> None:
         super().__init__(scope, construct_id)
 
+    @staticmethod
+    def __aws_account_takeover_prevention(aws_account_takeover_prevention):
+        return wafv2.CfnWebACL.RuleProperty(
+            name="AWS-AWSManagedRulesATPRuleSet",
+            priority=6,
+            override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
+            statement=wafv2.CfnWebACL.StatementProperty(
+                managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
+                    name="AWSManagedRulesATPRuleSet",
+                    vendor_name="AWS",
+                    managed_rule_group_configs=[
+                        wafv2.CfnWebACL.ManagedRuleGroupConfigProperty(
+                            login_path=aws_account_takeover_prevention["login_path"],  # type: ignore
+                        ),
+                        wafv2.CfnWebACL.ManagedRuleGroupConfigProperty(
+                            password_field=wafv2.CfnWebACL.FieldIdentifierProperty(
+                                identifier=aws_account_takeover_prevention["password_field"]  # type: ignore
+                            ),
+                        ),
+                        wafv2.CfnWebACL.ManagedRuleGroupConfigProperty(
+                            payload_type="FORM_ENCODED",
+                        ),
+                        wafv2.CfnWebACL.ManagedRuleGroupConfigProperty(
+                            username_field=wafv2.CfnWebACL.FieldIdentifierProperty(
+                                identifier=aws_account_takeover_prevention["username_field"]  # type: ignore
+                            ),
+                        ),
+                    ],
+                )
+            ),
+            visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
+                cloud_watch_metrics_enabled=True,
+                metric_name="AWS-AWSManagedRulesATPRuleSet",
+                sampled_requests_enabled=True,
+            ),
+        )
+
+    @staticmethod
+    def __aws_sqli_rule():
+        return wafv2.CfnWebACL.RuleProperty(
+            name="AWS-AWSManagedRulesSQLiRuleSet",
+            priority=5,
+            override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
+            statement=wafv2.CfnWebACL.StatementProperty(
+                managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
+                    name="AWSManagedRulesSQLiRuleSet",
+                    vendor_name="AWS",
+                )
+            ),
+            visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
+                cloud_watch_metrics_enabled=True,
+                metric_name="AWS-AWSManagedRulesSQLiRuleSet",
+                sampled_requests_enabled=True,
+            ),
+        )
+
+    @staticmethod
+    def __aws_bad_inputs_rule():
+        return wafv2.CfnWebACL.RuleProperty(
+            name="AWS-AWSManagedRulesKnownBadInputsRuleSet",
+            priority=4,
+            override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
+            statement=wafv2.CfnWebACL.StatementProperty(
+                managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
+                    name="AWSManagedRulesKnownBadInputsRuleSet",
+                    vendor_name="AWS",
+                )
+            ),
+            visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
+                cloud_watch_metrics_enabled=True,
+                metric_name="AWS-AWSManagedRulesKnownBadInputsRuleSet",
+                sampled_requests_enabled=True,
+            ),
+        )
+
+    @staticmethod
+    def __rate_list(rate_value: int):
+        return wafv2.CfnWebACL.RuleProperty(
+            name=f"Custom-RateLimit{rate_value}",
+            priority=1,
+            action=wafv2.CfnWebACL.RuleActionProperty(block=wafv2.CfnWebACL.BlockActionProperty()),
+            statement=wafv2.CfnWebACL.StatementProperty(
+                rate_based_statement=wafv2.CfnWebACL.RateBasedStatementProperty(
+                    aggregate_key_type="IP",
+                    limit=rate_value,
+                )
+            ),
+            visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
+                cloud_watch_metrics_enabled=True,
+                metric_name=f"Custom-RateLimit{rate_value}",
+                sampled_requests_enabled=True,
+            ),
+        )
+
+    @staticmethod
+    def __aws_ip_reputation_list():
+        return wafv2.CfnWebACL.RuleProperty(
+            name="AWS-AWSManagedRulesAmazonIpReputationList",
+            priority=0,
+            override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
+            statement=wafv2.CfnWebACL.StatementProperty(
+                managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
+                    name="AWSManagedRulesAmazonIpReputationList",
+                    vendor_name="AWS",
+                )
+            ),
+            visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
+                cloud_watch_metrics_enabled=True,
+                metric_name="AWS-AWSManagedRulesAmazonIpReputationList",
+                sampled_requests_enabled=True,
+            ),
+        )
+
+    @staticmethod
+    def __aws_common_rule(aws_common_excluded_rules):
+        return wafv2.CfnWebACL.RuleProperty(
+            name="AWS-AWSManagedRulesCommonRuleSet",
+            priority=2,
+            override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
+            statement=wafv2.CfnWebACL.StatementProperty(
+                managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
+                    excluded_rules=aws_common_excluded_rules,
+                    name="AWSManagedRulesCommonRuleSet",
+                    vendor_name="AWS",
+                )
+            ),
+            visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
+                cloud_watch_metrics_enabled=True,
+                metric_name="AWS-AWSManagedRulesCommonRuleSet",
+                sampled_requests_enabled=True,
+            ),
+        )
+
+    @staticmethod
+    def __aws_anonymous_list():
+        return wafv2.CfnWebACL.RuleProperty(
+            name="AWS-AWSManagedRulesAnonymousIpList",
+            priority=3,
+            override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
+            statement=wafv2.CfnWebACL.StatementProperty(
+                managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
+                    name="AWSManagedRulesAnonymousIpList",
+                    vendor_name="AWS",
+                )
+            ),
+            visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
+                cloud_watch_metrics_enabled=True,
+                metric_name="AWS-AWSManagedRulesAnonymousIpList",
+                sampled_requests_enabled=True,
+            ),
+        )
+
     def web_acl(
         self,
         name: str,
         rate_value: Union[int, None],
         aws_common_rule: bool = True,
         aws_common_rule_ignore_list: Optional[list] = None,
         aws_anony_list: bool = False,
@@ -43,175 +195,52 @@
         :param rate_value: The number of packets per seconds for custom rate limiting
         :param waf_scope: The WAF scope, it could be regional for API GW, Cognito and ALB or
         CLOUDFRONT for cloudfront distributions
         :param name: Then name of WAF ACL
         :return:
         """
 
-        # 0. Reputation List
-        aws_ip_rep_list = wafv2.CfnWebACL.RuleProperty(
-            name="AWS-AWSManagedRulesAmazonIpReputationList",
-            priority=0,
-            override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
-            statement=wafv2.CfnWebACL.StatementProperty(
-                managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
-                    name="AWSManagedRulesAmazonIpReputationList",
-                    vendor_name="AWS",
-                )
-            ),
-            visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
-                cloud_watch_metrics_enabled=True,
-                metric_name="AWS-AWSManagedRulesAmazonIpReputationList",
-                sampled_requests_enabled=True,
-            ),
-        )
+        # 0. Reputation List. The first rule is enabled by default
+        aws_ip_rep_list = self.__aws_ip_reputation_list()
         waf_rules = [aws_ip_rep_list]
 
         if rate_value:
             # 1. Custom Rate Limit
-            rate_list = wafv2.CfnWebACL.RuleProperty(
-                name=f"Custom-RateLimit{rate_value}",
-                priority=1,
-                action=wafv2.CfnWebACL.RuleActionProperty(block=wafv2.CfnWebACL.BlockActionProperty()),
-                statement=wafv2.CfnWebACL.StatementProperty(
-                    rate_based_statement=wafv2.CfnWebACL.RateBasedStatementProperty(
-                        aggregate_key_type="IP",
-                        limit=rate_value,
-                    )
-                ),
-                visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
-                    cloud_watch_metrics_enabled=True,
-                    metric_name=f"Custom-RateLimit{rate_value}",
-                    sampled_requests_enabled=True,
-                ),
-            )
-
+            rate_list = self.__rate_list(rate_value)
             waf_rules.append(rate_list)
 
         # 2. Common Rule
         aws_common_excluded_rules = None
         if aws_common_rule_ignore_list:
             aws_common_excluded_rules = [
                 wafv2.CfnWebACL.ExcludedRuleProperty(name=rule_name) for rule_name in aws_common_rule_ignore_list
             ]
         if aws_common_rule:
-            aws_common_rule = wafv2.CfnWebACL.RuleProperty(
-                name="AWS-AWSManagedRulesCommonRuleSet",
-                priority=2,
-                override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
-                statement=wafv2.CfnWebACL.StatementProperty(
-                    managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
-                        excluded_rules=aws_common_excluded_rules,
-                        name="AWSManagedRulesCommonRuleSet",
-                        vendor_name="AWS",
-                    )
-                ),
-                visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
-                    cloud_watch_metrics_enabled=True,
-                    metric_name="AWS-AWSManagedRulesCommonRuleSet",
-                    sampled_requests_enabled=True,
-                ),
-            )
+            aws_common_rule = self.__aws_common_rule(aws_common_excluded_rules)
             waf_rules.append(aws_common_rule)
 
         if aws_anony_list:
             # 3. AnonymousIpList
-            aws_anony_list = wafv2.CfnWebACL.RuleProperty(
-                name="AWS-AWSManagedRulesAnonymousIpList",
-                priority=3,
-                override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
-                statement=wafv2.CfnWebACL.StatementProperty(
-                    managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
-                        name="AWSManagedRulesAnonymousIpList",
-                        vendor_name="AWS",
-                    )
-                ),
-                visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
-                    cloud_watch_metrics_enabled=True,
-                    metric_name="AWS-AWSManagedRulesAnonymousIpList",
-                    sampled_requests_enabled=True,
-                ),
-            )
+            aws_anony_list = self.__aws_anonymous_list()
             waf_rules.append(aws_anony_list)
 
         if aws_bad_inputs_rule:
             # 4. Known Bad Inputs Rule
-            aws_bad_inputs_rule = wafv2.CfnWebACL.RuleProperty(
-                name="AWS-AWSManagedRulesKnownBadInputsRuleSet",
-                priority=4,
-                override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
-                statement=wafv2.CfnWebACL.StatementProperty(
-                    managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
-                        name="AWSManagedRulesKnownBadInputsRuleSet",
-                        vendor_name="AWS",
-                    )
-                ),
-                visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
-                    cloud_watch_metrics_enabled=True,
-                    metric_name="AWS-AWSManagedRulesKnownBadInputsRuleSet",
-                    sampled_requests_enabled=True,
-                ),
-            )
+            aws_bad_inputs_rule = self.__aws_bad_inputs_rule()
             waf_rules.append(aws_bad_inputs_rule)
 
         if aws_sqli_rule:
             # 5. SQLi Rule
-            aws_sqli_rule = wafv2.CfnWebACL.RuleProperty(
-                name="AWS-AWSManagedRulesSQLiRuleSet",
-                priority=5,
-                override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
-                statement=wafv2.CfnWebACL.StatementProperty(
-                    managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
-                        name="AWSManagedRulesSQLiRuleSet",
-                        vendor_name="AWS",
-                    )
-                ),
-                visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
-                    cloud_watch_metrics_enabled=True,
-                    metric_name="AWS-AWSManagedRulesSQLiRuleSet",
-                    sampled_requests_enabled=True,
-                ),
-            )
+            aws_sqli_rule = self.__aws_sqli_rule()
             waf_rules.append(aws_sqli_rule)
 
         if aws_account_takeover_prevention:
             # 6. Account takeover prevention
-            aws_account_takeover_prevention_rule = wafv2.CfnWebACL.RuleProperty(
-                name="AWS-AWSManagedRulesATPRuleSet",
-                priority=6,
-                override_action=wafv2.CfnWebACL.OverrideActionProperty(none={}),
-                statement=wafv2.CfnWebACL.StatementProperty(
-                    managed_rule_group_statement=wafv2.CfnWebACL.ManagedRuleGroupStatementProperty(
-                        name="AWSManagedRulesATPRuleSet",
-                        vendor_name="AWS",
-                        managed_rule_group_configs=[
-                            wafv2.CfnWebACL.ManagedRuleGroupConfigProperty(
-                                login_path=aws_account_takeover_prevention["login_path"],  # type: ignore
-                            ),
-                            wafv2.CfnWebACL.ManagedRuleGroupConfigProperty(
-                                password_field=wafv2.CfnWebACL.FieldIdentifierProperty(
-                                    identifier=aws_account_takeover_prevention["password_field"]  # type: ignore
-                                ),
-                            ),
-                            wafv2.CfnWebACL.ManagedRuleGroupConfigProperty(
-                                payload_type="FORM_ENCODED",
-                            ),
-                            wafv2.CfnWebACL.ManagedRuleGroupConfigProperty(
-                                username_field=wafv2.CfnWebACL.FieldIdentifierProperty(
-                                    identifier=aws_account_takeover_prevention["username_field"]  # type: ignore
-                                ),
-                            ),
-                        ],
-                    )
-                ),
-                visibility_config=wafv2.CfnWebACL.VisibilityConfigProperty(
-                    cloud_watch_metrics_enabled=True,
-                    metric_name="AWS-AWSManagedRulesATPRuleSet",
-                    sampled_requests_enabled=True,
-                ),
+            aws_account_takeover_prevention_rule = self.__aws_account_takeover_prevention(
+                aws_account_takeover_prevention
             )
             waf_rules.append(aws_account_takeover_prevention_rule)
 
         return wafv2.CfnWebACL(
             self,
             "WAF ACL",
             default_action=wafv2.CfnWebACL.DefaultActionProperty(allow={}),
@@ -229,21 +258,20 @@
         :param resource_arn: The ARN of resource that will be protected by WAF
         :param web_acl_arn: The WEB Application Access Control List ARN
         :return: wafv2.CfnWebACLAssociation
         """
         return wafv2.CfnWebACLAssociation(self, "ACLAssociation", resource_arn=resource_arn, web_acl_arn=web_acl_arn)
 
     def web_acl_log(self, web_acl_arn: str, log_group_name: str) -> wafv2.CfnLoggingConfiguration:
-        """Configure provided log group as a target for WAF log destination.
+        """Configure provided a log group as a target for WAF log destination.
 
         :param web_acl_arn: The WEB Application Access Control List ARN
         :param log_group_name: The name of log group
-        :return: AWS CDK wafv2.CfnLoggingConfiguration
+        :return: AWS CDK WAFv2.CfnLoggingConfiguration
         """
-
         log_group = logs.LogGroup(
             self,
             id="web_acl_log_group",
             log_group_name=log_group_name,
             retention=logs.RetentionDays.ONE_WEEK,
             removal_policy=cdk.RemovalPolicy.DESTROY,
         )
```

### Comparing `cdk-opinionated-constructs-2.1.2/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/setup.cfg` & `cdk-opinionated-constructs-2.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/setup.py` & `cdk-opinionated-constructs-2.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 https://packaging.python.org/en/latest/distributing.html
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="cdk-opinionated-constructs",
-    version="2.1.2",
+    version="2.1.3",
     description="AWS CDK constructs come without added security configurations.",
     long_description="The idea behind this project is to create secured constructs from the start. \n"
     "Supported constructs: ALB, ECR, LMB, NLB, S3, SNS, WAF, RDS",
     license="MIT",
     package_dir={"": "."},
     packages=find_packages(where="."),
     install_requires=[
```

### Comparing `cdk-opinionated-constructs-2.1.2/test/app.py` & `cdk-opinionated-constructs-2.1.3/test/app.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/alb_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/ecr_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/lmb_docker_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/lmb_docker_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/lmb_monitoring_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/lmb_monitoring_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/lmb_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/nlb_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/nlb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/rds_mysql_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/rds_mysql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/rds_postgresql_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/rds_postgresql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/s3_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/sns_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/stacks/wafv2_stack.py` & `cdk-opinionated-constructs-2.1.3/test/stacks/wafv2_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/unit/test_alb_stack.py` & `cdk-opinionated-constructs-2.1.3/test/unit/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/unit/test_ecr_stack.py` & `cdk-opinionated-constructs-2.1.3/test/unit/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/unit/test_lmb_stack.py` & `cdk-opinionated-constructs-2.1.3/test/unit/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/unit/test_s3_stack.py` & `cdk-opinionated-constructs-2.1.3/test/unit/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/unit/test_sns_stack.py` & `cdk-opinionated-constructs-2.1.3/test/unit/test_sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.2/test/unit/test_wafv2_stack.py` & `cdk-opinionated-constructs-2.1.3/test/unit/test_wafv2_stack.py`

 * *Files identical despite different names*

