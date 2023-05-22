# Comparing `tmp/kathara-3.5.5.tar.gz` & `tmp/kathara-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kathara-3.5.5.tar", last modified: Tue Jan 17 08:32:17 2023, max compression
+gzip compressed data, was "kathara-3.6.0.tar", last modified: Mon May 22 09:27:57 2023, max compression
```

## Comparing `kathara-3.5.5.tar` & `kathara-3.6.0.tar`

### file list

```diff
@@ -1,208 +1,215 @@
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.367628 kathara-3.5.5/
--rw-r--r--   0 skazza     (501) staff       (20)    35141 2020-08-11 14:46:05.000000 kathara-3.5.5/LICENSE
--rw-r--r--   0 skazza     (501) staff       (20)     9081 2023-01-17 08:32:17.367730 kathara-3.5.5/PKG-INFO
--rw-r--r--   0 skazza     (501) staff       (20)     8203 2022-10-11 22:52:11.000000 kathara-3.5.5/README.md
--rw-r--r--   0 skazza     (501) staff       (20)      683 2023-01-17 08:32:17.368012 kathara-3.5.5/setup.cfg
--rw-r--r--   0 skazza     (501) staff       (20)     1608 2023-01-17 05:54:46.000000 kathara-3.5.5/setup.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.346926 kathara-3.5.5/src/
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.347950 kathara-3.5.5/src/Kathara/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.348213 kathara-3.5.5/src/Kathara/auth/
--rw-r--r--   0 skazza     (501) staff       (20)     1650 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/auth/PrivilegeHandler.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/auth/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.348324 kathara-3.5.5/src/Kathara/cli/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/cli/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.350380 kathara-3.5.5/src/Kathara/cli/command/
--rw-r--r--   0 skazza     (501) staff       (20)     2241 2022-06-05 07:57:03.000000 kathara-3.5.5/src/Kathara/cli/command/CheckCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     2522 2022-09-14 21:00:18.000000 kathara-3.5.5/src/Kathara/cli/command/ConnectCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     3069 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/cli/command/ExecCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     1805 2022-09-14 21:00:18.000000 kathara-3.5.5/src/Kathara/cli/command/LcleanCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     3043 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/cli/command/LconfigCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     4607 2022-09-14 21:00:18.000000 kathara-3.5.5/src/Kathara/cli/command/LinfoCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     2496 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/cli/command/ListCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     4503 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/cli/command/LrestartCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     8206 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/cli/command/LstartCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     4508 2022-09-14 21:00:18.000000 kathara-3.5.5/src/Kathara/cli/command/LtestCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)      350 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/cli/command/SettingsCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     1255 2022-06-05 07:57:03.000000 kathara-3.5.5/src/Kathara/cli/command/VcleanCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     2699 2022-09-14 21:00:18.000000 kathara-3.5.5/src/Kathara/cli/command/VconfigCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     6934 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/cli/command/VstartCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)     2218 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/cli/command/WipeCommand.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/cli/command/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.350567 kathara-3.5.5/src/Kathara/cli/ui/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/cli/ui/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.351173 kathara-3.5.5/src/Kathara/cli/ui/event/
--rw-r--r--   0 skazza     (501) staff       (20)     1313 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/cli/ui/event/HandleProgressBar.py
--rw-r--r--   0 skazza     (501) staff       (20)      694 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/cli/ui/event/OpenMachineTerminal.py
--rw-r--r--   0 skazza     (501) staff       (20)     1058 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/cli/ui/event/UpdateDockerImage.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/cli/ui/event/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)     2402 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/cli/ui/event/register.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.351917 kathara-3.5.5/src/Kathara/cli/ui/setting/
--rw-r--r--   0 skazza     (501) staff       (20)    21212 2022-09-14 21:00:18.000000 kathara-3.5.5/src/Kathara/cli/ui/setting/CommonOptionsHandler.py
--rw-r--r--   0 skazza     (501) staff       (20)    13058 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/cli/ui/setting/DockerOptionsHandler.py
--rw-r--r--   0 skazza     (501) staff       (20)     8908 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py
--rw-r--r--   0 skazza     (501) staff       (20)     1483 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/cli/ui/setting/SettingsMenuFactory.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/cli/ui/setting/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)     3828 2022-09-14 21:00:18.000000 kathara-3.5.5/src/Kathara/cli/ui/setting/utils.py
--rw-r--r--   0 skazza     (501) staff       (20)     5779 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/cli/ui/utils.py
--rw-r--r--   0 skazza     (501) staff       (20)      623 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/decorators.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.352137 kathara-3.5.5/src/Kathara/event/
--rw-r--r--   0 skazza     (501) staff       (20)     2832 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/event/EventDispatcher.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/event/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)     3718 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/exceptions.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.352225 kathara-3.5.5/src/Kathara/foundation/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.352442 kathara-3.5.5/src/Kathara/foundation/cli/
--rw-r--r--   0 skazza     (501) staff       (20)      741 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/foundation/cli/CliArgs.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/cli/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.352780 kathara-3.5.5/src/Kathara/foundation/cli/command/
--rw-r--r--   0 skazza     (501) staff       (20)      595 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/cli/command/Command.py
--rw-r--r--   0 skazza     (501) staff       (20)      205 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/cli/command/CommandFactory.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/cli/command/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.352879 kathara-3.5.5/src/Kathara/foundation/cli/ui/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/cli/ui/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.353245 kathara-3.5.5/src/Kathara/foundation/cli/ui/setting/
--rw-r--r--   0 skazza     (501) staff       (20)     1023 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py
--rw-r--r--   0 skazza     (501) staff       (20)      233 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/cli/ui/setting/OptionsHandlerFactory.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/cli/ui/setting/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.353460 kathara-3.5.5/src/Kathara/foundation/factory/
--rw-r--r--   0 skazza     (501) staff       (20)     1010 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/factory/Factory.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/factory/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.353856 kathara-3.5.5/src/Kathara/foundation/manager/
--rw-r--r--   0 skazza     (501) staff       (20)    17939 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/foundation/manager/IManager.py
--rw-r--r--   0 skazza     (501) staff       (20)      213 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/manager/ManagerFactory.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/manager/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.354272 kathara-3.5.5/src/Kathara/foundation/manager/stats/
--rw-r--r--   0 skazza     (501) staff       (20)      681 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/foundation/manager/stats/ILinkStats.py
--rw-r--r--   0 skazza     (501) staff       (20)      674 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/foundation/manager/stats/IMachineStats.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/foundation/manager/stats/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.354591 kathara-3.5.5/src/Kathara/foundation/manager/terminal/
--rw-r--r--   0 skazza     (501) staff       (20)     2095 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/manager/terminal/Terminal.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/manager/terminal/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)     1178 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/manager/terminal/terminal_utils.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.354959 kathara-3.5.5/src/Kathara/foundation/setting/
--rw-r--r--   0 skazza     (501) staff       (20)      749 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/setting/SettingsAddon.py
--rw-r--r--   0 skazza     (501) staff       (20)      228 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/setting/SettingsAddonFactory.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/setting/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.355209 kathara-3.5.5/src/Kathara/foundation/test/
--rw-r--r--   0 skazza     (501) staff       (20)     1657 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/foundation/test/Test.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/foundation/test/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.355500 kathara-3.5.5/src/Kathara/manager/
--rw-r--r--   0 skazza     (501) staff       (20)    18970 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/manager/Kathara.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/manager/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.356501 kathara-3.5.5/src/Kathara/manager/docker/
--rw-r--r--   0 skazza     (501) staff       (20)     7141 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/manager/docker/DockerImage.py
--rw-r--r--   0 skazza     (501) staff       (20)    13588 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/manager/docker/DockerLink.py
--rw-r--r--   0 skazza     (501) staff       (20)    35888 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/manager/docker/DockerMachine.py
--rw-r--r--   0 skazza     (501) staff       (20)    31189 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/manager/docker/DockerManager.py
--rw-r--r--   0 skazza     (501) staff       (20)     3606 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/manager/docker/DockerPlugin.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/manager/docker/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.356979 kathara-3.5.5/src/Kathara/manager/docker/stats/
--rw-r--r--   0 skazza     (501) staff       (20)     3383 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/manager/docker/stats/DockerLinkStats.py
--rw-r--r--   0 skazza     (501) staff       (20)     5220 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/manager/docker/stats/DockerMachineStats.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/manager/docker/stats/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.357380 kathara-3.5.5/src/Kathara/manager/docker/terminal/
--rw-r--r--   0 skazza     (501) staff       (20)     2205 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py
--rw-r--r--   0 skazza     (501) staff       (20)     1157 2022-12-15 16:38:12.000000 kathara-3.5.5/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/manager/docker/terminal/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.358347 kathara-3.5.5/src/Kathara/manager/kubernetes/
--rw-r--r--   0 skazza     (501) staff       (20)     1924 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesConfig.py
--rw-r--r--   0 skazza     (501) staff       (20)     4252 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesConfigMap.py
--rw-r--r--   0 skazza     (501) staff       (20)    14016 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesLink.py
--rw-r--r--   0 skazza     (501) staff       (20)    34679 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesMachine.py
--rw-r--r--   0 skazza     (501) staff       (20)    30088 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesManager.py
--rw-r--r--   0 skazza     (501) staff       (20)     4366 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesNamespace.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.358742 kathara-3.5.5/src/Kathara/manager/kubernetes/stats/
--rw-r--r--   0 skazza     (501) staff       (20)     2144 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py
--rw-r--r--   0 skazza     (501) staff       (20)     3444 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/stats/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.359120 kathara-3.5.5/src/Kathara/manager/kubernetes/terminal/
--rw-r--r--   0 skazza     (501) staff       (20)     2418 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/manager/kubernetes/terminal/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.359794 kathara-3.5.5/src/Kathara/model/
--rw-r--r--   0 skazza     (501) staff       (20)     1975 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/model/ExternalLink.py
--rw-r--r--   0 skazza     (501) staff       (20)    14455 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/model/Lab.py
--rw-r--r--   0 skazza     (501) staff       (20)     1252 2022-06-05 07:57:03.000000 kathara-3.5.5/src/Kathara/model/Link.py
--rw-r--r--   0 skazza     (501) staff       (20)    18418 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/model/Machine.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/model/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.360068 kathara-3.5.5/src/Kathara/os/
--rw-r--r--   0 skazza     (501) staff       (20)     5402 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/os/Networking.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/os/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.360193 kathara-3.5.5/src/Kathara/parser/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/parser/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.361003 kathara-3.5.5/src/Kathara/parser/netkit/
--rw-r--r--   0 skazza     (501) staff       (20)     2657 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/parser/netkit/DepParser.py
--rw-r--r--   0 skazza     (501) staff       (20)     2665 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/parser/netkit/ExtParser.py
--rw-r--r--   0 skazza     (501) staff       (20)     1146 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/parser/netkit/FolderParser.py
--rw-r--r--   0 skazza     (501) staff       (20)     3429 2022-12-16 14:32:04.000000 kathara-3.5.5/src/Kathara/parser/netkit/LabParser.py
--rw-r--r--   0 skazza     (501) staff       (20)      903 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/parser/netkit/OptionParser.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/parser/netkit/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.361298 kathara-3.5.5/src/Kathara/setting/
--rw-r--r--   0 skazza     (501) staff       (20)    11573 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/setting/Setting.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/setting/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.361687 kathara-3.5.5/src/Kathara/setting/addon/
--rw-r--r--   0 skazza     (501) staff       (20)     1116 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/setting/addon/DockerSettingsAddon.py
--rw-r--r--   0 skazza     (501) staff       (20)      906 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/setting/addon/KubernetesSettingsAddon.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/setting/addon/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)     1404 2022-09-14 21:00:18.000000 kathara-3.5.5/src/Kathara/strings.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.362062 kathara-3.5.5/src/Kathara/test/
--rw-r--r--   0 skazza     (501) staff       (20)     5449 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/test/BuiltinTest.py
--rw-r--r--   0 skazza     (501) staff       (20)     4534 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/test/UserTest.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/test/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.362194 kathara-3.5.5/src/Kathara/trdparty/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.363344 kathara-3.5.5/src/Kathara/trdparty/consolemenu/
--rw-r--r--   0 skazza     (501) staff       (20)      519 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)    15168 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/console_menu.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.363923 kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/
--rw-r--r--   0 skazza     (501) staff       (20)      850 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)    14430 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/menu_borders.py
--rw-r--r--   0 skazza     (501) staff       (20)     1502 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/menu_margins.py
--rw-r--r--   0 skazza     (501) staff       (20)     1445 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/menu_padding.py
--rw-r--r--   0 skazza     (501) staff       (20)     3760 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/menu_style.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.364637 kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/
--rw-r--r--   0 skazza     (501) staff       (20)      385 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)     1335 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/command_item.py
--rw-r--r--   0 skazza     (501) staff       (20)      803 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/external_item.py
--rw-r--r--   0 skazza     (501) staff       (20)     1353 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/function_item.py
--rw-r--r--   0 skazza     (501) staff       (20)      595 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/selection_item.py
--rw-r--r--   0 skazza     (501) staff       (20)     1596 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/submenu_item.py
--rw-r--r--   0 skazza     (501) staff       (20)    13445 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/menu_component.py
--rw-r--r--   0 skazza     (501) staff       (20)    11425 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/menu_formatter.py
--rw-r--r--   0 skazza     (501) staff       (20)     3281 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/multiselect_menu.py
--rw-r--r--   0 skazza     (501) staff       (20)    12321 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/prompt_utils.py
--rw-r--r--   0 skazza     (501) staff       (20)     1805 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/screen.py
--rw-r--r--   0 skazza     (501) staff       (20)     2772 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/selection_menu.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.365132 kathara-3.5.5/src/Kathara/trdparty/consolemenu/validators/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/validators/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)      765 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/validators/base.py
--rw-r--r--   0 skazza     (501) staff       (20)     1009 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/validators/regex.py
--rw-r--r--   0 skazza     (501) staff       (20)      558 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/validators/url.py
--rw-r--r--   0 skazza     (501) staff       (20)       22 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/consolemenu/version.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.365388 kathara-3.5.5/src/Kathara/trdparty/curses/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/curses/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)     1352 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/curses/curses.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.365630 kathara-3.5.5/src/Kathara/trdparty/depgen/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/depgen/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)     2992 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/depgen/depgen.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.365855 kathara-3.5.5/src/Kathara/trdparty/libtmux/
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/libtmux/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)     2724 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/trdparty/libtmux/tmux.py
--rw-r--r--   0 skazza     (501) staff       (20)     9481 2022-10-11 22:52:11.000000 kathara-3.5.5/src/Kathara/utils.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.366269 kathara-3.5.5/src/Kathara/validator/
--rw-r--r--   0 skazza     (501) staff       (20)      599 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/validator/ImageValidator.py
--rw-r--r--   0 skazza     (501) staff       (20)      457 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/validator/TerminalValidator.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2021-10-11 10:43:00.000000 kathara-3.5.5/src/Kathara/validator/__init__.py
--rw-r--r--   0 skazza     (501) staff       (20)      308 2023-01-17 05:54:46.000000 kathara-3.5.5/src/Kathara/version.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.366664 kathara-3.5.5/src/Kathara/webhooks/
--rw-r--r--   0 skazza     (501) staff       (20)     1318 2022-09-14 21:00:35.000000 kathara-3.5.5/src/Kathara/webhooks/DockerHubApi.py
--rw-r--r--   0 skazza     (501) staff       (20)      795 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/webhooks/GitHubApi.py
--rw-r--r--   0 skazza     (501) staff       (20)        0 2022-05-13 14:12:49.000000 kathara-3.5.5/src/Kathara/webhooks/__init__.py
-drwxr-xr-x   0 skazza     (501) staff       (20)        0 2023-01-17 08:32:17.367495 kathara-3.5.5/src/kathara.egg-info/
--rw-r--r--   0 skazza     (501) staff       (20)     9081 2023-01-17 08:32:17.000000 kathara-3.5.5/src/kathara.egg-info/PKG-INFO
--rw-r--r--   0 skazza     (501) staff       (20)     6738 2023-01-17 08:32:17.000000 kathara-3.5.5/src/kathara.egg-info/SOURCES.txt
--rw-r--r--   0 skazza     (501) staff       (20)        1 2023-01-17 08:32:17.000000 kathara-3.5.5/src/kathara.egg-info/dependency_links.txt
--rw-r--r--   0 skazza     (501) staff       (20)      437 2023-01-17 08:32:17.000000 kathara-3.5.5/src/kathara.egg-info/requires.txt
--rw-r--r--   0 skazza     (501) staff       (20)       16 2023-01-17 08:32:17.000000 kathara-3.5.5/src/kathara.egg-info/top_level.txt
--rw-r--r--   0 skazza     (501) staff       (20)     4027 2022-09-14 21:00:35.000000 kathara-3.5.5/src/kathara.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.237546 kathara-3.6.0/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    35141 2022-09-29 09:36:59.000000 kathara-3.6.0/LICENSE
+-rw-rw-r--   0 tommaso   (1001) tommaso   (1001)    50225 2023-05-22 09:27:57.237546 kathara-3.6.0/PKG-INFO
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     8365 2023-01-31 11:35:52.000000 kathara-3.6.0/README.md
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1986 2023-05-22 08:35:38.000000 kathara-3.6.0/pyproject.toml
+-rw-rw-r--   0 tommaso   (1001) tommaso   (1001)      723 2023-05-22 09:27:57.237546 kathara-3.6.0/setup.cfg
+-rw-rw-r--   0 tommaso   (1001) tommaso   (1001)     1679 2023-05-22 08:35:38.000000 kathara-3.6.0/setup.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.213546 kathara-3.6.0/src/
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.213546 kathara-3.6.0/src/Kathara/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.213546 kathara-3.6.0/src/Kathara/auth/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1650 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/auth/PrivilegeHandler.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/auth/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.213546 kathara-3.6.0/src/Kathara/cli/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.217546 kathara-3.6.0/src/Kathara/cli/command/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2240 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/CheckCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2521 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/ConnectCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3068 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/cli/command/ExecCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1972 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LcleanCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3010 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LconfigCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4632 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LinfoCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2575 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/ListCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4324 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LrestartCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     8237 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LstartCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4512 2023-02-08 10:14:37.000000 kathara-3.6.0/src/Kathara/cli/command/LtestCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      350 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/command/SettingsCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1253 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/VcleanCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2698 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/VconfigCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     6964 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/VstartCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2217 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/WipeCommand.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/command/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.217546 kathara-3.6.0/src/Kathara/cli/ui/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.217546 kathara-3.6.0/src/Kathara/cli/ui/event/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1313 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/HandleProgressBar.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      694 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/OpenMachineTerminal.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1058 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/UpdateDockerImage.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2402 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/register.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/cli/ui/setting/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    21225 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/CommonOptionsHandler.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    13071 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/DockerOptionsHandler.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     8908 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1483 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/SettingsMenuFactory.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3828 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/utils.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     5981 2023-02-08 10:14:37.000000 kathara-3.6.0/src/Kathara/cli/ui/utils.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      623 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/decorators.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/event/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2832 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/event/EventDispatcher.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/event/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3718 2022-12-22 11:19:53.000000 kathara-3.6.0/src/Kathara/exceptions.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/cli/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      741 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/foundation/cli/CliArgs.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/cli/command/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      595 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/command/Command.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      205 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/command/CommandFactory.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/command/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/cli/ui/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/ui/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1023 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      233 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/OptionsHandlerFactory.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/factory/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1010 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/factory/Factory.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/factory/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/manager/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    17939 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/foundation/manager/IManager.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      213 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/ManagerFactory.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/manager/stats/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      681 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/stats/ILinkStats.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      674 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/stats/IMachineStats.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/stats/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/foundation/manager/terminal/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2095 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/terminal/Terminal.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/terminal/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1178 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/terminal/terminal_utils.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/foundation/model/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    11264 2023-05-17 10:04:03.000000 kathara-3.6.0/src/Kathara/foundation/model/FilesystemMixin.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2023-02-08 10:14:37.000000 kathara-3.6.0/src/Kathara/foundation/model/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/foundation/setting/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      749 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/setting/SettingsAddon.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      228 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/setting/SettingsAddonFactory.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/setting/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/foundation/test/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1662 2023-02-08 10:14:37.000000 kathara-3.6.0/src/Kathara/foundation/test/Test.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/test/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    18970 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/Kathara.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/docker/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     7128 2023-03-29 09:31:09.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerImage.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    13831 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerLink.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    36212 2023-05-17 10:04:03.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerMachine.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    31189 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerManager.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3606 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerPlugin.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/docker/stats/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3383 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/stats/DockerLinkStats.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     5220 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/stats/DockerMachineStats.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/stats/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/docker/terminal/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2205 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1157 2023-04-03 14:17:45.000000 kathara-3.6.0/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/terminal/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/kubernetes/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1924 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesConfig.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4252 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesConfigMap.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    14270 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesLink.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    34972 2023-05-17 10:04:03.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesMachine.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    30101 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesManager.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4366 2022-12-22 11:19:53.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesNamespace.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/kubernetes/stats/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2144 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3444 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/stats/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/kubernetes/terminal/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2418 2022-12-15 11:28:14.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/terminal/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/model/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1975 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/model/ExternalLink.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    14008 2023-03-29 09:31:09.000000 kathara-3.6.0/src/Kathara/model/Lab.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1252 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/model/Link.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    24708 2023-05-17 10:04:03.000000 kathara-3.6.0/src/Kathara/model/Machine.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/model/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/os/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     5402 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/os/Networking.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/os/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/parser/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/parser/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/parser/netkit/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2657 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/parser/netkit/DepParser.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2665 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/parser/netkit/ExtParser.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1146 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/parser/netkit/FolderParser.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3433 2023-05-09 11:16:07.000000 kathara-3.6.0/src/Kathara/parser/netkit/LabParser.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      903 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/parser/netkit/OptionParser.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/parser/netkit/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/setting/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    11573 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/setting/Setting.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/setting/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/setting/addon/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1116 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/setting/addon/DockerSettingsAddon.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      906 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/setting/addon/KubernetesSettingsAddon.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/setting/addon/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1404 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/strings.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/test/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     5449 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/test/BuiltinTest.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4534 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/test/UserTest.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/test/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/trdparty/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/trdparty/consolemenu/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      519 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    15168 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/console_menu.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      850 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    14430 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_borders.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1502 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_margins.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1445 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_padding.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3760 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_style.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      385 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1335 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/command_item.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      803 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/external_item.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1353 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/function_item.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      595 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/selection_item.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1596 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/submenu_item.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    13445 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/menu_component.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    11425 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/menu_formatter.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3281 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/multiselect_menu.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)    12321 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/prompt_utils.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1805 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/screen.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2772 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/selection_menu.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      765 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/base.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1009 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/regex.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      558 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/url.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)       22 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/version.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/curses/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/curses/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1352 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/curses/curses.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/depgen/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/depgen/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2992 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/depgen/depgen.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/libtmux/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/libtmux/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2738 2023-03-29 09:31:09.000000 kathara-3.6.0/src/Kathara/trdparty/libtmux/tmux.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/strtobool/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2023-01-31 11:35:52.000000 kathara-3.6.0/src/Kathara/trdparty/strtobool/__init__.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      692 2023-01-31 11:35:52.000000 kathara-3.6.0/src/Kathara/trdparty/strtobool/strtobool.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     9659 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/utils.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.237546 kathara-3.6.0/src/Kathara/validator/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      599 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/validator/ImageValidator.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      457 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/validator/TerminalValidator.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/validator/__init__.py
+-rw-rw-r--   0 tommaso   (1001) tommaso   (1001)      308 2023-05-22 08:35:38.000000 kathara-3.6.0/src/Kathara/version.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.237546 kathara-3.6.0/src/Kathara/webhooks/
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1318 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/webhooks/DockerHubApi.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)      795 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/webhooks/GitHubApi.py
+-rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/webhooks/__init__.py
+drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.237546 kathara-3.6.0/src/kathara.egg-info/
+-rw-rw-r--   0 tommaso   (1001) tommaso   (1001)    50225 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/PKG-INFO
+-rw-rw-r--   0 tommaso   (1001) tommaso   (1001)     6929 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/SOURCES.txt
+-rw-rw-r--   0 tommaso   (1001) tommaso   (1001)        1 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/dependency_links.txt
+-rw-rw-r--   0 tommaso   (1001) tommaso   (1001)      463 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/requires.txt
+-rw-rw-r--   0 tommaso   (1001) tommaso   (1001)       16 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/top_level.txt
+-rwxrwxrwx   0 tommaso   (1001) tommaso   (1001)     4027 2022-10-27 08:44:22.000000 kathara-3.6.0/src/kathara.py
```

### Comparing `kathara-3.5.5/LICENSE` & `kathara-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/PKG-INFO` & `kathara-3.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: kathara
-Version: 3.5.5
-Summary: A lightweight container based emulation system.
-Home-page: https://www.kathara.org
-Author: Kathara Framework
-Author-email: contact@kathara.org
-License: gpl-3.0
-Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.5.5.tar.gz
-Project-URL: Bug Tracker, https://github.com/KatharaFramework/Kathara/issues
-Keywords: NETWORK-EMULATION,CONTAINERS,NFV
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: pyuv
-License-File: LICENSE
-
 <p align="center">
     <a href="https://www.kathara.org">
         <img src="https://github.com/KatharaFramework/Kathara/wiki/logo_kathara_small.png" alt="Kathará" />
     </a>
 </p>
 <p align="right">
     <a href="https://github.com/KatharaFramework/Kathara/releases"><img src="https://img.shields.io/github/v/release/KatharaFramework/Kathara" /></a>
@@ -100,30 +78,29 @@
 - <a href="https://ieeexplore.ieee.org/document/9789876">**Sibyl: a Framework for Evaluating the Implementation of Routing Protocols in Fat-Trees**</a> (at NOMS 2022)
   - <a href="https://www.youtube.com/watch?v=FZjHjLZzXCY">NOMS2022 Presentation</a>
   - <a href="https://www.youtube.com/watch?v=FfjdqP8eKW8&t=3376s">RTGWG Session at IETF114</a>
 
 Kathará has been also presented in meetings and workshops:
 - <a href="https://datatracker.ietf.org/meeting/interim-2020-rift-01/materials/slides-interim-2020-rift-01-sessa-tools-for-experimenting-routing-in-dc-00" target="_blank">RIFT Working Group Meeting</a> (IETF 107 - March 2020)
 - <a href="https://www.youtube.com/watch?v=GVBOdNzwhBA" target="_blank">Kathará: A Lightweight Network Emulation System (Italian Audio)</a> (GraphRM - June 2022)
+- <a href="https://ripe85.ripe.net/archives/video/941/" target="_blank">Kathará: A Lightweight and Scalable Network Emulation System</a> (RIPE 85 - October 2022)
 
 ## External Tools
 
 - [Netkit Lab Generator](https://github.com/KatharaFramework/Netkit-Lab-Generator), a GUI that allows the easy creation of a network scenario configuration and the visualization of its network topology.
 - [VFTGen](https://github.com/KatharaFramework/VFTGen), a tool that allows to create three levels Fat Tree topologies (single-plane or multi-planes) and automatically configure them to run on Kathará.
 
 Being based on Netkit, all the previous tools still work. 
 
 ## Success Stories
 As far as we know, Kathará is currently being used in many [courses and projects](https://www.kathara.org/stories.html). 
  
 We encourage you to tell us your story! 
 
-We are also collecting network scenarios from the community. If you wanto to be added to the [list](https://github.com/KatharaFramework/Kathara-Labs/wiki/Community-Labs), please contact us!
+We are also collecting network scenarios from the community. If you want to be added to the [list](https://github.com/KatharaFramework/Kathara-Labs/wiki/Community-Labs), please contact us!
 
 ## Join Us
 
 Kathará is an open source project. 
 Feel free to download the code, play with it, and submit feature requests, notify bugs, or open pull requests!
 
 Thanks to everyone who has contributed to the development of Kathará!
-
-
```

#### html2text {}

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1 Name: kathara Version: 3.5.5 Summary: A lightweight
-container based emulation system. Home-page: https://www.kathara.org Author:
-Kathara Framework Author-email: contact@kathara.org License: gpl-3.0 Download-
-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.5.5.tar.gz
-Project-URL: Bug Tracker, https://github.com/KatharaFramework/Kathara/issues
-Keywords: NETWORK-EMULATION,CONTAINERS,NFV Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
-License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
-Extra: pyuv License-File: LICENSE
                                   [KatharÃ¡]
    [https://img.shields.io/github/v/release/KatharaFramework/Kathara] [https://
          img.shields.io/github/release-date/KatharaFramework/Kathara] [https://
       img.shields.io/github/downloads/KatharaFramework/Kathara/total] [https://
         img.shields.io/github/stars/KatharaFramework/Kathara] [License:_GPL_v3]
     * Official_Website
     * What_is_it?
@@ -80,22 +68,23 @@
 Emulation_System** (at NOMS 2020) - Presentation - Best_Demo_Paper_Award -
 **Megalos:_A_Scalable_Architecture_for_the_Virtualization_of_Large_Network
 Scenarios** (in MDPI Future Internet Journal 2021) - **Sibyl:_a_Framework_for
 Evaluating_the_Implementation_of_Routing_Protocols_in_Fat-Trees** (at NOMS
 2022) - NOMS2022_Presentation - RTGWG_Session_at_IETF114 KatharÃ¡ has been also
 presented in meetings and workshops: - RIFT_Working_Group_Meeting (IETF 107 -
 March 2020) - KatharÃ¡:_A_Lightweight_Network_Emulation_System_(Italian_Audio)
-(GraphRM - June 2022) ## External Tools - [Netkit Lab Generator](https://
-github.com/KatharaFramework/Netkit-Lab-Generator), a GUI that allows the easy
-creation of a network scenario configuration and the visualization of its
-network topology. - [VFTGen](https://github.com/KatharaFramework/VFTGen), a
+(GraphRM - June 2022) - KatharÃ¡:_A_Lightweight_and_Scalable_Network_Emulation
+System (RIPE 85 - October 2022) ## External Tools - [Netkit Lab Generator]
+(https://github.com/KatharaFramework/Netkit-Lab-Generator), a GUI that allows
+the easy creation of a network scenario configuration and the visualization of
+its network topology. - [VFTGen](https://github.com/KatharaFramework/VFTGen), a
 tool that allows to create three levels Fat Tree topologies (single-plane or
 multi-planes) and automatically configure them to run on KatharÃ¡. Being based
 on Netkit, all the previous tools still work. ## Success Stories As far as we
 know, KatharÃ¡ is currently being used in many [courses and projects](https://
 www.kathara.org/stories.html). We encourage you to tell us your story! We are
-also collecting network scenarios from the community. If you wanto to be added
+also collecting network scenarios from the community. If you want to be added
 to the [list](https://github.com/KatharaFramework/Kathara-Labs/wiki/Community-
 Labs), please contact us! ## Join Us KatharÃ¡ is an open source project. Feel
 free to download the code, play with it, and submit feature requests, notify
 bugs, or open pull requests! Thanks to everyone who has contributed to the
 development of KatharÃ¡!
```

### Comparing `kathara-3.5.5/setup.py` & `kathara-3.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 from setuptools import find_packages
 
 setup(
     name='kathara',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     py_modules=['kathara'],
-    version='3.5.5',
+    version='3.6.0',
     license='gpl-3.0',
     description='A lightweight container based emulation system.',
     author='Kathara Framework',
     author_email='contact@kathara.org',
     url='https://www.kathara.org',
-    download_url='https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.5.5.tar.gz',
+    download_url='https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.0.tar.gz',
     keywords=['NETWORK-EMULATION', 'CONTAINERS', 'NFV'],
     install_requires=[
         "binaryornot>=0.4.4",
         "docker>=6.0.1",
         "kubernetes>=23.3.0",
         "requests>=2.22.0",
         "coloredlogs>=10.0",
         "terminaltables>=3.1.0",
         "slug>=2.0",
         "deepdiff==6.2.2",
         "pyroute2>=0.5.19",
         "progressbar2>=1.14.0",
+        "fs>=2.4.16",
         "libtmux>=0.8.2; platform_system == 'darwin' or platform_system == 'linux'",
         "appscript>=1.1.0; platform_system == 'darwin'",
         "pypiwin32>=223; platform_system == 'win32'",
         "windows-curses>=2.1.0; platform_system == 'win32'"
     ],
     extras_require={
         'pyuv': ["pyuv @ https://api.github.com/repos/saghul/pyuv/tarball/master"],
@@ -37,9 +38,10 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
 )
```

### Comparing `kathara-3.5.5/src/Kathara/auth/PrivilegeHandler.py` & `kathara-3.6.0/src/Kathara/auth/PrivilegeHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/cli/command/CheckCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/CheckCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
     def run(self, current_path: str, argv: List[str]) -> None:
         self.parse_args(argv)
         args = self.get_args()
 
         print("*\tCurrent Manager is: %s" % Kathara.get_instance().get_formatted_manager_name())
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/ConnectCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/ConnectCommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         group = self.parser.add_mutually_exclusive_group(required=False)
 
         group.add_argument(
             '-d', '--directory',
             help='Specify the folder containing the network scenario.',
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/ExecCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/ExecCommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         group = self.parser.add_mutually_exclusive_group(required=False)
 
         group.add_argument(
             '-d', '--directory',
             help='Specify the folder containing the network scenario.',
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/LcleanCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/LcleanCommand.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         self.parser.add_argument(
             '-d', '--directory',
             required=False,
             help='Specify the folder containing the network scenario.'
         )
@@ -50,8 +50,10 @@
         try:
             lab = LabParser.parse(lab_path)
         except (Exception, IOError):
             lab = Lab(None, path=lab_path)
 
         logging.info(format_headers("Stopping Network Scenario"))
 
-        Kathara.get_instance().undeploy_lab(lab_hash=lab.hash, selected_machines=set(args['machine_names']))
+        Kathara.get_instance().undeploy_lab(lab_hash=lab.hash,
+                                            selected_machines=set(args['machine_names']) if args['machine_names']
+                                                                                         else None)
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/LconfigCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/LconfigCommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,27 +22,27 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
         self.parser.add_argument(
             '-d', '--directory',
             metavar='LAB_PATH',
             required=False,
             help='Path of the network scenario to configure, if not specified the current path is used'
         )
         self.parser.add_argument(
             '-n', '--name',
             metavar='DEVICE_NAME',
             required=True,
-            help='Name of the device to be connected on desired collision domains.'
+            help='Name of the device to configure.'
         )
 
         group = self.parser.add_mutually_exclusive_group(required=True)
 
         group.add_argument(
             '--add',
             type=alphanumeric,
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/LinfoCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/LinfoCommand.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,37 +24,37 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         self.parser.add_argument(
             '-d', '--directory',
             required=False,
             help='Specify the folder containing the network scenario.'
         )
 
         group = self.parser.add_mutually_exclusive_group(required=False)
 
         group.add_argument(
-            '-l', '--live',
+            '-w', '-l', '--watch', '--live',
             required=False,
             action='store_true',
-            help='Live mode, can be used only when a network scenario is launched.'
+            help='Watch mode, can be used only when a network scenario is launched.'
         )
 
         group.add_argument(
             '-c', '--conf',
             required=False,
             action='store_true',
-            help='Read information from lab.conf.'
+            help='Read static information from lab.conf.'
         )
 
         self.parser.add_argument(
             '-n', '--name',
             metavar='DEVICE_NAME',
             required=False,
             help='Show only information about a specified device.'
@@ -67,15 +67,15 @@
         lab_path = args['directory'].replace('"', '').replace("'", '') if args['directory'] else current_path
         lab_path = utils.get_absolute_path(lab_path)
         try:
             lab = LabParser.parse(lab_path)
         except (Exception, IOError):
             lab = Lab(None, path=lab_path)
 
-        if args['live']:
+        if args['watch']:
             if args['name']:
                 self._get_machine_live_info(lab, args['name'])
             else:
                 self._get_lab_live_info(lab)
 
             return
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/ListCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/ListCommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
-from typing import List
+from typing import List, Optional
 
 from ..ui.utils import create_table
 from ... import utils
+from ...exceptions import PrivilegeError
 from ...foundation.cli.command.Command import Command
 from ...manager.Kathara import Kathara
 from ...strings import strings, wiki_description
 from ...trdparty.curses.curses import Curses
 
 
 class ListCommand(Command):
@@ -20,29 +21,29 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         self.parser.add_argument(
             '-a', '--all',
             required=False,
             action='store_true',
             help='Show all running Kathara devices of all users. MUST BE ROOT FOR THIS OPTION.'
         )
 
         self.parser.add_argument(
-            '-l', '--live',
+            '-w', '-l', '--watch', '--live',
             required=False,
             action='store_true',
-            help='Live mode.'
+            help='Watch mode.'
         )
 
         self.parser.add_argument(
             '-n', '--name',
             metavar='DEVICE_NAME',
             required=False,
             help='Show only information about a specified device.'
@@ -53,22 +54,22 @@
         args = self.get_args()
 
         if args['all'] and not utils.is_admin():
             raise PrivilegeError("You must be root in order to show all Kathara devices of all users.")
 
         all_users = bool(args['all'])
 
-        if args['live']:
+        if args['watch']:
             self._get_live_info(machine_name=args['name'], all_users=all_users)
         else:
             machines_stats = Kathara.get_instance().get_machines_stats(machine_name=args['name'], all_users=all_users)
             print(next(create_table(machines_stats)))
 
     @staticmethod
-    def _get_live_info(machine_name: str, all_users: bool) -> None:
+    def _get_live_info(machine_name: Optional[str], all_users: bool) -> None:
         machines_stats = Kathara.get_instance().get_machines_stats(machine_name=machine_name, all_users=all_users)
         table = create_table(machines_stats)
 
         Curses.get_instance().init_window()
 
         try:
             while True:
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/LrestartCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/LrestartCommand.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 from typing import List
 
 from .LcleanCommand import LcleanCommand
 from .LstartCommand import LstartCommand
-from ... import utils
 from ...foundation.cli.command.Command import Command
 from ...strings import strings, wiki_description
 
 
 class LrestartCommand(Command):
     def __init__(self) -> None:
         Command.__init__(self)
@@ -19,15 +18,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         group = self.parser.add_mutually_exclusive_group(required=False)
 
         group.add_argument(
             "--noterminals",
             action="store_const",
@@ -118,17 +117,14 @@
             help='Restarts only specified devices.'
         )
 
     def run(self, current_path: str, argv: List[str]) -> None:
         self.parse_args(argv)
         args = self.get_args()
 
-        lab_path = args['directory'].replace('"', '').replace("'", '') if args['directory'] else current_path
-        lab_path = utils.get_absolute_path(lab_path)
-
         lclean_argv = ['-d', args['directory']] if args['directory'] else []
 
         if args['machine_name']:
             lclean_argv.extend(args['machine_name'])
 
-        LcleanCommand().run(lab_path, lclean_argv)
-        LstartCommand().run(lab_path, argv)
+        LcleanCommand().run(current_path, lclean_argv)
+        LstartCommand().run(current_path, argv)
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/LstartCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/LstartCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         group = self.parser.add_mutually_exclusive_group(required=False)
 
         group.add_argument(
             "--noterminals",
             action="store_const",
@@ -85,20 +85,20 @@
             dest='options',
             metavar="OPTION",
             nargs='*',
             required=False,
             help="Apply options to all devices of a network scenario during startup."
         )
         self.parser.add_argument(
-            '--xterm',
+            '--xterm', '--terminal-emu',
             required=False,
             help='Set a different terminal emulator application (Unix only).'
         )
         self.parser.add_argument(
-            '--print',
+            '--print', '--dry-mode',
             dest="dry_mode",
             required=False,
             action='store_true',
             help='Open the lab.conf file and check if it is correct (dry run).'
         )
         hosthome_group = self.parser.add_mutually_exclusive_group(required=False)
         hosthome_group.add_argument(
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/LtestCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/LtestCommand.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         self.parser.add_argument(
             '-d', '--directory',
             required=False,
             help='Specify the folder containing the network scenario.'
         )
@@ -103,15 +103,15 @@
             if not os.path.exists(signature_test_path) or args['rebuild_signature']:
                 shutil.rmtree(signature_test_path, ignore_errors=True)
                 os.makedirs(signature_test_path, exist_ok=True)
 
                 builtin_test.create_signature()
                 user_test.create_signature()
         else:
-            result_test_path = os.path.join(lab.path, "_test", "results")
+            result_test_path = os.path.join(lab.fs_path(), "_test", "results")
 
             shutil.rmtree(result_test_path, ignore_errors=True)
             os.makedirs(result_test_path, exist_ok=True)
 
             try:
                 if args['verify'] == "builtin" or args['verify'] == "both":
                     builtin_test_passed = builtin_test.test()
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/VcleanCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/VcleanCommand.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,22 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         self.parser.add_argument(
             '-n', '--name',
             metavar='DEVICE_NAME',
             required=True,
-            help='Name of the device to be cleaned.'
+            help='The name of the device to clean.'
         )
 
     def run(self, current_path: str, argv: List[str]) -> None:
         self.parse_args(argv)
         args = self.get_args()
 
         lab = Lab("kathara_vlab")
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/VconfigCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/VconfigCommand.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
         self.parser.add_argument(
             '-n', '--name',
             metavar='DEVICE_NAME',
             required=True,
             help='Name of the device to be connected on desired collision domains.'
         )
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/VstartCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/VstartCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         group = self.parser.add_mutually_exclusive_group(required=False)
 
         group.add_argument(
             "--noterminals",
             action="store_const",
@@ -110,20 +110,20 @@
             '--hosthome',
             dest="hosthome_mount",
             action="store_const",
             const=True,
             help='Mount "/hosthome" directory inside the device.'
         )
         self.parser.add_argument(
-            '--xterm',
+            '--xterm', '--terminal-emu',
             required=False,
             help='Set a different terminal emulator application (Unix only).'
         )
         self.parser.add_argument(
-            '--print',
+            '--print', '--dry-run',
             dest='dry_mode',
             required=False,
             action='store_true',
             help='Check if the device parameters are correct (dry run).'
         )
         self.parser.add_argument(
             '--bridged',
```

### Comparing `kathara-3.5.5/src/Kathara/cli/command/WipeCommand.py` & `kathara-3.6.0/src/Kathara/cli/command/WipeCommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
-            help='Show an help message and exit.'
+            help='Show a help message and exit.'
         )
 
         self.parser.add_argument(
             '-f', '--force',
             required=False,
             action='store_true',
             help='Force the wipe.'
```

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/event/HandleProgressBar.py` & `kathara-3.6.0/src/Kathara/cli/ui/event/HandleProgressBar.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/event/OpenMachineTerminal.py` & `kathara-3.6.0/src/Kathara/cli/ui/event/OpenMachineTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/event/UpdateDockerImage.py` & `kathara-3.6.0/src/Kathara/cli/ui/event/UpdateDockerImage.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/event/register.py` & `kathara-3.6.0/src/Kathara/cli/ui/event/register.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/setting/CommonOptionsHandler.py` & `kathara-3.6.0/src/Kathara/cli/ui/setting/CommonOptionsHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         manager_item = SubmenuItem(choose_manager_string, manager_menu, current_menu)
 
         # Image Selection Submenu
         image_string = "Choose default image"
         select_image_menu = SelectionMenu(strings=[],
                                           title=image_string,
                                           subtitle=setting_utils.current_string("image"),
-                                          prologue_text="""Default Docker image when you start a lab or """
+                                          prologue_text="""Default Docker image when you start a network scenario or """
                                                         """a single Kathara device.
                                                         Default is `%s`.""" % DEFAULTS['image'],
                                           formatter=menu_formatter
                                           )
 
         try:
             for image in DockerHubApi.get_images():
```

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/setting/DockerOptionsHandler.py` & `kathara-3.6.0/src/Kathara/cli/ui/setting/DockerOptionsHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         hosthome_item = SubmenuItem(hosthome_string, hosthome_menu, current_menu)
 
         # Shared Mount Option
         shared_string = "Automatically mount /shared on startup"
         shared_menu = SelectionMenu(strings=[],
                                     title=shared_string,
                                     subtitle=setting_utils.current_bool("shared_mount"),
-                                    prologue_text="""The shared directory inside the lab folder is made available """
-                                                  """for reading/writing inside the device under the special """
-                                                  """directory `/shared`.
+                                    prologue_text="""The shared directory inside the network scenario folder is """
+                                                  """made available for reading/writing inside the device """
+                                                  """under the special directory `/shared`.
                                                   
                                                   Default is %s.""" %
                                                   setting_utils.format_bool(DEFAULTS['shared_mount']),
                                     formatter=menu_formatter
                                     )
 
         shared_menu.append_item(FunctionItem(text="Yes",
```

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py` & `kathara-3.6.0/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/setting/SettingsMenuFactory.py` & `kathara-3.6.0/src/Kathara/cli/ui/setting/SettingsMenuFactory.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/setting/utils.py` & `kathara-3.6.0/src/Kathara/cli/ui/setting/utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/cli/ui/utils.py` & `kathara-3.6.0/src/Kathara/cli/ui/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,59 +78,69 @@
     logging.debug("Opening terminal for device %s.", machine.name)
 
     executable_path = utils.get_executable_path(sys.argv[0])
 
     if not executable_path:
         raise FileNotFoundError("Unable to find Kathara.")
 
-    is_vmachine = "-v" if machine.lab.path is None else ""
+    is_vmachine = "-v" if not machine.lab.has_host_path() else ""
     connect_command = "%s connect %s -l %s" % (executable_path, is_vmachine, machine.name)
 
-    logging.debug("Terminal will open in directory %s." % machine.lab.path)
+    logging.debug("Terminal will open in directory %s." % machine.lab.fs_path())
 
     def unix_connect() -> None:
         if terminal == "TMUX":
             from ...trdparty.libtmux.tmux import TMUX
 
             logging.debug("Attaching `%s` to TMUX session `%s` with command `%s`" % (machine.name, machine.lab.name,
                                                                                      connect_command))
 
-            TMUX.get_instance().add_window(machine.lab.name, machine.name, connect_command, cwd=machine.lab.path)
+            TMUX.get_instance().add_window(
+                machine.lab.name,
+                machine.name,
+                connect_command,
+                cwd=machine.lab.fs_path()
+            )
         else:
             logging.debug("Opening Linux terminal with command: %s." % connect_command)
 
             # Command should be passed as an array
             # https://stackoverflow.com/questions/9935151/popen-error-errno-2-no-such-file-or-directory/9935511
             subprocess.Popen([terminal, "-e", connect_command],
-                             cwd=machine.lab.path,
+                             cwd=machine.lab.fs_path(),
                              start_new_session=True
                              )
 
     def windows_connect() -> None:
         complete_win_command = "& %s" % connect_command
         logging.debug("Opening Windows terminal with command: %s." % complete_win_command)
         subprocess.Popen(["powershell.exe",
                           '-Command',
                           complete_win_command
                           ],
                          creationflags=subprocess.CREATE_NEW_CONSOLE,
-                         cwd=machine.lab.path
+                         cwd=machine.lab.fs_path()
                          )
 
     def osx_connect() -> None:
-        cd_to_lab_path = "cd \"%s\" &&" % machine.lab.path if machine.lab.path is not None else ""
+        cd_to_lab_path = "cd \"%s\" &&" % machine.lab.fs_path() if machine.lab.has_host_path() else ""
         complete_osx_command = "%s clear && %s && exit" % (cd_to_lab_path, connect_command)
 
         if terminal == "TMUX":
             from ...trdparty.libtmux.tmux import TMUX
 
             logging.debug("Attaching `%s` to TMUX session `%s` with command `%s`" % (machine.name, machine.lab.name,
                                                                                      complete_osx_command))
 
-            TMUX.get_instance().add_window(machine.lab.name, machine.name, complete_osx_command, cwd=machine.lab.path)
+            TMUX.get_instance().add_window(
+                machine.lab.name,
+                machine.name,
+                complete_osx_command,
+                cwd=machine.lab.fs_path()
+            )
         else:
             import appscript
             logging.debug("Opening OSX terminal with command: %s." % complete_osx_command)
             terminal_app = appscript.app(terminal)
             if terminal == 'iTerm':
                 window = terminal_app.create_window_with_default_profile()
                 window.current_session.write(text=complete_osx_command)
```

### Comparing `kathara-3.5.5/src/Kathara/decorators.py` & `kathara-3.6.0/src/Kathara/decorators.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/event/EventDispatcher.py` & `kathara-3.6.0/src/Kathara/event/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/exceptions.py` & `kathara-3.6.0/src/Kathara/exceptions.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/cli/CliArgs.py` & `kathara-3.6.0/src/Kathara/foundation/cli/CliArgs.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/cli/command/Command.py` & `kathara-3.6.0/src/Kathara/foundation/cli/command/Command.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py` & `kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/factory/Factory.py` & `kathara-3.6.0/src/Kathara/foundation/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/manager/IManager.py` & `kathara-3.6.0/src/Kathara/foundation/manager/IManager.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/manager/stats/ILinkStats.py` & `kathara-3.6.0/src/Kathara/foundation/manager/stats/ILinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/manager/stats/IMachineStats.py` & `kathara-3.6.0/src/Kathara/foundation/manager/stats/IMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/manager/terminal/Terminal.py` & `kathara-3.6.0/src/Kathara/foundation/manager/terminal/Terminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/manager/terminal/terminal_utils.py` & `kathara-3.6.0/src/Kathara/foundation/manager/terminal/terminal_utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/setting/SettingsAddon.py` & `kathara-3.6.0/src/Kathara/foundation/setting/SettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/foundation/test/Test.py` & `kathara-3.6.0/src/Kathara/foundation/test/Test.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Test(ABC):
     __slots__ = ['lab', 'test_path', 'signature_path', 'results_path']
 
     def __init__(self, lab: Lab) -> None:
         self.lab: Lab = lab
-        self.test_path: str = os.path.join(self.lab.path, '_test')
+        self.test_path: str = os.path.join(self.lab.fs_path(), '_test')
 
         self.signature_path: str = os.path.join(self.test_path, 'signature')
         self.results_path: str = os.path.join(self.test_path, 'results')
 
     @abstractmethod
     def create_signature(self) -> None:
         raise NotImplementedError("You must implement `create_signature` method.")
```

### Comparing `kathara-3.5.5/src/Kathara/manager/Kathara.py` & `kathara-3.6.0/src/Kathara/manager/Kathara.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/docker/DockerImage.py` & `kathara-3.6.0/src/Kathara/manager/docker/DockerImage.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,11 +180,11 @@
         """
         host_arch = utils.get_architecture()
 
         is_compatible = False
         if isinstance(image, docker.models.images.Image):
             is_compatible = (image.attrs['Architecture'] == host_arch)
         elif isinstance(image, docker.models.images.RegistryData):
-            is_compatible = len(list(filter(lambda x: x['architecture'] == host_arch, image.attrs['Platforms']))) > 0
+            is_compatible = any(map(lambda x: x['architecture'] == host_arch, image.attrs['Platforms']))
 
         if not is_compatible:
             raise InvalidImageArchitectureError(image, host_arch)
```

### Comparing `kathara-3.5.5/src/Kathara/manager/docker/DockerLink.py` & `kathara-3.6.0/src/Kathara/manager/docker/DockerLink.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """The class responsible for deploying Kathara collision domains as Docker networks and interact with them."""
     __slots__ = ['client']
 
     def __init__(self, client: DockerClient) -> None:
         self.client: DockerClient = client
 
     def deploy_links(self, lab: Lab, selected_links: Set[str] = None) -> None:
-        """Deploy all the lab collision domains as Docker networks.
+        """Deploy all the network scenario collision domains as Docker networks.
 
         Args:
             lab (Kathara.model.Lab.Lab): A Kathara network scenario.
             selected_links (Set[str]): A set containing the name of the collision domains to deploy.
 
         Returns:
             None
@@ -240,27 +240,35 @@
             if not link_name:
                 raise LinkNotFoundError("No collision domains found.")
             else:
                 raise LinkNotFoundError(f"Collision domains with name {link_name} not found.")
 
         networks = sorted(networks, key=lambda x: x.name)
 
-        network_streams = {}
+        networks_stats = {}
 
-        for network in networks:
-            network_streams[network.name] = DockerLinkStats(network)
+        def load_link_stats(network):
+            networks_stats[network.name] = DockerLinkStats(network)
+
+        pool_size = utils.get_pool_size()
+        links_pool = Pool(pool_size)
+
+        items = utils.chunk_list(networks, pool_size)
+
+        for chunk in items:
+            links_pool.map(func=load_link_stats, iterable=chunk)
 
         while True:
-            for network_stats in network_streams.values():
+            for network_stats in networks_stats.values():
                 try:
                     network_stats.update()
                 except StopIteration:
                     continue
 
-            yield network_streams
+            yield networks_stats
 
     def _attach_external_interfaces(self, external_links: List[ExternalLink],
                                     network: docker.models.networks.Network) -> None:
         """Attach an external collision domain to a Docker network.
 
         Args:
             external_links (Kathara.model.ExternalLink): A Kathara external collision domain. It is used to create
```

### Comparing `kathara-3.5.5/src/Kathara/manager/docker/DockerMachine.py` & `kathara-3.6.0/src/Kathara/manager/docker/DockerMachine.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 from .stats.DockerMachineStats import DockerMachineStats
 from ... import utils
 from ...event.EventDispatcher import EventDispatcher
 from ...exceptions import MountDeniedError, MachineAlreadyExistsError, MachineNotFoundError, DockerPluginError, \
     MachineBinaryError
 from ...model.Lab import Lab
 from ...model.Link import Link, BRIDGE_LINK_NAME
-from ...model.Machine import Machine
+from ...model.Machine import Machine, MACHINE_CAPABILITIES
 from ...setting.Setting import Setting
 
 RP_FILTER_NAMESPACE = "net.ipv4.conf.%s.rp_filter"
 OCI_RUNTIME_RE = re.compile(
     r"OCI runtime exec failed(.*?)(stat (.*): no such file or directory|exec: \"(.*)\": executable file not found)"
 )
 
 # Known commands that each container should execute
-# Run order: shared.startup, machine.startup and machine.startup_commands
+# Run order: shared.startup, machine.startup and machine.meta['startup_commands']
 STARTUP_COMMANDS = [
     # Unmount the /etc/resolv.conf and /etc/hosts files, automatically mounted by Docker inside the container.
     # In this way, they can be overwritten by custom user files.
     "umount /etc/resolv.conf",
     "umount /etc/hosts",
 
     # Copy the machine folder (if present) from the hostlab directory into the root folder of the container
@@ -46,15 +46,15 @@
 
     # Give proper permissions to /var/www
     "if [ -d \"/var/www\" ]; then "
     "chmod -R 777 /var/www/*; fi",
 
     # Give proper permissions to Quagga files (if present)
     "if [ -d \"/etc/quagga\" ]; then "
-    "chown quagga:quagga /etc/quagga/*",
+    "chown --recursive quagga:quagga /etc/quagga/",
     "chmod 640 /etc/quagga/*; fi",
 
     # Give proper permissions to FRR files (if present)
     "if [ -d \"/etc/frr\" ]; then "
     "chown frr:frr /etc/frr/*",
     "chmod 640 /etc/frr/*; fi",
 
@@ -99,15 +99,15 @@
 
     def __init__(self, client: DockerClient, docker_image: DockerImage) -> None:
         self.client: DockerClient = client
 
         self.docker_image: DockerImage = docker_image
 
     def deploy_machines(self, lab: Lab, selected_machines: Set[str] = None) -> None:
-        """Deploy all the lab devices as Docker containers.
+        """Deploy all the network scenario devices as Docker containers.
 
         Args:
             lab (Kathara.model.Lab.Lab): A Kathara network scenario.
             selected_machines (Set[str]): A set containing the name of the devices to deploy.
 
         Returns:
             None
@@ -240,16 +240,16 @@
 
         # Merge machine sysctls
         sysctl_parameters = {**sysctl_parameters, **machine.meta['sysctls']}
 
         volumes = {}
 
         shared_mount = options['shared_mount'] if 'shared_mount' in options else Setting.get_instance().shared_mount
-        if shared_mount and machine.lab.shared_folder:
-            volumes[machine.lab.shared_folder] = {'bind': '/shared', 'mode': 'rw'}
+        if shared_mount and machine.lab.shared_path:
+            volumes[machine.lab.shared_path] = {'bind': '/shared', 'mode': 'rw'}
 
         # Mount the host home only if specified in settings.
         hosthome_mount = options['hosthome_mount'] if 'hosthome_mount' in options else \
             Setting.get_instance().hosthome_mount
         if hosthome_mount and Setting.get_instance().remote_url is None:
             volumes[utils.get_current_user_home()] = {'bind': '/hosthome', 'mode': 'rw'}
 
@@ -260,15 +260,15 @@
 
         container_name = self.get_container_name(machine.name, machine.lab.hash)
 
         try:
             machine_container = self.client.containers.create(image=image,
                                                               name=container_name,
                                                               hostname=machine.name,
-                                                              cap_add=machine.capabilities if not privileged else None,
+                                                              cap_add=MACHINE_CAPABILITIES if not privileged else None,
                                                               privileged=privileged,
                                                               network=first_network.name if first_network else None,
                                                               network_mode="bridge" if first_network else "none",
                                                               environment=machine.meta['envs'],
                                                               sysctls=sysctl_parameters,
                                                               mem_limit=memory,
                                                               nano_cpus=cpus,
@@ -390,25 +390,25 @@
 
         # Bridged connection required but not added in `deploy` method.
         if "bridge_connected" not in machine.meta and machine.meta['bridged']:
             bridge_link = machine.lab.get_or_new_link(BRIDGE_LINK_NAME).api_object
             bridge_link.connect(machine.api_object)
 
         # Append executed machine startup commands inside the /var/log/startup.log file
-        if machine.startup_commands:
+        if machine.meta['startup_commands']:
             new_commands = []
-            for command in machine.startup_commands:
+            for command in machine.meta['startup_commands']:
                 new_commands.append("echo \"++ %s\" &>> /var/log/startup.log" % command)
                 new_commands.append(command)
-            machine.startup_commands = new_commands
+            machine.meta['startup_commands'] = new_commands
 
         # Build the final startup commands string
         startup_commands_string = "; ".join(STARTUP_COMMANDS).format(
             machine_name=machine.name,
-            machine_commands="; ".join(machine.startup_commands)
+            machine_commands="; ".join(machine.meta['startup_commands'])
         )
 
         logging.debug(f"Executing startup command on `{machine.name}`: {startup_commands_string}")
 
         try:
             # Execute the startup commands inside the container (without privileged flag so basic permissions are used)
             self._exec_run(machine.api_object,
@@ -613,16 +613,16 @@
             stdin (bool): Attach to stdin. Default: ``False``
             tty (bool): Allocate a pseudo-TTY. Default: False
             privileged (bool): Run as privileged.
             user (str): User to execute command as. Default: root
             detach (bool): If true, detach from the exec command. Default: False
             stream (bool): Stream response data. Default: False
             socket (bool): Return the connection socket to allow custom read/write operations. Default: False
-            environment (dict or list): A dictionary or a list of strings in the following format ``["PASSWORD=xxx"]`` or
-                ``{"PASSWORD": "xxx"}``.
+            environment (dict or list): A dictionary or a list of strings in the following format
+                ``["PASSWORD=xxx"]`` or ``{"PASSWORD": "xxx"}``.
             workdir (str): Path to working directory for this exec session
             demux (bool): Return stdout and stderr separately
 
         Returns:
             (Dict): A dict of (exit_code, output)
                 exit_code: (int):
                     Exit code for the executed command or ``None`` if
@@ -725,27 +725,35 @@
             if not machine_name:
                 raise MachineNotFoundError("No devices found.")
             else:
                 raise MachineNotFoundError(f"Devices with name {machine_name} not found.")
 
         containers = sorted(containers, key=lambda x: x.name)
 
-        machine_streams = {}
+        machines_stats = {}
 
-        for machine in containers:
-            machine_streams[machine.name] = DockerMachineStats(machine)
+        def load_machine_stats(machine):
+            machines_stats[machine.name] = DockerMachineStats(machine)
+
+        pool_size = utils.get_pool_size()
+        machines_pool = Pool(pool_size)
+
+        items = utils.chunk_list(containers, pool_size)
+
+        for chunk in items:
+            machines_pool.map(func=load_machine_stats, iterable=chunk)
 
         while True:
-            for machine_stats in machine_streams.values():
+            for machine_stats in machines_stats.values():
                 try:
                     machine_stats.update()
                 except StopIteration:
                     continue
 
-            yield machine_streams
+            yield machines_stats
 
     @staticmethod
     def get_container_name(name: str, lab_hash: str) -> str:
         """Return the name of a Docker container.
 
         Args:
             name (str): The name of a Kathara device.
```

### Comparing `kathara-3.5.5/src/Kathara/manager/docker/DockerManager.py` & `kathara-3.6.0/src/Kathara/manager/docker/DockerManager.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/docker/DockerPlugin.py` & `kathara-3.6.0/src/Kathara/manager/docker/DockerPlugin.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/docker/stats/DockerLinkStats.py` & `kathara-3.6.0/src/Kathara/manager/docker/stats/DockerLinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/docker/stats/DockerMachineStats.py` & `kathara-3.6.0/src/Kathara/manager/docker/stats/DockerMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py` & `kathara-3.6.0/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py` & `kathara-3.6.0/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesConfig.py` & `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesConfig.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesConfigMap.py` & `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesConfigMap.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesLink.py` & `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesLink.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,17 +239,25 @@
                 if not link_name:
                     raise LinkNotFoundError("No collision domains found.")
                 else:
                     raise LinkNotFoundError(f"Collision domains with name {link_name} not found.")
 
             networks_stats = {}
 
-            for network in networks:
+            def load_link_stats(network):
                 networks_stats[network['metadata']['name']] = KubernetesLinkStats(network)
 
+            pool_size = utils.get_pool_size()
+            links_pool = Pool(pool_size)
+
+            items = utils.chunk_list(networks, pool_size)
+
+            for chunk in items:
+                links_pool.map(func=load_link_stats, iterable=chunk)
+
             for network_stats in networks_stats.values():
                 try:
                     network_stats.update()
                 except StopIteration:
                     continue
 
             yield networks_stats
```

### Comparing `kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesMachine.py` & `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesMachine.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from ...model.Machine import Machine
 from ...setting.Setting import Setting
 
 RP_FILTER_NAMESPACE = "net.ipv4.conf.%s.rp_filter"
 MAX_RESTART_COUNT = 3
 
 # Known commands that each container should execute
-# Run order: shared.startup, machine.startup and machine.startup_commands
+# Run order: shared.startup, machine.startup and machine.meta['startup_commands']
 STARTUP_COMMANDS = [
     # If execution flag file is found, abort (this means that postStart has been called again)
     # If not flag the startup execution with a file
     "if [ -f \"/tmp/post_start\" ]; then exit; else touch /tmp/post_start; fi",
 
     "{sysctl_commands}",
 
@@ -63,15 +63,15 @@
 
     # Give proper permissions to /var/www
     "if [ -d \"/var/www\" ]; then "
     "chmod -R 777 /var/www/*; fi",
 
     # Give proper permissions to Quagga files (if present)
     "if [ -d \"/etc/quagga\" ]; then "
-    "chown quagga:quagga /etc/quagga/*",
+    "chown --recursive quagga:quagga /etc/quagga/",
     "chmod 640 /etc/quagga/*; fi",
 
     # Give proper permissions to FRR files (if present)
     "if [ -d \"/etc/frr\" ]; then "
     "chown frr:frr /etc/frr/*",
     "chmod 640 /etc/frr/*; fi",
 
@@ -337,15 +337,15 @@
         # On Ready state, the pod has volumes and network interfaces up, so this hook is used
         # to execute custom commands coming from .startup file and "exec" option
         # Build the final startup commands string
         sysctl_commands = "; ".join(["sysctl -w -q %s=%d" % item for item in machine.meta["sysctls"].items()])
         startup_commands_string = "; ".join(STARTUP_COMMANDS) \
             .format(machine_name=machine.name,
                     sysctl_commands=sysctl_commands,
-                    machine_commands="; ".join(machine.startup_commands)
+                    machine_commands="; ".join(machine.meta['startup_commands'])
                     )
 
         post_start = client.V1LifecycleHandler(
             _exec=client.V1ExecAction(
                 command=[shell, "-c", startup_commands_string]
             )
         )
@@ -800,17 +800,25 @@
                 if not machine_name:
                     raise MachineNotFoundError("No devices found.")
                 else:
                     raise MachineNotFoundError(f"Devices with name {machine_name} not found.")
 
             machines_stats = {}
 
-            for pod in pods:
+            def load_machine_stats(pod):
                 machines_stats[pod.metadata.name] = KubernetesMachineStats(pod)
 
+            pool_size = utils.get_pool_size()
+            machines_pool = Pool(pool_size)
+
+            items = utils.chunk_list(pods, pool_size)
+
+            for chunk in items:
+                machines_pool.map(func=load_machine_stats, iterable=chunk)
+
             for machine_stats in machines_stats.values():
                 try:
                     machine_stats.update()
                 except StopIteration:
                     continue
 
             yield machines_stats
```

### Comparing `kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesManager.py` & `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         self.k8s_namespace.create(lab)
         try:
             self.k8s_link.deploy_links(lab, selected_links=selected_links)
 
             self.k8s_machine.deploy_machines(lab, selected_machines=selected_machines)
         except ApiException as e:
             if e.status == 403 and 'Forbidden' in e.reason:
-                raise LabAlreadyExistsError("Previous lab execution is still terminating. Please wait.")
+                raise LabAlreadyExistsError("Previous network scenario execution is still terminating. Please wait.")
             else:
                 raise e
 
     def connect_machine_to_link(self, machine: Machine, link: Link) -> None:
         """Connect a Kathara device to a collision domain.
 
         Args:
```

### Comparing `kathara-3.5.5/src/Kathara/manager/kubernetes/KubernetesNamespace.py` & `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesNamespace.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py` & `kathara-3.6.0/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py` & `kathara-3.6.0/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py` & `kathara-3.6.0/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/model/ExternalLink.py` & `kathara-3.6.0/src/Kathara/model/ExternalLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/model/Lab.py` & `kathara-3.6.0/src/Kathara/model/Lab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,79 @@
 import collections
-import os
 from itertools import chain
 from typing import Dict, Set, Any, List, Union, Optional, Tuple
 
+from fs import open_fs
+from fs.base import FS
+
 from . import Machine as MachinePackage
 from .ExternalLink import ExternalLink
 from .Link import Link
 from .. import utils
 from ..exceptions import LinkNotFoundError, MachineNotFoundError, MachineAlreadyExistsError, LinkAlreadyExistsError
+from ..foundation.model.FilesystemMixin import FilesystemMixin
 
 
-class Lab(object):
+class Lab(FilesystemMixin):
     """A Kathara network scenario, containing information about devices and collision domains.
 
     Attributes:
         name (str): The name of the network scenario.
         description (str): A short description of the network scenario.
         version (str): The version of the network scenario.
         author (str): The author of the network scenario.
         email (str): The email of the author of the network scenario.
         web (str): The web address of the author of the network scenario.
-        path (str): The path of the network scenario, if exists.
         hash (str): The hash identifier of the network scenario.
         machines (Dict[str, Kathara.model.Machine]): The devices of the network scenario. Keys are device names, Values
             are Kathara device objects.
         links (Dict[str, Kathara.model.Link]): The collision domains of the network scenario.
             Keys are collision domains names, Values are Kathara collision domain objects.
         general_options (Dict[str, Any]): Keys are option names, values are option values.
         has_dependencies (bool): True if there are dependencies among the devices boot.
-        shared_startup_path(str) The path of the shared startup file, if exists.
-        shared_shutdown_path(str) The path of the shared shutdown file, if exists.
-        shared_folder(str) The path of the shared folder, if exists.
+        shared_path (str): Path to shared folder of the network scenario, if the network scenario has a real OS path.
+        fs (fs.FS): The filesystem of the network scenario. Contains files and configurations associated to it.
     """
-    __slots__ = ['_name', 'description', 'version', 'author', 'email', 'web',
-                 'path', 'hash', 'machines', 'links', 'general_options', 'has_dependencies',
-                 'shared_startup_path', 'shared_shutdown_path', 'shared_folder']
+    __slots__ = ['_name', 'description', 'version', 'author', 'email', 'web', 'hash',
+                 'machines', 'links', 'general_options', 'has_dependencies', 'shared_path']
 
     def __init__(self, name: Optional[str], path: Optional[str] = None) -> None:
         """Create a new instance of a Kathara network scenario.
 
         Args:
             name (str): The name of the network scenario.
             path (str): The path to the network scenario directory, if exists.
 
         Returns:
             None
         """
+        super().__init__()
+
         self._name: Optional[str] = name
         self.description: Optional[str] = None
         self.version: Optional[str] = None
         self.author: Optional[str] = None
         self.email: Optional[str] = None
         self.web: Optional[str] = None
 
         self.machines: Dict[str, 'MachinePackage.Machine'] = {}
         self.links: Dict[str, Link] = {}
 
         self.general_options: Dict[str, Any] = {}
 
         self.has_dependencies: bool = False
 
-        self.path: str = path
-        self.shared_startup_path: Optional[str] = None
-        self.shared_shutdown_path: Optional[str] = None
-
-        self.hash: str = utils.generate_urlsafe_hash(self.path if self._name is None else self._name)
+        self.shared_path: Optional[str] = None
 
-        if self.path:
-            shared_startup_file = os.path.join(self.path, 'shared.startup')
-            self.shared_startup_path = shared_startup_file if os.path.exists(shared_startup_file) else None
+        self.hash: str = utils.generate_urlsafe_hash(path if self._name is None else self._name)
 
-            shared_shutdown_file = os.path.join(self.path, 'shared.shutdown')
-            self.shared_shutdown_path = shared_shutdown_file if os.path.exists(shared_shutdown_file) else None
-
-        self.shared_folder: Optional[str] = None
+        if path:
+            self.fs: FS = open_fs(f"osfs://{path}")
+        else:
+            self.fs: FS = open_fs("mem://")
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
@@ -139,15 +135,15 @@
             None
 
         Raises:
             LinkNotFoundError: If the external collision domain specified is not associated to the network scenario.
         """
         for (link_name, link_external_links) in external_links.items():
             if link_name not in self.links:
-                raise LinkNotFoundError("Collision domain `%s` (declared in lab.ext) not found in lab "
+                raise LinkNotFoundError("Collision domain `%s` (declared in lab.ext) not found in network scenario "
                                         "collision domains." % link_name)
 
             self.links[link_name].external += link_external_links
 
     def check_integrity(self) -> None:
         """Check if the network interfaces numbers of all the devices in the network scenario are correctly assigned.
 
@@ -306,33 +302,32 @@
         Returns:
             None
 
         Raises:
             IOError: If the shared folder is a Symlink, delete it.
             OSError: If there is a permission error.
         """
-        if not self.has_path():
+        if not self.has_host_path():
             return
+
         try:
-            self.shared_folder = os.path.join(self.path, 'shared')
-            if not os.path.isdir(self.shared_folder):
-                os.mkdir(self.shared_folder)
-            elif os.path.islink(self.shared_folder):
-                raise IOError("`shared` folder is a symlink, delete it.")
+            self.shared_path = self.fs.makedir('shared', recreate=True).getsyspath("")
+            if self.fs.islink('shared'):
+                raise ValueError("`shared` folder is a symlink, delete it.")
         except OSError:
             # Do not create shared folder if not permitted.
             return
 
-    def has_path(self) -> bool:
-        """Check if the network scenario has a directory.
+    def has_host_path(self) -> bool:
+        """Check if the network scenario has a directory on the host.
 
         Returns:
-            bool: True if self.path is not None, else False.
+            bool: True if network scenario has a path on the host filesystem, else False.
         """
-        return self.path is not None
+        return self.fs_type() == "os"
 
     def add_option(self, name: str, value: Any) -> None:
         """Add an option to the network scenario.
 
         Args:
             name (str): The name of the option.
             value (Any): The value of the option.
@@ -362,15 +357,15 @@
 
         Returns:
             bool: True if the devices are all in the network scenario, else False.
         """
         return all(map(lambda x: self.find_machine(x), machine_names))
 
     def __repr__(self) -> str:
-        return "Lab(%s, %s, %s, %s)" % (self.path, self.hash, self.machines, self.links)
+        return "Lab(%s, %s, %s, %s)" % (self.fs, self.hash, self.machines, self.links)
 
     def __str__(self) -> str:
         lab_info = ""
 
         if self._name:
             lab_info += "Name: %s\n" % self._name
```

### Comparing `kathara-3.5.5/src/Kathara/model/Link.py` & `kathara-3.6.0/src/Kathara/model/Link.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/os/Networking.py` & `kathara-3.6.0/src/Kathara/os/Networking.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/parser/netkit/DepParser.py` & `kathara-3.6.0/src/Kathara/parser/netkit/DepParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/parser/netkit/ExtParser.py` & `kathara-3.6.0/src/Kathara/parser/netkit/ExtParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/parser/netkit/FolderParser.py` & `kathara-3.6.0/src/Kathara/parser/netkit/FolderParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/parser/netkit/LabParser.py` & `kathara-3.6.0/src/Kathara/parser/netkit/LabParser.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,18 @@
             raise IOError("Cannot open lab.conf file.")
 
         lab = Lab(None, path=path)
 
         line_number = 1
         line = lab_mem_file.readline().decode('utf-8')
         while line:
-            matches = re.search(r"^(?P<key>[a-z0-9_]{1,30})\[(?P<arg>\w+)\]=(?P<value>\".+\"|\'.+\'|\w+)$",
-                                line.strip())
+            matches = re.search(
+                r"^(?P<key>[a-z0-9_]{1,30})\[(?P<arg>\w+)\]=([\"\']?)(?P<value>[^\"\']+)(\3)(\s+\#.*)?$",
+                line.strip()
+            )
 
             if matches:
                 key = matches.group("key").strip()
                 arg = matches.group("arg").strip()
                 value = matches.group("value").replace('"', '').replace("'", '')
 
                 if key in RESERVED_MACHINE_NAMES:
@@ -54,29 +56,29 @@
                 try:
                     # It's an interface, handle it.
                     interface_number = int(arg)
 
                     if re.search(r"^\w+$", value):
                         lab.connect_machine_to_link(key, value, machine_iface_number=interface_number)
                     else:
-                        raise ValueError(f"In lab.conf - Line {line_number}: "
-                                         f"Collision domain `{value}` contains non-alphanumeric characters.")
+                        raise SyntaxError(f"In lab.conf - Line {line_number}: "
+                                          f"Collision domain `{value}` contains non-alphanumeric characters.")
                 except ValueError:
                     # Not an interface, add it to the machine metas.
                     lab.assign_meta_to_machine(key, arg, value)
             else:
                 if not line.startswith('#') and \
                         line.strip():
                     if not line.startswith("LAB_NAME=") and \
                             not line.startswith("LAB_DESCRIPTION=") and \
                             not line.startswith("LAB_VERSION=") and \
                             not line.startswith("LAB_AUTHOR=") and \
                             not line.startswith("LAB_EMAIL=") and \
                             not line.startswith("LAB_WEB="):
-                        raise SyntaxError("In lab.conf - Line %d: Invalid characters `%s`." % (line_number, line))
+                        raise SyntaxError(f"In lab.conf - Line {line_number}: `{line}`")
                     else:
                         (key, value) = line.split("=")
                         key = key.replace("LAB_", "").lower()
                         setattr(lab, key, value.replace('"', '').replace("'", '').strip())
 
             line_number += 1
             line = lab_mem_file.readline().decode('utf-8')
```

### Comparing `kathara-3.5.5/src/Kathara/parser/netkit/OptionParser.py` & `kathara-3.6.0/src/Kathara/parser/netkit/OptionParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/setting/Setting.py` & `kathara-3.6.0/src/Kathara/setting/Setting.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/setting/addon/DockerSettingsAddon.py` & `kathara-3.6.0/src/Kathara/setting/addon/DockerSettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/setting/addon/KubernetesSettingsAddon.py` & `kathara-3.6.0/src/Kathara/setting/addon/KubernetesSettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/strings.py` & `kathara-3.6.0/src/Kathara/strings.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/test/BuiltinTest.py` & `kathara-3.6.0/src/Kathara/test/BuiltinTest.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/test/UserTest.py` & `kathara-3.6.0/src/Kathara/test/UserTest.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/__init__.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/console_menu.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/console_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/__init__.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/__init__.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/menu_borders.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_borders.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/menu_margins.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_margins.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/menu_padding.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_padding.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/format/menu_style.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_style.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/command_item.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/command_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/external_item.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/external_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/function_item.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/function_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/selection_item.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/selection_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/items/submenu_item.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/submenu_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/menu_component.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/menu_component.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/menu_formatter.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/menu_formatter.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/multiselect_menu.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/multiselect_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/prompt_utils.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/screen.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/screen.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/selection_menu.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/selection_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/validators/base.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/base.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/validators/regex.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/regex.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/consolemenu/validators/url.py` & `kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/url.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/curses/curses.py` & `kathara-3.6.0/src/Kathara/trdparty/curses/curses.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/depgen/depgen.py` & `kathara-3.6.0/src/Kathara/trdparty/depgen/depgen.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/trdparty/libtmux/tmux.py` & `kathara-3.6.0/src/Kathara/trdparty/libtmux/tmux.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def add_window(self, session_name, machine_name, shell, cwd=None):
         session_name = "Kathara" if not session_name else session_name
 
         initial_window_name = "%008x" % random.getrandbits(32)
         session, added = self.add_session(session_name, initial_window_name)
 
-        machine_window = session.find_where({"window_name": machine_name})
+        machine_window = session.windows.get(window_name=machine_name, default=None)
         if not machine_window:
             logging.debug("Starting TMUX window for `%s`..." % machine_name)
             session.new_window(window_name=machine_name, window_shell=shell, start_directory=cwd)
 
         if added:
             self.kill_window(session, initial_window_name)
 
@@ -50,15 +50,15 @@
             if 'duplicate session' in e.args[0][0]:
                 session = self._get_session_from_server(session_name)
                 self.add_session_by_name(session_name, session)
                 return session, False
 
         logging.debug("Initialized TMUX session %s" % session_name)
 
-        session = self._server.find_where({"session_name": session_name})
+        session = self._server.sessions.get(session_name=session_name)
         self.add_session_by_name(session_name, session)
 
         return session, True
 
     def add_session_by_name(self, session_name, session):
         if session_name not in self._sessions:
             self._sessions[session_name] = session
@@ -67,17 +67,17 @@
         if session_name in self._sessions:
             return self._sessions[session_name]
 
         return None
 
     def _get_session_from_server(self, session_name):
         if self._server.has_session(session_name):
-            return self._server.find_where({"session_name": session_name})
+            return self._server.sessions.get(session_name=session_name)
 
         return None
 
     @staticmethod
     def kill_window(session, window_name):
-        window = session.find_where({"window_name": window_name})
+        window = session.windows.get(window_name=window_name, default=None)
 
         if window:
             window.kill_window()
```

### Comparing `kathara-3.5.5/src/Kathara/utils.py` & `kathara-3.6.0/src/Kathara/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,29 +157,35 @@
         return "armv7"
     elif architecture == "armv6l":
         return "armv6"
     else:
         raise HostArchitectureError(architecture)
 
 
-def convert_win_2_linux(filename: str) -> bytes:
+def convert_win_2_linux(filename: str, write: bool = False) -> Optional[bytes]:
     if not is_binary(filename):
         file_obj = None
         try:
             file_obj = open(filename, mode='r', encoding='utf-8-sig')
-            file_content = file_obj.read()
-            return file_content.replace("\n\r", "\n").encode('utf-8')
+            file_content = file_obj.read().replace("\n\r", "\n").replace("\r\n", "\n")
+            if not write:
+                return file_content.encode('utf-8')
+            else:
+                with open(filename, mode='w', encoding='utf-8', newline="\n") as file_obj_write:
+                    file_obj_write.write(file_content)
+                return
         except Exception:
             # In any case the binaryornot heuristics fail (so the file is not a text file), close the stream and
             # read the file as a standard binary file.
             if file_obj:
                 file_obj.close()
             pass
 
-    return open(filename, mode='rb').read()
+    if not write:
+        return open(filename, mode='rb').read()
 
 
 def is_admin() -> bool:
     def unix_root():
         return os.getuid() == 0
 
     def windows_admin():
@@ -303,13 +309,7 @@
                 tar_file.addfile(tar_info, file_content)
 
         temp_file.seek(0)
 
         tar_data = temp_file.read()
 
     return tar_data
-
-
-def is_excluded_file(path: str) -> bool:
-    _, filename = os.path.split(path)
-
-    return filename in EXCLUDED_FILES
```

### Comparing `kathara-3.5.5/src/Kathara/validator/ImageValidator.py` & `kathara-3.6.0/src/Kathara/validator/ImageValidator.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/webhooks/DockerHubApi.py` & `kathara-3.6.0/src/Kathara/webhooks/DockerHubApi.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/Kathara/webhooks/GitHubApi.py` & `kathara-3.6.0/src/Kathara/webhooks/GitHubApi.py`

 * *Files identical despite different names*

### Comparing `kathara-3.5.5/src/kathara.egg-info/SOURCES.txt` & `kathara-3.6.0/src/kathara.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 src/kathara.py
 src/Kathara/__init__.py
 src/Kathara/decorators.py
 src/Kathara/exceptions.py
 src/Kathara/strings.py
@@ -60,14 +61,16 @@
 src/Kathara/foundation/manager/__init__.py
 src/Kathara/foundation/manager/stats/ILinkStats.py
 src/Kathara/foundation/manager/stats/IMachineStats.py
 src/Kathara/foundation/manager/stats/__init__.py
 src/Kathara/foundation/manager/terminal/Terminal.py
 src/Kathara/foundation/manager/terminal/__init__.py
 src/Kathara/foundation/manager/terminal/terminal_utils.py
+src/Kathara/foundation/model/FilesystemMixin.py
+src/Kathara/foundation/model/__init__.py
 src/Kathara/foundation/setting/SettingsAddon.py
 src/Kathara/foundation/setting/SettingsAddonFactory.py
 src/Kathara/foundation/setting/__init__.py
 src/Kathara/foundation/test/Test.py
 src/Kathara/foundation/test/__init__.py
 src/Kathara/manager/Kathara.py
 src/Kathara/manager/__init__.py
@@ -144,14 +147,16 @@
 src/Kathara/trdparty/consolemenu/validators/url.py
 src/Kathara/trdparty/curses/__init__.py
 src/Kathara/trdparty/curses/curses.py
 src/Kathara/trdparty/depgen/__init__.py
 src/Kathara/trdparty/depgen/depgen.py
 src/Kathara/trdparty/libtmux/__init__.py
 src/Kathara/trdparty/libtmux/tmux.py
+src/Kathara/trdparty/strtobool/__init__.py
+src/Kathara/trdparty/strtobool/strtobool.py
 src/Kathara/validator/ImageValidator.py
 src/Kathara/validator/TerminalValidator.py
 src/Kathara/validator/__init__.py
 src/Kathara/webhooks/DockerHubApi.py
 src/Kathara/webhooks/GitHubApi.py
 src/Kathara/webhooks/__init__.py
 src/kathara.egg-info/PKG-INFO
```

### Comparing `kathara-3.5.5/src/kathara.py` & `kathara-3.6.0/src/kathara.py`

 * *Files identical despite different names*

