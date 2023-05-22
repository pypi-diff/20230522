# Comparing `tmp/ItsuBot-3.4.8.tar.gz` & `tmp/ItsuBot-4.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ItsuBot-3.4.8.tar", last modified: Sun May 14 23:39:38 2023, max compression
+gzip compressed data, was "dist\ItsuBot-4.5.8.tar", last modified: Mon May 22 16:29:47 2023, max compression
```

## Comparing `ItsuBot-3.4.8.tar` & `ItsuBot-4.5.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/
-drwxrwxrwx   0        0        0        0 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot/
--rw-rw-rw-   0        0        0    64899 2023-05-14 23:03:04.000000 ItsuBot-3.4.8/ItsuBot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/
--rw-rw-rw-   0        0        0      358 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      358 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/setup.cfg
--rw-rw-rw-   0        0        0      384 2023-05-14 23:39:18.000000 ItsuBot-3.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:29:47.000000 ItsuBot-4.5.8/
+drwxrwxrwx   0        0        0        0 2023-05-22 16:29:47.000000 ItsuBot-4.5.8/ItsuBot/
+-rw-rw-rw-   0        0        0    64752 2023-05-22 16:27:43.000000 ItsuBot-4.5.8/ItsuBot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:29:47.000000 ItsuBot-4.5.8/ItsuBot.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-05-22 16:29:47.000000 ItsuBot-4.5.8/ItsuBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-22 16:29:47.000000 ItsuBot-4.5.8/ItsuBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:29:47.000000 ItsuBot-4.5.8/ItsuBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 16:29:47.000000 ItsuBot-4.5.8/ItsuBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      358 2023-05-22 16:29:47.000000 ItsuBot-4.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:29:47.000000 ItsuBot-4.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      384 2023-05-22 16:29:36.000000 ItsuBot-4.5.8/setup.py
```

### Comparing `ItsuBot-3.4.8/ItsuBot/__init__.py` & `ItsuBot-4.5.8/ItsuBot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1176,19 +1176,15 @@
 
     @commands.command()
     async def cid(self, ctx: fortnitepy.ext.commands.Context, character_id: str) -> None:
         await self.party.me.set_outfit(asset=character_id,variants=self.party.me.create_variants(profile_banner='ProfileBanner'))
         await ctx.send(f'Skin set to {character_id}.')
         os.system('clear')
 
-    @is_admin()
-    @commands.command()
-    async def r(self, ctx: fortnitepy.ext.commands.Context) -> None:
-        await ctx.send(f'{self.url}')
-
+    
     @commands.command()
     async def eid(self, ctx: fortnitepy.ext.commands.Context, emote_id: str) -> None:
         await self.party.me.clear_emote()
         await self.party.me.set_emote(asset=emote_id)
         await ctx.send(f'Emote set to {emote_id}!')
         os.system('clear')
```

#### html2text {}

```diff
@@ -446,18 +446,16 @@
 fortnitepy.ext.commands.Context) -> None: await self.party.me.set_outfit
 (asset='CID_VIP_Athena_Commando_M_GalileoGondola_SG') await ctx.send('Skin set
 to Star Wars Hologram!') @commands.command() async def cid(self, ctx:
 fortnitepy.ext.commands.Context, character_id: str) -> None: await
 self.party.me.set_outfit
 (asset=character_id,variants=self.party.me.create_variants
 (profile_banner='ProfileBanner')) await ctx.send(f'Skin set to
-{character_id}.') os.system('clear') @is_admin() @commands.command() async def
-r(self, ctx: fortnitepy.ext.commands.Context) -> None: await ctx.send(f'
-{self.url}') @commands.command() async def eid(self, ctx:
-fortnitepy.ext.commands.Context, emote_id: str) -> None: await
+{character_id}.') os.system('clear') @commands.command() async def eid(self,
+ctx: fortnitepy.ext.commands.Context, emote_id: str) -> None: await
 self.party.me.clear_emote() await self.party.me.set_emote(asset=emote_id) await
 ctx.send(f'Emote set to {emote_id}!') os.system('clear') @commands.command()
 async def stop(self, ctx: fortnitepy.ext.commands.Context) -> None: await
 self.party.me.clear_emote() await ctx.send('Stopped emoting.') os.system
 ('clear') @commands.command() async def point(self, ctx:
 fortnitepy.ext.commands.Context, *, content: Optional[str] = None) -> None:
 await self.party.me.clear_emote() await self.party.me.set_emote
```

