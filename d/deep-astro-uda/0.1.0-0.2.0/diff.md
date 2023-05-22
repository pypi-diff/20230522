# Comparing `tmp/deep_astro_uda-0.1.0.tar.gz` & `tmp/deep_astro_uda-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_astro_uda-0.1.0.tar", max compression
+gzip compressed data, was "deep_astro_uda-0.2.0.tar", max compression
```

## Comparing `deep_astro_uda-0.1.0.tar` & `deep_astro_uda-0.2.0.tar`

### file list

```diff
@@ -1,418 +1,417 @@
--rw-r--r--   0        0        0    11357 2023-05-07 23:05:47.006112 deep_astro_uda-0.1.0/LICENSE
--rw-r--r--   0        0        0    15627 2023-05-07 23:05:47.006312 deep_astro_uda-0.1.0/README.md
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.006474 deep_astro_uda-0.1.0/deep_astro_uda/__init__.py
--rw-r--r--   0        0        0       22 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/RNN/README.md
--rw-r--r--   0        0        0    11578 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/RNN/RNNBackend.py
--rw-r--r--   0        0        0       71 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/RNN/__init__.py
--rw-r--r--   0        0        0     2550 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/RNN/cells.py
--rw-r--r--   0        0        0     2137 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/RNN/models.py
--rw-r--r--   0        0        0     1488 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/__init__.py
--rw-r--r--   0        0        0     1199 2022-04-06 23:54:02.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      881 2022-04-06 23:54:22.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/__pycache__/_autocast_utils.cpython-37.pyc
--rw-r--r--   0        0        0      622 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/_autocast_utils.py
--rw-r--r--   0        0        0     2107 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/README.md
--rw-r--r--   0        0        0      310 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__init__.py
--rw-r--r--   0        0        0      584 2022-04-06 23:54:12.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     1649 2022-04-06 23:54:14.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/_amp_state.cpython-37.pyc
--rw-r--r--   0        0        0     7696 2022-04-06 23:54:22.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/_initialize.cpython-37.pyc
--rw-r--r--   0        0        0    10481 2022-04-06 23:54:14.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/_process_optimizer.cpython-37.pyc
--rw-r--r--   0        0        0     4297 2022-04-06 23:54:12.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/amp.cpython-37.pyc
--rw-r--r--   0        0        0     1620 2022-04-06 23:54:14.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/compat.cpython-37.pyc
--rw-r--r--   0        0        0    14705 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/frontend.cpython-37.pyc
--rw-r--r--   0        0        0    10352 2022-04-06 23:54:16.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/handle.cpython-37.pyc
--rw-r--r--   0        0        0     3504 2022-04-06 23:54:16.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/opt.cpython-37.pyc
--rw-r--r--   0        0        0     1947 2022-04-06 23:54:14.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/rnn_compat.cpython-37.pyc
--rw-r--r--   0        0        0     5120 2022-04-06 23:54:16.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/scaler.cpython-37.pyc
--rw-r--r--   0        0        0     5532 2022-04-06 23:54:12.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0        0        0     8168 2022-04-06 23:54:14.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/wrap.cpython-37.pyc
--rw-r--r--   0        0        0       62 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__version__.py
--rw-r--r--   0        0        0     2008 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/_amp_state.py
--rw-r--r--   0        0        0    11606 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/_initialize.py
--rw-r--r--   0        0        0    20747 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/_process_optimizer.py
--rw-r--r--   0        0        0     7266 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/amp.py
--rw-r--r--   0        0        0     1393 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/compat.py
--rw-r--r--   0        0        0    21267 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/frontend.py
--rw-r--r--   0        0        0    12066 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/handle.py
--rw-r--r--   0        0        0        0 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/__init__.py
--rw-r--r--   0        0        0      167 2022-04-06 23:54:18.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     1602 2022-04-06 23:54:18.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/__pycache__/functional_overrides.cpython-37.pyc
--rw-r--r--   0        0        0      969 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/__pycache__/tensor_overrides.cpython-37.pyc
--rw-r--r--   0        0        0     1255 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/__pycache__/torch_overrides.cpython-37.pyc
--rw-r--r--   0        0        0     2248 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/functional_overrides.py
--rw-r--r--   0        0        0     1402 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/tensor_overrides.py
--rw-r--r--   0        0        0     2082 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/torch_overrides.py
--rw-r--r--   0        0        0     3446 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/opt.py
--rw-r--r--   0        0        0     1995 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/rnn_compat.py
--rw-r--r--   0        0        0    10494 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/scaler.py
--rw-r--r--   0        0        0     7222 2022-02-13 16:30:00.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/utils.py
--rw-r--r--   0        0        0    11242 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/wrap.py
--rw-r--r--   0        0        0        0 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/__init__.py
--rw-r--r--   0        0        0      165 2022-04-06 23:54:18.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0       54 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/bottleneck/__init__.py
--rw-r--r--   0        0        0    21874 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/bottleneck/bottleneck.py
--rw-r--r--   0        0        0    11705 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/bottleneck/bottleneck_module_test.py
--rw-r--r--   0        0        0     3070 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/bottleneck/test.py
--rw-r--r--   0        0        0   100795 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/bottleneck/bottleneck.cpp
--rw-r--r--   0        0        0    15179 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/fmha_api.cpp
--rw-r--r--   0        0        0    11812 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/gemm.h
--rw-r--r--   0        0        0    16854 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/gmem_tile.h
--rw-r--r--   0        0        0     4890 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/kernel_traits.h
--rw-r--r--   0        0        0     3172 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/mask.h
--rw-r--r--   0        0        0    52449 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/smem_tile.h
--rw-r--r--   0        0        0    18865 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/softmax.h
--rw-r--r--   0        0        0    32232 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/utils.h
--rw-r--r--   0        0        0     5215 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha.h
--rw-r--r--   0        0        0     3431 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_128_64_kernel.sm80.cu
--rw-r--r--   0        0        0     3431 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_256_64_kernel.sm80.cu
--rw-r--r--   0        0        0     3431 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_384_64_kernel.sm80.cu
--rw-r--r--   0        0        0     5400 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_512_64_kernel.sm80.cu
--rw-r--r--   0        0        0    22254 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_kernel_1xN_reload.h
--rw-r--r--   0        0        0    23103 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_kernel_1xN_reload_nl.h
--rw-r--r--   0        0        0     3182 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_128_64_kernel.sm80.cu
--rw-r--r--   0        0        0     3182 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_256_64_kernel.sm80.cu
--rw-r--r--   0        0        0     3092 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_384_64_kernel.sm80.cu
--rw-r--r--   0        0        0     5280 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_512_64_kernel.sm80.cu
--rw-r--r--   0        0        0    13090 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN.h
--rw-r--r--   0        0        0    13127 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN_nl.h
--rw-r--r--   0        0        0    12841 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN_reload_v.h
--rw-r--r--   0        0        0     5653 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_kernel.h
--rw-r--r--   0        0        0     6462 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_noloop_reduce.cu
--rw-r--r--   0        0        0     4560 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_utils.h
--rw-r--r--   0        0        0    11371 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm.cu
--rw-r--r--   0        0        0    28995 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm.h
--rw-r--r--   0        0        0    12003 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm_add_relu.cu
--rw-r--r--   0        0        0    26899 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm_add_relu.h
--rw-r--r--   0        0        0      288 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/cuda_utils.h
--rw-r--r--   0        0        0     7076 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/interface.cpp
--rw-r--r--   0        0        0     3629 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/ipc.cu
--rw-r--r--   0        0        0   111190 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/nhwc_batch_norm_kernel.h
--rw-r--r--   0        0        0     5031 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln.h
--rw-r--r--   0        0        0     8416 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_api.cpp
--rw-r--r--   0        0        0    12238 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_bwd_kernels.cuh
--rw-r--r--   0        0        0    12535 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_bwd_semi_cuda_kernel.cu
--rw-r--r--   0        0        0    11335 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_fwd_cuda_kernel.cu
--rw-r--r--   0        0        0     3621 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_fwd_kernels.cuh
--rw-r--r--   0        0        0     6142 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_kernel_traits.h
--rw-r--r--   0        0        0    24284 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_utils.cuh
--rw-r--r--   0        0        0     4349 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/additive_masked_softmax_dropout_cuda.cu
--rw-r--r--   0        0        0    10498 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/dropout.cuh
--rw-r--r--   0        0        0    16706 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/encdec_multihead_attn_cuda.cu
--rw-r--r--   0        0        0    20599 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/encdec_multihead_attn_norm_add_cuda.cu
--rw-r--r--   0        0        0    23885 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/layer_norm.cuh
--rw-r--r--   0        0        0     4953 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/masked_softmax_dropout_cuda.cu
--rw-r--r--   0        0        0    42291 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/multihead_attn_frontend.cpp
--rw-r--r--   0        0        0     3462 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/philox.cuh
--rw-r--r--   0        0        0    14096 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_bias_additive_mask_cuda.cu
--rw-r--r--   0        0        0    13983 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_bias_cuda.cu
--rw-r--r--   0        0        0    13801 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_cuda.cu
--rw-r--r--   0        0        0    17742 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_norm_add_cuda.cu
--rw-r--r--   0        0        0   120513 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/softmax.cuh
--rw-r--r--   0        0        0    34726 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/strided_batched_gemm.cuh
--rw-r--r--   0        0        0     5601 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_adam_cuda.cpp
--rw-r--r--   0        0        0    35125 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_adam_cuda_kernel.cu
--rw-r--r--   0        0        0      562 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_lamb_cuda.cpp
--rw-r--r--   0        0        0     8664 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_lamb_cuda_kernel.cu
--rw-r--r--   0        0        0      560 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_adam.cpp
--rw-r--r--   0        0        0     7426 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_adam_kernel.cu
--rw-r--r--   0        0        0     1180 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_lamb.cpp
--rw-r--r--   0        0        0    14973 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_lamb_kernel.cu
--rw-r--r--   0        0        0     2416 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_joint.cpp
--rw-r--r--   0        0        0    37378 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_joint_kernel.cu
--rw-r--r--   0        0        0     2512 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_loss.cpp
--rw-r--r--   0        0        0    31783 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_loss_kernel.cu
--rw-r--r--   0        0        0     1657 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/xentropy/interface.cpp
--rw-r--r--   0        0        0    24560 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/xentropy/xentropy_kernel.cu
--rw-r--r--   0        0        0     5740 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/examples/multihead_attn/func_test_multihead_attn.py
--rw-r--r--   0        0        0     6163 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/examples/multihead_attn/perf_test_multihead_attn.py
--rw-r--r--   0        0        0       26 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/fmha/__init__.py
--rw-r--r--   0        0        0     3394 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/fmha/fmha.py
--rw-r--r--   0        0        0      239 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/groupbn/__init__.py
--rw-r--r--   0        0        0    11208 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/groupbn/batch_norm.py
--rw-r--r--   0        0        0       38 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/layer_norm/__init__.py
--rw-r--r--   0        0        0     1737 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/layer_norm/layer_norm.py
--rw-r--r--   0        0        0    86630 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/MHA_bwd.png
--rw-r--r--   0        0        0    84392 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/MHA_fwd.png
--rw-r--r--   0        0        0     2267 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/README.md
--rw-r--r--   0        0        0      176 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/__init__.py
--rw-r--r--   0        0        0     7742 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/encdec_multihead_attn.py
--rw-r--r--   0        0        0    16838 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/encdec_multihead_attn_func.py
--rw-r--r--   0        0        0     2974 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/fast_encdec_multihead_attn_func.py
--rw-r--r--   0        0        0     4258 2022-02-12 21:46:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/fast_encdec_multihead_attn_norm_add_func.py
--rw-r--r--   0        0        0     7679 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/fast_self_multihead_attn_func.py
--rw-r--r--   0        0        0     3492 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/fast_self_multihead_attn_norm_add_func.py
--rw-r--r--   0        0        0     2456 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/mask_softmax_dropout_func.py
--rw-r--r--   0        0        0    10293 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/self_multihead_attn.py
--rw-r--r--   0        0        0    14120 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/self_multihead_attn_func.py
--rw-r--r--   0        0        0      111 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/__init__.py
--rw-r--r--   0        0        0      317 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     7073 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fp16_optimizer.cpython-37.pyc
--rw-r--r--   0        0        0     5801 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fused_adam.cpython-37.pyc
--rw-r--r--   0        0        0     6176 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fused_lamb.cpython-37.pyc
--rw-r--r--   0        0        0    34787 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam.py
--rw-r--r--   0        0        0    31780 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam_v2.py
--rw-r--r--   0        0        0    15709 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam_v3.py
--rw-r--r--   0        0        0    53560 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_lamb.py
--rw-r--r--   0        0        0    10448 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/fp16_optimizer.py
--rw-r--r--   0        0        0     9284 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/fused_adam.py
--rw-r--r--   0        0        0     9408 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/fused_lamb.py
--rw-r--r--   0        0        0     9468 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/fused_sgd.py
--rw-r--r--   0        0        0     6103 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/README.md
--rw-r--r--   0        0        0       61 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/__init__.py
--rw-r--r--   0        0        0    18676 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/asp.py
--rw-r--r--   0        0        0    72541 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_lib.py
--rw-r--r--   0        0        0    14493 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/CUDA_kernels/permutation_search_kernels.cu
--rw-r--r--   0        0        0      136 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/__init__.py
--rw-r--r--   0        0        0     4572 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/call_permutation_search_kernels.py
--rw-r--r--   0        0        0    17372 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/exhaustive_search.py
--rw-r--r--   0        0        0     4374 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/permutation_utilities.py
--rw-r--r--   0        0        0     7291 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/sparse_masklib.py
--rw-r--r--   0        0        0     3358 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_part1.py
--rw-r--r--   0        0        0     3131 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_part2.py
--rw-r--r--   0        0        0     3182 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_reference.py
--rw-r--r--   0        0        0     3217 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/test/toy_problem.py
--rw-r--r--   0        0        0     4383 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/fmha/test_fmha.py
--rw-r--r--   0        0        0     1725 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/fused_dense/test_fused_dense.py
--rw-r--r--   0        0        0     7904 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/layer_norm/test_fast_layer_norm.py
--rw-r--r--   0        0        0     7429 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_encdec_multihead_attn.py
--rw-r--r--   0        0        0     3875 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_encdec_multihead_attn_norm_add.py
--rw-r--r--   0        0        0     3668 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_fast_self_multihead_attn_bias.py
--rw-r--r--   0        0        0     1800 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_mha_fused_softmax.py
--rw-r--r--   0        0        0     6569 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_self_multihead_attn.py
--rw-r--r--   0        0        0     3305 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_self_multihead_attn_norm_add.py
--rw-r--r--   0        0        0     4800 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/test_label_smoothing.py
--rw-r--r--   0        0        0     7198 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/transducer/test_transducer_joint.py
--rw-r--r--   0        0        0     7003 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/transducer/test_transducer_loss.py
--rw-r--r--   0        0        0     4780 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/transducer/transducer_ref.py
--rw-r--r--   0        0        0       79 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/transducer/__init__.py
--rw-r--r--   0        0        0    10129 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/transducer/transducer.py
--rw-r--r--   0        0        0      284 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/xentropy/__init__.py
--rw-r--r--   0        0        0     1023 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/xentropy/softmax_xentropy.py
--rw-r--r--   0        0        0     1443 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/README.md
--rw-r--r--   0        0        0      367 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/__init__.py
--rw-r--r--   0        0        0      614 2022-04-06 23:54:16.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0    17123 2022-04-06 23:54:16.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/__pycache__/fp16_optimizer.cpython-37.pyc
--rw-r--r--   0        0        0     7288 2022-04-06 23:54:16.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/__pycache__/fp16util.cpython-37.pyc
--rw-r--r--   0        0        0     5912 2022-04-06 23:54:18.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/__pycache__/loss_scaler.cpython-37.pyc
--rw-r--r--   0        0        0    28323 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/fp16_optimizer.py
--rw-r--r--   0        0        0     7141 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/fp16util.py
--rw-r--r--   0        0        0     7568 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/loss_scaler.py
--rw-r--r--   0        0        0       27 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fused_dense/__init__.py
--rw-r--r--   0        0        0     3659 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/fused_dense/fused_dense.py
--rw-r--r--   0        0        0       19 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/mlp/__init__.py
--rw-r--r--   0        0        0     2614 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/mlp/mlp.py
--rw-r--r--   0        0        0      100 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/multi_tensor_apply/__init__.py
--rw-r--r--   0        0        0      272 2022-04-06 23:54:10.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/multi_tensor_apply/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     1252 2022-04-06 23:54:10.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/multi_tensor_apply/__pycache__/multi_tensor_apply.cpython-37.pyc
--rw-r--r--   0        0        0      991 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/multi_tensor_apply/multi_tensor_apply.py
--rw-r--r--   0        0        0       99 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/normalization/__init__.py
--rw-r--r--   0        0        0      307 2022-04-06 23:54:22.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/normalization/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0    15861 2022-04-06 23:54:22.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/normalization/__pycache__/fused_layer_norm.cpython-37.pyc
--rw-r--r--   0        0        0    18218 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/normalization/fused_layer_norm.py
--rw-r--r--   0        0        0      246 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__init__.py
--rw-r--r--   0        0        0      474 2022-04-06 23:54:18.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     4245 2022-04-06 23:54:18.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_adagrad.cpython-37.pyc
--rw-r--r--   0        0        0     5863 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_adam.cpython-37.pyc
--rw-r--r--   0        0        0     6261 2022-04-06 23:54:18.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_lamb.cpython-37.pyc
--rw-r--r--   0        0        0     7506 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_mixed_precision_lamb.cpython-37.pyc
--rw-r--r--   0        0        0     7556 2022-04-06 23:54:20.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_novograd.cpython-37.pyc
--rw-r--r--   0        0        0     8168 2022-04-06 23:54:18.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_sgd.cpython-37.pyc
--rw-r--r--   0        0        0     5231 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_adagrad.py
--rw-r--r--   0        0        0     7718 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_adam.py
--rw-r--r--   0        0        0     9910 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_lamb.py
--rw-r--r--   0        0        0    11231 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_mixed_precision_lamb.py
--rw-r--r--   0        0        0    10652 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_novograd.py
--rw-r--r--   0        0        0    10041 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_sgd.py
--rw-r--r--   0        0        0     4018 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/LARC.py
--rw-r--r--   0        0        0     2699 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/README.md
--rw-r--r--   0        0        0     3667 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__init__.py
--rw-r--r--   0        0        0     4129 2022-04-06 23:54:18.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/LARC.cpython-37.pyc
--rw-r--r--   0        0        0     2910 2022-04-06 23:54:08.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0    22210 2022-04-06 23:54:08.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/distributed.cpython-37.pyc
--rw-r--r--   0        0        0     4771 2022-04-06 23:54:10.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/sync_batchnorm.cpython-37.pyc
--rw-r--r--   0        0        0     2039 2022-04-06 23:54:12.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/sync_batchnorm_kernel.cpython-37.pyc
--rw-r--r--   0        0        0    30651 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/distributed.py
--rw-r--r--   0        0        0      884 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/multiproc.py
--rw-r--r--   0        0        0     4364 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/optimized_sync_batchnorm.py
--rw-r--r--   0        0        0     5467 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/optimized_sync_batchnorm_kernel.py
--rw-r--r--   0        0        0     6532 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/sync_batchnorm.py
--rw-r--r--   0        0        0     3761 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/sync_batchnorm_kernel.py
--rw-r--r--   0        0        0      529 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/FAQs.md
--rw-r--r--   0        0        0    17166 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/README.md
--rw-r--r--   0        0        0       42 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/__init__.py
--rw-r--r--   0        0        0      233 2022-04-06 23:54:22.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0       31 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/.gitignore
--rw-r--r--   0        0        0      124 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/apex/README.md
--rw-r--r--   0        0        0      546 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/apex/fused_adam.py
--rw-r--r--   0        0        0      790 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/apex/fused_layer_norm.py
--rw-r--r--   0        0        0      432 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/apex/test.sh
--rw-r--r--   0        0        0      315 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/README.md
--rw-r--r--   0        0        0      762 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/custom_function.py
--rw-r--r--   0        0        0      601 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/custom_module.py
--rw-r--r--   0        0        0      432 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/test.sh
--rw-r--r--   0        0        0     4109 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/imagenet/imagenet.py
--rw-r--r--   0        0        0      673 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/imagenet/test.sh
--rw-r--r--   0        0        0      393 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/README.md
--rw-r--r--   0        0        0      620 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/jit_script_function.py
--rw-r--r--   0        0        0      689 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/jit_script_method.py
--rw-r--r--   0        0        0      675 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/jit_trace_function.py
--rw-r--r--   0        0        0      817 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/jit_trace_method.py
--rw-r--r--   0        0        0      432 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/test.sh
--rw-r--r--   0        0        0     1679 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/lenet.py
--rw-r--r--   0        0        0     3439 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/operators.py
--rw-r--r--   0        0        0      791 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/simple.py
--rw-r--r--   0        0        0     1587 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/user_annotation/README.md
--rw-r--r--   0        0        0     5660 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/user_annotation/resnet.py
--rw-r--r--   0        0        0      544 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/user_annotation/test.sh
--rw-r--r--   0        0        0       69 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/nvtx/__init__.py
--rw-r--r--   0        0        0      246 2022-04-06 23:54:24.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/nvtx/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     6180 2022-04-06 23:54:24.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/nvtx/__pycache__/nvmarker.cpython-37.pyc
--rw-r--r--   0        0        0     6153 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/nvtx/nvmarker.py
--rw-r--r--   0        0        0        0 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/__init__.py
--rw-r--r--   0        0        0      250 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/__main__.py
--rw-r--r--   0        0        0     1205 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/db.py
--rw-r--r--   0        0        0     5286 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/kernel.py
--rw-r--r--   0        0        0     8803 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/nvvp.py
--rw-r--r--   0        0        0     2907 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/parse.py
--rw-r--r--   0        0        0       25 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__init__.py
--rw-r--r--   0        0        0      248 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__main__.py
--rw-r--r--   0        0        0      213 2022-04-06 23:54:24.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     2405 2022-04-06 23:54:32.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/activation.cpython-37.pyc
--rw-r--r--   0        0        0     1503 2022-04-06 23:54:28.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/base.cpython-37.pyc
--rw-r--r--   0        0        0     9133 2022-04-06 23:54:28.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/blas.cpython-37.pyc
--rw-r--r--   0        0        0     7166 2022-04-06 23:54:30.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/conv.cpython-37.pyc
--rw-r--r--   0        0        0     2051 2022-04-06 23:54:28.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/convert.cpython-37.pyc
--rw-r--r--   0        0        0     1584 2022-04-06 23:54:26.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/data.cpython-37.pyc
--rw-r--r--   0        0        0     1768 2022-04-06 23:54:30.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/dropout.cpython-37.pyc
--rw-r--r--   0        0        0     2005 2022-04-06 23:54:30.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/embedding.cpython-37.pyc
--rw-r--r--   0        0        0    11970 2022-04-06 23:54:32.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/index_slice_join_mutate.cpython-37.pyc
--rw-r--r--   0        0        0     4055 2022-04-06 23:54:32.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/linear.cpython-37.pyc
--rw-r--r--   0        0        0     2659 2022-04-06 23:54:34.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/loss.cpython-37.pyc
--rw-r--r--   0        0        0     7040 2022-04-06 23:54:34.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/misc.cpython-37.pyc
--rw-r--r--   0        0        0     1878 2022-04-06 23:54:32.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/normalization.cpython-37.pyc
--rw-r--r--   0        0        0     2079 2022-04-06 23:54:32.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/optim.cpython-37.pyc
--rw-r--r--   0        0        0     3489 2022-04-06 23:54:28.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/output.cpython-37.pyc
--rw-r--r--   0        0        0     5397 2022-04-06 23:54:28.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/pointwise.cpython-37.pyc
--rw-r--r--   0        0        0     4507 2022-04-06 23:54:26.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/prof.cpython-37.pyc
--rw-r--r--   0        0        0     1624 2022-04-06 23:54:32.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/randomSample.cpython-37.pyc
--rw-r--r--   0        0        0     4512 2022-04-06 23:54:32.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/recurrentCell.cpython-37.pyc
--rw-r--r--   0        0        0     4881 2022-04-06 23:54:30.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/reduction.cpython-37.pyc
--rw-r--r--   0        0        0     3813 2022-04-06 23:54:32.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/softmax.cpython-37.pyc
--rw-r--r--   0        0        0     2384 2022-04-06 23:54:28.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/usage.cpython-37.pyc
--rw-r--r--   0        0        0     1860 2022-04-06 23:54:26.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/utility.cpython-37.pyc
--rw-r--r--   0        0        0     1520 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/activation.py
--rw-r--r--   0        0        0      742 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/base.py
--rw-r--r--   0        0        0     6773 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/blas.py
--rw-r--r--   0        0        0     6355 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/conv.py
--rw-r--r--   0        0        0     1242 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/convert.py
--rw-r--r--   0        0        0     1388 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/data.py
--rw-r--r--   0        0        0      999 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/dropout.py
--rw-r--r--   0        0        0     1409 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/embedding.py
--rw-r--r--   0        0        0     8004 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/index_slice_join_mutate.py
--rw-r--r--   0        0        0     4426 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/linear.py
--rw-r--r--   0        0        0     1716 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/loss.py
--rw-r--r--   0        0        0     3988 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/misc.py
--rw-r--r--   0        0        0     1003 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/normalization.py
--rw-r--r--   0        0        0     1472 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/optim.py
--rw-r--r--   0        0        0     3665 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/output.py
--rw-r--r--   0        0        0     5521 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/pointwise.py
--rw-r--r--   0        0        0     1459 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/pooling.py
--rw-r--r--   0        0        0     4967 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/prof.py
--rw-r--r--   0        0        0      817 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/randomSample.py
--rw-r--r--   0        0        0     4307 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/recurrentCell.py
--rw-r--r--   0        0        0     2788 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/reduction.py
--rw-r--r--   0        0        0     2190 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/softmax.py
--rw-r--r--   0        0        0     2018 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/usage.py
--rw-r--r--   0        0        0     1326 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/utility.py
--rw-r--r--   0        0        0       22 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/reparameterization/README.md
--rw-r--r--   0        0        0     5501 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/reparameterization/__init__.py
--rw-r--r--   0        0        0     6442 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/reparameterization/reparameterization.py
--rw-r--r--   0        0        0     3281 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/reparameterization/weight_norm.py
--rw-r--r--   0        0        0     2775 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/README.md
--rw-r--r--   0        0        0      577 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__init__.py
--rw-r--r--   0        0        0      605 2022-04-06 23:54:34.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      930 2022-04-06 23:54:38.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/enums.cpython-37.pyc
--rw-r--r--   0        0        0      757 2022-04-06 23:54:44.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/log_util.cpython-37.pyc
--rw-r--r--   0        0        0     4745 2022-04-06 23:54:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/microbatches.cpython-37.pyc
--rw-r--r--   0        0        0    12611 2022-04-06 23:54:36.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/parallel_state.cpython-37.pyc
--rw-r--r--   0        0        0     1849 2022-04-06 23:54:36.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0        0        0      248 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/_data/__init__.py
--rw-r--r--   0        0        0     7203 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/_data/_batchsampler.py
--rw-r--r--   0        0        0       90 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/amp/__init__.py
--rw-r--r--   0        0        0      262 2022-04-06 23:54:34.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/amp/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     3859 2022-04-06 23:54:34.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/amp/__pycache__/grad_scaler.cpython-37.pyc
--rw-r--r--   0        0        0     4725 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/amp/grad_scaler.py
--rw-r--r--   0        0        0      914 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/enums.py
--rw-r--r--   0        0        0      120 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/functional/__init__.py
--rw-r--r--   0        0        0      289 2022-04-06 23:54:36.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/functional/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     5531 2022-04-06 23:54:38.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/functional/__pycache__/fused_softmax.cpython-37.pyc
--rw-r--r--   0        0        0     7443 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/functional/fused_softmax.py
--rw-r--r--   0        0        0      415 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/log_util.py
--rw-r--r--   0        0        0     6799 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/microbatches.py
--rw-r--r--   0        0        0    19273 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/parallel_state.py
--rw-r--r--   0        0        0      227 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/__init__.py
--rw-r--r--   0        0        0      399 2022-04-06 23:54:38.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     2750 2022-04-06 23:54:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/_timers.cpython-37.pyc
--rw-r--r--   0        0        0     7754 2022-04-06 23:54:46.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/p2p_communication.cpython-37.pyc
--rw-r--r--   0        0        0     9342 2022-04-06 23:54:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0        0        0     2538 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/_timers.py
--rw-r--r--   0        0        0    15038 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/p2p_communication.py
--rw-r--r--   0        0        0     1725 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__init__.py
--rw-r--r--   0        0        0     1662 2022-04-06 23:54:40.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     9433 2022-04-06 23:54:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/common.cpython-37.pyc
--rw-r--r--   0        0        0     3479 2022-04-06 23:54:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_no_pipelining.cpython-37.pyc
--rw-r--r--   0        0        0     8204 2022-04-06 23:54:44.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_pipelining_with_interleaving.cpython-37.pyc
--rw-r--r--   0        0        0     7603 2022-04-06 23:54:46.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_pipelining_without_interleaving.cpython-37.pyc
--rw-r--r--   0        0        0    13017 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/common.py
--rw-r--r--   0        0        0     4565 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_no_pipelining.py
--rw-r--r--   0        0        0    16254 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_pipelining_with_interleaving.py
--rw-r--r--   0        0        0    14989 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_pipelining_without_interleaving.py
--rw-r--r--   0        0        0    12563 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/utils.py
--rw-r--r--   0        0        0     2445 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__init__.py
--rw-r--r--   0        0        0     1464 2022-04-06 23:54:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     2421 2022-04-06 23:54:44.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/cross_entropy.cpython-37.pyc
--rw-r--r--   0        0        0     2792 2022-04-06 23:54:44.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/data.cpython-37.pyc
--rw-r--r--   0        0        0    12103 2022-04-06 23:54:46.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/layers.cpython-37.pyc
--rw-r--r--   0        0        0     4887 2022-04-06 23:54:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/mappings.cpython-37.pyc
--rw-r--r--   0        0        0     4541 2022-04-06 23:54:44.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/memory.cpython-37.pyc
--rw-r--r--   0        0        0     8539 2022-04-06 23:54:44.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/random.cpython-37.pyc
--rw-r--r--   0        0        0     1885 2022-04-06 23:54:44.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0        0        0     4720 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/cross_entropy.py
--rw-r--r--   0        0        0     3957 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/data.py
--rw-r--r--   0        0        0    18874 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/layers.py
--rw-r--r--   0        0        0     4534 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/mappings.py
--rw-r--r--   0        0        0     5108 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/memory.py
--rw-r--r--   0        0        0    11491 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/random.py
--rw-r--r--   0        0        0     2202 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/utils.py
--rw-r--r--   0        0        0        0 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/__init__.py
--rw-r--r--   0        0        0    41613 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/arguments.py
--rw-r--r--   0        0        0     4864 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/commons.py
--rw-r--r--   0        0        0     8862 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/global_vars.py
--rw-r--r--   0        0        0     9001 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/standalone_bert.py
--rw-r--r--   0        0        0    61609 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/standalone_gpt.py
--rw-r--r--   0        0        0     1543 2022-02-12 21:46:42.000000 deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/utils.py
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.006634 deep_astro_uda-0.1.0/deep_astro_uda/client/__init__.py
--rw-r--r--   0        0        0      576 2023-05-22 13:40:52.447152 deep_astro_uda-0.1.0/deep_astro_uda/client/astro_app.py
--rw-r--r--   0        0        0     1537 2023-05-22 13:44:11.732119 deep_astro_uda-0.1.0/deep_astro_uda/client/commands/demo_command.py
--rw-r--r--   0        0        0      211 2023-05-07 23:25:39.024353 deep_astro_uda-0.1.0/deep_astro_uda/client/commands/infer_command.py
--rw-r--r--   0        0        0     3718 2023-05-22 13:38:41.690234 deep_astro_uda-0.1.0/deep_astro_uda/client/commands/run_command.py
--rw-r--r--   0        0        0      746 2023-05-22 11:04:39.960250 deep_astro_uda-0.1.0/deep_astro_uda/client/options.py
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007013 deep_astro_uda-0.1.0/deep_astro_uda/configs/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-22 13:30:21.731901 deep_astro_uda-0.1.0/deep_astro_uda/configs/config.yaml
--rw-r--r--   0        0        0     1996 2023-05-22 11:12:40.144312 deep_astro_uda-0.1.0/deep_astro_uda/configs/config_functions.py
--rw-r--r--   0        0        0        0 2023-05-08 03:56:27.706969 deep_astro_uda-0.1.0/deep_astro_uda/data_utils/__init__.py
--rw-r--r--   0        0        0     2908 2023-05-08 05:07:18.180392 deep_astro_uda-0.1.0/deep_astro_uda/data_utils/download_data.py
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007291 deep_astro_uda-0.1.0/deep_astro_uda/dist/__init__.py
--rw-r--r--   0        0        0    10906 2023-05-07 23:05:47.007467 deep_astro_uda-0.1.0/deep_astro_uda/dist/deep_astro_uda-0.1.0.tar.gz
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007637 deep_astro_uda-0.1.0/deep_astro_uda/model/__init__.py
--rw-r--r--   0        0        0     6696 2023-05-22 12:36:09.942437 deep_astro_uda-0.1.0/deep_astro_uda/model/eval.py
--rw-r--r--   0        0        0     5632 2023-05-07 23:05:47.007756 deep_astro_uda-0.1.0/deep_astro_uda/model/get_loader.py
--rw-r--r--   0        0        0     4146 2023-05-07 23:05:47.007876 deep_astro_uda-0.1.0/deep_astro_uda/model/loss.py
--rw-r--r--   0        0        0      465 2023-05-07 23:05:47.007980 deep_astro_uda-0.1.0/deep_astro_uda/model/lr_schedule.py
--rw-r--r--   0        0        0     7913 2023-05-22 12:36:19.983415 deep_astro_uda-0.1.0/deep_astro_uda/model/train.py
--rw-r--r--   0        0        0      459 2023-05-22 13:15:04.892342 deep_astro_uda-0.1.0/deep_astro_uda/settings.py
--rw-r--r--   0        0        0     6468 2023-05-07 23:05:47.009742 deep_astro_uda-0.1.0/deep_astro_uda/tuner/tuner.py
--rw-r--r--   0        0        0        1 2023-05-07 23:05:47.008275 deep_astro_uda-0.1.0/deep_astro_uda/utils/__init__.py
--rw-r--r--   0        0        0      698 2023-05-07 23:05:47.008398 deep_astro_uda-0.1.0/deep_astro_uda/utils/utils.py
--rw-r--r--   0        0        0      379 2023-05-22 13:49:48.128012 deep_astro_uda-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    19611 1970-01-01 00:00:00.000000 deep_astro_uda-0.1.0/setup.py
--rw-r--r--   0        0        0    16071 1970-01-01 00:00:00.000000 deep_astro_uda-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-07 23:05:47.006112 deep_astro_uda-0.2.0/LICENSE
+-rw-r--r--   0        0        0    15627 2023-05-07 23:05:47.006312 deep_astro_uda-0.2.0/README.md
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.006474 deep_astro_uda-0.2.0/deep_astro_uda/__init__.py
+-rw-r--r--   0        0        0       22 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/RNN/README.md
+-rw-r--r--   0        0        0    11578 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/RNN/RNNBackend.py
+-rw-r--r--   0        0        0       71 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/RNN/__init__.py
+-rw-r--r--   0        0        0     2550 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/RNN/cells.py
+-rw-r--r--   0        0        0     2137 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/RNN/models.py
+-rw-r--r--   0        0        0     1488 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/__init__.py
+-rw-r--r--   0        0        0     1199 2022-04-06 23:54:02.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      881 2022-04-06 23:54:22.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/__pycache__/_autocast_utils.cpython-37.pyc
+-rw-r--r--   0        0        0      622 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/_autocast_utils.py
+-rw-r--r--   0        0        0     2107 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/README.md
+-rw-r--r--   0        0        0      310 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__init__.py
+-rw-r--r--   0        0        0      584 2022-04-06 23:54:12.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1649 2022-04-06 23:54:14.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/_amp_state.cpython-37.pyc
+-rw-r--r--   0        0        0     7696 2022-04-06 23:54:22.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/_initialize.cpython-37.pyc
+-rw-r--r--   0        0        0    10481 2022-04-06 23:54:14.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/_process_optimizer.cpython-37.pyc
+-rw-r--r--   0        0        0     4297 2022-04-06 23:54:12.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/amp.cpython-37.pyc
+-rw-r--r--   0        0        0     1620 2022-04-06 23:54:14.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/compat.cpython-37.pyc
+-rw-r--r--   0        0        0    14705 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/frontend.cpython-37.pyc
+-rw-r--r--   0        0        0    10352 2022-04-06 23:54:16.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/handle.cpython-37.pyc
+-rw-r--r--   0        0        0     3504 2022-04-06 23:54:16.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/opt.cpython-37.pyc
+-rw-r--r--   0        0        0     1947 2022-04-06 23:54:14.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/rnn_compat.cpython-37.pyc
+-rw-r--r--   0        0        0     5120 2022-04-06 23:54:16.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/scaler.cpython-37.pyc
+-rw-r--r--   0        0        0     5532 2022-04-06 23:54:12.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0        0        0     8168 2022-04-06 23:54:14.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/wrap.cpython-37.pyc
+-rw-r--r--   0        0        0       62 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__version__.py
+-rw-r--r--   0        0        0     2008 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/_amp_state.py
+-rw-r--r--   0        0        0    11606 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/_initialize.py
+-rw-r--r--   0        0        0    20747 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/_process_optimizer.py
+-rw-r--r--   0        0        0     7266 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/amp.py
+-rw-r--r--   0        0        0     1393 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/compat.py
+-rw-r--r--   0        0        0    21267 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/frontend.py
+-rw-r--r--   0        0        0    12066 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/handle.py
+-rw-r--r--   0        0        0        0 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/__init__.py
+-rw-r--r--   0        0        0      167 2022-04-06 23:54:18.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1602 2022-04-06 23:54:18.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/__pycache__/functional_overrides.cpython-37.pyc
+-rw-r--r--   0        0        0      969 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/__pycache__/tensor_overrides.cpython-37.pyc
+-rw-r--r--   0        0        0     1255 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/__pycache__/torch_overrides.cpython-37.pyc
+-rw-r--r--   0        0        0     2248 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/functional_overrides.py
+-rw-r--r--   0        0        0     1402 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/tensor_overrides.py
+-rw-r--r--   0        0        0     2082 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/torch_overrides.py
+-rw-r--r--   0        0        0     3446 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/opt.py
+-rw-r--r--   0        0        0     1995 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/rnn_compat.py
+-rw-r--r--   0        0        0    10494 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/scaler.py
+-rw-r--r--   0        0        0     7222 2022-02-13 16:30:00.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/utils.py
+-rw-r--r--   0        0        0    11242 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/wrap.py
+-rw-r--r--   0        0        0        0 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/__init__.py
+-rw-r--r--   0        0        0      165 2022-04-06 23:54:18.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0       54 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/bottleneck/__init__.py
+-rw-r--r--   0        0        0    21874 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/bottleneck/bottleneck.py
+-rw-r--r--   0        0        0    11705 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/bottleneck/bottleneck_module_test.py
+-rw-r--r--   0        0        0     3070 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/bottleneck/test.py
+-rw-r--r--   0        0        0   100795 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/bottleneck/bottleneck.cpp
+-rw-r--r--   0        0        0    15179 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/fmha_api.cpp
+-rw-r--r--   0        0        0    11812 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/gemm.h
+-rw-r--r--   0        0        0    16854 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/gmem_tile.h
+-rw-r--r--   0        0        0     4890 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/kernel_traits.h
+-rw-r--r--   0        0        0     3172 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/mask.h
+-rw-r--r--   0        0        0    52449 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/smem_tile.h
+-rw-r--r--   0        0        0    18865 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/softmax.h
+-rw-r--r--   0        0        0    32232 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/utils.h
+-rw-r--r--   0        0        0     5215 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha.h
+-rw-r--r--   0        0        0     3431 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_128_64_kernel.sm80.cu
+-rw-r--r--   0        0        0     3431 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_256_64_kernel.sm80.cu
+-rw-r--r--   0        0        0     3431 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_384_64_kernel.sm80.cu
+-rw-r--r--   0        0        0     5400 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_512_64_kernel.sm80.cu
+-rw-r--r--   0        0        0    22254 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_kernel_1xN_reload.h
+-rw-r--r--   0        0        0    23103 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_kernel_1xN_reload_nl.h
+-rw-r--r--   0        0        0     3182 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_128_64_kernel.sm80.cu
+-rw-r--r--   0        0        0     3182 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_256_64_kernel.sm80.cu
+-rw-r--r--   0        0        0     3092 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_384_64_kernel.sm80.cu
+-rw-r--r--   0        0        0     5280 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_512_64_kernel.sm80.cu
+-rw-r--r--   0        0        0    13090 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN.h
+-rw-r--r--   0        0        0    13127 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN_nl.h
+-rw-r--r--   0        0        0    12841 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN_reload_v.h
+-rw-r--r--   0        0        0     5653 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_kernel.h
+-rw-r--r--   0        0        0     6462 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_noloop_reduce.cu
+-rw-r--r--   0        0        0     4560 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_utils.h
+-rw-r--r--   0        0        0    11371 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm.cu
+-rw-r--r--   0        0        0    28995 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm.h
+-rw-r--r--   0        0        0    12003 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm_add_relu.cu
+-rw-r--r--   0        0        0    26899 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm_add_relu.h
+-rw-r--r--   0        0        0      288 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/cuda_utils.h
+-rw-r--r--   0        0        0     7076 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/interface.cpp
+-rw-r--r--   0        0        0     3629 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/ipc.cu
+-rw-r--r--   0        0        0   111190 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/nhwc_batch_norm_kernel.h
+-rw-r--r--   0        0        0     5031 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln.h
+-rw-r--r--   0        0        0     8416 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_api.cpp
+-rw-r--r--   0        0        0    12238 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_bwd_kernels.cuh
+-rw-r--r--   0        0        0    12535 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_bwd_semi_cuda_kernel.cu
+-rw-r--r--   0        0        0    11335 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_fwd_cuda_kernel.cu
+-rw-r--r--   0        0        0     3621 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_fwd_kernels.cuh
+-rw-r--r--   0        0        0     6142 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_kernel_traits.h
+-rw-r--r--   0        0        0    24284 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_utils.cuh
+-rw-r--r--   0        0        0     4349 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/additive_masked_softmax_dropout_cuda.cu
+-rw-r--r--   0        0        0    10498 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/dropout.cuh
+-rw-r--r--   0        0        0    16706 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/encdec_multihead_attn_cuda.cu
+-rw-r--r--   0        0        0    20599 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/encdec_multihead_attn_norm_add_cuda.cu
+-rw-r--r--   0        0        0    23885 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/layer_norm.cuh
+-rw-r--r--   0        0        0     4953 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/masked_softmax_dropout_cuda.cu
+-rw-r--r--   0        0        0    42291 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/multihead_attn_frontend.cpp
+-rw-r--r--   0        0        0     3462 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/philox.cuh
+-rw-r--r--   0        0        0    14096 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_bias_additive_mask_cuda.cu
+-rw-r--r--   0        0        0    13983 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_bias_cuda.cu
+-rw-r--r--   0        0        0    13801 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_cuda.cu
+-rw-r--r--   0        0        0    17742 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_norm_add_cuda.cu
+-rw-r--r--   0        0        0   120513 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/softmax.cuh
+-rw-r--r--   0        0        0    34726 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/strided_batched_gemm.cuh
+-rw-r--r--   0        0        0     5601 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_adam_cuda.cpp
+-rw-r--r--   0        0        0    35125 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_adam_cuda_kernel.cu
+-rw-r--r--   0        0        0      562 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_lamb_cuda.cpp
+-rw-r--r--   0        0        0     8664 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_lamb_cuda_kernel.cu
+-rw-r--r--   0        0        0      560 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_adam.cpp
+-rw-r--r--   0        0        0     7426 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_adam_kernel.cu
+-rw-r--r--   0        0        0     1180 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_lamb.cpp
+-rw-r--r--   0        0        0    14973 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_lamb_kernel.cu
+-rw-r--r--   0        0        0     2416 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_joint.cpp
+-rw-r--r--   0        0        0    37378 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_joint_kernel.cu
+-rw-r--r--   0        0        0     2512 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_loss.cpp
+-rw-r--r--   0        0        0    31783 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_loss_kernel.cu
+-rw-r--r--   0        0        0     1657 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/xentropy/interface.cpp
+-rw-r--r--   0        0        0    24560 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/xentropy/xentropy_kernel.cu
+-rw-r--r--   0        0        0     5740 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/examples/multihead_attn/func_test_multihead_attn.py
+-rw-r--r--   0        0        0     6163 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/examples/multihead_attn/perf_test_multihead_attn.py
+-rw-r--r--   0        0        0       26 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/fmha/__init__.py
+-rw-r--r--   0        0        0     3394 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/fmha/fmha.py
+-rw-r--r--   0        0        0      239 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/groupbn/__init__.py
+-rw-r--r--   0        0        0    11208 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/groupbn/batch_norm.py
+-rw-r--r--   0        0        0       38 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/layer_norm/__init__.py
+-rw-r--r--   0        0        0     1737 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/layer_norm/layer_norm.py
+-rw-r--r--   0        0        0    86630 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/MHA_bwd.png
+-rw-r--r--   0        0        0    84392 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/MHA_fwd.png
+-rw-r--r--   0        0        0     2267 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/README.md
+-rw-r--r--   0        0        0      176 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/__init__.py
+-rw-r--r--   0        0        0     7742 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/encdec_multihead_attn.py
+-rw-r--r--   0        0        0    16838 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/encdec_multihead_attn_func.py
+-rw-r--r--   0        0        0     2974 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/fast_encdec_multihead_attn_func.py
+-rw-r--r--   0        0        0     4258 2022-02-12 21:46:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/fast_encdec_multihead_attn_norm_add_func.py
+-rw-r--r--   0        0        0     7679 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/fast_self_multihead_attn_func.py
+-rw-r--r--   0        0        0     3492 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/fast_self_multihead_attn_norm_add_func.py
+-rw-r--r--   0        0        0     2456 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/mask_softmax_dropout_func.py
+-rw-r--r--   0        0        0    10293 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/self_multihead_attn.py
+-rw-r--r--   0        0        0    14120 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/self_multihead_attn_func.py
+-rw-r--r--   0        0        0      111 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/__init__.py
+-rw-r--r--   0        0        0      317 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     7073 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fp16_optimizer.cpython-37.pyc
+-rw-r--r--   0        0        0     5801 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fused_adam.cpython-37.pyc
+-rw-r--r--   0        0        0     6176 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fused_lamb.cpython-37.pyc
+-rw-r--r--   0        0        0    34787 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam.py
+-rw-r--r--   0        0        0    31780 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam_v2.py
+-rw-r--r--   0        0        0    15709 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam_v3.py
+-rw-r--r--   0        0        0    53560 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_lamb.py
+-rw-r--r--   0        0        0    10448 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/fp16_optimizer.py
+-rw-r--r--   0        0        0     9284 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/fused_adam.py
+-rw-r--r--   0        0        0     9408 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/fused_lamb.py
+-rw-r--r--   0        0        0     9468 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/fused_sgd.py
+-rw-r--r--   0        0        0     6103 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/README.md
+-rw-r--r--   0        0        0       61 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/__init__.py
+-rw-r--r--   0        0        0    18676 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/asp.py
+-rw-r--r--   0        0        0    72541 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_lib.py
+-rw-r--r--   0        0        0    14493 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/CUDA_kernels/permutation_search_kernels.cu
+-rw-r--r--   0        0        0      136 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/__init__.py
+-rw-r--r--   0        0        0     4572 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/call_permutation_search_kernels.py
+-rw-r--r--   0        0        0    17372 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/exhaustive_search.py
+-rw-r--r--   0        0        0     4374 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/permutation_utilities.py
+-rw-r--r--   0        0        0     7291 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/sparse_masklib.py
+-rw-r--r--   0        0        0     3358 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_part1.py
+-rw-r--r--   0        0        0     3131 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_part2.py
+-rw-r--r--   0        0        0     3182 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_reference.py
+-rw-r--r--   0        0        0     3217 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/test/toy_problem.py
+-rw-r--r--   0        0        0     4383 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/fmha/test_fmha.py
+-rw-r--r--   0        0        0     1725 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/fused_dense/test_fused_dense.py
+-rw-r--r--   0        0        0     7904 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/layer_norm/test_fast_layer_norm.py
+-rw-r--r--   0        0        0     7429 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_encdec_multihead_attn.py
+-rw-r--r--   0        0        0     3875 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_encdec_multihead_attn_norm_add.py
+-rw-r--r--   0        0        0     3668 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_fast_self_multihead_attn_bias.py
+-rw-r--r--   0        0        0     1800 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_mha_fused_softmax.py
+-rw-r--r--   0        0        0     6569 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_self_multihead_attn.py
+-rw-r--r--   0        0        0     3305 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_self_multihead_attn_norm_add.py
+-rw-r--r--   0        0        0     4800 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/test_label_smoothing.py
+-rw-r--r--   0        0        0     7198 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/transducer/test_transducer_joint.py
+-rw-r--r--   0        0        0     7003 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/transducer/test_transducer_loss.py
+-rw-r--r--   0        0        0     4780 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/transducer/transducer_ref.py
+-rw-r--r--   0        0        0       79 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/transducer/__init__.py
+-rw-r--r--   0        0        0    10129 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/transducer/transducer.py
+-rw-r--r--   0        0        0      284 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/xentropy/__init__.py
+-rw-r--r--   0        0        0     1023 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/xentropy/softmax_xentropy.py
+-rw-r--r--   0        0        0     1443 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/README.md
+-rw-r--r--   0        0        0      367 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/__init__.py
+-rw-r--r--   0        0        0      614 2022-04-06 23:54:16.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0    17123 2022-04-06 23:54:16.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/__pycache__/fp16_optimizer.cpython-37.pyc
+-rw-r--r--   0        0        0     7288 2022-04-06 23:54:16.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/__pycache__/fp16util.cpython-37.pyc
+-rw-r--r--   0        0        0     5912 2022-04-06 23:54:18.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/__pycache__/loss_scaler.cpython-37.pyc
+-rw-r--r--   0        0        0    28323 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/fp16_optimizer.py
+-rw-r--r--   0        0        0     7141 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/fp16util.py
+-rw-r--r--   0        0        0     7568 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/loss_scaler.py
+-rw-r--r--   0        0        0       27 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fused_dense/__init__.py
+-rw-r--r--   0        0        0     3659 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/fused_dense/fused_dense.py
+-rw-r--r--   0        0        0       19 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/mlp/__init__.py
+-rw-r--r--   0        0        0     2614 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/mlp/mlp.py
+-rw-r--r--   0        0        0      100 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/multi_tensor_apply/__init__.py
+-rw-r--r--   0        0        0      272 2022-04-06 23:54:10.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/multi_tensor_apply/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1252 2022-04-06 23:54:10.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/multi_tensor_apply/__pycache__/multi_tensor_apply.cpython-37.pyc
+-rw-r--r--   0        0        0      991 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/multi_tensor_apply/multi_tensor_apply.py
+-rw-r--r--   0        0        0       99 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/normalization/__init__.py
+-rw-r--r--   0        0        0      307 2022-04-06 23:54:22.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/normalization/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0    15861 2022-04-06 23:54:22.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/normalization/__pycache__/fused_layer_norm.cpython-37.pyc
+-rw-r--r--   0        0        0    18218 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/normalization/fused_layer_norm.py
+-rw-r--r--   0        0        0      246 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__init__.py
+-rw-r--r--   0        0        0      474 2022-04-06 23:54:18.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     4245 2022-04-06 23:54:18.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_adagrad.cpython-37.pyc
+-rw-r--r--   0        0        0     5863 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_adam.cpython-37.pyc
+-rw-r--r--   0        0        0     6261 2022-04-06 23:54:18.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_lamb.cpython-37.pyc
+-rw-r--r--   0        0        0     7506 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_mixed_precision_lamb.cpython-37.pyc
+-rw-r--r--   0        0        0     7556 2022-04-06 23:54:20.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_novograd.cpython-37.pyc
+-rw-r--r--   0        0        0     8168 2022-04-06 23:54:18.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_sgd.cpython-37.pyc
+-rw-r--r--   0        0        0     5231 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_adagrad.py
+-rw-r--r--   0        0        0     7718 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_adam.py
+-rw-r--r--   0        0        0     9910 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_lamb.py
+-rw-r--r--   0        0        0    11231 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_mixed_precision_lamb.py
+-rw-r--r--   0        0        0    10652 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_novograd.py
+-rw-r--r--   0        0        0    10041 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_sgd.py
+-rw-r--r--   0        0        0     4018 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/LARC.py
+-rw-r--r--   0        0        0     2699 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/README.md
+-rw-r--r--   0        0        0     3667 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__init__.py
+-rw-r--r--   0        0        0     4129 2022-04-06 23:54:18.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/LARC.cpython-37.pyc
+-rw-r--r--   0        0        0     2910 2022-04-06 23:54:08.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0    22210 2022-04-06 23:54:08.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/distributed.cpython-37.pyc
+-rw-r--r--   0        0        0     4771 2022-04-06 23:54:10.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/sync_batchnorm.cpython-37.pyc
+-rw-r--r--   0        0        0     2039 2022-04-06 23:54:12.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/sync_batchnorm_kernel.cpython-37.pyc
+-rw-r--r--   0        0        0    30651 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/distributed.py
+-rw-r--r--   0        0        0      884 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/multiproc.py
+-rw-r--r--   0        0        0     4364 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/optimized_sync_batchnorm.py
+-rw-r--r--   0        0        0     5467 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/optimized_sync_batchnorm_kernel.py
+-rw-r--r--   0        0        0     6532 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/sync_batchnorm.py
+-rw-r--r--   0        0        0     3761 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/sync_batchnorm_kernel.py
+-rw-r--r--   0        0        0      529 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/FAQs.md
+-rw-r--r--   0        0        0    17166 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/README.md
+-rw-r--r--   0        0        0       42 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/__init__.py
+-rw-r--r--   0        0        0      233 2022-04-06 23:54:22.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0       31 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/.gitignore
+-rw-r--r--   0        0        0      124 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/apex/README.md
+-rw-r--r--   0        0        0      546 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/apex/fused_adam.py
+-rw-r--r--   0        0        0      790 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/apex/fused_layer_norm.py
+-rw-r--r--   0        0        0      432 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/apex/test.sh
+-rw-r--r--   0        0        0      315 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/README.md
+-rw-r--r--   0        0        0      762 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/custom_function.py
+-rw-r--r--   0        0        0      601 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/custom_module.py
+-rw-r--r--   0        0        0      432 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/test.sh
+-rw-r--r--   0        0        0     4109 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/imagenet/imagenet.py
+-rw-r--r--   0        0        0      673 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/imagenet/test.sh
+-rw-r--r--   0        0        0      393 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/README.md
+-rw-r--r--   0        0        0      620 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/jit_script_function.py
+-rw-r--r--   0        0        0      689 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/jit_script_method.py
+-rw-r--r--   0        0        0      675 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/jit_trace_function.py
+-rw-r--r--   0        0        0      817 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/jit_trace_method.py
+-rw-r--r--   0        0        0      432 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/test.sh
+-rw-r--r--   0        0        0     1679 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/lenet.py
+-rw-r--r--   0        0        0     3439 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/operators.py
+-rw-r--r--   0        0        0      791 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/simple.py
+-rw-r--r--   0        0        0     1587 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/user_annotation/README.md
+-rw-r--r--   0        0        0     5660 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/user_annotation/resnet.py
+-rw-r--r--   0        0        0      544 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/user_annotation/test.sh
+-rw-r--r--   0        0        0       69 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/nvtx/__init__.py
+-rw-r--r--   0        0        0      246 2022-04-06 23:54:24.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/nvtx/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     6180 2022-04-06 23:54:24.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/nvtx/__pycache__/nvmarker.cpython-37.pyc
+-rw-r--r--   0        0        0     6153 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/nvtx/nvmarker.py
+-rw-r--r--   0        0        0        0 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/__init__.py
+-rw-r--r--   0        0        0      250 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/__main__.py
+-rw-r--r--   0        0        0     1205 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/db.py
+-rw-r--r--   0        0        0     5286 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/kernel.py
+-rw-r--r--   0        0        0     8803 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/nvvp.py
+-rw-r--r--   0        0        0     2907 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/parse.py
+-rw-r--r--   0        0        0       25 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__init__.py
+-rw-r--r--   0        0        0      248 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__main__.py
+-rw-r--r--   0        0        0      213 2022-04-06 23:54:24.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2405 2022-04-06 23:54:32.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/activation.cpython-37.pyc
+-rw-r--r--   0        0        0     1503 2022-04-06 23:54:28.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0        0        0     9133 2022-04-06 23:54:28.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/blas.cpython-37.pyc
+-rw-r--r--   0        0        0     7166 2022-04-06 23:54:30.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/conv.cpython-37.pyc
+-rw-r--r--   0        0        0     2051 2022-04-06 23:54:28.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/convert.cpython-37.pyc
+-rw-r--r--   0        0        0     1584 2022-04-06 23:54:26.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/data.cpython-37.pyc
+-rw-r--r--   0        0        0     1768 2022-04-06 23:54:30.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/dropout.cpython-37.pyc
+-rw-r--r--   0        0        0     2005 2022-04-06 23:54:30.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/embedding.cpython-37.pyc
+-rw-r--r--   0        0        0    11970 2022-04-06 23:54:32.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/index_slice_join_mutate.cpython-37.pyc
+-rw-r--r--   0        0        0     4055 2022-04-06 23:54:32.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/linear.cpython-37.pyc
+-rw-r--r--   0        0        0     2659 2022-04-06 23:54:34.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/loss.cpython-37.pyc
+-rw-r--r--   0        0        0     7040 2022-04-06 23:54:34.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/misc.cpython-37.pyc
+-rw-r--r--   0        0        0     1878 2022-04-06 23:54:32.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/normalization.cpython-37.pyc
+-rw-r--r--   0        0        0     2079 2022-04-06 23:54:32.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/optim.cpython-37.pyc
+-rw-r--r--   0        0        0     3489 2022-04-06 23:54:28.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/output.cpython-37.pyc
+-rw-r--r--   0        0        0     5397 2022-04-06 23:54:28.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/pointwise.cpython-37.pyc
+-rw-r--r--   0        0        0     4507 2022-04-06 23:54:26.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/prof.cpython-37.pyc
+-rw-r--r--   0        0        0     1624 2022-04-06 23:54:32.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/randomSample.cpython-37.pyc
+-rw-r--r--   0        0        0     4512 2022-04-06 23:54:32.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/recurrentCell.cpython-37.pyc
+-rw-r--r--   0        0        0     4881 2022-04-06 23:54:30.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/reduction.cpython-37.pyc
+-rw-r--r--   0        0        0     3813 2022-04-06 23:54:32.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/softmax.cpython-37.pyc
+-rw-r--r--   0        0        0     2384 2022-04-06 23:54:28.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/usage.cpython-37.pyc
+-rw-r--r--   0        0        0     1860 2022-04-06 23:54:26.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/utility.cpython-37.pyc
+-rw-r--r--   0        0        0     1520 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/activation.py
+-rw-r--r--   0        0        0      742 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/base.py
+-rw-r--r--   0        0        0     6773 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/blas.py
+-rw-r--r--   0        0        0     6355 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/conv.py
+-rw-r--r--   0        0        0     1242 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/convert.py
+-rw-r--r--   0        0        0     1388 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/data.py
+-rw-r--r--   0        0        0      999 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/dropout.py
+-rw-r--r--   0        0        0     1409 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/embedding.py
+-rw-r--r--   0        0        0     8004 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/index_slice_join_mutate.py
+-rw-r--r--   0        0        0     4426 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/linear.py
+-rw-r--r--   0        0        0     1716 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/loss.py
+-rw-r--r--   0        0        0     3988 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/misc.py
+-rw-r--r--   0        0        0     1003 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/normalization.py
+-rw-r--r--   0        0        0     1472 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/optim.py
+-rw-r--r--   0        0        0     3665 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/output.py
+-rw-r--r--   0        0        0     5521 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/pointwise.py
+-rw-r--r--   0        0        0     1459 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/pooling.py
+-rw-r--r--   0        0        0     4967 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/prof.py
+-rw-r--r--   0        0        0      817 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/randomSample.py
+-rw-r--r--   0        0        0     4307 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/recurrentCell.py
+-rw-r--r--   0        0        0     2788 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/reduction.py
+-rw-r--r--   0        0        0     2190 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/softmax.py
+-rw-r--r--   0        0        0     2018 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/usage.py
+-rw-r--r--   0        0        0     1326 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/utility.py
+-rw-r--r--   0        0        0       22 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/reparameterization/README.md
+-rw-r--r--   0        0        0     5501 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/reparameterization/__init__.py
+-rw-r--r--   0        0        0     6442 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/reparameterization/reparameterization.py
+-rw-r--r--   0        0        0     3281 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/reparameterization/weight_norm.py
+-rw-r--r--   0        0        0     2775 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/README.md
+-rw-r--r--   0        0        0      577 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__init__.py
+-rw-r--r--   0        0        0      605 2022-04-06 23:54:34.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      930 2022-04-06 23:54:38.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/enums.cpython-37.pyc
+-rw-r--r--   0        0        0      757 2022-04-06 23:54:44.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/log_util.cpython-37.pyc
+-rw-r--r--   0        0        0     4745 2022-04-06 23:54:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/microbatches.cpython-37.pyc
+-rw-r--r--   0        0        0    12611 2022-04-06 23:54:36.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/parallel_state.cpython-37.pyc
+-rw-r--r--   0        0        0     1849 2022-04-06 23:54:36.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0        0        0      248 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/_data/__init__.py
+-rw-r--r--   0        0        0     7203 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/_data/_batchsampler.py
+-rw-r--r--   0        0        0       90 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/amp/__init__.py
+-rw-r--r--   0        0        0      262 2022-04-06 23:54:34.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/amp/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     3859 2022-04-06 23:54:34.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/amp/__pycache__/grad_scaler.cpython-37.pyc
+-rw-r--r--   0        0        0     4725 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/amp/grad_scaler.py
+-rw-r--r--   0        0        0      914 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/enums.py
+-rw-r--r--   0        0        0      120 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/functional/__init__.py
+-rw-r--r--   0        0        0      289 2022-04-06 23:54:36.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/functional/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     5531 2022-04-06 23:54:38.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/functional/__pycache__/fused_softmax.cpython-37.pyc
+-rw-r--r--   0        0        0     7443 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/functional/fused_softmax.py
+-rw-r--r--   0        0        0      415 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/log_util.py
+-rw-r--r--   0        0        0     6799 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/microbatches.py
+-rw-r--r--   0        0        0    19273 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/parallel_state.py
+-rw-r--r--   0        0        0      227 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/__init__.py
+-rw-r--r--   0        0        0      399 2022-04-06 23:54:38.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2750 2022-04-06 23:54:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/_timers.cpython-37.pyc
+-rw-r--r--   0        0        0     7754 2022-04-06 23:54:46.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/p2p_communication.cpython-37.pyc
+-rw-r--r--   0        0        0     9342 2022-04-06 23:54:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0        0        0     2538 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/_timers.py
+-rw-r--r--   0        0        0    15038 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/p2p_communication.py
+-rw-r--r--   0        0        0     1725 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__init__.py
+-rw-r--r--   0        0        0     1662 2022-04-06 23:54:40.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     9433 2022-04-06 23:54:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/common.cpython-37.pyc
+-rw-r--r--   0        0        0     3479 2022-04-06 23:54:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_no_pipelining.cpython-37.pyc
+-rw-r--r--   0        0        0     8204 2022-04-06 23:54:44.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_pipelining_with_interleaving.cpython-37.pyc
+-rw-r--r--   0        0        0     7603 2022-04-06 23:54:46.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_pipelining_without_interleaving.cpython-37.pyc
+-rw-r--r--   0        0        0    13017 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/common.py
+-rw-r--r--   0        0        0     4565 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_no_pipelining.py
+-rw-r--r--   0        0        0    16254 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_pipelining_with_interleaving.py
+-rw-r--r--   0        0        0    14989 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_pipelining_without_interleaving.py
+-rw-r--r--   0        0        0    12563 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/utils.py
+-rw-r--r--   0        0        0     2445 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__init__.py
+-rw-r--r--   0        0        0     1464 2022-04-06 23:54:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2421 2022-04-06 23:54:44.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/cross_entropy.cpython-37.pyc
+-rw-r--r--   0        0        0     2792 2022-04-06 23:54:44.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/data.cpython-37.pyc
+-rw-r--r--   0        0        0    12103 2022-04-06 23:54:46.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/layers.cpython-37.pyc
+-rw-r--r--   0        0        0     4887 2022-04-06 23:54:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/mappings.cpython-37.pyc
+-rw-r--r--   0        0        0     4541 2022-04-06 23:54:44.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/memory.cpython-37.pyc
+-rw-r--r--   0        0        0     8539 2022-04-06 23:54:44.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/random.cpython-37.pyc
+-rw-r--r--   0        0        0     1885 2022-04-06 23:54:44.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0        0        0     4720 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/cross_entropy.py
+-rw-r--r--   0        0        0     3957 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/data.py
+-rw-r--r--   0        0        0    18874 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/layers.py
+-rw-r--r--   0        0        0     4534 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/mappings.py
+-rw-r--r--   0        0        0     5108 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/memory.py
+-rw-r--r--   0        0        0    11491 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/random.py
+-rw-r--r--   0        0        0     2202 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/utils.py
+-rw-r--r--   0        0        0        0 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/__init__.py
+-rw-r--r--   0        0        0    41613 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/arguments.py
+-rw-r--r--   0        0        0     4864 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/commons.py
+-rw-r--r--   0        0        0     8862 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/global_vars.py
+-rw-r--r--   0        0        0     9001 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/standalone_bert.py
+-rw-r--r--   0        0        0    61609 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/standalone_gpt.py
+-rw-r--r--   0        0        0     1543 2022-02-12 21:46:42.000000 deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/utils.py
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.006634 deep_astro_uda-0.2.0/deep_astro_uda/client/__init__.py
+-rw-r--r--   0        0        0      544 2023-05-22 15:12:04.267152 deep_astro_uda-0.2.0/deep_astro_uda/client/astro_app.py
+-rw-r--r--   0        0        0     1554 2023-05-22 15:13:39.642649 deep_astro_uda-0.2.0/deep_astro_uda/client/commands/demo_command.py
+-rw-r--r--   0        0        0      228 2023-05-22 15:13:37.003588 deep_astro_uda-0.2.0/deep_astro_uda/client/commands/infer_command.py
+-rw-r--r--   0        0        0     3735 2023-05-22 15:13:30.415931 deep_astro_uda-0.2.0/deep_astro_uda/client/commands/run_command.py
+-rw-r--r--   0        0        0      746 2023-05-22 11:04:39.960250 deep_astro_uda-0.2.0/deep_astro_uda/client/options.py
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007013 deep_astro_uda-0.2.0/deep_astro_uda/configs/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-22 13:30:21.731901 deep_astro_uda-0.2.0/deep_astro_uda/configs/config.yaml
+-rw-r--r--   0        0        0     1996 2023-05-22 11:12:40.144312 deep_astro_uda-0.2.0/deep_astro_uda/configs/config_functions.py
+-rw-r--r--   0        0        0        0 2023-05-08 03:56:27.706969 deep_astro_uda-0.2.0/deep_astro_uda/data_utils/__init__.py
+-rw-r--r--   0        0        0     2908 2023-05-08 05:07:18.180392 deep_astro_uda-0.2.0/deep_astro_uda/data_utils/download_data.py
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007291 deep_astro_uda-0.2.0/deep_astro_uda/dist/__init__.py
+-rw-r--r--   0        0        0    10906 2023-05-07 23:05:47.007467 deep_astro_uda-0.2.0/deep_astro_uda/dist/deep_astro_uda-0.1.0.tar.gz
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.007637 deep_astro_uda-0.2.0/deep_astro_uda/model/__init__.py
+-rw-r--r--   0        0        0     6696 2023-05-22 12:36:09.942437 deep_astro_uda-0.2.0/deep_astro_uda/model/eval.py
+-rw-r--r--   0        0        0     5632 2023-05-07 23:05:47.007756 deep_astro_uda-0.2.0/deep_astro_uda/model/get_loader.py
+-rw-r--r--   0        0        0     4146 2023-05-07 23:05:47.007876 deep_astro_uda-0.2.0/deep_astro_uda/model/loss.py
+-rw-r--r--   0        0        0      465 2023-05-07 23:05:47.007980 deep_astro_uda-0.2.0/deep_astro_uda/model/lr_schedule.py
+-rw-r--r--   0        0        0     7913 2023-05-22 12:36:19.983415 deep_astro_uda-0.2.0/deep_astro_uda/model/train.py
+-rw-r--r--   0        0        0      459 2023-05-22 13:15:04.892342 deep_astro_uda-0.2.0/deep_astro_uda/settings.py
+-rw-r--r--   0        0        0     6468 2023-05-07 23:05:47.009742 deep_astro_uda-0.2.0/deep_astro_uda/tuner/tuner.py
+-rw-r--r--   0        0        0        1 2023-05-07 23:05:47.008275 deep_astro_uda-0.2.0/deep_astro_uda/utils/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-07 23:05:47.008398 deep_astro_uda-0.2.0/deep_astro_uda/utils/utils.py
+-rw-r--r--   0        0        0      379 2023-05-22 15:08:06.733339 deep_astro_uda-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16071 1970-01-01 00:00:00.000000 deep_astro_uda-0.2.0/PKG-INFO
```

### Comparing `deep_astro_uda-0.1.0/LICENSE` & `deep_astro_uda-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/README.md` & `deep_astro_uda-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/RNN/RNNBackend.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/RNN/RNNBackend.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/RNN/cells.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/RNN/cells.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/RNN/models.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/RNN/models.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/__init__.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/__pycache__/__init__.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/__pycache__/_autocast_utils.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/__pycache__/_autocast_utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/_autocast_utils.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/_autocast_utils.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/README.md` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/__init__.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/_amp_state.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/_amp_state.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/_initialize.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/_initialize.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/_process_optimizer.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/_process_optimizer.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/amp.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/amp.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/compat.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/compat.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/frontend.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/frontend.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/handle.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/handle.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/opt.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/opt.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/rnn_compat.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/rnn_compat.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/scaler.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/scaler.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/utils.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/__pycache__/wrap.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/__pycache__/wrap.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/_amp_state.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/_amp_state.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/_initialize.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/_initialize.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/_process_optimizer.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/_process_optimizer.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/amp.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/amp.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/compat.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/compat.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/frontend.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/frontend.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/handle.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/handle.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/__pycache__/functional_overrides.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/__pycache__/functional_overrides.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/__pycache__/tensor_overrides.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/__pycache__/tensor_overrides.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/__pycache__/torch_overrides.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/__pycache__/torch_overrides.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/functional_overrides.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/functional_overrides.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/tensor_overrides.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/tensor_overrides.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/lists/torch_overrides.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/lists/torch_overrides.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/opt.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/opt.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/rnn_compat.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/rnn_compat.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/scaler.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/scaler.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/utils.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/utils.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/amp/wrap.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/amp/wrap.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/bottleneck/bottleneck.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/bottleneck/bottleneck.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/bottleneck/bottleneck_module_test.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/bottleneck/bottleneck_module_test.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/bottleneck/test.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/bottleneck/test.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/bottleneck/bottleneck.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/bottleneck/bottleneck.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/fmha_api.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/fmha_api.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/gemm.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/gemm.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/gmem_tile.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/gmem_tile.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/kernel_traits.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/kernel_traits.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/mask.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/mask.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/smem_tile.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/smem_tile.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/softmax.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/softmax.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/utils.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha/utils.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_128_64_kernel.sm80.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_128_64_kernel.sm80.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_256_64_kernel.sm80.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_256_64_kernel.sm80.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_384_64_kernel.sm80.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_384_64_kernel.sm80.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_512_64_kernel.sm80.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_fp16_512_64_kernel.sm80.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_kernel_1xN_reload.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_kernel_1xN_reload.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_kernel_1xN_reload_nl.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_dgrad_kernel_1xN_reload_nl.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_128_64_kernel.sm80.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_128_64_kernel.sm80.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_256_64_kernel.sm80.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_256_64_kernel.sm80.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_384_64_kernel.sm80.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_384_64_kernel.sm80.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_512_64_kernel.sm80.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_fp16_512_64_kernel.sm80.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN_nl.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN_nl.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN_reload_v.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_fprop_kernel_1xN_reload_v.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_kernel.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_kernel.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_noloop_reduce.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_noloop_reduce.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_utils.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/fmha/src/fmha_utils.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm_add_relu.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm_add_relu.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm_add_relu.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/batch_norm_add_relu.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/interface.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/interface.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/ipc.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/ipc.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/groupbn/nhwc_batch_norm_kernel.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/groupbn/nhwc_batch_norm_kernel.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_api.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_api.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_bwd_kernels.cuh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_bwd_kernels.cuh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_bwd_semi_cuda_kernel.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_bwd_semi_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_fwd_cuda_kernel.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_fwd_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_fwd_kernels.cuh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_fwd_kernels.cuh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_kernel_traits.h` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_kernel_traits.h`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_utils.cuh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/layer_norm/ln_utils.cuh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/additive_masked_softmax_dropout_cuda.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/additive_masked_softmax_dropout_cuda.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/dropout.cuh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/dropout.cuh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/encdec_multihead_attn_cuda.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/encdec_multihead_attn_cuda.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/encdec_multihead_attn_norm_add_cuda.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/encdec_multihead_attn_norm_add_cuda.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/layer_norm.cuh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/layer_norm.cuh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/masked_softmax_dropout_cuda.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/masked_softmax_dropout_cuda.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/multihead_attn_frontend.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/multihead_attn_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/philox.cuh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/philox.cuh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_bias_additive_mask_cuda.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_bias_additive_mask_cuda.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_bias_cuda.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_bias_cuda.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_cuda.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_cuda.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_norm_add_cuda.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/self_multihead_attn_norm_add_cuda.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/softmax.cuh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/softmax.cuh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/strided_batched_gemm.cuh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/multihead_attn/strided_batched_gemm.cuh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_adam_cuda.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_adam_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_adam_cuda_kernel.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_adam_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_lamb_cuda.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_lamb_cuda_kernel.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_adam.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_adam.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_adam_kernel.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_adam_kernel.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_lamb.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_lamb.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_lamb_kernel.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/optimizers/multi_tensor_distopt_lamb_kernel.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_joint.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_joint.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_joint_kernel.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_joint_kernel.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_loss.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_loss.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_loss_kernel.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/transducer/transducer_loss_kernel.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/xentropy/interface.cpp` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/xentropy/interface.cpp`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/csrc/xentropy/xentropy_kernel.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/csrc/xentropy/xentropy_kernel.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/examples/multihead_attn/func_test_multihead_attn.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/examples/multihead_attn/func_test_multihead_attn.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/examples/multihead_attn/perf_test_multihead_attn.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/examples/multihead_attn/perf_test_multihead_attn.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/fmha/fmha.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/fmha/fmha.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/groupbn/batch_norm.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/groupbn/batch_norm.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/layer_norm/layer_norm.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/layer_norm/layer_norm.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/MHA_bwd.png` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/MHA_bwd.png`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/MHA_fwd.png` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/MHA_fwd.png`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/README.md` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/encdec_multihead_attn.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/encdec_multihead_attn.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/encdec_multihead_attn_func.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/encdec_multihead_attn_func.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/fast_encdec_multihead_attn_func.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/fast_encdec_multihead_attn_func.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/fast_encdec_multihead_attn_norm_add_func.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/fast_encdec_multihead_attn_norm_add_func.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/fast_self_multihead_attn_func.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/fast_self_multihead_attn_func.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/fast_self_multihead_attn_norm_add_func.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/fast_self_multihead_attn_norm_add_func.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/mask_softmax_dropout_func.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/mask_softmax_dropout_func.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/self_multihead_attn.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/self_multihead_attn.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/multihead_attn/self_multihead_attn_func.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/multihead_attn/self_multihead_attn_func.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fp16_optimizer.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fp16_optimizer.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fused_adam.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fused_adam.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fused_lamb.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/__pycache__/fused_lamb.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam_v2.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam_v2.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam_v3.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_adam_v3.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_lamb.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/distributed_fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/fp16_optimizer.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/fused_adam.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/fused_lamb.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/optimizers/fused_sgd.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/optimizers/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/README.md` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/asp.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/asp.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_lib.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_lib.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/CUDA_kernels/permutation_search_kernels.cu` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/CUDA_kernels/permutation_search_kernels.cu`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/call_permutation_search_kernels.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/call_permutation_search_kernels.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/exhaustive_search.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/exhaustive_search.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/permutation_utilities.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/permutation_search_kernels/permutation_utilities.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/sparse_masklib.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/sparse_masklib.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_part1.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_part1.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_part2.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_part2.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_reference.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/test/checkpointing_test_reference.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/sparsity/test/toy_problem.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/sparsity/test/toy_problem.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/fmha/test_fmha.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/fmha/test_fmha.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/fused_dense/test_fused_dense.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/fused_dense/test_fused_dense.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/layer_norm/test_fast_layer_norm.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/layer_norm/test_fast_layer_norm.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_encdec_multihead_attn.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_encdec_multihead_attn.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_encdec_multihead_attn_norm_add.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_encdec_multihead_attn_norm_add.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_fast_self_multihead_attn_bias.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_fast_self_multihead_attn_bias.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_mha_fused_softmax.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_mha_fused_softmax.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_self_multihead_attn.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_self_multihead_attn.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_self_multihead_attn_norm_add.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/multihead_attn/test_self_multihead_attn_norm_add.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/test_label_smoothing.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/test_label_smoothing.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/transducer/test_transducer_joint.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/transducer/test_transducer_joint.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/transducer/test_transducer_loss.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/transducer/test_transducer_loss.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/test/transducer/transducer_ref.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/test/transducer/transducer_ref.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/transducer/transducer.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/transducer/transducer.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/contrib/xentropy/softmax_xentropy.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/contrib/xentropy/softmax_xentropy.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/README.md` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/__pycache__/__init__.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/__pycache__/fp16_optimizer.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/__pycache__/fp16_optimizer.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/__pycache__/fp16util.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/__pycache__/fp16util.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/__pycache__/loss_scaler.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/__pycache__/loss_scaler.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/fp16_optimizer.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/fp16util.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/fp16util.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/fp16_utils/loss_scaler.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/fp16_utils/loss_scaler.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/fused_dense/fused_dense.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/fused_dense/fused_dense.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/mlp/mlp.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/multi_tensor_apply/__pycache__/multi_tensor_apply.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/multi_tensor_apply/__pycache__/multi_tensor_apply.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/multi_tensor_apply/multi_tensor_apply.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/normalization/__pycache__/fused_layer_norm.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/normalization/__pycache__/fused_layer_norm.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/normalization/fused_layer_norm.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/normalization/fused_layer_norm.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_adagrad.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_adagrad.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_adam.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_adam.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_lamb.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_lamb.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_mixed_precision_lamb.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_mixed_precision_lamb.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_novograd.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_novograd.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/__pycache__/fused_sgd.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/__pycache__/fused_sgd.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_adagrad.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_adagrad.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_adam.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_lamb.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_mixed_precision_lamb.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_mixed_precision_lamb.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_novograd.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_novograd.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/optimizers/fused_sgd.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/optimizers/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/LARC.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/LARC.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/README.md` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__init__.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/LARC.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/LARC.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/__init__.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/distributed.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/distributed.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/sync_batchnorm.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/sync_batchnorm.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/__pycache__/sync_batchnorm_kernel.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/__pycache__/sync_batchnorm_kernel.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/distributed.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/multiproc.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/multiproc.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/optimized_sync_batchnorm.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/optimized_sync_batchnorm.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/optimized_sync_batchnorm_kernel.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/optimized_sync_batchnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/sync_batchnorm.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/sync_batchnorm.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/parallel/sync_batchnorm_kernel.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/parallel/sync_batchnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/FAQs.md` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/FAQs.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/README.md` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/apex/fused_adam.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/apex/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/apex/fused_layer_norm.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/apex/fused_layer_norm.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/custom_function.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/custom_function.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/custom_module.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/custom_func_module/custom_module.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/imagenet/imagenet.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/imagenet/imagenet.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/imagenet/test.sh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/imagenet/test.sh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/jit_script_function.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/jit_script_function.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/jit_script_method.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/jit_script_method.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/jit_trace_function.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/jit_trace_function.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/jit/jit_trace_method.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/jit/jit_trace_method.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/lenet.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/lenet.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/operators.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/operators.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/simple.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/simple.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/user_annotation/README.md` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/user_annotation/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/user_annotation/resnet.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/user_annotation/resnet.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/examples/user_annotation/test.sh` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/examples/user_annotation/test.sh`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/nvtx/__pycache__/nvmarker.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/nvtx/__pycache__/nvmarker.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/nvtx/nvmarker.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/nvtx/nvmarker.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/db.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/db.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/kernel.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/kernel.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/nvvp.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/nvvp.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/parse/parse.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/parse/parse.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/activation.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/activation.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/base.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/blas.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/blas.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/conv.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/conv.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/convert.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/convert.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/data.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/data.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/dropout.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/dropout.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/embedding.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/embedding.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/index_slice_join_mutate.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/index_slice_join_mutate.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/linear.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/linear.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/loss.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/loss.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/misc.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/misc.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/normalization.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/normalization.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/optim.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/optim.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/output.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/output.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/pointwise.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/pointwise.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/prof.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/prof.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/randomSample.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/randomSample.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/recurrentCell.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/recurrentCell.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/reduction.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/reduction.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/softmax.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/softmax.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/usage.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/usage.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/__pycache__/utility.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/__pycache__/utility.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/activation.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/activation.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/base.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/base.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/blas.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/blas.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/conv.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/conv.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/convert.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/convert.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/data.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/data.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/dropout.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/dropout.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/embedding.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/embedding.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/index_slice_join_mutate.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/index_slice_join_mutate.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/linear.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/linear.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/loss.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/loss.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/misc.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/misc.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/normalization.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/normalization.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/optim.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/optim.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/output.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/output.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/pointwise.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/pointwise.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/pooling.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/pooling.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/prof.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/prof.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/randomSample.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/randomSample.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/recurrentCell.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/recurrentCell.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/reduction.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/reduction.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/softmax.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/softmax.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/usage.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/usage.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/pyprof/prof/utility.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/pyprof/prof/utility.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/reparameterization/__init__.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/reparameterization/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/reparameterization/reparameterization.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/reparameterization/reparameterization.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/reparameterization/weight_norm.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/reparameterization/weight_norm.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/README.md` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/README.md`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__init__.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/__init__.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/enums.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/enums.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/log_util.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/log_util.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/microbatches.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/microbatches.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/parallel_state.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/parallel_state.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/__pycache__/utils.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/_data/_batchsampler.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/_data/_batchsampler.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/amp/__pycache__/grad_scaler.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/amp/__pycache__/grad_scaler.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/amp/grad_scaler.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/amp/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/enums.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/enums.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/functional/__pycache__/fused_softmax.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/functional/__pycache__/fused_softmax.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/functional/fused_softmax.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/functional/fused_softmax.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/microbatches.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/microbatches.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/parallel_state.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/parallel_state.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/_timers.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/_timers.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/p2p_communication.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/p2p_communication.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/utils.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/_timers.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/_timers.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/p2p_communication.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/p2p_communication.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__init__.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/__init__.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/common.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/common.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_no_pipelining.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_no_pipelining.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_pipelining_with_interleaving.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_pipelining_with_interleaving.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_pipelining_without_interleaving.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/__pycache__/fwd_bwd_pipelining_without_interleaving.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/common.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/common.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_no_pipelining.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_no_pipelining.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_pipelining_with_interleaving.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_pipelining_with_interleaving.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_pipelining_without_interleaving.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/schedules/fwd_bwd_pipelining_without_interleaving.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/pipeline_parallel/utils.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/pipeline_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__init__.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/__init__.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/cross_entropy.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/cross_entropy.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/data.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/data.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/layers.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/layers.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/mappings.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/mappings.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/memory.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/memory.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/random.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/random.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/utils.cpython-37.pyc` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/cross_entropy.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/data.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/data.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/layers.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/layers.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/mappings.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/mappings.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/memory.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/memory.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/random.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/random.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/tensor_parallel/utils.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/arguments.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/arguments.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/commons.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/commons.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/global_vars.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/global_vars.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/standalone_bert.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/standalone_bert.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/testing/standalone_gpt.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/testing/standalone_gpt.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/apex/transformer/utils.py` & `deep_astro_uda-0.2.0/deep_astro_uda/apex/transformer/utils.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/client/astro_app.py` & `deep_astro_uda-0.2.0/deep_astro_uda/client/astro_app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from cleo import Application
-#from commands.commands import DeepDanceRun
+from cleo.application import Application
 
 import sys
 
 from deep_astro_uda.client.commands.demo_command import DemoCommand
 from deep_astro_uda.client.commands.run_command import RunCommand
 from deep_astro_uda.client.commands.infer_command import InferCommand
```

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/client/commands/demo_command.py` & `deep_astro_uda-0.2.0/deep_astro_uda/client/commands/demo_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from cleo import option
-from cleo import Command
+from cleo.commands.command import Command
 from deep_astro_uda.model.train import train
 from deep_astro_uda.settings import DEFAULT_CONFIG_PATH
 from deep_astro_uda.client.options import config_path
 from deep_astro_uda.configs.config_functions import ConfigParser
 from deep_astro_uda.data_utils.download_data import Downloader
 
 # TODO: Add docstrings.
```

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/client/commands/run_command.py` & `deep_astro_uda-0.2.0/deep_astro_uda/client/commands/run_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cleo import Command
+from cleo.commands.command import Command
 from deep_astro_uda.client.options import full_options
 from deep_astro_uda.configs.config_functions import ConfigParser
 from deep_astro_uda.data_utils.download_data import Downloader
 from deep_astro_uda.settings import DATASET_NAMES, DEFAULT_CONFIG_PATH
 import os
 import shutil 
 from deep_astro_uda.model.train import train
```

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/client/options.py` & `deep_astro_uda-0.2.0/deep_astro_uda/client/options.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/configs/config.yaml` & `deep_astro_uda-0.2.0/deep_astro_uda/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/configs/config_functions.py` & `deep_astro_uda-0.2.0/deep_astro_uda/configs/config_functions.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/data_utils/download_data.py` & `deep_astro_uda-0.2.0/deep_astro_uda/data_utils/download_data.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/dist/deep_astro_uda-0.1.0.tar.gz` & `deep_astro_uda-0.2.0/deep_astro_uda/dist/deep_astro_uda-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/model/eval.py` & `deep_astro_uda-0.2.0/deep_astro_uda/model/eval.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/model/get_loader.py` & `deep_astro_uda-0.2.0/deep_astro_uda/model/get_loader.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/model/loss.py` & `deep_astro_uda-0.2.0/deep_astro_uda/model/loss.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/model/train.py` & `deep_astro_uda-0.2.0/deep_astro_uda/model/train.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/tuner/tuner.py` & `deep_astro_uda-0.2.0/deep_astro_uda/tuner/tuner.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/deep_astro_uda/utils/utils.py` & `deep_astro_uda-0.2.0/deep_astro_uda/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deep_astro_uda-0.1.0/PKG-INFO` & `deep_astro_uda-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-astro-uda
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Ashia Lewis
 Author-email: pantagruelspendulum@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

