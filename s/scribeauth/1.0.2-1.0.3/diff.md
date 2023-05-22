# Comparing `tmp/scribeauth-1.0.2-py3-none-any.whl.zip` & `tmp/scribeauth-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 5988 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       66 b- defN 22-Jul-26 14:43 scribeauth/__init__.py
+Zip file size: 6738 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       66 b- defN 23-May-17 09:44 scribeauth/__init__.py
 -rw-rw-rw-  2.0 fat      521 b- defN 22-Jul-27 09:39 scribeauth/__main__.py
--rw-rw-rw-  2.0 fat     8684 b- defN 22-Aug-12 14:26 scribeauth/scribeauth.py
--rw-rw-rw-  2.0 fat     1097 b- defN 22-Aug-12 14:27 scribeauth-1.0.2.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     3654 b- defN 22-Aug-12 14:27 scribeauth-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Aug-12 14:27 scribeauth-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 22-Aug-12 14:27 scribeauth-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      640 b- defN 22-Aug-12 14:27 scribeauth-1.0.2.dist-info/RECORD
-8 files, 14765 bytes uncompressed, 4868 bytes compressed:  67.0%
+-rw-rw-rw-  2.0 fat     8718 b- defN 23-May-17 16:30 scribeauth/scribeauth.py
+-rw-rw-rw-  2.0 fat     1351 b- defN 23-May-15 17:21 scribeauth/scribeauthfederation.py
+-rw-rw-rw-  2.0 fat     1097 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     3719 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      731 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/RECORD
+9 files, 16306 bytes uncompressed, 5474 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: scribeauth/__main__.py
 Comment: 
 
 Filename: scribeauth/scribeauth.py
 Comment: 
 
-Filename: scribeauth-1.0.2.dist-info/LICENSE.md
+Filename: scribeauth/scribeauthfederation.py
 Comment: 
 
-Filename: scribeauth-1.0.2.dist-info/METADATA
+Filename: scribeauth-1.0.3.dist-info/LICENSE.md
 Comment: 
 
-Filename: scribeauth-1.0.2.dist-info/WHEEL
+Filename: scribeauth-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: scribeauth-1.0.2.dist-info/top_level.txt
+Filename: scribeauth-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: scribeauth-1.0.2.dist-info/RECORD
+Filename: scribeauth-1.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: scribeauth-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scribeauth/scribeauth.py

```diff
@@ -56,19 +56,21 @@
 
     def change_password(self, username: str, password: str, new_password: str) -> bool: # pragma: no cover
         """Creates a new password for a user.
 
         Args
         ----
         username -- Username (usually an email address).
+
         password -- Password associated with this username.
+
         new_password -- New password for this username.
         
         Returns
-        ----
+        -------
         bool
         """
         try:
             response_initiate = self.__initiate_auth(username, password)
         except Exception:
             raise UnauthorizedException("Username and/or Password are incorrect")
         challenge_name = response_initiate.get('ChallengeName')
@@ -95,19 +97,21 @@
 
     def forgot_password(self, username: str, password: str, confirmation_code: str) -> bool: # pragma: no cover
         """Allows a user to enter a confirmation code sent to their email to reset a forgotten password.
 
         Args
         ----
         username -- Username (usually an email address).
+
         password -- Password associated with this username.
+        
         confirmation_code -- Confirmation code sent to the user's email.
         
         Returns
-        ----
+        -------
         bool
         """
         try:
             self.client_signed.confirm_forgot_password(
                 ClientId=self.client_id,
                 Username=username,
                 ConfirmationCode=confirmation_code,
@@ -119,20 +123,23 @@
 
     def get_tokens(self, **param: Unpack[UsernamePassword] | Unpack[RefreshToken]) -> Tokens:
         """A user gets their tokens (refresh_token, access_token and id_token).
 
         Args
         ----
         username -- Username (usually an email address).
+
         password -- Password associated with this username.
+
         Or
+
         refresh_token -- Refresh token to use.
         
         Returns
-        ----
+        -------
         Tokens -- Dictionary {"refresh_token": "str", "access_token": "str", "id_token": "str"}
         """
         auth_result = 'AuthenticationResult'
         refresh_token = param.get('refresh_token')
         if refresh_token == None:
             username = param.get('username')
             password = param.get('password')
@@ -167,15 +174,15 @@
         After the token is revoked, the user cannot use the revoked token.
 
         Args
         ----
         refresh_token -- Refresh token to be revoked.
         
         Returns
-        ----
+        -------
         bool
         """
         response = self.__revoke_token(refresh_token)
         status_code = response.get('ResponseMetadata').get('HTTPStatusCode')
         if(status_code == 200):
             return True
         if(status_code == 400): # pragma: no cover
```

## Comparing `scribeauth-1.0.2.dist-info/LICENSE.md` & `scribeauth-1.0.3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `scribeauth-1.0.2.dist-info/METADATA` & `scribeauth-1.0.3.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,106 +1,102 @@
-Metadata-Version: 2.1
-Name: scribeauth
-Version: 1.0.2
-Summary: Library to authenticate to Scribe's platform
-Home-page: https://github.com/ScribeLabsAI/ScribeAuth
-Author: Ailin Venerus
-Author-email: ailin@scribelabs.ai
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Security
-Classifier: Typing :: Typed
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: boto3
-Requires-Dist: typing-extensions
-
-# Scribe Auth
-
-Most calls to Scribe's API require authentication and authorization. This library simplifies this process.
-
-You first need a Scribe account and a client ID. Both can be requested at support[atsign]scribelabs[dotsign]ai or through Intercom on https://platform.scribelabs.ai if you already have a Scribe account.
-
-This library interacts directly with our authentication provider [AWS Cognito](https://aws.amazon.com/cognito/) meaning that your username and password never transit through our servers.
-
-## Installation
-
-```bash
-pip install scribeauth
-```
-
-This library requires Python >= 3.10 that supports typings.
-
-## Methods
-
-### 1. Changing password
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.change_password('username', 'password', 'new_password')
-```
-
-### 2. Recovering an account in case of forgotten password
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.forgot_password('username', 'password', 'confirmation_code')
-```
-
-### 3. Get or generate tokens
-
-##### With username and password
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.get_tokens(username='username', password='password')
-```
-
-##### With refresh token
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.get_tokens(refresh_token='refresh_token')
-```
-
-### 4. Revoking a refresh token
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.revoke_refresh_token('refresh_token')
-```
-
-## Flow
-
-- If you never have accessed your Scribe account, it probably still contains the temporary password we generated for you. You can change it directly on the [platform](https://platform.scribelabs.ai) or with the `change_password` method. You won't be able to access anything else until the temporary password has been changed.
-
-- Once the account is up and running, you can request new tokens with `get_tokens`. You will initially have to provide your username and password. The access and id tokens are valid for up to 30 minutes. The refresh token is valid for 30 days.
-
-- While you have a valid refresh token, you can request fresh access and id tokens with `get_tokens` but using the refresh token this time, so you're not sending your username and password over the wire anymore.
-
-- In case you suspect that your refresh token has been leaked, you can revoke it with `revoke_token`. This will also invalidate any access/id token that has been issued with it. In order to get a new one, you'll need to use your username and password again.
-
-## Command line
-
-You can also use the package as follows for quick access to tokens:
-
-```bash
-python -m scribeauth --client_id clientid --username username --password password
-```
-
----
-
-To flag an issue, open a ticket on [Github](https://github.com/ScribeLabsAI/ScribeAuth/issues) and contact us on Intercom through the platform.
-
-
+Metadata-Version: 2.1
+Name: scribeauth
+Version: 1.0.3
+Summary: Library to authenticate to Scribe's platform
+Home-page: https://github.com/ScribeLabsAI/ScribeAuth
+Author: Ailin Venerus
+Author-email: ailin@scribelabs.ai
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Security
+Classifier: Typing :: Typed
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: boto3
+Requires-Dist: typing-extensions
+
+# Scribe Auth
+
+Most calls to Scribe's API require authentication and authorization. This library simplifies this process.
+
+You first need a Scribe account and a client ID. Both can be requested at support[atsign]scribelabs[dotsign]ai or through Intercom on https://platform.scribelabs.ai if you already have a Scribe account.
+
+This library interacts directly with our authentication provider [AWS Cognito](https://aws.amazon.com/cognito/) meaning that your username and password never transit through our servers.
+
+## Installation
+
+```bash
+pip install scribeauth
+```
+
+This library requires Python >= 3.10 that supports typings.
+
+## Methods
+
+### 1. Changing password
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.change_password('username', 'password', 'new_password')
+```
+
+### 2. Recovering an account in case of forgotten password
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.forgot_password('username', 'password', 'confirmation_code')
+```
+
+### 3. Get or generate tokens
+
+##### With username and password
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.get_tokens(username='username', password='password')
+```
+
+##### With refresh token
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.get_tokens(refresh_token='refresh_token')
+```
+
+### 4. Revoking a refresh token
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.revoke_refresh_token('refresh_token')
+```
+
+## Flow
+
+- If you never have accessed your Scribe account, it probably still contains the temporary password we generated for you. You can change it directly on the [platform](https://platform.scribelabs.ai) or with the `change_password` method. You won't be able to access anything else until the temporary password has been changed.
+
+- Once the account is up and running, you can request new tokens with `get_tokens`. You will initially have to provide your username and password. The access and id tokens are valid for up to 30 minutes. The refresh token is valid for 30 days.
+
+- While you have a valid refresh token, you can request fresh access and id tokens with `get_tokens` but using the refresh token this time, so you're not sending your username and password over the wire anymore.
+
+- In case you suspect that your refresh token has been leaked, you can revoke it with `revoke_token`. This will also invalidate any access/id token that has been issued with it. In order to get a new one, you'll need to use your username and password again.
+
+## Command line
+
+You can also use the package as follows for quick access to tokens:
+
+```bash
+python -m scribeauth --client_id clientid --username username --password password
+```
+
+---
+
+To flag an issue, open a ticket on [Github](https://github.com/ScribeLabsAI/ScribeAuth/issues) and contact us on Intercom through the platform.
```

