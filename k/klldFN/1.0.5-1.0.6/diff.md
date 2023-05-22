# Comparing `tmp/klldFN-1.0.5.tar.gz` & `tmp/klldFN-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klldFN-1.0.5.tar", last modified: Sun Apr 23 18:57:45 2023, max compression
+gzip compressed data, was "klldFN-1.0.6.tar", last modified: Mon May 22 09:50:35 2023, max compression
```

## Comparing `klldFN-1.0.5.tar` & `klldFN-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 18:57:45.027027 klldFN-1.0.5/
--rw-r--r--   0 runner    (1000) runner    (1000)     1131 2023-04-23 18:57:45.027027 klldFN-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      670 2023-03-23 09:54:58.000000 klldFN-1.0.5/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 18:57:45.015027 klldFN-1.0.5/klldFN/
--rw-r--r--   0 runner    (1000) runner    (1000)    60569 2023-04-23 18:28:00.000000 klldFN-1.0.5/klldFN/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 18:57:45.027027 klldFN-1.0.5/klldFN.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1131 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      127 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      393 2023-02-19 12:22:33.000000 klldFN-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 18:57:45.027027 klldFN-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      806 2023-04-23 18:28:13.000000 klldFN-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-22 09:50:35.815198 klldFN-1.0.6/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1135 2023-05-22 09:50:35.815198 klldFN-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      670 2023-03-23 09:54:58.000000 klldFN-1.0.6/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-22 09:50:35.811198 klldFN-1.0.6/klldFN/
+-rw-r--r--   0 runner    (1000) runner    (1000)    67131 2023-05-21 19:02:20.000000 klldFN-1.0.6/klldFN/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-22 09:50:35.811198 klldFN-1.0.6/klldFN.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1135 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      127 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      393 2023-02-19 12:22:33.000000 klldFN-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-22 09:50:35.815198 klldFN-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      810 2023-05-19 14:02:19.000000 klldFN-1.0.6/setup.py
```

### Comparing `klldFN-1.0.5/PKG-INFO` & `klldFN-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: klldFN
-Version: 1.0.5
+Version: 1.0.6
 Summary: klldFN
-Home-page: https://klld.42web.io
+Home-page: https://www.klld.42web.io
 Author: klld
 License: UNKNOWN
 Description: # klldFN
         Use This To Upload Files To klldFN
         
         [![Downloads](https://pepy.tech/badge/klldFN)](https://pepy.tech/project/klldFN)
         [![Downloads](https://pepy.tech/badge/klldFN/week)](https://pepy.tech/project/klldFN)
```

### Comparing `klldFN-1.0.5/README.md` & `klldFN-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `klldFN-1.0.5/klldFN/__init__.py` & `klldFN-1.0.6/klldFN/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,9 @@
 """
-“Commons Clause” License Condition v1.0
-Copyright klld 2023
-The Software is provided to you by the Licensor under the
-License, as defined below, subject to the following condition.
-Without limiting other conditions in the License, the grant
-of rights under the License will not include, and the License
-does not grant to you, the right to Sell the Software.
-For purposes of the foregoing, “Sell” means practicing any or
-all of the rights granted to you under the License to provide
-to third parties, for a fee or other consideration (including
-without limitation fees for hosting or consulting/ support
-services related to the Software), a product or service whose
-value derives, entirely or substantially, from the functionality
-of the Software. Any license notice or attribution required by
-the License must also include this Commons Clause License
-Condition notice.
-Software: klldFN
-License: Apache 2.0
+
 """
 try:
     # System imports.
     from typing import Tuple, Any, Union, Optional
 
     import asyncio
     import sys
@@ -55,14 +38,15 @@
     import uvloop
     import requests
 
 except ModuleNotFoundError as e:
     print(f'Error: {e}\nAttempting to install packages now.')
 
     for module in (
+        'pytz',
         'crayons',
         'PirxcyPinger',
         'fortnitepy==3.6.7',
         'BenBotAsync',
         'FortniteAPIAsync',
         'sanic==20.6.3',
         'aiohttp',
@@ -73,28 +57,39 @@
     os.system('clear')
 
     print('Installed packages, restarting script.')
 
     python = sys.executable
     os.execl(python, python, *sys.argv)
 
+class configuration:
+  """Interact With The Bot Configuration("config.json")"""
+  def read():
+    """Read The Configuration File"""
+    with open("config.json") as config_file:
+      config = json.load(config_file)
+      return config
 
-print(crayons.blue(f'klldv5 by klld'))
-print(crayons.magenta(f'Discord server: https://klld.tk/discord.html - For support, questions, etc.'))
+print(crayons.blue(f'klldFN by klld'))
+print(crayons.magenta(f'Discord server: https://discord.gg/ybr7evg4q5 - For support, questions, etc.'))
 
 
 sanic_app = sanic.Sanic(__name__)
 server = None
 
+
+skin = configuration.read()['config']['skin']
+backpack = configuration.read()['config']['backpack']
+pickaxe = configuration.read()['config']['pickaxe']
 cid = ""
 name = ""
 friendlist = ""
 password = "4455"
 copied_player = ""
-__version__ = "1.0.2"
+__version__ = "1.0.6"
 adminsss = 'klld َََََ'
 owner = 'e375edab04964813a886ee974b66bd70'
 errordiff = 'errors.com.epicgames.common.throttled', 'errors.com.epicgames.friends.inviter_friendships_limit_exceeded'
 shit_partys_errrors = 'errors.com.epicgames.social.party.invite_already_exists', 'errors.com.epicgames.social.party.party_not_found', 'errors.com.epicgames.social.party.stale_revision', 'errors.com.epicgames.social.party.party_change_forbidden', 'errors.com.epicgames.social.party.invite_forbidden'#HTTPexception (soon...)
 vips = "klld َََََ"
 
 
@@ -141,15 +136,265 @@
             {
                 "status": "online"
             }
         )
 
     return sanic.response.html(
         """
+<!DOCTYPE html>
+<html lang="en">
+<head>
+	<meta charset="UTF-8">
+	<meta name="viewport" content="width=device-width, initial-scale=1.0">
+
+	<!-- Boxicons -->
+	<link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
+
+
+	<!-- My CSS -->
+<link href='https://unpkg.com/boxicons@2.1.1/css/boxicons.min.css' rel='stylesheet'>
+    <link href="https://cdn.klld.42web.io/dashfiles?path=css/sb-admin-2.min.css" type="text/css" rel="stylesheet">
+
+<link rel="stylesheet" href="https://unicons.iconscout.com/release/v4.0.0/css/line.css">
+  
+  <link href="https://raw.githubusercontent.com/nohello-net/site/main/src/css/styles.css" type="text/css" rel="stylesheet">
+  
+  <link href="https://cdn.klld.42web.io/dashfiles?path=vendor/fontawesome-free/css/all.min.css" rel=stylesheet type=text/css>
+
+<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/tiny-slider.css" rel="stylesheet">
+<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/Cookies.css" rel="stylesheet">
+<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/Click.css" rel="stylesheet">
+<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/tobii.min.css" rel="stylesheet">
+<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/style.min.css" class="theme-opt" rel="stylesheet" type="text/css" />
+<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/style.css" class="theme-opt" rel="stylesheet" type="text/css" />
+
+  <link rel="stylesheet" href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/style1.css">
+  
+	<link rel="stylesheet" href="https://klld.repl.co/style.css">
+	<link rel="stylesheet" href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/adminhub.css">
+
+	<title>klldFN</title>
+<meta name="viewport" content="width=device-width, initial-scale=1.0">
+<meta name="description" content="">
+<meta name="keywords" content="klld">
+<meta name="author" content="klld">
+<meta name="email" content="klld@email.com">
+<meta name="website" content="https://www.klld.42web.io/">
+<meta name="Version" content="v1.0.6">
+<link rel="shortcut icon" href="https://www.authcode.tk/klld.png">
+</head>
+<body>
+
+<nav>
+		<div class="container">
+			<div class="nav__wrapper">
+				<a href="#" class="nav__brand">
+					<span class="nav__logo">FN</span>
+					<span class="nav__logo__name">klld</span>
+				</a>
+				<div class="nav__list__wrapper">
+					<div class="nav__list">
+						<div class="nav__menu">
+							<a href="https://www.klld.42web.io/" class="nav__menu__item">Home</a>
+
+						<div class="nav__menu">
+							<a href="https://discord.gg/ybr7evg4q5" class="bx bxl-discord btn btn-blue">discord</a>
+						</div>
+						</div>
+					</div>
+				</div>
+				<i class='bx bx-menu nav__toggle'></i>
+			</div>
+		</div>
+	</nav>
+
+
+<header>
+		<div class="container">
+			<div class="header__wrapper">
+				<div class="header__content">
+	<section id="testimonial">
+		<div class="container">
+			<h4 class="header__title">klldFN</h4>
+			<div class="testimonial__list">
+				<div class="testimonial__item">
+					
+
+					<div class="testimonial__item__user">
+		<img src="https://www.just.edu.jo/Units_and_offices/Offices/IRO/PublishingImages/Pages/Mobility%20Calls/MobilityCalls/green2.gif" alt="">
+						<div class="testimonial__item__user__profile">
+							<h4>Online now</h4>
+              <h>""" + f""" {name} """ + """</h>
+
+						</div>
+					</div>
+				</div>
+
+        
+
+        			<div class="testimonial__list">
+				<div class="testimonial__item">
+
+									<div class="testimonial__item__user">
+						<div class="testimonial__item__user__profile">
+							<h4>Platform</h4>
+              <h>""" + f""" {(str((platform))[9:]).lower().capitalize()} """ + """</h>
+          </div>
+					</div>
+				</div>
+
+
+
+    
+			<div class="testimonial__list">
+				<div class="testimonial__item">
+					
+
+					<div class="testimonial__item__user">
+						
+						<div class="testimonial__item__user__profile">
+							<h4>Party</h4>
+             <h>""" + f"""{party_size} """ + """</h>
+
+						</div>
+					</div>
+				</div>
+
+                <div class="testimonial__list">
+				<div class="testimonial__item">
+
+									<div class="testimonial__item__user">
+						
+						<div class="testimonial__item__user__profile">
+							<h4>Friends</h4>
+              <h>""" + f"""{friendlist} """ + """ / 9500</h>
+              </div>
+					</div>
+				</div>
+
+
+
+
+              
+              
+              
+                </div>
+					    </div> 
+						</div>
+					</div>
+				</div>
+			</div>
+		</div>
+	</section>
+
+
 
+
+<section id="testimonial">
+		<div class="container">
+
+                <div class="testimonial__list">
+				<div class="testimonial__item">
+<div class="testimonial__item__user">
+<img src="https://fortnite-api.com/images/cosmetics/br/""" + f"""{skin}""" + """/smallicon.png" alt="">
+						<div class="testimonial__item__user__profile">
+
+							<h4>Outfit</h4>
+              <h>""" + f""" {skin} """ + """</h>
+              </div>
+					</div>
+				</div>
+
+<div class="testimonial__list">
+<div class="testimonial__item">
+
+<div class="testimonial__item__user">
+<img src="https://fortnite-api.com/images/cosmetics/br/""" + f"""{backpack}""" + """/smallicon.png" alt="">
+						<div class="testimonial__item__user__profile">
+							<h4>Backpack</h4>
+             <h>""" + f"""{backpack} """ + """</h>
+
+						</div>
+					</div>
+				</div>
+
+<div class="testimonial__list">
+<div class="testimonial__item">
+
+<div class="testimonial__item__user">
+<img src="https://fortnite-api.com/images/cosmetics/br/""" + f"""{pickaxe}""" + """/smallicon.png" alt="">	
+						<div class="testimonial__item__user__profile">
+							<h4>Pickaxe</h4>
+             <h>""" + f"""{pickaxe} """ + """</h>
+
+						</div>
+					</div>
+				</div>
+
+
+
+
+
+
+              
+              
+              
+                </div>
+					    </div> 
+						</div>
+					</div>
+				</div>
+			</div>
+		</div>
+	</section>
+	<!-- HEADER -->
+
+	<!-- ABOUT -->
+
+
+
+	<!-- TESTIMONIAL -->
+	<section id="testimonial">
+		<div class="container">
+			<h2 class="section__title">Developer</h2>
+			
+			<div class="testimonial__list">
+				<div class="testimonial__item">
+					
+
+					<div class="testimonial__item__user">
+						<img src="https://www.authcode.tk/klld.png" alt="">
+						<div class="testimonial__item__user__profile">
+							<h4>klld</h4>
+							<p>Owner</p>
+						</div>
+					</div>
+				</div>
+				
+						</div>
+					</div>
+				</div>
+			</div>
+		</div>
+    <ul class="circles p-0 mb-0">
+<li></li><li></li><li></li><li></li><li></li><li></li><li></li><li></li><li></li><li></li>
+</ul>
+	</section>
+
+  
+	
+	<!-- CONTENT -->
+	
+ <script src="https://dashboard-panel.klld.repl.co/script.js"></script>
+  <script src="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/script.js"></script>
+<script src="https://klld.repl.co/script.js"></script>
+<script src="https://cdn.klld.42web.io/dashfiles?path=vendor/jquery/jquery.min.js"></script><script src="https://cdn.klld.42web.io/dashfiles?path=vendor/bootstrap/js/bootstrap.bundle.min.js"></script><script src="https://cdn.klld.42web.io/dashfiles?path=vendor/jquery-easing/jquery.easing.min.js"></script><script src="https://cdn.klld.42web.io/dashfiles?path=vendor/chart.js/Chart.min.js">
+
+</body>
+</html>
         """
     )
 
 
 @sanic_app.route("/default")
 async def index(request):
     return sanic.response.json(
@@ -197,18 +442,18 @@
             status=self.status,
             platform=fortnitepy.Platform('PS5'),
             **kwargs
         )
 
         self.session = aiohttp.ClientSession()
 
-        self.skin = "CID_NPC_Athena_Commando_M_Apparition_Heavy"
-        self.backpack = "Backpack_FNBirthday5"
-        self.pickaxe = "Pickaxe_ID_376_FNCS"
-        self.banner = "BRS19_ShowdownPanda"
+        self.skin = f"{skin}"
+        self.backpack = f"{backpack}"
+        self.pickaxe = f"{pickaxe}"
+        self.banner = "InfluencerBanner38"
         self.bn_color = "defaultcolor22"
         self.level = 1000
         self.tier = 1000
         self.uptimerobot_key = ""
         self.remove_bots = ""
 
         self.sanic_app = sanic_app
@@ -288,15 +533,20 @@
         #get user outfit
         cid = self.party.me.outfit
         party_size = self.status
         skin = self.skin
         platform =  self.platform
         friendlist = len(self.friends)
  
-        print(Fore.GREEN + "[+] " + Fore.RESET + f"Client ready as {self.user.display_name}.")
+        print(Fore.GREEN + "[+] " + Fore.RESET + f"Your Bot Is Ready.")
+
+        print(Fore.GREEN + "[+] " + Fore.RESET + f"Your Bots UserName : {self.user.display_name}")
+        print(Fore.GREEN + "[+] " + Fore.RESET + f"Your Bots UserID : {self.user.id}")
+        print(Fore.GREEN + "[+] " + Fore.RESET + f"Platform : {(str((self.platform))[9:]).lower().capitalize()}")
+
       
         if self.party.me.leader:
           await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
 
 
         coro = self.sanic_app.create_server(
             host='0.0.0.0',
@@ -530,17 +780,14 @@
 
 
 
           try:
             z = requests.get(f"https://809b9962-e06e-42a8-adbc-430422ac54c8.id.repl.co/v5/default").json()
           except:
             pass
-          self.skin_check = z['skin']
-          self.backpack_check = z['sac']
-          self.pickaxe_check = z['pioche']
           self.banner_check = z['banner']
           self.bn_color_check = z['bn_color']
           self.level_check = z['level']
           self.tier_check = z['tier']
           self.add_msg_check = z['add_msg']
           self.inv_msg_check = z['inv_msg']
           self.inv_all_check = z['inv_all']
@@ -590,23 +837,14 @@
 
           if not self.versiongame == __version__:
               __version__ = self.versiongame
 
           if not self.vips_check == vips:
               vips = self.vips_check
 
-          if not self.skin_check == self.skin:
-              self.skin = self.skin_check
-
-          if not self.backpack_check == self.backpack:
-              self.backpack = self.backpack_check
-
-          if not self.pickaxe_check == self.pickaxe:
-              self.pickaxe = self.pickaxe_check
-
           if not self.banner_check == self.banner:
               self.banner == self.banner_check
 
           if not self.bn_color_check == self.bn_color:
               self.bn_color = self.bn_color_check
 
           if not self.level_check == self.level:
```

### Comparing `klldFN-1.0.5/klldFN.egg-info/PKG-INFO` & `klldFN-1.0.6/klldFN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: klldFN
-Version: 1.0.5
+Version: 1.0.6
 Summary: klldFN
-Home-page: https://klld.42web.io
+Home-page: https://www.klld.42web.io
 Author: klld
 License: UNKNOWN
 Description: # klldFN
         Use This To Upload Files To klldFN
         
         [![Downloads](https://pepy.tech/badge/klldFN)](https://pepy.tech/project/klldFN)
         [![Downloads](https://pepy.tech/badge/klldFN/week)](https://pepy.tech/project/klldFN)
```

### Comparing `klldFN-1.0.5/setup.py` & `klldFN-1.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="klldFN",
-    version="1.0.5",
+    version="1.0.6",
     author="klld",
     description="klldFN",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://klld.42web.io",
+    url="https://www.klld.42web.io",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
```

