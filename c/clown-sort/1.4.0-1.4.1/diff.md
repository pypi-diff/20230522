# Comparing `tmp/clown_sort-1.4.0.tar.gz` & `tmp/clown_sort-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.4.0.tar", max compression
+gzip compressed data, was "clown_sort-1.4.1.tar", max compression
```

## Comparing `clown_sort-1.4.0.tar` & `clown_sort-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2223 2023-05-09 18:21:24.058982 clown_sort-1.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.4.0/LICENSE
--rw-r--r--   0        0        0     7617 2023-04-16 21:33:01.097803 clown_sort-1.4.0/README.md
--rw-r--r--   0        0        0     3316 2023-04-24 00:56:40.931125 clown_sort-1.4.0/clown_sort/__init__.py
--rw-r--r--   0        0        0     7429 2023-05-09 18:20:37.529588 clown_sort-1.4.0/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.4.0/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4745 2023-05-09 18:20:37.530359 clown_sort-1.4.0/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     1330 2023-04-24 00:42:15.932759 clown_sort-1.4.0/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    10796 2023-05-09 18:20:37.530660 clown_sort-1.4.0/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3139 2023-05-09 18:20:37.531050 clown_sort-1.4.0/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     8483 2023-05-09 18:20:37.531375 clown_sort-1.4.0/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.4.0/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.4.0/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.4.0/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.4.0/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.4.0/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.4.0/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      520 2023-05-09 18:20:37.532239 clown_sort-1.4.0/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1558 2023-05-09 18:21:17.194294 clown_sort-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     8981 1970-01-01 00:00:00.000000 clown_sort-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2330 2023-05-22 02:18:01.650330 clown_sort-1.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.4.1/LICENSE
+-rw-r--r--   0        0        0     7796 2023-05-09 18:33:06.154216 clown_sort-1.4.1/README.md
+-rw-r--r--   0        0        0     3316 2023-04-24 00:56:40.931125 clown_sort-1.4.1/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7622 2023-05-22 01:52:09.100468 clown_sort-1.4.1/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.4.1/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4745 2023-05-09 18:20:37.530359 clown_sort-1.4.1/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     1330 2023-04-24 00:42:15.932759 clown_sort-1.4.1/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    10796 2023-05-09 18:20:37.530660 clown_sort-1.4.1/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3139 2023-05-09 18:20:37.531050 clown_sort-1.4.1/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     9596 2023-05-22 02:07:43.101538 clown_sort-1.4.1/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.4.1/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.4.1/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.4.1/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.4.1/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.4.1/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.4.1/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      520 2023-05-09 18:20:37.532239 clown_sort-1.4.1/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1558 2023-05-22 02:18:01.659658 clown_sort-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9160 1970-01-01 00:00:00.000000 clown_sort-1.4.1/PKG-INFO
```

### Comparing `clown_sort-1.4.0/CHANGELOG.md` & `clown_sort-1.4.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # NEXT RELEASE
 
+### 1.4.1
+* Make --manual-fallback and --only-if-match mutually exclusive
+* New default crypto sort rules
+
 ## 1.4.0
 * Add `--manual-fallback` option
 * Handle truncated image file binary errors
 * Display the string that matched the rule when copying
 * Better handling of re-scanning already sorted files
 * New crypto sorting rules
```

### Comparing `clown_sort-1.4.0/LICENSE` & `clown_sort-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/README.md` & `clown_sort-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+![Python Version](https://img.shields.io/pypi/pyversions/clown_sort)
+![Release](https://img.shields.io/pypi/v/clown_sort)
+![Downloads](https://img.shields.io/pypi/dm/clown_sort)
+
 # CLOWN SORT
 Sometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can't find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.
 
 Clown Sort[^1] solves this.
 
 
 ## What It Do
```

### Comparing `clown_sort-1.4.0/clown_sort/__init__.py` & `clown_sort-1.4.1/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/config.py` & `clown_sort-1.4.1/clown_sort/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,18 @@
 
         if args.manual_sort or args.manual_fallback:
             _check_for_pysimplegui()
 
             if args.manual_sort:
                 Config.manual_sort = True
             if args.manual_fallback:
+                if Config.only_if_match:
+                    Console().print('Only one of --manual-fallback and --only-if-match can be specified.', style='red')
+                    sys.exit()
+
                 Config.manual_fallback = True
 
     @classmethod
     def set_directories(
             cls,
             screenshots_dir: StringOrPath,
             destination_dir: StringOrPath,
```

### Comparing `clown_sort-1.4.0/clown_sort/filename_extractor.py` & `clown_sort-1.4.1/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/files/image_file.py` & `clown_sort-1.4.1/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/files/pdf_file.py` & `clown_sort-1.4.1/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/files/sortable_file.py` & `clown_sort-1.4.1/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/sort_selector.py` & `clown_sort-1.4.1/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.4.1/clown_sort/sorting_rules/crypto.csv`

 * *Files 7% similar despite different names*

```diff
@@ -5,65 +5,67 @@
 Aave,aave
 AAX,\baax
 Algorand,\bAlgorand|\b[$#]ALGO\b
 Arbitrum,Arbitrum|[$#]ARB\b
 Amber Group,Amber[-_\s]*Group|\btiantian\b|\bkullander\b|\btony[-_\s]*he\b|\bbo[-_\s]*shen\b
 Aptos,\bAptos\b
 Art,occult
-Avalanche,\bAvax|AVAX\b|avalanche
-Banks,SEBA[^a-z]|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group|\$FRC|Commercium[-_\s]*Financial|\bmetabank|\bHBAN\b|Huntington[-_\s]*Bancshares|United[-_\s]*Texas|\bUTB\b
+Avalanche,\bAvax|AVAX\b|avalanche|\bava[-_\s]*labs
+Banks,SEBA[^a-z]|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group|\$FRC|Commercium[-_\s]*Financial|\bmetabank|\bHBAN\b|Huntington[-_\s]*Bancshares|United[-_\s]*Texas|\bUTB\b|Craig[-_\s]*Sellars
 Bankless,Bankless|David[-_\s]*Hoffman
 Biconomy,\bBiconomy|Omchain
 Binary Options,binary[-_\s]*options
-Binance,binance|biconomy|\bbnb\b|\bbsc\b|\bcz\b|\bbifinity\b|binaryx|\bbillance|changpeng|joselito|paysafe|\bSwipe[-_\s]*(IO|Wallet)|\bkeyway|\bkey[-_\s]*vision|\bTrustWallet\b|BUSD|\boztures|Kaiser[-_\s]*Ng|InvestByBit
+Binance,binance|\bbiconomy|\bbnb\b|\bbsc\b|\bcz\b|\bbifinity\b|binaryx|\bbillance|changpeng|\bjoselito\b|\bpaysafe|\bSwipe[-_\s]*(IO|Wallet)|\bkeyway|\bkey[-_\s]*vision|\bTrustWallet\b|BUSD\b|\boztures|Kaiser[-_\s]*Ng|InvestByBit|Swyftx
 Bitdeer,Bitdeer
 BitGet,Bitget
 Bithumb,\bbithumb
 Bitmain,Bitmain
 Bitstamp,Bitstamp
-Bittrex,Bittrex|Ritchie[-_\s]*Lai|Kiran[-_\s]*Raj|John[-_\s]*Roth
+Bittrex,Bittrex|Ritchie[-_\s]*Lai|Kiran[-_\s]*Raj|John[-_\s]*Roth\b|\bAquila\b
 Bitzlato,Bitzlato
+Blockchain.com,\bblockchain\.com\b|@blockchain\b|@AskBlockchain\b
 Blockchain8,Blockchain8|tom[-_\s]*emmer|ritchie[-_\s]*torres|repritchie|Warren[-_\s]*Davidson|Byron[-_\s]*Donalds|Ted[-_\s]*Budd|Josh[-_\s]*Gotheimer|Jake[-_\s]*Auchincloss|Darren[-_\s]*Soto|ro[-_\s]*khanna|KMSmithDC|Kristin[-_\s]*Smith\b|Warren[-_\s]*Davidson
 Blockchain Capital,Blockchain[-_\s]*Capital|\bbrock\b|brockpierce
 BlockFi,BlockFi|Zac[-_\s]*Prince|Brian[-_\s]*Oliver
 Blockstream,Blockstream
 Bored Ape Yacht Club,BAYC|Bored[-_\s]*Ape|yuga[-_\s]*labs
-Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell|stackersatoshi|Max[-_\s]*Keiser|Cowboy[-_\s]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s]*Paul\b|raoul(gmi|[-_\s]*pal)
+Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell|stackersatoshi|Max[-_\s]*Keiser|Cowboy[-_\s]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s]*Paul\b|raoul(gmi|[-_\s]*pal)|mccormack
 Broettes,Nicole[-_\s]*Behnam|natbrunell
 Bybit,\bBybit\b|Ben[-_\s]*Zhou|InvestByBit|TravelByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
 Cathie Wood,Cathie\s*Wood|\bARK(F|G|K|\s*Innovation|\s*Invest)|\bIZRL
-Celsius,celsius|mashinsky|levity[-_\s]*and[-_\s]*love|celsian
+Celsius,celsius|mashinsky|levity[-_\s]*and[-_\s]*love|\bcelsian|Artur[-_\s]*Abreu|ronpaulbot
 Circle,[@#]circle|usdc|circle[-_\s]*internet|disparte|\ballaire|jerallaire
 CMCC Global,CMCC[-_\s]*Global
 Coinbase,Coinbase|\$COIN|brian[-_\s]*armstrong|grewal\b|Asiff[-_\s]*Hirji|\bbalaji|Fred[-_\s]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s]*Lamb|Roger[-_\s]*Ver|coinflex|Doug[-_\s]*Polk|OPNX|flexusd|Leslie[-_\s]*Lamb|dougpolkvids
-CoinLoan,coinloan|Faliushin
+CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
 Cross River Bank,CRB|Cross[-_\s]*River|Prestige[-_\s]*Capital|bae[-_\s]*communications|Zenfi|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv
+Cumberland,cumberland
 Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s
 CUBI,\bCUBI\b|Customers[-_\s]*Ban(k|corp)
 Custodia,custodia\b|caitlin[-_\s]*long
 dalle,craiyon|midjourney|\bdall[-_\s]*e\b
-DCG,DCG|digital\s*currency\s*group|sh?ill?bert|Grayscale|GBTC
+DCG,DCG|digital\s*currency\s*group|sh?ill?bert|Grayscale|GBTC|\bkraines\b
 DeFi,\bdefi\b|decentralized[-_\s]*finance
 Dragonfly Capital,Dragonfly[-_\s]*Capital
 DWF,DWF|Andrey[-_\s]*Grachev|\bgrachev\b
 Effective Altruism,\bE\.?A\.?\b|effective[-_\s]*altruism
 El Salvador,El[-_\s]*Salvador|Bukele|Max[-_\s]*Keiser
 Elon Musk,\bTesla\b|\bTSLA\b|\bElon\b|\bElmo\b
 EOS,\bEOS\b|\bBlumer\b|\bLarimer\b|@B1\b|Block[-_\.\s]One
 Euler Finance,\beuler\b
 FalconX,falconx
 Flip Filipkowski,filipkowski
 Finblox,finblox
 Fireblocks,fireblocks
 Frax,\bFrax\b|\bFRX|[\b#$]FXS
 Friedlander Group,Friedlander|Agro[-_\s]*Bank|all\s*year\*m|\bbrock\b|brockpierce|litvishhocker
-FTX,FTX|FTT|SBF|Trabucco|Bankman|Ellison|Nishad|Alameda|Moonstone|friedberg|autism\s*capital
+FTX,FTX|\bFTT\b|\bSBF|Trabucco|\bBankman\b|\bEllison|\bNishad|\bAlameda|Moonstone|friedberg|autism\s*capital|\bryne\b|clifton[-_\s]*bay|\bZUBR\b
 Galaxy Digital,novogratz|Alex[-_\s]*Thorn
 Gelato Network,Gelato[-_\s]*Network|\bSorbet[-_\s]*Finance|@gitpusha|hilmar[-_\s]*x|\bmistx\b|@_alchemistcoin|@ChaosLabs_NFT|Arrakis[-_\s]*Finance|Dave[-_\s]*Leibowitz|Hilmar[-_\s]*Orth|joehquak
 Gemini,Gemini|winklev|@cameron
 Genesis,Genesis|Michael\s?Moro
 Goldfinch,goldfinch
 Hamas,\bHamas\b|Al[-_\s]*Qassam
 Hex,\bHex\b|[#$]Hex|Pulsechain|Richard\s*Heart|Hexican
@@ -80,56 +82,57 @@
 Lexpunk Army,lexpunk|gabriel[-_\s]*shapiro|_gabrielShapir0|\blex_node\b
 Lifeboat Foundation,Lifeboat[-_\s]*Foundation
 North Korea,lazarus|North\s*Korea|pyongyang|\bDPRK|puuurtbubv|@fast4release
 Paul LeRoux,leroux
 Polygon Labs,polygon[-_\s]*labs|ryan[-_\s]*watt\b|@Fwiz|Rebecca[-_\s]*Rettig|[#$]DOT\b
 MakerDAO,makerdao|[$#\s]DAI[^\w]
 Marathon,\$MARA|marathon
-Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s]*Cheng
+Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s]*Cheng|\bBeauregard\b|\bGoCoin\b|Advent[-_\s]*International|Keystone[-_\s]*Capital[-_\s]*Partners
 Mario Nawfal,mario[-_\s]*nawfal
 Messari,Ryan\s*Selkis|twobitidiot|messari|@robustus|Dan[-_\s]*McArdle
 Memes,\smeme
-Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s]*Stewart
-Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s]*(Bank|Commercial)
+Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s]*Stewart|\bHayner\b
+Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s]*(Bank|Commercial)|Mission[-_\s]*Gateway|Aryeh[-_\s]*Realty
 Founders Bank,Michael[-_\s]*Bianchi|Founders[-_\s]*Bank
-Miles Guo,\bguo\b|hcoin|himalaya[-_\s]*exchange|bannon|fjb|miles[-_\s]*kwok|brother[-_\s]*seven|kin[-_\s]*ming[-_\s]*je|william[-_\s]*je\b|\bHaoyun\b
+Miles Guo,\bguo\b|\bhcoin|himalaya[-_\s]*exchange|\bbannon\b|\bfjb|\bkwok\b|brother[-_\s]*seven|kin[-_\s]*ming[-_\s]*je|william[-_\s]*je\b|\bHaoyun\b|\bLi[-_\s]*You\b
 Miners,bitcoin[-_\s]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s]*Scientific|Iris[-_\s]*Energy|Blockstream
 Moonpay,moonpay
 MSTR,Saylor|MSTR
+MtGox,Mt[-_\s.]*Gox|\bwilly[-_\s]*bot
 Near Protocol,NEAR[-_\s]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s]*Rettig
 Nexo,\bNexo\b|Antoni[-_\s]*Trenchev|Georgi[-_\s]*Shulev|Lydia[-_\s]*Shuleva
 NFTs,crypto[-_\s]*punk|pudgy[-_\s]*penguin
 OKX,oke?[cx]|star[-_\s]*xu
-Olympus DAO,\bOlympus\b|\bOHM\b
+Olympus DAO,\bOlympus\b|OlympusDAO|\bOHM\b
 OpenPayd,openpayd|CFD\s?Team
 OpenSea,OpenSea
 PAG,\bpag\b|Weijian[-_\s]*Shan
 Paradigm,Fred[-_\s]*Ehrsam|paradigm\b
 Paxful,paxful|Ray[-_\s]*(Youssef|Savant)|Artur[-_\s]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
 Payrnet,payrnet|railsr|railsbank
 Pi,\$PI[^\w]|Pi[-_\s]*Network
 Prime Trust,Prime[-\s_]?Trust
 PVBC,PVBC|BankProv
-Quadriga,Quadriga|Gerald[-_\s]*Cotten
+Quadriga,Quadriga|Gerald[-_\s]*Cotten|0xsifu\b|michael[-_\s]*patryn|wonderland|daniele[-_\s]*sesta\b
 Revolut,revolut[^\w]
 Ripple,XRP|garlinghouse|\bripple\b
 RIOT,[$#]RIOT\b|Riot[-\s_]*(Block|Platform)|Bioptix
 Safemoon,Safemoon
 Satoshi,Satoshi|Nakamoto
 SEC,\bSEC(\b|Gov)|Gensler|Securities.{0,6}Exchange.{0,6}Commission
-Signature Bank,SBNY|Signature[-_\s]*Bank|Signet|Scott[-_\s]*Shay\b|(Joseph|Joe)[-_\s]*DePaolo
+Signature Bank,SBNY|Signature[-_\s]*Bank|Signet|Scott[-_\s]*Shay\b|(Joseph|Joe)[-_\s]*DePaolo|\bKushner\b
 Silicon Valley Bank,si?vb|Silicon[-_\s]*Valley[-_\s]*Bank
 Silk Road,Silk[-_\s]*Road|\bulbricht|\bDPR\b
 Silvergate,\$SI|Silvergate|Alan\s*Lane|Eisele|\bSEN\b|SENnetwork|Rebecca[-_\s]*Rettig
 Skrill,\bskrill
 Solana,Solana|Serum
 Symbolic Capital,Symbolic[-_\s]*Capital|Lev[-_\s]Livnev
 TerraLuna,luna\b|do[-_\s]*kwon|stablekwon|\bterra\b|LFG|Macedo|\bLuna[-_\s]*Foundation\b
-Tether,tether|usdt|paolo|friedberg|hoegner|Noble\s?Bank|Deltec[^\']|b(e|i)tfinex[^e]|\bbrock\b|brockpierce|Capital[-_\s]*Union|Noblex|SJMBT|Global[-_\s]*Trad(ing|e)[-_\s]*Solutions|ifinex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s]*Potter|Stablehouse|Samson[-_\s]*Mow|Gabor[-_\s]*Grubacs|XBTO|Paul[-_\s]*Eisma|Philippe[-_\s]*Bekhazi
+Tether,\btether\b|usdt|paolo\b|paoloardoino|friedberg|hoegner|Noble[-_\s]*Bank|\bDeltec[^\']|b(e|i)tfinex[^e]|\bbrock([-_\s]*pierce)?\b|Clearstone[-_\s]*Global|Capital[-_\s]*Union|Noblex|SJMBT|Global[-_\s]*Trad(ing|e)[-_\s]*Solutions|(dig|i)finex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s]*Potter|Stablehouse|Samson[-_\s]*Mow|Gabor[-_\s]*Grubacs|XBTO|Paul[-_\s]*Eisma|Philippe[-_\s]*Bekhazi|\b(Master|Real)coin\b|Reeve[-_\s]*Collins|\bdevasini\b|phil(ip)?[-_\s]*potter\b|van[-_\s]*der[-_\s]*velde|Perpetual[-_\s]*Action[-_\s]*Group|\burwhatyouknow|global[-_\s]*trade[-_\s]*solutions|reginald[-_\s]*fowler|renrenbee\b|\bludovicus|Amos[-_\s]*Ltd|William[-_\s]*Quigley|Sunlot\b|\bD10e\b|\bGoCoin\b|Blade[-_\s]*payments|Five[-_\s]*Delta|\bXfire\b|\bPlaysino\b|\bEvertune|\bGamesTV|\bethfinex|coinapult|gabriel[-_\s]*sukenik|R(ondell|[ho][ho]n)[-_\s]*(Clyde)?[-_\s]*Monroe|\bTuxia\b|\bIGEL\b|\bInfomatec
 Tornado Cash,tornado\s*cash
 Transactive Systems UAB,Transactive
 Tron,\btron\b|tron(block|\s*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
 VCs,venture[-_\s]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s]*sacks|\bthiel\b|sequoia|founders[-_\s]*fund|Valar[-_\s]*Ventures|6th[-_\s]*Man[-_\s]*Ventures|Northzone|Warburg[-_\s]*Serres|Alan[-_\s]*Howard|Tiger[-_\s]*Global
 Vitalik Buterin,\bvitalik\b
```

### Comparing `clown_sort-1.4.0/clown_sort/util/argument_parser.py` & `clown_sort-1.4.1/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/util/constants.py` & `clown_sort-1.4.1/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/util/filesystem_helper.py` & `clown_sort-1.4.1/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/util/rich_helper.py` & `clown_sort-1.4.1/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/clown_sort/util/string_helper.py` & `clown_sort-1.4.1/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.0/pyproject.toml` & `clown_sort-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.4.0"
+version = "1.4.1"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.4.0/PKG-INFO` & `clown_sort-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.4.0
+Version: 1.4.1
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -26,14 +26,18 @@
 Requires-Dist: pypdf (>=3.4.1,<4.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: rich (>=13.0.1,<14.0.0)
 Requires-Dist: rich-argparse-plus (>=0.3.1.4,<0.4.0.0)
 Description-Content-Type: text/markdown
 
+![Python Version](https://img.shields.io/pypi/pyversions/clown_sort)
+![Release](https://img.shields.io/pypi/v/clown_sort)
+![Downloads](https://img.shields.io/pypi/dm/clown_sort)
+
 # CLOWN SORT
 Sometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can't find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.
 
 Clown Sort[^1] solves this.
 
 
 ## What It Do
```

