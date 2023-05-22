# Comparing `tmp/google_calendar_analytics-0.4.2.tar.gz` & `tmp/google_calendar_analytics-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_calendar_analytics-0.4.2.tar", max compression
+gzip compressed data, was "google_calendar_analytics-0.5.0.tar", max compression
```

## Comparing `google_calendar_analytics-0.4.2.tar` & `google_calendar_analytics-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2023-02-12 18:59:52.246285 google_calendar_analytics-0.4.2/LICENSE
--rw-r--r--   0        0        0     4356 2023-04-02 11:00:58.401965 google_calendar_analytics-0.4.2/README.md
--rw-r--r--   0        0        0     1097 2023-04-02 05:28:49.682864 google_calendar_analytics-0.4.2/google_calendar_analytics/__init__.py
--rw-r--r--   0        0        0       69 2023-04-02 11:02:13.892547 google_calendar_analytics-0.4.2/google_calendar_analytics/_version.py
--rw-r--r--   0        0        0    13415 2023-04-02 10:56:58.228911 google_calendar_analytics-0.4.2/google_calendar_analytics/analytics.py
--rw-r--r--   0        0        0        0 2023-03-18 06:29:15.506319 google_calendar_analytics-0.4.2/google_calendar_analytics/authentication/__init__.py
--rw-r--r--   0        0        0     1711 2023-03-21 12:47:26.161912 google_calendar_analytics-0.4.2/google_calendar_analytics/authentication/auth.py
--rw-r--r--   0        0        0        0 2023-03-18 06:29:18.543932 google_calendar_analytics-0.4.2/google_calendar_analytics/collecting/__init__.py
--rw-r--r--   0        0        0     2024 2023-03-31 09:15:51.113797 google_calendar_analytics-0.4.2/google_calendar_analytics/collecting/collector.py
--rw-r--r--   0        0        0        0 2023-03-18 06:29:20.261408 google_calendar_analytics-0.4.2/google_calendar_analytics/core/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-01 13:00:10.493454 google_calendar_analytics-0.4.2/google_calendar_analytics/core/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-18 06:29:21.718335 google_calendar_analytics-0.4.2/google_calendar_analytics/processing/__init__.py
--rw-r--r--   0        0        0     6074 2023-04-02 05:23:31.107421 google_calendar_analytics-0.4.2/google_calendar_analytics/processing/transformer.py
--rw-r--r--   0        0        0        0 2023-03-18 06:29:23.422477 google_calendar_analytics-0.4.2/google_calendar_analytics/visualization/__init__.py
--rw-r--r--   0        0        0      277 2023-03-18 06:29:23.419260 google_calendar_analytics-0.4.2/google_calendar_analytics/visualization/image_saver.py
--rw-r--r--   0        0        0     1373 2023-04-02 10:44:23.212207 google_calendar_analytics-0.4.2/google_calendar_analytics/visualization/visual_design.py
--rw-r--r--   0        0        0    11300 2023-04-02 10:56:58.305084 google_calendar_analytics-0.4.2/google_calendar_analytics/visualization/visualizer_factory.py
--rw-r--r--   0        0        0     1527 2023-04-02 11:02:13.897256 google_calendar_analytics-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5492 1970-01-01 00:00:00.000000 google_calendar_analytics-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-12 18:59:52.246285 google_calendar_analytics-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4982 2023-05-09 12:00:22.353227 google_calendar_analytics-0.5.0/README.md
+-rw-r--r--   0        0        0     1304 2023-05-09 12:02:27.569993 google_calendar_analytics-0.5.0/google_calendar_analytics/__init__.py
+-rw-r--r--   0        0        0       69 2023-05-09 12:01:18.944087 google_calendar_analytics-0.5.0/google_calendar_analytics/_version.py
+-rw-r--r--   0        0        0    14035 2023-05-22 02:23:37.921985 google_calendar_analytics-0.5.0/google_calendar_analytics/analytics.py
+-rw-r--r--   0        0        0        0 2023-03-18 06:29:15.506319 google_calendar_analytics-0.5.0/google_calendar_analytics/authentication/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-22 02:04:05.935890 google_calendar_analytics-0.5.0/google_calendar_analytics/authentication/auth.py
+-rw-r--r--   0        0        0        0 2023-03-18 06:29:18.543932 google_calendar_analytics-0.5.0/google_calendar_analytics/collecting/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-22 03:03:14.138885 google_calendar_analytics-0.5.0/google_calendar_analytics/collecting/collector.py
+-rw-r--r--   0        0        0        0 2023-03-18 06:29:20.261408 google_calendar_analytics-0.5.0/google_calendar_analytics/core/__init__.py
+-rw-r--r--   0        0        0     1442 2023-04-01 13:00:10.493454 google_calendar_analytics-0.5.0/google_calendar_analytics/core/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-18 06:29:21.718335 google_calendar_analytics-0.5.0/google_calendar_analytics/processing/__init__.py
+-rw-r--r--   0        0        0     6079 2023-05-22 03:04:26.525746 google_calendar_analytics-0.5.0/google_calendar_analytics/processing/transformer.py
+-rw-r--r--   0        0        0        0 2023-03-18 06:29:23.422477 google_calendar_analytics-0.5.0/google_calendar_analytics/visualization/__init__.py
+-rw-r--r--   0        0        0      277 2023-03-18 06:29:23.419260 google_calendar_analytics-0.5.0/google_calendar_analytics/visualization/image_saver.py
+-rw-r--r--   0        0        0     1373 2023-04-02 10:44:23.212207 google_calendar_analytics-0.5.0/google_calendar_analytics/visualization/visual_design.py
+-rw-r--r--   0        0        0    11300 2023-04-02 10:56:58.305084 google_calendar_analytics-0.5.0/google_calendar_analytics/visualization/visualizer_factory.py
+-rw-r--r--   0        0        0     1567 2023-05-22 02:11:24.346744 google_calendar_analytics-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6089 1970-01-01 00:00:00.000000 google_calendar_analytics-0.5.0/PKG-INFO
```

### Comparing `google_calendar_analytics-0.4.2/LICENSE` & `google_calendar_analytics-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_calendar_analytics-0.4.2/README.md` & `google_calendar_analytics-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 import asyncio
 from datetime import datetime
 
 from google.oauth2.credentials import Credentials
 from google_calendar_analytics import AnalyzerFacade
 
 # (You can get it from Google OAuth2 in you web app or from link above)
-# Example of creds dictionary. (You can get it from Google OAuth2 in your web app)
 creds = {
     "token": "ya29.a0AVvZVsoH4qZcrGK25VwsXspJv-r9K-",
     "refresh_token": "1//0hwlhrtalKgeRCgYIARAAGBESNwF-",
     "token_uri": "https://oauth2.googleapis.com/token",
     "client_id": "395np.apps.googleusercontent.com",
     "client_secret": "GOCSPXFqoucE03VRVz",
     "scopes": ["https://www.googleapis.com/auth/calendar"],
@@ -60,30 +59,44 @@
 }
 creds = Credentials.from_authorized_user_info(creds)
 ```
 
 Once you have created the credentials, you can create an instance of the AnalyzerFacade class and use it to analyze your data:
 
 ```python
-analyzer = AnalyzerFacade(creds=creds)
-
 # Choose time range for analysis
 start_time = datetime(2023, 3, 1)
 end_time = datetime(2023, 3, 18)
 
 
-def main():
-    plot = await analyzer.analyze_one(start_time, end_time, event_name="Programming", plot_type="Line")
-    plot.show()
-
+async def main():
+    async with AnalyzerFacade(creds=creds) as analyzer:
+        plot = await analyzer.analyze_one(start_time, end_time, event_name="Programming", plot_type="Line")
+        plot.show()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+What's about multiple plots?
+```python
+async def main():
+    async with AnalyzerFacade(creds=creds) as analyzer:
+        coroutines = []
+        
+        coroutines.append(analyzer.analyze_one(start_time, end_time, event_name="Programming", plot_type="Line")
+        coroutines.append(analyzer.analyze_one(start_time, end_time, event_name="Reading", plot_type="Line"))
+        coroutines.append(analyzer.analyze_many(start_time, end_time, plot_type="Pie"))
+        coroutines.append(analyzer.analyze_many(start_time, end_time, plot_type="Bar"))
+                          
+        result = await asyncio.gather(*coroutines)
+        for plot in result:
+            plot.show()
+```
+
 ## Contribution
 
 If you would like to contribute to this project, please feel free to submit a pull request. Some areas where
 contributions are particularly welcome include:
 
 - Adding new features
 - Improving existing features
```

### Comparing `google_calendar_analytics-0.4.2/google_calendar_analytics/__init__.py` & `google_calendar_analytics-0.5.0/google_calendar_analytics/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,23 @@
 :copyright: (c) 2023 Berupor
 """
 
 from ._version import __version__ as version
 from .analytics import AnalyzerFacade
 from .authentication.auth import CalendarAuth
 from .collecting.collector import AsyncCalendarDataCollector
-from .processing.transformer import (
-    AsyncDataTransformer,
-    EventDurationPeriodsStrategy,
-    ManyEventsDurationStrategy,
-    OneEventDurationStrategy,
-)
-from .visualization.visualizer_factory import (
-    BarPlot,
-    LinePlot,
-    MultyLinePlot,
-    PiePlot,
-    PlotFactory,
-)
-from .visualization.visual_design import VisualDesign, base_plot_design, pastel_palette
+from .processing.transformer import (AsyncDataTransformer,
+                                     EventDurationPeriodsStrategy,
+                                     ManyEventsDurationStrategy,
+                                     OneEventDurationStrategy)
+from .visualization.visual_design import (VisualDesign, base_plot_design,
+                                          pastel_palette)
+from .visualization.visualizer_factory import (BarPlot, LinePlot,
+                                               MultyLinePlot, PiePlot,
+                                               PlotFactory)
 
 __all__ = [
     "AnalyzerFacade",
     "AsyncCalendarDataCollector",
     "AsyncDataTransformer",
     "BarPlot",
     "CalendarAuth",
```

### Comparing `google_calendar_analytics-0.4.2/google_calendar_analytics/analytics.py` & `google_calendar_analytics-0.5.0/google_calendar_analytics/analytics.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 event, the analyze_many method analyzes multiple events, and the analyze_one_with_periods
 method analyzes a single event over a period of time.
 
 The AnalyzerBuilder class is a builder class that allows for creating instances of the
 AnalyzerFacade class with different options.
 
 """
-
+import ssl
 from datetime import datetime
 from typing import Type
 
+import aiohttp
+import certifi
 import plotly.graph_objs as go
 from google.oauth2.credentials import Credentials  # type: ignore
 
 from .collecting.collector import AsyncCalendarDataCollector
 from .core import exceptions
-from .processing.transformer import (
-    AsyncDataTransformer,
-    EventDurationPeriodsStrategy,
-    ManyEventsDurationStrategy,
-    OneEventDurationStrategy,
-)
-from .visualization.visual_design import base_plot_design, VisualDesign
+from .processing.transformer import (EventDurationPeriodsStrategy,
+                                     EventDurationStrategy,
+                                     ManyEventsDurationStrategy,
+                                     OneEventDurationStrategy)
+from .visualization.visual_design import VisualDesign, base_plot_design
 from .visualization.visualizer_factory import PlotFactory
 
 
 class AnalyzerFacade:
     """
     Facade class for analyzing calendar events and generating charts.
 
@@ -49,15 +49,14 @@
 
     Attributes:
         creds (Credentials): An instance of the Credentials class.
         plot_type (str): The type of chart to be generated.
         max_events (int): The maximum number of events to be analyzed.
         ascending (bool): If True, sort the events in ascending order of duration.
         data_collector (AsyncCalendarDataCollector): An instance of the CalendarDataCollector class.
-        data_transformer (DataTransformer): An instance of the DataTransformer class.
 
     Examples:
         ```python
         # Initialize AnalyzerFacade and analyze a single event
         analyzer = AnalyzerBuilder().with_credentials(creds).build()
         start_time = datetime(2023, 3, 1, tzinfo=pytz.UTC)
         end_time = datetime(2023, 3, 18, tzinfo=pytz.UTC)
@@ -91,16 +90,31 @@
     def __init__(self, creds: Credentials):
         self.style_class = None
         self.creds = creds
         self.plot_type = "Line"
         self.max_events = 5
         self.ascending = False
 
-        self.data_collector = AsyncCalendarDataCollector(creds)
-        self.data_transformer = AsyncDataTransformer()
+        self.session = None
+        self.data_collector = None
+
+    async def __aenter__(self):
+        ssl_context = ssl.create_default_context(cafile=certifi.where())
+        self.session = aiohttp.ClientSession(
+            connector=aiohttp.TCPConnector(ssl=ssl_context)
+        )
+        self.data_collector = AsyncCalendarDataCollector(self.creds, self.session)
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        if self.session:
+            await self.session.close()
+
+        self.session = None
+        self.data_collector = None
 
     async def analyze_one(
         self,
         start_time: datetime,
         end_time: datetime,
         event_name: str,
         plot_type: str,
@@ -139,20 +153,20 @@
         """
         if plot_type not in ("Line",):
             raise exceptions.InvalidPlotTypeError(self.plot_type, method="analyze_one")
 
         self.style_class = style_class
         self.plot_type = plot_type
 
-        self.data_transformer.set_strategy(OneEventDurationStrategy())
         return await self._analyze(
             start_time=start_time,
             end_time=end_time,
             event_name=event_name,
             method="one",
+            transformer_strategy=OneEventDurationStrategy(),
         )
 
     async def analyze_many(
         self,
         start_time: datetime,
         end_time: datetime,
         plot_type: str,
@@ -193,19 +207,19 @@
             raise exceptions.InvalidPlotTypeError(self.plot_type, method="analyze_many")
 
         self.style_class = style_class
         self.plot_type = plot_type
         self.max_events = max_events
         self.ascending = ascending
 
-        self.data_transformer.set_strategy(ManyEventsDurationStrategy())
         return await self._analyze(
             start_time=start_time,
             end_time=end_time,
             method="many",
+            transformer_strategy=ManyEventsDurationStrategy(),
         )
 
     async def analyze_one_with_periods(
         self,
         start_time: datetime,
         end_time: datetime,
         event_name: str,
@@ -253,41 +267,43 @@
             raise exceptions.InvalidPlotTypeError(
                 self.plot_type, method="analyze_one_with_periods"
             )
 
         self.style_class = style_class
         self.plot_type = plot_type
 
-        self.data_transformer.set_strategy(EventDurationPeriodsStrategy())
         return await self._analyze(
             start_time=start_time,
             end_time=end_time,
             event_name=event_name,
             method="one_with_periods",
             period_days=period_days,
             num_periods=num_periods,
+            transformer_strategy=EventDurationPeriodsStrategy(),
         )
 
     async def _analyze(
         self,
         start_time: datetime,
         end_time: datetime,
+        transformer_strategy: EventDurationStrategy,
         event_name: str = None,  # type: ignore
         method: str = "one",
         period_days: int = 7,
         num_periods: int = 2,
         **kwargs
     ) -> go.Figure:
         """
         Analyzes calendar events data and creates a plot using the specified method.
 
         Args:
             start_time (datetime): The start time for the analysis.
             end_time (datetime): The end time for the analysis.
             event_name (str, optional): The name of the event to analyze. Required for the 'one' and 'one_with_periods' methods. Defaults to None.
+            transformer_strategy (DataTransformerStrategy): The strategy to use for data transformation.
             method (str, optional): The method to use for analysis. Must be one of 'one', 'many', or 'one_with_periods'. Defaults to 'one'.
             period_days (int, optional): The number of days in each period. Required for the 'one_with_periods' method. Defaults to 7.
             num_periods (int, optional): The number of periods to analyze. Required for the 'one_with_periods' method. Defaults to 2.
             **kwargs: Additional keyword arguments for the plot creation.
 
         Returns:
             go.Figure: The plot generated by the PlotFactory.
@@ -302,29 +318,29 @@
 
         calendar_events = await self.data_collector.collect_data(
             start_time=start_time,
             end_time=end_time,
         )
 
         if method == "one":
-            event_durations = await self.data_transformer.calculate_duration(
+            event_durations = await transformer_strategy.calculate_duration(
                 events=calendar_events, event_name=event_name
             )
             return await plot_creator.plot(
                 events=event_durations, event_name=event_name
             )
         elif method == "many":
-            event_durations = await self.data_transformer.calculate_duration(
+            event_durations = await transformer_strategy.calculate_duration(
                 events=calendar_events,
                 max_events=self.max_events,
                 ascending=self.ascending,
             )
             return await plot_creator.plot(events=event_durations)
         elif method == "one_with_periods":
-            event_durations = await self.data_transformer.calculate_duration(
+            event_durations = await transformer_strategy.calculate_duration(
                 events=calendar_events,
                 event_name=event_name,
                 period_days=period_days,
                 num_periods=num_periods,
             )
 
             return await plot_creator.plot(
```

### Comparing `google_calendar_analytics-0.4.2/google_calendar_analytics/authentication/auth.py` & `google_calendar_analytics-0.5.0/google_calendar_analytics/authentication/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os.path
 
 from google.auth.transport.requests import Request  # type: ignore
 from google.oauth2.credentials import Credentials  # type: ignore
 from google_auth_oauthlib.flow import InstalledAppFlow  # type: ignore
+from pathlib import Path
 
 
 class CalendarAuth:
     SCOPES = ["https://www.googleapis.com/auth/calendar"]
 
-    def __init__(self, token_path: str, credentials_path: str):
+    def __init__(self, token_path: Path, credentials_path: Path):
         self.token_path = token_path
         self.credentials_path = credentials_path
 
     def get_credentials(self) -> Credentials | None:
         """
         Get the user's calendar credentials.
```

### Comparing `google_calendar_analytics-0.4.2/google_calendar_analytics/core/exceptions.py` & `google_calendar_analytics-0.5.0/google_calendar_analytics/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `google_calendar_analytics-0.4.2/google_calendar_analytics/processing/transformer.py` & `google_calendar_analytics-0.5.0/google_calendar_analytics/processing/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,9 +166,10 @@
         self.strategy = strategy
 
     async def calculate_duration(
         self, events: list[dict], *args, **kwargs
     ) -> pd.DataFrame:
         if not self.strategy:
             raise ValueError("Strategy is not set")
-
-        return await self.strategy.calculate_duration(events, *args, **kwargs)
+        return await self.strategy.calculate_duration(
+            events,
+        )
```

### Comparing `google_calendar_analytics-0.4.2/google_calendar_analytics/visualization/visual_design.py` & `google_calendar_analytics-0.5.0/google_calendar_analytics/visualization/visual_design.py`

 * *Files identical despite different names*

### Comparing `google_calendar_analytics-0.4.2/google_calendar_analytics/visualization/visualizer_factory.py` & `google_calendar_analytics-0.5.0/google_calendar_analytics/visualization/visualizer_factory.py`

 * *Files identical despite different names*

### Comparing `google_calendar_analytics-0.4.2/pyproject.toml` & `google_calendar_analytics-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "google-calendar-analytics"
-version = "0.4.2"
+version = "0.5.0"
 description = "A Python library for analyzing Google Calendar data."
 authors = [
     "Berupor <evgeniy.zelenoff@gmail.com>"
 ]
 readme = "README.md"
 packages = [{ include = "google_calendar_analytics" }]
 license = "MIT"
@@ -32,14 +32,16 @@
 pandas = "1.5.3"
 google-auth = "2.16.0"
 google-api-python-client = "2.77.0"
 google-auth-httplib2 = "0.1.0"
 google-auth-oauthlib = "1.0.0"
 plotly = "5.13.0"
 kaleido = "0.2.1"
+aiohttp = "3.8.4"
+certifi = "2022.12.7"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "1.0.1"
 flake8 = "6.0.0"
 black = "*"
 isort = "*"
 pytest = "7.2.1"
```

### Comparing `google_calendar_analytics-0.4.2/PKG-INFO` & `google_calendar_analytics-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: google-calendar-analytics
-Version: 0.4.2
+Version: 0.5.0
 Summary: A Python library for analyzing Google Calendar data.
 License: MIT
 Keywords: google,calendar,analytics,data analysis,event tracking,attendee tracking
 Author: Berupor
 Author-email: evgeniy.zelenoff@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Dist: aiohttp (==3.8.4)
+Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: google-api-python-client (==2.77.0)
 Requires-Dist: google-auth (==2.16.0)
 Requires-Dist: google-auth-httplib2 (==0.1.0)
 Requires-Dist: google-auth-oauthlib (==1.0.0)
 Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: plotly (==5.13.0)
@@ -72,15 +72,14 @@
 import asyncio
 from datetime import datetime
 
 from google.oauth2.credentials import Credentials
 from google_calendar_analytics import AnalyzerFacade
 
 # (You can get it from Google OAuth2 in you web app or from link above)
-# Example of creds dictionary. (You can get it from Google OAuth2 in your web app)
 creds = {
     "token": "ya29.a0AVvZVsoH4qZcrGK25VwsXspJv-r9K-",
     "refresh_token": "1//0hwlhrtalKgeRCgYIARAAGBESNwF-",
     "token_uri": "https://oauth2.googleapis.com/token",
     "client_id": "395np.apps.googleusercontent.com",
     "client_secret": "GOCSPXFqoucE03VRVz",
     "scopes": ["https://www.googleapis.com/auth/calendar"],
@@ -88,30 +87,44 @@
 }
 creds = Credentials.from_authorized_user_info(creds)
 ```
 
 Once you have created the credentials, you can create an instance of the AnalyzerFacade class and use it to analyze your data:
 
 ```python
-analyzer = AnalyzerFacade(creds=creds)
-
 # Choose time range for analysis
 start_time = datetime(2023, 3, 1)
 end_time = datetime(2023, 3, 18)
 
 
-def main():
-    plot = await analyzer.analyze_one(start_time, end_time, event_name="Programming", plot_type="Line")
-    plot.show()
-
+async def main():
+    async with AnalyzerFacade(creds=creds) as analyzer:
+        plot = await analyzer.analyze_one(start_time, end_time, event_name="Programming", plot_type="Line")
+        plot.show()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+What's about multiple plots?
+```python
+async def main():
+    async with AnalyzerFacade(creds=creds) as analyzer:
+        coroutines = []
+        
+        coroutines.append(analyzer.analyze_one(start_time, end_time, event_name="Programming", plot_type="Line")
+        coroutines.append(analyzer.analyze_one(start_time, end_time, event_name="Reading", plot_type="Line"))
+        coroutines.append(analyzer.analyze_many(start_time, end_time, plot_type="Pie"))
+        coroutines.append(analyzer.analyze_many(start_time, end_time, plot_type="Bar"))
+                          
+        result = await asyncio.gather(*coroutines)
+        for plot in result:
+            plot.show()
+```
+
 ## Contribution
 
 If you would like to contribute to this project, please feel free to submit a pull request. Some areas where
 contributions are particularly welcome include:
 
 - Adding new features
 - Improving existing features
```

