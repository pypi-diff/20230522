# Comparing `tmp/lexikos-0.0.1rc1.tar.gz` & `tmp/lexikos-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikos-0.0.1rc1.tar", last modified: Tue May  9 09:59:02 2023, max compression
+gzip compressed data, was "lexikos-0.0.1rc2.tar", last modified: Mon May 22 09:51:57 2023, max compression
```

## Comparing `lexikos-0.0.1rc1.tar` & `lexikos-0.0.1rc2.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.336356 lexikos-0.0.1rc1/
--rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc1/LICENSE
--rw-r--r--   0 mac        (502) staff       (20)       16 2023-04-21 13:04:42.000000 lexikos-0.0.1rc1/MANIFEST.in
--rw-r--r--   0 mac        (502) staff       (20)    27155 2023-05-09 09:59:02.336612 lexikos-0.0.1rc1/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)    13431 2023-05-09 09:56:15.000000 lexikos-0.0.1rc1/README.md
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.300489 lexikos-0.0.1rc1/lexikos/
--rw-r--r--   0 mac        (502) staff       (20)       77 2023-05-09 09:58:42.000000 lexikos-0.0.1rc1/lexikos/__init__.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.297810 lexikos-0.0.1rc1/lexikos/dict/
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.308823 lexikos-0.0.1rc1/lexikos/dict/cmudict-ipa/
--rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc1/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
--rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc1/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.335995 lexikos-0.0.1rc1/lexikos/dict/wikipron/
--rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_au_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_in_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_us_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)     2911 2023-05-09 09:56:54.000000 lexikos-0.0.1rc1/lexikos/lexicon.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.302199 lexikos-0.0.1rc1/lexikos.egg-info/
--rw-r--r--   0 mac        (502) staff       (20)    27155 2023-05-09 09:59:02.000000 lexikos-0.0.1rc1/lexikos.egg-info/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)      923 2023-05-09 09:59:02.000000 lexikos-0.0.1rc1/lexikos.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (502) staff       (20)        1 2023-05-09 09:59:02.000000 lexikos-0.0.1rc1/lexikos.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (502) staff       (20)        8 2023-05-09 09:59:02.000000 lexikos-0.0.1rc1/lexikos.egg-info/top_level.txt
--rw-r--r--   0 mac        (502) staff       (20)      821 2023-05-09 09:58:55.000000 lexikos-0.0.1rc1/pyproject.toml
--rw-r--r--   0 mac        (502) staff       (20)      113 2023-05-09 09:59:02.337157 lexikos-0.0.1rc1/setup.cfg
--rw-r--r--   0 mac        (502) staff       (20)      964 2023-04-21 13:31:07.000000 lexikos-0.0.1rc1/setup.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.430474 lexikos-0.0.1rc2/
+-rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc2/LICENSE
+-rw-r--r--   0 mac        (502) staff       (20)       16 2023-04-21 13:04:42.000000 lexikos-0.0.1rc2/MANIFEST.in
+-rw-r--r--   0 mac        (502) staff       (20)    27905 2023-05-22 09:51:57.430731 lexikos-0.0.1rc2/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)    14181 2023-05-22 09:48:54.000000 lexikos-0.0.1rc2/README.md
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.365913 lexikos-0.0.1rc2/lexikos/
+-rw-r--r--   0 mac        (502) staff       (20)       77 2023-05-22 09:37:26.000000 lexikos-0.0.1rc2/lexikos/__init__.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.363481 lexikos-0.0.1rc2/lexikos/dict/
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.375674 lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/
+-rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.390810 lexikos-0.0.1rc2/lexikos/dict/synthetic/
+-rw-r--r--   0 mac        (502) staff       (20)      406 2023-05-19 10:04:44.000000 lexikos-0.0.1rc2/lexikos/dict/synthetic/austalk_en_au.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     2618 2023-05-19 10:05:54.000000 lexikos-0.0.1rc2/lexikos/dict/synthetic/sc_cw_en_au.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.429491 lexikos-0.0.1rc2/lexikos/dict/wikipron/
+-rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_au_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_in_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_us_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     2911 2023-05-09 09:56:54.000000 lexikos-0.0.1rc2/lexikos/lexicon.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.367453 lexikos-0.0.1rc2/lexikos.egg-info/
+-rw-r--r--   0 mac        (502) staff       (20)    27905 2023-05-22 09:51:57.000000 lexikos-0.0.1rc2/lexikos.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)     1003 2023-05-22 09:51:57.000000 lexikos-0.0.1rc2/lexikos.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (502) staff       (20)        1 2023-05-22 09:51:57.000000 lexikos-0.0.1rc2/lexikos.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (502) staff       (20)        8 2023-05-22 09:51:57.000000 lexikos-0.0.1rc2/lexikos.egg-info/top_level.txt
+-rw-r--r--   0 mac        (502) staff       (20)      821 2023-05-22 09:37:31.000000 lexikos-0.0.1rc2/pyproject.toml
+-rw-r--r--   0 mac        (502) staff       (20)      113 2023-05-22 09:51:57.431175 lexikos-0.0.1rc2/setup.cfg
+-rw-r--r--   0 mac        (502) staff       (20)      964 2023-04-21 13:31:07.000000 lexikos-0.0.1rc2/setup.py
```

### Comparing `lexikos-0.0.1rc1/LICENSE` & `lexikos-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/PKG-INFO` & `lexikos-0.0.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -296,29 +296,32 @@
 | Language       | Dictionary   | Phone Set | Corpus                                                                                                                     | G2P Model                                                                                                             |
 | -------------- | ------------ | --------- | -------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-US          | CMU Dict     | ARPA      | [External Link](https://github.com/microsoft/CNTK/blob/master/Examples/SequenceToSequence/CMUDict/Data/cmudict-0.7b.train) | [bookbot/byt5-small-cmudict](https://huggingface.co/bookbot/byt5-small-cmudict)                                       |
 | en-US          | CMU Dict IPA | IPA       | [External Link](https://github.com/menelik3/cmudict-ipa/blob/master/cmudict-0.7b-ipa.txt)                                  |                                                                                                                       |
 | en-US          | CharsiuG2P   | IPA       | [External Link](https://github.com/lingjzhu/CharsiuG2P/blob/main/dicts/eng-us.tsv)                                         | [charsiu/g2p_multilingual_byT5_small_100](https://huggingface.co/charsiu/g2p_multilingual_byT5_small_100)             |
 | en-US (Broad)  | Wikipron     | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_us_broad.tsv)                     | [bookbot/byt5-small-wikipron-eng-latn-us-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-us-broad) |
 | en-US (Narrow) | Wikipron     | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_us_narrow.tsv)                    |
+| en-US          | LibriSpeech  | IPA       | [Link](./lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv)                                          |                                                                                                                       |
 
 ### English `(en-UK)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                                                                  | G2P Model                                                                                                             |
 | -------------- | ---------- | --------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-UK          | CharsiuG2P | IPA       | [External Link](https://github.com/lingjzhu/CharsiuG2P/blob/main/dicts/eng-uk.tsv)                      | [charsiu/g2p_multilingual_byT5_small_100](https://huggingface.co/charsiu/g2p_multilingual_byT5_small_100)             |
 | en-UK (Broad)  | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-uk-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-uk-broad) |
 | en-UK (Narrow) | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-AU)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
-| en-AU (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
-| en-AU (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
+| Language       | Dictionary  | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ----------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-AU (Broad)  | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
+| en-AU (Narrow) | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
+| en-AU          | AusTalk (§) | IPA       | [Link](./lexikos/dict/synthetic/austalk_en_au.tsv)     |                                                                                                                       |
+| en-AU          | SC-CW (§)   | IPA       | [Link](./lexikos/dict/synthetic/sc_cw_en_au.tsv)       |                                                                                                                       |
 
 ### English `(en-CA)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
 | -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
 | en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  |           |
 | en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |           |
@@ -433,18 +436,18 @@
 ### Wikipron
 
 | Language Family        | Code                              | Region                                                | Corpus | G2P Model |
 | ---------------------- | --------------------------------- | ----------------------------------------------------- | :----: | :-------: |
 | African English        | en-ZA                             | South Africa                                          |        |           |
 | Australian English     | en-AU                             | Australia                                             |   ✅    |     ✅     |
 | East Asian English     | en-CN, en-HK, en-JP, en-KR, en-TW | China, Hong Kong, Japan, South Korea, Taiwan          |        |           |
-| European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |        |           |
+| European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |   🚧    |     🚧     |
 | Mexican English        | en-MX                             | Mexico                                                |        |           |
 | New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |           |
-| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |           |
+| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |     🚧     |
 | Middle Eastern English | en-EG, en-IL                      | Egypt, Israel                                         |        |           |
 | Southeast Asian        | en-TH, en-ID, en-MY, en-PH, en-SG | Thailand, Indonesia, Malaysia, Philippines, Singapore |        |           |
 | South Asian English    | en-IN                             | India                                                 |   ✅    |           |
   
 ## Resources
 
 - [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P)
```

### Comparing `lexikos-0.0.1rc1/README.md` & `lexikos-0.0.1rc2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -77,29 +77,32 @@
 | Language       | Dictionary   | Phone Set | Corpus                                                                                                                     | G2P Model                                                                                                             |
 | -------------- | ------------ | --------- | -------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-US          | CMU Dict     | ARPA      | [External Link](https://github.com/microsoft/CNTK/blob/master/Examples/SequenceToSequence/CMUDict/Data/cmudict-0.7b.train) | [bookbot/byt5-small-cmudict](https://huggingface.co/bookbot/byt5-small-cmudict)                                       |
 | en-US          | CMU Dict IPA | IPA       | [External Link](https://github.com/menelik3/cmudict-ipa/blob/master/cmudict-0.7b-ipa.txt)                                  |                                                                                                                       |
 | en-US          | CharsiuG2P   | IPA       | [External Link](https://github.com/lingjzhu/CharsiuG2P/blob/main/dicts/eng-us.tsv)                                         | [charsiu/g2p_multilingual_byT5_small_100](https://huggingface.co/charsiu/g2p_multilingual_byT5_small_100)             |
 | en-US (Broad)  | Wikipron     | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_us_broad.tsv)                     | [bookbot/byt5-small-wikipron-eng-latn-us-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-us-broad) |
 | en-US (Narrow) | Wikipron     | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_us_narrow.tsv)                    |
+| en-US          | LibriSpeech  | IPA       | [Link](./lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv)                                          |                                                                                                                       |
 
 ### English `(en-UK)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                                                                  | G2P Model                                                                                                             |
 | -------------- | ---------- | --------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-UK          | CharsiuG2P | IPA       | [External Link](https://github.com/lingjzhu/CharsiuG2P/blob/main/dicts/eng-uk.tsv)                      | [charsiu/g2p_multilingual_byT5_small_100](https://huggingface.co/charsiu/g2p_multilingual_byT5_small_100)             |
 | en-UK (Broad)  | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-uk-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-uk-broad) |
 | en-UK (Narrow) | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-AU)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
-| en-AU (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
-| en-AU (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
+| Language       | Dictionary  | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ----------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-AU (Broad)  | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
+| en-AU (Narrow) | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
+| en-AU          | AusTalk (§) | IPA       | [Link](./lexikos/dict/synthetic/austalk_en_au.tsv)     |                                                                                                                       |
+| en-AU          | SC-CW (§)   | IPA       | [Link](./lexikos/dict/synthetic/sc_cw_en_au.tsv)       |                                                                                                                       |
 
 ### English `(en-CA)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
 | -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
 | en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  |           |
 | en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |           |
@@ -214,18 +217,18 @@
 ### Wikipron
 
 | Language Family        | Code                              | Region                                                | Corpus | G2P Model |
 | ---------------------- | --------------------------------- | ----------------------------------------------------- | :----: | :-------: |
 | African English        | en-ZA                             | South Africa                                          |        |           |
 | Australian English     | en-AU                             | Australia                                             |   ✅    |     ✅     |
 | East Asian English     | en-CN, en-HK, en-JP, en-KR, en-TW | China, Hong Kong, Japan, South Korea, Taiwan          |        |           |
-| European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |        |           |
+| European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |   🚧    |     🚧     |
 | Mexican English        | en-MX                             | Mexico                                                |        |           |
 | New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |           |
-| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |           |
+| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |     🚧     |
 | Middle Eastern English | en-EG, en-IL                      | Egypt, Israel                                         |        |           |
 | Southeast Asian        | en-TH, en-ID, en-MY, en-PH, en-SG | Thailand, Indonesia, Malaysia, Philippines, Singapore |        |           |
 | South Asian English    | en-IN                             | India                                                 |   ✅    |           |
   
 ## Resources
 
 - [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P)
```

### Comparing `lexikos-0.0.1rc1/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv` & `lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv` & `lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_au_broad.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_au_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_au_narrow.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_au_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_ca_broad.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_ca_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_in_broad.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_in_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_in_narrow.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_in_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_nz_broad.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_nz_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_uk_broad.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_uk_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_us_broad.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_us_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_us_narrow.tsv` & `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_us_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos/lexicon.py` & `lexikos-0.0.1rc2/lexikos/lexicon.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc1/lexikos.egg-info/PKG-INFO` & `lexikos-0.0.1rc2/lexikos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -296,29 +296,32 @@
 | Language       | Dictionary   | Phone Set | Corpus                                                                                                                     | G2P Model                                                                                                             |
 | -------------- | ------------ | --------- | -------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-US          | CMU Dict     | ARPA      | [External Link](https://github.com/microsoft/CNTK/blob/master/Examples/SequenceToSequence/CMUDict/Data/cmudict-0.7b.train) | [bookbot/byt5-small-cmudict](https://huggingface.co/bookbot/byt5-small-cmudict)                                       |
 | en-US          | CMU Dict IPA | IPA       | [External Link](https://github.com/menelik3/cmudict-ipa/blob/master/cmudict-0.7b-ipa.txt)                                  |                                                                                                                       |
 | en-US          | CharsiuG2P   | IPA       | [External Link](https://github.com/lingjzhu/CharsiuG2P/blob/main/dicts/eng-us.tsv)                                         | [charsiu/g2p_multilingual_byT5_small_100](https://huggingface.co/charsiu/g2p_multilingual_byT5_small_100)             |
 | en-US (Broad)  | Wikipron     | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_us_broad.tsv)                     | [bookbot/byt5-small-wikipron-eng-latn-us-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-us-broad) |
 | en-US (Narrow) | Wikipron     | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_us_narrow.tsv)                    |
+| en-US          | LibriSpeech  | IPA       | [Link](./lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv)                                          |                                                                                                                       |
 
 ### English `(en-UK)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                                                                  | G2P Model                                                                                                             |
 | -------------- | ---------- | --------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-UK          | CharsiuG2P | IPA       | [External Link](https://github.com/lingjzhu/CharsiuG2P/blob/main/dicts/eng-uk.tsv)                      | [charsiu/g2p_multilingual_byT5_small_100](https://huggingface.co/charsiu/g2p_multilingual_byT5_small_100)             |
 | en-UK (Broad)  | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-uk-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-uk-broad) |
 | en-UK (Narrow) | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-AU)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
-| en-AU (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
-| en-AU (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
+| Language       | Dictionary  | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ----------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-AU (Broad)  | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
+| en-AU (Narrow) | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
+| en-AU          | AusTalk (§) | IPA       | [Link](./lexikos/dict/synthetic/austalk_en_au.tsv)     |                                                                                                                       |
+| en-AU          | SC-CW (§)   | IPA       | [Link](./lexikos/dict/synthetic/sc_cw_en_au.tsv)       |                                                                                                                       |
 
 ### English `(en-CA)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
 | -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
 | en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  |           |
 | en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |           |
@@ -433,18 +436,18 @@
 ### Wikipron
 
 | Language Family        | Code                              | Region                                                | Corpus | G2P Model |
 | ---------------------- | --------------------------------- | ----------------------------------------------------- | :----: | :-------: |
 | African English        | en-ZA                             | South Africa                                          |        |           |
 | Australian English     | en-AU                             | Australia                                             |   ✅    |     ✅     |
 | East Asian English     | en-CN, en-HK, en-JP, en-KR, en-TW | China, Hong Kong, Japan, South Korea, Taiwan          |        |           |
-| European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |        |           |
+| European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |   🚧    |     🚧     |
 | Mexican English        | en-MX                             | Mexico                                                |        |           |
 | New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |           |
-| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |           |
+| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |     🚧     |
 | Middle Eastern English | en-EG, en-IL                      | Egypt, Israel                                         |        |           |
 | Southeast Asian        | en-TH, en-ID, en-MY, en-PH, en-SG | Thailand, Indonesia, Malaysia, Philippines, Singapore |        |           |
 | South Asian English    | en-IN                             | India                                                 |   ✅    |           |
   
 ## Resources
 
 - [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P)
```

### Comparing `lexikos-0.0.1rc1/lexikos.egg-info/SOURCES.txt` & `lexikos-0.0.1rc2/lexikos.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 lexikos/lexicon.py
 lexikos.egg-info/PKG-INFO
 lexikos.egg-info/SOURCES.txt
 lexikos.egg-info/dependency_links.txt
 lexikos.egg-info/top_level.txt
 lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
 lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
+lexikos/dict/synthetic/austalk_en_au.tsv
+lexikos/dict/synthetic/sc_cw_en_au.tsv
 lexikos/dict/wikipron/eng_latn.tsv
 lexikos/dict/wikipron/eng_latn_au_broad.tsv
 lexikos/dict/wikipron/eng_latn_au_narrow.tsv
 lexikos/dict/wikipron/eng_latn_ca_broad.tsv
 lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
 lexikos/dict/wikipron/eng_latn_in_broad.tsv
 lexikos/dict/wikipron/eng_latn_in_narrow.tsv
```

### Comparing `lexikos-0.0.1rc1/pyproject.toml` & `lexikos-0.0.1rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexikos"
-version = "0.0.1rc1"
+version = "0.0.1rc2"
 description = "A collection of pronunciation dictionaries and neural grapheme-to-phoneme models."
 readme = "README.md"
 authors = [{ name="w11wo", email="wilson@bookbotkids.com" }, { name="anantoj", email="gg.ananto@gmail.com" }, { name="DavidSamuell", email="davidsamuel.7878@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `lexikos-0.0.1rc1/setup.py` & `lexikos-0.0.1rc2/setup.py`

 * *Files identical despite different names*

