# Comparing `tmp/roadtx-1.2.1.tar.gz` & `tmp/roadtx-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadtx-1.2.1.tar", last modified: Tue Mar 21 16:29:04 2023, max compression
+gzip compressed data, was "roadtx-1.3.0.tar", last modified: Mon May 22 14:43:38 2023, max compression
```

## Comparing `roadtx-1.2.1.tar` & `roadtx-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-21 16:29:04.987513 roadtx-1.2.1/
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-03-21 16:29:04.987513 roadtx-1.2.1/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-21 16:29:04.983513 roadtx-1.2.1/roadtools/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-21 16:29:04.983513 roadtx-1.2.1/roadtools/roadtx/
--rw-r--r--   0 vsts      (1001) docker     (123)     7865 2023-03-21 16:27:28.000000 roadtx-1.2.1/roadtools/roadtx/keepass.py
--rw-r--r--   0 vsts      (1001) docker     (123)    45302 2023-03-21 16:27:28.000000 roadtx-1.2.1/roadtools/roadtx/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10910 2023-03-21 16:27:28.000000 roadtx-1.2.1/roadtools/roadtx/selenium.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-21 16:29:04.983513 roadtx-1.2.1/roadtx.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-03-21 16:29:04.000000 roadtx-1.2.1/roadtx.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      301 2023-03-21 16:29:04.000000 roadtx-1.2.1/roadtx.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-21 16:29:04.000000 roadtx-1.2.1/roadtx.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-03-21 16:29:04.000000 roadtx-1.2.1/roadtx.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-21 16:29:02.000000 roadtx-1.2.1/roadtx.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       66 2023-03-21 16:29:04.000000 roadtx-1.2.1/roadtx.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-03-21 16:29:04.000000 roadtx-1.2.1/roadtx.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-03-21 16:29:04.987513 roadtx-1.2.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-03-21 16:27:28.000000 roadtx-1.2.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 14:43:38.582876 roadtx-1.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-05-22 14:43:38.582876 roadtx-1.3.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 14:43:38.582876 roadtx-1.3.0/roadtools/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 14:43:38.582876 roadtx-1.3.0/roadtools/roadtx/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7865 2023-05-22 14:42:07.000000 roadtx-1.3.0/roadtools/roadtx/keepass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    51917 2023-05-22 14:42:07.000000 roadtx-1.3.0/roadtools/roadtx/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12028 2023-05-22 14:42:07.000000 roadtx-1.3.0/roadtools/roadtx/selenium.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 14:43:38.582876 roadtx-1.3.0/roadtx.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      301 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-22 14:43:35.000000 roadtx-1.3.0/roadtx.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       66 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-22 14:43:38.582876 roadtx-1.3.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-22 14:42:07.000000 roadtx-1.3.0/setup.py
```

### Comparing `roadtx-1.2.1/PKG-INFO` & `roadtx-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.2.1
+Version: 1.3.0
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.2.1/roadtools/roadtx/keepass.py` & `roadtx-1.3.0/roadtools/roadtx/keepass.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.2.1/roadtools/roadtx/main.py` & `roadtx-1.3.0/roadtools/roadtx/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,24 +62,36 @@
                             default='request',
                             help='Action to perform (default: request)')
     prt_parser.add_argument('-c', '--cert-pem', action='store', metavar='file', help='Certificate file with device certificate')
     prt_parser.add_argument('-k', '--key-pem', action='store', metavar='file', help='Private key file for device')
     prt_parser.add_argument('--cert-pfx', action='store', metavar='file', help='Device cert and key as PFX file')
     prt_parser.add_argument('--pfx-pass', action='store', metavar='password', help='PFX file password')
     prt_parser.add_argument('--pfx-base64', action='store', metavar='BASE64', help='PFX file as base64 string')
+    prt_parser.add_argument('-tk', '--transport-key-pem', action='store', metavar='file', help='Private key file containing transport key (if different from device key)')
 
     prt_parser.add_argument('-u', '--username', action='store', metavar='USER', help='User to authenticate')
     prt_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password')
     prt_parser.add_argument('-r', '--refresh-token', action='store', help='Refresh token')
 
 
     prt_parser.add_argument('-f', '--prt-file', default="roadtx.prt", action='store', metavar='FILE', help='PRT storage file (to save or load in case of renewal)')
     prt_parser.add_argument('--prt', action='store', metavar='PRT', help='Primary Refresh Token (for renewal)')
     prt_parser.add_argument('-s', '--prt-sessionkey', action='store', help='Primary Refresh Token session key (as hex key)')
 
+    prt_parser.add_argument('-hk', '--hello-key', action='store', help='Windows Hello PEM file')
+    # Construct winhello module
+    winhello_parser = subparsers.add_parser('winhello', help='Register Windows Hello key')
+    winhello_parser.add_argument('-k', '--key-pem', action='store', metavar='file', help='Private key file for key storage (default: winhello.key)')
+    winhello_parser.add_argument('--access-token', action='store', help='Access token for device registration service. If not specified, taken from .roadtools_auth')
+
+    # Construct winhello key generation module - included for reference
+    # winhello_parser = subparsers.add_parser('genhellokey', help='Generate Windows Hello key')
+    # winhello_parser.add_argument('-k', '--key-pem', action='store', metavar='file', help='Private key file for key storage (default: winhello.key)')
+    # winhello_parser.add_argument('-d', '--device-id', action='store', help='Device ID to use for key object')
+
     # Construct PRT authmodule
     prtauth_parser = subparsers.add_parser('prtauth', help='Authenticate using a PRT (emulates WAM token broker)')
     helptext = 'Client ID to use when authenticating.'
     prtauth_parser.add_argument('-c',
                                 '--client',
                                 action='store',
                                 help=helptext,
@@ -158,14 +170,45 @@
     codeauth_parser.add_argument('--tokens-stdout',
                                  action='store_true',
                                  help='Do not store tokens on disk, pipe to stdout instead')
     codeauth_parser.add_argument('code',
                                  action='store',
                                  help="Code to auth with that you got from Azure AD")
 
+    # Desktop SSO auth
+    desktopsso_parser = subparsers.add_parser('desktopsso', help='Desktop SSO authentication - either with plaintext creds or Kerberos auth')
+    clienthelptext = 'Client ID (application ID) to use when authenticating. Accepts aliases (list with roadtx listaliases)'
+    desktopsso_parser.add_argument('-c',
+                                   '--client',
+                                   action='store',
+                                   help=clienthelptext,
+                                   default='1b730954-1685-4b74-9bfd-dac224a7b894')
+    desktopsso_parser.add_argument('-u', '--username', action='store', metavar='USER', help='User to authenticate')
+    desktopsso_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password of the user')
+    desktopsso_parser.add_argument('--krbtoken',
+                                   action='store',
+                                   help='Kerberos auth data from krbsso.py')
+    desktopsso_parser.add_argument('-r',
+                                   '--resource',
+                                   action='store',
+                                   help='Resource to authenticate to. Either a full URL or alias (list with roadtx listaliases)',
+                                   default='https://graph.windows.net')
+    desktopsso_parser.add_argument('-t',
+                                   '--tenant',
+                                   action='store',
+                                   required=True,
+                                   help='Tenant ID or domain to auth to')
+    desktopsso_parser.add_argument('--tokenfile',
+                                   action='store',
+                                   help='File to store the credentials (default: .roadtools_auth)',
+                                   default='.roadtools_auth')
+    desktopsso_parser.add_argument('--tokens-stdout',
+                                   action='store_true',
+                                   help='Do not store tokens on disk, pipe to stdout instead')
+
     # List aliases
     subparsers.add_parser('listaliases', help='List aliases that can be used as client ID or resource URL')
 
     # Decrypt utilities
     decrypt_parser = subparsers.add_parser('decrypt', help='Decrypt data using session key or transport key')
     decrypt_parser.add_argument('-f', '--prt-file', default="roadtx.prt", action='store', metavar='FILE', help='PRT storage file (to load the session key)')
     decrypt_parser.add_argument('-k', '--key-pem', action='store', metavar='file', help='Private key file containing transport key')
@@ -190,14 +233,17 @@
 
 
     # Interactive auth using Selenium
     urlhelp = 'Url to initiate browsing. Will be constructed from below parameters if not supplied.'
     intauth_parser = subparsers.add_parser('interactiveauth', help='Interactive authentication in Selenium browser window, optional autofill')
     intauth_parser.add_argument('-u', '--username', action='store', metavar='USER', help='User to authenticate')
     intauth_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password of the user')
+    intauth_parser.add_argument('--krbtoken',
+                                action='store',
+                                help='Kerberos auth data from krbsso.py')
     intauth_parser.add_argument('-url', '--auth-url', action='store', metavar='URL', help=urlhelp)
     intauth_parser.add_argument('-c',
                                 '--client',
                                 action='store',
                                 help=clienthelptext,
                                 default='1b730954-1685-4b74-9bfd-dac224a7b894')
     intauth_parser.add_argument('-r',
@@ -226,14 +272,17 @@
     intauth_parser.add_argument('-d', '--driver-path',
                                 action='store',
                                 help='Path to geckodriver file on disk (download from: https://github.com/mozilla/geckodriver/releases)',
                                 default='geckodriver')
     intauth_parser.add_argument('-k', '--keep-open',
                                 action='store_true',
                                 help='Do not close the browser window after timeout. Useful if you want to browse online apps with the obtained credentials')
+    intauth_parser.add_argument('--capture-code',
+                                action='store_true',
+                                help='Do not attempt to redeem any authentication code but print it instead')
 
     # Interactive auth using Selenium - creds from keepass
     kdbauth_parser = subparsers.add_parser('keepassauth', help='Selenium based authentication with credentials from a KeePass database')
     kdbauth_parser.add_argument('-u', '--username', action='store', help='User to authenticate as (must exist as username in KeePass)')
     kdbauth_parser.add_argument('-kp', '--keepass', action='store', metavar='KPFILE', default='roadtx.kdbx', help='KeePass file (default: roadtx.kdbx)')
     kdbauth_parser.add_argument('-kpp', '--keepass-password', action='store', metavar='KPPASS', help='KeePass file password. Can also be provided via KPPASS environment variable.')
     kdbauth_parser.add_argument('-url', '--auth-url', action='store', metavar='URL', help=urlhelp)
@@ -272,14 +321,15 @@
     kdbauth_parser.add_argument('-k', '--keep-open',
                                 action='store_true',
                                 help='Do not close the browser window after timeout. Useful if you want to browse online apps with the obtained credentials')
     kdbauth_parser.add_argument('--capture-code',
                                 action='store_true',
                                 help='Do not attempt to redeem any authentication code but print it instead')
 
+
     # Interactive auth using Selenium - inject PRT
     browserprtauth_parser = subparsers.add_parser('browserprtauth', help='Selenium based auth with automatic PRT usage. Emulates Edge browser with PRT')
     browserprtauth_parser.add_argument('-url', '--auth-url', action='store', metavar='URL', help=urlhelp)
     browserprtauth_parser.add_argument('-c',
                                        '--client',
                                        action='store',
                                        help=helptext,
@@ -386,26 +436,23 @@
     enrauth_parser.add_argument('-f', '--prt-file', default="roadtx.prt", action='store', metavar='FILE', help='PRT storage file (default: roadtx.prt)')
     enrauth_parser.add_argument('--prt',
                                 action='store',
                                 help='Primary Refresh Token')
     enrauth_parser.add_argument('--prt-sessionkey',
                                 action='store',
                                 help='Primary Refresh Token session key (as hex key)')
-    # enrauth_parser.add_argument('--ngcmfa-drs-auth', action='store_true', help="Don't request PRT with MFA claim but get access token with ngcmfa claim for DRS instead.")
+    enrauth_parser.add_argument('--ngcmfa-drs-auth', action='store_true', help="Don't request PRT with MFA claim but get access token with ngcmfa claim for DRS instead.")
     enrauth_parser.add_argument('--tokenfile',
                                 action='store',
                                 help='File to store the credentials (default: .roadtools_auth)',
                                 default='.roadtools_auth')
     enrauth_parser.add_argument('--tokens-stdout',
                                 action='store_true',
                                 help='Do not store tokens on disk, pipe to stdout instead')
 
-
-    args = parser.parse_args()
-
     if len(sys.argv) < 2:
         parser.print_help()
         sys.exit(1)
         return
 
     deviceauth = DeviceAuthentication()
     args = parser.parse_args()
@@ -444,23 +491,26 @@
         if not deviceauth.loadcert(args.cert_pem, args.key_pem, args.cert_pfx, args.pfx_pass, args.pfx_base64):
             return
         deviceauth.register_hybrid_device(args.sid, args.tenant, certout=args.cert_pem, privout=args.key_pem, device_type=args.device_type, device_name=args.name, os_version=args.os_version)
     elif args.command == 'prt':
         if args.action == 'request':
             if not deviceauth.loadcert(args.cert_pem, args.key_pem, args.cert_pfx, args.pfx_pass, args.pfx_base64):
                 return
+            if args.transport_key_pem:
+                # Try loading transport key separately
+                if not deviceauth.loadkey(args.transport_key_pem, transport_only=True):
+                    return
             prtdata = None
             if args.username and args.password:
                 prtdata = deviceauth.get_prt_with_password(args.username, args.password)
             if args.refresh_token:
                 prtdata = deviceauth.get_prt_with_refresh_token(args.refresh_token)
-            # if args.username and deviceauth.loadhellokey(args.hello_key):
-            #     prtdata = deviceauth.get_prt_with_hello_key(args.username)
-            # if args.username and args.hello_assertion:
-            #     prtdata = deviceauth.get_prt_with_hello_key(args.username, args.hello_assertion)
+
+            if args.username and deviceauth.loadhellokey(args.hello_key):
+                prtdata = deviceauth.get_prt_with_hello_key(args.username)
             if not prtdata:
                 print('You must specify a username + password or refresh token that can be used to request a PRT')
                 return
             print(f"Obtained PRT: {prtdata['refresh_token']}")
             print(f"Obtained session key: {prtdata['session_key']}")
             deviceauth.saveprt(prtdata, args.prt_file)
         if args.action == 'renew':
@@ -524,63 +574,85 @@
             except (json.decoder.JSONDecodeError, UnicodeDecodeError):
                 print('Decrypted data (hex)')
                 print(binascii.hexlify(data))
 
     elif args.command == 'codeauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
+        auth.tenant = args.tenant
         auth.authenticate_with_code_native(args.code, args.redirect_url, client_secret=args.password)
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
+    elif args.command == 'desktopsso':
+        auth.set_client_id(args.client)
+        auth.set_resource_uri(args.resource)
+        auth.tenant = args.tenant
+        dsso_code = auth.get_desktopsso_token(args.username, args.password, args.krbtoken)
+        if dsso_code:
+            auth.authenticate_with_desktopsso_token(dsso_code)
+            auth.outfile = args.tokenfile
+            auth.save_tokens(args)
     elif args.command == 'listaliases':
         print('Well-known clients. Can be used as alias with -c or --client')
         print()
         for alias, clientid in WELLKNOWN_CLIENTS.items():
             print(f"{alias} - {clientid}")
         print()
         print('Well-known resources. Can be used as alias with -r or --resource')
         print()
         for alias, resourceurl in WELLKNOWN_RESOURCES.items():
             print(f"{alias} - {resourceurl}")
     elif args.command == 'interactiveauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
+        auth.tenant = args.tenant
         selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url)
         if args.auth_url:
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
         service = selauth.get_service(args.driver_path)
         if not service:
             return
-        selauth.driver = selauth.get_webdriver(service)
-        selauth.selenium_login(url, args.username, args.password)
+        selauth.driver = selauth.get_webdriver(service, intercept=True)
+        if args.krbtoken:
+            result = selauth.selenium_login_with_kerberos(url, args.username, args.password, capture=args.capture_code, krbdata=args.krbtoken)
+        else:
+            result = selauth.selenium_login(url, args.username, args.password, capture=args.capture_code)
+        if args.capture_code:
+            if result:
+                print(f'Captured auth code: {result}')
+            return
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'keepassauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
+        auth.tenant = args.tenant
         selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url)
         password, otpseed = selauth.get_keepass_cred(args.username, args.keepass, args.keepass_password)
         if args.auth_url:
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
         service = selauth.get_service(args.driver_path)
         if not service:
             return
         selauth.driver = selauth.get_webdriver(service)
-        selauth.selenium_login(url, args.username, password, otpseed, keep=args.keep_open, capture=args.capture_code)
+        result = selauth.selenium_login(url, args.username, password, otpseed, keep=args.keep_open, capture=args.capture_code)
         if args.capture_code:
+            if result:
+                print(f'Captured auth code: {result}')
             return
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'browserprtauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
+        auth.tenant = args.tenant
         if args.prt and args.prt_sessionkey:
             deviceauth.setprt(args.prt, args.prt_sessionkey)
         elif args.prt_cookie:
             pass
         elif args.prt_file and deviceauth.loadprt(args.prt_file):
             pass
         else:
@@ -591,23 +663,27 @@
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
         service = selauth.get_service(args.driver_path)
         if not service:
             return
         selauth.driver = selauth.get_webdriver(service, intercept=True)
-        if not selauth.selenium_login_with_prt(url, keep=args.keep_open, prtcookie=args.prt_cookie, capture=args.capture_code):
+        result = selauth.selenium_login_with_prt(url, keep=args.keep_open, prtcookie=args.prt_cookie, capture=args.capture_code)
+        if not result:
             return
         if args.capture_code:
+            if result:
+                print(f'Captured auth code: {result}')
             return
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'browserprtinject':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
+        auth.tenant = args.tenant
         if args.prt and args.prt_sessionkey:
             deviceauth.setprt(args.prt, args.prt_sessionkey)
         elif args.prt_file and deviceauth.loadprt(args.prt_file):
             pass
         else:
             print('You must either supply a PRT and session key on the command line or a file that contains them')
             return
@@ -646,41 +722,41 @@
         if args.username:
             hint = '&login_hint=' + quote_plus(args.username)
         else:
             hint = ''
         replyurl = "ms-appx-web://Microsoft.AAD.BrokerPlugin/DRS"
         url = f'https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&client_id=29d9ed98-a469-4536-ade2-f981bc1d605e&redirect_uri=ms-appx-web%3a%2f%2fMicrosoft.AAD.BrokerPlugin%2fDRS&resource=urn%3aaad%3atb%3aupdate%3aprt&add_account=noheadsup&scope=openid{hint}&response_mode=form_post&windows_api_version=2.0&amr_values=ngcmfa'
 
-        # if args.ngcmfa_drs_auth:
-        #     # Get ngcmfa token for device registration service
-        #     auth.set_client_id('dd762716-544d-4aeb-a526-687b73838a22')
-        #     replyurl = "ms-appx-web://Microsoft.AAD.BrokerPlugin/dd762716-544d-4aeb-a526-687b73838a22"
-        #     url = f'https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&client_id=dd762716-544d-4aeb-a526-687b73838a22&redirect_uri=ms-appx-web%3a%2f%2fMicrosoft.AAD.BrokerPlugin%2fdd762716-544d-4aeb-a526-687b73838a22&resource=urn%3ams-drs%3aenterpriseregistration.windows.net&add_account=noheadsup&scope=openid{hint}&response_mode=form_post&windows_api_version=2.0&amr_values=ngcmfa'
+        if args.ngcmfa_drs_auth:
+            # Get ngcmfa token for device registration service
+            auth.set_client_id('dd762716-544d-4aeb-a526-687b73838a22')
+            replyurl = "ms-appx-web://Microsoft.AAD.BrokerPlugin/dd762716-544d-4aeb-a526-687b73838a22"
+            url = f'https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&client_id=dd762716-544d-4aeb-a526-687b73838a22&redirect_uri=ms-appx-web%3a%2f%2fMicrosoft.AAD.BrokerPlugin%2fdd762716-544d-4aeb-a526-687b73838a22&resource=urn%3ams-drs%3aenterpriseregistration.windows.net&add_account=noheadsup&scope=openid{hint}&response_mode=form_post&windows_api_version=2.0&amr_values=ngcmfa'
 
         selauth = SeleniumAuthentication(auth, deviceauth, replyurl)
         if args.username and args.keepass and (args.keepass_password or 'KPPASS' in os.environ or args.keepass.endswith('.xml')):
             _, otpseed = selauth.get_keepass_cred(args.username, args.keepass, args.keepass_password)
         else:
             otpseed = None
         service = selauth.get_service(args.driver_path)
         if not service:
             return
         selauth.driver = selauth.get_webdriver(service, intercept=True)
         tokenreply = selauth.selenium_enrich_prt(url, otpseed=otpseed)
         # Save tokens
-        # if args.ngcmfa_drs_auth:
-        #     auth.tokendata = auth.tokenreply_to_tokendata(tokenreply)
-        #     auth.outfile = args.tokenfile
-        #     auth.save_tokens(args)
-        # else:
-        if tokenreply['refresh_token']:
-            print('Got refresh token. Can be used to request prt with roadtx prt -r <refreshtoken>')
-            print(tokenreply['refresh_token'])
+        if args.ngcmfa_drs_auth:
+            auth.tokendata = auth.tokenreply_to_tokendata(tokenreply)
+            auth.outfile = args.tokenfile
+            auth.save_tokens(args)
         else:
-            print('No tokendata found. Something probably went wrong')
+            if tokenreply['refresh_token']:
+                print('Got refresh token. Can be used to request prt with roadtx prt -r <refreshtoken>')
+                print(tokenreply['refresh_token'])
+            else:
+                print('No tokendata found. Something probably went wrong')
 
     elif args.command == 'getotp':
         selauth = SeleniumAuthentication(auth, deviceauth, None)
         if args.keepass and args.username and (args.keepass_password or 'KPPASS' in os.environ or args.keepass.endswith('.xml')):
             _, otpseed = selauth.get_keepass_cred(args.username, args.keepass, args.keepass_password)
         else:
             otpseed = args.otpseed
@@ -709,9 +785,47 @@
                     return
         if tokendata[0:2] == '0.':
             print('The supplied data looks like an encrypted token or nonce, nothing to decode here!')
             return
         header, body, signature = auth.parse_jwt(tokendata)
         print(json.dumps(header, sort_keys=True, indent=4))
         print(json.dumps(body, sort_keys=True, indent=4))
+    elif args.command == 'winhello':
+        if args.access_token:
+            tokenobject, tokendata = auth.parse_accesstoken(args.access_token)
+        else:
+            try:
+                with codecs.open('.roadtools_auth', 'r', 'utf-8') as infile:
+                    tokenobject = json.load(infile)
+                _, tokendata = auth.parse_accesstoken(tokenobject['accessToken'])
+            except FileNotFoundError:
+                print('No auth data found. Ether supply an access token with --access-token or make sure a token is present on disk in .roadtools_auth')
+                return
+        if tokendata['aud'] != 'urn:ms-drs:enterpriseregistration.windows.net':
+            print(f"Wrong token audience, got {tokendata['aud']} but expected: urn:ms-drs:enterpriseregistration.windows.net")
+            print("Make sure to request a token with -r urn:ms-drs:enterpriseregistration.windows.net")
+            return
+        key, pubkeycngblob = deviceauth.create_hello_key(args.key_pem)
+        result = deviceauth.register_winhello_key(pubkeycngblob, tokenobject['accessToken'])
+        print(result)
+
+    elif args.command == 'genhellokey':
+        key, pubkeycngblob = deviceauth.create_hello_key(args.key_pem)
+        if not args.device_id:
+            deviceid = "d22a8b4b-d138-4271-a677-de4208305cb3"
+        else:
+            deviceid = args.device_id
+        data = {
+            "usage": "NGC",
+            "keyIdentifier": deviceauth.get_privkey_kid(key),
+            "keyMaterial": pubkeycngblob.decode('utf-8'),
+            "creationTime": "2022-10-12T18:29:51.3793062Z",
+            "deviceId": deviceid,
+            "customKeyInformation": "AQAAAAACAAAAAAAAAAAA",
+            "fidoAaGuid": None,
+            "fidoAuthenticatorVersion": None,
+            "fidoAttestationCertificates": []
+        }
+        print(json.dumps(data, sort_keys=True, indent=4))
+
 if __name__ == '__main__':
     main()
```

### Comparing `roadtx-1.2.1/roadtools/roadtx/selenium.py` & `roadtx-1.3.0/roadtools/roadtx/selenium.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,16 +100,15 @@
             WebDriverWait(driver, 2).until(lambda d: '?code=' in d.current_url)
             res = urlparse(driver.current_url)
             params = parse_qs(res.query)
             code = params['code'][0]
             if not keep:
                 driver.close()
             if capture:
-                print(f'Captured auth code: {code}')
-                return True
+                return code
             return self.auth.authenticate_with_code_native(code, self.redirurl)
         except TimeoutException:
             pass
 
         if otpseed:
             try:
                 els = WebDriverWait(driver, 2).until(lambda d: d.find_element(By.CSS_SELECTOR, '[data-value="PhoneAppOTP"]'))
@@ -130,17 +129,16 @@
             WebDriverWait(driver, 120).until(lambda d: '?code=' in d.current_url)
             res = urlparse(driver.current_url)
             params = parse_qs(res.query)
             code = params['code'][0]
             if not keep:
                 driver.close()
             if capture:
-                print(f'Captured auth code: {code}')
-            else:
-                return self.auth.authenticate_with_code_native(code, self.redirurl)
+                return code
+            return self.auth.authenticate_with_code_native(code, self.redirurl)
         except TimeoutException:
             if not keep:
                 driver.close()
                 raise AuthenticationException('Authentication did not complete within time limit')
         return False
 
     def selenium_login_with_prt(self, url, identity=None, password=None, otpseed=None, keep=False, prtcookie=None, capture=False):
@@ -151,15 +149,15 @@
             del request.headers['User-Agent']
             request.headers['User-Agent'] = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/103.0.5060.134 Safari/537.36 Edg/103.0.1264.71'
             request.headers['Sec-Ch-Ua'] = '" Not;A Brand";v="99", "Microsoft Edge";v="103", "Chromium";v="103"'
             request.headers['Sec-Ch-Ua-Mobile'] =  '?0'
             request.headers['Sec-Ch-Ua-Platform'] =  '"Windows"'
             request.headers['Sec-Ch-Ua-Platform-Version'] = '"10.0.0"'
 
-            if request.url.startswith('https://login.microsoftonline.com'):
+            if request.url.startswith('https://login.microsoftonline.com/'):
                 if '/authorize' in request.url or '/login' in request.url or '/kmsi' in request.url or '/reprocess' in request.url or '/resume' in request.url:
                     if prtcookie:
                         # Force single cookie injection
                         request.headers['X-Ms-Refreshtokencredential'] = prtcookie
                     else:
                         if 'sso_nonce' in request.url:
                             res = urlparse(request.url)
@@ -170,14 +168,35 @@
                         else:
                             cookie = self.auth.create_prt_cookie_kdf_ver_2(self.deviceauth.prt,
                                                                            self.deviceauth.session_key)
                         request.headers['X-Ms-Refreshtokencredential'] = cookie
         self.driver.request_interceptor = interceptor
         return self.selenium_login(url, identity, password, otpseed, keep=keep, capture=capture)
 
+    def selenium_login_with_kerberos(self, url, identity=None, password=None, otpseed=None, keep=False, capture=False, krbdata=None):
+        '''
+        Selenium login with Kerberos auth header injection.
+        '''
+        def interceptor(request):
+            del request.headers['User-Agent']
+            request.headers['User-Agent'] = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/103.0.5060.134 Safari/537.36 Edg/103.0.1264.71'
+            request.headers['Sec-Ch-Ua'] = '" Not;A Brand";v="99", "Microsoft Edge";v="103", "Chromium";v="103"'
+            request.headers['Sec-Ch-Ua-Mobile'] =  '?0'
+            request.headers['Sec-Ch-Ua-Platform'] =  '"Windows"'
+            request.headers['Sec-Ch-Ua-Platform-Version'] = '"10.0.0"'
+
+            if request.url.startswith('https://autologon.microsoftazuread-sso.com/'):
+                if '/winauth/sso' in request.url and krbdata:
+
+                    # Force single cookie injection
+                    request.headers['Authorization'] = f'Negotiate {krbdata}'
+
+        self.driver.request_interceptor = interceptor
+        return self.selenium_login(url, identity, password, otpseed, keep=keep, capture=capture)
+
     def selenium_enrich_prt(self, url, otpseed=None):
         '''
         Selenium authentication to add NGC MFA claim to a PRT or token.
         Single factor auth is handled via PRT injection, MFA seed can come
         from keepass or manually. Result is refresh token that can be used to request
         a new PRT, or an access token to the desired resource (depends on supplied url).
         '''
```

### Comparing `roadtx-1.2.1/roadtx.egg-info/PKG-INFO` & `roadtx-1.3.0/roadtx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.2.1
+Version: 1.3.0
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.2.1/setup.py` & `roadtx-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='roadtx',
-      version='1.2.1',
+      version='1.3.0',
       description='ROADtools Token eXchange',
       author='Dirk-jan Mollema',
       author_email='dirkjan@outsidersecurity.nl',
       url='https://github.com/dirkjanm/ROADtools/',
       license='MIT',
       classifiers=[
           'Intended Audience :: Information Technology',
@@ -13,15 +13,15 @@
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
       ],
       packages=['roadtools.roadtx'],
       install_requires=[
-          'roadlib>=0.16',
+          'roadlib>=0.18',
           'requests',
           'selenium',
           'selenium-wire',
           'pyotp',
           'pycryptodomex'
       ],
       zip_safe=False,
```

