# Comparing `tmp/propan-0.1.1.2.tar.gz` & `tmp/propan-0.1.1.3.tar.gz`

## Comparing `propan-0.1.1.2.tar` & `propan-0.1.1.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 propan-0.1.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.1.2/SECURITY.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.1.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.1.2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.1.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 propan-0.1.1.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.1.2/examples/redis/pattern.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/__about__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/__main__.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/py.typed
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/model/utils.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/log/logging.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/test/__init__.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/test/redis.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.1.2/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.1.2/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.1.2/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.1.2/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.1.2/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.1.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.1.2/LICENSE
--rw-r--r--   0        0        0    12146 2020-02-02 00:00:00.000000 propan-0.1.1.2/README.md
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 propan-0.1.1.2/pyproject.toml
--rw-r--r--   0        0        0    15595 2020-02-02 00:00:00.000000 propan-0.1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 propan-0.1.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.1.3/SECURITY.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.1.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.1.3/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.1.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 propan-0.1.1.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/redis/pattern.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/__about__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/__main__.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/py.typed
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/model/utils.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/log/logging.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/test/__init__.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/test/redis.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.1.3/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.1.3/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.1.3/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.1.3/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.1.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.1.3/LICENSE
+-rw-r--r--   0        0        0    12146 2020-02-02 00:00:00.000000 propan-0.1.1.3/README.md
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 propan-0.1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    15595 2020-02-02 00:00:00.000000 propan-0.1.1.3/PKG-INFO
```

### Comparing `propan-0.1.1.2/CONTRIBUTING.md` & `propan-0.1.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/SECURITY.md` & `propan-0.1.1.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/.github/workflows/documentation.yml` & `propan-0.1.1.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/.github/workflows/publish_coverage.yml` & `propan-0.1.1.3/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/.github/workflows/publish_pypi.yml` & `propan-0.1.1.3/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/.github/workflows/tests.yml` & `propan-0.1.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/3_lifespan_events.py` & `propan-0.1.1.3/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/4_cli_attributes_promotion.py` & `propan-0.1.1.3/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/5_publishing.py` & `propan-0.1.1.3/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/6_arguments_casting.py` & `propan-0.1.1.3/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/7_handler_errors_processing.py` & `propan-0.1.1.3/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/dependencies/1_dependency_injection.py` & `propan-0.1.1.3/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.1.3/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.1.3/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.1.3/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.1.3/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/dependencies/7_annotated.py` & `propan-0.1.1.3/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.1.3/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.1.3/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.1.3/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.1.3/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/http_frameworks_integrations/quart.py` & `propan-0.1.1.3/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.1.3/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.1.3/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/rabbit/direct.py` & `propan-0.1.1.3/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/rabbit/fanout.py` & `propan-0.1.1.3/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/rabbit/header.py` & `propan-0.1.1.3/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/rabbit/topic.py` & `propan-0.1.1.3/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/redis/direct.py` & `propan-0.1.1.3/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/examples/redis/pattern.py` & `propan-0.1.1.3/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/__init__.py` & `propan-0.1.1.3/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/annotations.py` & `propan-0.1.1.3/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/types.py` & `propan-0.1.1.3/propan/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Awaitable, Callable, Coroutine, Dict, Sequence, Union
+from typing import Any, Awaitable, Callable, Dict, Sequence, Union
 
 from pydantic import BaseModel
 from typing_extensions import TypeAlias
 
 AsyncFunc: TypeAlias = Callable[..., Awaitable[Any]]
 
 AnyDict: TypeAlias = Dict[str, Any]
@@ -14,11 +14,15 @@
 DecoratedAsync: TypeAlias = AsyncFunc
 
 Wrapper: TypeAlias = Callable[[AnyCallable], DecoratedCallable]
 AsyncWrapper: TypeAlias = Callable[[AnyCallable], DecoratedAsync]
 DecodedMessage: TypeAlias = Union[AnyDict, Sequence[Any], str, bytes]
 SendableMessage: TypeAlias = Union[DecodedMessage, BaseModel, None]
 
+HandlerCallable: TypeAlias = Callable[
+    ...,
+    Union[Awaitable[SendableMessage], SendableMessage],
+]
 HandlerWrapper: TypeAlias = Callable[
-    [Callable[..., Coroutine[Any, Any, SendableMessage]]],
-    Callable[..., SendableMessage],
+    [HandlerCallable],
+    HandlerCallable,
 ]
```

### Comparing `propan-0.1.1.2/propan/brokers/push_back_watcher.py` & `propan-0.1.1.3/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/brokers/model/broker_usecase.py` & `propan-0.1.1.3/propan/brokers/model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/brokers/model/schemas.py` & `propan-0.1.1.3/propan/brokers/model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/brokers/model/utils.py` & `propan-0.1.1.3/propan/brokers/model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/brokers/nats/nats_broker.py` & `propan-0.1.1.3/propan/brokers/nats/nats_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
     async def close(self) -> None:
         for h in self.handlers:
             await h.subscription.unsubscribe()
 
         if self._connection:
             await self._connection.drain()
+            self._connection = None
 
     def _get_log_context(
         self,
         message: Optional[PropanMessage],
         subject: str,
         queue: str = "",
     ) -> Dict[str, Any]:
```

### Comparing `propan-0.1.1.2/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.1.3/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.1.3/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/brokers/nats/schemas.py` & `propan-0.1.1.3/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.1.3/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import aiormq
 from aio_pika.abc import DeliveryMode
 
 from propan.brokers.model import BrokerUsecase
 from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
-from propan.types import AnyDict, DecoratedCallable, SendableMessage, Wrapper
+from propan.types import AnyDict, DecoratedCallable, HandlerWrapper, SendableMessage
 
 TimeoutType = Optional[Union[int, float]]
 PikaSendableMessage = Union[aio_pika.message.Message, SendableMessage]
 T = TypeVar("T")
 
 
 class RabbitBroker(BrokerUsecase):
@@ -50,15 +50,15 @@
             await self._connection.close()
             self._connection = None
 
     async def _connect(
         self,
         *args: Any,
         **kwargs: Any,
-    ) -> aio_pika.Connection:
+    ) -> aio_pika.RobustConnection:
         connection = await aio_pika.connect_robust(
             *args, **kwargs, loop=asyncio.get_event_loop()
         )
 
         if self._channel is None:  # pragma: no branch
             max_consumers = self._max_consumers
             self._channel = await connection.channel()
@@ -69,26 +69,27 @@
 
         return connection
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
-        **original_kwargs,
-    ) -> Wrapper:
+        *,
+        retry: Union[bool, int] = False,
+    ) -> HandlerWrapper:
         queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
         self.__setup_log_context(queue, exchange)
 
         def wrapper(func: DecoratedCallable) -> Any:
             func = self._wrap_handler(
                 func,
                 queue=queue,
                 exchange=exchange,
-                **original_kwargs,
+                retry=retry,
             )
             handler = Handler(callback=func, queue=queue, exchange=exchange)
             self.handlers.append(handler)
 
             return func
 
         return wrapper
@@ -301,22 +302,18 @@
 
     def __setup_log_context(
         self,
         queue: Optional[RabbitQueue] = None,
         exchange: Optional[RabbitExchange] = None,
     ) -> None:
         if exchange is not None:
-            i = len(exchange.name)
-            if i > self.__max_exchange_len:  # pragma: no branch
-                self.__max_exchange_len = i
+            self.__max_exchange_len = max(self.__max_exchange_len, len(exchange.name))
 
         if queue is not None:  # pragma: no branch
-            i = len(queue.name)
-            if i > self.__max_queue_len:  # pragma: no branch
-                self.__max_queue_len = i
+            self.__max_queue_len = max(self.__max_queue_len, len(queue.name))
 
 
 def _validate_exchange(
     exchange: Union[str, RabbitExchange, None] = None,
 ) -> Optional[RabbitExchange]:
     if exchange is not None:  # pragma: no branch
         if isinstance(exchange, str):
```

### Comparing `propan-0.1.1.2/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.1.3/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         """
         ...
     async def __aenter__(self) -> "RabbitBroker": ...
     async def _connect(
         self,
         *args: Any,
         **kwargs: Any,
-    ) -> aio_pika.Connection: ...
+    ) -> aio_pika.RobustConnection: ...
     async def close(self) -> None: ...
     def _process_message(
         self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
     ) -> Callable[[PropanMessage], T]: ...
     def _get_log_context(  # type: ignore[override]
         self,
         message: Optional[PropanMessage],
```

### Comparing `propan-0.1.1.2/propan/brokers/rabbit/schemas.py` & `propan-0.1.1.3/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/brokers/redis/redis_broker.py` & `propan-0.1.1.3/propan/brokers/redis/redis_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from propan.brokers.model.schemas import PropanMessage, RawDecoced
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.redis.schemas import Handler, RedisMessage
 from propan.types import (
     AnyCallable,
     DecodedMessage,
     DecoratedCallable,
+    HandlerWrapper,
     SendableMessage,
-    Wrapper,
 )
 
 T = TypeVar("T")
 
 
 class RedisBroker(BrokerUsecase):
     handlers: List[Handler]
@@ -56,21 +56,24 @@
             kwargs["url"] = url
         return await super().connect(*args, **kwargs)
 
     async def close(self) -> None:
         for h in self.handlers:
             if h.task is not None:  # pragma: no branch
                 h.task.cancel()
+                h.task = None
 
             if h.subscription is not None:  # pragma: no branch
                 await h.subscription.unsubscribe()
                 await h.subscription.reset()
+                h.subscription = None
 
         if self._connection is not None:  # pragma: no branch
             await self._connection.close()
+            self._connection = None
 
     def _process_message(
         self,
         func: Callable[[PropanMessage], T],
         watcher: Optional[BaseWatcher],
     ) -> Callable[[PropanMessage], T]:
         @wraps(func)
@@ -86,15 +89,15 @@
         return wrapper
 
     def handle(
         self,
         channel: str = "",
         *,
         pattern: bool = False,
-    ) -> Wrapper:
+    ) -> HandlerWrapper:
         self.__max_channel_len = max(self.__max_channel_len, len(channel))
 
         def wrapper(func: AnyCallable) -> DecoratedCallable:
             func = self._wrap_handler(
                 func,
                 channel=channel,
             )
```

### Comparing `propan-0.1.1.2/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.1.3/propan/brokers/redis/redis_broker.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from redis.asyncio.connection import BaseParser, Connection, DefaultParser, Encoder
 
 from propan.brokers.model import BrokerUsecase
 from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.redis.schemas import Handler
 from propan.log import access_logger
-from propan.types import DecodedMessage, SendableMessage, Wrapper
+from propan.types import DecodedMessage, HandlerWrapper, SendableMessage
 
 T = TypeVar("T")
 
 class RedisBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Redis[bytes]
     __max_channel_len: int
@@ -82,15 +82,15 @@
         watcher: Optional[BaseWatcher],
     ) -> Callable[[PropanMessage], T]: ...
     def handle(  # type: ignore[override]
         self,
         channel: str,
         *,
         pattern: bool = False,
-    ) -> Wrapper: ...
+    ) -> HandlerWrapper: ...
     def _get_log_context(  # type: ignore[override]
         self, message: PropanMessage, channel: str
     ) -> Dict[str, Any]: ...
     @staticmethod
     async def _decode_message(message: PropanMessage) -> DecodedMessage: ...
     @property
     def fmt(self) -> str: ...
```

### Comparing `propan-0.1.1.2/propan/brokers/redis/schemas.py` & `propan-0.1.1.3/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/app.py` & `propan-0.1.1.3/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/main.py` & `propan-0.1.1.3/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/startproject/core.py` & `propan-0.1.1.3/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/startproject/async_app/app.py` & `propan-0.1.1.3/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/startproject/async_app/core.py` & `propan-0.1.1.3/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/startproject/async_app/nats.py` & `propan-0.1.1.3/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.1.3/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/startproject/async_app/redis.py` & `propan-0.1.1.3/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/supervisors/basereload.py` & `propan-0.1.1.3/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/supervisors/multiprocess.py` & `propan-0.1.1.3/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/supervisors/utils.py` & `propan-0.1.1.3/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/supervisors/watchfiles.py` & `propan-0.1.1.3/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/utils/imports.py` & `propan-0.1.1.3/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/utils/logs.py` & `propan-0.1.1.3/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/cli/utils/parser.py` & `propan-0.1.1.3/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/fastapi/core/route.py` & `propan-0.1.1.3/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/fastapi/core/router.py` & `propan-0.1.1.3/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/fastapi/rabbit/router.pyi` & `propan-0.1.1.3/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/fastapi/redis/router.pyi` & `propan-0.1.1.3/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/log/formatter.py` & `propan-0.1.1.3/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/log/logging.py` & `propan-0.1.1.3/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/test/rabbit.py` & `propan-0.1.1.3/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/test/redis.py` & `propan-0.1.1.3/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/test/utils.py` & `propan-0.1.1.3/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/utils/functions.py` & `propan-0.1.1.3/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/utils/context/main.py` & `propan-0.1.1.3/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/propan/utils/context/types.py` & `propan-0.1.1.3/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/LICENSE` & `propan-0.1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/README.md` & `propan-0.1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/pyproject.toml` & `propan-0.1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.2/PKG-INFO` & `propan-0.1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.1.2
+Version: 0.1.1.3
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.1.2 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.1.3 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
 framework,message brokers,rabbitmq Classifier: Development Status :: 5 -
```

