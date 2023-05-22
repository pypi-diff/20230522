# Comparing `tmp/ape-solidity-0.6.4.tar.gz` & `tmp/ape-solidity-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-solidity-0.6.4.tar", last modified: Thu May 18 15:22:34 2023, max compression
+gzip compressed data, was "ape-solidity-0.6.5.tar", last modified: Mon May 22 13:35:38 2023, max compression
```

## Comparing `ape-solidity-0.6.4.tar` & `ape-solidity-0.6.5.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/ape_solidity/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29021 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/ape_solidity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieProject/contracts/BrownieContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/BrownieStyleDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieStyleDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/BrownieStyleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieStyleDependency/contracts/FailingContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/Dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/Dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/contracts/Dependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/contracts/OlderDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/Dependency/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/Dependency/contracts/subfolder_with_imports/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/DependencyOfDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/DependencyOfDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/DependencyOfDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/ProjectWithinProject/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/ProjectWithinProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/ProjectWithinProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/ProjectWithinProject/contracts/Contract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/VersionSpecifiedInConfig/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/VersionSpecifiedInConfig/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/VersionSpecifiedInConfig/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/CircularImport1.sol
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/CircularImport2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/CompilesOnce.sol
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/DifferentNameThanFile.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/contracts/DirectoryWithExtension.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/DirectoryWithExtension.sol/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ExperimentalABIEncoderV2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ImportOlderDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ImportSourceWithEqualSignVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ImportSourceWithNoPrefixVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ImportingLessConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/Imports.sol
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/LibraryFun.sol
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/MissingPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/MultipleDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/NumerousDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/OlderVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/RandomVyperFile.vy
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/RangedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpacesInPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpecificVersionNoPrefix.sol
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpecificVersionNoPrefix2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpecificVersionRange.sol
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpecificVersionWithEqualSign.sol
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/UseYearn.sol
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/VagueVersion.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/subfolder/Relativecontract.sol
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/tests/data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)   698486 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)   879002 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/tests/data/packages/vault/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/tests/data/packages/vault/master/
--rw-r--r--   0 runner    (1001) docker     (123)   167518 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/data/packages/vault/master/vault_main.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/tests/data/packages/vault/v0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)   167551 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/data/packages/vault/v0.4.5/vault.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/scripts/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/ape_solidity/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29107 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/ape_solidity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-22 13:35:38.000000 ape-solidity-0.6.5/ape_solidity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieProject/contracts/BrownieContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/BrownieStyleDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieStyleDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/BrownieStyleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieStyleDependency/contracts/FailingContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/Dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/contracts/Dependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/contracts/OlderDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/Dependency/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/Dependency/contracts/subfolder_with_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/DependencyOfDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/DependencyOfDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/DependencyOfDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/ProjectWithinProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/ProjectWithinProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/ProjectWithinProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/ProjectWithinProject/contracts/Contract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/VersionSpecifiedInConfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/VersionSpecifiedInConfig/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/VersionSpecifiedInConfig/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/CircularImport1.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/CircularImport2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/CompilesOnce.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/DifferentNameThanFile.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/contracts/DirectoryWithExtension.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/DirectoryWithExtension.sol/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ExperimentalABIEncoderV2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ImportOlderDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ImportSourceWithEqualSignVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ImportSourceWithNoPrefixVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ImportingLessConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/Imports.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/LibraryFun.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/MissingPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/MultipleDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/NumerousDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/OlderVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/RandomVyperFile.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/RangedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpacesInPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpecificVersionNoPrefix.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpecificVersionNoPrefix2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpecificVersionRange.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpecificVersionWithEqualSign.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/UseYearn.sol
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/VagueVersion.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/subfolder/Relativecontract.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.217598 ape-solidity-0.6.5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.217598 ape-solidity-0.6.5/tests/data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.217598 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   698486 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   879002 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.217598 ape-solidity-0.6.5/tests/data/packages/vault/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/tests/data/packages/vault/master/
+-rw-r--r--   0 runner    (1001) docker     (123)   167518 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/data/packages/vault/master/vault_main.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/tests/data/packages/vault/v0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)   167551 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/data/packages/vault/v0.4.5/vault.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/scripts/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/test_integration.py
```

### Comparing `ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/bug.md` & `ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/feature.md` & `ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/work-item.md` & `ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.github/release-drafter.yml` & `ape-solidity-0.6.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.github/workflows/codeql.yml` & `ape-solidity-0.6.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.github/workflows/prtitle.yaml` & `ape-solidity-0.6.5/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.github/workflows/publish.yaml` & `ape-solidity-0.6.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.github/workflows/stale-prs.yml` & `ape-solidity-0.6.5/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.github/workflows/test.yaml` & `ape-solidity-0.6.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.gitignore` & `ape-solidity-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/.pre-commit-config.yaml` & `ape-solidity-0.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/CONTRIBUTING.md` & `ape-solidity-0.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/LICENSE` & `ape-solidity-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/PKG-INFO` & `ape-solidity-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.4
+Version: 0.6.5
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-solidity-0.6.4/README.md` & `ape-solidity-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/ape_solidity/_utils.py` & `ape-solidity-0.6.5/ape_solidity/_utils.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/ape_solidity/compiler.py` & `ape-solidity-0.6.5/ape_solidity/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,17 @@
                 # Source already present
                 continue
 
             # NOTE: Cached source may included sub-directories.
             cached_source.parent.mkdir(parents=True, exist_ok=True)
             if src.content:
                 cached_source.touch()
-                cached_source.write_text(src.content or "")
+                cached_source.write_text(
+                    src.content if isinstance(src.content, str) else str(src.content)
+                )
 
         # Add dependency remapping that may be needed.
         for compiler in manifest.compilers or []:
             settings = compiler.settings or {}
             settings_map = settings.get("remappings") or []
             remapping_list = [
                 ImportRemapping(entry=x, packages_cache=self.config_manager.packages_folder)
```

### Comparing `ape-solidity-0.6.4/ape_solidity.egg-info/PKG-INFO` & `ape-solidity-0.6.5/ape_solidity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.4
+Version: 0.6.5
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-solidity-0.6.4/ape_solidity.egg-info/SOURCES.txt` & `ape-solidity-0.6.5/ape_solidity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/ape_solidity.egg-info/requires.txt` & `ape-solidity-0.6.5/ape_solidity.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/pyproject.toml` & `ape-solidity-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/setup.py` & `ape-solidity-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/ape-config.yaml` & `ape-solidity-0.6.5/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/conftest.py` & `ape-solidity-0.6.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/contracts/Imports.sol` & `ape-solidity-0.6.5/tests/contracts/Imports.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/contracts/LibraryFun.sol` & `ape-solidity-0.6.5/tests/contracts/LibraryFun.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json` & `ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json` & `ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/data/packages/vault/master/vault_main.json` & `ape-solidity-0.6.5/tests/data/packages/vault/master/vault_main.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/data/packages/vault/v0.4.5/vault.json` & `ape-solidity-0.6.5/tests/data/packages/vault/v0.4.5/vault.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/scripts/clean.py` & `ape-solidity-0.6.5/tests/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/test_compiler.py` & `ape-solidity-0.6.5/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.4/tests/test_integration.py` & `ape-solidity-0.6.5/tests/test_integration.py`

 * *Files identical despite different names*

