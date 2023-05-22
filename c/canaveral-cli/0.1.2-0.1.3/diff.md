# Comparing `tmp/canaveral_cli-0.1.2.tar.gz` & `tmp/canaveral_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canaveral_cli-0.1.2.tar", max compression
+gzip compressed data, was "canaveral_cli-0.1.3.tar", max compression
```

## Comparing `canaveral_cli-0.1.2.tar` & `canaveral_cli-0.1.3.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0    11337 2023-04-20 10:01:17.537352 canaveral_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0     1063 2023-05-14 19:06:08.041164 canaveral_cli-0.1.2/README.md
--rw-r--r--   0        0        0     1479 2023-05-22 17:30:09.113480 canaveral_cli-0.1.2/canaveral_cli/__init__.py
--rw-r--r--   0        0        0      204 2023-05-22 17:30:04.733480 canaveral_cli-0.1.2/canaveral_cli/__main__.py
--rw-r--r--   0        0        0     2425 2023-05-22 17:34:59.783480 canaveral_cli-0.1.2/canaveral_cli/cli.py
--rw-r--r--   0        0        0    14128 2023-05-22 17:29:58.633479 canaveral_cli-0.1.2/canaveral_cli/create_oam.py
--rw-r--r--   0        0        0     6868 2023-05-22 17:29:51.893478 canaveral_cli-0.1.2/canaveral_cli/cue_parser.py
--rw-r--r--   0        0        0     2480 2023-05-22 17:29:46.123477 canaveral_cli-0.1.2/canaveral_cli/definitions.py
--rw-r--r--   0        0        0     1129 2023-05-22 17:29:42.993476 canaveral_cli-0.1.2/canaveral_cli/merge_oam.py
--rw-r--r--   0        0        0     5155 2023-05-21 14:53:02.338953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/cron-task.json
--rw-r--r--   0        0        0     3305 2023-05-21 14:53:02.948953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/daemon.json
--rw-r--r--   0        0        0      280 2023-05-21 14:53:03.458953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/k8s-objects.json
--rw-r--r--   0        0        0     2997 2023-05-21 14:53:04.038953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/task.json
--rw-r--r--   0        0        0     3558 2023-05-21 14:53:04.568953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/webservice.json
--rw-r--r--   0        0        0      627 2023-05-21 14:53:05.098953 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/apply-once.json
--rw-r--r--   0        0        0     1314 2023-05-21 14:53:05.748953 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/garbage-collect.json
--rw-r--r--   0        0        0      643 2023-05-21 14:53:06.368952 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/override.json
--rw-r--r--   0        0        0      402 2023-05-21 14:53:06.888952 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/read-only.json
--rw-r--r--   0        0        0      644 2023-05-21 14:53:07.418951 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/replication.json
--rw-r--r--   0        0        0      383 2023-05-21 14:53:07.918951 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/resource-update.json
--rw-r--r--   0        0        0      403 2023-05-21 14:53:08.498950 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/shared-resource.json
--rw-r--r--   0        0        0      400 2023-05-21 14:53:08.998949 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/take-over.json
--rw-r--r--   0        0        0      829 2023-05-21 14:53:09.548949 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/topology.json
--rw-r--r--   0        0        0      287 2023-05-21 14:53:10.048948 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/annotations.json
--rw-r--r--   0        0        0      279 2023-05-21 14:53:10.728947 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/command.json
--rw-r--r--   0        0        0      226 2023-05-21 14:53:11.318947 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/container-image.json
--rw-r--r--   0        0        0     1184 2023-05-21 14:53:11.898946 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/cpuscaler.json
--rw-r--r--   0        0        0      271 2023-05-21 14:53:12.518945 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/env.json
--rw-r--r--   0        0        0      956 2023-05-21 14:53:13.238945 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/expose.json
--rw-r--r--   0        0        0     1932 2023-05-21 14:53:13.788945 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/gateway.json
--rw-r--r--   0        0        0      364 2023-05-21 14:53:14.308946 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/hostalias.json
--rw-r--r--   0        0        0     1427 2023-05-21 14:53:14.848947 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/hpa.json
--rw-r--r--   0        0        0     2013 2023-05-21 14:53:15.548948 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/init-container.json
--rw-r--r--   0        0        0      732 2023-05-21 14:53:16.148949 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/k8s-update-strategy.json
--rw-r--r--   0        0        0      271 2023-05-21 14:53:16.848950 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/labels.json
--rw-r--r--   0        0        0      465 2023-05-21 14:53:17.578951 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/lifecycle.json
--rw-r--r--   0        0        0      561 2023-05-21 14:53:18.148952 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/pure-ingress.json
--rw-r--r--   0        0        0      990 2023-05-21 14:53:18.648953 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/resource.json
--rw-r--r--   0        0        0      356 2023-05-21 14:53:19.188953 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/scaler.json
--rw-r--r--   0        0        0      817 2023-05-21 14:53:19.758954 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/service-account.json
--rw-r--r--   0        0        0     1673 2023-05-21 14:53:20.378955 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/sidecar.json
--rw-r--r--   0        0        0      333 2023-05-21 14:53:20.938955 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/startup-probe.json
--rw-r--r--   0        0        0     1014 2023-05-21 14:53:21.428955 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/storage.json
--rw-r--r--   0        0        0      366 2023-05-21 14:53:22.028957 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/topologyspreadconstraints.json
--rw-r--r--   0        0        0      519 2023-05-21 14:53:22.558959 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-component.json
--rw-r--r--   0        0        0      614 2023-05-21 14:53:23.228961 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-deployment.json
--rw-r--r--   0        0        0      585 2023-05-21 14:53:23.808963 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-object.json
--rw-r--r--   0        0        0     1803 2023-05-21 14:53:24.488966 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-terraform-config.json
--rw-r--r--   0        0        0      353 2023-05-21 14:53:25.158968 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-terraform-provider.json
--rw-r--r--   0        0        0     1840 2023-05-21 14:53:25.798970 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/build-push-image.json
--rw-r--r--   0        0        0     1293 2023-05-21 14:53:26.458970 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/check-metrics.json
--rw-r--r--   0        0        0      409 2023-05-21 14:53:27.188970 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/clean-jobs.json
--rw-r--r--   0        0        0     1394 2023-05-21 14:53:27.828971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/collect-service-endpoints.json
--rw-r--r--   0        0        0      818 2023-05-21 14:53:28.448971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/create-config.json
--rw-r--r--   0        0        0      465 2023-05-21 14:53:29.078971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/delete-config.json
--rw-r--r--   0        0        0      525 2023-05-21 14:53:29.638971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/depends-on-app.json
--rw-r--r--   0        0        0      585 2023-05-21 14:53:30.228971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/deploy-cloud-resource.json
--rw-r--r--   0        0        0     1124 2023-05-21 14:53:30.838971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/deploy.json
--rw-r--r--   0        0        0     1039 2023-05-21 14:53:31.548971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export-data.json
--rw-r--r--   0        0        0     1186 2023-05-21 14:53:32.118971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export-service.json
--rw-r--r--   0        0        0      867 2023-05-21 14:53:32.738971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export2config.json
--rw-r--r--   0        0        0     1358 2023-05-21 14:53:33.328971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export2secret.json
--rw-r--r--   0        0        0      583 2023-05-21 14:53:33.968971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/generate-jdbc-connection.json
--rw-r--r--   0        0        0      472 2023-05-21 14:53:34.478971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/list-config.json
--rw-r--r--   0        0        0      987 2023-05-21 14:53:34.988971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/notification.json
--rw-r--r--   0        0        0      268 2023-05-21 14:53:35.558971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/print-message-in-status.json
--rw-r--r--   0        0        0      461 2023-05-21 14:53:36.248971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/read-config.json
--rw-r--r--   0        0        0     1171 2023-05-21 14:53:36.858971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/read-object.json
--rw-r--r--   0        0        0      614 2023-05-21 14:53:37.488971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/request.json
--rw-r--r--   0        0        0      818 2023-05-21 14:53:38.018968 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/share-cloud-resource.json
--rw-r--r--   0        0        0      295 2023-05-21 14:53:38.608965 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/step-group.json
--rw-r--r--   0        0        0      577 2023-05-21 14:53:39.138962 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/suspend.json
--rw-r--r--   0        0        0      981 2023-05-21 14:53:39.708958 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/vela-cli.json
--rw-r--r--   0        0        0      563 2023-05-21 14:53:40.288956 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/webhook.json
--rw-r--r--   0        0        0     1091 2023-05-14 19:06:08.091164 canaveral_cli-0.1.2/canaveral_cli/templates/vela_default.yaml
--rw-r--r--   0        0        0     1364 2023-05-21 11:24:22.059044 canaveral_cli-0.1.2/canaveral_cli/templates/vela_template.yaml.jinja
--rw-r--r--   0        0        0      777 2023-05-22 17:40:36.483485 canaveral_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2286 2023-05-22 17:40:57.763514 canaveral_cli-0.1.2/setup.py
--rw-r--r--   0        0        0     1843 2023-05-22 17:40:57.763817 canaveral_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-20 10:01:17.537352 canaveral_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1063 2023-05-14 19:06:08.041164 canaveral_cli-0.1.3/README.md
+-rw-r--r--   0        0        0     1550 2023-05-22 17:50:50.943498 canaveral_cli-0.1.3/canaveral_cli/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-22 17:30:04.733480 canaveral_cli-0.1.3/canaveral_cli/__main__.py
+-rw-r--r--   0        0        0     2471 2023-05-22 18:00:00.663485 canaveral_cli-0.1.3/canaveral_cli/cli.py
+-rw-r--r--   0        0        0    14144 2023-05-22 18:01:21.403483 canaveral_cli-0.1.3/canaveral_cli/create_oam.py
+-rw-r--r--   0        0        0     6868 2023-05-22 17:29:51.893478 canaveral_cli-0.1.3/canaveral_cli/cue_parser.py
+-rw-r--r--   0        0        0     3523 2023-05-22 18:08:16.403481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/component/cron-task.json
+-rw-r--r--   0        0        0     2183 2023-05-22 18:08:16.693481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/component/daemon.json
+-rw-r--r--   0        0        0      202 2023-05-22 18:08:16.943481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/component/k8s-objects.json
+-rw-r--r--   0        0        0     2025 2023-05-22 18:08:17.493481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/component/task.json
+-rw-r--r--   0        0        0     2370 2023-05-22 18:08:17.763481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/component/webservice.json
+-rw-r--r--   0        0        0      471 2023-05-22 18:08:25.673481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/policy/apply-once.json
+-rw-r--r--   0        0        0     1026 2023-05-22 18:08:25.963481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/policy/garbage-collect.json
+-rw-r--r--   0        0        0      487 2023-05-22 18:08:26.193481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/policy/override.json
+-rw-r--r--   0        0        0      312 2023-05-22 18:08:26.433481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/policy/read-only.json
+-rw-r--r--   0        0        0      488 2023-05-22 18:08:26.683481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/policy/replication.json
+-rw-r--r--   0        0        0      293 2023-05-22 18:08:26.933481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/policy/resource-update.json
+-rw-r--r--   0        0        0      313 2023-05-22 18:08:27.193481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/policy/shared-resource.json
+-rw-r--r--   0        0        0      310 2023-05-22 18:08:27.473481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/policy/take-over.json
+-rw-r--r--   0        0        0      553 2023-05-22 18:08:27.723481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/policy/topology.json
+-rw-r--r--   0        0        0      221 2023-05-22 18:08:18.793481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/annotations.json
+-rw-r--r--   0        0        0      213 2023-05-22 18:08:19.063481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/command.json
+-rw-r--r--   0        0        0      160 2023-05-22 18:08:19.323481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/container-image.json
+-rw-r--r--   0        0        0      830 2023-05-22 18:08:19.583481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/cpuscaler.json
+-rw-r--r--   0        0        0      205 2023-05-22 18:08:19.843481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/env.json
+-rw-r--r--   0        0        0      680 2023-05-22 18:08:20.133481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/expose.json
+-rw-r--r--   0        0        0     1380 2023-05-22 18:08:20.393481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/gateway.json
+-rw-r--r--   0        0        0      274 2023-05-22 18:08:20.673481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/hostalias.json
+-rw-r--r--   0        0        0      941 2023-05-22 18:08:20.933481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/hpa.json
+-rw-r--r--   0        0        0     1329 2023-05-22 18:08:21.213481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/init-container.json
+-rw-r--r--   0        0        0      510 2023-05-22 18:08:21.993481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/k8s-update-strategy.json
+-rw-r--r--   0        0        0      205 2023-05-22 18:08:22.253481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/labels.json
+-rw-r--r--   0        0        0      333 2023-05-22 18:08:22.513481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/lifecycle.json
+-rw-r--r--   0        0        0      405 2023-05-22 18:08:23.103481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/pure-ingress.json
+-rw-r--r--   0        0        0      702 2023-05-22 18:08:23.373481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/resource.json
+-rw-r--r--   0        0        0      266 2023-05-22 18:08:23.623481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/scaler.json
+-rw-r--r--   0        0        0      595 2023-05-22 18:08:23.883481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/service-account.json
+-rw-r--r--   0        0        0     1121 2023-05-22 18:08:24.383481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/sidecar.json
+-rw-r--r--   0        0        0      267 2023-05-22 18:08:24.643481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/startup-probe.json
+-rw-r--r--   0        0        0      660 2023-05-22 18:08:24.903481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/storage.json
+-rw-r--r--   0        0        0      288 2023-05-22 18:08:25.173481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/trait/topologyspreadconstraints.json
+-rw-r--r--   0        0        0      363 2023-05-22 18:08:28.253481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/apply-component.json
+-rw-r--r--   0        0        0      374 2023-05-22 18:08:28.513481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/apply-deployment.json
+-rw-r--r--   0        0        0      429 2023-05-22 18:08:28.783481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/apply-object.json
+-rw-r--r--   0        0        0     1251 2023-05-22 18:08:29.073481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/apply-terraform-config.json
+-rw-r--r--   0        0        0      287 2023-05-22 18:08:29.333481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/apply-terraform-provider.json
+-rw-r--r--   0        0        0     1288 2023-05-22 18:08:29.663481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/build-push-image.json
+-rw-r--r--   0        0        0      939 2023-05-22 18:08:29.943481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/check-metrics.json
+-rw-r--r--   0        0        0      277 2023-05-22 18:08:30.223481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/clean-jobs.json
+-rw-r--r--   0        0        0      908 2023-05-22 18:08:30.503481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/collect-service-endpoints.json
+-rw-r--r--   0        0        0      530 2023-05-22 18:08:30.763481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/create-config.json
+-rw-r--r--   0        0        0      309 2023-05-22 18:08:31.033481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/delete-config.json
+-rw-r--r--   0        0        0      369 2023-05-22 18:08:31.303481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/depends-on-app.json
+-rw-r--r--   0        0        0      429 2023-05-22 18:08:31.563481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/deploy-cloud-resource.json
+-rw-r--r--   0        0        0      836 2023-05-22 18:08:31.823481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/deploy.json
+-rw-r--r--   0        0        0      685 2023-05-22 18:08:32.093481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/export-data.json
+-rw-r--r--   0        0        0      766 2023-05-22 18:08:32.343481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/export-service.json
+-rw-r--r--   0        0        0      579 2023-05-22 18:08:32.603481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/export2config.json
+-rw-r--r--   0        0        0      872 2023-05-22 18:08:32.883481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/export2secret.json
+-rw-r--r--   0        0        0      427 2023-05-22 18:08:33.133481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/generate-jdbc-connection.json
+-rw-r--r--   0        0        0      316 2023-05-22 18:08:33.393481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/list-config.json
+-rw-r--r--   0        0        0      699 2023-05-22 18:08:33.643481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/notification.json
+-rw-r--r--   0        0        0      190 2023-05-22 18:08:33.893481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/print-message-in-status.json
+-rw-r--r--   0        0        0      305 2023-05-22 18:08:34.143481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/read-config.json
+-rw-r--r--   0        0        0      817 2023-05-22 18:08:34.423481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/read-object.json
+-rw-r--r--   0        0        0      374 2023-05-22 18:08:34.673481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/request.json
+-rw-r--r--   0        0        0      596 2023-05-22 18:08:34.933481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/share-cloud-resource.json
+-rw-r--r--   0        0        0      281 2023-05-22 18:08:35.183481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/step-group.json
+-rw-r--r--   0        0        0      421 2023-05-22 18:08:35.453481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/suspend.json
+-rw-r--r--   0        0        0      627 2023-05-22 18:08:35.713481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/vela-cli.json
+-rw-r--r--   0        0        0      407 2023-05-22 18:08:35.983481 canaveral_cli-0.1.3/canaveral_cli/data/oam_types/workflowstep/webhook.json
+-rw-r--r--   0        0        0     9149 2023-05-21 14:12:29.078901 canaveral_cli-0.1.3/canaveral_cli/data/raw_data.yaml
+-rw-r--r--   0        0        0     1091 2023-05-14 19:06:08.091164 canaveral_cli-0.1.3/canaveral_cli/data/templates/vela_default.yaml
+-rw-r--r--   0        0        0     1364 2023-05-21 11:24:22.059044 canaveral_cli-0.1.3/canaveral_cli/data/templates/vela_template.yaml.jinja
+-rw-r--r--   0        0        0     2523 2023-05-22 18:02:51.603482 canaveral_cli-0.1.3/canaveral_cli/definitions.py
+-rw-r--r--   0        0        0     1116 2023-05-22 18:03:08.973482 canaveral_cli-0.1.3/canaveral_cli/merge_oam.py
+-rw-r--r--   0        0        0      777 2023-05-22 18:10:05.503473 canaveral_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2340 2023-05-22 18:10:25.157972 canaveral_cli-0.1.3/setup.py
+-rw-r--r--   0        0        0     1843 2023-05-22 18:10:25.158627 canaveral_cli-0.1.3/PKG-INFO
```

### Comparing `canaveral_cli-0.1.2/LICENSE` & `canaveral_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.2/README.md` & `canaveral_cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.2/canaveral_cli/__init__.py` & `canaveral_cli-0.1.3/canaveral_cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Top-level package for Canaveral"""
 # canaveral_cli/__init__.py
 
 from dotenv import load_dotenv
+from pathlib import Path
 
 load_dotenv()
 
 __app_name__ = "canaveral"
 __version__ = "0.1.0"
+PACKAGEDIR = Path(__file__).parent.absolute()
 
 
 # COMPONENT_TYPES = ["webservice", "task", "cron-task", "daemon", "k8s-objects"]
 # TRAIT_TYPES = ["affinity", "annotations", "command", "container-image", "cpuscaler", "env", "expose", "gateway", "hostalias", "hpa", "init-container", "json-merge-patch", "json-patch",
 #                "k8s-update-strategy", "labels", "lifecycle", "nocalhost", "resource", "scaler", "service-account", "service-binding", "sidecar", "startup-probe", "storage", "topologyspreadconstraints"]
 # POLICY_TYPES = ["apply-once", "garbage-collect", "health", "override",
 #                 "read-only", "replication", "shared-resource", "take-over", "topology"]
```

### Comparing `canaveral_cli-0.1.2/canaveral_cli/cli.py` & `canaveral_cli-0.1.3/canaveral_cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # canaveral_cli/cli.py
 
 from typing import Optional
 from pathlib import Path
 import typer
 import shutil
 import yaml
-from canaveral_cli import __app_name__, __version__
+from canaveral_cli import PACKAGEDIR, __app_name__, __version__
 from canaveral_cli.definitions import get_updated_type_data
 from canaveral_cli.merge_oam import merge_oam
 from canaveral_cli.create_oam import oam_form, create_oam_file
 from rich import print
 
 app = typer.Typer()
 
@@ -26,28 +26,28 @@
     get_updated_type_data()
 
 
 @app.command()
 def create():
     """Interactively Create a OAM file"""
     oam_form_data = oam_form()
-    with open("raw_data.yaml", "w") as f:
+    with open(PACKAGEDIR/"data/raw_data.yaml", "w") as f:
         yaml.dump(oam_form_data, f)
         f.close()
 
     # return
 
-    oam_form_data = yaml.load(open("raw_data.yaml"), Loader=yaml.FullLoader)
+    oam_form_data = yaml.load(open(PACKAGEDIR/"data/raw_data.yaml"), Loader=yaml.FullLoader)
     create_oam_file(oam_form_data)
 
 
 @app.command()
 def default():
     """Create the default OAM file"""
-    shutil.copyfile("canaveral_cli/templates/vela_default.yaml", "vela.yaml")
+    shutil.copyfile(PACKAGEDIR/"data/templates/vela_default.yaml", "vela.yaml")
     print("Vela.yaml created.")
     
 
 @app.command()
 def merge(dev: Path = typer.Argument(..., exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True),
           ops: Path = typer.Argument(..., exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True)):
     """Merge Dev OAM file with Operations OAM file"""
```

### Comparing `canaveral_cli-0.1.2/canaveral_cli/create_oam.py` & `canaveral_cli-0.1.3/canaveral_cli/create_oam.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 import jinja2
 import typer
 from rich import print
 from InquirerPy import inquirer
 from InquirerPy.base.control import Choice
 from InquirerPy.validator import EmptyInputValidator
 
-from canaveral_cli import COMPONENT_TYPES, TRAIT_TYPES, POLICY_TYPES, WORKFLOWSTEP_TYPES
+from canaveral_cli import COMPONENT_TYPES, PACKAGEDIR, TRAIT_TYPES, POLICY_TYPES, WORKFLOWSTEP_TYPES
 
 used_component_names = []
 used_workflowstep_names = []
 
 def get_type_data():
     for pair in [("component", COMPONENT_TYPES), ("trait", TRAIT_TYPES), ("policy", POLICY_TYPES), ("workflowstep", WORKFLOWSTEP_TYPES)]:
-        for type_file in os.scandir(f"canaveral_cli/oam_types/{pair[0]}"):
+        for type_file in os.scandir(PACKAGEDIR/f"data/oam_types/{pair[0]}"):
             with open(type_file.path, "r") as f:
                 pair[1].append(json.load(f))
                 f.close()
 
     # move component with name webservice to first in list COMPONENT_TYPES
     for idx, component in enumerate(COMPONENT_TYPES):
         if component["name"] == "webservice":
             COMPONENT_TYPES.insert(0, COMPONENT_TYPES.pop(idx))
             break
 
 
 def create_oam_file(oam_file_data: dict):
     environment = jinja2.Environment(
-        loader=jinja2.FileSystemLoader('canaveral_cli/templates/'), trim_blocks=True, lstrip_blocks=True)
+        loader=jinja2.FileSystemLoader(PACKAGEDIR/"data/templates/"), trim_blocks=True, lstrip_blocks=True)
     template = environment.get_template('vela_template.yaml.jinja')
     with open("vela.yaml", "w") as f:
         f.write(template.render(oam_file_data))
         f.close()
     print("\nThe created file is most likely [bold red]incomplete[/bold red].",
          "Please check it and fill the missing fields by consulting the [link=https://kubevela.io/docs/end-user/components/references]docs[/]", sep=os.linesep)
     typer.confirm(text="Confirm [Enter]", default=True, show_default=False)
```

### Comparing `canaveral_cli-0.1.2/canaveral_cli/cue_parser.py` & `canaveral_cli-0.1.3/canaveral_cli/cue_parser.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.2/canaveral_cli/definitions.py` & `canaveral_cli-0.1.3/canaveral_cli/definitions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """This module provides funtions to update internal definitions"""
 # canaveral_cli/definitions.py
 
 import json
 import os
 from github import Github
+from canaveral_cli import PACKAGEDIR
 
 from canaveral_cli.cue_parser import parse_cue_hc
 
 
 def clean_cue_file(cue) -> str:
     #* File can have too many tokens
     #* cut off #HealthProbe (and add closing bracket removed by cutting off #HealthProbe)
@@ -40,21 +41,21 @@
                 #     continue
                 cue_file = definition.decoded_content.decode("utf-8")
                 
                 # If file has "ui-hidden": "true" in the labels, skip it
                 if cue_file.find('"ui-hidden": "true"') != -1:
                     print(f"Skipping {element} definition: {definition.name}")
                     # If local file exists, delete it
-                    if os.path.exists(f"canaveral_cli/oam_types/{element}/{definition.name[:-4]}.json"):
-                        os.remove(f"canaveral_cli/oam_types/{element}/{definition.name[:-4]}.json")
+                    if os.path.exists(PACKAGEDIR/f"data/oam_types/{element}/{definition.name[:-4]}.json"):
+                        os.remove(PACKAGEDIR/f"data/oam_types/{element}/{definition.name[:-4]}.json")
                     continue
                 
                 # cue_file = clean_cue_file(cue_file)
                 print(f'Parsing {element} definition: {definition.name}')
                 parsed_dict = parse_cue_hc(cue_file)
                 type_name = parsed_dict["name"]
-                with open(f"canaveral_cli/oam_types/{element}/{type_name}.json", "w") as f:
+                with open(PACKAGEDIR/f"data/oam_types/{element}/{type_name}.json", "w") as f:
                     f.write(json.dumps(parsed_dict))
                     f.close()
         else:
             raise Exception("No component definitions found in the Kubevela repository")
```

### Comparing `canaveral_cli-0.1.2/canaveral_cli/merge_oam.py` & `canaveral_cli-0.1.3/canaveral_cli/merge_oam.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """This module provides the merge_oam function"""
 # canaveral_cli/merge_oam.py
 
-import yaml
-
 def merge_oam(dev: dict, ops: dict):
     print(f"dev: {dev['spec']}\n\nops: {ops['spec']}")
     merged_yaml = {}
     # Keep header and components from dev
     merged_yaml["apiVersion"] = dev["apiVersion"]
     merged_yaml["kind"] = dev["kind"]
     merged_yaml["metadata"] = dev["metadata"]
```

### Comparing `canaveral_cli-0.1.2/canaveral_cli/templates/vela_default.yaml` & `canaveral_cli-0.1.3/canaveral_cli/data/templates/vela_default.yaml`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.2/canaveral_cli/templates/vela_template.yaml.jinja` & `canaveral_cli-0.1.3/canaveral_cli/data/templates/vela_template.yaml.jinja`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.2/pyproject.toml` & `canaveral_cli-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canaveral_cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "Helper CLI to interact with Devscope's internal platform codename Canaveral"
 authors = ["André Gomes <andre.gomes@devscope.net>", "Hugo Sousa <hugo.sousa@devscope.net>", "Vitor Correia <vitor.correia@devscope.net>"]
 readme = "README.md"
 repository = "https://github.com/DevScope/canaveral-cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `canaveral_cli-0.1.2/setup.py` & `canaveral_cli-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from setuptools import setup
 
 packages = \
 ['canaveral_cli']
 
 package_data = \
 {'': ['*'],
- 'canaveral_cli': ['oam_types/component/*',
-                   'oam_types/policy/*',
-                   'oam_types/trait/*',
-                   'oam_types/workflowstep/*',
-                   'templates/*']}
+ 'canaveral_cli': ['data/*',
+                   'data/oam_types/component/*',
+                   'data/oam_types/policy/*',
+                   'data/oam_types/trait/*',
+                   'data/oam_types/workflowstep/*',
+                   'data/templates/*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
  'PyGithub>=1.58.2,<2.0.0',
  'PyYAML>=6.0,<7.0',
  'inquirerpy>=0.3.4,<0.4.0',
  'python-dotenv>=1.0.0,<2.0.0',
@@ -22,15 +23,15 @@
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['canaveral = canaveral_cli.cli:app']}
 
 setup_kwargs = {
     'name': 'canaveral-cli',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': "Helper CLI to interact with Devscope's internal platform codename Canaveral",
     'long_description': '# Canaveral CLI\n\nThis Project uses [Typer](https://typer.tiangolo.com/) for the CLI functionality and [InquirerPy](https://inquirerpy.readthedocs.io/en/latest/index.html#) for the parameter selection\n\n## Run it\nWorking with virtual envs in Python:\n- https://realpython.com/python-virtual-environments-a-primer\n- https://aaronlelevier.github.io/virtualenv-cheatsheet/\n\n```bash\n$ python3 -m venv venv --prompt="canaveral-env"\n$ source venv/bin/activate\n(canaveral-env) $ \n(canaveral-env) $ deactivate\n$ \n$ pip install -r requirements.txt\n$ OR\n$ python -m pip install -r requirements.txt\n```\n\n## How to contribuite\nProject layout to adhere to:\n- https://realpython.com/python-application-layouts/#command-line-application-layouts\n\n## Internal Notes\n\nDevscope Internal notes and documentation avaible at [Canaveral](https://devscope365.sharepoint.com/sites/academy/_layouts/OneNote.aspx?id=%2Fsites%2Facademy%2FSiteAssets%2FAcademy%20Notebook&wd=target%282023.one%7C1069493A-33E1-4F4C-8D77-28AA9AE54494%2FCanaveral%20CLI%7CF359B855-A8C4-4DB9-B416-CA0D700F2904%2F%29)\n',
     'author': 'André Gomes',
     'author_email': 'andre.gomes@devscope.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/DevScope/canaveral-cli',
```

### Comparing `canaveral_cli-0.1.2/PKG-INFO` & `canaveral_cli-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canaveral-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Helper CLI to interact with Devscope's internal platform codename Canaveral
 Home-page: https://github.com/DevScope/canaveral-cli
 Author: André Gomes
 Author-email: andre.gomes@devscope.net
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

