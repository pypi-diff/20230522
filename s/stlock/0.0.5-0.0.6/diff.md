# Comparing `tmp/stlock-0.0.5.tar.gz` & `tmp/stlock-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlock-0.0.5.tar", last modified: Mon May 22 19:44:39 2023, max compression
+gzip compressed data, was "stlock-0.0.6.tar", last modified: Mon May 22 19:49:41 2023, max compression
```

## Comparing `stlock-0.0.5.tar` & `stlock-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:44:39.084804 stlock-0.0.5/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3238 2023-05-22 19:44:39.084804 stlock-0.0.5/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3093 2023-05-22 19:40:10.000000 stlock-0.0.5/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-22 19:44:39.084804 stlock-0.0.5/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      402 2023-05-22 19:44:34.000000 stlock-0.0.5/setup.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:44:39.084804 stlock-0.0.5/stlock/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.5/stlock/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2149 2023-05-22 17:38:41.000000 stlock-0.0.5/stlock/stlock.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:44:39.084804 stlock-0.0.5/stlock.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3238 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.5/stlock.egg-info/not-zip-safe
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-22 19:44:39.000000 stlock-0.0.5/stlock.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:49:41.781059 stlock-0.0.6/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3255 2023-05-22 19:49:41.781059 stlock-0.0.6/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3110 2023-05-22 19:49:35.000000 stlock-0.0.6/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-22 19:49:41.781059 stlock-0.0.6/setup.cfg
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      402 2023-05-22 19:49:40.000000 stlock-0.0.6/setup.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:49:41.781059 stlock-0.0.6/stlock/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.6/stlock/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2149 2023-05-22 17:38:41.000000 stlock-0.0.6/stlock/stlock.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:49:41.781059 stlock-0.0.6/stlock.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3255 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.6/stlock.egg-info/not-zip-safe
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/top_level.txt
```

### Comparing `stlock-0.0.5/PKG-INFO` & `stlock-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlock
-Version: 0.0.5
+Version: 0.0.6
 Summary: oauth2.0 stlock
 Author-email: office@stl.im
 Description-Content-Type: text/markdown
 
 # Библиотека Python stlock
 
 
@@ -16,15 +16,15 @@
 pip install stlock
 pip install fastapi
 pip install uvicorn
 ```
 
 app.py:
 ```
-from fastapi import FastAPI, HTTPException, Body
+from fastapi import FastAPI, HTTPException, Body, Query
 from stlock import AuthClient
 
 
 # создание экземпляра класса
 AC = AuthClient(client_id="client",  # id клиента
     client_secret="secret",  # secret клиента
     code_redirect_uri="http://localhost:8000/code",  # ссылка перенаправления запроса с кодом
@@ -32,15 +32,15 @@
     )
 
 
 app = FastAPI()
 
 
 # Регистрация пользователя
-@app.post("/register", status_code=status.HTTP_201_CREATED)
+@app.post("/register", status_code=201)
 def register_user(username=Body(...), password=Body(...)):
    data, status_code = AC.register(username, password)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 
 
@@ -49,15 +49,15 @@
 def login(username: str = Body(...), password: str = Body(...)):
    data, status_code = AC.authorize_user(username, password)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 
 
-@apps.get('/code')
+@app.get('/code')
 def getcode(code=Query(None)):
    data, status_code = AC.get_tokens(code)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 ```
 
@@ -97,28 +97,28 @@
     "password": "Password123!"
 }
 ```
 
 Output:
 ```
 {
-   
+    "detail": "User registred"
 }
 ```
 авторизация пользователя:
 ```
 POST http://localhost:8000/login
 Body {
     "username": "user1",
     "password": "Password123!"
 }
 ```
 
 Output:
 ```
 {
-   "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ3NzkyNTUsInN1YiI6IjZiN2Q0YzYxLTJhNzQtNDI3My05MzhjLTRlYTM3MGVjYmIxZSIsInJvbGUiOiJUZXN0In0.bpBW64XSQIFSdGHKt7RD2fWA-wiizk8bjcleTIfMqkg6QMaVtoulm-oyCe1nz_EViv7DQpZXjm82kTeXUzAmTg",
-   "expires_in": 60,
-   "refresh_token": "OGFLNTI1MDCTMWU2OS01MDQXLTHLYTMTYTRKNJMXMJGWNJVH",
-   "token_type": "Bearer"
+    "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ3ODUwMTUsInN1YiI6ImQ5YjBmYjE1LWJjYmQtNDNkNy1hMDdlLTAxNTIwMjBlZWI2ZiIsInJvbGUiOiJUZXN0In0.kOjADrKuTmLW-MGei4VEhf9Ce16eEzgle0UVB-t_vXoMQAtMQVzdI6iK14Rmds2w1bUMh82Wwru_AmMYS2NYYQ",
+    "expires_in": 60,
+    "refresh_token": "ZDI5ZMUZNDETNZYYZI01OTUZLTK5MZKTNJVLMDU1OTA5MDFM",
+    "token_type": "Bearer"
 }
 ```
```

### Comparing `stlock-0.0.5/README.md` & `stlock-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pip install stlock
 pip install fastapi
 pip install uvicorn
 ```
 
 app.py:
 ```
-from fastapi import FastAPI, HTTPException, Body
+from fastapi import FastAPI, HTTPException, Body, Query
 from stlock import AuthClient
 
 
 # создание экземпляра класса
 AC = AuthClient(client_id="client",  # id клиента
     client_secret="secret",  # secret клиента
     code_redirect_uri="http://localhost:8000/code",  # ссылка перенаправления запроса с кодом
@@ -25,15 +25,15 @@
     )
 
 
 app = FastAPI()
 
 
 # Регистрация пользователя
-@app.post("/register", status_code=status.HTTP_201_CREATED)
+@app.post("/register", status_code=201)
 def register_user(username=Body(...), password=Body(...)):
    data, status_code = AC.register(username, password)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 
 
@@ -42,15 +42,15 @@
 def login(username: str = Body(...), password: str = Body(...)):
    data, status_code = AC.authorize_user(username, password)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 
 
-@apps.get('/code')
+@app.get('/code')
 def getcode(code=Query(None)):
    data, status_code = AC.get_tokens(code)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 ```
 
@@ -90,28 +90,28 @@
     "password": "Password123!"
 }
 ```
 
 Output:
 ```
 {
-   
+    "detail": "User registred"
 }
 ```
 авторизация пользователя:
 ```
 POST http://localhost:8000/login
 Body {
     "username": "user1",
     "password": "Password123!"
 }
 ```
 
 Output:
 ```
 {
-   "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ3NzkyNTUsInN1YiI6IjZiN2Q0YzYxLTJhNzQtNDI3My05MzhjLTRlYTM3MGVjYmIxZSIsInJvbGUiOiJUZXN0In0.bpBW64XSQIFSdGHKt7RD2fWA-wiizk8bjcleTIfMqkg6QMaVtoulm-oyCe1nz_EViv7DQpZXjm82kTeXUzAmTg",
-   "expires_in": 60,
-   "refresh_token": "OGFLNTI1MDCTMWU2OS01MDQXLTHLYTMTYTRKNJMXMJGWNJVH",
-   "token_type": "Bearer"
+    "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ3ODUwMTUsInN1YiI6ImQ5YjBmYjE1LWJjYmQtNDNkNy1hMDdlLTAxNTIwMjBlZWI2ZiIsInJvbGUiOiJUZXN0In0.kOjADrKuTmLW-MGei4VEhf9Ce16eEzgle0UVB-t_vXoMQAtMQVzdI6iK14Rmds2w1bUMh82Wwru_AmMYS2NYYQ",
+    "expires_in": 60,
+    "refresh_token": "ZDI5ZMUZNDETNZYYZI01OTUZLTK5MZKTNJVLMDU1OTA5MDFM",
+    "token_type": "Bearer"
 }
 ```
```

### Comparing `stlock-0.0.5/stlock/stlock.py` & `stlock-0.0.6/stlock/stlock.py`

 * *Files identical despite different names*

### Comparing `stlock-0.0.5/stlock.egg-info/PKG-INFO` & `stlock-0.0.6/stlock.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlock
-Version: 0.0.5
+Version: 0.0.6
 Summary: oauth2.0 stlock
 Author-email: office@stl.im
 Description-Content-Type: text/markdown
 
 # Библиотека Python stlock
 
 
@@ -16,15 +16,15 @@
 pip install stlock
 pip install fastapi
 pip install uvicorn
 ```
 
 app.py:
 ```
-from fastapi import FastAPI, HTTPException, Body
+from fastapi import FastAPI, HTTPException, Body, Query
 from stlock import AuthClient
 
 
 # создание экземпляра класса
 AC = AuthClient(client_id="client",  # id клиента
     client_secret="secret",  # secret клиента
     code_redirect_uri="http://localhost:8000/code",  # ссылка перенаправления запроса с кодом
@@ -32,15 +32,15 @@
     )
 
 
 app = FastAPI()
 
 
 # Регистрация пользователя
-@app.post("/register", status_code=status.HTTP_201_CREATED)
+@app.post("/register", status_code=201)
 def register_user(username=Body(...), password=Body(...)):
    data, status_code = AC.register(username, password)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 
 
@@ -49,15 +49,15 @@
 def login(username: str = Body(...), password: str = Body(...)):
    data, status_code = AC.authorize_user(username, password)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 
 
-@apps.get('/code')
+@app.get('/code')
 def getcode(code=Query(None)):
    data, status_code = AC.get_tokens(code)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 ```
 
@@ -97,28 +97,28 @@
     "password": "Password123!"
 }
 ```
 
 Output:
 ```
 {
-   
+    "detail": "User registred"
 }
 ```
 авторизация пользователя:
 ```
 POST http://localhost:8000/login
 Body {
     "username": "user1",
     "password": "Password123!"
 }
 ```
 
 Output:
 ```
 {
-   "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ3NzkyNTUsInN1YiI6IjZiN2Q0YzYxLTJhNzQtNDI3My05MzhjLTRlYTM3MGVjYmIxZSIsInJvbGUiOiJUZXN0In0.bpBW64XSQIFSdGHKt7RD2fWA-wiizk8bjcleTIfMqkg6QMaVtoulm-oyCe1nz_EViv7DQpZXjm82kTeXUzAmTg",
-   "expires_in": 60,
-   "refresh_token": "OGFLNTI1MDCTMWU2OS01MDQXLTHLYTMTYTRKNJMXMJGWNJVH",
-   "token_type": "Bearer"
+    "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ3ODUwMTUsInN1YiI6ImQ5YjBmYjE1LWJjYmQtNDNkNy1hMDdlLTAxNTIwMjBlZWI2ZiIsInJvbGUiOiJUZXN0In0.kOjADrKuTmLW-MGei4VEhf9Ce16eEzgle0UVB-t_vXoMQAtMQVzdI6iK14Rmds2w1bUMh82Wwru_AmMYS2NYYQ",
+    "expires_in": 60,
+    "refresh_token": "ZDI5ZMUZNDETNZYYZI01OTUZLTK5MZKTNJVLMDU1OTA5MDFM",
+    "token_type": "Bearer"
 }
 ```
```

