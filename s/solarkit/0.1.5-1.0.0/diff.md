# Comparing `tmp/solarkit-0.1.5.tar.gz` & `tmp/solarkit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarkit-0.1.5.tar", last modified: Wed May 10 20:05:22 2023, max compression
+gzip compressed data, was "solarkit-1.0.0.tar", last modified: Mon May 22 17:57:58 2023, max compression
```

## Comparing `solarkit-0.1.5.tar` & `solarkit-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 20:05:22.919225 solarkit-0.1.5/
--rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2003 2023-05-10 20:05:22.918723 solarkit-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1399 2023-05-08 17:28:30.000000 solarkit-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 20:05:22.919726 solarkit-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-05-10 20:04:38.000000 solarkit-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:05:22.912225 solarkit-0.1.5/solarkit/
--rw-rw-rw-   0        0        0      290 2023-05-08 17:26:35.000000 solarkit-0.1.5/solarkit/__init__.py
--rw-rw-rw-   0        0        0     3597 2023-05-02 16:04:11.000000 solarkit-0.1.5/solarkit/planet.py
--rw-rw-rw-   0        0        0     2876 2023-05-08 17:27:06.000000 solarkit-0.1.5/solarkit/solar_system.py
--rw-rw-rw-   0        0        0     2099 2023-05-08 17:26:57.000000 solarkit-0.1.5/solarkit/utils.py
--rw-rw-rw-   0        0        0    12598 2023-05-10 20:02:59.000000 solarkit-0.1.5/solarkit/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:05:22.917224 solarkit-0.1.5/solarkit.egg-info/
--rw-rw-rw-   0        0        0     2003 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 17:57:58.170034 solarkit-1.0.0/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2054 2023-05-22 17:57:58.169534 solarkit-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1449 2023-05-22 17:56:15.000000 solarkit-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 17:57:58.170535 solarkit-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2023-05-22 17:57:31.000000 solarkit-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:57:58.163535 solarkit-1.0.0/solarkit/
+-rw-rw-rw-   0        0        0      290 2023-05-08 17:26:35.000000 solarkit-1.0.0/solarkit/__init__.py
+-rw-rw-rw-   0        0        0     3632 2023-05-22 17:14:51.000000 solarkit-1.0.0/solarkit/planet.py
+-rw-rw-rw-   0        0        0     4657 2023-05-22 17:33:44.000000 solarkit-1.0.0/solarkit/solar_system.py
+-rw-rw-rw-   0        0        0     2099 2023-05-08 17:26:57.000000 solarkit-1.0.0/solarkit/utils.py
+-rw-rw-rw-   0        0        0    14098 2023-05-22 17:51:27.000000 solarkit-1.0.0/solarkit/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:57:58.168534 solarkit-1.0.0/solarkit.egg-info/
+-rw-rw-rw-   0        0        0     2054 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/top_level.txt
```

### Comparing `solarkit-0.1.5/LICENSE` & `solarkit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solarkit-0.1.5/PKG-INFO` & `solarkit-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 0.1.5
+Version: 1.0.0
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -23,22 +23,23 @@
 * [Repo link](https://github.com/carlos-lorenzo/solarkit) (for PyPI)
 
 ### Challenges
 * Kepler's Third Law
 * Visualise a solar system
 * Visualise the solar system, animated
 * Spinograph
+* Angle vs Time
 * Heliocentric model
 
 ### Personal aditions
 * Tools to create, save & load a custom solar system
 * Save the model output to an image
 * Spinograph, animated
 
 ### How to use
 1. "pip install solarkit" or [download package files](https://github.com/carlos-lorenzo/solarkit/tree/main/Package) from repository and  install locally
 2. [Download](https://github.com/carlos-lorenzo/solarkit/blob/08a2d0ddc34b3abecce7789cbe7163d7d49cbd48/planet_data.csv) or create your own data
 3. Create .py file
 4. Start experimenting! (follow example image for guidance)
 
-### Use example
-![solarkit_example](https://user-images.githubusercontent.com/91377173/236692357-7e14751b-2e94-4a01-894f-2202fef1e30d.jpg)
+### Use example (example file available in repository)
+![solarkit_example](https://github.com/carlos-lorenzo/solarkit/assets/91377173/cdab5fb1-c55e-427f-a0d9-f156be7e535c)
```

### Comparing `solarkit-0.1.5/README.md` & `solarkit-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 * [Repo link](https://github.com/carlos-lorenzo/solarkit) (for PyPI)
 
 ### Challenges
 * Kepler's Third Law
 * Visualise a solar system
 * Visualise the solar system, animated
 * Spinograph
+* Angle vs Time
 * Heliocentric model
 
 ### Personal aditions
 * Tools to create, save & load a custom solar system
 * Save the model output to an image
 * Spinograph, animated
 
 ### How to use
 1. "pip install solarkit" or [download package files](https://github.com/carlos-lorenzo/solarkit/tree/main/Package) from repository and  install locally
 2. [Download](https://github.com/carlos-lorenzo/solarkit/blob/08a2d0ddc34b3abecce7789cbe7163d7d49cbd48/planet_data.csv) or create your own data
 3. Create .py file
 4. Start experimenting! (follow example image for guidance)
 
-### Use example
-![solarkit_example](https://user-images.githubusercontent.com/91377173/236692357-7e14751b-2e94-4a01-894f-2202fef1e30d.jpg)
+### Use example (example file available in repository)
+![solarkit_example](https://github.com/carlos-lorenzo/solarkit/assets/91377173/cdab5fb1-c55e-427f-a0d9-f156be7e535c)
```

### Comparing `solarkit-0.1.5/setup.py` & `solarkit-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.5"
+VERSION = "1.0.0"
 DESCRIPTION = "Visualise a solar system and do cool stuff with it"
 
 # Setting up
 setup(
     name="solarkit",
     version=VERSION,
     author="Carlos Lorenzo",
     author_email="<clorenzozuniga@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=["numpy", "pandas", "matplotlib"],
+    install_requires=["numpy", "pandas", "matplotlib", "scipy"],
     keywords=["solar system", "space", "astrophysics", "bpho"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `solarkit-0.1.5/solarkit/planet.py` & `solarkit-1.0.0/solarkit/planet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dataclasses import dataclass, field
 from typing import Dict, List
 
-
 import numpy as np
-
+from scipy.interpolate import interp1d
 
 # Objects
 @dataclass
 class Planet:
     """
     Holds planet data
     
@@ -125,9 +124,11 @@
                     "z": zz}
             
         else:
             return {"name": self.name,
                     "c": self.colour,
                     "x": x,
                     "y": y}
-            
+    
+    
+
```

### Comparing `solarkit-0.1.5/solarkit/utils.py` & `solarkit-1.0.0/solarkit/utils.py`

 * *Files identical despite different names*

### Comparing `solarkit-0.1.5/solarkit/viewer.py` & `solarkit-1.0.0/solarkit/viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,39 +58,51 @@
         self.dt = self.tmax/2500
         
     def __str__(self) -> str:
         return f"Planets: {self.system.__str__()}\n3D: {self.compute_3D}\nAnimation FPS: {self.target_fps}"
     
     
     
-    def initialise_plotter(self) -> None:
+    def initialise_plotter(self, square_ratio: bool = True) -> None:
         """
         Initalises the area where everythin will be drawn on. Call every time you want to draw a new model
+        
+        Args:
+            square_ratio (bool): Set the ratio of the plot to 1:1
+        
         """
         
         if self.compute_3D:
             self.fig: plt.figure = plt.figure()
             self.ax: plt.Axes = self.fig.add_subplot(projection='3d')
             self.ax.view_init(None, 225)
           
         else:
             self.fig, self.ax = plt.subplots()
             
-            #set aspect ratio to 1
-            RATIO = 1.0
-            x_left, x_right = self.ax.get_xlim()
-            y_low, y_high = self.ax.get_ylim()
-            self.ax.set_aspect(abs((x_right - x_left)/(y_low - y_high)) * RATIO)
+            if square_ratio:
+                #set aspect ratio to 1
+                RATIO = 1.0
+                x_left, x_right = self.ax.get_xlim()
+                y_low, y_high = self.ax.get_ylim()
+                self.ax.set_aspect(abs((x_right - x_left)/(y_low - y_high)) * RATIO)
     
     def server_mode(self) -> None:
         """
         Allow matplotlib to work when not in main thread (when running in server) 
         """
         matplotlib.use("Agg")
     
+    def close_graph(self) -> None:
+        """
+        Closes matplotlib tab
+        """
+        
+        plt.close()
+    
     def add_grid(self) -> None:
         """
         Adds a grid
         """
         plt.grid()
     
     def add_legend(self) -> None:
@@ -225,31 +237,63 @@
         plt.scatter(x, y, c="#4F81BD", marker="D", label="Kepler's third law")
         plt.plot(x, y, c="r", label="Linear (Kepler's third law)")
 
 
         plt.title("Kepler's third law")
         self.lable_axes(x_lable="a (AU)", y_lable="P (Yr)")
         
+    
+    
+    def angle_vs_time_comparison(self, planet_a_name: Optional[str] = "Pluto") -> None:
+        """
+        Compare the angle over time of a planet against a circular orbit 
+        
+        Args:
+            planet_a_name (Optional[str], optional): Planet name to be compared against (must be planet). Defaults to "Pluto".
+
+        Raises:
+            KeyError: Planet name not found in self.system.planets
+        """
+
+        try:
+            planet_a = self.system.planets[planet_a_name]
+        except KeyError:
+            raise KeyError(f"{planet_a_name} not found")
+        
+        
+        t = np.linspace(1, 800, 1000)
+
+        # Call angle_vs_time function to get polar angles
+        theta_planet_a = self.system.compute_angle_vs_time(t=t, P=planet_a.P, ecc=planet_a.ecc, theta0=0) 
+        theta_circular = self.system.compute_angle_vs_time(t=t, P=planet_a.P, ecc=0, theta0=0)
+
+        # Plotting
+        self.ax.plot(t, theta_planet_a, label=planet_a_name)
+        self.ax.plot(t, theta_circular, label='Circular Motion')
+        
+        self.ax.set_xlabel('Time (years)')
+        self.ax.set_ylabel('Polar Angle (radians)')
+        
+        plt.title('Variation of Polar Angle with Time')
         
         
     def system_orbits(self) -> None:
+        
         """
         Plot the orbits of the selected planets
         """
         self.plot_centre(name="Sun", colour="y")
         
         for planet_orbit_data in self.orbit_data:
             self.plot_orbit(orbit_data=planet_orbit_data)  
         
         plt.title("Planet orbits")
         self.lable_axes()
         
             
-        
-            
     def animate_orbits(self) -> None:
         """
         Animate the orbits of the selected planets
         """
         
         while self.t < self.tmax:
             self.plot_centre(name="Sun", colour="y")
```

### Comparing `solarkit-0.1.5/solarkit.egg-info/PKG-INFO` & `solarkit-1.0.0/solarkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 0.1.5
+Version: 1.0.0
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -23,22 +23,23 @@
 * [Repo link](https://github.com/carlos-lorenzo/solarkit) (for PyPI)
 
 ### Challenges
 * Kepler's Third Law
 * Visualise a solar system
 * Visualise the solar system, animated
 * Spinograph
+* Angle vs Time
 * Heliocentric model
 
 ### Personal aditions
 * Tools to create, save & load a custom solar system
 * Save the model output to an image
 * Spinograph, animated
 
 ### How to use
 1. "pip install solarkit" or [download package files](https://github.com/carlos-lorenzo/solarkit/tree/main/Package) from repository and  install locally
 2. [Download](https://github.com/carlos-lorenzo/solarkit/blob/08a2d0ddc34b3abecce7789cbe7163d7d49cbd48/planet_data.csv) or create your own data
 3. Create .py file
 4. Start experimenting! (follow example image for guidance)
 
-### Use example
-![solarkit_example](https://user-images.githubusercontent.com/91377173/236692357-7e14751b-2e94-4a01-894f-2202fef1e30d.jpg)
+### Use example (example file available in repository)
+![solarkit_example](https://github.com/carlos-lorenzo/solarkit/assets/91377173/cdab5fb1-c55e-427f-a0d9-f156be7e535c)
```

