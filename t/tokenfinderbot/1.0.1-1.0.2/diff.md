# Comparing `tmp/tokenfinderbot-1.0.1.tar.gz` & `tmp/tokenfinderbot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenfinderbot-1.0.1.tar", max compression
+gzip compressed data, was "tokenfinderbot-1.0.2.tar", max compression
```

## Comparing `tokenfinderbot-1.0.1.tar` & `tokenfinderbot-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1086 2023-05-22 06:39:03.838459 tokenfinderbot-1.0.1/LICENSE
--rw-r--r--   0        0        0      639 2023-05-22 13:53:32.879896 tokenfinderbot-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3679 2023-05-22 13:52:56.263518 tokenfinderbot-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-19 10:34:01.217406 tokenfinderbot-1.0.1/tokenfinderbot/__init__.py
--rw-r--r--   0        0        0     2900 2023-05-20 14:47:37.955310 tokenfinderbot-1.0.1/tokenfinderbot/db.py
--rw-r--r--   0        0        0     5042 2023-05-22 13:26:44.928589 tokenfinderbot-1.0.1/tokenfinderbot/tokenfinderbot.py
--rw-r--r--   0        0        0     2945 2023-05-20 11:13:04.510685 tokenfinderbot-1.0.1/tokenfinderbot/utils.py
--rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 tokenfinderbot-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-22 14:02:18.873618 tokenfinderbot-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3593 2023-05-22 14:02:18.873618 tokenfinderbot-1.0.2/README.md
+-rw-r--r--   0        0        0      618 2023-05-22 14:02:18.873618 tokenfinderbot-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 14:02:18.873618 tokenfinderbot-1.0.2/tokenfinderbot/__init__.py
+-rw-r--r--   0        0        0     3784 2023-05-22 14:02:18.873618 tokenfinderbot-1.0.2/tokenfinderbot/db.py
+-rw-r--r--   0        0        0     4864 2023-05-22 14:02:18.873618 tokenfinderbot-1.0.2/tokenfinderbot/tokenfinderbot.py
+-rw-r--r--   0        0        0     2861 2023-05-22 14:02:18.873618 tokenfinderbot-1.0.2/tokenfinderbot/utils.py
+-rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 tokenfinderbot-1.0.2/PKG-INFO
```

### Comparing `tokenfinderbot-1.0.1/pyproject.toml` & `tokenfinderbot-1.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-[tool.poetry]
-name = "tokenfinderbot"
-version = "1.0.1"
-description = "A simple bot for scanning new ERC-20 token pools created and filtering them based on the time created, liquidity and market cap"
-authors = ["Farzad Z <farzadex.eth@gmail.com>"]
-readme = "README.md"
-repository = "https://github.com/farzadex-eth/tokenfinderbot"
-homepage = "https://github.com/farzadex-eth/tokenfinderbot"
-
-[tool.poetry.dependencies]
-python = "^3.10"
-tinydb = "^4.7.1"
-requests = "^2.30.0"
-pytest = "^7.3.1"
-dotmap = "^1.3.30"
-schedule = "^1.2.0"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "tokenfinderbot"
+version = "1.0.2"
+description = "A simple bot for scanning new ERC-20 token pools created and filtering them based on the time created, liquidity and market cap"
+authors = ["Farzad Z <farzadex.eth@gmail.com>"]
+readme = "README.md"
+repository = "https://github.com/farzadex-eth/tokenfinderbot"
+homepage = "https://github.com/farzadex-eth/tokenfinderbot"
+
+[tool.poetry.dependencies]
+python = "^3.10"
+tinydb = "^4.7.1"
+requests = "^2.30.0"
+pytest = "^7.3.1"
+dotmap = "^1.3.30"
+schedule = "^1.2.0"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `tokenfinderbot-1.0.1/tokenfinderbot/db.py` & `tokenfinderbot-1.0.2/tokenfinderbot/db.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,111 @@
-from tinydb import TinyDB, Query
-from datetime import datetime, timedelta, timezone
-
-
-class PoolDB:
-    """A JSON database using tinydb
-    """
-
-    def __init__(self, name: str = "db") -> None:
-        self.db = TinyDB(f"{name}.json")
-        self.pools_table = self.db.table("pools")
-
-    def pool_exists(self, pool: dict) -> bool:
-        """Check if a pool with a specific address exists in the db
-
-        Args:
-            pool (dict): pool
-
-        Returns:
-            bool: True if it already exist
-        """
-        Pool = Query()
-        return len(self.pools_table.search(Pool.pairAddress == pool['pairAddress'])) > 0
-
-    def insert_pool(self, pool: dict) -> None:
-        """Insert pool data into db
-
-        Args:
-            pool (dict): pool
-
-        Raises:
-            Exception: Pool already exists
-        """
-        if self.pool_exists(pool):
-            raise ValueError('Pool already exists')
-        self.pools_table.insert(pool)
-
-    def delete_table(self) -> None:
-        """Delete table
-        """
-        self.db.drop_table("pools")
-
-    def get_pool(self, address: str) -> dict:
-        """Retrieve a pool
-
-        Args:
-            address (str): pool pair address
-
-        Returns:
-            dict: pool data
-        """
-        Pool = Query()
-        return self.pools_table.search(Pool.pairAddress == address)[0]
-
-    def get_pool_str(self, address: str) -> str:
-        """Returns a string of summarized pool info
-
-        Args:
-            address (str): pool pair address
-
-        Returns:
-            str: pool info
-        """
-        class bcolors:
-            HEADER = '\033[95m'
-            OKBLUE = '\033[94m'
-            OKCYAN = '\033[96m'
-            OKGREEN = '\033[92m'
-            WARNING = '\033[93m'
-            FAIL = '\033[91m'
-            ENDC = '\033[0m'
-            BOLD = '\033[1m'
-            UNDERLINE = '\033[4m'
-
-        pool = self.get_pool(address)
-        info_str = f"""\n--------------------------------------------------------------\n{bcolors.HEADER}{pool['baseToken']['symbol']} / {pool['quoteToken']['symbol']}:
-  {bcolors.OKBLUE}Pair Address: {bcolors.OKCYAN}{address}
-  {bcolors.OKBLUE}URL: {bcolors.OKCYAN}{pool['url']}
-  {bcolors.OKBLUE}Price: 
-    {bcolors.ENDC}{pool['priceNative']} {pool['quoteToken']['symbol']}
-    {pool['priceUsd']} USD
-  {bcolors.OKBLUE}Liquidity: {bcolors.ENDC}{pool['liquidity']['usd']}
-  {bcolors.OKBLUE}Market Cap: {bcolors.ENDC}{pool['fdv']}
-  {bcolors.OKBLUE}Created at: {bcolors.ENDC}{datetime.utcfromtimestamp(int(pool['pairCreatedAt']/1000)).strftime('%Y-%m-%d %H:%M:%S')} UTC [{(datetime.now(tz=timezone.utc) - timedelta(seconds=pool['pairCreatedAt']/1000)).strftime('%H hour(s), %M minute(s) ago')}]
---------------------------------------------------------------
-        """
-        return info_str
+from tinydb import TinyDB, Query
+from datetime import datetime, timedelta, timezone
+
+
+class PoolDB:
+    """A JSON database using tinydb
+    """
+
+    def __init__(self, name: str = "db") -> None:
+        self.db = TinyDB(f"{name}.json")
+        self.pools_table = self.db.table("pools")
+
+    def pool_exists(self, pool: dict) -> bool:
+        """Check if a pool with a specific address exists in the db
+
+        Args:
+            pool (dict): pool
+
+        Returns:
+            bool: True if it already exist
+        """
+        Pool = Query()
+        return len(self.pools_table.search(Pool.pairAddress == pool['pairAddress'])) > 0
+
+    def insert_pool(self, pool: dict) -> None:
+        """Insert pool data into db
+
+        Args:
+            pool (dict): pool
+
+        Raises:
+            Exception: Pool already exists
+        """
+        if self.pool_exists(pool):
+            raise ValueError('Pool already exists')
+        self.pools_table.insert(pool)
+
+    def delete_table(self) -> None:
+        """Delete table
+        """
+        self.db.drop_table("pools")
+
+    def get_pool(self, address: str) -> dict:
+        """Retrieve a pool
+
+        Args:
+            address (str): pool pair address
+
+        Returns:
+            dict: pool data
+        """
+        Pool = Query()
+        return self.pools_table.search(Pool.pairAddress == address)[0]
+
+    def get_pool_str(self, address: str) -> str:
+        """Returns a string of summarized pool info
+
+        Args:
+            address (str): pool pair address
+
+        Returns:
+            str: pool info
+        """
+        class bcolors:
+            HEADER = '\033[95m'
+            OKBLUE = '\033[94m'
+            OKCYAN = '\033[96m'
+            OKGREEN = '\033[92m'
+            WARNING = '\033[93m'
+            FAIL = '\033[91m'
+            ENDC = '\033[0m'
+            BOLD = '\033[1m'
+            UNDERLINE = '\033[4m'
+
+        pool = self.get_pool(address)
+        info_str = f"""\n--------------------------------------------------------------\n{bcolors.HEADER}{pool['baseToken']['symbol']} / {pool['quoteToken']['symbol']}:
+  {bcolors.OKBLUE}Pair Address: {bcolors.OKCYAN}{address}
+  {bcolors.OKBLUE}URL: {bcolors.OKCYAN}{pool['url']}
+  {bcolors.OKBLUE}Price: 
+    {bcolors.ENDC}{pool['priceNative']} {pool['quoteToken']['symbol']}
+    {pool['priceUsd']} USD
+  {bcolors.OKBLUE}Liquidity: {bcolors.ENDC}{pool['liquidity']['usd']}
+  {bcolors.OKBLUE}Market Cap: {bcolors.ENDC}{pool['fdv']}
+  {bcolors.OKBLUE}Created at: {bcolors.ENDC}{datetime.utcfromtimestamp(int(pool['pairCreatedAt']/1000)).strftime('%Y-%m-%d %H:%M:%S')} UTC [{(datetime.now(tz=timezone.utc) - timedelta(seconds=pool['pairCreatedAt']/1000)).strftime('%H hour(s), %M minute(s) ago')}]
+--------------------------------------------------------------
+        """
+        return info_str
+    
+    def get_pool_clean_str(self, address: str) -> str:
+        """Returns a string of summarized pool info without text colors
+
+        Args:
+            address (str): pool pair address
+
+        Returns:
+            str: pool info
+        """
+
+        pool = self.get_pool(address)
+        info_str = f"""\n--------------------------------------------------------------\n{pool['baseToken']['symbol']} / {pool['quoteToken']['symbol']}:
+Pair Address: {address}
+URL: {pool['url']}
+Price: 
+    {pool['priceNative']} {pool['quoteToken']['symbol']}
+    {pool['priceUsd']} USD
+Liquidity: {pool['liquidity']['usd']}
+Market Cap: {pool['fdv']}
+Created at: {datetime.utcfromtimestamp(int(pool['pairCreatedAt']/1000)).strftime('%Y-%m-%d %H:%M:%S')} UTC [{(datetime.now(tz=timezone.utc) - timedelta(seconds=pool['pairCreatedAt']/1000)).strftime('%H hour(s), %M minute(s) ago')}]
+--------------------------------------------------------------
+        """
+        return info_str
```

### Comparing `tokenfinderbot-1.0.1/tokenfinderbot/utils.py` & `tokenfinderbot-1.0.2/tokenfinderbot/utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-import requests
-from datetime import datetime, timedelta
-
-
-def get_new_pools() -> list:
-    """Get new pools from geckoterminal API
-
-    Raises:
-        Exception: Connection Error
-
-    Returns:
-        list: new pools recently created
-    """
-    try:
-        url = "https://api.geckoterminal.com/api/v2/networks/eth/new_pools"
-        response = requests.get(url)
-        data = response.json()
-        return data['data']
-    except Exception as e:
-        raise ConnectionError(f"geckoterminal API Error: {e}")
-
-
-def filter_pools_by_time(pools: list, hours: int = 1, minutes: int = 0) -> list:
-    """Filter pools by the time they have been created less than x hours, y minutes ago
-
-    Args:
-        pools (list): pools list from geckoterminal API
-        hours (int, optional): how many hours ago. Defaults to 1.
-        minutes (int, optional): how many minutes ago. Defaults to 0.
-
-    Returns:
-        list: filtered pools
-    """
-    address_list = []
-    time_diff = timedelta(hours=hours, minutes=minutes)
-    for pool in pools:
-        pool_created_at = datetime.strptime(pool['attributes']['pool_created_at'], '%Y-%m-%dT%H:%M:%SZ')
-        if datetime.now() - pool_created_at < time_diff:
-            address_list.append(pool['attributes']['address'])
-    return address_list
-
-def get_pools_details(address_list: list) -> list:
-    """Get pools info from dexscreener api
-
-    Args:
-        address_list (list): list of pool addresses
-
-    Raises:
-        Exception: Connection Error
-
-    Returns:
-        list: detailed info for each pool
-    """
-    if len(address_list) == 0:
-        return []
-    try:
-        url = f"https://api.dexscreener.com/latest/dex/pairs/ethereum/{','.join(address_list)}"
-        response = requests.get(url)
-        data = response.json()
-        return data['pairs']
-    except Exception as e:
-        raise ConnectionError(f"dexscreener API Error: {e}")
-
-
-def filter_pools_by_liq_mc(pairs: list, liq_mc_ratio: float = 1.5, min_mc: float = 100000, min_liq: float = 0) -> list:
-    """Filter pools by liquidity and market cap
-
-    Args:
-        pairs (list): list of pairs from dexscreener API
-        liq_mc_ratio (float, optional): minimum amount of accepted liquidity/market cap ratio. Defaults to 1.5.
-        min_mc (int, optional): minimum accepted market cap. Defaults to 100000.
-        min_liq (int, optional): minimum accepted liquidity. Defaults to 0.
-
-    Returns:
-        list: filtered list of accepted pools
-    """
-    filtered_pools = []
-    for pair in pairs:
-        if 'liquidity' not in pair or 'usd' not in pair['liquidity']:
-            continue
-        liquidity_usd = pair['liquidity']['usd']
-        if 'fdv' in pair and pair['fdv'] >= liq_mc_ratio * liquidity_usd and pair['fdv'] >= min_mc and liquidity_usd >= min_liq:
-            filtered_pools.append(pair)
-    
+import requests
+from datetime import datetime, timedelta
+
+
+def get_new_pools() -> list:
+    """Get new pools from geckoterminal API
+
+    Raises:
+        Exception: Connection Error
+
+    Returns:
+        list: new pools recently created
+    """
+    try:
+        url = "https://api.geckoterminal.com/api/v2/networks/eth/new_pools"
+        response = requests.get(url)
+        data = response.json()
+        return data['data']
+    except Exception as e:
+        raise ConnectionError(f"geckoterminal API Error: {e}")
+
+
+def filter_pools_by_time(pools: list, hours: int = 1, minutes: int = 0) -> list:
+    """Filter pools by the time they have been created less than x hours, y minutes ago
+
+    Args:
+        pools (list): pools list from geckoterminal API
+        hours (int, optional): how many hours ago. Defaults to 1.
+        minutes (int, optional): how many minutes ago. Defaults to 0.
+
+    Returns:
+        list: filtered pools
+    """
+    address_list = []
+    time_diff = timedelta(hours=hours, minutes=minutes)
+    for pool in pools:
+        pool_created_at = datetime.strptime(pool['attributes']['pool_created_at'], '%Y-%m-%dT%H:%M:%SZ')
+        if datetime.now() - pool_created_at < time_diff:
+            address_list.append(pool['attributes']['address'])
+    return address_list
+
+def get_pools_details(address_list: list) -> list:
+    """Get pools info from dexscreener api
+
+    Args:
+        address_list (list): list of pool addresses
+
+    Raises:
+        Exception: Connection Error
+
+    Returns:
+        list: detailed info for each pool
+    """
+    if len(address_list) == 0:
+        return []
+    try:
+        url = f"https://api.dexscreener.com/latest/dex/pairs/ethereum/{','.join(address_list)}"
+        response = requests.get(url)
+        data = response.json()
+        return data['pairs']
+    except Exception as e:
+        raise ConnectionError(f"dexscreener API Error: {e}")
+
+
+def filter_pools_by_liq_mc(pairs: list, liq_mc_ratio: float = 1.5, min_mc: float = 100000, min_liq: float = 0) -> list:
+    """Filter pools by liquidity and market cap
+
+    Args:
+        pairs (list): list of pairs from dexscreener API
+        liq_mc_ratio (float, optional): minimum amount of accepted liquidity/market cap ratio. Defaults to 1.5.
+        min_mc (int, optional): minimum accepted market cap. Defaults to 100000.
+        min_liq (int, optional): minimum accepted liquidity. Defaults to 0.
+
+    Returns:
+        list: filtered list of accepted pools
+    """
+    filtered_pools = []
+    for pair in pairs:
+        if 'liquidity' not in pair or 'usd' not in pair['liquidity']:
+            continue
+        liquidity_usd = pair['liquidity']['usd']
+        if 'fdv' in pair and pair['fdv'] >= liq_mc_ratio * liquidity_usd and pair['fdv'] >= min_mc and liquidity_usd >= min_liq:
+            filtered_pools.append(pair)
+    
     return filtered_pools
```

### Comparing `tokenfinderbot-1.0.1/PKG-INFO` & `tokenfinderbot-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenfinderbot
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple bot for scanning new ERC-20 token pools created and filtering them based on the time created, liquidity and market cap
 Home-page: https://github.com/farzadex-eth/tokenfinderbot
 Author: Farzad Z
 Author-email: farzadex.eth@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

