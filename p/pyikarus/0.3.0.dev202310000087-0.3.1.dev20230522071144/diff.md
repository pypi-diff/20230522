# Comparing `tmp/pyikarus-0.3.0.dev202310000087.tar.gz` & `tmp/pyikarus-0.3.1.dev20230522071144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.0.dev202310000087.tar", last modified: Wed May 17 21:05:49 2023, max compression
+gzip compressed data, was "pyikarus-0.3.1.dev20230522071144.tar", last modified: Mon May 22 07:11:45 2023, max compression
```

## Comparing `pyikarus-0.3.0.dev202310000087.tar` & `pyikarus-0.3.1.dev20230522071144.tar`

### file list

```diff
@@ -1,330 +1,331 @@
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.496288 pyikarus-0.3.0.dev202310000087/
--rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.bettercodehub.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1300 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.clang-format
--rwxrwxrwx   0 user      (1001) user      (1001)     1017 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.cmake-format
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.045416 pyikarus-0.3.0.dev202310000087/.github/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.432115 pyikarus-0.3.0.dev202310000087/.github/ISSUE_TEMPLATE/
--rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/ISSUE_TEMPLATE/bug_report.md
--rwxrwxrwx   0 user      (1001) user      (1001)      615 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.569080 pyikarus-0.3.0.dev202310000087/.github/workflows/
--rwxrwxrwx   0 user      (1001) user      (1001)      476 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/codespell.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1034 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/createDockerContainer.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     4900 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/createRelease.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1635 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/debian-coverage.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     2414 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/debian.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     2042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/ghpages.yml
--rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/reuseLint.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     2854 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/runExamples.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1212 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/style.yml
--rwxrwxrwx   0 user      (1001) user      (1001)      455 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/.gitignore
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.580646 pyikarus-0.3.0.dev202310000087/.reuse/
--rwxrwxrwx   0 user      (1001) user      (1001)      661 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.reuse/dep5
--rwxrwxrwx   0 user      (1001) user      (1001)     3324 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/CHANGELOG.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1342 2023-05-17 21:01:23.000000 pyikarus-0.3.0.dev202310000087/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5335 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 user      (1001) user      (1001)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSE.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.635819 pyikarus-0.3.0.dev202310000087/LICENSES/
--rwxrwxrwx   0 user      (1001) user      (1001)    18375 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSES/CC-BY-SA-4.0.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     7048 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSES/CC0-1.0.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    42098 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSES/LGPL-3.0-or-later.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1078 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/LICENSES/MIT.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    16727 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSES/MPL-2.0.txt
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-17 21:05:49.494606 pyikarus-0.3.0.dev202310000087/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/README.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.053761 pyikarus-0.3.0.dev202310000087/Testing/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.664654 pyikarus-0.3.0.dev202310000087/Testing/Temporary/
--rwxrwxrwx   0 user      (1001) user      (1001)        4 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/Testing/Temporary/CTestCostData.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/Testing/Temporary/LastTest.log
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.698677 pyikarus-0.3.0.dev202310000087/cmake/
--rwxrwxrwx   0 user      (1001) user      (1001)       57 2023-05-17 21:01:23.000000 pyikarus-0.3.0.dev202310000087/cmake/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      973 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/CPM.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.711591 pyikarus-0.3.0.dev202310000087/cmake/FormatTarget/
--rwxrwxrwx   0 user      (1001) user      (1001)     1270 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.799965 pyikarus-0.3.0.dev202310000087/cmake/modules/
--rwxrwxrwx   0 user      (1001) user      (1001)      715 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/AddAutoDiffFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      683 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/AddEigenFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      740 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/AddMatplotppFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      691 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/AddSpdlogFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-17 20:06:12.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      379 2023-05-17 20:12:55.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/IkarusMacros.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)     2040 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/tools.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      148 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/codecov.yml
--rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/codespellignore
--rwxrwxrwx   0 user      (1001) user      (1001)     1588 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/config.h.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.866838 pyikarus-0.3.0.dev202310000087/docs/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.879918 pyikarus-0.3.0.dev202310000087/docs/BuildLocally/
--rwxrwxrwx   0 user      (1001) user      (1001)      439 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/BuildLocally/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      333 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.907987 pyikarus-0.3.0.dev202310000087/docs/__pycache__/
--rwxrwxrwx   0 user      (1001) user      (1001)     1136 2023-04-21 10:05:27.000000 pyikarus-0.3.0.dev202310000087/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rwxrwxrwx   0 user      (1001) user      (1001)     6961 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/literature.bib
--rwxrwxrwx   0 user      (1001) user      (1001)      117 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/literature.bib.license
--rwxrwxrwx   0 user      (1001) user      (1001)     1245 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/mkdocs-macros.py
--rwxrwxrwx   0 user      (1001) user      (1001)      394 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/mkdocs.insiders.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     5042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/mkdocs.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.078989 pyikarus-0.3.0.dev202310000087/docs/overrides/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.924528 pyikarus-0.3.0.dev202310000087/docs/overrides/partials/
--rwxrwxrwx   0 user      (1001) user      (1001)     1732 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/overrides/partials/comments.html
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.982767 pyikarus-0.3.0.dev202310000087/docs/website/
--rwxrwxrwx   0 user      (1001) user      (1001)       24 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/.meta.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.217162 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/
--rwxrwxrwx   0 user      (1001) user      (1001)     4710 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/assembler.md
--rwxrwxrwx   0 user      (1001) user      (1001)     6387 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/controlRoutines.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2024 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/dirichletBCs.md
--rwxrwxrwx   0 user      (1001) user      (1001)     3237 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/feRequirements.md
--rwxrwxrwx   0 user      (1001) user      (1001)     8524 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/finiteElements.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2745 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/grids.md
--rwxrwxrwx   0 user      (1001) user      (1001)     4121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/index.md
--rwxrwxrwx   0 user      (1001) user      (1001)     4932 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/localBasis.md
--rwxrwxrwx   0 user      (1001) user      (1001)    44213 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/localFunctions.md
--rwxrwxrwx   0 user      (1001) user      (1001)     3978 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/manifolds.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2590 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/nonlinearOperator.md
--rwxrwxrwx   0 user      (1001) user      (1001)     3086 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/observer.md
--rwxrwxrwx   0 user      (1001) user      (1001)     5211 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.393545 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/
--rwxrwxrwx   0 user      (1001) user      (1001)     6655 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/cantileverBeam.md
--rwxrwxrwx   0 user      (1001) user      (1001)     7251 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/computePi.md
--rwxrwxrwx   0 user      (1001) user      (1001)     5439 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/cooksMembrane.md
--rwxrwxrwx   0 user      (1001) user      (1001)     7055 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/incompressibleRubberBlock.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2164 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/index.md
--rwxrwxrwx   0 user      (1001) user      (1001)     7702 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/kirchhoffPlate.md
--rwxrwxrwx   0 user      (1001) user      (1001)     5114 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/newtonRaphsonMethod.md
--rwxrwxrwx   0 user      (1001) user      (1001)     6200 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/nonLinearElasticity.md
--rwxrwxrwx   0 user      (1001) user      (1001)     4071 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.464276 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/
--rwxrwxrwx   0 user      (1001) user      (1001)     2439 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/buildDocumentationLocally.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1002 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/codeStyle.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2415 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/howToEdit.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1762 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.499853 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/
--rwxrwxrwx   0 user      (1001) user      (1001)      274 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/.authors.yml
--rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.519013 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/posts/
--rwxrwxrwx   0 user      (1001) user      (1001)     7731 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.537392 pyikarus-0.3.0.dev202310000087/docs/website/05_cppReferences/
--rwxrwxrwx   0 user      (1001) user      (1001)     2324 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.554643 pyikarus-0.3.0.dev202310000087/docs/website/99_Literature/
--rwxrwxrwx   0 user      (1001) user      (1001)      169 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.626425 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.834012 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/
--rwxrwxrwx   0 user      (1001) user      (1001)    52795 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    46250 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     2852 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    17924 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     9455 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.053197 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/
--rwxrwxrwx   0 user      (1001) user      (1001)    35234 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    62184 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     2281 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    40033 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    25505 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     8101 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_blue.svg
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_blue.svg.license
--rwxrwxrwx   0 user      (1001) user      (1001)     8255 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_white.svg
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_white.svg.license
--rwxrwxrwx   0 user      (1001) user      (1001)     4364 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/download.md
--rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/gallery.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1358 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.072337 pyikarus-0.3.0.dev202310000087/docs/website/javascripts/
--rwxrwxrwx   0 user      (1001) user      (1001)      486 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.089591 pyikarus-0.3.0.dev202310000087/docs/website/stylesheets/
--rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/stylesheets/extra.css
--rwxrwxrwx   0 user      (1001) user      (1001)      502 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/dune.module
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.101231 pyikarus-0.3.0.dev202310000087/ikarus/
--rwxrwxrwx   0 user      (1001) user      (1001)      748 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.146088 pyikarus-0.3.0.dev202310000087/ikarus/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)      268 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/assembler/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    11069 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/assembler/simpleAssemblers.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    10714 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.189581 pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/
--rwxrwxrwx   0 user      (1001) user      (1001)      239 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     2575 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/loadControl.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2970 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.277381 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/
--rwxrwxrwx   0 user      (1001) user      (1001)      349 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      185 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.348300 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/
--rwxrwxrwx   0 user      (1001) user      (1001)      282 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     2925 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/autodiffFE.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2305 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/powerBasisFE.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1827 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/scalarFE.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1041 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feRequirements.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     8419 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feRequirements.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1338 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.438110 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/
--rwxrwxrwx   0 user      (1001) user      (1001)      345 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    19628 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    12549 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.608826 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/
--rwxrwxrwx   0 user      (1001) user      (1001)      397 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5699 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/interface.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2718 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     4635 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     3809 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     5734 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/svk.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      473 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/tags.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     8010 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1196 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     7827 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    12655 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.667948 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/
--rwxrwxrwx   0 user      (1001) user      (1001)      301 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     6734 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/dirichletValues.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     7791 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/nonLinearOperator.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    12303 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.682564 pyikarus-0.3.0.dev202310000087/ikarus/python/
--rwxrwxrwx   0 user      (1001) user      (1001)      294 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.716833 pyikarus-0.3.0.dev202310000087/ikarus/python/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)      249 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/assembler/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3149 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.751965 pyikarus-0.3.0.dev202310000087/ikarus/python/basis/
--rwxrwxrwx   0 user      (1001) user      (1001)      237 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/basis/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     4559 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.788310 pyikarus-0.3.0.dev202310000087/ikarus/python/dirichletValues/
--rwxrwxrwx   0 user      (1001) user      (1001)      257 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/dirichletValues/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     4116 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.843687 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/
--rwxrwxrwx   0 user      (1001) user      (1001)      303 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5036 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.884012 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/materials/
--rwxrwxrwx   0 user      (1001) user      (1001)      259 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/materials/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5107 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/materials/material.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     5503 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.997674 pyikarus-0.3.0.dev202310000087/ikarus/python/test/
--rwxrwxrwx   0 user      (1001) user      (1001)      564 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     4062 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/linearElasticTest.py
--rwxrwxrwx   0 user      (1001) user      (1001)  2704357 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/nameTest.vtu
--rwxrwxrwx   0 user      (1001) user      (1001)     4447 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/nonLinearElasticTest.py
--rwxrwxrwx   0 user      (1001) user      (1001)      862 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.034166 pyikarus-0.3.0.dev202310000087/ikarus/python/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)      245 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/utils/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1181 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.050627 pyikarus-0.3.0.dev202310000087/ikarus/solver/
--rwxrwxrwx   0 user      (1001) user      (1001)      211 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.084303 pyikarus-0.3.0.dev202310000087/ikarus/solver/linearSolver/
--rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/linearSolver/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     8891 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.155485 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/
--rwxrwxrwx   0 user      (1001) user      (1001)      272 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5407 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     8297 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    18574 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.462496 pyikarus-0.3.0.dev202310000087/ikarus/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)      712 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1741 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/algorithms.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      878 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/autodiffHelper.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1445 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/basis.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     6930 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/concepts.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      503 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.534118 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/
--rwxrwxrwx   0 user      (1001) user      (1001)      262 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1654 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/griddrawer.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      544 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/matplotHelper.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      703 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/matplotHelper.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2484 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/duneUtilities.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2347 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/eigenDuneTransformations.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      682 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/eigenSparseAddon.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1367 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/findLineSegment.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/findLineSegment.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     3611 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/flatPreBasis.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2171 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/functionSanityChecks.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6359 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/functionSanityChecks.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     3152 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/init.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    15244 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/linearAlgebraHelper.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1711 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.693182 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/
--rwxrwxrwx   0 user      (1001) user      (1001)      450 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1554 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/controlLogger.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2307 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/controlVTKWriter.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      905 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/genericControlObserver.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1053 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/gridDrawerObserver.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1132 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/loadControlObserver.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1985 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/nonLinearSolverLogger.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     5497 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/observer.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      489 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/observerMessages.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     4159 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/pathFollowingFunctions.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1131 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/polyfit.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      570 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/polyfit.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    10054 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/tensorUtils.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    15044 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/traits.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      432 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus.pc.in
--rwxrwxrwx   0 user      (1001) user      (1001)      196 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/iwyu.imp
--rwxrwxrwx   0 user      (1001) user      (1001)    47361 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/logfile
--rwxrwxrwx   0 user      (1001) user      (1001)      422 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/pyproject.toml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.717821 pyikarus-0.3.0.dev202310000087/python/
--rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-17 19:26:46.000000 pyikarus-0.3.0.dev202310000087/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.801017 pyikarus-0.3.0.dev202310000087/python/ikarus/
--rwxrwxrwx   0 user      (1001) user      (1001)      517 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      603 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     5636 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.834710 pyikarus-0.3.0.dev202310000087/python/ikarus/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)      167 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/assembler/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     2300 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/assembler/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1491 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/basis.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1408 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.869674 pyikarus-0.3.0.dev202310000087/python/ikarus/finite_elements/
--rwxrwxrwx   0 user      (1001) user      (1001)      173 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/finite_elements/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3465 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/finite_elements/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1792 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/materials.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.904624 pyikarus-0.3.0.dev202310000087/python/ikarus/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)      163 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/utils/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1496 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.978720 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/
--rwxrwxrwx   0 user      (1001) user      (1001)     3638 2023-05-17 21:05:43.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     9980 2023-05-17 21:05:45.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1001) user      (1001)        1 2023-05-17 21:05:43.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 21:05:43.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/requires.txt
--rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-17 21:05:43.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      632 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/setup.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.990660 pyikarus-0.3.0.dev202310000087/sandbox/
--rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/sandbox/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.018338 pyikarus-0.3.0.dev202310000087/sandbox/src/
--rwxrwxrwx   0 user      (1001) user      (1001)     1220 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.034326 pyikarus-0.3.0.dev202310000087/sandbox/src/auxiliaryFiles/
--rwxrwxrwx   0 user      (1001) user      (1001)   674469 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/sandbox/src/auxiliaryFiles/circle.msh
--rwxrwxrwx   0 user      (1001) user      (1001)      320 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/sandbox/src/sandbox.cpp
--rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-17 21:05:49.496795 pyikarus-0.3.0.dev202310000087/setup.cfg
--rwxrwxrwx   0 user      (1001) user      (1001)     1308 2023-05-17 21:05:40.000000 pyikarus-0.3.0.dev202310000087/setup.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.054202 pyikarus-0.3.0.dev202310000087/tests/
--rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/tests/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.388406 pyikarus-0.3.0.dev202310000087/tests/src/
--rwxrwxrwx   0 user      (1001) user      (1001)     1418 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3906 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/assemblerTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     9913 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/common.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2639 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/dependenciesTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6520 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/tests/src/dirichletValueTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     3820 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/easTest.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1473 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/enhancedAssumedStrainsTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      608 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/tests/src/factories.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1870 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/functionTraitsTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     2661 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/tests/src/linearElasticityTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     2378 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/manifoldsTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     7961 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/materialTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6770 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTest.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTestNeoHooke.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      729 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTestSVK.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     9936 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/nonLinearOperatorTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6327 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/pathFollowingTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     1651 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/polyFitTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      695 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/pythonConversionTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     1292 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/testAutodiffHelper.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     5805 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFEElement.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.478309 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/
--rwxrwxrwx   0 user      (1001) user      (1001)     9028 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredQuadscoarse.msh
--rwxrwxrwx   0 user      (1001) user      (1001)      395 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTest.geo
--rwxrwxrwx   0 user      (1001) user      (1001)      497 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTest.msh
--rwxrwxrwx   0 user      (1001) user      (1001)      546 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTest2.geo
--rwxrwxrwx   0 user      (1001) user      (1001)    11431 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTrianglesfine.msh
--rwxrwxrwx   0 user      (1001) user      (1001)     1114 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/tests/src/testHelpers.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    17595 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/trustRegionTest.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.012634 pyikarus-0.3.1.dev20230522071144/
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.bettercodehub.yml
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.clang-format
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.cmake-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.968633 pyikarus-0.3.1.dev20230522071144/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.976633 pyikarus-0.3.1.dev20230522071144/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      615 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.976633 pyikarus-0.3.1.dev20230522071144/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 root         (0) root         (0)     5639 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/createRelease.yml
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/ghpages.yml
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/reuseLint.yml
+-rw-r--r--   0 root         (0) root         (0)     3045 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/runExamples.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.976633 pyikarus-0.3.1.dev20230522071144/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.976633 pyikarus-0.3.1.dev20230522071144/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.980633 pyikarus-0.3.1.dev20230522071144/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    18375 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/LICENSES/MIT.txt
+-rw-r--r--   0 root         (0) root         (0)    16727 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-05-22 07:11:45.012634 pyikarus-0.3.1.dev20230522071144/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.980633 pyikarus-0.3.1.dev20230522071144/cmake/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      973 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.980633 pyikarus-0.3.1.dev20230522071144/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.980633 pyikarus-0.3.1.dev20230522071144/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      683 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      691 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      325 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/cmake/tools.cmake
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.980633 pyikarus-0.3.1.dev20230522071144/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.980633 pyikarus-0.3.1.dev20230522071144/docs/BuildLocally/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      333 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.980633 pyikarus-0.3.1.dev20230522071144/docs/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/literature.bib
+-rw-r--r--   0 root         (0) root         (0)      117 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/literature.bib.license
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/mkdocs-macros.py
+-rw-r--r--   0 root         (0) root         (0)      394 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/mkdocs.insiders.yml
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.968633 pyikarus-0.3.1.dev20230522071144/docs/overrides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.980633 pyikarus-0.3.1.dev20230522071144/docs/overrides/partials/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/overrides/partials/comments.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.980633 pyikarus-0.3.1.dev20230522071144/docs/website/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/.meta.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.984633 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/assembler.md
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 root         (0) root         (0)     8524 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/grids.md
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/index.md
+-rw-r--r--   0 root         (0) root         (0)     4932 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 root         (0) root         (0)    44213 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/observer.md
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.984633 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/computePi.md
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/index.md
+-rw-r--r--   0 root         (0) root         (0)     7702 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 root         (0) root         (0)     5114 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 root         (0) root         (0)     6200 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 root         (0) root         (0)     4071 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.984633 pyikarus-0.3.1.dev20230522071144/docs/website/03_contribution/
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.984633 pyikarus-0.3.1.dev20230522071144/docs/website/04_blog/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/04_blog/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.988633 pyikarus-0.3.1.dev20230522071144/docs/website/04_blog/posts/
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.988633 pyikarus-0.3.1.dev20230522071144/docs/website/05_cppReferences/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.988633 pyikarus-0.3.1.dev20230522071144/docs/website/99_Literature/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.988633 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.988633 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 root         (0) root         (0)    52795 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)    46250 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 root         (0) root         (0)    17924 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.992633 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 root         (0) root         (0)    35234 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 root         (0) root         (0)    62184 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 root         (0) root         (0)    40033 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 root         (0) root         (0)    25505 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 root         (0) root         (0)     8101 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/logo_blue.svg
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/logo_blue.svg.license
+-rw-r--r--   0 root         (0) root         (0)     8255 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/logo_white.svg
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/logo_white.svg.license
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/download.md
+-rw-r--r--   0 root         (0) root         (0)      244 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/gallery.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.992633 pyikarus-0.3.1.dev20230522071144/docs/website/javascripts/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.992633 pyikarus-0.3.1.dev20230522071144/docs/website/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/docs/website/stylesheets/extra.css
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/dune.module
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.992633 pyikarus-0.3.1.dev20230522071144/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.992633 pyikarus-0.3.1.dev20230522071144/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 root         (0) root         (0)    10714 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.992633 pyikarus-0.3.1.dev20230522071144/ikarus/controlRoutines/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.992633 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.992633 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feBases/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 root         (0) root         (0)     9346 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.992633 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    19446 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 root         (0) root         (0)    12479 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.996634 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 root         (0) root         (0)     9574 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 root         (0) root         (0)    12655 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.996634 pyikarus-0.3.1.dev20230522071144/ikarus/io/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/io/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/io/resultEvaluators.hh
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/io/resultFunction.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.996634 pyikarus-0.3.1.dev20230522071144/ikarus/linearAlgebra/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6735 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 root         (0) root         (0)     7789 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.996634 pyikarus-0.3.1.dev20230522071144/ikarus/python/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.996634 pyikarus-0.3.1.dev20230522071144/ikarus/python/assembler/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.996634 pyikarus-0.3.1.dev20230522071144/ikarus/python/basis/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.996634 pyikarus-0.3.1.dev20230522071144/ikarus/python/dirichletValues/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4169 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.996634 pyikarus-0.3.1.dev20230522071144/ikarus/python/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5220 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:44.996634 pyikarus-0.3.1.dev20230522071144/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9949 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 root         (0) root         (0)     5518 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.000634 pyikarus-0.3.1.dev20230522071144/ikarus/python/test/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.000634 pyikarus-0.3.1.dev20230522071144/ikarus/python/utils/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.000634 pyikarus-0.3.1.dev20230522071144/ikarus/solver/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.000634 pyikarus-0.3.1.dev20230522071144/ikarus/solver/linearSolver/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     8891 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.000634 pyikarus-0.3.1.dev20230522071144/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 root         (0) root         (0)    18574 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.004634 pyikarus-0.3.1.dev20230522071144/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/algorithms.hh
+-rw-r--r--   0 root         (0) root         (0)      878 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/basis.hh
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.004634 pyikarus-0.3.1.dev20230522071144/ikarus/utils/drawing/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 root         (0) root         (0)      544 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 root         (0) root         (0)      682 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 root         (0) root         (0)      724 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/init.hh
+-rw-r--r--   0 root         (0) root         (0)    15244 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.004634 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 root         (0) root         (0)      905 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 root         (0) root         (0)      570 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/polyfit.hh
+-rw-r--r--   0 root         (0) root         (0)    10054 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 root         (0) root         (0)    15044 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus/utils/traits.hh
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/ikarus.pc.in
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/iwyu.imp
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.004634 pyikarus-0.3.1.dev20230522071144/python/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.008634 pyikarus-0.3.1.dev20230522071144/python/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.008634 pyikarus-0.3.1.dev20230522071144/python/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/basis.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.008634 pyikarus-0.3.1.dev20230522071144/python/ikarus/finite_elements/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/finite_elements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/finite_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/materials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.008634 pyikarus-0.3.1.dev20230522071144/python/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      768 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.008634 pyikarus-0.3.1.dev20230522071144/python/pyikarus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-05-22 07:11:44.000000 pyikarus-0.3.1.dev20230522071144/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10022 2023-05-22 07:11:44.000000 pyikarus-0.3.1.dev20230522071144/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 07:11:44.000000 pyikarus-0.3.1.dev20230522071144/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 07:11:44.000000 pyikarus-0.3.1.dev20230522071144/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 07:11:44.000000 pyikarus-0.3.1.dev20230522071144/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      632 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/python/setup.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.008634 pyikarus-0.3.1.dev20230522071144/sandbox/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/sandbox/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.008634 pyikarus-0.3.1.dev20230522071144/sandbox/src/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.008634 pyikarus-0.3.1.dev20230522071144/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)   674469 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/sandbox/src/sandbox.cpp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 07:11:45.012634 pyikarus-0.3.1.dev20230522071144/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-05-22 07:11:44.000000 pyikarus-0.3.1.dev20230522071144/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.008634 pyikarus-0.3.1.dev20230522071144/tests/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.012634 pyikarus-0.3.1.dev20230522071144/tests/src/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/assemblerTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     9842 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/common.hh
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/dependenciesTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/dirichletValueTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     4594 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/easTest.hh
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/enhancedAssumedStrainsTest.cpp
+-rw-r--r--   0 root         (0) root         (0)      608 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/factories.hh
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/functionTraitsTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/linearElasticityTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/manifoldsTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     7961 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/materialTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/nonLinearElasticityTest.hh
+-rw-r--r--   0 root         (0) root         (0)      724 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/nonLinearElasticityTestNeoHooke.cpp
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/nonLinearElasticityTestSVK.cpp
+-rw-r--r--   0 root         (0) root         (0)     9936 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/nonLinearOperatorTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/pathFollowingTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/polyFitTest.cpp
+-rw-r--r--   0 root         (0) root         (0)      695 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/pythonConversionTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)     6143 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/testFEElement.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 07:11:45.012634 pyikarus-0.3.1.dev20230522071144/tests/src/testFiles/
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 root         (0) root         (0)      395 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 root         (0) root         (0)      546 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 root         (0) root         (0)    11431 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/testHelpers.hh
+-rw-r--r--   0 root         (0) root         (0)    17595 2023-05-22 07:11:36.000000 pyikarus-0.3.1.dev20230522071144/tests/src/trustRegionTest.cpp
```

### Comparing `pyikarus-0.3.0.dev202310000087/.clang-format` & `pyikarus-0.3.1.dev20230522071144/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/.cmake-format` & `pyikarus-0.3.1.dev20230522071144/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.1.dev20230522071144/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.1.dev20230522071144/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.1.dev20230522071144/.github/workflows/debian-coverage.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 on:
   push:
     paths-ignore:
       - 'docs/**'
       - '.github/workflows/ghpages.yml'
       - '.github/workflows/createDockerContainer.yml'
       - '**.md'
+
+  pull_request:
+    branches:
+      - main
+    paths-ignore:
+      - 'docs/**'
+      - '.github/workflows/ghpages.yml'
+      - '.github/workflows/createDockerContainer.yml'
+      - '**.md'
 env:
   CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
 
 jobs:
   GCC-Debug-CodeCov:
     runs-on: ubuntu-latest
     container:
```

### Comparing `pyikarus-0.3.0.dev202310000087/.github/workflows/debian.yml` & `pyikarus-0.3.1.dev20230522071144/.github/workflows/debian.yml`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,24 @@
 on:
   push:
     paths-ignore:
       - 'docs/**'
       - '.github/workflows/ghpages.yml'
       - '.github/workflows/createDockerContainer.yml'
       - '**.md'
+
+  pull_request:
+    branches:
+      - main
+    paths-ignore:
+      - 'docs/**'
+      - '.github/workflows/ghpages.yml'
+      - '.github/workflows/createDockerContainer.yml'
+      - '**.md'
+      -
 jobs:
   Build:
     name: ${{ matrix.config.name }}
     runs-on: ubuntu-latest
     container:
       image: ikarusproject/ikarus-dev:latest
       options: --memory-swap="20g" --memory="20g" --cpus="2" --user root
```

### Comparing `pyikarus-0.3.0.dev202310000087/.github/workflows/ghpages.yml` & `pyikarus-0.3.1.dev20230522071144/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/.github/workflows/runExamples.yml` & `pyikarus-0.3.1.dev20230522071144/.github/workflows/runExamples.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,24 @@
 on:
   push:
     paths-ignore:
       - 'docs/**'
       - '.github/workflows/ghpages.yml'
       - '.github/workflows/createDockerContainer.yml'
       - '**.md'
+
+
+  pull_request:
+    branches:
+      - main
+    paths-ignore:
+      - 'docs/**'
+      - '.github/workflows/ghpages.yml'
+      - '.github/workflows/createDockerContainer.yml'
+      - '**.md'
 jobs:
   Build:
     name: ${{ matrix.config.name }}
     runs-on: ubuntu-latest
     container:
       image: ikarusproject/ikarus-dev:latest
       options: --memory-swap="20g" --memory="20g" --cpus="2" --user root
```

### Comparing `pyikarus-0.3.0.dev202310000087/.github/workflows/style.yml` & `pyikarus-0.3.1.dev20230522071144/.github/workflows/style.yml`

 * *Files 22% similar despite different names*

```diff
@@ -36,15 +36,17 @@
       - uses: actions/checkout@v2
         with:
          path: 'repo'
       - name: Install format dependencies
         run: |
           sudo cp /usr/bin/clang-format-13 /usr/bin/clang-format
           pip install cmake_format==0.6.13 pyyaml
+          pip install black==23.3.0
 
       - name: configure
-        run: cmake -S "cmake/FormatTarget" -Bbuild -DADD_FORMATTARGET=TRUE
+        run: cmake -S "cmake/FormatTarget" -Bbuild -DADD_FORMATTARGET=TRUE -DADD_PYTHONFORMATTING=1
 
       - name: check style
         run: |
           cmake --build build --target format
           cmake --build build --target check-format
+          cmake --build build --target check-pythonformat
```

### Comparing `pyikarus-0.3.0.dev202310000087/.reuse/dep5` & `pyikarus-0.3.1.dev20230522071144/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/CHANGELOG.md` & `pyikarus-0.3.1.dev20230522071144/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - Added comment section to blog post ([511d83](https://github.com/ikarus-project/ikarus/commit/511d83f9e7c474c9b320db5bc9367114ebe2825d))
 - Updated license information ([#138](https://github.com/ikarus-project/ikarus/pull/138))
 - Added detailed documentation for ikarus-examples ([#140](https://github.com/ikarus-project/ikarus/pull/140))
 - Added computation of Cauchy stress in linear elasticity ([#137](https://github.com/ikarus-project/ikarus/pull/137))
 - Added greeting and init function for reasonable default, e.g. log also to file ([#147](https://github.com/ikarus-project/ikarus/pull/147))
 - Added an interface for the material library ([#154](https://github.com/ikarus-project/ikarus/pull/154))
 - Added a wrapper for flat and blocked basis ([#157](https://github.com/ikarus-project/ikarus/pull/157))
-- Added basic python bindings and infrastructure 
+- Added basic python bindings and infrastructure. Ikarus can now be downloaded via `pip install pyikarus` ([#157](https://github.com/ikarus-project/ikarus/pull/152))
 
 ## Release v0.3 (Prometheus)
 
 - Added codespell workflow (CI checks now for grammar and typos in comments and variable names) [#70](https://github.com/ikarus-project/ikarus/pull/70)
 - Added `EnhancedAssumedStrains` to decorate a linear-elastic element with various EAS methods [#74](https://github.com/ikarus-project/ikarus/pull/74)
 - Added the ability for the linear solver to accept matrix-valued rhs [#76](https://github.com/ikarus-project/ikarus/pull/76)
 - Added a path-following technique, such that a scalar subsidiary equation, for example, for `Arc length method`,  can be implemented independently [#80](https://github.com/ikarus-project/ikarus/pull/80)
```

### Comparing `pyikarus-0.3.0.dev202310000087/CMakeLists.txt` & `pyikarus-0.3.1.dev20230522071144/CMakeLists.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 # SPDX-License-Identifier: LGPL-3.0-or-later
-message(STATUS "${SKBUILD}")
+
 cmake_minimum_required(VERSION 3.18 FATAL_ERROR)
 
 option(DUNE_ENABLE_PYTHONBINDINGS "Enable Python bindings" ON)
 option(DUNE_PYTHON_ALLOW_GET_PIP "Allow dune-common to install pip into venv" ON)
 project(
-        ikarus
-  VERSION 0.3
+  ikarus
+  VERSION 0.3.0
   LANGUAGES C CXX
 )
 
 add_definitions(-DDUNE_LOCALFEFUNCTIONS_USE_EIGEN=1)
 add_definitions(-DCMAKE_DISABLE_FIND_PACKAGE_Vc=1)
 add_definitions(-DCMAKE_DISABLE_FIND_PACKAGE_LATEX=1)
 add_definitions(-DBUILD_SHARED_LIBS=1)
 
 # find dune packages to make cmake modules available
 find_package(dune-common REQUIRED EXCLUDE_FROM_ALL)
 list(APPEND CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/cmake/modules" ${dune-common_MODULE_PATH})
 include(DuneMacros)
-# set(CXX_MAX_STANDARD 20)
+
 dune_project()
 dune_enable_all_packages()
 
 add_subdirectory(ikarus)
 add_subdirectory(cmake)
 if(NOT SKBUILD)
-add_subdirectory(sandbox)
-add_subdirectory(tests)
-add_subdirectory(cmake/FormatTarget)
+  add_subdirectory(sandbox)
+  add_subdirectory(tests)
 endif()
 
 if(BUILD_DOCS)
   message("Build docs locally target ENABLED")
   add_subdirectory(docs/BuildLocally)
 endif()
```

### Comparing `pyikarus-0.3.0.dev202310000087/CODE_OF_CONDUCT.md` & `pyikarus-0.3.1.dev20230522071144/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/LICENSE.md` & `pyikarus-0.3.1.dev20230522071144/LICENSE.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 # Copyright holders
 
 - 2021-2023 Alexander Müller
 - 2022-2023 Tarun Kumar Mitruka Vinod Kumar Mitruka
 - 2022      Tobias Willmann
+- 2023      Henrik Jakob
 
 We use [REUSE software](https://reuse.software/) to manage our licenses.
 All licenses reside in the folder `LICENSES`.
 Each source file here has the corresponding header for license information.
 The Ikarus source and header files are released under `LGPL-3.0-or-later`.
 
 Only `ikarus/linearAlgebra/truncatedConjugateGradient.hh` adapted from the
```

### Comparing `pyikarus-0.3.0.dev202310000087/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.1.dev20230522071144/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.1.dev20230522071144/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.1.dev20230522071144/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/LICENSES/MIT.txt` & `pyikarus-0.3.1.dev20230522071144/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.1.dev20230522071144/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/PKG-INFO` & `pyikarus-0.3.1.dev20230522071144/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000087
+Version: 0.3.1.dev20230522071144
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
@@ -20,14 +20,15 @@
 [![Debian](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml)
 [![codecov](https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus)
 [![CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml)
 [![Docs](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/repository/github/ikarus-project/ikarus/overview/main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/ikarus/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ikarus-project/ikarus&amp;utm_campaign=Badge_Grade)
 [![Gitter](https://badges.gitter.im/ikarus-project/community.svg)](https://gitter.im/ikarus-project/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![PyPI version](https://badge.fury.io/py/pyikarus.svg)](https://badge.fury.io/py/pyikarus)
 
 
 [![Release](https://badgen.net/badge/Release/0.3/purple?icon=github)](https://github.com/ikarus-project/ikarus/releases)
 [![Doi](https://img.shields.io/badge/DOI-10.18419%2Fdarus--3303-orange)](https://doi.org/10.18419/darus-3303)
 [![SWH](https://archive.softwareheritage.org/badge/origin/https://github.com/ikarus-project/ikarus/)](https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/ikarus-project/ikarus)
 [![SWHRelease](https://archive.softwareheritage.org/badge/swh:1:rel:2cbfacc591c5fa48bdc84b375e42d1ab5304425f/)](https://archive.softwareheritage.org/swh:1:rel:2cbfacc591c5fa48bdc84b375e42d1ab5304425f;origin=https://github.com/ikarus-project/ikarus;visit=swh:1:snp:22424908ab42ab0d38be84c34235b8b5ae7af6c4)
```

#### html2text {}

```diff
@@ -1,37 +1,39 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000087 Home-page:
-Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
-Classifier: Programming Language :: C++ Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
-(GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
-File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
-actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
-ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
-project/ikarus/branch/main/graph/badge.svg?token=zJgggitPMc)](https://
-codecov.io/gh/ikarus-project/ikarus) [![CodeStyle](https://github.com/ikarus-
-project/ikarus/actions/workflows/style.yml/badge.svg)](https://github.com/
-ikarus-project/ikarus/actions/workflows/style.yml) [![Docs](https://github.com/
-ikarus-project/ikarus/actions/workflows/ghpages.yml/badge.svg)](https://
-github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml) [![CodeFactor]
-(https://www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)]
-(https://www.codefactor.io/repository/github/ikarus-project/ikarus/overview/
-main) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/
-5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/
-ikarus/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ikarus-
-project/ikarus&utm_campaign=Badge_Grade) [![Gitter](https://badges.gitter.im/
-ikarus-project/community.svg)](https://gitter.im/ikarus-project/
-community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![Release]
-(https://badgen.net/badge/Release/0.3/purple?icon=github)](https://github.com/
-ikarus-project/ikarus/releases) [![Doi](https://img.shields.io/badge/DOI-
-10.18419%2Fdarus--3303-orange)](https://doi.org/10.18419/darus-3303) [![SWH]
-(https://archive.softwareheritage.org/badge/origin/https://github.com/ikarus-
-project/ikarus/)](https://archive.softwareheritage.org/browse/origin/
-?origin_url=https://github.com/ikarus-project/ikarus) [![SWHRelease](https://
-archive.softwareheritage.org/badge/swh:1:rel:
-2cbfacc591c5fa48bdc84b375e42d1ab5304425f/)](https://
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.1.dev20230522071144 Home-
+page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
+stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
+Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
+markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
+ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
+github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
+(https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/
+badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus) [!
+[CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/
+style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/
+workflows/style.yml) [![Docs](https://github.com/ikarus-project/ikarus/actions/
+workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/
+actions/workflows/ghpages.yml) [![CodeFactor](https://www.codefactor.io/
+repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/
+repository/github/ikarus-project/ikarus/overview/main) [![Codacy Badge](https:/
+/app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://
+www.codacy.com/gh/ikarus-project/ikarus/
+dashboard?utm_source=github.com&utm_medium=referral&utm_content=ikarus-project/
+ikarus&utm_campaign=Badge_Grade) [![Gitter](https://badges.gitter.im/ikarus-
+project/community.svg)](https://gitter.im/ikarus-project/
+community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![PyPI
+version](https://badge.fury.io/py/pyikarus.svg)](https://badge.fury.io/py/
+pyikarus) [![Release](https://badgen.net/badge/Release/0.3/purple?icon=github)]
+(https://github.com/ikarus-project/ikarus/releases) [![Doi](https://
+img.shields.io/badge/DOI-10.18419%2Fdarus--3303-orange)](https://doi.org/
+10.18419/darus-3303) [![SWH](https://archive.softwareheritage.org/badge/origin/
+https://github.com/ikarus-project/ikarus/)](https://
+archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/
+ikarus-project/ikarus) [![SWHRelease](https://archive.softwareheritage.org/
+badge/swh:1:rel:2cbfacc591c5fa48bdc84b375e42d1ab5304425f/)](https://
 archive.softwareheritage.org/swh:1:rel:
 2cbfacc591c5fa48bdc84b375e42d1ab5304425f;origin=https://github.com/ikarus-
 project/ikarus;visit=swh:1:snp:22424908ab42ab0d38be84c34235b8b5ae7af6c4) This
 project tries to provide an easy to read and an easy to use finite element
 framework. It is heavily inspired by the finite element software [DUNE](https:/
 /dune-project.org/), the book [DUNE â The Distributed and Unified Numerics
 Environment](https://www.springer.com/gp/book/9783030597016), [deal.II](https:/
```

### Comparing `pyikarus-0.3.0.dev202310000087/README.md` & `pyikarus-0.3.1.dev20230522071144/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 [![Debian](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml)
 [![codecov](https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus)
 [![CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml)
 [![Docs](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/repository/github/ikarus-project/ikarus/overview/main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/ikarus/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ikarus-project/ikarus&amp;utm_campaign=Badge_Grade)
 [![Gitter](https://badges.gitter.im/ikarus-project/community.svg)](https://gitter.im/ikarus-project/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![PyPI version](https://badge.fury.io/py/pyikarus.svg)](https://badge.fury.io/py/pyikarus)
 
 
 [![Release](https://badgen.net/badge/Release/0.3/purple?icon=github)](https://github.com/ikarus-project/ikarus/releases)
 [![Doi](https://img.shields.io/badge/DOI-10.18419%2Fdarus--3303-orange)](https://doi.org/10.18419/darus-3303)
 [![SWH](https://archive.softwareheritage.org/badge/origin/https://github.com/ikarus-project/ikarus/)](https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/ikarus-project/ikarus)
 [![SWHRelease](https://archive.softwareheritage.org/badge/swh:1:rel:2cbfacc591c5fa48bdc84b375e42d1ab5304425f/)](https://archive.softwareheritage.org/swh:1:rel:2cbfacc591c5fa48bdc84b375e42d1ab5304425f;origin=https://github.com/ikarus-project/ikarus;visit=swh:1:snp:22424908ab42ab0d38be84c34235b8b5ae7af6c4)
```

#### html2text {}

```diff
@@ -10,23 +10,24 @@
 www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)](https://
 www.codefactor.io/repository/github/ikarus-project/ikarus/overview/main) [!
 [Codacy Badge](https://app.codacy.com/project/badge/Grade/
 5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/
 ikarus/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ikarus-
 project/ikarus&utm_campaign=Badge_Grade) [![Gitter](https://badges.gitter.im/
 ikarus-project/community.svg)](https://gitter.im/ikarus-project/
-community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![Release]
-(https://badgen.net/badge/Release/0.3/purple?icon=github)](https://github.com/
-ikarus-project/ikarus/releases) [![Doi](https://img.shields.io/badge/DOI-
-10.18419%2Fdarus--3303-orange)](https://doi.org/10.18419/darus-3303) [![SWH]
-(https://archive.softwareheritage.org/badge/origin/https://github.com/ikarus-
-project/ikarus/)](https://archive.softwareheritage.org/browse/origin/
-?origin_url=https://github.com/ikarus-project/ikarus) [![SWHRelease](https://
-archive.softwareheritage.org/badge/swh:1:rel:
-2cbfacc591c5fa48bdc84b375e42d1ab5304425f/)](https://
+community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![PyPI
+version](https://badge.fury.io/py/pyikarus.svg)](https://badge.fury.io/py/
+pyikarus) [![Release](https://badgen.net/badge/Release/0.3/purple?icon=github)]
+(https://github.com/ikarus-project/ikarus/releases) [![Doi](https://
+img.shields.io/badge/DOI-10.18419%2Fdarus--3303-orange)](https://doi.org/
+10.18419/darus-3303) [![SWH](https://archive.softwareheritage.org/badge/origin/
+https://github.com/ikarus-project/ikarus/)](https://
+archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/
+ikarus-project/ikarus) [![SWHRelease](https://archive.softwareheritage.org/
+badge/swh:1:rel:2cbfacc591c5fa48bdc84b375e42d1ab5304425f/)](https://
 archive.softwareheritage.org/swh:1:rel:
 2cbfacc591c5fa48bdc84b375e42d1ab5304425f;origin=https://github.com/ikarus-
 project/ikarus;visit=swh:1:snp:22424908ab42ab0d38be84c34235b8b5ae7af6c4) This
 project tries to provide an easy to read and an easy to use finite element
 framework. It is heavily inspired by the finite element software [DUNE](https:/
 /dune-project.org/), the book [DUNE â The Distributed and Unified Numerics
 Environment](https://www.springer.com/gp/book/9783030597016), [deal.II](https:/
```

### Comparing `pyikarus-0.3.0.dev202310000087/cmake/CPM.cmake` & `pyikarus-0.3.1.dev20230522071144/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.1.dev20230522071144/cmake/FormatTarget/CMakeLists.txt`

 * *Files 27% similar despite different names*

```diff
@@ -48,7 +48,31 @@
     )
   else()
     message(STATUS "python not found, codespell target not available")
 
   endif()
 
 endif()
+
+if(ADD_PYTHONFORMATTING)
+  find_package(Python)
+  if(Python_FOUND)
+    message("Adding python format command")
+
+    set(PYTHONFORMATTINGCOMAND python -m black .)
+    add_custom_target(
+      fix-pythonformat
+      COMMAND ${PYTHONFORMATTINGCOMAND}
+      WORKING_DIRECTORY ${CMAKE_SOURCE_DIR}
+    )
+
+    set(PYTHONFORMATTINGCOMANDCHECK python -m black . --check)
+    add_custom_target(
+      check-pythonformat
+      COMMAND ${PYTHONFORMATTINGCOMANDCHECK}
+      WORKING_DIRECTORY ${CMAKE_SOURCE_DIR}
+    )
+  else()
+    message(STATUS "python not found, codespell target not available")
+  endif()
+
+endif()
```

### Comparing `pyikarus-0.3.0.dev202310000087/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.1.dev20230522071144/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.1.dev20230522071144/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.1.dev20230522071144/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.1.dev20230522071144/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/cmake/tools.cmake` & `pyikarus-0.3.1.dev20230522071144/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/config.h.cmake` & `pyikarus-0.3.1.dev20230522071144/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.1.dev20230522071144/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/literature.bib` & `pyikarus-0.3.1.dev20230522071144/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/mkdocs-macros.py` & `pyikarus-0.3.1.dev20230522071144/docs/mkdocs-macros.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
-#
 # SPDX-License-Identifier: CC-BY-SA-4.0
 
 "These macros are taken and modified from https://github.com/autodiff/autodiff"
 
+
 def define_env(env):
     """
     This is the hook for the functions
 
     - variables: the dictionary that contains the variables
     - macro: a decorator function, to declare a macro.
     """
 
     @env.macro
     def inputcode(filename, language, linenumbers=False, startline=0, endline=None):
-        filename = '../' + filename  # file path must be given relative to root directory
-        f = open(filename, 'r')
+        filename = (
+            "../" + filename
+        )  # file path must be given relative to root directory
+        f = open(filename, "r")
         if startline != 0 or endline is None:
             lines = f.readlines()
             lines = lines[startline:endline]
             text = "".join(lines)
         else:
             text = f.read()
         if linenumbers is False:
-            textblock = f'```{{ .{language} .annotate}}\n{text}\n```'
+            textblock = f"```{{ .{language} .annotate}}\n{text}\n```"
         else:
             textblock = f'```{{ .{language} linenums="1" .annotate}} \n{text}\n```'
         return textblock
 
     @env.macro
-    def inputcpp(filename,linenumbers=False, startline=0, endline=None):
-        return inputcode(filename, 'cpp', linenumbers, startline, endline)
+    def inputcpp(filename, linenumbers=False, startline=0, endline=None):
+        return inputcode(filename, "cpp", linenumbers, startline, endline)
```

### Comparing `pyikarus-0.3.0.dev202310000087/docs/mkdocs.yml` & `pyikarus-0.3.1.dev20230522071144/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/overrides/partials/comments.html` & `pyikarus-0.3.1.dev20230522071144/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/assembler.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/grids.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/index.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/observer.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/solvers.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/computePi.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/index.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/03_contribution/openTask.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 * Nonlinear Reissner-Mindlin shell [@muller2022consistent]
 * Kirchhoff-Love shell
 * 3D-Beam
 * Implement forces and stiffness matrix of `NonLinearElastic`
 * Standard beam and plate formulations
 
 ### Further addons
-* Python binding ([pybind11](https://github.com/pybind/pybind11))
 * [Muesli](https://materials.imdea.org/muesli/)
 
 [^KLNote]: This is usually needed for a Kirchhoff-Love shell implementation, see [@kiendlKLshell].
 
 !!! note  "Code style"
     For details on the code style, refer [link](codeStyle.md).
```

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_blue.svg` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/logo_blue.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_white.svg` & `pyikarus-0.3.1.dev20230522071144/docs/website/auxiliaryImages/logo_white.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/download.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/docs/website/index.md` & `pyikarus-0.3.1.dev20230522071144/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/CMakeLists.txt` & `pyikarus-0.3.1.dev20230522071144/ikarus/CMakeLists.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 cmake_minimum_required(VERSION 3.18)
-# set(CXX_MAX_STANDARD 20)
+
 file(
   GLOB_RECURSE sources
   RELATIVE ${CMAKE_CURRENT_SOURCE_DIR}
   CONFIGURE_DEPENDS *.cpp
 )
 
 dune_add_library(${PROJECT_NAME} ${sources})
@@ -17,10 +17,11 @@
 
 add_subdirectory(assembler)
 add_subdirectory(controlRoutines)
 add_subdirectory(finiteElements)
 add_subdirectory(linearAlgebra)
 add_subdirectory(solver)
 add_subdirectory(utils)
+add_subdirectory(io)
 if(DUNE_ENABLE_PYTHONBINDINGS)
   add_subdirectory(python)
 endif()
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/assembler/simpleAssemblers.hh`

 * *Files 5% similar despite different names*

```diff
@@ -19,22 +19,25 @@
 
   /*!
    * The FlatAssemblerBase takes care of common subtask done by flat assemblers
    */
   template <typename FEContainer_, typename DirichletValuesType_>
   class FlatAssemblerBase {
   public:
-    using FERequirementType = typename FEContainer_::value_type::FERequirementType;
-    using GlobalIndex     = typename FEContainer_::value_type::GlobalIndex;
-    using Basis = typename DirichletValuesType_::Basis;
-    using GridView = typename Basis::GridView;
-    using FEContainer = FEContainer_;
+    using FEContainerRaw    = std::remove_cvref_t<FEContainer_>;
+    using FERequirementType = typename FEContainerRaw::value_type::FERequirementType;
+    using GlobalIndex       = typename FEContainerRaw::value_type::GlobalIndex;
+    using Basis             = typename DirichletValuesType_::Basis;
+    using GridView          = typename Basis::GridView;
+    using FEContainer       = FEContainer_;
+    // If we get a reference we store the reference but if we get an r-value we store by value
+    using FEContainerType     = std::conditional_t<std::is_reference_v<FEContainer>, const FEContainer, FEContainer>;
     using DirichletValuesType = DirichletValuesType_;
-    FlatAssemblerBase(const FEContainer &fes, const DirichletValuesType &p_dirichletValues)
-        : feContainer{fes}, dirichletValues{&p_dirichletValues} {
+    FlatAssemblerBase(FEContainer &&fes, const DirichletValuesType &p_dirichletValues)
+        : feContainer{std::forward<FEContainer>(fes)}, dirichletValues{&p_dirichletValues} {
       constraintsBelow_.reserve(dirichletValues->size());
       size_t counter = 0;
       for (auto iv : std::ranges::iota_view{decltype(dirichletValues->size())(0), dirichletValues->size()}) {
         constraintsBelow_.emplace_back(counter);
         if (dirichletValues->isConstrained(iv)) ++counter;
       }
       fixedDofs = dirichletValues->fixedDOFsize();
@@ -51,43 +54,50 @@
      * writes a zero for the fixed doffs */
     Eigen::VectorXd createFullVector(Eigen::Ref<const Eigen::VectorXd> reducedVector);
 
     /**  Returns the container of finite elements */
     auto &finiteElements() const { return feContainer; }
 
     /**  Returns the number of constraints below a given degrees of freedom index */
-    size_t constraintsBelow(size_t i) const { return constraintsBelow_[i]; }
+    [[nodiscard]] size_t constraintsBelow(size_t i) const { return constraintsBelow_[i]; }
 
     /**  Returns the boolean if a given degree of freedom is fixed */
-    bool isConstrained(size_t i) const { return dirichletValues->isConstrained(i); }
+    [[nodiscard]] bool isConstrained(size_t i) const { return dirichletValues->isConstrained(i); }
 
     /**  Coarse estimate of node connectivity, i.e. this relates the bandwidth of an sparse matrix.
      * This estimate is designed that it overestimates the real connectivity since it should
      * only be used for allocating vectors */
-    size_t estimateOfConnectivity() const { return dirichletValues->basis().gridView().size(GridView::dimension) * 8; }
+    [[nodiscard]] size_t estimateOfConnectivity() const {
+      return dirichletValues->basis().gridView().size(GridView::dimension) * 8;
+    }
 
   private:
-    FEContainer feContainer;
+    FEContainerType feContainer;
     DirichletValuesType const *dirichletValues;
     std::vector<size_t> constraintsBelow_{};
     size_t fixedDofs{};
   };
 
+  template <class T, class DirichletValuesType>
+  FlatAssemblerBase(T &&fes, const DirichletValuesType &dirichletValues_) -> FlatAssemblerBase<T, DirichletValuesType>;
+
   /** ScalarAssembler assembles scalar quantities */
-  template < typename FEContainer_,typename DirichletValuesType_>
+  template <typename FEContainer_, typename DirichletValuesType_>
   class ScalarAssembler : public FlatAssemblerBase<FEContainer_, DirichletValuesType_> {
-    using FERequirementType = typename FEContainer_::value_type::FERequirementType;
-    using GlobalIndex     = typename FEContainer_::value_type::GlobalIndex;
-    using Basis = typename DirichletValuesType_::Basis;
-    using FEContainer = FEContainer_;
+    using FEContainerRaw = std::remove_cvref_t<FEContainer_>;
+
+    using FERequirementType   = typename FEContainerRaw::value_type::FERequirementType;
+    using GlobalIndex         = typename FEContainerRaw::value_type::GlobalIndex;
+    using Basis               = typename DirichletValuesType_::Basis;
+    using FEContainer         = FEContainer_;
     using DirichletValuesType = DirichletValuesType_;
 
   public:
-    ScalarAssembler(const FEContainer &fes, const DirichletValuesType &dirichletValues_)
-        : FlatAssemblerBase<FEContainer,DirichletValuesType>(fes, dirichletValues_) {}
+    ScalarAssembler(FEContainer &&fes, const DirichletValuesType &dirichletValues_)
+        : FlatAssemblerBase<FEContainer, DirichletValuesType>(std::forward<FEContainer>(fes), dirichletValues_) {}
 
     /** Calculates the scalar quantity which is requested by fErequirements and returns a reference */
     double &getScalar(const FERequirementType &fErequirements) { return getScalarImpl(fErequirements); }
 
   private:
     double &getScalarImpl(const FERequirementType &fErequirements) {
       scal = 0.0;
@@ -96,26 +106,31 @@
       }
       return scal;
     }
 
     double scal{0.0};
   };
 
+  template <class T, class DirichletValuesType>
+  ScalarAssembler(T &&fes, const DirichletValuesType &dirichletValues_) -> ScalarAssembler<T, DirichletValuesType>;
+
   /** VectorFlatAssembler assembles vector quantities using a flat basis Indexing strategy */
-  template < typename FEContainer_,typename DirichletValuesType_>
+  template <typename FEContainer_, typename DirichletValuesType_>
   class VectorFlatAssembler : public ScalarAssembler<FEContainer_, DirichletValuesType_> {
-    using FERequirementType = typename FEContainer_::value_type::FERequirementType;
-    using GlobalIndex     = typename FEContainer_::value_type::GlobalIndex;
-    using Basis = typename DirichletValuesType_::Basis;
-    using FEContainer = FEContainer_;
+    using FEContainerRaw = std::remove_cvref_t<FEContainer_>;
+
+    using FERequirementType   = typename FEContainerRaw::value_type::FERequirementType;
+    using GlobalIndex         = typename FEContainerRaw::value_type::GlobalIndex;
+    using Basis               = typename DirichletValuesType_::Basis;
+    using FEContainer         = FEContainer_;
     using DirichletValuesType = DirichletValuesType_;
 
   public:
-    VectorFlatAssembler(const FEContainer &fes, const DirichletValuesType &dirichletValues_)
-        : ScalarAssembler<FEContainer,DirichletValuesType>(fes, dirichletValues_) {}
+    VectorFlatAssembler(FEContainer &&fes, const DirichletValuesType &dirichletValues_)
+        : ScalarAssembler<FEContainer, DirichletValuesType>(std::forward<FEContainer>(fes), dirichletValues_) {}
 
     /** Calculates the vectorial quantity which is requested by fErequirements and returns a reference
      * A zero is written on fixed dofs */
     Eigen::VectorXd &getVector(const FERequirementType &fErequirements) { return getVectorImpl(fErequirements); }
 
     /** Calculates the vectorial quantity which is requested by fErequirements and returns a reference
      * This vector has a reduced size by the number of fixed degrees of freedom */
@@ -127,29 +142,34 @@
     Eigen::VectorXd &getVectorImpl(const FERequirementType &fErequirements);
     Eigen::VectorXd &getReducedVectorImpl(const FERequirementType &fErequirements);
 
     Eigen::VectorXd vec{};
     Eigen::VectorXd vecRed{};
   };
 
+  template <class T, class DirichletValuesType>
+  VectorFlatAssembler(T &&fes, const DirichletValuesType &dirichletValues_)
+      -> VectorFlatAssembler<T, DirichletValuesType>;
+
   /** SparseFlatAssembler assembles matrix quantities using a flat basis Indexing strategy
    * The matrix is stored in a sparse matrix format. This format is exploited during the assembly process
    */
-  template < typename FEContainer_,typename DirichletValuesType_>
+  template <typename FEContainer_, typename DirichletValuesType_>
   class SparseFlatAssembler : public VectorFlatAssembler<FEContainer_, DirichletValuesType_> {
-   public:
-    using FERequirementType = typename FEContainer_::value_type::FERequirementType;
-    using GlobalIndex     = typename FEContainer_::value_type::GlobalIndex;
-    using Basis = typename DirichletValuesType_::Basis;
-    using FEContainer = FEContainer_;
-    using DirichletValuesType = DirichletValuesType_;
+  public:
+    using FEContainerRaw = std::remove_cvref_t<FEContainer_>;
 
+    using FERequirementType   = typename FEContainerRaw::value_type::FERequirementType;
+    using GlobalIndex         = typename FEContainerRaw::value_type::GlobalIndex;
+    using Basis               = typename DirichletValuesType_::Basis;
+    using FEContainer         = FEContainer_;
+    using DirichletValuesType = DirichletValuesType_;
 
-    SparseFlatAssembler(const FEContainer &fes, const DirichletValuesType &dirichletValues_)
-        : VectorFlatAssembler<FEContainer,DirichletValuesType>(fes, dirichletValues_) {}
+    SparseFlatAssembler(FEContainer &&fes, const DirichletValuesType &dirichletValues_)
+        : VectorFlatAssembler<FEContainer, DirichletValuesType>(std::forward<FEContainer>(fes), dirichletValues_) {}
 
     using GridView = typename Basis::GridView;
 
     /** Calculates the matrix quantity which is requested by fErequirements and returns a reference
      * A zero is written on fixed dofs rows and columns and a one is written on the diagonal */
     Eigen::SparseMatrix<double> &getMatrix(const FERequirementType &fErequirements) {
       return getMatrixImpl(fErequirements);
@@ -188,27 +208,35 @@
     bool isReducedOccupationPatternCreated{false};
     bool arelinearDofsPerElementCreated{false};
     bool arelinearReducedDofsPerElementCreated{false};
     std::vector<std::vector<Eigen::Index>> elementLinearIndices;
     std::vector<std::vector<Eigen::Index>> elementLinearReducedIndices;
   };
 
+  template <class T, class DirichletValuesType>
+  SparseFlatAssembler(T &&fes, const DirichletValuesType &dirichletValues_)
+      -> SparseFlatAssembler<T, DirichletValuesType>;
+
   /** DenseFlatAssembler assembles matrix quantities using a flat basis Indexing strategy
    * The matrix is stored in a dense matrix format. This format is exploited during the assembly process
    */
-  template <typename FEContainer_,typename DirichletValuesType_ >  // requires Ikarus::Concepts::FlatIndexBasis<BasisEmbedded>
+  template <typename FEContainer_,
+            typename DirichletValuesType_>  // requires Ikarus::Concepts::FlatIndexBasis<BasisEmbedded>
   class DenseFlatAssembler : public VectorFlatAssembler<FEContainer_, DirichletValuesType_> {
   public:
-    using FERequirementType = typename FEContainer_::value_type::FERequirementType;
-    using GlobalIndex     = typename FEContainer_::value_type::GlobalIndex;
-    using Basis = typename DirichletValuesType_::Basis;
-    using FEContainer = FEContainer_;
+    using FEContainerRaw = std::remove_cvref_t<FEContainer_>;
+
+    using FERequirementType   = typename FEContainerRaw::value_type::FERequirementType;
+    using GlobalIndex         = typename FEContainerRaw::value_type::GlobalIndex;
+    using Basis               = typename DirichletValuesType_::Basis;
+    using FEContainer         = FEContainer_;
     using DirichletValuesType = DirichletValuesType_;
-    explicit DenseFlatAssembler(const FEContainer &fes, const DirichletValuesType &dirichletValues_)
-        : VectorFlatAssembler<FEContainer,DirichletValuesType >(fes, dirichletValues_) {}
+
+    explicit DenseFlatAssembler(FEContainer &&fes, const DirichletValuesType &dirichletValues_)
+        : VectorFlatAssembler<FEContainer, DirichletValuesType>(std::forward<FEContainer>(fes), dirichletValues_) {}
 
     /** Calculates the matrix quantity which is requested by fErequirements and returns a reference
      * A zero is written on fixed dofs rows and columns and a one is written on the diagonal */
     Eigen::MatrixXd &getMatrix(const FERequirementType &fErequirements) { return getMatrixImpl(fErequirements); }
 
     /** Calculates the matrix quantity which is requested by fErequirements and returns a reference
      * The size of the matrix has the size of the free degrees of freedom */
@@ -220,10 +248,15 @@
     Eigen::MatrixXd &getReducedMatrixImpl(const FERequirementType &fErequirements);
     Eigen::MatrixXd &getMatrixImpl(const FERequirementType &fErequirements);
 
     Eigen::MatrixXd mat{};
     Eigen::MatrixXd matRed{};
   };
 
+  // https://en.cppreference.com/w/cpp/language/class_template_argument_deduction
+  template <class T, class DirichletValuesType>
+  DenseFlatAssembler(T &&fes, const DirichletValuesType &dirichletValues_)
+      -> DenseFlatAssembler<T, DirichletValuesType>;
+
 }  // namespace Ikarus
 
 #include "simpleAssemblers.inl"
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.1.dev20230522071144/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 #include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/finiteElements/physicsHelper.hh>
 
 namespace Ikarus {
   ////This element can not be used on its own but it should be inherited from
   //// The class constructor can only be called from the templated class.
-  template <typename RealElement, typename Basis, typename FERequirementType_ = FErequirements<>, bool useEigenRef = false >
+  template <typename RealElement, typename Basis, typename FERequirementType_ = FErequirements<>,
+            bool useEigenRef = false>
   class AutoDiffFE {
   public:
-    using LocalView = typename Basis::LocalView;
-    using Traits    = TraitsFromLocalView<LocalView,useEigenRef>;
+    using LocalView   = typename Basis::LocalView;
+    using Traits      = TraitsFromLocalView<LocalView, useEigenRef>;
     using GridElement = typename LocalView::Element;
 
     using FERequirementType = FERequirementType_;
     void calculateMatrix(const FERequirementType& par, typename Traits::MatrixType h) const {
       Eigen::VectorXdual2nd dx(localDofSize);
       Eigen::VectorXd g;
       autodiff::dual2nd e;
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
       for (size_t i = 0; i < fe.size(); ++i) {
         for (int j = 0; j < num_children; ++j) {
           globalIndices.push_back(localView_.index((localView_.tree().child(j).localIndex(i))));
         }
       }
     }
 
-    const GridElementEntityType& getEntity() { return localView_.element(); }
+    const GridElementEntityType& gridElement() { return localView_.element(); }
     const LocalView& localView() const { return localView_; }
     LocalView& localView() { return localView_; }
 
   private:
     LocalView localView_;
   };
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feRequirements.hh`

 * *Files 12% similar despite different names*

```diff
@@ -8,66 +8,70 @@
 #include <set>
 #include <vector>
 
 #include <dune/common/exceptions.hh>
 
 #include <Eigen/Core>
 
+#include <ikarus/utils/makeEnum.hh>
+
 namespace Ikarus {
 
   // clang-format off
-  enum class ScalarAffordances {
+  MAKE_ENUM(ScalarAffordances,
     noAffordance,
     mechanicalPotentialEnergy,
     microMagneticPotentialEnergy
-  };
+  );
 
-  enum class VectorAffordances {
+  MAKE_ENUM(VectorAffordances,
     noAffordance,
     forces,
     microMagneticForces
-  };
+  );
 
-  enum class MatrixAffordances {
+  MAKE_ENUM(MatrixAffordances,
     noAffordance,
     stiffness,
     materialstiffness,
     geometricstiffness,
     stiffnessdiffBucklingVector,
     microMagneticHessian,
     mass
-  };
+  );
 
-  enum class FEParameter {
+  MAKE_ENUM(FEParameter,
     noParameter,
     loadfactor,
     time
-  };
+    );
 
-  enum class FESolutions {
+  MAKE_ENUM(FESolutions,
     noSolution,
     displacement,
     velocity,
     director,
     magnetizationAndVectorPotential
-  };
+  );
 
-  enum class ResultType {
+  MAKE_ENUM(ResultType,
     noType,
     magnetization,
     gradientNormOfMagnetization,
     vectorPotential,
     divergenceOfVectorPotential,
     BField,
     HField,
     cauchyStress,
+    PK2Stress,
+    linearStress,
     director
-  };
+  );
+
   // clang-format on
-  std::string getResultType(const ResultType &res);
 
   struct AffordanceCollectionImpl {
     ScalarAffordances scalarAffordances{ScalarAffordances::noAffordance};
     VectorAffordances vectorAffordances{VectorAffordances::noAffordance};
     MatrixAffordances matrixAffordances{MatrixAffordances::noAffordance};
   };
 
@@ -142,21 +146,29 @@
     const SolutionVectorTypeRaw &getGlobalSolution(const FESolutions &key) const {
       try {
         if constexpr (std::is_same_v<SolutionVectorType, std::reference_wrapper<Eigen::VectorXd>>)
           return sols.at(key).get();
         else
           return sols.at(key);
       } catch (std::out_of_range &oor) {
-        DUNE_THROW(Dune::RangeError,
-                   std::string("Out of Range error: ") + std::string(oor.what()) + " in getGlobalSolution");
+        DUNE_THROW(Dune::RangeError, std::string("Out of Range error: ") + std::string(oor.what())
+                                         + " in getGlobalSolution with key" + toString(key));
         abort();
       }
     }
 
-    const ParameterTypeRaw &getParameter(FEParameter &&key) const { return parameter.at(key).get(); }
+    const ParameterTypeRaw &getParameter(FEParameter &&key) const {
+      try {
+        return parameter.at(key).get();
+      } catch (std::out_of_range &oor) {
+        DUNE_THROW(Dune::RangeError, std::string("Out of Range error: ") + std::string(oor.what())
+                                         + " in getParameter with key" + toString(key));
+        abort();
+      }
+    }
 
     template <FEAffordance Affordance>
     bool hasAffordance(Affordance &&affordance) const {
       if constexpr (std::is_same_v<Affordance, ScalarAffordances>)
         return affordances.scalarAffordances == affordance;
       else if constexpr (std::is_same_v<Affordance, VectorAffordances>)
         return affordances.vectorAffordances == affordance;
@@ -176,43 +188,52 @@
   class ResultTypeMap {
   public:
     using ResultArray = Eigen::Matrix<double, Eigen::Dynamic, Eigen::Dynamic, 0, 3, 3>;
     void insertOrAssignResult(ResultType &&resultType, const ResultArray &resultArray) {
       results.insert_or_assign(resultType, resultArray);
     }
 
-    ResultArray &getResult(ResultType &&resultType) { return results.at(resultType); }
+    ResultArray &getResult(const ResultType &resultType) { return results.at(resultType); }
+
+    auto &getSingleResult() {
+      if (results.size() != 1)
+        DUNE_THROW(Dune::RangeError, "getSingleResult can only be called when a single result was inserted");
+      else
+        return *(results.begin());
+    }
 
   private:
     std::map<ResultType, ResultArray> results;
   };
 
   template <typename Type>
   concept ResultTypeConcept = std::is_same_v<Type, ResultType>;
 
   template <typename FErequirements = FErequirements<>>
   class ResultRequirements {
   public:
-    using ParameterType         = typename FErequirements::ParameterType;
+    using ParameterTypeRaw      = typename FErequirements::ParameterTypeRaw;
     using SolutionVectorType    = typename FErequirements::SolutionVectorType;
     using SolutionVectorTypeRaw = typename FErequirements::SolutionVectorTypeRaw;
 
     ResultRequirements(FErequirements &&req, std::set<ResultType> &&p_resType)
         : reqB{req}, resType(std::move(p_resType)) {}
 
+    explicit ResultRequirements(const FErequirements &req) : reqB{req} {}
+
     ResultRequirements() = default;
     bool isResultRequested(ResultType &&key) const { return resType.contains(key); }
 
     template <FEAffordance Affordance>
     ResultRequirements &addAffordance(Affordance &&affordance) {
       reqB.addAffordance(std::forward<Affordance>(affordance));
       return *this;
     }
 
-    ResultRequirements &insertParameter(FEParameter &&key, ParameterType &val) {
+    ResultRequirements &insertParameter(FEParameter &&key, ParameterTypeRaw &val) {
       reqB.insertParameter(std::forward<FEParameter>(key), val);
       return *this;
     }
 
     ResultRequirements &insertGlobalSolution(FESolutions &&key, SolutionVectorTypeRaw &sol) {
       reqB.insertGlobalSolution(std::forward<FESolutions>(key), sol);
       return *this;
@@ -224,17 +245,25 @@
       return *this;
     }
 
     const SolutionVectorTypeRaw &getGlobalSolution(FESolutions &&key) const {
       return reqB.getGlobalSolution(std::move(key));
     }
 
-    const ParameterType &getParameter(FEParameter &&key) const { return reqB.getParameter(std::move(key)); }
+    const ParameterTypeRaw &getParameter(FEParameter &&key) const { return reqB.getParameter(std::move(key)); }
 
     const FErequirements &getFERequirements() const { return reqB; }
 
+    auto getRequestedResult() const {
+      if (resType.size() == 1)
+        return *(resType.begin());
+      else {
+        DUNE_THROW(Dune::InvalidStateException, "This function can only be called when a single result is requested");
+      }
+    }
+
   private:
     std::set<ResultType> resType;
     FErequirements reqB;
   };
 
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files 2% similar despite different names*

```diff
@@ -255,18 +255,17 @@
     using FERequirementType      = typename DisplacementBasedElement::FERequirementType;
     using ResultRequirementsType = typename DisplacementBasedElement::ResultRequirementsType;
     using LocalView              = typename DisplacementBasedElement::LocalView;
     using GridView               = typename DisplacementBasedElement::GridView;
     using Traits                 = typename DisplacementBasedElement::Traits;
     using DisplacementBasedElement::localView;
 
-    template <typename ...Args>
-        explicit EnhancedAssumedStrains(Args&& ...args)
-        : DisplacementBasedElement(std::forward<Args>(args)...) {
-        setEASType(0);
+    template <typename... Args>
+    explicit EnhancedAssumedStrains(Args&&... args) : DisplacementBasedElement(std::forward<Args>(args)...) {
+      setEASType(0);
     }
 
     double calculateScalar(const FERequirementType& par) const {
       if (onlyDisplacementBase) return DisplacementBasedElement::calculateScalar(par);
       DUNE_THROW(Dune::NotImplemented,
                  "EAS element do not support any scalar calculations, i.e. they are not derivable from a potential");
       return 0.0;
@@ -341,29 +340,27 @@
 
             K.template triangularView<Eigen::Upper>() -= L.transpose() * D.inverse() * L;
             K.template triangularView<Eigen::StrictlyLower>() = K.transpose();
           },
           easVariant_);
     }
 
-    void calculateAt(const ResultRequirementsType& req, const Eigen::Vector<double, Traits::mydim>& local,
+    void calculateAt(const ResultRequirementsType& req, const Dune::FieldVector<double, Traits::mydim>& local,
                      ResultTypeMap<double>& result) const {
       using namespace Dune::Indices;
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
 
       DisplacementBasedElement::calculateAt(req, local, result);
 
       if (onlyDisplacementBase) return;
 
-      const auto& d             = req.getGlobalSolution(Ikarus::FESolutions::displacement);
-      const auto strainFunction = DisplacementBasedElement::getStrainFunction(req.getFERequirements());
-      const auto C              = DisplacementBasedElement::getMaterialTangentFunction(req.getFERequirements());
-      auto gpLocal              = toDune(local);
-      const auto& numNodes      = DisplacementBasedElement::numberOfNodes;
+      const auto& d        = req.getGlobalSolution(Ikarus::FESolutions::displacement);
+      const auto C         = DisplacementBasedElement::getMaterialTangentFunction(req.getFERequirements());
+      const auto& numNodes = DisplacementBasedElement::numberOfNodes;
 
       Eigen::VectorXd disp(localView().size());
       for (auto i = 0U; i < numNodes; ++i)
         for (auto k2 = 0U; k2 < Traits::mydim; ++k2)
           disp[i * Traits::mydim + k2] = d[localView().index(localView().tree().child(k2).localIndex(i))[0]];
 
       assert(((numNodes == 4 and Traits::mydim == 2) or (numNodes == 8 and Traits::mydim == 3))
@@ -371,22 +368,22 @@
 
       std::visit(
           [&]<typename EAST>(const EAST& easFunction) {
             constexpr int enhancedStrainSize = EAST::enhancedStrainSize;
             Eigen::Matrix<double, enhancedStrainSize, enhancedStrainSize> D;
             calculateDAndLMatrix(easFunction, req.getFERequirements(), D, L);
             const auto alpha = (-D.inverse() * L * disp).eval();
-            const auto M     = easFunction.calcM(gpLocal);
-            const auto CEval = C(gpLocal);
+            const auto M     = easFunction.calcM(local);
+            const auto CEval = C(local);
             auto easStress   = (CEval * M * alpha).eval();
             typename ResultTypeMap<double>::ResultArray resultVector;
-            if (req.isResultRequested(ResultType::cauchyStress)) {
+            if (req.isResultRequested(ResultType::linearStress)) {
               resultVector.resize(3, 1);
-              resultVector = result.getResult(ResultType::cauchyStress) + easStress;
-              result.insertOrAssignResult(ResultType::cauchyStress, resultVector);
+              resultVector = result.getResult(ResultType::linearStress) + easStress;
+              result.insertOrAssignResult(ResultType::linearStress, resultVector);
             }
           },
           easVariant_);
     }
 
     void setEASType(int numberOfEASParameters) {
       if constexpr (Traits::mydim == 2) {
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files 2% similar despite different names*

```diff
@@ -20,59 +20,53 @@
 
 #include <ikarus/finiteElements/feBases/autodiffFE.hh>
 #include <ikarus/finiteElements/feBases/powerBasisFE.hh>
 #include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/finiteElements/feTraits.hh>
 #include <ikarus/finiteElements/mechanics/materials.hh>
 #include <ikarus/finiteElements/physicsHelper.hh>
+#include <ikarus/utils/defaultFunctions.hh>
 #include <ikarus/utils/eigenDuneTransformations.hh>
 #include <ikarus/utils/linearAlgebraHelper.hh>
-#include <ikarus/utils/defaultFunctions.hh>
 
 namespace Ikarus {
 
-
   template <typename Basis_, typename FErequirements_ = FErequirements<>, bool useEigenRef = false>
   class LinearElastic : public PowerBasisFE<typename Basis_::FlatBasis> {
   public:
-    using Basis = Basis_;
-    using FlatBasis = typename Basis::FlatBasis;
+    using Basis                  = Basis_;
+    using FlatBasis              = typename Basis::FlatBasis;
     using BaseDisp               = PowerBasisFE<FlatBasis>;  // Handles globalIndices function
     using FERequirementType      = FErequirements_;
     using ResultRequirementsType = ResultRequirements<FERequirementType>;
     using LocalView              = typename FlatBasis::LocalView;
     using Element                = typename LocalView::Element;
     using GridView               = typename FlatBasis::GridView;
 
     using Traits = TraitsFromLocalView<LocalView, useEigenRef>;
 
     static constexpr int mydim = Traits::mydim;
 
     template <typename VolumeLoad = LoadDefault, typename NeumannBoundaryLoad = LoadDefault>
-        LinearElastic(const Basis& globalBasis, const typename LocalView::Element& element, double emod, double nu,
-                      VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* p_neumannBoundary = nullptr,
-                      NeumannBoundaryLoad p_neumannBoundaryLoad = {})
-        : BaseDisp(globalBasis.flat(), element),
-          neumannBoundary{p_neumannBoundary},
-          emod_{emod},
-          nu_{nu} {
+    LinearElastic(const Basis& globalBasis, const typename LocalView::Element& element, double emod, double nu,
+                  VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* p_neumannBoundary = nullptr,
+                  NeumannBoundaryLoad p_neumannBoundaryLoad = {})
+        : BaseDisp(globalBasis.flat(), element), neumannBoundary{p_neumannBoundary}, emod_{emod}, nu_{nu} {
       this->localView().bind(element);
       auto& first_child = this->localView().tree().child(0);
       const auto& fe    = first_child.finiteElement();
       numberOfNodes     = fe.size();
       dispAtNodes.resize(fe.size());
       const int order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
       localBasis      = Dune::CachedLocalBasis(this->localView().tree().child(0).finiteElement().localBasis());
       localBasis.bind(Dune::QuadratureRules<double, Traits::mydim>::rule(this->localView().element().type(), order),
                       Dune::bindDerivatives(0, 1));
 
-      if constexpr (!std::is_same_v<VolumeLoad,LoadDefault>)
-        volumeLoad =p_volumeLoad;
-      if constexpr (!std::is_same_v<NeumannBoundaryLoad,LoadDefault>)
-        neumannBoundaryLoad =p_neumannBoundaryLoad;
+      if constexpr (!std::is_same_v<VolumeLoad, LoadDefault>) volumeLoad = p_volumeLoad;
+      if constexpr (!std::is_same_v<NeumannBoundaryLoad, LoadDefault>) neumannBoundaryLoad = p_neumannBoundaryLoad;
 
       assert(((not p_neumannBoundary and not neumannBoundaryLoad) or (p_neumannBoundary and neumannBoundaryLoad))
              && "If you pass a Neumann boundary you should also pass the function for the Neumann load!");
     }
 
   public:
     //    const auto& localView() const { return localView(); }
@@ -142,16 +136,15 @@
 
           const double integrationElement = intersection.geometry().integrationElement(curQuad.position());
 
           // The value of the local function
           const auto uVal = u.evaluate(quadPos);
 
           // Value of the Neumann data at the current position
-          auto neumannValue
-              = neumannBoundaryLoad(toEigen(intersection.geometry().global(curQuad.position())), lambda);
+          auto neumannValue = neumannBoundaryLoad(toEigen(intersection.geometry().global(curQuad.position())), lambda);
 
           energy -= neumannValue.dot(uVal) * curQuad.weight() * integrationElement;
         }
       }
       return energy;
     }
 
@@ -171,32 +164,31 @@
             const auto bopJ = eps.evaluateDerivative(gpIndex, wrt(coeff(j)), on(gridElement));
             K.template block<mydim, mydim>(i * mydim, j * mydim) += bopI.transpose() * C * bopJ * intElement;
           }
         }
       }
     }
 
-    void calculateAt(const ResultRequirementsType& req, const Eigen::Vector<double, Traits::mydim>& local,
+    void calculateAt(const ResultRequirementsType& req, const Dune::FieldVector<double, Traits::mydim>& local,
                      ResultTypeMap<double>& result) const {
       using namespace Dune::Indices;
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
 
       const auto eps = getStrainFunction(req.getFERequirements());
       const auto C   = getMaterialTangent();
-      auto gp        = toDune(local);
-      auto epsVoigt  = eps.evaluate(gp, on(gridElement));
+      auto epsVoigt  = eps.evaluate(local, on(gridElement));
 
       auto cauchyStress = (C * epsVoigt).eval();
 
       typename ResultTypeMap<double>::ResultArray resultVector;
-      if (req.isResultRequested(ResultType::cauchyStress)) {
+      if (req.isResultRequested(ResultType::linearStress)) {
         resultVector.resize(3, 1);
         resultVector = cauchyStress;
-        result.insertOrAssignResult(ResultType::cauchyStress, resultVector);
+        result.insertOrAssignResult(ResultType::linearStress, resultVector);
       }
     }
 
     void calculateVector(const FERequirementType& par, typename Traits::VectorType force) const {
       const auto& lambda = par.getParameter(Ikarus::FEParameter::loadfactor);
       const auto eps     = getStrainFunction(par);
       using namespace Dune::DerivativeDirections;
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files 1% similar despite different names*

```diff
@@ -173,12 +173,11 @@
 
     MaterialImpl matImpl;
     double tol{};
   };
 
   template <Impl::StressIndexPair... stressIndexPair, typename MaterialImpl>
   auto makeVanishingStress(MaterialImpl mat, typename MaterialImpl::ScalarType p_tol = 1e-12) {
-
     return VanishingStress<std::to_array({stressIndexPair...}), MaterialImpl>(mat, p_tol);
   }
 
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files 10% similar despite different names*

```diff
@@ -24,34 +24,35 @@
 #include <ikarus/finiteElements/physicsHelper.hh>
 #include <ikarus/utils/eigenDuneTransformations.hh>
 #include <ikarus/utils/linearAlgebraHelper.hh>
 
 namespace Ikarus {
 
   template <typename Basis_, typename Material_, typename FErequirements_ = FErequirements<>, bool useEigenRef = false>
-  class NonLinearElastic
-      : public PowerBasisFE<typename Basis_::FlatBasis>,
-        public Ikarus::AutoDiffFE<NonLinearElastic<Basis_, Material_,FErequirements_,useEigenRef>, typename Basis_::FlatBasis,FErequirements_,useEigenRef> {
+  class NonLinearElastic : public PowerBasisFE<typename Basis_::FlatBasis>,
+                           public Ikarus::AutoDiffFE<NonLinearElastic<Basis_, Material_, FErequirements_, useEigenRef>,
+                                                     typename Basis_::FlatBasis, FErequirements_, useEigenRef> {
   public:
-    using Basis = Basis_;
-    using FlatBasis = typename Basis::FlatBasis;
-    using BaseDisp  = PowerBasisFE<FlatBasis>;  // Handles globalIndices function
-    using BaseAD    = Ikarus::AutoDiffFE<NonLinearElastic<Basis_, Material_,FErequirements_,useEigenRef>, typename Basis_::FlatBasis,FErequirements_,useEigenRef>;
-    using FERequirementType      = FErequirements_;
+    using Basis             = Basis_;
+    using FlatBasis         = typename Basis::FlatBasis;
+    using BaseDisp          = PowerBasisFE<FlatBasis>;  // Handles globalIndices function
+    using BaseAD            = Ikarus::AutoDiffFE<NonLinearElastic<Basis_, Material_, FErequirements_, useEigenRef>,
+                                      typename Basis_::FlatBasis, FErequirements_, useEigenRef>;
+    using LocalView         = typename FlatBasis::LocalView;
+    using Geometry          = typename LocalView::Element::Geometry;
+    using GridView          = typename FlatBasis::GridView;
+    using FERequirementType = FErequirements_;
 
     using ResultRequirementsType = ResultRequirements<FERequirementType>;
 
     using BaseAD::localView;
     using BaseAD::size;
     friend BaseAD;
-    using LocalView         = typename FlatBasis::LocalView;
-    using Element        = typename LocalView::Element;
-    using Geometry          = typename Element::Geometry;
-    using GridView          = typename FlatBasis::GridView;
-    using Material          = Material_;
+    using Element  = typename LocalView::Element;
+    using Material = Material_;
 
     template <typename VolumeLoad = LoadDefault, typename NeumannBoundaryLoad = LoadDefault>
     NonLinearElastic(const Basis& globalBasis, const typename LocalView::Element& element, const Material& p_mat,
                      VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* p_neumannBoundary = nullptr,
                      NeumannBoundaryLoad p_neumannBoundaryLoad = {})
         : BaseDisp(globalBasis.flat(), element),
           BaseAD(globalBasis.flat(), element),
@@ -59,24 +60,22 @@
           mat{p_mat} {
       this->localView().bind(element);
       const int order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
       localBasis      = Dune::CachedLocalBasis(this->localView().tree().child(0).finiteElement().localBasis());
       localBasis.bind(Dune::QuadratureRules<double, Traits::mydim>::rule(this->localView().element().type(), order),
                       Dune::bindDerivatives(0, 1));
 
-      if constexpr (!std::is_same_v<VolumeLoad,LoadDefault>)
-        volumeLoad =p_volumeLoad;
-      if constexpr (!std::is_same_v<NeumannBoundaryLoad,LoadDefault>)
-        neumannBoundaryLoad =p_neumannBoundaryLoad;
+      if constexpr (!std::is_same_v<VolumeLoad, LoadDefault>) volumeLoad = p_volumeLoad;
+      if constexpr (!std::is_same_v<NeumannBoundaryLoad, LoadDefault>) neumannBoundaryLoad = p_neumannBoundaryLoad;
 
       assert(((not p_neumannBoundary and not neumannBoundaryLoad) or (p_neumannBoundary and neumannBoundaryLoad))
-                 && "If you pass a Neumann boundary you should also pass the function for the Neumann load!");
+             && "If you pass a Neumann boundary you should also pass the function for the Neumann load!");
     }
 
-    using Traits = TraitsFromLocalView<LocalView,useEigenRef>;
+    using Traits = TraitsFromLocalView<LocalView, useEigenRef>;
 
   private:
     template <class ScalarType>
     ScalarType calculateScalarImpl(const FERequirementType& req, Eigen::VectorX<ScalarType>& dx) const {
       const auto& d      = req.getGlobalSolution(Ikarus::FESolutions::displacement);
       const auto& lambda = req.getParameter(Ikarus::FEParameter::loadfactor);
       using namespace Dune::DerivativeDirections;
@@ -102,15 +101,15 @@
         const auto EVoigt   = toVoigt(E);
         auto internalEnergy = matAD.template storedEnergy<StrainTags::greenLagrangian>(EVoigt);
         energy += internalEnergy * geo.integrationElement(gp.position()) * gp.weight();
       }
 
       if (volumeLoad) {
         for (const auto& [gpIndex, gp] : uFunction.viewOverIntegrationPoints()) {
-          const auto u                              = uFunction.evaluate(gpIndex);
+          const auto u                                 = uFunction.evaluate(gpIndex);
           Eigen::Vector<double, Traits::worlddim> fext = volumeLoad(toEigen(gp.position()), lambda);
           energy -= u.dot(fext) * geo.integrationElement(gp.position()) * gp.weight();
         }
       }
 
       const int order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
       // line or surface loads, i.e. neumann boundary
@@ -138,14 +137,45 @@
           energy -= neumannValue.dot(u) * curQuad.weight() * integrationElement;
         }
       }
 
       return energy;
     }
 
+  public:
+    void calculateAt(const ResultRequirementsType& req, const Dune::FieldVector<double, Traits::mydim>& local,
+                     ResultTypeMap<double>& result) const {
+      const auto& d      = req.getGlobalSolution(Ikarus::FESolutions::displacement);
+      const auto& lambda = req.getParameter(Ikarus::FEParameter::loadfactor);
+      using namespace Dune::DerivativeDirections;
+      using namespace Dune;
+      auto& first_child = this->localView().tree().child(0);
+      const auto& fe    = first_child.finiteElement();
+      Dune::BlockVector<RealTuple<double, Traits::dimension>> disp(fe.size());
+
+      for (auto i = 0U; i < fe.size(); ++i)
+        for (auto k2 = 0U; k2 < Traits::mydim; ++k2)
+          disp[i][k2] = d[this->localView().index(this->localView().tree().child(k2).localIndex(i))[0]];
+      const auto geo = this->localView().element().geometry();
+
+      Dune::StandardLocalFunction uFunction(localBasis, disp, std::make_shared<const Geometry>(geo));
+      const auto H      = uFunction.evaluateDerivative(local, Dune::wrt(spatialAll), Dune::on(gridElement));
+      const auto E      = (0.5 * (H.transpose() + H + H.transpose() * H)).eval();
+      const auto EVoigt = toVoigt(E);
+      auto PK2          = mat.template stresses<StrainTags::greenLagrangian>(EVoigt);
+
+      typename ResultTypeMap<double>::ResultArray resultVector;
+      if (req.isResultRequested(ResultType::PK2Stress)) {
+        resultVector.resizeLike(PK2);
+        resultVector = PK2;
+        result.insertOrAssignResult(ResultType::PK2Stress, resultVector);
+      }
+    }
+
+  private:
     Dune::CachedLocalBasis<
         std::remove_cvref_t<decltype(std::declval<LocalView>().tree().child(0).finiteElement().localBasis())>>
         localBasis;
     std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
                                                           const double&)>
         volumeLoad;
     std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 #pragma once
 #include <memory>
-#include <ikarus/utils/concepts.hh>
-#include <ikarus/utils/traits.hh>
 #include <type_traits>
 
 #include <dune/functions/backends/istlvectorbackend.hh>
 #include <dune/functions/functionspacebases/boundarydofs.hh>
 
 #include <autodiff/forward/real.hpp>
 #include <autodiff/forward/real/eigen.hpp>
 
+#include <ikarus/utils/concepts.hh>
+#include <ikarus/utils/traits.hh>
+
 namespace Ikarus {
 
   template <typename Basis_, typename FlagsType_ = std::vector<bool>>
   class DirichletValues {
   public:
     using Basis                         = std::remove_cvref_t<Basis_>;
     using FlagsType                     = FlagsType_;
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #pragma once
 #include <functional>
 
 #include <dune/common/hybridutilities.hh>
 
 #include <ikarus/utils/traits.hh>
 
-
 namespace Ikarus {
 
   namespace Impl {
     template <class F, class Tuple, std::size_t... I>
     constexpr decltype(auto) applyAndRemoveRefererenceWrapper(F&& f, Tuple&& t, std::index_sequence<I...>) {
       return std::invoke(
           std::forward<F>(f),
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
-#include <ikarus/finiteElements/feRequirements.hh>
-
 #include <dune/functions/functionspacebases/lagrangebasis.hh>
 #include <dune/functions/functionspacebases/powerbasis.hh>
 #include <dune/grid/yaspgrid.hh>
 #include <dune/python/common/typeregistry.hh>
 #include <dune/python/functions/globalbasis.hh>
 #include <dune/python/pybind11/eigen.h>
 #include <dune/python/pybind11/functional.h>
 #include <dune/python/pybind11/pybind11.h>
 #include <dune/python/pybind11/stl.h>
 #include <dune/python/pybind11/stl_bind.h>
+
+#include <ikarus/finiteElements/feRequirements.hh>
 // PYBIND11_MAKE_OPAQUE(std::vector<bool>);
 namespace Ikarus::Python {
 
   // Python wrapper for the FVAssembler C++ class
   template <class DirichletValues, class... options>
   void registerDirichletValues(pybind11::handle scope, pybind11::class_<DirichletValues, options...> cls) {
     using pybind11::operator""_a;
@@ -51,31 +51,34 @@
               self.fixBoundaryDOFs(lambda);
             });
 
     cls.def("fixBoundaryDOFsUsingLocalView",
             [](DirichletValues& self,
                const std::function<void(Eigen::Ref<Eigen::VectorX<bool>>, int, LocalViewWrapper&)>& f) {
               auto lambda = [&](BackendType& vec, int localIndex, LocalView& lv) {
-                auto lvWrapper       = LocalViewWrapper(lv.globalBasis());
-                //this can be simplified when https://gitlab.dune-project.org/staging/dune-functions/-/merge_requests/418 becomes available
+                auto lvWrapper = LocalViewWrapper(lv.globalBasis());
+                // this can be simplified when
+                // https://gitlab.dune-project.org/staging/dune-functions/-/merge_requests/418 becomes available
                 pybind11::object obj = pybind11::cast(lv.element());
                 lvWrapper.bind(obj);
                 f(vec.vector(), localIndex, lvWrapper);
               };
               self.fixBoundaryDOFs(lambda);
             });
 
     cls.def("fixBoundaryDOFsUsingLocalViewAndIntersection",
             [](DirichletValues& self,
-               const std::function<void(Eigen::Ref<Eigen::VectorX<bool>>, int, LocalViewWrapper&,const Intersection&)>& f) {
-              auto lambda = [&](BackendType& vec, int localIndex, LocalView& lv,const Intersection& intersection) {
-                auto lvWrapper       = LocalViewWrapper(lv.globalBasis());
-                //this can be simplified when https://gitlab.dune-project.org/staging/dune-functions/-/merge_requests/418 becomes available
+               const std::function<void(Eigen::Ref<Eigen::VectorX<bool>>, int, LocalViewWrapper&, const Intersection&)>&
+                   f) {
+              auto lambda = [&](BackendType& vec, int localIndex, LocalView& lv, const Intersection& intersection) {
+                auto lvWrapper = LocalViewWrapper(lv.globalBasis());
+                // this can be simplified when
+                // https://gitlab.dune-project.org/staging/dune-functions/-/merge_requests/418 becomes available
                 pybind11::object obj = pybind11::cast(lv.element());
                 lvWrapper.bind(obj);
-                f(vec.vector(), localIndex, lvWrapper,intersection);
+                f(vec.vector(), localIndex, lvWrapper, intersection);
               };
               self.fixBoundaryDOFs(lambda);
             });
   }
 
 }  // namespace Ikarus::Python
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/python/finiteElements/linearElastic.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,101 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
+#include <dune/fufem/boundarypatch.hh>
 #include <dune/functions/functionspacebases/lagrangebasis.hh>
 #include <dune/functions/functionspacebases/powerbasis.hh>
 #include <dune/grid/yaspgrid.hh>
 #include <dune/python/common/typeregistry.hh>
+#include <dune/python/functions/globalbasis.hh>
 #include <dune/python/pybind11/eigen.h>
+#include <dune/python/pybind11/functional.h>
 #include <dune/python/pybind11/pybind11.h>
 #include <dune/python/pybind11/stl.h>
-#include <dune/python/pybind11/functional.h>
-#include <dune/fufem/boundarypatch.hh>
 
 #include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/utils/basis.hh>
-#include <dune/python/functions/globalbasis.hh>
 
 namespace Ikarus::Python {
 
   template <class LinearElastic, class... options>
   void registerLinearElastic(pybind11::handle scope, pybind11::class_<LinearElastic, options...> cls) {
     using pybind11::operator""_a;
 
     using GlobalBasis    = typename LinearElastic::Basis;
-    using FlatBasis    = typename LinearElastic::FlatBasis;
-    using GridView    = typename GlobalBasis::GridView;
+    using FlatBasis      = typename LinearElastic::FlatBasis;
+    using GridView       = typename GlobalBasis::GridView;
     using Element        = typename LinearElastic::Element;
-    using Traits        = typename LinearElastic::Traits;
+    using Traits         = typename LinearElastic::Traits;
     using FErequirements = typename LinearElastic::FERequirementType;
 
     cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, double emod, double nu) {
               return new LinearElastic(basis, element, emod, nu);
             }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>());
 
-    using LoadFunction = std::function<Eigen::Vector<double, Traits::worlddim>(Eigen::Vector<double, Traits::worlddim>, const double&)>;
-    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, double emod, double nu,const LoadFunction volumeLoad) {
-              return new LinearElastic(basis, element, emod, nu,volumeLoad);
-            }),
+    using LoadFunction = std::function<Eigen::Vector<double, Traits::worlddim>(Eigen::Vector<double, Traits::worlddim>,
+                                                                               const double&)>;
+    cls.def(pybind11::init(
+                [](const GlobalBasis& basis, const Element& element, double emod, double nu,
+                   const LoadFunction volumeLoad) { return new LinearElastic(basis, element, emod, nu, volumeLoad); }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>());
 
-    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, double emod, double nu,const LoadFunction volumeLoad,const BoundaryPatch<GridView>& bp
-                              ,const LoadFunction neumannBoundaryLoad) {
-              return new LinearElastic(basis, element, emod, nu,volumeLoad,&bp,neumannBoundaryLoad);
+    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, double emod, double nu,
+                              const LoadFunction volumeLoad, const BoundaryPatch<GridView>& bp,
+                              const LoadFunction neumannBoundaryLoad) {
+              return new LinearElastic(basis, element, emod, nu, volumeLoad, &bp, neumannBoundaryLoad);
             }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>(), pybind11::keep_alive<1, 7>());
 
     pybind11::module scopedf = pybind11::module::import("dune.functions");
 
-    typedef Dune::Python::LocalViewWrapper< FlatBasis > LocalViewWrapper;
+    typedef Dune::Python::LocalViewWrapper<FlatBasis> LocalViewWrapper;
     auto includes = Dune::Python::IncludeFiles{"dune/python/functions/globalbasis.hh"};
-    auto lv = Dune::Python::insertClass< LocalViewWrapper >( scopedf, "LocalViewWrapper",
-    Dune::Python::GenerateTypeName("Dune::Python::LocalViewWrapperWrapper", Dune::MetaType<FlatBasis>()),
-        includes).first;
-    lv.def( "bind", &LocalViewWrapper::bind );
-    lv.def( "unbind", &LocalViewWrapper::unbind );
-    lv.def( "index", [] ( const LocalViewWrapper &localView, int index ) { return localView.index( index ); });
-    lv.def( "__len__", [] ( LocalViewWrapper &self ) -> int { return self.size(); } );
+    auto lv       = Dune::Python::insertClass<LocalViewWrapper>(
+                  scopedf, "LocalViewWrapper",
+                  Dune::Python::GenerateTypeName("Dune::Python::LocalViewWrapperWrapper", Dune::MetaType<FlatBasis>()),
+                  includes)
+                  .first;
+    lv.def("bind", &LocalViewWrapper::bind);
+    lv.def("unbind", &LocalViewWrapper::unbind);
+    lv.def("index", [](const LocalViewWrapper& localView, int index) { return localView.index(index); });
+    lv.def("__len__", [](LocalViewWrapper& self) -> int { return self.size(); });
 
     Dune::Python::Functions::registerTree<typename LocalViewWrapper::Tree>(lv);
     lv.def("tree", [](const LocalViewWrapper& view) { return view.tree(); });
 
-    auto basisName =Dune::className<FlatBasis>();
-    auto entry = Dune::Python::insertClass<FlatBasis>(scopedf, "DefaultGlobalBasis", pybind11::buffer_protocol(),
-                                                  Dune::Python::GenerateTypeName(basisName),Dune::Python::IncludeFiles{"dune/python/functions/globalbasis.hh"}
-    );
-    if (entry.second)
-      Dune::Python::registerGlobalBasis(scopedf,entry.first);
+    auto basisName = Dune::className<FlatBasis>();
+    auto entry     = Dune::Python::insertClass<FlatBasis>(
+        scopedf, "DefaultGlobalBasis", pybind11::buffer_protocol(), Dune::Python::GenerateTypeName(basisName),
+        Dune::Python::IncludeFiles{"dune/python/functions/globalbasis.hh"});
+    if (entry.second) Dune::Python::registerGlobalBasis(scopedf, entry.first);
 
     cls.def(
-        "localView", [](LinearElastic& self) -> LocalViewWrapper{
+        "localView",
+        [](LinearElastic& self) -> LocalViewWrapper {
           auto lvWrapped = LocalViewWrapper(self.localView().globalBasis());
-          //this can be simplified when https://gitlab.dune-project.org/staging/dune-functions/-/merge_requests/418 becomes available
+          // this can be simplified when https://gitlab.dune-project.org/staging/dune-functions/-/merge_requests/418
+          // becomes available
           pybind11::object obj = pybind11::cast(self.localView().element());
           lvWrapped.bind(obj);
-          return lvWrapped; } , pybind11::keep_alive< 0, 1 >());
+          return lvWrapped;
+        },
+        pybind11::keep_alive<0, 1>());
     cls.def("calculateScalar",
             [](LinearElastic& self, const FErequirements& req) { return self.calculateScalar(req); });
     cls.def("calculateVector", [](LinearElastic& self, const FErequirements& req, Eigen::Ref<Eigen::VectorXd> vec) {
       return self.calculateVector(req, vec);
     });
     cls.def(
         "calculateMatrix",
         [](LinearElastic& self, const FErequirements& req, Eigen::Ref<Eigen::MatrixXd> mat) {
           return self.calculateMatrix(req, mat);
         },
         pybind11::arg("FErequirements"), pybind11::arg("elementMatrix").noconvert());
 
     cls.def("getMaterialTangent", [](LinearElastic& self) { return self.getMaterialTangent(); });
-
   }
 
 }  // namespace Ikarus::Python
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
-#include <ikarus/finiteElements/feRequirements.hh>
-
 #include <dune/fufem/boundarypatch.hh>
 #include <dune/functions/functionspacebases/lagrangebasis.hh>
 #include <dune/functions/functionspacebases/powerbasis.hh>
 #include <dune/grid/yaspgrid.hh>
 #include <dune/python/common/typeregistry.hh>
 #include <dune/python/functions/globalbasis.hh>
 #include <dune/python/pybind11/eigen.h>
 #include <dune/python/pybind11/functional.h>
 #include <dune/python/pybind11/pybind11.h>
 #include <dune/python/pybind11/stl.h>
+
+#include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/utils/basis.hh>
 
 namespace Ikarus::Python {
 
   template <class NonLinearElastic, class... options>
   void registerNonLinearElastic(pybind11::handle scope, pybind11::class_<NonLinearElastic, options...> cls) {
     using pybind11::operator""_a;
 
     using GlobalBasis    = typename NonLinearElastic::Basis;
-    using FlatBasis    = typename NonLinearElastic::FlatBasis;
+    using FlatBasis      = typename NonLinearElastic::FlatBasis;
     using GridView       = typename GlobalBasis::GridView;
     using Element        = typename NonLinearElastic::Element;
     using Traits         = typename NonLinearElastic::Traits;
     using FErequirements = typename NonLinearElastic::FERequirementType;
     using Material       = typename NonLinearElastic::Material;
 
     cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, const Material& mat) {
@@ -54,20 +54,19 @@
             }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>(), pybind11::keep_alive<1, 7>());
 
     pybind11::module scopedf = pybind11::module::import("dune.functions");
 
     typedef Dune::Python::LocalViewWrapper<FlatBasis> LocalViewWrapper;
     auto includes = Dune::Python::IncludeFiles{"dune/python/functions/globalbasis.hh"};
-    auto lv
-        = Dune::Python::insertClass<LocalViewWrapper>(
-              scopedf, "LocalViewWrapper",
-              Dune::Python::GenerateTypeName("Dune::Python::LocalViewWrapperWrapper", Dune::MetaType<FlatBasis>()),
-              includes)
-              .first;
+    auto lv       = Dune::Python::insertClass<LocalViewWrapper>(
+                  scopedf, "LocalViewWrapper",
+                  Dune::Python::GenerateTypeName("Dune::Python::LocalViewWrapperWrapper", Dune::MetaType<FlatBasis>()),
+                  includes)
+                  .first;
     lv.def("bind", &LocalViewWrapper::bind);
     lv.def("unbind", &LocalViewWrapper::unbind);
     lv.def("index", [](const LocalViewWrapper& localView, int index) { return localView.index(index); });
     lv.def("__len__", [](LocalViewWrapper& self) -> int { return self.size(); });
 
     Dune::Python::Functions::registerTree<typename LocalViewWrapper::Tree>(lv);
     lv.def("tree", [](const LocalViewWrapper& view) { return view.tree(); });
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.1.dev20230522071144/ikarus/python/test/linearElasticTest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,123 @@
 # SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 import setpath
+
 setpath.set_path()
 import ikarus as iks
 import ikarus.finite_elements
 import ikarus.utils
 import ikarus.assembler
 import ikarus.dirichletValues
 import numpy as np
 import scipy as sp
 
 import dune.grid
 import dune.functions
-from dune.vtk import vtkUnstructuredGridWriter, vtkWriter, RangeTypes, FieldInfo
+from dune.vtk import vtkWriter
 
 if __name__ == "__main__":
-    svk = iks.StVenantKirchhoff(emodul=1000,nu=0.3)
-
-    svkPS = svk.asPlaneStress()
-    # help(iks)
     lowerLeft = []
     upperRight = []
     elements = []
     for i in range(2):
         lowerLeft.append(-1)
         upperRight.append(1)
         elements.append(3)
 
-    req= ikarus.FErequirements()
+    req = ikarus.FErequirements()
     req.addAffordance(iks.ScalarAffordances.mechanicalPotentialEnergy)
 
-    grid = dune.grid.structuredGrid(lowerLeft,upperRight,elements)
-    grid. hierarchicalGrid . globalRefine(6)
-    basisLagrange12 = dune.functions.defaultGlobalBasis(grid, dune.functions.Power(dune.functions.Lagrange(order=1),2))
+    grid = dune.grid.structuredGrid(lowerLeft, upperRight, elements)
+    grid.hierarchicalGrid.globalRefine(6)
+    basisLagrange12 = dune.functions.defaultGlobalBasis(
+        grid, dune.functions.Power(dune.functions.Lagrange(order=1), 2)
+    )
     dirichletValuesT = iks.dirichletValues(basisLagrange12)
 
-    basisLagrange1 = iks.basis(grid, dune.functions.Power(dune.functions.Lagrange(order=1),2))
+    basisLagrange1 = iks.basis(
+        grid, dune.functions.Power(dune.functions.Lagrange(order=1), 2)
+    )
     flatBasis = basisLagrange1.flat()
     d = np.zeros(len(flatBasis))
-    d[0]=0.0
+    d[0] = 0.0
 
     lambdaLoad = iks.ValueWrapper(3.0)
-    req.insertParameter(iks.FEParameter.loadfactor,lambdaLoad)
+    req.insertParameter(iks.FEParameter.loadfactor, lambdaLoad)
 
     assert req.getParameter(iks.FEParameter.loadfactor) == lambdaLoad
-    req.insertGlobalSolution(iks.FESolutions.displacement,d)
+    req.insertGlobalSolution(iks.FESolutions.displacement, d)
 
-    d2= req.getGlobalSolution(iks.FESolutions.displacement)
+    d2 = req.getGlobalSolution(iks.FESolutions.displacement)
 
-    assert ('{}'.format(hex(d2.__array_interface__['data'][0]))) == ('{}'.format(hex(d.__array_interface__['data'][0])))
-    assert len(d2)== len(d)
-    assert (d2== d).all()
+    assert ("{}".format(hex(d2.__array_interface__["data"][0]))) == (
+        "{}".format(hex(d.__array_interface__["data"][0]))
+    )
+    assert len(d2) == len(d)
+    assert (d2 == d).all()
     fes = []
-    forces = np.zeros(8)
-    stiffness = np.zeros((8,8))
 
-    def volumeLoad(x,lambdaVal) :
-        return np.array([lambdaVal*x[0]*2, 2*lambdaVal*x[1]*0])
+    def volumeLoad(x, lambdaVal):
+        return np.array([lambdaVal * x[0] * 2, 2 * lambdaVal * x[1] * 0])
 
-    def neumannLoad(x,lambdaVal) :
-        return np.array([lambdaVal*0, lambdaVal])
+    def neumannLoad(x, lambdaVal):
+        return np.array([lambdaVal * 0, lambdaVal])
 
+    neumannVertices = np.zeros(grid.size(2) * 2, dtype=bool)
+    assert len(neumannVertices) == len(flatBasis)
 
-    neumannVertices = np.zeros(grid.size(2)*2, dtype=bool)
-    assert len(neumannVertices)== len(flatBasis)
+    flatBasis.interpolate(neumannVertices, lambda x: True if x[1] > 0.9 else False)
 
-    flatBasis.interpolate(neumannVertices, lambda x :  True  if x[1]>0.9 else False)
-
-    boundaryPatch = iks.utils.boundaryPatch(grid,neumannVertices)
+    boundaryPatch = iks.utils.boundaryPatch(grid, neumannVertices)
 
     # the following should throw
     try:
         for e in grid.elements:
-            iks.finite_elements.linearElasticElement(basisLagrange1,e,1000,0.2,volumeLoad,boundaryPatch)
+            iks.finite_elements.linearElasticElement(
+                basisLagrange1, e, 1000, 0.2, volumeLoad, boundaryPatch
+            )
         assert False
-    except TypeError :
+    except TypeError:
         pass
 
     for e in grid.elements:
-        fes.append(iks.finite_elements.linearElasticElement(basisLagrange1,e,1000,0.2,volumeLoad,boundaryPatch,neumannLoad))
+        fes.append(
+            iks.finite_elements.linearElasticElement(
+                basisLagrange1, e, 1000, 0.2, volumeLoad, boundaryPatch, neumannLoad
+            )
+        )
 
-    fes[0].calculateVector(req,forces)
-    fes[0].calculateMatrix(req,stiffness)
+    forces = np.zeros(8)
+    stiffness = np.zeros((8, 8))
+    fes[0].calculateVector(req, forces)
+    fes[0].calculateMatrix(req, stiffness)
     fes[0].localView()
 
     dirichletValues = iks.dirichletValues(flatBasis)
 
-    def fixFirstIndex(vec,globalIndex):
-        vec[0]= True
+    def fixFirstIndex(vec, globalIndex):
+        vec[0] = True
 
-    def fixAnotherVertex(vec,localIndex,localView):
+    def fixAnotherVertex(vec, localIndex, localView):
         localView.index(localIndex)
-        vec[1]= True
+        vec[1] = True
 
-    def fixLeftHandEdge(vec,localIndex,localView,intersection):
-        if (intersection.geometry.center[1]<-0.9):
-            vec[localView.index(localIndex)]= True
+    def fixLeftHandEdge(vec, localIndex, localView, intersection):
+        if intersection.geometry.center[1] < -0.9:
+            vec[localView.index(localIndex)] = True
 
     dirichletValues.fixBoundaryDOFs(fixFirstIndex)
     dirichletValues.fixBoundaryDOFsUsingLocalView(fixAnotherVertex)
     dirichletValues.fixBoundaryDOFsUsingLocalViewAndIntersection(fixLeftHandEdge)
 
-    assembler = iks.assembler.sparseFlatAssembler(fes,dirichletValues)
-    assemblerDense = iks.assembler.denseFlatAssembler(fes,dirichletValues)
+    assembler = iks.assembler.sparseFlatAssembler(fes, dirichletValues)
+    assemblerDense = iks.assembler.denseFlatAssembler(fes, dirichletValues)
 
     Msparse = assembler.getMatrix(req)
     forces = assembler.getVector(req)
-    # Mdense = assemblerDense.getMatrix(req)
-    # assert (Msparse == Mdense).all()
-    # print(Mdense)
-    # print("F:",forces)
 
-    x = sp.sparse.linalg.spsolve(Msparse,-forces)
-    # print(x)
+    x = sp.sparse.linalg.spsolve(Msparse, -forces)
     fx = flatBasis.asFunction(x)
     grid.plot()
-    # grid.writeVTK(pointdata={"fx":fx},name="nameTest",number=1)
-    writer = vtkWriter( grid, "nameTest",
-                    pointData   = {( "displacement",(0,1)):fx}
 
-                    )
+    writer = vtkWriter(grid, "nameTest", pointData={("displacement", (0, 1)): fx})
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.1.dev20230522071144/ikarus/python/test/nonLinearElasticTest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,138 @@
 # SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 import setpath
+
 setpath.set_path()
 import ikarus as iks
 import ikarus.finite_elements
 import ikarus.utils
 import ikarus.assembler
 import ikarus.dirichletValues
 import numpy as np
 import scipy as sp
 from scipy.optimize import minimize
 
 import dune.grid
 import dune.functions
-from dune.vtk import vtkUnstructuredGridWriter, vtkWriter, RangeTypes, FieldInfo
 
 if __name__ == "__main__":
-
-    # help(iks)
     lowerLeft = []
     upperRight = []
     elements = []
     for i in range(2):
         lowerLeft.append(-1)
         upperRight.append(1)
         elements.append(3)
 
-    req= ikarus.FErequirements()
+    req = ikarus.FErequirements()
     req.addAffordance(iks.ScalarAffordances.mechanicalPotentialEnergy)
 
-    grid = dune.grid.structuredGrid(lowerLeft,upperRight,elements)
-    grid. hierarchicalGrid.globalRefine(0)
-    basisLagrange1 = ikarus.basis(grid, dune.functions.Power(dune.functions.Lagrange(order=1),2))
+    grid = dune.grid.structuredGrid(lowerLeft, upperRight, elements)
+    grid.hierarchicalGrid.globalRefine(0)
+    basisLagrange1 = ikarus.basis(
+        grid, dune.functions.Power(dune.functions.Lagrange(order=1), 2)
+    )
     flatBasis = basisLagrange1.flat()
 
-
     forces = np.zeros(8)
-    stiffness = np.zeros((8,8))
-
-    def volumeLoad(x,lambdaVal) :
-        return np.array([lambdaVal*x[0]*2, 2*lambdaVal*x[1]*0])
+    stiffness = np.zeros((8, 8))
 
-    def neumannLoad(x,lambdaVal) :
-        return np.array([lambdaVal*0, lambdaVal])
+    def volumeLoad(x, lambdaVal):
+        return np.array([lambdaVal * x[0] * 2, 2 * lambdaVal * x[1] * 0])
 
+    def neumannLoad(x, lambdaVal):
+        return np.array([lambdaVal * 0, lambdaVal])
 
-    neumannVertices = np.zeros(grid.size(2)*2, dtype=bool)
-    assert len(neumannVertices)== len(flatBasis)
+    neumannVertices = np.zeros(grid.size(2) * 2, dtype=bool)
+    assert len(neumannVertices) == len(flatBasis)
 
-    flatBasis.interpolate(neumannVertices, lambda x :  True  if x[1]>0.9 else False)
+    flatBasis.interpolate(neumannVertices, lambda x: True if x[1] > 0.9 else False)
 
-    boundaryPatch = iks.utils.boundaryPatch(grid,neumannVertices)
+    boundaryPatch = iks.utils.boundaryPatch(grid, neumannVertices)
 
-    svk = iks.StVenantKirchhoff(emodul=1000,nu=0.3)
+    svk = iks.StVenantKirchhoff(emodul=1000, nu=0.3)
 
     psNH = svk.asPlaneStress()
     fes = []
     for e in grid.elements:
-        fes.append(iks.finite_elements.nonLinearElasticElement(basisLagrange1,e,psNH,volumeLoad,boundaryPatch,neumannLoad))
+        fes.append(
+            iks.finite_elements.nonLinearElasticElement(
+                basisLagrange1, e, psNH, volumeLoad, boundaryPatch, neumannLoad
+            )
+        )
 
     dirichletValues = iks.dirichletValues(flatBasis)
 
-    def fixFirstIndex(vec,globalIndex):
-        vec[0]= True
+    def fixFirstIndex(vec, globalIndex):
+        vec[0] = True
 
-    def fixAnotherVertex(vec,localIndex,localView):
+    def fixAnotherVertex(vec, localIndex, localView):
         localView.index(localIndex)
-        vec[1]= True
+        vec[1] = True
 
-    def fixLeftHandEdge(vec,localIndex,localView,intersection):
-        if (intersection.geometry.center[1]<-0.9):
-            vec[localView.index(localIndex)]= True
+    def fixLeftHandEdge(vec, localIndex, localView, intersection):
+        if intersection.geometry.center[1] < -0.9:
+            vec[localView.index(localIndex)] = True
 
     dirichletValues.fixBoundaryDOFs(fixFirstIndex)
     dirichletValues.fixBoundaryDOFsUsingLocalView(fixAnotherVertex)
     dirichletValues.fixBoundaryDOFsUsingLocalViewAndIntersection(fixLeftHandEdge)
 
-    assembler = iks.assembler.sparseFlatAssembler(fes,dirichletValues)
+    assembler = iks.assembler.sparseFlatAssembler(fes, dirichletValues)
 
     dRed = np.zeros(assembler.reducedSize())
 
     lambdaLoad = iks.ValueWrapper(3.0)
-    def energy(dRedInput) :
-        global assembler
 
-        reqL= ikarus.FErequirements()
+    def energy(dRedInput):
+        reqL = ikarus.FErequirements()
         reqL.addAffordance(iks.ScalarAffordances.mechanicalPotentialEnergy)
-        reqL.insertParameter(iks.FEParameter.loadfactor,lambdaLoad)
+        reqL.insertParameter(iks.FEParameter.loadfactor, lambdaLoad)
 
         dBig = assembler.createFullVector(dRedInput)
-        reqL.insertGlobalSolution(iks.FESolutions.displacement,dBig)
+        reqL.insertGlobalSolution(iks.FESolutions.displacement, dBig)
         return assembler.getScalar(reqL)
-    def gradient(dRedInput) :
-        global assembler
 
-        reqL= ikarus.FErequirements()
+    def gradient(dRedInput):
+        reqL = ikarus.FErequirements()
         reqL.addAffordance(iks.VectorAffordances.forces)
-        reqL.insertParameter(iks.FEParameter.loadfactor,lambdaLoad)
+        reqL.insertParameter(iks.FEParameter.loadfactor, lambdaLoad)
 
         dBig = assembler.createFullVector(dRedInput)
-        reqL.insertGlobalSolution(iks.FESolutions.displacement,dBig)
+        reqL.insertGlobalSolution(iks.FESolutions.displacement, dBig)
         return assembler.getReducedVector(reqL)
-    def hess(dRedInput) :
-        global assembler
 
-        reqL= ikarus.FErequirements()
+    def hess(dRedInput):
+        reqL = ikarus.FErequirements()
         reqL.addAffordance(iks.MatrixAffordances.stiffness)
-        reqL.insertParameter(iks.FEParameter.loadfactor,lambdaLoad)
+        reqL.insertParameter(iks.FEParameter.loadfactor, lambdaLoad)
 
         dBig = assembler.createFullVector(dRedInput)
-        reqL.insertGlobalSolution(iks.FESolutions.displacement,dBig)
+        reqL.insertGlobalSolution(iks.FESolutions.displacement, dBig)
         return assembler.getReducedMatrix(reqL).todense()
 
-    print("energy(dRed):",energy(dRed))
+    print("energy(dRed):", energy(dRed))
     print("energyafer")
-    resultd = minimize(energy,x0=dRed,options={"disp": True},tol=1e-14)
-    resultd2 = minimize(energy,x0=dRed,jac=gradient,options={"disp": True},tol=1e-14)
-    resultd3 = minimize(energy,method="trust-constr",x0=dRed,jac=gradient,hess=hess,options={ 'disp': True})
-    resultd4 = sp.optimize.root(gradient,jac=hess,x0=dRed,options={ 'disp': True},tol=1e-10)
+    resultd = minimize(energy, x0=dRed, options={"disp": True}, tol=1e-14)
+    resultd2 = minimize(
+        energy, x0=dRed, jac=gradient, options={"disp": True}, tol=1e-14
+    )
+    resultd3 = minimize(
+        energy,
+        method="trust-constr",
+        x0=dRed,
+        jac=gradient,
+        hess=hess,
+        options={"disp": True},
+    )
+    resultd4 = sp.optimize.root(
+        gradient, jac=hess, x0=dRed, options={"disp": True}, tol=1e-10
+    )
     # print(assembler.createFullVector(resultd.g))
     np.set_printoptions(precision=3)
 
-    assert(np.allclose(resultd.x,resultd2.x,atol=1e-6))
-    assert(np.allclose(resultd3.x,resultd4.x))
-    assert(np.all(abs(resultd3.grad)<1e-8))
-    assert(np.all(abs(resultd4.fun)<1e-8))
+    assert np.allclose(resultd.x, resultd2.x, atol=1e-6)
+    assert np.allclose(resultd3.x, resultd4.x)
+    assert np.all(abs(resultd3.grad) < 1e-8)
+    assert np.all(abs(resultd4.fun) < 1e-8)
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.1.dev20230522071144/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/python/utils/boundarypatch.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
 #include <dune/python/pybind11/eigen.h>
+#include <dune/python/pybind11/functional.h>
 #include <dune/python/pybind11/pybind11.h>
 #include <dune/python/pybind11/stl.h>
-#include <dune/python/pybind11/functional.h>
 
 #include <ikarus/finiteElements/feRequirements.hh>
 
 namespace Ikarus::Python {
 
   // Python wrapper for the FVAssembler C++ class
   template <class BoundaryPatch, class... options>
   void registerBoundaryPatch(pybind11::handle scope, pybind11::class_<BoundaryPatch, options...> cls) {
     using pybind11::operator""_a;
 
-    using GridView    = typename BoundaryPatch::GridView;
+    using GridView = typename BoundaryPatch::GridView;
 
     cls.def(pybind11::init([](const GridView& gv, Eigen::Ref<Eigen::VectorX<bool>> vec) {
               Dune::BitSetVector<1> bitSetVector;
               bitSetVector.resize(vec.size());
-              for(size_t i=0; i< vec.size();++i)
-                bitSetVector[i]=vec[i];
-              return new BoundaryPatch(gv,bitSetVector);
+              for (size_t i = 0; i < vec.size(); ++i)
+                bitSetVector[i] = vec[i];
+              return new BoundaryPatch(gv, bitSetVector);
             }),
-            pybind11::keep_alive<1, 2>(),pybind11::keep_alive<1, 3>());
-
+            pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>());
   }
 
 }  // namespace Ikarus::Python
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #pragma once
 #include <iosfwd>
 
 #include <ikarus/linearAlgebra/nonLinearOperator.hh>
 #include <ikarus/solver/linearSolver/linearSolver.hh>
 #include <ikarus/utils/defaultFunctions.hh>
 #include <ikarus/utils/linearAlgebraHelper.hh>
-
 #include <ikarus/utils/observer/observer.hh>
 #include <ikarus/utils/observer/observerMessages.hh>
 
 namespace Ikarus {
 
   struct NewtonRaphsonSettings {
     double tol{1e-8};
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/algorithms.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/basis.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/basis.hh`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 
 #include <ikarus/utils/flatPreBasis.hh>
 
 namespace Ikarus {
   template <typename PreBasis_>
   class Basis {
   public:
-    using PreBasis     = PreBasis_;
-    using GridView     = typename PreBasis::GridView;
+    using PreBasis       = PreBasis_;
+    using GridView       = typename PreBasis::GridView;
     using UntouchedBasis = decltype(Dune::Functions::DefaultGlobalBasis(std::declval<PreBasis>()));
-    using FlatBasis    = decltype(Dune::Functions::DefaultGlobalBasis(Ikarus::flatPreBasis(std::declval<PreBasis>())));
+    using FlatBasis = decltype(Dune::Functions::DefaultGlobalBasis(Ikarus::flatPreBasis(std::declval<PreBasis>())));
 
-    explicit Basis(const PreBasis& pb) : bb{Dune::Functions::DefaultGlobalBasis(pb)}, fb{Dune::Functions::DefaultGlobalBasis(Ikarus::flatPreBasis(pb))} {}
+    explicit Basis(const PreBasis& pb)
+        : bb{Dune::Functions::DefaultGlobalBasis(pb)},
+          fb{Dune::Functions::DefaultGlobalBasis(Ikarus::flatPreBasis(pb))} {}
 
     auto& flat() { return fb; }
 
     auto& untouched() { return bb; }
 
     const auto& flat() const { return fb; }
 
@@ -36,12 +38,12 @@
   };
 
   template <typename GridView, typename PreBasisFactory>
   auto makeBasis(const GridView& gv, const PreBasisFactory& pb) {
     return Basis(pb(gv));
   }
 
-template < typename PreBasis>
-auto makeBasis(const Dune::Functions::DefaultGlobalBasis<PreBasis>& gb) {
+  template <typename PreBasis>
+  auto makeBasis(const Dune::Functions::DefaultGlobalBasis<PreBasis>& gb) {
     return Basis(gb.preBasis());
-}
+  }
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/concepts.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/init.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/polyfit.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/ikarus/utils/traits.hh` & `pyikarus-0.3.1.dev20230522071144/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/python/ikarus/__init__.py` & `pyikarus-0.3.1.dev20230522071144/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/python/ikarus/_ikarus.cc` & `pyikarus-0.3.1.dev20230522071144/python/ikarus/_ikarus.cc`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
-#include <ikarus/finiteElements/feRequirements.hh>
-#include <ikarus/python/finiteElements/materials/material.hh>
-
 #include <dune/common/float_cmp.hh>
 #include <dune/python/common/typeregistry.hh>
 #include <dune/python/pybind11/eigen.h>
 #include <dune/python/pybind11/operators.h>
 #include <dune/python/pybind11/pybind11.h>
 
+#include <ikarus/finiteElements/feRequirements.hh>
+#include <ikarus/python/finiteElements/materials/material.hh>
+
 // since python does not support passing python float by reference to a double&, we have to wrap everything
 // see also https://pybind11.readthedocs.io/en/stable/faq.html#limitations-involving-reference-arguments
-template<typename T>
-struct ValueWrapper
-{
+template <typename T>
+struct ValueWrapper {
   T val;
-  ValueWrapper operator+(const ValueWrapper &v) const { return ValueWrapper{val + v.val}; }
-  ValueWrapper operator-(const ValueWrapper &v) const { return ValueWrapper{val - v.val}; }
-  ValueWrapper operator-() const  {  return ValueWrapper{-val}; }
+  ValueWrapper operator+(const ValueWrapper& v) const { return ValueWrapper{val + v.val}; }
+  ValueWrapper operator-(const ValueWrapper& v) const { return ValueWrapper{val - v.val}; }
+  ValueWrapper operator-() const { return ValueWrapper{-val}; }
   ValueWrapper operator*(T value) const { return ValueWrapper{val * value}; }
-  ValueWrapper& operator+=(const ValueWrapper &v) { val += v.val;  return *this; }
-  ValueWrapper& operator*=(T v) { val *= v; return *this; }
-
-  friend ValueWrapper operator*(T f, const ValueWrapper &v) {
-    return ValueWrapper{f * v.val};
+  ValueWrapper& operator+=(const ValueWrapper& v) {
+    val += v.val;
+    return *this;
   }
+  ValueWrapper& operator*=(T v) {
+    val *= v;
+    return *this;
+  }
+
+  friend ValueWrapper operator*(T f, const ValueWrapper& v) { return ValueWrapper{f * v.val}; }
 };
 
 PYBIND11_MODULE(_ikarus, m) {
   namespace py = pybind11;
   using namespace pybind11::literals;
   using namespace Ikarus;
   using namespace Eigen;
@@ -105,9 +108,9 @@
       [](FEreq& self, FEParameter parType, ValueWrapper<double>& parVal) {
         self.insertParameter(std::move(parType), parVal.val);
       },
       py::keep_alive<1, 3>(), "FEParameter"_a, "parameterValue"_a.noconvert());
 
   lv.def("getParameter", [](const FEreq& self, FEParameter parType) { return self.getParameter(std::move(parType)); });
 
-//  MAKE_MATERIAL_CLASS_IN_MODULE(StVenantKirchhoff,double);
+  //  MAKE_MATERIAL_CLASS_IN_MODULE(StVenantKirchhoff,double);
 }
```

### Comparing `pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.1.dev20230522071144/python/pyikarus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000087
+Version: 0.3.1.dev20230522071144
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
@@ -20,14 +20,15 @@
 [![Debian](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml)
 [![codecov](https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus)
 [![CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml)
 [![Docs](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/repository/github/ikarus-project/ikarus/overview/main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/ikarus/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ikarus-project/ikarus&amp;utm_campaign=Badge_Grade)
 [![Gitter](https://badges.gitter.im/ikarus-project/community.svg)](https://gitter.im/ikarus-project/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![PyPI version](https://badge.fury.io/py/pyikarus.svg)](https://badge.fury.io/py/pyikarus)
 
 
 [![Release](https://badgen.net/badge/Release/0.3/purple?icon=github)](https://github.com/ikarus-project/ikarus/releases)
 [![Doi](https://img.shields.io/badge/DOI-10.18419%2Fdarus--3303-orange)](https://doi.org/10.18419/darus-3303)
 [![SWH](https://archive.softwareheritage.org/badge/origin/https://github.com/ikarus-project/ikarus/)](https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/ikarus-project/ikarus)
 [![SWHRelease](https://archive.softwareheritage.org/badge/swh:1:rel:2cbfacc591c5fa48bdc84b375e42d1ab5304425f/)](https://archive.softwareheritage.org/swh:1:rel:2cbfacc591c5fa48bdc84b375e42d1ab5304425f;origin=https://github.com/ikarus-project/ikarus;visit=swh:1:snp:22424908ab42ab0d38be84c34235b8b5ae7af6c4)
```

#### html2text {}

```diff
@@ -1,37 +1,39 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000087 Home-page:
-Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
-Classifier: Programming Language :: C++ Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
-(GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
-File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
-actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
-ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
-project/ikarus/branch/main/graph/badge.svg?token=zJgggitPMc)](https://
-codecov.io/gh/ikarus-project/ikarus) [![CodeStyle](https://github.com/ikarus-
-project/ikarus/actions/workflows/style.yml/badge.svg)](https://github.com/
-ikarus-project/ikarus/actions/workflows/style.yml) [![Docs](https://github.com/
-ikarus-project/ikarus/actions/workflows/ghpages.yml/badge.svg)](https://
-github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml) [![CodeFactor]
-(https://www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)]
-(https://www.codefactor.io/repository/github/ikarus-project/ikarus/overview/
-main) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/
-5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/
-ikarus/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ikarus-
-project/ikarus&utm_campaign=Badge_Grade) [![Gitter](https://badges.gitter.im/
-ikarus-project/community.svg)](https://gitter.im/ikarus-project/
-community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![Release]
-(https://badgen.net/badge/Release/0.3/purple?icon=github)](https://github.com/
-ikarus-project/ikarus/releases) [![Doi](https://img.shields.io/badge/DOI-
-10.18419%2Fdarus--3303-orange)](https://doi.org/10.18419/darus-3303) [![SWH]
-(https://archive.softwareheritage.org/badge/origin/https://github.com/ikarus-
-project/ikarus/)](https://archive.softwareheritage.org/browse/origin/
-?origin_url=https://github.com/ikarus-project/ikarus) [![SWHRelease](https://
-archive.softwareheritage.org/badge/swh:1:rel:
-2cbfacc591c5fa48bdc84b375e42d1ab5304425f/)](https://
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.1.dev20230522071144 Home-
+page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
+stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
+Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
+markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
+ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
+github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
+(https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/
+badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus) [!
+[CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/
+style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/
+workflows/style.yml) [![Docs](https://github.com/ikarus-project/ikarus/actions/
+workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/
+actions/workflows/ghpages.yml) [![CodeFactor](https://www.codefactor.io/
+repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/
+repository/github/ikarus-project/ikarus/overview/main) [![Codacy Badge](https:/
+/app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://
+www.codacy.com/gh/ikarus-project/ikarus/
+dashboard?utm_source=github.com&utm_medium=referral&utm_content=ikarus-project/
+ikarus&utm_campaign=Badge_Grade) [![Gitter](https://badges.gitter.im/ikarus-
+project/community.svg)](https://gitter.im/ikarus-project/
+community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![PyPI
+version](https://badge.fury.io/py/pyikarus.svg)](https://badge.fury.io/py/
+pyikarus) [![Release](https://badgen.net/badge/Release/0.3/purple?icon=github)]
+(https://github.com/ikarus-project/ikarus/releases) [![Doi](https://
+img.shields.io/badge/DOI-10.18419%2Fdarus--3303-orange)](https://doi.org/
+10.18419/darus-3303) [![SWH](https://archive.softwareheritage.org/badge/origin/
+https://github.com/ikarus-project/ikarus/)](https://
+archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/
+ikarus-project/ikarus) [![SWHRelease](https://archive.softwareheritage.org/
+badge/swh:1:rel:2cbfacc591c5fa48bdc84b375e42d1ab5304425f/)](https://
 archive.softwareheritage.org/swh:1:rel:
 2cbfacc591c5fa48bdc84b375e42d1ab5304425f;origin=https://github.com/ikarus-
 project/ikarus;visit=swh:1:snp:22424908ab42ab0d38be84c34235b8b5ae7af6c4) This
 project tries to provide an easy to read and an easy to use finite element
 framework. It is heavily inspired by the finite element software [DUNE](https:/
 /dune-project.org/), the book [DUNE â The Distributed and Unified Numerics
 Environment](https://www.springer.com/gp/book/9783030597016), [deal.II](https:/
```

### Comparing `pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.1.dev20230522071144/python/pyikarus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,36 +9,35 @@
 README.md
 codecov.yml
 codespellignore
 config.h.cmake
 dune.module
 ikarus.pc.in
 iwyu.imp
-logfile
 pyproject.toml
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/codespell.yml
 .github/workflows/createDockerContainer.yml
 .github/workflows/createRelease.yml
 .github/workflows/debian-coverage.yml
 .github/workflows/debian.yml
 .github/workflows/ghpages.yml
+.github/workflows/releasePythonPackage.yml
 .github/workflows/reuseLint.yml
 .github/workflows/runExamples.yml
 .github/workflows/style.yml
+.github/workflows/scripts/release.py
 .reuse/dep5
 LICENSES/CC-BY-SA-4.0.txt
 LICENSES/CC0-1.0.txt
 LICENSES/LGPL-3.0-or-later.txt
 LICENSES/MIT.txt
 LICENSES/MPL-2.0.txt
-Testing/Temporary/CTestCostData.txt
-Testing/Temporary/LastTest.log
 cmake/CMakeLists.txt
 cmake/CPM.cmake
 cmake/tools.cmake
 cmake/FormatTarget/CMakeLists.txt
 cmake/modules/AddAutoDiffFlags.cmake
 cmake/modules/AddEigenFlags.cmake
 cmake/modules/AddMatplotppFlags.cmake
@@ -121,15 +120,14 @@
 ikarus/assembler/simpleAssemblers.hh
 ikarus/assembler/simpleAssemblers.inl
 ikarus/controlRoutines/CMakeLists.txt
 ikarus/controlRoutines/loadControl.hh
 ikarus/controlRoutines/pathFollowingTechnique.hh
 ikarus/finiteElements/CMakeLists.txt
 ikarus/finiteElements/fEparameter.hh
-ikarus/finiteElements/feRequirements.cpp
 ikarus/finiteElements/feRequirements.hh
 ikarus/finiteElements/feTraits.hh
 ikarus/finiteElements/physicsHelper.hh
 ikarus/finiteElements/feBases/CMakeLists.txt
 ikarus/finiteElements/feBases/autodiffFE.hh
 ikarus/finiteElements/feBases/powerBasisFE.hh
 ikarus/finiteElements/feBases/scalarFE.hh
@@ -142,14 +140,17 @@
 ikarus/finiteElements/mechanics/materials/interface.hh
 ikarus/finiteElements/mechanics/materials/linearElasticity.hh
 ikarus/finiteElements/mechanics/materials/neohooke.hh
 ikarus/finiteElements/mechanics/materials/strainConversions.hh
 ikarus/finiteElements/mechanics/materials/svk.hh
 ikarus/finiteElements/mechanics/materials/tags.hh
 ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+ikarus/io/CMakeLists.txt
+ikarus/io/resultEvaluators.hh
+ikarus/io/resultFunction.hh
 ikarus/linearAlgebra/CMakeLists.txt
 ikarus/linearAlgebra/dirichletValues.hh
 ikarus/linearAlgebra/nonLinearOperator.hh
 ikarus/linearAlgebra/truncatedConjugateGradient.hh
 ikarus/python/CMakeLists.txt
 ikarus/python/assembler/CMakeLists.txt
 ikarus/python/assembler/flatAssembler.hh
@@ -160,15 +161,14 @@
 ikarus/python/finiteElements/CMakeLists.txt
 ikarus/python/finiteElements/linearElastic.hh
 ikarus/python/finiteElements/nonLinearElastic.hh
 ikarus/python/finiteElements/materials/CMakeLists.txt
 ikarus/python/finiteElements/materials/material.hh
 ikarus/python/test/CMakeLists.txt
 ikarus/python/test/linearElasticTest.py
-ikarus/python/test/nameTest.vtu
 ikarus/python/test/nonLinearElasticTest.py
 ikarus/python/test/setpath.py.in
 ikarus/python/utils/CMakeLists.txt
 ikarus/python/utils/boundarypatch.hh
 ikarus/solver/CMakeLists.txt
 ikarus/solver/linearSolver/CMakeLists.txt
 ikarus/solver/linearSolver/linearSolver.hh
@@ -214,14 +214,15 @@
 python/CMakeLists.txt
 python/setup.py.in
 python/ikarus/CMakeLists.txt
 python/ikarus/__init__.py
 python/ikarus/_ikarus.cc
 python/ikarus/basis.py
 python/ikarus/dirichletValues.py
+python/ikarus/generator.py
 python/ikarus/materials.py
 python/ikarus/assembler/CMakeLists.txt
 python/ikarus/assembler/__init__.py
 python/ikarus/finite_elements/CMakeLists.txt
 python/ikarus/finite_elements/__init__.py
 python/ikarus/utils/CMakeLists.txt
 python/ikarus/utils/__init__.py
```

### Comparing `pyikarus-0.3.0.dev202310000087/python/setup.py.in` & `pyikarus-0.3.1.dev20230522071144/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.1.dev20230522071144/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.1.dev20230522071144/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/setup.py` & `pyikarus-0.3.1.dev20230522071144/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,24 @@
 try:
     from dune.packagemetadata import metaData
 except ImportError:
     from packagemetadata import metaData
 from skbuild import setup
 
 # When building a new package, update the version numbers below and run:
-# acess docker container with mounted repo to /tmp/Ikarus
+# access  docker container with mounted repo to /tmp/Ikarus
 # build _ikarus
 # cd /tmp/Ikarus
-#  /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
+# /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
-# > /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
+# /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-
-ikarusVersion = "0.3.0.dev202310000087" #+ datetime.today().time().strftime("%H%M%S")
+ikarusVersion = "0.3.1.dev20230522071144"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
-# refactor sicne ikarus pypi package already exists
-print(metadata)
-# metadata["name"] = "ikarus"
+# refactor since ikarus pypi package already exists
 metadata["name"] = "pyikarus"
-#for key in metadata["packages"]:
-#    key.replace("ikarus","pyikarus")
-
-# from setuptools import setup, find_packages
-print(metadata)
-
 setup(**metadata)
```

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/CMakeLists.txt` & `pyikarus-0.3.1.dev20230522071144/tests/src/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 find_dependency(autodiff REQUIRED)
 find_dependency(Matplot++ REQUIRED)
 
 file(GLOB programSourceFiles CONFIGURE_DEPENDS *.cpp)
 
 foreach(programSourceFile ${programSourceFiles})
   get_filename_component(programName ${programSourceFile} NAME_WLE)
-  dune_add_test(SOURCES ${programSourceFile} LINK_LIBRARIES ikarus LABELS
-          cpp)
+  dune_add_test(SOURCES ${programSourceFile} LINK_LIBRARIES ikarus LABELS cpp)
   target_compile_features(${programName} PUBLIC cxx_std_20)
   set_tests_properties(${programName} PROPERTIES TIMEOUT 1000)
   add_dune_pythonlibs_flags(${programName})
   find_package(PythonLibs REQUIRED)
   include_directories(${PYTHON_INCLUDE_DIRS})
   target_link_libraries(${programName} PUBLIC ${PYTHON_LIBRARIES})
   target_compile_options(${programName} PUBLIC -ftemplate-backtrace-limit=0)
```

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/assemblerTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/assemblerTest.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 #include <dune/functions/functionspacebases/basistags.hh>
 #include <dune/functions/functionspacebases/boundarydofs.hh>
 #include <dune/functions/functionspacebases/lagrangebasis.hh>
 #include <dune/functions/functionspacebases/powerbasis.hh>
 #include <dune/grid/yaspgrid.hh>
 
 using Dune::TestSuite;
+#include <Eigen/Core>
+
 #include <ikarus/assembler/simpleAssemblers.hh>
 #include <ikarus/finiteElements/mechanics/nonLinearElastic.hh>
 #include <ikarus/linearAlgebra/dirichletValues.hh>
 #include <ikarus/utils/basis.hh>
 #include <ikarus/utils/init.hh>
 
-#include <Eigen/Core>
-
 auto SimpleAssemblersTest() {
   TestSuite t("SimpleAssemblersTest");
   using Grid = Dune::YaspGrid<2>;
 
   Dune::FieldVector<double, 2> bbox       = {4, 2};
   std::array<int, 2> elementsPerDirection = {2, 1};
   auto grid                               = std::make_shared<Grid>(bbox, elementsPerDirection);
@@ -46,15 +46,15 @@
       Eigen::Vector2d fext;
       fext.setZero();
       fext[1] = 2 * lamb;
       fext[0] = lamb;
       return fext;
     };
     for (auto&& ge : elements(gridView))
-      fes.emplace_back(basis, ge, reducedMat,volumeLoad);
+      fes.emplace_back(basis, ge, reducedMat, volumeLoad);
 
     auto basisP = std::make_shared<const decltype(basis)>(basis);
     Ikarus::DirichletValues dirichletValues(basisP->flat());
     dirichletValues.fixDOFs([](auto& basis_, auto& dirichletFlags) {
       Dune::Functions::forEachBoundaryDOF(basis_, [&](auto&& indexGlobal) { dirichletFlags[indexGlobal] = true; });
     });
```

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/common.hh` & `pyikarus-0.3.1.dev20230522071144/tests/src/common.hh`

 * *Files 2% similar despite different names*

```diff
@@ -166,32 +166,31 @@
                        {1214.2857144055, 214.2857142945, 384.6153847400},
                        {214.2857142945, 1214.2857144055, 384.6153845600},
                        {214.2857143245, 214.2857143245, 384.6153846200}}};
   }
 
   auto resultRequirements = Ikarus::ResultRequirements<>()
                                 .insertGlobalSolution(Ikarus::FESolutions::displacement, displacement)
-                                .addResultRequest(ResultType::cauchyStress);
+                                .addResultRequest(ResultType::linearStress);
 
   ResultTypeMap<double> result;
   auto gridView        = fe.localView().globalBasis().gridView();
   auto scalarBasis     = makeConstSharedBasis(gridView, lagrangeDG<1>());
   auto localScalarView = scalarBasis->localView();
   std::vector<Dune::FieldVector<double, 3>> stressVector(scalarBasis->size());
   auto ele = elements(gridView).begin();
 
   localScalarView.bind(*ele);
   const auto& fe2              = localScalarView.tree().finiteElement();
   const auto& referenceElement = Dune::ReferenceElements<double, gridDim>::general(ele->type());
   for (auto c = 0UL; c < fe2.size(); ++c) {
     const auto fineKey                        = fe2.localCoefficients().localKey(c);
     const auto nodalPositionInChildCoordinate = referenceElement.position(fineKey.subEntity(), fineKey.codim());
-    auto coord                                = toEigen(nodalPositionInChildCoordinate);
-    fe.calculateAt(resultRequirements, coord, result);
-    Eigen::Vector3d computedResult = result.getResult(ResultType::cauchyStress).eval();
+    fe.calculateAt(resultRequirements, nodalPositionInChildCoordinate, result);
+    Eigen::Vector3d computedResult = result.getResult(ResultType::linearStress);
     const auto nodeIndex           = localScalarView.index(localScalarView.tree().localIndex(c))[0];
     stressVector[nodeIndex]        = toDune(computedResult);
     for (auto voigtIndex = 0UL; voigtIndex < 3; ++voigtIndex) {
       const auto FEStressComponent       = stressVector[nodeIndex][voigtIndex];
       const auto expectedStressComponent = expectedStress[c][voigtIndex];
       const bool isStressCorrect
           = Dune::FloatCmp::eq<double, Dune::FloatCmp::CmpStyle::absolute>(FEStressComponent, expectedStressComponent);
```

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/dependenciesTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/dependenciesTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/dirichletValueTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/dirichletValueTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/easTest.hh` & `pyikarus-0.3.1.dev20230522071144/tests/src/easTest.hh`

 * *Files 20% similar despite different names*

```diff
@@ -39,18 +39,22 @@
         t.subTest(checkJacobianOfElement(subOp, messageIfFailed));
 
         auto stiffnessMatrix = subOp.derivative();
 
         Eigen::SelfAdjointEigenSolver<Eigen::MatrixXd> es(stiffnessMatrix);
         newEigenValues = es.eigenvalues();
 
-        t.check((newEigenValues.array() < 1e-5 * newEigenValues.norm()).count() == 3 * gridDim - 3)
-            << "We always should have 3 or 6 zero eigenvalues, for 3 or 6 rigid body motions"
-               "\nEigenValues: \n"
-            << newEigenValues.transpose() << std::endl;
+        t.check((newEigenValues.array() < 1e-6 * newEigenValues.norm()).count() == 3 * gridDim - 3,
+                "Number of eigenvalues")
+            << "We always should have " << 3 * gridDim - 3 << " zero eigenvalues, for " << 3 * gridDim - 3
+            << " rigid body motions"
+            << " but we counted " << (newEigenValues.array() < 1e-6 * newEigenValues.norm()).count()
+            << "\nEigenValues: \n"
+            << newEigenValues.transpose() << "The tolerance is " << 1e-6 * newEigenValues.norm()
+            << "The number of EAS parameters is" << numberOfEASParameter << std::endl;
         if (numberOfEASParameter > 0 and numberOfEASParameter != 5)          // Q1E4 and Q1E5 are the same
           t.check((newEigenValues.array() <= oldEigenValues.array()).sum())  // Q1E4 and Q1E7 are the same in the case
                                                                              // of undistorted element
               << "More EAS parameter mean that the stiffness gets reduced. EAS parameter: " << numberOfEASParameter
               << "\noldEigenValues: \n"
               << oldEigenValues.transpose() << "\nnewEigenValues: \n"
               << newEigenValues.transpose() << std::endl;
@@ -73,14 +77,26 @@
                   MIntegrated += M * detJ * gp.weight();
                 }
                 t.check(MIntegrated.isZero())
                     << "Orthogonality condition check: The M matrix of the EAS method should be "
                        "zero, integrated over the domain.";
               },
               easVariant);
+          try {
+            auto requirements = Ikarus::FErequirements();
+            fe.calculateScalar(requirements);
+            t.check(false) << "fe.calculateScalar should have failed for numberOfEASParameter > 0";
+          } catch (const Dune::NotImplemented&) {
+          }
+        }
+
+        try {
+          fe.setEASType(100);
+          t.check(false) << "fe.setEASType(100) should have failed";
+        } catch (const Dune::NotImplemented&) {
         }
       };
       return t;
     };
     return easFunctor;
   }
 };
```

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/enhancedAssumedStrainsTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/enhancedAssumedStrainsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/factories.hh` & `pyikarus-0.3.1.dev20230522071144/tests/src/factories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/functionTraitsTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/functionTraitsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/linearElasticityTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/linearElasticityTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/manifoldsTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/manifoldsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/materialTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/materialTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTestNeoHooke.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/nonLinearElasticityTestNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTestSVK.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/nonLinearElasticityTestSVK.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
-//
 #include <config.h>
 
 #include "common.hh"
 #include "nonLinearElasticityTest.hh"
 #include "testHelpers.hh"
 
+#include <dune/python/pybind11/stl_bind.h>
+
+#include "ikarus/finiteElements/mechanics/linearElastic.hh"
 using Dune::TestSuite;
 
 int main(int argc, char** argv) {
   Ikarus::init(argc, argv);
   TestSuite t;
 
   auto matParameter = Ikarus::toLamesFirstParameterAndShearModulus({.emodul = 1000, .nu = 0.3});
 
   Ikarus::StVenantKirchhoff matSVK(matParameter);
-
   t.subTest(NonLinearElasticityLoadControlNRandTR<Grids::Alu>(matSVK));
   t.subTest(NonLinearElasticityLoadControlNRandTR<Grids::Yasp>(matSVK));
   t.subTest(NonLinearElasticityLoadControlNRandTR<Grids::Iga>(matSVK));
   return t.exit();
 }
```

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/nonLinearOperatorTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/nonLinearOperatorTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/pathFollowingTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/pathFollowingTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/polyFitTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/polyFitTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/pythonConversionTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/pythonConversionTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/testFEElement.hh` & `pyikarus-0.3.1.dev20230522071144/tests/src/testFEElement.hh`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 #include "common.hh"
 
 #include <dune/common/bitsetvector.hh>
 #include <dune/fufem/boundarypatch.hh>
 #include <dune/grid/uggrid.hh>
 
+#include "ikarus/io/resultFunction.hh"
 #include <ikarus/assembler/simpleAssemblers.hh>
 #include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/linearAlgebra/dirichletValues.hh>
 #include <ikarus/linearAlgebra/nonLinearOperator.hh>
 #include <ikarus/utils/basis.hh>
 
 /** These tests test your element on some gridElement with some basis
@@ -22,16 +23,16 @@
  * @tparam PreBasis The preBasis you want to test the element with
  * @tparam F A variadic number of the test functor you want to be checked, they need to accept a non-linear operator and
  * the finite element
  */
 template <template <typename> typename FEElementTemplate, int gridDim, typename PreBasis, typename... F>
 auto testFEElement(const PreBasis& preBasis, const std::string& elementName, const bool& isRandomlyDistorted,
                    F&&... f) {
-  Dune::TestSuite t(std::string("testFEElement ") + elementName + " on grid element with dimension"
-                    + std::to_string(gridDim) + ".");
+  Dune::TestSuite t(std::string("testFEElement ") + elementName + " on grid element with dimension "
+                    + std::to_string(gridDim));
 
   auto fTuple = std::forward_as_tuple(f...);
 
   using Grid = Dune::UGGrid<gridDim>;
 
   std::vector<Dune::FieldVector<double, gridDim>> corners;
 
@@ -89,33 +90,31 @@
   fes.emplace_back(basis, *element, youngsModulus, poissonsRatio, volumeLoad, &neumannBoundary, neumannBoundaryLoad);
   auto basisP = std::make_shared<const decltype(basis)>(basis);
 
   Ikarus::DirichletValues dirichletValues(basisP->flat());
   auto& fe             = fes[0];
   auto sparseAssembler = SparseFlatAssembler(fes, dirichletValues);
 
+  static_assert(std::is_reference_v<typename decltype(sparseAssembler)::FEContainerType>);
+
   typename FEElementType::FERequirementType::SolutionVectorTypeRaw d;
   d.setRandom(basis.flat().size());
 
   double lambda = 7.3;
 
   auto requirements = FErequirements()
                           .insertParameter(Ikarus::FEParameter::loadfactor, lambda)
                           .addAffordance(Ikarus::AffordanceCollections::elastoStatics);
-  Eigen::VectorXd forces;
-  Eigen::MatrixXd stiffnessmatrix;
 
   auto fvLambda = [&](auto&& d_) -> auto {
-    forces.setZero(flatBasis.localView().maxSize());
     requirements.insertGlobalSolution(Ikarus::FESolutions::displacement, d_);
     return sparseAssembler.getScalar(requirements);
   };
 
   auto dfvLambda = [&](auto&& d_) -> auto& {
-    forces.setZero(flatBasis.localView().maxSize());
     requirements.insertGlobalSolution(Ikarus::FESolutions::displacement, d_);
     return sparseAssembler.getVector(requirements);
   };
   auto ddfvLambda = [&](auto&& d_) -> auto& {
     requirements.insertGlobalSolution(Ikarus::FESolutions::displacement, d_);
     return sparseAssembler.getMatrix(requirements);
   };
@@ -126,14 +125,21 @@
   Dune::Hybrid::forEach(Dune::Hybrid::integralRange(Dune::index_constant<sizeof...(F)>()),
                         [&](auto i) { t.subTest(std::get<i.value>(fTuple)(nonLinOp, fe)); });
 
   // check if element has a test functor, if yes we execute it
   if constexpr (requires { ElementTest<FEElementType>::test(); }) {
     auto testFunctor = ElementTest<FEElementType>::test();
     t.subTest(testFunctor(nonLinOp, fe));
+  } else
+    spdlog::info("No element test functor found for {}", Dune::className<FEElementType>());
+
+  // Trying to instantiate the Result Evaluator
+  if constexpr (gridDim == 2) {
+    auto resReq         = Ikarus::ResultRequirements(requirements).addResultRequest(ResultType::PK2Stress);
+    auto resultFunction = std::make_shared<ResultFunction<FEElementType>>(&fes, resReq);
   }
 
   return t;
 }
 
 auto checkGradientFunctor = [](auto& nonLinOp, [[maybe_unused]] auto& fe) { return checkGradientOfElement(nonLinOp); };
 auto checkHessianFunctor  = [](auto& nonLinOp, [[maybe_unused]] auto& fe) { return checkHessianOfElement(nonLinOp); };
```

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.1.dev20230522071144/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.1.dev20230522071144/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.1.dev20230522071144/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/testHelpers.hh` & `pyikarus-0.3.1.dev20230522071144/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000087/tests/src/trustRegionTest.cpp` & `pyikarus-0.3.1.dev20230522071144/tests/src/trustRegionTest.cpp`

 * *Files identical despite different names*

