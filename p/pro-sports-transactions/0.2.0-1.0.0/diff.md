# Comparing `tmp/pro_sports_transactions-0.2.0.tar.gz` & `tmp/pro_sports_transactions-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pro_sports_transactions-0.2.0.tar", max compression
+gzip compressed data, was "pro_sports_transactions-1.0.0.tar", max compression
```

## Comparing `pro_sports_transactions-0.2.0.tar` & `pro_sports_transactions-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-05-14 17:50:23.756712 pro_sports_transactions-0.2.0/LICENSE
--rw-r--r--   0        0        0     5066 2023-05-18 21:02:37.352728 pro_sports_transactions-0.2.0/README.md
--rw-r--r--   0        0        0     1396 2023-05-18 21:04:24.747503 pro_sports_transactions-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      103 2023-05-18 21:02:37.390633 pro_sports_transactions-0.2.0/src/pro_sports_transactions/__init__.py
--rw-r--r--   0        0        0     5399 2023-05-18 21:02:37.417001 pro_sports_transactions-0.2.0/src/pro_sports_transactions/search.py
--rw-r--r--   0        0        0     6448 1970-01-01 00:00:00.000000 pro_sports_transactions-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 17:50:23.756712 pro_sports_transactions-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5286 2023-05-22 13:48:25.269219 pro_sports_transactions-1.0.0/README.md
+-rw-r--r--   0        0        0     1440 2023-05-22 13:48:53.882963 pro_sports_transactions-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-05-18 21:02:37.390633 pro_sports_transactions-1.0.0/src/pro_sports_transactions/__init__.py
+-rw-r--r--   0        0        0     5566 2023-05-22 13:27:04.438977 pro_sports_transactions-1.0.0/src/pro_sports_transactions/search.py
+-rw-r--r--   0        0        0     6700 1970-01-01 00:00:00.000000 pro_sports_transactions-1.0.0/PKG-INFO
```

### Comparing `pro_sports_transactions-0.2.0/LICENSE` & `pro_sports_transactions-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pro_sports_transactions-0.2.0/README.md` & `pro_sports_transactions-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Pro Sports Transactions API
 ===============
 
-An API for Software Engineers, Data Scientists, and sports fans of all to over the world to easily pull transactional data from https://www.prosportstransactions.com/.
+Pro Sports Transactions is a Python API client-library for https://www.prosportstransactions.com enabling software engineers, data scientists, and sports fans with the ability to easily retrieve trades, free agent movements, signings, injuries, disciplinary actions, legal/criminal actions, and much more for five of the North American professional leagues: MLB, MLS, NBA, NFL, and NHL.
 
 &nbsp;
 # About
 What is sports data without the transactions?
 - "Did he just throw his mouthpiece into the stands?"
 - "Yep."
 
@@ -20,15 +20,15 @@
 import pro_sports_transactions as pst
 
 # League (MLB, MLS, NBA, NFL, and NHL)
 league = pst.League.NBA
 
 # Disciplinary Actions, Injured List, Injuries,
 # Legal Incidents, Minor League To/For, Personal Reasons,
-# and General (e.g., Trades, Acquisitions, Waivers, Draft Picks, etc.)
+# and Movement (e.g., Trades, Acquisitions, Waivers, Draft Picks, etc.)
 transaction_types = tuple([t for t in pst.TransactionType])
 
 # From the start of the 2022-23 NBA Regular Season
 start_date = date.fromisoformat("2022-10-18")
 
 # From the end of the 2022-23 NBA Regular Season
 end_date = date.fromisoformat("2023-04-09")
```

### Comparing `pro_sports_transactions-0.2.0/pyproject.toml` & `pro_sports_transactions-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "pro_sports_transactions"
-version = "0.2.0"
+version = "1.0.0"
 description = "A Python Library for Consuming Transactions from Pro Sports Transactions (https://www.prosportstransactions.com)"
 license = "MIT"
 authors = ["Randy Forbes <randy.forbes@gmail.com>"]
 readme = "README.md"
 maintainers = ["Randy Forbes <randy.forbes@gmail.com>"]
 repository = "https://github.com/rsforbes/pro_sports_transactions"
 documentation = "https://github.com/rsforbes/pro_sports_transactions/blob/main/README.md"
-keywords = ["api", "data science", "basketball", "prosports", "prosportstransactions", "pro sports", "pro sports transactions", "trades", "draft", "transactions", "injuries", "fines", "data", "nba", "mlb", "mls", "nfl", "nhl","sports", "stats"]
+keywords = ["api", "basketball", "baseball", "data", "data science", "draft", "fines", "football", "hockey", "injuries", "mlb", "mls", "nba", "nfl", "nhl", "prosports", "prosportstransactions", "pro sports", "pro sports transactions", "soccer","sports", "stats", "trades", "transactions"]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development"
 ]
```

### Comparing `pro_sports_transactions-0.2.0/src/pro_sports_transactions/search.py` & `pro_sports_transactions-1.0.0/src/pro_sports_transactions/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class TransactionType(Enum):
     Disciplinary = {"default": "DisciplinaryChkBx"}
     InjuredList = {"default": "ILChkBx", "MLB": "DLChkBx"}
     Injury = {"default": "InjuriesChkBx"}
     LegalIncident = {"default": "LegalChkBx"}
     MinorLeagueToFrom = {"default": "NBADLChkBx", "MLB": "MinorsChkBx"}
-    General = {"default": "PlayerMovementChkBx"}
+    Movement = {"default": "PlayerMovementChkBx"}
     PersonalReason = {"default": "PersonalChkBx"}
 
     def __getitem__(cls, value):
         if type(value) == League:
             name = value.name
             return cls.value[name] if name in cls.value else cls.value["default"]
         else:
@@ -58,19 +58,22 @@
         # Generic DataFrame to hold results
         response = await Http.get(self._url)
 
         df = None
         try:
             df_list = read_html(response, header=0, keep_default_na=False)
             df = pd.DataFrame(
-                df_list[0], columns=["Date", "Team", "Acquired", "Relinquished", "Notes"]
+                df_list[0],
+                columns=["Date", "Team", "Acquired", "Relinquished", "Notes"],
             )
             df.attrs["pages"] = int(df_list[1].columns[2].split(" ")[-1])
         except Exception as e:
-            df = pd.DataFrame(columns=["Date", "Team", "Acquired", "Relinquished", "Notes"])
+            df = pd.DataFrame(
+                columns=["Date", "Team", "Acquired", "Relinquished", "Notes"]
+            )
             df.attrs["pages"] = 0
             df.attrs["errors"] = (repr(e),)
 
         return df
 
     async def get_dict(self):
         df = await self._get_dataframe()
@@ -158,18 +161,24 @@
         params |= Parameter.player(player)
         params |= Parameter.team(team)
         params |= Parameter.starting_row(starting_row)
         params |= Parameter.submit()
 
         # Add all Transaction Type parameter values
         for transaction_type in transaction_types:
-            params |= Parameter.transaction_type(TransactionType[transaction_type.name][league])
+            params |= Parameter.transaction_type(
+                TransactionType[transaction_type.name][league]
+            )
 
         return f"{netloc}/{league.value}/{path}?{parse.urlencode(params)}"
 
 
 class Http:
     @staticmethod
     async def get(url):
         async with aiohttp.ClientSession(headers=headers) as session:
             async with session.get(url) as response:
-                return None if response.status != 200 else await response.text(encoding="utf-8")
+                return (
+                    None
+                    if response.status != 200
+                    else await response.text(encoding="utf-8")
+                )
```

### Comparing `pro_sports_transactions-0.2.0/PKG-INFO` & `pro_sports_transactions-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pro-sports-transactions
-Version: 0.2.0
+Version: 1.0.0
 Summary: A Python Library for Consuming Transactions from Pro Sports Transactions (https://www.prosportstransactions.com)
 Home-page: https://github.com/rsforbes/pro_sports_transactions
 License: MIT
-Keywords: api,data science,basketball,prosports,prosportstransactions,pro sports,pro sports transactions,trades,draft,transactions,injuries,fines,data,nba,mlb,mls,nfl,nhl,sports,stats
+Keywords: api,basketball,baseball,data,data science,draft,fines,football,hockey,injuries,mlb,mls,nba,nfl,nhl,prosports,prosportstransactions,pro sports,pro sports transactions,soccer,sports,stats,trades,transactions
 Author: Randy Forbes
 Author-email: randy.forbes@gmail.com
 Maintainer: Randy Forbes
 Maintainer-email: randy.forbes@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -26,15 +26,15 @@
 Project-URL: Documentation, https://github.com/rsforbes/pro_sports_transactions/blob/main/README.md
 Project-URL: Repository, https://github.com/rsforbes/pro_sports_transactions
 Description-Content-Type: text/markdown
 
 Pro Sports Transactions API
 ===============
 
-An API for Software Engineers, Data Scientists, and sports fans of all to over the world to easily pull transactional data from https://www.prosportstransactions.com/.
+Pro Sports Transactions is a Python API client-library for https://www.prosportstransactions.com enabling software engineers, data scientists, and sports fans with the ability to easily retrieve trades, free agent movements, signings, injuries, disciplinary actions, legal/criminal actions, and much more for five of the North American professional leagues: MLB, MLS, NBA, NFL, and NHL.
 
 &nbsp;
 # About
 What is sports data without the transactions?
 - "Did he just throw his mouthpiece into the stands?"
 - "Yep."
 
@@ -49,15 +49,15 @@
 import pro_sports_transactions as pst
 
 # League (MLB, MLS, NBA, NFL, and NHL)
 league = pst.League.NBA
 
 # Disciplinary Actions, Injured List, Injuries,
 # Legal Incidents, Minor League To/For, Personal Reasons,
-# and General (e.g., Trades, Acquisitions, Waivers, Draft Picks, etc.)
+# and Movement (e.g., Trades, Acquisitions, Waivers, Draft Picks, etc.)
 transaction_types = tuple([t for t in pst.TransactionType])
 
 # From the start of the 2022-23 NBA Regular Season
 start_date = date.fromisoformat("2022-10-18")
 
 # From the end of the 2022-23 NBA Regular Season
 end_date = date.fromisoformat("2023-04-09")
```

