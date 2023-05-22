# Comparing `tmp/pyikarus-0.3.1.dev20230522182134.tar.gz` & `tmp/pyikarus-0.3.2.dev20230522090628.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.1.dev20230522182134.tar", last modified: Mon May 22 18:21:35 2023, max compression
+gzip compressed data, was "pyikarus-0.3.2.dev20230522090628.tar", last modified: Mon May 22 09:06:28 2023, max compression
```

## Comparing `pyikarus-0.3.1.dev20230522182134.tar` & `pyikarus-0.3.2.dev20230522090628.tar`

### file list

```diff
@@ -1,331 +1,331 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.205355 pyikarus-0.3.1.dev20230522182134/
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.bettercodehub.yml
--rw-r--r--   0 root         (0) root         (0)     1300 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.clang-format
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.cmake-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.141354 pyikarus-0.3.1.dev20230522182134/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.153354 pyikarus-0.3.1.dev20230522182134/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      615 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.157354 pyikarus-0.3.1.dev20230522182134/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1034 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 root         (0) root         (0)     5830 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/createRelease.yml
--rw-r--r--   0 root         (0) root         (0)     1834 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2612 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     2042 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/ghpages.yml
--rw-r--r--   0 root         (0) root         (0)     1711 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/reuseLint.yml
--rw-r--r--   0 root         (0) root         (0)     3045 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/runExamples.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.157354 pyikarus-0.3.1.dev20230522182134/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3071 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.157354 pyikarus-0.3.1.dev20230522182134/.reuse/
--rw-r--r--   0 root         (0) root         (0)      661 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)     3440 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1251 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5335 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.157354 pyikarus-0.3.1.dev20230522182134/LICENSES/
--rw-r--r--   0 root         (0) root         (0)    18375 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 root         (0) root         (0)     7048 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/LICENSES/MIT.txt
--rw-r--r--   0 root         (0) root         (0)    16727 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3732 2023-05-22 18:21:35.205355 pyikarus-0.3.1.dev20230522182134/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3321 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.157354 pyikarus-0.3.1.dev20230522182134/cmake/
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      973 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.161354 pyikarus-0.3.1.dev20230522182134/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1875 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.161354 pyikarus-0.3.1.dev20230522182134/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      715 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      683 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      691 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      325 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      379 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 root         (0) root         (0)     2040 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/cmake/tools.cmake
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/codecov.yml
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1588 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.161354 pyikarus-0.3.1.dev20230522182134/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.161354 pyikarus-0.3.1.dev20230522182134/docs/BuildLocally/
--rw-r--r--   0 root         (0) root         (0)      439 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      333 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.161354 pyikarus-0.3.1.dev20230522182134/docs/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     1136 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 root         (0) root         (0)     6961 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/literature.bib
--rw-r--r--   0 root         (0) root         (0)      117 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/literature.bib.license
--rw-r--r--   0 root         (0) root         (0)     1271 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/mkdocs-macros.py
--rw-r--r--   0 root         (0) root         (0)      395 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/mkdocs.insiders.yml
--rw-r--r--   0 root         (0) root         (0)     5042 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.145354 pyikarus-0.3.1.dev20230522182134/docs/overrides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.161354 pyikarus-0.3.1.dev20230522182134/docs/overrides/partials/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/overrides/partials/comments.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.165354 pyikarus-0.3.1.dev20230522182134/docs/website/
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/.meta.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.165354 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/
--rw-r--r--   0 root         (0) root         (0)     4710 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/assembler.md
--rw-r--r--   0 root         (0) root         (0)     6387 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 root         (0) root         (0)     2024 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 root         (0) root         (0)     3237 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 root         (0) root         (0)     8524 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 root         (0) root         (0)     2745 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/grids.md
--rw-r--r--   0 root         (0) root         (0)     4121 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/index.md
--rw-r--r--   0 root         (0) root         (0)     4932 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/localBasis.md
--rw-r--r--   0 root         (0) root         (0)    44213 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 root         (0) root         (0)     3978 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/manifolds.md
--rw-r--r--   0 root         (0) root         (0)     2590 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 root         (0) root         (0)     3086 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/observer.md
--rw-r--r--   0 root         (0) root         (0)     5211 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.169355 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/
--rw-r--r--   0 root         (0) root         (0)     6655 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 root         (0) root         (0)     7251 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/computePi.md
--rw-r--r--   0 root         (0) root         (0)     5439 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 root         (0) root         (0)     7055 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 root         (0) root         (0)     2164 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/index.md
--rw-r--r--   0 root         (0) root         (0)     7702 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 root         (0) root         (0)     5114 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 root         (0) root         (0)     6200 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 root         (0) root         (0)     4071 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.169355 pyikarus-0.3.1.dev20230522182134/docs/website/03_contribution/
--rw-r--r--   0 root         (0) root         (0)     2439 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 root         (0) root         (0)     2415 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 root         (0) root         (0)     1696 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.169355 pyikarus-0.3.1.dev20230522182134/docs/website/04_blog/
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/04_blog/.authors.yml
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/04_blog/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.169355 pyikarus-0.3.1.dev20230522182134/docs/website/04_blog/posts/
--rw-r--r--   0 root         (0) root         (0)     7731 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.169355 pyikarus-0.3.1.dev20230522182134/docs/website/05_cppReferences/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.169355 pyikarus-0.3.1.dev20230522182134/docs/website/99_Literature/
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.169355 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.173354 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 root         (0) root         (0)    52795 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 root         (0) root         (0)    46250 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 root         (0) root         (0)     2852 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 root         (0) root         (0)    17924 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 root         (0) root         (0)     9455 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.173354 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/
--rw-r--r--   0 root         (0) root         (0)    35234 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rw-r--r--   0 root         (0) root         (0)    62184 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rw-r--r--   0 root         (0) root         (0)     2281 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rw-r--r--   0 root         (0) root         (0)    40033 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rw-r--r--   0 root         (0) root         (0)    25505 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rw-r--r--   0 root         (0) root         (0)     8101 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/logo_blue.svg
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/logo_blue.svg.license
--rw-r--r--   0 root         (0) root         (0)     8255 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/logo_white.svg
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/logo_white.svg.license
--rw-r--r--   0 root         (0) root         (0)     4364 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/download.md
--rw-r--r--   0 root         (0) root         (0)      244 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/gallery.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.177355 pyikarus-0.3.1.dev20230522182134/docs/website/javascripts/
--rw-r--r--   0 root         (0) root         (0)      486 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.177355 pyikarus-0.3.1.dev20230522182134/docs/website/stylesheets/
--rw-r--r--   0 root         (0) root         (0)      302 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/docs/website/stylesheets/extra.css
--rw-r--r--   0 root         (0) root         (0)      504 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/dune.module
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.177355 pyikarus-0.3.1.dev20230522182134/ikarus/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.177355 pyikarus-0.3.1.dev20230522182134/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      268 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    12924 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 root         (0) root         (0)    10714 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.177355 pyikarus-0.3.1.dev20230522182134/ikarus/controlRoutines/
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2575 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 root         (0) root         (0)     2970 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.177355 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.177355 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feBases/
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 root         (0) root         (0)     1827 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 root         (0) root         (0)     9346 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 root         (0) root         (0)     1338 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.181355 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    19446 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 root         (0) root         (0)    12479 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.181355 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5699 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 root         (0) root         (0)     2718 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)     4635 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 root         (0) root         (0)     3809 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 root         (0) root         (0)     5734 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 root         (0) root         (0)     8008 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 root         (0) root         (0)     9574 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 root         (0) root         (0)    12655 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.181355 pyikarus-0.3.1.dev20230522182134/ikarus/io/
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/io/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2351 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/io/resultEvaluators.hh
--rw-r--r--   0 root         (0) root         (0)     3829 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/io/resultFunction.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.181355 pyikarus-0.3.1.dev20230522182134/ikarus/linearAlgebra/
--rw-r--r--   0 root         (0) root         (0)      301 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6735 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 root         (0) root         (0)     7789 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 root         (0) root         (0)    12303 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.181355 pyikarus-0.3.1.dev20230522182134/ikarus/python/
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.185355 pyikarus-0.3.1.dev20230522182134/ikarus/python/assembler/
--rw-r--r--   0 root         (0) root         (0)      249 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6752 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.185355 pyikarus-0.3.1.dev20230522182134/ikarus/python/basis/
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1469 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.185355 pyikarus-0.3.1.dev20230522182134/ikarus/python/dirichletValues/
--rw-r--r--   0 root         (0) root         (0)      257 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4169 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.185355 pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5220 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.185355 pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/materials/
--rw-r--r--   0 root         (0) root         (0)      268 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9949 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 root         (0) root         (0)     5518 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.185355 pyikarus-0.3.1.dev20230522182134/ikarus/python/test/
--rw-r--r--   0 root         (0) root         (0)      511 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3830 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/test/linearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)     4481 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.185355 pyikarus-0.3.1.dev20230522182134/ikarus/python/utils/
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1185 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.185355 pyikarus-0.3.1.dev20230522182134/ikarus/solver/
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.185355 pyikarus-0.3.1.dev20230522182134/ikarus/solver/linearSolver/
--rw-r--r--   0 root         (0) root         (0)      244 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     8891 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.189355 pyikarus-0.3.1.dev20230522182134/ikarus/solver/nonLinearSolver/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5406 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 root         (0) root         (0)     8297 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 root         (0) root         (0)    18574 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.193355 pyikarus-0.3.1.dev20230522182134/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      712 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/algorithms.hh
--rw-r--r--   0 root         (0) root         (0)      878 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/autodiffHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1469 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/basis.hh
--rw-r--r--   0 root         (0) root         (0)     6930 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.193355 pyikarus-0.3.1.dev20230522182134/ikarus/utils/drawing/
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 root         (0) root         (0)      544 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 root         (0) root         (0)     2484 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/duneUtilities.hh
--rw-r--r--   0 root         (0) root         (0)     2347 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/findLineSegment.cpp
--rw-r--r--   0 root         (0) root         (0)      724 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/findLineSegment.hh
--rw-r--r--   0 root         (0) root         (0)     3611 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/flatPreBasis.hh
--rw-r--r--   0 root         (0) root         (0)     2171 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 root         (0) root         (0)     6359 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 root         (0) root         (0)     3152 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/init.hh
--rw-r--r--   0 root         (0) root         (0)    15244 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1711 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.193355 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/
--rw-r--r--   0 root         (0) root         (0)      450 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1554 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 root         (0) root         (0)      905 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1132 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1985 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 root         (0) root         (0)     5497 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/observer.hh
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 root         (0) root         (0)     4159 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 root         (0) root         (0)     1131 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/polyfit.cpp
--rw-r--r--   0 root         (0) root         (0)      570 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/polyfit.hh
--rw-r--r--   0 root         (0) root         (0)    10054 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/tensorUtils.hh
--rw-r--r--   0 root         (0) root         (0)    15044 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus/utils/traits.hh
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/ikarus.pc.in
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/iwyu.imp
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.197355 pyikarus-0.3.1.dev20230522182134/python/
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.197355 pyikarus-0.3.1.dev20230522182134/python/ikarus/
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.197355 pyikarus-0.3.1.dev20230522182134/python/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/assembler/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/basis.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.197355 pyikarus-0.3.1.dev20230522182134/python/ikarus/finite_elements/
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/finite_elements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3119 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/finite_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/generator.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/materials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.197355 pyikarus-0.3.1.dev20230522182134/python/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      163 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      768 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.197355 pyikarus-0.3.1.dev20230522182134/python/pyikarus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3732 2023-05-22 18:21:35.000000 pyikarus-0.3.1.dev20230522182134/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10022 2023-05-22 18:21:35.000000 pyikarus-0.3.1.dev20230522182134/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 18:21:35.000000 pyikarus-0.3.1.dev20230522182134/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 18:21:35.000000 pyikarus-0.3.1.dev20230522182134/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 18:21:35.000000 pyikarus-0.3.1.dev20230522182134/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/python/setup.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.201355 pyikarus-0.3.1.dev20230522182134/sandbox/
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/sandbox/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.201355 pyikarus-0.3.1.dev20230522182134/sandbox/src/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.201355 pyikarus-0.3.1.dev20230522182134/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)   674469 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 root         (0) root         (0)      320 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/sandbox/src/sandbox.cpp
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 18:21:35.209355 pyikarus-0.3.1.dev20230522182134/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1080 2023-05-22 18:21:34.000000 pyikarus-0.3.1.dev20230522182134/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.201355 pyikarus-0.3.1.dev20230522182134/tests/
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.205355 pyikarus-0.3.1.dev20230522182134/tests/src/
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3907 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/assemblerTest.cpp
--rw-r--r--   0 root         (0) root         (0)     9842 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/common.hh
--rw-r--r--   0 root         (0) root         (0)     2639 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/dependenciesTest.cpp
--rw-r--r--   0 root         (0) root         (0)     6520 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/dirichletValueTest.cpp
--rw-r--r--   0 root         (0) root         (0)     4594 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/easTest.hh
--rw-r--r--   0 root         (0) root         (0)     1473 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/enhancedAssumedStrainsTest.cpp
--rw-r--r--   0 root         (0) root         (0)      608 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/factories.hh
--rw-r--r--   0 root         (0) root         (0)     1870 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/functionTraitsTest.cpp
--rw-r--r--   0 root         (0) root         (0)     2661 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/linearElasticityTest.cpp
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/manifoldsTest.cpp
--rw-r--r--   0 root         (0) root         (0)     7961 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/materialTest.cpp
--rw-r--r--   0 root         (0) root         (0)     9330 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/nonLinearElasticityTest.hh
--rw-r--r--   0 root         (0) root         (0)      724 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/nonLinearElasticityTestNeoHooke.cpp
--rw-r--r--   0 root         (0) root         (0)      829 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/nonLinearElasticityTestSVK.cpp
--rw-r--r--   0 root         (0) root         (0)     9936 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/nonLinearOperatorTest.cpp
--rw-r--r--   0 root         (0) root         (0)     6327 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/pathFollowingTest.cpp
--rw-r--r--   0 root         (0) root         (0)     1651 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/polyFitTest.cpp
--rw-r--r--   0 root         (0) root         (0)      695 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/pythonConversionTest.cpp
--rw-r--r--   0 root         (0) root         (0)     1292 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 root         (0) root         (0)     6143 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/testFEElement.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:21:35.205355 pyikarus-0.3.1.dev20230522182134/tests/src/testFiles/
--rw-r--r--   0 root         (0) root         (0)     9028 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 root         (0) root         (0)      395 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 root         (0) root         (0)      546 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 root         (0) root         (0)    11431 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 root         (0) root         (0)     1114 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/testHelpers.hh
--rw-r--r--   0 root         (0) root         (0)    17595 2023-05-22 18:21:27.000000 pyikarus-0.3.1.dev20230522182134/tests/src/trustRegionTest.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.925716 pyikarus-0.3.2.dev20230522090628/
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.bettercodehub.yml
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.clang-format
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.cmake-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.881716 pyikarus-0.3.2.dev20230522090628/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.889716 pyikarus-0.3.2.dev20230522090628/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      615 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.893716 pyikarus-0.3.2.dev20230522090628/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/createRelease.yml
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/ghpages.yml
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/reuseLint.yml
+-rw-r--r--   0 root         (0) root         (0)     3045 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/runExamples.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.893716 pyikarus-0.3.2.dev20230522090628/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.893716 pyikarus-0.3.2.dev20230522090628/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.893716 pyikarus-0.3.2.dev20230522090628/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    18375 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/LICENSES/MIT.txt
+-rw-r--r--   0 root         (0) root         (0)    16727 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-05-22 09:06:28.925716 pyikarus-0.3.2.dev20230522090628/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.893716 pyikarus-0.3.2.dev20230522090628/cmake/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      973 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.893716 pyikarus-0.3.2.dev20230522090628/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.893716 pyikarus-0.3.2.dev20230522090628/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      683 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      691 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      325 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/cmake/tools.cmake
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.897716 pyikarus-0.3.2.dev20230522090628/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.897716 pyikarus-0.3.2.dev20230522090628/docs/BuildLocally/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      333 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.897716 pyikarus-0.3.2.dev20230522090628/docs/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/literature.bib
+-rw-r--r--   0 root         (0) root         (0)      117 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/literature.bib.license
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/mkdocs-macros.py
+-rw-r--r--   0 root         (0) root         (0)      394 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/mkdocs.insiders.yml
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.885716 pyikarus-0.3.2.dev20230522090628/docs/overrides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.897716 pyikarus-0.3.2.dev20230522090628/docs/overrides/partials/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/overrides/partials/comments.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.897716 pyikarus-0.3.2.dev20230522090628/docs/website/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/.meta.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.897716 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/assembler.md
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 root         (0) root         (0)     8524 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/grids.md
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/index.md
+-rw-r--r--   0 root         (0) root         (0)     4932 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 root         (0) root         (0)    44213 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/observer.md
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.901716 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/computePi.md
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/index.md
+-rw-r--r--   0 root         (0) root         (0)     7702 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 root         (0) root         (0)     5114 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 root         (0) root         (0)     6200 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 root         (0) root         (0)     4071 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.901716 pyikarus-0.3.2.dev20230522090628/docs/website/03_contribution/
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.901716 pyikarus-0.3.2.dev20230522090628/docs/website/04_blog/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/04_blog/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.901716 pyikarus-0.3.2.dev20230522090628/docs/website/04_blog/posts/
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.901716 pyikarus-0.3.2.dev20230522090628/docs/website/05_cppReferences/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.901716 pyikarus-0.3.2.dev20230522090628/docs/website/99_Literature/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.901716 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.905716 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 root         (0) root         (0)    52795 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)    46250 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 root         (0) root         (0)    17924 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.905716 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 root         (0) root         (0)    35234 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 root         (0) root         (0)    62184 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 root         (0) root         (0)    40033 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 root         (0) root         (0)    25505 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 root         (0) root         (0)     8101 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/logo_blue.svg
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/logo_blue.svg.license
+-rw-r--r--   0 root         (0) root         (0)     8255 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/logo_white.svg
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/logo_white.svg.license
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/download.md
+-rw-r--r--   0 root         (0) root         (0)      244 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/gallery.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.905716 pyikarus-0.3.2.dev20230522090628/docs/website/javascripts/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.905716 pyikarus-0.3.2.dev20230522090628/docs/website/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/docs/website/stylesheets/extra.css
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/dune.module
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.905716 pyikarus-0.3.2.dev20230522090628/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.905716 pyikarus-0.3.2.dev20230522090628/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 root         (0) root         (0)    10714 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.905716 pyikarus-0.3.2.dev20230522090628/ikarus/controlRoutines/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.905716 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.909716 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feBases/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 root         (0) root         (0)     9346 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.909716 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    19446 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 root         (0) root         (0)    12479 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.909716 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 root         (0) root         (0)     9574 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 root         (0) root         (0)    12655 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.909716 pyikarus-0.3.2.dev20230522090628/ikarus/io/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/io/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/io/resultEvaluators.hh
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/io/resultFunction.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.909716 pyikarus-0.3.2.dev20230522090628/ikarus/linearAlgebra/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6735 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 root         (0) root         (0)     7789 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.909716 pyikarus-0.3.2.dev20230522090628/ikarus/python/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.909716 pyikarus-0.3.2.dev20230522090628/ikarus/python/assembler/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.909716 pyikarus-0.3.2.dev20230522090628/ikarus/python/basis/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.913716 pyikarus-0.3.2.dev20230522090628/ikarus/python/dirichletValues/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4169 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.913716 pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5220 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.913716 pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9949 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 root         (0) root         (0)     5518 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.913716 pyikarus-0.3.2.dev20230522090628/ikarus/python/test/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.913716 pyikarus-0.3.2.dev20230522090628/ikarus/python/utils/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.913716 pyikarus-0.3.2.dev20230522090628/ikarus/solver/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.913716 pyikarus-0.3.2.dev20230522090628/ikarus/solver/linearSolver/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     8891 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.913716 pyikarus-0.3.2.dev20230522090628/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 root         (0) root         (0)    18574 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.917716 pyikarus-0.3.2.dev20230522090628/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/algorithms.hh
+-rw-r--r--   0 root         (0) root         (0)      878 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/basis.hh
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.917716 pyikarus-0.3.2.dev20230522090628/ikarus/utils/drawing/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 root         (0) root         (0)      544 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 root         (0) root         (0)      682 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 root         (0) root         (0)      724 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/init.hh
+-rw-r--r--   0 root         (0) root         (0)    15244 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.917716 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 root         (0) root         (0)      905 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 root         (0) root         (0)      570 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/polyfit.hh
+-rw-r--r--   0 root         (0) root         (0)    10054 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 root         (0) root         (0)    15044 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus/utils/traits.hh
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/ikarus.pc.in
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/iwyu.imp
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.917716 pyikarus-0.3.2.dev20230522090628/python/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.921716 pyikarus-0.3.2.dev20230522090628/python/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.921716 pyikarus-0.3.2.dev20230522090628/python/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/basis.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.921716 pyikarus-0.3.2.dev20230522090628/python/ikarus/finite_elements/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/finite_elements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/finite_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/materials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.921716 pyikarus-0.3.2.dev20230522090628/python/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      768 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.921716 pyikarus-0.3.2.dev20230522090628/python/pyikarus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-05-22 09:06:28.000000 pyikarus-0.3.2.dev20230522090628/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10022 2023-05-22 09:06:28.000000 pyikarus-0.3.2.dev20230522090628/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 09:06:28.000000 pyikarus-0.3.2.dev20230522090628/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 09:06:28.000000 pyikarus-0.3.2.dev20230522090628/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 09:06:28.000000 pyikarus-0.3.2.dev20230522090628/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      632 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/python/setup.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.921716 pyikarus-0.3.2.dev20230522090628/sandbox/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/sandbox/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.921716 pyikarus-0.3.2.dev20230522090628/sandbox/src/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.921716 pyikarus-0.3.2.dev20230522090628/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)   674469 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/sandbox/src/sandbox.cpp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 09:06:28.925716 pyikarus-0.3.2.dev20230522090628/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-05-22 09:06:28.000000 pyikarus-0.3.2.dev20230522090628/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.921716 pyikarus-0.3.2.dev20230522090628/tests/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.925716 pyikarus-0.3.2.dev20230522090628/tests/src/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/assemblerTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     9842 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/common.hh
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/dependenciesTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/dirichletValueTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     4594 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/easTest.hh
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/enhancedAssumedStrainsTest.cpp
+-rw-r--r--   0 root         (0) root         (0)      608 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/factories.hh
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/functionTraitsTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/linearElasticityTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/manifoldsTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     7961 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/materialTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/nonLinearElasticityTest.hh
+-rw-r--r--   0 root         (0) root         (0)      724 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/nonLinearElasticityTestNeoHooke.cpp
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/nonLinearElasticityTestSVK.cpp
+-rw-r--r--   0 root         (0) root         (0)     9936 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/nonLinearOperatorTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/pathFollowingTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/polyFitTest.cpp
+-rw-r--r--   0 root         (0) root         (0)      695 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/pythonConversionTest.cpp
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)     6143 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/testFEElement.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:06:28.925716 pyikarus-0.3.2.dev20230522090628/tests/src/testFiles/
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 root         (0) root         (0)      395 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 root         (0) root         (0)      546 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 root         (0) root         (0)    11431 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/testHelpers.hh
+-rw-r--r--   0 root         (0) root         (0)    17595 2023-05-22 09:06:21.000000 pyikarus-0.3.2.dev20230522090628/tests/src/trustRegionTest.cpp
```

### Comparing `pyikarus-0.3.1.dev20230522182134/.clang-format` & `pyikarus-0.3.2.dev20230522090628/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.cmake-format` & `pyikarus-0.3.2.dev20230522090628/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.2.dev20230522090628/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.2.dev20230522090628/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/workflows/createRelease.yml` & `pyikarus-0.3.2.dev20230522090628/.github/workflows/createRelease.yml`

 * *Files 10% similar despite different names*

```diff
@@ -63,17 +63,19 @@
           cp -R ../repo/docs/ .
           cp -R ../repo/ikarus/ .
           git config --local user.email "mueller@ibb.uni-stuttgart.de"
           git config --local user.name "AlexanderMueller"
           cd docs
           export MKDOCSOFFLINE=false
           mike deploy v$NEWVERSION  --config-file mkdocs.insiders.yml
-          mike deploy dev  --config-file mkdocs.insiders.yml
+          ls
+          git add .
           git remote set-url origin https://${{ secrets.ORGANIZATION_TOKEN }}@github.com/ikarus-project/ikarus-project.github.io.git
-          git push origin gh-pages 
+          git commit --amend -m "Deploy v$NEWVERSION at ${{ github.event.head_commit.message }} ikarus-project/ikarus@${{ github.event.head_commit.id }}" --allow-empty
+
           export MKDOCSOFFLINE=true
 
       - uses: actions/cache@v2
         with:
           key: ${{ github.ref }}
           path: .cache
       - name: Build Website for offline use
@@ -97,44 +99,44 @@
           docker save ikarusproject/ikarus:v$NEWVERSION     > ikarus-docker-v$NEWVERSION.tar
           gzip -c9 ikarus-dev-docker-v$NEWVERSION.tar > ikarus-dev-docker-v$NEWVERSION.tar.gz
           gzip -c9 ikarus-docker-v$NEWVERSION.tar > ikarus-docker-v$NEWVERSION.tar.gz
 
       - name: Checkout ikarus-examples and create tag, push it, zip it
         run: |
           git clone https://github.com/ikarus-project/ikarus-examples.git
-          cd ikarus-examples-v$NEWVERSION
+          cd ikarus-examples
           git config --local user.email "mueller@ibb.uni-stuttgart.de"
           git config --local user.name "AlexanderMueller"
           git tag -a v$NEWVERSION -m "Create release v$NEWVERSION"
          
           cd ..
           mv ikarus-examples ikarus-examples-v$NEWVERSION
           tar -czf ikarus-examples-v$NEWVERSION.tar.gz ./ikarus-examples-v$NEWVERSION
           zip -9r  ikarus-examples-v$NEWVERSION.zip    ./ikarus-examples-v$NEWVERSION
 
       - name: Push and finalize
         run: |    
           cd ikarus-project.github.io 
           git push origin gh-pages     
-          cd ../ikarus-examples
+          cd ../ikarus-examples-v$NEWVERSION
           git push https://${{ secrets.ORGANIZATION_TOKEN }}@github.com/ikarus-project/ikarus-examples.git v$NEWVERSION
           cd .. 
           docker push ikarusproject/ikarus-dev:v$NEWVERSION  
           docker push ikarusproject/ikarus:v$NEWVERSION
           cd repo
           git push origin v$NEWVERSION
           git push origin main
 
       - uses: "marvinpinto/action-automatic-releases@latest"
         with:
           repo_token: "${{ secrets.ORGANIZATION_TOKEN }}"
-          automatic_release_tag: ${{ github.event.inputs.releaseTag }}
+          automatic_release_tag: v$NEWVERSION
           draft: false
           prerelease: true
-          title: ${{ github.event.inputs.releaseTag }}
+          title: v$NEWVERSION
           files: |
-            ./ikarus-${{ github.event.inputs.releaseTag }}/docs/docs-${{ github.event.inputs.releaseTag }}.tar.gz
-            ./ikarus-${{ github.event.inputs.releaseTag }}/docs/docs-${{ github.event.inputs.releaseTag }}.zip
-            ikarus-dev-docker-${{ github.event.inputs.releaseTag }}.tar.gz
-            ikarus-docker-${{ github.event.inputs.releaseTag }}.tar.gz
-            ikarus-examples-${{ github.event.inputs.releaseTag }}.tar.gz
-            ikarus-examples-${{ github.event.inputs.releaseTag }}.zip
+            ./ikarus-v$NEWVERSION/docs/docs-v$NEWVERSION.tar.gz
+            ./ikarus-v$NEWVERSION/docs/docs-v$NEWVERSION.zip
+            ikarus-dev-docker-v$NEWVERSION.tar.gz
+            ikarus-docker-v$NEWVERSION.tar.gz
+            ikarus-examples-v$NEWVERSION.tar.gz
+            ikarus-examples-v$NEWVERSION.zip
```

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.2.dev20230522090628/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/workflows/debian.yml` & `pyikarus-0.3.2.dev20230522090628/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/workflows/ghpages.yml` & `pyikarus-0.3.2.dev20230522090628/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/workflows/releasePythonPackage.yml` & `pyikarus-0.3.2.dev20230522090628/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/workflows/runExamples.yml` & `pyikarus-0.3.2.dev20230522090628/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/workflows/scripts/release.py` & `pyikarus-0.3.2.dev20230522090628/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.github/workflows/style.yml` & `pyikarus-0.3.2.dev20230522090628/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/.reuse/dep5` & `pyikarus-0.3.2.dev20230522090628/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/CHANGELOG.md` & `pyikarus-0.3.2.dev20230522090628/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/CMakeLists.txt` & `pyikarus-0.3.2.dev20230522090628/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 cmake_minimum_required(VERSION 3.18 FATAL_ERROR)
 
 option(DUNE_ENABLE_PYTHONBINDINGS "Enable Python bindings" ON)
 option(DUNE_PYTHON_ALLOW_GET_PIP "Allow dune-common to install pip into venv" ON)
 project(
   ikarus
-  VERSION 0.3.0
+  VERSION 0.3.1
   LANGUAGES C CXX
 )
 
 add_definitions(-DDUNE_LOCALFEFUNCTIONS_USE_EIGEN=1)
 add_definitions(-DCMAKE_DISABLE_FIND_PACKAGE_Vc=1)
 add_definitions(-DCMAKE_DISABLE_FIND_PACKAGE_LATEX=1)
 add_definitions(-DBUILD_SHARED_LIBS=1)
```

### Comparing `pyikarus-0.3.1.dev20230522182134/CODE_OF_CONDUCT.md` & `pyikarus-0.3.2.dev20230522090628/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/LICENSE.md` & `pyikarus-0.3.2.dev20230522090628/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.2.dev20230522090628/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.2.dev20230522090628/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.2.dev20230522090628/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/LICENSES/MIT.txt` & `pyikarus-0.3.2.dev20230522090628/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.2.dev20230522090628/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/PKG-INFO` & `pyikarus-0.3.2.dev20230522090628/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.1.dev20230522182134
+Version: 0.3.2.dev20230522090628
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.1.dev20230522182134 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.2.dev20230522090628 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
 ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
 github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
```

### Comparing `pyikarus-0.3.1.dev20230522182134/README.md` & `pyikarus-0.3.2.dev20230522090628/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/cmake/CPM.cmake` & `pyikarus-0.3.2.dev20230522090628/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.2.dev20230522090628/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.2.dev20230522090628/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.2.dev20230522090628/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.2.dev20230522090628/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.2.dev20230522090628/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/cmake/tools.cmake` & `pyikarus-0.3.2.dev20230522090628/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/config.h.cmake` & `pyikarus-0.3.2.dev20230522090628/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.2.dev20230522090628/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/literature.bib` & `pyikarus-0.3.2.dev20230522090628/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/mkdocs-macros.py` & `pyikarus-0.3.2.dev20230522090628/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/mkdocs.yml` & `pyikarus-0.3.2.dev20230522090628/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/overrides/partials/comments.html` & `pyikarus-0.3.2.dev20230522090628/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/assembler.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/grids.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/index.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/observer.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/01_framework/solvers.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/computePi.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/index.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/logo_blue.svg` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/logo_blue.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/auxiliaryImages/logo_white.svg` & `pyikarus-0.3.2.dev20230522090628/docs/website/auxiliaryImages/logo_white.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/download.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/docs/website/index.md` & `pyikarus-0.3.2.dev20230522090628/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/CMakeLists.txt` & `pyikarus-0.3.2.dev20230522090628/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.2.dev20230522090628/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/io/resultEvaluators.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/io/resultEvaluators.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/io/resultFunction.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/io/resultFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/basis/basis.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/algorithms.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/basis.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/concepts.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/init.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/polyfit.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/ikarus/utils/traits.hh` & `pyikarus-0.3.2.dev20230522090628/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/ikarus/__init__.py` & `pyikarus-0.3.2.dev20230522090628/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/ikarus/_ikarus.cc` & `pyikarus-0.3.2.dev20230522090628/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.2.dev20230522090628/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/ikarus/basis.py` & `pyikarus-0.3.2.dev20230522090628/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/ikarus/dirichletValues.py` & `pyikarus-0.3.2.dev20230522090628/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.2.dev20230522090628/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/ikarus/generator.py` & `pyikarus-0.3.2.dev20230522090628/python/ikarus/generator.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/ikarus/materials.py` & `pyikarus-0.3.2.dev20230522090628/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/ikarus/utils/__init__.py` & `pyikarus-0.3.2.dev20230522090628/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.2.dev20230522090628/python/pyikarus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.1.dev20230522182134
+Version: 0.3.2.dev20230522090628
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.1.dev20230522182134 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.2.dev20230522090628 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
 ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
 github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
```

### Comparing `pyikarus-0.3.1.dev20230522182134/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.2.dev20230522090628/python/pyikarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/python/setup.py.in` & `pyikarus-0.3.2.dev20230522090628/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.2.dev20230522090628/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.2.dev20230522090628/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/setup.py` & `pyikarus-0.3.2.dev20230522090628/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # build _ikarus
 # cd /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-ikarusVersion = "0.3.1.dev20230522182134"
+ikarusVersion = "0.3.2.dev20230522090628"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor since ikarus pypi package already exists
 metadata["name"] = "pyikarus"
```

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/CMakeLists.txt` & `pyikarus-0.3.2.dev20230522090628/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/assemblerTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/assemblerTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/common.hh` & `pyikarus-0.3.2.dev20230522090628/tests/src/common.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/dependenciesTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/dependenciesTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/dirichletValueTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/dirichletValueTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/easTest.hh` & `pyikarus-0.3.2.dev20230522090628/tests/src/easTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/enhancedAssumedStrainsTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/enhancedAssumedStrainsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/factories.hh` & `pyikarus-0.3.2.dev20230522090628/tests/src/factories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/functionTraitsTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/functionTraitsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/linearElasticityTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/linearElasticityTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/manifoldsTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/manifoldsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/materialTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/materialTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/nonLinearElasticityTest.hh` & `pyikarus-0.3.2.dev20230522090628/tests/src/nonLinearElasticityTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/nonLinearElasticityTestNeoHooke.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/nonLinearElasticityTestNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/nonLinearElasticityTestSVK.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/nonLinearElasticityTestSVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/nonLinearOperatorTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/nonLinearOperatorTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/pathFollowingTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/pathFollowingTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/polyFitTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/polyFitTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/pythonConversionTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/pythonConversionTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/testFEElement.hh` & `pyikarus-0.3.2.dev20230522090628/tests/src/testFEElement.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.2.dev20230522090628/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.2.dev20230522090628/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.2.dev20230522090628/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/testHelpers.hh` & `pyikarus-0.3.2.dev20230522090628/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.1.dev20230522182134/tests/src/trustRegionTest.cpp` & `pyikarus-0.3.2.dev20230522090628/tests/src/trustRegionTest.cpp`

 * *Files identical despite different names*

