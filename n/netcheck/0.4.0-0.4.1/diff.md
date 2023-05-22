# Comparing `tmp/netcheck-0.4.0.tar.gz` & `tmp/netcheck-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netcheck-0.4.0.tar", max compression
+gzip compressed data, was "netcheck-0.4.1.tar", max compression
```

## Comparing `netcheck-0.4.0.tar` & `netcheck-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-15 09:52:07.646954 netcheck-0.4.0/LICENSE
--rw-r--r--   0        0        0     8655 2023-05-15 09:52:07.646954 netcheck-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/__init__.py
--rw-r--r--   0        0        0     5829 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/cli.py
--rw-r--r--   0        0        0     3790 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/context.py
--rw-r--r--   0        0        0     2374 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/dns.py
--rw-r--r--   0        0        0     2150 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/http.py
--rw-r--r--   0        0        0     4907 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/runner.py
--rw-r--r--   0        0        0     2131 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/validation.py
--rw-r--r--   0        0        0      214 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/version.py
--rw-r--r--   0        0        0      850 2023-05-15 09:52:07.670956 netcheck-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9447 1970-01-01 00:00:00.000000 netcheck-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-22 04:59:55.211509 netcheck-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8655 2023-05-22 04:59:55.211509 netcheck-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/__init__.py
+-rw-r--r--   0        0        0     6019 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/cli.py
+-rw-r--r--   0        0        0     3790 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/context.py
+-rw-r--r--   0        0        0     2374 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/dns.py
+-rw-r--r--   0        0        0     2150 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/http.py
+-rw-r--r--   0        0        0     5730 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/runner.py
+-rw-r--r--   0        0        0     2207 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/validation.py
+-rw-r--r--   0        0        0      214 2023-05-22 04:59:55.223509 netcheck-0.4.1/netcheck/version.py
+-rw-r--r--   0        0        0      868 2023-05-22 04:59:55.235509 netcheck-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9447 1970-01-01 00:00:00.000000 netcheck-0.4.1/PKG-INFO
```

### Comparing `netcheck-0.4.0/LICENSE` & `netcheck-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.0/README.md` & `netcheck-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.0/netcheck/cli.py` & `netcheck-0.4.1/netcheck/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,30 +54,34 @@
         ...,
         "--config",
         "-c",
         exists=True,
         file_okay=True,
         help="Config file with netcheck assertions",
     ),
-    output: Optional[NetcheckOutputType] = typer.Option(
-        NetcheckOutputType.json, "-o", "--output", help="Output format"
-    ),
+    # output: Optional[NetcheckOutputType] = typer.Option(
+    #     NetcheckOutputType.json, "-o", "--output", help="Output format"
+    # ),
     verbose: bool = typer.Option(False, "-v", "--verbose"),
+    disable_redaction: bool = typer.Option(False, "--disable-redaction", is_flag=True),
 ):
-    """Carry out all network assertions in given config file."""
-    if verbose:
-        err_console.print(f"Loading assertions from {config}")
+    """
+    Carry out all network assertions in given config file.
+
+    """
     with config.open() as f:
         data = json.load(f)
 
     # TODO: Validate the config format once stable
-    overall_results = run_from_config(data, err_console, verbose)
+    overall_results = run_from_config(data, err_console, verbose, disable_redaction)
 
-    if verbose:
-        err_console.print(f"Output type {output}")
+    if not verbose:
+        # Unless we are in verbose mode we strip the context from
+        # the output
+        overall_results.pop("context", None)
 
     print_json(data=overall_results)
 
 
 @app.command()
 def http(
     url: str = typer.Option(
@@ -120,14 +124,15 @@
 
     result = check_individual_assertion(
         NetcheckTestType.http,
         test_config,
         err_console,
         validation_rule,
         verbose=verbose,
+        include_context=True,
     )
 
     output_result(result, should_fail, verbose)
 
 
 def output_result(result, should_fail, verbose):
     failed = result["status"] == "fail"
@@ -175,14 +180,15 @@
 
     result = check_individual_assertion(
         NetcheckTestType.dns,
         test_config,
         err_console,
         validation_rule=validation_rule,
         verbose=verbose,
+        include_context=True,
     )
 
     output_result(result, should_fail, verbose)
 
 
 def notify_for_unexpected_test_result(failed, should_fail, verbose=False):
     if verbose:
```

### Comparing `netcheck-0.4.0/netcheck/context.py` & `netcheck-0.4.1/netcheck/context.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.0/netcheck/dns.py` & `netcheck-0.4.1/netcheck/dns.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.0/netcheck/http.py` & `netcheck-0.4.1/netcheck/http.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.4.0/netcheck/runner.py` & `netcheck-0.4.1/netcheck/runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,37 +11,46 @@
 from netcheck.dns import dns_lookup_check, DEFAULT_DNS_VALIDATION_RULE
 from netcheck.http import http_request_check, DEFAULT_HTTP_VALIDATION_RULE
 from netcheck.context import replace_template, LazyFileLoadingDict
 
 logger = logging.getLogger("netcheck.runner")
 
 
-def run_from_config(netchecks_config: Dict, err_console, verbose: bool = False):
+def run_from_config(
+    netchecks_config: Dict,
+    err_console,
+    verbose: bool = False,
+    include_context: bool = False,
+):
     if verbose:
         err_console.print(f"Loaded {len(netchecks_config['assertions'])} assertions")
+
     overall_results = {
         "type": "netcheck-output",
         "outputVersion": OUTPUT_JSON_VERSION,
         "metadata": {
             "creationTimestamp": datetime.datetime.utcnow().isoformat(),
             "version": NETCHECK_VERSION,
         },
         "assertions": [],
     }
 
     # Load optional external contexts from the config
     context = {}
     for c in netchecks_config.get("contexts", []):
-        # If type is "directory", load the file at "path", parse it as JSON,
-        # then add it to the context using its "name" as the key
         if c["type"] == "file":
+            # load the file at "path", parse it as JSON,
+            # then add it to the context using its "name" as the key
             with open(c["path"], "r") as f:
                 context[c["name"]] = json.load(f)
         elif c["type"] == "inline":
-            context[c["name"]] = c["data"]
+            # Inline contexts are processed for CEL templates
+            inline_context = c["data"]
+            inline_context = replace_template(inline_context, context)
+            context[c["name"]] = inline_context
         elif c["type"] == "directory":
             # Return a Dict like object that lazy loads individual files
             # from the directory (with caching) and add them to the context
             context[c["name"]] = LazyFileLoadingDict(c["path"])
         else:
             logger.warning(f"Unknown context type '{c['type']}'")
 
@@ -57,30 +66,33 @@
             result = check_individual_assertion(
                 rule["type"],
                 rule,
                 err_console=err_console,
                 validation_rule=rule.get("validation"),
                 validation_context=context,
                 verbose=verbose,
+                include_context=include_context,
             )
             assertion_results.append(result)
 
         overall_results["assertions"].append(
             {"name": assertion["name"], "results": assertion_results}
         )
+
     return overall_results
 
 
 def check_individual_assertion(
     test_type: str,
     test_config,
     err_console,
     validation_rule=None,
     validation_context=None,
     verbose=False,
+    include_context=False,
 ):
     match test_type:
         case "dns":
             if verbose:
                 err_console.print(f"DNS check looking up host '{test_config['host']}'")
             test_detail = dns_lookup_check(
                 host=test_config["host"],
@@ -118,14 +130,28 @@
     if validation_context is not None:
         if "data" in validation_context or "spec" in validation_context:
             raise ValueError("validation_context cannot contain a 'data' or 'spec' key")
         test_detail.update(validation_context)
 
     passed = evaluate_cel_with_context(test_detail, validation_rule)
 
+    # Remove the context from the `test_detail` object
+    if not include_context and validation_context is not None:
+        for key in validation_context:
+            if key in test_detail:
+                del test_detail[key]
+
+    # Strip out known sensitive fields
+    if not include_context:
+        for field in {"headers"}:
+            if field in test_detail["spec"]:
+                test_detail["spec"][field] = "REDACTED"
+            if field in test_detail["data"]:
+                test_detail["data"][field] = "REDACTED"
+
     # Add the pass/status to the individual result. We also support an "expected": "fail" option
     # which will cause the test to fail if the validation passes.
     if test_config.get("expected") == "fail":
         test_detail["status"] = "fail" if passed else "pass"
     else:
         test_detail["status"] = "pass" if passed else "fail"
```

### Comparing `netcheck-0.4.0/netcheck/validation.py` & `netcheck-0.4.1/netcheck/validation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 import json
 import logging
 from typing import Dict
 
 import celpy
+import yaml
 from celpy import CELParseError, CELEvalError, json_to_cel
 
 logger = logging.getLogger("netcheck.validation")
 
 
 def evaluate_cel_with_context(context: Dict, validation_rule: str):
     """
@@ -39,14 +40,15 @@
     except CELParseError as e:
         print("Invalid CEL expression. Treating as error.")
         raise ValueError("Invalid CEL expression")
 
     # create the CEL program
     functions = {
         "parse_json": lambda s: json_to_cel(json.loads(s)),
+        "parse_yaml": lambda s: json_to_cel(yaml.safe_load(s)),
         "b64decode": lambda s: base64.b64decode(s).decode("utf-8"),
         "b64encode": lambda s: base64.b64encode(s.encode()).decode(),
     }
     prgm = env.program(ast, functions=functions)
 
     # Set up the context
     activation = celpy.json_to_cel(context)
```

### Comparing `netcheck-0.4.0/pyproject.toml` & `netcheck-0.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netcheck"
-version = "0.4.0"
+version = "0.4.1"
 description = "Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration."
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 packages = [{include = "netcheck"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -21,14 +21,15 @@
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 coveralls = "^3.3.1"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.241"
+black = "^23.3.0"
 
 [tool.ruff]
 line-length = 120
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `netcheck-0.4.0/PKG-INFO` & `netcheck-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netcheck
-Version: 0.4.0
+Version: 0.4.1
 Summary: Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration.
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

