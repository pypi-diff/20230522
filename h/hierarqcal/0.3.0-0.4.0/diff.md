# Comparing `tmp/hierarqcal-0.3.0.tar.gz` & `tmp/hierarqcal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/matt/code/projects/hierarqcal/dist/.tmp-sh4dyu10/hierarqcal-0.3.0.tar", last modified: Mon Jan 23 15:03:48 2023, max compression
+gzip compressed data, was "hierarqcal-0.4.0.tar", last modified: Mon May 22 12:02:25 2023, max compression
```

## Comparing `hierarqcal-0.3.0.tar` & `hierarqcal-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-01-23 15:03:48.801934 hierarqcal-0.3.0/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1528 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/LICENSE.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     4045 2023-01-23 15:03:48.801934 hierarqcal-0.3.0/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     3853 2023-01-23 15:03:37.000000 hierarqcal-0.3.0/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-01-23 15:03:48.801934 hierarqcal-0.3.0/hierarqcal/
--rw-rw-r--   0 matt      (1000) matt      (1000)      258 2023-01-23 11:43:45.000000 hierarqcal-0.3.0/hierarqcal/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-01-23 15:03:48.801934 hierarqcal-0.3.0/hierarqcal/cirq/
--rw-rw-r--   0 matt      (1000) matt      (1000)       55 2023-01-23 10:11:40.000000 hierarqcal-0.3.0/hierarqcal/cirq/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4024 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/hierarqcal/cirq/cirq_helper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6869 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/hierarqcal/cirq/tf_helper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    25189 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/hierarqcal/core.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-01-23 15:03:48.801934 hierarqcal-0.3.0/hierarqcal/pennylane/
--rw-rw-r--   0 matt      (1000) matt      (1000)       82 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/hierarqcal/pennylane/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4155 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/hierarqcal/pennylane/pennylane_helper.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-01-23 15:03:48.801934 hierarqcal-0.3.0/hierarqcal/qiskit/
--rw-rw-r--   0 matt      (1000) matt      (1000)       58 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/hierarqcal/qiskit/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5362 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/hierarqcal/qiskit/qiskit_helper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6359 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/hierarqcal/utils.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-01-23 15:03:48.801934 hierarqcal-0.3.0/hierarqcal.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)     4045 2023-01-23 15:03:48.000000 hierarqcal-0.3.0/hierarqcal.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      504 2023-01-23 15:03:48.000000 hierarqcal-0.3.0/hierarqcal.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-01-23 15:03:48.000000 hierarqcal-0.3.0/hierarqcal.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)      194 2023-01-23 15:03:48.000000 hierarqcal-0.3.0/hierarqcal.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       11 2023-01-23 15:03:48.000000 hierarqcal-0.3.0/hierarqcal.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       84 2023-01-23 08:42:03.000000 hierarqcal-0.3.0/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)      560 2023-01-23 15:03:48.801934 hierarqcal-0.3.0/setup.cfg
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.756121 hierarqcal-0.4.0/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1528 2023-01-23 08:42:03.000000 hierarqcal-0.4.0/LICENSE.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4806 2023-05-22 12:02:25.756121 hierarqcal-0.4.0/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4614 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/README.md
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      335 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal/cirq/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       42 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/cirq/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2007 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/cirq/cirq_circuits.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2467 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/cirq/cirq_helper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6869 2023-01-23 08:42:03.000000 hierarqcal-0.4.0/hierarqcal/cirq/tf_helper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    53811 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/core.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal/pennylane/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       56 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/pennylane/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1464 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/pennylane/pennylane_circuits.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5028 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/pennylane/pennylane_helper.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal/qiskit/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       45 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/qiskit/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2391 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/qiskit/qiskit_circuits.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2993 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/qiskit/qiskit_helper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7702 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/utils.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal.egg-info/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4806 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      636 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)      167 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       11 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       84 2023-01-23 08:42:03.000000 hierarqcal-0.4.0/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)      472 2023-05-22 12:02:25.756121 hierarqcal-0.4.0/setup.cfg
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/tests/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-01-23 08:42:03.000000 hierarqcal-0.4.0/tests/test_core.py
```

### Comparing `hierarqcal-0.3.0/LICENSE.txt` & `hierarqcal-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hierarqcal-0.3.0/PKG-INFO` & `hierarqcal-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-Metadata-Version: 2.1
-Name: hierarqcal
-Version: 0.3.0
-Description-Content-Type: text/markdown
-Provides-Extra: cirq
-Provides-Extra: pennylane
-Provides-Extra: qiskit
-License-File: LICENSE.txt
-
-# HierarQcal
+# HierarQcal 
 
 <img src="https://github.com/matt-lourens/hierarqcal/blob/master/img/dalle_img.png?raw=true" alt="dalle image" height="150" style="padding-right:10px" align="left"/>
 
 <p style="height:150px">
-**HierarQcal** is an Open-Source Python Package for Building Custom Quantum Circuits for Machine Learning. The package simplifies the process of creating general quantum convolutional neural networks (QCNN) by enabling an hierarchical design process. With HierarQcal, automatic generation of QCNN circuits is made easy, and it facilitates QCNN search space design for neural architecture search (NAS). The package includes primitives such as <code>Qconv, Qpool, Qdense, Qfree </code> that can be stacked together hierarchically to form complex QCNN circuit architectures.
+<b>HierarQcal</b> is a quantum circuit builder that simplifies circuit design, composition, generation, scaling, and parameter management. It provides an intuitive and dynamic data structure for constructing computation graphs hierarchically. This enables the generation of complex quantum circuit architectures, which is particularly useful for Neural Architecture Search (NAS), where an algorithm can determine the most efficient circuit architecture for a specific task and hardware. HierarQcal also facilitates the creation of hierarchical quantum circuits, such as those resembling tensor tree networks or MERA, with a single line of code. The package is open-source and framework-agnostic, it includes tutorials for Qiskit, PennyLane, and Cirq. Built to address the unique challenges of applying NAS to Quantum Computing, HierarQcal offers a novel approach to explore and optimize quantum circuit architectures. 
 </p>
 <br/>
 
-*A robot building itself with artifical intelligence, pencil drawing -  generated with* [Dall E 2](https://openai.com/dall-e-2/)
+*A robot building itself with artificial intelligence, pencil drawing -  generated with* [Dall E 2](https://openai.com/dall-e-2/)
+___
+
+
+[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](http://unitary.fund)
 
 
 ## Quick example
+
+#### Building a [Quantum Convolutional Neural Network (QCNN)](https://qiskit.org/ecosystem/machine-learning/tutorials/11_quantum_convolutional_neural_networks.html) with one line of code:
+
 ```python
-from hierarqcal import Qconv, Qpool, Qfree
-qcnn = Qfree(8) + (Qconv(stride=1) + Qpool(filter="right")) * 3
+from hierarqcal import Qinit, Qcycle, Qmask
+hierq = Qinit(8) + (Qcycle(mapping=u) + Qmask("right", mapping=v))*3
 ```
-$\text{QCNN:}$
 
 <img src="https://github.com/matt-lourens/hierarqcal/blob/master/img/rbt_right.png?raw=true" style="border:solid 2px black;">
 
+#### Modular and hierarchical circuit building:
 ```python
 ### Reverse binary tree
-from hierarqcal import Qconv, Qpool, Qfree
+from hierarqcal import Qinit, Qcycle, Qmask
 # motif: level 1
-m1_1 = Qconv(stride=2)
-m1_2 = Qpool(filter="left")
+m1_1 = Qcycle(stride=2)
+m1_2 = Qmask(pattern="left")
 # motif: level 2
 m2_1 = m1_1 + m1_2
 # motif: level 3
-m3_1 = Qfree(8) + m2_1 * 3
+m3_1 = Qinit(8) + m2_1 * 3
 ```
 $m^3_1\rightarrow \text{QCNN}:$
 
 <img src="https://github.com/matt-lourens/hierarqcal/blob/master/img/rbt_left.png?raw=true" style="border:solid 2px black;">
 
 ```python
 # extending follows naturally, repeating the above circuit 5 times is just:
 m3_1 * 5
 ```
 ## Installation
+[![PyPI version](https://badge.fury.io/py/hierarqcal.svg)](https://badge.fury.io/py/hierarqcal)
+
 <code>HierarQcal</code> is hosted on [pypi](https://pypi.org/project/hierarqcal/) and can be installed via pip:
 
 ```bash
 # Based on the quantum computing framework you use, choose one of:
 pip install hierarqcal[cirq]
 # or
 pip install hierarqcal[qiskit]
@@ -61,34 +61,30 @@
 
 The package is quantum computing framework independent, there are helper functions for Cirq, Qiskit and Pennylane to represent the circuits in their respective frameworks. You can also use the the package independent of any framework, if you want to do this just run:
 ```bash
 pip install hierarqcal
 ```
 
 ## Tutorial and Documentation
-There are quickstart tutorials for each major Quantum computing framework: 
- - [HierarQcal Cirq Tutorial](https://github.com/matt-lourens/hierarqcal/blob/master/examples/examples_cirq.ipynb)
- - [HierarQcal Qiskit Tutorial](https://github.com/matt-lourens/hierarqcal/blob/master/examples/examples_qiskit.ipynb) 
- - [HierarQcal Pennylane Tutorial](https://github.com/matt-lourens/hierarqcal/blob/master/examples/examples_pennylane.ipynb). 
+There is a quickstart tutorial containing code examples for qiskit, cirq and pennylane: 
+ - [HierarQcal Quickstart](https://github.com/matt-lourens/hierarqcal/blob/master/examples/quickstart.ipynb)
  
- For more detailed usage see the [documentation](https://matt-lourens.github.io/hierarqcal/index.html).
+ For an overview of the package there is this [blogpost](https://unitary.fund/posts/2023_hierarqcal.html) which might be worht a read. Altough the syntax has changed since then, the overall functionality is still the same. There is also this paper on the [arXiv](https://arxiv.org/abs/2210.15073) which describes some of the use cases of the package. For specific details see the [documentation](https://matt-lourens.github.io/hierarqcal/index.html).
 
 ## Contributing
 We welcome contributions to the project. Please see the [contribution guidelines](https://github.com/matt-lourens/hierarqcal/blob/master/CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md) for more information.
 
 ## License
 BSD 3-Clause "New" or "Revised" License, see [LICENSE](https://github.com/matt-lourens/hierarqcal/blob/master/LICENSE.txt) for more information.
 
 ## Citation
 ```latex
-@article{lourensArchitectureRepresentationsQuantum2022,
-  doi = {10.48550/ARXIV.2210.15073},
-  url = {https://arxiv.org/abs/2210.15073},
-  author = {Lourens, Matt and Sinayskiy, Ilya and Park, Daniel K. and Blank, Carsten and Petruccione,   Francesco},
-  keywords = {Quantum Physics (quant-ph), Artificial Intelligence (cs.AI)},
-  title = {Architecture representations for quantum convolutional neural networks},
-  publisher = {arXiv},
-  journal = {arXiv:2210.15073[quant-ph]},
-  year = {2022},
-  copyright = {arXiv.org perpetual, non-exclusive license}
+@article{lourens2023hierarchical,
+      title={Hierarchical quantum circuit representations for neural architecture search},
+      url = {https://arxiv.org/abs/2210.15073},
+      author={Matt Lourens and Ilya Sinayskiy and Daniel K. Park and Carsten Blank and Francesco Petruccione},
+      year={2023},
+      eprint={2210.15073},
+      archivePrefix={arXiv},
+      primaryClass={quant-ph}
 }
-```
+```
```

### Comparing `hierarqcal-0.3.0/hierarqcal/cirq/tf_helper.py` & `hierarqcal-0.4.0/hierarqcal/cirq/tf_helper.py`

 * *Files identical despite different names*

### Comparing `hierarqcal-0.3.0/hierarqcal.egg-info/PKG-INFO` & `hierarqcal-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 Metadata-Version: 2.1
 Name: hierarqcal
-Version: 0.3.0
+Version: 0.4.0
 Description-Content-Type: text/markdown
 Provides-Extra: cirq
 Provides-Extra: pennylane
 Provides-Extra: qiskit
 License-File: LICENSE.txt
 
-# HierarQcal
+# HierarQcal 
 
 <img src="https://github.com/matt-lourens/hierarqcal/blob/master/img/dalle_img.png?raw=true" alt="dalle image" height="150" style="padding-right:10px" align="left"/>
 
 <p style="height:150px">
-**HierarQcal** is an Open-Source Python Package for Building Custom Quantum Circuits for Machine Learning. The package simplifies the process of creating general quantum convolutional neural networks (QCNN) by enabling an hierarchical design process. With HierarQcal, automatic generation of QCNN circuits is made easy, and it facilitates QCNN search space design for neural architecture search (NAS). The package includes primitives such as <code>Qconv, Qpool, Qdense, Qfree </code> that can be stacked together hierarchically to form complex QCNN circuit architectures.
+<b>HierarQcal</b> is a quantum circuit builder that simplifies circuit design, composition, generation, scaling, and parameter management. It provides an intuitive and dynamic data structure for constructing computation graphs hierarchically. This enables the generation of complex quantum circuit architectures, which is particularly useful for Neural Architecture Search (NAS), where an algorithm can determine the most efficient circuit architecture for a specific task and hardware. HierarQcal also facilitates the creation of hierarchical quantum circuits, such as those resembling tensor tree networks or MERA, with a single line of code. The package is open-source and framework-agnostic, it includes tutorials for Qiskit, PennyLane, and Cirq. Built to address the unique challenges of applying NAS to Quantum Computing, HierarQcal offers a novel approach to explore and optimize quantum circuit architectures. 
 </p>
 <br/>
 
-*A robot building itself with artifical intelligence, pencil drawing -  generated with* [Dall E 2](https://openai.com/dall-e-2/)
+*A robot building itself with artificial intelligence, pencil drawing -  generated with* [Dall E 2](https://openai.com/dall-e-2/)
+___
+
+
+[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](http://unitary.fund)
 
 
 ## Quick example
+
+#### Building a [Quantum Convolutional Neural Network (QCNN)](https://qiskit.org/ecosystem/machine-learning/tutorials/11_quantum_convolutional_neural_networks.html) with one line of code:
+
 ```python
-from hierarqcal import Qconv, Qpool, Qfree
-qcnn = Qfree(8) + (Qconv(stride=1) + Qpool(filter="right")) * 3
+from hierarqcal import Qinit, Qcycle, Qmask
+hierq = Qinit(8) + (Qcycle(mapping=u) + Qmask("right", mapping=v))*3
 ```
-$\text{QCNN:}$
 
 <img src="https://github.com/matt-lourens/hierarqcal/blob/master/img/rbt_right.png?raw=true" style="border:solid 2px black;">
 
+#### Modular and hierarchical circuit building:
 ```python
 ### Reverse binary tree
-from hierarqcal import Qconv, Qpool, Qfree
+from hierarqcal import Qinit, Qcycle, Qmask
 # motif: level 1
-m1_1 = Qconv(stride=2)
-m1_2 = Qpool(filter="left")
+m1_1 = Qcycle(stride=2)
+m1_2 = Qmask(pattern="left")
 # motif: level 2
 m2_1 = m1_1 + m1_2
 # motif: level 3
-m3_1 = Qfree(8) + m2_1 * 3
+m3_1 = Qinit(8) + m2_1 * 3
 ```
 $m^3_1\rightarrow \text{QCNN}:$
 
 <img src="https://github.com/matt-lourens/hierarqcal/blob/master/img/rbt_left.png?raw=true" style="border:solid 2px black;">
 
 ```python
 # extending follows naturally, repeating the above circuit 5 times is just:
 m3_1 * 5
 ```
 ## Installation
+[![PyPI version](https://badge.fury.io/py/hierarqcal.svg)](https://badge.fury.io/py/hierarqcal)
+
 <code>HierarQcal</code> is hosted on [pypi](https://pypi.org/project/hierarqcal/) and can be installed via pip:
 
 ```bash
 # Based on the quantum computing framework you use, choose one of:
 pip install hierarqcal[cirq]
 # or
 pip install hierarqcal[qiskit]
@@ -61,34 +70,30 @@
 
 The package is quantum computing framework independent, there are helper functions for Cirq, Qiskit and Pennylane to represent the circuits in their respective frameworks. You can also use the the package independent of any framework, if you want to do this just run:
 ```bash
 pip install hierarqcal
 ```
 
 ## Tutorial and Documentation
-There are quickstart tutorials for each major Quantum computing framework: 
- - [HierarQcal Cirq Tutorial](https://github.com/matt-lourens/hierarqcal/blob/master/examples/examples_cirq.ipynb)
- - [HierarQcal Qiskit Tutorial](https://github.com/matt-lourens/hierarqcal/blob/master/examples/examples_qiskit.ipynb) 
- - [HierarQcal Pennylane Tutorial](https://github.com/matt-lourens/hierarqcal/blob/master/examples/examples_pennylane.ipynb). 
+There is a quickstart tutorial containing code examples for qiskit, cirq and pennylane: 
+ - [HierarQcal Quickstart](https://github.com/matt-lourens/hierarqcal/blob/master/examples/quickstart.ipynb)
  
- For more detailed usage see the [documentation](https://matt-lourens.github.io/hierarqcal/index.html).
+ For an overview of the package there is this [blogpost](https://unitary.fund/posts/2023_hierarqcal.html) which might be worht a read. Altough the syntax has changed since then, the overall functionality is still the same. There is also this paper on the [arXiv](https://arxiv.org/abs/2210.15073) which describes some of the use cases of the package. For specific details see the [documentation](https://matt-lourens.github.io/hierarqcal/index.html).
 
 ## Contributing
 We welcome contributions to the project. Please see the [contribution guidelines](https://github.com/matt-lourens/hierarqcal/blob/master/CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md) for more information.
 
 ## License
 BSD 3-Clause "New" or "Revised" License, see [LICENSE](https://github.com/matt-lourens/hierarqcal/blob/master/LICENSE.txt) for more information.
 
 ## Citation
 ```latex
-@article{lourensArchitectureRepresentationsQuantum2022,
-  doi = {10.48550/ARXIV.2210.15073},
-  url = {https://arxiv.org/abs/2210.15073},
-  author = {Lourens, Matt and Sinayskiy, Ilya and Park, Daniel K. and Blank, Carsten and Petruccione,   Francesco},
-  keywords = {Quantum Physics (quant-ph), Artificial Intelligence (cs.AI)},
-  title = {Architecture representations for quantum convolutional neural networks},
-  publisher = {arXiv},
-  journal = {arXiv:2210.15073[quant-ph]},
-  year = {2022},
-  copyright = {arXiv.org perpetual, non-exclusive license}
+@article{lourens2023hierarchical,
+      title={Hierarchical quantum circuit representations for neural architecture search},
+      url = {https://arxiv.org/abs/2210.15073},
+      author={Matt Lourens and Ilya Sinayskiy and Daniel K. Park and Carsten Blank and Francesco Petruccione},
+      year={2023},
+      eprint={2210.15073},
+      archivePrefix={arXiv},
+      primaryClass={quant-ph}
 }
 ```
```

