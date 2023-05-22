# Comparing `tmp/flyswot-0.3.8.tar.gz` & `tmp/flyswot-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyswot-0.3.8.tar", max compression
+gzip compressed data, was "flyswot-0.3.9.tar", max compression
```

## Comparing `flyswot-0.3.8.tar` & `flyswot-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1094 2022-08-24 16:17:02.284996 flyswot-0.3.8/LICENSE.rst
--rw-r--r--   0        0        0    17676 2022-08-24 16:17:02.284996 flyswot-0.3.8/README.md
--rw-r--r--   0        0        0     1860 2022-08-24 16:17:17.713776 flyswot-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       15 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/__init__.py
--rw-r--r--   0        0        0      471 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/cli.py
--rw-r--r--   0        0        0    13851 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/cli_inference.py
--rw-r--r--   0        0        0       95 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/config.py
--rw-r--r--   0        0        0       68 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/console.py
--rw-r--r--   0        0        0     3231 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/core.py
--rw-r--r--   0        0        0     3018 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/inference.py
--rw-r--r--   0        0        0      371 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/logo.py
--rw-r--r--   0        0        0     5671 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/models.py
--rw-r--r--   0        0        0     3792 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/onnx_inference.py
--rw-r--r--   0        0        0        0 2022-08-24 16:17:02.292996 flyswot-0.3.8/src/flyswot/py.typed
--rw-r--r--   0        0        0    18972 2022-08-24 16:17:20.664965 flyswot-0.3.8/setup.py
--rw-r--r--   0        0        0    18712 2022-08-24 16:17:20.666215 flyswot-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1094 2022-09-23 09:09:00.509463 flyswot-0.3.9/LICENSE.rst
+-rw-r--r--   0        0        0    17676 2022-09-23 09:09:00.509463 flyswot-0.3.9/README.md
+-rw-r--r--   0        0        0     1860 2022-09-23 09:09:13.693658 flyswot-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0       15 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/__init__.py
+-rw-r--r--   0        0        0      471 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/cli.py
+-rw-r--r--   0        0        0    13887 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/cli_inference.py
+-rw-r--r--   0        0        0       95 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/config.py
+-rw-r--r--   0        0        0       68 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/console.py
+-rw-r--r--   0        0        0     3231 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/core.py
+-rw-r--r--   0        0        0     3018 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/inference.py
+-rw-r--r--   0        0        0      371 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/logo.py
+-rw-r--r--   0        0        0     5671 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/models.py
+-rw-r--r--   0        0        0     3792 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/onnx_inference.py
+-rw-r--r--   0        0        0        0 2022-09-23 09:09:00.517463 flyswot-0.3.9/src/flyswot/py.typed
+-rw-r--r--   0        0        0    18976 1970-01-01 00:00:00.000000 flyswot-0.3.9/setup.py
+-rw-r--r--   0        0        0    18812 1970-01-01 00:00:00.000000 flyswot-0.3.9/PKG-INFO
```

### Comparing `flyswot-0.3.8/LICENSE.rst` & `flyswot-0.3.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flyswot-0.3.8/README.md` & `flyswot-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `flyswot-0.3.8/pyproject.toml` & `flyswot-0.3.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flyswot"
-version = "0.3.8"
+version = "0.3.9"
 description = "flyswot"
 authors = ["Daniel van Strien <daniel.van-strien@bl.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/davanstrien/flyswot"
 repository = "https://github.com/davanstrien/flyswot"
 documentation = "https://flyswot.readthedocs.io"
@@ -25,40 +25,40 @@
 Pillow = ">=8,<10"
 typing_extensions = ">=3.10,<5.0"
 huggingface-hub = ">=0.2.1,<0.10.0"
 transformers = {extras = ["torch"], version = "^4.16.2"}
 typer = ">=0.5.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+pytest = "^7.1.3"
 coverage = {extras = ["toml"], version = "^6.4"}
-safety = "^2.1.1"
+safety = "^2.2.0"
 mypy = "^0.971"
-xdoctest = {extras = ["colors"], version = "^1.0.2"}
+xdoctest = {extras = ["colors"], version = "^1.1.0"}
 sphinx = "^5.1.1"
 sphinx-autobuild = "^2021.3.14"
 pre-commit = "^2.20.0"
 flake8 = "^4.0.1"
-black = "^22.6"
+black = "^22.8"
 flake8-bandit = "^3.0.0"
-flake8-bugbear = "^22.8.23"
+flake8-bugbear = "^22.9.11"
 flake8-docstrings = "^1.5.0"
 flake8-rst-docstrings = "^0.2.7"
 pep8-naming = "^0.13.2"
 darglint = "^1.8.1"
 reorder-python-imports = "^3.8.2"
 pre-commit-hooks = "^4.3.0"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-click = "^4.3.0"
 Pygments = "^2.13.0"
-hypothesis = "^6.54.4"
+hypothesis = "^6.54.6"
 memory-profiler = "^0.60.0"
 pytest-datafiles = "^2.0"
 onnxruntime = "^1.12.1"
-furo = "^2022.6.21"
+furo = "^2022.9.15"
 myst-parser = "^0.18.0"
 cogapp = "^3.3.0"
 
 [tool.poetry.scripts]
 flyswot = "flyswot.cli:main"
```

### Comparing `flyswot-0.3.8/src/flyswot/cli_inference.py` & `flyswot-0.3.9/src/flyswot/cli_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,15 +335,15 @@
     """print batch preds to csv"""
     raise NotImplementedError(f"Not implemented for type {predictions}")
 
 
 @write_batch_preds_to_csv.register
 def _(predictions: PredictionBatch, csv_fpath: Path) -> None:
     """Appends `predictions` batch to `csv_path`"""
-    with open(csv_fpath, mode="a", newline="") as csv_file:
+    with open(csv_fpath, mode="a", newline="", encoding="utf-8") as csv_file:
         field_names = ["path", "directory", "predicted_label", "confidence"]
         writer = csv.DictWriter(csv_file, fieldnames=field_names)
         for pred in predictions.batch:
             row = asdict(pred)
             row["directory"] = pred.path.parent
             writer.writerow(row)
 
@@ -355,15 +355,15 @@
         row["path"] = asdict(pred)["path"]
         row["directory"] = asdict(pred)["path"].parent
         for i, v in enumerate(pred.predictions):
             sorted_predictions = sorted(v.items(), reverse=True)
             for j in range(top_n):
                 row[f"prediction_label_{i}_{j}"] = sorted_predictions[j][1]
                 row[f"confidence_label_{i}_{j}"] = sorted_predictions[j][0]
-        with open(csv_fpath, mode="a", newline="") as csv_file:
+        with open(csv_fpath, mode="a", newline="", encoding="utf-8") as csv_file:
             field_names = list(row.keys())
             writer = csv.DictWriter(csv_file, fieldnames=field_names)
             writer.writerow(row)
 
 
 class HuggingFaceInferenceSession(InferenceSession):
     "Huggingface inference session"
```

### Comparing `flyswot-0.3.8/src/flyswot/core.py` & `flyswot-0.3.9/src/flyswot/core.py`

 * *Files identical despite different names*

### Comparing `flyswot-0.3.8/src/flyswot/inference.py` & `flyswot-0.3.9/src/flyswot/inference.py`

 * *Files identical despite different names*

### Comparing `flyswot-0.3.8/src/flyswot/models.py` & `flyswot-0.3.9/src/flyswot/models.py`

 * *Files identical despite different names*

### Comparing `flyswot-0.3.8/src/flyswot/onnx_inference.py` & `flyswot-0.3.9/src/flyswot/onnx_inference.py`

 * *Files identical despite different names*

### Comparing `flyswot-0.3.8/setup.py` & `flyswot-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,21 @@
  'typing_extensions>=3.10,<5.0']
 
 entry_points = \
 {'console_scripts': ['flyswot = flyswot.cli:main']}
 
 setup_kwargs = {
     'name': 'flyswot',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'flyswot',
     'long_description': '# flyswot\n\n[![PyPI](https://img.shields.io/pypi/v/flyswot.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/flyswot.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/flyswot)][python version]\n[![License](https://img.shields.io/pypi/l/flyswot)][license]\n\n[![Read the documentation at https://flyswot.readthedocs.io/](https://img.shields.io/readthedocs/flyswot/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/davanstrien/flyswot/actions/workflows/tests.yml/badge.svg)](https://github.com/davanstrien/flyswot/actions/workflows/tests.yml)\n[![Codecov](https://codecov.io/gh/davanstrien/flyswot/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/flyswot/\n[status]: https://pypi.org/project/flyswot/\n[python version]: https://pypi.org/project/flyswot\n[license]: https://opensource.org/licenses/MIT\n[read the docs]: https://flyswot.readthedocs.io/\n[tests]: https://github.com/davanstrien/flyswot/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/davanstrien/flyswot\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n![flyswot logo](https://raw.githubusercontent.com/davanstrien/flyswot/main/docs/_static/fly.png?token=ACEUI5KJ2HPO4ZGNTBX6OE3ARMXII)\n\n## Disclaimer 😬\n\n_flyswot_ is a work in progress. Things may not work and behaviour may change in the future!\n\n## tl;dr\n\n_flyswot_ is a Command Line Tool which allows you to run [Hugging Face Transformers](https://huggingface.co/docs/transformers/) [image classification models](https://huggingface.co/models?pipeline_tag=image-classification&sort=downloads) available via the [Hugging Face Hub](https://huggingface.co/models) 🤗 against a directory of images. It returns a CSV report containing the models predictions.\n\n```console\nflyswot predict directory image_directory csv_reports --model_id flyswot/convnext-tiny-224_flyswot\n```\n\n## Features\n\nCurrently _flyswot_ supports:\n\n- 🚀 automatic downloading of models from the Hugging Face Hub\n- 🔎 UNIX style search patterns for matching images to predict against\n- 📸 filtering by image extension\n- 📜 a CSV output report containing the paths to the input images, the predicted label and the models confidence for that prediction.\n- 📊 a summary \'report\' on the command line providing a high level summary of the predictions made\n\n[![asciicast](https://asciinema.org/a/492427.svg)](https://asciinema.org/a/492427)\n\n## Why?\n\nWhat is the point of this? Why not just write a Python script? This seems like a terrible idea...\n\n_flyswot_ was originally for a project with the [Heritage Made Digital](https://www.bl.uk/projects/heritage-made-digital) team at the [British Library](https://www.bl.uk). In this project we wanted to detect \'fake flysheets\'. We designed how _flyswot_ works with this particular use case in mind.\n\nThere are a few main reasons why we decided a command line tool was the best approaches to utilising the models we were developing.\n\n- The digitised images we are working with can be very large\n- The images we are working with are often subject to copyright\n- Inference speed isn\'t a big priority\n\nSince we\'re using computer vision for _assisting_ rather than _automation_ we felt a CLI was a useful interface for interacting with the models.\n\n## Installation\n\nYou can install _flyswot_ via [pip] from [PyPI]:\n\n```console\n$ pip install flyswot\n```\n\nThis will install the latest release version of _flyswot_\n\n## Detailed Installation Guide\n\n[Installation] provides a more detailed guide to installing _flyswot_. This more detailed guide is aimed at users of _flyswot_ who may be less familiar with Python.\n\n## Usage\n\nYou can see help for _flyswot_ using `flyswot --help`\n\n<!-- [[[cog\nimport cog\nfrom flyswot.cli import app\nfrom typer.testing import CliRunner\nrunner = CliRunner()\nresult = runner.invoke(app, ["--help"])\nhelp = result.output.replace("Usage: root", "Usage: flyswot")\ncog.out(\n    "```\\n{}\\n```".format(help)\n)\n]]] -->\n\n```\n\n Usage: flyswot [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --install-completion        [bash|zsh|fish|powershell|pwsh]  Install completion for the specified shell. [default: None]                                                 │\n│ --show-completion           [bash|zsh|fish|powershell|pwsh]  Show completion for the specified shell, to copy it or customize the installation. [default: None]          │\n│ --help                                                       Show this message and exit.                                                                                 │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ model                      flyswot commands for interacting with models                                                                                                  │\n│ predict                    flyswot commands for making predictions                                                                                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n\n\n```\n\n<!-- [[[end]]] -->\n\n### Making predictions\n\nYou can get help for the prediction functionality for _flyswot_ as follows:\n\n<!-- [[[cog\nimport cog\nfrom flyswot.cli import app\nfrom typer.testing import CliRunner\nrunner = CliRunner()\nresult = runner.invoke(app,  ["predict", "directory", "--help"])\nhelp = result.output.replace("Usage: root", "Usage: flyswot")\ncog.out(\n    "```\\n{}\\n```".format(help)\n)\n]]] -->\n\n```\n\n Usage: flyswot predict directory [OPTIONS] DIRECTORY CSV_SAVE_DIR\n\n Predicts against all images stored under DIRECTORY which match PATTERN in the filename.\n By default searches for filenames containing \'fs\'.\n Creates a CSV report saved to `csv_save_dir`\n\n╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ *    directory         PATH  Directory to start searching for images from [default: None] [required]                                                                     │\n│ *    csv_save_dir      PATH  Directory used to store the csv report [default: None] [required]                                                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --model-id             TEXT     The model flyswot should use for making predictions [default: flyswot/convnext-tiny-224_flyswot]                                         │\n│ --pattern              TEXT     Pattern used to filter image filenames [default: None]                                                                                   │\n│ --bs                   INTEGER  Batch Size [default: 16]                                                                                                                 │\n│ --image-formats        TEXT     Image format(s) to check [default: .tif]                                                                                                 │\n│ --help                          Show this message and exit.                                                                                                              │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n\n\n```\n\n<!-- [[[end]]] -->\n\nTo run predictions against a directory of images:\n\n```console\n$ flyswot predict directory manuscripts_folder .\n```\n\n- _flyswot_ will search inside the manuscripts_folder looking for image files.\n- By default it will look for files that contain `FS` in the filename since these are files which have been labelled as being "end flysheets" or "front flysheets"\n- Once it has found all the files labelled as `flysheet` it will then run a computer vision model against these images to see if they are labelled correctly i.e. if it is indeed a flysheet or something else.\n- _flyswot_ will save a csv report containing the paths to the image, the directory the image is stored in, the label, and the confidence for that prediction.\n\n#### Changing the model\n\nYou can also tell _flyswot_ to use a different image classification model via the `model-id` parameter. For example to use the [microsoft/dit-base-finetuned-rvlcdip](https://huggingface.co/microsoft/dit-base-finetuned-rvlcdip) model we could run:\n\n```console\nflyswot predict directory Documents/DS/hugit-cli/fs Desktop/ --model-id microsoft/dit-base-finetuned-rvlcdip\n\n```\n\nThis will download the latest available version of this model from the Hugging Face Hub and predict against the specified filenames. **Note** under the hood _flyswot_ uses the Hugging Face [transformers](https://huggingface.co/docs/transformers/) [pipelines](https://huggingface.co/docs/transformers/pipeline_tutorial) for inference. The model you specific must therefore be compatible with this pipeline.\n\n## Detailed Usage Guide\n\nThis section provides additional guidance on the usage of _flyswot_. This is primarily aimed at [HMD](https://www.bl.uk/projects/heritage-made-digital) users of _flyswot_.\n\n### How flyswot searches for images\n\n_flyswot_ is currently intended to identify images which have an incorrect label associated with them. In particular it is currently intended to identify "fake" flysheets. These images have `fs` as part of their filename so we can tell _flyswot_ to use this pattern in the filename to identify images which should be checked using the computer vision model. This can be changed if you also want to match other filename patterns.\n\nSince these images of concern will often be inside a directory structure _flyswot_ will look in sub-folders from the input folder for images which contain `fs` in the name. For example in the following folder structure:\n\n```console\nCollection/\n├─ item1/\n│  ├─ add_ms_9403_fbspi.tif\n│  ├─ add_ms_9403_fse001r.tif\n│  ├─ add_ms_9403_fse001v.tif\n├─ item2/\n│  ├─ sloane_ms_116_fblefr.tif\n│  ├─ sloane_ms_116_fbspi.tif\n│  ├─ sloane_ms_116_fse004r.tif\n```\n\nAll of the files which have `fs` in the filname will be check but files which don\'t contains `fs` such as `add_ms_9403_fbspi.tif` will be ignored since these aren\'t labelled as flysheets.\n\n### Running flyswot against a directory of images\n\nTo run _flyswot_ against a directory of images you need to give it the path to that directory/folder.\nThere are different ways you could do this. The following is suggested for people who are not very familiar (yet 😜) with terminal interfaces.\n\nIdentify the folder you want to _flyswot_ to check for "fake" flysheets. If you are using _flyswot_ for the first time it may make sense to choose a folder which doesn\'t contain a huge number of collection items so you don\'t have to wait to long for _flyswot_ to finish running. Once you have found a directory you want to predict against copy the path. This path should be the full path to the item.\n\nFor example something that looks like:\n\n```console\n\\\\ad\\collections\\hmd\\excitingcollection\\excitingsubcollection\\\n```\n\nThis will be the folder from which _flyswot_ starts looking.\n\nWhen you activated your conda environment in a terminal, you were likely \'inside\' your user directory. Since we need to specify a place for _flyswot_ to store the CSV report, we\'ll move to a better place to store that output; your `Desktop` folder. To do we can navigate using the command:\n\n```console\n$ chdir desktop\n```\n\nif you are using Mac, Linux or have GitBash installed you should instead run:\n\n```console\n$ cd Desktop\n```\n\nThis will take you to your Desktop. We\'ll now run _flyswot_. As with many other command line tools, _flyswot_ has commands and sub-commands. We are interested in the `predict` command. This includes two sub-commands: `predict-image` and `directory`. We will mostly want to predict directories. To do this we use the following approach. Since we only care about checking things with `fs` in the filename we can specify this as our `pattern`.\n\n```console\n$ flyswot predict directory input_directory output_directory --pattern fs\n```\n\nThe input directory is the folder containing our images and the output directory is where we want to save our CSV report. Using the folder we previously identified this would look like:\n\n```console\n$ flyswot predict directory "\\\\ad\\collections\\hmd\\excitingcollection\\excitingsubcollection\\" .\n```\n\nWe can use `.` to indicate we want the CSV report to be saved to the current directory (in this case the Deskop directory). Also notice that there are quotation marks `""` around the path. This is used to make sure that any spaces in the path are escaped.\n\nOnce you run this command you should see some progress reported by _flyswot_, including a progress bar that shows how many of the images _flyswot_ has predicted against.\n\nWhen _flyswot_ has finished you will have a CSV \'report\' which contains the path to the image, the predicted label and the confidence for that prediction.\n\n## License\n\nDistributed under the terms of the [MIT license],\n_flyswot_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[cookiecutter]: https://github.com/audreyr/cookiecutter\n[mit license]: https://opensource.org/licenses/MIT\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/davanstrien/flyswot/issues\n[pip]: https://pip.pypa.io/\n[installation]: https://flyswot.readthedocs.io/en/latest/installation.html\n\n<!-- github-only -->\n\n[contributor guide]: https://github.com/davanstrien/flyswot/blob/main/CONTRIBUTING.md\n[background]: https://flyswot.readthedocs.io/en/latest/background.html\n',
     'author': 'Daniel van Strien',
     'author_email': 'daniel.van-strien@bl.uk',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/davanstrien/flyswot',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8.0,<4.0.0',
```

### Comparing `flyswot-0.3.8/PKG-INFO` & `flyswot-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: flyswot
-Version: 0.3.8
+Version: 0.3.9
 Summary: flyswot
 Home-page: https://github.com/davanstrien/flyswot
 License: MIT
 Author: Daniel van Strien
 Author-email: daniel.van-strien@bl.uk
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Pillow (>=8,<10)
 Requires-Dist: huggingface-hub (>=0.2.1,<0.10.0)
 Requires-Dist: numpy (>=1.20,<2.0)
 Requires-Dist: rich (>=10.1,<13.0)
```

