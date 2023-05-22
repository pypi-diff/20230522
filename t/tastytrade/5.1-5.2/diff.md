# Comparing `tmp/tastytrade-5.1.tar.gz` & `tmp/tastytrade-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-5.1.tar", last modified: Sat May 20 16:53:07 2023, max compression
+gzip compressed data, was "tastytrade-5.2.tar", last modified: Mon May 22 02:05:21 2023, max compression
```

## Comparing `tastytrade-5.1.tar` & `tastytrade-5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:53:07.861299 tastytrade-5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 16:52:54.000000 tastytrade-5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-20 16:53:07.861299 tastytrade-5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-20 16:52:54.000000 tastytrade-5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:53:07.861299 tastytrade-5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-20 16:52:54.000000 tastytrade-5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:53:07.857299 tastytrade-5.1/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34247 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:53:07.861299 tastytrade-5.1/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    30051 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:53:07.861299 tastytrade-5.1/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:05:21.518469 tastytrade-5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 02:05:09.000000 tastytrade-5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-22 02:05:21.518469 tastytrade-5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-05-22 02:05:09.000000 tastytrade-5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:05:21.518469 tastytrade-5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-22 02:05:09.000000 tastytrade-5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:05:21.514469 tastytrade-5.2/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34247 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:05:21.518469 tastytrade-5.2/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:05:21.514469 tastytrade-5.2/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-5.1/LICENSE` & `tastytrade-5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/PKG-INFO` & `tastytrade-5.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: tastytrade
-Version: 5.1
-Summary: An unofficial SDK for Tastytrade!
-Home-page: https://github.com/tastyware/tastytrade
-Author: Graeme Holliday
-Author-email: graeme.holliday@pm.me
-License: MIT
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
    :target: https://pypi.org/project/tastytrade
    :alt: PyPI Package
@@ -85,16 +74,14 @@
    from tastytrade.search import symbol_search
 
    results = symbol_search(session, 'AAP')
    print(results)
 
 >>> [SymbolData(symbol='AAP', description='Advance Auto Parts Inc.'), SymbolData(symbol='AAPD', description='Direxion Daily AAPL Bear 1X Shares'), SymbolData(symbol='AAPL', description='Apple Inc. - Common Stock'), SymbolData(symbol='AAPB', description='GraniteShares 1.75x Long AAPL Daily ETF'), SymbolData(symbol='AAPU', description='Direxion Daily AAPL Bull 1.5X Shares')]
 
-For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
-
 Placing an order
 ----------------
 
 .. code-block:: python
 
    from decimal import Decimal
    from tastytrade.account import Account
@@ -108,14 +95,34 @@
    order = NewOrder(
       time_in_force=OrderTimeInForce.DAY,
       order_type=OrderType.LIMIT,
       legs=[leg],  # you can have multiple legs in an order
       price=Decimal('50'),  # limit price, here $50 for 5 shares = $10/share
       price_effect=PriceEffect.DEBIT
    )
+   response = account.place_order(session, order, dry_run=True)  # a test order
+   print(response)
 
 >>> PlacedOrderResponse(buying_power_effect=BuyingPowerEffect(change_in_margin_requirement=Decimal('125.0'), change_in_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, change_in_buying_power=Decimal('125.004'), change_in_buying_power_effect=<PriceEffect.DEBIT: 'Debit'>, current_buying_power=Decimal('1000.0'), current_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, new_buying_power=Decimal('874.996'), new_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, isolated_order_margin_requirement=Decimal('125.0'), isolated_order_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, is_spread=False, impact=Decimal('125.004'), effect=<PriceEffect.DEBIT: 'Debit'>), fee_calculation=FeeCalculation(regulatory_fees=Decimal('0.0'), regulatory_fees_effect=<PriceEffect.NONE: 'None'>, clearing_fees=Decimal('0.004'), clearing_fees_effect=<PriceEffect.DEBIT: 'Debit'>, commission=Decimal('0.0'), commission_effect=<PriceEffect.NONE: 'None'>, proprietary_index_option_fees=Decimal('0.0'), proprietary_index_option_fees_effect=<PriceEffect.NONE: 'None'>, total_fees=Decimal('0.004'), total_fees_effect=<PriceEffect.DEBIT: 'Debit'>), order=PlacedOrder(account_number='5WV69754', time_in_force=<OrderTimeInForce.DAY: 'Day'>, order_type=<OrderType.LIMIT: 'Limit'>, size='5', underlying_symbol='USO', underlying_instrument_type=<InstrumentType.EQUITY: 'Equity'>, status=<OrderStatus.RECEIVED: 'Received'>, cancellable=True, editable=True, edited=False, updated_at=datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc), legs=[Leg(instrument_type=<InstrumentType.EQUITY: 'Equity'>, symbol='USO', action=<OrderAction.BUY_TO_OPEN: 'Buy to Open'>, quantity=Decimal('5'), remaining_quantity=Decimal('5'), fills=[])], id=None, price=Decimal('50.0'), price_effect=<PriceEffect.DEBIT: 'Debit'>, gtc_date=None, value=None, value_effect=None, stop_trigger=None, contingent_status=None, confirmation_status=None, cancelled_at=None, cancel_user_id=None, cancel_username=None, replacing_order_id=None, replaces_order_id=None, in_flight_at=None, live_at=None, received_at=None, reject_reason=None, user_id=None, username=None, terminal_at=None, complex_order_id=None, complex_order_tag=None, preflight_id=None, order_rule=None), complex_order=None, warnings=[Message(code='tif_next_valid_sesssion', message='Your order will begin working during next valid session.', preflight_id=None)], errors=None)
 
+Options chain/streaming greeks
+------------------------------
+
+.. code-block:: python
+
+   from tastytrade.instruments import get_option_chain
+   from datetime import date
+
+   chain = get_option_chain(session, 'SPLG')
+   subs_list = [chain[date(2023, 6, 16)][0].streamer_symbol]
+
+   greeks = await streamer.oneshot(EventType.GREEKS, subs_list)
+   print(greeks)
+
+>>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
+
+For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
+
 Disclaimer
 ----------
 
 This is an unofficial SDK for Tastytrade. There is no implied warranty for any actions and results which arise from using it.
```

### Comparing `tastytrade-5.1/README.rst` & `tastytrade-5.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: tastytrade
+Version: 5.2
+Summary: An unofficial SDK for Tastytrade!
+Home-page: https://github.com/tastyware/tastytrade
+Author: Graeme Holliday
+Author-email: graeme.holliday@pm.me
+License: MIT
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
    :target: https://pypi.org/project/tastytrade
    :alt: PyPI Package
@@ -74,16 +85,14 @@
    from tastytrade.search import symbol_search
 
    results = symbol_search(session, 'AAP')
    print(results)
 
 >>> [SymbolData(symbol='AAP', description='Advance Auto Parts Inc.'), SymbolData(symbol='AAPD', description='Direxion Daily AAPL Bear 1X Shares'), SymbolData(symbol='AAPL', description='Apple Inc. - Common Stock'), SymbolData(symbol='AAPB', description='GraniteShares 1.75x Long AAPL Daily ETF'), SymbolData(symbol='AAPU', description='Direxion Daily AAPL Bull 1.5X Shares')]
 
-For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
-
 Placing an order
 ----------------
 
 .. code-block:: python
 
    from decimal import Decimal
    from tastytrade.account import Account
@@ -97,14 +106,34 @@
    order = NewOrder(
       time_in_force=OrderTimeInForce.DAY,
       order_type=OrderType.LIMIT,
       legs=[leg],  # you can have multiple legs in an order
       price=Decimal('50'),  # limit price, here $50 for 5 shares = $10/share
       price_effect=PriceEffect.DEBIT
    )
+   response = account.place_order(session, order, dry_run=True)  # a test order
+   print(response)
 
 >>> PlacedOrderResponse(buying_power_effect=BuyingPowerEffect(change_in_margin_requirement=Decimal('125.0'), change_in_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, change_in_buying_power=Decimal('125.004'), change_in_buying_power_effect=<PriceEffect.DEBIT: 'Debit'>, current_buying_power=Decimal('1000.0'), current_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, new_buying_power=Decimal('874.996'), new_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, isolated_order_margin_requirement=Decimal('125.0'), isolated_order_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, is_spread=False, impact=Decimal('125.004'), effect=<PriceEffect.DEBIT: 'Debit'>), fee_calculation=FeeCalculation(regulatory_fees=Decimal('0.0'), regulatory_fees_effect=<PriceEffect.NONE: 'None'>, clearing_fees=Decimal('0.004'), clearing_fees_effect=<PriceEffect.DEBIT: 'Debit'>, commission=Decimal('0.0'), commission_effect=<PriceEffect.NONE: 'None'>, proprietary_index_option_fees=Decimal('0.0'), proprietary_index_option_fees_effect=<PriceEffect.NONE: 'None'>, total_fees=Decimal('0.004'), total_fees_effect=<PriceEffect.DEBIT: 'Debit'>), order=PlacedOrder(account_number='5WV69754', time_in_force=<OrderTimeInForce.DAY: 'Day'>, order_type=<OrderType.LIMIT: 'Limit'>, size='5', underlying_symbol='USO', underlying_instrument_type=<InstrumentType.EQUITY: 'Equity'>, status=<OrderStatus.RECEIVED: 'Received'>, cancellable=True, editable=True, edited=False, updated_at=datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc), legs=[Leg(instrument_type=<InstrumentType.EQUITY: 'Equity'>, symbol='USO', action=<OrderAction.BUY_TO_OPEN: 'Buy to Open'>, quantity=Decimal('5'), remaining_quantity=Decimal('5'), fills=[])], id=None, price=Decimal('50.0'), price_effect=<PriceEffect.DEBIT: 'Debit'>, gtc_date=None, value=None, value_effect=None, stop_trigger=None, contingent_status=None, confirmation_status=None, cancelled_at=None, cancel_user_id=None, cancel_username=None, replacing_order_id=None, replaces_order_id=None, in_flight_at=None, live_at=None, received_at=None, reject_reason=None, user_id=None, username=None, terminal_at=None, complex_order_id=None, complex_order_tag=None, preflight_id=None, order_rule=None), complex_order=None, warnings=[Message(code='tif_next_valid_sesssion', message='Your order will begin working during next valid session.', preflight_id=None)], errors=None)
 
+Options chain/streaming greeks
+------------------------------
+
+.. code-block:: python
+
+   from tastytrade.instruments import get_option_chain
+   from datetime import date
+
+   chain = get_option_chain(session, 'SPLG')
+   subs_list = [chain[date(2023, 6, 16)][0].streamer_symbol]
+
+   greeks = await streamer.oneshot(EventType.GREEKS, subs_list)
+   print(greeks)
+
+>>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
+
+For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
+
 Disclaimer
 ----------
 
-This is an unofficial SDK for Tastytrade. There is no implied warranty for any actions and results which arise from using it.
+This is an unofficial SDK for Tastytrade. There is no implied warranty for any actions and results which arise from using it.
```

### Comparing `tastytrade-5.1/setup.py` & `tastytrade-5.2/setup.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/account.py` & `tastytrade-5.2/tastytrade/account.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/dxfeed/candle.py` & `tastytrade-5.2/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/dxfeed/event.py` & `tastytrade-5.2/tastytrade/dxfeed/event.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/dxfeed/greeks.py` & `tastytrade-5.2/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/dxfeed/profile.py` & `tastytrade-5.2/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/dxfeed/quote.py` & `tastytrade-5.2/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/dxfeed/summary.py` & `tastytrade-5.2/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/dxfeed/theoprice.py` & `tastytrade-5.2/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/dxfeed/trade.py` & `tastytrade-5.2/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/instruments.py` & `tastytrade-5.2/tastytrade/instruments.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,51 @@
     expiration_type: str
     expiration_date: date
     days_to_expiration: int
     settlement_type: str
     strikes: list[Strike]
 
 
+class NestedFutureOptionChainExpiration(TastytradeJsonDataclass):
+    """
+    Dataclass representing an expiration in a nested future options chain.
+    """
+    root_symbol: str
+    notional_value: Decimal
+    underlying_symbol: str
+    strike_factor: Decimal
+    days_to_expiration: int
+    option_root_symbol: str
+    expiration_date: date
+    expires_at: datetime
+    asset: str
+    expiration_type: str
+    display_factor: Decimal
+    option_contract_symbol: str
+    stops_trading_at: datetime
+    settlement_type: str
+    strikes: list[Strike]
+    tick_sizes: list[TickSize]
+
+
+class NestedFutureOptionFuture(TastytradeJsonDataclass):
+    """
+    Dataclass representing an underlying future in a nested future options chain.
+    """
+    root_symbol: str
+    days_to_expiration: int
+    expiration_date: date
+    expires_at: datetime
+    next_active_month: bool
+    symbol: str
+    active_month: bool
+    stops_trading_at: datetime
+    maturity_date: Optional[date] = None
+
+
 class FutureEtfEquivalent(TastytradeJsonDataclass):
     """
     Dataclass that represents the ETF equivalent for a future (aka, the number
     of shares of the ETF that are equivalent to one future, leverage-wise).
     """
     symbol: str
     share_quantity: int
@@ -445,15 +482,15 @@
     option_chain_type: str
     shares_per_contract: int
     tick_sizes: list[TickSize]
     deliverables: list[Deliverable]
     expirations: list[NestedOptionChainExpiration]
 
     @classmethod
-    def get_nested_option_chain(cls, session: Session, symbol: str) -> 'NestedOptionChain':
+    def get_chain(cls, session: Session, symbol: str) -> 'NestedOptionChain':
         """
         Gets the option chain for the given symbol in nested format.
 
         :param session: the session to use for the request.
         :param symbol: the symbol to get the option chain for.
 
         :return: a :class:`NestedOptionChain` object.
@@ -826,14 +863,59 @@
         validate_response(response)
 
         data = response.json()['data']
 
         return cls(**data)
 
 
+class NestedFutureOptionSubchain(TastytradeJsonDataclass):
+    """
+    Dataclass that represents a Tastytrade nested future option chain for a
+    specific futures underlying symbol.
+    """
+    underlying_symbol: str
+    root_symbol: str
+    exercise_style: str
+    expirations: list[NestedFutureOptionChainExpiration]
+
+
+class NestedFutureOptionChain(TastytradeJsonDataclass):
+    """
+    Dataclass that represents a Tastytrade nested option chain object. Contains
+    information about the option chain and a method to fetch one for a symbol.
+
+    The nested option chain is a bit neater than calling :meth:`get_future_option_chain`
+    but if you want to create actual :class:`FutureOption` objects you'll need to make an
+    extra API request or two.
+    """
+    futures: list[NestedFutureOptionFuture]
+    option_chains: list[NestedFutureOptionSubchain]
+
+    @classmethod
+    def get_chain(cls, session: Session, symbol: str) -> 'NestedFutureOptionChain':
+        """
+        Gets the futures option chain for the given symbol in nested format.
+
+        :param session: the session to use for the request.
+        :param symbol: the symbol to get the option chain for.
+
+        :return: a :class:`NestedFutureOptionChain` object.
+        """
+        symbol = symbol.replace('/', '')
+        response = requests.get(
+            f'{session.base_url}/futures-option-chains/{symbol}/nested',
+            headers=session.headers
+        )
+        validate_response(response)
+
+        data = response.json()['data']
+
+        return cls(**data)
+
+
 class Warrant(TastytradeJsonDataclass):
     """
     Dataclass that represents a Tastytrade warrant object. Contains
     information about the warrant, and methods to get warrants.
     """
     symbol: str
     instrument_type: InstrumentType
@@ -949,15 +1031,15 @@
     representing the options chain for the given symbol.
 
     :param session: the session to use for the request.
     :param symbol: the symbol to get the option chain for.
 
     :return: a dict mapping expiration date to a list of :class:`FutureOption` objects.
     """
-    symbol = symbol.replace('/', '%2F')
+    symbol = symbol.replace('/', '')
     response = requests.get(
         f'{session.base_url}/futures-option-chains/{symbol}',
         headers=session.headers
     )
     validate_response(response)
 
     data = response.json()['data']['items']
```

### Comparing `tastytrade-5.1/tastytrade/metrics.py` & `tastytrade-5.2/tastytrade/metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/order.py` & `tastytrade-5.2/tastytrade/order.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/search.py` & `tastytrade-5.2/tastytrade/search.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/session.py` & `tastytrade-5.2/tastytrade/session.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/streamer.py` & `tastytrade-5.2/tastytrade/streamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import json
 from asyncio import Lock, Queue
 from datetime import datetime
 from enum import Enum
-from typing import Any, AsyncIterator, Optional
+from typing import Any, AsyncIterator, Optional, Union
 
 import requests
 import websockets
 
 from tastytrade import logger
 from tastytrade.account import Account
 from tastytrade.dxfeed import Channel
@@ -149,15 +149,15 @@
         Sends a heartbeat message every 10 seconds to keep the connection alive.
         """
         while not self._done:
             await self._subscribe(SubscriptionType.HEARTBEAT, '')
             # send the heartbeat every 10 seconds
             await asyncio.sleep(10)
 
-    async def _subscribe(self, subscription: SubscriptionType, value: Optional[str] | list[str] = '') -> None:
+    async def _subscribe(self, subscription: SubscriptionType, value: Union[Optional[str], list[str]] = '') -> None:
         """
         Subscribes to one of the :class:`SubscriptionType`s. Depending on the kind of
         subscription, the value parameter may be required.
         """
         message: dict[str, Any] = {
             'auth-token': self.token,
             'action': subscription
@@ -207,20 +207,30 @@
     @classmethod
     async def create(cls, session: Session) -> 'DataStreamer':
         """
         Factory method for the :class:`DataStreamer` object. Simply calls the
         constructor and performs the asynchronous setup tasks. This should be used
         instead of the constructor.
 
+        Setup time is around 10-15 seconds.
+
         :param session: active user session to use
         """
         self = cls(session)
         while not self.client_id:
             await asyncio.sleep(0.1)
 
+        # see Github issue #45:
+        # once the handshake completes, although setup is completed locally, remotely there
+        # is still some kind of setup process that hasn't happened that takes about 8-9
+        # seconds, and afterwards you're good to go. Unfortunately, there's no way to know
+        # when that process concludes remotely, as there's no kind of confirmation message
+        # sent. This is a hacky solution to ensure streamer setup completes.
+        await self.oneshot(EventType.QUOTE, ['SPY'])
+
         return self
 
     async def _next_id(self):
         async with self._lock:
             self._counter += 1
         return self._counter
 
@@ -449,15 +459,16 @@
         :param interval: the width of each candle in time, e.g. '5m', '1h', '3d', '1w', '1mo'
         """
         await self.subscribe_candle(ticker, start_time, interval)
         candles = []
         async for candle in self.listen_candle():
             candles.append(candle)
             # until we hit the start date, keep going
-            if datetime.fromtimestamp(candle.time / 1000) <= start_time:
+            # use timestamp to support timezone in start_time
+            if candle.time <= start_time.timestamp() * 1000:
                 break
         await self.unsubscribe_candle(ticker, interval)
 
         candles.reverse()
         return candles
```

### Comparing `tastytrade-5.1/tastytrade/utils.py` & `tastytrade-5.2/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade/watchlists.py` & `tastytrade-5.2/tastytrade/watchlists.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.1/tastytrade.egg-info/PKG-INFO` & `tastytrade-5.2/tastytrade.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.1
+Version: 5.2
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -85,16 +85,14 @@
    from tastytrade.search import symbol_search
 
    results = symbol_search(session, 'AAP')
    print(results)
 
 >>> [SymbolData(symbol='AAP', description='Advance Auto Parts Inc.'), SymbolData(symbol='AAPD', description='Direxion Daily AAPL Bear 1X Shares'), SymbolData(symbol='AAPL', description='Apple Inc. - Common Stock'), SymbolData(symbol='AAPB', description='GraniteShares 1.75x Long AAPL Daily ETF'), SymbolData(symbol='AAPU', description='Direxion Daily AAPL Bull 1.5X Shares')]
 
-For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
-
 Placing an order
 ----------------
 
 .. code-block:: python
 
    from decimal import Decimal
    from tastytrade.account import Account
@@ -108,14 +106,34 @@
    order = NewOrder(
       time_in_force=OrderTimeInForce.DAY,
       order_type=OrderType.LIMIT,
       legs=[leg],  # you can have multiple legs in an order
       price=Decimal('50'),  # limit price, here $50 for 5 shares = $10/share
       price_effect=PriceEffect.DEBIT
    )
+   response = account.place_order(session, order, dry_run=True)  # a test order
+   print(response)
 
 >>> PlacedOrderResponse(buying_power_effect=BuyingPowerEffect(change_in_margin_requirement=Decimal('125.0'), change_in_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, change_in_buying_power=Decimal('125.004'), change_in_buying_power_effect=<PriceEffect.DEBIT: 'Debit'>, current_buying_power=Decimal('1000.0'), current_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, new_buying_power=Decimal('874.996'), new_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, isolated_order_margin_requirement=Decimal('125.0'), isolated_order_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, is_spread=False, impact=Decimal('125.004'), effect=<PriceEffect.DEBIT: 'Debit'>), fee_calculation=FeeCalculation(regulatory_fees=Decimal('0.0'), regulatory_fees_effect=<PriceEffect.NONE: 'None'>, clearing_fees=Decimal('0.004'), clearing_fees_effect=<PriceEffect.DEBIT: 'Debit'>, commission=Decimal('0.0'), commission_effect=<PriceEffect.NONE: 'None'>, proprietary_index_option_fees=Decimal('0.0'), proprietary_index_option_fees_effect=<PriceEffect.NONE: 'None'>, total_fees=Decimal('0.004'), total_fees_effect=<PriceEffect.DEBIT: 'Debit'>), order=PlacedOrder(account_number='5WV69754', time_in_force=<OrderTimeInForce.DAY: 'Day'>, order_type=<OrderType.LIMIT: 'Limit'>, size='5', underlying_symbol='USO', underlying_instrument_type=<InstrumentType.EQUITY: 'Equity'>, status=<OrderStatus.RECEIVED: 'Received'>, cancellable=True, editable=True, edited=False, updated_at=datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc), legs=[Leg(instrument_type=<InstrumentType.EQUITY: 'Equity'>, symbol='USO', action=<OrderAction.BUY_TO_OPEN: 'Buy to Open'>, quantity=Decimal('5'), remaining_quantity=Decimal('5'), fills=[])], id=None, price=Decimal('50.0'), price_effect=<PriceEffect.DEBIT: 'Debit'>, gtc_date=None, value=None, value_effect=None, stop_trigger=None, contingent_status=None, confirmation_status=None, cancelled_at=None, cancel_user_id=None, cancel_username=None, replacing_order_id=None, replaces_order_id=None, in_flight_at=None, live_at=None, received_at=None, reject_reason=None, user_id=None, username=None, terminal_at=None, complex_order_id=None, complex_order_tag=None, preflight_id=None, order_rule=None), complex_order=None, warnings=[Message(code='tif_next_valid_sesssion', message='Your order will begin working during next valid session.', preflight_id=None)], errors=None)
 
+Options chain/streaming greeks
+------------------------------
+
+.. code-block:: python
+
+   from tastytrade.instruments import get_option_chain
+   from datetime import date
+
+   chain = get_option_chain(session, 'SPLG')
+   subs_list = [chain[date(2023, 6, 16)][0].streamer_symbol]
+
+   greeks = await streamer.oneshot(EventType.GREEKS, subs_list)
+   print(greeks)
+
+>>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
+
+For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
+
 Disclaimer
 ----------
 
 This is an unofficial SDK for Tastytrade. There is no implied warranty for any actions and results which arise from using it.
```

### Comparing `tastytrade-5.1/tastytrade.egg-info/SOURCES.txt` & `tastytrade-5.2/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

