# Comparing `tmp/sleeper-1.5.0.tar.gz` & `tmp/sleeper-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleeper-1.5.0.tar", last modified: Sat Jan 28 18:47:26 2023, max compression
+gzip compressed data, was "sleeper-1.6.0.tar", last modified: Mon May 22 02:18:32 2023, max compression
```

## Comparing `sleeper-1.5.0.tar` & `sleeper-1.6.0.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:26.026277 sleeper-1.5.0/
--rw-rw-rw-   0        0        0     1088 2022-07-13 03:05:11.000000 sleeper-1.5.0/LICENSE
--rw-rw-rw-   0        0        0       56 2022-10-18 21:48:02.000000 sleeper-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1690 2023-01-28 18:47:26.025277 sleeper-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1269 2022-08-19 06:21:54.000000 sleeper-1.5.0/README.md
--rw-rw-rw-   0        0        0       72 2023-01-28 18:46:02.000000 sleeper-1.5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-28 18:47:26.026277 sleeper-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1064 2022-10-16 21:35:29.000000 sleeper-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.610420 sleeper-1.5.0/sleeper/
--rw-rw-rw-   0        0        0       43 2022-08-08 05:17:56.000000 sleeper-1.5.0/sleeper/__init__.py
--rw-rw-rw-   0        0        0       98 2023-01-28 18:46:02.000000 sleeper-1.5.0/sleeper/_version.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.665411 sleeper-1.5.0/sleeper/api/
--rw-rw-rw-   0        0        0      638 2022-09-12 20:49:11.000000 sleeper-1.5.0/sleeper/api/AvatarAPIClient.py
--rw-rw-rw-   0        0        0     2597 2022-07-24 18:50:13.000000 sleeper-1.5.0/sleeper/api/DraftAPIClient.py
--rw-rw-rw-   0        0        0     5332 2022-07-24 23:35:49.000000 sleeper-1.5.0/sleeper/api/LeagueAPIClient.py
--rw-rw-rw-   0        0        0     1571 2022-07-24 18:01:33.000000 sleeper-1.5.0/sleeper/api/PlayerAPIClient.py
--rw-rw-rw-   0        0        0     3457 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/api/SleeperAPIClient.py
--rw-rw-rw-   0        0        0      748 2022-07-21 20:25:55.000000 sleeper-1.5.0/sleeper/api/UserAPIClient.py
--rw-rw-rw-   0        0        0      224 2022-07-25 01:09:09.000000 sleeper-1.5.0/sleeper/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.689413 sleeper-1.5.0/sleeper/api/unofficial/
--rw-rw-rw-   0        0        0     5365 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/api/unofficial/UPlayerAPIClient.py
--rw-rw-rw-   0        0        0      879 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/api/unofficial/USportAPIClient.py
--rw-rw-rw-   0        0        0      758 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/api/unofficial/UTeamAPIClient.py
--rw-rw-rw-   0        0        0      138 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/api/unofficial/__init__.py
--rw-rw-rw-   0        0        0      732 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/app.properties
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.779276 sleeper-1.5.0/sleeper/enum/
--rw-rw-rw-   0        0        0      457 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/enum/Category.py
--rw-rw-rw-   0        0        0      492 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/enum/Company.py
--rw-rw-rw-   0        0        0      508 2022-07-21 20:56:05.000000 sleeper-1.5.0/sleeper/enum/DraftStatus.py
--rw-rw-rw-   0        0        0      575 2022-07-21 20:56:54.000000 sleeper-1.5.0/sleeper/enum/DraftType.py
--rw-rw-rw-   0        0        0     1191 2022-07-21 20:57:12.000000 sleeper-1.5.0/sleeper/enum/InjuryStatus.py
--rw-rw-rw-   0        0        0      426 2022-07-21 21:14:52.000000 sleeper-1.5.0/sleeper/enum/ModelEnum.py
--rw-rw-rw-   0        0        0      662 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/enum/PlayerPosition.py
--rw-rw-rw-   0        0        0      665 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/enum/PlayerStatus.py
--rw-rw-rw-   0        0        0      883 2022-09-07 17:01:51.000000 sleeper-1.5.0/sleeper/enum/PlayoffRoundType.py
--rw-rw-rw-   0        0        0      541 2022-07-21 20:57:58.000000 sleeper-1.5.0/sleeper/enum/PracticeParticipation.py
--rw-rw-rw-   0        0        0      679 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/enum/RosterPosition.py
--rw-rw-rw-   0        0        0     1011 2022-07-21 20:59:05.000000 sleeper-1.5.0/sleeper/enum/ScoringType.py
--rw-rw-rw-   0        0        0      965 2022-12-22 19:05:39.000000 sleeper-1.5.0/sleeper/enum/SeasonStatus.py
--rw-rw-rw-   0        0        0      651 2022-07-21 21:00:07.000000 sleeper-1.5.0/sleeper/enum/SeasonType.py
--rw-rw-rw-   0        0        0      515 2022-07-21 21:00:07.000000 sleeper-1.5.0/sleeper/enum/Sport.py
--rw-rw-rw-   0        0        0      626 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/enum/SportTeam.py
--rw-rw-rw-   0        0        0      526 2022-07-21 21:00:07.000000 sleeper-1.5.0/sleeper/enum/TransactionStatus.py
--rw-rw-rw-   0        0        0      623 2022-07-21 21:00:07.000000 sleeper-1.5.0/sleeper/enum/TransactionType.py
--rw-rw-rw-   0        0        0      458 2022-07-21 21:00:07.000000 sleeper-1.5.0/sleeper/enum/TrendType.py
--rw-rw-rw-   0        0        0      746 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/enum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.801277 sleeper-1.5.0/sleeper/enum/nfl/
--rw-rw-rw-   0        0        0     1318 2022-07-21 21:08:59.000000 sleeper-1.5.0/sleeper/enum/nfl/NFLPlayerStatus.py
--rw-rw-rw-   0        0        0     2883 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/enum/nfl/NFLPosition.py
--rw-rw-rw-   0        0        0     1149 2022-07-24 19:42:01.000000 sleeper-1.5.0/sleeper/enum/nfl/NFLRosterPosition.py
--rw-rw-rw-   0        0        0     3156 2022-07-21 21:10:07.000000 sleeper-1.5.0/sleeper/enum/nfl/NFLTeam.py
--rw-rw-rw-   0        0        0      164 2022-07-25 00:54:52.000000 sleeper-1.5.0/sleeper/enum/nfl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.806275 sleeper-1.5.0/sleeper/exception/
--rw-rw-rw-   0        0        0      123 2022-07-23 01:05:59.000000 sleeper-1.5.0/sleeper/exception/SleeperAPIException.py
--rw-rw-rw-   0        0        0       54 2022-07-25 00:57:06.000000 sleeper-1.5.0/sleeper/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.937276 sleeper-1.5.0/sleeper/model/
--rw-rw-rw-   0        0        0      664 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/DepthChart.py
--rw-rw-rw-   0        0        0     2312 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/Draft.py
--rw-rw-rw-   0        0        0      586 2022-07-20 22:28:26.000000 sleeper-1.5.0/sleeper/model/DraftMetadata.py
--rw-rw-rw-   0        0        0     1014 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/DraftPick.py
--rw-rw-rw-   0        0        0     1865 2022-07-20 22:30:57.000000 sleeper-1.5.0/sleeper/model/DraftSettings.py
--rw-rw-rw-   0        0        0      830 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/FAABTransaction.py
--rw-rw-rw-   0        0        0      579 2022-07-20 22:32:15.000000 sleeper-1.5.0/sleeper/model/FromPlayoffMatchup.py
--rw-rw-rw-   0        0        0     1148 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/Game.py
--rw-rw-rw-   0        0        0     2162 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/League.py
--rw-rw-rw-   0        0        0     5093 2022-09-07 17:01:51.000000 sleeper-1.5.0/sleeper/model/LeagueSettings.py
--rw-rw-rw-   0        0        0     1298 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/Matchup.py
--rw-rw-rw-   0        0        0     5601 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/Player.py
--rw-rw-rw-   0        0        0     1744 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/PlayerDraftPick.py
--rw-rw-rw-   0        0        0     1993 2022-07-21 21:04:01.000000 sleeper-1.5.0/sleeper/model/PlayerDraftPickMetadata.py
--rw-rw-rw-   0        0        0     2279 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/PlayerStats.py
--rw-rw-rw-   0        0        0      673 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/PlayerTrend.py
--rw-rw-rw-   0        0        0     1640 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/PlayoffMatchup.py
--rw-rw-rw-   0        0        0     1550 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/Roster.py
--rw-rw-rw-   0        0        0     1577 2022-07-24 21:44:13.000000 sleeper-1.5.0/sleeper/model/RosterSettings.py
--rw-rw-rw-   0        0        0    10573 2022-07-20 23:01:10.000000 sleeper-1.5.0/sleeper/model/ScoringSettings.py
--rw-rw-rw-   0        0        0     1377 2022-07-25 04:44:17.000000 sleeper-1.5.0/sleeper/model/SportState.py
--rw-rw-rw-   0        0        0      707 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/Stats.py
--rw-rw-rw-   0        0        0      945 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/TradedPick.py
--rw-rw-rw-   0        0        0     2465 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/Transaction.py
--rw-rw-rw-   0        0        0      558 2022-07-20 23:06:23.000000 sleeper-1.5.0/sleeper/model/TransactionSettings.py
--rw-rw-rw-   0        0        0     2431 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/User.py
--rw-rw-rw-   0        0        0      966 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.950277 sleeper-1.5.0/sleeper/model/nfl/
--rw-rw-rw-   0        0        0     1965 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/nfl/NFLDepthChart.py
--rw-rw-rw-   0        0        0    17494 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/nfl/NFLStats.py
--rw-rw-rw-   0        0        0       74 2022-09-16 18:00:32.000000 sleeper-1.5.0/sleeper/model/nfl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.959275 sleeper-1.5.0/sleeper/util/
--rw-rw-rw-   0        0        0      818 2022-07-13 03:32:47.000000 sleeper-1.5.0/sleeper/util/ConfigReader.py
--rw-rw-rw-   0        0        0     1113 2022-07-21 21:13:09.000000 sleeper-1.5.0/sleeper/util/CustomFormatter.py
--rw-rw-rw-   0        0        0      859 2022-07-21 21:18:04.000000 sleeper-1.5.0/sleeper/util/CustomLogger.py
--rw-rw-rw-   0        0        0        0 2022-07-21 03:34:50.000000 sleeper-1.5.0/sleeper/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.634413 sleeper-1.5.0/sleeper.egg-info/
--rw-rw-rw-   0        0        0     1690 2023-01-28 18:47:25.000000 sleeper-1.5.0/sleeper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2853 2023-01-28 18:47:25.000000 sleeper-1.5.0/sleeper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-28 18:47:25.000000 sleeper-1.5.0/sleeper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-01-28 18:47:25.000000 sleeper-1.5.0/sleeper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-28 18:47:25.000000 sleeper-1.5.0/sleeper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.595414 sleeper-1.5.0/test/
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:25.998277 sleeper-1.5.0/test/test_api/
--rw-rw-rw-   0        0        0        0 2022-07-21 03:00:23.000000 sleeper-1.5.0/test/test_api/__init__.py
--rw-rw-rw-   0        0        0     3257 2022-09-16 18:00:32.000000 sleeper-1.5.0/test/test_api/test_AvatarAPIClient.py
--rw-rw-rw-   0        0        0    22121 2022-08-10 06:16:52.000000 sleeper-1.5.0/test/test_api/test_DraftAPIClient.py
--rw-rw-rw-   0        0        0    62353 2022-09-07 17:01:51.000000 sleeper-1.5.0/test/test_api/test_LeagueAPIClient.py
--rw-rw-rw-   0        0        0    11017 2022-08-10 06:20:20.000000 sleeper-1.5.0/test/test_api/test_PlayerAPIClient.py
--rw-rw-rw-   0        0        0     3548 2022-08-10 06:20:44.000000 sleeper-1.5.0/test/test_api/test_UserAPIClient.py
-drwxrwxrwx   0        0        0        0 2023-01-28 18:47:26.023277 sleeper-1.5.0/test/test_api/test_unofficial/
--rw-rw-rw-   0        0        0        0 2022-09-16 18:00:32.000000 sleeper-1.5.0/test/test_api/test_unofficial/__init__.py
--rw-rw-rw-   0        0        0    17071 2022-09-16 18:00:32.000000 sleeper-1.5.0/test/test_api/test_unofficial/test_UPlayerAPIClient.py
--rw-rw-rw-   0        0        0     1461 2022-09-16 18:00:32.000000 sleeper-1.5.0/test/test_api/test_unofficial/test_USportAPIClient.py
--rw-rw-rw-   0        0        0     6661 2022-09-16 18:00:32.000000 sleeper-1.5.0/test/test_api/test_unofficial/test_UTeamAPIClient.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.704865 sleeper-1.6.0/
+-rw-rw-rw-   0        0        0     1088 2022-07-13 03:05:11.000000 sleeper-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0       56 2022-10-18 21:48:02.000000 sleeper-1.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1857 2023-05-22 02:18:32.703867 sleeper-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1436 2023-05-22 02:17:04.000000 sleeper-1.6.0/README.md
+-rw-rw-rw-   0        0        0      203 2023-05-22 02:17:04.000000 sleeper-1.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       72 2023-01-28 18:46:02.000000 sleeper-1.6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 02:18:32.704865 sleeper-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2023-05-22 02:17:04.000000 sleeper-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.488866 sleeper-1.6.0/sleeper/
+-rw-rw-rw-   0        0        0       43 2022-08-08 05:17:56.000000 sleeper-1.6.0/sleeper/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-05-22 02:17:08.000000 sleeper-1.6.0/sleeper/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.520865 sleeper-1.6.0/sleeper/api/
+-rw-rw-rw-   0        0        0      632 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/api/AvatarAPIClient.py
+-rw-rw-rw-   0        0        0     2823 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/api/DraftAPIClient.py
+-rw-rw-rw-   0        0        0     5703 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/api/LeagueAPIClient.py
+-rw-rw-rw-   0        0        0     1669 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/api/PlayerAPIClient.py
+-rw-rw-rw-   0        0        0     3459 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/api/SleeperAPIClient.py
+-rw-rw-rw-   0        0        0      770 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/api/UserAPIClient.py
+-rw-rw-rw-   0        0        0      224 2022-07-25 01:09:09.000000 sleeper-1.6.0/sleeper/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.529866 sleeper-1.6.0/sleeper/api/unofficial/
+-rw-rw-rw-   0        0        0     5731 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/api/unofficial/UPlayerAPIClient.py
+-rw-rw-rw-   0        0        0      949 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/api/unofficial/USportAPIClient.py
+-rw-rw-rw-   0        0        0      846 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/api/unofficial/UTeamAPIClient.py
+-rw-rw-rw-   0        0        0      138 2022-09-16 18:00:32.000000 sleeper-1.6.0/sleeper/api/unofficial/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-09-16 18:00:32.000000 sleeper-1.6.0/sleeper/app.properties
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.576868 sleeper-1.6.0/sleeper/enum/
+-rw-rw-rw-   0        0        0      457 2022-09-16 18:00:32.000000 sleeper-1.6.0/sleeper/enum/Category.py
+-rw-rw-rw-   0        0        0      492 2022-09-16 18:00:32.000000 sleeper-1.6.0/sleeper/enum/Company.py
+-rw-rw-rw-   0        0        0      508 2022-07-21 20:56:05.000000 sleeper-1.6.0/sleeper/enum/DraftStatus.py
+-rw-rw-rw-   0        0        0      575 2022-07-21 20:56:54.000000 sleeper-1.6.0/sleeper/enum/DraftType.py
+-rw-rw-rw-   0        0        0     1191 2022-07-21 20:57:12.000000 sleeper-1.6.0/sleeper/enum/InjuryStatus.py
+-rw-rw-rw-   0        0        0      428 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/enum/ModelEnum.py
+-rw-rw-rw-   0        0        0      666 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/enum/PlayerPosition.py
+-rw-rw-rw-   0        0        0      669 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/enum/PlayerStatus.py
+-rw-rw-rw-   0        0        0      883 2022-09-07 17:01:51.000000 sleeper-1.6.0/sleeper/enum/PlayoffRoundType.py
+-rw-rw-rw-   0        0        0      541 2022-07-21 20:57:58.000000 sleeper-1.6.0/sleeper/enum/PracticeParticipation.py
+-rw-rw-rw-   0        0        0      681 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/enum/RosterPosition.py
+-rw-rw-rw-   0        0        0     1011 2022-07-21 20:59:05.000000 sleeper-1.6.0/sleeper/enum/ScoringType.py
+-rw-rw-rw-   0        0        0      965 2022-12-22 19:05:39.000000 sleeper-1.6.0/sleeper/enum/SeasonStatus.py
+-rw-rw-rw-   0        0        0      651 2022-07-21 21:00:07.000000 sleeper-1.6.0/sleeper/enum/SeasonType.py
+-rw-rw-rw-   0        0        0      515 2022-07-21 21:00:07.000000 sleeper-1.6.0/sleeper/enum/Sport.py
+-rw-rw-rw-   0        0        0      630 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/enum/SportTeam.py
+-rw-rw-rw-   0        0        0      526 2022-07-21 21:00:07.000000 sleeper-1.6.0/sleeper/enum/TransactionStatus.py
+-rw-rw-rw-   0        0        0      623 2022-07-21 21:00:07.000000 sleeper-1.6.0/sleeper/enum/TransactionType.py
+-rw-rw-rw-   0        0        0      458 2022-07-21 21:00:07.000000 sleeper-1.6.0/sleeper/enum/TrendType.py
+-rw-rw-rw-   0        0        0      746 2022-09-16 18:00:32.000000 sleeper-1.6.0/sleeper/enum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.587864 sleeper-1.6.0/sleeper/enum/nfl/
+-rw-rw-rw-   0        0        0     1318 2022-07-21 21:08:59.000000 sleeper-1.6.0/sleeper/enum/nfl/NFLPlayerStatus.py
+-rw-rw-rw-   0        0        0     2883 2022-09-16 18:00:32.000000 sleeper-1.6.0/sleeper/enum/nfl/NFLPosition.py
+-rw-rw-rw-   0        0        0     1149 2022-07-24 19:42:01.000000 sleeper-1.6.0/sleeper/enum/nfl/NFLRosterPosition.py
+-rw-rw-rw-   0        0        0     3156 2022-07-21 21:10:07.000000 sleeper-1.6.0/sleeper/enum/nfl/NFLTeam.py
+-rw-rw-rw-   0        0        0      164 2022-07-25 00:54:52.000000 sleeper-1.6.0/sleeper/enum/nfl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.592865 sleeper-1.6.0/sleeper/exception/
+-rw-rw-rw-   0        0        0      125 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/exception/SleeperAPIException.py
+-rw-rw-rw-   0        0        0       54 2022-07-25 00:57:06.000000 sleeper-1.6.0/sleeper/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.660864 sleeper-1.6.0/sleeper/model/
+-rw-rw-rw-   0        0        0      668 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/DepthChart.py
+-rw-rw-rw-   0        0        0     2193 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/Draft.py
+-rw-rw-rw-   0        0        0      577 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/DraftMetadata.py
+-rw-rw-rw-   0        0        0      974 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/DraftPick.py
+-rw-rw-rw-   0        0        0     1635 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/DraftSettings.py
+-rw-rw-rw-   0        0        0      817 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/FAABTransaction.py
+-rw-rw-rw-   0        0        0      582 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/FromPlayoffMatchup.py
+-rw-rw-rw-   0        0        0     1106 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/Game.py
+-rw-rw-rw-   0        0        0     2376 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/League.py
+-rw-rw-rw-   0        0        0     2087 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/LeagueMetadata.py
+-rw-rw-rw-   0        0        0     4433 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/LeagueSettings.py
+-rw-rw-rw-   0        0        0     1246 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/Matchup.py
+-rw-rw-rw-   0        0        0     5250 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/Player.py
+-rw-rw-rw-   0        0        0     1574 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/PlayerDraftPick.py
+-rw-rw-rw-   0        0        0     1704 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/PlayerDraftPickMetadata.py
+-rw-rw-rw-   0        0        0     2135 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/PlayerStats.py
+-rw-rw-rw-   0        0        0      669 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/PlayerTrend.py
+-rw-rw-rw-   0        0        0     1521 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/PlayoffMatchup.py
+-rw-rw-rw-   0        0        0     1475 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/Roster.py
+-rw-rw-rw-   0        0        0     1465 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/RosterSettings.py
+-rw-rw-rw-   0        0        0     8755 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/ScoringSettings.py
+-rw-rw-rw-   0        0        0     1360 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/SportState.py
+-rw-rw-rw-   0        0        0      707 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/Stats.py
+-rw-rw-rw-   0        0        0      914 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/TradedPick.py
+-rw-rw-rw-   0        0        0     2280 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/Transaction.py
+-rw-rw-rw-   0        0        0      560 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/TransactionSettings.py
+-rw-rw-rw-   0        0        0     2288 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/User.py
+-rw-rw-rw-   0        0        0      966 2022-09-16 18:00:32.000000 sleeper-1.6.0/sleeper/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.667869 sleeper-1.6.0/sleeper/model/nfl/
+-rw-rw-rw-   0        0        0     1966 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/nfl/NFLDepthChart.py
+-rw-rw-rw-   0        0        0    15287 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/model/nfl/NFLStats.py
+-rw-rw-rw-   0        0        0       74 2022-09-16 18:00:32.000000 sleeper-1.6.0/sleeper/model/nfl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.676871 sleeper-1.6.0/sleeper/util/
+-rw-rw-rw-   0        0        0      886 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/util/ConfigReader.py
+-rw-rw-rw-   0        0        0     1114 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/util/CustomFormatter.py
+-rw-rw-rw-   0        0        0      889 2023-05-22 02:17:04.000000 sleeper-1.6.0/sleeper/util/CustomLogger.py
+-rw-rw-rw-   0        0        0        0 2022-07-21 03:34:50.000000 sleeper-1.6.0/sleeper/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.504866 sleeper-1.6.0/sleeper.egg-info/
+-rw-rw-rw-   0        0        0     1857 2023-05-22 02:18:32.000000 sleeper-1.6.0/sleeper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2900 2023-05-22 02:18:32.000000 sleeper-1.6.0/sleeper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 02:18:32.000000 sleeper-1.6.0/sleeper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-22 02:18:32.000000 sleeper-1.6.0/sleeper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-22 02:18:32.000000 sleeper-1.6.0/sleeper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.466866 sleeper-1.6.0/test/
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.689866 sleeper-1.6.0/test/test_api/
+-rw-rw-rw-   0        0        0        0 2022-07-21 03:00:23.000000 sleeper-1.6.0/test/test_api/__init__.py
+-rw-rw-rw-   0        0        0     3305 2023-05-22 02:17:04.000000 sleeper-1.6.0/test/test_api/test_AvatarAPIClient.py
+-rw-rw-rw-   0        0        0    21970 2023-05-22 02:17:04.000000 sleeper-1.6.0/test/test_api/test_DraftAPIClient.py
+-rw-rw-rw-   0        0        0    61057 2023-05-22 02:17:04.000000 sleeper-1.6.0/test/test_api/test_LeagueAPIClient.py
+-rw-rw-rw-   0        0        0    10505 2023-05-22 02:17:04.000000 sleeper-1.6.0/test/test_api/test_PlayerAPIClient.py
+-rw-rw-rw-   0        0        0     3571 2023-05-22 02:17:04.000000 sleeper-1.6.0/test/test_api/test_UserAPIClient.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:18:32.700865 sleeper-1.6.0/test/test_api/test_unofficial/
+-rw-rw-rw-   0        0        0        0 2022-09-16 18:00:32.000000 sleeper-1.6.0/test/test_api/test_unofficial/__init__.py
+-rw-rw-rw-   0        0        0    16591 2023-05-22 02:17:04.000000 sleeper-1.6.0/test/test_api/test_unofficial/test_UPlayerAPIClient.py
+-rw-rw-rw-   0        0        0     1470 2023-05-22 02:17:04.000000 sleeper-1.6.0/test/test_api/test_unofficial/test_USportAPIClient.py
+-rw-rw-rw-   0        0        0     5416 2023-05-22 02:17:04.000000 sleeper-1.6.0/test/test_api/test_unofficial/test_UTeamAPIClient.py
```

### Comparing `sleeper-1.5.0/LICENSE` & `sleeper-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/PKG-INFO` & `sleeper-1.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleeper
-Version: 1.5.0
+Version: 1.6.0
 Summary: A Python wrapper for the Sleeper API.
 Home-page: https://github.com/joeyagreco/sleeper
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: nfl football sleeper sleeper-api sleeper-fantasy-football fantasy-football wrapper wrapper-api
 Requires-Python: >=3.10
@@ -48,10 +48,17 @@
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
+## Development
+
+_Run these commands from the root folder_
+- Format Code: `./main fmt`
+- Run Unit Tests: `./main test`
+- Generate Coverage Report: `./main cov`
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `sleeper-1.5.0/README.md` & `sleeper-1.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -35,10 +35,17 @@
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
+## Development
+
+_Run these commands from the root folder_
+- Format Code: `./main fmt`
+- Run Unit Tests: `./main test`
+- Generate Coverage Report: `./main cov`
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `sleeper-1.5.0/setup.py` & `sleeper-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,9 +23,9 @@
     long_description=read_me,
     license="MIT",
     url="https://github.com/joeyagreco/sleeper",
     include_package_data=True,
     packages=setuptools.find_packages(exclude=("test", "docs")),
     install_requires=required_packages,
     python_requires=f">={minimum_python_version_required}",
-    keywords="nfl football sleeper sleeper-api sleeper-fantasy-football fantasy-football wrapper wrapper-api"
+    keywords="nfl football sleeper sleeper-api sleeper-fantasy-football fantasy-football wrapper wrapper-api",
 )
```

### Comparing `sleeper-1.5.0/sleeper/api/AvatarAPIClient.py` & `sleeper-1.6.0/sleeper/api/AvatarAPIClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sleeper.api.SleeperAPIClient import SleeperAPIClient
 
 
 class AvatarAPIClient(SleeperAPIClient):
-
     @classmethod
     def get_avatar(cls, *, avatar_id: str, save_to_path: str, **kwargs) -> None:
         thumbnail = kwargs.pop("thumbnail", False)
         if thumbnail:
-            url = cls._build_route(cls._SLEEPER_CDN_BASE_URL, None, cls._AVATARS_ROUTE, cls._THUMBS_ROUTE,
-                                   avatar_id)
+            url = cls._build_route(
+                cls._SLEEPER_CDN_BASE_URL, None, cls._AVATARS_ROUTE, cls._THUMBS_ROUTE, avatar_id
+            )
         else:
             url = cls._build_route(cls._SLEEPER_CDN_BASE_URL, None, cls._AVATARS_ROUTE, avatar_id)
         image_file = cls._get_image_file(url)
         image_file.save(save_to_path)
```

### Comparing `sleeper-1.5.0/sleeper/api/DraftAPIClient.py` & `sleeper-1.6.0/sleeper/api/DraftAPIClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,37 @@
 from sleeper.enum.Sport import Sport
 from sleeper.model.Draft import Draft
 from sleeper.model.DraftPick import DraftPick
 from sleeper.model.PlayerDraftPick import PlayerDraftPick
 
 
 class DraftAPIClient(SleeperAPIClient):
-
     @classmethod
     def get_user_drafts_for_year(cls, *, user_id: str, sport: Sport, year: str) -> list[Draft]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._USER_ROUTE, user_id, cls._DRAFTS_ROUTE,
-                               sport.name.lower(), year)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._USER_ROUTE,
+            user_id,
+            cls._DRAFTS_ROUTE,
+            sport.name.lower(),
+            year,
+        )
         response_list = cls._get(url)
         if response_list is None:
-            raise ValueError(f"Could not get Drafts for user_id '{user_id}', sport '{sport.name}', and year '{year}'.")
+            raise ValueError(
+                f"Could not get Drafts for user_id '{user_id}', sport '{sport.name}', and year '{year}'."
+            )
         return Draft.from_dict_list(response_list)
 
     @classmethod
     def get_drafts_in_league(cls, *, league_id: str) -> list[Draft]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id, cls._DRAFTS_ROUTE)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id, cls._DRAFTS_ROUTE
+        )
         response_list = cls._get(url)
         if response_list is None:
             raise ValueError(f"Could not get Drafts for league_id '{league_id}'.")
         return Draft.from_dict_list(cls._get(url))
 
     @classmethod
     def get_draft(cls, *, draft_id: str) -> Draft:
@@ -30,21 +40,30 @@
         response_dict = cls._get(url)
         if response_dict is None:
             raise ValueError(f"Could not get Draft with draft_id '{draft_id}'.")
         return Draft.from_dict(cls._get(url))
 
     @classmethod
     def get_player_draft_picks(cls, *, draft_id: str, sport: Sport) -> list[PlayerDraftPick]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._DRAFT_ROUTE, draft_id, cls._PICKS_ROUTE)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._DRAFT_ROUTE, draft_id, cls._PICKS_ROUTE
+        )
         response_list = cls._get(url)
         if response_list is None:
-            raise ValueError(f"Could not get PlayerDraftPicks with draft_id '{draft_id}' and sport '{sport.name}'.")
+            raise ValueError(
+                f"Could not get PlayerDraftPicks with draft_id '{draft_id}' and sport '{sport.name}'."
+            )
         return PlayerDraftPick.from_dict_list(cls._get(url), sport)
 
     @classmethod
     def get_traded_draft_picks(cls, *, draft_id: str) -> list[DraftPick]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._DRAFT_ROUTE, draft_id,
-                               cls._TRADED_PICKS_ROUTE)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._DRAFT_ROUTE,
+            draft_id,
+            cls._TRADED_PICKS_ROUTE,
+        )
         response_list = cls._get(url)
         if response_list is None:
             raise ValueError(f"Could not get traded DraftPicks with draft_id '{draft_id}'.")
         return DraftPick.from_dict_list(cls._get(url))
```

### Comparing `sleeper-1.5.0/sleeper/api/LeagueAPIClient.py` & `sleeper-1.6.0/sleeper/api/LeagueAPIClient.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,103 +7,144 @@
 from sleeper.model.SportState import SportState
 from sleeper.model.TradedPick import TradedPick
 from sleeper.model.Transaction import Transaction
 from sleeper.model.User import User
 
 
 class LeagueAPIClient(SleeperAPIClient):
-
     @classmethod
     def get_league(cls, *, league_id: str) -> League:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id
+        )
         response_dict = cls._get(url)
         if response_dict is None:
             raise ValueError(f"Could not get League with league_id '{league_id}'.")
         return League.from_dict(response_dict)
 
     @classmethod
     def get_user_leagues_for_year(cls, *, user_id: str, sport: Sport, year: str) -> list[League]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._USER_ROUTE, user_id, cls._LEAGUES_ROUTE,
-                               sport.value.lower(), year)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._USER_ROUTE,
+            user_id,
+            cls._LEAGUES_ROUTE,
+            sport.value.lower(),
+            year,
+        )
         response_list = cls._get(url)
         if response_list is None:
             raise ValueError(
-                f"Could not get user Leagues for user_id '{user_id}', sport '{sport.name}', and year '{year}'.")
+                f"Could not get user Leagues for user_id '{user_id}', sport '{sport.name}', and year '{year}'."
+            )
         return League.from_dict_list(response_list)
 
     @classmethod
     def get_rosters(cls, *, league_id: str) -> list[Roster]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id,
-                               cls._ROSTERS_ROUTE)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._LEAGUE_ROUTE,
+            league_id,
+            cls._ROSTERS_ROUTE,
+        )
         response_list = cls._get(url)
         if response_list is None:
-            raise ValueError(
-                f"Could not get Rosters for league_id '{league_id}'.")
+            raise ValueError(f"Could not get Rosters for league_id '{league_id}'.")
         return Roster.from_dict_list(response_list)
 
     @classmethod
     def get_users_in_league(cls, *, league_id: str) -> list[User]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id, cls._USERS_ROUTE)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id, cls._USERS_ROUTE
+        )
         response_list = cls._get(url)
         if response_list is None:
-            raise ValueError(
-                f"Could not get Users for league_id '{league_id}'.")
+            raise ValueError(f"Could not get Users for league_id '{league_id}'.")
         return User.from_dict_list(response_list)
 
     @classmethod
     def get_matchups_for_week(cls, *, league_id: str, week: int) -> list[Matchup]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id,
-                               cls._MATCHUPS_ROUTE, week)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._LEAGUE_ROUTE,
+            league_id,
+            cls._MATCHUPS_ROUTE,
+            week,
+        )
         response_list = cls._get(url)
         if response_list is None:
             raise ValueError(
-                f"Could not get Matchups for league_id '{league_id}' and week '{week}'.")
+                f"Could not get Matchups for league_id '{league_id}' and week '{week}'."
+            )
         return Matchup.from_dict_list(response_list)
 
     @classmethod
     def get_winners_bracket(cls, *, league_id: str) -> list[PlayoffMatchup]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id,
-                               cls._WINNERS_BRACKET_ROUTE)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._LEAGUE_ROUTE,
+            league_id,
+            cls._WINNERS_BRACKET_ROUTE,
+        )
         response_list = cls._get(url)
         if response_list is None:
-            raise ValueError(
-                f"Could not get PlayoffMatchups for league_id '{league_id}'.")
+            raise ValueError(f"Could not get PlayoffMatchups for league_id '{league_id}'.")
         return PlayoffMatchup.from_dict_str(response_list)
 
     @classmethod
     def get_losers_bracket(cls, *, league_id: str) -> list[PlayoffMatchup]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id,
-                               cls._LOSERS_BRACKET_ROUTE)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._LEAGUE_ROUTE,
+            league_id,
+            cls._LOSERS_BRACKET_ROUTE,
+        )
         response_list = cls._get(url)
         if response_list is None:
-            raise ValueError(
-                f"Could not get PlayoffMatchups for league_id '{league_id}'.")
+            raise ValueError(f"Could not get PlayoffMatchups for league_id '{league_id}'.")
         return PlayoffMatchup.from_dict_str(response_list)
 
     @classmethod
     def get_transactions(cls, *, league_id: str, week: int) -> list[Transaction]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id,
-                               cls._TRANSACTIONS_ROUTE, week)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._LEAGUE_ROUTE,
+            league_id,
+            cls._TRANSACTIONS_ROUTE,
+            week,
+        )
         response_list = cls._get(url)
         if response_list is None:
             raise ValueError(
-                f"Could not get Transactions for league_id '{league_id}' and week '{week}'.")
+                f"Could not get Transactions for league_id '{league_id}' and week '{week}'."
+            )
         return Transaction.from_dict_list(response_list)
 
     @classmethod
     def get_traded_picks(cls, *, league_id: str) -> list[TradedPick]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._LEAGUE_ROUTE, league_id,
-                               cls._TRADED_PICKS_ROUTE)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._LEAGUE_ROUTE,
+            league_id,
+            cls._TRADED_PICKS_ROUTE,
+        )
         response_list = cls._get(url)
         if response_list is None:
-            raise ValueError(
-                f"Could not get TradedPicks for league_id '{league_id}'.")
+            raise ValueError(f"Could not get TradedPicks for league_id '{league_id}'.")
         return TradedPick.from_dict_list(response_list)
 
     @classmethod
     def get_sport_state(cls, *, sport: Sport) -> SportState:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._STATE_ROUTE, sport.value.lower())
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._STATE_ROUTE, sport.value.lower()
+        )
         response_dict = cls._get(url)
         if response_dict is None:
-            raise ValueError(
-                f"Could not get SportState for sport '{sport.name}'.")
+            raise ValueError(f"Could not get SportState for sport '{sport.name}'.")
         return SportState.from_dict(response_dict)
```

### Comparing `sleeper-1.5.0/sleeper/api/PlayerAPIClient.py` & `sleeper-1.6.0/sleeper/api/PlayerAPIClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,34 @@
 
 class PlayerAPIClient(SleeperAPIClient):
     __DEFAULT_TRENDING_PLAYERS_LOOKBACK_HOURS = 24
     __DEFAULT_TRENDING_PLAYERS_LIMIT = 25
 
     @classmethod
     def get_all_players(cls, *, sport: Sport) -> dict[str, Player]:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._PLAYERS_ROUTE, sport.name.lower())
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._PLAYERS_ROUTE, sport.name.lower()
+        )
         response_dict = cls._get(url)
         if response_dict is None:
             raise ValueError(f"Could not get Players for sport: '{sport.name}'.")
         return Player.dict_by_id(response_dict, sport)
 
     @classmethod
-    def get_trending_players(cls, *, sport: Sport, trend_type: TrendType, **kwargs) -> list[PlayerTrend]:
+    def get_trending_players(
+        cls, *, sport: Sport, trend_type: TrendType, **kwargs
+    ) -> list[PlayerTrend]:
         lookback_hours = kwargs.pop("lookback_hours", cls.__DEFAULT_TRENDING_PLAYERS_LOOKBACK_HOURS)
         limit = kwargs.pop("limit", cls.__DEFAULT_TRENDING_PLAYERS_LIMIT)
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._PLAYERS_ROUTE, sport.name.lower(),
-                               cls._TRENDING_ROUTE, trend_type.name.lower())
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            cls._VERSION,
+            cls._PLAYERS_ROUTE,
+            sport.name.lower(),
+            cls._TRENDING_ROUTE,
+            trend_type.name.lower(),
+        )
         url = cls._add_filters(url, ("lookback_hours", lookback_hours), ("limit", limit))
         response_dict = cls._get(url)
         if response_dict is None:
             raise ValueError(f"Could not get PlayerTrends.")
         return PlayerTrend.from_dict_list(response_dict)
```

### Comparing `sleeper-1.5.0/sleeper/api/SleeperAPIClient.py` & `sleeper-1.6.0/sleeper/api/SleeperAPIClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class SleeperAPIClient(ABC):
     """
     Should be inherited by all API Clients.
 
     Sleeper API Documentation: https://docs.sleeper.app/
     """
+
     _SLEEPER_APP_BASE_URL = ConfigReader.get("api", "sleeper_app_base_url")
     _SLEEPER_CDN_BASE_URL = ConfigReader.get("api", "sleeper_cdn_base_url")
     _VERSION = ConfigReader.get("api", "version")
 
     # ROUTES
     _AVATARS_ROUTE = ConfigReader.get("api", "avatars_route")
     _CONTENT_ROUTE = ConfigReader.get("api", "content_route")
```

### Comparing `sleeper-1.5.0/sleeper/api/UserAPIClient.py` & `sleeper-1.6.0/sleeper/api/UserAPIClient.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from sleeper.api.SleeperAPIClient import SleeperAPIClient
 from sleeper.model.User import User
 
 
 class UserAPIClient(SleeperAPIClient):
-
     @classmethod
     def get_user(cls, *, username: str = None, user_id: str = None) -> User:
         if username is None and user_id is None:
             raise ValueError("'username' and 'user_id' cannot both be None.")
         user_arg = username if username is not None else user_id
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._USER_ROUTE, f"{user_arg}")
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL, cls._VERSION, cls._USER_ROUTE, f"{user_arg}"
+        )
         response_dict = cls._get(url)
         if response_dict is None:
             raise ValueError(f"Could not find User for username/user_id: '{user_arg}'.")
         return User.from_dict(response_dict)
```

### Comparing `sleeper-1.5.0/sleeper/api/unofficial/UPlayerAPIClient.py` & `sleeper-1.6.0/sleeper/api/unofficial/UPlayerAPIClient.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,63 +3,86 @@
 from sleeper.api.SleeperAPIClient import SleeperAPIClient
 from sleeper.enum import SeasonType, PlayerPosition
 from sleeper.enum.Sport import Sport
 from sleeper.model.PlayerStats import PlayerStats
 
 
 class UPlayerAPIClient(SleeperAPIClient):
-
     @classmethod
-    def get_player_stats(cls, *, sport: Sport, player_id: str, season: str, **kwargs) -> PlayerStats:
+    def get_player_stats(
+        cls, *, sport: Sport, player_id: str, season: str, **kwargs
+    ) -> PlayerStats:
         """
         Gets player stats for the given season OR just the given week.
         """
         season_type: SeasonType = kwargs.pop("season_type", SeasonType.REGULAR)
         week: int = kwargs.pop("week", None)
 
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, None, cls._STATS_ROUTE, sport.name.lower(), cls._PLAYER_ROUTE,
-                               player_id)
-        url = cls._add_filters(url, ("season_type", season_type.name.lower()), ("season", season), ("week", week))
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            None,
+            cls._STATS_ROUTE,
+            sport.name.lower(),
+            cls._PLAYER_ROUTE,
+            player_id,
+        )
+        url = cls._add_filters(
+            url, ("season_type", season_type.name.lower()), ("season", season), ("week", week)
+        )
 
         response_dict = cls._get(url)
         if response_dict is None:
             error_message = f"Could not get PlayerStats for sport: '{sport.name}', player_id: '{player_id}', season_type: '{season_type}', season: '{season}'"
             if week is not None:
                 error_message += f", week: '{week}'"
             error_message += "."
             raise ValueError(error_message)
         return PlayerStats.from_dict(response_dict)
 
     @classmethod
-    def get_player_projections(cls, *, sport: Sport, player_id: str, season: str, **kwargs) -> PlayerStats:
+    def get_player_projections(
+        cls, *, sport: Sport, player_id: str, season: str, **kwargs
+    ) -> PlayerStats:
         """
         Gets player projections for the given season OR just the given week.
         """
         season_type: SeasonType = kwargs.pop("season_type", SeasonType.REGULAR)
         week: int = kwargs.pop("week", None)
 
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, None, cls._PROJECTIONS_ROUTE, sport.name.lower(),
-                               cls._PLAYER_ROUTE, player_id)
-        url = cls._add_filters(url, ("season_type", season_type.name.lower()), ("season", season), ("week", week))
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            None,
+            cls._PROJECTIONS_ROUTE,
+            sport.name.lower(),
+            cls._PLAYER_ROUTE,
+            player_id,
+        )
+        url = cls._add_filters(
+            url, ("season_type", season_type.name.lower()), ("season", season), ("week", week)
+        )
 
         response_dict = cls._get(url)
         if response_dict is None:
             error_message = f"Could not get PlayerStats for sport: '{sport.name}', player_id: '{player_id}', season_type: '{season_type}', season: '{season}'"
             if week is not None:
                 error_message += f", week: '{week}'"
             error_message += "."
             raise ValueError(error_message)
         return PlayerStats.from_dict(response_dict)
 
     @classmethod
-    def get_all_player_stats(cls, *, sport: Sport, season: str, week: int, **kwargs) -> list[PlayerStats]:
+    def get_all_player_stats(
+        cls, *, sport: Sport, season: str, week: int, **kwargs
+    ) -> list[PlayerStats]:
         season_type: SeasonType = kwargs.pop("season_type", SeasonType.REGULAR)
         positions: list[PlayerPosition] = kwargs.pop("positions", list())
 
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, None, cls._STATS_ROUTE, sport.name.lower(), season, week)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL, None, cls._STATS_ROUTE, sport.name.lower(), season, week
+        )
         filters: list[tuple[str, Any]] = [("season_type", season_type.name.lower())]
         for position in positions:
             filters.append(("position[]", position.name.upper()))
         url = cls._add_filters(url, *filters)
 
         response_list = cls._get(url)
         if response_list is None:
@@ -69,20 +92,28 @@
             if len(positions) > 0:
                 error_message += f", positions: '{positions}'"
             error_message += "."
             raise ValueError(error_message)
         return PlayerStats.from_dict_list(response_list)
 
     @classmethod
-    def get_all_player_projections(cls, *, sport: Sport, season: str, week: int, **kwargs) -> list[PlayerStats]:
+    def get_all_player_projections(
+        cls, *, sport: Sport, season: str, week: int, **kwargs
+    ) -> list[PlayerStats]:
         season_type: SeasonType = kwargs.pop("season_type", SeasonType.REGULAR)
         positions: list[PlayerPosition] = kwargs.pop("positions", list())
 
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, None, cls._PROJECTIONS_ROUTE, sport.name.lower(), season,
-                               week)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            None,
+            cls._PROJECTIONS_ROUTE,
+            sport.name.lower(),
+            season,
+            week,
+        )
         filters: list[tuple[str, Any]] = [("season_type", season_type.name.lower())]
         for position in positions:
             filters.append(("position[]", position.name.upper()))
         url = cls._add_filters(url, *filters)
 
         response_list = cls._get(url)
         if response_list is None:
@@ -97,12 +128,18 @@
 
     @classmethod
     def get_player_head_shot(cls, *, sport: Sport, player_id: str, save_to_path: str) -> None:
         """
         save_to_path should end in ".png".
         """
 
-        url = cls._build_route(cls._SLEEPER_CDN_BASE_URL, None, cls._CONTENT_ROUTE, sport.name.lower(),
-                               cls._PLAYERS_ROUTE, player_id)
+        url = cls._build_route(
+            cls._SLEEPER_CDN_BASE_URL,
+            None,
+            cls._CONTENT_ROUTE,
+            sport.name.lower(),
+            cls._PLAYERS_ROUTE,
+            player_id,
+        )
         url += ".jpg"
         image_file = cls._get_image_file(url)
         image_file.save(save_to_path)
```

### Comparing `sleeper-1.5.0/sleeper/api/unofficial/USportAPIClient.py` & `sleeper-1.6.0/sleeper/api/unofficial/USportAPIClient.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from sleeper.api.SleeperAPIClient import SleeperAPIClient
 from sleeper.enum import SeasonType
 from sleeper.enum.Sport import Sport
 from sleeper.model.Game import Game
 
 
 class USportAPIClient(SleeperAPIClient):
-
     @classmethod
     def get_regular_season_schedule(cls, *, sport: Sport, season: str, **kwargs) -> list[Game]:
         season_type: SeasonType = kwargs.pop("season_type", SeasonType.REGULAR)
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, None, cls._SCHEDULE_ROUTE, sport.name.lower(),
-                               season_type.name.lower(), season)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            None,
+            cls._SCHEDULE_ROUTE,
+            sport.name.lower(),
+            season_type.name.lower(),
+            season,
+        )
 
         response_list = cls._get(url)
         if response_list is None:
             raise ValueError(
-                f"Could not get Game list for sport: '{sport.name}', season: '{season}', season_type: '{season_type.name}'.")
+                f"Could not get Game list for sport: '{sport.name}', season: '{season}', season_type: '{season_type.name}'."
+            )
         return Game.from_dict_list(response_list, sport)
```

### Comparing `sleeper-1.5.0/sleeper/api/unofficial/UTeamAPIClient.py` & `sleeper-1.6.0/sleeper/api/unofficial/UTeamAPIClient.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from sleeper.api.SleeperAPIClient import SleeperAPIClient
 from sleeper.enum import SportTeam
 from sleeper.enum.Sport import Sport
 from sleeper.model.DepthChart import DepthChart
 
 
 class UTeamAPIClient(SleeperAPIClient):
-
     @classmethod
     def get_team_depth_chart(cls, *, sport: Sport, team: SportTeam) -> DepthChart:
-        url = cls._build_route(cls._SLEEPER_APP_BASE_URL, None, cls._PLAYERS_ROUTE, sport.name.lower(),
-                               team.name.lower(), cls._DEPTH_CHART_ROUTE)
+        url = cls._build_route(
+            cls._SLEEPER_APP_BASE_URL,
+            None,
+            cls._PLAYERS_ROUTE,
+            sport.name.lower(),
+            team.name.lower(),
+            cls._DEPTH_CHART_ROUTE,
+        )
 
         response_dict = cls._get(url)
         if response_dict is None:
-            raise ValueError(f"Could not get DepthChart for sport: '{sport.name}', team: '{team.name}'")
+            raise ValueError(
+                f"Could not get DepthChart for sport: '{sport.name}', team: '{team.name}'"
+            )
         return DepthChart.model(sport).from_dict(response_dict)
```

### Comparing `sleeper-1.5.0/sleeper/app.properties` & `sleeper-1.6.0/sleeper/app.properties`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/DraftType.py` & `sleeper-1.6.0/sleeper/enum/DraftType.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/InjuryStatus.py` & `sleeper-1.6.0/sleeper/enum/InjuryStatus.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/PlayerPosition.py` & `sleeper-1.6.0/sleeper/enum/PlayerPosition.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 
 @unique
 class PlayerPosition(Enum):
     """
     Parent for all Enum positions for each sport.
     """
+
     ...
 
     @classmethod
     @abstractmethod
     def from_str(cls, s: str) -> PlayerPosition:
         ...
 
     @staticmethod
     def enum(sport: Sport) -> PlayerPosition:
         from sleeper.enum.nfl.NFLPosition import NFLPosition
+
         if sport == Sport.NFL:
             return NFLPosition
         else:
             raise ValueError(f"Cannot find PlayerPosition for sport: '{sport.name}'.")
```

### Comparing `sleeper-1.5.0/sleeper/enum/PlayerStatus.py` & `sleeper-1.6.0/sleeper/enum/PlayerStatus.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 
 @unique
 class PlayerStatus(Enum):
     """
     Parent for all Enum statuses for each sport.
     """
+
     ...
 
     @classmethod
     @abstractmethod
     def from_str(cls, s: str) -> PlayerStatus:
         ...
 
     @staticmethod
     def enum(sport: Sport) -> PlayerStatus:
         from sleeper.enum.nfl.NFLPlayerStatus import NFLPlayerStatus
+
         if sport == Sport.NFL:
             return NFLPlayerStatus
         else:
             raise ValueError(f"Cannot find PlayerStatus for sport: '{sport.name}'.")
```

### Comparing `sleeper-1.5.0/sleeper/enum/PlayoffRoundType.py` & `sleeper-1.6.0/sleeper/enum/PlayoffRoundType.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/PracticeParticipation.py` & `sleeper-1.6.0/sleeper/enum/PracticeParticipation.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/RosterPosition.py` & `sleeper-1.6.0/sleeper/enum/RosterPosition.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 @unique
 class RosterPosition(Enum):
     """
     Parent for all Enum roster positions for each sport.
     """
+
     ...
 
     @classmethod
     @abstractmethod
     def from_str(cls, s: str) -> RosterPosition:
         ...
```

### Comparing `sleeper-1.5.0/sleeper/enum/ScoringType.py` & `sleeper-1.6.0/sleeper/enum/ScoringType.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/SeasonStatus.py` & `sleeper-1.6.0/sleeper/enum/SeasonStatus.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/SeasonType.py` & `sleeper-1.6.0/sleeper/enum/SeasonType.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/Sport.py` & `sleeper-1.6.0/sleeper/enum/Sport.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/SportTeam.py` & `sleeper-1.6.0/sleeper/enum/SportTeam.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 
 @unique
 class SportTeam(Enum):
     """
     Parent for all Enum teams for each sport.
     """
+
     ...
 
     @classmethod
     @abstractmethod
     def from_str(cls, s: str) -> SportTeam:
         ...
 
     @staticmethod
     def enum(sport: Sport) -> SportTeam:
         from sleeper.enum.nfl.NFLTeam import NFLTeam
+
         if sport == Sport.NFL:
             return NFLTeam
         else:
             raise ValueError(f"Cannot find SportTeam for sport: '{sport.name}'.")
```

### Comparing `sleeper-1.5.0/sleeper/enum/TransactionStatus.py` & `sleeper-1.6.0/sleeper/enum/TransactionStatus.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/TransactionType.py` & `sleeper-1.6.0/sleeper/enum/TransactionType.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/__init__.py` & `sleeper-1.6.0/sleeper/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/nfl/NFLPlayerStatus.py` & `sleeper-1.6.0/sleeper/enum/nfl/NFLPlayerStatus.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/nfl/NFLPosition.py` & `sleeper-1.6.0/sleeper/enum/nfl/NFLPosition.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/nfl/NFLRosterPosition.py` & `sleeper-1.6.0/sleeper/enum/nfl/NFLRosterPosition.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/enum/nfl/NFLTeam.py` & `sleeper-1.6.0/sleeper/enum/nfl/NFLTeam.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/model/DepthChart.py` & `sleeper-1.6.0/sleeper/model/DepthChart.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 
 
 @dataclass(kw_only=True)
 class DepthChart:
     """
     Parent for all DepthChart models for each sport.
     """
+
     ...
 
     @staticmethod
     def model(sport: Sport) -> DepthChart:
         from sleeper.model.nfl.NFLDepthChart import NFLDepthChart
+
         if sport == Sport.NFL:
             return NFLDepthChart
         else:
             raise ValueError(f"Cannot find DepthChart for sport: '{sport.name}'.")
 
     @staticmethod
     @abstractmethod
```

### Comparing `sleeper-1.5.0/sleeper/model/Draft.py` & `sleeper-1.6.0/sleeper/model/Draft.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,31 +28,33 @@
     sport: Sport
     start_time: int
     status: DraftStatus
     type: DraftType
 
     @staticmethod
     def from_dict(draft_dict: dict) -> Draft:
-        return Draft(type=DraftType.from_str(draft_dict.get("type")),
-                     status=DraftStatus.from_str(draft_dict.get("status")),
-                     start_time=draft_dict.get("start_time"),
-                     sport=Sport.from_str(draft_dict.get("sport")),
-                     settings=DraftSettings.from_dict(draft_dict.get("settings")),
-                     season_type=SeasonType.from_str(draft_dict.get("season_type")),
-                     season=draft_dict.get("season"),
-                     metadata=DraftMetadata.from_dict(draft_dict.get("metadata")),
-                     league_id=draft_dict.get("league_id"),
-                     last_picked=draft_dict.get("last_picked"),
-                     last_message_time=draft_dict.get("last_message_time"),
-                     last_message_id=draft_dict.get("last_message_id"),
-                     draft_order=draft_dict.get("draft_order"),
-                     slot_to_roster_id=draft_dict.get("slot_to_roster_id"),
-                     draft_id=draft_dict.get("draft_id"),
-                     creators=draft_dict.get("creators"),
-                     created=draft_dict.get("created"))
+        return Draft(
+            type=DraftType.from_str(draft_dict.get("type")),
+            status=DraftStatus.from_str(draft_dict.get("status")),
+            start_time=draft_dict.get("start_time"),
+            sport=Sport.from_str(draft_dict.get("sport")),
+            settings=DraftSettings.from_dict(draft_dict.get("settings")),
+            season_type=SeasonType.from_str(draft_dict.get("season_type")),
+            season=draft_dict.get("season"),
+            metadata=DraftMetadata.from_dict(draft_dict.get("metadata")),
+            league_id=draft_dict.get("league_id"),
+            last_picked=draft_dict.get("last_picked"),
+            last_message_time=draft_dict.get("last_message_time"),
+            last_message_id=draft_dict.get("last_message_id"),
+            draft_order=draft_dict.get("draft_order"),
+            slot_to_roster_id=draft_dict.get("slot_to_roster_id"),
+            draft_id=draft_dict.get("draft_id"),
+            creators=draft_dict.get("creators"),
+            created=draft_dict.get("created"),
+        )
 
     @staticmethod
     def from_dict_list(draft_dict_list: list) -> list[Draft]:
         drafts = list()
         for draft_dict in draft_dict_list:
             drafts.append(Draft.from_dict(draft_dict))
         return drafts
```

### Comparing `sleeper-1.5.0/sleeper/model/DraftMetadata.py` & `sleeper-1.6.0/sleeper/model/DraftMetadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,10 +9,12 @@
 class DraftMetadata:
     description: str
     name: str
     scoring_type: ScoringType
 
     @staticmethod
     def from_dict(draft_metadata_dict: dict) -> DraftMetadata:
-        return DraftMetadata(scoring_type=ScoringType.from_str(draft_metadata_dict.get("scoring_type")),
-                             name=draft_metadata_dict.get("name"),
-                             description=draft_metadata_dict.get("description"))
+        return DraftMetadata(
+            scoring_type=ScoringType.from_str(draft_metadata_dict.get("scoring_type")),
+            name=draft_metadata_dict.get("name"),
+            description=draft_metadata_dict.get("description"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/DraftPick.py` & `sleeper-1.6.0/sleeper/model/DraftPick.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,22 @@
     previous_owner_id: int
     roster_id: int
     round: int
     season: str
 
     @staticmethod
     def from_dict(draft_pick_dict: dict) -> DraftPick:
-        return DraftPick(season=draft_pick_dict.get("season"),
-                         round=draft_pick_dict.get("round"),
-                         roster_id=draft_pick_dict.get("roster_id"),
-                         previous_owner_id=draft_pick_dict.get("previous_owner_id"),
-                         owner_id=draft_pick_dict.get("owner_id"),
-                         draft_id=draft_pick_dict.get("draft_id"))
+        return DraftPick(
+            season=draft_pick_dict.get("season"),
+            round=draft_pick_dict.get("round"),
+            roster_id=draft_pick_dict.get("roster_id"),
+            previous_owner_id=draft_pick_dict.get("previous_owner_id"),
+            owner_id=draft_pick_dict.get("owner_id"),
+            draft_id=draft_pick_dict.get("draft_id"),
+        )
 
     @classmethod
     def from_dict_list(cls, draft_pick_dict_list: list) -> list[DraftPick]:
         draft_picks = list()
         for draft_pick_dict in draft_pick_dict_list:
             draft_picks.append(DraftPick.from_dict(draft_pick_dict))
         return draft_picks
```

### Comparing `sleeper-1.5.0/sleeper/model/DraftSettings.py` & `sleeper-1.6.0/sleeper/model/DraftSettings.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,23 +20,25 @@
     slots_super_flex: int
     slots_te: int
     slots_wr: int
     teams: int
 
     @staticmethod
     def from_dict(draft_settings_dict: dict) -> DraftSettings:
-        return DraftSettings(teams=draft_settings_dict.get("teams"),
-                             slots_wr=draft_settings_dict.get("slots_wr"),
-                             slots_te=draft_settings_dict.get("slots_te"),
-                             slots_rb=draft_settings_dict.get("slots_rb"),
-                             slots_qb=draft_settings_dict.get("slots_qb"),
-                             slots_flex=draft_settings_dict.get("slots_flex"),
-                             slots_super_flex=draft_settings_dict.get("slots_super_flex"),
-                             slots_bn=draft_settings_dict.get("slots_bn"),
-                             rounds=draft_settings_dict.get("rounds"),
-                             pick_timer=draft_settings_dict.get("pick_timer"),
-                             reversal_round=draft_settings_dict.get("reversal_round"),
-                             player_type=draft_settings_dict.get("player_type"),
-                             nomination_timer=draft_settings_dict.get("nomination_timer"),
-                             enforce_position_limits=draft_settings_dict.get("enforce_position_limits"),
-                             cpu_autopick=draft_settings_dict.get("cpu_autopick"),
-                             alpha_sort=draft_settings_dict.get("alpha_sort"))
+        return DraftSettings(
+            teams=draft_settings_dict.get("teams"),
+            slots_wr=draft_settings_dict.get("slots_wr"),
+            slots_te=draft_settings_dict.get("slots_te"),
+            slots_rb=draft_settings_dict.get("slots_rb"),
+            slots_qb=draft_settings_dict.get("slots_qb"),
+            slots_flex=draft_settings_dict.get("slots_flex"),
+            slots_super_flex=draft_settings_dict.get("slots_super_flex"),
+            slots_bn=draft_settings_dict.get("slots_bn"),
+            rounds=draft_settings_dict.get("rounds"),
+            pick_timer=draft_settings_dict.get("pick_timer"),
+            reversal_round=draft_settings_dict.get("reversal_round"),
+            player_type=draft_settings_dict.get("player_type"),
+            nomination_timer=draft_settings_dict.get("nomination_timer"),
+            enforce_position_limits=draft_settings_dict.get("enforce_position_limits"),
+            cpu_autopick=draft_settings_dict.get("cpu_autopick"),
+            alpha_sort=draft_settings_dict.get("alpha_sort"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/FAABTransaction.py` & `sleeper-1.6.0/sleeper/model/FAABTransaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 class FAABTransaction:
     amount: int
     receiver: int
     sender: int
 
     @staticmethod
     def from_dict(faab_transaction_dict: dict) -> FAABTransaction:
-        return FAABTransaction(sender=faab_transaction_dict.get("sender"),
-                               receiver=faab_transaction_dict.get("receiver"),
-                               amount=faab_transaction_dict.get("amount"))
+        return FAABTransaction(
+            sender=faab_transaction_dict.get("sender"),
+            receiver=faab_transaction_dict.get("receiver"),
+            amount=faab_transaction_dict.get("amount"),
+        )
 
     @staticmethod
     def from_dict_list(faab_transaction_dict_list: list) -> list[FAABTransaction]:
         faab_transactions = list()
         for faab_transaction_dict in faab_transaction_dict_list:
             faab_transactions.append(FAABTransaction.from_dict(faab_transaction_dict))
         return faab_transactions
```

### Comparing `sleeper-1.5.0/sleeper/model/FromPlayoffMatchup.py` & `sleeper-1.6.0/sleeper/model/FromPlayoffMatchup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,9 +9,11 @@
     lost_matchup_id: int
     won_matchup_id: int
 
     @staticmethod
     def from_dict(from_playoff_matchup_object: Optional[dict]) -> Optional[FromPlayoffMatchup]:
         if from_playoff_matchup_object is None:
             return None
-        return FromPlayoffMatchup(won_matchup_id=from_playoff_matchup_object.get("w"),
-                                  lost_matchup_id=from_playoff_matchup_object.get("l"))
+        return FromPlayoffMatchup(
+            won_matchup_id=from_playoff_matchup_object.get("w"),
+            lost_matchup_id=from_playoff_matchup_object.get("l"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/Game.py` & `sleeper-1.6.0/sleeper/model/Game.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import datetime
 from dataclasses import dataclass
-from datetime import date
 
 from sleeper.enum import SportTeam, Sport
 from sleeper.enum.SeasonStatus import SeasonStatus
 
 
 @dataclass(kw_only=True)
 class Game:
@@ -22,13 +21,15 @@
         game_list = list()
         for game_dict in game_dict_list:
             game_list.append(Game.from_dict(game_dict, sport))
         return game_list
 
     @staticmethod
     def from_dict(game_dict: dict, sport: Sport) -> Game:
-        return Game(week=game_dict.get("week"),
-                    status=SeasonStatus.from_str(game_dict.get("status")),
-                    home=SportTeam.enum(sport).from_str(game_dict.get("home")),
-                    game_id=game_dict.get("game_id"),
-                    date=datetime.datetime.strptime(game_dict.get("date"), "%Y-%m-%d").date(),
-                    away=SportTeam.enum(sport).from_str(game_dict.get("away")))
+        return Game(
+            week=game_dict.get("week"),
+            status=SeasonStatus.from_str(game_dict.get("status")),
+            home=SportTeam.enum(sport).from_str(game_dict.get("home")),
+            game_id=game_dict.get("game_id"),
+            date=datetime.datetime.strptime(game_dict.get("date"), "%Y-%m-%d").date(),
+            away=SportTeam.enum(sport).from_str(game_dict.get("away")),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/League.py` & `sleeper-1.6.0/sleeper/model/League.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,52 +2,63 @@
 
 from dataclasses import dataclass
 
 from sleeper.enum.RosterPosition import RosterPosition
 from sleeper.enum.SeasonStatus import SeasonStatus
 from sleeper.enum.SeasonType import SeasonType
 from sleeper.enum.Sport import Sport
+from sleeper.model.LeagueMetadata import LeagueMetadata
 from sleeper.model.LeagueSettings import LeagueSettings
 from sleeper.model.ScoringSettings import ScoringSettings
 
 
 @dataclass(kw_only=True)
 class League:
     avatar: str
+    bracket_id: int
     draft_id: str
     league_id: str
+    metadata: LeagueMetadata
     name: str
     previous_league_id: str
     roster_positions: list[RosterPosition]
     scoring_settings: ScoringSettings
     season: str
     season_type: SeasonType
     settings: LeagueSettings
+    shard: int
     sport: Sport
     status: SeasonStatus
     total_rosters: int
 
     @staticmethod
     def from_dict(league_dict: dict) -> League:
         sport = Sport.from_str(league_dict.get("sport"))
 
-        return League(total_rosters=league_dict.get("total_rosters"),
-                      status=SeasonStatus.from_str(league_dict.get("status")),
-                      sport=sport,
-                      settings=LeagueSettings.from_dict(league_dict.get("settings")),
-                      season_type=SeasonType.from_str(league_dict.get("season_type")),
-                      season=league_dict.get("season"),
-                      scoring_settings=ScoringSettings.from_dict(league_dict.get("scoring_settings")),
-                      roster_positions=[RosterPosition.enum(sport).from_str(roster_position) for roster_position in
-                                        league_dict.get("roster_positions")],
-                      previous_league_id=league_dict.get("previous_league_id"),
-                      name=league_dict.get("name"),
-                      league_id=league_dict.get("league_id"),
-                      draft_id=league_dict.get("draft_id"),
-                      avatar=league_dict.get("avatar"))
+        return League(
+            total_rosters=league_dict.get("total_rosters"),
+            status=SeasonStatus.from_str(league_dict.get("status")),
+            sport=sport,
+            settings=LeagueSettings.from_dict(league_dict.get("settings")),
+            shard=league_dict.get("shard"),
+            season_type=SeasonType.from_str(league_dict.get("season_type")),
+            season=league_dict.get("season"),
+            scoring_settings=ScoringSettings.from_dict(league_dict.get("scoring_settings")),
+            roster_positions=[
+                RosterPosition.enum(sport).from_str(roster_position)
+                for roster_position in league_dict.get("roster_positions")
+            ],
+            previous_league_id=league_dict.get("previous_league_id"),
+            name=league_dict.get("name"),
+            league_id=league_dict.get("league_id"),
+            metadata=LeagueMetadata.from_dict(league_dict.get("metadata")),
+            draft_id=league_dict.get("draft_id"),
+            avatar=league_dict.get("avatar"),
+            bracket_id=league_dict.get("bracket_id"),
+        )
 
     @staticmethod
     def from_dict_list(league_dict_list: list) -> list[League]:
         leagues = list()
         for league_dict in league_dict_list:
             leagues.append(League.from_dict(league_dict))
         return leagues
```

### Comparing `sleeper-1.5.0/sleeper/model/LeagueSettings.py` & `sleeper-1.6.0/sleeper/model/LeagueSettings.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     commissioner_direct_invite: int
     daily_waivers: int
     daily_waivers_days: int
     daily_waivers_hour: int
     daily_waivers_last_ran: int
     disable_adds: int
     disable_trades: int
+    divisions: int
     draft_rounds: int
     last_report: int
     last_scored_leg: int
     league_average_match: int
     leg: int
     max_keepers: int
     num_teams: int
@@ -49,51 +50,55 @@
     waiver_budget: int
     waiver_clear_days: int
     waiver_day_of_week: int
     waiver_type: int
 
     @staticmethod
     def from_dict(settings_dict: dict) -> LeagueSettings:
-        return LeagueSettings(waiver_type=settings_dict.get("waiver_type"),
-                              waiver_day_of_week=settings_dict.get("waiver_day_of_week"),
-                              waiver_clear_days=settings_dict.get("waiver_clear_days"),
-                              waiver_budget=settings_dict.get("waiver_budget"),
-                              type=settings_dict.get("type"),
-                              trade_review_days=settings_dict.get("trade_review_days"),
-                              trade_deadline=settings_dict.get("trade_deadline"),
-                              start_week=settings_dict.get("start_week"),
-                              reserve_slots=settings_dict.get("reserve_slots"),
-                              reserve_allow_out=settings_dict.get("reserve_allow_out"),
-                              playoff_week_start=settings_dict.get("playoff_week_start"),
-                              playoff_teams=settings_dict.get("playoff_teams"),
-                              pick_trading=settings_dict.get("pick_trading"),
-                              offseason_adds=settings_dict.get("offseason_adds"),
-                              num_teams=settings_dict.get("num_teams"),
-                              max_keepers=settings_dict.get("max_keepers"),
-                              leg=settings_dict.get("leg"),
-                              last_scored_leg=settings_dict.get("last_scored_leg"),
-                              last_report=settings_dict.get("last_report"),
-                              draft_rounds=settings_dict.get("draft_rounds"),
-                              bench_lock=settings_dict.get("bench_lock"),
-                              best_ball=settings_dict.get("best_ball"),
-                              capacity_override=settings_dict.get("capacity_override"),
-                              commissioner_direct_invite=settings_dict.get("commissioner_direct_invite"),
-                              daily_waivers=settings_dict.get("daily_waivers"),
-                              daily_waivers_days=settings_dict.get("daily_waivers_days"),
-                              daily_waivers_hour=settings_dict.get("daily_waivers_hour"),
-                              daily_waivers_last_ran=settings_dict.get("daily_waivers_last_ran"),
-                              disable_adds=settings_dict.get("disable_adds"),
-                              disable_trades=settings_dict.get("disable_trades"),
-                              league_average_match=settings_dict.get("league_average_match"),
-                              playoff_round_type=settings_dict.get("playoff_round_type"),
-                              playoff_round_type_enum=PlayoffRoundType.from_int(
-                                  settings_dict.get("playoff_round_type")),
-                              playoff_seed_type=settings_dict.get("playoff_seed_type"),
-                              playoff_type=settings_dict.get("playoff_type"),
-                              reserve_allow_cov=settings_dict.get("reserve_allow_cov"),
-                              reserve_allow_dnr=settings_dict.get("reserve_allow_dnr"),
-                              reserve_allow_na=settings_dict.get("reserve_allow_na"),
-                              reserve_allow_sus=settings_dict.get("reserve_allow_sus"),
-                              taxi_allow_vets=settings_dict.get("taxi_allow_vets"),
-                              taxi_slots=settings_dict.get("taxi_slots"),
-                              taxi_years=settings_dict.get("taxi_years"),
-                              waiver_bid_min=settings_dict.get("waiver_bid_min"))
+        return LeagueSettings(
+            waiver_type=settings_dict.get("waiver_type"),
+            waiver_day_of_week=settings_dict.get("waiver_day_of_week"),
+            waiver_clear_days=settings_dict.get("waiver_clear_days"),
+            waiver_budget=settings_dict.get("waiver_budget"),
+            type=settings_dict.get("type"),
+            trade_review_days=settings_dict.get("trade_review_days"),
+            trade_deadline=settings_dict.get("trade_deadline"),
+            start_week=settings_dict.get("start_week"),
+            reserve_slots=settings_dict.get("reserve_slots"),
+            reserve_allow_out=settings_dict.get("reserve_allow_out"),
+            playoff_week_start=settings_dict.get("playoff_week_start"),
+            playoff_teams=settings_dict.get("playoff_teams"),
+            pick_trading=settings_dict.get("pick_trading"),
+            offseason_adds=settings_dict.get("offseason_adds"),
+            num_teams=settings_dict.get("num_teams"),
+            max_keepers=settings_dict.get("max_keepers"),
+            leg=settings_dict.get("leg"),
+            last_scored_leg=settings_dict.get("last_scored_leg"),
+            last_report=settings_dict.get("last_report"),
+            draft_rounds=settings_dict.get("draft_rounds"),
+            bench_lock=settings_dict.get("bench_lock"),
+            best_ball=settings_dict.get("best_ball"),
+            capacity_override=settings_dict.get("capacity_override"),
+            commissioner_direct_invite=settings_dict.get("commissioner_direct_invite"),
+            daily_waivers=settings_dict.get("daily_waivers"),
+            daily_waivers_days=settings_dict.get("daily_waivers_days"),
+            daily_waivers_hour=settings_dict.get("daily_waivers_hour"),
+            daily_waivers_last_ran=settings_dict.get("daily_waivers_last_ran"),
+            disable_adds=settings_dict.get("disable_adds"),
+            disable_trades=settings_dict.get("disable_trades"),
+            divisions=settings_dict.get("divisions"),
+            league_average_match=settings_dict.get("league_average_match"),
+            playoff_round_type=settings_dict.get("playoff_round_type"),
+            playoff_round_type_enum=PlayoffRoundType.from_int(
+                settings_dict.get("playoff_round_type")
+            ),
+            playoff_seed_type=settings_dict.get("playoff_seed_type"),
+            playoff_type=settings_dict.get("playoff_type"),
+            reserve_allow_cov=settings_dict.get("reserve_allow_cov"),
+            reserve_allow_dnr=settings_dict.get("reserve_allow_dnr"),
+            reserve_allow_na=settings_dict.get("reserve_allow_na"),
+            reserve_allow_sus=settings_dict.get("reserve_allow_sus"),
+            taxi_allow_vets=settings_dict.get("taxi_allow_vets"),
+            taxi_slots=settings_dict.get("taxi_slots"),
+            taxi_years=settings_dict.get("taxi_years"),
+            waiver_bid_min=settings_dict.get("waiver_bid_min"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/Matchup.py` & `sleeper-1.6.0/sleeper/model/Matchup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,24 @@
     points: float
     roster_id: int
     starters: list[str]
     starters_points: list[float]
 
     @staticmethod
     def from_dict(matchup_object_dict: dict) -> Matchup:
-        return Matchup(starters=matchup_object_dict.get("starters"),
-                       roster_id=matchup_object_dict.get("roster_id"),
-                       players=matchup_object_dict.get("players"),
-                       matchup_id=matchup_object_dict.get("matchup_id"),
-                       points=matchup_object_dict.get("points"),
-                       custom_points=matchup_object_dict.get("custom_points"),
-                       players_points=matchup_object_dict.get("players_points"),
-                       starters_points=matchup_object_dict.get("starters_points"))
+        return Matchup(
+            starters=matchup_object_dict.get("starters"),
+            roster_id=matchup_object_dict.get("roster_id"),
+            players=matchup_object_dict.get("players"),
+            matchup_id=matchup_object_dict.get("matchup_id"),
+            points=matchup_object_dict.get("points"),
+            custom_points=matchup_object_dict.get("custom_points"),
+            players_points=matchup_object_dict.get("players_points"),
+            starters_points=matchup_object_dict.get("starters_points"),
+        )
 
     @staticmethod
     def from_dict_list(matchup_dict_list: list) -> list[Matchup]:
         matchups = list()
         for matchup_dict in matchup_dict_list:
             matchups.append(Matchup.from_dict(matchup_dict))
         return matchups
```

### Comparing `sleeper-1.5.0/sleeper/model/Player.py` & `sleeper-1.6.0/sleeper/model/Player.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,66 +62,75 @@
     years_exp: int
 
     @staticmethod
     def from_dict(player_dict: dict, sport: Sport) -> Optional[Player]:
         if player_dict is None:
             return None
         given_fantasy_positions = player_dict.get("fantasy_positions")
-        fantasy_positions = [PlayerPosition.enum(sport).from_str(pos) for pos in
-                             given_fantasy_positions] if given_fantasy_positions is not None else None
+        fantasy_positions = (
+            [PlayerPosition.enum(sport).from_str(pos) for pos in given_fantasy_positions]
+            if given_fantasy_positions is not None
+            else None
+        )
 
-        birth_date = None if player_dict.get("birth_date") is None else datetime.datetime.strptime(
-            player_dict.get("birth_date"), "%Y-%m-%d").date()
+        birth_date = (
+            None
+            if player_dict.get("birth_date") is None
+            else datetime.datetime.strptime(player_dict.get("birth_date"), "%Y-%m-%d").date()
+        )
 
-        return Player(hashtag=player_dict.get("hashtag"),
-                      depth_chart_position=player_dict.get("depth_chart_position"),
-                      status=PlayerStatus.enum(sport).from_str(player_dict.get("status")),
-                      sport=sport,
-                      fantasy_positions=fantasy_positions,
-                      number=player_dict.get("number"),
-                      search_last_name=player_dict.get("search_last_name"),
-                      injury_start_date=player_dict.get("injury_start_date"),
-                      weight=player_dict.get("weight"),
-                      position=PlayerPosition.enum(sport).from_str(player_dict.get("position")),
-                      practice_participation=PracticeParticipation.from_str(
-                          player_dict.get("practice_participation")),
-                      sportradar_id=player_dict.get("sportradar_id"),
-                      team=SportTeam.enum(sport).from_str(player_dict.get("team")),
-                      last_name=player_dict.get("last_name"),
-                      college=player_dict.get("college"),
-                      fantasy_data_id=player_dict.get("fantasy_data_id"),
-                      injury_status=InjuryStatus.from_str(player_dict.get("injury_status")),
-                      player_id=player_dict.get("player_id"),
-                      height=player_dict.get("height"),
-                      search_full_name=player_dict.get("search_full_name"),
-                      age=player_dict.get("age"),
-                      stats_id=player_dict.get("stats_id"),
-                      birth_country=player_dict.get("birth_country"),
-                      espn_id=player_dict.get("espn_id"),
-                      search_rank=player_dict.get("search_rank"),
-                      first_name=player_dict.get("first_name"),
-                      depth_chart_order=player_dict.get("depth_chart_order"),
-                      years_exp=player_dict.get("years_exp"),
-                      rotowire_id=player_dict.get("rotowire_id"),
-                      rotoworld_id=player_dict.get("rotoworld_id"),
-                      search_first_name=player_dict.get("search_first_name"),
-                      yahoo_id=player_dict.get("yahoo_id"),
-                      swish_id=player_dict.get("swish_id"),
-                      birth_city=player_dict.get("birth_city"),
-                      injury_notes=player_dict.get("injury_notes"),
-                      gsis_id=player_dict.get("gsis_id"),
-                      birth_state=player_dict.get("birth_state"),
-                      practice_description=player_dict.get("practice_description"),
-                      pandascore_id=player_dict.get("pandascore_id"),
-                      high_school=player_dict.get("high_school"),
-                      news_updated=player_dict.get("news_updated"),
-                      metadata=player_dict.get("metadata"),
-                      injury_body_part=player_dict.get("injury_body_part"),
-                      birth_date=birth_date,
-                      active=player_dict.get("active"))
+        return Player(
+            hashtag=player_dict.get("hashtag"),
+            depth_chart_position=player_dict.get("depth_chart_position"),
+            status=PlayerStatus.enum(sport).from_str(player_dict.get("status")),
+            sport=sport,
+            fantasy_positions=fantasy_positions,
+            number=player_dict.get("number"),
+            search_last_name=player_dict.get("search_last_name"),
+            injury_start_date=player_dict.get("injury_start_date"),
+            weight=player_dict.get("weight"),
+            position=PlayerPosition.enum(sport).from_str(player_dict.get("position")),
+            practice_participation=PracticeParticipation.from_str(
+                player_dict.get("practice_participation")
+            ),
+            sportradar_id=player_dict.get("sportradar_id"),
+            team=SportTeam.enum(sport).from_str(player_dict.get("team")),
+            last_name=player_dict.get("last_name"),
+            college=player_dict.get("college"),
+            fantasy_data_id=player_dict.get("fantasy_data_id"),
+            injury_status=InjuryStatus.from_str(player_dict.get("injury_status")),
+            player_id=player_dict.get("player_id"),
+            height=player_dict.get("height"),
+            search_full_name=player_dict.get("search_full_name"),
+            age=player_dict.get("age"),
+            stats_id=player_dict.get("stats_id"),
+            birth_country=player_dict.get("birth_country"),
+            espn_id=player_dict.get("espn_id"),
+            search_rank=player_dict.get("search_rank"),
+            first_name=player_dict.get("first_name"),
+            depth_chart_order=player_dict.get("depth_chart_order"),
+            years_exp=player_dict.get("years_exp"),
+            rotowire_id=player_dict.get("rotowire_id"),
+            rotoworld_id=player_dict.get("rotoworld_id"),
+            search_first_name=player_dict.get("search_first_name"),
+            yahoo_id=player_dict.get("yahoo_id"),
+            swish_id=player_dict.get("swish_id"),
+            birth_city=player_dict.get("birth_city"),
+            injury_notes=player_dict.get("injury_notes"),
+            gsis_id=player_dict.get("gsis_id"),
+            birth_state=player_dict.get("birth_state"),
+            practice_description=player_dict.get("practice_description"),
+            pandascore_id=player_dict.get("pandascore_id"),
+            high_school=player_dict.get("high_school"),
+            news_updated=player_dict.get("news_updated"),
+            metadata=player_dict.get("metadata"),
+            injury_body_part=player_dict.get("injury_body_part"),
+            birth_date=birth_date,
+            active=player_dict.get("active"),
+        )
 
     @staticmethod
     def dict_by_id(player_dict_list: list, sport: Sport) -> dict[str, Player]:
         players_by_id = dict()
         for player_id in player_dict_list:
             players_by_id[player_id] = Player.from_dict(player_dict_list[player_id], sport)
         return players_by_id
```

### Comparing `sleeper-1.5.0/sleeper/model/PlayerDraftPick.py` & `sleeper-1.6.0/sleeper/model/PlayerDraftPick.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,27 @@
     picked_by: str
     player_id: str
     roster_id: str
     round: int
 
     @staticmethod
     def from_dict(player_draft_pick_dict: dict, sport: Sport) -> PlayerDraftPick:
-        return PlayerDraftPick(player_id=player_draft_pick_dict.get("player_id"),
-                               picked_by=player_draft_pick_dict.get("picked_by"),
-                               roster_id=player_draft_pick_dict.get("roster_id"),
-                               round=player_draft_pick_dict.get("round"),
-                               draft_slot=player_draft_pick_dict.get("draft_slot"),
-                               pick_no=player_draft_pick_dict.get("pick_no"),
-                               metadata=PlayerDraftPickMetadata.from_dict(player_draft_pick_dict.get("metadata"),
-                                                                          sport),
-                               is_keeper=player_draft_pick_dict.get("is_keeper", False),
-                               draft_id=player_draft_pick_dict.get("draft_id"))
+        return PlayerDraftPick(
+            player_id=player_draft_pick_dict.get("player_id"),
+            picked_by=player_draft_pick_dict.get("picked_by"),
+            roster_id=player_draft_pick_dict.get("roster_id"),
+            round=player_draft_pick_dict.get("round"),
+            draft_slot=player_draft_pick_dict.get("draft_slot"),
+            pick_no=player_draft_pick_dict.get("pick_no"),
+            metadata=PlayerDraftPickMetadata.from_dict(
+                player_draft_pick_dict.get("metadata"), sport
+            ),
+            is_keeper=player_draft_pick_dict.get("is_keeper", False),
+            draft_id=player_draft_pick_dict.get("draft_id"),
+        )
 
     @staticmethod
     def from_dict_list(player_draft_pick_dict_list: list, sport: Sport) -> list[PlayerDraftPick]:
         player_draft_picks = list()
         for player_draft_pick in player_draft_pick_dict_list:
             player_draft_picks.append(PlayerDraftPick.from_dict(player_draft_pick, sport))
         return player_draft_picks
```

### Comparing `sleeper-1.5.0/sleeper/model/PlayerDraftPickMetadata.py` & `sleeper-1.6.0/sleeper/model/PlayerDraftPickMetadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,23 @@
     position: PlayerPosition
     sport: Sport
     status: PlayerStatus
     team: SportTeam
 
     @staticmethod
     def from_dict(player_draft_pick_metadata_dict: dict, sport: Sport) -> PlayerDraftPickMetadata:
-        return PlayerDraftPickMetadata(team=SportTeam.enum(sport).from_str(player_draft_pick_metadata_dict.get("team")),
-                                       status=PlayerStatus.enum(sport).from_str(
-                                           player_draft_pick_metadata_dict.get("status")),
-                                       sport=Sport.from_str(player_draft_pick_metadata_dict.get("sport")),
-                                       position=PlayerPosition.enum(sport).from_str(
-                                           player_draft_pick_metadata_dict.get("position")),
-                                       player_id=player_draft_pick_metadata_dict.get("player_id"),
-                                       number=player_draft_pick_metadata_dict.get("number"),
-                                       news_updated=player_draft_pick_metadata_dict.get("news_updated"),
-                                       first_name=player_draft_pick_metadata_dict.get("first_name"),
-                                       last_name=player_draft_pick_metadata_dict.get("last_name"),
-                                       injury_status=InjuryStatus.from_str(
-                                           player_draft_pick_metadata_dict.get("injury_status")))
+        return PlayerDraftPickMetadata(
+            team=SportTeam.enum(sport).from_str(player_draft_pick_metadata_dict.get("team")),
+            status=PlayerStatus.enum(sport).from_str(player_draft_pick_metadata_dict.get("status")),
+            sport=Sport.from_str(player_draft_pick_metadata_dict.get("sport")),
+            position=PlayerPosition.enum(sport).from_str(
+                player_draft_pick_metadata_dict.get("position")
+            ),
+            player_id=player_draft_pick_metadata_dict.get("player_id"),
+            number=player_draft_pick_metadata_dict.get("number"),
+            news_updated=player_draft_pick_metadata_dict.get("news_updated"),
+            first_name=player_draft_pick_metadata_dict.get("first_name"),
+            last_name=player_draft_pick_metadata_dict.get("last_name"),
+            injury_status=InjuryStatus.from_str(
+                player_draft_pick_metadata_dict.get("injury_status")
+            ),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/PlayerStats.py` & `sleeper-1.6.0/sleeper/model/PlayerStats.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import datetime
 from dataclasses import dataclass
-from datetime import date
 
 from sleeper.enum import SportTeam, Sport, SeasonType
 from sleeper.enum.Category import Category
 from sleeper.enum.Company import Company
 from sleeper.model import Player
 from sleeper.model.Stats import Stats
 
@@ -33,22 +32,27 @@
         for player_stats_dict in player_stats_dict_list:
             player_stats_list.append(PlayerStats.from_dict(player_stats_dict))
         return player_stats_list
 
     @staticmethod
     def from_dict(player_stats_dict: dict) -> PlayerStats:
         sport = Sport.from_str(player_stats_dict.get("sport"))
-        date_ = None if player_stats_dict.get("date") is None else datetime.datetime.strptime(
-            player_stats_dict.get("date"), "%Y-%m-%d").date()
-        return PlayerStats(category=Category.from_str(player_stats_dict.get("category")),
-                           company=Company.from_str(player_stats_dict.get("company")),
-                           date=date_,
-                           game_id=player_stats_dict.get("game_id"),
-                           opponent=SportTeam.enum(sport).from_str(player_stats_dict.get("opponent")),
-                           player=Player.from_dict(player_stats_dict.get("player"), sport),
-                           player_id=player_stats_dict.get("player_id"),
-                           season=player_stats_dict.get("season"),
-                           season_type=SeasonType.from_str(player_stats_dict.get("season_type")),
-                           sport=sport,
-                           stats=Stats.model(sport).from_dict(player_stats_dict.get("stats")),
-                           team=SportTeam.enum(sport).from_str(player_stats_dict.get("team")),
-                           week=player_stats_dict.get("week"))
+        date_ = (
+            None
+            if player_stats_dict.get("date") is None
+            else datetime.datetime.strptime(player_stats_dict.get("date"), "%Y-%m-%d").date()
+        )
+        return PlayerStats(
+            category=Category.from_str(player_stats_dict.get("category")),
+            company=Company.from_str(player_stats_dict.get("company")),
+            date=date_,
+            game_id=player_stats_dict.get("game_id"),
+            opponent=SportTeam.enum(sport).from_str(player_stats_dict.get("opponent")),
+            player=Player.from_dict(player_stats_dict.get("player"), sport),
+            player_id=player_stats_dict.get("player_id"),
+            season=player_stats_dict.get("season"),
+            season_type=SeasonType.from_str(player_stats_dict.get("season_type")),
+            sport=sport,
+            stats=Stats.model(sport).from_dict(player_stats_dict.get("stats")),
+            team=SportTeam.enum(sport).from_str(player_stats_dict.get("team")),
+            week=player_stats_dict.get("week"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/PlayerTrend.py` & `sleeper-1.6.0/sleeper/model/PlayerTrend.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 @dataclass(kw_only=True)
 class PlayerTrend:
     count: int
     player_id: str
 
     @staticmethod
     def from_dict(player_trend_dict: dict) -> PlayerTrend:
-        return PlayerTrend(player_id=player_trend_dict.get("player_id"),
-                           count=player_trend_dict.get("count"))
+        return PlayerTrend(
+            player_id=player_trend_dict.get("player_id"), count=player_trend_dict.get("count")
+        )
 
     @staticmethod
     def from_dict_list(player_trend_dict_list: list) -> list[PlayerTrend]:
         player_trends = list()
         for player_trend_dict in player_trend_dict_list:
             player_trends.append(PlayerTrend.from_dict(player_trend_dict))
         return player_trends
```

### Comparing `sleeper-1.5.0/sleeper/model/PlayoffMatchup.py` & `sleeper-1.6.0/sleeper/model/PlayoffMatchup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,25 @@
     team_2_from: FromPlayoffMatchup
     team_2_roster_id: int
     winning_roster_id: int
     p: int  # no documentation on what this field means
 
     @staticmethod
     def from_dict(playoff_matchup_object: dict) -> PlayoffMatchup:
-        return PlayoffMatchup(round=playoff_matchup_object.get("r"),
-                              matchup_id=playoff_matchup_object.get("m"),
-                              team_1_roster_id=playoff_matchup_object.get("t1"),
-                              team_2_roster_id=playoff_matchup_object.get("t2"),
-                              winning_roster_id=playoff_matchup_object.get("w"),
-                              losing_roster_id=playoff_matchup_object.get("l"),
-                              team_1_from=FromPlayoffMatchup.from_dict(playoff_matchup_object.get("t1_from")),
-                              team_2_from=FromPlayoffMatchup.from_dict(playoff_matchup_object.get("t2_from")),
-                              p=playoff_matchup_object.get("p"))
+        return PlayoffMatchup(
+            round=playoff_matchup_object.get("r"),
+            matchup_id=playoff_matchup_object.get("m"),
+            team_1_roster_id=playoff_matchup_object.get("t1"),
+            team_2_roster_id=playoff_matchup_object.get("t2"),
+            winning_roster_id=playoff_matchup_object.get("w"),
+            losing_roster_id=playoff_matchup_object.get("l"),
+            team_1_from=FromPlayoffMatchup.from_dict(playoff_matchup_object.get("t1_from")),
+            team_2_from=FromPlayoffMatchup.from_dict(playoff_matchup_object.get("t2_from")),
+            p=playoff_matchup_object.get("p"),
+        )
 
     @staticmethod
     def from_dict_str(playoff_matchup_dict_list: list) -> list[PlayoffMatchup]:
         playoff_matchups = list()
         for playoff_matchup_dict in playoff_matchup_dict_list:
             playoff_matchups.append(PlayoffMatchup.from_dict(playoff_matchup_dict))
         return playoff_matchups
```

### Comparing `sleeper-1.5.0/sleeper/model/Roster.py` & `sleeper-1.6.0/sleeper/model/Roster.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,27 @@
     roster_id: int
     settings: RosterSettings
     starters: list[str]
     taxi: Any  # not sure what this is
 
     @staticmethod
     def from_dict(roster_dict: dict) -> Roster:
-        return Roster(starters=roster_dict.get("starters"),
-                      settings=RosterSettings.from_dict(roster_dict.get("settings")),
-                      roster_id=roster_dict.get("roster_id"),
-                      reserve=roster_dict.get("reserve"),
-                      players=roster_dict.get("players"),
-                      owner_id=roster_dict.get("owner_id"),
-                      league_id=roster_dict.get("league_id"),
-                      co_owners=roster_dict.get("co_owners"),
-                      metadata=roster_dict.get("metadata"),
-                      player_map=roster_dict.get("player_map"),
-                      taxi=roster_dict.get("taxi"))
+        return Roster(
+            starters=roster_dict.get("starters"),
+            settings=RosterSettings.from_dict(roster_dict.get("settings")),
+            roster_id=roster_dict.get("roster_id"),
+            reserve=roster_dict.get("reserve"),
+            players=roster_dict.get("players"),
+            owner_id=roster_dict.get("owner_id"),
+            league_id=roster_dict.get("league_id"),
+            co_owners=roster_dict.get("co_owners"),
+            metadata=roster_dict.get("metadata"),
+            player_map=roster_dict.get("player_map"),
+            taxi=roster_dict.get("taxi"),
+        )
 
     @staticmethod
     def from_dict_list(roster_dict_list: list) -> list[Roster]:
         rosters = list()
         for roster_dict in roster_dict_list:
             rosters.append(Roster.from_dict(roster_dict))
         return rosters
```

### Comparing `sleeper-1.5.0/sleeper/model/RosterSettings.py` & `sleeper-1.6.0/sleeper/model/RosterSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 
 @dataclass(kw_only=True)
 class RosterSettings:
+    division: int
     fpts: int
     fpts_against: int
     fpts_against_decimal: int
     fpts_decimal: int
     losses: int
     ppts: int
     ppts_decimal: int
@@ -17,20 +18,23 @@
     waiver_adjusted: int
     waiver_budget_used: int
     waiver_position: int
     wins: int
 
     @classmethod
     def from_dict(cls, roster_settings_dict: dict) -> RosterSettings:
-        return RosterSettings(wins=roster_settings_dict.get("wins"),
-                              waiver_position=roster_settings_dict.get("waiver_position"),
-                              waiver_budget_used=roster_settings_dict.get("waiver_budget_used"),
-                              total_moves=roster_settings_dict.get("total_moves"),
-                              ties=roster_settings_dict.get("ties"),
-                              losses=roster_settings_dict.get("losses"),
-                              fpts_decimal=roster_settings_dict.get("fpts_decimal"),
-                              fpts_against_decimal=roster_settings_dict.get("fpts_against_decimal"),
-                              fpts_against=roster_settings_dict.get("fpts_against"),
-                              fpts=roster_settings_dict.get("fpts"),
-                              ppts_decimal=roster_settings_dict.get("ppts_decimal"),
-                              ppts=roster_settings_dict.get("ppts"),
-                              waiver_adjusted=roster_settings_dict.get("waiver_adjusted"))
+        return RosterSettings(
+            division=roster_settings_dict.get("division"),
+            wins=roster_settings_dict.get("wins"),
+            waiver_position=roster_settings_dict.get("waiver_position"),
+            waiver_budget_used=roster_settings_dict.get("waiver_budget_used"),
+            total_moves=roster_settings_dict.get("total_moves"),
+            ties=roster_settings_dict.get("ties"),
+            losses=roster_settings_dict.get("losses"),
+            fpts_decimal=roster_settings_dict.get("fpts_decimal"),
+            fpts_against_decimal=roster_settings_dict.get("fpts_against_decimal"),
+            fpts_against=roster_settings_dict.get("fpts_against"),
+            fpts=roster_settings_dict.get("fpts"),
+            ppts_decimal=roster_settings_dict.get("ppts_decimal"),
+            ppts=roster_settings_dict.get("ppts"),
+            waiver_adjusted=roster_settings_dict.get("waiver_adjusted"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/ScoringSettings.py` & `sleeper-1.6.0/sleeper/model/ScoringSettings.py`

 * *Files 7% similar despite different names*

```diff
@@ -102,105 +102,107 @@
     yds_allow_400_449: float
     yds_allow_450_499: float
     yds_allow_500_549: float
     yds_allow_550p: float
 
     @staticmethod
     def from_dict(scoring_settings_dict: dict) -> ScoringSettings:
-        return ScoringSettings(yds_allow_0_100=scoring_settings_dict.get("yds_allow_0_100"),
-                               yds_allow_100_199=scoring_settings_dict.get("yds_allow_100_199"),
-                               yds_allow_200_299=scoring_settings_dict.get("yds_allow_200_299"),
-                               yds_allow_300_349=scoring_settings_dict.get("yds_allow_300_349"),
-                               yds_allow_350_399=scoring_settings_dict.get("yds_allow_350_399"),
-                               yds_allow_400_449=scoring_settings_dict.get("yds_allow_400_449"),
-                               yds_allow_450_499=scoring_settings_dict.get("yds_allow_450_499"),
-                               yds_allow_500_549=scoring_settings_dict.get("yds_allow_500_549"),
-                               yds_allow_550p=scoring_settings_dict.get("yds_allow_550p"),
-                               fgm=scoring_settings_dict.get("fgm"),
-                               fgm_0_19=scoring_settings_dict.get("fgm_0_19"),
-                               fgm_20_29=scoring_settings_dict.get("fgm_20_29"),
-                               fgm_30_39=scoring_settings_dict.get("fgm_30_39"),
-                               fgm_40_49=scoring_settings_dict.get("fgm_40_49"),
-                               fgm_50p=scoring_settings_dict.get("fgm_50p"),
-                               fgmiss=scoring_settings_dict.get("fgmiss"),
-                               fgmiss_0_19=scoring_settings_dict.get("fgmiss_0_19"),
-                               fgmiss_20_29=scoring_settings_dict.get("fgmiss_20_29"),
-                               fgmiss_30_39=scoring_settings_dict.get("fgmiss_30_39"),
-                               fgmiss_40_49=scoring_settings_dict.get("fgmiss_40_49"),
-                               fgmiss_50p=scoring_settings_dict.get("fgmiss_50p"),
-                               fg_ret_yd=scoring_settings_dict.get("fg_ret_yd"),
-                               pass_2pt=scoring_settings_dict.get("pass_2pt"),
-                               pass_int=scoring_settings_dict.get("pass_int"),
-                               pass_sack=scoring_settings_dict.get("pass_sack"),
-                               pass_cmp=scoring_settings_dict.get("pass_cmp"),
-                               pass_cmp_40p=scoring_settings_dict.get("pass_cmp_40p"),
-                               pass_inc=scoring_settings_dict.get("pass_inc"),
-                               pass_att=scoring_settings_dict.get("pass_att"),
-                               pass_yd=scoring_settings_dict.get("pass_yd"),
-                               pass_td=scoring_settings_dict.get("pass_td"),
-                               def_pass_def=scoring_settings_dict.get("def_pass_def"),
-                               def_td=scoring_settings_dict.get("def_td"),
-                               def_st_fum_rec=scoring_settings_dict.get("def_st_fum_rec"),
-                               def_st_td=scoring_settings_dict.get("def_st_td"),
-                               def_st_ff=scoring_settings_dict.get("def_st_ff"),
-                               def_2pt=scoring_settings_dict.get("def_2pt"),
-                               st_fum_rec=scoring_settings_dict.get("st_fum_rec"),
-                               st_ff=scoring_settings_dict.get("st_ff"),
-                               st_tkl_solo=scoring_settings_dict.get("st_tkl_solo"),
-                               st_td=scoring_settings_dict.get("st_td"),
-                               fum_rec=scoring_settings_dict.get("fum_rec"),
-                               fum_lost=scoring_settings_dict.get("fum_lost"),
-                               fum=scoring_settings_dict.get("fum"),
-                               fum_ret_yd=scoring_settings_dict.get("fum_ret_yd"),
-                               idp_safe=scoring_settings_dict.get("idp_safe"),
-                               idp_ff=scoring_settings_dict.get("idp_ff"),
-                               idp_blk_kick=scoring_settings_dict.get("idp_blk_kick"),
-                               idp_int=scoring_settings_dict.get("idp_int"),
-                               idp_tkl=scoring_settings_dict.get("idp_tkl"),
-                               idp_def_td=scoring_settings_dict.get("idp_def_td"),
-                               idp_pass_def=scoring_settings_dict.get("idp_pass_def"),
-                               idp_fum_rec=scoring_settings_dict.get("idp_fum_rec"),
-                               idp_sack=scoring_settings_dict.get("idp_sack"),
-                               idp_tkl_ast=scoring_settings_dict.get("idp_tkl_ast"),
-                               idp_tkl_solo=scoring_settings_dict.get("idp_tkl_solo"),
-                               rush_att=scoring_settings_dict.get("rush_att"),
-                               pts_allow_0=scoring_settings_dict.get("pts_allow_0"),
-                               pts_allow_1_6=scoring_settings_dict.get("pts_allow_1_6"),
-                               pts_allow_7_13=scoring_settings_dict.get("pts_allow_7_13"),
-                               pts_allow_14_20=scoring_settings_dict.get("pts_allow_14_20"),
-                               pts_allow_21_27=scoring_settings_dict.get("pts_allow_21_27"),
-                               pts_allow_28_34=scoring_settings_dict.get("pts_allow_28_34"),
-                               pts_allow_35p=scoring_settings_dict.get("pts_allow_35p"),
-                               rush_40p=scoring_settings_dict.get("rush_40p"),
-                               rush_2pt=scoring_settings_dict.get("rush_2pt"),
-                               rush_yd=scoring_settings_dict.get("rush_yd"),
-                               rush_td=scoring_settings_dict.get("rush_td"),
-                               bonus_rush_yd_100=scoring_settings_dict.get("bonus_rush_yd_100"),
-                               bonus_rush_yd_200=scoring_settings_dict.get("bonus_rush_yd_200"),
-                               bonus_rec_yd_100=scoring_settings_dict.get("bonus_rec_yd_100"),
-                               bonus_rec_yd_200=scoring_settings_dict.get("bonus_rec_yd_200"),
-                               bonus_pass_yd_300=scoring_settings_dict.get("bonus_pass_yd_300"),
-                               bonus_pass_yd_400=scoring_settings_dict.get("bonus_pass_yd_400"),
-                               rec_yd=scoring_settings_dict.get("rec_yd"),
-                               rec_2pt=scoring_settings_dict.get("rec_2pt"),
-                               rec=scoring_settings_dict.get("rec"),
-                               rec_td=scoring_settings_dict.get("rec_td"),
-                               rec_40p=scoring_settings_dict.get("rec_40p"),
-                               tkl=scoring_settings_dict.get("tkl"),
-                               tkl_loss=scoring_settings_dict.get("tkl_loss"),
-                               tkl_solo=scoring_settings_dict.get("tkl_solo"),
-                               tkl_ast=scoring_settings_dict.get("tkl_ast"),
-                               int_ret_yd=scoring_settings_dict.get("int_ret_yd"),
-                               int=scoring_settings_dict.get("int"),
-                               pr_td=scoring_settings_dict.get("pr_td"),
-                               pr_yd=scoring_settings_dict.get("pr_yd"),
-                               sack_yd=scoring_settings_dict.get("sack_yd"),
-                               sack=scoring_settings_dict.get("sack"),
-                               kr_yd=scoring_settings_dict.get("kr_yd"),
-                               kr_td=scoring_settings_dict.get("kr_td"),
-                               blk_kick=scoring_settings_dict.get("blk_kick"),
-                               blk_kick_ret_yd=scoring_settings_dict.get("blk_kick_ret_yd"),
-                               xpmiss=scoring_settings_dict.get("xpmiss"),
-                               ff=scoring_settings_dict.get("ff"),
-                               qb_hit=scoring_settings_dict.get("qb_hit"),
-                               xpm=scoring_settings_dict.get("xpm"),
-                               safe=scoring_settings_dict.get("safe"))
+        return ScoringSettings(
+            yds_allow_0_100=scoring_settings_dict.get("yds_allow_0_100"),
+            yds_allow_100_199=scoring_settings_dict.get("yds_allow_100_199"),
+            yds_allow_200_299=scoring_settings_dict.get("yds_allow_200_299"),
+            yds_allow_300_349=scoring_settings_dict.get("yds_allow_300_349"),
+            yds_allow_350_399=scoring_settings_dict.get("yds_allow_350_399"),
+            yds_allow_400_449=scoring_settings_dict.get("yds_allow_400_449"),
+            yds_allow_450_499=scoring_settings_dict.get("yds_allow_450_499"),
+            yds_allow_500_549=scoring_settings_dict.get("yds_allow_500_549"),
+            yds_allow_550p=scoring_settings_dict.get("yds_allow_550p"),
+            fgm=scoring_settings_dict.get("fgm"),
+            fgm_0_19=scoring_settings_dict.get("fgm_0_19"),
+            fgm_20_29=scoring_settings_dict.get("fgm_20_29"),
+            fgm_30_39=scoring_settings_dict.get("fgm_30_39"),
+            fgm_40_49=scoring_settings_dict.get("fgm_40_49"),
+            fgm_50p=scoring_settings_dict.get("fgm_50p"),
+            fgmiss=scoring_settings_dict.get("fgmiss"),
+            fgmiss_0_19=scoring_settings_dict.get("fgmiss_0_19"),
+            fgmiss_20_29=scoring_settings_dict.get("fgmiss_20_29"),
+            fgmiss_30_39=scoring_settings_dict.get("fgmiss_30_39"),
+            fgmiss_40_49=scoring_settings_dict.get("fgmiss_40_49"),
+            fgmiss_50p=scoring_settings_dict.get("fgmiss_50p"),
+            fg_ret_yd=scoring_settings_dict.get("fg_ret_yd"),
+            pass_2pt=scoring_settings_dict.get("pass_2pt"),
+            pass_int=scoring_settings_dict.get("pass_int"),
+            pass_sack=scoring_settings_dict.get("pass_sack"),
+            pass_cmp=scoring_settings_dict.get("pass_cmp"),
+            pass_cmp_40p=scoring_settings_dict.get("pass_cmp_40p"),
+            pass_inc=scoring_settings_dict.get("pass_inc"),
+            pass_att=scoring_settings_dict.get("pass_att"),
+            pass_yd=scoring_settings_dict.get("pass_yd"),
+            pass_td=scoring_settings_dict.get("pass_td"),
+            def_pass_def=scoring_settings_dict.get("def_pass_def"),
+            def_td=scoring_settings_dict.get("def_td"),
+            def_st_fum_rec=scoring_settings_dict.get("def_st_fum_rec"),
+            def_st_td=scoring_settings_dict.get("def_st_td"),
+            def_st_ff=scoring_settings_dict.get("def_st_ff"),
+            def_2pt=scoring_settings_dict.get("def_2pt"),
+            st_fum_rec=scoring_settings_dict.get("st_fum_rec"),
+            st_ff=scoring_settings_dict.get("st_ff"),
+            st_tkl_solo=scoring_settings_dict.get("st_tkl_solo"),
+            st_td=scoring_settings_dict.get("st_td"),
+            fum_rec=scoring_settings_dict.get("fum_rec"),
+            fum_lost=scoring_settings_dict.get("fum_lost"),
+            fum=scoring_settings_dict.get("fum"),
+            fum_ret_yd=scoring_settings_dict.get("fum_ret_yd"),
+            idp_safe=scoring_settings_dict.get("idp_safe"),
+            idp_ff=scoring_settings_dict.get("idp_ff"),
+            idp_blk_kick=scoring_settings_dict.get("idp_blk_kick"),
+            idp_int=scoring_settings_dict.get("idp_int"),
+            idp_tkl=scoring_settings_dict.get("idp_tkl"),
+            idp_def_td=scoring_settings_dict.get("idp_def_td"),
+            idp_pass_def=scoring_settings_dict.get("idp_pass_def"),
+            idp_fum_rec=scoring_settings_dict.get("idp_fum_rec"),
+            idp_sack=scoring_settings_dict.get("idp_sack"),
+            idp_tkl_ast=scoring_settings_dict.get("idp_tkl_ast"),
+            idp_tkl_solo=scoring_settings_dict.get("idp_tkl_solo"),
+            rush_att=scoring_settings_dict.get("rush_att"),
+            pts_allow_0=scoring_settings_dict.get("pts_allow_0"),
+            pts_allow_1_6=scoring_settings_dict.get("pts_allow_1_6"),
+            pts_allow_7_13=scoring_settings_dict.get("pts_allow_7_13"),
+            pts_allow_14_20=scoring_settings_dict.get("pts_allow_14_20"),
+            pts_allow_21_27=scoring_settings_dict.get("pts_allow_21_27"),
+            pts_allow_28_34=scoring_settings_dict.get("pts_allow_28_34"),
+            pts_allow_35p=scoring_settings_dict.get("pts_allow_35p"),
+            rush_40p=scoring_settings_dict.get("rush_40p"),
+            rush_2pt=scoring_settings_dict.get("rush_2pt"),
+            rush_yd=scoring_settings_dict.get("rush_yd"),
+            rush_td=scoring_settings_dict.get("rush_td"),
+            bonus_rush_yd_100=scoring_settings_dict.get("bonus_rush_yd_100"),
+            bonus_rush_yd_200=scoring_settings_dict.get("bonus_rush_yd_200"),
+            bonus_rec_yd_100=scoring_settings_dict.get("bonus_rec_yd_100"),
+            bonus_rec_yd_200=scoring_settings_dict.get("bonus_rec_yd_200"),
+            bonus_pass_yd_300=scoring_settings_dict.get("bonus_pass_yd_300"),
+            bonus_pass_yd_400=scoring_settings_dict.get("bonus_pass_yd_400"),
+            rec_yd=scoring_settings_dict.get("rec_yd"),
+            rec_2pt=scoring_settings_dict.get("rec_2pt"),
+            rec=scoring_settings_dict.get("rec"),
+            rec_td=scoring_settings_dict.get("rec_td"),
+            rec_40p=scoring_settings_dict.get("rec_40p"),
+            tkl=scoring_settings_dict.get("tkl"),
+            tkl_loss=scoring_settings_dict.get("tkl_loss"),
+            tkl_solo=scoring_settings_dict.get("tkl_solo"),
+            tkl_ast=scoring_settings_dict.get("tkl_ast"),
+            int_ret_yd=scoring_settings_dict.get("int_ret_yd"),
+            int=scoring_settings_dict.get("int"),
+            pr_td=scoring_settings_dict.get("pr_td"),
+            pr_yd=scoring_settings_dict.get("pr_yd"),
+            sack_yd=scoring_settings_dict.get("sack_yd"),
+            sack=scoring_settings_dict.get("sack"),
+            kr_yd=scoring_settings_dict.get("kr_yd"),
+            kr_td=scoring_settings_dict.get("kr_td"),
+            blk_kick=scoring_settings_dict.get("blk_kick"),
+            blk_kick_ret_yd=scoring_settings_dict.get("blk_kick_ret_yd"),
+            xpmiss=scoring_settings_dict.get("xpmiss"),
+            ff=scoring_settings_dict.get("ff"),
+            qb_hit=scoring_settings_dict.get("qb_hit"),
+            xpm=scoring_settings_dict.get("xpm"),
+            safe=scoring_settings_dict.get("safe"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/SportState.py` & `sleeper-1.6.0/sleeper/model/SportState.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,18 +17,25 @@
     season: str
     season_start_date: date
     season_type: SeasonType
     week: int
 
     @staticmethod
     def from_dict(sport_state_dict) -> SportState:
-        season_start_date = None if sport_state_dict.get("season_start_date") is None else datetime.datetime.strptime(
-            sport_state_dict.get("season_start_date"), "%Y-%m-%d").date()
-        return SportState(week=sport_state_dict.get("week"),
-                          season_type=SeasonType.from_str(sport_state_dict.get("season_type")),
-                          season_start_date=season_start_date,
-                          season=sport_state_dict.get("season"),
-                          previous_season=sport_state_dict.get("previous_season"),
-                          leg=sport_state_dict.get("leg"),
-                          league_season=sport_state_dict.get("league_season"),
-                          league_create_season=sport_state_dict.get("league_create_season"),
-                          display_week=sport_state_dict.get("display_week"))
+        season_start_date = (
+            None
+            if sport_state_dict.get("season_start_date") is None
+            else datetime.datetime.strptime(
+                sport_state_dict.get("season_start_date"), "%Y-%m-%d"
+            ).date()
+        )
+        return SportState(
+            week=sport_state_dict.get("week"),
+            season_type=SeasonType.from_str(sport_state_dict.get("season_type")),
+            season_start_date=season_start_date,
+            season=sport_state_dict.get("season"),
+            previous_season=sport_state_dict.get("previous_season"),
+            leg=sport_state_dict.get("leg"),
+            league_season=sport_state_dict.get("league_season"),
+            league_create_season=sport_state_dict.get("league_create_season"),
+            display_week=sport_state_dict.get("display_week"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/Stats.py` & `sleeper-1.6.0/sleeper/model/Stats.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 
 
 @dataclass(kw_only=True)
 class Stats:
     """
     Parent for all Stat models for each sport.
     """
+
     ...
 
     @staticmethod
     def model(sport: Sport) -> Stats:
         from sleeper.model.nfl.NFLStats import NFLStats
+
         if sport == Sport.NFL:
             return NFLStats
         else:
             raise ValueError(f"Cannot find Stats for sport: '{sport.name}'.")
 
     @staticmethod
     @abstractmethod
     def from_dict(d: dict) -> Stats:
         ...
-    
+
     @abstractmethod
     def get_populated_stats(self) -> dict:
         ...
```

### Comparing `sleeper-1.5.0/sleeper/model/TradedPick.py` & `sleeper-1.6.0/sleeper/model/TradedPick.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,21 @@
     previous_owner_id: int
     roster_id: int
     round: int
     season: str
 
     @staticmethod
     def from_dict(traded_pick_dict: dict) -> TradedPick:
-        return TradedPick(season=traded_pick_dict.get("season"),
-                          round=traded_pick_dict.get("round"),
-                          roster_id=traded_pick_dict.get("roster_id"),
-                          previous_owner_id=traded_pick_dict.get("previous_owner_id"),
-                          owner_id=traded_pick_dict.get("owner_id"))
+        return TradedPick(
+            season=traded_pick_dict.get("season"),
+            round=traded_pick_dict.get("round"),
+            roster_id=traded_pick_dict.get("roster_id"),
+            previous_owner_id=traded_pick_dict.get("previous_owner_id"),
+            owner_id=traded_pick_dict.get("owner_id"),
+        )
 
     @staticmethod
     def from_dict_list(traded_pick_dict_list: list) -> list[TradedPick]:
         traded_picks = list()
         for traded_pick_dict in traded_pick_dict_list:
             traded_picks.append(TradedPick.from_dict(traded_pick_dict))
         return traded_picks
```

### Comparing `sleeper-1.5.0/sleeper/model/Transaction.py` & `sleeper-1.6.0/sleeper/model/Transaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,29 +26,31 @@
     type: TransactionType
     waiver_budget: list[FAABTransaction]
     leg: int
     metadata: Any  # not sure what this is
 
     @staticmethod
     def from_dict(transaction_dict: dict) -> Transaction:
-        return Transaction(type=TransactionType.from_str(transaction_dict.get("type")),
-                           transaction_id=transaction_dict.get("transaction_id"),
-                           status_updated=transaction_dict.get("status_updated"),
-                           status=TransactionStatus.from_str(transaction_dict.get("status")),
-                           settings=TransactionSettings.from_dict(transaction_dict.get("settings")),
-                           roster_ids=transaction_dict.get("roster_ids"),
-                           leg=transaction_dict.get("leg"),
-                           adds=transaction_dict.get("adds"),
-                           drops=transaction_dict.get("drops"),
-                           draft_picks=DraftPick.from_dict_list(transaction_dict.get("draft_picks")),
-                           creator=transaction_dict.get("creator"),
-                           created=transaction_dict.get("created"),
-                           consenter_ids=transaction_dict.get("consenter_ids"),
-                           waiver_budget=FAABTransaction.from_dict_list(transaction_dict.get("waiver_budget")),
-                           metadata=transaction_dict.get("metadata"))
+        return Transaction(
+            type=TransactionType.from_str(transaction_dict.get("type")),
+            transaction_id=transaction_dict.get("transaction_id"),
+            status_updated=transaction_dict.get("status_updated"),
+            status=TransactionStatus.from_str(transaction_dict.get("status")),
+            settings=TransactionSettings.from_dict(transaction_dict.get("settings")),
+            roster_ids=transaction_dict.get("roster_ids"),
+            leg=transaction_dict.get("leg"),
+            adds=transaction_dict.get("adds"),
+            drops=transaction_dict.get("drops"),
+            draft_picks=DraftPick.from_dict_list(transaction_dict.get("draft_picks")),
+            creator=transaction_dict.get("creator"),
+            created=transaction_dict.get("created"),
+            consenter_ids=transaction_dict.get("consenter_ids"),
+            waiver_budget=FAABTransaction.from_dict_list(transaction_dict.get("waiver_budget")),
+            metadata=transaction_dict.get("metadata"),
+        )
 
     @staticmethod
     def from_dict_list(transaction_dict_list: list) -> list[Transaction]:
         transactions = list()
         for transaction_dict in transaction_dict_list:
             transactions.append(Transaction.from_dict(transaction_dict))
         return transactions
```

### Comparing `sleeper-1.5.0/sleeper/model/TransactionSettings.py` & `sleeper-1.6.0/sleeper/model/TransactionSettings.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,9 +9,11 @@
     seq: int
     waiver_bid: int
 
     @classmethod
     def from_dict(cls, transaction_settings_dict: Optional[dict]) -> Optional[TransactionSettings]:
         if transaction_settings_dict is None:
             return None
-        return TransactionSettings(waiver_bid=transaction_settings_dict.get("waiver_bid"),
-                                   seq=transaction_settings_dict.get("seq"))
+        return TransactionSettings(
+            waiver_bid=transaction_settings_dict.get("waiver_bid"),
+            seq=transaction_settings_dict.get("seq"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/model/User.py` & `sleeper-1.6.0/sleeper/model/User.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,36 +27,38 @@
     token: str
     user_id: str
     username: str
     verification: Any  # not sure what this is
 
     @staticmethod
     def from_dict(user_dict: dict) -> User:
-        return User(username=user_dict.get("username"),
-                    user_id=user_dict.get("user_id"),
-                    display_name=user_dict.get("display_name"),
-                    avatar=user_dict.get("avatar"),
-                    is_owner=user_dict.get("is_owner", False),
-                    is_bot=user_dict.get("is_bot", False),
-                    league_id=user_dict.get("league_id"),
-                    cookies=user_dict.get("cookies"),
-                    created=user_dict.get("created"),
-                    currencies=user_dict.get("currencies"),
-                    data_updated=user_dict.get("data_updated"),
-                    deleted=user_dict.get("deleted"),
-                    email=user_dict.get("email"),
-                    metadata=user_dict.get("metadata"),
-                    notifications=user_dict.get("notifications"),
-                    pending=user_dict.get("pending"),
-                    phone=user_dict.get("phone"),
-                    real_name=user_dict.get("real_name"),
-                    solicitable=user_dict.get("solicitable"),
-                    summoner_region=user_dict.get("summoner_region"),
-                    token=user_dict.get("token"),
-                    verification=user_dict.get("verification"))
+        return User(
+            username=user_dict.get("username"),
+            user_id=user_dict.get("user_id"),
+            display_name=user_dict.get("display_name"),
+            avatar=user_dict.get("avatar"),
+            is_owner=user_dict.get("is_owner", False),
+            is_bot=user_dict.get("is_bot", False),
+            league_id=user_dict.get("league_id"),
+            cookies=user_dict.get("cookies"),
+            created=user_dict.get("created"),
+            currencies=user_dict.get("currencies"),
+            data_updated=user_dict.get("data_updated"),
+            deleted=user_dict.get("deleted"),
+            email=user_dict.get("email"),
+            metadata=user_dict.get("metadata"),
+            notifications=user_dict.get("notifications"),
+            pending=user_dict.get("pending"),
+            phone=user_dict.get("phone"),
+            real_name=user_dict.get("real_name"),
+            solicitable=user_dict.get("solicitable"),
+            summoner_region=user_dict.get("summoner_region"),
+            token=user_dict.get("token"),
+            verification=user_dict.get("verification"),
+        )
 
     @staticmethod
     def from_dict_list(user_dict_list: list) -> list[User]:
         users = list()
         for user_dict in user_dict_list:
             users.append(User.from_dict(user_dict))
         return users
```

### Comparing `sleeper-1.5.0/sleeper/model/__init__.py` & `sleeper-1.6.0/sleeper/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sleeper-1.5.0/sleeper/model/nfl/NFLDepthChart.py` & `sleeper-1.6.0/sleeper/model/nfl/NFLDepthChart.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,9 +54,9 @@
             RILB=nfl_depth_chart_dict.get("RILB"),
             ROLB=nfl_depth_chart_dict.get("ROLB"),
             RT=nfl_depth_chart_dict.get("RT"),
             SS=nfl_depth_chart_dict.get("SS"),
             TE=nfl_depth_chart_dict.get("TE"),
             WR1=nfl_depth_chart_dict.get("WR1"),
             WR2=nfl_depth_chart_dict.get("WR2"),
-            WR3=nfl_depth_chart_dict.get("WR3")
+            WR3=nfl_depth_chart_dict.get("WR3"),
         )
```

### Comparing `sleeper-1.5.0/sleeper/model/nfl/NFLStats.py` & `sleeper-1.6.0/sleeper/model/nfl/NFLStats.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,194 +196,196 @@
     yds_allow_450_499: float
 
     def get_populated_stats(self) -> dict:
         return {k: v for (k, v) in vars(self).items() if v is not None}
 
     @staticmethod
     def from_dict(nfl_stats_dict: dict) -> NFLStats:
-        return NFLStats(blk_kick=nfl_stats_dict.get("blk_kick"),
-                        blk_kick_ret_yd=nfl_stats_dict.get("blk_kick_ret_yd"),
-                        bonus_pass_cmp_25=nfl_stats_dict.get("bonus_pass_cmp_25"),
-                        bonus_pass_yd_300=nfl_stats_dict.get("bonus_pass_yd_300"),
-                        bonus_pass_yd_400=nfl_stats_dict.get("bonus_pass_yd_400"),
-                        bonus_rec_rb=nfl_stats_dict.get("bonus_rec_rb"),
-                        bonus_rec_te=nfl_stats_dict.get("bonus_rec_te"),
-                        bonus_rec_wr=nfl_stats_dict.get("bonus_rec_wr"),
-                        bonus_rec_yd_100=nfl_stats_dict.get("bonus_rec_yd_100"),
-                        bonus_rush_rec_yd_200=nfl_stats_dict.get("bonus_rush_rec_yd_200"),
-                        bonus_rush_yd_100=nfl_stats_dict.get("bonus_rush_yd_100"),
-                        bonus_rush_att_20=nfl_stats_dict.get("bonus_rush_att_20"),
-                        bonus_rush_rec_yd_100=nfl_stats_dict.get("bonus_rush_rec_yd_100"),
-                        bonus_sack_2p=nfl_stats_dict.get("bonus_sack_2p"),
-                        bonus_tkl_10p=nfl_stats_dict.get("bonus_tkl_10p"),
-                        cmp_pct=nfl_stats_dict.get("cmp_pct"),
-                        def_3_and_out=nfl_stats_dict.get("def_3_and_out"),
-                        def_4_and_stop=nfl_stats_dict.get("def_4_and_stop"),
-                        def_forced_punts=nfl_stats_dict.get("def_forced_punts"),
-                        def_kr=nfl_stats_dict.get("def_kr"),
-                        def_kr_lng=nfl_stats_dict.get("def_kr_lng"),
-                        def_kr_yd=nfl_stats_dict.get("def_kr_yd"),
-                        def_kr_ypa=nfl_stats_dict.get("def_kr_ypa"),
-                        def_pass_def=nfl_stats_dict.get("def_pass_def"),
-                        def_pr=nfl_stats_dict.get("def_pr"),
-                        def_pr_lng=nfl_stats_dict.get("def_pr_lng"),
-                        def_pr_yd=nfl_stats_dict.get("def_pr_yd"),
-                        def_pr_ypa=nfl_stats_dict.get("def_pr_ypa"),
-                        def_snp=nfl_stats_dict.get("def_snp"),
-                        def_st_td=nfl_stats_dict.get("def_st_td"),
-                        def_st_tkl_solo=nfl_stats_dict.get("def_st_tkl_solo"),
-                        def_td=nfl_stats_dict.get("def_td"),
-                        fan_pts_allow=nfl_stats_dict.get("fan_pts_allow"),
-                        fan_pts_allow_k=nfl_stats_dict.get("fan_pts_allow_k"),
-                        fan_pts_allow_qb=nfl_stats_dict.get("fan_pts_allow_qb"),
-                        fan_pts_allow_rb=nfl_stats_dict.get("fan_pts_allow_rb"),
-                        fan_pts_allow_te=nfl_stats_dict.get("fan_pts_allow_te"),
-                        fan_pts_allow_wr=nfl_stats_dict.get("fan_pts_allow_wr"),
-                        ff=nfl_stats_dict.get("ff"),
-                        fga=nfl_stats_dict.get("fga"),
-                        fgm=nfl_stats_dict.get("fgm"),
-                        fgm_20_29=nfl_stats_dict.get("fgm_20_29"),
-                        fgm_30_39=nfl_stats_dict.get("fgm_30_39"),
-                        fgm_40_49=nfl_stats_dict.get("fgm_40_49"),
-                        fgm_50p=nfl_stats_dict.get("fgm_50p"),
-                        fgm_lng=nfl_stats_dict.get("fgm_lng"),
-                        fgm_pct=nfl_stats_dict.get("fgm_pct"),
-                        fgm_yds=nfl_stats_dict.get("fgm_yds"),
-                        fgm_yds_over_30=nfl_stats_dict.get("fgm_yds_over_30"),
-                        fgmiss=nfl_stats_dict.get("fgmiss"),
-                        fgmiss_30_39=nfl_stats_dict.get("fgmiss_30_39"),
-                        fgmiss_40_49=nfl_stats_dict.get("fgmiss_40_49"),
-                        fgmiss_50p=nfl_stats_dict.get("fgmiss_50p"),
-                        fum=nfl_stats_dict.get("fum"),
-                        fum_lost=nfl_stats_dict.get("fum_lost"),
-                        fum_rec=nfl_stats_dict.get("fum_rec"),
-                        fum_ret_yd=nfl_stats_dict.get("fum_ret_yd"),
-                        gms_active=nfl_stats_dict.get("gms_active"),
-                        gp=nfl_stats_dict.get("gp"),
-                        idp_blk_kick=nfl_stats_dict.get("idp_blk_kick"),
-                        idp_def_td=nfl_stats_dict.get("idp_def_td"),
-                        idp_ff=nfl_stats_dict.get("idp_ff"),
-                        idp_fum_rec=nfl_stats_dict.get("idp_fum_rec"),
-                        idp_fum_ret_yd=nfl_stats_dict.get("idp_fum_ret_yd"),
-                        idp_int=nfl_stats_dict.get("idp_int"),
-                        idp_int_ret_yd=nfl_stats_dict.get("idp_int_ret_yd"),
-                        idp_pass_def=nfl_stats_dict.get("idp_pass_def"),
-                        idp_qb_hit=nfl_stats_dict.get("idp_qb_hit"),
-                        idp_sack=nfl_stats_dict.get("idp_sack"),
-                        idp_sack_yd=nfl_stats_dict.get("idp_sack_yd"),
-                        idp_tkl=nfl_stats_dict.get("idp_tkl"),
-                        idp_tkl_ast=nfl_stats_dict.get("idp_tkl_ast"),
-                        idp_tkl_loss=nfl_stats_dict.get("idp_tkl_loss"),
-                        idp_tkl_solo=nfl_stats_dict.get("idp_tkl_solo"),
-                        int_=nfl_stats_dict.get("int"),
-                        int_ret_yd=nfl_stats_dict.get("int_ret_yd"),
-                        kr=nfl_stats_dict.get("kr"),
-                        kr_lng=nfl_stats_dict.get("kr_lng"),
-                        kr_yd=nfl_stats_dict.get("kr_yd"),
-                        kr_ypa=nfl_stats_dict.get("kr_ypa"),
-                        gs=nfl_stats_dict.get("gs"),
-                        off_snp=nfl_stats_dict.get("off_snp"),
-                        pass_2pt=nfl_stats_dict.get("pass_2pt"),
-                        pass_air_yd=nfl_stats_dict.get("pass_air_yd"),
-                        pass_att=nfl_stats_dict.get("pass_att"),
-                        pass_cmp=nfl_stats_dict.get("pass_cmp"),
-                        pass_cmp_40p=nfl_stats_dict.get("pass_cmp_40p"),
-                        pass_fd=nfl_stats_dict.get("pass_fd"),
-                        pass_inc=nfl_stats_dict.get("pass_inc"),
-                        pass_int=nfl_stats_dict.get("pass_int"),
-                        pass_int_td=nfl_stats_dict.get("pass_int_td"),
-                        pass_lng=nfl_stats_dict.get("pass_lng"),
-                        pass_rtg=nfl_stats_dict.get("pass_rtg"),
-                        pass_rz_att=nfl_stats_dict.get("pass_rz_att"),
-                        pass_sack=nfl_stats_dict.get("pass_sack"),
-                        pass_sack_yds=nfl_stats_dict.get("pass_sack_yds"),
-                        pass_td=nfl_stats_dict.get("pass_td"),
-                        pass_td_40p=nfl_stats_dict.get("pass_td_40p"),
-                        pass_td_50p=nfl_stats_dict.get("pass_td_50p"),
-                        pass_td_lng=nfl_stats_dict.get("pass_td_lng"),
-                        pass_yd=nfl_stats_dict.get("pass_yd"),
-                        pass_ypa=nfl_stats_dict.get("pass_ypa"),
-                        penalty=nfl_stats_dict.get("penalty"),
-                        penalty_yd=nfl_stats_dict.get("penalty_yd"),
-                        pr=nfl_stats_dict.get("pr"),
-                        pr_lng=nfl_stats_dict.get("pr_lng"),
-                        pr_yd=nfl_stats_dict.get("pr_yd"),
-                        pr_ypa=nfl_stats_dict.get("pr_ypa"),
-                        pts_allow=nfl_stats_dict.get("pts_allow"),
-                        pts_allow_14_20=nfl_stats_dict.get("pts_allow_14_20"),
-                        pts_allow_1_6=nfl_stats_dict.get("pts_allow_1_6"),
-                        pts_allow_21_27=nfl_stats_dict.get("pts_allow_21_27"),
-                        pts_allow_28_34=nfl_stats_dict.get("pts_allow_28_34"),
-                        pts_allow_35p=nfl_stats_dict.get("pts_allow_35p"),
-                        pts_allow_7_13=nfl_stats_dict.get("pts_allow_7_13"),
-                        pts_half_ppr=nfl_stats_dict.get("pts_half_ppr"),
-                        pts_ppr=nfl_stats_dict.get("pts_ppr"),
-                        pts_std=nfl_stats_dict.get("pts_std"),
-                        punt_blkd=nfl_stats_dict.get("punt_blkd"),
-                        punt_in_20=nfl_stats_dict.get("punt_in_20"),
-                        punt_net_yd=nfl_stats_dict.get("punt_net_yd"),
-                        punt_tb=nfl_stats_dict.get("punt_tb"),
-                        punt_yds=nfl_stats_dict.get("punt_yds"),
-                        punts=nfl_stats_dict.get("punts"),
-                        qb_hit=nfl_stats_dict.get("qb_hit"),
-                        rec=nfl_stats_dict.get("rec"),
-                        rec_0_4=nfl_stats_dict.get("rec_0_4"),
-                        rec_10_19=nfl_stats_dict.get("rec_10_19"),
-                        rec_20_29=nfl_stats_dict.get("rec_20_29"),
-                        rec_2pt=nfl_stats_dict.get("rec_2pt"),
-                        rec_30_39=nfl_stats_dict.get("rec_30_39"),
-                        rec_40p=nfl_stats_dict.get("rec_40p"),
-                        rec_5_9=nfl_stats_dict.get("rec_5_9"),
-                        rec_air_yd=nfl_stats_dict.get("rec_air_yd"),
-                        rec_drop=nfl_stats_dict.get("rec_drop"),
-                        rec_fd=nfl_stats_dict.get("rec_fd"),
-                        rec_lng=nfl_stats_dict.get("rec_lng"),
-                        rec_rz_tgt=nfl_stats_dict.get("rec_rz_tgt"),
-                        rec_td=nfl_stats_dict.get("rec_td"),
-                        rec_td_40p=nfl_stats_dict.get("rec_td_40p"),
-                        rec_td_50p=nfl_stats_dict.get("rec_td_50p"),
-                        rec_td_lng=nfl_stats_dict.get("rec_td_lng"),
-                        rec_tgt=nfl_stats_dict.get("rec_tgt"),
-                        rec_yar=nfl_stats_dict.get("rec_yar"),
-                        rec_yd=nfl_stats_dict.get("rec_yd"),
-                        rec_ypr=nfl_stats_dict.get("rec_ypr"),
-                        rec_ypt=nfl_stats_dict.get("rec_ypt"),
-                        rush_2pt=nfl_stats_dict.get("rush_2pt"),
-                        rush_40p=nfl_stats_dict.get("rush_40p"),
-                        rush_att=nfl_stats_dict.get("rush_att"),
-                        rush_btkl=nfl_stats_dict.get("rush_btkl"),
-                        rush_fd=nfl_stats_dict.get("rush_fd"),
-                        rush_lng=nfl_stats_dict.get("rush_lng"),
-                        rush_rz_att=nfl_stats_dict.get("rush_rz_att"),
-                        rush_td=nfl_stats_dict.get("rush_td"),
-                        rush_td_40p=nfl_stats_dict.get("rush_td_40p"),
-                        rush_td_50p=nfl_stats_dict.get("rush_td_50p"),
-                        rush_td_lng=nfl_stats_dict.get("rush_td_lng"),
-                        rush_tkl_loss=nfl_stats_dict.get("rush_tkl_loss"),
-                        rush_tkl_loss_yd=nfl_stats_dict.get("rush_tkl_loss_yd"),
-                        rush_yac=nfl_stats_dict.get("rush_yac"),
-                        rush_yd=nfl_stats_dict.get("rush_yd"),
-                        rush_ypa=nfl_stats_dict.get("rush_ypa"),
-                        sack=nfl_stats_dict.get("sack"),
-                        sack_yd=nfl_stats_dict.get("sack_yd"),
-                        st_snp=nfl_stats_dict.get("st_snp"),
-                        st_td=nfl_stats_dict.get("st_td"),
-                        st_tkl_solo=nfl_stats_dict.get("st_tkl_solo"),
-                        td=nfl_stats_dict.get("td"),
-                        tkl=nfl_stats_dict.get("tkl"),
-                        tkl_ast=nfl_stats_dict.get("tkl_ast"),
-                        tkl_ast_misc=nfl_stats_dict.get("tkl_ast_misc"),
-                        tkl_loss=nfl_stats_dict.get("tkl_loss"),
-                        tkl_solo=nfl_stats_dict.get("tkl_solo"),
-                        tkl_solo_misc=nfl_stats_dict.get("tkl_solo_misc"),
-                        tm_def_snp=nfl_stats_dict.get("tm_def_snp"),
-                        tm_off_snp=nfl_stats_dict.get("tm_off_snp"),
-                        tm_st_snp=nfl_stats_dict.get("tm_st_snp"),
-                        xpa=nfl_stats_dict.get("xpa"),
-                        xpm=nfl_stats_dict.get("xpm"),
-                        xpmiss=nfl_stats_dict.get("xpmiss"),
-                        yds_allow=nfl_stats_dict.get("yds_allow"),
-                        yds_allow_200_299=nfl_stats_dict.get("yds_allow_200_299"),
-                        yds_allow_300_349=nfl_stats_dict.get("yds_allow_300_349"),
-                        yds_allow_350_399=nfl_stats_dict.get("yds_allow_350_399"),
-                        yds_allow_400_449=nfl_stats_dict.get("yds_allow_400_449"),
-                        yds_allow_450_499=nfl_stats_dict.get("yds_allow_450_499"))
+        return NFLStats(
+            blk_kick=nfl_stats_dict.get("blk_kick"),
+            blk_kick_ret_yd=nfl_stats_dict.get("blk_kick_ret_yd"),
+            bonus_pass_cmp_25=nfl_stats_dict.get("bonus_pass_cmp_25"),
+            bonus_pass_yd_300=nfl_stats_dict.get("bonus_pass_yd_300"),
+            bonus_pass_yd_400=nfl_stats_dict.get("bonus_pass_yd_400"),
+            bonus_rec_rb=nfl_stats_dict.get("bonus_rec_rb"),
+            bonus_rec_te=nfl_stats_dict.get("bonus_rec_te"),
+            bonus_rec_wr=nfl_stats_dict.get("bonus_rec_wr"),
+            bonus_rec_yd_100=nfl_stats_dict.get("bonus_rec_yd_100"),
+            bonus_rush_rec_yd_200=nfl_stats_dict.get("bonus_rush_rec_yd_200"),
+            bonus_rush_yd_100=nfl_stats_dict.get("bonus_rush_yd_100"),
+            bonus_rush_att_20=nfl_stats_dict.get("bonus_rush_att_20"),
+            bonus_rush_rec_yd_100=nfl_stats_dict.get("bonus_rush_rec_yd_100"),
+            bonus_sack_2p=nfl_stats_dict.get("bonus_sack_2p"),
+            bonus_tkl_10p=nfl_stats_dict.get("bonus_tkl_10p"),
+            cmp_pct=nfl_stats_dict.get("cmp_pct"),
+            def_3_and_out=nfl_stats_dict.get("def_3_and_out"),
+            def_4_and_stop=nfl_stats_dict.get("def_4_and_stop"),
+            def_forced_punts=nfl_stats_dict.get("def_forced_punts"),
+            def_kr=nfl_stats_dict.get("def_kr"),
+            def_kr_lng=nfl_stats_dict.get("def_kr_lng"),
+            def_kr_yd=nfl_stats_dict.get("def_kr_yd"),
+            def_kr_ypa=nfl_stats_dict.get("def_kr_ypa"),
+            def_pass_def=nfl_stats_dict.get("def_pass_def"),
+            def_pr=nfl_stats_dict.get("def_pr"),
+            def_pr_lng=nfl_stats_dict.get("def_pr_lng"),
+            def_pr_yd=nfl_stats_dict.get("def_pr_yd"),
+            def_pr_ypa=nfl_stats_dict.get("def_pr_ypa"),
+            def_snp=nfl_stats_dict.get("def_snp"),
+            def_st_td=nfl_stats_dict.get("def_st_td"),
+            def_st_tkl_solo=nfl_stats_dict.get("def_st_tkl_solo"),
+            def_td=nfl_stats_dict.get("def_td"),
+            fan_pts_allow=nfl_stats_dict.get("fan_pts_allow"),
+            fan_pts_allow_k=nfl_stats_dict.get("fan_pts_allow_k"),
+            fan_pts_allow_qb=nfl_stats_dict.get("fan_pts_allow_qb"),
+            fan_pts_allow_rb=nfl_stats_dict.get("fan_pts_allow_rb"),
+            fan_pts_allow_te=nfl_stats_dict.get("fan_pts_allow_te"),
+            fan_pts_allow_wr=nfl_stats_dict.get("fan_pts_allow_wr"),
+            ff=nfl_stats_dict.get("ff"),
+            fga=nfl_stats_dict.get("fga"),
+            fgm=nfl_stats_dict.get("fgm"),
+            fgm_20_29=nfl_stats_dict.get("fgm_20_29"),
+            fgm_30_39=nfl_stats_dict.get("fgm_30_39"),
+            fgm_40_49=nfl_stats_dict.get("fgm_40_49"),
+            fgm_50p=nfl_stats_dict.get("fgm_50p"),
+            fgm_lng=nfl_stats_dict.get("fgm_lng"),
+            fgm_pct=nfl_stats_dict.get("fgm_pct"),
+            fgm_yds=nfl_stats_dict.get("fgm_yds"),
+            fgm_yds_over_30=nfl_stats_dict.get("fgm_yds_over_30"),
+            fgmiss=nfl_stats_dict.get("fgmiss"),
+            fgmiss_30_39=nfl_stats_dict.get("fgmiss_30_39"),
+            fgmiss_40_49=nfl_stats_dict.get("fgmiss_40_49"),
+            fgmiss_50p=nfl_stats_dict.get("fgmiss_50p"),
+            fum=nfl_stats_dict.get("fum"),
+            fum_lost=nfl_stats_dict.get("fum_lost"),
+            fum_rec=nfl_stats_dict.get("fum_rec"),
+            fum_ret_yd=nfl_stats_dict.get("fum_ret_yd"),
+            gms_active=nfl_stats_dict.get("gms_active"),
+            gp=nfl_stats_dict.get("gp"),
+            idp_blk_kick=nfl_stats_dict.get("idp_blk_kick"),
+            idp_def_td=nfl_stats_dict.get("idp_def_td"),
+            idp_ff=nfl_stats_dict.get("idp_ff"),
+            idp_fum_rec=nfl_stats_dict.get("idp_fum_rec"),
+            idp_fum_ret_yd=nfl_stats_dict.get("idp_fum_ret_yd"),
+            idp_int=nfl_stats_dict.get("idp_int"),
+            idp_int_ret_yd=nfl_stats_dict.get("idp_int_ret_yd"),
+            idp_pass_def=nfl_stats_dict.get("idp_pass_def"),
+            idp_qb_hit=nfl_stats_dict.get("idp_qb_hit"),
+            idp_sack=nfl_stats_dict.get("idp_sack"),
+            idp_sack_yd=nfl_stats_dict.get("idp_sack_yd"),
+            idp_tkl=nfl_stats_dict.get("idp_tkl"),
+            idp_tkl_ast=nfl_stats_dict.get("idp_tkl_ast"),
+            idp_tkl_loss=nfl_stats_dict.get("idp_tkl_loss"),
+            idp_tkl_solo=nfl_stats_dict.get("idp_tkl_solo"),
+            int_=nfl_stats_dict.get("int"),
+            int_ret_yd=nfl_stats_dict.get("int_ret_yd"),
+            kr=nfl_stats_dict.get("kr"),
+            kr_lng=nfl_stats_dict.get("kr_lng"),
+            kr_yd=nfl_stats_dict.get("kr_yd"),
+            kr_ypa=nfl_stats_dict.get("kr_ypa"),
+            gs=nfl_stats_dict.get("gs"),
+            off_snp=nfl_stats_dict.get("off_snp"),
+            pass_2pt=nfl_stats_dict.get("pass_2pt"),
+            pass_air_yd=nfl_stats_dict.get("pass_air_yd"),
+            pass_att=nfl_stats_dict.get("pass_att"),
+            pass_cmp=nfl_stats_dict.get("pass_cmp"),
+            pass_cmp_40p=nfl_stats_dict.get("pass_cmp_40p"),
+            pass_fd=nfl_stats_dict.get("pass_fd"),
+            pass_inc=nfl_stats_dict.get("pass_inc"),
+            pass_int=nfl_stats_dict.get("pass_int"),
+            pass_int_td=nfl_stats_dict.get("pass_int_td"),
+            pass_lng=nfl_stats_dict.get("pass_lng"),
+            pass_rtg=nfl_stats_dict.get("pass_rtg"),
+            pass_rz_att=nfl_stats_dict.get("pass_rz_att"),
+            pass_sack=nfl_stats_dict.get("pass_sack"),
+            pass_sack_yds=nfl_stats_dict.get("pass_sack_yds"),
+            pass_td=nfl_stats_dict.get("pass_td"),
+            pass_td_40p=nfl_stats_dict.get("pass_td_40p"),
+            pass_td_50p=nfl_stats_dict.get("pass_td_50p"),
+            pass_td_lng=nfl_stats_dict.get("pass_td_lng"),
+            pass_yd=nfl_stats_dict.get("pass_yd"),
+            pass_ypa=nfl_stats_dict.get("pass_ypa"),
+            penalty=nfl_stats_dict.get("penalty"),
+            penalty_yd=nfl_stats_dict.get("penalty_yd"),
+            pr=nfl_stats_dict.get("pr"),
+            pr_lng=nfl_stats_dict.get("pr_lng"),
+            pr_yd=nfl_stats_dict.get("pr_yd"),
+            pr_ypa=nfl_stats_dict.get("pr_ypa"),
+            pts_allow=nfl_stats_dict.get("pts_allow"),
+            pts_allow_14_20=nfl_stats_dict.get("pts_allow_14_20"),
+            pts_allow_1_6=nfl_stats_dict.get("pts_allow_1_6"),
+            pts_allow_21_27=nfl_stats_dict.get("pts_allow_21_27"),
+            pts_allow_28_34=nfl_stats_dict.get("pts_allow_28_34"),
+            pts_allow_35p=nfl_stats_dict.get("pts_allow_35p"),
+            pts_allow_7_13=nfl_stats_dict.get("pts_allow_7_13"),
+            pts_half_ppr=nfl_stats_dict.get("pts_half_ppr"),
+            pts_ppr=nfl_stats_dict.get("pts_ppr"),
+            pts_std=nfl_stats_dict.get("pts_std"),
+            punt_blkd=nfl_stats_dict.get("punt_blkd"),
+            punt_in_20=nfl_stats_dict.get("punt_in_20"),
+            punt_net_yd=nfl_stats_dict.get("punt_net_yd"),
+            punt_tb=nfl_stats_dict.get("punt_tb"),
+            punt_yds=nfl_stats_dict.get("punt_yds"),
+            punts=nfl_stats_dict.get("punts"),
+            qb_hit=nfl_stats_dict.get("qb_hit"),
+            rec=nfl_stats_dict.get("rec"),
+            rec_0_4=nfl_stats_dict.get("rec_0_4"),
+            rec_10_19=nfl_stats_dict.get("rec_10_19"),
+            rec_20_29=nfl_stats_dict.get("rec_20_29"),
+            rec_2pt=nfl_stats_dict.get("rec_2pt"),
+            rec_30_39=nfl_stats_dict.get("rec_30_39"),
+            rec_40p=nfl_stats_dict.get("rec_40p"),
+            rec_5_9=nfl_stats_dict.get("rec_5_9"),
+            rec_air_yd=nfl_stats_dict.get("rec_air_yd"),
+            rec_drop=nfl_stats_dict.get("rec_drop"),
+            rec_fd=nfl_stats_dict.get("rec_fd"),
+            rec_lng=nfl_stats_dict.get("rec_lng"),
+            rec_rz_tgt=nfl_stats_dict.get("rec_rz_tgt"),
+            rec_td=nfl_stats_dict.get("rec_td"),
+            rec_td_40p=nfl_stats_dict.get("rec_td_40p"),
+            rec_td_50p=nfl_stats_dict.get("rec_td_50p"),
+            rec_td_lng=nfl_stats_dict.get("rec_td_lng"),
+            rec_tgt=nfl_stats_dict.get("rec_tgt"),
+            rec_yar=nfl_stats_dict.get("rec_yar"),
+            rec_yd=nfl_stats_dict.get("rec_yd"),
+            rec_ypr=nfl_stats_dict.get("rec_ypr"),
+            rec_ypt=nfl_stats_dict.get("rec_ypt"),
+            rush_2pt=nfl_stats_dict.get("rush_2pt"),
+            rush_40p=nfl_stats_dict.get("rush_40p"),
+            rush_att=nfl_stats_dict.get("rush_att"),
+            rush_btkl=nfl_stats_dict.get("rush_btkl"),
+            rush_fd=nfl_stats_dict.get("rush_fd"),
+            rush_lng=nfl_stats_dict.get("rush_lng"),
+            rush_rz_att=nfl_stats_dict.get("rush_rz_att"),
+            rush_td=nfl_stats_dict.get("rush_td"),
+            rush_td_40p=nfl_stats_dict.get("rush_td_40p"),
+            rush_td_50p=nfl_stats_dict.get("rush_td_50p"),
+            rush_td_lng=nfl_stats_dict.get("rush_td_lng"),
+            rush_tkl_loss=nfl_stats_dict.get("rush_tkl_loss"),
+            rush_tkl_loss_yd=nfl_stats_dict.get("rush_tkl_loss_yd"),
+            rush_yac=nfl_stats_dict.get("rush_yac"),
+            rush_yd=nfl_stats_dict.get("rush_yd"),
+            rush_ypa=nfl_stats_dict.get("rush_ypa"),
+            sack=nfl_stats_dict.get("sack"),
+            sack_yd=nfl_stats_dict.get("sack_yd"),
+            st_snp=nfl_stats_dict.get("st_snp"),
+            st_td=nfl_stats_dict.get("st_td"),
+            st_tkl_solo=nfl_stats_dict.get("st_tkl_solo"),
+            td=nfl_stats_dict.get("td"),
+            tkl=nfl_stats_dict.get("tkl"),
+            tkl_ast=nfl_stats_dict.get("tkl_ast"),
+            tkl_ast_misc=nfl_stats_dict.get("tkl_ast_misc"),
+            tkl_loss=nfl_stats_dict.get("tkl_loss"),
+            tkl_solo=nfl_stats_dict.get("tkl_solo"),
+            tkl_solo_misc=nfl_stats_dict.get("tkl_solo_misc"),
+            tm_def_snp=nfl_stats_dict.get("tm_def_snp"),
+            tm_off_snp=nfl_stats_dict.get("tm_off_snp"),
+            tm_st_snp=nfl_stats_dict.get("tm_st_snp"),
+            xpa=nfl_stats_dict.get("xpa"),
+            xpm=nfl_stats_dict.get("xpm"),
+            xpmiss=nfl_stats_dict.get("xpmiss"),
+            yds_allow=nfl_stats_dict.get("yds_allow"),
+            yds_allow_200_299=nfl_stats_dict.get("yds_allow_200_299"),
+            yds_allow_300_349=nfl_stats_dict.get("yds_allow_300_349"),
+            yds_allow_350_399=nfl_stats_dict.get("yds_allow_350_399"),
+            yds_allow_400_449=nfl_stats_dict.get("yds_allow_400_449"),
+            yds_allow_450_499=nfl_stats_dict.get("yds_allow_450_499"),
+        )
```

### Comparing `sleeper-1.5.0/sleeper/util/ConfigReader.py` & `sleeper-1.6.0/sleeper/util/ConfigReader.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 import os
 
 
 class ConfigReader:
     """
     Used to read from .properties files
     """
+
     __propertiesFileName = "app.properties"
 
     @classmethod
     def get(cls, section: str, name: str, asType=None) -> str:
-        configParser = configparser.ConfigParser(converters={'list': lambda x: [i.strip() for i in x.split(',')]})
+        configParser = configparser.ConfigParser(
+            converters={"list": lambda x: [i.strip() for i in x.split(",")]}
+        )
         propertiesFilePath = os.path.abspath(
-            os.path.join(os.path.dirname(os.path.realpath(__file__)), f"../{cls.__propertiesFileName}"))
+            os.path.join(
+                os.path.dirname(os.path.realpath(__file__)), f"../{cls.__propertiesFileName}"
+            )
+        )
         configParser.read(propertiesFilePath)
         if asType == list:
             return configParser.getlist(section, name)
         elif asType is None:
             return configParser[section][name]
         else:
             raise ValueError(f"Type conversion for '{asType}' not supported.")
```

### Comparing `sleeper-1.5.0/sleeper/util/CustomFormatter.py` & `sleeper-1.6.0/sleeper/util/CustomFormatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 
 class CustomFormatter(logging.Formatter):
     """
     Logging colored formatter, adapted from https://stackoverflow.com/a/56944256/3638629
     """
 
-    grey = '\x1b[38;21m'
-    blue = '\x1b[38;5;39m'
-    yellow = '\x1b[38;5;226m'
-    red = '\x1b[38;5;196m'
-    bold_red = '\x1b[31;1m'
-    reset = '\x1b[0m'
+    grey = "\x1b[38;21m"
+    blue = "\x1b[38;5;39m"
+    yellow = "\x1b[38;5;226m"
+    red = "\x1b[38;5;196m"
+    bold_red = "\x1b[31;1m"
+    reset = "\x1b[0m"
 
     def __init__(self, formatStr: str, timeFormatStr: str):
         super().__init__()
         self.__formatStr = formatStr
         self.__timeFormatStr = timeFormatStr
         self.FORMATS = {
             logging.DEBUG: self.grey + self.__formatStr + self.reset,
             logging.INFO: self.blue + self.__formatStr + self.reset,
             logging.WARNING: self.yellow + self.__formatStr + self.reset,
             logging.ERROR: self.red + self.__formatStr + self.reset,
-            logging.CRITICAL: self.bold_red + self.__formatStr + self.reset
+            logging.CRITICAL: self.bold_red + self.__formatStr + self.reset,
         }
 
     def format(self, record):
         logFormat = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(logFormat, self.__timeFormatStr)
         return formatter.format(record)
```

### Comparing `sleeper-1.5.0/sleeper/util/CustomLogger.py` & `sleeper-1.6.0/sleeper/util/CustomLogger.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import logging
 import sys
 
 from sleeper.util.CustomFormatter import CustomFormatter
 
 
 class CustomLogger:
-
     @staticmethod
     def getLogger() -> logging.Logger:
         # set up logging
         # https://docs.python.org/3/howto/logging.html
         logger = logging.getLogger("root")
         logger.setLevel(logging.INFO)
         if not logger.hasHandlers():
             # set up handler
             handler = logging.StreamHandler()
             handler.setLevel(logging.INFO)
             handler.setStream(sys.stdout)
             # set up formatter
-            formatter = CustomFormatter("%(asctime)-8s %(levelname)-8s %(message)s", "%Y-%m-%d %H:%M:%S")
+            formatter = CustomFormatter(
+                "%(asctime)-8s %(levelname)-8s %(message)s", "%Y-%m-%d %H:%M:%S"
+            )
             # set in each other
             handler.setFormatter(formatter)
             logger.addHandler(handler)
         return logger
```

### Comparing `sleeper-1.5.0/sleeper.egg-info/PKG-INFO` & `sleeper-1.6.0/sleeper.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleeper
-Version: 1.5.0
+Version: 1.6.0
 Summary: A Python wrapper for the Sleeper API.
 Home-page: https://github.com/joeyagreco/sleeper
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: nfl football sleeper sleeper-api sleeper-fantasy-football fantasy-football wrapper wrapper-api
 Requires-Python: >=3.10
@@ -48,10 +48,17 @@
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
+## Development
+
+_Run these commands from the root folder_
+- Format Code: `./main fmt`
+- Run Unit Tests: `./main test`
+- Generate Coverage Report: `./main cov`
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `sleeper-1.5.0/sleeper.egg-info/SOURCES.txt` & `sleeper-1.6.0/sleeper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 sleeper/__init__.py
 sleeper/_version.py
 sleeper/app.properties
 sleeper.egg-info/PKG-INFO
 sleeper.egg-info/SOURCES.txt
@@ -54,14 +55,15 @@
 sleeper/model/DraftMetadata.py
 sleeper/model/DraftPick.py
 sleeper/model/DraftSettings.py
 sleeper/model/FAABTransaction.py
 sleeper/model/FromPlayoffMatchup.py
 sleeper/model/Game.py
 sleeper/model/League.py
+sleeper/model/LeagueMetadata.py
 sleeper/model/LeagueSettings.py
 sleeper/model/Matchup.py
 sleeper/model/Player.py
 sleeper/model/PlayerDraftPick.py
 sleeper/model/PlayerDraftPickMetadata.py
 sleeper/model/PlayerStats.py
 sleeper/model/PlayerTrend.py
```

### Comparing `sleeper-1.5.0/test/test_api/test_AvatarAPIClient.py` & `sleeper-1.6.0/test/test_api/test_AvatarAPIClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 from sleeper.api.AvatarAPIClient import AvatarAPIClient
 from sleeper.exception.SleeperAPIException import SleeperAPIException
 from test.helper.helper_classes import MockResponse
 
 
 class TestAvatarAPIClient(unittest.TestCase):
-    PATH_TO_TEST_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "files", "api"))
+    PATH_TO_TEST_DIR = os.path.abspath(
+        os.path.join(os.path.dirname(__file__), "..", "files", "api")
+    )
 
     @mock.patch("requests.get")
     def test_get_avatar_happy_path(self, mock_requests_get):
         mock_dict = dict()
         with open(os.path.join(self.PATH_TO_TEST_DIR, "test.png"), "rb") as image:
             f = image.read()
             original_image_bytes = bytearray(f)
@@ -39,15 +41,17 @@
             f = image.read()
             original_image_bytes = bytearray(f)
         mock_response = MockResponse(mock_dict, 200, content=original_image_bytes)
         mock_requests_get.return_value = mock_response
 
         with tempfile.TemporaryDirectory() as temp_dir:
             full_image_path = os.path.join(temp_dir, "tmp.png")
-            AvatarAPIClient.get_avatar(avatar_id="avatar_id", save_to_path=full_image_path, thumbnail=True)
+            AvatarAPIClient.get_avatar(
+                avatar_id="avatar_id", save_to_path=full_image_path, thumbnail=True
+            )
 
             with open(full_image_path, "rb") as image:
                 f = image.read()
                 saved_image_bytes = bytearray(f)
             self.assertEqual(original_image_bytes, saved_image_bytes)
             self.assertTrue(os.path.exists(full_image_path))
```

### Comparing `sleeper-1.5.0/test/test_api/test_DraftAPIClient.py` & `sleeper-1.6.0/test/test_api/test_DraftAPIClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from sleeper.model.DraftSettings import DraftSettings
 from sleeper.model.PlayerDraftPick import PlayerDraftPick
 from sleeper.model.PlayerDraftPickMetadata import PlayerDraftPickMetadata
 from test.helper.helper_classes import MockResponse
 
 
 class TestDraftAPIClient(unittest.TestCase):
-
     @mock.patch("requests.get")
     def test_get_user_drafts_for_year_happy_path(self, mock_requests_get):
         mock_list = [
             {
                 "type": "snake",
                 "status": "complete",
                 "start_time": 1630891562020,
@@ -44,38 +43,36 @@
                     "rounds": 17,
                     "reversal_round": 0,
                     "player_type": 0,
                     "pick_timer": 0,
                     "nomination_timer": 60,
                     "enforce_position_limits": 1,
                     "cpu_autopick": 1,
-                    "alpha_sort": 0
+                    "alpha_sort": 0,
                 },
                 "season_type": "regular",
                 "season": "2021",
-                "metadata": {
-                    "scoring_type": "2qb",
-                    "name": "The Test",
-                    "description": "des"
-                },
+                "metadata": {"scoring_type": "2qb", "name": "The Test", "description": "des"},
                 "league_id": "738979251063275520",
                 "last_picked": 1630897024291,
                 "last_message_time": 1630897024793,
                 "last_message_id": "740439424466202624",
                 "draft_order": {"123": 45},
                 "draft_id": "738979252392919040",
                 "creators": ["12345", "67890"],
                 "created": 1630548892636,
-                "slot_to_roster_id": {"123": 45}
+                "slot_to_roster_id": {"123": 45},
             }
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
-        response = DraftAPIClient.get_user_drafts_for_year(user_id="user_id", sport=Sport.NFL, year="2020")
+        response = DraftAPIClient.get_user_drafts_for_year(
+            user_id="user_id", sport=Sport.NFL, year="2020"
+        )
 
         self.assertIsInstance(response, list)
         self.assertIsInstance(response[0], Draft)
         self.assertEqual(1630548892636, response[0].created)
         self.assertEqual(["12345", "67890"], response[0].creators)
         self.assertEqual("738979252392919040", response[0].draft_id)
         self.assertEqual({"123": 45}, response[0].draft_order)
@@ -116,16 +113,18 @@
     def test_get_user_drafts_for_year_not_found_raises_exception(self, mock_requests_get):
         mock_dict = None
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(ValueError) as context:
             DraftAPIClient.get_user_drafts_for_year(user_id="user_id", sport=Sport.NFL, year="2020")
-        self.assertEqual("Could not get Drafts for user_id 'user_id', sport 'NFL', and year '2020'.",
-                         str(context.exception))
+        self.assertEqual(
+            "Could not get Drafts for user_id 'user_id', sport 'NFL', and year '2020'.",
+            str(context.exception),
+        )
 
     @mock.patch("requests.get")
     def test_get_user_drafts_for_year_non_200_status_code_raises_exception(self, mock_requests_get):
         mock_dict = {}
         mock_response = MockResponse(mock_dict, 404)
         mock_requests_get.return_value = mock_response
 
@@ -153,32 +152,28 @@
                     "rounds": 17,
                     "reversal_round": 0,
                     "player_type": 0,
                     "pick_timer": 0,
                     "nomination_timer": 60,
                     "enforce_position_limits": 1,
                     "cpu_autopick": 1,
-                    "alpha_sort": 0
+                    "alpha_sort": 0,
                 },
                 "season_type": "regular",
                 "season": "2021",
-                "metadata": {
-                    "scoring_type": "2qb",
-                    "name": "The Test",
-                    "description": "des"
-                },
+                "metadata": {"scoring_type": "2qb", "name": "The Test", "description": "des"},
                 "league_id": "738979251063275520",
                 "last_picked": 1630897024291,
                 "last_message_time": 1630897024793,
                 "last_message_id": "740439424466202624",
                 "draft_order": {"123": 45},
                 "draft_id": "738979252392919040",
                 "creators": ["12345", "67890"],
                 "created": 1630548892636,
-                "slot_to_roster_id": {"123": 45}
+                "slot_to_roster_id": {"123": 45},
             }
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = DraftAPIClient.get_drafts_in_league(league_id="12345")
 
@@ -260,32 +255,28 @@
                 "rounds": 17,
                 "reversal_round": 0,
                 "player_type": 0,
                 "pick_timer": 0,
                 "nomination_timer": 60,
                 "enforce_position_limits": 1,
                 "cpu_autopick": 1,
-                "alpha_sort": 0
+                "alpha_sort": 0,
             },
             "season_type": "regular",
             "season": "2021",
-            "metadata": {
-                "scoring_type": "2qb",
-                "name": "The Test",
-                "description": "des"
-            },
+            "metadata": {"scoring_type": "2qb", "name": "The Test", "description": "des"},
             "league_id": "738979251063275520",
             "last_picked": 1630897024291,
             "last_message_time": 1630897024793,
             "last_message_id": "740439424466202624",
             "draft_order": {"123": 45},
             "draft_id": "738979252392919040",
             "creators": ["12345", "67890"],
             "created": 1630548892636,
-            "slot_to_roster_id": {"123": 45}
+            "slot_to_roster_id": {"123": 45},
         }
 
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         response = DraftAPIClient.get_draft(draft_id="12345")
 
@@ -363,18 +354,18 @@
                     "sport": "nfl",
                     "position": "RB",
                     "player_id": "2391",
                     "number": "31",
                     "news_updated": "1513007102037",
                     "last_name": "Johnson",
                     "injury_status": "Out",
-                    "first_name": "David"
+                    "first_name": "David",
                 },
                 "is_keeper": True,
-                "draft_id": "257270643320426496"
+                "draft_id": "257270643320426496",
             }
         ]
 
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = DraftAPIClient.get_player_draft_picks(draft_id="12345", sport=Sport.NFL)
@@ -405,16 +396,18 @@
     def test_get_player_draft_picks_not_found_raises_exception(self, mock_requests_get):
         mock_dict = None
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(ValueError) as context:
             DraftAPIClient.get_player_draft_picks(draft_id="12345", sport=Sport.NFL)
-        self.assertEqual("Could not get PlayerDraftPicks with draft_id '12345' and sport 'NFL'.",
-                         str(context.exception))
+        self.assertEqual(
+            "Could not get PlayerDraftPicks with draft_id '12345' and sport 'NFL'.",
+            str(context.exception),
+        )
 
     @mock.patch("requests.get")
     def test_get_player_draft_picks_non_200_status_code_raises_exception(self, mock_requests_get):
         mock_dict = {}
         mock_response = MockResponse(mock_dict, 404)
         mock_requests_get.return_value = mock_response
 
@@ -427,15 +420,15 @@
         mock_list = [
             {
                 "season": "2021",
                 "round": 3,
                 "roster_id": 1,
                 "previous_owner_id": 1,
                 "owner_id": 4,
-                "draft_id": 726312889421496320
+                "draft_id": 726312889421496320,
             }
         ]
 
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = DraftAPIClient.get_traded_draft_picks(draft_id="12345")
@@ -453,15 +446,17 @@
     def test_get_traded_draft_picks_not_found_raises_exception(self, mock_requests_get):
         mock_dict = None
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(ValueError) as context:
             DraftAPIClient.get_traded_draft_picks(draft_id="12345")
-        self.assertEqual("Could not get traded DraftPicks with draft_id '12345'.", str(context.exception))
+        self.assertEqual(
+            "Could not get traded DraftPicks with draft_id '12345'.", str(context.exception)
+        )
 
     @mock.patch("requests.get")
     def test_get_traded_draft_picks_non_200_status_code_raises_exception(self, mock_requests_get):
         mock_dict = {}
         mock_response = MockResponse(mock_dict, 404)
         mock_requests_get.return_value = mock_response
```

### Comparing `sleeper-1.5.0/test/test_api/test_LeagueAPIClient.py` & `sleeper-1.6.0/test/test_api/test_LeagueAPIClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from sleeper.model.Transaction import Transaction
 from sleeper.model.TransactionSettings import TransactionSettings
 from sleeper.model.User import User
 from test.helper.helper_classes import MockResponse
 
 
 class TestLeagueAPIClient(unittest.TestCase):
-
     @mock.patch("requests.get")
     def test_get_league_happy_path(self, mock_requests_get):
         mock_dict = {
             "total_rosters": 12,
             "status": "in_season",
             "sport": "nfl",
             "shard": 679,
@@ -78,15 +77,15 @@
                 "trade_deadline": 11,
                 "reserve_allow_doubtful": 0,
                 "taxi_deadline": 0,
                 "reserve_allow_na": 0,
                 "taxi_slots": 0,
                 "playoff_type": 0,
                 "last_report": 1,
-                "last_scored_leg": 3
+                "last_scored_leg": 3,
             },
             "season_type": "regular",
             "season": "2022",
             "scoring_settings": {
                 "pass_2pt": 2.0,
                 "pass_int": -1.0,
                 "fgmiss": -1.0,
@@ -181,31 +180,20 @@
                 "yds_allow_100_199": 1.0,
                 "yds_allow_200_299": 1.0,
                 "yds_allow_300_349": 1.0,
                 "yds_allow_350_399": 1.0,
                 "yds_allow_400_449": 1.0,
                 "yds_allow_450_499": 1.0,
                 "yds_allow_500_549": 1.0,
-                "yds_allow_550p": 1.0
+                "yds_allow_550p": 1.0,
             },
-            "roster_positions": [
-                "QB",
-                "RB",
-                "RB",
-                "WR",
-                "TE",
-                "FLEX",
-                "BN"
-            ],
+            "roster_positions": ["QB", "RB", "RB", "WR", "TE", "FLEX", "BN"],
             "previous_league_id": "12345",
             "name": "R2 PooPoo DooDoo",
-            "metadata": {
-                "keeper_deadline": "0",
-                "auto_continue": "off"
-            },
+            "metadata": {"keeper_deadline": "0", "auto_continue": "off"},
             "loser_bracket_id": None,
             "league_id": "854528180957097984",
             "last_read_id": None,
             "last_pinned_message_id": "854538979343712256",
             "last_message_time": 1658185095507,
             "last_message_text_map": None,
             "last_message_id": "854893888614273024",
@@ -214,15 +202,15 @@
             "last_author_id": "444590402142466048",
             "last_author_display_name": "BIGCELL561",
             "last_author_avatar": "9b69495def7b9b9d77e0a0126c22efbe",
             "group_id": None,
             "draft_id": "854528182030835712",
             "company_id": None,
             "bracket_id": None,
-            "avatar": "d4ed6e3ae14b56422de8029566d51234"
+            "avatar": "d4ed6e3ae14b56422de8029566d51234",
         }
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         response = LeagueAPIClient.get_league(league_id="12345")
 
         self.assertIsInstance(response, League)
@@ -365,15 +353,17 @@
         self.assertEqual(5461, response.settings.daily_waivers_days)
         self.assertEqual(0, response.settings.daily_waivers_hour)
         self.assertEqual(17, response.settings.daily_waivers_last_ran)
         self.assertEqual(1, response.settings.disable_adds)
         self.assertEqual(1, response.settings.disable_trades)
         self.assertEqual(0, response.settings.league_average_match)
         self.assertEqual(0, response.settings.playoff_round_type)
-        self.assertEqual(PlayoffRoundType.ONE_WEEK_PER_ROUND, response.settings.playoff_round_type_enum)
+        self.assertEqual(
+            PlayoffRoundType.ONE_WEEK_PER_ROUND, response.settings.playoff_round_type_enum
+        )
         self.assertEqual(0, response.settings.playoff_seed_type)
         self.assertEqual(0, response.settings.playoff_type)
         self.assertEqual(0, response.settings.reserve_allow_cov)
         self.assertEqual(0, response.settings.reserve_allow_dnr)
         self.assertEqual(0, response.settings.reserve_allow_na)
         self.assertEqual(0, response.settings.reserve_allow_sus)
         self.assertEqual(0, response.settings.taxi_allow_vets)
@@ -452,15 +442,15 @@
                     "trade_deadline": 11,
                     "reserve_allow_doubtful": 0,
                     "taxi_deadline": 0,
                     "reserve_allow_na": 0,
                     "taxi_slots": 0,
                     "playoff_type": 0,
                     "last_report": 1,
-                    "last_scored_leg": 3
+                    "last_scored_leg": 3,
                 },
                 "season_type": "regular",
                 "season": "2022",
                 "scoring_settings": {
                     "pass_2pt": 2.0,
                     "pass_int": -1.0,
                     "fgmiss": -1.0,
@@ -555,31 +545,20 @@
                     "yds_allow_100_199": 1.0,
                     "yds_allow_200_299": 1.0,
                     "yds_allow_300_349": 1.0,
                     "yds_allow_350_399": 1.0,
                     "yds_allow_400_449": 1.0,
                     "yds_allow_450_499": 1.0,
                     "yds_allow_500_549": 1.0,
-                    "yds_allow_550p": 1.0
+                    "yds_allow_550p": 1.0,
                 },
-                "roster_positions": [
-                    "QB",
-                    "RB",
-                    "RB",
-                    "WR",
-                    "TE",
-                    "FLEX",
-                    "BN"
-                ],
+                "roster_positions": ["QB", "RB", "RB", "WR", "TE", "FLEX", "BN"],
                 "previous_league_id": "12345",
                 "name": "R2 PooPoo DooDoo",
-                "metadata": {
-                    "keeper_deadline": "0",
-                    "auto_continue": "off"
-                },
+                "metadata": {"keeper_deadline": "0", "auto_continue": "off"},
                 "loser_bracket_id": None,
                 "league_id": "854528180957097984",
                 "last_read_id": None,
                 "last_pinned_message_id": "854538979343712256",
                 "last_message_time": 1658185095507,
                 "last_message_text_map": None,
                 "last_message_id": "854893888614273024",
@@ -588,21 +567,23 @@
                 "last_author_id": "444590402142466048",
                 "last_author_display_name": "BIGCELL561",
                 "last_author_avatar": "9b69495def7b9b9d77e0a0126c22efbe",
                 "group_id": None,
                 "draft_id": "854528182030835712",
                 "company_id": None,
                 "bracket_id": None,
-                "avatar": "d4ed6e3ae14b56422de8029566d51234"
+                "avatar": "d4ed6e3ae14b56422de8029566d51234",
             }
         ]
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
-        response = LeagueAPIClient.get_user_leagues_for_year(user_id="12345", sport=Sport.NFL, year="2020")[0]
+        response = LeagueAPIClient.get_user_leagues_for_year(
+            user_id="12345", sport=Sport.NFL, year="2020"
+        )[0]
 
         self.assertIsInstance(response, League)
         self.assertEqual("d4ed6e3ae14b56422de8029566d51234", response.avatar)
         self.assertEqual("854528182030835712", response.draft_id)
         self.assertEqual("854528180957097984", response.league_id)
         self.assertEqual("R2 PooPoo DooDoo", response.name)
         self.assertEqual("12345", response.previous_league_id)
@@ -740,15 +721,17 @@
         self.assertEqual(5461, response.settings.daily_waivers_days)
         self.assertEqual(0, response.settings.daily_waivers_hour)
         self.assertEqual(17, response.settings.daily_waivers_last_ran)
         self.assertEqual(1, response.settings.disable_adds)
         self.assertEqual(1, response.settings.disable_trades)
         self.assertEqual(0, response.settings.league_average_match)
         self.assertEqual(0, response.settings.playoff_round_type)
-        self.assertEqual(PlayoffRoundType.ONE_WEEK_PER_ROUND, response.settings.playoff_round_type_enum)
+        self.assertEqual(
+            PlayoffRoundType.ONE_WEEK_PER_ROUND, response.settings.playoff_round_type_enum
+        )
         self.assertEqual(0, response.settings.playoff_seed_type)
         self.assertEqual(0, response.settings.playoff_type)
         self.assertEqual(0, response.settings.reserve_allow_cov)
         self.assertEqual(0, response.settings.reserve_allow_dnr)
         self.assertEqual(0, response.settings.reserve_allow_na)
         self.assertEqual(0, response.settings.reserve_allow_sus)
         self.assertEqual(0, response.settings.taxi_allow_vets)
@@ -763,64 +746,60 @@
     def test_get_user_leagues_for_year_not_found_raises_exception(self, mock_requests_get):
         mock_dict = None
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(ValueError) as context:
             LeagueAPIClient.get_user_leagues_for_year(user_id="12345", sport=Sport.NFL, year="2020")
-        self.assertEqual("Could not get user Leagues for user_id '12345', sport 'NFL', and year '2020'.",
-                         str(context.exception))
+        self.assertEqual(
+            "Could not get user Leagues for user_id '12345', sport 'NFL', and year '2020'.",
+            str(context.exception),
+        )
 
     @mock.patch("requests.get")
-    def test_get_user_leagues_for_year_non_200_status_code_raises_exception(self, mock_requests_get):
+    def test_get_user_leagues_for_year_non_200_status_code_raises_exception(
+        self, mock_requests_get
+    ):
         mock_dict = {}
         mock_response = MockResponse(mock_dict, 404)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(HTTPError) as context:
             LeagueAPIClient.get_user_leagues_for_year(user_id="12345", sport=Sport.NFL, year="2020")
         self.assertEqual("404 Client Error", str(context.exception))
 
     @mock.patch("requests.get")
     def test_get_rosters_happy_path(self, mock_requests_get):
         mock_dict = [
             {
                 "taxi": 1,
-                "starters": [
-                    "3163",
-                    "CHI"
-                ],
+                "starters": ["3163", "CHI"],
                 "settings": {
                     "wins": 10,
                     "waiver_position": 10,
                     "waiver_budget_used": 0,
                     "waiver_adjusted": 14,
                     "total_moves": 0,
                     "ties": 0,
                     "ppts_decimal": 64,
                     "ppts": 1934,
                     "losses": 3,
                     "fpts_decimal": 8,
                     "fpts_against_decimal": 4,
                     "fpts_against": 1101,
-                    "fpts": 1611
+                    "fpts": 1611,
                 },
                 "roster_id": 1,
                 "reserve": ["test"],
-                "players": [
-                    "1833",
-                    "CHI"
-                ],
+                "players": ["1833", "CHI"],
                 "player_map": {"test": "t"},
                 "owner_id": "66947650880421888",
-                "metadata": {
-                    "test": "t"
-                },
+                "metadata": {"test": "t"},
                 "league_id": "308857914418823168",
-                "co_owners": 1
+                "co_owners": 1,
             }
         ]
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         response = LeagueAPIClient.get_rosters(league_id="12345")[0]
 
@@ -889,15 +868,15 @@
                 "email": "email",
                 "display_name": "display_name",
                 "deleted": "deleted",
                 "data_updated": "data",
                 "currencies": "currencies",
                 "created": "created",
                 "cookies": "cookies",
-                "avatar": "avatar"
+                "avatar": "avatar",
             }
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = LeagueAPIClient.get_users_in_league(league_id="12345")[0]
 
@@ -942,34 +921,22 @@
             LeagueAPIClient.get_users_in_league(league_id="12345")
         self.assertEqual("404 Client Error", str(context.exception))
 
     @mock.patch("requests.get")
     def test_get_matchups_for_week_happy_path(self, mock_requests_get):
         mock_list = [
             {
-                "starters_points": [
-                    10.04,
-                    20.7
-                ],
-                "starters": [
-                    "421",
-                    "2315"
-                ],
+                "starters_points": [10.04, 20.7],
+                "starters": ["421", "2315"],
                 "roster_id": 1,
                 "points": 74.04,
-                "players_points": {
-                    "NO": -9.0,
-                    "830": 11.2
-                },
-                "players": [
-                    "NO",
-                    "830"
-                ],
+                "players_points": {"NO": -9.0, "830": 11.2},
+                "players": ["NO", "830"],
                 "matchup_id": 5,
-                "custom_points": "cp"
+                "custom_points": "cp",
             }
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = LeagueAPIClient.get_matchups_for_week(league_id="12345", week=1)[0]
 
@@ -987,15 +954,17 @@
     def test_get_matchups_for_week_not_found_raises_exception(self, mock_requests_get):
         mock_dict = None
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(ValueError) as context:
             LeagueAPIClient.get_matchups_for_week(league_id="12345", week=1)
-        self.assertEqual("Could not get Matchups for league_id '12345' and week '1'.", str(context.exception))
+        self.assertEqual(
+            "Could not get Matchups for league_id '12345' and week '1'.", str(context.exception)
+        )
 
     @mock.patch("requests.get")
     def test_get_matchups_for_week_non_200_status_code_raises_exception(self, mock_requests_get):
         mock_dict = {}
         mock_response = MockResponse(mock_dict, 404)
         mock_requests_get.return_value = mock_response
 
@@ -1004,28 +973,22 @@
         self.assertEqual("404 Client Error", str(context.exception))
 
     @mock.patch("requests.get")
     def test_get_winners_bracket_happy_path(self, mock_requests_get):
         mock_list = [
             {
                 "w": 8,
-                "t2_from": {
-                    "l": 5,
-                    "w": 6
-                },
+                "t2_from": {"l": 5, "w": 6},
                 "t2": 4,
-                "t1_from": {
-                    "l": 6,
-                    "w": 5
-                },
+                "t1_from": {"l": 6, "w": 5},
                 "t1": 8,
                 "r": 3,
                 "p": 1,
                 "m": 9,
-                "l": 4
+                "l": 4,
             }
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = LeagueAPIClient.get_winners_bracket(league_id="12345")[0]
 
@@ -1048,15 +1011,17 @@
     def test_get_winners_bracket_not_found_raises_exception(self, mock_requests_get):
         mock_dict = None
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(ValueError) as context:
             LeagueAPIClient.get_winners_bracket(league_id="12345")
-        self.assertEqual("Could not get PlayoffMatchups for league_id '12345'.", str(context.exception))
+        self.assertEqual(
+            "Could not get PlayoffMatchups for league_id '12345'.", str(context.exception)
+        )
 
     @mock.patch("requests.get")
     def test_get_winners_bracket_non_200_status_code_raises_exception(self, mock_requests_get):
         mock_dict = {}
         mock_response = MockResponse(mock_dict, 404)
         mock_requests_get.return_value = mock_response
 
@@ -1065,28 +1030,22 @@
         self.assertEqual("404 Client Error", str(context.exception))
 
     @mock.patch("requests.get")
     def test_get_losers_bracket_happy_path(self, mock_requests_get):
         mock_list = [
             {
                 "w": 8,
-                "t2_from": {
-                    "l": 5,
-                    "w": 6
-                },
+                "t2_from": {"l": 5, "w": 6},
                 "t2": 4,
-                "t1_from": {
-                    "l": 6,
-                    "w": 5
-                },
+                "t1_from": {"l": 6, "w": 5},
                 "t1": 8,
                 "r": 3,
                 "p": 1,
                 "m": 9,
-                "l": 4
+                "l": 4,
             }
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = LeagueAPIClient.get_losers_bracket(league_id="12345")[0]
 
@@ -1109,15 +1068,17 @@
     def test_get_losers_bracket_not_found_raises_exception(self, mock_requests_get):
         mock_dict = None
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(ValueError) as context:
             LeagueAPIClient.get_losers_bracket(league_id="12345")
-        self.assertEqual("Could not get PlayoffMatchups for league_id '12345'.", str(context.exception))
+        self.assertEqual(
+            "Could not get PlayoffMatchups for league_id '12345'.", str(context.exception)
+        )
 
     @mock.patch("requests.get")
     def test_get_losers_bracket_non_200_status_code_raises_exception(self, mock_requests_get):
         mock_dict = {}
         mock_response = MockResponse(mock_dict, 404)
         mock_requests_get.return_value = mock_response
 
@@ -1125,55 +1086,38 @@
             LeagueAPIClient.get_losers_bracket(league_id="12345")
         self.assertEqual("404 Client Error", str(context.exception))
 
     @mock.patch("requests.get")
     def test_get_transactions_happy_path(self, mock_requests_get):
         mock_list = [
             {
-                "waiver_budget": [
-                    {
-                        "sender": 2,
-                        "receiver": 3,
-                        "amount": 55
-                    }
-                ],
+                "waiver_budget": [{"sender": 2, "receiver": 3, "amount": 55}],
                 "type": "free_agent",
                 "transaction_id": "852289191705423872",
                 "status_updated": 1657564087371,
                 "status": "complete",
-                "settings": {
-                    "seq": 1,
-                    "waiver_bid": 1
-                },
-                "roster_ids": [
-                    1
-                ],
+                "settings": {"seq": 1, "waiver_bid": 1},
+                "roster_ids": [1],
                 "metadata": {"test": "t"},
                 "leg": 1,
-                "drops": {
-                    "1234": 1
-                },
+                "drops": {"1234": 1},
                 "draft_picks": [
                     {
                         "season": "2019",
                         "round": 5,
                         "roster_id": 1,
                         "previous_owner_id": 1,
                         "owner_id": 2,
-                        "draft_id": "12345"
+                        "draft_id": "12345",
                     }
                 ],
                 "creator": "342404703486779392",
                 "created": 1657564087371,
-                "consenter_ids": [
-                    1
-                ],
-                "adds": {
-                    "5880": 1
-                }
+                "consenter_ids": [1],
+                "adds": {"5880": 1},
             }
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = LeagueAPIClient.get_transactions(league_id="12345", week=1)[0]
 
@@ -1211,35 +1155,32 @@
     def test_get_transactions_not_found_raises_exception(self, mock_requests_get):
         mock_dict = None
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(ValueError) as context:
             LeagueAPIClient.get_transactions(league_id="12345", week=1)
-        self.assertEqual("Could not get Transactions for league_id '12345' and week '1'.", str(context.exception))
+        self.assertEqual(
+            "Could not get Transactions for league_id '12345' and week '1'.", str(context.exception)
+        )
 
     @mock.patch("requests.get")
     def test_get_transactions_non_200_status_code_raises_exception(self, mock_requests_get):
         mock_dict = {}
         mock_response = MockResponse(mock_dict, 404)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(HTTPError) as context:
             LeagueAPIClient.get_transactions(league_id="12345", week=1)
         self.assertEqual("404 Client Error", str(context.exception))
 
     @mock.patch("requests.get")
     def test_get_traded_picks_happy_path(self, mock_requests_get):
         mock_list = [
-            {
-                "season": "2019",
-                "round": 5,
-                "roster_id": 1,
-                "previous_owner_id": 1,
-                "owner_id": 2}
+            {"season": "2019", "round": 5, "roster_id": 1, "previous_owner_id": 1, "owner_id": 2}
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = LeagueAPIClient.get_traded_picks(league_id="12345")[0]
 
         self.assertIsInstance(response, TradedPick)
@@ -1276,15 +1217,15 @@
             "season_type": "off",
             "season_start_date": "2022-09-08",
             "season": "2022",
             "previous_season": "2021",
             "leg": 0,
             "league_season": "2022",
             "league_create_season": "2022",
-            "display_week": 0
+            "display_week": 0,
         }
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         response = LeagueAPIClient.get_sport_state(sport=Sport.NFL)
 
         self.assertIsInstance(response, SportState)
```

### Comparing `sleeper-1.5.0/test/test_api/test_PlayerAPIClient.py` & `sleeper-1.6.0/test/test_api/test_PlayerAPIClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from sleeper.enum.nfl.NFLTeam import NFLTeam
 from sleeper.model.Player import Player
 from sleeper.model.PlayerTrend import PlayerTrend
 from test.helper.helper_classes import MockResponse
 
 
 class TestPlayerAPIClient(unittest.TestCase):
-
     @mock.patch("requests.get")
     def test_get_all_players_happy_path(self, mock_requests_get):
         mock_dict = {
             "2103": {
                 "player_id": "2103",
                 "number": 60,
                 "years_exp": 1,
@@ -34,17 +33,15 @@
                 "gsis_id": "gsis",
                 "birth_state": "WI",
                 "weight": "285",
                 "status": "Inactive",
                 "practice_description": "practice description",
                 "last_name": "Booth",
                 "hashtag": "#codybooth-NFL-FA-60",
-                "fantasy_positions": [
-                    "OL"
-                ],
+                "fantasy_positions": ["OL"],
                 "position": "OT",
                 "stats_id": 12345,
                 "search_last_name": "booth",
                 "yahoo_id": 27841,
                 "birth_country": "USA",
                 "full_name": "Cody Booth",
                 "age": 27,
@@ -66,15 +63,15 @@
                 "first_name": "Cody",
                 "active": False,
                 "depth_chart_order": 1,
                 "college": "Temple",
                 "rotoworld_id": 12345,
                 "search_rank": 9999999,
                 "search_first_name": "cody",
-                "search_full_name": "codybooth"
+                "search_full_name": "codybooth",
             }
         }
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         response = PlayerAPIClient.get_all_players(sport=Sport.NFL)
 
@@ -147,26 +144,17 @@
         with self.assertRaises(HTTPError) as context:
             PlayerAPIClient.get_all_players(sport=Sport.NFL)
         self.assertEqual("404 Client Error", str(context.exception))
 
     @mock.patch("requests.get")
     def test_get_trending_players_add_happy_path(self, mock_requests_get):
         mock_dict = [
-            {
-                "player_id": "943",
-                "count": 13750
-            },
-            {
-                "player_id": "5284",
-                "count": 8070
-            },
-            {
-                "player_id": "4863",
-                "count": 6139
-            }
+            {"player_id": "943", "count": 13750},
+            {"player_id": "5284", "count": 8070},
+            {"player_id": "4863", "count": 6139},
         ]
 
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         response = PlayerAPIClient.get_trending_players(sport=Sport.NFL, trend_type=TrendType.ADD)
 
@@ -175,26 +163,17 @@
         self.assertIsInstance(response[0], PlayerTrend)
         self.assertEqual("943", response[0].player_id)
         self.assertEqual(13750, response[0].count)
 
     @mock.patch("requests.get")
     def test_get_trending_players_drop_happy_path(self, mock_requests_get):
         mock_dict = [
-            {
-                "player_id": "943",
-                "count": 13750
-            },
-            {
-                "player_id": "5284",
-                "count": 8070
-            },
-            {
-                "player_id": "4863",
-                "count": 6139
-            }
+            {"player_id": "943", "count": 13750},
+            {"player_id": "5284", "count": 8070},
+            {"player_id": "4863", "count": 6139},
         ]
 
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         response = PlayerAPIClient.get_trending_players(sport=Sport.NFL, trend_type=TrendType.DROP)
 
@@ -203,33 +182,25 @@
         self.assertIsInstance(response[0], PlayerTrend)
         self.assertEqual("943", response[0].player_id)
         self.assertEqual(13750, response[0].count)
 
     @mock.patch("requests.get")
     def test_get_trending_players_filters_given(self, mock_requests_get):
         mock_dict = [
-            {
-                "player_id": "943",
-                "count": 13750
-            },
-            {
-                "player_id": "5284",
-                "count": 8070
-            },
-            {
-                "player_id": "4863",
-                "count": 6139
-            }
+            {"player_id": "943", "count": 13750},
+            {"player_id": "5284", "count": 8070},
+            {"player_id": "4863", "count": 6139},
         ]
 
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
-        response = PlayerAPIClient.get_trending_players(sport=Sport.NFL, trend_type=TrendType.ADD, lookback_hours=1,
-                                                        limit=3)
+        response = PlayerAPIClient.get_trending_players(
+            sport=Sport.NFL, trend_type=TrendType.ADD, lookback_hours=1, limit=3
+        )
 
         self.assertIsInstance(response, list)
         self.assertEqual(3, len(response))
         self.assertIsInstance(response[0], PlayerTrend)
         self.assertEqual("943", response[0].player_id)
         self.assertEqual(13750, response[0].count)
```

### Comparing `sleeper-1.5.0/test/test_api/test_UserAPIClient.py` & `sleeper-1.6.0/test/test_api/test_UserAPIClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from sleeper.api.UserAPIClient import UserAPIClient
 from sleeper.model.User import User
 from test.helper.helper_classes import MockResponse
 
 
 class TestUserAPIClient(unittest.TestCase):
-
     @mock.patch("requests.get")
     def test_get_user_happy_path(self, mock_requests_get):
         mock_dict = {
             "verification": "v",
             "username": "username",
             "user_id": "user_id",
             "token": "t",
@@ -28,15 +27,15 @@
             "email": "email",
             "display_name": "display_name",
             "deleted": "deleted",
             "data_updated": "data",
             "currencies": "currencies",
             "created": "created",
             "cookies": "cookies",
-            "avatar": "avatar"
+            "avatar": "avatar",
         }
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         response = UserAPIClient.get_user(user_id="user_id")
 
         self.assertIsInstance(response, User)
@@ -69,15 +68,17 @@
     def test_get_user_username_or_user_id_not_found_raises_exception(self, mock_requests_get):
         mock_dict = None
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         with self.assertRaises(ValueError) as context:
             UserAPIClient.get_user(user_id="user_id")
-        self.assertEqual("Could not find User for username/user_id: 'user_id'.", str(context.exception))
+        self.assertEqual(
+            "Could not find User for username/user_id: 'user_id'.", str(context.exception)
+        )
 
     @mock.patch("requests.get")
     def test_get_user_non_200_status_code_raises_exception(self, mock_requests_get):
         mock_dict = {}
         mock_response = MockResponse(mock_dict, 404)
         mock_requests_get.return_value = mock_response
```

### Comparing `sleeper-1.5.0/test/test_api/test_unofficial/test_UPlayerAPIClient.py` & `sleeper-1.6.0/test/test_api/test_unofficial/test_UPlayerAPIClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,48 +9,46 @@
 from sleeper.enum.nfl import NFLTeam, NFLPosition
 from sleeper.model import PlayerStats, Player
 from sleeper.model.nfl import NFLStats
 from test.helper.helper_classes import MockResponse
 
 
 class TestUPlayerAPIClient(unittest.TestCase):
-    PATH_TO_TEST_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "..", "files", "api"))
+    PATH_TO_TEST_DIR = os.path.abspath(
+        os.path.join(os.path.dirname(__file__), "..", "..", "files", "api")
+    )
 
     @mock.patch("requests.get")
     def test_get_player_stats_no_week_given_happy_path(self, mock_requests_get):
         mock_dict = {
             "team": "LAR",
-            "stats": {
-                "rush_yd": 1.0,
-                "rush_fd": 2.0,
-                "rush_att": 3.0
-            },
+            "stats": {"rush_yd": 1.0, "rush_fd": 2.0, "rush_att": 3.0},
             "sport": "nfl",
             "season_type": "regular",
             "season": "2021",
             "player_id": "1234",
             "player": {
                 "years_exp": 1,
                 "team": "LAR",
                 "position": "WR",
                 "news_updated": 1234,
                 "last_name": "ln",
                 "first_name": "fn",
-                "fantasy_positions": [
-                    "WR"
-                ]
+                "fantasy_positions": ["WR"],
             },
             "game_id": "season",
             "company": "rotowire",
-            "category": "stat"
+            "category": "stat",
         }
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
-        response = UPlayerAPIClient.get_player_stats(sport=Sport.NFL, player_id="1234", season="2021")
+        response = UPlayerAPIClient.get_player_stats(
+            sport=Sport.NFL, player_id="1234", season="2021"
+        )
 
         self.assertIsInstance(response, PlayerStats)
         self.assertEqual(NFLTeam.LAR, response.team)
         self.assertIsInstance(response.stats, NFLStats)
         self.assertEqual(1.0, response.stats.rush_yd)
         self.assertEqual(2.0, response.stats.rush_fd)
         self.assertEqual(3.0, response.stats.rush_att)
@@ -72,43 +70,39 @@
         self.assertEqual(Category.STAT, response.category)
 
     @mock.patch("requests.get")
     def test_get_player_stats_week_is_given_happy_path(self, mock_requests_get):
         mock_dict = {
             "week": 1,
             "team": "LAR",
-            "stats": {
-                "rush_yd": 1.0,
-                "rush_fd": 2.0,
-                "rush_att": 3.0
-            },
+            "stats": {"rush_yd": 1.0, "rush_fd": 2.0, "rush_att": 3.0},
             "sport": "nfl",
             "season_type": "regular",
             "season": "2021",
             "opponent": "SEA",
             "player_id": "1234",
             "player": {
                 "years_exp": 1,
                 "team": "LAR",
                 "position": "WR",
                 "news_updated": 1234,
                 "last_name": "ln",
                 "first_name": "fn",
-                "fantasy_positions": [
-                    "WR"
-                ]
+                "fantasy_positions": ["WR"],
             },
             "game_id": "1234",
             "company": "sportradar",
-            "category": "stat"
+            "category": "stat",
         }
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
-        response = UPlayerAPIClient.get_player_stats(sport=Sport.NFL, player_id="1234", season="2021", week=1)
+        response = UPlayerAPIClient.get_player_stats(
+            sport=Sport.NFL, player_id="1234", season="2021", week=1
+        )
 
         self.assertIsInstance(response, PlayerStats)
         self.assertEqual(NFLTeam.LAR, response.team)
         self.assertIsInstance(response.stats, NFLStats)
         self.assertEqual(1, response.week)
         self.assertEqual(1.0, response.stats.rush_yd)
         self.assertEqual(2.0, response.stats.rush_fd)
@@ -131,42 +125,38 @@
         self.assertEqual(Category.STAT, response.category)
         self.assertEqual(NFLTeam.SEA, response.opponent)
 
     @mock.patch("requests.get")
     def test_get_player_projections_no_week_given_happy_path(self, mock_requests_get):
         mock_dict = {
             "team": "LAR",
-            "stats": {
-                "rush_yd": 1.0,
-                "rush_fd": 2.0,
-                "rush_att": 3.0
-            },
+            "stats": {"rush_yd": 1.0, "rush_fd": 2.0, "rush_att": 3.0},
             "sport": "nfl",
             "season_type": "regular",
             "season": "2021",
             "player_id": "1234",
             "player": {
                 "years_exp": 1,
                 "team": "LAR",
                 "position": "WR",
                 "news_updated": 1234,
                 "last_name": "ln",
                 "first_name": "fn",
-                "fantasy_positions": [
-                    "WR"
-                ]
+                "fantasy_positions": ["WR"],
             },
             "game_id": "season",
             "company": "rotowire",
-            "category": "proj"
+            "category": "proj",
         }
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
-        response = UPlayerAPIClient.get_player_projections(sport=Sport.NFL, player_id="1234", season="2021")
+        response = UPlayerAPIClient.get_player_projections(
+            sport=Sport.NFL, player_id="1234", season="2021"
+        )
 
         self.assertIsInstance(response, PlayerStats)
         self.assertEqual(NFLTeam.LAR, response.team)
         self.assertIsInstance(response.stats, NFLStats)
         self.assertEqual(1.0, response.stats.rush_yd)
         self.assertEqual(2.0, response.stats.rush_fd)
         self.assertEqual(3.0, response.stats.rush_att)
@@ -188,43 +178,39 @@
         self.assertEqual(Category.PROJ, response.category)
 
     @mock.patch("requests.get")
     def test_get_player_projections_week_is_given_happy_path(self, mock_requests_get):
         mock_dict = {
             "week": 1,
             "team": "LAR",
-            "stats": {
-                "rush_yd": 1.0,
-                "rush_fd": 2.0,
-                "rush_att": 3.0
-            },
+            "stats": {"rush_yd": 1.0, "rush_fd": 2.0, "rush_att": 3.0},
             "sport": "nfl",
             "season_type": "regular",
             "season": "2021",
             "opponent": "SEA",
             "player_id": "1234",
             "player": {
                 "years_exp": 1,
                 "team": "LAR",
                 "position": "WR",
                 "news_updated": 1234,
                 "last_name": "ln",
                 "first_name": "fn",
-                "fantasy_positions": [
-                    "WR"
-                ]
+                "fantasy_positions": ["WR"],
             },
             "game_id": "1234",
             "company": "sportradar",
-            "category": "proj"
+            "category": "proj",
         }
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
-        response = UPlayerAPIClient.get_player_stats(sport=Sport.NFL, player_id="1234", season="2021", week=1)
+        response = UPlayerAPIClient.get_player_stats(
+            sport=Sport.NFL, player_id="1234", season="2021", week=1
+        )
 
         self.assertIsInstance(response, PlayerStats)
         self.assertEqual(NFLTeam.LAR, response.team)
         self.assertIsInstance(response.stats, NFLStats)
         self.assertEqual(1, response.week)
         self.assertEqual(1.0, response.stats.rush_yd)
         self.assertEqual(2.0, response.stats.rush_fd)
@@ -249,44 +235,40 @@
 
     @mock.patch("requests.get")
     def test_get_all_player_stats_happy_path(self, mock_requests_get):
         mock_list = [
             {
                 "week": 1,
                 "team": "LAR",
-                "stats": {
-                    "rush_yd": 1.0,
-                    "rush_fd": 2.0,
-                    "rush_att": 3.0
-                },
+                "stats": {"rush_yd": 1.0, "rush_fd": 2.0, "rush_att": 3.0},
                 "sport": "nfl",
                 "season_type": "regular",
                 "season": "2021",
                 "opponent": "SEA",
                 "player_id": "1234",
                 "player": {
                     "years_exp": 1,
                     "team": "LAR",
                     "position": "WR",
                     "news_updated": 1234,
                     "last_name": "ln",
                     "first_name": "fn",
-                    "fantasy_positions": [
-                        "WR"
-                    ]
+                    "fantasy_positions": ["WR"],
                 },
                 "game_id": "1234",
                 "company": "sportradar",
-                "category": "stat"
+                "category": "stat",
             }
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
-        response_list = UPlayerAPIClient.get_all_player_stats(sport=Sport.NFL, season="2021", week=1)
+        response_list = UPlayerAPIClient.get_all_player_stats(
+            sport=Sport.NFL, season="2021", week=1
+        )
         response = response_list[0]
 
         self.assertIsInstance(response_list, list)
         self.assertEqual(1, len(response_list))
         self.assertIsInstance(response, PlayerStats)
         self.assertEqual(NFLTeam.LAR, response.team)
         self.assertIsInstance(response.stats, NFLStats)
@@ -314,44 +296,40 @@
 
     @mock.patch("requests.get")
     def test_get_all_player_projections_happy_path(self, mock_requests_get):
         mock_list = [
             {
                 "week": 1,
                 "team": "LAR",
-                "stats": {
-                    "rush_yd": 1.0,
-                    "rush_fd": 2.0,
-                    "rush_att": 3.0
-                },
+                "stats": {"rush_yd": 1.0, "rush_fd": 2.0, "rush_att": 3.0},
                 "sport": "nfl",
                 "season_type": "regular",
                 "season": "2021",
                 "opponent": "SEA",
                 "player_id": "1234",
                 "player": {
                     "years_exp": 1,
                     "team": "LAR",
                     "position": "WR",
                     "news_updated": 1234,
                     "last_name": "ln",
                     "first_name": "fn",
-                    "fantasy_positions": [
-                        "WR"
-                    ]
+                    "fantasy_positions": ["WR"],
                 },
                 "game_id": "1234",
                 "company": "sportradar",
-                "category": "proj"
+                "category": "proj",
             }
         ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
-        response_list = UPlayerAPIClient.get_all_player_projections(sport=Sport.NFL, season="2021", week=1)
+        response_list = UPlayerAPIClient.get_all_player_projections(
+            sport=Sport.NFL, season="2021", week=1
+        )
         response = response_list[0]
 
         self.assertIsInstance(response_list, list)
         self.assertEqual(1, len(response_list))
         self.assertIsInstance(response, PlayerStats)
         self.assertEqual(NFLTeam.LAR, response.team)
         self.assertIsInstance(response.stats, NFLStats)
@@ -383,14 +361,16 @@
             f = image.read()
             original_image_bytes = bytearray(f)
         mock_response = MockResponse(dict(), 200, content=original_image_bytes)
         mock_requests_get.return_value = mock_response
 
         with tempfile.TemporaryDirectory() as temp_dir:
             full_image_path = os.path.join(temp_dir, "tmp.png")
-            UPlayerAPIClient.get_player_head_shot(sport=Sport.NFL, player_id="1234", save_to_path=full_image_path)
+            UPlayerAPIClient.get_player_head_shot(
+                sport=Sport.NFL, player_id="1234", save_to_path=full_image_path
+            )
 
             with open(full_image_path, "rb") as image:
                 f = image.read()
                 saved_image_bytes = bytearray(f)
             self.assertEqual(original_image_bytes, saved_image_bytes)
             self.assertTrue(os.path.exists(full_image_path))
```

### Comparing `sleeper-1.5.0/test/test_api/test_unofficial/test_USportAPIClient.py` & `sleeper-1.6.0/test/test_api/test_unofficial/test_USportAPIClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from sleeper.enum.Sport import Sport
 from sleeper.enum.nfl import NFLTeam
 from sleeper.model import Game
 from test.helper.helper_classes import MockResponse
 
 
 class TestUSportAPIClient(unittest.TestCase):
-
     @mock.patch("requests.get")
     def test_get_player_stats_no_week_given_happy_path(self, mock_requests_get):
         mock_list = [
             {
                 "week": 1,
                 "status": "complete",
                 "home": "ATL",
                 "game_id": "1234",
                 "date": "2021-09-12",
-                "away": "PHI"
-            }]
+                "away": "PHI",
+            }
+        ]
         mock_response = MockResponse(mock_list, 200)
         mock_requests_get.return_value = mock_response
 
         response = USportAPIClient.get_regular_season_schedule(sport=Sport.NFL, season="2021")
 
         self.assertIsInstance(response, list)
         self.assertEqual(1, len(response))
```

### Comparing `sleeper-1.5.0/test/test_api/test_unofficial/test_UTeamAPIClient.py` & `sleeper-1.6.0/test/test_api/test_unofficial/test_UTeamAPIClient.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,118 +5,41 @@
 from sleeper.enum.Sport import Sport
 from sleeper.enum.nfl import NFLTeam
 from sleeper.model.nfl import NFLDepthChart
 from test.helper.helper_classes import MockResponse
 
 
 class TestUSTeamAPIClient(unittest.TestCase):
-
     @mock.patch("requests.get")
     def test_get_team_depth_chart_happy_path(self, mock_requests_get):
         mock_dict = {
-            "WR3": [
-                "1817",
-                "8167"
-            ],
-            "WR2": [
-                "928",
-                "7540",
-                "8235"
-            ],
-            "WR1": [
-                "5185",
-                "8121",
-                "6223"
-            ],
-            "TE": [
-                "4602",
-                "111",
-                "7050"
-            ],
-            "SS": [
-                "2445",
-                "5736",
-                "6355"
-            ],
-            "RT": [
-                "5877",
-                "8511"
-            ],
-            "ROLB": [
-                "5839",
-                "8382"
-            ],
-            "RILB": [
-                "8266",
-                "7782"
-            ],
-            "RG": [
-                "7702",
-                "8460"
-            ],
-            "RDE": [
-                "3220",
-                "8270"
-            ],
-            "RCB": [
-                "7628",
-                "6333"
-            ],
-            "RB": [
-                "4199",
-                "6828"
-            ],
-            "QB": [
-                "96",
-                "6804"
-            ],
-            "PK": [
-                "59"
-            ],
-            "NT": [
-                "3186",
-                "7818",
-                "8344"
-            ],
-            "NB": [
-                "4136",
-                "4223"
-            ],
-            "LT": [
-                "1521",
-                "6008"
-            ],
-            "LOLB": [
-                "2343",
-                "6965",
-                "6981"
-            ],
-            "LILB": [
-                "3276",
-                "7268"
-            ],
-            "LG": [
-                "6980",
-                "8463"
-            ],
-            "LDE": [
-                "3295"
-            ],
-            "LCB": [
-                "4979",
-                "7813"
-            ],
-            "FS": [
-                "6210",
-                "8405"
-            ],
-            "C": [
-                "7645",
-                "7132"
-            ]
+            "WR3": ["1817", "8167"],
+            "WR2": ["928", "7540", "8235"],
+            "WR1": ["5185", "8121", "6223"],
+            "TE": ["4602", "111", "7050"],
+            "SS": ["2445", "5736", "6355"],
+            "RT": ["5877", "8511"],
+            "ROLB": ["5839", "8382"],
+            "RILB": ["8266", "7782"],
+            "RG": ["7702", "8460"],
+            "RDE": ["3220", "8270"],
+            "RCB": ["7628", "6333"],
+            "RB": ["4199", "6828"],
+            "QB": ["96", "6804"],
+            "PK": ["59"],
+            "NT": ["3186", "7818", "8344"],
+            "NB": ["4136", "4223"],
+            "LT": ["1521", "6008"],
+            "LOLB": ["2343", "6965", "6981"],
+            "LILB": ["3276", "7268"],
+            "LG": ["6980", "8463"],
+            "LDE": ["3295"],
+            "LCB": ["4979", "7813"],
+            "FS": ["6210", "8405"],
+            "C": ["7645", "7132"],
         }
         mock_response = MockResponse(mock_dict, 200)
         mock_requests_get.return_value = mock_response
 
         response = UTeamAPIClient.get_team_depth_chart(sport=Sport.NFL, team=NFLTeam.GB)
 
         self.assertIsInstance(response, NFLDepthChart)
```

