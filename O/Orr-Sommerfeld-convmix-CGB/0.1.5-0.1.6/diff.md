# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.1.5.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.1.6.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.1.5.tar` & `orr_sommerfeld_convmix_cgb-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/LICENSE
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/LICENSE
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.5/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.1.6/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,14 @@
                                                                    yaxis=dict(title=r'$c_{i}$',titlefont=dict(size=18), tickfont=dict(family='latex')),
                                                                    plot_bgcolor='rgba(0,0,0,0.1)',
                                                                    title_x=0.5)
     fig = go.Figure(data=[traza], layout=layout)
     iplot(fig)
     return
  def vector_perturbaciones(N,lam,V,n,alpha,beta):
-    
     D,D2,D4=Dmat(N)
     #Chekeado que Dmat funciona bien
     
     #Calculo parámetros de mis ecuaciones
     I=eye(N-1)
     k2=(alpha*alpha)+(beta*beta)
     k22=k2*k2
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.5/LICENSE` & `orr_sommerfeld_convmix_cgb-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.1.5/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.5/PKG-INFO` & `orr_sommerfeld_convmix_cgb-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orr_Sommerfeld_convmix_CGB
-Version: 0.1.5
+Version: 0.1.6
 Summary: Paquete para cálculo de autovalores y autofunciones.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Pablo Szuban <pablo.szuban@ib.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

