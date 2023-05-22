# Comparing `tmp/hydrogibs-0.3.3.tar.gz` & `tmp/hydrogibs-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.3.3.tar", last modified: Mon May 15 13:58:33 2023, max compression
+gzip compressed data, was "hydrogibs-0.3.4.tar", last modified: Mon May 22 14:27:05 2023, max compression
```

## Comparing `hydrogibs-0.3.3.tar` & `hydrogibs-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-15 13:58:33.006546 hydrogibs-0.3.3/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.3/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-15 13:58:33.002546 hydrogibs-0.3.3/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.3.3/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-15 13:58:32.998546 hydrogibs-0.3.3/hydrogibs/
--rwxrwxr-x   0 axel      (1000) axel      (1000)    12872 2023-05-15 13:57:10.000000 hydrogibs-0.3.3/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     5162 2023-05-15 06:33:21.000000 hydrogibs-0.3.3/hydrogibs/ModelApp.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.3/hydrogibs/ModelTemplate.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     8243 2023-05-15 11:39:50.000000 hydrogibs-0.3.3/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.3/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.3.3/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.3.3/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.3/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-15 13:58:33.002546 hydrogibs-0.3.3/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-15 13:58:32.000000 hydrogibs-0.3.3/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-05-15 13:58:32.000000 hydrogibs-0.3.3/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-05-15 13:58:32.000000 hydrogibs-0.3.3/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-05-15 13:58:32.000000 hydrogibs-0.3.3/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-05-15 13:58:23.000000 hydrogibs-0.3.3/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-05-15 13:58:33.006546 hydrogibs-0.3.3/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-22 14:27:05.206971 hydrogibs-0.3.4/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.4/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-22 14:27:05.206971 hydrogibs-0.3.4/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.3.4/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-22 14:27:05.206971 hydrogibs-0.3.4/hydrogibs/
+-rwxrwxr-x   0 axel      (1000) axel      (1000)    14689 2023-05-22 14:24:02.000000 hydrogibs-0.3.4/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     5176 2023-05-16 12:38:08.000000 hydrogibs-0.3.4/hydrogibs/ModelApp.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.4/hydrogibs/ModelTemplate.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     9762 2023-05-22 14:18:40.000000 hydrogibs-0.3.4/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.4/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.3.4/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.3.4/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.4/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-22 14:27:05.206971 hydrogibs-0.3.4/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-22 14:27:05.000000 hydrogibs-0.3.4/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-05-22 14:27:05.000000 hydrogibs-0.3.4/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-05-22 14:27:05.000000 hydrogibs-0.3.4/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-05-22 14:27:05.000000 hydrogibs-0.3.4/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-05-22 14:26:25.000000 hydrogibs-0.3.4/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-05-22 14:27:05.206971 hydrogibs-0.3.4/setup.cfg
```

### Comparing `hydrogibs-0.3.3/LICENSE` & `hydrogibs-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.3/PKG-INFO` & `hydrogibs-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.3
+Version: 0.3.4
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.3.3/hydrogibs/GR4.py` & `hydrogibs-0.3.4/hydrogibs/GR4.py`

 * *Files 21% similar despite different names*

```diff
@@ -116,41 +116,116 @@
         X1 (float)  [-] : dQ = X1 * dPrecipitations
         X2 (float)  [mm]: Initial abstraction (vegetation interception)
         X3 (float) [1/h]: Sub-surface water volume emptying rate dQs = X3*V*dt
         X4 (float)  [h] : the hydrogram's raising time
     """
 
     def __init__(self,
-                 X1: float,
-                 X2: float,
-                 X3: float,
-                 X4: float,
+                 X1: float = 0,
+                 X2: float = 0,
+                 X3: float = 0,
+                 X4: float = 0,
                  surface: float = 1,
                  initial_volume: float = 0,
                  transfer_function: Callable = None) -> None:
 
         assert 0 <= X1 <= 1, "Runoff coefficient must be within [0 : 1]"
         assert 0 <= X2, "Initial abstraction must be positive"
         assert 0 <= X3 <= 1, "Emptying rate must be within [0 : 1]"
         assert 0 <= X4, "Raising time must be positive"
 
         self.X1 = X1
         self.X2 = X2
         self.X3 = X3
         self.X4 = X4
+
         self.surface = surface
         self.transfer_function = (transfer_function
                                   if transfer_function is not None
                                   else _transfer_func)
         self.initial_volume = initial_volume
 
     def __matmul__(self, rain):
         return rain @ self
 
 
+class Laval(Catchment):
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(57.6/100, 7.8, 2.4/100, 0.38,
+                         *args, **kwargs)
+
+
+class Erlenbach(Catchment):
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(46.5/100, 13.6, 16.2/100, 0.63,
+                         *args, **kwargs)
+
+
+class Rimbaud(Catchment):
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(35.4/100, 40, 2.28/100, 1.07,
+                         *args, **kwargs)
+
+
+class Latte(Catchment):
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(14.4/100, 75.4, 3.96/100, 0.78,
+                         *args, **kwargs)
+
+
+class Sapine(Catchment):
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(15.7/100, 71.1, 0.90/100, 1.03,
+                         *args, **kwargs)
+
+
+class Rietholzbach(Catchment):
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(26.5/100, 17, 2.82/100, 1.11,
+                         *args, **kwargs)
+
+
+class Lumpenenbach(Catchment):
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(22.6/100, 12.2, 9.6/100, 0.5,
+                         *args, **kwargs)
+
+
+class Vogelbach(Catchment):
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(31.4/100, 11.5, 5.88/100, 0.64,
+                         *args, **kwargs)
+
+
+class Brusquet(Catchment):
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(13.8/100, 22.4, 0.72/100, 1.63,
+                         *args, **kwargs)
+
+
+presets = (
+    Laval, Erlenbach, Rimbaud,
+    Latte,
+    Sapine,
+    Rietholzbach,
+    Lumpenenbach,
+    Vogelbach,
+    Brusquet
+)
+
+
 class Event(ModelTemplate.Event):
     """
     Stores all relevant results of a GR4h calculation
 
     basic class instead of dataclass, namedtuple or dataframe is used
     for speed reasons (an event will be created at every diagram update)
     """
@@ -184,14 +259,15 @@
                  colors=("teal",
                          "k",
                          "indigo",
                          "tomato",
                          "green"),
                  flows_margin=0.3,
                  rain_margin=7,
+                 figsize=(6, 3.5),
                  show=True) -> None:
 
         self.colors = colors
         self.flows_margin = flows_margin
         self.rain_margin = rain_margin
 
         time = event.time
@@ -201,55 +277,55 @@
         Qv = event.discharge_volume
         Q = event.discharge
 
         with plt.style.context(style):
 
             c1, c2, c3, c4, c5 = self.colors
 
-            fig, ax1 = plt.subplots(figsize=(6, 3.5), dpi=100)
-            ax1.set_title("Runoff response to rainfall")
+            fig, ax1 = plt.subplots(figsize=figsize, dpi=100)
 
             lineQ, = ax1.plot(
                 time,
                 Q,
                 lw=2,
                 color=c1,
-                label="total discharge",
+                label="Discharge",
                 zorder=10
             )
             lineQp, = ax1.plot(
                 time,
                 Qp,
                 lw=1,
                 ls='-.',
                 color=c4,
-                label="Runoff discharge",
+                label="Surface runoff",
                 zorder=9
             )
             lineQv, = ax1.plot(
                 time,
                 Qv,
                 lw=1,
                 ls='-.',
                 color=c5,
-                label="Sub-surface discharge",
+                label="Sub-surface runoff",
                 zorder=9
             )
-            ax1.set_ylabel("$Q$ (m³/s)", color=c1)
-            ax1.set_xlabel("Time (h)")
+            ax1.set_ylabel("$Q$ (m$^3$/s)", color=c1)
+            ax1.set_xlabel("t (h)")
             ax1.set_xlim((time.min(), time.max()))
             Qmax = Q.max()
             if Qmax:
                 ax1.set_ylim((0, (1 + self.flows_margin)*Qmax))
             ax1.set_yscale("linear")
             yticks = ax1.get_yticks()
             yticks = [
                 y for y in yticks
                 if y < max(yticks)/(self.flows_margin + 1)
             ]
+            yticks = [float(f"{y:.3e}") for y in yticks]
             ax1.set_yticks(yticks)
             ax1.set_yticklabels(yticks, color=c1)
 
             ax2 = ax1.twinx()
             lineP, = ax2.step(
                 time,
                 rain,
@@ -262,33 +338,33 @@
                 ax2.set_ylim(((1 + self.rain_margin) * max_rain, 0))
             ax2.grid(False)
             ax2.set_yticks((0, max_rain))
             ax2.set_yticklabels(ax2.get_yticklabels(), color=c2)
 
             ax3 = ax2.twinx()
             lineV, = ax3.plot(time, V, ":",
-                              color=c3, label="Storage volume", lw=1)
+                              color=c3, label="Stored volume", lw=1)
             ax3.set_ylabel("$V$ (mm)", color=c3)
-            ax3.set_xlabel("$t$ (h)")
             Vmax = V.max()
             if Vmax:
                 ax3.set_ylim((0, (1 + 2*self.flows_margin) * Vmax))
             yticks = ax3.get_yticks()
             yticks = [
                 y for y in yticks
                 if y < max(yticks)/(1 + self.flows_margin)
             ]
+            yticks = [float(f"{y:.3e}") for y in yticks]
             ax3.set_yticks(yticks)
             ax3.set_yticklabels(ax3.get_yticks(), color=c3)
             ax3.set_yscale("linear")
             ax3.grid(False)
 
             lines = (lineP, lineQ, lineQp, lineQv, lineV)
             labs = [line.get_label() for line in lines]
-            ax1.legend(lines, labs)
+            ax3.legend(lines, labs, loc="upper right")
 
             plt.tight_layout()
 
             self.figure, self.axes, self.lines = fig, (ax1, ax2, ax3), lines
 
         if show:
             plt.show()
@@ -401,16 +477,16 @@
     dTp = X1*dP
     dTv = X3*V
     dTp[t_abstraction] = 0
     dTv[t_abstraction] = 0
 
     q = catchment.transfer_function(X4, num=(time <= 2*X4).sum())
 
-    Qp = S * np.convolve(dTp, q)[:time.size] * dt
-    Qv = S * np.convolve(dTv, q)[:time.size] * dt
+    Qp = S * np.convolve(dTp, q)[:time.size] * dt / 3.6
+    Qv = S * np.convolve(dTv, q)[:time.size] * dt / 3.6
 
     return Event(time, dP, V, dTp+dTv, Qp, Qv, Qp+Qv)
 
 
 def GR4_demo(kind: Literal["array", "block"] = "array"):
 
     if kind == "block":
```

### Comparing `hydrogibs-0.3.3/hydrogibs/ModelApp.py` & `hydrogibs-0.3.4/hydrogibs/ModelApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             close()
 
     def init_diagram(self, *args, **kwargs):
 
         diagram = self.event.diagram(*args, **kwargs)
 
         self.canvas = FigureCanvasTkAgg(diagram.figure, master=self.dframe)
-        toolbar = NavigationToolbar2Tk(self.canvas, self.dframe)
+        toolbar = NavigationToolbar2Tk(canvas=self.canvas, window=self.dframe)
         toolbar.update()
         self.canvas._tkcanvas.pack()
         self.canvas.draw()
         self.canvas.get_tk_widget().pack()
         self.canvas.mpl_connect('key_press_event',
                                 lambda arg: key_press_handler(
                                     arg, self.canvas, toolbar
```

### Comparing `hydrogibs-0.3.3/hydrogibs/ModelTemplate.py` & `hydrogibs-0.3.4/hydrogibs/ModelTemplate.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.3/hydrogibs/QDF.py` & `hydrogibs-0.3.4/hydrogibs/QDF.py`

 * *Files 14% similar despite different names*

```diff
@@ -192,14 +192,15 @@
     else:
         entries = [
             ("catchment", "surface", "km^2", "S"),
             ("catchment", "length", "km", "L"),
             ("catchment", "mean_slope", "%", "im")
         ]
     entries += [
+        ("rain", "duration", "h", "d"),
         ("rain", "return_period", "y", "T"),
         ("rain", "specific_discharge", "m3/s", "Qs"),
         ("rain", "discharge_Q10", "m3/s", "Q10"),
         ("rain", "tf", "h")
     ]
     entries = map(lambda e: Entry(*e), entries)
     ModelApp(
@@ -229,14 +230,49 @@
 
     discharge_peak = discharge(Q10=rain.discharge_Q10,
                                Qsp=rain.specific_discharge,
                                T=rain.return_period,
                                constants=constants_mean,
                                d=rain.duration,
                                ds=ds)
+    _d = np.linspace(0, 5)
+    print(f"{rain.discharge_Q10 = }")
+    print(f"{rain.specific_discharge = }")
+    print(f"{rain.return_period = }")
+    print(f"{ds = }")
+    with plt.style.context("ggplot"):
+        plt.figure(figsize=(3, 3))
+        plt.plot(_d, discharge(Q10=rain.discharge_Q10,
+                               Qsp=rain.specific_discharge,
+                               T=rain.return_period,
+                               constants=constants_mean,
+                               d=_d,
+                               ds=ds), label="Q$_{10}$ = 1.3 m$^3$/s")
+        print(discharge(Q10=rain.discharge_Q10,
+                        Qsp=rain.specific_discharge,
+                        T=rain.return_period,
+                        constants=constants_mean,
+                        d=1,
+                        ds=ds))
+        print(discharge(Q10=2,
+                        Qsp=2,
+                        T=rain.return_period,
+                        constants=constants_mean,
+                        d=1,
+                        ds=ds))
+        plt.plot(_d, discharge(Q10=2,
+                               Qsp=2,
+                               T=rain.return_period,
+                               constants=constants_mean,
+                               d=_d,
+                               ds=ds), label="Q$_{10}$ = 2.0 m$^3$/s")
+        plt.xlabel("Durée de la pluie (h)")
+        plt.ylabel("Débit de pointe (m$^3$/s)")
+        plt.legend()
+        plt.show()
 
     dt = rain.dt
     time = np.arange(0, rain.tf, step=rain.dt)
     Q = np.full_like(time, discharge_peak)
 
     ds = catchment.specific_duration
     i = time <= ds
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hydrogibs-0.3.3/hydrogibs/RationalMethod.py` & `hydrogibs-0.3.4/hydrogibs/RationalMethod.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.3/hydrogibs/SoCoSe.py` & `hydrogibs-0.3.4/hydrogibs/SoCoSe.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.3/hydrogibs/misc.py` & `hydrogibs-0.3.4/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.3/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.3.4/hydrogibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.3
+Version: 0.3.4
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

