# Comparing `tmp/canaveral_cli-0.1.0.tar.gz` & `tmp/canaveral_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canaveral_cli-0.1.0.tar", max compression
+gzip compressed data, was "canaveral_cli-0.1.1.tar", max compression
```

## Comparing `canaveral_cli-0.1.0.tar` & `canaveral_cli-0.1.1.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0    11337 2023-04-20 10:01:17.537352 canaveral_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     1475 2023-05-22 10:44:01.284311 canaveral_cli-0.1.0/canaveral_cli/__init__.py
--rw-r--r--   0        0        0      200 2023-05-22 17:18:39.523449 canaveral_cli-0.1.0/canaveral_cli/__main__.py
--rw-r--r--   0        0        0     2418 2023-05-22 17:18:39.523449 canaveral_cli-0.1.0/canaveral_cli/cli.py
--rw-r--r--   0        0        0    14116 2023-05-22 17:18:39.523449 canaveral_cli-0.1.0/canaveral_cli/create_oam.py
--rw-r--r--   0        0        0     6864 2023-05-22 10:45:18.284332 canaveral_cli-0.1.0/canaveral_cli/cue_parser.py
--rw-r--r--   0        0        0     2465 2023-05-22 17:18:39.523449 canaveral_cli-0.1.0/canaveral_cli/definitions.py
--rw-r--r--   0        0        0     1125 2023-05-22 10:45:54.334341 canaveral_cli-0.1.0/canaveral_cli/merge_oam.py
--rw-r--r--   0        0        0     5155 2023-05-21 14:53:02.338953 canaveral_cli-0.1.0/canaveral_cli/oam_types/component/cron-task.json
--rw-r--r--   0        0        0     3305 2023-05-21 14:53:02.948953 canaveral_cli-0.1.0/canaveral_cli/oam_types/component/daemon.json
--rw-r--r--   0        0        0      280 2023-05-21 14:53:03.458953 canaveral_cli-0.1.0/canaveral_cli/oam_types/component/k8s-objects.json
--rw-r--r--   0        0        0     2997 2023-05-21 14:53:04.038953 canaveral_cli-0.1.0/canaveral_cli/oam_types/component/task.json
--rw-r--r--   0        0        0     3558 2023-05-21 14:53:04.568953 canaveral_cli-0.1.0/canaveral_cli/oam_types/component/webservice.json
--rw-r--r--   0        0        0      627 2023-05-21 14:53:05.098953 canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/apply-once.json
--rw-r--r--   0        0        0     1314 2023-05-21 14:53:05.748953 canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/garbage-collect.json
--rw-r--r--   0        0        0      643 2023-05-21 14:53:06.368952 canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/override.json
--rw-r--r--   0        0        0      402 2023-05-21 14:53:06.888952 canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/read-only.json
--rw-r--r--   0        0        0      644 2023-05-21 14:53:07.418951 canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/replication.json
--rw-r--r--   0        0        0      383 2023-05-21 14:53:07.918951 canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/resource-update.json
--rw-r--r--   0        0        0      403 2023-05-21 14:53:08.498950 canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/shared-resource.json
--rw-r--r--   0        0        0      400 2023-05-21 14:53:08.998949 canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/take-over.json
--rw-r--r--   0        0        0      829 2023-05-21 14:53:09.548949 canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/topology.json
--rw-r--r--   0        0        0      287 2023-05-21 14:53:10.048948 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/annotations.json
--rw-r--r--   0        0        0      279 2023-05-21 14:53:10.728947 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/command.json
--rw-r--r--   0        0        0      226 2023-05-21 14:53:11.318947 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/container-image.json
--rw-r--r--   0        0        0     1184 2023-05-21 14:53:11.898946 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/cpuscaler.json
--rw-r--r--   0        0        0      271 2023-05-21 14:53:12.518945 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/env.json
--rw-r--r--   0        0        0      956 2023-05-21 14:53:13.238945 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/expose.json
--rw-r--r--   0        0        0     1932 2023-05-21 14:53:13.788945 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/gateway.json
--rw-r--r--   0        0        0      364 2023-05-21 14:53:14.308946 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/hostalias.json
--rw-r--r--   0        0        0     1427 2023-05-21 14:53:14.848947 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/hpa.json
--rw-r--r--   0        0        0     2013 2023-05-21 14:53:15.548948 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/init-container.json
--rw-r--r--   0        0        0      732 2023-05-21 14:53:16.148949 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/k8s-update-strategy.json
--rw-r--r--   0        0        0      271 2023-05-21 14:53:16.848950 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/labels.json
--rw-r--r--   0        0        0      465 2023-05-21 14:53:17.578951 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/lifecycle.json
--rw-r--r--   0        0        0      561 2023-05-21 14:53:18.148952 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/pure-ingress.json
--rw-r--r--   0        0        0      990 2023-05-21 14:53:18.648953 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/resource.json
--rw-r--r--   0        0        0      356 2023-05-21 14:53:19.188953 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/scaler.json
--rw-r--r--   0        0        0      817 2023-05-21 14:53:19.758954 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/service-account.json
--rw-r--r--   0        0        0     1673 2023-05-21 14:53:20.378955 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/sidecar.json
--rw-r--r--   0        0        0      333 2023-05-21 14:53:20.938955 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/startup-probe.json
--rw-r--r--   0        0        0     1014 2023-05-21 14:53:21.428955 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/storage.json
--rw-r--r--   0        0        0      366 2023-05-21 14:53:22.028957 canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/topologyspreadconstraints.json
--rw-r--r--   0        0        0      519 2023-05-21 14:53:22.558959 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/apply-component.json
--rw-r--r--   0        0        0      614 2023-05-21 14:53:23.228961 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/apply-deployment.json
--rw-r--r--   0        0        0      585 2023-05-21 14:53:23.808963 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/apply-object.json
--rw-r--r--   0        0        0     1803 2023-05-21 14:53:24.488966 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/apply-terraform-config.json
--rw-r--r--   0        0        0      353 2023-05-21 14:53:25.158968 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/apply-terraform-provider.json
--rw-r--r--   0        0        0     1840 2023-05-21 14:53:25.798970 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/build-push-image.json
--rw-r--r--   0        0        0     1293 2023-05-21 14:53:26.458970 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/check-metrics.json
--rw-r--r--   0        0        0      409 2023-05-21 14:53:27.188970 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/clean-jobs.json
--rw-r--r--   0        0        0     1394 2023-05-21 14:53:27.828971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/collect-service-endpoints.json
--rw-r--r--   0        0        0      818 2023-05-21 14:53:28.448971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/create-config.json
--rw-r--r--   0        0        0      465 2023-05-21 14:53:29.078971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/delete-config.json
--rw-r--r--   0        0        0      525 2023-05-21 14:53:29.638971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/depends-on-app.json
--rw-r--r--   0        0        0      585 2023-05-21 14:53:30.228971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/deploy-cloud-resource.json
--rw-r--r--   0        0        0     1124 2023-05-21 14:53:30.838971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/deploy.json
--rw-r--r--   0        0        0     1039 2023-05-21 14:53:31.548971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/export-data.json
--rw-r--r--   0        0        0     1186 2023-05-21 14:53:32.118971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/export-service.json
--rw-r--r--   0        0        0      867 2023-05-21 14:53:32.738971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/export2config.json
--rw-r--r--   0        0        0     1358 2023-05-21 14:53:33.328971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/export2secret.json
--rw-r--r--   0        0        0      583 2023-05-21 14:53:33.968971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/generate-jdbc-connection.json
--rw-r--r--   0        0        0      472 2023-05-21 14:53:34.478971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/list-config.json
--rw-r--r--   0        0        0      987 2023-05-21 14:53:34.988971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/notification.json
--rw-r--r--   0        0        0      268 2023-05-21 14:53:35.558971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/print-message-in-status.json
--rw-r--r--   0        0        0      461 2023-05-21 14:53:36.248971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/read-config.json
--rw-r--r--   0        0        0     1171 2023-05-21 14:53:36.858971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/read-object.json
--rw-r--r--   0        0        0      614 2023-05-21 14:53:37.488971 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/request.json
--rw-r--r--   0        0        0      818 2023-05-21 14:53:38.018968 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/share-cloud-resource.json
--rw-r--r--   0        0        0      295 2023-05-21 14:53:38.608965 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/step-group.json
--rw-r--r--   0        0        0      577 2023-05-21 14:53:39.138962 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/suspend.json
--rw-r--r--   0        0        0      981 2023-05-21 14:53:39.708958 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/vela-cli.json
--rw-r--r--   0        0        0      563 2023-05-21 14:53:40.288956 canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/webhook.json
--rw-r--r--   0        0        0     1091 2023-05-14 19:06:08.091164 canaveral_cli-0.1.0/canaveral_cli/templates/vela_default.yaml
--rw-r--r--   0        0        0     1364 2023-05-21 11:24:22.059044 canaveral_cli-0.1.0/canaveral_cli/templates/vela_template.yaml.jinja
--rw-r--r--   0        0        0      695 2023-05-22 17:18:32.973449 canaveral_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1155 2023-05-22 17:18:41.783812 canaveral_cli-0.1.0/setup.py
--rw-r--r--   0        0        0      618 2023-05-22 17:18:41.784406 canaveral_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-20 10:01:17.537352 canaveral_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1063 2023-05-14 19:06:08.041164 canaveral_cli-0.1.1/README.md
+-rw-r--r--   0        0        0     1479 2023-05-22 17:30:09.113480 canaveral_cli-0.1.1/canaveral_cli/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-22 17:30:04.733480 canaveral_cli-0.1.1/canaveral_cli/__main__.py
+-rw-r--r--   0        0        0     2426 2023-05-22 17:30:01.613479 canaveral_cli-0.1.1/canaveral_cli/cli.py
+-rw-r--r--   0        0        0    14128 2023-05-22 17:29:58.633479 canaveral_cli-0.1.1/canaveral_cli/create_oam.py
+-rw-r--r--   0        0        0     6868 2023-05-22 17:29:51.893478 canaveral_cli-0.1.1/canaveral_cli/cue_parser.py
+-rw-r--r--   0        0        0     2480 2023-05-22 17:29:46.123477 canaveral_cli-0.1.1/canaveral_cli/definitions.py
+-rw-r--r--   0        0        0     1129 2023-05-22 17:29:42.993476 canaveral_cli-0.1.1/canaveral_cli/merge_oam.py
+-rw-r--r--   0        0        0     5155 2023-05-21 14:53:02.338953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/cron-task.json
+-rw-r--r--   0        0        0     3305 2023-05-21 14:53:02.948953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/daemon.json
+-rw-r--r--   0        0        0      280 2023-05-21 14:53:03.458953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/k8s-objects.json
+-rw-r--r--   0        0        0     2997 2023-05-21 14:53:04.038953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/task.json
+-rw-r--r--   0        0        0     3558 2023-05-21 14:53:04.568953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/webservice.json
+-rw-r--r--   0        0        0      627 2023-05-21 14:53:05.098953 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/apply-once.json
+-rw-r--r--   0        0        0     1314 2023-05-21 14:53:05.748953 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/garbage-collect.json
+-rw-r--r--   0        0        0      643 2023-05-21 14:53:06.368952 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/override.json
+-rw-r--r--   0        0        0      402 2023-05-21 14:53:06.888952 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/read-only.json
+-rw-r--r--   0        0        0      644 2023-05-21 14:53:07.418951 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/replication.json
+-rw-r--r--   0        0        0      383 2023-05-21 14:53:07.918951 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/resource-update.json
+-rw-r--r--   0        0        0      403 2023-05-21 14:53:08.498950 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/shared-resource.json
+-rw-r--r--   0        0        0      400 2023-05-21 14:53:08.998949 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/take-over.json
+-rw-r--r--   0        0        0      829 2023-05-21 14:53:09.548949 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/topology.json
+-rw-r--r--   0        0        0      287 2023-05-21 14:53:10.048948 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/annotations.json
+-rw-r--r--   0        0        0      279 2023-05-21 14:53:10.728947 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/command.json
+-rw-r--r--   0        0        0      226 2023-05-21 14:53:11.318947 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/container-image.json
+-rw-r--r--   0        0        0     1184 2023-05-21 14:53:11.898946 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/cpuscaler.json
+-rw-r--r--   0        0        0      271 2023-05-21 14:53:12.518945 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/env.json
+-rw-r--r--   0        0        0      956 2023-05-21 14:53:13.238945 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/expose.json
+-rw-r--r--   0        0        0     1932 2023-05-21 14:53:13.788945 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/gateway.json
+-rw-r--r--   0        0        0      364 2023-05-21 14:53:14.308946 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/hostalias.json
+-rw-r--r--   0        0        0     1427 2023-05-21 14:53:14.848947 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/hpa.json
+-rw-r--r--   0        0        0     2013 2023-05-21 14:53:15.548948 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/init-container.json
+-rw-r--r--   0        0        0      732 2023-05-21 14:53:16.148949 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/k8s-update-strategy.json
+-rw-r--r--   0        0        0      271 2023-05-21 14:53:16.848950 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/labels.json
+-rw-r--r--   0        0        0      465 2023-05-21 14:53:17.578951 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/lifecycle.json
+-rw-r--r--   0        0        0      561 2023-05-21 14:53:18.148952 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/pure-ingress.json
+-rw-r--r--   0        0        0      990 2023-05-21 14:53:18.648953 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/resource.json
+-rw-r--r--   0        0        0      356 2023-05-21 14:53:19.188953 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/scaler.json
+-rw-r--r--   0        0        0      817 2023-05-21 14:53:19.758954 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/service-account.json
+-rw-r--r--   0        0        0     1673 2023-05-21 14:53:20.378955 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/sidecar.json
+-rw-r--r--   0        0        0      333 2023-05-21 14:53:20.938955 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/startup-probe.json
+-rw-r--r--   0        0        0     1014 2023-05-21 14:53:21.428955 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/storage.json
+-rw-r--r--   0        0        0      366 2023-05-21 14:53:22.028957 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/topologyspreadconstraints.json
+-rw-r--r--   0        0        0      519 2023-05-21 14:53:22.558959 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-component.json
+-rw-r--r--   0        0        0      614 2023-05-21 14:53:23.228961 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-deployment.json
+-rw-r--r--   0        0        0      585 2023-05-21 14:53:23.808963 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-object.json
+-rw-r--r--   0        0        0     1803 2023-05-21 14:53:24.488966 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-terraform-config.json
+-rw-r--r--   0        0        0      353 2023-05-21 14:53:25.158968 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-terraform-provider.json
+-rw-r--r--   0        0        0     1840 2023-05-21 14:53:25.798970 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/build-push-image.json
+-rw-r--r--   0        0        0     1293 2023-05-21 14:53:26.458970 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/check-metrics.json
+-rw-r--r--   0        0        0      409 2023-05-21 14:53:27.188970 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/clean-jobs.json
+-rw-r--r--   0        0        0     1394 2023-05-21 14:53:27.828971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/collect-service-endpoints.json
+-rw-r--r--   0        0        0      818 2023-05-21 14:53:28.448971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/create-config.json
+-rw-r--r--   0        0        0      465 2023-05-21 14:53:29.078971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/delete-config.json
+-rw-r--r--   0        0        0      525 2023-05-21 14:53:29.638971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/depends-on-app.json
+-rw-r--r--   0        0        0      585 2023-05-21 14:53:30.228971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/deploy-cloud-resource.json
+-rw-r--r--   0        0        0     1124 2023-05-21 14:53:30.838971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/deploy.json
+-rw-r--r--   0        0        0     1039 2023-05-21 14:53:31.548971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export-data.json
+-rw-r--r--   0        0        0     1186 2023-05-21 14:53:32.118971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export-service.json
+-rw-r--r--   0        0        0      867 2023-05-21 14:53:32.738971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export2config.json
+-rw-r--r--   0        0        0     1358 2023-05-21 14:53:33.328971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export2secret.json
+-rw-r--r--   0        0        0      583 2023-05-21 14:53:33.968971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/generate-jdbc-connection.json
+-rw-r--r--   0        0        0      472 2023-05-21 14:53:34.478971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/list-config.json
+-rw-r--r--   0        0        0      987 2023-05-21 14:53:34.988971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/notification.json
+-rw-r--r--   0        0        0      268 2023-05-21 14:53:35.558971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/print-message-in-status.json
+-rw-r--r--   0        0        0      461 2023-05-21 14:53:36.248971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/read-config.json
+-rw-r--r--   0        0        0     1171 2023-05-21 14:53:36.858971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/read-object.json
+-rw-r--r--   0        0        0      614 2023-05-21 14:53:37.488971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/request.json
+-rw-r--r--   0        0        0      818 2023-05-21 14:53:38.018968 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/share-cloud-resource.json
+-rw-r--r--   0        0        0      295 2023-05-21 14:53:38.608965 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/step-group.json
+-rw-r--r--   0        0        0      577 2023-05-21 14:53:39.138962 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/suspend.json
+-rw-r--r--   0        0        0      981 2023-05-21 14:53:39.708958 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/vela-cli.json
+-rw-r--r--   0        0        0      563 2023-05-21 14:53:40.288956 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/webhook.json
+-rw-r--r--   0        0        0     1091 2023-05-14 19:06:08.091164 canaveral_cli-0.1.1/canaveral_cli/templates/vela_default.yaml
+-rw-r--r--   0        0        0     1364 2023-05-21 11:24:22.059044 canaveral_cli-0.1.1/canaveral_cli/templates/vela_template.yaml.jinja
+-rw-r--r--   0        0        0      773 2023-05-22 17:31:31.853483 canaveral_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2282 2023-05-22 17:31:34.762287 canaveral_cli-0.1.1/setup.py
+-rw-r--r--   0        0        0     1843 2023-05-22 17:31:34.762581 canaveral_cli-0.1.1/PKG-INFO
```

### Comparing `canaveral_cli-0.1.0/LICENSE` & `canaveral_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/__init__.py` & `canaveral_cli-0.1.1/canaveral_cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Top-level package for Canaveral"""
-# canaveral/__init__.py
+# canaveral_cli/__init__.py
 
 from dotenv import load_dotenv
 
 load_dotenv()
 
 __app_name__ = "canaveral"
 __version__ = "0.1.0"
```

### Comparing `canaveral_cli-0.1.0/canaveral_cli/cli.py` & `canaveral_cli-0.1.1/canaveral_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module provides the Canaveral CLI"""
-# canaveral/cli.py
+# canaveral_cli/cli.py
 
 from typing import Optional
 from pathlib import Path
 import typer
 import shutil
 import yaml
 from canaveral_cli import __app_name__, __version__
@@ -40,15 +40,15 @@
     oam_form_data = yaml.load(open("raw_data.yaml"), Loader=yaml.FullLoader)
     create_oam_file(oam_form_data)
 
 
 @app.command()
 def default():
     """Create the default OAM file"""
-    shutil.copyfile("canaveral/templates/vela_default.yaml", "vela.yaml")
+    shutil.copyfile("canaveral_cli/templates/vela_default.yaml", "vela.yaml")
     print("Vela.yaml created.")
     
 
 @app.command()
 def merge(dev: Path = typer.Argument(..., exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True),
           ops: Path = typer.Argument(..., exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True)):
     """Merge Dev OAM file with Operations OAM file"""
```

### Comparing `canaveral_cli-0.1.0/canaveral_cli/create_oam.py` & `canaveral_cli-0.1.1/canaveral_cli/create_oam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module provides the functions to create OAM files"""
-# canaveral/create_oam.py
+# canaveral_cli/create_oam.py
 
 import json
 import os
 import jinja2
 import typer
 from rich import print
 from InquirerPy import inquirer
@@ -13,29 +13,29 @@
 from canaveral_cli import COMPONENT_TYPES, TRAIT_TYPES, POLICY_TYPES, WORKFLOWSTEP_TYPES
 
 used_component_names = []
 used_workflowstep_names = []
 
 def get_type_data():
     for pair in [("component", COMPONENT_TYPES), ("trait", TRAIT_TYPES), ("policy", POLICY_TYPES), ("workflowstep", WORKFLOWSTEP_TYPES)]:
-        for type_file in os.scandir(f"canaveral/oam_types/{pair[0]}"):
+        for type_file in os.scandir(f"canaveral_cli/oam_types/{pair[0]}"):
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
-        loader=jinja2.FileSystemLoader('canaveral/templates/'), trim_blocks=True, lstrip_blocks=True)
+        loader=jinja2.FileSystemLoader('canaveral_cli/templates/'), trim_blocks=True, lstrip_blocks=True)
     template = environment.get_template('vela_template.yaml.jinja')
     with open("vela.yaml", "w") as f:
         f.write(template.render(oam_file_data))
         f.close()
     print("\nThe created file is most likely [bold red]incomplete[/bold red].",
          "Please check it and fill the missing fields by consulting the [link=https://kubevela.io/docs/end-user/components/references]docs[/]", sep=os.linesep)
     typer.confirm(text="Confirm [Enter]", default=True, show_default=False)
```

### Comparing `canaveral_cli-0.1.0/canaveral_cli/cue_parser.py` & `canaveral_cli-0.1.1/canaveral_cli/cue_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module provides the Cue Parser"""
-# canaveral/cue_parser.py
+# canaveral_cli/cue_parser.py
 
 import re
 # from langchain.chat_models import ChatOpenAI
 # from langchain.prompts.chat import (
 #     ChatPromptTemplate,
 #     SystemMessagePromptTemplate,
 #     HumanMessagePromptTemplate,
```

### Comparing `canaveral_cli-0.1.0/canaveral_cli/definitions.py` & `canaveral_cli-0.1.1/canaveral_cli/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module provides funtions to update internal definitions"""
-# canaveral/definitions.py
+# canaveral_cli/definitions.py
 
 import json
 import os
-
 from github import Github
 
 from canaveral_cli.cue_parser import parse_cue_hc
 
 
 def clean_cue_file(cue) -> str:
     #* File can have too many tokens
@@ -41,21 +40,21 @@
                 #     continue
                 cue_file = definition.decoded_content.decode("utf-8")
                 
                 # If file has "ui-hidden": "true" in the labels, skip it
                 if cue_file.find('"ui-hidden": "true"') != -1:
                     print(f"Skipping {element} definition: {definition.name}")
                     # If local file exists, delete it
-                    if os.path.exists(f"canaveral/oam_types/{element}/{definition.name[:-4]}.json"):
-                        os.remove(f"canaveral/oam_types/{element}/{definition.name[:-4]}.json")
+                    if os.path.exists(f"canaveral_cli/oam_types/{element}/{definition.name[:-4]}.json"):
+                        os.remove(f"canaveral_cli/oam_types/{element}/{definition.name[:-4]}.json")
                     continue
                 
                 # cue_file = clean_cue_file(cue_file)
                 print(f'Parsing {element} definition: {definition.name}')
                 parsed_dict = parse_cue_hc(cue_file)
                 type_name = parsed_dict["name"]
-                with open(f"canaveral/oam_types/{element}/{type_name}.json", "w") as f:
+                with open(f"canaveral_cli/oam_types/{element}/{type_name}.json", "w") as f:
                     f.write(json.dumps(parsed_dict))
                     f.close()
         else:
             raise Exception("No component definitions found in the Kubevela repository")
```

### Comparing `canaveral_cli-0.1.0/canaveral_cli/merge_oam.py` & `canaveral_cli-0.1.1/canaveral_cli/merge_oam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module provides the merge_oam function"""
-# canaveral/merge_oam.py
+# canaveral_cli/merge_oam.py
 
 import yaml
 
 def merge_oam(dev: dict, ops: dict):
     print(f"dev: {dev['spec']}\n\nops: {ops['spec']}")
     merged_yaml = {}
     # Keep header and components from dev
```

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/component/cron-task.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/component/cron-task.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/component/daemon.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/component/daemon.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/component/task.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/component/task.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/component/webservice.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/component/webservice.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/apply-once.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/apply-once.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/garbage-collect.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/garbage-collect.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/override.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/override.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/replication.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/replication.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/policy/topology.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/topology.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/cpuscaler.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/cpuscaler.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/expose.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/expose.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/gateway.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/gateway.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/hpa.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/hpa.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/init-container.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/init-container.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/k8s-update-strategy.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/k8s-update-strategy.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/pure-ingress.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/pure-ingress.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/resource.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/resource.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/service-account.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/service-account.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/sidecar.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/sidecar.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/trait/storage.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/storage.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/apply-component.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-component.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/apply-deployment.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-deployment.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/apply-object.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-object.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/apply-terraform-config.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-terraform-config.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/build-push-image.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/build-push-image.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/check-metrics.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/check-metrics.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/collect-service-endpoints.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/collect-service-endpoints.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/create-config.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/create-config.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/depends-on-app.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/depends-on-app.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/deploy-cloud-resource.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/deploy-cloud-resource.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/deploy.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/deploy.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/export-data.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export-data.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/export-service.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export-service.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/export2config.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export2config.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/export2secret.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export2secret.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/generate-jdbc-connection.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/generate-jdbc-connection.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/notification.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/notification.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/read-object.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/read-object.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/request.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/request.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/share-cloud-resource.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/share-cloud-resource.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/suspend.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/suspend.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/vela-cli.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/vela-cli.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/oam_types/workflowstep/webhook.json` & `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/webhook.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/templates/vela_default.yaml` & `canaveral_cli-0.1.1/canaveral_cli/templates/vela_default.yaml`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/canaveral_cli/templates/vela_template.yaml.jinja` & `canaveral_cli-0.1.1/canaveral_cli/templates/vela_template.yaml.jinja`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.0/pyproject.toml` & `canaveral_cli-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "canaveral_cli"
-version = "0.1.0"
+version = "0.1.1"
 description = "Helper CLI to interact with Devscope's internal platform codename Canaveral"
 authors = ["André Gomes <andre.gomes@devscope.net>", "Hugo Sousa <hugo.sousa@devscope.net>", "Vitor Correia <vitor.correia@devscope.net>"]
+readme = "README.md"
+repository = "https://github.com/DevScope/canaveral-cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
 rich = "^13.3.5"
 Jinja2 = "^3.1.2"
 inquirerpy = "^0.3.4"
```

