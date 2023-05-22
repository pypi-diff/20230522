# Comparing `tmp/rvt_py-2.1.0.tar.gz` & `tmp/rvt_py-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rvt_py-2.1.0.tar", last modified: Sun Mar  6 19:31:35 2022, max compression
+gzip compressed data, was "rvt_py-2.2.0.tar", last modified: Mon May 22 19:15:45 2023, max compression
```

## Comparing `rvt_py-2.1.0.tar` & `rvt_py-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-03-06 19:31:35.000000 rvt_py-2.1.0/
--rw-rw-rw-   0        0        0    11567 2021-01-08 07:43:58.000000 rvt_py-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     5261 2022-03-06 19:31:35.000000 rvt_py-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4137 2021-09-14 06:51:57.000000 rvt_py-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-03-06 19:31:35.000000 rvt_py-2.1.0/rvt/
--rw-rw-rw-   0        0        0      468 2021-01-08 12:43:40.000000 rvt_py-2.1.0/rvt/__init__.py
--rw-rw-rw-   0        0        0    73858 2022-01-30 21:16:26.000000 rvt_py-2.1.0/rvt/blend.py
--rw-rw-rw-   0        0        0    18393 2022-01-27 19:59:50.000000 rvt_py-2.1.0/rvt/blend_func.py
--rw-rw-rw-   0        0        0   152384 2022-03-06 11:34:40.000000 rvt_py-2.1.0/rvt/default.py
--rw-rw-rw-   0        0        0    23064 2022-02-13 19:20:21.000000 rvt_py-2.1.0/rvt/tile.py
--rw-rw-rw-   0        0        0    65562 2022-01-27 19:45:57.000000 rvt_py-2.1.0/rvt/vis.py
-drwxrwxrwx   0        0        0        0 2022-03-06 19:31:35.000000 rvt_py-2.1.0/rvt_py.egg-info/
--rw-rw-rw-   0        0        0     5261 2022-03-06 19:31:34.000000 rvt_py-2.1.0/rvt_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2022-03-06 19:31:34.000000 rvt_py-2.1.0/rvt_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-06 19:31:34.000000 rvt_py-2.1.0/rvt_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2022-03-06 19:31:34.000000 rvt_py-2.1.0/rvt_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-03-06 19:31:34.000000 rvt_py-2.1.0/rvt_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      876 2022-03-06 19:31:35.000000 rvt_py-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1441 2022-03-06 19:30:36.000000 rvt_py-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:45.835048 rvt_py-2.2.0/
+-rw-rw-rw-   0        0        0    11567 2021-01-08 07:43:58.000000 rvt_py-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5875 2023-05-22 19:15:45.835048 rvt_py-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4792 2023-05-21 19:08:15.000000 rvt_py-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:45.812049 rvt_py-2.2.0/rvt/
+-rw-rw-rw-   0        0        0      484 2023-05-21 19:08:15.000000 rvt_py-2.2.0/rvt/__init__.py
+-rw-rw-rw-   0        0        0    74233 2023-05-21 19:08:15.000000 rvt_py-2.2.0/rvt/blend.py
+-rw-rw-rw-   0        0        0    19373 2023-05-21 20:29:49.000000 rvt_py-2.2.0/rvt/blend_func.py
+-rw-rw-rw-   0        0        0   156675 2023-05-21 19:08:15.000000 rvt_py-2.2.0/rvt/default.py
+-rw-rw-rw-   0        0        0    23080 2023-05-21 19:08:15.000000 rvt_py-2.2.0/rvt/tile.py
+-rw-rw-rw-   0        0        0    68259 2023-05-21 20:03:46.000000 rvt_py-2.2.0/rvt/vis.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:15:45.833049 rvt_py-2.2.0/rvt_py.egg-info/
+-rw-rw-rw-   0        0        0     5875 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      876 2023-05-22 19:15:45.838051 rvt_py-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1441 2023-05-22 19:15:35.000000 rvt_py-2.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rvt_py-2.1.0/LICENSE` & `rvt_py-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rvt_py-2.1.0/PKG-INFO` & `rvt_py-2.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,120 @@
 Metadata-Version: 2.1
 Name: rvt_py
-Version: 2.1.0
-Summary: Relief Visualization Toolbox python library. It helps scientist visualize raster elevation model datasets. 
+Version: 2.2.0
+Summary: Relief Visualization Toolbox Python library. It helps scientist visualize raster elevation model datasets. 
 Home-page: https://github.com/EarthObservation/RVT_py
 Author: ZRC SAZU and University of Ljubljana (UL FGG)
 Author-email: ziga.kokalj@zrc-sazu.si
-License: UNKNOWN
 Project-URL: Documentation, https://rvt-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/EarthObservation/RVT_py
 Project-URL: Old RVT, https://iaps.zrc-sazu.si/en/rvt#v
 Project-URL: ArcGIS Pro, https://github.com/EarthObservation/rvt-arcgis-pro
 Project-URL: QGIS plugin, https://github.com/EarthObservation/rvt-qgis
 Keywords: relief_visualization_toolbox relief_visualization relief rvt raster raster_visualization visualization
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Relief Visualization Toolbox in Python
+[![PyPI](https://img.shields.io/pypi/v/RVT_py?style=flat-square)](https://pypi.org/project/rvt-py/)
+[![Anaconda-Server Badge](https://anaconda.org/zmigyyy/rvt_py/badges/version.svg)](https://anaconda.org/zmigyyy/rvt_py)
+[![Anaconda-Server Badge](https://anaconda.org/zmigyyy/rvt_py/badges/latest_release_date.svg)](https://anaconda.org/zmigyyy/rvt_py)
+
+# Relief Visualization Toolbox Python library
 
 ![](./docs/figures/RVT_head.png)
 
-Relief Visualization Toolbox was produced to help scientist visualize raster elevation model datasets. We have narrowed down the selection to include techniques that have proven to be effective for identification of small scale features. Default settings therefore assume working with high resolution digital elevation models, derived from airborne laser scanning missions (lidar).
+Relief Visualization Toolbox (RVT) was produced to help scientists visualize raster elevation model datasets. We have narrowed down the selection to include techniques that have proven to be effective for identification of small scale features. The default settings therefore assume working with high resolution digital elevation models derived from airborne laser scanning missions (lidar), however RVT methods can also be used for other purposes.
 
-Despite this, techniques are also used for different other purposes. Sky-view factor, for example, can be efficiently used in numerous studies where digital elevation model visualizations and automatic feature extraction techniques are indispensable, e.g. in geography, archeology,  geomorphology, cartography, hydrology, glaciology, forestry and disaster management. It can be used even in engineering applications, such as, predicting the availability of the GPS signal in urban areas.
+Sky-view factor, for example, can be efficiently used in numerous studies where digital elevation model visualizations and automatic feature extraction techniques are indispensable, e.g. in geography, archaeology,  geomorphology, cartography, hydrology, glaciology, forestry and disaster management. It can even be used in engineering applications, such as predicting the availability of the GPS signal in urban areas.
 
 Methods currently implemented are:
 
-*   hillshading,
-*   hillshading from multiple directions,
-*   slope gradient,
-*   simple local relief model,
-*   multi-scale relief model,
-*   sky illumination,
-*   sky-view factor (as developed by our team),
-*   anisotropic sky-view factor,
-*   positive and negative openness,
-*   local dominance,
+* hillshading,
+* hillshading from multiple directions,
+* slope gradient,
+* simple local relief model,
+* multi-scale relief model,
+* sky illumination,
+* sky-view factor (as developed by our team),
+* anisotropic sky-view factor,
+* positive and negative openness,
+* local dominance,
 *	multi-scale topographic position.
 
-For a more detailed description see references given at each method in the manual and a comparative paper describing them (e.g. Kokalj and Hesse 2017, see below).
+## RVT for Python
+
+The ``rvt`` Python package contains three modules:
 
-RVT python library called rvt contains 3 modules: vis (rvt.vis), blend (rvt.blend) and default (rvt.default). Modules contains:
-* vis       -   visualization functions (mentioned above), for computing visualizations;
-* blend     -   blender (mixer), for blending visualizations;
-* default   -   default values, class for defining default parameters with methods to compute and save visualization functions using set parameters.
+* `rvt.vis` for computing visualizations
 
-For every visualization function directory also contains Python Esri raster functions for ArcGIS Pro (rvt_esri_*.py).
+* `rvt.blend` for blending visualizations together
+  
+* ``rvt.default`` for defining default parameters with methods to compute and save visualization functions using set parameters
 
 ## References
 
 When using the tools, please cite:
 
 *   Kokalj, Ž., Somrak, M. 2019. Why Not a Single Image? Combining Visualizations to Facilitate Fieldwork and On-Screen Mapping. Remote Sensing 11(7): 747.
 *   Zakšek, K., Oštir, K., Kokalj, Ž. 2011. Sky-View Factor as a Relief Visualization Technique. Remote Sensing 3: 398-415.
 
 ## Installation
 
-### conda
+The RVT Python package can be installed using Conda or PyPI, and can be used in Python scripts, Jupyter Notebooks and ArcGIS Pro.
+
+RVT can also be installed as [a set of custom raster functions for ArcGIS](https://rvt-py.readthedocs.io/en/latest/install_arcgis.html "ArcGIS installation"), and [a plugin for QGIS](https://rvt-py.readthedocs.io/en/latest/install_qgis.html "QGIS installation").
+
+You can also clone the repository.
+
+### Conda
+
+The ``rvt`` package is [available from the Anaconda Cloud repository](https://anaconda.org/rvtpy/rvt_py "rvt_py on Anaconda Cloud"). Using Conda to install the ``rvt`` package will include all required libraries.
+
+To use this method, first [install Anaconda and Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html "Getting started with conda").
 
-You can install all required libraries and rvt-py with Anaconda environment from Anaconda cloud ([conda rvt_py](https://anaconda.org/zmigyyy/rvt_py)). To do that open Anaconda Prompt (activate conda environment) and run:
+Then open Anaconda Prompt (Windows) or Terminal (MacOS) and run:
 
-`conda install -c zmigyyy rvt_py`
+``conda install -c rvtpy rvt_py``
 
-### pypi
+### PyPI
 
-Another option is to install required libraries and rvt-py with Python Package Index, pypi ([pypi rvt-py](https://pypi.org/project/rvt-py)). To do that open command prompt (terminal) and run:
+Another option is to install the ``rvt-py`` package and required libraries [using the Python Package Index (PyPI)](https://pypi.org/project/rvt-py "rvt-py on PyPI").
 
-`pip install rvt-py`
+PyPI usually has problems installing ``gdal``, so [install ``gdal`` first](https://pypi.org/project/GDAL/ "GDAL on PyPI") to use this method.
 
-This might not work, because pypi usually has problems installing gdal. To solve that first try to install gdal then run above command.
+Then open Command Prompt (Windows) or Terminal (MacOS) and run:
 
-### requirements
+``pip install rvt-py``
 
-We suggest using an Anaconda environment (easiest gdal installation) and Python 3.6 or higher. Required libraries with tested versions (could also work with other versions):
+### Requirements
+
+Required libraries (specified versions have been tested, other versions may also work):
 
 *   numpy 1.19.2
 *   scipy 1.5.2
 *   gdal 3.0.2
 
-
-You can also clone the repository ([github rvt_py](https://github.com/EarthObservation/RVT_py)).
-
-Library `rvt-py` can be used in Python scripts, Jupyter Notebooks and in ArcGIS Pro.
+We recommend using Python 3.6 or higher and a Conda environment (this works best with ``gdal``).
 
 ## Documentation
-
-Documentation of the package and its usage is available at [Relief Visualization Toolbox in Python documentation](https://rvt-py.readthedocs.io/).
+Documentation of the package and its use is available at [Relief Visualization Toolbox in Python documentation](https://rvt-py.readthedocs.io/).
 
 ## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-Please report any bugs and suggestions for improvements.
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please report any bugs and suggestions for improvements.
 
 ## Acknowledgment
-
 Development of RVT Python scripts was part financed by the Slovenian Research Agency core funding No. P2-0406, and by research project No. J6-9395.
 
 ## License
 This project is licensed under the terms of the [Apache License](LICENSE).
 
+## About
+RVT Python library by Žiga Kokalj, Žiga Maroh, Krištof Oštir, Klemen Zakšek and Nejc Čož, 2022.
+
+It is developed in collaboration between ZRC SAZU and University of Ljubljana.
```

### Comparing `rvt_py-2.1.0/README.md` & `rvt_py-2.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,99 @@
-# Relief Visualization Toolbox in Python
+[![PyPI](https://img.shields.io/pypi/v/RVT_py?style=flat-square)](https://pypi.org/project/rvt-py/)
+[![Anaconda-Server Badge](https://anaconda.org/zmigyyy/rvt_py/badges/version.svg)](https://anaconda.org/zmigyyy/rvt_py)
+[![Anaconda-Server Badge](https://anaconda.org/zmigyyy/rvt_py/badges/latest_release_date.svg)](https://anaconda.org/zmigyyy/rvt_py)
+
+# Relief Visualization Toolbox Python library
 
 ![](./docs/figures/RVT_head.png)
 
-Relief Visualization Toolbox was produced to help scientist visualize raster elevation model datasets. We have narrowed down the selection to include techniques that have proven to be effective for identification of small scale features. Default settings therefore assume working with high resolution digital elevation models, derived from airborne laser scanning missions (lidar).
+Relief Visualization Toolbox (RVT) was produced to help scientists visualize raster elevation model datasets. We have narrowed down the selection to include techniques that have proven to be effective for identification of small scale features. The default settings therefore assume working with high resolution digital elevation models derived from airborne laser scanning missions (lidar), however RVT methods can also be used for other purposes.
 
-Despite this, techniques are also used for different other purposes. Sky-view factor, for example, can be efficiently used in numerous studies where digital elevation model visualizations and automatic feature extraction techniques are indispensable, e.g. in geography, archeology,  geomorphology, cartography, hydrology, glaciology, forestry and disaster management. It can be used even in engineering applications, such as, predicting the availability of the GPS signal in urban areas.
+Sky-view factor, for example, can be efficiently used in numerous studies where digital elevation model visualizations and automatic feature extraction techniques are indispensable, e.g. in geography, archaeology,  geomorphology, cartography, hydrology, glaciology, forestry and disaster management. It can even be used in engineering applications, such as predicting the availability of the GPS signal in urban areas.
 
 Methods currently implemented are:
 
-*   hillshading,
-*   hillshading from multiple directions,
-*   slope gradient,
-*   simple local relief model,
-*   multi-scale relief model,
-*   sky illumination,
-*   sky-view factor (as developed by our team),
-*   anisotropic sky-view factor,
-*   positive and negative openness,
-*   local dominance,
+* hillshading,
+* hillshading from multiple directions,
+* slope gradient,
+* simple local relief model,
+* multi-scale relief model,
+* sky illumination,
+* sky-view factor (as developed by our team),
+* anisotropic sky-view factor,
+* positive and negative openness,
+* local dominance,
 *	multi-scale topographic position.
 
-For a more detailed description see references given at each method in the manual and a comparative paper describing them (e.g. Kokalj and Hesse 2017, see below).
+## RVT for Python
+
+The ``rvt`` Python package contains three modules:
 
-RVT python library called rvt contains 3 modules: vis (rvt.vis), blend (rvt.blend) and default (rvt.default). Modules contains:
-* vis       -   visualization functions (mentioned above), for computing visualizations;
-* blend     -   blender (mixer), for blending visualizations;
-* default   -   default values, class for defining default parameters with methods to compute and save visualization functions using set parameters.
+* `rvt.vis` for computing visualizations
 
-For every visualization function directory also contains Python Esri raster functions for ArcGIS Pro (rvt_esri_*.py).
+* `rvt.blend` for blending visualizations together
+  
+* ``rvt.default`` for defining default parameters with methods to compute and save visualization functions using set parameters
 
 ## References
 
 When using the tools, please cite:
 
 *   Kokalj, Ž., Somrak, M. 2019. Why Not a Single Image? Combining Visualizations to Facilitate Fieldwork and On-Screen Mapping. Remote Sensing 11(7): 747.
 *   Zakšek, K., Oštir, K., Kokalj, Ž. 2011. Sky-View Factor as a Relief Visualization Technique. Remote Sensing 3: 398-415.
 
 ## Installation
 
-### conda
+The RVT Python package can be installed using Conda or PyPI, and can be used in Python scripts, Jupyter Notebooks and ArcGIS Pro.
+
+RVT can also be installed as [a set of custom raster functions for ArcGIS](https://rvt-py.readthedocs.io/en/latest/install_arcgis.html "ArcGIS installation"), and [a plugin for QGIS](https://rvt-py.readthedocs.io/en/latest/install_qgis.html "QGIS installation").
+
+You can also clone the repository.
+
+### Conda
+
+The ``rvt`` package is [available from the Anaconda Cloud repository](https://anaconda.org/rvtpy/rvt_py "rvt_py on Anaconda Cloud"). Using Conda to install the ``rvt`` package will include all required libraries.
+
+To use this method, first [install Anaconda and Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html "Getting started with conda").
+
+Then open Anaconda Prompt (Windows) or Terminal (MacOS) and run:
 
-You can install all required libraries and rvt-py with Anaconda environment from Anaconda cloud ([conda rvt_py](https://anaconda.org/zmigyyy/rvt_py)). To do that open Anaconda Prompt (activate conda environment) and run:
+``conda install -c rvtpy rvt_py``
 
-`conda install -c zmigyyy rvt_py`
+### PyPI
 
-### pypi
+Another option is to install the ``rvt-py`` package and required libraries [using the Python Package Index (PyPI)](https://pypi.org/project/rvt-py "rvt-py on PyPI").
 
-Another option is to install required libraries and rvt-py with Python Package Index, pypi ([pypi rvt-py](https://pypi.org/project/rvt-py)). To do that open command prompt (terminal) and run:
+PyPI usually has problems installing ``gdal``, so [install ``gdal`` first](https://pypi.org/project/GDAL/ "GDAL on PyPI") to use this method.
 
-`pip install rvt-py`
+Then open Command Prompt (Windows) or Terminal (MacOS) and run:
 
-This might not work, because pypi usually has problems installing gdal. To solve that first try to install gdal then run above command.
+``pip install rvt-py``
 
-### requirements
+### Requirements
 
-We suggest using an Anaconda environment (easiest gdal installation) and Python 3.6 or higher. Required libraries with tested versions (could also work with other versions):
+Required libraries (specified versions have been tested, other versions may also work):
 
 *   numpy 1.19.2
 *   scipy 1.5.2
 *   gdal 3.0.2
 
-
-You can also clone the repository ([github rvt_py](https://github.com/EarthObservation/RVT_py)).
-
-Library `rvt-py` can be used in Python scripts, Jupyter Notebooks and in ArcGIS Pro.
+We recommend using Python 3.6 or higher and a Conda environment (this works best with ``gdal``).
 
 ## Documentation
-
-Documentation of the package and its usage is available at [Relief Visualization Toolbox in Python documentation](https://rvt-py.readthedocs.io/).
+Documentation of the package and its use is available at [Relief Visualization Toolbox in Python documentation](https://rvt-py.readthedocs.io/).
 
 ## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-Please report any bugs and suggestions for improvements.
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please report any bugs and suggestions for improvements.
 
 ## Acknowledgment
-
 Development of RVT Python scripts was part financed by the Slovenian Research Agency core funding No. P2-0406, and by research project No. J6-9395.
 
 ## License
 This project is licensed under the terms of the [Apache License](LICENSE).
 
+## About
+RVT Python library by Žiga Kokalj, Žiga Maroh, Krištof Oštir, Klemen Zakšek and Nejc Čož, 2022.
+
+It is developed in collaboration between ZRC SAZU and University of Ljubljana. 
+
+
```

### Comparing `rvt_py-2.1.0/rvt/blend.py` & `rvt_py-2.2.0/rvt/blend.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,31 +7,33 @@
     Žiga Kokalj (ziga.kokalj@zrc-sazu.si)
     Krištof Oštir (kristof.ostir@fgg.uni-lj.si)
     Klemen Zakšek
     Peter Pehani
     Klemen Čotar
     Maja Somrak
     Žiga Maroh
+    Nejc Čož
 
 Copyright:
     2010-2020 Research Centre of the Slovenian Academy of Sciences and Arts
     2016-2020 University of Ljubljana, Faculty of Civil and Geodetic Engineering
 """
 
 # TODO: more testing, find and fix bugs if they exists
 
-# python libraries
-import numpy as np
+import datetime
+import json
+import os
 import warnings
+
+import numpy as np
+
 import rvt.default
 import rvt.vis
 from rvt.blend_func import *
-import os
-import json
-import datetime
 
 
 def create_blender_file_example(file_path=None):
     """Create blender .json file example (can be changed and read). Example is VAT - Archaeological combination"""
     data = {"combination": {"name": "VAT - Archaeological",
                             "layers":
                                 [
@@ -234,15 +236,14 @@
 
     def read_from_json(self, json_data):
         """Fill class attributes with json data."""
         self.layers = []
         self.name = json_data["combination"]["name"]
         layers_data = json_data["combination"]["layers"]
         for layer in layers_data:
-            layer_name = layer["layer"]
             if layer["visualization_method"] is None:
                 continue
             if layer["visualization_method"].lower() == "none" or layer["visualization_method"].lower() == "null":
                 continue
             else:
                 vis_method = str(layer["visualization_method"])
             norm = str(layer["norm"])
@@ -336,70 +337,91 @@
         path. If both image and image_path are None method calculates visualization. If save_visualization is True
         method needs dem_path and saves each visualization (if it doesn't exists) in directory of dem_path,
         else (save_visualization=False) method needs dem_arr, dem_resolution and calculates each visualization
         simultaneously (in memory). Be careful save_visualisation applies only if specific BlenderLayer
         image and image_path are None. Parameter no_data changes all pixels with this values to np.nan,
         if save_visualizations is Ture it is not needed."""
 
-        # check data
+        # Preform checks
         self.check_data()
 
         if save_render_path is not None and self.dem_path is None:
             raise Exception(
                 "rvt.blend.BlenderCombination.render_all_images: If you would like to save rendered image (blender), "
                 "you have to define dem_path (BlenderCombination.add_dem_path())!")
+
         if not save_float and not save_8bit and save_render_path:
             raise Exception(
                 "rvt.blend.BlenderCombination.render_all_images: If you would like to save rendered image (blender), "
                 "you have to set save_float or save_8bit to True!")
+
+        # Prepare directory for saving renders
         if save_render_path is not None:
             save_render_directory = os.path.abspath(os.path.dirname(save_render_path))
-            save_render_8bit_path = r"{}\{}_8bit.tif".format(save_render_directory,
-                                                             os.path.splitext(os.path.basename(save_render_path))[0])
+            save_render_8bit_path = os.path.join(
+                save_render_directory,
+                "{}_8bit.tif".format(os.path.splitext(os.path.basename(save_render_path))[0])
+            )
         else:
             save_render_directory = None
+            save_render_8bit_path = None
 
-        # default is rvt.default.DefaultValues class
-        if default is None:  # if not defined, predefined values are used
+        # If default (rvt.default.DefaultValues class) is not defined, use predefined values
+        if default is None:
             default = rvt.default.DefaultValues()
 
-        # rendering across all layers - form last to first layer
-        rendered_image = []
+        # Rendering across all layers - form last to first layer
+        rendered_image = None
         for i_img in range(len(self.layers) - 1, -1, -1):
+
+            # Get visualization type (string)
             visualization = self.layers[i_img].vis
             if visualization is None:  # empty layer, skip
                 continue
 
+            # Get other parameters for processing this layer
             min_norm = self.layers[i_img].min
             max_norm = self.layers[i_img].max
             normalization = self.layers[i_img].normalization
             image = self.layers[i_img].image
             image_path = self.layers[i_img].image_path
 
             if save_visualizations and self.dem_path is None and image_path is None and image is None:
                 raise Exception(
                     "rvt.blend.BlenderCombination.render_all_images: If you would like to save visualizations, "
                     "you have to define dem_path (BlenderCombination.add_dem_path())!")
+
             if not save_visualizations and self.dem_arr is None and self.dem_resolution is None and \
                     image_path is None and image is None:
                 raise Exception(
                     "rvt.blend.BlenderCombination.render_all_images: If you would like to compute visualizations, "
                     "you have to define dem_arr and its resolution (BlenderCombination.add_dem_arr())!")
 
-            # normalize images
-            # if image is not presented and image_path is
+            # Normalize images
             norm_image = None
             if image is None and image_path is not None:
-                norm_image = normalize_image(visualization, rvt.default.get_raster_arr(image_path)["array"], min_norm,
-                                             max_norm, normalization)
-            # if image is presented
+                # LOAD image from file if it doesn't exist (as an array) but we have image_path present
+                norm_image = normalize_image(
+                    visualization,
+                    rvt.default.get_raster_arr(image_path)["array"],
+                    min_norm,
+                    max_norm,
+                    normalization
+                )
             elif image is not None:
-                norm_image = normalize_image(visualization, image, min_norm, max_norm, normalization)
-            # they are both none
+                # if image exist (as an array)
+                norm_image = normalize_image(
+                    visualization,
+                    image,
+                    min_norm,
+                    max_norm,
+                    normalization
+                )
             else:
+                # calculate image from DEM
                 if self.layers[i_img].vis.lower() == "slope gradient":
                     if save_visualizations:
                         default.save_slope(dem_path=self.dem_path, custom_dir=save_render_directory, save_float=True,
                                            save_8bit=False)
                         image_path = default.get_slope_path(self.dem_path)
                         norm_image = normalize_image(visualization, rvt.default.get_raster_arr(image_path)["array"],
                                                      min_norm, max_norm, normalization)
@@ -543,57 +565,70 @@
                         norm_image = normalize_image(visualization, rvt.default.get_raster_arr(image_path)["array"],
                                                      min_norm, max_norm, normalization)
                     else:
                         image = default.get_msrm(dem_arr=self.dem_arr, resolution=self.dem_resolution, no_data=no_data)
                         norm_image = normalize_image(visualization, image, min_norm, max_norm, normalization)
                 elif self.layers[i_img].vis.lower() == "multi-scale topographic position":
                     if save_visualizations:
-                        default.save_mstp(dem_path=self.dem_path, custom_dir=save_render_directory)
+                        default.save_mstp(
+                            dem_path=self.dem_path, custom_dir=save_render_directory, save_float=True, save_8bit=False
+                        )
                         image_path = default.get_mstp_path(self.dem_path)
                         norm_image = normalize_image(visualization, rvt.default.get_raster_arr(image_path)["array"],
                                                      min_norm, max_norm, normalization)
                     else:
                         image = default.get_mstp(dem_arr=self.dem_arr, no_data=no_data)
                         norm_image = normalize_image(visualization, image, min_norm, max_norm, normalization)
 
+            # Apply colormap
             colormap = self.layers[i_img].colormap
             min_colormap_cut = self.layers[i_img].min_colormap_cut
             max_colormap_cut = self.layers[i_img].max_colormap_cut
             if colormap is not None and len(image.shape) < 3:
                 norm_image = gray_scale_to_color_ramp(gray_scale=norm_image, colormap=colormap, output_8bit=False,
                                                       min_colormap_cut=min_colormap_cut,
                                                       max_colormap_cut=max_colormap_cut)
 
-            # if current layer has visualization applied, but there has been no rendering
-            # of images yet, than current layer will be the initial value of rendered_image
-            if rendered_image == []:
+            # Blend current layer with background layer
+            if not rendered_image:
+                # if current layer has visualization applied, but there has been no rendering
+                # of images yet, than current layer will be the initial value of rendered_image
                 rendered_image = norm_image
                 continue
             else:
                 active = norm_image
                 background = rendered_image
-                blend_mode = self.layers[i_img].blend_mode
-                opacity = self.layers[i_img].opacity
+
+                # Scale images if needed
                 if np.nanmin(active) < 0 or np.nanmax(active) > 1:
                     active = scale_0_to_1(active)
                 if np.nanmin(background) < 0 or np.nanmax(background) > 1:
                     background = scale_0_to_1(background)
+
+                # Blend background with active layer
+                blend_mode = self.layers[i_img].blend_mode
                 top = blend_images(blend_mode, active, background)
+
+                # Apply opacity
+                opacity = self.layers[i_img].opacity
                 rendered_image = render_images(top, background, opacity)
 
-                if np.nanmin(rendered_image) < 0 or np.nanmax(rendered_image > 1):
+                if np.nanmin(rendered_image) < 0 or np.nanmax(rendered_image) > 1:
                     warnings.warn("rvt.blend.BlenderCombination.render_all_images: Rendered image scale distorted")
-        if save_render_path is not None:  # if paths presented it saves image
+
+        # Save image to file if path is present
+        if save_render_path is not None:
             if save_float:
                 rvt.default.save_raster(src_raster_path=self.dem_path, out_raster_path=save_render_path,
                                         out_raster_arr=rendered_image)
             if save_8bit:
                 rendered_image_8bit = rvt.vis.byte_scale(rendered_image, c_min=0, c_max=1)
                 rvt.default.save_raster(src_raster_path=self.dem_path, out_raster_path=save_render_8bit_path,
                                         out_raster_arr=rendered_image_8bit, e_type=1)
+
         return rendered_image  # returns float
 
     def create_log_file(self, dem_path, combination_name, render_path, default: rvt.default.DefaultValues,
                         terrain_sett_name=None, custom_dir=None, computation_time=None):
         """Creates log file in custom_dir, if custom_dir=None it creates it in dem directory (dem_path)."""
         dict_arr_res = rvt.default.get_raster_arr(raster_path=dem_path)
         resolution = dict_arr_res["resolution"]
@@ -758,15 +793,15 @@
         List of BlenderCombination instances.
     """
 
     def __init__(self):
         self.combinations = []  # list of BlenderCombination
 
     def add_combination(self, combination: BlenderCombination, name=None):
-        """Adds cobmination if parameter name not None it renames combination."""
+        """Adds combination if parameter name not None it renames combination."""
         if name is not None:
             combination.name = name
         self.combinations.append(combination)
 
     def remove_all_combinations(self):
         """Removes all combinations from self.combinations."""
         self.combinations = []
@@ -847,15 +882,15 @@
         self.svf_r_max = None
         self.svf_noise = None
         # anisotropic sky-view factor
         self.asvf_dir = None
         self.asvf_level = None
         # positive openness
         # negative openness
-        # sky_illum
+        # sky_illumination
         self.sim_sky_mod = None
         self.sim_compute_shadow = None
         self.sim_nr_dir = None
         self.sim_shadow_dist = None
         self.sim_shadow_az = None
         self.sim_shadow_el = None
         # local dominance
@@ -1223,29 +1258,23 @@
     ----------
     dem : numpy.ndarray
         Input digital elevation model as 2D numpy array.
     resolution : float
         DEM pixel size.
     default : rvt.default.DefaultValues
         Default values for visualization functions.
-    slope_norm : tuple(mode, min, max)
-        Cutoff normalization for slope.
-        Mode can be 'value' or 'percent' (cut-off units).
-        Values min and max define stretch borders (in mode units).
-    op_on_norm : tuple(mode, min, max)
-        Cutoff normalization for (openness positive - openness negative).
-        Mode can be 'value' or 'percent' (cut-off units).
-        Values min and max define stretch borders (in mode units).
     colormap : str
         Colormap form matplotlib (https://matplotlib.org/3.3.2/tutorials/colors/colormaps.html).
     min_colormap_cut : float
-        What lower part of colormap to cut. Between 0 and 1, if 0.2 it cuts off (deletes) 20% of lower colors in colormap.
+        What lower part of colormap to cut. Between 0 and 1, if 0.2 it cuts off (deletes) 20% of lower colors in
+        colormap.
         If None cut is not applied.
     max_colormap_cut : float
-        What upper part of colormap to cut. Between 0 and 1, if 0.8 it cuts off (deletes) 20% of upper colors in colormap.
+        What upper part of colormap to cut. Between 0 and 1, if 0.8 it cuts off (deletes) 20% of upper colors in
+        colormap.
         If None cut is not applied.
     no_data : int or float
         Value that represents no_data, all pixels with this value are changed to np.nan .
 
     Returns
     -------
     crim_out : numpy.ndarray
@@ -1261,39 +1290,45 @@
     opns_pos_arr = default.get_sky_view_factor(dem_arr=dem, resolution=resolution,
                                                compute_svf=False, compute_asvf=False, compute_opns=True,
                                                no_data=None)["opns"]
     opns_neg_arr = default.get_sky_view_factor(dem_arr=-1 * dem, resolution=resolution,
                                                compute_svf=False, compute_asvf=False, compute_opns=True,
                                                no_data=None)["opns"]
     opns_pos_neg_arr = opns_pos_arr - opns_neg_arr
-    slope_arr = rvt.vis.slope_aspect(dem=dem, resolution_x=resolution, resolution_y=resolution, output_units="radian")[
-        "slope"]
+
+    slope_arr = rvt.vis.slope_aspect(
+        dem=dem,
+        resolution_x=resolution,
+        resolution_y=resolution,
+        output_units="radian"
+    )["slope"]
 
     blend_combination = rvt.blend.BlenderCombination()
     blend_combination.create_layer(vis_method="Openness_Pos-Neg", normalization=op_on_norm[0], minimum=op_on_norm[1],
                                    maximum=op_on_norm[2], blend_mode="overlay", opacity=50,
                                    image=opns_pos_neg_arr)
     blend_combination.create_layer(vis_method="Openness_Pos-Neg", normalization=op_on_norm[0], minimum=op_on_norm[1],
                                    maximum=op_on_norm[2], blend_mode="luminosity", opacity=50,
                                    image=opns_pos_neg_arr)
     blend_combination.create_layer(vis_method="slope gradient rad", normalization=slope_norm[0], minimum=slope_norm[1],
                                    maximum=slope_norm[2], blend_mode="normal", opacity=100, colormap=colormap,
                                    min_colormap_cut=min_colormap_cut, max_colormap_cut=max_colormap_cut,
                                    image=slope_arr)
     crim_out = blend_combination.render_all_images()
+
     return crim_out
 
 
 def e3mstp(dem, resolution, default: rvt.default.DefaultValues = rvt.default.DefaultValues(), no_data=None):
     """
-    RVT enahanced version 3 Multi-scale topographic position (e3MSTP)
+    RVT enhanced version 3 Multi-scale topographic position (e3MSTP)
     Blending combination where layers are:
-    1st: Simple local relief model (SLRM), sreen, 25% opacity
+    1st: Simple local relief model (SLRM), screen, 25% opacity
     2nd: Color relief image map where cmap=Reds_r(0.5-1) (CRIM_Reds_r), soft_light, 70% opacity
-    3rd: Multi-scale topographic postion (MSTP)
+    3rd: Multi-scale topographic position (MSTP)
 
     Parameters
     ----------
     dem : numpy.ndarray
         Input digital elevation model as 2D numpy array.
     resolution : float
         DEM pixel size.
@@ -1319,14 +1354,13 @@
                                    minimum=-0.5,
                                    maximum=0.5, blend_mode="screen", opacity=25,
                                    image=slrm_arr)
     blend_combination.create_layer(vis_method="crim_red", normalization="value",
                                    minimum=0,
                                    maximum=1, blend_mode="soft_light", opacity=70,
                                    image=crim_red_arr)
-    blend_combination.create_layer(vis_method="mstp", normalization="value",
-                                   minimum=0,
-                                   maximum=255, blend_mode="normal", opacity=100,
+    blend_combination.create_layer(vis_method="mstp",
+                                   normalization="value", minimum=0, maximum=1,
+                                   blend_mode="normal", opacity=100,
                                    image=mstp_arr)
     e3mstp_out = blend_combination.render_all_images()
     return e3mstp_out
-
```

### Comparing `rvt_py-2.1.0/rvt/blend_func.py` & `rvt_py-2.2.0/rvt/blend_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Žiga Kokalj (ziga.kokalj@zrc-sazu.si)
     Krištof Oštir (kristof.ostir@fgg.uni-lj.si)
     Klemen Zakšek
     Peter Pehani
     Klemen Čotar
     Maja Somrak
     Žiga Maroh
+    Nejc Čož
 
 Copyright:
     2010-2020 Research Centre of the Slovenian Academy of Sciences and Arts
     2016-2020 University of Ljubljana, Faculty of Civil and Geodetic Engineering
 """
 
 # TODO: more testing, find and fix bugs if they exists
 
-# python libraries
-import matplotlib as mpl
-import matplotlib.cm
-import matplotlib.colors
-import numpy as np
 import warnings
 
+import numpy as np
+from matplotlib.cm import get_cmap
+from matplotlib.colors import LinearSegmentedColormap
+
 
 def gray_scale_to_color_ramp(gray_scale, colormap, min_colormap_cut=None, max_colormap_cut=None, alpha=False,
                              output_8bit=True):
     """
     Turns normalized gray scale np.array to rgba (np.array of 4 np.arrays r, g, b, a).
 
     Parameters
@@ -51,40 +51,50 @@
     output_8bit : bool
         If true output values will be int 0-255 instead of normalized values.
     Returns
     -------
     rgba_out : np.array (3D: red 0-255, green 0-255, blue 0-255)
             If alpha False: np.array (4D: red 0-255, green 0-255, blue 0-255, alpha 0-255)
     """
-    cm = mpl.cm.get_cmap(colormap)
+    cm = get_cmap(colormap)
+
+    # Truncate colormap if required
     if min_colormap_cut is not None or max_colormap_cut is not None:
         if min_colormap_cut is None:
             min_colormap_cut = 0.0
         if max_colormap_cut is None:
             max_colormap_cut = 1.0
         if min_colormap_cut > 1 or min_colormap_cut < 0 or max_colormap_cut > 1 or max_colormap_cut < 0:
-            raise Exception("rvt.blend_funct.gray_scale_to_color_ramp: min_colormap_cut and max_colormap_cut must be"
+            raise Exception("rvt.blend_func.gray_scale_to_color_ramp: min_colormap_cut and max_colormap_cut must be"
                             " between 0 and 1!")
         if min_colormap_cut >= max_colormap_cut:
-            raise Exception("rvt.blend_funct.gray_scale_to_color_ramp: min_colormap_cut can't be smaller than"
+            raise Exception("rvt.blend_func.gray_scale_to_color_ramp: min_colormap_cut can't be smaller than"
                             " max_colormap_cut!")
         cm = truncate_colormap(cmap=cm, minval=min_colormap_cut, maxval=max_colormap_cut)
-    rgba_mtpl_out = cm(gray_scale)  # normalized rgb
+
+    # Compute normalized RGBA
+    rgba_mtpl_out = cm(gray_scale)
+
     if output_8bit:
+        nan_mask = np.isnan(gray_scale)
+        rgba_mtpl_out[nan_mask] = 0  # Change nan to 0
         rgba_mtpl_out = np.uint8(rgba_mtpl_out * 255)  # 0-1 scale to 0-255 and change type to uint8
+
+    # Move array axes to correct positions, i.e. (x, y, bands) to (bands, x, y)
+    rgba_out = rgba_mtpl_out.transpose(2, 0, 1)
+
+    # Discard 4th band if not using Alpha
     if not alpha:
-        rgba_out = np.array([rgba_mtpl_out[:, :, 0], rgba_mtpl_out[:, :, 1], rgba_mtpl_out[:, :, 2]])
-    else:
-        rgba_out = np.array([rgba_mtpl_out[:, :, 0], rgba_mtpl_out[:, :, 1], rgba_mtpl_out[:, :, 2],
-                             rgba_mtpl_out[:, :, 3]])
+        rgba_out = rgba_out[:3, ...]
+
     return rgba_out
 
 
 def truncate_colormap(cmap, minval=0.0, maxval=1.0, n=100):
-    new_cmap = matplotlib.colors.LinearSegmentedColormap.from_list(
+    new_cmap = LinearSegmentedColormap.from_list(
         'trunc({n},{a:.2f},{b:.2f})'.format(n=cmap.name, a=minval, b=maxval),
         cmap(np.linspace(minval, maxval, n)))
     return new_cmap
 
 
 def normalize_lin(image, minimum, maximum):
     # linear cut off
@@ -98,18 +108,18 @@
     return np.float32(image)
 
 
 def lin_cutoff_calc_from_perc(image, minimum, maximum):
     """Minimum cutoff in percent, maximum cutoff in percent (0%-100%). Returns min and max values for linear
     stretch (cut-off)."""
     if minimum < 0 or maximum < 0 or minimum > 100 or maximum > 100:
-        raise Exception("rvt.blend_funct.lin_cutoff_calc_from_perc: minimum, maximum are percent and have to be in "
+        raise Exception("rvt.blend_func.lin_cutoff_calc_from_perc: minimum, maximum are percent and have to be in "
                         "range 0-100!")
     if minimum + maximum > 100:
-        raise Exception("rvt.blend_funct.lin_cutoff_calc_from_perc: if minimum + maximum > 100% then there are no"
+        raise Exception("rvt.blend_func.lin_cutoff_calc_from_perc: if minimum + maximum > 100% then there are no"
                         " values left! You can't cutoff whole image!")
     distribution = np.nanpercentile(a=image, q=np.array([minimum, 100 - maximum]))
     min_lin = distribution[0]
     max_lin = distribution[1]
     if min_lin == max_lin:
         min_lin = np.nanmin(image)
         max_lin = np.nanmax(image)
@@ -120,72 +130,74 @@
     min_max_lin_dict = lin_cutoff_calc_from_perc(image, minimum, maximum)
     min_lin = min_max_lin_dict["min_lin"]
     max_lin = min_max_lin_dict["max_lin"]
     return normalize_lin(image, min_lin, max_lin)
 
 
 def advanced_normalization(image, minimum, maximum, normalization):
-    equ_image = image
+    """Runs normalization based on the selected normalization type: value or percent."""
+
+    # Preform checks if correct values were given
     if minimum == maximum and normalization == "value":
         raise Exception("rvt.blend_func.advanced_normalization: If normalization == value, min and max cannot be the"
                         " same!")
+
     if minimum > maximum and normalization == "value":
         raise Exception("rvt.blend_func.advanced_normalization: If normalization == value, max can't be smaller"
                         " than min!")
+
+    # Select normalization type
     if normalization.lower() == "value":
         equ_image = normalize_lin(image=image, minimum=minimum, maximum=maximum)
     elif normalization.lower() == "perc":
         equ_image = normalize_perc(image=image, minimum=minimum, maximum=maximum)
     elif normalization is None:
         equ_image = image
-    return equ_image
-
+    else:
+        raise Exception(f"rvt.blend_func.advanced_normalization: Unknown normalization type: {normalization}")
 
-def image_join_channels(r, g, b):
-    if r.shape != g.shape or r.shape != b.shape or g.shape != b.shape:
-        raise Exception("rvt.blend.image_join_channels: r, g, b must me same dimensions!")
-    return np.array([r, g, b])
+    return equ_image
 
 
 def lum(img):
     if len(img.shape) == 3:
         r = img[0]
         g = img[1]
         b = img[2]
         lum_img = np.float32((0.3 * r) + (0.59 * g) + (0.11 * b))
     else:
         lum_img = img
 
     return lum_img
 
 
-def matrix_eq_min_lt_zero(r, idx_min_lt_zero, lum_c, min_c):
+def matrix_eq_min_lt_zero(r: np.ndarray, idx_min_lt_zero, lum_c, min_c):
     r[idx_min_lt_zero] = lum_c[idx_min_lt_zero] + (((r[idx_min_lt_zero] - lum_c[idx_min_lt_zero]) *
                                                     lum_c[idx_min_lt_zero]) / (lum_c[idx_min_lt_zero] -
                                                                                min_c[idx_min_lt_zero]))
     return r
 
 
-def matrix_eq_max_gt_one(r, idx_max_c_gt_one, lum_c, max_c):
+def matrix_eq_max_gt_one(r: np.ndarray, idx_max_c_gt_one, lum_c, max_c):
     r[idx_max_c_gt_one] = lum_c[idx_max_c_gt_one] + (((r[idx_max_c_gt_one] - lum_c[idx_max_c_gt_one]) *
                                                       (1.0 - lum_c[idx_max_c_gt_one])) / (max_c[idx_max_c_gt_one]
                                                                                           - lum_c[idx_max_c_gt_one]))
     return r
 
 
-def channel_min(r, g, b):
+def channel_min(r: np.ndarray, g: np.ndarray, b: np.ndarray):
     min_c = r * 1.0
     idx_min = np.where(g < min_c)
     min_c[idx_min] = g[idx_min]
     idx_min = np.where(b < min_c)
     min_c[idx_min] = b[idx_min]
     return min_c
 
 
-def channel_max(r, g, b):
+def channel_max(r: np.ndarray, g: np.ndarray, b: np.ndarray):
     max_c = r * 1.0
     idx_max = np.where(g > max_c)
     max_c[idx_max] = g[idx_max]
     idx_max = np.where(b > max_c)
     max_c[idx_max] = b[idx_max]
     return max_c
 
@@ -313,63 +325,76 @@
     elif blend_mode.lower() == "luminosity":
         return blend_luminosity(active, background, min_c, max_c)
     else:
         return blend_normal(active, background)
 
 
 def render_images(active, background, opacity):
+
+    # Both active and background image have to be between 0 and 1, scale if not
     if np.nanmin(active) < 0 or np.nanmax(active) > 1:
         active = scale_0_to_1(active)
     if np.nanmin(background) < 0 or np.nanmax(background) > 1:
         background = scale_0_to_1(background)
 
+    # True if image has 3 bands (RGB), false if single band
     a_rgb = len(active.shape) == 3
     b_rgb = len(background.shape) == 3
-    render_image = 0
+
+    # Apply opacity
     if a_rgb and b_rgb:
+        # Both images 3 bands
         render_image = np.zeros(background.shape)
         for i in range(3):
             render_image[i, :, :] = apply_opacity(active[i, :, :], background[i, :, :], opacity)
-    if a_rgb and not b_rgb:
+    elif a_rgb and not b_rgb:
+        # Active image 3 bands
         render_image = np.zeros(active.shape)
         for i in range(3):
             render_image[i, :, :] = apply_opacity(active[i, :, :], background, opacity)
-    if not a_rgb and b_rgb:
+    elif not a_rgb and b_rgb:
+        # Background image 3 bands
         render_image = np.zeros(background.shape)
         for i in range(3):
             render_image[i, :, :] = apply_opacity(active, background[i, :, :], opacity)
-    if not a_rgb and not b_rgb:
+    else:
         render_image = apply_opacity(active, background, opacity)
+
     return render_image
 
 
 def scale_within_0_and_1(numeric_value):
     if np.nanmin(numeric_value) >= 0 and np.nanmax(numeric_value) <= 1:
         return numeric_value
 
+    # Create mask for NaN values
+    # nan_mask = np.isnan(numeric_value)
+
     numeric_value[np.isnan(numeric_value)] = np.nanmin(numeric_value)  # nan change to nanmin
 
     actual_min = np.nanmin(numeric_value)
     norm_min_value = np.nanmax(np.array(0, actual_min))
 
     actual_max = np.nanmax(numeric_value)
     norm_max_value = np.nanmin(np.array(1, actual_max))
 
-    # do not scale values where max is between 1 and 255 if the max-min values diffrence is at least 30 and min >0
+    # Do not scale values where max is between 1 and 255 if the max-min values difference is at least 30 and min >0
     # and numeric values are integer type
     if 255 >= actual_max > 1:
         if actual_max - actual_min > 30 and actual_min > 0:
             scaled = numeric_value / 255
             return scaled
 
     scaled = (numeric_value - norm_min_value) / (norm_max_value - norm_min_value)
 
     if np.nanmin(scaled) > -0.01:
         scaled[(0 > scaled) & (scaled > -0.01)] = 0
 
+    # scaled[nan_mask] = np.nan
+
     return scaled
 
 
 def scale_strict_0_to_1(numeric_value):
     if np.nanmin(numeric_value) == 0 and np.nanmax(numeric_value) == 1:
         return numeric_value
 
@@ -398,72 +423,78 @@
 def apply_opacity(active, background, opacity):
     if opacity > 1:
         opacity = opacity / 100
     return active * opacity + background * (1 - opacity)
 
 
 def normalize_image(visualization, image, min_norm, max_norm, normalization):
+    """Main function for normalization. Runs advanced normalization on the array and preforms special operations for
+    some visualization types (e.g. invert scale for slope, scale for mhs, etc.).
+    """
     if visualization is None:
         return None
+
     if normalization == "percent":
         normalization = "perc"
 
     norm_image = advanced_normalization(image=image, minimum=min_norm, maximum=max_norm, normalization=normalization)
 
-    # make sure it scales 0 to 1
+    # Make sure it scales 0 to 1
     if np.nanmax(norm_image) > 1:
         if visualization.lower() == "multiple directions hillshade" or visualization == "mhs":
             norm_image = scale_0_to_1(norm_image)
         else:
             norm_image = scale_0_to_1(norm_image)
-            warnings.warn("rvt.blend.normalize_images_on_layers: unexpected values! max > 1")
-        if np.nanmin(norm_image) < 0:
-            warnings.warn("rvt.blend.normalize_images_on_layers: unexpected values! min < 0")
+            warnings.warn("rvt.blend_func.normalize_image: unexpected values! max > 1")
+
+    if np.nanmin(norm_image) < 0:
+        norm_image = scale_0_to_1(norm_image)
+        warnings.warn("rvt.blend_func.normalize_image: unexpected values! min < 0")
 
-    # for slope, invert scale
-    # meaning high slopes will be black
+    # For slope invert scale (high slopes will be black)
     if visualization.lower() == "slope gradient" or visualization.lower() == "openness - negative" or \
             visualization == "slp" or visualization == "neg_opns":
         norm_image = 1 - norm_image
+
     return norm_image
 
 
-def cut_off_normalize(image, mode, min=None, max=None, bool_norm=True):
+def cut_off_normalize(image, mode, cutoff_min=None, cutoff_max=None, bool_norm=True):
     """
     One band image cut-off or normalization or both. Image is 2D np.ndarray of raster, mode is perc or value
     (min and max units), min and max are minimum value to cutoff and maximum value to cutoff.
     (e.x. percent min=2 and max=3 -> cutoff lower 2% values and higher 3% values;
      e.x. value min=10 and max=60 -> cutoff bellow 10 and above 60, image values will be 10-60)
     """
-    if min is not None and max is not None:
-        if min == max and mode == "value":
+    if cutoff_min is not None and cutoff_max is not None:
+        if cutoff_min == cutoff_max and mode == "value":
             raise Exception("rvt.blend_func.cut_off_normalize: If normalization == value, min and max cannot be the"
                             " same!")
-        if min > max and mode == "value":
+        if cutoff_min > cutoff_max and mode == "value":
             raise Exception("rvt.blend_func.cut_off_normalize: If normalization == value, max can't be smaller"
                             " than min!")
 
     cut_off_arr = image
-    if min is None and mode.lower() == "value":
-        min = np.amin(image)
-    if max is None and mode.lower() == "value":
-        max = np.amax(image)
-    if min is None and (mode.lower() == "perc" or mode.lower() == "percent"):
-        min = 0
-    if max is None and (mode.lower() == "perc" or mode.lower() == "percent"):
-        max = 0
+    if cutoff_min is None and mode.lower() == "value":
+        cutoff_min = np.amin(image)
+    if cutoff_max is None and mode.lower() == "value":
+        cutoff_max = np.amax(image)
+    if cutoff_min is None and (mode.lower() == "perc" or mode.lower() == "percent"):
+        cutoff_min = 0
+    if cutoff_max is None and (mode.lower() == "perc" or mode.lower() == "percent"):
+        cutoff_max = 0
     if bool_norm:
         if mode.lower() == "value":
-            cut_off_arr = normalize_lin(cut_off_arr, min, max)
+            cut_off_arr = normalize_lin(cut_off_arr, cutoff_min, cutoff_max)
         elif mode.lower() == "perc" or mode.lower() == "percent":
-            cut_off_arr = normalize_perc(cut_off_arr, min, max)
+            cut_off_arr = normalize_perc(cut_off_arr, cutoff_min, cutoff_max)
     else:
         if mode.lower() == "value":
-            cut_off_arr[cut_off_arr > max] = max
-            cut_off_arr[cut_off_arr < min] = min
+            cut_off_arr[cut_off_arr > cutoff_max] = cutoff_max
+            cut_off_arr[cut_off_arr < cutoff_min] = cutoff_min
         elif mode.lower() == "perc" or mode.lower() == "percent":
-            min_max_value_dict = lin_cutoff_calc_from_perc(cut_off_arr, min, max)
+            min_max_value_dict = lin_cutoff_calc_from_perc(cut_off_arr, cutoff_min, cutoff_max)
             min_value = min_max_value_dict["min_lin"]
             max_value = min_max_value_dict["max_lin"]
             cut_off_arr[cut_off_arr > max_value] = max_value
             cut_off_arr[cut_off_arr < min_value] = min_value
     return cut_off_arr
```

### Comparing `rvt_py-2.1.0/rvt/default.py` & `rvt_py-2.2.0/rvt/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Žiga Kokalj (ziga.kokalj@zrc-sazu.si)
     Krištof Oštir (kristof.ostir@fgg.uni-lj.si)
     Klemen Zakšek
     Peter Pehani
     Klemen Čotar
     Maja Somrak
     Žiga Maroh
+    Nejc Čož
 
 Copyright:
     2010-2022 Research Centre of the Slovenian Academy of Sciences and Arts
     2016-2022 University of Ljubljana, Faculty of Civil and Geodetic Engineering
 """
 
 import warnings
@@ -276,50 +277,53 @@
         # multi-scale relief model
         self.msrm_compute = 0
         self.msrm_feature_min = 0
         self.msrm_feature_max = 20
         self.msrm_scaling_factor = 2
         # multi-scale topographic position
         self.mstp_compute = 0
-        self.mstp_local_scale = (1, 5, 1)
-        self.mstp_meso_scale = (5, 50, 5)
-        self.mstp_broad_scale = (50, 500, 50)
+        self.mstp_local_scale = (3, 21, 2)
+        self.mstp_meso_scale = (23, 203, 18)
+        self.mstp_broad_scale = (223, 2023, 180)
         self.mstp_lightness = 1.2
         # save float
         self.slp_save_float = 1
         self.hs_save_float = 1
         self.mhs_save_float = 1
         self.slrm_save_float = 1
         self.svf_save_float = 1
         self.neg_opns_save_float = 1
         self.sim_save_float = 1
         self.ld_save_float = 1
         self.msrm_save_float = 1
+        self.mstp_save_float = 1
         # save 8bit
         self.slp_save_8bit = 0
         self.hs_save_8bit = 0
         self.mhs_save_8bit = 0
         self.slrm_save_8bit = 0
         self.svf_save_8bit = 0
         self.neg_opns_save_8bit = 0
         self.sim_save_8bit = 0
         self.ld_save_8bit = 0
         self.msrm_save_8bit = 0
+        self.mstp_save_8bit = 0
         # 8-bit bytescale parameters
         self.slp_bytscl = ("value", 0.00, 51.00)
         self.hs_bytscl = ("value", 0.00, 1.00)
         self.mhs_bytscl = ("value", 0.00, 1.00)
         self.slrm_bytscl = ("value", -2.00, 2.00)
         self.svf_bytscl = ("value", 0.6375, 1.00)
         self.asvf_bytscl = ("value", 0.70, 0.90)
         self.pos_opns_bytscl = ("value", 60.00, 95.00)
         self.neg_opns_bytscl = ("value", 60.00, 95.00)
         self.sim_bytscl = ("percent", 0.25, 0.00)
         self.ld_bytscl = ("value", 0.50, 1.80)
         self.msrm_bytscl = ("value", -2.50, 2.50)
+        self.mstp_bytscl = ("value", 0.00, 1.00)
         # tile
         self.tile_size_limit = 10000 * 10000  # if arr size > tile_size limit, it uses tile module
         self.tile_size = (4000, 4000)  # size of single tile when using tile module (x_size, y_size)
 
     def save_default_to_file(self, file_path=None):
         """Saves default attributes into .json file."""
         data = {"default_settings": {
@@ -545,15 +549,23 @@
                                                    " All have to be integers!"},
                 "mstp_broad_scale": {"min": self.mstp_broad_scale[0], "max": self.mstp_broad_scale[1],
                                      "step": self.mstp_broad_scale[2],
                                      "description": "Broad scale minimum radius, maximum radius and step in pixels to"
                                                     " calculate maximum mean deviation from elevation."
                                                     " All have to be integers!"},
                 "mstp_lightness": {"value": self.mstp_lightness,
-                                   "description": "Lightness factor to adjust MSTP visibility."}
+                                   "description": "Lightness factor to adjust MSTP visibility."},
+                "mstp_save_float": {"value": self.mstp_save_float,
+                                  "description": "If 1 it saves float raster, if 0 it doesn't."},
+                "mstp_save_8bit": {"value": self.mstp_save_8bit,
+                                 "description": "If 1 it saves 8bit raster, if 0 it doesn't."},
+                "mstp_bytscl": {"mode": self.mstp_bytscl[0], "min": self.mstp_bytscl[1], "max": self.mstp_bytscl[2],
+                              "description": "Linear stretch and byte scale (0-255) for 8bit raster. "
+                                             "Mode can be 'value' or 'percent' (cut-off units). "
+                                             "Values min and max define stretch borders (in mode units)."}
             }
 
         }}
         if file_path is None:
             file_path = r"settings\default_settings.json"
             if os.path.isfile(file_path):
                 pass
@@ -768,14 +780,19 @@
             self.mstp_meso_scale = (int(default_data["Multi-scale topographic position"]["mstp_meso_scale"]["min"]),
                                     int(default_data["Multi-scale topographic position"]["mstp_meso_scale"]["max"]),
                                     int(default_data["Multi-scale topographic position"]["mstp_meso_scale"]["step"]))
             self.mstp_broad_scale = (int(default_data["Multi-scale topographic position"]["mstp_broad_scale"]["min"]),
                                      int(default_data["Multi-scale topographic position"]["mstp_broad_scale"]["max"]),
                                      int(default_data["Multi-scale topographic position"]["mstp_broad_scale"]["step"]))
             self.mstp_lightness = float(default_data["Multi-scale topographic position"]["mstp_lightness"]["value"])
+            self.mstp_save_float = int(default_data["Multi-scale topographic position"]["mstp_save_float"]["value"])
+            self.mstp_save_8bit = int(default_data["Multi-scale topographic position"]["mstp_save_8bit"]["value"])
+            self.mstp_bytscl = (str(default_data["Multi-scale topographic position"]["mstp_bytscl"]["mode"]),
+                              float(default_data["Multi-scale topographic position"]["mstp_bytscl"]["min"]),
+                              float(default_data["Multi-scale topographic position"]["mstp_bytscl"]["max"]))
             dat.close()
 
     def get_shadow_file_name(self, dem_path):
         """Returns shadow name, with added hillshade parameters (hs_sun_azi == shadow azimuth,
         hs_sun_el == shadow_elevation)."""
         dem_name = os.path.basename(dem_path).split(".")[0]  # base name without extension
         return "{}_shadow_A{}_H{}.tif".format(dem_name, self.hs_sun_azi, self.hs_sun_el)
@@ -973,23 +990,34 @@
                                                      self.msrm_scaling_factor)
 
     def get_msrm_path(self, dem_path, bit8=False):
         """Returns path to Multi-scale relief model. Generates msrm name (uses default attributes and dem name from
         dem_path) and adds dem directory (dem_path) to it. If bit8 it returns 8bit file path."""
         return os.path.normpath(os.path.join(os.path.dirname(dem_path), self.get_msrm_file_name(dem_path, bit8)))
 
-    def get_mstp_file_name(self, dem_path):
+    def get_mstp_file_name(self, dem_path, bit8=False):
         """Returns Multi-scale topographic position name, dem name (from dem_path) with added mstp parameters.
         If bit8 it returns 8bit file name."""
         dem_name = os.path.basename(dem_path).split(".")[0]  # base name without extension
-        return "{}_MSTP_{}_{}_{}_L{}.tif".format(dem_name, self.mstp_local_scale[1], self.mstp_meso_scale[1],
-                                                 self.mstp_broad_scale[1], self.mstp_lightness)
 
-    def get_mstp_path(self, dem_path):
-        return os.path.normpath(os.path.join(os.path.dirname(dem_path), self.get_mstp_file_name(dem_path)))
+        mstp_file_name = "{}_MSTP_{}_{}_{}_L{}.tif".format(
+            dem_name,
+            self.mstp_local_scale[1],
+            self.mstp_meso_scale[1],
+            self.mstp_broad_scale[1],
+            self.mstp_lightness
+        )
+
+        if bit8:
+            mstp_file_name = mstp_file_name.replace(".tif", "_8bit.tif")
+
+        return mstp_file_name
+
+    def get_mstp_path(self, dem_path, bit8=False):
+        return os.path.normpath(os.path.join(os.path.dirname(dem_path), self.get_mstp_file_name(dem_path, bit8)))
 
     def get_visualization_file_name(self,
                                     rvt_visualization: RVTVisualization,
                                     dem_path: Path,
                                     path_8bit: bool
                                     ) -> str:
         """"Return visualization path."""
@@ -1014,15 +1042,15 @@
         elif rvt_visualization == rvt.default.RVTVisualization.SKY_ILLUMINATION:
             return self.get_sky_illumination_file_name(dem_path=dem_path, bit8=path_8bit)
         elif rvt_visualization == rvt.default.RVTVisualization.LOCAL_DOMINANCE:
             return self.get_local_dominance_file_name(dem_path=dem_path, bit8=path_8bit)
         elif rvt_visualization == rvt.default.RVTVisualization.MULTI_SCALE_RELIEF_MODEL:
             return self.get_msrm_file_name(dem_path=dem_path, bit8=path_8bit)
         elif rvt_visualization == rvt.default.RVTVisualization.MULTI_SCALE_TOPOGRAPHIC_POSITION:
-            return self.get_mstp_file_name(dem_path=dem_path)
+            return self.get_mstp_file_name(dem_path=dem_path, bit8=path_8bit)
 
     def get_visualization_path(
             self,
             rvt_visualization: RVTVisualization,
             dem_path: Path,
             output_dir_path: Path,
             path_8bit: bool
@@ -1049,15 +1077,15 @@
         elif rvt_visualization == rvt.default.RVTVisualization.SKY_ILLUMINATION:
             return output_dir_path / Path(self.get_sky_illumination_file_name(dem_path=dem_path, bit8=path_8bit))
         elif rvt_visualization == rvt.default.RVTVisualization.LOCAL_DOMINANCE:
             return output_dir_path / Path(self.get_local_dominance_file_name(dem_path=dem_path, bit8=path_8bit))
         elif rvt_visualization == rvt.default.RVTVisualization.MULTI_SCALE_RELIEF_MODEL:
             return output_dir_path / Path(self.get_msrm_file_name(dem_path=dem_path, bit8=path_8bit))
         elif rvt_visualization == rvt.default.RVTVisualization.MULTI_SCALE_TOPOGRAPHIC_POSITION:
-            return output_dir_path / Path(self.get_mstp_file_name(dem_path=dem_path))
+            return output_dir_path / Path(self.get_mstp_file_name(dem_path=dem_path, bit8=path_8bit))
 
     def float_to_8bit(
             self,
             float_arr: np.array,
             visualization: RVTVisualization,
             x_res: float = None,
             y_res: float = None,
@@ -1158,15 +1186,24 @@
             return rvt.vis.byte_scale(data=norm_arr, no_data=np.nan, c_min=0, c_max=1)
         elif visualization == RVTVisualization.MULTI_SCALE_RELIEF_MODEL:
             norm_arr = rvt.blend_func.normalize_image(visualization="msrm", image=float_arr,
                                                       min_norm=self.msrm_bytscl[1], max_norm=self.msrm_bytscl[2],
                                                       normalization=self.msrm_bytscl[0])
             return rvt.vis.byte_scale(data=norm_arr, no_data=np.nan, c_min=0, c_max=1)
         elif visualization == RVTVisualization.MULTI_SCALE_TOPOGRAPHIC_POSITION:
-            return float_arr
+            # This might not be necessary, as all mstp data should already be between 0 and 1
+            norm_arr = rvt.blend_func.normalize_image(
+                visualization="mstp",
+                image=float_arr,
+                min_norm=self.mstp_bytscl[1],
+                max_norm=self.mstp_bytscl[2],
+                normalization=self.mstp_bytscl[0]
+            )
+
+            return rvt.vis.byte_scale(data=norm_arr, no_data=np.nan, c_min=0, c_max=1)
         else:
             raise Exception("rvt.default.DefaultValues.float_to_8bit: Wrong visualization (visualization) parameter!")
 
     def get_slope(self, dem_arr, resolution_x, resolution_y, no_data=None):
         slope_arr = rvt.vis.slope_aspect(dem=dem_arr, resolution_x=resolution_x, resolution_y=resolution_y,
                                          ve_factor=self.ve_factor, output_units=self.slp_output_units,
                                          no_data=no_data)["slope"]
@@ -2021,49 +2058,98 @@
             return 1
 
     def get_mstp(self, dem_arr, no_data=None):
         mstp_arr = rvt.vis.mstp(dem=dem_arr, local_scale=self.mstp_local_scale, meso_scale=self.mstp_meso_scale,
                                 broad_scale=self.mstp_broad_scale, lightness=self.mstp_lightness, no_data=no_data)
         return mstp_arr
 
-    def save_mstp(self, dem_path, custom_dir=None):
+    def save_mstp(self, dem_path, custom_dir=None, save_float=None, save_8bit=None):
         """Calculates and saves Multi-scale topographic position from dem (dem_path) with default parameters.
         If custom_dir is None it saves in dem directory else in custom_dir. If path to file already exists we can
         overwrite file (overwrite=1) or not (overwrite=0)."""
+
+        # if save_float is None it takes boolean from default (self)
+        if save_float is None:
+            save_float = self.mstp_save_float
+        # if save_8bit is None it takes boolean from default (self)
+        if save_8bit is None:
+            save_8bit = self.mstp_save_8bit
+
+        if not save_float and not save_8bit:
+            raise Exception("rvt.default.DefaultValues.save_mstp: Both save_float and save_8bit are False,"
+                            " at least one of them has to be True!")
+
         if not os.path.isfile(dem_path):
-            raise Exception("rvt.default.DefaultValues.save_msrm: dem_path doesn't exist!")
+            raise Exception("rvt.default.DefaultValues.save_mstp: dem_path doesn't exist!")
+
         if custom_dir is None:
             mstp_path = self.get_mstp_path(dem_path)
+            mstp_8bit_path = self.get_mstp_path(dem_path, bit8=True)
         else:
             mstp_path = os.path.join(custom_dir, self.get_mstp_file_name(dem_path))
+            mstp_8bit_path = os.path.join(custom_dir, self.get_mstp_file_name(dem_path, bit8=True))
 
-        if os.path.isfile(mstp_path) and not self.overwrite:
-            return 0
+        # if file already exists and overwrite=0
+        if save_float and save_8bit:
+            if os.path.isfile(mstp_8bit_path) and os.path.isfile(mstp_path) and not self.overwrite:
+                return 0
+        elif save_float and not save_8bit:
+            if os.path.isfile(mstp_path) and not self.overwrite:
+                return 0
+        elif not save_float and not save_8bit:
+            if os.path.isfile(mstp_8bit_path) and not self.overwrite:
+                return 0
 
         dem_size = get_raster_size(raster_path=dem_path)
         if dem_size[0] * dem_size[1] > self.tile_size_limit:  # tile by tile calculation
             if custom_dir is None:
                 custom_dir = Path(dem_path).parent
             rvt.tile.save_rvt_visualization_tile_by_tile(
                 rvt_visualization=RVTVisualization.MULTI_SCALE_TOPOGRAPHIC_POSITION,
                 rvt_default=self,
                 dem_path=Path(dem_path),
                 output_dir_path=Path(custom_dir),
-                save_float=False,
-                save_8bit=True
+                save_float=save_float,
+                save_8bit=save_8bit
             )
             return 1
         else:  # singleprocess
             dict_arr_res = get_raster_arr(raster_path=dem_path)
             dem_arr = dict_arr_res["array"]
             no_data = dict_arr_res["no_data"]
 
-            mstp_arr = self.get_mstp(dem_arr=dem_arr, no_data=no_data).astype('float32')
-            save_raster(src_raster_path=dem_path, out_raster_path=mstp_path, out_raster_arr=mstp_arr,
-                        e_type=1)
+            mstp_arr = self.get_mstp(dem_arr=dem_arr, no_data=no_data)
+
+            if save_float:
+                if os.path.isfile(mstp_path) and not self.overwrite:  # file exists and overwrite=0
+                    pass
+                else:
+                    save_raster(
+                        src_raster_path=dem_path,
+                        out_raster_path=mstp_path,
+                        out_raster_arr=mstp_arr,
+                        no_data=np.nan,
+                        e_type=6
+                    )
+            if save_8bit:
+                if os.path.isfile(mstp_8bit_path) and not self.overwrite:  # file exists and overwrite=0
+                    pass
+                else:
+                    mstp_8bit_arr = self.float_to_8bit(
+                        float_arr=mstp_arr,
+                        visualization=RVTVisualization.MULTI_SCALE_TOPOGRAPHIC_POSITION
+                    )
+                    save_raster(
+                        src_raster_path=dem_path,
+                        out_raster_path=mstp_8bit_path,
+                        out_raster_arr=mstp_8bit_arr,
+                        no_data=np.nan,
+                        e_type=1
+                    )
+
             return 1
 
     def save_visualizations(self, dem_path, custom_dir=None):
         """Save all visualizations where self.'visualization'_compute = True also saves float where self.'visualization'
         _save_float = True and 8bit where self.'visualization'_save_8bit = True. In the end method creates log file."""
         start_time = time.time()
         if self.slp_compute:
```

### Comparing `rvt_py-2.1.0/rvt/tile.py` & `rvt_py-2.2.0/rvt/tile.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Žiga Kokalj (ziga.kokalj@zrc-sazu.si)
     Krištof Oštir (kristof.ostir@fgg.uni-lj.si)
     Klemen Zakšek
     Peter Pehani
     Klemen Čotar
     Maja Somrak
     Žiga Maroh
+    Nejc Čož
 
 Copyright:
     2010-2022 Research Centre of the Slovenian Academy of Sciences and Arts
     2016-2022 University of Ljubljana, Faculty of Civil and Geodetic Engineering
 """
 from pathlib import Path
 from typing import Callable, Dict, Any, Optional, Union, Tuple
```

### Comparing `rvt_py-2.1.0/rvt/vis.py` & `rvt_py-2.2.0/rvt/vis.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,26 @@
     Žiga Kokalj (ziga.kokalj@zrc-sazu.si)
     Krištof Oštir (kristof.ostir@fgg.uni-lj.si)
     Klemen Zakšek
     Peter Pehani
     Klemen Čotar
     Maja Somrak
     Žiga Maroh
+    Nejc Čož
 
 Copyright:
     2010-2020 Research Centre of the Slovenian Academy of Sciences and Arts
     2016-2020 University of Ljubljana, Faculty of Civil and Geodetic Engineering
 """
 
 # python libraries
 import numpy as np
-import scipy.interpolate
-import scipy.ndimage.filters
-import scipy.ndimage.morphology
-import scipy.spatial
-import warnings
+from scipy.interpolate import griddata, RectBivariateSpline
+from scipy.ndimage.morphology import distance_transform_edt
+from scipy.spatial import cKDTree
 
 
 def byte_scale(data,
                c_min=None,
                c_max=None,
                high=255,
                low=0,
@@ -120,16 +119,20 @@
                  resolution_y=1,
                  output_units="radian",
                  ve_factor=1,
                  no_data=None
                  ):
     """
     Procedure can return terrain slope and aspect in radian units (default) or in alternative units (if specified).
-    Slope is defined as 0 for Hz plane and pi/2 for vertical plane.
-    Aspect iz defined as geographic azimuth: clockwise increasing, 0 or 2pi for the North direction.
+    Available alternative units are 'degree' and 'percent'.
+    Slope is defined as 0 for horizontal plane and pi/2 for vertical plane.
+    Aspect is defined as geographic azimuth: clockwise increasing, 0 or 2pi for the North direction.
+         0
+     270    90
+        180
     Currently applied finite difference method.
 
     Parameters
     ----------
     dem : numpy.ndarray
         Input digital elevation model as 2D numpy array.
     resolution_x : int
@@ -137,15 +140,16 @@
     resolution_y : int
         DEM resolution in Y direction.
     output_units : str
         Output units, you can choose between: percent, degree, radian. Default value is radian.
     ve_factor : int or float
         Vertical exaggeration factor.
     no_data : int or float
-        Value that represents no_data, all pixels with this value are changed to np.nan .
+        Value that represents no_data, all pixels with this value are changed to np.nan. Only has to be specified if
+        a numerical value is used for nodata (e.g. -9999).
 
     Returns
     -------
     dict_out: dict
         Returns {"slope": slope_out, "aspect": aspect_out};
         slope_out, slope gradient : 2D numpy array (numpy.ndarray) of slope;
         aspect_out, aspect : 2D numpy array (numpy.ndarray) of aspect.
@@ -153,56 +157,81 @@
     if dem.ndim != 2:
         raise Exception("rvt.visualization.slope_aspect: dem has to be 2D np.array!")
     if not (10000 >= ve_factor >= -10000):
         raise Exception("rvt.visualization.slope_aspect: ve_factor must be between -10000 and 10000!")
     if resolution_x < 0 or resolution_y < 0:
         raise Exception("rvt.visualization.slope_aspect: resolution must be a positive number!")
 
-    # change no_data to np.nan
+    # Make sure array has the correct dtype!
+    dem = dem.astype(np.float32)
+
+    # Change no_data to np.nan
     if no_data is not None:
         dem[dem == no_data] = np.nan
 
-    dem = dem.astype(np.float32)
+    # Save NaN mask
+    nan_dem = np.isnan(dem)
+
+    # Add 1 pixel edge padding
+    dem = np.pad(array=dem, pad_width=1, mode="edge")
+
+    # Vertical exaggeration
     dem = dem * ve_factor
 
-    # derivatives in X and Y direction
-    dzdx = ((np.roll(dem, 1, axis=1) - np.roll(dem, -1, axis=1)) / 2) / resolution_x
-    dzdy = ((np.roll(dem, -1, axis=0) - np.roll(dem, 1, axis=0)) / 2) / resolution_y
+    # Derivatives in X and Y direction
+    dzdx = ((roll_fill_nans(dem, 1, axis=1) - roll_fill_nans(dem, -1, axis=1)) / 2) / resolution_x
+    dzdy = ((roll_fill_nans(dem, -1, axis=0) - roll_fill_nans(dem, 1, axis=0)) / 2) / resolution_y
     tan_slope = np.sqrt(dzdx ** 2 + dzdy ** 2)
 
     # Compute slope
     if output_units == "percent":
         slope_out = tan_slope * 100
     elif output_units == "degree":
         slope_out = np.rad2deg(np.arctan(tan_slope))
     elif output_units == "radian":
         slope_out = np.arctan(tan_slope)
     else:
         raise Exception("rvt.visualization.calculate_slope: Wrong function input 'output_units'!")
 
-    # compute Aspect
+    # Compute Aspect
     # aspect identifies the down slope direction of the maximum rate of change in value from each cell to its neighbors:
     #     0
     # 270    90
     #    180
-    dzdy[dzdy == 0] = 10e-9  # important for numeric stability - where dzdy is zero, make tangens to really high value
-
+    dzdy[dzdy == 0] = 10e-9  # important for numeric stability - where dzdy is zero, make tangent to really high value
     aspect_out = np.arctan2(dzdx, dzdy)  # atan2 took care of the quadrants
     if output_units == "degree":
         aspect_out = np.rad2deg(aspect_out)
 
-    # edges to np.nan
-    slope_out[:, 0] = np.nan
-    slope_out[0, :] = np.nan
-    slope_out[:, -1] = np.nan
-    slope_out[-1, :] = np.nan
+    # Remove padding
+    aspect_out = aspect_out[1:-1, 1:-1]
+    slope_out = slope_out[1:-1, 1:-1]
+
+    # Apply NaN mask
+    slope_out[nan_dem] = np.nan
+    aspect_out[nan_dem] = np.nan
 
     return {"slope": slope_out, "aspect": aspect_out}
 
 
+def roll_fill_nans(dem, shift, axis):
+    """
+    Uses numpy.roll() function to roll array, then checks element-wise if new array has NaN value, but there was a
+    numerical value in the source array, then use the original value instead of NaN. It is equivalent to edge padding.
+
+    https://numpy.org/doc/stable/reference/generated/numpy.roll.html#numpy.roll
+    """
+    out = np.roll(dem, shift, axis=axis)
+
+    # Fill NaNs with values from dem
+    out[np.isnan(out) != np.isnan(dem)] = dem[np.isnan(out) != np.isnan(dem)]
+
+    return out
+
+
 def hillshade(dem,
               resolution_x,
               resolution_y,
               sun_azimuth=315,
               sun_elevation=35,
               slope=None,
               aspect=None,
@@ -248,14 +277,16 @@
         raise Exception("rvt.visualization.hillshade: resolution must be a positive number!")
 
     # change no_data to np.nan
     if no_data is not None:
         dem[dem == no_data] = np.nan
 
     dem = dem.astype(np.float32)
+    # add 1 pixel edge padding
+    dem = np.pad(array=dem, pad_width=1, mode="edge")
     dem = dem * ve_factor
 
     # Convert solar position (degrees) to radians
     sun_azimuth_rad = np.deg2rad(sun_azimuth)
     sun_elevation_rad = np.deg2rad(sun_elevation)
 
     # Convert to solar zenith angle
@@ -271,19 +302,16 @@
 
     # Compute solar incidence angle, hillshading
     hillshade_out = np.cos(sun_zenith_rad) * np.cos(slope) + np.sin(sun_zenith_rad) * np.sin(slope) * np.cos(
         aspect - sun_azimuth_rad)
 
     hillshade_out[hillshade_out < 0] = 0  # set all negative to 0
 
-    # edges to -1
-    hillshade_out[:, 0] = np.nan
-    hillshade_out[0, :] = np.nan
-    hillshade_out[:, -1] = np.nan
-    hillshade_out[-1, :] = np.nan
+    # remove padding
+    hillshade_out = hillshade_out[1:-1, 1:-1]
 
     return hillshade_out
 
 
 def multi_hillshade(dem,
                     resolution_x,
                     resolution_y,
@@ -344,15 +372,15 @@
     # calculates slope and aspect if they are not added
     if slope is None or aspect is None:  # slope and aspect are the same, so we have to calculate it once
         dict_slp_asp = slope_aspect(dem=dem, resolution_x=resolution_x, resolution_y=resolution_y,
                                     output_units="radian")
         slope = dict_slp_asp["slope"]
         aspect = dict_slp_asp["aspect"]
 
-    hillshades_arr_list = []  # list of all hillshades in diffrent directions
+    hillshades_arr_list = []  # list of all hillshades in different directions
     for i_direction in range(nr_directions):
         sun_azimuth = (360 / nr_directions) * i_direction
         hillshading = hillshade(dem=dem, resolution_x=resolution_x, resolution_y=resolution_y,
                                 sun_elevation=sun_elevation, sun_azimuth=sun_azimuth, slope=slope, aspect=aspect)
         hillshades_arr_list.append(hillshading)
     multi_hillshade_out = np.asarray(hillshades_arr_list)
 
@@ -377,26 +405,26 @@
     idx_nan_dem_pad = np.isnan(dem_pad)
     # change nan to 0
     dem_pad[idx_nan_dem_pad] = 0
 
     # kernel nr pixel integral image
     dem_i_nr_pixels = np.ones(dem_pad.shape)
     dem_i_nr_pixels[idx_nan_dem_pad] = 0
-    dem_i_nr_pixels = integral_image(dem_i_nr_pixels, np.int)
+    dem_i_nr_pixels = integral_image(dem_i_nr_pixels, np.int64)
 
     dem_i1 = integral_image(dem_pad)
 
     kernel_nr_pix_arr = (np.roll(dem_i_nr_pixels, (radius_cell, radius_cell), axis=(0, 1)) +
                          np.roll(dem_i_nr_pixels, (-radius_cell - 1, -radius_cell - 1), axis=(0, 1)) -
                          np.roll(dem_i_nr_pixels, (-radius_cell - 1, radius_cell), axis=(0, 1)) -
                          np.roll(dem_i_nr_pixels, (radius_cell, -radius_cell - 1), axis=(0, 1)))
-    mean_out = np.roll(dem_i1, (radius_cell, radius_cell), axis=(0, 1)) + \
-               np.roll(dem_i1, (-radius_cell - 1, -radius_cell - 1), axis=(0, 1)) - \
-               np.roll(dem_i1, (-radius_cell - 1, radius_cell), axis=(0, 1)) - \
-               np.roll(dem_i1, (radius_cell, -radius_cell - 1), axis=(0, 1))
+    mean_out = (np.roll(dem_i1, (radius_cell, radius_cell), axis=(0, 1)) +
+                np.roll(dem_i1, (-radius_cell - 1, -radius_cell - 1), axis=(0, 1)) -
+                np.roll(dem_i1, (-radius_cell - 1, radius_cell), axis=(0, 1)) -
+                np.roll(dem_i1, (radius_cell, -radius_cell - 1), axis=(0, 1)))
     mean_out = mean_out / kernel_nr_pix_arr
     mean_out = mean_out.astype(np.float32)
     mean_out = mean_out[radius_cell:-(radius_cell + 1), radius_cell:-(radius_cell + 1)]  # remove padding
     # nan back to nan
     mean_out[idx_nan_dem] = np.nan
 
     return mean_out
@@ -480,27 +508,27 @@
     # and Y (lines) direction
     angles = (2 * np.pi / num_directions) * np.arange(num_directions)
     x = np.cos(angles)
     y = np.sin(angles)
     angles = np.round(np.degrees(angles), decimals=1)
 
     # Generate a range of radius values in pixels.
-    # Make it finer for the selcted scaling.
+    # Make it finer for the selected scaling.
     # By adding the last constant we make sure that we do not start with
     # point (0,0).
     scale = 3.
     radii = np.arange((radius_pixels - min_radius) * scale + 1) / scale + min_radius
 
-    # For each direction compute all possible horizont point position
+    # For each direction compute all possible horizon point position
     # and round them to integers
     for i in range(num_directions):
         x_int = np.round(x[i] * radii, decimals=0)
         y_int = np.round(y[i] * radii, decimals=0)
         # consider only the minimal number of points
-        # use the trick with set and complex nuber as the input
+        # use the trick with set and complex number as the input
         coord_complex = set(x_int + 1j * y_int)
         # to sort proportional with increasing radius, 
         # set has to be converted to numpy array
         shift_pairs = np.array([(k.real, k.imag) for k in coord_complex]).astype(int)
         distance = np.sqrt(np.sum(shift_pairs ** 2, axis=1))
         sort_index = np.argsort(distance)
         # write for each direction shifts and corresponding distances
@@ -517,19 +545,26 @@
                             radius_min=1,
                             num_directions=16,
                             compute_svf=True,
                             compute_opns=False,
                             compute_asvf=False,
                             a_main_direction=315.,
                             a_poly_level=4,
-                            a_min_weight=0.4,
-                            no_data=None
+                            a_min_weight=0.4
                             ):
     """
-    Calculates horizon based visualizations: Sky-view factor, Anisotopic SVF and Openess.
+    Calculates horizon based visualizations: Sky-view factor, Anisotropic SVF and Openness.
+
+    SVF processing is using search radius, that looks at values beyond the edge of an array. Consider using a buffered
+    array as an input, with the buffer size equal to the radius_max.
+    To prevent erosion of the edge, function applies mirrored padding in all four directions, however, this means that
+    edge values are "averaged over half of the hemisphere". Similarly, the edges of the dataset (i.e. areas with NaN
+    values), will be considered as fully open (SFV angle 0, Openness angle -90).
+
+    Input array should use np.nan as nodata value.
 
     Parameters
     ----------
     height_arr : numpy.ndarray
         Elevation (DEM) as 2D numpy array.
     radius_max : int
         Maximal search radius in pixels/cells (not in meters).
@@ -543,92 +578,96 @@
         If true it computes and outputs asvf.
     compute_opns : bool
         If true it computes and outputs opns.
     a_main_direction : int or float
         Main direction of anisotropy.
     a_poly_level : int
         Level of polynomial that determines the anisotropy.
-    a_min_weight : int
+    a_min_weight : float
         Weight to consider anisotropy:
                  0 - low anisotropy, 
                  1 - high  anisotropy (no illumination from the direction opposite the main direction)
-    no_data : int or float
-        Value that represents no_data, all pixels with this value are changed to np.nan .
 
     Returns
     -------
     dict_out : dictionary
         Return {"svf": svf_out, "asvf": asvf_out, "opns": opns_out};
         svf_out, skyview factor : 2D numpy array (numpy.ndarray) of skyview factor;
         asvf_out, anisotropic skyview factor : 2D numpy array (numpy.ndarray) of anisotropic skyview factor;
         opns_out, openness : 2D numpy array (numpy.ndarray) openness (elevation angle of horizon).
     """
-    # change no_data to np.nan
-    if no_data is not None:
-        height_arr[height_arr == no_data] = np.nan
 
-    # pad the array for the radius_max on all 4 sides
-    height = np.pad(height_arr, radius_max, mode='symmetric')
+    # Pad the array for the radius_max on all 4 sides
+    height = np.pad(height_arr, radius_max, mode='reflect')
 
-    # compute the vector of movement and corresponding distances
+    # Compute the vector of movement and corresponding distances
     move = horizon_shift_vector(num_directions=num_directions, radius_pixels=radius_max, min_radius=radius_min)
 
-    # init the output for usual SVF
+    # Initiate the output for SVF
     if compute_svf:
-        svf_out = np.zeros(height.shape, dtype=np.float32)
+        svf_out = height * 0  # Multiply with 0 instead of using np.zeros to preserve nodata
     else:
         svf_out = None
-    # init the output for azimuth dependent SVF
+
+    # Initiate the output for azimuth dependent SVF
     if compute_asvf:
-        asvf_out = np.zeros(height.shape, dtype=np.float32)
+        asvf_out = height * 0  # Multiply with 0 instead of using np.zeros to preserve nodata
         w_m = a_min_weight
         w_a = np.deg2rad(a_main_direction)
         weight = np.arange(num_directions) * (2 * np.pi / num_directions)
         weight = (1 - w_m) * (np.cos((weight - w_a) / 2)) ** a_poly_level + w_m
     else:
         asvf_out = None
-    # init the output for Openess
+        weight = None
+
+    # Initiate the output for Openness
     if compute_opns:
-        opns_out = np.zeros(height.shape, dtype=np.float32)
+        opns_out = height * 0  # Multiply with 0 instead of using np.zeros to preserve nodata
     else:
         opns_out = None
 
-        # search for horizon in each direction...
+    # Search for horizon in each direction...
     for i_dir, direction in enumerate(move):
-        # reset maximum at each iteration (direction)
+        # Reset maximum at each iteration (i.e. at the start of new direction),
+        # smallest possible elevation angle is -1000 rad (i.e. -90 deg)
         max_slope = np.zeros(height.shape, dtype=np.float32) - 1000
 
-        # ... and to the search radius
+        # ... and for each search radius
         for i_rad, radius in enumerate(move[direction]["distance"]):
-            # get shift index from move dictionary
+            # Get shift index from move dictionary
             shift_indx = move[direction]["shift"][i_rad]
-            # estimate the slope
+            # Estimate the slope
             _ = (np.roll(height, shift_indx, axis=(0, 1)) - height) / radius
-            # compare to the previus max slope and keep the larges
-            max_slope = np.maximum(max_slope, _)
+            # Compare to the previous max slope and keep the largest values (element wise). Use np.fmax to prevent NaN
+            # values contaminating the edge of the image (if one of the elements is NaN, pick non-NaN element)
+            max_slope = np.fmax(max_slope, _)
 
-        # convert to angle in radians and compute directional output
-        _ = np.arctan(max_slope)
+        # Convert to angle in radians and compute directional output
+        max_slope = np.arctan(max_slope)
+
+        # Sum max angle for all directions
         if compute_svf:
-            svf_out = svf_out + (1 - np.sin(np.maximum(_, 0)))
+            # For SVF minimum possible angle is 0 (hemisphere), use np.fmax() to change NaNs to 0
+            svf_out = svf_out + (1 - np.sin(np.fmax(max_slope, 0)))
         if compute_asvf:
-            asvf_out = asvf_out + (1 - np.sin(np.maximum(_, 0))) * weight[i_dir]
+            # For SVF minimum possible angle is 0 (hemisphere), use np.fmax() to change NaNs to 0
+            asvf_out = asvf_out + (1 - np.sin(np.fmax(max_slope, 0))) * weight[i_dir]
         if compute_opns:
-            opns_out = opns_out + _
+            # For Openness taking the entire sphere
+            opns_out = opns_out + max_slope
 
-    # cut to original extent and 
-    # average the directional output over all directions
+    # Cut to original extent and average the directional output over all directions
     if compute_svf:
         svf_out = svf_out[radius_max:-radius_max, radius_max:-radius_max] / num_directions
     if compute_asvf:
         asvf_out = asvf_out[radius_max:-radius_max, radius_max:-radius_max] / np.sum(weight)
     if compute_opns:
         opns_out = np.rad2deg(0.5 * np.pi - (opns_out[radius_max:-radius_max, radius_max:-radius_max] / num_directions))
 
-    # return results within dict
+    # Return results within dict
     dict_svf_asvf_opns = {"svf": svf_out, "asvf": asvf_out, "opns": opns_out}
     dict_svf_asvf_opns = {k: v for k, v in dict_svf_asvf_opns.items() if v is not None}  # filter out none
 
     return dict_svf_asvf_opns
 
 
 def sky_view_factor(dem,
@@ -664,84 +703,92 @@
     svf_noise : int
         The level of noise remove (0-don't remove, 1-low, 2-med, 3-high).
     compute_asvf : bool
         Compute anisotropic SVF (True) or not (False).
     asvf_level : int
         Level of anisotropy, 1-low, 2-high.
     asvf_dir : int or float
-        Dirction of anisotropy.
+        Direction of anisotropy.
     ve_factor : int or float
         Vertical exaggeration factor.
     no_data : int or float
-        Value that represents no_data, all pixels with this value are changed to np.nan .
-    
-    Constants
-    ---------
-        sc_asvf_min : level of polynomial that determines the anisotropy, selected with in_asvf_level
-        sc_asvf_pol : level of polynomial that determines the anisotropy, selected with in_asvf_level
-        sc_svf_r_min : the portion (percent) of the maximal search radius to ignore in horizon estimation;
-        for each noise level, selected with in_svf_noise
+        Value that represents no_data, all pixels with this value are changed to np.nan. Use this parameter when nodata
+        is not np.nan.
 
     Returns
     -------
     dict_out : dictionary
         Return {"svf": svf_out, "asvf": asvf_out, "opns": opns_out};
         svf_out, skyview factor : 2D numpy array (numpy.ndarray) of skyview factor;
         asvf_out, anisotropic skyview factor : 2D numpy array (numpy.ndarray) of anisotropic skyview factor;
         opns_out, openness : 2D numpy array (numpy.ndarray) openness (elevation angle of horizon).
     """
+
+    # Checks for input parameters
     if dem.ndim != 2:
         raise Exception("rvt.visualization.sky_view_factor: dem has to be 2D np.array!")
     if not (10000 >= ve_factor >= -10000):
         raise Exception("rvt.visualization.sky_view_factor: ve_factor must be between -10000 and 10000!")
     if svf_noise != 0 and svf_noise != 1 and svf_noise != 2 and svf_noise != 3:
-        raise Exception("rvt.visualization.sky_view_factor: svf_noise must be one of the following values (0-don't remove, 1-low,"
-                        " 2-med, 3-high)!")
+        raise Exception("rvt.visualization.sky_view_factor: svf_noise must be one of the following"
+                        "values (0-don't remove, 1-low, 2-med, 3-high)!")
     if asvf_level != 1 and asvf_level != 2:
-        raise Exception("rvt.visualization.sky_view_factor: asvf_leve must be one of the following values (1-low, 2-high)!")
+        raise Exception("rvt.visualization.sky_view_factor: asvf_leve must be one of the following"
+                        "values (1-low, 2-high)!")
     if not compute_svf and not compute_asvf and not compute_opns:
         raise Exception("rvt.visualization.sky_view_factor: All computes are false!")
     if resolution < 0:
         raise Exception("rvt.visualization.sky_view_factor: resolution must be a positive number!")
 
-    # TODO: proper check of input data: DEM 2D nummeric array, resolution, max_radius....
-
+    # Make sure array has the correct dtype!
     dem = dem.astype(np.float32)
-    dem = dem * ve_factor
 
     # CONSTANTS
-    # level of polynomial that determines the anisotropy, selected with in_asvf_level (1 - low, 2 - high)
+    # Level of polynomial that determines the anisotropy, selected with asvf_level (1 - low, 2 - high)
     sc_asvf_pol = [4, 8]
     sc_asvf_min = [0.4, 0.1]
-    # the portion (percent) of the maximal search radius to ignore in horizon estimation; for each noise level,
-    # selected with in_svf_noise (0-3)
+    # The portion (percent) of the maximal search radius to ignore in horizon estimation; for each noise level,
+    # selected with svf_noise (0-3)
     sc_svf_r_min = [0., 10., 20., 40.]
 
-    # pixel size
+    # Before doing anything to the array, make sure all NODATA values are set to np.nan
+    if no_data is not None:
+        dem[dem == no_data] = np.nan
+    # Save NaN mask (processing may change NaNs to arbitrary values)
+    nan_mask = np.isnan(dem)
+
+    # Vertical exaggeration
+    dem = dem * ve_factor
+    # Pixel size (adjust elevation to correctly calculate the vertical elevation angle, calculation thinks 1px == 1m)
     dem = dem / resolution
 
-    # minimal search radious depends on the noise level, it has to be an integer not smaller than 1
+    # Minimal search radius depends on the noise level, it has to be an integer not smaller than 1
     svf_r_min = max(np.round(svf_r_max * sc_svf_r_min[svf_noise] * 0.01, decimals=0), 1)
 
-    # set anisotropy parameters
+    # Set anisotropy parameters
     poly_level = sc_asvf_pol[asvf_level - 1]
     min_weight = sc_asvf_min[asvf_level - 1]
 
-    dict_svf_asvf_opns = sky_view_factor_compute(height_arr=dem,
-                                                 radius_max=svf_r_max,
-                                                 radius_min=svf_r_min,
-                                                 num_directions=svf_n_dir,
-                                                 compute_svf=compute_svf,
-                                                 compute_opns=compute_opns,
-                                                 compute_asvf=compute_asvf,
-                                                 a_main_direction=asvf_dir,
-                                                 a_poly_level=poly_level,
-                                                 a_min_weight=min_weight,
-                                                 no_data=no_data
-                                                 )
+    # Main routine for SVF processing
+    dict_svf_asvf_opns = sky_view_factor_compute(
+        height_arr=dem,
+        radius_max=svf_r_max,
+        radius_min=svf_r_min,
+        num_directions=svf_n_dir,
+        compute_svf=compute_svf,
+        compute_opns=compute_opns,
+        compute_asvf=compute_asvf,
+        a_main_direction=asvf_dir,
+        a_poly_level=poly_level,
+        a_min_weight=min_weight
+    )
+
+    # Apply NaN mask to outputs
+    for item in dict_svf_asvf_opns.values():
+        item[nan_mask] = np.nan
 
     return dict_svf_asvf_opns
 
 
 def local_dominance(dem,
                     min_rad=10,
                     max_rad=20,
@@ -785,14 +832,17 @@
         raise Exception("rvt.visualization.local_dominance: ve_factor must be between -10000 and 10000!")
 
     # change no_data to np.nan
     if no_data is not None:
         dem[dem == no_data] = np.nan
 
     dem = dem.astype(np.float32)
+    # add max_rad pixel edge padding
+    pad_width = max_rad
+    dem = np.pad(array=dem, pad_width=pad_width, mode="edge")
     dem = dem * ve_factor
 
     # create a vector with possible distances
     n_dist = int((max_rad - min_rad) / rad_inc + 1)
     distances = np.arange(n_dist * rad_inc, step=rad_inc) + min_rad
     # create vector with possible angles
     n_ang = int(359 / angular_res + 1)
@@ -801,28 +851,31 @@
     norma = np.sum((observer_height / distances) * (2 * distances + rad_inc)) * n_ang
 
     # image shifts
     n_shifts = distances.size * angles.size
     x_t = (np.outer(np.cos(np.deg2rad(angles)), distances)).reshape(n_shifts)
     y_t = (np.outer(np.sin(np.deg2rad(angles)), distances)).reshape(n_shifts)
     distances = (np.outer(np.ones(n_ang), distances)).reshape(n_shifts)
-    dist_factr = 2 * distances + rad_inc
+    dist_factor = 2 * distances + rad_inc
 
     local_dom_out = dem * 0
     for i_s in range(n_shifts):
         dem_moved = np.roll(dem, int(round(y_t[i_s])), axis=0)
         dem_moved = np.roll(dem_moved, int(round(x_t[i_s])), axis=1)
         idx_lower = np.where((dem + observer_height) > dem_moved)
         if idx_lower[0].size > 0:
             local_dom_out[idx_lower[0], idx_lower[1]] = local_dom_out[idx_lower[0], idx_lower[1]] + \
                                                         (dem[idx_lower[0], idx_lower[1]] + observer_height -
                                                          dem_moved[idx_lower[0], idx_lower[1]]) / \
-                                                        distances[i_s] * dist_factr[i_s]
+                                                        distances[i_s] * dist_factor[i_s]
     local_dom_out = local_dom_out / norma
 
+    # Remove padding
+    local_dom_out = local_dom_out[pad_width:-pad_width, pad_width:-pad_width]
+
     return local_dom_out
 
 
 def horizon_generate_coarse_dem(dem_fine,
                                 pyramid_scale,
                                 conv_from,
                                 conv_to,
@@ -836,15 +889,15 @@
     n_col_fine = in_shape[1]
     n_lin_fine = in_shape[0]
     n_lin_coarse = int(np.floor(n_lin_fine / pyramid_scale)) + 1
     n_col_coarse = int(np.floor(n_col_fine / pyramid_scale)) + 1
     # The corner points must fit in the new grid.
     # This is always the case with the left most column or the upper line.
     # But you have to adjust ne number of columns to the right and number of lines below.
-    # The final number of columns/lines has to fullfil:
+    # The final number of columns/lines has to fulfill:
     #     n_coarse = pyramid_scale * n_fine + 1
     # columns
     mod_col = n_col_fine % pyramid_scale
     pad_col = 0
     if mod_col != 1:
         pad_col = np.abs(1 - mod_col)
     # lines
@@ -861,23 +914,23 @@
     dem_fine = np.pad(dem_fine, ((-conv_from, conv_to), (-conv_from, conv_to)), mode="symmetric")
 
     # Convolution (keep maximum)
     dem_convolve = np.zeros(dem_fine.shape)
     for i in np.arange(pyramid_scale) + conv_from:
         for j in np.arange(pyramid_scale) + conv_from:
             dem_convolve = np.maximum(dem_convolve, np.roll(dem_fine, (i, j), axis=(0, 1)))
-    # Divide by pyramid_scale to account for the chage of resolution
+    # Divide by pyramid_scale to account for the change of resolution
     # (important for the angle computation later on)
     dem_convolve = dem_convolve / pyramid_scale
 
-    # Consider only the selceted convoluted points according to the scale change.
+    # Consider only the selected convoluted points according to the scale change.
     # As we select slice's end point make sure to consider at least 1 point more 
     # to the right / below to really include it (Python way of considering end index).
     dem_coarse = dem_convolve[-conv_from:(n_lin_coarse * pyramid_scale + 1):pyramid_scale,
-                 -conv_from:(n_col_coarse * pyramid_scale + 1):pyramid_scale]
+                              -conv_from:(n_col_coarse * pyramid_scale + 1):pyramid_scale]
 
     # Final padding to enable searching the horizon over the edge:
     # use constant-mode set to the minimal height, so it doesn't 
     # affect the horizon estimation.
     dem_coarse = np.pad(dem_coarse, ((max_radius, max_radius), (max_radius, max_radius)), mode="constant",
                         constant_values=dem_coarse.min())
 
@@ -898,15 +951,15 @@
     #     num_directions = 8
     # then you have original distances in level 0:
     # 1, 2, 3, ... 9, 10
     # In level 1, your resolution is 3-times coarser.
     # The first pixel that takes that this new resolution,
     # has in original distance value 12 (in coarse resolution 4):
     # 12->4, 15->5, 18->6 ... 27->9, 30->10
-    # So you start in the level 1 with tmin_pyramid_radius=4
+    # So you start in the level 1 with min_pyramid_radius=4
     # and you search from 4 to 10 distances (n_pyramid_radius=7)
     min_pyramid_radius = int(np.floor(max_pyramid_radius / pyramid_scale)) + 1
     n_pyramid_radius = max_pyramid_radius - min_pyramid_radius + 1
 
     # get the convolution window indices
     conv_to = int(np.floor(pyramid_scale / 2.))
     if (pyramid_scale % 2) == 0:
@@ -917,23 +970,23 @@
     # initializations
     pyramid_levels = 0
     work = True
     pyramid = {}
 
     # Determine the number of levels and
     # the last radius to be used in the highest level.
-    while work == True:
+    while work:
         _ = max_fine_radius / pyramid_scale ** pyramid_levels
         if _ > max_pyramid_radius:
             pyramid_levels = pyramid_levels + 1
         else:
             work = False
             last_radius = np.round(max_fine_radius / pyramid_scale ** pyramid_levels, decimals=0)
 
-    # fill out the pyramid dict with the metadata required for horizont searching.
+    # fill out the pyramid dict with the metadata required for horizon searching.
     for level in np.arange(pyramid_levels + 1):
         # the level 0 contains the other min_radius as the rest of levels
         if level == 0:
             min_radius = 1
             dem_fine = np.copy(np.pad(dem, max_pyramid_radius, mode="constant", constant_values=dem.min()))
         else:
             min_radius = min_pyramid_radius - 1
@@ -1000,15 +1053,15 @@
     ve_factor : int or float
         Vertical exaggeration factor.
     no_data : int or float
         Value that represents no_data, all pixels with this value are changed to np.nan .
 
     Returns
     -------
-    sky_illum_out : numpy.ndarray
+    sky_illumination : numpy.ndarray
         2D numpy result array of Sky illumination.
     """
     # standard pyramid settings
     pyramid_scale = 2
     max_pyramid_radius = 20
 
     if not (10000 >= ve_factor >= -10000):
@@ -1106,26 +1159,26 @@
 
             # ... and to the search radius
             for i_rad, radius in enumerate(move[direction]["distance"]):
                 # get shift index from move dictionary
                 shift_indx = move[direction]["shift"][i_rad]
                 # estimate the slope
                 _ = np.maximum((np.roll(height, shift_indx, axis=(0, 1)) - height) / radius, 0.)
-                # compare to the previus max slope and keep the larges
+                # compare to the previous max slope and keep the larges
                 max_slope = np.maximum(max_slope, _)
 
             # resample the max_slope to a lower pyramid level
             if i_level > 0:
                 lin_fine = pyramid[i_level - 1]["i_lin"] + (
                         conv_from + max_pyramid_radius * pyramid_scale - max_pyramid_radius)
                 col_fine = pyramid[i_level - 1]["i_col"] + (
                         conv_from + max_pyramid_radius * pyramid_scale - max_pyramid_radius)
                 lin_coarse = pyramid[i_level]["i_lin"] * pyramid_scale
                 col_coarse = pyramid[i_level]["i_col"] * pyramid_scale
-                interp_spline = scipy.interpolate.RectBivariateSpline(lin_coarse, col_coarse, max_slope, kx=1, ky=1)
+                interp_spline = RectBivariateSpline(lin_coarse, col_coarse, max_slope, kx=1, ky=1)
                 max_slope = interp_spline(lin_fine, col_fine)
 
         # convert to angle in radians and compute directional output
         _ = np.arctan(max_slope)
         uniform_a = uniform_a + (np.cos(_)) ** 2
         _d_aspect = -2 * np.sin(da) * np.cos(dir_rad - aspect)
         uniform_b = uniform_b + np.maximum(_d_aspect * (np.pi / 4. - _ / 2. - np.sin(2. * _) / 4.), 0)
@@ -1135,16 +1188,16 @@
             overcast_d = overcast_d + np.maximum(_d_aspect * (2. / 3. - np.cos(_) + _cos3 / 3.), 0)
         if compute_shadow and (direction == shadow_az):
             horizon_out = np.degrees(_[max_pyramid_radius:-max_pyramid_radius, max_pyramid_radius:-max_pyramid_radius])
             shadow_out = (horizon_out < shadow_el) * 1
             if shadow_horizon_only:
                 return {"shadow": shadow_out, "horizon": horizon_out}
 
-    # because of numeric stabilty check if the uniform_b is less then pi
-    uniform_out = (da) * np.cos(slope) * uniform_a + np.sin(slope) * np.minimum(uniform_b, np.pi)
+    # because of numeric stability check if the uniform_b is less then pi
+    uniform_out = da * np.cos(slope) * uniform_a + np.sin(slope) * np.minimum(uniform_b, np.pi)
     uniform_out = uniform_out[max_pyramid_radius:-max_pyramid_radius, max_pyramid_radius:-max_pyramid_radius]
 
     if compute_overcast:
         overcast_out = (2. * da / 3.) * np.cos(slope) * overcast_c + np.sin(slope) * overcast_d
         overcast_out = overcast_out[max_pyramid_radius:-max_pyramid_radius, max_pyramid_radius:-max_pyramid_radius]
         overcast_out = 0.33 * uniform_out + 0.67 * overcast_out
         overcast_out = overcast_out / overcast_out.max()
@@ -1266,15 +1319,15 @@
     # change no_data to np.nan
     if no_data is not None:
         dem[dem == no_data] = np.nan
 
     dem = dem.astype(np.float32)
     dem = dem * ve_factor
 
-    if feature_min < resolution:  # feature min can't be smaller than resolution
+    if feature_min < resolution:  # feature_min can't be smaller than resolution
         feature_min = resolution
 
     scaling_factor = int(scaling_factor)  # has to be integer
 
     # calculation of i and n (from article)
     i = int(np.floor(((feature_min - resolution) / (2 * resolution)) ** (1 / scaling_factor)))
     n = int(np.ceil(((feature_max - resolution) / (2 * resolution)) ** (1 / scaling_factor)))
@@ -1299,26 +1352,39 @@
     return msrm_out
 
 
 def integral_image(dem, data_type=np.float64):
     """
     Calculates integral image (summed-area table), where origin is left upper corner.
 
+    Parameters
+    ----------
+    dem : numpy.ndarray
+        Input digital elevation model as 2D numpy array.
+    data_type : np.__class__
+        dtype as numpy data type class (np.float64, np.int8, etc.)
+
+    Returns
+    -------
+    msrm_out : numpy.ndarray
+        Cumulative sum of the elements along each axis of a 2D array.
+
     References
     ----------
     https://en.wikipedia.org/wiki/Summed-area_table
 
     Examples
     --------
-    >>> print(integral_image(np.array([[7, 4, 7, 2],
+    In: print(integral_image(np.array([[7, 4, 7, 2],
     ... [6, 9, 9, 5],
     ... [6, 6, 7, 6]])))
-    [[ 7. 11. 18. 20.]
-     [13. 26. 42. 49.]
-     [19. 38. 61. 74.]]
+
+    Out: [[ 7. 11. 18. 20.]
+          [13. 26. 42. 49.]
+          [19. 38. 61. 74.]]
     """
     dem = dem.astype(data_type)
     return dem.cumsum(axis=0).cumsum(axis=1)
 
 
 def topographic_dev(dem, dem_i_nr_pixels, dem_i1, dem_i2, kernel_radius):
     """
@@ -1327,17 +1393,17 @@
     sD is standard deviation of kernel.
 
     Parameters
     ----------
     dem : numpy.ndarray
         Input digital elevation model as 2D numpy array.
     dem_i_nr_pixels : numpy.ndarray
-        Summed area table (itegral image) of number of pixels.
+        Summed area table (integral image) of number of pixels.
     dem_i1 : numpy.ndarray
-        Summed area table (itegral image) of dem.
+        Summed area table (integral image) of dem.
     dem_i2 : numpy.ndarray
         Summed area table (integral image) of dem squared (dem**2).
     kernel_radius : int
         Kernel radius (D).
 
     Returns
     -------
@@ -1350,36 +1416,40 @@
 
     kernel_nr_pix_arr = (np.roll(dem_i_nr_pixels, (radius_cell, radius_cell), axis=(0, 1)) +
                          np.roll(dem_i_nr_pixels, (-radius_cell - 1, -radius_cell - 1), axis=(0, 1)) -
                          np.roll(dem_i_nr_pixels, (-radius_cell - 1, radius_cell), axis=(0, 1)) -
                          np.roll(dem_i_nr_pixels, (radius_cell, -radius_cell - 1), axis=(0, 1)))
 
     # sum
-    dem_mean = np.roll(dem_i1, (radius_cell, radius_cell), axis=(0, 1)) + \
-               np.roll(dem_i1, (-radius_cell - 1, -radius_cell - 1), axis=(0, 1)) - \
-               np.roll(dem_i1, (-radius_cell - 1, radius_cell), axis=(0, 1)) - \
-               np.roll(dem_i1, (radius_cell, -radius_cell - 1), axis=(0, 1))
+    dem_mean = (np.roll(dem_i1, (radius_cell, radius_cell), axis=(0, 1)) +
+                np.roll(dem_i1, (-radius_cell - 1, -radius_cell - 1), axis=(0, 1)) -
+                np.roll(dem_i1, (-radius_cell - 1, radius_cell), axis=(0, 1)) -
+                np.roll(dem_i1, (radius_cell, -radius_cell - 1), axis=(0, 1)))
     # divide with nr of pixels inside kernel
-    dem_mean = dem_mean / kernel_nr_pix_arr
+    with np.errstate(divide='ignore', invalid='ignore'):  # Suppress warning for dividing by zero
+        dem_mean = dem_mean / kernel_nr_pix_arr
 
     # std
-    dem_std = np.roll(dem_i2, (radius_cell, radius_cell), axis=(0, 1)) + \
-              np.roll(dem_i2, (-radius_cell - 1, -radius_cell - 1), axis=(0, 1)) - \
-              np.roll(dem_i2, (-radius_cell - 1, radius_cell), axis=(0, 1)) - \
-              np.roll(dem_i2, (radius_cell, -radius_cell - 1), axis=(0, 1))
-    dem_std = np.sqrt(np.abs(dem_std / kernel_nr_pix_arr - dem_mean ** 2))
+    dem_std = (np.roll(dem_i2, (radius_cell, radius_cell), axis=(0, 1)) +
+               np.roll(dem_i2, (-radius_cell - 1, -radius_cell - 1), axis=(0, 1)) -
+               np.roll(dem_i2, (-radius_cell - 1, radius_cell), axis=(0, 1)) -
+               np.roll(dem_i2, (radius_cell, -radius_cell - 1), axis=(0, 1)))
+
+    with np.errstate(divide='ignore', invalid='ignore'):  # Suppress warning for dividing by zero
+        dem_std = np.sqrt(np.abs(dem_std / kernel_nr_pix_arr - dem_mean ** 2))
+        # returns nan values where division by zero happens
 
     dev_out = (np.roll(dem, (-1, -1), axis=(0, 1)) - dem_mean) / (dem_std + 1e-6)  # add 1e-6 to prevent division with 0
 
     return dev_out
 
 
 def max_elevation_deviation(dem, minimum_radius, maximum_radius, step):
     """
-    Calculates maximum deviation from mean elevation, DEVmax (Maximum Deviation from mean elevation) for each
+    Calculates maximum deviation from mean elevation, dev_max (Maximum Deviation from mean elevation) for each
     grid cell in a digital elevation model (DEM) across a range specified spatial scales.
 
     Parameters
     ----------
     dem : numpy.ndarray
         Input digital elevation model as 2D numpy array.
     minimum_radius : int
@@ -1406,42 +1476,43 @@
     idx_nan_dem_pad = np.isnan(dem_pad)
     # change nan to 0
     dem_pad[idx_nan_dem_pad] = 0
 
     # number of pixels for summed area table
     dem_i_nr_pixels = np.ones(dem_pad.shape)
     dem_i_nr_pixels[idx_nan_dem_pad] = 0
-    dem_i_nr_pixels = integral_image(dem_i_nr_pixels, np.int)
+    dem_i_nr_pixels = integral_image(dem_i_nr_pixels, np.int64)
 
+    # This outputs float64, which is by design. Change final array to float32 at the end of the function (at return)
     dem_i1 = integral_image(dem_pad)
     dem_i2 = integral_image(dem_pad ** 2)
 
     for kernel_radius in range(minimum_radius, maximum_radius + 1, step):
         dev = topographic_dev(dem_pad, dem_i_nr_pixels, dem_i1, dem_i2, kernel_radius)[
               maximum_radius:-(maximum_radius + 1),
               maximum_radius:-(maximum_radius + 1)]
         if kernel_radius == minimum_radius:
             dev_max_out = dev
-            rad_max_out = np.zeros_like(dev) + kernel_radius
+            rad_max_out = np.zeros_like(dev, dtype=np.float32) + kernel_radius
         else:
             rad_max_out = np.where(np.abs(dev_max_out) >= np.abs(dev), rad_max_out, kernel_radius)
             dev_max_out = np.where(np.abs(dev_max_out) >= np.abs(dev), dev_max_out, dev)
     # rad_max_out, radius of DEV for maxDEV (for each pixel)
 
     # change where dem nan back to nan
     dev_max_out[idx_nan_dem] = np.nan
     rad_max_out[idx_nan_dem] = np.nan
 
-    return dev_max_out
+    return dev_max_out.astype(np.float32)
 
 
 def mstp(dem,
-         local_scale=(1, 5, 1),
-         meso_scale=(5, 50, 5),
-         broad_scale=(50, 500, 50),
+         local_scale=(3, 21, 2),
+         meso_scale=(23, 203, 18),
+         broad_scale=(223, 2023, 180),
          lightness=1.2,
          ve_factor=1,
          no_data=None
          ):
     """
     Compute Multi-scale topographic position (MSTP).
 
@@ -1467,46 +1538,48 @@
     msrm_out : numpy.ndarray
         3D numpy RGB result array of Multi-scale topographic position.
     """
     if local_scale[0] > local_scale[1] or meso_scale[0] > meso_scale[1] or broad_scale[0] > broad_scale[1]:
         raise Exception("rvt.visualization.mstp: local_scale, meso_scale, broad_scale min has to be smaller than max!")
     if (local_scale[1] - local_scale[0] < local_scale[2]) or (meso_scale[1] - meso_scale[0] < meso_scale[2]) or \
             (broad_scale[1] - broad_scale[0] < broad_scale[2]):
-        raise Exception("rvt.visualization.mstp: local_scale, meso_scale, broad_scale step has to be within min and max!")
+        raise Exception("rvt.visualization.mstp: local_scale, meso_scale, broad_scale step has"
+                        " to be within min and max!")
     if not (10000 >= ve_factor >= -1000):
         raise Exception("rvt.visualization.mstp: ve_factor must be between -10000 and 10000!")
 
     # change no_data to np.nan
     if no_data is not None:
         dem[dem == no_data] = np.nan
 
     dem = dem.astype(np.float32)
     dem = dem * ve_factor
 
-    local_DEV = max_elevation_deviation(dem=dem, minimum_radius=local_scale[0], maximum_radius=local_scale[1],
+    local_dev = max_elevation_deviation(dem=dem, minimum_radius=local_scale[0], maximum_radius=local_scale[1],
                                         step=local_scale[2])
-    meso_DEV = max_elevation_deviation(dem=dem, minimum_radius=meso_scale[0], maximum_radius=meso_scale[1],
+    meso_dev = max_elevation_deviation(dem=dem, minimum_radius=meso_scale[0], maximum_radius=meso_scale[1],
                                        step=meso_scale[2])
-    broad_DEV = max_elevation_deviation(dem=dem, minimum_radius=broad_scale[0], maximum_radius=broad_scale[1],
+    broad_dev = max_elevation_deviation(dem=dem, minimum_radius=broad_scale[0], maximum_radius=broad_scale[1],
                                         step=broad_scale[2])
 
     cutoff = lightness
-    red = np.floor(512 / (1 + np.exp(-cutoff * np.abs(broad_DEV)))) - 256  # broad
-    green = np.floor(512 / (1 + np.exp(-cutoff * np.abs(meso_DEV)))) - 256  # meso
-    blue = np.floor(512 / (1 + np.exp(-cutoff * np.abs(local_DEV)))) - 256  # local
+    # RGB order - broad, meso, local
+    red = 1 - np.exp(-cutoff * np.abs(broad_dev))
+    green = 1 - np.exp(-cutoff * np.abs(meso_dev))
+    blue = 1 - np.exp(-cutoff * np.abs(local_dev))
 
     red[red < 0] = 0
     green[green < 0] = 0
     blue[blue < 0] = 0
 
-    red[red > 255] = 255
-    green[green > 255] = 255
-    blue[blue > 255] = 255
+    red[red > 1] = 1
+    green[green > 1] = 1
+    blue[blue > 1] = 1
 
-    return np.asarray([red, green, blue])  # RGB 24-bit (3 x 8bit)
+    return np.asarray([red, green, blue])  # RGB float32 (3 x 32bit)
 
 
 def fill_where_nan(dem, method="idw"):
     """
     Replaces np.nan values, with interpolation (extrapolation).
 
     Parameters
@@ -1524,19 +1597,19 @@
     """
     if np.all(~np.isnan(dem)):  # if there is no nan return dem
         return dem
 
     dem_out = np.copy(dem)
     mask = np.isnan(dem_out)
 
-    # 1D row linear interpolation
     if method == "linear_row":
+        # 1D row linear interpolation
         dem_out[mask] = np.interp(np.flatnonzero(mask), np.flatnonzero(~mask), dem_out[~mask])
 
-    if method.split("_")[0] == "idw":
+    elif method.split("_")[0] == "idw":
         radius = 20
         power = 2
         if len(method.split("_")) == 3:
             radius = int(method.split("_")[1])
             power = float(method.split("_")[2])
         nan_idx = zip(*np.where(mask))  # find nan positions
         for i_row, i_column in nan_idx:  # iterate through nans
@@ -1563,34 +1636,34 @@
             if np.all(np.isnan(nan_surrounding_arr)):  # whole surrounding array is nan
                 dem_out[i_row, i_column] = np.nan
             else:
                 # calculate distance array (wight matrix)
                 dist_arr = np.ones(nan_surrounding_arr.shape)  # all ones
                 # center pixel is 0 to calc distance matrix around 0 pixel with distance_transform_edt
                 dist_arr[i_row_center, i_column_center] = 0
-                dist_arr = scipy.ndimage.morphology.distance_transform_edt(dist_arr)
+                dist_arr = distance_transform_edt(dist_arr)
                 dist_arr[dist_arr == 0] = np.nan  # can't divide with zero
                 dist_arr = 1 / dist_arr ** power
                 nan_mask = np.isnan(nan_surrounding_arr)
                 dist_arr[nan_mask] = 0  # where nan weight matrix is zero
                 # calculate idw for one nan value
                 dem_out[i_row, i_column] = np.nansum(nan_surrounding_arr * dist_arr) / np.nansum(dist_arr)
 
     elif method == "kd_tree" or method == "nearest_neighbour" or method == "nearest_neighbor":
         x, y = np.mgrid[0:dem_out.shape[0], 0:dem_out.shape[1]]
-        xygood = np.array((x[~mask], y[~mask])).T
-        xybad = np.array((x[mask], y[mask])).T
+        xy_good = np.array((x[~mask], y[~mask])).T
+        xy_bad = np.array((x[mask], y[mask])).T
 
         # cKD-Tree (K-D Tree) interpolation
         # https://stackoverflow.com/questions/3662361/fill-in-missing-values-with-nearest-neighbour-in-python-numpy-masked-arrays
         if method == "kd_tree":
             leaf_size = 1000
-            dem_out[mask] = dem_out[~mask][scipy.spatial.cKDTree(data=xygood, leafsize=leaf_size).query(xybad)[1]]
+            dem_out[mask] = dem_out[~mask][cKDTree(data=xy_good, leafsize=leaf_size).query(xy_bad)[1]]
 
         # Nearest neighbour interpolation
         elif method == "nearest_neighbour" or method == "nearest_neighbor":
-            dem_out[mask] = scipy.interpolate.griddata(xygood, dem_out[~mask], xybad,
-                                                       method='nearest')
+            dem_out[mask] = griddata(xy_good, dem_out[~mask], xy_bad, method='nearest')
+
     else:
         raise Exception("rvt.visualization.fill_where_nan: Wrong method!")
 
     return dem_out
```

### Comparing `rvt_py-2.1.0/rvt_py.egg-info/PKG-INFO` & `rvt_py-2.2.0/rvt_py.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,120 @@
 Metadata-Version: 2.1
 Name: rvt-py
-Version: 2.1.0
-Summary: Relief Visualization Toolbox python library. It helps scientist visualize raster elevation model datasets. 
+Version: 2.2.0
+Summary: Relief Visualization Toolbox Python library. It helps scientist visualize raster elevation model datasets. 
 Home-page: https://github.com/EarthObservation/RVT_py
 Author: ZRC SAZU and University of Ljubljana (UL FGG)
 Author-email: ziga.kokalj@zrc-sazu.si
-License: UNKNOWN
 Project-URL: Documentation, https://rvt-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/EarthObservation/RVT_py
 Project-URL: Old RVT, https://iaps.zrc-sazu.si/en/rvt#v
 Project-URL: ArcGIS Pro, https://github.com/EarthObservation/rvt-arcgis-pro
 Project-URL: QGIS plugin, https://github.com/EarthObservation/rvt-qgis
 Keywords: relief_visualization_toolbox relief_visualization relief rvt raster raster_visualization visualization
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Relief Visualization Toolbox in Python
+[![PyPI](https://img.shields.io/pypi/v/RVT_py?style=flat-square)](https://pypi.org/project/rvt-py/)
+[![Anaconda-Server Badge](https://anaconda.org/zmigyyy/rvt_py/badges/version.svg)](https://anaconda.org/zmigyyy/rvt_py)
+[![Anaconda-Server Badge](https://anaconda.org/zmigyyy/rvt_py/badges/latest_release_date.svg)](https://anaconda.org/zmigyyy/rvt_py)
+
+# Relief Visualization Toolbox Python library
 
 ![](./docs/figures/RVT_head.png)
 
-Relief Visualization Toolbox was produced to help scientist visualize raster elevation model datasets. We have narrowed down the selection to include techniques that have proven to be effective for identification of small scale features. Default settings therefore assume working with high resolution digital elevation models, derived from airborne laser scanning missions (lidar).
+Relief Visualization Toolbox (RVT) was produced to help scientists visualize raster elevation model datasets. We have narrowed down the selection to include techniques that have proven to be effective for identification of small scale features. The default settings therefore assume working with high resolution digital elevation models derived from airborne laser scanning missions (lidar), however RVT methods can also be used for other purposes.
 
-Despite this, techniques are also used for different other purposes. Sky-view factor, for example, can be efficiently used in numerous studies where digital elevation model visualizations and automatic feature extraction techniques are indispensable, e.g. in geography, archeology,  geomorphology, cartography, hydrology, glaciology, forestry and disaster management. It can be used even in engineering applications, such as, predicting the availability of the GPS signal in urban areas.
+Sky-view factor, for example, can be efficiently used in numerous studies where digital elevation model visualizations and automatic feature extraction techniques are indispensable, e.g. in geography, archaeology,  geomorphology, cartography, hydrology, glaciology, forestry and disaster management. It can even be used in engineering applications, such as predicting the availability of the GPS signal in urban areas.
 
 Methods currently implemented are:
 
-*   hillshading,
-*   hillshading from multiple directions,
-*   slope gradient,
-*   simple local relief model,
-*   multi-scale relief model,
-*   sky illumination,
-*   sky-view factor (as developed by our team),
-*   anisotropic sky-view factor,
-*   positive and negative openness,
-*   local dominance,
+* hillshading,
+* hillshading from multiple directions,
+* slope gradient,
+* simple local relief model,
+* multi-scale relief model,
+* sky illumination,
+* sky-view factor (as developed by our team),
+* anisotropic sky-view factor,
+* positive and negative openness,
+* local dominance,
 *	multi-scale topographic position.
 
-For a more detailed description see references given at each method in the manual and a comparative paper describing them (e.g. Kokalj and Hesse 2017, see below).
+## RVT for Python
+
+The ``rvt`` Python package contains three modules:
 
-RVT python library called rvt contains 3 modules: vis (rvt.vis), blend (rvt.blend) and default (rvt.default). Modules contains:
-* vis       -   visualization functions (mentioned above), for computing visualizations;
-* blend     -   blender (mixer), for blending visualizations;
-* default   -   default values, class for defining default parameters with methods to compute and save visualization functions using set parameters.
+* `rvt.vis` for computing visualizations
 
-For every visualization function directory also contains Python Esri raster functions for ArcGIS Pro (rvt_esri_*.py).
+* `rvt.blend` for blending visualizations together
+  
+* ``rvt.default`` for defining default parameters with methods to compute and save visualization functions using set parameters
 
 ## References
 
 When using the tools, please cite:
 
 *   Kokalj, Ž., Somrak, M. 2019. Why Not a Single Image? Combining Visualizations to Facilitate Fieldwork and On-Screen Mapping. Remote Sensing 11(7): 747.
 *   Zakšek, K., Oštir, K., Kokalj, Ž. 2011. Sky-View Factor as a Relief Visualization Technique. Remote Sensing 3: 398-415.
 
 ## Installation
 
-### conda
+The RVT Python package can be installed using Conda or PyPI, and can be used in Python scripts, Jupyter Notebooks and ArcGIS Pro.
+
+RVT can also be installed as [a set of custom raster functions for ArcGIS](https://rvt-py.readthedocs.io/en/latest/install_arcgis.html "ArcGIS installation"), and [a plugin for QGIS](https://rvt-py.readthedocs.io/en/latest/install_qgis.html "QGIS installation").
+
+You can also clone the repository.
+
+### Conda
+
+The ``rvt`` package is [available from the Anaconda Cloud repository](https://anaconda.org/rvtpy/rvt_py "rvt_py on Anaconda Cloud"). Using Conda to install the ``rvt`` package will include all required libraries.
+
+To use this method, first [install Anaconda and Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html "Getting started with conda").
 
-You can install all required libraries and rvt-py with Anaconda environment from Anaconda cloud ([conda rvt_py](https://anaconda.org/zmigyyy/rvt_py)). To do that open Anaconda Prompt (activate conda environment) and run:
+Then open Anaconda Prompt (Windows) or Terminal (MacOS) and run:
 
-`conda install -c zmigyyy rvt_py`
+``conda install -c rvtpy rvt_py``
 
-### pypi
+### PyPI
 
-Another option is to install required libraries and rvt-py with Python Package Index, pypi ([pypi rvt-py](https://pypi.org/project/rvt-py)). To do that open command prompt (terminal) and run:
+Another option is to install the ``rvt-py`` package and required libraries [using the Python Package Index (PyPI)](https://pypi.org/project/rvt-py "rvt-py on PyPI").
 
-`pip install rvt-py`
+PyPI usually has problems installing ``gdal``, so [install ``gdal`` first](https://pypi.org/project/GDAL/ "GDAL on PyPI") to use this method.
 
-This might not work, because pypi usually has problems installing gdal. To solve that first try to install gdal then run above command.
+Then open Command Prompt (Windows) or Terminal (MacOS) and run:
 
-### requirements
+``pip install rvt-py``
 
-We suggest using an Anaconda environment (easiest gdal installation) and Python 3.6 or higher. Required libraries with tested versions (could also work with other versions):
+### Requirements
+
+Required libraries (specified versions have been tested, other versions may also work):
 
 *   numpy 1.19.2
 *   scipy 1.5.2
 *   gdal 3.0.2
 
-
-You can also clone the repository ([github rvt_py](https://github.com/EarthObservation/RVT_py)).
-
-Library `rvt-py` can be used in Python scripts, Jupyter Notebooks and in ArcGIS Pro.
+We recommend using Python 3.6 or higher and a Conda environment (this works best with ``gdal``).
 
 ## Documentation
-
-Documentation of the package and its usage is available at [Relief Visualization Toolbox in Python documentation](https://rvt-py.readthedocs.io/).
+Documentation of the package and its use is available at [Relief Visualization Toolbox in Python documentation](https://rvt-py.readthedocs.io/).
 
 ## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-Please report any bugs and suggestions for improvements.
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please report any bugs and suggestions for improvements.
 
 ## Acknowledgment
-
 Development of RVT Python scripts was part financed by the Slovenian Research Agency core funding No. P2-0406, and by research project No. J6-9395.
 
 ## License
 This project is licensed under the terms of the [Apache License](LICENSE).
 
+## About
+RVT Python library by Žiga Kokalj, Žiga Maroh, Krištof Oštir, Klemen Zakšek and Nejc Čož, 2022.
+
+It is developed in collaboration between ZRC SAZU and University of Ljubljana.
```

### Comparing `rvt_py-2.1.0/setup.cfg` & `rvt_py-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `rvt_py-2.1.0/setup.py` & `rvt_py-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rvt_py",
-    version="2.1.0",
+    version="2.2.0",
     author="ZRC SAZU and University of Ljubljana (UL FGG)",
     author_email="ziga.kokalj@zrc-sazu.si",
-    description="Relief Visualization Toolbox python library. "
+    description="Relief Visualization Toolbox Python library. "
                 "It helps scientist visualize raster elevation model datasets. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EarthObservation/RVT_py",
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

