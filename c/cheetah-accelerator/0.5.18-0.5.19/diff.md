# Comparing `tmp/cheetah-accelerator-0.5.18.tar.gz` & `tmp/cheetah-accelerator-0.5.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheetah-accelerator-0.5.18.tar", last modified: Mon Feb  6 17:24:05 2023, max compression
+gzip compressed data, was "cheetah-accelerator-0.5.19.tar", last modified: Mon May 22 07:44:46 2023, max compression
```

## Comparing `cheetah-accelerator-0.5.18.tar` & `cheetah-accelerator-0.5.19.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxr-xr-x   0 jankaiser   (501) staff       (20)        0 2023-02-06 17:24:05.307859 cheetah-accelerator-0.5.18/
--rw-r--r--   0 jankaiser   (501) staff       (20)     2892 2023-02-06 17:24:05.307661 cheetah-accelerator-0.5.18/PKG-INFO
--rw-r--r--   0 jankaiser   (501) staff       (20)     2563 2023-02-02 11:54:41.000000 cheetah-accelerator-0.5.18/README.md
-drwxr-xr-x   0 jankaiser   (501) staff       (20)        0 2023-02-06 17:24:05.306301 cheetah-accelerator-0.5.18/cheetah/
--rw-r--r--   0 jankaiser   (501) staff       (20)       66 2022-09-28 18:01:00.000000 cheetah-accelerator-0.5.18/cheetah/__init__.py
--rw-r--r--   0 jankaiser   (501) staff       (20)    32249 2023-02-06 17:17:20.000000 cheetah-accelerator-0.5.18/cheetah/accelerator.py
--rw-r--r--   0 jankaiser   (501) staff       (20)    26348 2023-02-06 17:18:53.000000 cheetah-accelerator-0.5.18/cheetah/particles.py
--rw-r--r--   0 jankaiser   (501) staff       (20)     4382 2023-02-05 09:15:20.000000 cheetah-accelerator-0.5.18/cheetah/utils.py
-drwxr-xr-x   0 jankaiser   (501) staff       (20)        0 2023-02-06 17:24:05.307270 cheetah-accelerator-0.5.18/cheetah_accelerator.egg-info/
--rw-r--r--   0 jankaiser   (501) staff       (20)     2892 2023-02-06 17:24:05.000000 cheetah-accelerator-0.5.18/cheetah_accelerator.egg-info/PKG-INFO
--rw-r--r--   0 jankaiser   (501) staff       (20)      313 2023-02-06 17:24:05.000000 cheetah-accelerator-0.5.18/cheetah_accelerator.egg-info/SOURCES.txt
--rw-r--r--   0 jankaiser   (501) staff       (20)        1 2023-02-06 17:24:05.000000 cheetah-accelerator-0.5.18/cheetah_accelerator.egg-info/dependency_links.txt
--rw-r--r--   0 jankaiser   (501) staff       (20)       29 2023-02-06 17:24:05.000000 cheetah-accelerator-0.5.18/cheetah_accelerator.egg-info/requires.txt
--rw-r--r--   0 jankaiser   (501) staff       (20)        8 2023-02-06 17:24:05.000000 cheetah-accelerator-0.5.18/cheetah_accelerator.egg-info/top_level.txt
--rw-r--r--   0 jankaiser   (501) staff       (20)       38 2023-02-06 17:24:05.307921 cheetah-accelerator-0.5.18/setup.cfg
--rw-r--r--   0 jankaiser   (501) staff       (20)      713 2023-02-06 17:19:56.000000 cheetah-accelerator-0.5.18/setup.py
+drwxr-xr-x   0 jankaiser   (501) staff       (20)        0 2023-05-22 07:44:46.719596 cheetah-accelerator-0.5.19/
+-rw-r--r--   0 jankaiser   (501) staff       (20)     3258 2023-05-22 07:44:46.719468 cheetah-accelerator-0.5.19/PKG-INFO
+-rw-r--r--   0 jankaiser   (501) staff       (20)     2906 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/README.md
+drwxr-xr-x   0 jankaiser   (501) staff       (20)        0 2023-05-22 07:44:46.717635 cheetah-accelerator-0.5.19/cheetah/
+-rw-r--r--   0 jankaiser   (501) staff       (20)       81 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/cheetah/__init__.py
+-rw-r--r--   0 jankaiser   (501) staff       (20)    36311 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/cheetah/accelerator.py
+-rw-r--r--   0 jankaiser   (501) staff       (20)    28595 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/cheetah/particles.py
+-rw-r--r--   0 jankaiser   (501) staff       (20)     4460 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/cheetah/utils.py
+drwxr-xr-x   0 jankaiser   (501) staff       (20)        0 2023-05-22 07:44:46.718298 cheetah-accelerator-0.5.19/cheetah_accelerator.egg-info/
+-rw-r--r--   0 jankaiser   (501) staff       (20)     3258 2023-05-22 07:44:46.000000 cheetah-accelerator-0.5.19/cheetah_accelerator.egg-info/PKG-INFO
+-rw-r--r--   0 jankaiser   (501) staff       (20)      483 2023-05-22 07:44:46.000000 cheetah-accelerator-0.5.19/cheetah_accelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 jankaiser   (501) staff       (20)        1 2023-05-22 07:44:46.000000 cheetah-accelerator-0.5.19/cheetah_accelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 jankaiser   (501) staff       (20)       29 2023-05-22 07:44:46.000000 cheetah-accelerator-0.5.19/cheetah_accelerator.egg-info/requires.txt
+-rw-r--r--   0 jankaiser   (501) staff       (20)        8 2023-05-22 07:44:46.000000 cheetah-accelerator-0.5.19/cheetah_accelerator.egg-info/top_level.txt
+-rw-r--r--   0 jankaiser   (501) staff       (20)       38 2023-05-22 07:44:46.719640 cheetah-accelerator-0.5.19/setup.cfg
+-rw-r--r--   0 jankaiser   (501) staff       (20)      742 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/setup.py
+drwxr-xr-x   0 jankaiser   (501) staff       (20)        0 2023-05-22 07:44:46.719280 cheetah-accelerator-0.5.19/test/
+-rw-r--r--   0 jankaiser   (501) staff       (20)    37392 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/test/test_accelerator.py
+-rw-r--r--   0 jankaiser   (501) staff       (20)      519 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/test/test_external_import.py
+-rw-r--r--   0 jankaiser   (501) staff       (20)    20265 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/test/test_final.py
+-rw-r--r--   0 jankaiser   (501) staff       (20)    11265 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/test/test_less_pytest.py
+-rw-r--r--   0 jankaiser   (501) staff       (20)      376 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/test/test_parameterbeam.py
+-rw-r--r--   0 jankaiser   (501) staff       (20)    14890 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/test/test_particles.py
+-rw-r--r--   0 jankaiser   (501) staff       (20)      538 2023-05-22 07:38:50.000000 cheetah-accelerator-0.5.19/test/test_tracking.py
```

### Comparing `cheetah-accelerator-0.5.18/PKG-INFO` & `cheetah-accelerator-0.5.19/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: cheetah-accelerator
-Version: 0.5.18
+Version: 0.5.19
 Summary: Fast particle accelerator optics simulation for reinforcement learning and optimisation applications.
 Home-page: https://github.com/desy-ml/cheetah
 Author: Jan Kaiser & Oliver Stein
 Author-email: jan.kaiser@desy.de
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
+<img src="images/logo.png" align="right" width="25%"/>
+
 # Cheetah
 
 Cheetah is a particle tracking accelerator we built specifically to speed up the training of reinforcement learning models.
 
-
 ## Installation
 
 Simply install *Cheetah* from PyPI by running the following command.
 
 ```bash
 pip install cheetah-accelerator
 ```
 
-
 ## How To Use
 
 A sequence of accelerator elements (or a lattice) is called a `Segment` in *Cheetah*. You can create a `Segment` as follows
 
 ```python
 segment = Segment([
     BPM(name="BPM1SMATCH"),
@@ -79,15 +80,14 @@
 segment.plot_overview(beam=beam)
 ```
 
 ![Overview Plot](images/misalignment.png)
 
 where the optional keyword argument `beam` is the incoming beam represented by the reference particles. Cheetah will use a default incoming beam, if no beam is passed.
 
-
 ## Cite Cheetah
 
 To cite Cheetah in publications:
 
 ```bibtex
 @inproceedings{stein2022accelerating,
     author = {Stein, Oliver and
@@ -95,7 +95,24 @@
               Eichler, Annika},
     title = {Accelerating Linear Beam Dynamics Simulations for Machine Learning Applications},
     booktitle = {Proceedings of the 13th International Particle Accelerator Conference},
     year = {2022},
     url = {https://github.com/desy-ml/cheetah},
 }
 ```
+
+## For Developers
+
+Activate your virtual envrionment. (Optional)
+
+Install the cheetah package as editable
+
+```sh
+pip install -e .
+```
+
+We suggest to install pre-commit hooks to automatically conform with the code formatting in commits:
+
+```sh
+pip install pre-commit
+pre-commit install
+```
```

### Comparing `cheetah-accelerator-0.5.18/README.md` & `cheetah-accelerator-0.5.19/cheetah_accelerator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+Metadata-Version: 2.1
+Name: cheetah-accelerator
+Version: 0.5.19
+Summary: Fast particle accelerator optics simulation for reinforcement learning and optimisation applications.
+Home-page: https://github.com/desy-ml/cheetah
+Author: Jan Kaiser & Oliver Stein
+Author-email: jan.kaiser@desy.de
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+<img src="images/logo.png" align="right" width="25%"/>
+
 # Cheetah
 
 Cheetah is a particle tracking accelerator we built specifically to speed up the training of reinforcement learning models.
 
-
 ## Installation
 
 Simply install *Cheetah* from PyPI by running the following command.
 
 ```bash
 pip install cheetah-accelerator
 ```
 
-
 ## How To Use
 
 A sequence of accelerator elements (or a lattice) is called a `Segment` in *Cheetah*. You can create a `Segment` as follows
 
 ```python
 segment = Segment([
     BPM(name="BPM1SMATCH"),
@@ -70,15 +80,14 @@
 segment.plot_overview(beam=beam)
 ```
 
 ![Overview Plot](images/misalignment.png)
 
 where the optional keyword argument `beam` is the incoming beam represented by the reference particles. Cheetah will use a default incoming beam, if no beam is passed.
 
-
 ## Cite Cheetah
 
 To cite Cheetah in publications:
 
 ```bibtex
 @inproceedings{stein2022accelerating,
     author = {Stein, Oliver and
@@ -86,7 +95,24 @@
               Eichler, Annika},
     title = {Accelerating Linear Beam Dynamics Simulations for Machine Learning Applications},
     booktitle = {Proceedings of the 13th International Particle Accelerator Conference},
     year = {2022},
     url = {https://github.com/desy-ml/cheetah},
 }
 ```
+
+## For Developers
+
+Activate your virtual envrionment. (Optional)
+
+Install the cheetah package as editable
+
+```sh
+pip install -e .
+```
+
+We suggest to install pre-commit hooks to automatically conform with the code formatting in commits:
+
+```sh
+pip install pre-commit
+pre-commit install
+```
```

### Comparing `cheetah-accelerator-0.5.18/cheetah/accelerator.py` & `cheetah-accelerator-0.5.19/cheetah/accelerator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from copy import deepcopy
+from typing import Optional
 
+import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from matplotlib.patches import Rectangle
 from scipy import constants
 from scipy.stats import multivariate_normal
 
@@ -14,14 +16,27 @@
 REST_ENERGY = (
     constants.electron_mass
     * constants.speed_of_light**2
     / constants.elementary_charge
 )
 
 
+class DeviceError(Exception):
+    """
+    Used to create an exception, in case the device used for the beam
+    and the elements are different.
+    """
+
+    def __init__(self):
+        super().__init__(
+            "Warning! The device used for calculating the elements is not the same, "
+            "as the device used to calculate the Beam."
+        )
+
+
 class Element:
     """
     Base class for elements of particle accelerators.
 
     Parameters
     ----------
     name : string, optional
@@ -41,34 +56,64 @@
         Device to move the beam's particle array to. If set to `"auto"` a CUDA GPU is
         selected if available. The CPU is used otherwise.
     """
 
     is_active = False
     is_skippable = True
 
-    def __init__(self, name=None, device="auto"):
+    def __init__(self, name: Optional[str] = None, device: str = "auto") -> None:
         global ELEMENT_COUNT
         if name is not None:
             self.name = name
         else:
             self.name = f"{self.__class__.__name__}_{ELEMENT_COUNT:06d}"
         ELEMENT_COUNT += 1
 
         if device == "auto":
             device = "cuda" if torch.cuda.is_available() else "cpu"
         self.device = device
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
+        """
+        Generates the element's transfer map that describes how the beam and its
+        particles are transformed when travelling through the element.
+        The state vector is consisting of 6 values with a physical meaning:
+            x: Position in x direction
+            xp: Momentum in x direction
+            y: Position in y direction
+            yp: Momentum in y direction
+            s: Position in z direction, the zero value is set to the middle of the pulse
+            sp: Momentum in s direction
+        As well as a seventh value used to add constants to some of the prior values if
+        necesassary. Through this seventh state, the addition of constants can be
+        represented using a matrix multiplication.
+
+        Parameters
+        ----------
+        energy: cheetah.Beam.energy
+            Energy of the Beam. Read from the fed in Cheetah Beam.
+
+        Returns
+        --------
+        R
+            A 7x7 Matrix for further calculations.
+
+        Raises
+        -------
+        NotImplementedError
+            If no transfer_map function is implemented for the given `Element` subclass.
+        """
         raise NotImplementedError
 
-    def __call__(self, incoming):
+    def __call__(self, incoming: Beam) -> Beam:
         """
-        Track particles through the element.
+        Track particles through the element. The input can be a `ParameterBeam` or a
+        `ParticleBeam`.
 
-        Pramameters
+        Parameters
         -----------
         incoming : cheetah.Beam
             Beam of particles entering the element.
 
         Returns
         -------
         cheetah.Beam
@@ -76,23 +121,27 @@
         """
         if incoming is Beam.empty:
             return incoming
         elif isinstance(incoming, ParameterBeam):
             tm = self.transfer_map(incoming.energy)
             mu = torch.matmul(tm, incoming._mu)
             cov = torch.matmul(tm, torch.matmul(incoming._cov, tm.t()))
+            if self.device != "cpu":
+                raise DeviceError
             return ParameterBeam(mu, cov, incoming.energy)
         elif isinstance(incoming, ParticleBeam):
             tm = self.transfer_map(incoming.energy)
             new_particles = torch.matmul(incoming.particles, tm.t())
+            if self.device != incoming.device:
+                raise DeviceError
             return ParticleBeam(new_particles, incoming.energy, device=incoming.device)
         else:
             raise TypeError(f"Parameter incoming is of invalid type {type(incoming)}")
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list["Element"]:
         """
         Split the element into slices no longer than `resolution`.
 
         Parameters
         ----------
         resolution : float
             Length of the longest allowed split in meters.
@@ -101,67 +150,66 @@
         -------
         list
             Ordered sequence of sliced elements.
 
         Raises
         ------
         NotImplementedError
-            If not split function is implemented for the given `Element` subclass.
+            If no split function is implemented for the given `Element` subclass.
         """
         raise NotImplementedError
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         """
         Plot a representation of this element into a `matplotlib` Axes at position `s`.
 
         Parameters
         ----------
         ax : matplotlib.axes.Axes
             Axes to plot the representation into.
         s : float
             Position of the object along s in meters.
 
         Raises
         ------
         NotImplementedError
-            If not split function is implemented for the given `Element` subclass.
+            If no plot function is implemented for the given `Element` subclass.
         """
         raise NotImplementedError
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'{self.__class__.__name__}(name="{self.name}")'
 
 
 class Drift(Element):
     """
     Drift section in a particle accelerator.
 
     Parameters
     ----------
     length : float
         Length in meters.
-    energy : float, optional
     name : string, optional
         Unique identifier of the element.
 
     Attributes
     ---------
     is_active : bool
         Drifts are always set as active.
     """
 
     is_active = True
     is_skippable = True
 
-    def __init__(self, length, name=None, **kwargs):
+    def __init__(self, length: float, name: Optional[str] = None, **kwargs) -> None:
         self.length = length
 
         super().__init__(name=name, **kwargs)
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
         gamma = energy / REST_ENERGY
         igamma2 = 1 / gamma**2 if gamma != 0 else 0
 
         return torch.tensor(
             [
                 [1, self.length, 0, 0, 0, 0, 0],
                 [0, 1, 0, 0, 0, 0, 0],
@@ -171,27 +219,27 @@
                 [0, 0, 0, 0, 0, 1, 0],
                 [0, 0, 0, 0, 0, 0, 1],
             ],
             dtype=torch.float32,
             device=self.device,
         )
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list[Element]:
         split_elements = []
         remaining = self.length
         while remaining > 0:
             element = Drift(min(resolution, remaining), device=self.device)
             split_elements.append(element)
             remaining -= resolution
         return split_elements
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         pass
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f'{self.__class__.__name__}(length={self.length:.2f}, name="{self.name}")'
         )
 
 
 class Quadrupole(Element):
     """
@@ -201,34 +249,40 @@
     ----------
     length : float
         Length in meters.
     k1 : float, optional
         Strength of the quadrupole in rad/m.
     misalignment : (float, float), optional
         Misalignment vector of the quadrupole in x- and y-directions.
-    energy : float, optional
     name : string, optional
         Unique identifier of the element.
 
     Attributes
     ---------
     is_active : bool
         Is set `True` when `k1 != 0`.
     """
 
     is_skippable = True
 
-    def __init__(self, length, k1=0.0, misalignment=(0, 0), name=None, **kwargs):
+    def __init__(
+        self,
+        length: float,
+        k1: float = 0.0,
+        misalignment: tuple[float, float] = (0, 0),
+        name: Optional[str] = None,
+        **kwargs,
+    ) -> None:
         self.length = length
         self.k1 = k1
         self.misalignment = misalignment
 
         super().__init__(name=name, **kwargs)
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
         gamma = energy / REST_ENERGY
         igamma2 = 1 / gamma**2 if gamma != 0 else 0
 
         beta = np.sqrt(1 - igamma2)
 
         hx = 0
         kx2 = self.k1 + hx**2
@@ -293,40 +347,40 @@
                 dtype=torch.float32,
                 device=self.device,
             )
             R = torch.matmul(R_exit, torch.matmul(R, R_entry))
             return R
 
     @property
-    def is_active(self):
+    def is_active(self) -> bool:
         return self.k1 != 0
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list[Element]:
         split_elements = []
         remaining = self.length
         while remaining > 0:
             element = Quadrupole(
                 min(resolution, remaining),
                 self.k1,
                 misalignment=self.misalignment,
                 device=self.device,
             )
             split_elements.append(element)
             remaining -= resolution
         return split_elements
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         alpha = 1 if self.is_active else 0.2
         height = 0.8 * (np.sign(self.k1) if self.is_active else 1)
         patch = Rectangle(
             (s, 0), self.length, height, color="tab:red", alpha=alpha, zorder=2
         )
         ax.add_patch(patch)
 
-    def __repr__(self):
+    def __repr__(self) -> None:
         return (
             f"{self.__class__.__name__}(length={self.length:.2f}, "
             + f"k1={self.k1}, "
             + f"misalignment={self.misalignment}, "
             + f'name="{self.name}")'
         )
 
@@ -337,33 +391,34 @@
 
     Parameters
     ----------
     length : float
         Length in meters.
     angle : float, optional
         Particle deflection angle in the horizontal plane in rad.
-    energy : float, optional
     name : string, optional
         Unique identifier of the element.
 
     Attributes
     ---------
     is_active : bool
         Is set `True` when `angle != 0`.
     """
 
     is_skippable = True
 
-    def __init__(self, length, angle=0.0, name=None, **kwargs):
+    def __init__(
+        self, length: float, angle: float = 0.0, name: Optional[str] = None, **kwargs
+    ) -> None:
         self.length = length
         self.angle = angle
 
         super().__init__(name=name, **kwargs)
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
         return torch.tensor(
             [
                 [1, self.length, 0, 0, 0, 0, 0],
                 [0, 1, 0, 0, 0, 0, self.angle],
                 [0, 0, 1, self.length, 0, 0, 0],
                 [0, 0, 0, 1, 0, 0, 0],
                 [0, 0, 0, 0, 1, 0, 0],
@@ -371,39 +426,39 @@
                 [0, 0, 0, 0, 0, 0, 1],
             ],
             dtype=torch.float32,
             device=self.device,
         )
 
     @property
-    def is_active(self):
+    def is_active(self) -> bool:
         return self.angle != 0
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list[Element]:
         split_elements = []
         remaining = self.length
         while remaining > 0:
             length = min(resolution, remaining)
             element = HorizontalCorrector(
                 length, self.angle * length / self.length, device=self.device
             )
             split_elements.append(element)
             remaining -= resolution
         return split_elements
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         alpha = 1 if self.is_active else 0.2
         height = 0.8 * (np.sign(self.angle) if self.is_active else 1)
 
         patch = Rectangle(
             (s, 0), self.length, height, color="tab:blue", alpha=alpha, zorder=2
         )
         ax.add_patch(patch)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(length={self.length:.2f}, "
             + f"angle={self.angle}, "
             + f'name="{self.name}")'
         )
 
 
@@ -413,33 +468,34 @@
 
     Parameters
     ----------
     length : float
         Length in meters.
     angle : float, optional
         Particle deflection angle in the vertical plane in rad.
-    energy : float, optional
     name : string, optional
         Unique identifier of the element.
 
     Attributes
     ---------
     is_active : bool
         Is set `True` when `angle != 0`.
     """
 
     is_skippable = True
 
-    def __init__(self, length, angle=0.0, name=None, **kwargs):
+    def __init__(
+        self, length: float, angle: float = 0.0, name: Optional[str] = None, **kwargs
+    ) -> None:
         self.length = length
         self.angle = angle
 
         super().__init__(name=name, **kwargs)
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
         return torch.tensor(
             [
                 [1, self.length, 0, 0, 0, 0, 0],
                 [0, 1, 0, 0, 0, 0, 0],
                 [0, 0, 1, self.length, 0, 0, 0],
                 [0, 0, 0, 1, 0, 0, self.angle],
                 [0, 0, 0, 0, 1, 0, 0],
@@ -447,39 +503,39 @@
                 [0, 0, 0, 0, 0, 0, 1],
             ],
             dtype=torch.float32,
             device=self.device,
         )
 
     @property
-    def is_active(self):
+    def is_active(self) -> bool:
         return self.angle != 0
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list[Element]:
         split_elements = []
         remaining = self.length
         while remaining > 0:
             length = min(resolution, remaining)
             element = VerticalCorrector(
                 length, self.angle * length / self.length, device=self.device
             )
             split_elements.append(element)
             remaining -= resolution
         return split_elements
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         alpha = 1 if self.is_active else 0.2
         height = 0.8 * (np.sign(self.angle) if self.is_active else 1)
 
         patch = Rectangle(
             (s, 0), self.length, height, color="tab:cyan", alpha=alpha, zorder=2
         )
         ax.add_patch(patch)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(length={self.length:.2f}, "
             + f"angle={self.angle}, "
             + f'name="{self.name}")'
         )
 
 
@@ -493,29 +549,35 @@
         Length in meters.
     delta_energy : float, optional
         Energy added to the beam by the accelerating cavity.
     name : string, optional
         Unique identifier of the element.
     """
 
-    def __init__(self, length, delta_energy=0, name=None, **kwargs):
+    def __init__(
+        self,
+        length: float,
+        delta_energy: float = 0,
+        name: Optional[str] = None,
+        **kwargs,
+    ) -> None:
         self.length = length
         self.delta_energy = delta_energy
 
         super().__init__(name=name, **kwargs)
 
     @property
-    def is_active(self):
+    def is_active(self) -> bool:
         return self.delta_energy != 0
 
     @property
-    def is_skippable(self):
+    def is_skippable(self) -> bool:
         return not self.is_active
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
         gamma = energy / REST_ENERGY
         igamma2 = 1 / gamma**2 if gamma != 0 else 0
 
         return torch.tensor(
             [
                 [1, self.length, 0, 0, 0, 0, 0],
                 [0, 1, 0, 0, 0, 0, 0],
@@ -525,43 +587,43 @@
                 [0, 0, 0, 0, 0, 1, 0],
                 [0, 0, 0, 0, 0, 0, 1],
             ],
             dtype=torch.float32,
             device=self.device,
         )
 
-    def __call__(self, incoming):
+    def __call__(self, incoming: Beam) -> Beam:
         outgoing = super().__call__(incoming)
         if outgoing is not Beam.empty:
             outgoing.energy += self.delta_energy
         return outgoing
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list[Element]:
         split_elements = []
         remaining = self.length
         while remaining > 0:
             split_length = min(resolution, remaining)
             split_delta_energy = self.delta_energy * split_length / self.length
             element = Cavity(
                 split_length, delta_energy=split_delta_energy, device=self.device
             )
             split_elements.append(element)
             remaining -= resolution
         return split_elements
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         alpha = 1 if self.is_active else 0.2
         height = 0.4
 
         patch = Rectangle(
             (s, 0), self.length, height, color="gold", alpha=alpha, zorder=2
         )
         ax.add_patch(patch)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(length={self.length:.2f},"
             f' delta_energy={self.delta_energy}, name="{self.name}")'
         )
 
 
 class BPM(Element):
@@ -586,32 +648,37 @@
 
     length = 0
     is_skippable = True  # TODO: Temporary
 
     reading = (None, None)
 
     @property
-    def is_skippable(self):
+    def is_skippable(self) -> bool:
         return not self.is_active
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
         return torch.eye(7, device=self.device)
 
-    def __call__(self, incoming):
+    def __call__(self, incoming: Beam) -> Beam:
         if incoming is Beam.empty:
             self.reading = (None, None)
             return Beam.empty
-        else:
+        elif isinstance(incoming, ParameterBeam):
+            self.reading = (incoming.mu_x, incoming.mu_y)
+            return ParameterBeam(incoming._mu, incoming._cov, incoming.energy)
+        elif isinstance(incoming, ParticleBeam):
             self.reading = (incoming.mu_x, incoming.mu_y)
             return ParticleBeam(incoming.particles, incoming.energy, device=self.device)
+        else:
+            raise TypeError(f"Parameter incoming is of invalid type {type(incoming)}")
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list[Element]:
         return [self]
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         alpha = 1 if self.is_active else 0.2
         patch = Rectangle(
             (s, -0.3), 0, 0.3 * 2, color="darkkhaki", alpha=alpha, zorder=2
         )
         ax.add_patch(patch)
 
 
@@ -636,74 +703,74 @@
         particles when a beam is tracked through it.
     """
 
     length = 0
 
     def __init__(
         self,
-        resolution,
-        pixel_size,
-        binning=1,
-        misalignment=(0, 0),
-        name=None,
+        resolution: tuple[int, int],
+        pixel_size: tuple[float, float],
+        binning: int = 1,
+        misalignment: tuple[float, float] = (0, 0),
+        name: Optional[str] = None,
         **kwargs,
-    ):
+    ) -> None:
         super().__init__(name=name, **kwargs)
 
         self.resolution = resolution
         self.pixel_size = pixel_size
         self.binning = binning
         self.misalignment = misalignment
 
         self.read_beam = None
         self.cached_reading = None
 
     @property
-    def is_skippable(self):
+    def is_skippable(self) -> bool:
         return not self.is_active
 
     @property
-    def effective_resolution(self):
+    def effective_resolution(self) -> tuple[int, int]:
         return (
             int(self.resolution[0] / self.binning),
             int(self.resolution[1] / self.binning),
         )
 
     @property
-    def effective_pixel_size(self):
+    def effective_pixel_size(self) -> tuple[float, float]:
         return (self.pixel_size[0] * self.binning, self.pixel_size[0] * self.binning)
 
     @property
-    def extent(self):
+    def extent(self) -> tuple[float, float, float, float]:
         return (
             -self.resolution[0] * self.pixel_size[0] / 2,
             self.resolution[0] * self.pixel_size[0] / 2,
             -self.resolution[1] * self.pixel_size[1] / 2,
             self.resolution[1] * self.pixel_size[1] / 2,
         )
 
     @property
-    def pixel_bin_edges(self):
+    def pixel_bin_edges(self) -> tuple[torch.Tensor, torch.Tensor]:
         return (
             torch.linspace(
                 -self.resolution[0] * self.pixel_size[0] / 2,
                 self.resolution[0] * self.pixel_size[0] / 2,
                 self.effective_resolution[0] + 1,
             ),
             torch.linspace(
                 -self.resolution[1] * self.pixel_size[1] / 2,
                 self.resolution[1] * self.pixel_size[1] / 2,
                 self.effective_resolution[1] + 1,
             ),
         )
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
         return torch.eye(7, device=self.device)
 
-    def __call__(self, incoming):
+    def __call__(self, incoming: Beam) -> Beam:
         if self.is_active:
             if isinstance(incoming, ParameterBeam):
                 self.read_beam = deepcopy(incoming)
                 self.read_beam._mu[0] -= self.misalignment[0]
                 self.read_beam._mu[2] -= self.misalignment[1]
             elif isinstance(incoming, ParticleBeam):
                 self.read_beam = deepcopy(incoming)
@@ -715,15 +782,15 @@
                 self.read_beam = incoming
 
             return Beam.empty
         else:
             return incoming
 
     @property
-    def reading(self):
+    def reading(self) -> torch.Tensor:
         if self.cached_reading is not None:
             return self.cached_reading
 
         if self.read_beam is Beam.empty or self.read_beam is None:
             image = torch.zeros(
                 (self.effective_resolution[1], self.effective_resolution[0])
             )
@@ -747,45 +814,45 @@
             vstep = self.pixel_size[1] * self.binning
             x, y = np.mgrid[left:right:hstep, bottom:top:vstep]
             pos = np.dstack((x, y))
             image = dist.pdf(pos)
             image = np.flipud(image.T)
         elif isinstance(self.read_beam, ParticleBeam):
             image, _ = torch.histogramdd(
-                torch.stack((self.read_beam.xs, self.read_beam.ys)),
+                torch.stack((self.read_beam.xs, self.read_beam.ys)).T,
                 bins=self.pixel_bin_edges,
             )
             image = torch.flipud(image.T)
             image = image.cpu()
         else:
             raise TypeError(f"Read beam is of invalid type {type(self.read_beam)}")
 
         self.cached_reading = image
         return image
 
     @property
-    def read_beam(self):
+    def read_beam(self) -> Beam:
         return self._read_beam
 
     @read_beam.setter
-    def read_beam(self, value):
+    def read_beam(self, value: Beam) -> None:
         self._read_beam = value
         self.cached_reading = None
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list[Element]:
         return [self]
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         alpha = 1 if self.is_active else 0.2
         patch = Rectangle(
             (s, -0.6), 0, 0.6 * 2, color="tab:green", alpha=alpha, zorder=2
         )
         ax.add_patch(patch)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(resolution={self.resolution},"
             f" pixel_size={self.pixel_size}, binning={self.binning},"
             f' misalignment={self.misalignment}, name="{self.name}")'
         )
 
 
@@ -803,20 +870,20 @@
     Notes
     -----
     Currently behaves like a drift section but is plotted distinctively.
     """
 
     is_skippable = True  # TODO: Temporary?
 
-    def __init__(self, length, name=None, **kwargs):
+    def __init__(self, length: float, name: Optional[str] = None, **kwargs) -> None:
         self.length = length
 
         super().__init__(name=name, **kwargs)
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
         gamma = energy / REST_ENERGY
         igamma2 = 1 / gamma**2 if gamma != 0 else 0
 
         return torch.tensor(
             [
                 [1, self.length, 0, 0, 0, 0, 0],
                 [0, 1, 0, 0, 0, 0, 0],
@@ -826,33 +893,33 @@
                 [0, 0, 0, 0, 0, 1, 0],
                 [0, 0, 0, 0, 0, 0, 1],
             ],
             dtype=torch.float32,
             device=self.device,
         )
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list[Element]:
         split_elements = []
         remaining = self.length
         while remaining > 0:
             element = Cavity(min(resolution, remaining), device=self.device)
             split_elements.append(element)
             remaining -= resolution
         return split_elements
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         alpha = 1 if self.is_active else 0.2
         height = 0.4
 
         patch = Rectangle(
             (s, 0), self.length, height, color="tab:purple", alpha=alpha, zorder=2
         )
         ax.add_patch(patch)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f'{self.__class__.__name__}(length={self.length:.2f}, name="{self.name}")'
         )
 
 
 class Segment(Element):
     """
@@ -862,62 +929,66 @@
     ----------
     cell : list
         List of Cheetah elements that describe an accelerator (section).
     name : string, optional
         Unique identifier of the element.
     """
 
-    def __init__(self, cell, name=None, **kwargs):
+    def __init__(
+        self, cell: list[Element], name: Optional[str] = None, **kwargs
+    ) -> None:
         super().__init__(name=name, **kwargs)
 
         self.elements = cell
 
         for element in self.elements:
             element.device = self.device
             self.__dict__[element.name] = element
 
-    def subcell(self, start, end, **kwargs):
+    def subcell(self, start: str, end: str, **kwargs) -> "Segment":
         """Extract a subcell `[start, end]` from an this segment."""
         subcell = []
         is_in_subcell = False
         for element in self.elements:
             if element.name == start:
                 is_in_subcell = True
             if is_in_subcell:
                 subcell.append(element)
             if element.name == end:
                 break
 
         return self.__class__(subcell, device=self.device, **kwargs)
 
     @classmethod
-    def from_ocelot(cls, cell, name=None, warnings=True, **kwargs):
+    def from_ocelot(
+        cls, cell, name: Optional[str] = None, warnings: bool = True, **kwargs
+    ) -> "Segment":
         converted = [
             utils.ocelot2cheetah(element, warnings=warnings) for element in cell
         ]
         return cls(converted, name=name, **kwargs)
 
     @property
-    def is_skippable(self):
+    def is_skippable(self) -> bool:
         return all(element.is_skippable for element in self.elements)
 
     @property
-    def length(self):
+    def length(self) -> float:
         return sum(element.length for element in self.elements)
 
-    def transfer_map(self, energy):
+    def transfer_map(self, energy: float) -> torch.Tensor:
         if self.is_skippable:
             tm = torch.eye(7, dtype=torch.float32, device=self.device)
             for element in self.elements:
                 tm = torch.matmul(element.transfer_map(energy), tm)
             return tm
         else:
             return None
 
-    def __call__(self, incoming):
+    def __call__(self, incoming: Beam) -> Beam:
         if self.is_skippable:
             return super().__call__(incoming)
         else:
             todos = []
             for element in self.elements:
                 if not element.is_skippable:
                     todos.append(element)
@@ -927,22 +998,22 @@
                     todos[-1].elements.append(element)
 
             for todo in todos:
                 incoming = todo(incoming)
 
             return incoming
 
-    def split(self, resolution):
+    def split(self, resolution: float) -> list[Element]:
         return [
             split_element
             for element in self.elements
             for split_element in element.split(resolution)
         ]
 
-    def plot(self, ax, s):
+    def plot(self, ax: matplotlib.axes.Axes, s: float) -> None:
         element_lengths = [element.length for element in self.elements]
         element_ss = [0] + [
             sum(element_lengths[: i + 1]) for i, _ in enumerate(element_lengths)
         ]
         element_ss = [s + element_s for element_s in element_ss]
 
         ax.plot([0, element_ss[-1]], [0, 0], "--", color="black")
@@ -952,16 +1023,21 @@
 
         ax.set_ylim(-1, 1)
         ax.set_xlabel("s (m)")
         ax.set_yticks([])
         ax.grid()
 
     def plot_reference_particle_traces(
-        self, axx, axy, beam=None, n=10, resolution=0.01
-    ):
+        self,
+        axx: matplotlib.axes.Axes,
+        axy: matplotlib.axes.Axes,
+        beam: Optional[Beam] = None,
+        n: int = 10,
+        resolution: float = 0.01,
+    ) -> None:
         """
         Plot `n` reference particles along the segment view in x- and y-direction.
 
         Parameters
         ----------
         axx : matplotlib.axes.Axes
             Axes to plot the particle traces into viewed in x-direction.
@@ -1024,15 +1100,21 @@
                 if reference_beam is not Beam.empty
             ]
             axy.plot(ss[: len(ys)], ys)
         axx.set_xlabel("s (m)")
         axy.set_ylabel("y (m)")
         axy.grid()
 
-    def plot_overview(self, fig=None, beam=None, n=10, resolution=0.01):
+    def plot_overview(
+        self,
+        fig: Optional[matplotlib.figure.Figure] = None,
+        beam: Optional[Beam] = None,
+        n: int = 10,
+        resolution: float = 0.01,
+    ) -> None:
         """
         Plot an overview of the segment with the lattice and traced reference particles.
 
         Parameters
         ----------
         fig: matplotlib.figure.Figure, optional
             Figure to plot the overview into.
@@ -1052,15 +1134,15 @@
         axs[0].set_title("Reference Particle Traces")
         self.plot_reference_particle_traces(axs[0], axs[1], beam, n, resolution)
 
         self.plot(axs[2], 0)
 
         plt.tight_layout()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         start = f"{self.__class__.__name__}(["
 
         s = start + self.elements[0].__repr__()
         x = [", " + element.__repr__() for element in self.elements[1:]]
         s += "".join(x)
         s += "])"
```

### Comparing `cheetah-accelerator-0.5.18/cheetah/particles.py` & `cheetah-accelerator-0.5.19/cheetah/particles.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+from typing import Optional
+
 import numpy as np
 import torch
 from torch.distributions import MultivariateNormal
 
 from cheetah.utils import from_astrabeam
 
 
 class Beam:
     empty = "I'm an empty beam!"
 
     @classmethod
     def from_parameters(
         cls,
-        mu_x=0,
-        mu_xp=0,
-        mu_y=0,
-        mu_yp=0,
-        sigma_x=175e-9,
-        sigma_xp=2e-7,
-        sigma_y=175e-9,
-        sigma_yp=2e-7,
-        sigma_s=1e-6,
-        sigma_p=1e-6,
-        cor_x=0,
-        cor_y=0,
-        cor_s=0,
-        energy=1e8,
-    ):
+        mu_x: float = 0,
+        mu_xp: float = 0,
+        mu_y: float = 0,
+        mu_yp: float = 0,
+        sigma_x: float = 1,
+        sigma_xp: float = 0,
+        sigma_y: float = 1,
+        sigma_yp: float = 0,
+        sigma_s: float = 0,
+        sigma_p: float = 0,
+        cor_x: float = 0,
+        cor_y: float = 0,
+        cor_s: float = 0,
+        energy: float = 1e8,
+    ) -> "Beam":
         """
         Create beam that with given beam parameters.
 
         Parameters
         ----------
         n : int, optional
             Number of particles to generate.
@@ -38,56 +40,56 @@
         mu_xp : float, optional
             Center of the particle distribution on px in meters.
         mu_y : float, optional
             Center of the particle distribution on y in meters.
         mu_yp : float, optional
             Center of the particle distribution on py in meters.
         sigma_x : float, optional
-            Sgima of the particle distribution in x direction in meters.
+            Sigma of the particle distribution in x direction in meters.
         sigma_xp : float, optional
-            Sgima of the particle distribution in px direction in meters.
+            Sigma of the particle distribution in px direction in meters.
         sigma_y : float, optional
-            Sgima of the particle distribution in y direction in meters.
+            Sigma of the particle distribution in y direction in meters.
         sigma_yp : float, optional
-            Sgima of the particle distribution in py direction in meters.
+            Sigma of the particle distribution in py direction in meters.
         sigma_s : float, optional
-            Sgima of the particle distribution in s direction in meters.
+            Sigma of the particle distribution in s direction in meters.
         sigma_p : float, optional
-            Sgima of the particle distribution in p direction in meters.
+            Sigma of the particle distribution in p direction in meters.
         energy : float, optional
             Energy of the beam in eV.
         """
         raise NotImplementedError
 
     @classmethod
-    def from_ocelot(cls, parray):
+    def from_ocelot(cls, parray) -> "Beam":
         """
         Convert an Ocelot ParticleArray `parray` to a Cheetah Beam.
         """
         raise NotImplementedError
 
     @classmethod
-    def from_astra(cls, path, **kwargs):
+    def from_astra(cls, path: str, **kwargs) -> "Beam":
         """Load an Astra particle distribution as a Cheetah Beam."""
         raise NotImplementedError
 
     def transformed_to(
         self,
-        mu_x=None,
-        mu_xp=None,
-        mu_y=None,
-        mu_yp=None,
-        sigma_x=None,
-        sigma_xp=None,
-        sigma_y=None,
-        sigma_yp=None,
-        sigma_s=None,
-        sigma_p=None,
-        energy=None,
-    ):
+        mu_x: Optional[float] = None,
+        mu_xp: Optional[float] = None,
+        mu_y: Optional[float] = None,
+        mu_yp: Optional[float] = None,
+        sigma_x: Optional[float] = None,
+        sigma_xp: Optional[float] = None,
+        sigma_y: Optional[float] = None,
+        sigma_yp: Optional[float] = None,
+        sigma_s: Optional[float] = None,
+        sigma_p: Optional[float] = None,
+        energy: Optional[float] = None,
+    ) -> "Beam":
         """
         Create version of this beam that is transformed to new beam parameters.
 
         Parameters
         ----------
         n : int, optional
             Number of particles to generate.
@@ -96,25 +98,25 @@
         mu_xp : float, optional
             Center of the particle distribution on px in meters.
         mu_y : float, optional
             Center of the particle distribution on y in meters.
         mu_yp : float, optional
             Center of the particle distribution on py in meters.
         sigma_x : float, optional
-            Sgima of the particle distribution in x direction in meters.
+            Sigma of the particle distribution in x direction in meters.
         sigma_xp : float, optional
-            Sgima of the particle distribution in px direction in meters.
+            Sigma of the particle distribution in px direction in meters.
         sigma_y : float, optional
-            Sgima of the particle distribution in y direction in meters.
+            Sigma of the particle distribution in y direction in meters.
         sigma_yp : float, optional
-            Sgima of the particle distribution in py direction in meters.
+            Sigma of the particle distribution in py direction in meters.
         sigma_s : float, optional
-            Sgima of the particle distribution in s direction in meters.
+            Sigma of the particle distribution in s direction in meters.
         sigma_p : float, optional
-            Sgima of the particle distribution in p direction in meters.
+            Sigma of the particle distribution in p direction in meters.
         energy : float, optional
             Energy of the beam in eV.
         """
         mu_x = mu_x if mu_x is not None else self.mu_x
         mu_xp = mu_xp if mu_xp is not None else self.mu_xp
         mu_y = mu_y if mu_y is not None else self.mu_y
         mu_yp = mu_yp if mu_yp is not None else self.mu_yp
@@ -137,15 +139,15 @@
             sigma_yp=sigma_yp,
             sigma_s=sigma_s,
             sigma_p=sigma_p,
             energy=energy,
         )
 
     @property
-    def parameters(self):
+    def parameters(self) -> dict[str, float]:
         return {
             "mu_x": self.mu_x,
             "mu_xp": self.mu_xp,
             "mu_y": self.mu_y,
             "mu_yp": self.mu_yp,
             "sigma_x": self.sigma_x,
             "sigma_xp": self.sigma_xp,
@@ -153,62 +155,62 @@
             "sigma_yp": self.sigma_yp,
             "sigma_s": self.sigma_s,
             "sigma_p": self.sigma_p,
             "energy": self.energy,
         }
 
     @property
-    def mu_x(self):
+    def mu_x(self) -> float:
         raise NotImplementedError
 
     @property
-    def sigma_x(self):
+    def sigma_x(self) -> float:
         raise NotImplementedError
 
     @property
-    def mu_xp(self):
+    def mu_xp(self) -> float:
         raise NotImplementedError
 
     @property
-    def sigma_xp(self):
+    def sigma_xp(self) -> float:
         raise NotImplementedError
 
     @property
-    def mu_y(self):
+    def mu_y(self) -> float:
         raise NotImplementedError
 
     @property
-    def sigma_y(self):
+    def sigma_y(self) -> float:
         raise NotImplementedError
 
     @property
-    def mu_yp(self):
+    def mu_yp(self) -> float:
         raise NotImplementedError
 
     @property
-    def sigma_yp(self):
+    def sigma_yp(self) -> float:
         raise NotImplementedError
 
     @property
-    def mu_s(self):
+    def mu_s(self) -> float:
         raise NotImplementedError
 
     @property
-    def sigma_s(self):
+    def sigma_s(self) -> float:
         raise NotImplementedError
 
     @property
-    def mu_p(self):
+    def mu_p(self) -> float:
         raise NotImplementedError
 
     @property
-    def sigma_p(self):
+    def sigma_p(self) -> float:
         raise NotImplementedError
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(mu_x={self.mu_x}, mu_xp={self.mu_xp},"
             f" mu_y={self.mu_y}, mu_yp={self.mu_yp}, sigma_x={self.sigma_x},"
             f" sigma_xp={self.sigma_xp}, sigma_y={self.sigma_y},"
             f" sigma_yp={self.sigma_yp}, sigma_s={self.sigma_s},"
             f" sigma_p={self.sigma_p}, energy={self.energy})"
         )
@@ -224,37 +226,37 @@
         Mu vector of the beam.
     cov : torch.Tensor
         Covariance matrix of the beam.
     energy : float
         Energy of the beam in eV.
     """
 
-    def __init__(self, mu, cov, energy):
+    def __init__(self, mu: torch.Tensor, cov: torch.Tensor, energy: float) -> None:
         self._mu = mu
         self._cov = cov
         self.energy = energy
 
     @classmethod
     def from_parameters(
         cls,
-        mu_x=0,
-        mu_xp=0,
-        mu_y=0,
-        mu_yp=0,
-        sigma_x=175e-9,
-        sigma_xp=2e-7,
-        sigma_y=175e-9,
-        sigma_yp=2e-7,
-        sigma_s=1e-6,
-        sigma_p=1e-6,
-        cor_x=0,
-        cor_y=0,
-        cor_s=0,
-        energy=1e8,
-    ):
+        mu_x: float = 0,
+        mu_xp: float = 0,
+        mu_y: float = 0,
+        mu_yp: float = 0,
+        sigma_x: float = 175e-9,
+        sigma_xp: float = 2e-7,
+        sigma_y: float = 175e-9,
+        sigma_yp: float = 2e-7,
+        sigma_s: float = 1e-6,
+        sigma_p: float = 1e-6,
+        cor_x: float = 0,
+        cor_y: float = 0,
+        cor_s: float = 0,
+        energy: float = 1e8,
+    ) -> "ParameterBeam":
         return cls(
             mu=torch.tensor([mu_x, mu_xp, mu_y, mu_yp, 0, 0, 1], dtype=torch.float32),
             cov=torch.tensor(
                 [
                     [sigma_x**2, cor_x, 0, 0, 0, 0, 0],
                     [cor_x, sigma_xp**2, 0, 0, 0, 0, 0],
                     [0, 0, sigma_y**2, cor_y, 0, 0, 0],
@@ -265,51 +267,51 @@
                 ],
                 dtype=torch.float32,
             ),
             energy=energy,
         )
 
     @classmethod
-    def from_ocelot(cls, parray):
+    def from_ocelot(cls, parray) -> "ParameterBeam":
         mu = torch.ones(7)
         mu[:6] = torch.tensor(parray.rparticles.mean(axis=1), dtype=torch.float32)
 
         cov = torch.zeros(7, 7)
         cov[:6, :6] = torch.tensor(np.cov(parray.rparticles), dtype=torch.float32)
 
         energy = 1e9 * parray.E
 
         return cls(mu=mu, cov=cov, energy=energy)
 
     @classmethod
-    def from_astra(cls, path, **kwargs):
+    def from_astra(cls, path: str, **kwargs) -> "ParameterBeam":
         """Load an Astra particle distribution as a Cheetah Beam."""
         particles, energy = from_astrabeam(path)
         mu = torch.ones(7)
         mu[:6] = torch.tensor(particles.mean(axis=0), dtype=torch.float32)
 
         cov = torch.zeros(7, 7)
         cov[:6, :6] = torch.tensor(np.cov(particles.transpose()), dtype=torch.float32)
 
         return cls(mu=mu, cov=cov, energy=energy)
 
     def transformed_to(
         self,
-        mu_x=None,
-        mu_xp=None,
-        mu_y=None,
-        mu_yp=None,
-        sigma_x=None,
-        sigma_xp=None,
-        sigma_y=None,
-        sigma_yp=None,
-        sigma_s=None,
-        sigma_p=None,
-        energy=None,
-    ):
+        mu_x: Optional[float] = None,
+        mu_xp: Optional[float] = None,
+        mu_y: Optional[float] = None,
+        mu_yp: Optional[float] = None,
+        sigma_x: Optional[float] = None,
+        sigma_xp: Optional[float] = None,
+        sigma_y: Optional[float] = None,
+        sigma_yp: Optional[float] = None,
+        sigma_s: Optional[float] = None,
+        sigma_p: Optional[float] = None,
+        energy: Optional[float] = None,
+    ) -> "ParameterBeam":
         """
         Create version of this beam that is transformed to new beam parameters.
 
         Parameters
         ----------
         n : int, optional
             Number of particles to generate.
@@ -318,25 +320,25 @@
         mu_xp : float, optional
             Center of the particle distribution on px in meters.
         mu_y : float, optional
             Center of the particle distribution on y in meters.
         mu_yp : float, optional
             Center of the particle distribution on py in meters.
         sigma_x : float, optional
-            Sgima of the particle distribution in x direction in meters.
+            Sigma of the particle distribution in x direction in meters.
         sigma_xp : float, optional
-            Sgima of the particle distribution in px direction in meters.
+            Sigma of the particle distribution in px direction in meters.
         sigma_y : float, optional
-            Sgima of the particle distribution in y direction in meters.
+            Sigma of the particle distribution in y direction in meters.
         sigma_yp : float, optional
-            Sgima of the particle distribution in py direction in meters.
+            Sigma of the particle distribution in py direction in meters.
         sigma_s : float, optional
-            Sgima of the particle distribution in s direction in meters.
+            Sigma of the particle distribution in s direction in meters.
         sigma_p : float, optional
-            Sgima of the particle distribution in p direction in meters.
+            Sigma of the particle distribution in p direction in meters.
         energy : float, optional
             Energy of the beam in eV.
         """
         mu_x = mu_x if mu_x is not None else self.mu_x
         mu_xp = mu_xp if mu_xp is not None else self.mu_xp
         mu_y = mu_y if mu_y is not None else self.mu_y
         mu_yp = mu_yp if mu_yp is not None else self.mu_yp
@@ -359,62 +361,62 @@
             sigma_yp=sigma_yp,
             sigma_s=sigma_s,
             sigma_p=sigma_p,
             energy=energy,
         )
 
     @property
-    def mu_x(self):
+    def mu_x(self) -> float:
         return self._mu[0]
 
     @property
-    def sigma_x(self):
+    def sigma_x(self) -> float:
         return torch.sqrt(self._cov[0, 0])
 
     @property
-    def mu_xp(self):
+    def mu_xp(self) -> float:
         return self._mu[1]
 
     @property
-    def sigma_xp(self):
+    def sigma_xp(self) -> float:
         return torch.sqrt(self._cov[1, 1])
 
     @property
-    def mu_y(self):
+    def mu_y(self) -> float:
         return self._mu[2]
 
     @property
-    def sigma_y(self):
+    def sigma_y(self) -> float:
         return torch.sqrt(self._cov[2, 2])
 
     @property
-    def mu_yp(self):
+    def mu_yp(self) -> float:
         return self._mu[3]
 
     @property
-    def sigma_yp(self):
+    def sigma_yp(self) -> float:
         return torch.sqrt(self._cov[3, 3])
 
     @property
-    def mu_s(self):
+    def mu_s(self) -> float:
         return self._mu[4]
 
     @property
-    def sigma_s(self):
+    def sigma_s(self) -> float:
         return torch.sqrt(self._cov[4, 4])
 
     @property
-    def mu_p(self):
+    def mu_p(self) -> float:
         return self._mu[5]
 
     @property
-    def sigma_p(self):
+    def sigma_p(self) -> float:
         return torch.sqrt(self._cov[5, 5])
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(mu_x={self.mu_x:.6f}, mu_xp={self.mu_xp:.6f},"
             f" mu_y={self.mu_y:.6f}, mu_yp={self.mu_yp:.6f},"
             f" sigma_x={self.sigma_x:.6f}, sigma_xp={self.sigma_xp:.6f},"
             f" sigma_y={self.sigma_y:.6f}, sigma_yp={self.sigma_yp:.6f},"
             f" sigma_s={self.sigma_s:.6f}, sigma_p={self.sigma_p:.6f},"
             f" energy={self.energy:.3f})"
@@ -432,15 +434,17 @@
     energy : float
         Energy of the beam in eV.
     device : string
         Device to move the beam's particle array to. If set to `"auto"` a CUDA GPU is
         selected if available. The CPU is used otherwise.
     """
 
-    def __init__(self, particles, energy, device="auto"):
+    def __init__(
+        self, particles: torch.Tensor, energy: float, device: str = "auto"
+    ) -> None:
         assert (
             len(particles) > 0 and particles.shape[1] == 7
         ), "Particle vectors must be 7-dimensional."
 
         if device == "auto":
             device = "cuda" if torch.cuda.is_available() else "cpu"
         self.device = device
@@ -450,31 +454,31 @@
         )
 
         self.energy = energy
 
     @classmethod
     def from_parameters(
         cls,
-        n=100000,
-        mu_x=0,
-        mu_y=0,
-        mu_xp=0,
-        mu_yp=0,
-        sigma_x=175e-9,
-        sigma_y=175e-9,
-        sigma_xp=2e-7,
-        sigma_yp=2e-7,
-        sigma_s=1e-6,
-        sigma_p=1e-6,
-        cor_x=0,
-        cor_y=0,
-        cor_s=0,
-        energy=1e8,
-        device="auto",
-    ):
+        n: int = 100000,
+        mu_x: float = 0,
+        mu_y: float = 0,
+        mu_xp: float = 0,
+        mu_yp: float = 0,
+        sigma_x: float = 175e-9,
+        sigma_y: float = 175e-9,
+        sigma_xp: float = 2e-7,
+        sigma_yp: float = 2e-7,
+        sigma_s: float = 1e-6,
+        sigma_p: float = 1e-6,
+        cor_x: float = 0,
+        cor_y: float = 0,
+        cor_s: float = 0,
+        energy: float = 1e8,
+        device: str = "auto",
+    ) -> "ParticleBeam":
         """
         Generate Cheetah Beam of random particles.
 
         Parameters
         ----------
         n : int, optional
             Number of particles to generate.
@@ -483,25 +487,25 @@
         mu_y : float, optional
             Center of the particle distribution on y in meters.
         mu_xp : float, optional
             Center of the particle distribution on px in meters.
         mu_yp : float, optional
             Center of the particle distribution on py in meters.
         sigma_x : float, optional
-            Sgima of the particle distribution in x direction in meters.
+            Sigma of the particle distribution in x direction in meters.
         sigma_y : float, optional
-            Sgima of the particle distribution in y direction in meters.
+            Sigma of the particle distribution in y direction in meters.
         sigma_xp : float, optional
-            Sgima of the particle distribution in px direction in meters.
+            Sigma of the particle distribution in px direction in meters.
         sigma_yp : float, optional
-            Sgima of the particle distribution in py direction in meters.
+            Sigma of the particle distribution in py direction in meters.
         sigma_s : float, optional
-            Sgima of the particle distribution in s direction in meters.
+            Sigma of the particle distribution in s direction in meters.
         sigma_p : float, optional
-            Sgima of the particle distribution in p direction in meters.
+            Sigma of the particle distribution in p direction in meters.
         cor_x : float, optional
             Correlation between x and xp.
         cor_y : float, optional
             Correlation between y and yp.
         cor_s : float, optional
             Correlation between s and p.
         energy : float, optional
@@ -528,28 +532,28 @@
         particles[:, :6] = distribution.sample((n,))
 
         return cls(particles, energy, device=device)
 
     @classmethod
     def make_linspaced(
         cls,
-        n=10,
-        mu_x=0,
-        mu_y=0,
-        mu_xp=0,
-        mu_yp=0,
-        sigma_x=175e-9,
-        sigma_y=175e-9,
-        sigma_xp=2e-7,
-        sigma_yp=2e-7,
-        sigma_s=0,
-        sigma_p=0,
-        energy=1e8,
-        device="auto",
-    ):
+        n: int = 10,
+        mu_x: float = 0,
+        mu_y: float = 0,
+        mu_xp: float = 0,
+        mu_yp: float = 0,
+        sigma_x: float = 175e-9,
+        sigma_y: float = 175e-9,
+        sigma_xp: float = 2e-7,
+        sigma_yp: float = 2e-7,
+        sigma_s: float = 0,
+        sigma_p: float = 0,
+        energy: float = 1e8,
+        device: str = "auto",
+    ) -> "ParticleBeam":
         """
         Generate Cheetah Beam of *n* linspaced particles.
 
         Parameters
         ----------
         n : int, optional
             Number of particles to generate.
@@ -558,25 +562,25 @@
         mu_y : float, optional
             Center of the particle distribution on y in meters.
         mu_px : float, optional
             Center of the particle distribution on px in meters.
         mu_py : float, optional
             Center of the particle distribution on py in meters.
         sigma_x : float, optional
-            Sgima of the particle distribution in x direction in meters.
+            Sigma of the particle distribution in x direction in meters.
         sigma_y : float, optional
-            Sgima of the particle distribution in y direction in meters.
+            Sigma of the particle distribution in y direction in meters.
         sigma_xp : float, optional
-            Sgima of the particle distribution in px direction in meters.
+            Sigma of the particle distribution in px direction in meters.
         sigma_yp : float, optional
-            Sgima of the particle distribution in py direction in meters.
+            Sigma of the particle distribution in py direction in meters.
         sigma_s : float, optional
-            Sgima of the particle distribution in s direction in meters.
+            Sigma of the particle distribution in s direction in meters.
         sigma_p : float, optional
-            Sgima of the particle distribution in p direction in meters.
+            Sigma of the particle distribution in p direction in meters.
         energy : float, optional
             Energy of the beam in eV.
         device : string
             Device to move the beam's particle array to. If set to `"auto"` a CUDA GPU
             is selected if available. The CPU is used otherwise.
         """
         particles = torch.ones((n, 7), dtype=torch.float32)
@@ -595,48 +599,48 @@
         )
         particles[:, 4] = torch.linspace(-sigma_s, sigma_s, n, dtype=torch.float32)
         particles[:, 5] = torch.linspace(-sigma_p, sigma_p, n, dtype=torch.float32)
 
         return cls(particles, energy, device=device)
 
     @classmethod
-    def from_ocelot(cls, parray, device="auto"):
+    def from_ocelot(cls, parray, device: str = "auto") -> "ParticleBeam":
         """
         Convert an Ocelot ParticleArray `parray` to a Cheetah Beam.
         """
         n = parray.rparticles.shape[1]
         particles = torch.ones((n, 7))
         particles[:, :6] = torch.tensor(
             parray.rparticles.transpose(), dtype=torch.float32
         )
 
         return cls(particles, 1e9 * parray.E, device=device)
 
     @classmethod
-    def from_astra(cls, path, **kwargs):
+    def from_astra(cls, path: str, **kwargs) -> "ParticleBeam":
         """Load an Astra particle distribution as a Cheetah Beam."""
         particles, energy = from_astrabeam(path)
         particles_7d = torch.ones((particles.shape[0], 7))
         particles_7d[:, :6] = torch.from_numpy(particles)
         return cls(particles_7d, energy, **kwargs)
 
     def transformed_to(
         self,
-        mu_x=None,
-        mu_y=None,
-        mu_xp=None,
-        mu_yp=None,
-        sigma_x=None,
-        sigma_y=None,
-        sigma_xp=None,
-        sigma_yp=None,
-        sigma_s=None,
-        sigma_p=None,
-        energy=None,
-    ):
+        mu_x: Optional[float] = None,
+        mu_y: Optional[float] = None,
+        mu_xp: Optional[float] = None,
+        mu_yp: Optional[float] = None,
+        sigma_x: Optional[float] = None,
+        sigma_y: Optional[float] = None,
+        sigma_xp: Optional[float] = None,
+        sigma_yp: Optional[float] = None,
+        sigma_s: Optional[float] = None,
+        sigma_p: Optional[float] = None,
+        energy: Optional[float] = None,
+    ) -> "ParticleBeam":
         """
         Create version of this beam that is transformed to new beam parameters.
 
         Parameters
         ----------
         n : int, optional
             Number of particles to generate.
@@ -645,25 +649,25 @@
         mu_y : float, optional
             Center of the particle distribution on y in meters.
         mu_xp : float, optional
             Center of the particle distribution on px in meters.
         mu_yp : float, optional
             Center of the particle distribution on py in meters.
         sigma_x : float, optional
-            Sgima of the particle distribution in x direction in meters.
+            Sigma of the particle distribution in x direction in meters.
         sigma_y : float, optional
-            Sgima of the particle distribution in y direction in meters.
+            Sigma of the particle distribution in y direction in meters.
         sigma_xp : float, optional
-            Sgima of the particle distribution in px direction in meters.
+            Sigma of the particle distribution in px direction in meters.
         sigma_yp : float, optional
-            Sgima of the particle distribution in py direction in meters.
+            Sigma of the particle distribution in py direction in meters.
         sigma_s : float, optional
-            Sgima of the particle distribution in s direction in meters.
+            Sigma of the particle distribution in s direction in meters.
         sigma_p : float, optional
-            Sgima of the particle distribution in p direction in meters.
+            Sigma of the particle distribution in p direction in meters.
         energy : float, optional
             Energy of the beam in eV.
         device : string
             Device to move the beam's particle array to. If set to `"auto"` a CUDA GPU
             is selected if available. The CPU is used otherwise.
         """
         mu_x = mu_x if mu_x is not None else self.mu_x
@@ -711,118 +715,118 @@
         particles = torch.ones_like(
             self.particles, dtype=torch.float32, device=self.device
         )
         particles[:, :6] = phase_space
 
         return self.__class__(particles=particles, energy=energy)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.n
 
     @property
-    def n(self):
+    def n(self) -> int:
         return len(self.particles)
 
     @property
-    def xs(self):
+    def xs(self) -> Optional[torch.Tensor]:
         return self.particles[:, 0] if self is not Beam.empty else None
 
     @xs.setter
-    def xs(self, value):
+    def xs(self, value: torch.Tensor) -> None:
         self.particles[:, 0] = value
 
     @property
-    def mu_x(self):
+    def mu_x(self) -> Optional[float]:
         return float(self.xs.mean()) if self is not Beam.empty else None
 
     @property
-    def sigma_x(self):
+    def sigma_x(self) -> Optional[float]:
         return float(self.xs.std()) if self is not Beam.empty else None
 
     @property
-    def xps(self):
+    def xps(self) -> Optional[torch.Tensor]:
         return self.particles[:, 1] if self is not Beam.empty else None
 
     @xps.setter
-    def xps(self, value):
+    def xps(self, value: torch.Tensor) -> None:
         self.particles[:, 1] = value
 
     @property
-    def mu_xp(self):
+    def mu_xp(self) -> Optional[float]:
         return float(self.xps.mean()) if self is not Beam.empty else None
 
     @property
-    def sigma_xp(self):
+    def sigma_xp(self) -> Optional[float]:
         return float(self.xps.std()) if self is not Beam.empty else None
 
     @property
-    def ys(self):
+    def ys(self) -> Optional[torch.Tensor]:
         return self.particles[:, 2] if self is not Beam.empty else None
 
     @ys.setter
-    def ys(self, value):
+    def ys(self, value: torch.Tensor) -> None:
         self.particles[:, 2] = value
 
     @property
-    def mu_y(self):
+    def mu_y(self) -> Optional[float]:
         return float(self.ys.mean()) if self is not Beam.empty else None
 
     @property
-    def sigma_y(self):
+    def sigma_y(self) -> Optional[float]:
         return float(self.ys.std()) if self is not Beam.empty else None
 
     @property
-    def yps(self):
+    def yps(self) -> Optional[torch.Tensor]:
         return self.particles[:, 3] if self is not Beam.empty else None
 
     @yps.setter
-    def yps(self, value):
+    def yps(self, value: torch.Tensor) -> None:
         self.particles[:, 3] = value
 
     @property
-    def mu_yp(self):
+    def mu_yp(self) -> Optional[float]:
         return float(self.yps.mean()) if self is not Beam.empty else None
 
     @property
-    def sigma_yp(self):
+    def sigma_yp(self) -> Optional[float]:
         return float(self.yps.std()) if self is not Beam.empty else None
 
     @property
-    def ss(self):
+    def ss(self) -> Optional[torch.Tensor]:
         return self.particles[:, 4] if self is not Beam.empty else None
 
     @ss.setter
-    def ss(self, value):
+    def ss(self, value: torch.Tensor) -> None:
         self.particles[:, 4] = value
 
     @property
-    def mu_s(self):
+    def mu_s(self) -> Optional[float]:
         return float(self.ss.mean()) if self is not Beam.empty else None
 
     @property
-    def sigma_s(self):
+    def sigma_s(self) -> Optional[float]:
         return float(self.ss.std()) if self is not Beam.empty else None
 
     @property
-    def ps(self):
+    def ps(self) -> Optional[torch.Tensor]:
         return self.particles[:, 5] if self is not Beam.empty else None
 
     @ps.setter
-    def ps(self, value):
+    def ps(self, value: torch.Tensor) -> None:
         self.particles[:, 5] = value
 
     @property
-    def mu_p(self):
+    def mu_p(self) -> Optional[float]:
         return float(self.ps.mean()) if self is not Beam.empty else None
 
     @property
-    def sigma_p(self):
+    def sigma_p(self) -> Optional[float]:
         return float(self.ps.std()) if self is not Beam.empty else None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(n={self.n}, mu_x={self.mu_x:.6f},"
             f" mu_xp={self.mu_xp:.6f}, mu_y={self.mu_y:.6f}, mu_yp={self.mu_yp:.6f},"
             f" sigma_x={self.sigma_x:.6f}, sigma_xp={self.sigma_xp:.6f},"
             f" sigma_y={self.sigma_y:.6f}, sigma_yp={self.sigma_yp:.6f},"
             f" sigma_s={self.sigma_s:.6f}, sigma_p={self.sigma_p:.6f},"
             f" energy={self.energy:.3f})"
```

### Comparing `cheetah-accelerator-0.5.18/cheetah/utils.py` & `cheetah-accelerator-0.5.19/cheetah/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import numpy as np
-import torch
 
 from cheetah import accelerator as acc
 
 # electron mass in eV
 m_e_eV = 510998.8671
 
 
-def from_astrabeam(path: str):
+def from_astrabeam(path: str) -> tuple[np.ndarray, float]:
     """
     Read from a ASTRA beam distribution, and prepare for conversion to a Cheetah
     ParticleBeam or ParameterBeam.
 
     Adapted from the implementation in ocelot:
     https://github.com/ocelot-collab/ocelot/blob/master/ocelot/adaptors/astra2ocelot.py
 
@@ -66,15 +65,15 @@
     particles[:, 1] = xp[:, 3] / Pref
     particles[:, 3] = xp[:, 4] / Pref
     particles[:, 5] = (gamma / gamref - 1) / betaref
 
     return particles, energy
 
 
-def ocelot2cheetah(element, warnings=True):
+def ocelot2cheetah(element, warnings: bool = True) -> "acc.Element":
     """
     Translate an Ocelot element to a Cheetah element.
 
     Parameters
     ----------
     element : ocelot.Element
         Ocelot element object representing an element of particle accelerator.
@@ -83,38 +82,38 @@
     -------
     cheetah.Element
         Cheetah element object representing an element of particle accelerator.
 
     Notes
     -----
     Object not supported by Cheetah are translated to drift sections. Screen objects are
-    created only from `ocelot.Monitor` objects when the string "SCR" in their `id`
-    attribute. Their screen properties are always set to default values and most likely
-    need adjusting afterwards. BPM objects are only created from `ocelot.Monitor`
-    objects when their id has a substring "BPM".
+    created only from `ocelot.Monitor` objects when the string "SCR" is contained
+    in their `id` attribute. Their screen properties are always set to default
+    values and most likely need adjusting afterwards. BPM objects are only created
+    from `ocelot.Monitor` objects when their id has a substring "BPM".
     """
     try:
         import ocelot as oc
     except ImportError:
         raise ImportError(
-            """To use the ocelot2cheetah lattice converter, Ocelot must be first 
+            """To use the ocelot2cheetah lattice converter, Ocelot must be first
         installed, see https://github.com/ocelot-collab/ocelot """
         )
 
     if isinstance(element, oc.Drift):
         return acc.Drift(element.l, name=element.id)
     elif isinstance(element, oc.Quadrupole):
         return acc.Quadrupole(element.l, element.k1, name=element.id)
     elif isinstance(element, oc.Hcor):
         return acc.HorizontalCorrector(element.l, element.angle, name=element.id)
     elif isinstance(element, oc.Vcor):
         return acc.VerticalCorrector(element.l, element.angle, name=element.id)
     elif isinstance(element, oc.Cavity):
         return acc.Cavity(element.l, name=element.id)
-    elif isinstance(element, oc.Monitor) and "BSC" in element.id:
+    elif isinstance(element, oc.Monitor) and ("SCR" in element.id):
         if warnings:
             print(
                 "WARNING: Diagnostic screen was converted with default screen"
                 " properties."
             )
         return acc.Screen((2448, 2040), (3.5488e-6, 2.5003e-6), name=element.id)
     elif isinstance(element, oc.Monitor) and "BPM" in element.id:
@@ -125,15 +124,15 @@
         if warnings:
             print(
                 f"WARNING: Unknown element {element.id}, replacing with drift section."
             )
         return acc.Drift(element.l, name=element.id)
 
 
-def subcell_of_ocelot(cell, start, end):
+def subcell_of_ocelot(cell: list, start: str, end: str) -> list:
     """Extract a subcell `[start, end]` from an Ocelot cell."""
     subcell = []
     is_in_subcell = False
     for el in cell:
         if el.id == start:
             is_in_subcell = True
         if is_in_subcell:
```

### Comparing `cheetah-accelerator-0.5.18/cheetah_accelerator.egg-info/PKG-INFO` & `cheetah-accelerator-0.5.19/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-Metadata-Version: 2.1
-Name: cheetah-accelerator
-Version: 0.5.18
-Summary: Fast particle accelerator optics simulation for reinforcement learning and optimisation applications.
-Home-page: https://github.com/desy-ml/cheetah
-Author: Jan Kaiser & Oliver Stein
-Author-email: jan.kaiser@desy.de
-Description-Content-Type: text/markdown
+<img src="images/logo.png" align="right" width="25%"/>
 
 # Cheetah
 
 Cheetah is a particle tracking accelerator we built specifically to speed up the training of reinforcement learning models.
 
-
 ## Installation
 
 Simply install *Cheetah* from PyPI by running the following command.
 
 ```bash
 pip install cheetah-accelerator
 ```
 
-
 ## How To Use
 
 A sequence of accelerator elements (or a lattice) is called a `Segment` in *Cheetah*. You can create a `Segment` as follows
 
 ```python
 segment = Segment([
     BPM(name="BPM1SMATCH"),
@@ -79,15 +70,14 @@
 segment.plot_overview(beam=beam)
 ```
 
 ![Overview Plot](images/misalignment.png)
 
 where the optional keyword argument `beam` is the incoming beam represented by the reference particles. Cheetah will use a default incoming beam, if no beam is passed.
 
-
 ## Cite Cheetah
 
 To cite Cheetah in publications:
 
 ```bibtex
 @inproceedings{stein2022accelerating,
     author = {Stein, Oliver and
@@ -95,7 +85,24 @@
               Eichler, Annika},
     title = {Accelerating Linear Beam Dynamics Simulations for Machine Learning Applications},
     booktitle = {Proceedings of the 13th International Particle Accelerator Conference},
     year = {2022},
     url = {https://github.com/desy-ml/cheetah},
 }
 ```
+
+## For Developers
+
+Activate your virtual envrionment. (Optional)
+
+Install the cheetah package as editable
+
+```sh
+pip install -e .
+```
+
+We suggest to install pre-commit hooks to automatically conform with the code formatting in commits:
+
+```sh
+pip install pre-commit
+pre-commit install
+```
```

