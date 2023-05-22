# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.1.6.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.1.7.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.1.6.tar` & `orr_sommerfeld_convmix_cgb-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/LICENSE
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.7/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.7/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.7/LICENSE
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.7/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.7/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.6/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.1.7/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,50 +245,50 @@
                                                                    yaxis=dict(title=r'$c_{i}$',titlefont=dict(size=18), tickfont=dict(family='latex')),
                                                                    plot_bgcolor='rgba(0,0,0,0.1)',
                                                                    title_x=0.5)
     fig = go.Figure(data=[traza], layout=layout)
     iplot(fig)
     return
  def vector_perturbaciones(N,lam,V,n,alpha,beta):
-    D,D2,D4=Dmat(N)
-    #Chekeado que Dmat funciona bien
+     D,D2,D4=Dmat(N)
+     #Chekeado que Dmat funciona bien
     
-    #Calculo parámetros de mis ecuaciones
-    I=eye(N-1)
-    k2=(alpha*alpha)+(beta*beta)
-    k22=k2*k2
+     #Calculo parámetros de mis ecuaciones
+     I=eye(N-1)
+     k2=(alpha*alpha)+(beta*beta)
+     k22=k2*k2
     
-    v=V[0:(N-1),n]
-    tita=V[(N-1):(2*(N-1)),n]
-    eta=V[2*(N-1):3*(N-1),n]
-    #Expresión de u
-    u= (1j*alpha*dot(D,v)/k2) + dot(beta/k2,eta)
-    #Expresión de w
-    w=((beta*u)-eta)/alpha
+     v=V[0:(N-1),n]
+     tita=V[(N-1):(2*(N-1)),n]
+     eta=V[2*(N-1):3*(N-1),n]
+     #Expresión de u
+     u= (1j*alpha*dot(D,v)/k2) + dot(beta/k2,eta)
+     #Expresión de w
+     w=((beta*u)-eta)/alpha
 
-    # Falta agregar la presion y las expresiones individuales de w y u
-    return  v,u,w,tita
+     # Falta agregar la presion y las expresiones individuales de w y u
+     return  v,u,w,tita
  def normalizacion(v,u,w,tita):
-    vr=v.real
-    vi=v.imag
-    #Busca el valor de màxima norma de u
-    norm= vr*vr+vi*vi
-    i=np.where(abs(norm) == np.max(norm))
-    #Para ese valor máximo, multiplico por un complejo c=a+bj/su fase sea cero y su norma sea 1
-    a=vr[i]/norm[i]
-    b=-vi[i]/norm[i]
-    #a=vi[i]/sqrt(norm[i])
-    #b=-v[i]**2/(vr[i]*sqrt(norm[i]))
-    c= a + (1j*b)   
-    #Luego normalizo todas las autofunciones con el c hallado
-    v=c*v
-    u=c*u
-    w=c*w
-    tita=c*tita
-    return v,u,w,tita  
+     vr=v.real
+     vi=v.imag
+     #Busca el valor de màxima norma de u
+     norm= vr*vr+vi*vi
+     i=np.where(abs(norm) == np.max(norm))
+     #Para ese valor máximo, multiplico por un complejo c=a+bj/su fase sea cero y su norma sea 1
+     a=vr[i]/norm[i]
+     b=-vi[i]/norm[i]
+     #a=vi[i]/sqrt(norm[i])
+     #b=-v[i]**2/(vr[i]*sqrt(norm[i]))
+     c= a + (1j*b)   
+     #Luego normalizo todas las autofunciones con el c hallado
+     v=c*v
+     u=c*u
+     w=c*w
+     tita=c*tita
+     return v,u,w,tita  
 def grafica_autofunciones(N,Ra,Pr,Re,alpha,beta):
     #plt.style.use('ggplot')
     #Vector y
     D,y = cheb(N)
     #Vectores de perturbaciones para un autovalor dado. En este caso tomo el mayor de todos dado que Orr_Sommerfeld() las ordena y voy a elegir n=0
     n=0
     lam,V,max_real,max_imag=Orr_Sommerfeld(N,Ra,Pr,Re,alpha,beta)
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.6/LICENSE` & `orr_sommerfeld_convmix_cgb-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.1.6/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.6/PKG-INFO` & `orr_sommerfeld_convmix_cgb-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orr_Sommerfeld_convmix_CGB
-Version: 0.1.6
+Version: 0.1.7
 Summary: Paquete para cálculo de autovalores y autofunciones.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Pablo Szuban <pablo.szuban@ib.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

