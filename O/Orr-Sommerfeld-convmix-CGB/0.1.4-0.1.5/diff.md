# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.1.4.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.1.5.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.1.4.tar` & `orr_sommerfeld_convmix_cgb-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.4/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.4/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.4/LICENSE
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.4/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/LICENSE
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.5/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.4/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.1.5/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,31 +204,34 @@
 
     return lam,V,max_real,max_imag
 def grafica_autovalores(N,Ra,Pr,Re,alpha,beta):
     lam,V,max_real,max_imag=Orr_Sommerfeld(N,Ra,Pr,Re,alpha,beta)
     imaginaria=lam.imag
     real=lam.real
     #Grafico comun
-    plt.style.use('ggplot')
+    #plt.style.use('ggplot')
 
     plt.ylim(-2,0.2)
     plt.xlim(0.1,1.5)
-    plt.scatter(real, imaginaria, marker='o', s=9)
+    plt.grid(color='lightgray')
+    plt.axhline(y=0, color='limegreen', linewidth=1.5, linestyle='-')
+    plt.scatter(real, imaginaria, marker='o', c='red' , s=9)
 
-    label_text = r'$Re= {:.2f}$' + "\n" + r'$Ra = {:.2f}$' + "\n" + r'$ Pr = {:.2f}$' + "\n" + r'$ \alpha = {:.2f}$' + "\n" + r'$ \beta= {:.2f}$'
+    label_text = r'$Re= {:.2f}$' + "\n" + r'$Ra = {:.2f}$' + "\n" + r'$ Pr = {:.2f}$' + "\n" + r'$ \alpha = {:.3f}$' + "\n" + r'$ \beta= {:.2f}$'
     label_text = label_text.format(Re, Ra, Pr, alpha, beta)
-    plt.text(0.2, -1.5, label_text, ha='left', va='center', fontsize=14, bbox=dict(facecolor=(0.9,0.9,0.9), edgecolor='gray', boxstyle='round'))
+    plt.text(0.2, -1.5, label_text, ha='left', va='center', fontsize=14, bbox=dict(facecolor='white', edgecolor='lightgray', boxstyle='round'))
     plt.text(max_real, max_imag+0.03, r'$(%0.5f,\,%0.5f)$' % (max_real, max_imag), ha='center', va='bottom', fontsize=10)
     plt.scatter(max_real, max_imag, c='orange', s=9)
 
     plt.xlabel(r'$c_r$', fontsize=18)
     plt.ylabel(r'$c_i$', fontsize=18)
     plt.title('Gráfico de autovalores', fontsize=18)
+    
 
-    #plt.savefig("Autovalores.png")
+    plt.savefig("Autovalores.png")
     plt.show()
 
     #-------------------------------------
     #Para hacer grafico interactivo, para que funcione descomentar bibliotecas arriba del todo
 
     df = pd.DataFrame({
         'real': real,
@@ -241,18 +244,19 @@
     layout = go.Layout(title=dict(text=titulo), xaxis=dict(title='r$c_{r}$',titlefont=dict(size=18), tickfont=dict(family='latex')), 
                                                                    yaxis=dict(title=r'$c_{i}$',titlefont=dict(size=18), tickfont=dict(family='latex')),
                                                                    plot_bgcolor='rgba(0,0,0,0.1)',
                                                                    title_x=0.5)
     fig = go.Figure(data=[traza], layout=layout)
     iplot(fig)
     return
-def vector_perturbaciones(N,lam,V,n,alpha,beta):
-  
+ def vector_perturbaciones(N,lam,V,n,alpha,beta):
+    
     D,D2,D4=Dmat(N)
-    #Chekeado que Dmat funciona bien   
+    #Chekeado que Dmat funciona bien
+    
     #Calculo parámetros de mis ecuaciones
     I=eye(N-1)
     k2=(alpha*alpha)+(beta*beta)
     k22=k2*k2
     
     v=V[0:(N-1),n]
     tita=V[(N-1):(2*(N-1)),n]
@@ -260,15 +264,15 @@
     #Expresión de u
     u= (1j*alpha*dot(D,v)/k2) + dot(beta/k2,eta)
     #Expresión de w
     w=((beta*u)-eta)/alpha
 
     # Falta agregar la presion y las expresiones individuales de w y u
     return  v,u,w,tita
-def normalizacion(v,u,w,tita):
+ def normalizacion(v,u,w,tita):
     vr=v.real
     vi=v.imag
     #Busca el valor de màxima norma de u
     norm= vr*vr+vi*vi
     i=np.where(abs(norm) == np.max(norm))
     #Para ese valor máximo, multiplico por un complejo c=a+bj/su fase sea cero y su norma sea 1
     a=vr[i]/norm[i]
@@ -277,17 +281,17 @@
     #b=-v[i]**2/(vr[i]*sqrt(norm[i]))
     c= a + (1j*b)   
     #Luego normalizo todas las autofunciones con el c hallado
     v=c*v
     u=c*u
     w=c*w
     tita=c*tita
-    return v,u,w,tita 
+    return v,u,w,tita  
 def grafica_autofunciones(N,Ra,Pr,Re,alpha,beta):
-    plt.style.use('ggplot')
+    #plt.style.use('ggplot')
     #Vector y
     D,y = cheb(N)
     #Vectores de perturbaciones para un autovalor dado. En este caso tomo el mayor de todos dado que Orr_Sommerfeld() las ordena y voy a elegir n=0
     n=0
     lam,V,max_real,max_imag=Orr_Sommerfeld(N,Ra,Pr,Re,alpha,beta)
 
     v,u,w,tita=vector_perturbaciones(N,lam,V,n,alpha,beta)
@@ -298,23 +302,27 @@
     realtita = (hstack(( [0.],tita.real , [0.])))
     imtita = (hstack(( [0.],tita.imag , [0.])))
     realu = (hstack(( [0.],u.real , [0.])))
     imu = (hstack(( [0.],u.imag , [0.])))
     realw = (hstack(( [0.],w.real , [0.])))
     imw = (hstack(( [0.],w.imag , [0.])))
 
-    plt.plot(y,realv,label= "$v_r(y)$")
-    plt.plot(y,imv,label= "$v_i(y)$")
-    plt.plot(y,realtita,"-",label= r'$\theta_{r}(y)$')
-    plt.plot(y,imtita,"-",label= r'$\theta_{i}(y)$')
-    plt.plot(y,realu,label= r'$u_{r}(y)$')
-    plt.plot(y,imu,label= r'$u_{i}(y)$')
+    plt.plot(y,realv,c='red',label= "$v_r(y)$")
+    plt.plot(y,imv,"--",c='red',label= "$v_i(y)$")
+    plt.plot(y,realtita,"-",c='blue',label= r'$\theta_{r}(y)$')
+    plt.plot(y,imtita,"--",c='blue',label= r'$\theta_{i}(y)$')
+    plt.plot(y,realu,c='lightgreen',label= r'$u_{r}(y)$')
+    plt.plot(y,imu,"--",c='lightgreen',label= r'$u_{i}(y)$')
+    #plt.plot(y,realw,c='pink',label= r'$w_{r}(y)$')
+    #plt.plot(y,imw,"--",c='pink',label= r'$w_{i}(y)$')
 
 
     plt.xlim(-1,1)
+    #plt.ylim(-41,45)
 
-    plt.ylabel(r'$y$', fontsize=18)
+    plt.xlabel(r'$y^{*}$', fontsize=18)
     title('Perfil de las perturbaciones',  fontsize=18)
     plt.legend()
-    #plt.savefig('u_poiseuille_Re5772a1b0.png', dpi=1000)
+    plt.grid(color='lightgray')
+    plt.savefig('ejemploautofunc1.png')
     plt.show()
     return
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.4/LICENSE` & `orr_sommerfeld_convmix_cgb-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.1.4/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.4/PKG-INFO` & `orr_sommerfeld_convmix_cgb-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orr_Sommerfeld_convmix_CGB
-Version: 0.1.4
+Version: 0.1.5
 Summary: Paquete para cálculo de autovalores y autofunciones.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Pablo Szuban <pablo.szuban@ib.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

