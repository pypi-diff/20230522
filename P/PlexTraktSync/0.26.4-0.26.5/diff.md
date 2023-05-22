# Comparing `tmp/PlexTraktSync-0.26.4.tar.gz` & `tmp/PlexTraktSync-0.26.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-ro158mv9/PlexTraktSync-0.26.4.tar", last modified: Tue Apr 25 07:57:20 2023, max compression
+gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-y7kxfii4/PlexTraktSync-0.26.5.tar", last modified: Mon May 22 17:56:10 2023, max compression
```

## Comparing `PlexTraktSync-0.26.4.tar` & `PlexTraktSync-0.26.5.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/ServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/http_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/plex/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/rich_addons.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/servers.default.yml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/trakt_list_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/util/remove_empty_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-25 07:57:12.000000 PlexTraktSync-0.26.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:57:20.000000 PlexTraktSync-0.26.4/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_plex_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-25 07:57:10.000000 PlexTraktSync-0.26.4/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/ServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/http_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/rich_addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/servers.default.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt_list_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/remove_empty_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-22 17:56:02.000000 PlexTraktSync-0.26.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_plex_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_walker.py
```

### Comparing `PlexTraktSync-0.26.4/LICENSE` & `PlexTraktSync-0.26.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/PKG-INFO` & `PlexTraktSync-0.26.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.4
+Version: 0.26.5
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,27 +25,35 @@
 
 This project adds a two-way-sync between trakt.tv and Plex Media Server. It
 requires a trakt.tv account but no Plex premium and no Trakt VIP subscriptions,
 unlike the Plex app provided by Trakt.
 
 ![image](https://raw.githubusercontent.com/twolaw/PlexTraktSync/img/plextraktsync_banner.png)
 
-Originally created by [@Taxel][@taxel], but now maintained by [contributors].
+Originally created by [@Taxel][@taxel], now maintained by [contributors].
 
 [@taxel]: https://github.com/Taxel
 [contributors]: https://github.com/Taxel/PlexTraktSync/graphs/contributors
 
 Note: The PyTrakt API keys are not stored securely, so if you do not want to
 have a file containing those on your harddrive, you can not use this project.
 
-**Looking for a way to contribute? Please find issues with the [help-wanted]
-label or to improve documentation [docs-needed], thank you.**
+## Contribute
+
+**Looking for a way to contribute?**
+- find issues with the [help-wanted] label
+- improve documentation [docs-needed] label
+- you can also just [create a pull request] to improve documentation
+- ... more [developer contribution](CONTRIBUTING.md) docs
 
 [help-wanted]: https://github.com/Taxel/PlexTraktSync/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22
 [docs-needed]: https://github.com/Taxel/PlexTraktSync/issues?q=label%3A%22docs+needed%22+sort%3Aupdated-desc
+[create a pull request]: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
+
+----
 
 - [Plex-Trakt-Sync](#plex-trakt-sync)
   - [Features](#features)
   - [Pre-requisites](#pre-requisites)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [Docker Compose](#docker-compose)
@@ -322,14 +330,19 @@
 the "debug" variable in `config.yml` to `true`.
 
 By default the logs will append, if you wish to maintain the log of only your
 last run then edit the "append" variable in `config.yml` to `false`.
 
 ## Commands
 
+Run `plextraktsync --help` to see available commands.
+Run `plextraktsync COMMAND --help` to see help for `COMMAND`.
+
+You can [contribute](#contribute) yourself missing documentation.
+
 ### Sync
 
 The `sync` subcommand supports `--sync=shows` and `--sync=movies` options,
 so you can sync only specific library types.
 Or only watchlist: `--sync=watchlist`.
 
 ```
```

### Comparing `PlexTraktSync-0.26.4/PlexTraktSync.egg-info/PKG-INFO` & `PlexTraktSync-0.26.5/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.4
+Version: 0.26.5
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,27 +25,35 @@
 
 This project adds a two-way-sync between trakt.tv and Plex Media Server. It
 requires a trakt.tv account but no Plex premium and no Trakt VIP subscriptions,
 unlike the Plex app provided by Trakt.
 
 ![image](https://raw.githubusercontent.com/twolaw/PlexTraktSync/img/plextraktsync_banner.png)
 
-Originally created by [@Taxel][@taxel], but now maintained by [contributors].
+Originally created by [@Taxel][@taxel], now maintained by [contributors].
 
 [@taxel]: https://github.com/Taxel
 [contributors]: https://github.com/Taxel/PlexTraktSync/graphs/contributors
 
 Note: The PyTrakt API keys are not stored securely, so if you do not want to
 have a file containing those on your harddrive, you can not use this project.
 
-**Looking for a way to contribute? Please find issues with the [help-wanted]
-label or to improve documentation [docs-needed], thank you.**
+## Contribute
+
+**Looking for a way to contribute?**
+- find issues with the [help-wanted] label
+- improve documentation [docs-needed] label
+- you can also just [create a pull request] to improve documentation
+- ... more [developer contribution](CONTRIBUTING.md) docs
 
 [help-wanted]: https://github.com/Taxel/PlexTraktSync/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22
 [docs-needed]: https://github.com/Taxel/PlexTraktSync/issues?q=label%3A%22docs+needed%22+sort%3Aupdated-desc
+[create a pull request]: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
+
+----
 
 - [Plex-Trakt-Sync](#plex-trakt-sync)
   - [Features](#features)
   - [Pre-requisites](#pre-requisites)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [Docker Compose](#docker-compose)
@@ -322,14 +330,19 @@
 the "debug" variable in `config.yml` to `true`.
 
 By default the logs will append, if you wish to maintain the log of only your
 last run then edit the "append" variable in `config.yml` to `false`.
 
 ## Commands
 
+Run `plextraktsync --help` to see available commands.
+Run `plextraktsync COMMAND --help` to see help for `COMMAND`.
+
+You can [contribute](#contribute) yourself missing documentation.
+
 ### Sync
 
 The `sync` subcommand supports `--sync=shows` and `--sync=movies` options,
 so you can sync only specific library types.
 Or only watchlist: `--sync=watchlist`.
 
 ```
```

### Comparing `PlexTraktSync-0.26.4/PlexTraktSync.egg-info/SOURCES.txt` & `PlexTraktSync-0.26.5/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/PlexTraktSync.egg-info/requires.txt` & `PlexTraktSync-0.26.5/PlexTraktSync.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 attrs==23.1.0
-certifi==2022.12.7
+certifi==2023.5.7
 charset-normalizer==3.1.0
 click==8.1.3
 deprecated==1.2.13
 inquirerpy==0.3.4
 oauthlib==3.2.2
 plexapi==4.13.4
 prompt-toolkit==3.0.38
 pygments==2.15.1
 python-dotenv==0.21.1
 python-git-info==0.8.3
 pytimeparse==1.1.8
-pytrakt==3.4.22
+pytrakt==3.4.23
 pyyaml==6.0
 requests-cache==1.0.0b1
-requests==2.28.2
-rich==13.3.4
+requests==2.30.0
+rich==13.3.5
 tqdm==4.65.0
-urllib3==1.26.15
+urllib3==2.0.2
 wcwidth==0.2.6
 websocket-client==1.5.1
 
 [:python_version <= "3.7"]
 backports.cached-property==1.0.2
 
 [:python_version >= "3.4"]
@@ -35,11 +35,11 @@
 [:python_version >= "3.6"]
 url-normalize==1.4.3
 
 [:python_version >= "3.7"]
 cattrs==22.2.0
 markdown-it-py==2.2.0
 mdurl==0.1.2
-platformdirs==3.2.0
+platformdirs==3.5.0
 
 [:python_version >= "3.7" and python_version < "4.0"]
 pfzy==0.3.4
```

### Comparing `PlexTraktSync-0.26.4/README.md` & `PlexTraktSync-0.26.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,35 @@
 
 This project adds a two-way-sync between trakt.tv and Plex Media Server. It
 requires a trakt.tv account but no Plex premium and no Trakt VIP subscriptions,
 unlike the Plex app provided by Trakt.
 
 ![image](https://raw.githubusercontent.com/twolaw/PlexTraktSync/img/plextraktsync_banner.png)
 
-Originally created by [@Taxel][@taxel], but now maintained by [contributors].
+Originally created by [@Taxel][@taxel], now maintained by [contributors].
 
 [@taxel]: https://github.com/Taxel
 [contributors]: https://github.com/Taxel/PlexTraktSync/graphs/contributors
 
 Note: The PyTrakt API keys are not stored securely, so if you do not want to
 have a file containing those on your harddrive, you can not use this project.
 
-**Looking for a way to contribute? Please find issues with the [help-wanted]
-label or to improve documentation [docs-needed], thank you.**
+## Contribute
+
+**Looking for a way to contribute?**
+- find issues with the [help-wanted] label
+- improve documentation [docs-needed] label
+- you can also just [create a pull request] to improve documentation
+- ... more [developer contribution](CONTRIBUTING.md) docs
 
 [help-wanted]: https://github.com/Taxel/PlexTraktSync/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22
 [docs-needed]: https://github.com/Taxel/PlexTraktSync/issues?q=label%3A%22docs+needed%22+sort%3Aupdated-desc
+[create a pull request]: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
+
+----
 
 - [Plex-Trakt-Sync](#plex-trakt-sync)
   - [Features](#features)
   - [Pre-requisites](#pre-requisites)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [Docker Compose](#docker-compose)
@@ -301,14 +309,19 @@
 the "debug" variable in `config.yml` to `true`.
 
 By default the logs will append, if you wish to maintain the log of only your
 last run then edit the "append" variable in `config.yml` to `false`.
 
 ## Commands
 
+Run `plextraktsync --help` to see available commands.
+Run `plextraktsync COMMAND --help` to see help for `COMMAND`.
+
+You can [contribute](#contribute) yourself missing documentation.
+
 ### Sync
 
 The `sync` subcommand supports `--sync=shows` and `--sync=movies` options,
 so you can sync only specific library types.
 Or only watchlist: `--sync=watchlist`.
 
 ```
```

### Comparing `PlexTraktSync-0.26.4/plextraktsync/cli.py` & `PlexTraktSync-0.26.5/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/bug_report.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/cache.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/clear_collections.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/config.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/download.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/imdb_import.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/info.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/inspect.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/login.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/plex_login.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/self_update.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/sync.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/trakt_login.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/unmatched.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/watch.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/commands/watched_shows.py` & `PlexTraktSync-0.26.5/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/config/Config.py` & `PlexTraktSync-0.26.5/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/config/ConfigLoader.py` & `PlexTraktSync-0.26.5/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/config/HttpCacheConfig.py` & `PlexTraktSync-0.26.5/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/config/ServerConfig.py` & `PlexTraktSync-0.26.5/plextraktsync/config/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/config/SyncConfig.py` & `PlexTraktSync-0.26.5/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/config.default.yml` & `PlexTraktSync-0.26.5/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/decorators/rate_limit.py` & `PlexTraktSync-0.26.5/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/decorators/retry.py` & `PlexTraktSync-0.26.5/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/logger/filter.py` & `PlexTraktSync-0.26.5/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/media.py` & `PlexTraktSync-0.26.5/plextraktsync/media.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/mixin/ChangeNotifier.py` & `PlexTraktSync-0.26.5/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/plex/PlexApi.py` & `PlexTraktSync-0.26.5/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/plex/PlexAudioCodec.py` & `PlexTraktSync-0.26.5/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/plex/PlexGuid.py` & `PlexTraktSync-0.26.5/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/plex/PlexLibraryItem.py` & `PlexTraktSync-0.26.5/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/plex/PlexLibrarySection.py` & `PlexTraktSync-0.26.5/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/plex/PlexRatings.py` & `PlexTraktSync-0.26.5/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/plex/PlexServerConnection.py` & `PlexTraktSync-0.26.5/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/plex/PlexWatchList.py` & `PlexTraktSync-0.26.5/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/plex/SessionCollection.py` & `PlexTraktSync-0.26.5/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/pytrakt_extensions.py` & `PlexTraktSync-0.26.5/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/queue/BackgroundTask.py` & `PlexTraktSync-0.26.5/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/queue/Queue.py` & `PlexTraktSync-0.26.5/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/queue/TraktBatchWorker.py` & `PlexTraktSync-0.26.5/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/queue/TraktMarkWatchedWorker.py` & `PlexTraktSync-0.26.5/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/rich_addons.py` & `PlexTraktSync-0.26.5/plextraktsync/rich_addons.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/sync.py` & `PlexTraktSync-0.26.5/plextraktsync/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/trakt/ScrobblerCollection.py` & `PlexTraktSync-0.26.5/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/trakt/ScrobblerProxy.py` & `PlexTraktSync-0.26.5/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktApi.py` & `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktItem.py` & `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktLookup.py` & `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktRatingCollection.py` & `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/trakt/TraktWatchlist.py` & `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/trakt_list_util.py` & `PlexTraktSync-0.26.5/plextraktsync/trakt_list_util.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/util/Factory.py` & `PlexTraktSync-0.26.5/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/util/Path.py` & `PlexTraktSync-0.26.5/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/util/Timer.py` & `PlexTraktSync-0.26.5/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/util/Version.py` & `PlexTraktSync-0.26.5/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/util/expand_id.py` & `PlexTraktSync-0.26.5/plextraktsync/util/expand_id.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/util/local_url.py` & `PlexTraktSync-0.26.5/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/util/openurl.py` & `PlexTraktSync-0.26.5/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/util/packaging.py` & `PlexTraktSync-0.26.5/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/util/remove_empty_values.py` & `PlexTraktSync-0.26.5/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/walker.py` & `PlexTraktSync-0.26.5/plextraktsync/walker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/watch/EventDispatcher.py` & `PlexTraktSync-0.26.5/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/watch/EventFactory.py` & `PlexTraktSync-0.26.5/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/watch/ProgressBar.py` & `PlexTraktSync-0.26.5/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/watch/WatchStateUpdater.py` & `PlexTraktSync-0.26.5/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/watch/WebSocketListener.py` & `PlexTraktSync-0.26.5/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/plextraktsync/watch/events.py` & `PlexTraktSync-0.26.5/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/requirements.txt` & `PlexTraktSync-0.26.5/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 #
 #    pipenv lock --requirements
 #
 
 attrs==23.1.0
 backports.cached-property==1.0.2; python_version <= '3.7'
 cattrs==22.2.0; python_version >= '3.7'
-certifi==2022.12.7
+certifi==2023.5.7
 charset-normalizer==3.1.0
 click==8.1.3
 deprecated==1.2.13
 idna==3.4; python_version >= '3.5'
 inquirerpy==0.3.4
 markdown-it-py==2.2.0; python_version >= '3.7'
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
-platformdirs==3.2.0; python_version >= '3.7'
+platformdirs==3.5.0; python_version >= '3.7'
 plexapi==4.13.4
 prompt-toolkit==3.0.38
 pygments==2.15.1
 python-dotenv==0.21.1
 python-git-info==0.8.3
 pytimeparse==1.1.8
-pytrakt==3.4.22
+pytrakt==3.4.23
 pyyaml==6.0
 requests-cache==1.0.0b1
 requests-oauthlib==1.3.1; python_version >= '3.4'
-requests==2.28.2
-rich==13.3.4
+requests==2.30.0
+rich==13.3.5
 six==1.16.0; python_version >= '3.4'
 tqdm==4.65.0
 url-normalize==1.4.3; python_version >= '3.6'
-urllib3==1.26.15
+urllib3==2.0.2
 wcwidth==0.2.6
 websocket-client==1.5.1
 wrapt==1.15.0; python_version >= '3.5'
```

### Comparing `PlexTraktSync-0.26.4/setup.cfg` & `PlexTraktSync-0.26.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/tests/test_collection_metadata.py` & `PlexTraktSync-0.26.5/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/tests/test_config.py` & `PlexTraktSync-0.26.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/tests/test_events.py` & `PlexTraktSync-0.26.5/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/tests/test_new_agent.py` & `PlexTraktSync-0.26.5/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/tests/test_timer.py` & `PlexTraktSync-0.26.5/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/tests/test_trakt_progress.py` & `PlexTraktSync-0.26.5/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/tests/test_tv_lookup.py` & `PlexTraktSync-0.26.5/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.4/tests/test_walker.py` & `PlexTraktSync-0.26.5/tests/test_walker.py`

 * *Files identical despite different names*

