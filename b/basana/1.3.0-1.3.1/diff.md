# Comparing `tmp/basana-1.3.0.tar.gz` & `tmp/basana-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basana-1.3.0.tar", max compression
+gzip compressed data, was "basana-1.3.1.tar", max compression
```

## Comparing `basana-1.3.0.tar` & `basana-1.3.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      583 2023-02-25 02:54:08.614680 basana-1.3.0/LICENSE
--rw-r--r--   0        0        0     1263 2023-04-13 16:56:31.180127 basana-1.3.0/basana/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.759693 basana-1.3.0/basana/backtesting/__init__.py
--rw-r--r--   0        0        0     3922 2023-04-25 19:59:42.240369 basana-1.3.0/basana/backtesting/account_balances.py
--rw-r--r--   0        0        0    13416 2023-04-28 03:07:23.322333 basana-1.3.0/basana/backtesting/charts.py
--rw-r--r--   0        0        0      679 2023-04-03 17:28:32.834201 basana-1.3.0/basana/backtesting/errors.py
--rw-r--r--   0        0        0    22695 2023-04-28 03:07:23.323961 basana-1.3.0/basana/backtesting/exchange.py
--rw-r--r--   0        0        0     2547 2023-04-28 03:07:23.324848 basana-1.3.0/basana/backtesting/fees.py
--rw-r--r--   0        0        0     1683 2023-03-29 02:43:04.761285 basana-1.3.0/basana/backtesting/helpers.py
--rw-r--r--   0        0        0     6150 2023-04-28 03:07:23.325407 basana-1.3.0/basana/backtesting/liquidity.py
--rw-r--r--   0        0        0    16012 2023-04-28 03:07:23.326054 basana-1.3.0/basana/backtesting/orders.py
--rw-r--r--   0        0        0     7913 2023-04-28 03:07:23.326667 basana-1.3.0/basana/backtesting/requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.762632 basana-1.3.0/basana/core/__init__.py
--rw-r--r--   0        0        0     6035 2023-04-03 17:28:32.838372 basana-1.3.0/basana/core/bar.py
--rw-r--r--   0        0        0     1394 2023-03-29 02:43:04.763204 basana-1.3.0/basana/core/config.py
--rw-r--r--   0        0        0     9620 2023-04-28 03:07:23.327710 basana-1.3.0/basana/core/dispatcher.py
--rw-r--r--   0        0        0     1493 2023-03-29 02:43:04.763794 basana-1.3.0/basana/core/dt.py
--rw-r--r--   0        0        0      968 2023-03-29 02:43:04.764040 basana-1.3.0/basana/core/enums.py
--rw-r--r--   0        0        0     3456 2023-04-28 03:07:23.328623 basana-1.3.0/basana/core/event.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.764708 basana-1.3.0/basana/core/event_sources/__init__.py
--rw-r--r--   0        0        0     3025 2023-04-28 03:07:23.329229 basana-1.3.0/basana/core/event_sources/csv.py
--rw-r--r--   0        0        0     2277 2023-04-03 17:28:32.840140 basana-1.3.0/basana/core/event_sources/trading_signal.py
--rw-r--r--   0        0        0     2978 2023-03-29 02:43:04.765532 basana-1.3.0/basana/core/helpers.py
--rw-r--r--   0        0        0     1539 2023-03-29 02:43:04.765805 basana-1.3.0/basana/core/logs.py
--rw-r--r--   0        0        0     1459 2023-04-03 17:28:32.841069 basana-1.3.0/basana/core/pair.py
--rw-r--r--   0        0        0     2280 2023-04-13 16:56:31.182428 basana-1.3.0/basana/core/token_bucket.py
--rw-r--r--   0        0        0     6010 2023-04-28 03:07:23.329823 basana-1.3.0/basana/core/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.766920 basana-1.3.0/basana/external/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.767178 basana-1.3.0/basana/external/binance/__init__.py
--rw-r--r--   0        0        0    20702 2023-04-28 03:07:23.330411 basana-1.3.0/basana/external/binance/client.py
--rw-r--r--   0        0        0    10335 2023-04-13 16:56:31.184239 basana-1.3.0/basana/external/binance/common.py
--rw-r--r--   0        0        0      867 2023-03-29 02:43:04.768133 basana-1.3.0/basana/external/binance/config.py
--rw-r--r--   0        0        0     2111 2023-04-13 16:56:31.184643 basana-1.3.0/basana/external/binance/cross_margin.py
--rw-r--r--   0        0        0      662 2023-03-29 02:43:04.768810 basana-1.3.0/basana/external/binance/csv/__init__.py
--rw-r--r--   0        0        0     1648 2023-03-29 02:43:04.769173 basana-1.3.0/basana/external/binance/csv/bars.py
--rw-r--r--   0        0        0    10385 2023-04-16 21:31:22.354698 basana-1.3.0/basana/external/binance/exchange.py
--rw-r--r--   0        0        0     3052 2023-03-29 02:43:04.769989 basana-1.3.0/basana/external/binance/helpers.py
--rw-r--r--   0        0        0     3187 2023-04-13 16:56:31.186035 basana-1.3.0/basana/external/binance/isolated_margin.py
--rw-r--r--   0        0        0     1913 2023-04-13 16:56:31.186636 basana-1.3.0/basana/external/binance/klines.py
--rw-r--r--   0        0        0    12082 2023-04-28 03:07:23.331079 basana-1.3.0/basana/external/binance/margin.py
--rw-r--r--   0        0        0     6165 2023-04-28 03:07:23.331858 basana-1.3.0/basana/external/binance/margin_requests.py
--rw-r--r--   0        0        0     4143 2023-04-16 21:31:22.355396 basana-1.3.0/basana/external/binance/order_book.py
--rw-r--r--   0        0        0    12177 2023-04-13 16:56:31.188619 basana-1.3.0/basana/external/binance/spot.py
--rw-r--r--   0        0        0     5555 2023-04-28 03:07:23.332666 basana-1.3.0/basana/external/binance/spot_requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.772127 basana-1.3.0/basana/external/binance/tools/__init__.py
--rw-r--r--   0        0        0     4373 2023-03-29 02:43:04.772398 basana-1.3.0/basana/external/binance/tools/download_bars.py
--rw-r--r--   0        0        0     2710 2023-04-13 16:56:31.189265 basana-1.3.0/basana/external/binance/trades.py
--rw-r--r--   0        0        0     2647 2023-03-29 02:43:04.772931 basana-1.3.0/basana/external/binance/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.773220 basana-1.3.0/basana/external/bitstamp/__init__.py
--rw-r--r--   0        0        0     8684 2023-03-29 02:43:04.773512 basana-1.3.0/basana/external/bitstamp/client.py
--rw-r--r--   0        0        0      865 2023-03-29 02:43:04.773899 basana-1.3.0/basana/external/bitstamp/config.py
--rw-r--r--   0        0        0      662 2023-03-29 02:43:04.774215 basana-1.3.0/basana/external/bitstamp/csv/__init__.py
--rw-r--r--   0        0        0     2047 2023-03-29 02:43:04.774543 basana-1.3.0/basana/external/bitstamp/csv/bars.py
--rw-r--r--   0        0        0    23031 2023-04-16 21:31:22.356361 basana-1.3.0/basana/external/bitstamp/exchange.py
--rw-r--r--   0        0        0     2374 2023-03-29 02:43:04.775164 basana-1.3.0/basana/external/bitstamp/helpers.py
--rw-r--r--   0        0        0     4150 2023-04-16 21:31:22.357186 basana-1.3.0/basana/external/bitstamp/order_book.py
--rw-r--r--   0        0        0     3067 2023-04-16 21:31:22.357564 basana-1.3.0/basana/external/bitstamp/orders.py
--rw-r--r--   0        0        0     4283 2023-04-28 03:07:23.333551 basana-1.3.0/basana/external/bitstamp/requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.776276 basana-1.3.0/basana/external/bitstamp/tools/__init__.py
--rw-r--r--   0        0        0     4069 2023-03-29 02:43:04.777227 basana-1.3.0/basana/external/bitstamp/tools/download_bars.py
--rw-r--r--   0        0        0     2968 2023-04-16 21:31:22.357932 basana-1.3.0/basana/external/bitstamp/trades.py
--rw-r--r--   0        0        0     4620 2023-03-29 02:43:04.777839 basana-1.3.0/basana/external/bitstamp/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778237 basana-1.3.0/basana/external/common/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778648 basana-1.3.0/basana/external/common/csv/__init__.py
--rw-r--r--   0        0        0     1763 2023-03-29 02:43:04.779031 basana-1.3.0/basana/external/common/csv/bars.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.779403 basana-1.3.0/basana/external/yahoo/__init__.py
--rw-r--r--   0        0        0     3384 2023-03-29 02:43:04.779788 basana-1.3.0/basana/external/yahoo/bars.py
--rw-r--r--   0        0        0     1161 2023-04-28 03:12:38.894557 basana-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 basana-1.3.0/setup.py
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 basana-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-02-25 02:54:08.614680 basana-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1263 2023-04-13 16:56:31.180127 basana-1.3.1/basana/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.759693 basana-1.3.1/basana/backtesting/__init__.py
+-rw-r--r--   0        0        0     3922 2023-04-25 19:59:42.240369 basana-1.3.1/basana/backtesting/account_balances.py
+-rw-r--r--   0        0        0    13477 2023-05-22 18:02:28.536545 basana-1.3.1/basana/backtesting/charts.py
+-rw-r--r--   0        0        0      679 2023-04-03 17:28:32.834201 basana-1.3.1/basana/backtesting/errors.py
+-rw-r--r--   0        0        0    22695 2023-04-28 03:07:23.323961 basana-1.3.1/basana/backtesting/exchange.py
+-rw-r--r--   0        0        0     2547 2023-04-28 03:07:23.324848 basana-1.3.1/basana/backtesting/fees.py
+-rw-r--r--   0        0        0     1683 2023-03-29 02:43:04.761285 basana-1.3.1/basana/backtesting/helpers.py
+-rw-r--r--   0        0        0     6150 2023-04-28 03:07:23.325407 basana-1.3.1/basana/backtesting/liquidity.py
+-rw-r--r--   0        0        0    16012 2023-04-28 03:07:23.326054 basana-1.3.1/basana/backtesting/orders.py
+-rw-r--r--   0        0        0     7913 2023-04-28 03:07:23.326667 basana-1.3.1/basana/backtesting/requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.762632 basana-1.3.1/basana/core/__init__.py
+-rw-r--r--   0        0        0     6035 2023-04-03 17:28:32.838372 basana-1.3.1/basana/core/bar.py
+-rw-r--r--   0        0        0     1394 2023-03-29 02:43:04.763204 basana-1.3.1/basana/core/config.py
+-rw-r--r--   0        0        0     9620 2023-04-28 03:07:23.327710 basana-1.3.1/basana/core/dispatcher.py
+-rw-r--r--   0        0        0     1493 2023-03-29 02:43:04.763794 basana-1.3.1/basana/core/dt.py
+-rw-r--r--   0        0        0      968 2023-03-29 02:43:04.764040 basana-1.3.1/basana/core/enums.py
+-rw-r--r--   0        0        0     3456 2023-04-28 03:07:23.328623 basana-1.3.1/basana/core/event.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.764708 basana-1.3.1/basana/core/event_sources/__init__.py
+-rw-r--r--   0        0        0     3025 2023-04-28 03:07:23.329229 basana-1.3.1/basana/core/event_sources/csv.py
+-rw-r--r--   0        0        0     2277 2023-04-03 17:28:32.840140 basana-1.3.1/basana/core/event_sources/trading_signal.py
+-rw-r--r--   0        0        0     2978 2023-03-29 02:43:04.765532 basana-1.3.1/basana/core/helpers.py
+-rw-r--r--   0        0        0     1539 2023-03-29 02:43:04.765805 basana-1.3.1/basana/core/logs.py
+-rw-r--r--   0        0        0     1459 2023-04-03 17:28:32.841069 basana-1.3.1/basana/core/pair.py
+-rw-r--r--   0        0        0     2280 2023-04-13 16:56:31.182428 basana-1.3.1/basana/core/token_bucket.py
+-rw-r--r--   0        0        0     6010 2023-04-28 03:07:23.329823 basana-1.3.1/basana/core/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.766920 basana-1.3.1/basana/external/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.767178 basana-1.3.1/basana/external/binance/__init__.py
+-rw-r--r--   0        0        0    20702 2023-04-28 03:07:23.330411 basana-1.3.1/basana/external/binance/client.py
+-rw-r--r--   0        0        0    10335 2023-04-13 16:56:31.184239 basana-1.3.1/basana/external/binance/common.py
+-rw-r--r--   0        0        0      867 2023-03-29 02:43:04.768133 basana-1.3.1/basana/external/binance/config.py
+-rw-r--r--   0        0        0     2111 2023-04-13 16:56:31.184643 basana-1.3.1/basana/external/binance/cross_margin.py
+-rw-r--r--   0        0        0      662 2023-03-29 02:43:04.768810 basana-1.3.1/basana/external/binance/csv/__init__.py
+-rw-r--r--   0        0        0     1648 2023-03-29 02:43:04.769173 basana-1.3.1/basana/external/binance/csv/bars.py
+-rw-r--r--   0        0        0    10385 2023-04-16 21:31:22.354698 basana-1.3.1/basana/external/binance/exchange.py
+-rw-r--r--   0        0        0     3052 2023-03-29 02:43:04.769989 basana-1.3.1/basana/external/binance/helpers.py
+-rw-r--r--   0        0        0     3187 2023-04-13 16:56:31.186035 basana-1.3.1/basana/external/binance/isolated_margin.py
+-rw-r--r--   0        0        0     1913 2023-04-13 16:56:31.186636 basana-1.3.1/basana/external/binance/klines.py
+-rw-r--r--   0        0        0    12082 2023-04-28 03:07:23.331079 basana-1.3.1/basana/external/binance/margin.py
+-rw-r--r--   0        0        0     6165 2023-04-28 03:07:23.331858 basana-1.3.1/basana/external/binance/margin_requests.py
+-rw-r--r--   0        0        0     4143 2023-04-16 21:31:22.355396 basana-1.3.1/basana/external/binance/order_book.py
+-rw-r--r--   0        0        0    12177 2023-04-13 16:56:31.188619 basana-1.3.1/basana/external/binance/spot.py
+-rw-r--r--   0        0        0     5555 2023-04-28 03:07:23.332666 basana-1.3.1/basana/external/binance/spot_requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.772127 basana-1.3.1/basana/external/binance/tools/__init__.py
+-rw-r--r--   0        0        0     4373 2023-03-29 02:43:04.772398 basana-1.3.1/basana/external/binance/tools/download_bars.py
+-rw-r--r--   0        0        0     2710 2023-04-13 16:56:31.189265 basana-1.3.1/basana/external/binance/trades.py
+-rw-r--r--   0        0        0     2647 2023-03-29 02:43:04.772931 basana-1.3.1/basana/external/binance/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.773220 basana-1.3.1/basana/external/bitstamp/__init__.py
+-rw-r--r--   0        0        0     8684 2023-03-29 02:43:04.773512 basana-1.3.1/basana/external/bitstamp/client.py
+-rw-r--r--   0        0        0      865 2023-03-29 02:43:04.773899 basana-1.3.1/basana/external/bitstamp/config.py
+-rw-r--r--   0        0        0      662 2023-03-29 02:43:04.774215 basana-1.3.1/basana/external/bitstamp/csv/__init__.py
+-rw-r--r--   0        0        0     2047 2023-03-29 02:43:04.774543 basana-1.3.1/basana/external/bitstamp/csv/bars.py
+-rw-r--r--   0        0        0    23031 2023-04-16 21:31:22.356361 basana-1.3.1/basana/external/bitstamp/exchange.py
+-rw-r--r--   0        0        0     2374 2023-03-29 02:43:04.775164 basana-1.3.1/basana/external/bitstamp/helpers.py
+-rw-r--r--   0        0        0     4150 2023-04-16 21:31:22.357186 basana-1.3.1/basana/external/bitstamp/order_book.py
+-rw-r--r--   0        0        0     3067 2023-04-16 21:31:22.357564 basana-1.3.1/basana/external/bitstamp/orders.py
+-rw-r--r--   0        0        0     4283 2023-04-28 03:07:23.333551 basana-1.3.1/basana/external/bitstamp/requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.776276 basana-1.3.1/basana/external/bitstamp/tools/__init__.py
+-rw-r--r--   0        0        0     4069 2023-03-29 02:43:04.777227 basana-1.3.1/basana/external/bitstamp/tools/download_bars.py
+-rw-r--r--   0        0        0     2968 2023-04-16 21:31:22.357932 basana-1.3.1/basana/external/bitstamp/trades.py
+-rw-r--r--   0        0        0     4620 2023-03-29 02:43:04.777839 basana-1.3.1/basana/external/bitstamp/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778237 basana-1.3.1/basana/external/common/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778648 basana-1.3.1/basana/external/common/csv/__init__.py
+-rw-r--r--   0        0        0     1763 2023-03-29 02:43:04.779031 basana-1.3.1/basana/external/common/csv/bars.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.779403 basana-1.3.1/basana/external/yahoo/__init__.py
+-rw-r--r--   0        0        0     3384 2023-03-29 02:43:04.779788 basana-1.3.1/basana/external/yahoo/bars.py
+-rw-r--r--   0        0        0     1189 2023-05-22 18:55:08.883336 basana-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 basana-1.3.1/setup.py
+-rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 basana-1.3.1/PKG-INFO
```

### Comparing `basana-1.3.0/LICENSE` & `basana-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/__init__.py` & `basana-1.3.1/basana/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/backtesting/__init__.py` & `basana-1.3.1/basana/backtesting/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/backtesting/account_balances.py` & `basana-1.3.1/basana/backtesting/account_balances.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/backtesting/charts.py` & `basana-1.3.1/basana/backtesting/charts.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,17 @@
         x, y = self._ts.get_x_y()
         figure.add_trace(go.Scatter(x=x, y=y, name=f"Portfolio ({self._symbol})"), row=row, col=1)
 
     async def _on_any_event(self, event: event.Event):
         portfolio_value = Decimal(0)
         balances = await self._exchange.get_balances()
         for symbol, balance in balances.items():
+            if balance.total == 0:
+                continue
+
             rate: Optional[Decimal] = Decimal(1)
             if symbol != self._symbol:
                 rate, _ = await self._exchange.get_bid_ask(Pair(symbol, self._symbol))
 
             if rate:
                 portfolio_value += rate * balance.total
             else:
```

### Comparing `basana-1.3.0/basana/backtesting/errors.py` & `basana-1.3.1/basana/backtesting/errors.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/backtesting/exchange.py` & `basana-1.3.1/basana/backtesting/exchange.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/backtesting/fees.py` & `basana-1.3.1/basana/backtesting/fees.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/backtesting/helpers.py` & `basana-1.3.1/basana/backtesting/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/backtesting/liquidity.py` & `basana-1.3.1/basana/backtesting/liquidity.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/backtesting/orders.py` & `basana-1.3.1/basana/backtesting/orders.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/backtesting/requests.py` & `basana-1.3.1/basana/backtesting/requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/__init__.py` & `basana-1.3.1/basana/core/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/bar.py` & `basana-1.3.1/basana/core/bar.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/config.py` & `basana-1.3.1/basana/core/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/dispatcher.py` & `basana-1.3.1/basana/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/dt.py` & `basana-1.3.1/basana/core/dt.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/enums.py` & `basana-1.3.1/basana/core/enums.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/event.py` & `basana-1.3.1/basana/core/event.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/event_sources/__init__.py` & `basana-1.3.1/basana/core/event_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/event_sources/csv.py` & `basana-1.3.1/basana/core/event_sources/csv.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/event_sources/trading_signal.py` & `basana-1.3.1/basana/core/event_sources/trading_signal.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/helpers.py` & `basana-1.3.1/basana/core/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/logs.py` & `basana-1.3.1/basana/core/logs.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/pair.py` & `basana-1.3.1/basana/core/pair.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/token_bucket.py` & `basana-1.3.1/basana/core/token_bucket.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/core/websockets.py` & `basana-1.3.1/basana/core/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/__init__.py` & `basana-1.3.1/basana/external/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/__init__.py` & `basana-1.3.1/basana/external/binance/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/client.py` & `basana-1.3.1/basana/external/binance/client.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/common.py` & `basana-1.3.1/basana/external/binance/common.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/config.py` & `basana-1.3.1/basana/external/binance/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/cross_margin.py` & `basana-1.3.1/basana/external/binance/cross_margin.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/csv/__init__.py` & `basana-1.3.1/basana/external/binance/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/csv/bars.py` & `basana-1.3.1/basana/external/binance/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/exchange.py` & `basana-1.3.1/basana/external/binance/exchange.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/helpers.py` & `basana-1.3.1/basana/external/binance/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/isolated_margin.py` & `basana-1.3.1/basana/external/binance/isolated_margin.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/klines.py` & `basana-1.3.1/basana/external/binance/klines.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/margin.py` & `basana-1.3.1/basana/external/binance/margin.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/margin_requests.py` & `basana-1.3.1/basana/external/binance/margin_requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/order_book.py` & `basana-1.3.1/basana/external/binance/order_book.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/spot.py` & `basana-1.3.1/basana/external/binance/spot.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/spot_requests.py` & `basana-1.3.1/basana/external/binance/spot_requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/tools/__init__.py` & `basana-1.3.1/basana/external/binance/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/tools/download_bars.py` & `basana-1.3.1/basana/external/binance/tools/download_bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/trades.py` & `basana-1.3.1/basana/external/binance/trades.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/binance/websockets.py` & `basana-1.3.1/basana/external/binance/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/__init__.py` & `basana-1.3.1/basana/external/bitstamp/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/client.py` & `basana-1.3.1/basana/external/bitstamp/client.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/config.py` & `basana-1.3.1/basana/external/bitstamp/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/csv/__init__.py` & `basana-1.3.1/basana/external/bitstamp/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/csv/bars.py` & `basana-1.3.1/basana/external/bitstamp/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/exchange.py` & `basana-1.3.1/basana/external/bitstamp/exchange.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/helpers.py` & `basana-1.3.1/basana/external/bitstamp/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/order_book.py` & `basana-1.3.1/basana/external/bitstamp/order_book.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/orders.py` & `basana-1.3.1/basana/external/bitstamp/orders.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/requests.py` & `basana-1.3.1/basana/external/bitstamp/requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/tools/__init__.py` & `basana-1.3.1/basana/external/bitstamp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/tools/download_bars.py` & `basana-1.3.1/basana/external/bitstamp/tools/download_bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/trades.py` & `basana-1.3.1/basana/external/bitstamp/trades.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/bitstamp/websockets.py` & `basana-1.3.1/basana/external/bitstamp/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/common/__init__.py` & `basana-1.3.1/basana/external/common/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/common/csv/__init__.py` & `basana-1.3.1/basana/external/common/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/common/csv/bars.py` & `basana-1.3.1/basana/external/common/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/yahoo/__init__.py` & `basana-1.3.1/basana/external/yahoo/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/basana/external/yahoo/bars.py` & `basana-1.3.1/basana/external/yahoo/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.0/pyproject.toml` & `basana-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "basana"
-version = "1.3.0"
+version = "1.3.1"
 homepage = "https://github.com/gbeced/basana"
 repository = "https://github.com/gbeced/basana"
 documentation = "https://basana.readthedocs.io/en/latest/"
 description = "A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies."
 authors = ["Gabriel Becedillas <gabriel.becedillas@gmail.com>"]
 license = "Apache-2.0"
 packages = [{include = "basana"}]
@@ -27,12 +27,13 @@
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 talipp = "^1.9.1"
 types-python-dateutil = "^2.8.19.8"
 websockets = "^10.4"
 sphinx = "^6.1.3"
+sphinx-rtd-theme = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `basana-1.3.0/setup.py` & `basana-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ['aiohttp[speedups]>=3.8.4,<4.0.0', 'python-dateutil>=2.8.2,<3.0.0']
 
 extras_require = \
 {'charts': ['plotly>=5.14.1,<6.0.0', 'kaleido==0.2.1']}
 
 setup_kwargs = {
     'name': 'basana',
-    'version': '1.3.0',
+    'version': '1.3.1',
     'description': 'A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies.',
     'long_description': 'None',
     'author': 'Gabriel Becedillas',
     'author_email': 'gabriel.becedillas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/gbeced/basana',
```

### Comparing `basana-1.3.0/PKG-INFO` & `basana-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basana
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies.
 Home-page: https://github.com/gbeced/basana
 License: Apache-2.0
 Author: Gabriel Becedillas
 Author-email: gabriel.becedillas@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

