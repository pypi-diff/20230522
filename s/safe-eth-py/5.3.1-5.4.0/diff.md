# Comparing `tmp/safe-eth-py-5.3.1.tar.gz` & `tmp/safe-eth-py-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-eth-py-5.3.1.tar", last modified: Wed May  3 08:27:00 2023, max compression
+gzip compressed data, was "safe-eth-py-5.4.0.tar", last modified: Mon May 22 11:05:12 2023, max compression
```

## Comparing `safe-eth-py-5.3.1.tar` & `safe-eth-py-5.4.0.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.837375 safe-eth-py-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-03 08:27:00.837375 safe-eth-py-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.797374 safe-eth-py-5.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.801374 safe-eth-py-5.3.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/gnosis.eth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/gnosis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/gnosis.safe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.801374 safe-eth-py-5.3.1/gnosis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.801374 safe-eth-py-5.3.1/gnosis/eth/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.801374 safe-eth-py-5.3.1/gnosis/eth/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/abis/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.801374 safe-eth-py-5.3.1/gnosis/eth/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/clients/sourcify.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.813374 safe-eth-py-5.3.1/gnosis/eth/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/CPKFactory.json
--rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/DelegateConstructorProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/ERC1155.json
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/ERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/ERC20TestToken.json
--rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/ERC721.json
--rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
--rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/MultiSend.json
--rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/PayingProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/kyber_network_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_pair.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_router.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.813374 safe-eth-py-5.3.1/gnosis/eth/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.817374 safe-eth-py-5.3.1/gnosis/eth/django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/django/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.817374 safe-eth-py-5.3.1/gnosis/eth/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77421 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/ethereum_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.817374 safe-eth-py-5.3.1/gnosis/eth/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.821375 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.821375 safe-eth-py-5.3.1/gnosis/eth/oracles/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)    32144 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.821375 safe-eth-py-5.3.1/gnosis/eth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.825374 safe-eth-py-5.3.1/gnosis/eth/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_sourcify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.825374 safe-eth-py-5.3.1/gnosis/eth/tests/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.825374 safe-eth-py-5.3.1/gnosis/eth/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)   793149 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)   171076 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.829374 safe-eth-py-5.3.1/gnosis/eth/tests/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    61046 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/eth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.829374 safe-eth-py-5.3.1/gnosis/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/protocol/gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/protocol/order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.829374 safe-eth-py-5.3.1/gnosis/protocol/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/protocol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/protocol/tests/test_gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.833374 safe-eth-py-5.3.1/gnosis/safe/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24396 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.833374 safe-eth-py-5.3.1/gnosis/safe/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/api/base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/api/relay_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/api/transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    41997 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.837375 safe-eth-py-5.3.1/gnosis/safe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.837375 safe-eth-py-5.3.1/gnosis/safe/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/test_multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/test_proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    32608 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.837375 safe-eth-py-5.3.1/gnosis/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/gnosis/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:27:00.837375 safe-eth-py-5.3.1/safe_eth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-03 08:27:00.000000 safe-eth-py-5.3.1/safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-05-03 08:27:00.000000 safe-eth-py-5.3.1/safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:27:00.000000 safe-eth-py-5.3.1/safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-03 08:27:00.000000 safe-eth-py-5.3.1/safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 08:27:00.000000 safe-eth-py-5.3.1/safe_eth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-03 08:27:00.841374 safe-eth-py-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-03 08:26:42.000000 safe-eth-py-5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.097002 safe-eth-py-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-22 11:05:12.097002 safe-eth-py-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.061002 safe-eth-py-5.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.061002 safe-eth-py-5.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/gnosis.eth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/gnosis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/gnosis.safe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.061002 safe-eth-py-5.4.0/gnosis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.065002 safe-eth-py-5.4.0/gnosis/eth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.065002 safe-eth-py-5.4.0/gnosis/eth/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/abis/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.065002 safe-eth-py-5.4.0/gnosis/eth/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/clients/sourcify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.073002 safe-eth-py-5.4.0/gnosis/eth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/CPKFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/DelegateConstructorProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/ERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/ERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/ERC20TestToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/ERC721.json
+-rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/MultiSend.json
+-rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/PayingProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/Proxy_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/Proxy_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/Proxy_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/kyber_network_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_v2_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_v2_pair.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_v2_router.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.077002 safe-eth-py-5.4.0/gnosis/eth/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.077002 safe-eth-py-5.4.0/gnosis/eth/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/django/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.077002 safe-eth-py-5.4.0/gnosis/eth/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77427 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.077002 safe-eth-py-5.4.0/gnosis/eth/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.081002 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.081002 safe-eth-py-5.4.0/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32144 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.081002 safe-eth-py-5.4.0/gnosis/eth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.085002 safe-eth-py-5.4.0/gnosis/eth/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/clients/test_sourcify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.085002 safe-eth-py-5.4.0/gnosis/eth/tests/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.085002 safe-eth-py-5.4.0/gnosis/eth/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   793149 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171076 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.085002 safe-eth-py-5.4.0/gnosis/eth/tests/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61046 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/eth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.089002 safe-eth-py-5.4.0/gnosis/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/protocol/gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/protocol/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.089002 safe-eth-py-5.4.0/gnosis/protocol/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/protocol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/protocol/tests/test_gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.089002 safe-eth-py-5.4.0/gnosis/safe/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.089002 safe-eth-py-5.4.0/gnosis/safe/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/api/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/api/relay_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41997 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.093002 safe-eth-py-5.4.0/gnosis/safe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.093002 safe-eth-py-5.4.0/gnosis/safe/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/test_multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/test_proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32608 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/test_safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.093002 safe-eth-py-5.4.0/gnosis/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/gnosis/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:05:12.093002 safe-eth-py-5.4.0/safe_eth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-22 11:05:12.000000 safe-eth-py-5.4.0/safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-05-22 11:05:12.000000 safe-eth-py-5.4.0/safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:05:12.000000 safe-eth-py-5.4.0/safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-22 11:05:12.000000 safe-eth-py-5.4.0/safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 11:05:12.000000 safe-eth-py-5.4.0/safe_eth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-22 11:05:12.097002 safe-eth-py-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 11:04:56.000000 safe-eth-py-5.4.0/setup.py
```

### Comparing `safe-eth-py-5.3.1/LICENSE` & `safe-eth-py-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/PKG-INFO` & `safe-eth-py-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 5.3.1
+Version: 5.4.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-5.3.1/README.rst` & `safe-eth-py-5.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/Makefile` & `safe-eth-py-5.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/make.bat` & `safe-eth-py-5.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/source/conf.py` & `safe-eth-py-5.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/source/gnosis.eth.clients.rst` & `safe-eth-py-5.4.0/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/source/gnosis.eth.django.rst` & `safe-eth-py-5.4.0/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/source/gnosis.eth.oracles.abis.rst` & `safe-eth-py-5.4.0/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/source/gnosis.eth.rst` & `safe-eth-py-5.4.0/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/source/gnosis.safe.rst` & `safe-eth-py-5.4.0/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/source/index.rst` & `safe-eth-py-5.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/docs/source/quickstart.rst` & `safe-eth-py-5.4.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/__init__.py` & `safe-eth-py-5.4.0/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/abis/multicall.py` & `safe-eth-py-5.4.0/gnosis/eth/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/clients/__init__.py` & `safe-eth-py-5.4.0/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/clients/blockscout_client.py` & `safe-eth-py-5.4.0/gnosis/eth/clients/blockscout_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         EthereumNetwork.RABBIT_ANALOG_TESTNET_CHAIN: "https://rabbit.analogscan.com",
         EthereumNetwork.KCC_MAINNET: "https://scan.kcc.io/",
         EthereumNetwork.KCC_TESTNET: "https://scan-testnet.kcc.network/",
         EthereumNetwork.ARBITRUM_ONE: "https://explorer.arbitrum.io",
         EthereumNetwork.ARBITRUM_NOVA: "https://nova-explorer.arbitrum.io",
         EthereumNetwork.ARBITRUM_GOERLI: "https://goerli-rollup-explorer.arbitrum.io",
         EthereumNetwork.CROSSBELL: "https://scan.crossbell.io",
+        EthereumNetwork.ETHEREUM_CLASSIC_MAINNET: "https://blockscout.com/etc/mainnet/",
+        EthereumNetwork.ETHEREUM_CLASSIC_TESTNET_MORDOR: "https://blockscout.com/etc/mordor/",
     }
 
     def __init__(self, network: EthereumNetwork):
         self.network = network
         self.base_url = self.NETWORK_WITH_URL.get(network)
         if self.base_url is None:
             raise BlockScoutConfigurationProblem(
```

### Comparing `safe-eth-py-5.3.1/gnosis/eth/clients/etherscan_client.py` & `safe-eth-py-5.4.0/gnosis/eth/clients/etherscan_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         EthereumNetwork.MOONRIVER: "https://moonriver.moonscan.io",
         EthereumNetwork.MOONBASE_ALPHA: "https://moonbase.moonscan.io",
         EthereumNetwork.CRONOS_MAINNET_BETA: "https://cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://testnet.cronoscan.com",
         EthereumNetwork.CELO_MAINNET: "https://celoscan.io",
         EthereumNetwork.BASE_GOERLI_TESTNET: "https://goerli.basescan.org",
         EthereumNetwork.NEON_EVM_DEVNET: "https://neonscan.org",
+        EthereumNetwork.SEPOLIA: "https://sepolia.etherscan.io",
     }
 
     NETWORK_WITH_API_URL = {
         EthereumNetwork.MAINNET: "https://api.etherscan.io",
         EthereumNetwork.RINKEBY: "https://api-rinkeby.etherscan.io",
         EthereumNetwork.ROPSTEN: "https://api-ropsten.etherscan.io",
         EthereumNetwork.GOERLI: "https://api-goerli.etherscan.io",
@@ -64,14 +65,15 @@
         EthereumNetwork.MOONRIVER: "https://api-moonriver.moonscan.io",
         EthereumNetwork.MOONBASE_ALPHA: "https://api-moonbase.moonscan.io",
         EthereumNetwork.CRONOS_MAINNET_BETA: "https://api.cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://api-testnet.cronoscan.com",
         EthereumNetwork.CELO_MAINNET: "https://api.celoscan.io",
         EthereumNetwork.BASE_GOERLI_TESTNET: "https://api-goerli.basescan.org",
         EthereumNetwork.NEON_EVM_DEVNET: "https://devnet-api.neonscan.org",
+        EthereumNetwork.SEPOLIA: "https://api-sepolia.etherscan.io",
     }
     HTTP_HEADERS = {
         "User-Agent": "curl/7.77.0",
     }
 
     def __init__(self, network: EthereumNetwork, api_key: Optional[str] = None):
         self.network = network
```

### Comparing `safe-eth-py-5.3.1/gnosis/eth/clients/sourcify.py` & `safe-eth-py-5.4.0/gnosis/eth/clients/sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/constants.py` & `safe-eth-py-5.4.0/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/CPKFactory.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/DelegateConstructorProxy.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/ERC1155.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/ERC1155.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/ERC20.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/ERC20.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/ERC20TestToken.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/ERC721.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/ERC721.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V0_0_1.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_0_0.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_1_1.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_3_0.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/MultiSend.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/MultiSend.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/PayingProxy.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_0_0.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_1_1.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_3_0.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_0_0.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_1_1.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_3_0.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/__init__.py` & `safe-eth-py-5.4.0/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/kyber_network_proxy.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_exchange.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_factory.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_factory.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_pair.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_router.json` & `safe-eth-py-5.4.0/gnosis/eth/contracts/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/django/admin.py` & `safe-eth-py-5.4.0/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/django/forms.py` & `safe-eth-py-5.4.0/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/django/models.py` & `safe-eth-py-5.4.0/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/django/serializers.py` & `safe-eth-py-5.4.0/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/django/tests/models.py` & `safe-eth-py-5.4.0/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/django/tests/test_forms.py` & `safe-eth-py-5.4.0/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/django/tests/test_models.py` & `safe-eth-py-5.4.0/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/django/tests/test_serializers.py` & `safe-eth-py-5.4.0/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/eip712/__init__.py` & `safe-eth-py-5.4.0/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/ethereum_client.py` & `safe-eth-py-5.4.0/gnosis/eth/ethereum_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1329,15 +1329,15 @@
         contract_functions: Iterable[ContractFunction],
         from_address: Optional[ChecksumAddress] = None,
         raise_exception: bool = True,
         force_batch_call: bool = False,
         block_identifier: Optional[BlockIdentifier] = "latest",
     ) -> List[Optional[Union[bytes, Any]]]:
         """
-        Call multiple functions. Multicall contract by MakerDAO will be used by default if available
+        Call multiple functions. ``Multicall`` contract by MakerDAO will be used by default if available
 
         :param contract_functions:
         :param from_address: Only available when ``Multicall`` is not used
         :param raise_exception: If ``True``, raise ``BatchCallException`` if one of the calls fails
         :param force_batch_call: If ``True``, ignore multicall and always use batch calls to get the
             result (less optimal). If ``False``, more optimal way will be tried.
         :param block_identifier:
@@ -1368,15 +1368,15 @@
         contract_addresses: Sequence[ChecksumAddress],
         from_address: Optional[ChecksumAddress] = None,
         raise_exception: bool = True,
         force_batch_call: bool = False,
         block_identifier: Optional[BlockIdentifier] = "latest",
     ) -> List[Optional[Union[bytes, Any]]]:
         """
-        Call the same function in multiple contracts. Way more optimal than using `batch_call` generating multiple
+        Call the same function in multiple contracts. Way more optimal than using ``batch_call`` generating multiple
         ``ContractFunction`` objects.
 
         :param contract_function:
         :param contract_addresses:
         :param from_address: Only available when ``Multicall`` is not used
         :param raise_exception: If ``True``, raise ``BatchCallException`` if one of the calls fails
         :param force_batch_call: If ``True``, ignore multicall and always use batch calls to get the
```

### Comparing `safe-eth-py-5.3.1/gnosis/eth/ethereum_network.py` & `safe-eth-py-5.4.0/gnosis/eth/ethereum_network.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/exceptions.py` & `safe-eth-py-5.4.0/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/multicall.py` & `safe-eth-py-5.4.0/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/__init__.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/abis/aave_abis.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/abis/balancer_abis.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/abis/cream_abis.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/abis/curve_abis.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/abis/mooniswap_abis.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/abis/uniswap_v3.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/abis/yearn_abis.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/abis/zerion_abis.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/cowswap.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/kyber.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/oracles.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/superfluid.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/sushiswap.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/uniswap_v3.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/oracles/utils.py` & `safe-eth-py-5.4.0/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/clients/mocks.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_blockscout_client.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_etherscan_client.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_sourcify.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/clients/test_sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/eip712/test_eip712.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/ethereum_test_case.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_internal_txs.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_log_receipts.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_block.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         ),
         "transactionPosition": 2,
         "type": "call",
     },
     {
         "action": {
             "value": 5000000000000000000,
-            "author": "0x52bc44d5378309ee2abf1539bf71de1b7d7be3b5",
+            "author": "0x52bc44d5378309EE2abF1539BF71dE1b7d7bE3b5",
             "rewardType": "block",
         },
         "blockHash": HexBytes(
             "0x4169fc8dfb9ece41c90044ebc9b8e2daed9f5e08c0ba3746e337732aa48b3bc3"
         ),
         "blockNumber": 2191709,
         "result": None,
@@ -2966,15 +2966,15 @@
             "0x73c429f04ca56cd06ec53cfdaf845faf6f284e368eeeb310b1b7b825fa70a6db"
         ),
         "transactionPosition": 44,
         "type": "call",
     },
     {
         "action": {
-            "author": "0x5a0b54d5dc17e0aadc383d2db43b0a0d3e029c4c",
+            "author": "0x5A0b54D5dc17e0AadC383d2db43B0a0D3E029c4c",
             "rewardType": "block",
             "value": 2000000000000000000,
         },
         "blockHash": HexBytes(
             "0x8f9809f6012f85803956a419e2e54914dfdebba33e4f7a0d1574b12e92499c0e"
         ),
         "blockNumber": 13191781,
@@ -16321,15 +16321,15 @@
             "0x3894b0d1325a8a91171a2e0a58394287066fef3174945e4ff56eacfc0e4bda58"
         ),
         "transactionPosition": 124,
         "type": "call",
     },
     {
         "action": {
-            "author": "0xdafea492d9c6733ae3d56b7ed1adb60692c98bc5",
+            "author": "0xDAFEA492D9c6733ae3d56b7Ed1ADB60692c98Bc5",
             "rewardType": "block",
             "value": 0,
         },
         "blockHash": HexBytes(
             "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
         ),
         "blockNumber": 15630274,
```

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_filter.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_cowswap.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_kyber.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_superfluid.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_sushiswap.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/test_ethereum_client.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/test_multicall.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/test_oracles.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/test_utils.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/tests/utils.py` & `safe-eth-py-5.4.0/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/eth/utils.py` & `safe-eth-py-5.4.0/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/protocol/gnosis_protocol_api.py` & `safe-eth-py-5.4.0/gnosis/protocol/gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/protocol/order.py` & `safe-eth-py-5.4.0/gnosis/protocol/order.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/protocol/tests/test_gnosis_protocol_api.py` & `safe-eth-py-5.4.0/gnosis/protocol/tests/test_gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/__init__.py` & `safe-eth-py-5.4.0/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/addresses.py` & `safe-eth-py-5.4.0/gnosis/safe/addresses.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 """
 from typing import Dict, List, Tuple
 
 from gnosis.eth import EthereumNetwork
 
 MASTER_COPIES: Dict[EthereumNetwork, List[Tuple[str, int, str]]] = {
     EthereumNetwork.MAINNET: [
-        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 12504423, "1.3.0+L2"),
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            14981217,
+            "1.3.0+L2",
+        ),  # safe singleton address
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            12504423,
+            "1.3.0+L2",
+        ),  # default singleton address
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 12504268, "1.3.0"),
         ("0x6851D6fDFAfD08c0295C392436245E5bc78B0185", 10329734, "1.2.0"),
         ("0x34CfAC646f301356fAa8B21e94227e3583Fe3F5F", 9084503, "1.1.1"),
         ("0xaE32496491b53841efb51829d6f886387708F99B", 8915728, "1.1.0"),
         ("0xb6029EA3B2c51D09a50B53CA8012FeEB05bDa35A", 7457553, "1.0.0"),
         ("0x8942595A2dC5181Df0465AF0D7be08c8f23C93af", 6766257, "0.1.0"),
         ("0xAC6072986E985aaBE7804695EC2d8970Cf7541A2", 6569433, "0.0.2"),
@@ -25,16 +34,34 @@
         ("0x34CfAC646f301356fAa8B21e94227e3583Fe3F5F", 5590754, "1.1.1"),
         ("0xaE32496491b53841efb51829d6f886387708F99B", 5423491, "1.1.0"),
         ("0xb6029EA3B2c51D09a50B53CA8012FeEB05bDa35A", 4110083, "1.0.0"),
         ("0x8942595A2dC5181Df0465AF0D7be08c8f23C93af", 3392692, "0.1.0"),
         ("0x2727D69C0BD14B1dDd28371B8D97e808aDc1C2f7", 3055781, "0.0.2"),
     ],
     EthereumNetwork.GOERLI: [
-        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 4854168, "1.3.0+L2"),
-        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 4854169, "1.3.0"),
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            6900544,
+            "1.3.0+L2",
+        ),  # safe singleton address
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            4854168,
+            "1.3.0+L2",
+        ),  # default singleton address
+        (
+            "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
+            6900547,
+            "1.3.0",
+        ),  # safe singleton address
+        (
+            "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
+            4854169,
+            "1.3.0",
+        ),  # default singleton address
         ("0x6851D6fDFAfD08c0295C392436245E5bc78B0185", 2930373, "1.2.0"),
         ("0x34CfAC646f301356fAa8B21e94227e3583Fe3F5F", 1798663, "1.1.1"),
         ("0xaE32496491b53841efb51829d6f886387708F99B", 1631488, "1.1.0"),
         ("0xb6029EA3B2c51D09a50B53CA8012FeEB05bDa35A", 319108, "1.0.0"),
         ("0x8942595A2dC5181Df0465AF0D7be08c8f23C93af", 34096, "0.1.0"),
     ],
     EthereumNetwork.KOVAN: [
@@ -43,16 +70,34 @@
         ("0x6851D6fDFAfD08c0295C392436245E5bc78B0185", 19242615, "1.2.0"),
         ("0x34CfAC646f301356fAa8B21e94227e3583Fe3F5F", 15366145, "1.1.1"),
         ("0xaE32496491b53841efb51829d6f886387708F99B", 14740724, "1.1.0"),
         ("0xb6029EA3B2c51D09a50B53CA8012FeEB05bDa35A", 10638132, "1.0.0"),
         ("0x8942595A2dC5181Df0465AF0D7be08c8f23C93af", 9465686, "0.1.0"),
     ],
     EthereumNetwork.GNOSIS: [
-        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 16236936, "1.3.0+L2"),
-        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 16236998, "1.3.0"),
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            27679972,
+            "1.3.0+L2",
+        ),  # safe singleton address
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            16236936,
+            "1.3.0+L2",
+        ),  # default singleton address
+        (
+            "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
+            27679975,
+            "1.3.0",
+        ),  # safe singleton address
+        (
+            "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
+            16236998,
+            "1.3.0",
+        ),  # default singleton address
         ("0x6851D6fDFAfD08c0295C392436245E5bc78B0185", 10612049, "1.2.0"),
         ("0x34CfAC646f301356fAa8B21e94227e3583Fe3F5F", 10045292, "1.1.1"),
         ("0x2CB0ebc503dE87CFD8f0eCEED8197bF7850184ae", 12529466, "1.1.1+Circles"),
         ("0xb6029EA3B2c51D09a50B53CA8012FeEB05bDa35A", 19560130, "1.0.0"),
     ],
     EthereumNetwork.ENERGY_WEB_CHAIN: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 12028662, "1.3.0+L2"),
@@ -63,27 +108,45 @@
     EthereumNetwork.ENERGY_WEB_VOLTA_TESTNET: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 11942450, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 11942451, "1.3.0"),
         ("0x6851D6fDFAfD08c0295C392436245E5bc78B0185", 6876086, "1.2.0"),
         ("0x34CfAC646f301356fAa8B21e94227e3583Fe3F5F", 6876642, "1.1.1"),
     ],
     EthereumNetwork.POLYGON: [
-        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 14306478, "1.3.0+L2"),
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            34516629,
+            "1.3.0+L2",
+        ),  # safe singleton address
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            14306478,
+            "1.3.0+L2",
+        ),  # default singleton address
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 14306478, "1.3.0"),
     ],
     EthereumNetwork.POLYGON_ZKEVM: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 79000, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 79000, "1.3.0"),
     ],
     EthereumNetwork.MUMBAI: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 13736914, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 13736914, "1.3.0"),
     ],
     EthereumNetwork.ARBITRUM_ONE: [
-        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 1146, "1.3.0+L2"),
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            88610931,
+            "1.3.0+L2",
+        ),  # safe singleton address
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            1146,
+            "1.3.0+L2",
+        ),  # default singleton address
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 1140, "1.3.0"),
     ],
     EthereumNetwork.ARBITRUM_NOVA: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 426, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 427, "1.3.0"),
     ],
     EthereumNetwork.ARBITRUM_RINKEBY: [
@@ -91,24 +154,57 @@
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 57070, "1.3.0"),
     ],
     EthereumNetwork.ARBITRUM_GOERLI: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 11545, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 11546, "1.3.0"),
     ],
     EthereumNetwork.BINANCE_SMART_CHAIN_MAINNET: [
-        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 8485899, "1.3.0+L2"),
-        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 8485903, "1.3.0"),
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            28092011,
+            "1.3.0+L2",
+        ),  # safe singleton address
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            8485899,
+            "1.3.0+L2",
+        ),  # default singleton address
+        (
+            "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
+            28092014,
+            "1.3.0",
+        ),  # safe singleton address
+        (
+            "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
+            8485903,
+            "1.3.0",
+        ),  # default singleton address
     ],
     EthereumNetwork.CELO_MAINNET: [
         ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 8944350, "1.3.0+L2"),
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 8944351, "1.3.0"),
     ],
     EthereumNetwork.AVALANCHE_C_CHAIN: [
-        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 4_949_507, "1.3.0+L2"),
-        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 4_949_512, "1.3.0"),
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            22_123_383,
+            "1.3.0+L2",
+        )(  # default singleton address
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 4_949_507, "1.3.0+L2"
+        ),  # safe singleton address
+        (
+            "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
+            14_747_111,
+            "1.3.0",
+        ),  # default singleton address
+        (
+            "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
+            4_949_512,
+            "1.3.0",
+        ),  # safe singleton address
     ],
     EthereumNetwork.MOONBEAM: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 172_092, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 172_094, "1.3.0"),
     ],
     EthereumNetwork.MOONRIVER: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 707_738, "1.3.0+L2"),
@@ -127,16 +223,34 @@
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 1_010_520, "1.3.0"),
     ],
     EthereumNetwork.POLIS_MAINNET: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 1227, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 1278, "1.3.0"),
     ],
     EthereumNetwork.OPTIMISM: [
-        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 173749, "1.3.0+L2"),
-        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 173751, "1.3.0"),
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            30813792,
+            "1.3.0+L2",
+        ),  # default singleton address
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            173749,
+            "1.3.0+L2",
+        ),  # safe singleton address
+        (
+            "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
+            3936972,
+            "1.3.0",
+        ),  # default singleton address
+        (
+            "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
+            173751,
+            "1.3.0",
+        ),  # safe singleton address
     ],
     EthereumNetwork.BOBA_BNB_MAINNET: [
         ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 22284, "1.3.0+L2"),
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 22285, "1.3.0"),
     ],
     EthereumNetwork.BOBA_AVAX: [
         ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 55746, "1.3.0+L2"),
@@ -293,83 +407,180 @@
         ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 12651754, "1.3.0+L2"),
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 12651757, "1.3.0"),
     ],
     EthereumNetwork.WEMIX3_0_TESTNET: [
         ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 20834033, "1.3.0+L2"),
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 20834039, "1.3.0"),
     ],
+    EthereumNetwork.EVMOS_TESTNET: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 70652, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 70654, "1.3.0"),
+    ],
+    EthereumNetwork.EVMOS: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 158463, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 158486, "1.3.0"),
+    ],
+    EthereumNetwork.SCROLL_GOERLI_TESTNET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 676474, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 676478, "1.3.0"),
+    ],
+    EthereumNetwork.MAP_MAINNET: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 5190553, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 5190556, "1.3.0"),
+    ],
+    EthereumNetwork.MAP_MAKALU: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 2987582, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 2987584, "1.3.0"),
+    ],
+    EthereumNetwork.ETHEREUM_CLASSIC_MAINNET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 15904944, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 15904946, "1.3.0"),
+    ],
+    EthereumNetwork.ETHEREUM_CLASSIC_TESTNET_MORDOR: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 6333171, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 6333172, "1.3.0"),
+    ],
+    EthereumNetwork.SEPOLIA: [
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            2086878,
+            "1.3.0+L2",
+        ),  # Default singleton address
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            2087039,
+            "1.3.0+L2",
+        ),  # Safe singleton address
+        (
+            "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
+            2086880,
+            "1.3.0",
+        ),  # Default singleton address
+        (
+            "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
+            2087040,
+            "1.3.0",
+        ),  # Safe singleton address
+    ],
 }
 
 PROXY_FACTORIES: Dict[EthereumNetwork, List[Tuple[str, int]]] = {
     EthereumNetwork.MAINNET: [
-        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 12504126),  # v1.3.0
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            14981216,
+        ),  # v1.3.0 safe singleton address
+        (
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            12504126,
+        ),  # v1.3.0 default singleton address
         ("0x76E2cFc1F5Fa8F6a5b3fC4c8F4788F0116861F9B", 9084508),  # v1.1.1
         ("0x50e55Af101C777bA7A1d560a774A82eF002ced9F", 8915731),  # v1.1.0
         ("0x12302fE9c02ff50939BaAaaf415fc226C078613C", 7450116),  # v1.0.0
     ],
     EthereumNetwork.RINKEBY: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 8493997),  # v1.3.0
         ("0x76E2cFc1F5Fa8F6a5b3fC4c8F4788F0116861F9B", 5590757),
         ("0x50e55Af101C777bA7A1d560a774A82eF002ced9F", 5423494),
         ("0x12302fE9c02ff50939BaAaaf415fc226C078613C", 4110083),
     ],
     EthereumNetwork.GOERLI: [
-        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 4695402),  # v1.3.0
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            6900531,
+        ),  # v1.3.0 safe singleton address
+        (
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            4695402,
+        ),  # v1.3.0 default singleton address
         ("0x76E2cFc1F5Fa8F6a5b3fC4c8F4788F0116861F9B", 1798666),
         ("0x50e55Af101C777bA7A1d560a774A82eF002ced9F", 1631491),
         ("0x12302fE9c02ff50939BaAaaf415fc226C078613C", 312509),
     ],
     EthereumNetwork.KOVAN: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 25059601),  # v1.3.0
         ("0x76E2cFc1F5Fa8F6a5b3fC4c8F4788F0116861F9B", 15366151),
         ("0x50e55Af101C777bA7A1d560a774A82eF002ced9F", 14740731),
         ("0x12302fE9c02ff50939BaAaaf415fc226C078613C", 10629898),
     ],
     EthereumNetwork.GNOSIS: [
-        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 16236878),  # v1.3.0
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            27679953,
+        ),  # v1.3.0 safe singleton address
+        (
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            16236878,
+        ),  # v1.3.0 default singleton address
         ("0x76E2cFc1F5Fa8F6a5b3fC4c8F4788F0116861F9B", 10045327),  # v1.1.1
         ("0x12302fE9c02ff50939BaAaaf415fc226C078613C", 17677119),  # v1.0.0
     ],
     EthereumNetwork.ENERGY_WEB_CHAIN: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 12028652),  # v1.3.0
         ("0x76E2cFc1F5Fa8F6a5b3fC4c8F4788F0116861F9B", 6399239),
     ],
     EthereumNetwork.ENERGY_WEB_VOLTA_TESTNET: [
         # ('0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2', 0),  # v1.3.0
         ("0x76E2cFc1F5Fa8F6a5b3fC4c8F4788F0116861F9B", 6876681),
     ],
     EthereumNetwork.POLYGON: [
-        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 14306478),  # v1.3.0
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            34504003,
+        ),  # v1.3.0 safe singleton address
+        (
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            14306478,
+        ),  # v1.3.0 default singleton address
     ],
     EthereumNetwork.MUMBAI: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 13736914),  # v1.3.0
     ],
     EthereumNetwork.POLYGON_ZKEVM: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 79000),  # v1.3.0
     ],
     EthereumNetwork.ARBITRUM_ONE: [
-        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 1140),  # v1.3.0
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            88610602,
+        ),  # v1.3.0 safe singleton address
+        (
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            1140,
+        ),  # v1.3.0 default singleton address
     ],
     EthereumNetwork.ARBITRUM_NOVA: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 419),  # v1.3.0
     ],
     EthereumNetwork.ARBITRUM_RINKEBY: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 57070),  # v1.3.0
     ],
     EthereumNetwork.ARBITRUM_GOERLI: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 11538),  # v1.3.0
     ],
     EthereumNetwork.BINANCE_SMART_CHAIN_MAINNET: [
-        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 8485873),  # v1.3.0
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            28059981,
+        ),  # v1.3.0 safe singleton address
+        (
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            8485873,
+        ),  # v1.3.0 default singleton address
     ],
     EthereumNetwork.CELO_MAINNET: [
         ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 8944342),  # v1.3.0
     ],
     EthereumNetwork.AVALANCHE_C_CHAIN: [
-        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 4_949_487),  # v1.3.0
+        (
+            " 0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            14_747_108,
+        )(  # v1.3.0 default singleton address
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 4_949_487
+        ),  # v1.3.0 safe singleton address
     ],
     EthereumNetwork.MOONBEAM: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 172078),  # v1.3.0
     ],
     EthereumNetwork.MOONRIVER: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 707_721),  # v1.3.0
     ],
@@ -382,15 +593,22 @@
     EthereumNetwork.FUSE_SPARKNET: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 1_010_506),  # v1.3.0
     ],
     EthereumNetwork.POLIS_MAINNET: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 1266),  # v1.3.0
     ],
     EthereumNetwork.OPTIMISM: [
-        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 173709),  # v1.3.0
+        (
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            3936933,
+        ),  # v1.3.0 default singleton address
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            173709,
+        ),  # v1.3.0 safe singleton address
     ],
     EthereumNetwork.BOBA_BNB_MAINNET: [
         ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 22831),  # v1.3.0
     ],
     EthereumNetwork.BOBA_AVAX: [
         ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 55739),  # v1.3.0
     ],
@@ -484,15 +702,15 @@
     EthereumNetwork.XINFIN_XDC_NETWORK: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 53901564),  # v1.3.0
     ],
     EthereumNetwork.XDC_APOTHEM_NETWORK: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 42293264),  # v1.3.0
     ],
     EthereumNetwork.BASE_GOERLI_TESTNET: [
-        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 938848),  # v1.3.0
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 938696),  # v1.3.0
     ],
     EthereumNetwork.KAVA_EVM: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 2116356),  # v1.3.0
     ],
     EthereumNetwork.CROSSBELL: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 28314747),  # v1.3.0
     ],
@@ -511,8 +729,39 @@
     ],
     EthereumNetwork.WEMIX3_0_MAINNET: [
         ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 12651730),  # v1.3.0
     ],
     EthereumNetwork.WEMIX3_0_TESTNET: [
         ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 20833988),  # v1.3.0
     ],
+    EthereumNetwork.EVMOS_TESTNET: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 70637),  # v1.3.0
+    ],
+    EthereumNetwork.EVMOS: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 146858),  # v1.3.0
+    ],
+    EthereumNetwork.SCROLL_GOERLI_TESTNET: [
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 676384),  # v1.3.0
+    ],
+    EthereumNetwork.MAP_MAINNET: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 5190546),  # v1.3.0
+    ],
+    EthereumNetwork.MAP_MAKALU: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 2987578),  # v1.3.0
+    ],
+    EthereumNetwork.ETHEREUM_CLASSIC_MAINNET: [
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 15904946),  # v1.3.0
+    ],
+    EthereumNetwork.ETHEREUM_CLASSIC_TESTNET_MORDOR: [
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 6333172),  # v1.3.0
+    ],
+    EthereumNetwork.SEPOLIA: [
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            2087031,
+        ),  # v1.3.0  Safe singleton address
+        (
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            2086864,
+        ),  # v1.3.0  Default singleton address
+    ],
 }
```

### Comparing `safe-eth-py-5.3.1/gnosis/safe/api/base_api.py` & `safe-eth-py-5.4.0/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/api/relay_service_api.py` & `safe-eth-py-5.4.0/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/api/transaction_service_api.py` & `safe-eth-py-5.4.0/gnosis/safe/api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/exceptions.py` & `safe-eth-py-5.4.0/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/multi_send.py` & `safe-eth-py-5.4.0/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/proxy_factory.py` & `safe-eth-py-5.4.0/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/safe.py` & `safe-eth-py-5.4.0/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/safe_create2_tx.py` & `safe-eth-py-5.4.0/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/safe_creation_tx.py` & `safe-eth-py-5.4.0/gnosis/safe/safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/safe_signature.py` & `safe-eth-py-5.4.0/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/safe_tx.py` & `safe-eth-py-5.4.0/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/serializers.py` & `safe-eth-py-5.4.0/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/signatures.py` & `safe-eth-py-5.4.0/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/api/test_transaction_service_api.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/safe_test_case.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/test_multi_send.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/test_proxy_factory.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/test_safe.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_create2_tx.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_creation_tx.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/test_safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_signature.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_tx.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/test_serializers.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/test_signatures.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/gnosis/safe/tests/utils.py` & `safe-eth-py-5.4.0/gnosis/safe/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/safe_eth_py.egg-info/PKG-INFO` & `safe-eth-py-5.4.0/safe_eth_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 5.3.1
+Version: 5.4.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-5.3.1/safe_eth_py.egg-info/SOURCES.txt` & `safe-eth-py-5.4.0/safe_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.3.1/setup.cfg` & `safe-eth-py-5.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = safe-eth-py
-version = 5.3.1
+version = 5.4.0
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

