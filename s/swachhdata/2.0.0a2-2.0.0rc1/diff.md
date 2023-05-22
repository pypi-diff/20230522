# Comparing `tmp/swachhdata-2.0.0a2-py3-none-any.whl.zip` & `tmp/swachhdata-2.0.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,23 @@
-Zip file size: 23124 bytes, number of entries: 19
--rw-r--r--  2.0 unx      227 b- defN 23-May-22 04:14 swachhdata/__init__.py
+Zip file size: 26195 bytes, number of entries: 21
+-rw-r--r--  2.0 unx      228 b- defN 23-May-22 04:01 swachhdata/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 23-May-21 04:19 swachhdata/compose/__init__.py
 -rw-r--r--  2.0 unx     1334 b- defN 23-May-21 20:59 swachhdata/compose/core.py
 -rw-r--r--  2.0 unx      131 b- defN 22-Jan-25 09:02 swachhdata/image/__init__.py
 -rw-r--r--  2.0 unx     7477 b- defN 22-Jan-25 09:02 swachhdata/image/_image.py
--rw-r--r--  2.0 unx      805 b- defN 23-May-22 04:07 swachhdata/text/__init__.py
--rw-r--r--  2.0 unx     1473 b- defN 23-May-22 04:03 swachhdata/text/_base.py
--rw-r--r--  2.0 unx    73401 b- defN 23-May-22 04:06 swachhdata/text/_text.py
+-rw-r--r--  2.0 unx      173 b- defN 22-Jan-25 09:02 swachhdata/legacy/__init__.py
+-rw-r--r--  2.0 unx    15947 b- defN 23-Mar-10 23:37 swachhdata/legacy/_text.py
+-rw-r--r--  2.0 unx      803 b- defN 23-May-22 04:00 swachhdata/text/__init__.py
+-rw-r--r--  2.0 unx     2196 b- defN 23-May-21 21:30 swachhdata/text/_base.py
+-rw-r--r--  2.0 unx    74326 b- defN 23-May-22 03:57 swachhdata/text/_text.py
 -rw-r--r--  2.0 unx      642 b- defN 23-May-21 03:53 swachhdata/utils/__init__.py
 -rw-r--r--  2.0 unx     1114 b- defN 23-May-22 01:57 swachhdata/utils/exceptions.py
 -rw-r--r--  2.0 unx      377 b- defN 23-May-22 02:30 swachhdata/utils/probe.py
 -rw-r--r--  2.0 unx     1150 b- defN 23-May-21 14:42 swachhdata/utils/recast.py
 -rw-r--r--  2.0 unx      480 b- defN 23-May-21 03:06 swachhdata/utils/tools.py
 -rw-r--r--  2.0 unx     1310 b- defN 23-May-21 14:42 swachhdata/utils/verify.py
--rw-rw-rw-  2.0 unx    17096 b- defN 23-May-22 04:14 swachhdata-2.0.0a2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2205 b- defN 23-May-22 04:14 swachhdata-2.0.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 04:14 swachhdata-2.0.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 04:14 swachhdata-2.0.0a2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1575 b- defN 23-May-22 04:14 swachhdata-2.0.0a2.dist-info/RECORD
-19 files, 111006 bytes uncompressed, 20548 bytes compressed:  81.5%
+-rw-rw-rw-  2.0 unx    17096 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2206 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1749 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/RECORD
+21 files, 128948 bytes uncompressed, 23347 bytes compressed:  81.9%
```

## zipnote {}

```diff
@@ -9,14 +9,20 @@
 
 Filename: swachhdata/image/__init__.py
 Comment: 
 
 Filename: swachhdata/image/_image.py
 Comment: 
 
+Filename: swachhdata/legacy/__init__.py
+Comment: 
+
+Filename: swachhdata/legacy/_text.py
+Comment: 
+
 Filename: swachhdata/text/__init__.py
 Comment: 
 
 Filename: swachhdata/text/_base.py
 Comment: 
 
 Filename: swachhdata/text/_text.py
@@ -36,23 +42,23 @@
 
 Filename: swachhdata/utils/tools.py
 Comment: 
 
 Filename: swachhdata/utils/verify.py
 Comment: 
 
-Filename: swachhdata-2.0.0a2.dist-info/LICENSE.txt
+Filename: swachhdata-2.0.0rc1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: swachhdata-2.0.0a2.dist-info/METADATA
+Filename: swachhdata-2.0.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: swachhdata-2.0.0a2.dist-info/WHEEL
+Filename: swachhdata-2.0.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: swachhdata-2.0.0a2.dist-info/top_level.txt
+Filename: swachhdata-2.0.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: swachhdata-2.0.0a2.dist-info/RECORD
+Filename: swachhdata-2.0.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swachhdata/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = '2.0.0a2'
+__version__ = '2.0.0rc1'
 __author__ = 'Kritik Seth'
 __maintainer__ = __author__
 __license__ = 'Mozilla Public License Version 2.0'
 __url__ = 'https://swachhdata.readthedocs.io/'
 __connect__ = 'https://www.kritikseth.com/'
```

## swachhdata/text/__init__.py

```diff
@@ -6,15 +6,15 @@
     ContractionsRecast,
     CaseRecast,
     HashtagsRecast,
     ShortWordsRecast,
     StopWordsRecast,
     NumberRecast,
     AlphabetRecast,
-    PunctuationsRecast,
+    PunctuationRecast,
     StemmingRecast,
     LemmatizationRecast,
     TokenisationRecast,
     TextRecast,
     RecastPipeline
 )
 
@@ -26,14 +26,14 @@
     'ContractionsRecast',
     'CaseRecast',
     'HashtagsRecast',
     'ShortWordsRecast',
     'StopWordsRecast',
     'NumberRecast',
     'AlphabetRecast',
-    'PunctuationsRecast',
+    'PunctuationRecast',
     'StemmingRecast',
     'LemmatizationRecast',
     'TokenisationRecast',
     'TextRecast',
     'RecastPipeline'
 ]
```

## swachhdata/text/_base.py

```diff
@@ -1,14 +1,43 @@
+import pandas
 from ..compose.core import BaseTextDatum
 from ..utils.exceptions import (
     IncorrectProcessDataType,
     IncorrectVerboseDataType,
     SetupNotImplementedError
 )
 
+class TextFormatter:
+    """
+    Base Data Formatter for all recasts in swachhdata.text module
+
+    Accepted text input format:
+        * string
+        * list of string
+        * pandas.core.series.Series
+    """
+
+    def __init__(self):
+        
+        self._dtype = None
+        self._text = None
+        self._count = None
+    
+    def __text_formatter(self):
+        
+        self._count = len(self._text)
+
+        if self._dtype == pandas.core.series.Series:
+            self._text = self._text.tolist()
+            self._dtype = type(self._text)
+
+        if self._dtype == str:
+            self._count = len(self._text.split())
+            self._dtype = type(self._text)
+
 class BaseTextRecast(BaseTextDatum):
 
     def __init__(self, process=None, verbose=0):
         """
         Initialize
         """
         super().__init__()
```

## swachhdata/text/_text.py

```diff
@@ -14,15 +14,15 @@
 import string
 
 import emoji
 from emoji import EMOJI_DATA
 
 from tqdm.auto import trange, tqdm
 
-from ._base import BaseTextRecast
+from ._base import TextFormatter, BaseTextRecast
 from ..utils import probe_string_data
 
 class urlRecast(BaseTextRecast):
     """Recast text data by removing or extracting URLs.
 
     URLs supported:
         * HTTP address: http://www.website.com
@@ -263,15 +263,15 @@
         else:
             return self.recast()
 
 
 ##############################################################################################################
 
 
-class EscapeSequencesRecast(BaseTextRecast):
+class EscapeSequencesRecast(TextFormatter):
     """Recast text data by removing Escape Sequences.
 
     Parameters
     ----------
     verbose: int (0, 1, -1), default=0
     
 
@@ -287,42 +287,76 @@
     >>> rec.setup_recast(text)
     'To have a look at the menu Click Here'
     """
 
 
     def __init__(self, verbose=0):
 
-        super().__init__(verbose=verbose)
+        TextFormatter.__init__(self)
+        self.__setup = False
+        self.__verbose_status = True
+        self.__verbose = verbose
+        if self.__verbose == -1:
+            self.__verbose_status = False
+
+        try:
+            assert(isinstance(self.__verbose, int))
+        except:
+            print(f'Expected verbose input type <class \'int\'>, input type received {type(self.__verbose)}')
     
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Returns
         -------
         ntext : string
             Processed text
         """
 
         ntext = text.replace('\r', ' ').replace('\n', ' ').replace('\t', ' ').replace('\n', ' ').replace('\f', ' ')
         return ntext
 
+
     def recast(self):
         """Perform selected process on the setup text
 
         Returns
         -------
         ntext : string / list of strings 
             Processed text
         """
-        super().recast()
         
-        data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
-        data_tqdm.set_postfix({'EscapeSequencesRecast process': 'remove'})
-        recast_text = [self.__base_recast(text) for text in data_tqdm]
-        return recast_text
+        try:
+            assert(self.__setup)
+        except:
+            print(f'method setup needs to be called before recast')
+        
+        if self._dtype == str:
+
+            return self.__base_recast(self._text)
+
+        elif self._dtype == list:
+
+            if self.__verbose == 0:
+
+                ntext = []
+                for text in self._text:
+                    ntext.append(self.__base_recast(text))
+                return ntext
+            
+            if self.__verbose == 1 or self.__verbose == -1:
+
+                ntext = []
+                progress_bar = trange(self._count, leave=self.__verbose_status)
+                for i in progress_bar:
+                    progress_bar.set_postfix({'EscapeSequenceRecast process': 'removing'})
+                    text = self._text[i]
+                    ntext.append(self.__base_recast(text))
+                return ntext
+
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
         Parameters
@@ -330,19 +364,17 @@
         text : string / list of strings / pandas.core.series.Series
 
         Returns
         -------
         ntext : string / list of strings (process='remove')
             Processed text
         """
-        if not self._setup_check:
-            self.setup(text)
-            return self.recast()
-        else:
-            return self.recast()
+
+        self.setup(text)
+        return self.recast()
 
 
 ##############################################################################################################
 
 
 class MentionsRecast(BaseTextRecast):
     """Recast text data by removing or extracting Mentions.
```

## Comparing `swachhdata-2.0.0a2.dist-info/LICENSE.txt` & `swachhdata-2.0.0rc1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `swachhdata-2.0.0a2.dist-info/METADATA` & `swachhdata-2.0.0rc1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swachhdata
-Version: 2.0.0a2
+Version: 2.0.0rc1
 Summary: Data cleaning made easy with swachhdata
 Home-page: https://swachhdata.readthedocs.io/
 Author: Kritik Seth
 Author-email: sethkritik@gmail.com
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swachhdata Version: 2.0.0a2 Summary: Data cleaning
+Metadata-Version: 2.1 Name: swachhdata Version: 2.0.0rc1 Summary: Data cleaning
 made easy with swachhdata Home-page: https://swachhdata.readthedocs.io/ Author:
 Kritik Seth Author-email: sethkritik@gmail.com Classifier: Natural Language ::
 English Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL
 2.0) Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 6 - Mature Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: regex (>=2019.12.20) Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: tqdm (>=4.41.1) Requires-Dist: beautifulsoup4 (>=4.6.3)
```

## Comparing `swachhdata-2.0.0a2.dist-info/RECORD` & `swachhdata-2.0.0rc1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-swachhdata/__init__.py,sha256=oZnCrt94EWUwobkGGwX3Q5WgiPGwg3rQNiblQdRMB7Q,227
+swachhdata/__init__.py,sha256=g8MaBSKSiE0Y9g5-dolAX83pg2SasVZYnJcEBGFFpr8,228
 swachhdata/compose/__init__.py,sha256=9NKRJN3d38FxfExXwK8L1jfi5IMI5jKqfEtFLt97LO8,106
 swachhdata/compose/core.py,sha256=-jqnUkAcIa8A--eoLGAWyqMKEooOm36bHWvzbrArC9A,1334
 swachhdata/image/__init__.py,sha256=m6pEvV60cN9cj5G-mMsr27F41s6A-IbPNIpmSwFvSmE,131
 swachhdata/image/_image.py,sha256=9RkuFHcWZOSVXWByBfvCnO6hhB19KLwia4QErqr6SY8,7477
-swachhdata/text/__init__.py,sha256=TTL7TowD8_m0Wx82IldvqEW8V_p03uNPYL1S-2tOf44,805
-swachhdata/text/_base.py,sha256=h69sC754xospdQWa_NZk_KiueDrL2zv_U2bBcLivdFo,1473
-swachhdata/text/_text.py,sha256=qDwT6SOgwhfxu53i1sy4sLQMeXEH_YzFtp9Yxl74yEo,73401
+swachhdata/legacy/__init__.py,sha256=MQGn-ahr-9jjg4T_hp1Btl39mSAuw7qw359evKHUnjk,173
+swachhdata/legacy/_text.py,sha256=lQqrPQunEwCeNf0hUBrxBBIp3e7iX-WRovYb0kHi1_4,15947
+swachhdata/text/__init__.py,sha256=w4DSub20tUcvJ5iommCEDw0Fu9Fvx7LQyVqO3Zs15-k,803
+swachhdata/text/_base.py,sha256=-VGYBegK3YrUazPUMNKFB2fwbciUG9KZsMfs-jTHIqo,2196
+swachhdata/text/_text.py,sha256=igBc1yP6nU-xcM9d5ma8Aa9U6EZzy11BGCgB5RaOgUE,74326
 swachhdata/utils/__init__.py,sha256=1ZH0VgYFVYuf0jTP8ncCxPxDnHBOEQ8OZgjy-iuvYlU,642
 swachhdata/utils/exceptions.py,sha256=4_cANml56Jeev2rEq4JDjxnqdK_cE1-ZO_CcFNBBNOU,1114
 swachhdata/utils/probe.py,sha256=q1p-R9CKXnq-eBNVSl1tyADefX64KHrlmxNElzM97TU,377
 swachhdata/utils/recast.py,sha256=WGu3HXRPDyrjXD5pLKfLfjqPBHSdfQezs1Ux4UoQZNA,1150
 swachhdata/utils/tools.py,sha256=1K9ekx8Lqt15GY7RuEH5-wgL_TtMEkEYyevN9KrP03I,480
 swachhdata/utils/verify.py,sha256=GbPuizBw7-BFRPMCLnaHDF2YnsjzABiLFzZzLOmlu10,1310
-swachhdata-2.0.0a2.dist-info/LICENSE.txt,sha256=k0P1sbYupRWlxoESvbYq2UzoMW6MXA84LltqR-4mEo4,17096
-swachhdata-2.0.0a2.dist-info/METADATA,sha256=Mh3niRLhmwhJD9q1ug_eMH_MaPl4F_4WDe_5DohQ4dk,2205
-swachhdata-2.0.0a2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-swachhdata-2.0.0a2.dist-info/top_level.txt,sha256=UPLFTkg5MwIkJLZzEOsLnndE5jByl-BGbZ0_Z40oq0Y,11
-swachhdata-2.0.0a2.dist-info/RECORD,,
+swachhdata-2.0.0rc1.dist-info/LICENSE.txt,sha256=k0P1sbYupRWlxoESvbYq2UzoMW6MXA84LltqR-4mEo4,17096
+swachhdata-2.0.0rc1.dist-info/METADATA,sha256=ENM5g6hdyqBicjj04bmvlnq_KzZ6RhFSx_2aScrBFOc,2206
+swachhdata-2.0.0rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+swachhdata-2.0.0rc1.dist-info/top_level.txt,sha256=UPLFTkg5MwIkJLZzEOsLnndE5jByl-BGbZ0_Z40oq0Y,11
+swachhdata-2.0.0rc1.dist-info/RECORD,,
```

