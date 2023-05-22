# Comparing `tmp/django_watch-0.5.2.1-py3-none-any.whl.zip` & `tmp/django_watch-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4010 bytes, number of entries: 7
+Zip file size: 3706 bytes, number of entries: 7
 -rwxr-xr-x  2.0 unx        0 b- defN 20-Jan-27 13:04 django_watch/__init__.py
--rw-rw-r--  2.0 unx     3230 b- defN 23-May-17 17:13 django_watch/middleware.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-May-17 17:14 django_watch-0.5.2.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1902 b- defN 23-May-17 17:14 django_watch-0.5.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-17 17:14 django_watch-0.5.2.1.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       13 b- defN 23-May-17 17:14 django_watch-0.5.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      582 b- defN 23-May-17 17:14 django_watch-0.5.2.1.dist-info/RECORD
-7 files, 6913 bytes uncompressed, 2968 bytes compressed:  57.1%
+-rw-rw-r--  2.0 unx     3151 b- defN 23-May-22 06:33 django_watch/middleware.py
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-May-22 06:36 django_watch-0.5.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1207 b- defN 23-May-22 06:36 django_watch-0.5.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 06:36 django_watch-0.5.3.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       13 b- defN 23-May-22 06:36 django_watch-0.5.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      572 b- defN 23-May-22 06:36 django_watch-0.5.3.dist-info/RECORD
+7 files, 6129 bytes uncompressed, 2684 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: django_watch/__init__.py
 Comment: 
 
 Filename: django_watch/middleware.py
 Comment: 
 
-Filename: django_watch-0.5.2.1.dist-info/LICENSE
+Filename: django_watch-0.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: django_watch-0.5.2.1.dist-info/METADATA
+Filename: django_watch-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: django_watch-0.5.2.1.dist-info/WHEEL
+Filename: django_watch-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: django_watch-0.5.2.1.dist-info/top_level.txt
+Filename: django_watch-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: django_watch-0.5.2.1.dist-info/RECORD
+Filename: django_watch-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_watch/middleware.py

```diff
@@ -46,16 +46,16 @@
             process_stdout_end += f"{self.YELLOW} • STATUS {response.status_code} • Total time • {round((time.monotonic() - time_start), 2)}s{self.END}"        
             print(process_stdout_end)
         return response
 
     def process_view(self, request, func, args, kwargs):                 
         func = unwrap(func)   
         if hasattr(func, "__code__"):
-            process_stdout_start = f"\n░░ {self.GREEN}START {request.method} {func.__code__.co_filename} {self.END} • {self.GREEN}{self.BOLD}{func.__name__}{self.END}{self.END} {self.GREEN}•{self.END} {self.GREEN}Line number {func.__code__.co_firstlineno}{self.END}"
-            request.process_stdout_end = f"\n░░ {self.YELLOW}{self.BOLD}END {request.method} {func.__code__.co_filename} {self.END} • {self.YELLOW}{self.BOLD}{func.__name__}{self.END}{self.END}"
+            process_stdout_start = f"\n░░ {self.BOLD}{request.method} {func.__code__.co_filename} {self.END} • {self.GREEN}{func.__name__}{self.END} • {self.YELLOW}Line number {func.__code__.co_firstlineno}{self.END}"
+            request.process_stdout_end = f"\n░░ {self.BOLD}{request.method} {func.__code__.co_filename} {self.END} • {self.GREEN}{func.__name__} [  OK  ]{self.END}"
             
             print(process_stdout_start)
             if args: 
                 print(f"░░░░ args: {args}"[:200])
             if kwargs: 
                 print(f"░░░░ kwargs: {kwargs}"[:200])
             if request.GET:
```

## Comparing `django_watch-0.5.2.1.dist-info/LICENSE` & `django_watch-0.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

