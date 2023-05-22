# Comparing `tmp/novel_swarms-0.1.1a0.tar.gz` & `tmp/novel_swarms-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novel_swarms-0.1.1a0.tar", last modified: Wed Apr 19 21:05:51 2023, max compression
+gzip compressed data, was "novel_swarms-0.1.2a0.tar", last modified: Mon May 22 16:06:08 2023, max compression
```

## Comparing `novel_swarms-0.1.1a0.tar` & `novel_swarms-0.1.2a0.tar`

### file list

```diff
@@ -1,125 +1,147 @@
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/
--rw-rw-r--   0 connor    (1001) connor    (1001)      486 2023-04-18 02:45:46.000000 novel_swarms-0.1.1a0/.gitignore
--rw-rw-r--   0 connor    (1001) connor    (1001)     1107 2023-04-19 20:59:13.000000 novel_swarms-0.1.1a0/LICENSE
--rw-rw-r--   0 connor    (1001) connor    (1001)       42 2022-09-19 15:01:24.000000 novel_swarms-0.1.1a0/MANIFEST.in
--rw-rw-r--   0 connor    (1001) connor    (1001)     6944 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/PKG-INFO
--rw-rw-r--   0 connor    (1001) connor    (1001)     6404 2023-03-13 21:19:45.000000 novel_swarms-0.1.1a0/README.md
--rw-rw-r--   0 connor    (1001) connor    (1001)       72 2023-04-17 22:17:05.000000 novel_swarms-0.1.1a0/git.sh
--rw-rw-r--   0 connor    (1001) connor    (1001)      617 2023-04-19 20:58:09.000000 novel_swarms-0.1.1a0/pyproject.toml
--rw-rw-r--   0 connor    (1001) connor    (1001)      480 2023-04-17 17:32:11.000000 novel_swarms-0.1.1a0/requirements.txt
--rw-rw-r--   0 connor    (1001) connor    (1001)       38 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/setup.cfg
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.211975 novel_swarms-0.1.1a0/src/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.1a0/src/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.211975 novel_swarms-0.1.1a0/src/novel_swarms/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-15 20:43:52.000000 novel_swarms-0.1.1a0/src/novel_swarms/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/agent/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1150 2023-03-04 01:07:11.000000 novel_swarms-0.1.1a0/src/novel_swarms/agent/Agent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1070 2023-03-27 22:19:16.000000 novel_swarms-0.1.1a0/src/novel_swarms/agent/AgentFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     6905 2023-04-05 17:20:56.000000 novel_swarms-0.1.1a0/src/novel_swarms/agent/DiffDriveAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4739 2023-04-04 17:55:08.000000 novel_swarms-0.1.1a0/src/novel_swarms/agent/LevyAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     6037 2023-04-04 03:25:20.000000 novel_swarms-0.1.1a0/src/novel_swarms/agent/MazeAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2595 2023-03-04 01:21:09.000000 novel_swarms-0.1.1a0/src/novel_swarms/agent/StaticAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     8166 2023-04-04 02:15:06.000000 novel_swarms-0.1.1a0/src/novel_swarms/agent/UnicycleAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:30.000000 novel_swarms-0.1.1a0/src/novel_swarms/agent/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/behavior/
--rw-rw-r--   0 connor    (1001) connor    (1001)      892 2023-04-04 18:24:20.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/AbstractBehavior.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2085 2023-04-04 14:55:04.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/AgentsAtGoal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1250 2023-03-13 21:54:19.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/AlgebraicConnectivity.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1196 2022-09-16 18:11:09.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/AngularMomentum.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      583 2022-09-16 18:11:09.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/AverageSpeed.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3349 2023-04-18 15:30:56.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/ConvexHull.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1365 2023-04-04 17:37:56.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/DistanceToGoal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1176 2022-09-16 18:11:09.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/GroupRotationBehavior.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1849 2023-04-18 19:46:18.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/PersistentHomology.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1622 2023-03-31 17:32:32.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/RadialVariance.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1134 2022-09-16 18:11:09.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/ScatterBehavior.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      699 2022-10-22 17:04:28.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/SensorOffset.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      548 2022-10-22 17:33:52.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/SensorRotation.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:40.000000 novel_swarms-0.1.1a0/src/novel_swarms/behavior/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/cache/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1681 2023-01-17 23:54:56.000000 novel_swarms-0.1.1a0/src/novel_swarms/cache/ExternalSimulationArchive.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 22:42:03.000000 novel_swarms-0.1.1a0/src/novel_swarms/cache/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/config/
--rw-rw-r--   0 connor    (1001) connor    (1001)     5103 2023-04-04 02:04:33.000000 novel_swarms-0.1.1a0/src/novel_swarms/config/AgentConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1800 2023-03-13 23:06:38.000000 novel_swarms-0.1.1a0/src/novel_swarms/config/EvolutionaryConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      760 2023-03-04 01:41:43.000000 novel_swarms-0.1.1a0/src/novel_swarms/config/HeterogenSwarmConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      637 2023-01-20 15:33:41.000000 novel_swarms-0.1.1a0/src/novel_swarms/config/OutputTensorConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      520 2022-09-15 20:43:52.000000 novel_swarms-0.1.1a0/src/novel_swarms/config/ResultsConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2231 2023-04-04 17:43:06.000000 novel_swarms-0.1.1a0/src/novel_swarms/config/WorldConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:49.000000 novel_swarms-0.1.1a0/src/novel_swarms/config/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1406 2022-10-06 14:01:57.000000 novel_swarms-0.1.1a0/src/novel_swarms/config/defaults.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/gui/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:58.000000 novel_swarms-0.1.1a0/src/novel_swarms/gui/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      391 2022-12-07 17:19:45.000000 novel_swarms-0.1.1a0/src/novel_swarms/gui/abstractGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3216 2023-04-04 19:51:34.000000 novel_swarms-0.1.1a0/src/novel_swarms/gui/agentGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2401 2022-12-07 17:37:58.000000 novel_swarms-0.1.1a0/src/novel_swarms/gui/connectivityGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2670 2022-09-16 18:13:19.000000 novel_swarms-0.1.1a0/src/novel_swarms/gui/evolutionGUI.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/novelty/
--rw-rw-r--   0 connor    (1001) connor    (1001)    10186 2023-03-14 00:06:00.000000 novel_swarms-0.1.1a0/src/novel_swarms/novelty/BehaviorDiscovery.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     7812 2023-03-14 00:05:33.000000 novel_swarms-0.1.1a0/src/novel_swarms/novelty/GeneRule.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3931 2022-10-26 23:42:12.000000 novel_swarms-0.1.1a0/src/novel_swarms/novelty/NoveltyArchive.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:05.000000 novel_swarms-0.1.1a0/src/novel_swarms/novelty/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3834 2023-03-13 23:07:39.000000 novel_swarms-0.1.1a0/src/novel_swarms/novelty/evolve.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/results/
--rw-rw-r--   0 connor    (1001) connor    (1001)     6708 2023-03-13 23:21:09.000000 novel_swarms-0.1.1a0/src/novel_swarms/results/Cluster.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      612 2022-10-10 15:58:53.000000 novel_swarms-0.1.1a0/src/novel_swarms/results/ClusterPoint.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2728 2023-03-13 21:38:40.000000 novel_swarms-0.1.1a0/src/novel_swarms/results/Trends.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:12.000000 novel_swarms-0.1.1a0/src/novel_swarms/results/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4590 2023-04-19 21:01:00.000000 novel_swarms-0.1.1a0/src/novel_swarms/results/behavior_metrics.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      424 2023-03-13 23:23:49.000000 novel_swarms-0.1.1a0/src/novel_swarms/results/results.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/results/scripts/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.1a0/src/novel_swarms/results/scripts/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4869 2022-09-16 18:58:24.000000 novel_swarms-0.1.1a0/src/novel_swarms/results/scripts/domain_codomain.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/sensors/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1021 2023-01-23 17:59:03.000000 novel_swarms-0.1.1a0/src/novel_swarms/sensors/AbstractSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)    11129 2023-03-13 20:07:34.000000 novel_swarms-0.1.1a0/src/novel_swarms/sensors/BinaryFOVSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3222 2023-01-17 16:42:38.000000 novel_swarms-0.1.1a0/src/novel_swarms/sensors/BinaryLOSSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1779 2023-03-14 00:02:26.000000 novel_swarms-0.1.1a0/src/novel_swarms/sensors/GenomeDependentSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      929 2023-01-23 18:00:12.000000 novel_swarms-0.1.1a0/src/novel_swarms/sensors/SensorSet.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      315 2022-10-27 17:32:39.000000 novel_swarms-0.1.1a0/src/novel_swarms/sensors/StaticSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:21.000000 novel_swarms-0.1.1a0/src/novel_swarms/sensors/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/util/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:29.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/util/collider/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1072 2023-03-04 01:09:15.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/collider/AABB.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2396 2023-03-13 18:33:33.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/collider/AngleSensitiveCC.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1024 2023-04-18 16:06:10.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/collider/CircularCollider.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/collider/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/util/conversion/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1192 2023-03-28 18:39:59.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/conversion/ControllerConverter.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/conversion/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/util/datasets/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1179 2023-04-19 21:01:00.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/datasets/DiffDriveDataset.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1553 2022-09-15 20:43:52.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/datasets/GenomeDataSet.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/datasets/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/util/geometry/
--rw-rw-r--   0 connor    (1001) connor    (1001)     5151 2023-04-17 22:41:54.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/geometry/ConvexHull.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1225 2023-04-05 16:32:12.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/geometry/Point.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1184 2023-04-17 21:58:13.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/geometry/Polygon.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/geometry/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3058 2023-04-19 21:01:00.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/labeler.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/util/processing/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/processing/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1299 2023-04-19 18:17:09.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/processing/multicoreprocessing.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-03-30 19:03:58.000000 novel_swarms-0.1.1a0/src/novel_swarms/util/timer.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/world/
--rw-rw-r--   0 connor    (1001) connor    (1001)    13411 2023-04-04 17:46:14.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/RectangularWorld.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2981 2023-04-04 17:54:38.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/World.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      273 2022-09-19 15:08:06.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/WorldFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      320 2023-01-23 18:54:12.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/WorldObject.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:45.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/world/generation/
--rw-rw-r--   0 connor    (1001) connor    (1001)     5347 2023-01-17 20:19:42.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/generation/Maze.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 17:04:53.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/generation/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/world/goals/
--rw-rw-r--   0 connor    (1001) connor    (1001)      636 2023-03-30 21:05:12.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/goals/Goal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 20:36:43.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/goals/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.215975 novel_swarms-0.1.1a0/src/novel_swarms/world/obstacles/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1225 2023-01-23 18:54:36.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/obstacles/Wall.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 16:14:14.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/obstacles/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4416 2023-04-05 18:07:28.000000 novel_swarms-0.1.1a0/src/novel_swarms/world/simulate.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-04-19 21:05:51.211975 novel_swarms-0.1.1a0/src/novel_swarms.egg-info/
--rw-rw-r--   0 connor    (1001) connor    (1001)     6944 2023-04-19 21:05:51.000000 novel_swarms-0.1.1a0/src/novel_swarms.egg-info/PKG-INFO
--rw-rw-r--   0 connor    (1001) connor    (1001)     3892 2023-04-19 21:05:51.000000 novel_swarms-0.1.1a0/src/novel_swarms.egg-info/SOURCES.txt
--rw-rw-r--   0 connor    (1001) connor    (1001)        1 2023-04-19 21:05:51.000000 novel_swarms-0.1.1a0/src/novel_swarms.egg-info/dependency_links.txt
--rw-rw-r--   0 connor    (1001) connor    (1001)       22 2023-04-19 21:05:51.000000 novel_swarms-0.1.1a0/src/novel_swarms.egg-info/top_level.txt
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/
+-rw-rw-r--   0 connor    (1001) connor    (1001)      486 2023-04-18 02:45:46.000000 novel_swarms-0.1.2a0/.gitignore
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1107 2023-04-19 20:59:13.000000 novel_swarms-0.1.2a0/LICENSE
+-rw-rw-r--   0 connor    (1001) connor    (1001)       42 2022-09-19 15:01:24.000000 novel_swarms-0.1.2a0/MANIFEST.in
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6782 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/PKG-INFO
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6242 2023-04-19 21:16:59.000000 novel_swarms-0.1.2a0/README.md
+-rw-rw-r--   0 connor    (1001) connor    (1001)       72 2023-04-17 22:17:05.000000 novel_swarms-0.1.2a0/git.sh
+-rw-rw-r--   0 connor    (1001) connor    (1001)      617 2023-05-22 16:06:00.000000 novel_swarms-0.1.2a0/pyproject.toml
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1061 2023-04-27 20:54:12.000000 novel_swarms-0.1.2a0/requirements.txt
+-rw-rw-r--   0 connor    (1001) connor    (1001)       38 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/setup.cfg
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.2a0/src/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-15 20:43:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/agent/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1199 2023-05-17 17:50:16.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/Agent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1472 2023-05-19 17:51:10.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/AgentFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7341 2023-04-24 18:59:47.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/DiffDriveAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6651 2023-04-27 23:29:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/DroneAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1208 2023-04-27 17:48:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/HumanAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4726 2023-05-12 20:50:55.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/LevyAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7272 2023-05-19 16:23:44.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/MazeAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      885 2023-05-17 18:40:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/ModeSwitchingAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2595 2023-03-04 01:21:09.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/StaticAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     8166 2023-04-04 02:15:06.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/UnicycleAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:30.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/behavior/
+-rw-rw-r--   0 connor    (1001) connor    (1001)      993 2023-05-18 23:13:24.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AbstractBehavior.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2085 2023-04-04 14:55:04.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AgentsAtGoal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1249 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AlgebraicConnectivity.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1196 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AngularMomentum.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      583 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AverageSpeed.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2604 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/BehaviorFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1340 2023-05-12 16:44:43.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/Centroid.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3349 2023-04-18 15:30:56.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/ConvexHull.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1621 2023-05-03 16:44:51.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/DistanceToGoal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1176 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/GroupRotationBehavior.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1849 2023-04-18 19:46:18.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/PersistentHomology.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1746 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/RadialVariance.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1387 2023-04-24 22:53:06.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/ScatterBehavior.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      700 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorOffset.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorRotation.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1514 2023-04-24 23:01:45.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorSignal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      616 2023-05-18 23:41:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/TotalCollisions.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:40.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/cache/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1681 2023-01-17 23:54:56.000000 novel_swarms-0.1.2a0/src/novel_swarms/cache/ExternalSimulationArchive.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 22:42:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/cache/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/config/
+-rw-rw-r--   0 connor    (1001) connor    (1001)    13756 2023-05-19 17:55:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/AgentConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1800 2023-03-13 23:06:38.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/EvolutionaryConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1513 2023-05-19 16:59:04.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/HeterogenSwarmConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)       56 2023-05-17 17:50:16.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/ModeConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      637 2023-01-20 15:33:41.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/OutputTensorConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      520 2022-09-15 20:43:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/ResultsConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4114 2023-05-19 17:03:21.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/WorldConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:49.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1961 2023-05-19 18:43:55.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/defaults.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/gui/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:58.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      479 2023-05-12 21:01:36.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/abstractGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3431 2023-04-27 22:51:31.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/agentGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2401 2022-12-07 17:37:58.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/connectivityGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4143 2023-05-15 22:49:40.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/controllerGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2670 2022-09-16 18:13:19.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/evolutionGUI.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/novelty/
+-rw-rw-r--   0 connor    (1001) connor    (1001)    10186 2023-03-14 00:06:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/BehaviorDiscovery.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7812 2023-03-14 00:05:33.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/GeneRule.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3931 2022-10-26 23:42:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/NoveltyArchive.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:05.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3834 2023-03-13 23:07:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/evolve.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/optim/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7106 2023-05-16 16:48:55.000000 novel_swarms-0.1.2a0/src/novel_swarms/optim/CMAES.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      113 2023-05-03 18:10:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/optim/OptimVar.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-27 15:37:22.000000 novel_swarms-0.1.2a0/src/novel_swarms/optim/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/results/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6708 2023-03-13 23:21:09.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/Cluster.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      612 2022-10-10 15:58:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/ClusterPoint.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2728 2023-03-13 21:38:40.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/Trends.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4590 2023-04-19 21:01:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/behavior_metrics.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      424 2023-03-13 23:23:49.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/results.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/results/scripts/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/scripts/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4869 2022-09-16 18:58:24.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/scripts/domain_codomain.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/sensors/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1021 2023-01-23 17:59:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/AbstractSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)    13602 2023-05-19 17:20:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/BinaryFOVSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4032 2023-05-19 17:21:38.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/BinaryLOSSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1779 2023-03-14 00:02:26.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/GenomeDependentSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1973 2023-04-27 21:53:05.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/RegionalSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      710 2023-05-19 18:17:23.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/SensorFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1818 2023-05-19 18:16:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/SensorSet.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      319 2023-04-28 19:58:35.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/StaticSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:21.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:29.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1072 2023-03-04 01:09:15.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/AABB.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2396 2023-03-13 18:33:33.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/AngleSensitiveCC.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1024 2023-04-18 16:06:10.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/CircularCollider.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/conversion/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1832 2023-05-17 18:31:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/conversion/ControllerConverter.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/conversion/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1179 2023-04-19 21:01:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/DiffDriveDataset.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1553 2022-09-15 20:43:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/GenomeDataSet.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     5151 2023-04-17 22:41:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/ConvexHull.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1287 2023-05-05 19:12:46.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/Point.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1184 2023-04-17 21:58:13.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/Polygon.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3058 2023-04-19 21:01:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/labeler.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/processing/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/processing/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1707 2023-05-03 20:18:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/processing/multicoreprocessing.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/signal/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1809 2023-04-21 17:51:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/signal/Signal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-21 17:17:09.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/signal/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-03-30 19:03:58.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/timer.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/world/
+-rw-rw-r--   0 connor    (1001) connor    (1001)    16018 2023-05-18 23:51:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/RectangularWorld.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3115 2023-05-18 22:57:09.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/World.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      273 2022-09-19 15:08:06.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/WorldFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1315 2023-05-19 18:23:26.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/WorldIO.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:45.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/src/novel_swarms/world/generation/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     5347 2023-01-17 20:19:42.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/generation/Maze.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 17:04:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/generation/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2165 2023-05-18 23:15:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/Goal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      418 2023-05-19 15:51:16.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/GoalFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1128 2023-05-19 15:45:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/GrowthRegion.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 20:36:43.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/
+-rw-rw-r--   0 connor    (1001) connor    (1001)      313 2023-05-19 15:48:02.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/ObjectFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1507 2023-05-19 15:45:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/Wall.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      320 2023-05-19 15:46:02.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/WorldObject.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 16:14:14.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4977 2023-05-18 23:51:23.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/simulate.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6782 2023-05-22 16:06:08.000000 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/PKG-INFO
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4699 2023-05-22 16:06:08.000000 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/SOURCES.txt
+-rw-rw-r--   0 connor    (1001) connor    (1001)        1 2023-05-22 16:06:08.000000 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/dependency_links.txt
+-rw-rw-r--   0 connor    (1001) connor    (1001)       22 2023-05-22 16:06:08.000000 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/top_level.txt
```

### Comparing `novel_swarms-0.1.1a0/LICENSE` & `novel_swarms-0.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/PKG-INFO` & `novel_swarms-0.1.2a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: novel_swarms
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: A Swarm Simulation Package
 Author-email: Connor Mattson <c.mattson@utah.edu>
 Project-URL: Homepage, https://github.com/Connor-Mattson/RobotSwarmSimulator
 Project-URL: Bug Tracker, https://github.com/Connor-Mattson/RobotSwarmSimulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Novel Behavior Discovery in Computation Free Swarms
-Contributors: Anon. <br>
-Experiments replicated from *Discovery and Exploration of Novel Swarm Behaviors given Limited Robot Capabilities* by Daniel S. Brown, Ryan Turner, Oliver Hennigh, and Steven Loscalzo
+Contributors: Connor Mattson, Daniel S. Brown
 
 ## Required Software
 - Python & Pip
 - External Python Packages as defined in [requirements.txt](requirements.txt) 
 
 ## Setup
 Install Python Packages
```

### Comparing `novel_swarms-0.1.1a0/README.md` & `novel_swarms-0.1.2a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Novel Behavior Discovery in Computation Free Swarms
-Contributors: Anon. <br>
-Experiments replicated from *Discovery and Exploration of Novel Swarm Behaviors given Limited Robot Capabilities* by Daniel S. Brown, Ryan Turner, Oliver Hennigh, and Steven Loscalzo
+Contributors: Connor Mattson, Daniel S. Brown
 
 ## Required Software
 - Python & Pip
 - External Python Packages as defined in [requirements.txt](requirements.txt) 
 
 ## Setup
 Install Python Packages
```

### Comparing `novel_swarms-0.1.1a0/pyproject.toml` & `novel_swarms-0.1.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "novel_swarms"
-version = "0.1.1-alpha"
+version = "0.1.2-alpha"
 authors = [
   { name="Connor Mattson", email="c.mattson@utah.edu" },
 ]
 description = "A Swarm Simulation Package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/agent/Agent.py` & `novel_swarms-0.1.2a0/src/novel_swarms/agent/Agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,8 +39,11 @@
         return self.x_pos + math.cos(self.angle), self.y_pos + math.sin(self.angle)
 
     def attach_agent_to_sensors(self):
         for sensor in self.sensors:
             sensor.parent = self
 
     def get_aabb(self):
+        pass
+
+    def on_key_press(self, event):
         pass
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/agent/DiffDriveAgent.py` & `novel_swarms-0.1.2a0/src/novel_swarms/agent/DroneAgent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-from typing import Tuple
-import pygame
 import random
 import math
+import pygame
 import numpy as np
+from typing import Tuple
 from copy import deepcopy
-from .Agent import Agent
-from ..config.AgentConfig import DiffDriveAgentConfig
-from ..sensors.GenomeDependentSensor import GenomeBinarySensor
-from ..util.collider.AABB import AABB
-from ..util.collider.CircularCollider import CircularCollider
-from ..util.timer import Timer
+from src.novel_swarms.agent.Agent import Agent
+from src.novel_swarms.config.AgentConfig import DroneAgentConfig
+from src.novel_swarms.sensors.GenomeDependentSensor import GenomeBinarySensor
+from src.novel_swarms.util.collider.AABB import AABB
+from src.novel_swarms.util.collider.CircularCollider import CircularCollider
 
-class DifferentialDriveAgent(Agent):
 
-    SEED = -1
-    DEBUG = False
+class DroneAgent(Agent):
 
-    def __init__(self, config: DiffDriveAgentConfig = None) -> None:
+    DEBUG = False
 
+    def __init__(self, config: DroneAgentConfig, name=None):
         self.controller = config.controller
 
-        if config.seed is not None:
-            self.seed(config.seed)
-
         if config.x is None:
             self.x_pos = random.randint(0 + config.agent_radius, config.world.w - config.agent_radius)
         else:
             self.x_pos = config.x
 
         if config.y is None:
             self.y_pos = random.randint(0 + config.agent_radius, config.world.h - config.agent_radius)
@@ -37,19 +32,20 @@
 
         if config.angle is None:
             self.angle = random.random() * math.pi * 2
         else:
             self.angle = config.angle
 
         self.radius = config.agent_radius
-        self.wheel_radius = config.wheel_radius
         self.dt = config.dt
         self.is_highlighted = False
+        self.deleted = False
         self.body_filled = config.body_filled
         self.agent_in_sight = None
+        self.config = config
 
         # Set Trace Settings if a trace was assigned to this object.
         self.trace = config.trace_length is not None
         if self.trace:
             self.trace_path = []
             self.trace_length = config.trace_length
 
@@ -66,35 +62,27 @@
         self.sensors = deepcopy(config.sensors)
         for sensor in self.sensors:
             if isinstance(sensor, GenomeBinarySensor):
                 sensor.augment_from_genome(config.controller)
 
         self.attach_agent_to_sensors()
 
-    def seed(self, seed):
-        # random.seed(DifferentialDriveAgent.SEED)
-        pass
-
     def step(self, check_for_world_boundaries=None, world=None, check_for_agent_collisions=None) -> None:
 
         if world is None:
             raise Exception("Expected a Valid value for 'World' in step method call")
 
         # timer = Timer("Calculations")
         super().step()
         self.aabb = None
+        delta_x, delta_y, da = self.interpretSensors()
 
-        if world.goals and world.goals[0].agent_achieved_goal(self):
-            vl, vr = 0, 0
-        else:
-            vl, vr = self.interpretSensors()
-
-        self.dx = (self.wheel_radius / 2) * (vl + vr) * math.cos(self.angle)
-        self.dy = (self.wheel_radius / 2) * (vl + vr) * math.sin(self.angle)
-        heading = (vl - vr) / (self.radius * 2)
+        self.dx = delta_x * np.cos(self.angle) - delta_y * np.cos(self.angle)
+        self.dy = delta_x * np.sin(self.angle) - delta_y * np.sin(self.angle)
+        heading = da
 
         old_x_pos = self.x_pos
         old_y_pos = self.y_pos
 
         self.x_pos += self.dx * self.dt
         self.y_pos += self.dy * self.dt
         self.angle += heading * self.dt
@@ -111,15 +99,15 @@
         # timer = timer.check_watch()
 
         self.add_to_trace(self.x_pos, self.y_pos)
 
         # timer = Timer("Sensors")
         for sensor in self.sensors:
             sensor.step(world=world)
-        # timer = timer.check_watch()
+
 
     def draw(self, screen) -> None:
         super().draw(screen)
         for sensor in self.sensors:
             sensor.draw(screen)
 
         # Draw Cell Membrane
@@ -136,19 +124,21 @@
         mag = self.radius * 2
         vec_with_magnitude = ((vec[0] * mag) + tail[0], (vec[1] * mag) + tail[1])
         pygame.draw.line(screen, self.body_color, tail, vec_with_magnitude)
 
         if self.DEBUG:
             self.debug_draw(screen)
 
+
     def interpretSensors(self) -> Tuple:
         sensor_state = self.sensors.getState()
-        vl = self.controller[sensor_state * 2]
-        vr = self.controller[(sensor_state * 2) + 1]
-        return vl, vr
+        vl = self.controller[sensor_state][0]
+        vr = self.controller[sensor_state][1]
+        theta = self.controller[sensor_state][2]
+        return vl, vr, theta
 
     def draw_trace(self, screen):
         if not self.trace:
             return
         for x, y in self.trace_path:
             pygame.draw.circle(screen, self.trace_color, (x, y), 2)
 
@@ -198,8 +188,8 @@
         if not self.aabb:
             top_left = (self.x_pos - self.radius, self.y_pos - self.radius)
             bottom_right = (self.x_pos + self.radius, self.y_pos + self.radius)
             self.aabb = AABB(top_left, bottom_right)
         return self.aabb
 
     def __str__(self) -> str:
-        return "(x: {}, y: {}, r: {}, θ: {})".format(self.x_pos, self.y_pos, self.radius, self.angle)
+        return "(x: {}, y: {}, r: {}, θ: {})".format(self.x_pos, self.y_pos, self.radius, self.angle)
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/agent/LevyAgent.py` & `novel_swarms-0.1.2a0/src/novel_swarms/agent/LevyAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 import pygame
 import random
 import math
 import time
 import numpy as np
 from copy import deepcopy
 
-import scipy.special
-
 from .Agent import Agent
 from .UnicycleAgent import UnicycleAgent
 from ..config.AgentConfig import UnicycleAgentConfig, LevyAgentConfig
 from ..sensors.GenomeDependentSensor import GenomeBinarySensor, GenomeFOVSensor
 from ..util.timer import Timer
 from ..util.collider.AABB import AABB
 from ..util.collider.AngleSensitiveCC import AngleSensitiveCC
-from scipy.special import gamma
+
 
 class LevyAgent(UnicycleAgent):
     def __init__(self, config: LevyAgentConfig = None, name=None) -> None:
         super().__init__(config.unicycle_config)
 
         if config.seed is not None:
             random.seed(config.seed)
@@ -137,11 +135,12 @@
 
     def _sigma(self, beta):
         numer = (self._gamma(1 + beta) * np.sin(np.pi * (beta / 2)))
         denom = (self._gamma((1 + beta) / 2) * beta * np.power(2, ((beta - 1) / 2)))
         return np.power((numer / denom), 1 / beta)
 
     def _gamma(self, z):
+        from scipy.special import gamma
         return gamma(z)
 
     def get_action(self):
         return np.array([self.dx * self.dt, self.dy, self.dt])
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/agent/MazeAgent.py` & `novel_swarms-0.1.2a0/src/novel_swarms/agent/MazeAgent.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import math
 import numpy as np
 from copy import deepcopy
 from .Agent import Agent
 from ..config.AgentConfig import MazeAgentConfig
 from ..sensors.GenomeDependentSensor import GenomeBinarySensor
 from ..util.collider.AABB import AABB
+from ..util.collider.CircularCollider import CircularCollider
 from ..util.timer import Timer
 
 
 class MazeAgent(Agent):
     SEED = -1
 
     def __init__(self, config: MazeAgentConfig = None, name=None) -> None:
@@ -45,14 +46,16 @@
         self.agent_in_sight = None
         self.idiosyncrasies = config.idiosyncrasies
         I1_MEAN, I1_SD = 0.93, 0.08
         I2_MEAN, I2_SD = 0.95, 0.06
         self.i_1 = np.random.normal(I1_MEAN, I1_SD) if self.idiosyncrasies else 1.0
         self.i_2 = np.random.normal(I2_MEAN, I2_SD) if self.idiosyncrasies else 1.0
         self.stop_on_collision = config.stop_on_collision
+        self.stop_at_goal = config.stop_at_goal
+        self.config = config
 
         self.sensors = deepcopy(config.sensors)
         for sensor in self.sensors:
             if isinstance(sensor, GenomeBinarySensor):
                 sensor.augment_from_genome(config.controller)
 
         self.attach_agent_to_sensors()
@@ -71,17 +74,20 @@
         if world is None:
             raise Exception("Expected a Valid value for 'World' in step method call - Unicycle Agent")
 
         # timer = Timer("Calculations")
         super().step()
 
         if world.goals and world.goals[0].agent_achieved_goal(self) or self.detection_id == 2:
-            v, omega = 0, 0
-            self.detection_id = 2
-            self.set_color_by_id(3)
+            if self.stop_at_goal:
+                v, omega = 0, 0
+            else:
+                v, omega = self.interpretSensors()
+            # self.detection_id = 2
+            # self.set_color_by_id(3)
         else:
             v, omega = self.interpretSensors()
 
         # Define Idiosyncrasies that may occur in actuation/sensing
         idiosync_1 = self.i_1
         idiosync_2 = self.i_2
 
@@ -97,19 +103,19 @@
 
         else:
             self.x_pos += self.dx * self.dt
             self.y_pos += self.dy * self.dt
 
         self.angle += dw * self.dt
 
+        self.collision_flag = False
         if check_for_world_boundaries is not None:
             check_for_world_boundaries(self)
 
-        if check_for_agent_collisions is not None:
-            check_for_agent_collisions(self)
+        self.handle_collisions(world)
 
         # Calculate the 'real' dx, dy after collisions have been calculated.
         # This is what we use for velocity in our equations
         self.dx = self.x_pos - old_x_pos
         self.dy = self.y_pos - old_y_pos
         # timer = timer.check_watch()
 
@@ -135,45 +141,71 @@
         mag = self.radius * 2
         vec_with_magnitude = ((vec[0] * mag) + tail[0], (vec[1] * mag) + tail[1])
         pygame.draw.line(screen, (255, 255, 255), tail, vec_with_magnitude)
 
     def interpretSensors(self) -> Tuple:
         sensor_state = self.sensors.getState()
         sensor_detection_id = self.sensors.getDetectionId()
-        self.set_color_by_id(sensor_detection_id)
+        # self.set_color_by_id(sensor_detection_id)
 
-        if sensor_detection_id == 2:
-            return 12, 0
+        # if sensor_state == 2:
+        #     return 12, 0
 
         v = self.controller[sensor_state * 2]
         omega = self.controller[(sensor_state * 2) + 1]
         return v, omega
 
     def set_color_by_id(self, id):
         if id == 0:
-            self.body_color = (255, 255, 255)
+            self.body_color = self.config.body_color
         elif id == 2:
             self.body_color = (255, 255, 0)
             self.body_filled = True
         elif id == 3:
             self.body_color = (15, 15, 255)
             self.body_filled = True
 
     def get_random_color(self):
         rand_color = [255, 255, 255]
         while sum(rand_color) > 245*3:
             rand_color = np.random.choice(256, 3)
         return rand_color
 
+    def handle_collisions(self, world):
+        collisions = True
+        attempts = 0
+        while collisions and attempts < 10:
+            collisions = False
+            attempts += 1
+            collider = self.build_collider()
+            agent_set = world.getAgentsMatchingYRange(self.get_aabb())
+            for agent in agent_set:
+                if agent.name == self.name:
+                    continue
+                if self.get_aabb().intersects(agent.get_aabb()):
+                    self.collision_flag = True
+                    self.get_aabb().toggle_intersection()
+                    correction = collider.collision_then_correction(agent.build_collider())
+                    if correction is not None:
+                        self.x_pos += correction[0]
+                        self.y_pos += correction[1]
+                        collisions = True
+                        break
+
+    def build_collider(self):
+        return CircularCollider(self.x_pos, self.y_pos, self.radius)
+
     def debug_draw(self, screen):
         self.get_aabb().draw(screen)
 
     def get_aabb(self):
         """
         Return the Bounding Box of the agent
         """
         top_left = (self.x_pos - self.radius, self.y_pos - self.radius)
         bottom_right = (self.x_pos + self.radius, self.y_pos + self.radius)
         return AABB(top_left, bottom_right)
 
+
+
     def __str__(self) -> str:
         return "(x: {}, y: {}, r: {}, θ: {})".format(self.x_pos, self.y_pos, self.radius, self.angle)
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/agent/StaticAgent.py` & `novel_swarms-0.1.2a0/src/novel_swarms/agent/StaticAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/agent/UnicycleAgent.py` & `novel_swarms-0.1.2a0/src/novel_swarms/agent/UnicycleAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/AgentsAtGoal.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/AgentsAtGoal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/AlgebraicConnectivity.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/AlgebraicConnectivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from typing import List
 from .AbstractBehavior import AbstractBehavior
 
 
 class AlgebraicConn(AbstractBehavior):
     def __init__(self, history=100, r_disk_size=10):
-        super().__init__(name="Alg. Connectivity", history_size=history)
+        super().__init__(name="Alg_Connectivity", history_size=history)
         self.population = None
         self.r_disk_size = r_disk_size
 
     def attach_world(self, world):
         self.population = world.population
 
     def getLapacianMatrix(self):
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/AngularMomentum.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/AngularMomentum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from typing import List
 from .AbstractBehavior import AbstractBehavior
 
 class AngularMomentumBehavior(AbstractBehavior):
     def __init__(self, history=100):
-        super().__init__(name="Angular Momentum", history_size=history)
+        super().__init__(name="Angular_Momentum", history_size=history)
         self.population = None
         self.world_radius = 0
 
     def attach_world(self, world):
         self.population = world.population
         self.world_radius = world.config.radius
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/AverageSpeed.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/AverageSpeed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from typing import List
 from .AbstractBehavior import AbstractBehavior
 
 
 class AverageSpeedBehavior(AbstractBehavior):
     def __init__(self, history=100):
-        super().__init__(name="Average Speed", history_size=history)
+        super().__init__(name="Average_Speed", history_size=history)
         self.population = None
 
     def attach_world(self, world):
         self.population = world.population
 
     def calculate(self):
         n = len(self.population)
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/ConvexHull.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/ConvexHull.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/DistanceToGoal.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/DistanceToGoal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 
 import numpy as np
 from typing import List
 from .AbstractBehavior import AbstractBehavior
+from src.novel_swarms.world.goals.Goal import CylinderGoal, AreaGoal
 
 class DistanceToGoal(AbstractBehavior):
 
     def __init__(self, history=100):
         super().__init__(name = "Goal_Dist", history_size=history)
         self.population = None
         self.goals = None
@@ -30,13 +31,16 @@
             self.set_value(np.average(distances))
         else:
             self.set_value(0.0)
 
     def calc_dist_to_goal(self, agent, goal):
         if goal.agent_achieved_goal(agent):
             return 0.0
-        a_pos = [agent.x_pos, agent.y_pos]
-        goal_positions = [goal.rect.topleft, goal.rect.topright, goal.rect.bottomleft, goal.rect.bottomright]
-        dist_squared = []
-        for x, y in goal_positions:
-            dist_squared.append((x - a_pos[0]) ** 2 + (y - a_pos[1]) ** 2)
-        return math.sqrt(min(dist_squared))
+        if isinstance(goal, AreaGoal):
+            a_pos = [agent.x_pos, agent.y_pos]
+            goal_positions = [goal.rect.topleft, goal.rect.topright, goal.rect.bottomleft, goal.rect.bottomright]
+            dist_squared = []
+            for x, y in goal_positions:
+                dist_squared.append((x - a_pos[0]) ** 2 + (y - a_pos[1]) ** 2)
+            return math.sqrt(min(dist_squared))
+        elif isinstance(goal, CylinderGoal):
+            return np.linalg.norm(agent.getPosition() - np.array(goal.center))
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/GroupRotationBehavior.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/GroupRotationBehavior.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from typing import List
 from .AbstractBehavior import AbstractBehavior
 
 class GroupRotationBehavior(AbstractBehavior):
 
     def __init__(self, history=100):
-        super().__init__(name = "Group Rotation", history_size=history)
+        super().__init__(name = "Group_Rotation", history_size=history)
         self.population = None
 
     def attach_world(self, world):
         self.population = world.population
 
     def calculate(self):
         n = len(self.population)
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/PersistentHomology.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/PersistentHomology.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/RadialVariance.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/RadialVariance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import numpy as np
 from typing import List
 from .AbstractBehavior import AbstractBehavior
 
+
 class RadialVarianceBehavior(AbstractBehavior):
-    def __init__(self, history=100):
-        super().__init__(name = "Radial Variance", history_size=history)
+    def __init__(self, history=100, regularize=True):
+        super().__init__(name="Radial_Variance", history_size=history)
         self.population = None
         self.world_radius = 0
+        self.regularize = regularize
 
     def attach_world(self, world):
         self.population = world.population
         self.world_radius = world.config.radius
 
     def calculate(self):
         n = len(self.population)
@@ -25,23 +27,24 @@
             distance_list.append(distance)
         avg_dist = np.average(distance_list)
 
         variance_list = []
         for agent in self.population:
             x_i = agent.getPosition()
             distance = np.linalg.norm(x_i - mew)
-            variance = (distance - avg_dist) ** 2      # Square to make positive(?)
+            variance = (distance - avg_dist) ** 2  # Square to make positive(?)
             variance_list.append(variance)
 
-        radial_variance = sum(variance_list) / (r * r * n)
+        scaling_factor = (1 / (r * r * n)) if self.regularize else (1 / n)
+        radial_variance = sum(variance_list) * scaling_factor
 
         WEIGHT = 20.0
-        self.set_value(radial_variance * WEIGHT)    
+        self.set_value(radial_variance * WEIGHT)
 
     def center_of_mass(self):
         positions = [
             [
                 agent.getPosition()[i] for agent in self.population
             ] for i in range(len(self.population[0].getPosition()))
         ]
         center = np.array([np.average(pos) for pos in positions])
-        return center
+        return center
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/ScatterBehavior.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/ScatterBehavior.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import numpy as np
 from typing import List
 from .AbstractBehavior import AbstractBehavior
 
 
 class ScatterBehavior(AbstractBehavior):
-    def __init__(self, history=100):
+    def __init__(self, history=100, regularize=True):
         super().__init__(name="Scatter", history_size=history)
         self.population = None
         self.world_radius = 0
+        self.regularize = regularize
 
     def attach_world(self, world):
         self.population = world.population
         self.world_radius = world.config.radius
 
     def calculate(self):
         n = len(self.population)
@@ -19,18 +20,25 @@
 
         distance_list = []
         mew = self.center_of_mass()
 
         for agent in self.population:
             x_i = agent.getPosition()
 
-            distance = np.linalg.norm(x_i - mew) ** 2
+            if self.regularize:
+                distance = np.linalg.norm(x_i - mew) ** 2
+            else:
+                distance = np.linalg.norm(x_i - mew)
             distance_list.append(distance)
 
-        scatter = sum(distance_list) / (r * r * n)
+        if self.regularize:
+            scatter = sum(distance_list) / (r * r * n)
+        else:
+            scatter = sum(distance_list) / n
+
         self.set_value(scatter)
 
     def center_of_mass(self):
         positions = [
             [
                 agent.getPosition()[i] for agent in self.population
             ] for i in range(len(self.population[0].getPosition()))
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/SensorOffset.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorOffset.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 from .AbstractBehavior import AbstractBehavior
 
 
 class GeneElementDifference(AbstractBehavior):
 
     def __init__(self, genome_a_index, genome_b_index, history=100):
-        super().__init__(name="SensorOffset", history_size=history)
+        super().__init__(name="Sensor_Offset", history_size=history)
         self.population = 0
         self.a = genome_a_index
         self.b = genome_b_index
 
     def attach_world(self, world):
         self.population = world.population
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/behavior/SensorRotation.py` & `novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorRotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 from .AbstractBehavior import AbstractBehavior
 
 
 class SensorRotation(AbstractBehavior):
 
     def __init__(self, sensor_index, history=100):
-        super().__init__(name="SensorRotation", history_size=history)
+        super().__init__(name="Sensor_Rotation", history_size=history)
         self.population = None
         self.i = sensor_index
 
     def attach_world(self, world):
         self.population = world.population
 
     def calculate(self):
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/cache/ExternalSimulationArchive.py` & `novel_swarms-0.1.2a0/src/novel_swarms/cache/ExternalSimulationArchive.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/config/EvolutionaryConfig.py` & `novel_swarms-0.1.2a0/src/novel_swarms/config/EvolutionaryConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/config/HeterogenSwarmConfig.py` & `novel_swarms-0.1.2a0/src/novel_swarms/config/HeterogenSwarmConfig.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ..agent.AgentFactory import AgentFactory
+from .AgentConfig import AgentConfigFactory
 
 
 class HeterogeneousSwarmConfig:
     def __init__(self):
         self.subpopulation_information = {}
         self.world = None
 
@@ -17,7 +18,33 @@
                 population.append(agent)
         return population
 
     def attach_world_config(self, world_config):
         self.world = world_config
         for key in self.subpopulation_information:
             key.attach_world_config(world_config)
+
+    def as_dict(self):
+        return {
+            "type": "HeterogeneousSwarmConfig",
+            "sub_population_configs": [
+                k.as_dict() for k in self.subpopulation_information.keys()
+            ],
+            "counts": [
+                v for v in self.subpopulation_information.values()
+            ]
+        }
+
+    @staticmethod
+    def from_dict(d):
+        counts = d['counts']
+        configs = []
+        for c in d["sub_population_configs"]:
+            configs.append(AgentConfigFactory.create(c))
+        ret = HeterogeneousSwarmConfig()
+
+        i = 0
+        for config in configs:
+            ret.add_sub_populuation(config, counts[i])
+            i += 1
+
+        return ret
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/config/OutputTensorConfig.py` & `novel_swarms-0.1.2a0/src/novel_swarms/config/OutputTensorConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/config/ResultsConfig.py` & `novel_swarms-0.1.2a0/src/novel_swarms/config/ResultsConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/config/WorldConfig.py` & `novel_swarms-0.1.2a0/src/novel_swarms/config/WorldConfig.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     def __init__(self,
                  size=(500, 500),
                  n_agents=30,
                  seed=None,
                  behavior=None,
                  agentConfig=None,
                  padding=0,
-                 collide_walls=False,
-                 show_walls=False,
+                 collide_walls=True,
+                 show_walls=True,
                  agent_initialization=None,
                  stop_at=None,
                  objects=[],
                  goals=[],
                  background_color=(0, 0, 0),
                  metadata=None,
                  ):
@@ -24,15 +24,16 @@
             behavior = []
 
         self.defined_start = False
         if agent_initialization is not None:
             self.defined_start = True
             self.agent_init = agent_initialization
             if len(agent_initialization) != n_agents:
-                raise Exception(f"Length of Predefined Starting Locations ({len(agent_initialization)}) must equal number of agents ({n_agents})")
+                raise Exception(
+                    f"Length of Predefined Starting Locations ({len(agent_initialization)}) must equal number of agents ({n_agents})")
 
         self.behavior = behavior
         self.w = size[0]
         self.h = size[1]
         self.population_size = n_agents
         self.seed = seed
         self.padding = padding
@@ -63,7 +64,55 @@
             goals=self.goals,
             objects=self.objects
         )
 
     def set_attributes(self, dictionary):
         for key in dictionary:
             setattr(self, key, dictionary[key])
+
+    def as_dict(self):
+        return {
+            "behavior": [b.as_config_dict() for b in self.behavior],
+            "w": self.w,
+            "h": self.h,
+            "population_size": self.population_size,
+            "seed": self.seed,
+            "padding": self.padding,
+            "agent_config": self.agentConfig.as_dict(),
+            "show_walls": self.show_walls,
+            "collide_walls": self.collide_walls,
+            "stop_at": self.stop_at,
+            "objects": [o.as_config_dict() for o in self.objects],
+            "goals": [g.as_config_dict() for g in self.goals],
+            "background_color": self.background_color,
+            "metadata": self.metadata,
+            "agent_init": self.agent_init
+        }
+
+    @staticmethod
+    def from_dict(d):
+        from src.novel_swarms.world.objects.ObjectFactory import ObjectFactory
+        from src.novel_swarms.world.goals.GoalFactory import GoalFactory
+        from src.novel_swarms.behavior.BehaviorFactory import BehaviorFactory
+        from src.novel_swarms.config.AgentConfig import AgentConfigFactory
+
+        objects = [ObjectFactory.create(o) for o in d["objects"]]
+        goals = [GoalFactory.create(g) for g in d["goals"]]
+        behavior = [BehaviorFactory.create(b) for b in d["behavior"]]
+        a_config = AgentConfigFactory.create(d["agent_config"])
+
+        return RectangularWorldConfig(
+            size=(d["w"], d["h"]),
+            behavior=behavior,
+            n_agents=d["population_size"],
+            seed=d["seed"],
+            padding=d["padding"],
+            agentConfig=a_config,
+            show_walls=d["show_walls"],
+            collide_walls=d["collide_walls"],
+            stop_at=d["stop_at"],
+            goals=goals,
+            objects=objects,
+            metadata=d["metadata"],
+            agent_initialization=d["agent_init"]
+        )
+
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/config/defaults.py` & `novel_swarms-0.1.2a0/src/novel_swarms/config/defaults.py`

 * *Files 26% similar despite different names*

```diff
@@ -45,7 +45,24 @@
     )
 
     RESULTS = ResultsConfig(
         k_clusters=10,
         display_trends=False
     )
 
+    FLOCKBOT_SENSOR_SET = SensorSet([
+        BinaryFOVSensor(
+            theta=14 / 2,
+            distance=(15.1 * 13.25),
+            bias=4,
+            degrees=True,
+            false_positive=0.1,
+            false_negative=0.05,
+            # Rectangle Representing Environment Boundaries
+            walls=None,
+            wall_sensing_range=(15.1 * 4),
+            time_step_between_sensing=1,
+            goal_sensing_range=(15.1 * 29.13),
+            detect_goal_with_added_state=True,
+        )
+    ],
+        custom_state_decision="Linear")
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/gui/agentGUI.py` & `novel_swarms-0.1.2a0/src/novel_swarms/gui/agentGUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,15 @@
                 a = self.selected
                 self.appendTextToGUI(screen, f"Current Agent: {a.name}")
                 self.appendTextToGUI(screen, f"")
                 self.appendTextToGUI(screen, f"x: {a.x_pos}")
                 self.appendTextToGUI(screen, f"y: {a.y_pos}")
                 self.appendTextToGUI(screen, f"dx: {a.dx}")
                 self.appendTextToGUI(screen, f"dy: {a.dy}")
+                self.appendTextToGUI(screen, f"sense-state: {a.sensors.getState()}")
                 if hasattr(a, "i_1") and hasattr(a, "i_2"):
                     self.appendTextToGUI(screen, f"Idio_1: {a.i_1}")
                     self.appendTextToGUI(screen, f"Idio_2: {a.i_2}")
                 self.appendTextToGUI(screen, f"")
                 if hasattr(a, "controller"):
                     self.appendTextToGUI(screen, f"controller: {a.controller}")
                     self.appendTextToGUI(screen, f"")
@@ -66,14 +67,16 @@
                 for b in self.world.behavior:
                     out = b.out_average()
                     b.draw(screen)
                     try:
                         self.appendTextToGUI(screen, "{} : {:0.3f}".format(out[0], out[1]))
                     except ValueError as e:
                         pass
+                    except Exception as e:
+                        self.appendTextToGUI(screen, "{} : {}".format(out[0], out[1]))
 
         else:
             print("NO FONT")
 
     def appendTextToGUI(self, screen, text, x=None, y=None, color=(255, 255, 255), aliasing=True, size=16):
 
         if not x:
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/gui/connectivityGUI.py` & `novel_swarms-0.1.2a0/src/novel_swarms/gui/connectivityGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/gui/evolutionGUI.py` & `novel_swarms-0.1.2a0/src/novel_swarms/gui/evolutionGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/novelty/BehaviorDiscovery.py` & `novel_swarms-0.1.2a0/src/novel_swarms/novelty/BehaviorDiscovery.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/novelty/GeneRule.py` & `novel_swarms-0.1.2a0/src/novel_swarms/novelty/GeneRule.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/novelty/NoveltyArchive.py` & `novel_swarms-0.1.2a0/src/novel_swarms/novelty/NoveltyArchive.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/novelty/evolve.py` & `novel_swarms-0.1.2a0/src/novel_swarms/novelty/evolve.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/results/Cluster.py` & `novel_swarms-0.1.2a0/src/novel_swarms/results/Cluster.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/results/ClusterPoint.py` & `novel_swarms-0.1.2a0/src/novel_swarms/results/ClusterPoint.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/results/Trends.py` & `novel_swarms-0.1.2a0/src/novel_swarms/results/Trends.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/results/behavior_metrics.py` & `novel_swarms-0.1.2a0/src/novel_swarms/results/behavior_metrics.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/results/scripts/domain_codomain.py` & `novel_swarms-0.1.2a0/src/novel_swarms/results/scripts/domain_codomain.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/sensors/AbstractSensor.py` & `novel_swarms-0.1.2a0/src/novel_swarms/sensors/AbstractSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/sensors/BinaryFOVSensor.py` & `novel_swarms-0.1.2a0/src/novel_swarms/sensors/BinaryFOVSensor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 import pygame
 import numpy as np
 import math
 from .AbstractSensor import AbstractSensor
 from typing import List
+from ..world.World import World
+from ..world.goals.Goal import CylinderGoal
 
 
 class BinaryFOVSensor(AbstractSensor):
+
     def __init__(self,
                  parent=None,
                  theta=10,
                  distance=100,
                  degrees=False,
                  bias=0.0,
                  false_positive=0.0,
                  false_negative=0.0,
                  walls=None,
+                 goal_sensing_range=10,
                  wall_sensing_range=10,
                  time_step_between_sensing=1,
-                 store_history=False
+                 store_history=False,
+                 detect_goal_with_added_state=False,
                  ):
         super(BinaryFOVSensor, self).__init__(parent=parent)
         self.current_state = 0
         self.angle = 0
         self.theta = theta
         self.bias = bias
         self.fp = false_positive
         self.fn = false_negative
         self.walls = walls
         self.wall_sensing_range = wall_sensing_range
         self.time_step_between_sensing = time_step_between_sensing
         self.time_since_last_sensing = 0
         self.history = []
         self.store_history = store_history
+        self.use_goal_state = detect_goal_with_added_state
+        self.goal_sensing_range = goal_sensing_range
 
         if degrees:
             self.theta = np.deg2rad(self.theta)
             self.bias = np.deg2rad(self.bias)
         self.r = distance
 
-    def checkForLOSCollisions(self, world: object) -> None:
+    def checkForLOSCollisions(self, world: World) -> None:
         # Mathematics obtained from Sundaram Ramaswamy
         # https://legends2k.github.io/2d-fov/design.html
         # See section 3.1.1.2
         self.time_since_last_sensing += 1
         if self.time_since_last_sensing % self.time_step_between_sensing != 0:
             # Our sensing rate occurs less frequently than our dt physics update, so we need to
             #   only check for LOS collisions every n timesteps.
@@ -72,15 +79,16 @@
             wall_bottom = [self.walls[1], [self.walls[0][0], self.walls[1][1]]]
             wall_left = [[self.walls[0][0], self.walls[1][1]], self.walls[0]]
 
             # Brute Check for intersection with each wall
             for wall in [wall_top, wall_right, wall_bottom, wall_left]:
                 for line in [l, r]:
                     if self.lines_segments_intersect(line, wall):
-                        d_to_inter = np.linalg.norm(np.array(self.line_seg_int_point(line, wall)) - np.array(sensor_origin))
+                        d_to_inter = np.linalg.norm(
+                            np.array(self.line_seg_int_point(line, wall)) - np.array(sensor_origin))
                         consideration_set.append((d_to_inter, None))
 
         # Detect for World Objects
         for world_obj in world.objects:
             if not world_obj.detectable:
                 continue
             l = [sensor_origin, sensor_origin + (e_left[:2] * self.wall_sensing_range)]
@@ -90,51 +98,32 @@
                     d_to_inter = np.linalg.norm(np.array(self.line_seg_int_point(segment, l)) - np.array(sensor_origin))
                     consideration_set.append((d_to_inter, None))
 
                 if self.lines_segments_intersect(segment, r):
                     d_to_inter = np.linalg.norm(np.array(self.line_seg_int_point(segment, r)) - np.array(sensor_origin))
                     consideration_set.append((d_to_inter, None))
 
+        # Add this to its own class later -- need to separate the binary from the trinary sensors
+        if self.use_goal_state:
+            for world_goal in world.goals:
+                if isinstance(world_goal, CylinderGoal):
+                    u = np.array(world_goal.center) - sensor_origin
+                    if np.linalg.norm(u) < self.goal_sensing_range + world_goal.r:
+                        d = self.circle_interesect_sensing_cone(u, world_goal.r)
+                        if d is not None:
+                            self.parent.agent_in_sight = None
+                            self.current_state = 2
+                            return
 
         # Detect Other Agents
         for agent in bag:
             u = agent.getPosition() - sensor_origin
-            directional = np.dot(u, self.getLOSVector())
-            if directional > 0:
-                u = np.append(u, [0])
-                cross_l = np.cross(e_left, u)
-                cross_r = np.cross(u, e_right)
-                sign_l = np.sign(cross_l)
-                sign_r = np.sign(cross_r)
-                added_signs = sign_l - sign_r
-                sector_boundaries = np.all(added_signs == 0)
-                if sector_boundaries:
-                    d_to_inter = np.linalg.norm(u)
-                    consideration_set.append((d_to_inter, agent))
-
-                # It may also be the case that the center of the agent is not within the FOV, but that some part of the
-                # circle is visible and on the edges of the left and right viewing vectors.
-                # LinAlg Calculations obtained from https://www.bluebill.net/circle_ray_intersection.html
-
-                # u, defined earlier is the vector from the point of interest to the center of the circle
-                # Project u onto e_left and e_right
-                u_l = np.dot(u, e_left) * e_left
-                u_r = np.dot(u, e_right) * e_right
-
-                # Determine the minimum distance between the agent's center (center of circle) and the projected vector
-                dist_l = np.linalg.norm(u - u_l)
-                dist_r = np.linalg.norm(u - u_r)
-
-                radius = self.parent.radius    # Note: Assumes homogenous radius
-                if dist_l < radius:
-                    d_to_inter = np.linalg.norm(u)
-                    consideration_set.append((d_to_inter, agent))
-                if dist_r < radius:
-                    d_to_inter = np.linalg.norm(u)
-                    consideration_set.append((d_to_inter, agent))
+            d = self.circle_interesect_sensing_cone(u, self.parent.radius)
+            if d is not None:
+                consideration_set.append((d, agent))
 
         if not consideration_set:
             self.determineState(False, None)
             return
 
         # consideration_set.sort()
         # print(consideration_set)
@@ -220,14 +209,16 @@
     def draw(self, screen):
         super(BinaryFOVSensor, self).draw(screen)
 
         # Draw Sensory Vector (Vision Vector)
         sight_color = (255, 0, 0)
         if self.current_state == 1:
             sight_color = (0, 255, 0)
+        if self.current_state == 2:
+            sight_color = (255, 255, 0)
 
         magnitude = self.r if self.parent.is_highlighted else self.parent.radius * 5
 
         head = (self.parent.x_pos, self.parent.y_pos)
         e_left, e_right = self.getSectorVectors()
 
         tail_l = (self.parent.x_pos + (magnitude * e_left[0]),
@@ -239,28 +230,74 @@
         pygame.draw.line(screen, sight_color, head, tail_l)
         pygame.draw.line(screen, sight_color, head, tail_r)
         if self.parent.is_highlighted:
             pygame.draw.circle(screen, sight_color, self.parent.getPosition(), self.r, 3)
             if self.wall_sensing_range:
                 pygame.draw.circle(screen, (150, 150, 150), self.parent.getPosition(), self.wall_sensing_range, 3)
 
+    def circle_interesect_sensing_cone(self, u, r):
+        e_left, e_right = self.getSectorVectors()
+        directional = np.dot(u, self.getBiasedSightAngle())
+        if directional > 0:
+            u = np.append(u, [0])
+            cross_l = np.cross(e_left, u)
+            cross_r = np.cross(u, e_right)
+            sign_l = np.sign(cross_l)
+            sign_r = np.sign(cross_r)
+            added_signs = sign_l - sign_r
+            sector_boundaries = np.all(added_signs == 0)
+            if sector_boundaries:
+                d_to_inter = np.linalg.norm(u)
+                return d_to_inter
+
+            # It may also be the case that the center of the agent is not within the FOV, but that some part of the
+            # circle is visible and on the edges of the left and right viewing vectors.
+            # LinAlg Calculations obtained from https://www.bluebill.net/circle_ray_intersection.html
+
+            # u, defined earlier is the vector from the point of interest to the center of the circle
+            # Project u onto e_left and e_right
+            u_l = np.dot(u, e_left) * e_left
+            u_r = np.dot(u, e_right) * e_right
+
+            # Determine the minimum distance between the agent's center (center of circle) and the projected vector
+            dist_l = np.linalg.norm(u - u_l)
+            dist_r = np.linalg.norm(u - u_r)
+
+            radius = r  # Note: Assumes homogenous radius
+            if dist_l < radius:
+                d_to_inter = np.linalg.norm(u)
+                return d_to_inter
+            if dist_r < radius:
+                d_to_inter = np.linalg.norm(u)
+                return d_to_inter
+        return None
+
     def getDistance(self, a, b):
         return np.linalg.norm(b - a)
 
     def getLOSVector(self) -> List:
         head = self.parent.getPosition()
         tail = self.getFrontalPoint()
         return [tail[0] - head[0], tail[1] - head[1]]
 
     def getFrontalPoint(self):
         if self.angle is None:
             return self.parent.getFrontalPoint()
         return self.parent.x_pos + math.cos(self.angle + self.parent.angle), self.parent.y_pos + math.sin(
             self.angle + self.parent.angle)
 
+    def getBiasedSightAngle(self):
+        bias_transform = np.array([
+            [np.cos(self.bias), -np.sin(self.bias), 0],
+            [np.sin(self.bias), np.cos(self.bias), 0],
+            [0, 0, 1]
+        ])
+        v = np.append(self.getLOSVector(), [0])
+        return np.matmul(bias_transform, v)[:2]
+
     def getSectorVectors(self):
         theta_l = self.theta + self.bias
         theta_r = -self.theta + self.bias
 
         rot_z_left = np.array([
             [np.cos(theta_l), -np.sin(theta_l), 0],
             [np.sin(theta_l), np.cos(theta_l), 0],
@@ -273,7 +310,37 @@
             [0, 0, 1]
         ])
 
         v = np.append(self.getLOSVector(), [0])
         e_left = np.matmul(rot_z_left, v)
         e_right = np.matmul(rot_z_right, v)
         return e_left, e_right
+
+    def as_config_dict(self):
+        return {
+            "type": "BinaryFOVSensor",
+            "theta": self.theta,
+            "bias": self.bias,
+            "fp": self.fp,
+            "fn": self.fn,
+            "time_step_between_sensing": self.time_step_between_sensing,
+            "store_history": self.store_history,
+            "use_goal_state": self.use_goal_state,
+            "wall_sensing_range": self.wall_sensing_range,
+            "goal_sensing_range": self.goal_sensing_range,
+            "agent_sensing_range": self.r,
+        }
+
+    @staticmethod
+    def from_dict(d):
+        return BinaryFOVSensor(
+            parent=None,
+            theta=d["theta"],
+            distance=d["agent_sensing_range"],
+            bias=d["bias"],
+            false_positive=d["fp"],
+            false_negative=d["fn"],
+            store_history=d["store_history"],
+            detect_goal_with_added_state=d["use_goal_state"],
+            wall_sensing_range=d["wall_sensing_range"],
+            goal_sensing_range=d["goal_sensing_range"]
+        )
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/sensors/GenomeDependentSensor.py` & `novel_swarms-0.1.2a0/src/novel_swarms/sensors/GenomeDependentSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/collider/AABB.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/collider/AABB.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/collider/AngleSensitiveCC.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/collider/AngleSensitiveCC.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/collider/CircularCollider.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/collider/CircularCollider.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/conversion/ControllerConverter.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/conversion/ControllerConverter.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,15 +23,33 @@
             v_r = self.from_controller[i + 1]
             forward_velocity = (self.w_rad / 2) * (v_l + v_r)
             d_theta = (v_l - v_r) / (2 * self.a_rad)
             output.append(forward_velocity)
             output.append(d_theta)
         return output
 
+class DiffDriveToRatio(ControllerConverter):
+    """
+    Takes controllers of the Form: [v_l0, vr_0, vl_1, vr_1] and converts it into a ratio?
+    """
+    def __init__(self, controller):
+        super().__init__(controller)
+
+    def convert(self):
+        output = []
+        assert len(self.from_controller) == 4
+        v_r, v_l = self.from_controller[2], self.from_controller[3]
+        v_on = (v_r + v_l) / 2
+        dtheta_on = (v_r - v_l) / 7
+
+        v_r, v_l = self.from_controller[0], self.from_controller[1]
+        v_off = (v_r + v_l) / 2
+        dtheta_off = (v_r - v_l) / 7
+        return [dtheta_on / dtheta_off, v_on / v_off]
 
 if __name__ == "__main__":
     wheel_radius = 2.0
     agent_radius = 5.0
-    input_controller = [-0.7, -1.0, 1.0, -1.0]
+    input_controller = [0.2, 0.7, -0.5, -0.1]
 
     converter = DiffDriveToUnicycle(input_controller, agent_radius, wheel_radius)
     print(converter.convert())
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/datasets/DiffDriveDataset.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/DiffDriveDataset.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/datasets/GenomeDataSet.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/GenomeDataSet.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/geometry/ConvexHull.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/ConvexHull.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/geometry/Point.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/Point.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
     def __hash__(self):
         return hash((self.x, self.y))
 
     def dist(self, other):
         return np.linalg.norm(other.p - self.p)
 
+    def __lt__(self, other):
+        return self.x < other.x
+
     @staticmethod
     def from_agent(agent):
         return Point(agent.x_pos, agent.y_pos)
 
     @staticmethod
     def from_vector(vector):
         return Point(vector[0], vector[1])
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/geometry/Polygon.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/Polygon.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/labeler.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/labeler.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/processing/multicoreprocessing.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/processing/multicoreprocessing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 import warnings
 from multiprocessing import Pool
-from novel_swarms.world.simulate import main as sim
+from src.novel_swarms.world.simulate import main as sim
 
 
 def simulate(world_config, terminate_function, show_gui=False):
     try:
         world = sim(world_config, show_gui=show_gui, stop_detection=terminate_function, step_size=5)
         return world
     except Exception as e:
         warnings.WarningMessage("World could not be simulated: " + str(e))
     return None
 
+def simulate_batch(world_config_list, terminate_function, show_gui=False):
+    ret = []
+    for w in world_config_list:
+        ret.append(simulate(w, terminate_function, show_gui=False))
+    return ret
+
 class MultiWorldSimulation:
     """
     A Multi-Threaded Implementation of the novel_swarms.world.simulate package
     """
 
     def __init__(self, pool_size=4, single_step=False, with_gui=False):
         self.single_step = single_step
         self.with_gui = with_gui
         self.pool_size = pool_size
 
-    def execute(self, world_setup: list, world_stop_condition=None):
+    def execute(self, world_setup: list, world_stop_condition=None, batched=False):
 
         if not world_setup:
             raise Exception("No world_setup list provided to execute.")
 
         ret = []
         if not self.single_step:
             with Pool(self.pool_size) as pool:
-                ret = pool.starmap(simulate, zip(world_setup, [world_stop_condition for _ in world_setup]))
+                ret = pool.starmap(simulate_batch if batched else simulate, zip(world_setup, [world_stop_condition for _ in world_setup]))
         else:
             for w in world_setup:
-                print(w.agentConfig.controller)
-                ret.append(simulate(w, world_stop_condition, show_gui=self.with_gui))
-
+                if batched:
+                    ret.append(simulate_batch(w, world_stop_condition, show_gui=self.with_gui))
+                else:
+                    print(w.agentConfig.controller)
+                    ret.append(simulate(w, world_stop_condition, show_gui=self.with_gui))
         return ret
+
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/util/timer.py` & `novel_swarms-0.1.2a0/src/novel_swarms/util/timer.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/world/RectangularWorld.py` & `novel_swarms-0.1.2a0/src/novel_swarms/world/RectangularWorld.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import math
 import random
 import numpy as np
 from typing import List, Tuple
 import pygame.draw
 from ..agent.Agent import Agent
 from ..agent.DiffDriveAgent import DifferentialDriveAgent
+from .. agent.HumanAgent import HumanDrivenAgent
 from ..config.WorldConfig import RectangularWorldConfig
 from ..agent.AgentFactory import AgentFactory
 from ..config.HeterogenSwarmConfig import HeterogeneousSwarmConfig
 from .World import World
 from ..util.timer import Timer
 from ..util.collider.AABB import AABB
+from .goals.Goal import CylinderGoal
 
 
 def distance(pointA, pointB) -> float:
     return math.dist(pointA, pointB)
 
 
 class RectangularWorld(World):
@@ -26,14 +28,19 @@
         self.config = config
         self.population_size = config.population_size
         self.behavior = config.behavior
         self.padding = config.padding
         self.objects = config.objects
         self.goals = config.goals
         self.seed = config.seed
+
+        self.selected = None
+        self.highlighted_set = []
+        self.human_controlled = []
+
         if config.seed is not None:
             # print(f"World Instantiated with Seed: {config.seed}")
             # print(f"TESTING RAND: {random.random()}")
             random.seed(config.seed)
 
         self.heterogeneous = False
         if isinstance(config.agentConfig, HeterogeneousSwarmConfig):
@@ -45,20 +52,20 @@
                 AgentFactory.create(config.agentConfig, name=f"{i}") for i in range(int(self.population_size))
             ]
 
         ac = config.agentConfig
         if config.defined_start:
             for i in range(len(config.agent_init)):
                 init = config.agent_init[i]
-                noise_x = ((np.random.random() * 2) - 1) * 20
-                noise_y = ((np.random.random() * 2) - 1) * 20
-                noise_theta = ((np.random.random() * 2) - 1) * (np.pi / 8)
-                # noise_x = 0
-                # noise_y = 0
-                # noise_theta = 0
+                # noise_x = ((np.random.random() * 2) - 1) * 20
+                # noise_y = ((np.random.random() * 2) - 1) * 20
+                # noise_theta = ((np.random.random() * 2) - 1) * (np.pi / 8)
+                noise_x = 0
+                noise_y = 0
+                noise_theta = 0
                 self.population[i].x_pos = init[0] + noise_x
                 self.population[i].y_pos = init[1] + noise_y
                 if len(init) > 2:
                     self.population[i].angle = init[2] + noise_theta
 
         elif self.heterogeneous:
             for agent in self.population:
@@ -68,16 +75,14 @@
 
         elif ac.x is None and config.seed is not None:
             for agent in self.population:
                 agent.x_pos = random.uniform(0 + ac.agent_radius, ac.world.w - ac.agent_radius)
                 agent.y_pos = random.uniform(0 + ac.agent_radius, ac.world.h - ac.agent_radius)
                 agent.angle = random.random() * 2 * math.pi
 
-        # print([(a.x_pos, a.y_pos, a.angle) for a in self.population])
-
         for i in range(len(self.objects)):
             self.objects[i].world = self
 
         # Assign Agents Identifiers
         for i, agent in enumerate(self.population):
             agent.name = str(i)
 
@@ -97,14 +102,15 @@
                 raise Exception("Agents must be subtype of Agent, not {}".format(type(agent)))
 
             agent.step(
                 check_for_world_boundaries=self.withinWorldBoundaries if self.config.collide_walls else None,
                 check_for_agent_collisions=self.preventAgentCollisions,
                 world=self
             )
+            self.handleGoalCollisions(agent)
         # agent_step_timer.check_watch()
 
         behavior_timer = Timer("Behavior Calculation Step")
         for behavior in self.behavior:
             behavior.calculate()
         # behavior_timer.check_watch()
 
@@ -142,21 +148,24 @@
                     filtered_agents.append(agent)
         return filtered_agents
 
     def onClick(self, pos) -> None:
         neighborhood = self.getNeighborsWithinDistance(pos, self.population[0].radius)
 
         # Remove Highlights from all agents
-        for n in self.population:
-            n.is_highlighted = False
+        if self.selected is not None:
+            self.selected.is_highlighted = False
 
-        if self.gui is not None and len(neighborhood) == 0:
-            self.gui.set_selected(None)
+        if len(neighborhood) == 0:
+            self.selected = None
+            if self.gui is not None:
+                self.gui.set_selected(None)
             return
 
+        self.selected = neighborhood[0]
         if self.gui is not None:
             self.gui.set_selected(neighborhood[0])
             neighborhood[0].is_highlighted = True
 
     def withinWorldBoundaries(self, agent: DifferentialDriveAgent):
         """
         Set agent position with respect to the world's boundaries and the bounding box of the agent
@@ -174,20 +183,28 @@
         # Prevent Top Collisions
         agent.y_pos = max(agent.radius + padding, agent.y_pos)
 
         # Prevent Bottom Collisions
         agent.y_pos = min((self.bounded_height - agent.radius - padding), agent.y_pos)
 
         # agent.angle += (math.pi / 720)
-        in_coll = self.handleWallCollisions(agent)
+        self.handleWallCollisions(agent)
 
         if agent.x_pos != old_x or agent.y_pos != old_y:
             return True
         return False
 
+    def handleGoalCollisions(self, agent):
+        for goal in self.goals:
+            if isinstance(goal, CylinderGoal):
+                correction = agent.build_collider().collision_then_correction(goal.get_collider())
+                if correction is not None:
+                    agent.x_pos += correction[0]
+                    agent.y_pos += correction[1]
+
     def handleWallCollisions(self, agent: DifferentialDriveAgent):
         # Check for distances between the agent and the line segments
         in_collision = False
         for obj in self.objects:
             segs = obj.get_sensing_segments()
             c = (agent.x_pos, agent.y_pos)
             for p1, p2 in segs:
@@ -265,37 +282,16 @@
 
                 # print(f"Overlap. A: {agent_center}, B: {colliding_agent.getPosition()}")
                 distance_needed = target_distance - center_distance
                 a_to_b = colliding_agent.getPosition() - agent_center
                 b_to_a = agent_center - colliding_agent.getPosition()
 
                 # Check to see if the collision takes place in the forward facing direction
-                if forward_freeze:
-                    heading = agent.getFrontalPoint()
-                    dot = np.dot(a_to_b, heading)
-                    mag_a = np.linalg.norm(a_to_b)
-                    mag_b = np.linalg.norm(heading)
-                    angle = np.arccos(dot / (mag_a * mag_b))
-                    degs = np.degrees(abs(angle))
-                    if degs < 30:
-                        # print(f"Collision at angle {degs}.")
-                        agent.stopped_duration = 2
-                        continue
-
-                    # Now Calculate B_to_A
-                    heading = colliding_agent.getFrontalPoint()
-                    dot = np.dot(b_to_a, heading)
-                    mag_a = np.linalg.norm(b_to_a)
-                    mag_b = np.linalg.norm(heading)
-                    angle = np.arccos(dot / (mag_a * mag_b))
-                    degs = np.degrees(abs(angle))
-                    if degs < 30:
-                        # print(f"Collision at angle {degs}.")
-                        colliding_agent.stopped_duration = 2
-                        continue
+                if forward_freeze and self.collision_forward(agent, colliding_agent):
+                    continue
 
                 # If distance super close to 0, we have a problem. Add noise.
                 SIGNIFICANCE = 0.0001
                 if b_to_a[0] < SIGNIFICANCE and b_to_a[1] < SIGNIFICANCE:
                     MAGNITUDE = 0.001
                     direction = 1
                     if random.random() > 0.5:
@@ -317,20 +313,16 @@
                 # print(base, a_to_b, theta)
                 delta_x = pushback[0]
                 delta_y = pushback[1]
 
                 if math.isnan(delta_x) or math.isnan(delta_y):
                     break
 
-                # print(delta_x, delta_y)
-
                 agent.x_pos += delta_x
                 agent.y_pos += delta_y
-
-                # agent.angle += (math.pi / 720)
                 agent_center = agent.getPosition()
 
             neighborhood = self.getNeighborsWithinDistance(agent_center, minimum_distance, excluded=agent)
             remaining_attempts -= 1
 
     def getAgentsMatchingYRange(self, bb: AABB):
         ret = []
@@ -340,8 +332,84 @@
         return ret
 
     def getBehaviorVector(self):
         behavior = np.array([s.out_average()[1] for s in self.behavior])
         return behavior
 
     def removeAgent(self, agent):
+        agent.deleted = True
         self.population.remove(agent)
+
+    def collision_forward(self, agent, colliding_agent):
+        a_to_b = colliding_agent.getPosition() - agent.getPosition()
+        b_to_a = agent.getPosition() - colliding_agent.getPosition()
+        heading = agent.getFrontalPoint()
+        dot = np.dot(a_to_b, heading)
+        mag_a = np.linalg.norm(a_to_b)
+        mag_b = np.linalg.norm(heading)
+        angle = np.arccos(dot / (mag_a * mag_b))
+        degs = np.degrees(abs(angle))
+        if degs < 30:
+            # print(f"Collision at angle {degs}.")
+            agent.stopped_duration = 2
+            return True
+
+        # Now Calculate B_to_A
+        heading = colliding_agent.getFrontalPoint()
+        dot = np.dot(b_to_a, heading)
+        mag_a = np.linalg.norm(b_to_a)
+        mag_b = np.linalg.norm(heading)
+        angle = np.arccos(dot / (mag_a * mag_b))
+        degs = np.degrees(abs(angle))
+        if degs < 30:
+            # print(f"Collision at angle {degs}.")
+            colliding_agent.stopped_duration = 2
+            return True
+        return False
+
+    def handle_key_press(self, event):
+
+        for a in self.population:
+            a.on_key_press(event)
+
+        if self.selected is not None:
+            if event.key == pygame.K_l:
+                self.selected.simulate_error("Death")
+            if event.key == pygame.K_o:
+                self.selected.simulate_error("Divergence")
+            if event.key == pygame.K_p:
+                self.removeAgent(self.selected)
+            if event.key == pygame.K_a:
+                COLORS = [(247, 146, 86), (146, 220, 229), (235, 185, 223), (251, 209, 162), (99, 105, 209)]
+                self.selected.body_color = COLORS[len(self.highlighted_set) % len(COLORS)]
+                self.selected.is_highlighted = True
+                self.highlighted_set.append(self.selected)
+            if event.key == pygame.K_h:
+                i = self.population.index(self.selected)
+                new_human = HumanDrivenAgent(self.selected.config)
+                new_human.x_pos = self.selected.x_pos
+                new_human.y_pos = self.selected.y_pos
+                new_human.angle = self.selected.angle
+                self.population[i] = new_human
+                self.human_controlled.append(new_human)
+
+        if event.key == pygame.K_c:
+            for agent in self.highlighted_set:
+                agent.is_highlighted = False
+                agent.body_color = agent.config.body_color
+            for agent in self.human_controlled:
+                i = self.population.index(agent)
+                new_bot = DifferentialDriveAgent(agent.config)
+                new_bot.x_pos = agent.x_pos
+                new_bot.y_pos = agent.y_pos
+                new_bot.angle = agent.angle
+                self.population[i] = new_bot
+            self.human_controlled = []
+            self.highlighted_set = []
+
+    def handle_held_keys(self, keys):
+        for agent in self.human_controlled:
+            agent.handle_key_press(keys)
+
+    def as_config_dict(self):
+        return self.config.as_dict()
+
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/world/World.py` & `novel_swarms-0.1.2a0/src/novel_swarms/world/World.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,26 @@
 
     def step(self):
         self.total_steps += 1
 
     def draw(self, screen):
         pass
 
+    def handle_key_press(self, event):
+        pass
+
     def attach_gui(self, gui: AbstractGUI):
         self.gui = gui
 
+    def as_dict(self):
+        pass
+
+    def as_config_dict(self):
+        pass
+
     def evaluate(self, steps: int, output_capture: OutputTensorConfig = None, screen=None):
         frame_markers = []
         output = None
         screen = None
         if output_capture is not None:
             if output_capture.total_frames * output_capture.step > steps:
                 raise Exception("Error: You have indicated an output capture that is larger than the lifespan of the simulation.")
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/world/generation/Maze.py` & `novel_swarms-0.1.2a0/src/novel_swarms/world/generation/Maze.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms/world/simulate.py` & `novel_swarms-0.1.2a0/src/novel_swarms/world/simulate.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ..gui.agentGUI import DifferentialDriveGUI
 from .WorldFactory import WorldFactory
 from ..util.timer import Timer
 
 screen = None
 FRAMERATE = 200
 
-def main(world_config, show_gui=True, gui=None, stop_detection=None, step_size=1):
+def main(world_config, show_gui=True, gui=None, stop_detection=None, world_key_events=False, gui_key_events=False, step_size=1):
     # initialize the pygame module
     if show_gui:
         pygame.init()
         pygame.display.set_caption("Swarm Simulation")
 
     # screen must be global so that other modules can access + draw to the window
     global screen
@@ -48,15 +48,15 @@
     time_me = Timer("World Step")
     while running:
         # Looped Event Handling
         if gui:
             for event in pygame.event.get():
                 # Cancel the game loop if user quits the GUI
                 if event.type == pygame.QUIT:
-                    running = False
+                    return world
                 if event.type == pygame.KEYDOWN:
                     if event.key == pygame.K_SPACE:
                         paused = not paused
                         # print(f"Paused on Simulation Step: {steps_taken}")
                     if event.key == pygame.K_RIGHT and paused:
                         # ON Right Arrow Pressed, draw single frame
                         world.step()
@@ -75,20 +75,32 @@
                         steps_per_frame *= 2
                         steps_per_frame = min(steps_per_frame, 50)
                     if event.key == pygame.K_LSHIFT and steps_per_frame > 1:
                         steps_per_frame /= 2
                         steps_per_frame = round(steps_per_frame)
                     if event.key == pygame.K_w:
                         draw_world = not draw_world
+                    if event.key == pygame.K_F3:
+                        from src.novel_swarms.world.WorldIO import WorldIO
+                        WorldIO.save_world(world)
+                    if world_key_events:
+                        world.handle_key_press(event)
+                    if gui and gui_key_events:
+                        gui.pass_key_events(event)
                     if event.key in labels:
                         return event.key, steps_taken
 
                 if event.type == pygame.MOUSEBUTTONUP:
                     pos = pygame.mouse.get_pos()
                     world.onClick(pos)
+
+            if world_key_events:
+                keys = pygame.key.get_pressed()
+                world.handle_held_keys(keys)
+
             if paused:
                 pygame.time.Clock().tick(FRAMERATE)
                 continue
 
         # Calculate Steps - Stop if we reach desired frame
         for _ in range(steps_per_frame):
 
@@ -109,14 +121,15 @@
 
         # Draw!
         if gui and screen:
             gui.set_time(steps_taken)
             screen.fill(world_config.background_color)
             if draw_world:
                 world.draw(screen)
+            gui.step()
             gui.draw(screen)
 
         # Limit the FPS of the simulation to FRAMERATE
         if gui:
             pygame.display.flip()
             pygame.time.Clock().tick(FRAMERATE)
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms.egg-info/PKG-INFO` & `novel_swarms-0.1.2a0/src/novel_swarms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: novel-swarms
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: A Swarm Simulation Package
 Author-email: Connor Mattson <c.mattson@utah.edu>
 Project-URL: Homepage, https://github.com/Connor-Mattson/RobotSwarmSimulator
 Project-URL: Bug Tracker, https://github.com/Connor-Mattson/RobotSwarmSimulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Novel Behavior Discovery in Computation Free Swarms
-Contributors: Anon. <br>
-Experiments replicated from *Discovery and Exploration of Novel Swarm Behaviors given Limited Robot Capabilities* by Daniel S. Brown, Ryan Turner, Oliver Hennigh, and Steven Loscalzo
+Contributors: Connor Mattson, Daniel S. Brown
 
 ## Required Software
 - Python & Pip
 - External Python Packages as defined in [requirements.txt](requirements.txt) 
 
 ## Setup
 Install Python Packages
```

### Comparing `novel_swarms-0.1.1a0/src/novel_swarms.egg-info/SOURCES.txt` & `novel_swarms-0.1.2a0/src/novel_swarms.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,65 +10,79 @@
 src/novel_swarms.egg-info/PKG-INFO
 src/novel_swarms.egg-info/SOURCES.txt
 src/novel_swarms.egg-info/dependency_links.txt
 src/novel_swarms.egg-info/top_level.txt
 src/novel_swarms/agent/Agent.py
 src/novel_swarms/agent/AgentFactory.py
 src/novel_swarms/agent/DiffDriveAgent.py
+src/novel_swarms/agent/DroneAgent.py
+src/novel_swarms/agent/HumanAgent.py
 src/novel_swarms/agent/LevyAgent.py
 src/novel_swarms/agent/MazeAgent.py
+src/novel_swarms/agent/ModeSwitchingAgent.py
 src/novel_swarms/agent/StaticAgent.py
 src/novel_swarms/agent/UnicycleAgent.py
 src/novel_swarms/agent/__init__.py
 src/novel_swarms/behavior/AbstractBehavior.py
 src/novel_swarms/behavior/AgentsAtGoal.py
 src/novel_swarms/behavior/AlgebraicConnectivity.py
 src/novel_swarms/behavior/AngularMomentum.py
 src/novel_swarms/behavior/AverageSpeed.py
+src/novel_swarms/behavior/BehaviorFactory.py
+src/novel_swarms/behavior/Centroid.py
 src/novel_swarms/behavior/ConvexHull.py
 src/novel_swarms/behavior/DistanceToGoal.py
 src/novel_swarms/behavior/GroupRotationBehavior.py
 src/novel_swarms/behavior/PersistentHomology.py
 src/novel_swarms/behavior/RadialVariance.py
 src/novel_swarms/behavior/ScatterBehavior.py
 src/novel_swarms/behavior/SensorOffset.py
 src/novel_swarms/behavior/SensorRotation.py
+src/novel_swarms/behavior/SensorSignal.py
+src/novel_swarms/behavior/TotalCollisions.py
 src/novel_swarms/behavior/__init__.py
 src/novel_swarms/cache/ExternalSimulationArchive.py
 src/novel_swarms/cache/__init__.py
 src/novel_swarms/config/AgentConfig.py
 src/novel_swarms/config/EvolutionaryConfig.py
 src/novel_swarms/config/HeterogenSwarmConfig.py
+src/novel_swarms/config/ModeConfig.py
 src/novel_swarms/config/OutputTensorConfig.py
 src/novel_swarms/config/ResultsConfig.py
 src/novel_swarms/config/WorldConfig.py
 src/novel_swarms/config/__init__.py
 src/novel_swarms/config/defaults.py
 src/novel_swarms/gui/__init__.py
 src/novel_swarms/gui/abstractGUI.py
 src/novel_swarms/gui/agentGUI.py
 src/novel_swarms/gui/connectivityGUI.py
+src/novel_swarms/gui/controllerGUI.py
 src/novel_swarms/gui/evolutionGUI.py
 src/novel_swarms/novelty/BehaviorDiscovery.py
 src/novel_swarms/novelty/GeneRule.py
 src/novel_swarms/novelty/NoveltyArchive.py
 src/novel_swarms/novelty/__init__.py
 src/novel_swarms/novelty/evolve.py
+src/novel_swarms/optim/CMAES.py
+src/novel_swarms/optim/OptimVar.py
+src/novel_swarms/optim/__init__.py
 src/novel_swarms/results/Cluster.py
 src/novel_swarms/results/ClusterPoint.py
 src/novel_swarms/results/Trends.py
 src/novel_swarms/results/__init__.py
 src/novel_swarms/results/behavior_metrics.py
 src/novel_swarms/results/results.py
 src/novel_swarms/results/scripts/__init__.py
 src/novel_swarms/results/scripts/domain_codomain.py
 src/novel_swarms/sensors/AbstractSensor.py
 src/novel_swarms/sensors/BinaryFOVSensor.py
 src/novel_swarms/sensors/BinaryLOSSensor.py
 src/novel_swarms/sensors/GenomeDependentSensor.py
+src/novel_swarms/sensors/RegionalSensor.py
+src/novel_swarms/sensors/SensorFactory.py
 src/novel_swarms/sensors/SensorSet.py
 src/novel_swarms/sensors/StaticSensor.py
 src/novel_swarms/sensors/__init__.py
 src/novel_swarms/util/__init__.py
 src/novel_swarms/util/labeler.py
 src/novel_swarms/util/timer.py
 src/novel_swarms/util/collider/AABB.py
@@ -82,19 +96,25 @@
 src/novel_swarms/util/datasets/__init__.py
 src/novel_swarms/util/geometry/ConvexHull.py
 src/novel_swarms/util/geometry/Point.py
 src/novel_swarms/util/geometry/Polygon.py
 src/novel_swarms/util/geometry/__init__.py
 src/novel_swarms/util/processing/__init__.py
 src/novel_swarms/util/processing/multicoreprocessing.py
+src/novel_swarms/util/signal/Signal.py
+src/novel_swarms/util/signal/__init__.py
 src/novel_swarms/world/RectangularWorld.py
 src/novel_swarms/world/World.py
 src/novel_swarms/world/WorldFactory.py
-src/novel_swarms/world/WorldObject.py
+src/novel_swarms/world/WorldIO.py
 src/novel_swarms/world/__init__.py
 src/novel_swarms/world/simulate.py
 src/novel_swarms/world/generation/Maze.py
 src/novel_swarms/world/generation/__init__.py
 src/novel_swarms/world/goals/Goal.py
+src/novel_swarms/world/goals/GoalFactory.py
+src/novel_swarms/world/goals/GrowthRegion.py
 src/novel_swarms/world/goals/__init__.py
-src/novel_swarms/world/obstacles/Wall.py
-src/novel_swarms/world/obstacles/__init__.py
+src/novel_swarms/world/objects/ObjectFactory.py
+src/novel_swarms/world/objects/Wall.py
+src/novel_swarms/world/objects/WorldObject.py
+src/novel_swarms/world/objects/__init__.py
```

