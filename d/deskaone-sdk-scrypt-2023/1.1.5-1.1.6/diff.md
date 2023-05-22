# Comparing `tmp/deskaone_sdk_scrypt_2023-1.1.5.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.5.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.6.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.1.5.tar` & `deskaone_sdk_scrypt_2023-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      754 2023-05-17 23:56:25.812906 deskaone_sdk_scrypt_2023-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.5/README.md
--rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     6046 2023-05-09 16:58:57.983045 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-09 16:39:36.272506 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      491 2023-05-17 23:56:19.494552 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    30045 2023-05-17 23:56:15.831112 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.5/setup.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-05-22 14:31:50.221475 deskaone_sdk_scrypt_2023-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.6/README.md
+-rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     6046 2023-05-09 16:58:57.983045 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-09 16:39:36.272506 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-22 14:31:55.838997 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    34717 2023-05-19 13:16:00.694179 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.6/setup.py
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.6/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.1.5"
+version = "1.1.6"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -231,15 +231,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
         
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=socks4&timeout=5000&country=all&ssl=all&anonymity=all'
         Result  = self.Session.get(URL).text
         Saves = [Proxy for Proxy in Result.replace(' ', '').replace('\r', '').split('\n')]
         for i in range(len(Saves)):
             Proxy = Saves[random.randint(0, len(Saves) - 1)]
@@ -254,15 +254,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
         
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=socks5&timeout=5000&country=all&ssl=all&anonymity=all'
         Result  = self.Session.get(URL).text
         Saves = [Proxy for Proxy in Result.replace(' ', '').replace('\r', '').split('\n')]
         for i in range(len(Saves)):
             Proxy = Saves[random.randint(0, len(Saves) - 1)]
@@ -277,15 +277,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
@@ -316,15 +316,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
@@ -355,15 +355,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
@@ -393,15 +393,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
     
     @property
     def __https__(self):
         r  = self.Session.get('https://www.proxy-list.download/HTTPS')
         Result = BeautifulSoup(r.content, 'html5lib')
         Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
@@ -421,15 +421,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
         
     @property
     def __socks4__(self):
         r  = self.Session.get('https://www.proxy-list.download/SOCKS4')
         Result = BeautifulSoup(r.content, 'html5lib')
         Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
@@ -449,15 +449,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
         
     @property
     def __socks5__(self):
         r  = self.Session.get('https://www.proxy-list.download/SOCKS5')
         Result = BeautifulSoup(r.content, 'html5lib')
         Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
@@ -477,15 +477,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
     
     @property
     def __proxy__(self):
         self.__http__
         self.__https__
         self.__socks4__
@@ -524,30 +524,124 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == 20: break
+                #if i == random.randint(3 if len(Saves) < 20 else 20, len(Saves) - 1): break
             except Error:pass
             
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
 
+class __PremiumProxy__:
+    
+    def __init__(self) -> None:
+        self.__url__ = [
+            "https://premiumproxy.net/anonymous-proxy-list",
+            'https://premiumproxy.net/elite-proxy-list',
+            'https://premiumproxy.net/http-proxy-list',
+            'https://premiumproxy.net/https-ssl-proxy-list',
+            'https://premiumproxy.net/mikrotik-proxy-list',
+            'https://premiumproxy.net/socks-proxy-list',
+            'https://premiumproxy.net/squid-proxy-list',
+            'https://premiumproxy.net/transparent-proxy-list',
+            'https://premiumproxy.net/top-country-proxy-list'
+        ]
+        self.__payload__={}
+        self.__headers__ = {}        
+    
+    def __result__(self, url: str):
+        response = requests.request("GET", url, headers=self.__headers__, data=self.__payload__)
+        return BeautifulSoup(response.text, features='html.parser')
+    
+    def __parse__(self, Proxys: list, Result: BeautifulSoup):
+        Saves   = [List for List in Result.findAll('tbody')[0].findAll('tr', attrs={'class': 'pp1x'})]
+        for S in Saves:
+            I_P = S.findAll('td', attrs={'colspan': 1})[0].findAll('font')
+            SCHEMA = 'http' if S.findAll('td', attrs={'colspan': 1})[1].findAll('font')[0].text.lower() == 'https' else S.findAll('td', attrs={'colspan': 1})[1].findAll('font')[0].text.lower()
+            Proxys.append(dict(
+                http    = f'{SCHEMA}://{I_P[0].text}',
+                https   = f'{SCHEMA}://{I_P[0].text}',
+            ))
+        return Proxys
+
+    @property
+    def __proxy__(self):
+        Proxys = list()
+        for url in self.__url__:
+            Proxys = self.__parse__(Proxys, self.__result__(url))
+        for proxy in Proxys:
+            PR = proxy.get('http')
+            if PR is None:
+                PR = proxy.get('socks4')
+                if PR is None:
+                    PR = proxy.get('socks5')
+                    if PR is None:
+                        PR = ''
+            try:
+                IpPort  = str(PR).split('//')[1]
+                __ProxyBase__.Proxys.SaveProxy().Set(
+                        country         = '',
+                        countryCode     = '',
+                        IpPort          = f'{IpPort}',
+                        Proxies         = proxy,
+                        BProgrammers    = False,
+                        Givvy           = False,
+                        Viker           = False,
+                        PlayFabapi      = False,
+                        Zebedee         = False
+                    )
+            except Error:pass
+            except:pass
+    
+    def Main(self, New: bool) -> List[Dict[str, str]]:
+        if New is True:
+            self.__proxy__
+        return __ProxyBase__.Proxys.SaveProxy().Get()
+
+
 class Proxy:
     
     def __init__(self, Authorization: Optional[str] = None, New = True, *args, **kwargs) -> None:
         if New is True:
             Typer.Print(f'{Color.RED}=> {Color.WHITE}Please Wait {Color.GREEN}Scraping New Proxy', Refresh=True)
             self.__get__(Authorization, New, **kwargs)
-    
+        
+        if kwargs.get('DESKAONE') is True:
+            PR = 'resi.proxyscrape.com:8000'
+            US = '88slkvnrbz'
+            PS = 'wwlkgj723d'
+            PRX = dict(
+                http    = f'http://{US}:{PS}@{PR}',
+                https   = f'http://{US}:{PS}@{PR}',
+            )
+            __ProxyBase__.Proxys.SaveProxy().Set(
+                country         = '',
+                countryCode     = '',
+                IpPort          = PR,
+                Proxies         = PRX,
+                BProgrammers    = False,
+                Givvy           = False,
+                Viker           = False,
+                PlayFabapi      = False,
+                Zebedee         = False
+            )
+        self.__Authorization__ = Authorization
+        self.__New__ = New
+        self.__kwargs__ = kwargs
+        self.__args__ = args
+    
+    @classmethod
+    def Rescan(cls, Authorization: Optional[str] = None, New = True, *args, **kwargs):
+        return cls(Authorization, New, *args, **kwargs)
         
     def ProxyError(self, IpPort: Optional[str] = None, Add = False):
         if Add is True:
             open('Database/ProxyError.txt', 'a').write(f'{IpPort}\n')
         else:
             if os.path.exists('Database/ProxyError.txt') is True:
                 return set(open('Database/ProxyError.txt').read().split())
@@ -580,14 +674,17 @@
         except:pass
         try:
             if kwargs.get('ProxyList') is True or kwargs.get('ProxyList') is None:__ProxyList__().Main(New)
         except:pass
         try:
             if kwargs.get('HideMy') is True or kwargs.get('HideMy') is None:__HideMy__().Main(New)
         except:pass
+        try:
+            if kwargs.get('PremiumProxy') is True or kwargs.get('PremiumProxy') is None:__PremiumProxy__().Main(New)
+        except:pass
     
     def __check__(self, *args, **kwargs):
         if kwargs.get('IpPort') is None: raise Error('IpPort Required')
         ListProxy, Count = self.ListProxy, 0
         while True:
             Count += 1
             try:
@@ -595,31 +692,30 @@
                 ProxyDetectGO = False
                 PROXY   = ListProxy[random.randint(0, len(ListProxy) - 1)]
                 IpPort = PROXY.get("IpPort")
                 if IpPort in self.ProxyError(Add=False): ProxyErrorGO = True
                 if IpPort in self.ProxyDetect(Add=False): ProxyDetectGO = True
                 Typer.Print(f'{Color.RED}=> {Color.WHITE}Generate New Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Count {Color.GREEN}{Count}', Refresh=True) 
                 if ProxyDetectGO is False and ProxyErrorGO is False:
-                    Count = 0
                     if kwargs.get('IpPort') != PROXY.get("IpPort"):
                         API     = dict(requests.get("http://ip-api.com/json/%1s" % (PROXY.get('IpPort').split(":")[0])).json())
                         Typer.Print(f'{Color.RED}=> {Color.WHITE}Check New Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Country {Color.GREEN}{API.get("country")}', Refresh=True) 
                         MYIP    = dict(requests.get("https://kin4u.com/test").json())
                         S1 = requests.Session()
                         CHECK   = dict(S1.get("https://kin4u.com/test", proxies=PROXY.get('Proxies') if PROXY.get('Proxies') == dict else json.loads(PROXY.get('Proxies')), timeout=15).json())
                         if MYIP.get('HTTP_X_FORWARDED_FOR') != CHECK.get('HTTP_X_FORWARDED_FOR'):
                             S1.close()
                             __ProxyBase__.Proxys.SaveProxy().Up(IpPort = PROXY.get("IpPort"), Values = dict(countryCode = API.get("countryCode"), country = API.get("country")))
                             return dict(
                                 PROXY   = PROXY.get('Proxies') if PROXY.get('Proxies') == dict else json.loads(PROXY.get('Proxies')),
                                 DATA    = API,
                                 IpPort  = PROXY.get('IpPort')
                             )
-                if Count >= 100:
-                    raise Error('No Proxy Scan Again')
+                if Count >= len(self.ListProxy):
+                    self.Rescan(self.__Authorization__, self.__New__, *self.__args__, **self.__kwargs__)
             except ProxyError as e:
                 self.ProxyError(IpPort=IpPort, Add=True)
             except ConnectTimeout as e:
                 self.ProxyError(IpPort=IpPort, Add=True)
             except ConnectionError as e:
                 self.ProxyError(IpPort=IpPort, Add=True)
             except ReadTimeout as e:
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/setup.py` & `deskaone_sdk_scrypt_2023-1.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.1.5',
+    'version': '1.1.6',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.5/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.1.5
+Version: 1.1.6
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

