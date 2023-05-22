# Comparing `tmp/hatch_fancy_pypi_readme-22.8.0.tar.gz` & `tmp/hatch_fancy_pypi_readme-23.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Mon May 22 06:59:35 2023, max compression
```

## Comparing `hatch_fancy_pypi_readme-22.8.0.tar` & `hatch_fancy_pypi_readme-23.1.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    10583 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/README.md
--rw-r--r--   0        0        0    16551 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/rich-cli-out.svg
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tox.ini
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/.github/SECURITY.md
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/__init__.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/__main__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/_builder.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/_cli.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/_config.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/_fragments.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/_substitutions.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/exceptions.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/py.typed
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/__init__.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/conftest.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/example_changelog.md
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/example_pyproject.toml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/example_text.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/test_builder.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/test_cli.py
--rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/test_config.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/test_end_to_end.py
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/test_fragments.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/test_substitutions.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/tests/utils.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/.gitignore
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/AUTHORS.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/LICENSE.txt
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/pyproject.toml
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 hatch_fancy_pypi_readme-22.8.0/PKG-INFO
+-rw-r--r--   0        0        0      503 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3322 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    12079 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/README.md
+-rw-r--r--   0        0        0    16551 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/rich-cli-out.svg
+-rw-r--r--   0        0        0     1318 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tox.ini
+-rw-r--r--   0        0        0     5483 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     8083 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       18 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      277 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      119 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3088 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1609 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0       91 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/__init__.py
+-rw-r--r--   0        0        0     1934 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/__main__.py
+-rw-r--r--   0        0        0      467 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/_builder.py
+-rw-r--r--   0        0        0     2019 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/_cli.py
+-rw-r--r--   0        0        0     2517 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/_config.py
+-rw-r--r--   0        0        0     3396 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/_fragments.py
+-rw-r--r--   0        0        0     1554 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/_substitutions.py
+-rw-r--r--   0        0        0      281 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/exceptions.py
+-rw-r--r--   0        0        0      915 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/hooks.py
+-rw-r--r--   0        0        0        0 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/py.typed
+-rw-r--r--   0        0        0       91 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1699 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      593 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/example_changelog.md
+-rw-r--r--   0        0        0     1421 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/example_pyproject.toml
+-rw-r--r--   0        0        0      122 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/example_text.md
+-rw-r--r--   0        0        0      840 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/test_builder.py
+-rw-r--r--   0        0        0     7318 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     7320 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     1932 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/test_end_to_end.py
+-rw-r--r--   0        0        0     6167 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/test_fragments.py
+-rw-r--r--   0        0        0     2394 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/test_substitutions.py
+-rw-r--r--   0        0        0      518 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/tests/utils.py
+-rw-r--r--   0        0        0      128 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/.gitignore
+-rw-r--r--   0        0        0      520 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/AUTHORS.md
+-rw-r--r--   0        0        0     1117 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4216 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1997 2023-05-22 06:59:35.000000 hatch_fancy_pypi_readme-23.1.0/PKG-INFO
```

### Comparing `hatch_fancy_pypi_readme-22.8.0/CHANGELOG.md` & `hatch_fancy_pypi_readme-23.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,30 @@
 
 The **first number** of the version is the year.
 The **second number** is incremented with each release, starting at 1 for each year.
 The **third number** is for emergencies when we need to start branches for older releases.
 
 <!-- changelog follows -->
 
+## [23.1.0](https://github.com/hynek/hatch-fancy-pypi-readme/compare/22.8.0...23.1.0) - 2023-05-22
+
+### Added
+
+- CLI support for `hatch.toml`.
+  [#27](https://github.com/hynek/hatch-fancy-pypi-readme/issues/27)
+
 
 ## [22.8.0](https://github.com/hynek/hatch-fancy-pypi-readme/compare/22.7.0...22.8.0) - 2022-10-02
 
 ### Added
 
 - Added `start-at` in addition to `start-after` that preserves the string that is looked for. This often removes the need for adding markers because you can define the starting point using a heading that becomes part of the fragment.
 
    For example: `start-at = "## License"` gives you `## License` and everything that follows.
-   [#71](https://github.com/hynek/hatch-fancy-pypi-readme/issues/71)
+   [#16](https://github.com/hynek/hatch-fancy-pypi-readme/issues/16)
 
 
 ## [22.7.0](https://github.com/hynek/hatch-fancy-pypi-readme/compare/22.6.0...22.7.0) - 2022-09-12
 
 ### Changed
 
 - Removed another circular dependency: this time the wonderful [*jsonschema*](https://python-jsonschema.readthedocs.io/).
```

### Comparing `hatch_fancy_pypi_readme-22.8.0/README.md` & `hatch_fancy_pypi_readme-23.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Your ✨Fancy✨ Project Deserves a ✨Fancy✨ PyPI Readme! 🧐
+# Your ✨Fancy✨ Project Deserves a ✨Fancy✨ PyPI Readme!
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hatch-fancy-pypi-readme.svg)](https://pypi.org/project/hatch-fancy-pypi-readme)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hatch-fancy-pypi-readme.svg)](https://pypi.org/project/hatch-fancy-pypi-readme)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/hynek/hatch-fancy-pypi-readme/blob/main/LICENSE.txt)
 
-*hatch-fancy-pypi-readme* is a [*Hatch*] metadata plugin for everyone who cares about the first impression of their project’s PyPI landing page.
+*hatch-fancy-pypi-readme* is a [Hatch] metadata plugin for everyone who cares about the first impression of their project’s PyPI landing page.
 It allows you to define your PyPI project description in terms of concatenated fragments that are based on **static strings**, **files**, and most importantly:
 **parts of files** defined using **cut-off points** or **regular expressions**.
 
 Once you’ve assembled your readme, you can additionally run **regular expression-based substitutions** over it.
 For instance to make relative links absolute or to linkify users and issue numbers in your changelog.
 
 Do you want your PyPI readme to be the project readme, but without badges, followed by the license file, and the changelog section for *only the last* release?
@@ -17,43 +17,55 @@
 
 > **Note**
 > “PyPI project description”, “PyPI landing page”, and “PyPI readme” all refer to the same thing.
 > In *setuptools* it’s called `long_description` and is the text shown on a project’s PyPI page.
 > We refer to it as “readme” because that’s how it’s called in [PEP 621](https://peps.python.org/pep-0621/)-based `pyproject.toml` files.
 
 
-### Showcases
+### Showcases 🧐
 
 <!-- Please add your project in alphabetic order, except leave hatch-fancy-pypi-readme last. -->
+- [*Awkward Array*](https://pypi.org/project/awkward/) ([`pyproject.toml`](https://github.com/scikit-hep/awkward/blob/main/pyproject.toml))
+- [*Black*](https://pypi.org/project/black/) ([`pyproject.toml`](https://github.com/psf/black/blob/main/pyproject.toml))
+- [*doc2dash*](https://pypi.org/project/doc2dash/) ([`pyproject.toml`](https://github.com/hynek/doc2dash/blob/main/pyproject.toml))
+- [*environ-config*](https://pypi.org/project/environ-config/) ([`pyproject.toml`](https://github.com/hynek/environ-config/blob/main/pyproject.toml))
 - [*jsonschema*](https://pypi.org/project/jsonschema/) ([`pyproject.toml`](https://github.com/python-jsonschema/jsonschema/blob/main/pyproject.toml))
 - [*Gradio*](https://pypi.org/project/gradio/) ([`pyproject.toml`](https://github.com/gradio-app/gradio/blob/main/pyproject.toml))
+- [*httpx*](https://pypi.org/project/httpx/) ([`pyproject.toml`](https://github.com/encode/httpx/blob/master/pyproject.toml))
 - [*pytermgui*](https://pypi.org/project/pytermgui/) ([`pyproject.toml`](https://github.com/bczsalba/pytermgui/blob/master/pyproject.toml))
+- [*scikit-build*](https://pypi.org/project/scikit-build/) ([`pyproject.toml`](https://github.com/scikit-build/scikit-build/blob/main/pyproject.toml))
 - [*stamina*](https://pypi.org/project/stamina/) ([`pyproject.toml`](https://github.com/hynek/stamina/blob/main/pyproject.toml))
-- And finally [*hatch-fancy-pypi-readme*](https://pypi.org/project/hatch-fancy-pypi-readme/22.5.0/) 22.5.0 ([`pyproject.toml`](https://github.com/hynek/hatch-fancy-pypi-readme/blob/1a76f0d6cb78448e59466716ee3d5b5ea99915d1/pyproject.toml#L125-L168)), before we went back to a static readme to avoid a circular dependency that can be problematic in some cases.
-  The shoemaker’s kids always go barefoot.
+- [*structlog*](https://pypi.org/project/structlog/) ([`pyproject.toml`](https://github.com/hynek/structlog/blob/main/pyproject.toml))
+
+*hatch-fancy-pypi-readme* doesn’t use itself to avoid a circular dependency that can be problematic in some cases.
+The shoemaker’s kids always go barefoot.
 
 <!-- start docs -->
 
 Please [open a pull request](https://github.com/hynek/hatch-fancy-pypi-readme/edit/main/README.md) to add *your* ✨fancy✨ project!
 
 
 ## Motivation
 
 The main reason for my (past) hesitancy to move away from `setup.py` files is that I like to make my PyPI readmes a lot more interesting, than what static strings or static files can offer me.
 
 For example [this](https://github.com/python-attrs/attrs/blob/b3dfebe2e10b44437c4f97d788fb5220d790efd0/setup.py#L110-L124) is the code that gave me the PyPI readme for [*attrs* 22.1.0](https://pypi.org/project/attrs/22.1.0/).
 Especially having a summary of the *latest* changes is something I’ve found users to appreciate.
 
-[*Hatch*]’s extensibility finally allowed me to build this plugin that allows you to switch away from `setup.py` without compromising on the user experience.
+[Hatch]’s extensibility finally allowed me to build this plugin that allows you to switch away from `setup.py` without compromising on the user experience.
 Now *you* too can have fancy PyPI readmes – just by adding a few lines of configuration to your `pyproject.toml`.
 
 
 ## Configuration
 
-*hatch-fancy-pypi-readme* is, like [*Hatch*], configured in your project’s `pyproject.toml`.
+*hatch-fancy-pypi-readme* is, like [Hatch], configured in your project’s `pyproject.toml`[^hatch-toml].
+
+[^hatch-toml]: As with Hatch, you can also use `hatch.toml` for configuration options that start with `tool.hatch` and leave that prefix out.
+  That means `pyprojects.toml`’s `[tool.hatch.metadata.hooks.fancy-pypi-readme]` becomes `[metadata.hooks.fancy-pypi-readme]` when in `hatch.toml`.
+  To keep the documentation simple, the more common `pyproject.toml` syntax is used throughout.
 
 First you add *hatch-fancy-pypi-readme* to your `[build-system]`:
 
 ```toml
 [build-system]
 requires = ["hatchling", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
@@ -82,15 +94,15 @@
 
 
 ### Fragments
 
 Finally, you also **must** supply an *array* of `fragments`.
 A fragment is a piece of text that is appended to your readme in the order that it’s specified.
 
-We recommend *TOML*’s [syntactic sugar for arrays of wrapping the array name in double brackets](https://toml.io/en/v1.0.0#array-of-tables) and will use it throughout this documentation.
+We recommend TOML’s [syntactic sugar for arrays of wrapping the array name in double brackets](https://toml.io/en/v1.0.0#array-of-tables) and will use it throughout this documentation.
 
 
 #### Text
 
 Text fragments consist of a single `text` key and are appended to the readme exactly as you specify them:
 
 ```toml
@@ -132,15 +144,15 @@
 
   ```python
   re.search(pattern, whatever_is_left_after_slicing, re.DOTALL).group(1)
   ```
 
   to find it.
 
-Both *Markdown* and *reST* have comments (`<!-- this is a Markdown comment -->` and `.. this is a reST comment`) that you can use for invisible markers:
+Both Markdown and *reST* have comments (`<!-- this is a Markdown comment -->` and `.. this is a reST comment`) that you can use for invisible markers:
 
 ```markdown
 # Boring Header
 
 <!-- cut after this -->
 
 This is the *interesting* body!
@@ -242,26 +254,31 @@
 ```
 
 with our [example configuration][example-config], you will get the following output:
 
 ![rich-cli output](rich-cli-out.svg)
 
 > **Warning**
-> While the execution model is somewhat different from the [*Hatch*]-Python packaging pipeline, it uses the same configuration validator and text renderer, so the fidelity should be high.
+> While the execution model is somewhat different from the [Hatch]-Python packaging pipeline, it uses the same configuration validator and text renderer, so the fidelity should be high.
 >
 > It will **not** help you debug **packaging issues**, though.
 >
 > To verify your PyPI readme using the full packaging pipeline, check out my [*build-and-inspect-python-package*](https://github.com/hynek/build-and-inspect-python-package) GitHub Action.
+>
+> If you ensure that *hatch-fancy-pypi-readme* is installed in your Hatch environment (that means where the `hatch` CLI command lives – not your development environment), you can also let Hatch render it for you:
+>
+> - `hatch project metadata readme` gives you a rendered version of the readme.
+> - `hatch project metadata | jq -r .readme.text` gives you the raw Markdown (needs [*jq*](https://stedolan.github.io/jq/)).
 
-<!-- end docs -->
 
 ## Project Links
 
 - **License**: [MIT](LICENSE.txt)
-- **Documentation**:  https://github.com/hynek/hatch-fancy-pypi-readme#readme
-- **Changelog**: [CHANGELOG.md](CHANGELOG.md)
-- **PyPI**: https://pypi.org/project/hatch-fancy-pypi-readme/
-- **Source Code**: https://github.com/hynek/hatch-fancy-pypi-readme
-- **Supported Python Versions**: 3.7 and later (follows [*Hatch*])
+- **Supported Python Versions**: 3.7 and later (follows [Hatch])
+- [**Documentation**](https://github.com/hynek/hatch-fancy-pypi-readme#readme)
+- [**Changelog**](CHANGELOG.md)
+- [**PyPI**](https://pypi.org/project/hatch-fancy-pypi-readme/)
+- [**Source Code**](https://github.com/hynek/hatch-fancy-pypi-readme)
+
 
 [example-config]: tests/example_pyproject.toml
-[*Hatch*]: https://hatch.pypa.io/
+[Hatch]: https://hatch.pypa.io/
```

### Comparing `hatch_fancy_pypi_readme-22.8.0/rich-cli-out.svg` & `hatch_fancy_pypi_readme-23.1.0/rich-cli-out.svg`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/tox.ini` & `hatch_fancy_pypi_readme-23.1.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-[gh-actions]
-python =
-    3.7: py37
-    3.8: py38
-    3.9: py39
-    3.10: py310, mypy
-    3.11: py311
-
-
 [tox]
-envlist = pre-commit,mypy,py37,py38,py39,py310,py311,py3{7,10,11}-cli,coverage-report
+min_version = 4
+env_list =
+    pre-commit,
+    mypy,
+    py37,
+    py38,
+    py39,
+    py310,
+    py311,
+    py3{7,10,11}-cli,
+    coverage-report
 isolated_build = true
 
 
 [testenv:py3{7,10,11}-cli]
 deps = coverage[toml]
 commands =
     # Use -o only once, so we exercise both code paths.
     coverage run -m hatch_fancy_pypi_readme tests/example_pyproject.toml -o {envtmpdir}{/}t.md
     coverage run {envbindir}{/}hatch-fancy-pypi-readme tests/example_pyproject.toml
 
 
 [testenv:pre-commit]
-basepython = python3.10
 skip_install = true
 deps = pre-commit
 commands = pre-commit run --all-files
 
 
 [testenv:mypy]
 extras = tests
 deps = mypy
 commands = mypy src
 
 
 [testenv]
 extras = tests
-commands = python -m pytest {posargs}
+commands = pytest {posargs}
 
 
-[testenv:py3{10,11}]
+[testenv:py31{0,1}]
 deps = coverage[toml]
-commands = python -m coverage run -m pytest {posargs}
+commands = coverage run -m pytest {posargs}
 
 
 [testenv:coverage-report]
-basepython = python3.10
+base_python = python3.11
 deps = coverage[toml]
 skip_install = true
 commands =
-    python -m coverage combine
-    python -m coverage report
+    coverage combine
+    coverage report
 
 
 [testenv:svg]
 description = Refresh SVG, test running using pipx.
 deps = pipx
 skip_install = true
 allowlist_externals = npx
```

### Comparing `hatch_fancy_pypi_readme-22.8.0/.github/CODE_OF_CONDUCT.md` & `hatch_fancy_pypi_readme-23.1.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/.github/CONTRIBUTING.md` & `hatch_fancy_pypi_readme-23.1.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/.github/workflows/ci.yml` & `hatch_fancy_pypi_readme-23.1.0/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -9,36 +9,37 @@
     branches: [main]
   workflow_dispatch:
 
 env:
   FORCE_COLOR: "1" # Make tools pretty.
   PYTHONIOENCODING: utf-8
   TOX_TESTENV_PASSENV: FORCE_COLOR
+  PIP_DISABLE_PIP_VERSION_CHECK: "1"
+  PIP_NO_PYTHON_VERSION_WARNING: "1"
   SETUPTOOLS_SCM_PRETEND_VERSION: "1.0" # avoid warnings about shallow checkout
-  PYTHON_LATEST: "3.10"
+  PYTHON_LATEST: "3.11"
 
 jobs:
   tests:
-    name: tox on ${{ matrix.python-version }}
+    name: Tests on ${{ matrix.python-version }}
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "~3.11.0-0"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+      - run: python -Im pip install --upgrade wheel tox
 
-      - run: python -m pip install --upgrade tox tox-gh-actions
-
-      - run: python -m tox
+      - run: python -Im tox run -f py$(echo ${{ matrix.python-version }} | tr -d .)
 
       - name: Upload coverage data
         uses: actions/upload-artifact@v3
         with:
           name: coverage-data
           path: .coverage.*
           if-no-files-found: ignore
@@ -47,69 +48,73 @@
     runs-on: ubuntu-latest
     needs: tests
 
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: ${{env.PYTHON_LATEST}}
+          python-version: ${{ env.PYTHON_LATEST }}
 
-      - run: python -m pip install --upgrade coverage[toml]
+      - run: python -Im pip install --upgrade coverage[toml]
 
       - name: Download coverage data
         uses: actions/download-artifact@v3
         with:
           name: coverage-data
 
       - name: Combine coverage and fail if it's <100%.
         run: |
-          python -m coverage combine
-          python -m coverage html --skip-covered --skip-empty
-          python -m coverage report --fail-under=100
+          python -Im coverage combine
+          python -Im coverage html --skip-covered --skip-empty
+          python -Im coverage report --fail-under=100
 
       - name: Upload HTML report if check failed.
         uses: actions/upload-artifact@v3
         with:
           name: html-report
           path: htmlcov
         if: ${{ failure() }}
 
-  package:
-    name: Build & verify package
+  mypy:
+    name: Mypy
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
-      - uses: hynek/build-and-inspect-python-package@v1
+      - uses: actions/setup-python@v4
+        with:
+          python-version: ${{ env.PYTHON_LATEST }}
+      - run: python -Im pip install --upgrade wheel tox
+
+      - run: python -Im tox run -e mypy
 
   install-dev:
     name: Verify dev env
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: ${{env.PYTHON_LATEST}}
-      - run: python -m pip install -e .[dev]
-      - run: python -c 'import hatch_fancy_pypi_readme'
+          python-version: ${{ env.PYTHON_LATEST }}
+      - run: python -Im pip install -e .[dev]
+      - run: python -Ic 'import hatch_fancy_pypi_readme'
       - run: python -m hatch_fancy_pypi_readme tests/example_pyproject.toml
       - run: hatch-fancy-pypi-readme tests/example_pyproject.toml
 
   # Ensure everything required is passing for branch protection.
   required-checks-pass:
     if: always()
 
     needs:
       - coverage
       - install-dev
-      - package
 
     runs-on: ubuntu-latest
 
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
```

### Comparing `hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/_cli.py` & `hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,44 +2,64 @@
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import sys
 
+from contextlib import suppress
 from typing import Any, NoReturn, TextIO
 
 from hatch_fancy_pypi_readme.exceptions import ConfigurationError
 
 from ._builder import build_text
 from ._config import load_and_validate_config
 
 
-def cli_run(pyproject: dict[str, Any], out: TextIO) -> None:
+def cli_run(
+    pyproject: dict[str, Any], hatch_toml: dict[str, Any], out: TextIO
+) -> None:
     """
     Best-effort verify config and print resulting PyPI readme.
     """
     is_dynamic = False
-    try:
+    with suppress(KeyError):
         is_dynamic = "readme" in pyproject["project"]["dynamic"]
-    except KeyError:
-        pass
 
     if not is_dynamic:
         _fail("You must add 'readme' to 'project.dynamic'.")
 
     try:
-        cfg = pyproject["tool"]["hatch"]["metadata"]["hooks"][
-            "fancy-pypi-readme"
-        ]
+        if (
+            pyproject["tool"]["hatch"]["metadata"]["hooks"][
+                "fancy-pypi-readme"
+            ]
+            and hatch_toml["metadata"]["hooks"]["fancy-pypi-readme"]
+        ):
+            _fail(
+                "Both pyproject.toml and hatch.toml contain "
+                "hatch-fancy-pypi-readme configuration."
+            )
     except KeyError:
-        _fail(
-            "Missing configuration "
-            "(`[tool.hatch.metadata.hooks.fancy-pypi-readme]`)",
-        )
+        pass
+
+    try:
+        cfg = hatch_toml["metadata"]["hooks"]["fancy-pypi-readme"]
+    except KeyError:
+        try:
+            cfg = pyproject["tool"]["hatch"]["metadata"]["hooks"][
+                "fancy-pypi-readme"
+            ]
+        except KeyError:
+            _fail(
+                "Missing configuration "
+                "(`[tool.hatch.metadata.hooks.fancy-pypi-readme]` in"
+                " pyproject.toml or `[metadata.hooks.fancy-pypi-readme]`"
+                " in hatch.toml)",
+            )
 
     try:
         config = load_and_validate_config(cfg)
     except ConfigurationError as e:
         _fail(
             "Configuration has errors:\n\n"
             + "\n".join(f"- {msg}" for msg in e.errors),
```

### Comparing `hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/_config.py` & `hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/_config.py`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/_fragments.py` & `hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/_fragments.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .exceptions import ConfigurationError
 
 
 class Fragment(Protocol):
     key: ClassVar[str]
 
     @classmethod
-    def from_config(self, cfg: dict[str, str]) -> Fragment:
+    def from_config(cls, cfg: dict[str, str]) -> Fragment:
         ...
 
     def render(self) -> str:
         ...
 
 
 @dataclass
@@ -72,15 +72,17 @@
         pattern = cfg.pop("pattern", None)
 
         errs: list[str] = []
 
         try:
             contents = path.read_text(encoding="utf-8")
         except FileNotFoundError:
-            raise ConfigurationError([f"Fragment file '{path}' not found."])
+            raise ConfigurationError(
+                [f"Fragment file '{path}' not found."]
+            ) from None
 
         if start_after and start_at:
             raise ConfigurationError(
                 [
                     "file fragment: 'start-after' and 'start-at' are "
                     "mutually exclusive."
                 ]
```

### Comparing `hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/_substitutions.py` & `hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/_substitutions.py`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/src/hatch_fancy_pypi_readme/hooks.py` & `hatch_fancy_pypi_readme-23.1.0/src/hatch_fancy_pypi_readme/hooks.py`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/tests/conftest.py` & `hatch_fancy_pypi_readme-23.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/tests/example_changelog.md` & `hatch_fancy_pypi_readme-23.1.0/tests/example_changelog.md`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/tests/example_pyproject.toml` & `hatch_fancy_pypi_readme-23.1.0/tests/example_pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/tests/test_builder.py` & `hatch_fancy_pypi_readme-23.1.0/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/tests/test_config.py` & `hatch_fancy_pypi_readme-23.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/tests/test_end_to_end.py` & `hatch_fancy_pypi_readme-23.1.0/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/tests/test_fragments.py` & `hatch_fancy_pypi_readme-23.1.0/tests/test_fragments.py`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/tests/test_substitutions.py` & `hatch_fancy_pypi_readme-23.1.0/tests/test_substitutions.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,23 +31,23 @@
     def test_twisted(self):
         """
         Twisted example works.
 
         https://github.com/twisted/twisted/blob/eda9d29dc7fe34e7b207781e5674dc92f798bffe/setup.py#L19-L24
         """
         assert (
-            "For information on changes in this release, see the `NEWS <https://github.com/twisted/twisted/blob/trunk/NEWS.rst>`_ file."  # noqa
+            "For information on changes in this release, see the `NEWS <https://github.com/twisted/twisted/blob/trunk/NEWS.rst>`_ file."
         ) == Substituter.from_config(
             {
                 "pattern": r"`([^`]+)\s+<(?!https?://)([^>]+)>`_",
-                "replacement": r"`\1 <https://github.com/twisted/twisted/blob/trunk/\2>`_",  # noqa
+                "replacement": r"`\1 <https://github.com/twisted/twisted/blob/trunk/\2>`_",
                 "ignore-case": True,
             }
         ).substitute(
-            "For information on changes in this release, see the `NEWS <NEWS.rst>`_ file."  # noqa
+            "For information on changes in this release, see the `NEWS <NEWS.rst>`_ file."
         )
 
     @pytest.mark.parametrize(
         "pat,repl,text,expect",
         [
             (
                 r"#(\d+)",
```

### Comparing `hatch_fancy_pypi_readme-22.8.0/AUTHORS.md` & `hatch_fancy_pypi_readme-23.1.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/LICENSE.txt` & `hatch_fancy_pypi_readme-23.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_fancy_pypi_readme-22.8.0/pyproject.toml` & `hatch_fancy_pypi_readme-23.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "hatch-fancy-pypi-readme"
-version = "22.8.0"
+version = "23.1.0"
 description = "Fancy PyPI READMEs with Hatch"
 requires-python = ">=3.7"
 keywords = ["hatch", "pypi", "readme", "documentation"]
 authors = [{ name = "Hynek Schlawack", email = "hs@ox.cx" }]
-license = { text = "MIT" }
+license = "MIT"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: Hatch",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Build Tools",
 
-  "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "hatchling",
   "tomli; python_version<'3.11'",
   "typing-extensions; python_version<'3.8'",
 ]
 
@@ -44,27 +41,20 @@
 dev = ["hatch-fancy-pypi-readme[tests]", "mypy"]
 
 [project.urls]
 Documentation = "https://github.com/hynek/hatch-fancy-pypi-readme#readme"
 Changelog = "https://github.com/hynek/hatch-fancy-pypi-readme/blob/main/CHANGELOG.md"
 "Source Code" = "https://github.com/hynek/hatch-fancy-pypi-readme"
 Funding = "https://github.com/sponsors/hynek"
-Ko-fi = "https://ko-fi.com/the_hynek"
 
 [project.readme]
 content-type = "text/markdown"
-text = """# Your ✨Fancy✨ Project Deserves a ✨Fancy✨ PyPI Readme! 🧐
+text = """# Your ✨Fancy✨ Project Deserves a ✨Fancy✨ PyPI Readme!
 
-[![PyPI - Version](https://img.shields.io/pypi/v/hatch-fancy-pypi-readme.svg)](https://pypi.org/project/hatch-fancy-pypi-readme)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hatch-fancy-pypi-readme.svg)](https://pypi.org/project/hatch-fancy-pypi-readme)
-[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
-[![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/hynek/hatch-fancy-pypi-readme/blob/main/LICENSE.txt)
-
-
-*hatch-fancy-pypi-readme* is an MIT-licensed metadata plugin for [*Hatch*](https://hatch.pypa.io/).
+*hatch-fancy-pypi-readme* is an MIT-licensed metadata plugin for [Hatch](https://hatch.pypa.io/) by [Hynek Schlawack](https://hynek.me/).
 
 Its purpose is to help you to have fancy PyPI readmes – unlike *this* one you’re looking at right now.
 
 Please check out the [documentation](https://github.com/hynek/hatch-fancy-pypi-readme#readme) to see what *hatch-fancy-pypi-readme* can do for you and your projects!
 """
 
 
@@ -78,15 +68,15 @@
 
 [tool.coverage.run]
 parallel = true
 branch = true
 source = ["hatch_fancy_pypi_readme"]
 
 [tool.coverage.paths]
-source = ["src", ".tox/*/site-packages"]
+source = ["src", ".tox/py*/**/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 omit = ["src/hatch_fancy_pypi_readme/hooks.py"]
 exclude_lines = [
   # a more strict default pragma
@@ -113,22 +103,58 @@
 ]
 
 
 [tool.black]
 line-length = 79
 
 
-[tool.isort]
-profile = "attrs"
-
-
 [tool.mypy]
 strict = true
 follow_imports = "normal"
 enable_error_code = ["ignore-without-code"]
 show_error_codes = true
 warn_no_return = true
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 ignore_errors = true
+
+
+[tool.ruff]
+src = ["src", "tests"]
+select = [
+  "E",   # pycodestyle
+  "W",   # pycodestyle
+  "F",   # Pyflakes
+  "UP",  # pyupgrade
+  "N",   # pep8-naming
+  "YTT", # flake8-2020
+  "S",   # flake8-bandit
+  "B",   # flake8-bugbear
+  "C4",  # flake8-comprehensions
+  "T10", # flake8-debugger
+  "ISC", # flake8-implicit-str-concat
+  "RET", # flake8-return
+  "SIM", # flake8-simplify
+  "DTZ", # flake8-datetimez
+  "I",   # isort
+  "PGH", # pygrep-hooks
+  "PLC", # Pylint
+  "PIE", # flake8-pie
+  "RUF", # ruff
+]
+
+ignore = [
+  "E501", # leave line-length enforcement to Black
+]
+
+[tool.ruff.per-file-ignores]
+"tests/*" = [
+  "S101",    # assert
+  "SIM300",  # Yoda rocks in tests
+  "PLC1901", # empty strings are falsey, but are less specific in tests
+]
+
+[tool.ruff.isort]
+lines-between-types = 1
+lines-after-imports = 2
```

### Comparing `hatch_fancy_pypi_readme-22.8.0/PKG-INFO` & `hatch_fancy_pypi_readme-23.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,43 @@
 Metadata-Version: 2.1
 Name: hatch-fancy-pypi-readme
-Version: 22.8.0
+Version: 23.1.0
 Summary: Fancy PyPI READMEs with Hatch
 Project-URL: Documentation, https://github.com/hynek/hatch-fancy-pypi-readme#readme
 Project-URL: Changelog, https://github.com/hynek/hatch-fancy-pypi-readme/blob/main/CHANGELOG.md
 Project-URL: Source Code, https://github.com/hynek/hatch-fancy-pypi-readme
 Project-URL: Funding, https://github.com/sponsors/hynek
-Project-URL: Ko-fi, https://ko-fi.com/the_hynek
 Author-email: Hynek Schlawack <hs@ox.cx>
-License: MIT
+License-Expression: MIT
 License-File: AUTHORS.md
 License-File: LICENSE.txt
 Keywords: documentation,hatch,pypi,readme
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Hatch
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.7
 Requires-Dist: hatchling
 Requires-Dist: tomli; python_version < '3.11'
 Requires-Dist: typing-extensions; python_version < '3.8'
 Provides-Extra: dev
 Requires-Dist: hatch-fancy-pypi-readme[tests]; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Provides-Extra: tests
 Requires-Dist: build; extra == 'tests'
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: wheel; extra == 'tests'
 Description-Content-Type: text/markdown
 
-# Your ✨Fancy✨ Project Deserves a ✨Fancy✨ PyPI Readme! 🧐
+# Your ✨Fancy✨ Project Deserves a ✨Fancy✨ PyPI Readme!
 
-[![PyPI - Version](https://img.shields.io/pypi/v/hatch-fancy-pypi-readme.svg)](https://pypi.org/project/hatch-fancy-pypi-readme)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hatch-fancy-pypi-readme.svg)](https://pypi.org/project/hatch-fancy-pypi-readme)
-[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
-[![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/hynek/hatch-fancy-pypi-readme/blob/main/LICENSE.txt)
-
-
-*hatch-fancy-pypi-readme* is an MIT-licensed metadata plugin for [*Hatch*](https://hatch.pypa.io/).
+*hatch-fancy-pypi-readme* is an MIT-licensed metadata plugin for [Hatch](https://hatch.pypa.io/) by [Hynek Schlawack](https://hynek.me/).
 
 Its purpose is to help you to have fancy PyPI readmes – unlike *this* one you’re looking at right now.
 
 Please check out the [documentation](https://github.com/hynek/hatch-fancy-pypi-readme#readme) to see what *hatch-fancy-pypi-readme* can do for you and your projects!
```

