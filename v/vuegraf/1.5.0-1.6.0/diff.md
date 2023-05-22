# Comparing `tmp/vuegraf-1.5.0.tar.gz` & `tmp/vuegraf-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vuegraf-1.5.0.tar", last modified: Tue Jan  3 00:03:39 2023, max compression
+gzip compressed data, was "vuegraf-1.6.0.tar", last modified: Mon May 22 11:31:01 2023, max compression
```

## Comparing `vuegraf-1.5.0.tar` & `vuegraf-1.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:03:39.736244 vuegraf-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-03 00:03:22.000000 vuegraf-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-01-03 00:03:39.736244 vuegraf-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-01-03 00:03:22.000000 vuegraf-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-03 00:03:39.736244 vuegraf-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-01-03 00:03:22.000000 vuegraf-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:03:39.736244 vuegraf-1.5.0/vuegraf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-01-03 00:03:39.000000 vuegraf-1.5.0/vuegraf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-03 00:03:39.000000 vuegraf-1.5.0/vuegraf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 00:03:39.000000 vuegraf-1.5.0/vuegraf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-03 00:03:39.000000 vuegraf-1.5.0/vuegraf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-03 00:03:39.000000 vuegraf-1.5.0/vuegraf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 00:03:39.000000 vuegraf-1.5.0/vuegraf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:31:01.523576 vuegraf-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-22 11:30:50.000000 vuegraf-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-22 11:31:01.523576 vuegraf-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-22 11:30:50.000000 vuegraf-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:31:01.523576 vuegraf-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-22 11:30:50.000000 vuegraf-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:31:01.523576 vuegraf-1.6.0/vuegraf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-22 11:31:01.000000 vuegraf-1.6.0/vuegraf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-22 11:31:01.000000 vuegraf-1.6.0/vuegraf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:31:01.000000 vuegraf-1.6.0/vuegraf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 11:31:01.000000 vuegraf-1.6.0/vuegraf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 11:31:01.000000 vuegraf-1.6.0/vuegraf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:31:01.000000 vuegraf-1.6.0/vuegraf.egg-info/top_level.txt
```

### Comparing `vuegraf-1.5.0/LICENSE` & `vuegraf-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vuegraf-1.5.0/README.md` & `vuegraf-1.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,81 @@
+![Vuegraf Logo](https://github.com/jertel/vuegraf/blob/master/vuegraf.png?raw=true "Vuegraf Logo")
+
 # Overview
 
 The [Emporia Vue](https://emporiaenergy.com "Emporia's Homepage") energy monitoring kit allows homeowners to monitor their electrical usage. It monitors the main feed consumption and up to 8 (or 16 in the newer version) individual branch circuits, and feeds that data back to the Emporia API server.
 
-This project, Vuegraf, fetches those metrics from the Emporia Vue API host and stores the metrics into your own InfluxDB. When paired with Grafana you'll be able to:
+This project, Vuegraf, fetches those metrics from the Emporia Vue API host and stores the metrics into your own InfluxDB. After installation you will be able to:
 * View your energy usage across all circuits on a single graph
 * Create alerts to notify when certain energy usage thresholds are exceeded
 
 This project is not affiliated with _emporia energy_ company.
 
 # Dependencies
 
-## Required
 * [Emporia Vue](https://emporiaenergy.com "Emporia Energy") Account - Username and password for the Emporia Vue system are required.
 * [Python 3](https://python.org "Python") - With Pip.
-* [InfluxDB](https://influxdata.com "InfluxDB") - Host, port, and login credentials are required.
+* [InfluxDB 2](https://influxdata.com "InfluxDB") - Host, port, org, bucket, and token are all required.
+
+# Influx
+
+## Setup
 
-## Recommended
-* [Grafana](https://grafana.com "Grafana") - Can be used to read metrics from the InfluxDB.
+If you do not yet have a running InfluxDB 2 instance, you will need to set one up. You can do this very quickly by launching an InfluxDB 2 Docker container as follows:
 
-# Screenshots
+```
+mkdir -p /home/myuser/influxdb2
+docker run -v /home/myuser/influxdb2:/var/lib/influxdb2 -p 8086:8086 -e INFLUXD_SESSION_LENGTH=432000 --name influxdb influxdb
+```
 
-The following screenshots are provided to illustrate the possibilities available after using Vuegraf. These were all taken from a functionaing Grafana installation.
+Substitute an appropriate host path for the `/home/myuser/influxdb2` location above. Once running, access the web UI at `http://localhost:8086`. It will prompt you for a username, password, organization name, and bucket name. The rest of this document assumes you have entered the word `vuegraf` for all of these inputs.
 
-A sample Grafana dashboard is shown below:
+Note that the default session timeout for Influx is only 60 minutes, so this command increases the login session to 300 days.
 
-![Dashboard Example Screenshot](https://github.com/jertel/vuegraf/blob/master/screenshots/dashboard.png?raw=true "Dashboard Example")
+Once logged in, go to the _Load Data -> API Tokens_ screen and generate a new All Access token with the description of _vuegraf_. Copy the generated token for use in the rest of this document, specifically when referenced as `<my-influx-token>`.
 
-A single graph showing multiple overlayed circuits is shown below:
+## Dashboard
 
-![Graph Example Screenshot](https://github.com/jertel/vuegraf/blob/master/screenshots/graph.png?raw=true "Graph Example")
+By default, a new InfluxDB instance will not have any dashboards loaded. You will need to import the included Influx JSON template, or create your own dashboard in order to visualize your energy usage.
+
+The included template file named `influx_dashboard.json` includes the provided dashboard and accompanying variables to reproduce the visualizations shown below. This dashboard assumes your main device name contains the word `Panel`, such as `House Panel`, or `Right Panel`. If it does not, the Flux queries will need to be adjusted manually to look for your device's name.
+
+![Influx Dashboard Screenshot](https://github.com/jertel/vuegraf/blob/master/screenshots/influx_dashboard.png?raw=true "Influx Dashboard")
+
+You will need to apply this template file to your running InfluxDB instance. Copy the `influx_dashboard.json` file into your host's influxdb2 path. If you followed the Setup instructions above, the path would be `/home/myuser/influxdb2`. The below command can be used to perform this step. This command assumes you are running Influx in a container named `influxdb`.
+
+```
+docker exec influxdb influx apply -f /var/lib/influxdb2/influx_dashboard.json --org vuegraf --force yes -t <my-influx-token>
+```
+
+Replace the `<my-influx-token>` with the All Access Token you generated in the Influx _Load Data -> API Tokens_ screen.
+
+You're now ready to proceed with the Vuegraf configuration and startup.
 
 # Configuration
+
 The configuration allows for the definition of multiple Emporia Vue accounts. This will only be useful to users that need to pull metrics from multiple accounts. This is not needed if you have multiple Vue devices in a single account. Vuegraf will find multiple devices on its own within each account.
 
 The email address and password must match the credentials used when creating the Emporia Vue account in their mobile app.
 
 Important: Ensure that sufficient protection is in place on this configuration file, since it contains the plain-text login credentials into the Emporia Vue account.
 
 A [sample configuration file](https://github.com/jertel/vuegraf/blob/master/vuegraf.json.sample "Sample Vuegraf Configuration File") is provided in this repository, and details are described below.
 
 ## Minimal Configuration
 The minimum configuration required to start Vuegraf is shown below.
 
-InfluxDB v1:
-
-```json
-{
-    "influxDb": {
-        "host": "my.influxdb.hostname",
-        "port": 8086,
-        "user": "root",
-        "pass": "root",
-        "database": "vue",
-        "reset": false
-    },
-    "accounts": [
-        {
-            "name": "Primary Residence",
-            "email": "my@email.address",
-            "password": "my-emporia-password"
-        }
-    ]
-}
-```
-
-InfluxDB v2:
-
 ```json
 {
     "influxDb": {
         "version": 2,
         "url": "http://my.influxdb.hostname:8086",
         "org": "vuegraf",
         "bucket": "vuegraf",
-        "token": "veugraf-secret-token",
-        "reset": false
+        "token": "<my-secret-token>",
     },
     "accounts": [
         {
             "name": "Primary Residence",
             "email": "my@email.address",
             "password": "my-emporia-password"
         }
@@ -86,22 +83,29 @@
 }
 ```
 
 ## Advanced Configuration
 
 ### Ingesting Historical Data
 
-If desired, it is possible to have Vuegraf import historical data. To do so, specify a new temporary parameter called `historyDays` inside the `influxDb` section, with an integer value greater than zero. Once restarted, One-minute data from the past `historyDays` days will be ingested into InfluxDB. Emporia currently retains this data for 7 days, and therefore `historyDays` must be less than or equal to `7`. If `historyDays` is set to `0`, no historical data will be ingested into InfluxDB.
+If desired, it is possible to have Vuegraf import historical data. To do so, run vuegraf.py with the optional `--historydays` parameter with a value between 1 and 720.  When this parameter is provided Vuegraf will start and collect all hourly data points up to the specified parameter, or max history available.  It will also collect one day's summary data for each day, storing it with the timestamp 23:59:59 for each day.  It collects the time using your local server time, but stores it in influxDB in UTC.
+
+IMPORTANT - If you restart Vuegraf with `--historydays` on the command line (or forget to remove it from the dockerfile) it will import history data _again_. This will likely cause confusion with your data since you will now have duplicate/overlapping data. For best results, only enable `--historydays` on a single run.
 
-IMPORTANT - If you restart Vuegraf with historyDays still set to a non-zero value then it will _again_ import history data. This will likely cause confusion with your data since you will now have duplicate/overlapping data. For best results, only enable historyDays > 0 for a single run, and then immediately set it back to 0 to avoid this duplicated import data scenario.
+For Example:
+```
+python3 path/to/vuegraf.py vuegraf.json --historydays 365
+```
 
 ### Channel Names
 
 To provide more user-friendly names of each Vue device and branch circuit, the following device configuration can be added to the configuration file, within the account block. List each device and circuit in the order that you added them to the Vue mobile app. The channel names do not need to match the names specified in the Vue mobile app but the device names must match. The below example shows two 8-channel Vue devices for a home with two breaker panels.
 
+Be aware that the included dashboard assumes your device name contains the word "Panel". For best results, consider renaming your Vue device to contain that word, otherwise you will need to manually adjust the included dashboards' queries.
+
 ```json
             "devices": [
                 {
                     "name": "Right Panel",
                     "channels": [
                         "Air Conditioner",
                         "Furnace",
@@ -125,56 +129,30 @@
                         "Deep Freeze",
                         "Sprinkler Pump"        
                     ]
                 }
             ]
 ```
 
-### Per-second Data Details
-
-By default, Vuegraf will poll every minute to collect the energy usage value over the past 60 seconds. This results in a single value being capture per minute per channel, or 60 values per hour per channel. If you also would like to see per-second values, you can enable the detailed collection, which is polled once per hour, and backfilled over the previous 3600 seconds. This API call is very expensive on the Emporia servers, so it should not be polled more frequently than once per hour. To enable this detailed data, add (or update) the top-level `detailedDataEnabled` configuration value with a value of `true`.
-
-```
-detailedDataEnabled: true
-```
-
-## Vue Utility Connect Energy Monitor
-
-As reported in [discussion #104](https://github.com/jertel/vuegraf/discussions/104), the Utility Connect device is supported without any custom changes.
+# Running
+Vuegraf can be run either as a container (recommended), or as a host process.
 
-## Smart Plugs
+## Container (recommended)
 
-To include an Emporia smart plug in the configuration, add each plug as it's own device, without channels. Again, the name of the Smart Plug device must exactly match the name you gave the device in the Vue app during initial registration.
+A Docker container is provided at [hub.docker.com](https://hub.docker.com/r/jertel/vuegraf). Refer to the command below to launch Vuegraf as a container. This assumes you have created a folder called `/home/myuser/vuegraf` and placed the vuegraf.json file inside of it.
 
-```json
-            devices: [
-                {
-                    "name": "Main Panel",
-                    "channels": [
-                        "Air Conditioner",
-                        "Furnace",
-                        "Coffee Maker",
-                        "Oven",
-                        "Dishwasher",
-                        "Tesla Charger",
-                        "Refrigerator",
-                        "Office"
-                    ]
-                },
-                {
-                    "name": "Projector Plug"
-                },
-                {
-                    "name": "3D-Printer Plug"
-                }
-            ]
+Normal run with docker
+```sh
+docker run --name vuegraf -d -v /home/myuser/vuegraf:/opt/vuegraf/conf jertel/vuegraf
 ```
 
-# Running
-Vuegraf can be run either as a host process, or as a container (recommended).
+Recreate database and load 25 days of history
+```sh
+docker run --name vuegraf -d -v /home/myuser/vuegraf:/opt/vuegraf/conf jertel/vuegraf --resetdatabase --historydays=24
+```
 
 ## Host Process
 
 Ensure Python 3 and Pip are both installed. Install the required dependencies:
 
 ```sh
 pip install -r src/requirements.txt
@@ -192,63 +170,133 @@
 python src/vuegraf/vuegraf.py vuegraf.json
 ```
 or, on some Linux installations:
 ```sh
 python3 src/vuegraf/vuegraf.py vuegraf.json
 ```
 
-## Container (recommended)
+Optional Command Line Parameters
+```
+usage: vuegraf.py [-h] [--version] [-v] [-q] [--historydays HISTORYDAYS] [--resetdatabase] configFilename
 
-A Docker container is provided at [hub.docker.com](https://hub.docker.com/r/jertel/vuegraf). Refer to the command below to launch Vuegraf as a container. This assumes you have create a folder called vuegraf and placed the vuegraf.json file inside of it.
+Retrieves data from cloud servers and inserts it into an InfluxDB database.
 
-```sh
-docker run --name vuegraf -d -v /home/myusername/vuegraf:/opt/vuegraf/conf jertel/vuegraf
+positional arguments:
+  configFilename        JSON config file
+
+options:
+  -h, --help            show this help message and exit
+  --version             Display version number
+  -v, --verbose         Verbose output - summaries
+  --historydays HISTORYDAYS
+                        Starts executing by pulling history of Hours and Day data for specified number of days.
+                        example: --load-history-day 60
+  --resetdatabase       Drop database and create a new one
 ```
 
-If you are new to Docker, the next two commands will help you get the InfluxDB (version 1) and Grafana containers up and running, assuming you have Docker installed and running already. In the above config example, your influxdb host name will be your host's real IP (*not* localhost or 127.0.0.1).
+## Alerts
 
-```sh
-docker run -d --name influxdb -v /home/myusername/vuegraf:/var/lib/influxdb -p 8086:8086 influxdb:1.8-alpine
-docker run -d --name grafana -v /home/myusername/vuegraf:/var/lib/grafana -p 3000:3000 grafana/grafana
-```
+The included dashboard template contains two alerts which will trigger when either a power outage occurs, or a loss of Vuegraf data. There are various reasons why alerts can be helpful. See the below screenshots which help illustrate how a fully functioning alert and notification rule might look. Note that the included alerts do not send out notifications. To enable outbound notifactions, such as to Slack, you can create a Notification Endpoint and Notification Rule.
 
-### Docker Compose
+This alert was edited via the text (Flux) interface since the alert edit UI does not yet accommodate advanced alerting inputs.
 
-For those that want to run Vuegraf using Docker Compose, the following files have been included: `docker-compose.yaml.template` and `docker-compose-run.sh`. These assume InfluxDB version 1 will be utilized. Copy the`docker-compose.yaml.template` file to a new file called `docker-compose.yaml`. In the newly copied file, `vuegraf.volumes` values will need to be changed to the same directory you have created your vuegraf.json file. Additionally, adjust the persistent host storage path for the Grafana and InfluxDB data volumes.
+Side note: The logo at the top of this documentation satisfies Slack's icon requirements. Consider using it to help quickly distinguish between other alerts.
 
-Finally run the `docker-compose-run.sh` script to start up the multi-container application. 
+![Influx Alert Edit](https://github.com/jertel/vuegraf/blob/master/screenshots/alert_edit.png?raw=true "Influx Alert")
 
-```sh
-./docker-compose-run.sh
+This notification rule provides an example of how you can have several alerts change the status to crit, but only a single notification rule is required to transmit notifications to external endpoints (such as email or Slack).
+
+![Influx Notification Rule](https://github.com/jertel/vuegraf/blob/master/screenshots/notification_rule.png?raw=true "Influx Notification Rule")
+
+
+# Additional Topics
+
+## Per-second Data Details
+
+By default, Vuegraf will poll every minute to collect the energy usage value over the past 60 seconds. This results in a single value being capture per minute per channel, or 60 values per hour per channel. If you also would like to see per-second values, you can enable the detailed collection, which is polled once per hour, and backfilled over the previous 3600 seconds. This API call is very expensive on the Emporia servers, so it should not be polled more frequently than once per hour. To enable this detailed data, add (or update) the top-level `detailedDataEnabled` configuration value with a value of `true`.  The details is also what pulls the Hourly datapoint.  
+
+```
+detailedDataEnabled: true
 ```
 
-# Grafana
+For every datapoint a tag is stored in InfluxDB for the type of measurement
+
+- `detailed = True` represents backfilled per-second data that is optionally queried from Emporia once every hour.
+- `detailed = False` represents the per-minute average data that is collected every minute.
+- `detailed = Hour` represents the data summarized in hours
+- `detailed = Day` represents a single data point to summarize the entire day
+
+When building graphs that show a sum of the energy usage, be sure to only include the correct detail tag, otherwise your summed values will be higher than expected. Detailed data will take more time for the graphs to query due to the extra data involved. If you want to have a chart that shows daily data over a long period or even a full year, use the `detailed = Day` tag.
+If you are running this on a small server, you might want to look at setting a RETENTION POLICY on your InfluxDB bucket to remove minute or second data over time. For example, it will reduce storage needs if you retain only 30 days of per-_second_ data. 
+
+## Vue Utility Connect Energy Monitor
+
+As reported in [discussion #104](https://github.com/jertel/vuegraf/discussions/104), the Utility Connect device is supported without any custom changes.
+
+## Smart Plugs
+
+To include an Emporia smart plug in the configuration, add each plug as it's own device, without channels. Again, the name of the Smart Plug device must exactly match the name you gave the device in the Vue app during initial registration.
 
-Use [Grafana](https://grafana.com "Grafana") to visualize the data collected by Vuegraf. A sample [dashboard.json](https://github.com/jertel/vuegraf/blob/master/dashboard.json) file is provided with this project, to get started. However, this sample dashboard is only compatible with InfluxDB version 1.
+```json
+            devices: [
+                {
+                    "name": "Main Panel",
+                    "channels": [
+                        "Air Conditioner",
+                        "Furnace",
+                        "Coffee Maker",
+                        "Oven",
+                        "Dishwasher",
+                        "Tesla Charger",
+                        "Refrigerator",
+                        "Office"
+                    ]
+                },
+                {
+                    "name": "Projector Plug"
+                },
+                {
+                    "name": "3D-Printer Plug"
+                }
+            ]
+```
 
-If you only have one Vue device you should remove the Left/Right panel references.
+## Docker Compose
 
-Refer to the screenshots below for examples on how to define the InfluxDB data source, graphs, and alerts.
+For those that want to run Vuegraf using Docker Compose, the following files have been included: `docker-compose.yaml.template` and `docker-compose-run.sh`. Copy the`docker-compose.yaml.template` file to a new file called `docker-compose.yaml`. In the newly copied file, `vuegraf.volumes` values will need to be changed to the same directory you have created your vuegraf.json file. Additionally, adjust the persistent host storage path for the InfluxDB data volume.
 
-NOTE: The energy_usage measurement includes two types of data:
+Finally run the `docker-compose-run.sh` script to start up the multi-container application. 
 
-- `detailed = true` represents backfilled per-second data that is optionally queried from Emporia once every hour.
-- `detailed = false` represents the per-minute average data that is collected every minute.
+```sh
+./docker-compose-run.sh
+```
 
-When building graphs that show a sum of the energy usage, be sure to only include either detailed=true or detailed=false, otherwise your summed values will be higher than expected.
+## Upgrading from InfluxDB v1
 
+Early Vuegraf users still on InfluxDB v1 can upgrade to InfluxDB 2. To do so, stop the Influx v1 container (again, assuming you're using Docker). Then run the following command to install InfluxDB 2 and automatically upgrade your data.
 
-![Grafana Data Source Screenshot](https://github.com/jertel/vuegraf/blob/master/screenshots/datasource.png?raw=true "Data Source Example")
+```
+docker run --rm --pull always -p 8086:8086 \
+  -v /home/myuser/influxdb:/var/lib/influxdb \
+  -v /home/myuser/influxdb2:/var/lib/influxdb2 \
+  -e DOCKER_INFLUXDB_INIT_MODE=upgrade \
+  -e DOCKER_INFLUXDB_INIT_USERNAME=vuegraf \
+  -e DOCKER_INFLUXDB_INIT_PASSWORD=vuegraf \
+  -e DOCKER_INFLUXDB_INIT_ORG=vuegraf \
+  -e DOCKER_INFLUXDB_INIT_BUCKET=vuegraf \
+  -e DOCKER_INFLUXDB_INIT_RETENTION=1y \
+  influxdb
+```
 
-A graph query is shown below, showing a simple filter to pull data for a specific circuit.
+Adjust the host paths above as necessary, to match the old and new influxdb directories. The upgrade should complete relatively quickly. For reference, a 7GB database, spanning several months, upgrades in about 15 seconds on SSD storage.
 
-![Query Example Screenshot](https://github.com/jertel/vuegraf/blob/master/screenshots/query.png?raw=true "Query Example")
+Monitor the console output and once the upgrade completes and the Influx server finishes starting, shut it down (CTRL+C) and then restart the Influx DB using the command referenced earlier in this document.
 
-Grafana also supports alerts, with a number of alert channels, such as Email or Slack.
+Login to the new Influx DB 2 UI from your web browser, using the _vuegraf / vuegraf_ credentials. Go into the _Load Data -> Buckets_ screen and rename the `vue/autogen` bucket to `vuegraf` via the Settings button.
 
-![Alert Example Screenshot](https://github.com/jertel/vuegraf/blob/master/screenshots/alert.png?raw=true "Alert Example")
+Finally, apply the dashboard template as instructed earlier in this document.
 
 # License
 
 Vuegraf is distributed under the MIT license.
 
 See [LICENSE](https://github.com/jertel/vuegraf/blob/master/LICENSE) for more information.
```

### Comparing `vuegraf-1.5.0/setup.py` & `vuegraf-1.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages
 from setuptools import setup
 
 base_dir = os.path.dirname(__file__)
 setup(
     name='vuegraf',
-    version='1.5.0',
+    version='1.6.0',
     author='Jason Ertel',
     url='https://github.com/jertel/vuegraf',
     description='Populate metrics from your Emporia Vue energy monitoring devices into an InfluxDB',
     setup_requires='setuptools',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.9',
@@ -19,10 +19,11 @@
     entry_points={
         'console_scripts': ['vuegraf=vuegraf.vuegraf']
     },
     packages=find_packages(),
     install_requires=[
         'influxdb>=5.3.1',
         'influxdb_client>=1.33.0',
-        'pyemvue>=0.16.0'
+        'pyemvue>=0.16.0',
+        'argparse>= 1.4.0'
     ]
 )
```

