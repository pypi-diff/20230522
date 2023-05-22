# Comparing `tmp/CardGameBase-1.0.2.tar.gz` & `tmp/CardGameBase-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CardGameBase-1.0.2.tar", last modified: Tue May 16 13:07:40 2023, max compression
+gzip compressed data, was "CardGameBase-1.0.3.tar", last modified: Mon May 22 14:04:58 2023, max compression
```

## Comparing `CardGameBase-1.0.2.tar` & `CardGameBase-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:07:40.892034 CardGameBase-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-16 13:07:40.882207 CardGameBase-1.0.2/CardGameBase/
--rw-rw-rw-   0        0        0     3116 2023-05-16 09:08:46.000000 CardGameBase-1.0.2/CardGameBase/Card.py
--rw-rw-rw-   0        0        0     6242 2023-05-16 10:12:24.000000 CardGameBase-1.0.2/CardGameBase/Deck.py
--rw-rw-rw-   0        0        0       39 2023-04-13 10:08:54.000000 CardGameBase-1.0.2/CardGameBase/Exceptions.py
--rw-rw-rw-   0        0        0     7743 2023-05-16 10:42:22.000000 CardGameBase-1.0.2/CardGameBase/Hand.py
--rw-rw-rw-   0        0        0      970 2023-04-14 08:52:08.000000 CardGameBase-1.0.2/CardGameBase/Utility.py
--rw-rw-rw-   0        0        0      119 2023-04-13 10:09:58.000000 CardGameBase-1.0.2/CardGameBase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:07:40.892034 CardGameBase-1.0.2/CardGameBase.egg-info/
--rw-rw-rw-   0        0        0     1499 2023-05-16 13:07:40.000000 CardGameBase-1.0.2/CardGameBase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-05-16 13:07:40.000000 CardGameBase-1.0.2/CardGameBase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:07:40.000000 CardGameBase-1.0.2/CardGameBase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-16 13:07:40.000000 CardGameBase-1.0.2/CardGameBase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1235 2023-05-16 07:57:54.000000 CardGameBase-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1499 2023-05-16 13:07:40.892034 CardGameBase-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-05-16 11:03:15.000000 CardGameBase-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 13:07:40.892034 CardGameBase-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1171 2023-05-16 13:07:38.000000 CardGameBase-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:04:58.120648 CardGameBase-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:04:58.105009 CardGameBase-1.0.3/CardGameBase/
+-rw-rw-rw-   0        0        0     3116 2023-05-16 09:08:46.000000 CardGameBase-1.0.3/CardGameBase/Card.py
+-rw-rw-rw-   0        0        0     6242 2023-05-16 10:12:24.000000 CardGameBase-1.0.3/CardGameBase/Deck.py
+-rw-rw-rw-   0        0        0       39 2023-04-13 10:08:54.000000 CardGameBase-1.0.3/CardGameBase/Exceptions.py
+-rw-rw-rw-   0        0        0     7854 2023-05-22 13:37:46.000000 CardGameBase-1.0.3/CardGameBase/Hand.py
+-rw-rw-rw-   0        0        0      970 2023-04-14 08:52:08.000000 CardGameBase-1.0.3/CardGameBase/Utility.py
+-rw-rw-rw-   0        0        0      119 2023-04-13 10:09:58.000000 CardGameBase-1.0.3/CardGameBase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:04:58.120648 CardGameBase-1.0.3/CardGameBase.egg-info/
+-rw-rw-rw-   0        0        0     1499 2023-05-22 14:04:57.000000 CardGameBase-1.0.3/CardGameBase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-05-22 14:04:58.000000 CardGameBase-1.0.3/CardGameBase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:04:57.000000 CardGameBase-1.0.3/CardGameBase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-22 14:04:57.000000 CardGameBase-1.0.3/CardGameBase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1235 2023-05-16 07:57:54.000000 CardGameBase-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1499 2023-05-22 14:04:58.120648 CardGameBase-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-05-16 11:03:15.000000 CardGameBase-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 14:04:58.120648 CardGameBase-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1171 2023-05-22 14:01:45.000000 CardGameBase-1.0.3/setup.py
```

### Comparing `CardGameBase-1.0.2/CardGameBase/Card.py` & `CardGameBase-1.0.3/CardGameBase/Card.py`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.2/CardGameBase/Deck.py` & `CardGameBase-1.0.3/CardGameBase/Deck.py`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.2/CardGameBase/Hand.py` & `CardGameBase-1.0.3/CardGameBase/Hand.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,23 +80,25 @@
                     self.hand = fixed_hand
                 return self.rules
 
     def get_total_value(self, symbol : str = None, with_rank: bool = False) -> int:
         """
         Get the value of all cards in hand
         :param symbol: if set only cards with the given symbol are counted
-        :param with_rank: when set the value of the card is multiplied by the symbol_rank
+        :param with_rank: when set the value of the card is multiplied by the cards symbol_rank
         :return: The sum
         """
         _sum = 0
         if symbol:
             if with_rank:
                 for card in self.hand:
                     if card.symbol == symbol:
                         _sum += card.value * card.symbol_rank
+                    elif symbol is None:
+                        _sum += card.value * card.symbol_rank
                 return _sum
 
             for card in self.hand:
                 if card.symbol == symbol:
                     _sum += card.value
             return _sum
```

### Comparing `CardGameBase-1.0.2/CardGameBase/Utility.py` & `CardGameBase-1.0.3/CardGameBase/Utility.py`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.2/CardGameBase.egg-info/PKG-INFO` & `CardGameBase-1.0.3/CardGameBase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CardGameBase
-Version: 1.0.2
+Version: 1.0.3
 Summary: Card Game Base with basic deck and card class
 Home-page: https://github.com/DerSchinken/CardGameBase/
 Author: DerSchinken
 Maintainer: DerSchinken
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `CardGameBase-1.0.2/LICENSE` & `CardGameBase-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.2/PKG-INFO` & `CardGameBase-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CardGameBase
-Version: 1.0.2
+Version: 1.0.3
 Summary: Card Game Base with basic deck and card class
 Home-page: https://github.com/DerSchinken/CardGameBase/
 Author: DerSchinken
 Maintainer: DerSchinken
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `CardGameBase-1.0.2/README.md` & `CardGameBase-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.2/setup.py` & `CardGameBase-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get requirements
 with open("requirements.txt", "r") as reqs:
     requirements = reqs.read().splitlines()
 
 setup(
     name="CardGameBase",
-    version="1.0.2",
+    version="1.0.3",
     # Major version 1
     # Minor version 0
     # Maintenance version 0
 
     author="DerSchinken",
     maintainer="DerSchinken",
     description="Card Game Base with basic deck and card class",
```

