# Comparing `tmp/snowconvert-helpers-2.0.8.tar.gz` & `tmp/snowconvert-helpers-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowconvert-helpers-2.0.8.tar", last modified: Fri Oct 15 15:23:22 2021, max compression
+gzip compressed data, was "snowconvert-helpers-2.0.9.tar", last modified: Mon Oct 18 20:36:13 2021, max compression
```

## Comparing `snowconvert-helpers-2.0.8.tar` & `snowconvert-helpers-2.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-10-15 15:23:22.975765 snowconvert-helpers-2.0.8/
--rw-rw-rw-   0        0        0      620 2021-10-15 15:22:08.000000 snowconvert-helpers-2.0.8/LICENSE
--rw-rw-rw-   0        0        0     5131 2021-10-15 15:23:22.975765 snowconvert-helpers-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3914 2021-10-15 15:22:08.000000 snowconvert-helpers-2.0.8/README.md
--rw-rw-rw-   0        0        0      142 2021-10-15 15:23:22.975765 snowconvert-helpers-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2480 2021-10-15 15:22:08.000000 snowconvert-helpers-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-15 15:23:22.960140 snowconvert-helpers-2.0.8/snowconvert/
--rw-rw-rw-   0        0        0       80 2021-10-15 15:23:21.000000 snowconvert-helpers-2.0.8/snowconvert/__init__.py
--rw-rw-rw-   0        0        0    31727 2021-10-15 15:22:08.000000 snowconvert-helpers-2.0.8/snowconvert/helpers.py
-drwxrwxrwx   0        0        0        0 2021-10-15 15:23:22.975765 snowconvert-helpers-2.0.8/snowconvert_helpers.egg-info/
--rw-rw-rw-   0        0        0     5131 2021-10-15 15:23:22.000000 snowconvert-helpers-2.0.8/snowconvert_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2021-10-15 15:23:22.000000 snowconvert-helpers-2.0.8/snowconvert_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-15 15:23:22.000000 snowconvert-helpers-2.0.8/snowconvert_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2021-10-15 15:23:22.000000 snowconvert-helpers-2.0.8/snowconvert_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-10-15 15:23:22.000000 snowconvert-helpers-2.0.8/snowconvert_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-10-18 20:36:13.983042 snowconvert-helpers-2.0.9/
+-rw-rw-rw-   0        0        0      620 2021-10-18 20:34:50.000000 snowconvert-helpers-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5227 2021-10-18 20:36:13.983042 snowconvert-helpers-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4010 2021-10-18 20:34:50.000000 snowconvert-helpers-2.0.9/README.md
+-rw-rw-rw-   0        0        0      142 2021-10-18 20:36:13.983042 snowconvert-helpers-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2480 2021-10-18 20:34:50.000000 snowconvert-helpers-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-18 20:36:13.983042 snowconvert-helpers-2.0.9/snowconvert/
+-rw-rw-rw-   0        0        0       80 2021-10-18 20:36:12.000000 snowconvert-helpers-2.0.9/snowconvert/__init__.py
+-rw-rw-rw-   0        0        0    31841 2021-10-18 20:34:50.000000 snowconvert-helpers-2.0.9/snowconvert/helpers.py
+drwxrwxrwx   0        0        0        0 2021-10-18 20:36:13.983042 snowconvert-helpers-2.0.9/snowconvert_helpers.egg-info/
+-rw-rw-rw-   0        0        0     5227 2021-10-18 20:36:13.000000 snowconvert-helpers-2.0.9/snowconvert_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2021-10-18 20:36:13.000000 snowconvert-helpers-2.0.9/snowconvert_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-10-18 20:36:13.000000 snowconvert-helpers-2.0.9/snowconvert_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2021-10-18 20:36:13.000000 snowconvert-helpers-2.0.9/snowconvert_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2021-10-18 20:36:13.000000 snowconvert-helpers-2.0.9/snowconvert_helpers.egg-info/top_level.txt
```

### Comparing `snowconvert-helpers-2.0.8/LICENSE` & `snowconvert-helpers-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snowconvert-helpers-2.0.8/PKG-INFO` & `snowconvert-helpers-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowconvert-helpers
-Version: 2.0.8
+Version: 2.0.9
 Summary: Migration helpers for Mobilize SnowConvert for Teradata.
 Home-page: https://docs.mobilize.net/snowconvert/for-teradata/introduction
 Author: Mobilize.Net
 Author-email: info@mobilize.com
 License: Proprietary License (Copyright (C) Mobilize.Net - All Rights Reserved)
 Keywords: Mobilize,Snowflake,Teradata,BTEQ,FastLoad,MultiLoad,TPT,TPump,database,cloud
 Platform: UNKNOWN
@@ -41,14 +41,17 @@
 > [Mobilize.Net SnowConvert for Teradata Product](https://www.mobilize.net/products/database-migrations/teradata-to-snowflake)
 
 > [Mobilize.Net SnowConvert for Teradata Documentation](https://docs.mobilize.net/snowconvert/for-teradata/introduction)
 
 > [User Guide for snowconvert-helpers](https://docs.mobilize.net/snowconvert-limited-access/-MUuBuIkrrZbtDaKcru_/for-teradata/translation-reference/scripts-translation-reference/snowconvert-scripts-helpers)
 
 ## Release Notes
+* v2.0.9 (October 18, 2021)
+  > * _Fix for SNOW_DEBUG_COLOR usage when logging is disabled.
+
 * v2.0.8 (October 15, 2021)
   > * _Adding posiblity to configure python logging for snowconvert-helpers
 
 * v2.0.7 (September 9, 2021)
   > * _Updating User Guide documentation for snowconvert-helpers
 
 * v2.0.6 (July 23, 2021)
```

### Comparing `snowconvert-helpers-2.0.8/README.md` & `snowconvert-helpers-2.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 > [Mobilize.Net SnowConvert for Teradata Product](https://www.mobilize.net/products/database-migrations/teradata-to-snowflake)
 
 > [Mobilize.Net SnowConvert for Teradata Documentation](https://docs.mobilize.net/snowconvert/for-teradata/introduction)
 
 > [User Guide for snowconvert-helpers](https://docs.mobilize.net/snowconvert-limited-access/-MUuBuIkrrZbtDaKcru_/for-teradata/translation-reference/scripts-translation-reference/snowconvert-scripts-helpers)
 
 ## Release Notes
+* v2.0.9 (October 18, 2021)
+  > * _Fix for SNOW_DEBUG_COLOR usage when logging is disabled.
+
 * v2.0.8 (October 15, 2021)
   > * _Adding posiblity to configure python logging for snowconvert-helpers
 
 * v2.0.7 (September 9, 2021)
   > * _Updating User Guide documentation for snowconvert-helpers
 
 * v2.0.6 (July 23, 2021)
```

### Comparing `snowconvert-helpers-2.0.8/setup.py` & `snowconvert-helpers-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `snowconvert-helpers-2.0.8/snowconvert/helpers.py` & `snowconvert-helpers-2.0.9/snowconvert/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,18 @@
             logging.debug(finalmsg)
         elif level == logging.WARNING:
             logging.warning(finalmsg)
         else:
             logging.info(finalmsg)
 
     else :
-        print(msg, file=writter)
+        finalmsg = ""
+        for item in msg :
+            finalmsg += str(item)
+        print(finalmsg, file=writter)
 
 def get_from_vars_or_args_or_environment(arg_pos, variable_name, vars, args):
     """Gets the argument from the position specified or gets the value from the table vars or gets the environment variable name passed.
 
         arg_pos
             The argument position to be used from the arguments parameter.
         variable_name
@@ -290,15 +293,15 @@
             login_timeout=login_timeout,
             session_parameters={
                 'QUERY_TAG': query_tag
             }
         )
     except Exception as e:
         print(e)
-        log(colored('*** Failure: logon failed :', 'red') + str(e), level = logging.ERROR, writter = sys.stderr)
+        log(f"{colored('*** Failure: logon failed :', 'red')} { str(e) }", level = logging.ERROR, writter = sys.stderr)
         error_code = 333
         quit_application(error_code)
     if c:
         opened_connections.append(c)
         error_code = 0
     return c
 
@@ -371,19 +374,19 @@
     if (con is None):
         # get last connection
         con = opened_connections[-1]
 
     cur = con.cursor()
     try:
         error_code = 0
-        log(colored("Executing: ") + colored(sql_string, 'cyan'))
+        log(f"{colored('Executing: ')} { colored(sql_string, 'cyan') }")
         if ("$" in sql_string or "&" in sql_string):
             log ("Expanding variables in SQL statement")
             sql_string = expandvars(sql_string, passed_variables)
-            log (colored("Expanded string: ") + colored(sql_string, 'green'))
+            log (f"{colored('Expanded string: ')} {colored(sql_string, 'green')}")
         if (using is not None):
                 #we need to change variables from {var} to %(format)
                 sql_string = re.sub(r'\{([^}]*)\}', r'%(\1)', sql_string)
                 log(f"using parameters {using}")
         cur.execute(sql_string, params=using)
         activity_count = cur.rowcount
         if activity_count and activity_count >= 1:
@@ -453,25 +456,25 @@
         sql_lines = sql_string.splitlines()
         last_line = -1       
         for matchNum, match in enumerate(matches, start=1):
                 line = int(match.groups()[0])-1
                 column = int(match.groups()[1])
                 if line != last_line:
                     error_line = sql_lines[line]
-                    error_line = error_line[:column] + colored(error_line[column:], 'red')
+                    error_line = f"{error_line[:column]} {colored(error_line[column:], 'red')}"
                     error_fragment = error_fragment + f"{line:0>2d},{column:0>2d}:{error_line}\n"
                 last_line = line
         log(error_fragment, level = logging.ERROR)
     _handle_sql_error(e)
 
 def _handle_sql_error(e):
     global error_code, error_level
     error_code = e.errno
     if error_code not in _severities_dictionary or _severities_dictionary[error_code] != 0:
-        msg = colored("*** Failure " + str(e), 'red')
+        msg = colored(f"*** Failure {str(e)}", 'red')
         log(msg, level = logging.ERROR, writter = sys.stderr)
         if error_code in _severities_dictionary:
             error_level = max(error_level, _severities_dictionary[error_code])
         else:
             error_level = max(error_level, _default_error_level)
 
 @singledispatch
```

### Comparing `snowconvert-helpers-2.0.8/snowconvert_helpers.egg-info/PKG-INFO` & `snowconvert-helpers-2.0.9/snowconvert_helpers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowconvert-helpers
-Version: 2.0.8
+Version: 2.0.9
 Summary: Migration helpers for Mobilize SnowConvert for Teradata.
 Home-page: https://docs.mobilize.net/snowconvert/for-teradata/introduction
 Author: Mobilize.Net
 Author-email: info@mobilize.com
 License: Proprietary License (Copyright (C) Mobilize.Net - All Rights Reserved)
 Keywords: Mobilize,Snowflake,Teradata,BTEQ,FastLoad,MultiLoad,TPT,TPump,database,cloud
 Platform: UNKNOWN
@@ -41,14 +41,17 @@
 > [Mobilize.Net SnowConvert for Teradata Product](https://www.mobilize.net/products/database-migrations/teradata-to-snowflake)
 
 > [Mobilize.Net SnowConvert for Teradata Documentation](https://docs.mobilize.net/snowconvert/for-teradata/introduction)
 
 > [User Guide for snowconvert-helpers](https://docs.mobilize.net/snowconvert-limited-access/-MUuBuIkrrZbtDaKcru_/for-teradata/translation-reference/scripts-translation-reference/snowconvert-scripts-helpers)
 
 ## Release Notes
+* v2.0.9 (October 18, 2021)
+  > * _Fix for SNOW_DEBUG_COLOR usage when logging is disabled.
+
 * v2.0.8 (October 15, 2021)
   > * _Adding posiblity to configure python logging for snowconvert-helpers
 
 * v2.0.7 (September 9, 2021)
   > * _Updating User Guide documentation for snowconvert-helpers
 
 * v2.0.6 (July 23, 2021)
```

