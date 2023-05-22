# Comparing `tmp/glow-0.12.3.tar.gz` & `tmp/glow-0.12.4.tar.gz`

## Comparing `glow-0.12.3.tar` & `glow-0.12.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.3/examples/__init__.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.3/examples/cifar10.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.3/examples/gan.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/__init__.py
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/cli.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/cli.pyi
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/distributed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/py.typed
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/api/__init__.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/api/config.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/api/exporting.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/__init__.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_coro.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_import_hook.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_more.py
--rw-r--r--   0        0        0    14592 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_parallel.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_parallel.pyi
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_patch_len.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_patch_print.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_patch_scipy.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_profile.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_profile.pyi
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_reduction.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_repr.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_sizeof.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_thread_quota.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_uuid.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/debug.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/__init__.py
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/cache.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/cache.pyi
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/concurrency.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/concurrency.pyi
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/reusable.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/util.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/io/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/io/_sound.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/io/_svg.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/metrics/__init__.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/metrics/base.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/metrics/confusion.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/metrics/raw.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/__init__.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/_loader.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/_sampler.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/_trainer.py
--rw-r--r--   0        0        0    13042 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/amp.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/driver.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/functional.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/optimizers.py
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/plot.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/proto.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/util.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/__init__.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/aggregates.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/context.py
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/convnets.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/lazy.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/simple.py
--rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/transformers.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/util.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/vision.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/__init__.py
--rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/classes.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/core.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/functional/__init__.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/functional/core.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/functional/numba.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.3/test/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.3/test/run_metrics.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_api.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_batch.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_buffered.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_cli.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_iter.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_loader.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_shm.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_thread_pool.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_timed.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_timer.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_uuid.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.3/LICENSE
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.3/README.md
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 glow-0.12.3/pyproject.toml
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 glow-0.12.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.4/examples/__init__.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.4/examples/cifar10.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.4/examples/gan.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/__init__.py
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/cli.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/cli.pyi
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/distributed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/py.typed
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/api/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/api/config.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/api/exporting.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/__init__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_coro.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_import_hook.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_more.py
+-rw-r--r--   0        0        0    14592 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_parallel.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_parallel.pyi
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_patch_len.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_patch_print.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_patch_scipy.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_profile.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_profile.pyi
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_reduction.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_repr.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_sizeof.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_thread_quota.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_uuid.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/debug.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/__init__.py
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/cache.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/cache.pyi
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/concurrency.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/concurrency.pyi
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/reusable.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/util.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/io/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/io/_sound.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/io/_svg.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/metrics/__init__.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/metrics/base.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/metrics/confusion.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/metrics/raw.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/__init__.py
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/_loader.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/_sampler.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/_trainer.py
+-rw-r--r--   0        0        0    13042 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/amp.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/driver.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/functional.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/optimizers.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/plot.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/proto.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/util.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/__init__.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/aggregates.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/context.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/convnets.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/lazy.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/simple.py
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/transformers.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/util.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/vision.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/__init__.py
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/classes.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/core.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/functional/__init__.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/functional/core.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/functional/numba.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.4/test/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.4/test/run_metrics.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_api.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_batch.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_buffered.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_cli.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_iter.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_loader.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_shm.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_thread_pool.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_timed.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_timer.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_uuid.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.4/LICENSE
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.4/README.md
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 glow-0.12.4/pyproject.toml
+-rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 glow-0.12.4/PKG-INFO
```

### Comparing `glow-0.12.3/examples/cifar10.py` & `glow-0.12.4/examples/cifar10.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/cli.py` & `glow-0.12.4/src/glow/cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/cli.pyi` & `glow-0.12.4/src/glow/cli.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/distributed.py` & `glow-0.12.4/src/glow/distributed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/api/config.py` & `glow-0.12.4/src/glow/api/config.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/api/exporting.py` & `glow-0.12.4/src/glow/api/exporting.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/__init__.py` & `glow-0.12.4/src/glow/core/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_coro.py` & `glow-0.12.4/src/glow/core/_coro.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_import_hook.py` & `glow-0.12.4/src/glow/core/_import_hook.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_more.py` & `glow-0.12.4/src/glow/core/_more.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_parallel.py` & `glow-0.12.4/src/glow/core/_parallel.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_parallel.pyi` & `glow-0.12.4/src/glow/core/_parallel.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_patch_len.py` & `glow-0.12.4/src/glow/core/_patch_len.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_patch_print.py` & `glow-0.12.4/src/glow/core/_patch_print.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_patch_scipy.py` & `glow-0.12.4/src/glow/core/_patch_scipy.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_profile.py` & `glow-0.12.4/src/glow/core/_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,20 +119,21 @@
                 timer(self.cpu_ns.add, thread_time_ns):
             return op(*args, **kwargs)
 
     def stat(self) -> tuple[float, float, str] | None:
         if not (n := next(self.calls)):
             return None
         w = self.nlwp.max()
-        t = self.cpu_ns.total() / 1e9
-        a = self.all_ns.total() / 1e9
+        t_ns = self.cpu_ns.total()  # CPU
+        i_ns = self.all_ns.total() - t_ns  # idle = total - CPU
+        t, i = t_ns / 1e9, i_ns / 1e9
 
         tail = (f'{n} x {si(t / n)}s' +
                 (f' @ {w}T' if w > 1 else '')) if n > 1 else ''
-        return t, (a - t), tail
+        return t, i, tail
 
 
 class _Proxy(ObjectProxy):
     def __init__(self, wrapped, wrapper):
         super().__init__(wrapped)
         self._self_wrapper = wrapper
```

### Comparing `glow-0.12.3/src/glow/core/_profile.pyi` & `glow-0.12.4/src/glow/core/_profile.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_reduction.py` & `glow-0.12.4/src/glow/core/_reduction.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_repr.py` & `glow-0.12.4/src/glow/core/_repr.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_sizeof.py` & `glow-0.12.4/src/glow/core/_sizeof.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_thread_quota.py` & `glow-0.12.4/src/glow/core/_thread_quota.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/_uuid.py` & `glow-0.12.4/src/glow/core/_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/debug.py` & `glow-0.12.4/src/glow/core/debug.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/wrap/cache.py` & `glow-0.12.4/src/glow/core/wrap/cache.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/wrap/cache.pyi` & `glow-0.12.4/src/glow/core/wrap/cache.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/wrap/concurrency.py` & `glow-0.12.4/src/glow/core/wrap/concurrency.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,14 @@
 
     endtime = monotonic() + timeout
     while len(batch) < batch_size and (waittime := endtime - monotonic()) > 0:
         try:
             batch.append(q.get(timeout=waittime))
         except Empty:
             break
-
-    if len(batch) < batch_size:
-        print(f'timeout({len(batch)})')
     return batch
 
 
 def _batch_invoke(
     func: _BatchFn[_T, _R],
     batch: Sequence[tuple[Future[_R], _T]],
 ):
```

### Comparing `glow-0.12.3/src/glow/core/wrap/concurrency.pyi` & `glow-0.12.4/src/glow/core/wrap/concurrency.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/wrap/reusable.py` & `glow-0.12.4/src/glow/core/wrap/reusable.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/core/wrap/util.py` & `glow-0.12.4/src/glow/core/wrap/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/io/_sound.py` & `glow-0.12.4/src/glow/io/_sound.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/io/_svg.py` & `glow-0.12.4/src/glow/io/_svg.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/metrics/__init__.py` & `glow-0.12.4/src/glow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/metrics/base.py` & `glow-0.12.4/src/glow/metrics/base.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/metrics/confusion.py` & `glow-0.12.4/src/glow/metrics/confusion.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/metrics/raw.py` & `glow-0.12.4/src/glow/metrics/raw.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/__init__.py` & `glow-0.12.4/src/glow/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/_loader.py` & `glow-0.12.4/src/glow/nn/_loader.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/_sampler.py` & `glow-0.12.4/src/glow/nn/_sampler.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/_trainer.py` & `glow-0.12.4/src/glow/nn/_trainer.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/amp.py` & `glow-0.12.4/src/glow/nn/amp.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/driver.py` & `glow-0.12.4/src/glow/nn/driver.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/functional.py` & `glow-0.12.4/src/glow/nn/functional.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/optimizers.py` & `glow-0.12.4/src/glow/nn/optimizers.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/plot.py` & `glow-0.12.4/src/glow/nn/plot.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/proto.py` & `glow-0.12.4/src/glow/nn/proto.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     # CCT (Compact Convolutional Transformer)
     #   = CVT + patchify replaced with one of
     #   - 1-2 x [conv3x3 - relu - maxpool(2,2)], i.e. eff.stride = 2-4
     #   - 1-2 x [conv7x7/s2 - relu - maxpool(2,2)], i.e. eff.stride = 4-16
     transformer = nn.Sequential(
         # Operates in (b n d) domain
         nn.Identity() if pool == 'mean' else CatToken(dim),
-        nn.Dropout(dropout_emb),
+        nn.Dropout(dropout_emb, inplace=True),
         *(VitBlock(dim, dim_head, mlp_ratio, dropout, qkv_bias, reattn)
           for _ in range(depth)),
         Reduce('b n d -> b d', 'mean') if pool == 'mean' else PopToken(),
     )
     head = nn.Sequential(
         nn.LayerNorm(dim),
         nn.Linear(dim, num_classes),
```

### Comparing `glow-0.12.3/src/glow/nn/util.py` & `glow-0.12.4/src/glow/nn/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/modules/__init__.py` & `glow-0.12.4/src/glow/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/modules/aggregates.py` & `glow-0.12.4/src/glow/nn/modules/aggregates.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/modules/context.py` & `glow-0.12.4/src/glow/nn/modules/context.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/modules/convnets.py` & `glow-0.12.4/src/glow/nn/modules/convnets.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/modules/lazy.py` & `glow-0.12.4/src/glow/nn/modules/lazy.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/modules/simple.py` & `glow-0.12.4/src/glow/nn/modules/simple.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/modules/transformers.py` & `glow-0.12.4/src/glow/nn/modules/transformers.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,27 @@
     'FeedForward',
     'MaxVitBlock',
     'MultiAxisAttention',
     'VitBlock',
 ]
 
 import torch
+import torch.nn.functional as F
 from einops import rearrange
 from einops.layers.torch import Rearrange
 from packaging.version import Version
 from torch import nn
 
 from .aggregates import pre_norm
 from .context import ConvCtx
 from .convnets import mbconv
 from .util import NameMixin, round8
 
-_IS_TORCH_1_12 = Version(torch.__version__) >= Version('1.12')
+_IS_TORCH_1_12 = Version('1.12') <= Version(torch.__version__) < Version('2.0')
+_IS_TORCH_2X = Version(torch.__version__) >= Version('2.0')
 _TORCH_MHA_AUTOCAST = True
 
 
 class ReAttention(nn.Sequential):
     """Re-Attention from [DeepViT](https://arxiv.org/abs/2103.11886)"""
     def __init__(self, heads: int) -> None:
         super().__init__(
@@ -52,30 +54,34 @@
                  qkv_bias: bool = False,
                  reattention: bool = False):
         super().__init__()
         assert dim % dim_head == 0
         self.dim = dim
         self.heads = heads = dim // dim_head
         self.scale = dim_head ** -0.5
+        self.dropout = dropout
 
         self.to_qkv = nn.Sequential(
             fc := nn.Linear(dim, 3 * dim, bias=qkv_bias),
             Rearrange('b n (split h d) -> split b h n d', h=heads, split=3),
         )
         nn.init.normal_(fc.weight, 0, (2 / (dim + dim_head)) ** .5)
 
-        self.attend = nn.Sequential(nn.Softmax(-1), nn.Dropout(dropout))
+        self.attend = nn.Sequential(
+            nn.Softmax(-1),
+            nn.Dropout(dropout, inplace=True),
+        )
         self.reattention = reattention
         if reattention:
             self.attend.append(ReAttention(heads))
 
         self.to_out = nn.Sequential(
             Rearrange('b h n d -> b n (h d)'),
             fc := nn.Linear(dim, dim),
-            nn.Dropout(dropout),
+            nn.Dropout(dropout, inplace=True),
         )
         nn.init.xavier_normal_(fc.weight)
 
         self.name = f'{dim}, {heads=}'
         if qkv_bias:
             self.name += ', qkv_bias=True'
         if dropout:
@@ -104,20 +110,28 @@
                     None, False)
                 return out
 
         # b n dim -> b h n d
         qkv = self.to_qkv(x)
         q, k, v = qkv[0], qkv[1], qkv[2]  # make torchscript happy
 
-        # Compute weights for each token
-        dots = torch.einsum('bhid,bhjd -> bhij', q, k)
-        attn = self.attend(dots * self.scale)
+        # Use FLASH-attention (https://arxiv.org/abs/2205.14135)
+        # and Memory-Efficient attention from XFormers
+        # for PyTorch 2.x
+        if _IS_TORCH_2X and not self.reattention:
+            dropout = self.droupout if self.is_train else 0
+            out = F.scaled_dot_product_attention(q, k, v, dropout_p=dropout)
+
+        else:
+            # Compute weights for each token
+            dots = torch.einsum('bhid,bhjd -> bhij', q, k)
+            attn = self.attend(dots * self.scale)
 
-        # Remix tokens using weights
-        out = torch.einsum('bhij,bhjd -> bhid', attn, v)
+            # Remix tokens using weights
+            out = torch.einsum('bhij,bhjd -> bhid', attn, v)
 
         # Restore shape, b h n d -> b n (h d)
         return self.to_out(out)
 
 
 class _RelativePositionalBias(nn.Module):
     def __init__(self, heads: int, window_size: int) -> None:
@@ -162,20 +176,20 @@
             nn.Linear(dim, dim * 3, bias=qkv_bias),
             Rearrange('... i (s h d) -> s ... h i d', s=3, h=heads),
         )
         self.bias = _RelativePositionalBias(heads, window_size)
 
         self.attend = nn.Sequential(
             nn.Softmax(-1),
-            nn.Dropout(dropout),
+            nn.Dropout(dropout, inplace=True),
         )
         self.to_out = nn.Sequential(
             Rearrange('... h i d -> ... i (h d)'),
             nn.Linear(dim, dim, bias=False),
-            nn.Dropout(dropout),
+            nn.Dropout(dropout, inplace=True),
         )
         self.name = f'{dim}, {heads=}, {window_size=}'
         if qkv_bias:
             self.name += ', qkv_bias=True'
         if dropout:
             self.name += f', {dropout=}'
 
@@ -196,17 +210,17 @@
 
 class FeedForward(NameMixin, nn.Sequential):
     def __init__(self, dim: int, ratio: float, dropout: float = 0.):
         dim_inner = round8(dim * ratio)
         super().__init__(
             nn.Linear(dim, dim_inner),
             nn.GELU(),
-            nn.Dropout(dropout),
+            nn.Dropout(dropout, inplace=True),
             nn.Linear(dim_inner, dim),
-            nn.Dropout(dropout),
+            nn.Dropout(dropout, inplace=True),
         )
         self.name = f'{dim}, {dim_inner=}'
         if dropout:
             self.name += f', {dropout=}'
 
 
 # ----------------------------- complete blocks ------------------------------
```

### Comparing `glow-0.12.3/src/glow/nn/modules/util.py` & `glow-0.12.4/src/glow/nn/modules/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/nn/modules/vision.py` & `glow-0.12.4/src/glow/nn/modules/vision.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/transforms/__init__.py` & `glow-0.12.4/src/glow/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/transforms/classes.py` & `glow-0.12.4/src/glow/transforms/classes.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/transforms/core.py` & `glow-0.12.4/src/glow/transforms/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/transforms/functional/core.py` & `glow-0.12.4/src/glow/transforms/functional/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/src/glow/transforms/functional/numba.py` & `glow-0.12.4/src/glow/transforms/functional/numba.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/run_metrics.py` & `glow-0.12.4/test/run_metrics.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_api.py` & `glow-0.12.4/test/test_api.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_batch.py` & `glow-0.12.4/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_buffered.py` & `glow-0.12.4/test/test_buffered.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_cli.py` & `glow-0.12.4/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_iter.py` & `glow-0.12.4/test/test_iter.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_loader.py` & `glow-0.12.4/test/test_loader.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_shm.py` & `glow-0.12.4/test/test_shm.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_thread_pool.py` & `glow-0.12.4/test/test_thread_pool.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_timed.py` & `glow-0.12.4/test/test_timed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/test/test_uuid.py` & `glow-0.12.4/test/test_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/LICENSE` & `glow-0.12.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/README.md` & `glow-0.12.4/README.md`

 * *Files identical despite different names*

### Comparing `glow-0.12.3/pyproject.toml` & `glow-0.12.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 only-packages = true
 
 [project]
 name = "glow"
-version = "0.12.3"
+version = "0.12.4"
 description = "Functional Python tools with a PyTorch flavour"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = []
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
@@ -46,31 +46,30 @@
 nn = [
     "graphviz",
     "einops",
     "packaging",
     "pynvml~=11.4",
     "torch~=2.0",
     "torchvision~=0.15",
-    # --extra-index-url https://download.pytorch.org/whl/cu117
+    # --extra-index-url https://download.pytorch.org/whl/cu118
     # "torch-tensorrt~=1.3; platform_system=='Linux'",  # TODO: upd for torch 2.x
     # -f https://github.com/NVIDIA/Torch-TensorRT/releases
 ]
 all = ["glow[cv,io,nn]", "matplotlib"]
 dev-core = [
     "flake8~=6.0.0",
     "flake8-pie",
     "flake8-pyi",
     "flake8-pyproject",
     "flake8-simplify",
     "isort",
     "mypy~=1.1.1",
     "pytest~=6.0",
     "ruff",
-    "yapf[pyproject]==0.33.0",
-    "toml; python_version>='3.11'",  # See: https://github.com/google/yapf/pull/1040. Drop for yapf~=0.33
+    "yapf==0.33.0",
 ]
 dev = [
     "glow[dev-core]",
     "flake8-alphabetize",
     # "flake8-class-attributes-order",
     # "flake8-newspaper-style",
     "typing-extensions~=4.4",
```

### Comparing `glow-0.12.3/PKG-INFO` & `glow-0.12.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glow
-Version: 0.12.3
+Version: 0.12.4
 Summary: Functional Python tools with a PyTorch flavour
 Project-URL: homepage, https://github.com/arquolo/glow
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Paul Maevskikh
@@ -58,16 +58,15 @@
 Requires-Dist: flake8-pyproject; extra == 'dev-core'
 Requires-Dist: flake8-simplify; extra == 'dev-core'
 Requires-Dist: flake8~=6.0.0; extra == 'dev-core'
 Requires-Dist: isort; extra == 'dev-core'
 Requires-Dist: mypy~=1.1.1; extra == 'dev-core'
 Requires-Dist: pytest~=6.0; extra == 'dev-core'
 Requires-Dist: ruff; extra == 'dev-core'
-Requires-Dist: toml; python_version >= '3.11' and extra == 'dev-core'
-Requires-Dist: yapf[pyproject]==0.33.0; extra == 'dev-core'
+Requires-Dist: yapf==0.33.0; extra == 'dev-core'
 Provides-Extra: dev-wemake
 Requires-Dist: glow[dev-core]; extra == 'dev-wemake'
 Requires-Dist: wemake-python-styleguide~=0.15.0; extra == 'dev-wemake'
 Provides-Extra: io
 Requires-Dist: sounddevice; extra == 'io'
 Requires-Dist: soundfile; extra == 'io'
 Provides-Extra: memprof
```

