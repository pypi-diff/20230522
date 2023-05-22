# Comparing `tmp/canaveral_cli-0.1.1.tar.gz` & `tmp/canaveral_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canaveral_cli-0.1.1.tar", max compression
+gzip compressed data, was "canaveral_cli-0.1.2.tar", max compression
```

## Comparing `canaveral_cli-0.1.1.tar` & `canaveral_cli-0.1.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    11337 2023-04-20 10:01:17.537352 canaveral_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0     1063 2023-05-14 19:06:08.041164 canaveral_cli-0.1.1/README.md
--rw-r--r--   0        0        0     1479 2023-05-22 17:30:09.113480 canaveral_cli-0.1.1/canaveral_cli/__init__.py
--rw-r--r--   0        0        0      204 2023-05-22 17:30:04.733480 canaveral_cli-0.1.1/canaveral_cli/__main__.py
--rw-r--r--   0        0        0     2426 2023-05-22 17:30:01.613479 canaveral_cli-0.1.1/canaveral_cli/cli.py
--rw-r--r--   0        0        0    14128 2023-05-22 17:29:58.633479 canaveral_cli-0.1.1/canaveral_cli/create_oam.py
--rw-r--r--   0        0        0     6868 2023-05-22 17:29:51.893478 canaveral_cli-0.1.1/canaveral_cli/cue_parser.py
--rw-r--r--   0        0        0     2480 2023-05-22 17:29:46.123477 canaveral_cli-0.1.1/canaveral_cli/definitions.py
--rw-r--r--   0        0        0     1129 2023-05-22 17:29:42.993476 canaveral_cli-0.1.1/canaveral_cli/merge_oam.py
--rw-r--r--   0        0        0     5155 2023-05-21 14:53:02.338953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/cron-task.json
--rw-r--r--   0        0        0     3305 2023-05-21 14:53:02.948953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/daemon.json
--rw-r--r--   0        0        0      280 2023-05-21 14:53:03.458953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/k8s-objects.json
--rw-r--r--   0        0        0     2997 2023-05-21 14:53:04.038953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/task.json
--rw-r--r--   0        0        0     3558 2023-05-21 14:53:04.568953 canaveral_cli-0.1.1/canaveral_cli/oam_types/component/webservice.json
--rw-r--r--   0        0        0      627 2023-05-21 14:53:05.098953 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/apply-once.json
--rw-r--r--   0        0        0     1314 2023-05-21 14:53:05.748953 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/garbage-collect.json
--rw-r--r--   0        0        0      643 2023-05-21 14:53:06.368952 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/override.json
--rw-r--r--   0        0        0      402 2023-05-21 14:53:06.888952 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/read-only.json
--rw-r--r--   0        0        0      644 2023-05-21 14:53:07.418951 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/replication.json
--rw-r--r--   0        0        0      383 2023-05-21 14:53:07.918951 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/resource-update.json
--rw-r--r--   0        0        0      403 2023-05-21 14:53:08.498950 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/shared-resource.json
--rw-r--r--   0        0        0      400 2023-05-21 14:53:08.998949 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/take-over.json
--rw-r--r--   0        0        0      829 2023-05-21 14:53:09.548949 canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/topology.json
--rw-r--r--   0        0        0      287 2023-05-21 14:53:10.048948 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/annotations.json
--rw-r--r--   0        0        0      279 2023-05-21 14:53:10.728947 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/command.json
--rw-r--r--   0        0        0      226 2023-05-21 14:53:11.318947 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/container-image.json
--rw-r--r--   0        0        0     1184 2023-05-21 14:53:11.898946 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/cpuscaler.json
--rw-r--r--   0        0        0      271 2023-05-21 14:53:12.518945 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/env.json
--rw-r--r--   0        0        0      956 2023-05-21 14:53:13.238945 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/expose.json
--rw-r--r--   0        0        0     1932 2023-05-21 14:53:13.788945 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/gateway.json
--rw-r--r--   0        0        0      364 2023-05-21 14:53:14.308946 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/hostalias.json
--rw-r--r--   0        0        0     1427 2023-05-21 14:53:14.848947 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/hpa.json
--rw-r--r--   0        0        0     2013 2023-05-21 14:53:15.548948 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/init-container.json
--rw-r--r--   0        0        0      732 2023-05-21 14:53:16.148949 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/k8s-update-strategy.json
--rw-r--r--   0        0        0      271 2023-05-21 14:53:16.848950 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/labels.json
--rw-r--r--   0        0        0      465 2023-05-21 14:53:17.578951 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/lifecycle.json
--rw-r--r--   0        0        0      561 2023-05-21 14:53:18.148952 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/pure-ingress.json
--rw-r--r--   0        0        0      990 2023-05-21 14:53:18.648953 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/resource.json
--rw-r--r--   0        0        0      356 2023-05-21 14:53:19.188953 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/scaler.json
--rw-r--r--   0        0        0      817 2023-05-21 14:53:19.758954 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/service-account.json
--rw-r--r--   0        0        0     1673 2023-05-21 14:53:20.378955 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/sidecar.json
--rw-r--r--   0        0        0      333 2023-05-21 14:53:20.938955 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/startup-probe.json
--rw-r--r--   0        0        0     1014 2023-05-21 14:53:21.428955 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/storage.json
--rw-r--r--   0        0        0      366 2023-05-21 14:53:22.028957 canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/topologyspreadconstraints.json
--rw-r--r--   0        0        0      519 2023-05-21 14:53:22.558959 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-component.json
--rw-r--r--   0        0        0      614 2023-05-21 14:53:23.228961 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-deployment.json
--rw-r--r--   0        0        0      585 2023-05-21 14:53:23.808963 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-object.json
--rw-r--r--   0        0        0     1803 2023-05-21 14:53:24.488966 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-terraform-config.json
--rw-r--r--   0        0        0      353 2023-05-21 14:53:25.158968 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-terraform-provider.json
--rw-r--r--   0        0        0     1840 2023-05-21 14:53:25.798970 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/build-push-image.json
--rw-r--r--   0        0        0     1293 2023-05-21 14:53:26.458970 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/check-metrics.json
--rw-r--r--   0        0        0      409 2023-05-21 14:53:27.188970 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/clean-jobs.json
--rw-r--r--   0        0        0     1394 2023-05-21 14:53:27.828971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/collect-service-endpoints.json
--rw-r--r--   0        0        0      818 2023-05-21 14:53:28.448971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/create-config.json
--rw-r--r--   0        0        0      465 2023-05-21 14:53:29.078971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/delete-config.json
--rw-r--r--   0        0        0      525 2023-05-21 14:53:29.638971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/depends-on-app.json
--rw-r--r--   0        0        0      585 2023-05-21 14:53:30.228971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/deploy-cloud-resource.json
--rw-r--r--   0        0        0     1124 2023-05-21 14:53:30.838971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/deploy.json
--rw-r--r--   0        0        0     1039 2023-05-21 14:53:31.548971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export-data.json
--rw-r--r--   0        0        0     1186 2023-05-21 14:53:32.118971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export-service.json
--rw-r--r--   0        0        0      867 2023-05-21 14:53:32.738971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export2config.json
--rw-r--r--   0        0        0     1358 2023-05-21 14:53:33.328971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export2secret.json
--rw-r--r--   0        0        0      583 2023-05-21 14:53:33.968971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/generate-jdbc-connection.json
--rw-r--r--   0        0        0      472 2023-05-21 14:53:34.478971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/list-config.json
--rw-r--r--   0        0        0      987 2023-05-21 14:53:34.988971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/notification.json
--rw-r--r--   0        0        0      268 2023-05-21 14:53:35.558971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/print-message-in-status.json
--rw-r--r--   0        0        0      461 2023-05-21 14:53:36.248971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/read-config.json
--rw-r--r--   0        0        0     1171 2023-05-21 14:53:36.858971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/read-object.json
--rw-r--r--   0        0        0      614 2023-05-21 14:53:37.488971 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/request.json
--rw-r--r--   0        0        0      818 2023-05-21 14:53:38.018968 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/share-cloud-resource.json
--rw-r--r--   0        0        0      295 2023-05-21 14:53:38.608965 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/step-group.json
--rw-r--r--   0        0        0      577 2023-05-21 14:53:39.138962 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/suspend.json
--rw-r--r--   0        0        0      981 2023-05-21 14:53:39.708958 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/vela-cli.json
--rw-r--r--   0        0        0      563 2023-05-21 14:53:40.288956 canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/webhook.json
--rw-r--r--   0        0        0     1091 2023-05-14 19:06:08.091164 canaveral_cli-0.1.1/canaveral_cli/templates/vela_default.yaml
--rw-r--r--   0        0        0     1364 2023-05-21 11:24:22.059044 canaveral_cli-0.1.1/canaveral_cli/templates/vela_template.yaml.jinja
--rw-r--r--   0        0        0      773 2023-05-22 17:31:31.853483 canaveral_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2282 2023-05-22 17:31:34.762287 canaveral_cli-0.1.1/setup.py
--rw-r--r--   0        0        0     1843 2023-05-22 17:31:34.762581 canaveral_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-20 10:01:17.537352 canaveral_cli-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1063 2023-05-14 19:06:08.041164 canaveral_cli-0.1.2/README.md
+-rw-r--r--   0        0        0     1479 2023-05-22 17:30:09.113480 canaveral_cli-0.1.2/canaveral_cli/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-22 17:30:04.733480 canaveral_cli-0.1.2/canaveral_cli/__main__.py
+-rw-r--r--   0        0        0     2425 2023-05-22 17:34:59.783480 canaveral_cli-0.1.2/canaveral_cli/cli.py
+-rw-r--r--   0        0        0    14128 2023-05-22 17:29:58.633479 canaveral_cli-0.1.2/canaveral_cli/create_oam.py
+-rw-r--r--   0        0        0     6868 2023-05-22 17:29:51.893478 canaveral_cli-0.1.2/canaveral_cli/cue_parser.py
+-rw-r--r--   0        0        0     2480 2023-05-22 17:29:46.123477 canaveral_cli-0.1.2/canaveral_cli/definitions.py
+-rw-r--r--   0        0        0     1129 2023-05-22 17:29:42.993476 canaveral_cli-0.1.2/canaveral_cli/merge_oam.py
+-rw-r--r--   0        0        0     5155 2023-05-21 14:53:02.338953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/cron-task.json
+-rw-r--r--   0        0        0     3305 2023-05-21 14:53:02.948953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/daemon.json
+-rw-r--r--   0        0        0      280 2023-05-21 14:53:03.458953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/k8s-objects.json
+-rw-r--r--   0        0        0     2997 2023-05-21 14:53:04.038953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/task.json
+-rw-r--r--   0        0        0     3558 2023-05-21 14:53:04.568953 canaveral_cli-0.1.2/canaveral_cli/oam_types/component/webservice.json
+-rw-r--r--   0        0        0      627 2023-05-21 14:53:05.098953 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/apply-once.json
+-rw-r--r--   0        0        0     1314 2023-05-21 14:53:05.748953 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/garbage-collect.json
+-rw-r--r--   0        0        0      643 2023-05-21 14:53:06.368952 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/override.json
+-rw-r--r--   0        0        0      402 2023-05-21 14:53:06.888952 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/read-only.json
+-rw-r--r--   0        0        0      644 2023-05-21 14:53:07.418951 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/replication.json
+-rw-r--r--   0        0        0      383 2023-05-21 14:53:07.918951 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/resource-update.json
+-rw-r--r--   0        0        0      403 2023-05-21 14:53:08.498950 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/shared-resource.json
+-rw-r--r--   0        0        0      400 2023-05-21 14:53:08.998949 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/take-over.json
+-rw-r--r--   0        0        0      829 2023-05-21 14:53:09.548949 canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/topology.json
+-rw-r--r--   0        0        0      287 2023-05-21 14:53:10.048948 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/annotations.json
+-rw-r--r--   0        0        0      279 2023-05-21 14:53:10.728947 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/command.json
+-rw-r--r--   0        0        0      226 2023-05-21 14:53:11.318947 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/container-image.json
+-rw-r--r--   0        0        0     1184 2023-05-21 14:53:11.898946 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/cpuscaler.json
+-rw-r--r--   0        0        0      271 2023-05-21 14:53:12.518945 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/env.json
+-rw-r--r--   0        0        0      956 2023-05-21 14:53:13.238945 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/expose.json
+-rw-r--r--   0        0        0     1932 2023-05-21 14:53:13.788945 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/gateway.json
+-rw-r--r--   0        0        0      364 2023-05-21 14:53:14.308946 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/hostalias.json
+-rw-r--r--   0        0        0     1427 2023-05-21 14:53:14.848947 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/hpa.json
+-rw-r--r--   0        0        0     2013 2023-05-21 14:53:15.548948 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/init-container.json
+-rw-r--r--   0        0        0      732 2023-05-21 14:53:16.148949 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/k8s-update-strategy.json
+-rw-r--r--   0        0        0      271 2023-05-21 14:53:16.848950 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/labels.json
+-rw-r--r--   0        0        0      465 2023-05-21 14:53:17.578951 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/lifecycle.json
+-rw-r--r--   0        0        0      561 2023-05-21 14:53:18.148952 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/pure-ingress.json
+-rw-r--r--   0        0        0      990 2023-05-21 14:53:18.648953 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/resource.json
+-rw-r--r--   0        0        0      356 2023-05-21 14:53:19.188953 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/scaler.json
+-rw-r--r--   0        0        0      817 2023-05-21 14:53:19.758954 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/service-account.json
+-rw-r--r--   0        0        0     1673 2023-05-21 14:53:20.378955 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/sidecar.json
+-rw-r--r--   0        0        0      333 2023-05-21 14:53:20.938955 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/startup-probe.json
+-rw-r--r--   0        0        0     1014 2023-05-21 14:53:21.428955 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/storage.json
+-rw-r--r--   0        0        0      366 2023-05-21 14:53:22.028957 canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/topologyspreadconstraints.json
+-rw-r--r--   0        0        0      519 2023-05-21 14:53:22.558959 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-component.json
+-rw-r--r--   0        0        0      614 2023-05-21 14:53:23.228961 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-deployment.json
+-rw-r--r--   0        0        0      585 2023-05-21 14:53:23.808963 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-object.json
+-rw-r--r--   0        0        0     1803 2023-05-21 14:53:24.488966 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-terraform-config.json
+-rw-r--r--   0        0        0      353 2023-05-21 14:53:25.158968 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-terraform-provider.json
+-rw-r--r--   0        0        0     1840 2023-05-21 14:53:25.798970 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/build-push-image.json
+-rw-r--r--   0        0        0     1293 2023-05-21 14:53:26.458970 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/check-metrics.json
+-rw-r--r--   0        0        0      409 2023-05-21 14:53:27.188970 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/clean-jobs.json
+-rw-r--r--   0        0        0     1394 2023-05-21 14:53:27.828971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/collect-service-endpoints.json
+-rw-r--r--   0        0        0      818 2023-05-21 14:53:28.448971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/create-config.json
+-rw-r--r--   0        0        0      465 2023-05-21 14:53:29.078971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/delete-config.json
+-rw-r--r--   0        0        0      525 2023-05-21 14:53:29.638971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/depends-on-app.json
+-rw-r--r--   0        0        0      585 2023-05-21 14:53:30.228971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/deploy-cloud-resource.json
+-rw-r--r--   0        0        0     1124 2023-05-21 14:53:30.838971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/deploy.json
+-rw-r--r--   0        0        0     1039 2023-05-21 14:53:31.548971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export-data.json
+-rw-r--r--   0        0        0     1186 2023-05-21 14:53:32.118971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export-service.json
+-rw-r--r--   0        0        0      867 2023-05-21 14:53:32.738971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export2config.json
+-rw-r--r--   0        0        0     1358 2023-05-21 14:53:33.328971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export2secret.json
+-rw-r--r--   0        0        0      583 2023-05-21 14:53:33.968971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/generate-jdbc-connection.json
+-rw-r--r--   0        0        0      472 2023-05-21 14:53:34.478971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/list-config.json
+-rw-r--r--   0        0        0      987 2023-05-21 14:53:34.988971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/notification.json
+-rw-r--r--   0        0        0      268 2023-05-21 14:53:35.558971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/print-message-in-status.json
+-rw-r--r--   0        0        0      461 2023-05-21 14:53:36.248971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/read-config.json
+-rw-r--r--   0        0        0     1171 2023-05-21 14:53:36.858971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/read-object.json
+-rw-r--r--   0        0        0      614 2023-05-21 14:53:37.488971 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/request.json
+-rw-r--r--   0        0        0      818 2023-05-21 14:53:38.018968 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/share-cloud-resource.json
+-rw-r--r--   0        0        0      295 2023-05-21 14:53:38.608965 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/step-group.json
+-rw-r--r--   0        0        0      577 2023-05-21 14:53:39.138962 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/suspend.json
+-rw-r--r--   0        0        0      981 2023-05-21 14:53:39.708958 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/vela-cli.json
+-rw-r--r--   0        0        0      563 2023-05-21 14:53:40.288956 canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/webhook.json
+-rw-r--r--   0        0        0     1091 2023-05-14 19:06:08.091164 canaveral_cli-0.1.2/canaveral_cli/templates/vela_default.yaml
+-rw-r--r--   0        0        0     1364 2023-05-21 11:24:22.059044 canaveral_cli-0.1.2/canaveral_cli/templates/vela_template.yaml.jinja
+-rw-r--r--   0        0        0      777 2023-05-22 17:40:36.483485 canaveral_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2286 2023-05-22 17:40:57.763514 canaveral_cli-0.1.2/setup.py
+-rw-r--r--   0        0        0     1843 2023-05-22 17:40:57.763817 canaveral_cli-0.1.2/PKG-INFO
```

### Comparing `canaveral_cli-0.1.1/LICENSE` & `canaveral_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/README.md` & `canaveral_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/__init__.py` & `canaveral_cli-0.1.2/canaveral_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/cli.py` & `canaveral_cli-0.1.2/canaveral_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import yaml
 from canaveral_cli import __app_name__, __version__
 from canaveral_cli.definitions import get_updated_type_data
 from canaveral_cli.merge_oam import merge_oam
 from canaveral_cli.create_oam import oam_form, create_oam_file
 from rich import print
 
-
 app = typer.Typer()
 
 def _version_callback(value: bool):
     if value:
         typer.echo(f"{__app_name__} v{__version__}")
         raise typer.Exit()
```

### Comparing `canaveral_cli-0.1.1/canaveral_cli/create_oam.py` & `canaveral_cli-0.1.2/canaveral_cli/create_oam.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/cue_parser.py` & `canaveral_cli-0.1.2/canaveral_cli/cue_parser.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/definitions.py` & `canaveral_cli-0.1.2/canaveral_cli/definitions.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/merge_oam.py` & `canaveral_cli-0.1.2/canaveral_cli/merge_oam.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/component/cron-task.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/component/cron-task.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/component/daemon.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/component/daemon.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/component/task.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/component/task.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/component/webservice.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/component/webservice.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/apply-once.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/apply-once.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/garbage-collect.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/garbage-collect.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/override.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/override.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/replication.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/replication.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/policy/topology.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/policy/topology.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/cpuscaler.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/cpuscaler.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/expose.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/expose.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/gateway.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/gateway.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/hpa.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/hpa.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/init-container.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/init-container.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/k8s-update-strategy.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/k8s-update-strategy.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/pure-ingress.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/pure-ingress.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/resource.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/resource.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/service-account.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/service-account.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/sidecar.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/sidecar.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/trait/storage.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/trait/storage.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-component.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-component.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-deployment.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-deployment.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-object.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-object.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/apply-terraform-config.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/apply-terraform-config.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/build-push-image.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/build-push-image.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/check-metrics.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/check-metrics.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/collect-service-endpoints.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/collect-service-endpoints.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/create-config.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/create-config.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/depends-on-app.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/depends-on-app.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/deploy-cloud-resource.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/deploy-cloud-resource.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/deploy.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/deploy.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export-data.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export-data.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export-service.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export-service.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export2config.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export2config.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/export2secret.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/export2secret.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/generate-jdbc-connection.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/generate-jdbc-connection.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/notification.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/notification.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/read-object.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/read-object.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/request.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/request.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/share-cloud-resource.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/share-cloud-resource.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/suspend.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/suspend.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/vela-cli.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/vela-cli.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/oam_types/workflowstep/webhook.json` & `canaveral_cli-0.1.2/canaveral_cli/oam_types/workflowstep/webhook.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/templates/vela_default.yaml` & `canaveral_cli-0.1.2/canaveral_cli/templates/vela_default.yaml`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/canaveral_cli/templates/vela_template.yaml.jinja` & `canaveral_cli-0.1.2/canaveral_cli/templates/vela_template.yaml.jinja`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.1/pyproject.toml` & `canaveral_cli-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canaveral_cli"
-version = "0.1.1"
+version = "0.1.2"
 description = "Helper CLI to interact with Devscope's internal platform codename Canaveral"
 authors = ["André Gomes <andre.gomes@devscope.net>", "Hugo Sousa <hugo.sousa@devscope.net>", "Vitor Correia <vitor.correia@devscope.net>"]
 readme = "README.md"
 repository = "https://github.com/DevScope/canaveral-cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -16,12 +16,12 @@
 PyYAML = "^6.0"
 PyGithub = "^1.58.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.scripts]
-canaveral = "canaveral.cli:app"
+canaveral = "canaveral_cli.cli:app"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `canaveral_cli-0.1.1/setup.py` & `canaveral_cli-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,19 @@
  'PyYAML>=6.0,<7.0',
  'inquirerpy>=0.3.4,<0.4.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'rich>=13.3.5,<14.0.0',
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
-{'console_scripts': ['canaveral = canaveral.cli:app']}
+{'console_scripts': ['canaveral = canaveral_cli.cli:app']}
 
 setup_kwargs = {
     'name': 'canaveral-cli',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': "Helper CLI to interact with Devscope's internal platform codename Canaveral",
     'long_description': '# Canaveral CLI\n\nThis Project uses [Typer](https://typer.tiangolo.com/) for the CLI functionality and [InquirerPy](https://inquirerpy.readthedocs.io/en/latest/index.html#) for the parameter selection\n\n## Run it\nWorking with virtual envs in Python:\n- https://realpython.com/python-virtual-environments-a-primer\n- https://aaronlelevier.github.io/virtualenv-cheatsheet/\n\n```bash\n$ python3 -m venv venv --prompt="canaveral-env"\n$ source venv/bin/activate\n(canaveral-env) $ \n(canaveral-env) $ deactivate\n$ \n$ pip install -r requirements.txt\n$ OR\n$ python -m pip install -r requirements.txt\n```\n\n## How to contribuite\nProject layout to adhere to:\n- https://realpython.com/python-application-layouts/#command-line-application-layouts\n\n## Internal Notes\n\nDevscope Internal notes and documentation avaible at [Canaveral](https://devscope365.sharepoint.com/sites/academy/_layouts/OneNote.aspx?id=%2Fsites%2Facademy%2FSiteAssets%2FAcademy%20Notebook&wd=target%282023.one%7C1069493A-33E1-4F4C-8D77-28AA9AE54494%2FCanaveral%20CLI%7CF359B855-A8C4-4DB9-B416-CA0D700F2904%2F%29)\n',
     'author': 'André Gomes',
     'author_email': 'andre.gomes@devscope.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/DevScope/canaveral-cli',
```

### Comparing `canaveral_cli-0.1.1/PKG-INFO` & `canaveral_cli-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canaveral-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Helper CLI to interact with Devscope's internal platform codename Canaveral
 Home-page: https://github.com/DevScope/canaveral-cli
 Author: André Gomes
 Author-email: andre.gomes@devscope.net
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

