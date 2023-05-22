# Comparing `tmp/chainlit-0.2.0.tar.gz` & `tmp/chainlit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-0.2.0.tar", max compression
+gzip compressed data, was "chainlit-0.2.1.tar", max compression
```

## Comparing `chainlit-0.2.0.tar` & `chainlit-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2505 2023-05-19 15:35:08.664537 chainlit-0.2.0/README.md
--rw-r--r--   0        0        0    12867 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/__main__.py
--rw-r--r--   0        0        0      765 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/action.py
--rw-r--r--   0        0        0     3527 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/cli/__init__.py
--rw-r--r--   0        0        0     4093 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/cli/auth.py
--rw-r--r--   0        0        0     2594 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/cli/deploy.py
--rw-r--r--   0        0        0      716 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/cli/utils.py
--rw-r--r--   0        0        0     5278 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/client.py
--rw-r--r--   0        0        0     6426 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/config.py
--rw-r--r--   0        0        0     3293 2023-05-19 15:34:31.959792 chainlit-0.2.0/chainlit/element.py
--rw-r--r--   0        0        0  2071021 2023-05-19 15:35:35.025010 chainlit-0.2.0/chainlit/frontend/dist/assets/index-b6b4925e.js
--rw-r--r--   0        0        0     4317 2023-05-19 15:35:35.025010 chainlit-0.2.0/chainlit/frontend/dist/assets/index-bdffdaa0.css
--rw-r--r--   0        0        0     8889 2023-05-19 15:35:35.017010 chainlit-0.2.0/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
--rw-r--r--   0        0        0     8891 2023-05-19 15:35:35.025010 chainlit-0.2.0/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
--rw-r--r--   0        0        0     6455 2023-05-19 15:35:33.780986 chainlit-0.2.0/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0      772 2023-05-19 15:35:35.025010 chainlit-0.2.0/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      344 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/hello.py
--rw-r--r--   0        0        0        0 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/lc/__init__.py
--rw-r--r--   0        0        0     8077 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/lc/chainlit_handler.py
--rw-r--r--   0        0        0      863 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/lc/monkey.py
--rw-r--r--   0        0        0     5388 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/lc/new_monkey.py
--rw-r--r--   0        0        0     4129 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/lc/old_monkey.py
--rw-r--r--   0        0        0     1068 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/lc/utils.py
--rw-r--r--   0        0        0      398 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/logger.py
--rw-r--r--   0        0        0     1618 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/markdown.py
--rw-r--r--   0        0        0     6747 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/sdk.py
--rw-r--r--   0        0        0     9991 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/server.py
--rw-r--r--   0        0        0      813 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/session.py
--rw-r--r--   0        0        0     2017 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/telemetry.py
--rw-r--r--   0        0        0      965 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/types.py
--rw-r--r--   0        0        0     1145 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/user_session.py
--rw-r--r--   0        0        0      196 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/version.py
--rw-r--r--   0        0        0     1551 2023-05-19 15:34:31.963792 chainlit-0.2.0/chainlit/watch.py
--rw-r--r--   0        0        0     1018 2023-05-19 15:34:31.963792 chainlit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 chainlit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2505 2023-05-22 11:40:47.167350 chainlit-0.2.1/README.md
+-rw-r--r--   0        0        0    12876 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/__main__.py
+-rw-r--r--   0        0        0      765 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/action.py
+-rw-r--r--   0        0        0     3527 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0     4093 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/cli/auth.py
+-rw-r--r--   0        0        0     2594 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/cli/deploy.py
+-rw-r--r--   0        0        0      716 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/cli/utils.py
+-rw-r--r--   0        0        0     5278 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/client.py
+-rw-r--r--   0        0        0     6426 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/config.py
+-rw-r--r--   0        0        0     3293 2023-05-22 11:40:01.433992 chainlit-0.2.1/chainlit/element.py
+-rw-r--r--   0        0        0  2071080 2023-05-22 11:41:19.524269 chainlit-0.2.1/chainlit/frontend/dist/assets/index-03f89089.js
+-rw-r--r--   0        0        0     4317 2023-05-22 11:41:19.524269 chainlit-0.2.1/chainlit/frontend/dist/assets/index-bdffdaa0.css
+-rw-r--r--   0        0        0     8889 2023-05-22 11:41:19.520269 chainlit-0.2.1/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
+-rw-r--r--   0        0        0     8891 2023-05-22 11:41:19.524269 chainlit-0.2.1/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
+-rw-r--r--   0        0        0     6455 2023-05-22 11:41:17.996224 chainlit-0.2.1/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0      772 2023-05-22 11:41:19.524269 chainlit-0.2.1/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      344 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/hello.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/lc/__init__.py
+-rw-r--r--   0        0        0     8077 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/lc/chainlit_handler.py
+-rw-r--r--   0        0        0      863 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/lc/monkey.py
+-rw-r--r--   0        0        0     5388 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/lc/new_monkey.py
+-rw-r--r--   0        0        0     4129 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/lc/old_monkey.py
+-rw-r--r--   0        0        0     1068 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/lc/utils.py
+-rw-r--r--   0        0        0      398 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/logger.py
+-rw-r--r--   0        0        0     1618 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/markdown.py
+-rw-r--r--   0        0        0     6747 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/sdk.py
+-rw-r--r--   0        0        0     9991 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/server.py
+-rw-r--r--   0        0        0      813 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/session.py
+-rw-r--r--   0        0        0     2017 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/telemetry.py
+-rw-r--r--   0        0        0      965 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/types.py
+-rw-r--r--   0        0        0     1145 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/user_session.py
+-rw-r--r--   0        0        0      196 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/version.py
+-rw-r--r--   0        0        0     1551 2023-05-22 11:40:01.437991 chainlit-0.2.1/chainlit/watch.py
+-rw-r--r--   0        0        0     1018 2023-05-22 11:40:01.437991 chainlit-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 chainlit-0.2.1/PKG-INFO
```

### Comparing `chainlit-0.2.0/README.md` & `chainlit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/__init__.py` & `chainlit-0.2.1/chainlit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
         Callable[[], Any]: The decorated stop hook.
     """
 
     config.on_stop = wrap_user_function(func)
     return func
 
 
-def action(name: str) -> Callable:
+def action_callback(name: str) -> Callable:
     """
     Callback to call when an action is clicked in the UI.
 
     Args:
         func (Callable[[Action], Any]): The action callback to exexute. First parameter is the action.
     """
```

### Comparing `chainlit-0.2.0/chainlit/action.py` & `chainlit-0.2.1/chainlit/action.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/cli/__init__.py` & `chainlit-0.2.1/chainlit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/cli/auth.py` & `chainlit-0.2.1/chainlit/cli/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/cli/deploy.py` & `chainlit-0.2.1/chainlit/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/cli/utils.py` & `chainlit-0.2.1/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/client.py` & `chainlit-0.2.1/chainlit/client.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/config.py` & `chainlit-0.2.1/chainlit/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/element.py` & `chainlit-0.2.1/chainlit/element.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/frontend/dist/assets/index-b6b4925e.js` & `chainlit-0.2.1/chainlit/frontend/dist/assets/index-03f89089.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
     writable: !0,
     value: n
 }) : e[t] = n;
 var Kce = (e, t) => () => (t || e((t = {
     exports: {}
 }).exports, t), t.exports);
 var Ns = (e, t, n) => (Gce(e, typeof t != "symbol" ? t + "" : t, n), n);
-var gmt = Kce((fa, Ti) => {
+var gmt = Kce((da, Ti) => {
     function Yce(e, t) {
         for (var n = 0; n < t.length; n++) {
             const r = t[n];
             if (typeof r != "string" && !Array.isArray(r)) {
                 for (const i in r)
                     if (i !== "default" && !(i in e)) {
                         const a = Object.getOwnPropertyDescriptor(r, i);
@@ -511,15 +511,15 @@
             get exports() {
                 return Cc
             },
             set exports(e) {
                 Cc = e
             }
         },
-        va = {},
+        ma = {},
         QI = {},
         Sde = {
             get exports() {
                 return QI
             },
             set exports(e) {
                 QI = e
@@ -778,15 +778,15 @@
      *
      * Copyright (c) Facebook, Inc. and its affiliates.
      *
      * This source code is licensed under the MIT license found in the
      * LICENSE file in the root directory of this source tree.
      */
     var U9 = k,
-        ma = QI;
+        ga = QI;
 
     function Qe(e) {
         for (var t = "https://reactjs.org/docs/error-decoder.html?invariant=" + e, n = 1; n < arguments.length; n++) t += "&args[]=" + encodeURIComponent(arguments[n]);
         return "Minified React error #" + e + "; visit " + t + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
     }
     var z9 = new Set,
         um = {};
@@ -1644,25 +1644,25 @@
         for (e = e.child; e !== null;) {
             var t = o8(e);
             if (t !== null) return t;
             e = e.sibling
         }
         return null
     }
-    var s8 = ma.unstable_scheduleCallback,
-        CB = ma.unstable_cancelCallback,
-        Mde = ma.unstable_shouldYield,
-        Pde = ma.unstable_requestPaint,
-        br = ma.unstable_now,
-        $de = ma.unstable_getCurrentPriorityLevel,
-        lL = ma.unstable_ImmediatePriority,
-        l8 = ma.unstable_UserBlockingPriority,
-        GE = ma.unstable_NormalPriority,
-        Bde = ma.unstable_LowPriority,
-        u8 = ma.unstable_IdlePriority,
+    var s8 = ga.unstable_scheduleCallback,
+        CB = ga.unstable_cancelCallback,
+        Mde = ga.unstable_shouldYield,
+        Pde = ga.unstable_requestPaint,
+        br = ga.unstable_now,
+        $de = ga.unstable_getCurrentPriorityLevel,
+        lL = ga.unstable_ImmediatePriority,
+        l8 = ga.unstable_UserBlockingPriority,
+        GE = ga.unstable_NormalPriority,
+        Bde = ga.unstable_LowPriority,
+        u8 = ga.unstable_IdlePriority,
         n0 = null,
         rs = null;
 
     function Ude(e) {
         if (rs && typeof rs.onCommitFiberRoot == "function") try {
             rs.onCommitFiberRoot(n0, e, void 0, (e.current.flags & 128) === 128)
         } catch {}
@@ -1939,15 +1939,15 @@
     }
 
     function Yde() {
         mO = !1, Jl !== null && sE(Jl) && (Jl = null), eu !== null && sE(eu) && (eu = null), tu !== null && sE(tu) && (tu = null), fm.forEach(RB), pm.forEach(RB)
     }
 
     function Oh(e, t) {
-        e.blockedOn === t && (e.blockedOn = null, mO || (mO = !0, ma.unstable_scheduleCallback(ma.unstable_NormalPriority, Yde)))
+        e.blockedOn === t && (e.blockedOn = null, mO || (mO = !0, ga.unstable_scheduleCallback(ga.unstable_NormalPriority, Yde)))
     }
 
     function hm(e) {
         function t(i) {
             return Oh(i, e)
         }
         if (0 < eb.length) {
@@ -2132,15 +2132,15 @@
         return !0
     }
 
     function kB() {
         return !1
     }
 
-    function ya(e) {
+    function va(e) {
         function t(n, r, i, a, o) {
             this._reactName = n, this._targetInst = i, this.type = r, this.nativeEvent = a, this.target = o, this.currentTarget = null;
             for (var s in e) e.hasOwnProperty(s) && (n = e[s], this[s] = n ? n(a) : a[s]);
             return this.isDefaultPrevented = (a.defaultPrevented != null ? a.defaultPrevented : a.returnValue === !1) ? tb : kB, this.isPropagationStopped = kB, this
         }
         return rr(t.prototype, {
             preventDefault: function() {
@@ -2162,20 +2162,20 @@
             cancelable: 0,
             timeStamp: function(e) {
                 return e.timeStamp || Date.now()
             },
             defaultPrevented: 0,
             isTrusted: 0
         },
-        pL = ya(yp),
+        pL = va(yp),
         Qm = rr({}, yp, {
             view: 0,
             detail: 0
         }),
-        Qde = ya(Qm),
+        Qde = va(Qm),
         Px, $x, Nh, r0 = rr({}, Qm, {
             screenX: 0,
             screenY: 0,
             clientX: 0,
             clientY: 0,
             pageX: 0,
             pageY: 0,
@@ -2192,39 +2192,39 @@
             movementX: function(e) {
                 return "movementX" in e ? e.movementX : (e !== Nh && (Nh && e.type === "mousemove" ? (Px = e.screenX - Nh.screenX, $x = e.screenY - Nh.screenY) : $x = Px = 0, Nh = e), Px)
             },
             movementY: function(e) {
                 return "movementY" in e ? e.movementY : $x
             }
         }),
-        IB = ya(r0),
+        IB = va(r0),
         Jde = rr({}, r0, {
             dataTransfer: 0
         }),
-        efe = ya(Jde),
+        efe = va(Jde),
         tfe = rr({}, Qm, {
             relatedTarget: 0
         }),
-        Bx = ya(tfe),
+        Bx = va(tfe),
         nfe = rr({}, yp, {
             animationName: 0,
             elapsedTime: 0,
             pseudoElement: 0
         }),
-        rfe = ya(nfe),
+        rfe = va(nfe),
         ife = rr({}, yp, {
             clipboardData: function(e) {
                 return "clipboardData" in e ? e.clipboardData : window.clipboardData
             }
         }),
-        afe = ya(ife),
+        afe = va(ife),
         ofe = rr({}, yp, {
             data: 0
         }),
-        OB = ya(ofe),
+        OB = va(ofe),
         sfe = {
             Esc: "Escape",
             Spacebar: " ",
             Left: "ArrowLeft",
             Up: "ArrowUp",
             Right: "ArrowRight",
             Down: "ArrowDown",
@@ -2311,56 +2311,56 @@
             keyCode: function(e) {
                 return e.type === "keydown" || e.type === "keyup" ? e.keyCode : 0
             },
             which: function(e) {
                 return e.type === "keypress" ? uE(e) : e.type === "keydown" || e.type === "keyup" ? e.keyCode : 0
             }
         }),
-        ffe = ya(dfe),
+        ffe = va(dfe),
         pfe = rr({}, r0, {
             pointerId: 0,
             width: 0,
             height: 0,
             pressure: 0,
             tangentialPressure: 0,
             tiltX: 0,
             tiltY: 0,
             twist: 0,
             pointerType: 0,
             isPrimary: 0
         }),
-        NB = ya(pfe),
+        NB = va(pfe),
         hfe = rr({}, Qm, {
             touches: 0,
             targetTouches: 0,
             changedTouches: 0,
             altKey: 0,
             metaKey: 0,
             ctrlKey: 0,
             shiftKey: 0,
             getModifierState: hL
         }),
-        gfe = ya(hfe),
+        gfe = va(hfe),
         mfe = rr({}, yp, {
             propertyName: 0,
             elapsedTime: 0,
             pseudoElement: 0
         }),
-        vfe = ya(mfe),
+        vfe = va(mfe),
         yfe = rr({}, r0, {
             deltaX: function(e) {
                 return "deltaX" in e ? e.deltaX : "wheelDeltaX" in e ? -e.wheelDeltaX : 0
             },
             deltaY: function(e) {
                 return "deltaY" in e ? e.deltaY : "wheelDeltaY" in e ? -e.wheelDeltaY : "wheelDelta" in e ? -e.wheelDelta : 0
             },
             deltaZ: 0,
             deltaMode: 0
         }),
-        bfe = ya(yfe),
+        bfe = va(yfe),
         Efe = [9, 13, 27, 32],
         gL = Ys && "CompositionEvent" in window,
         Mg = null;
     Ys && "documentMode" in document && (Mg = document.documentMode);
     var Sfe = Ys && "TextEvent" in window && !Mg,
         b8 = Ys && (!gL || Mg && 8 < Mg && 11 >= Mg),
         DB = String.fromCharCode(32),
@@ -3234,108 +3234,108 @@
         e.return !== null && (tc(e, 1), P8(e, 1, 0))
     }
 
     function yL(e) {
         for (; e === tS;) tS = pf[--hf], pf[hf] = null, nS = pf[--hf], pf[hf] = null;
         for (; e === Rc;) Rc = Fa[--Ma], Fa[Ma] = null, Hs = Fa[--Ma], Fa[Ma] = null, Vs = Fa[--Ma], Fa[Ma] = null
     }
-    var pa = null,
-        da = null,
+    var fa = null,
+        ca = null,
         Gn = !1,
         xo = null;
 
     function $8(e, t) {
         var n = za(5, null, null, 0);
         n.elementType = "DELETED", n.stateNode = t, n.return = e, t = e.deletions, t === null ? (e.deletions = [n], e.flags |= 16) : t.push(n)
     }
 
     function YB(e, t) {
         switch (e.tag) {
             case 5:
                 var n = e.type;
-                return t = t.nodeType !== 1 || n.toLowerCase() !== t.nodeName.toLowerCase() ? null : t, t !== null ? (e.stateNode = t, pa = e, da = nu(t.firstChild), !0) : !1;
+                return t = t.nodeType !== 1 || n.toLowerCase() !== t.nodeName.toLowerCase() ? null : t, t !== null ? (e.stateNode = t, fa = e, ca = nu(t.firstChild), !0) : !1;
             case 6:
-                return t = e.pendingProps === "" || t.nodeType !== 3 ? null : t, t !== null ? (e.stateNode = t, pa = e, da = null, !0) : !1;
+                return t = e.pendingProps === "" || t.nodeType !== 3 ? null : t, t !== null ? (e.stateNode = t, fa = e, ca = null, !0) : !1;
             case 13:
                 return t = t.nodeType !== 8 ? null : t, t !== null ? (n = Rc !== null ? {
                     id: Vs,
                     overflow: Hs
                 } : null, e.memoizedState = {
                     dehydrated: t,
                     treeContext: n,
                     retryLane: 1073741824
-                }, n = za(18, null, null, 0), n.stateNode = t, n.return = e, e.child = n, pa = e, da = null, !0) : !1;
+                }, n = za(18, null, null, 0), n.stateNode = t, n.return = e, e.child = n, fa = e, ca = null, !0) : !1;
             default:
                 return !1
         }
     }
 
     function CO(e) {
         return (e.mode & 1) !== 0 && (e.flags & 128) === 0
     }
 
     function AO(e) {
         if (Gn) {
-            var t = da;
+            var t = ca;
             if (t) {
                 var n = t;
                 if (!YB(e, t)) {
                     if (CO(e)) throw Error(Qe(418));
                     t = nu(n.nextSibling);
-                    var r = pa;
-                    t && YB(e, t) ? $8(r, n) : (e.flags = e.flags & -4097 | 2, Gn = !1, pa = e)
+                    var r = fa;
+                    t && YB(e, t) ? $8(r, n) : (e.flags = e.flags & -4097 | 2, Gn = !1, fa = e)
                 }
             } else {
                 if (CO(e)) throw Error(Qe(418));
-                e.flags = e.flags & -4097 | 2, Gn = !1, pa = e
+                e.flags = e.flags & -4097 | 2, Gn = !1, fa = e
             }
         }
     }
 
     function XB(e) {
         for (e = e.return; e !== null && e.tag !== 5 && e.tag !== 3 && e.tag !== 13;) e = e.return;
-        pa = e
+        fa = e
     }
 
     function ab(e) {
-        if (e !== pa) return !1;
+        if (e !== fa) return !1;
         if (!Gn) return XB(e), Gn = !0, !1;
         var t;
-        if ((t = e.tag !== 3) && !(t = e.tag !== 5) && (t = e.type, t = t !== "head" && t !== "body" && !_O(e.type, e.memoizedProps)), t && (t = da)) {
+        if ((t = e.tag !== 3) && !(t = e.tag !== 5) && (t = e.type, t = t !== "head" && t !== "body" && !_O(e.type, e.memoizedProps)), t && (t = ca)) {
             if (CO(e)) throw B8(), Error(Qe(418));
             for (; t;) $8(e, t), t = nu(t.nextSibling)
         }
         if (XB(e), e.tag === 13) {
             if (e = e.memoizedState, e = e !== null ? e.dehydrated : null, !e) throw Error(Qe(317));
             e: {
                 for (e = e.nextSibling, t = 0; e;) {
                     if (e.nodeType === 8) {
                         var n = e.data;
                         if (n === "/$") {
                             if (t === 0) {
-                                da = nu(e.nextSibling);
+                                ca = nu(e.nextSibling);
                                 break e
                             }
                             t--
                         } else n !== "$" && n !== "$!" && n !== "$?" || t++
                     }
                     e = e.nextSibling
                 }
-                da = null
+                ca = null
             }
-        } else da = pa ? nu(e.stateNode.nextSibling) : null;
+        } else ca = fa ? nu(e.stateNode.nextSibling) : null;
         return !0
     }
 
     function B8() {
-        for (var e = da; e;) e = nu(e.nextSibling)
+        for (var e = ca; e;) e = nu(e.nextSibling)
     }
 
     function Gf() {
-        da = pa = null, Gn = !1
+        ca = fa = null, Gn = !1
     }
 
     function bL(e) {
         xo === null ? xo = [e] : xo.push(e)
     }
     var Hfe = il.ReactCurrentBatchConfig;
 
@@ -4577,28 +4577,28 @@
             i = r.children,
             a = e !== null ? e.memoizedState : null;
         if (r.mode === "hidden")
             if (!(t.mode & 1)) t.memoizedState = {
                 baseLanes: 0,
                 cachePool: null,
                 transitions: null
-            }, Fn(vf, la), la |= n;
+            }, Fn(vf, sa), sa |= n;
             else {
                 if (!(n & 1073741824)) return e = a !== null ? a.baseLanes | n : n, t.lanes = t.childLanes = 1073741824, t.memoizedState = {
                     baseLanes: e,
                     cachePool: null,
                     transitions: null
-                }, t.updateQueue = null, Fn(vf, la), la |= e, null;
+                }, t.updateQueue = null, Fn(vf, sa), sa |= e, null;
                 t.memoizedState = {
                     baseLanes: 0,
                     cachePool: null,
                     transitions: null
-                }, r = a !== null ? a.baseLanes : n, Fn(vf, la), la |= r
+                }, r = a !== null ? a.baseLanes : n, Fn(vf, sa), sa |= r
             }
-        else a !== null ? (r = a.baseLanes | n, t.memoizedState = null) : r = n, Fn(vf, la), la |= r;
+        else a !== null ? (r = a.baseLanes | n, t.memoizedState = null) : r = n, Fn(vf, sa), sa |= r;
         return wi(e, t, i, n), t.child
     }
 
     function m7(e, t) {
         var n = t.ref;
         (e === null && n !== null || e !== null && e.ref !== n) && (t.flags |= 512, t.flags |= 2097152)
     }
@@ -4755,15 +4755,15 @@
                     default:
                         i = 0
                 }
                 i = i & (r.suspendedLanes | o) ? 0 : i, i !== 0 && i !== a.retryLane && (a.retryLane = i, Zs(e, i), Ao(r, e, i, -1))
             }
             return BL(), r = Jx(Error(Qe(421))), sb(e, t, o, r)
         }
-        return i.data === "$?" ? (t.flags |= 128, t.child = e.child, t = hpe.bind(null, e), i._reactRetry = t, null) : (e = a.treeContext, da = nu(i.nextSibling), pa = t, Gn = !0, xo = null, e !== null && (Fa[Ma++] = Vs, Fa[Ma++] = Hs, Fa[Ma++] = Rc, Vs = e.id, Hs = e.overflow, Rc = t), t = DL(t, r.children), t.flags |= 4096, t)
+        return i.data === "$?" ? (t.flags |= 128, t.child = e.child, t = hpe.bind(null, e), i._reactRetry = t, null) : (e = a.treeContext, ca = nu(i.nextSibling), fa = t, Gn = !0, xo = null, e !== null && (Fa[Ma++] = Vs, Fa[Ma++] = Hs, Fa[Ma++] = Rc, Vs = e.id, Hs = e.overflow, Rc = t), t = DL(t, r.children), t.flags |= 4096, t)
     }
 
     function dU(e, t, n) {
         e.lanes |= t;
         var r = e.alternate;
         r !== null && (r.lanes |= t), RO(e.return, t, n)
     }
@@ -5144,28 +5144,28 @@
                 }
                 return di(t), null;
             case 6:
                 if (e && t.stateNode != null) _7(e, t, e.memoizedProps, r);
                 else {
                     if (typeof r != "string" && t.stateNode === null) throw Error(Qe(166));
                     if (n = hc(Sm.current), hc(is.current), ab(t)) {
-                        if (r = t.stateNode, n = t.memoizedProps, r[Jo] = t, (a = r.nodeValue !== n) && (e = pa, e !== null)) switch (e.tag) {
+                        if (r = t.stateNode, n = t.memoizedProps, r[Jo] = t, (a = r.nodeValue !== n) && (e = fa, e !== null)) switch (e.tag) {
                             case 3:
                                 ib(r.nodeValue, n, (e.mode & 1) !== 0);
                                 break;
                             case 5:
                                 e.memoizedProps.suppressHydrationWarning !== !0 && ib(r.nodeValue, n, (e.mode & 1) !== 0)
                         }
                         a && (t.flags |= 4)
                     } else r = (n.nodeType === 9 ? n : n.ownerDocument).createTextNode(r), r[Jo] = t, t.stateNode = r
                 }
                 return di(t), null;
             case 13:
                 if (qn(er), r = t.memoizedState, e === null || e.memoizedState !== null && e.memoizedState.dehydrated !== null) {
-                    if (Gn && da !== null && t.mode & 1 && !(t.flags & 128)) B8(), Gf(), t.flags |= 98560, a = !1;
+                    if (Gn && ca !== null && t.mode & 1 && !(t.flags & 128)) B8(), Gf(), t.flags |= 98560, a = !1;
                     else if (a = ab(t), r !== null && r.dehydrated !== null) {
                         if (e === null) {
                             if (!a) throw Error(Qe(318));
                             if (a = t.memoizedState, a = a !== null ? a.dehydrated : null, !a) throw Error(Qe(317));
                             a[Jo] = t
                         } else Gf(), !(t.flags & 128) && (t.memoizedState = null), t.flags |= 4;
                         di(t), a = !1
@@ -5203,15 +5203,15 @@
                             if (t.flags |= 128, r = !0, n = e.updateQueue, n !== null && (t.updateQueue = n, t.flags |= 4), Lh(a, !0), a.tail === null && a.tailMode === "hidden" && !o.alternate && !Gn) return di(t), null
                         } else 2 * br() - a.renderingStartTime > Zf && n !== 1073741824 && (t.flags |= 128, r = !0, Lh(a, !1), t.lanes = 4194304);
                     a.isBackwards ? (o.sibling = t.child, t.child = o) : (n = a.last, n !== null ? n.sibling = o : t.child = o, a.last = o)
                 }
                 return a.tail !== null ? (t = a.tail, a.rendering = t, a.tail = t.sibling, a.renderingStartTime = br(), t.sibling = null, n = er.current, Fn(er, r ? n & 1 | 2 : n & 1), t) : (di(t), null);
             case 22:
             case 23:
-                return $L(), r = t.memoizedState !== null, e !== null && e.memoizedState !== null !== r && (t.flags |= 8192), r && t.mode & 1 ? la & 1073741824 && (di(t), t.subtreeFlags & 6 && (t.flags |= 8192)) : di(t), null;
+                return $L(), r = t.memoizedState !== null, e !== null && e.memoizedState !== null !== r && (t.flags |= 8192), r && t.mode & 1 ? sa & 1073741824 && (di(t), t.subtreeFlags & 6 && (t.flags |= 8192)) : di(t), null;
             case 24:
                 return null;
             case 25:
                 return null
         }
         throw Error(Qe(156, t.tag))
     }
@@ -5948,15 +5948,15 @@
         uS = il.ReactCurrentDispatcher,
         LL = il.ReactCurrentOwner,
         qa = il.ReactCurrentBatchConfig,
         sn = 0,
         qr = null,
         Ar = null,
         ri = 0,
-        la = 0,
+        sa = 0,
         vf = Su(0),
         Dr = 0,
         Tm = null,
         Ic = 0,
         d0 = 0,
         FL = 0,
         zg = null,
@@ -6170,15 +6170,15 @@
             if (qa.transition = null, wn = 1, e) return e()
         } finally {
             wn = r, qa.transition = n, sn = t, !(sn & 6) && _u()
         }
     }
 
     function $L() {
-        la = vf.current, qn(vf)
+        sa = vf.current, qn(vf)
     }
 
     function bc(e, t) {
         e.finishedWork = null, e.finishedLanes = 0;
         var n = e.timeoutHandle;
         if (n !== -1 && (e.timeoutHandle = -1, Bfe(n)), Ar !== null)
             for (n = Ar.return; n !== null;) {
@@ -6207,15 +6207,15 @@
                         break;
                     case 22:
                     case 23:
                         $L()
                 }
                 n = n.return
             }
-        if (qr = e, Ar = e = ou(e.current, null), ri = la = t, Dr = 0, Tm = null, FL = d0 = Ic = 0, Pi = zg = null, pc !== null) {
+        if (qr = e, Ar = e = ou(e.current, null), ri = sa = t, Dr = 0, Tm = null, FL = d0 = Ic = 0, Pi = zg = null, pc !== null) {
             for (t = 0; t < pc.length; t++)
                 if (n = pc[t], r = n.interleaved, r !== null) {
                     n.interleaved = null;
                     var i = r.next,
                         a = n.pending;
                     if (a !== null) {
                         var o = a.next;
@@ -6341,15 +6341,15 @@
     }
 
     function dpe() {
         for (; Ar !== null && !Mde();) O7(Ar)
     }
 
     function O7(e) {
-        var t = L7(e.alternate, e, la);
+        var t = L7(e.alternate, e, sa);
         e.memoizedProps = e.pendingProps, t === null ? N7(e) : Ar = t, LL.current = null
     }
 
     function N7(e) {
         var t = e;
         do {
             var n = t.alternate;
@@ -6359,15 +6359,15 @@
                     return
                 }
                 if (e !== null) e.flags |= 32768, e.subtreeFlags = 0, e.deletions = null;
                 else {
                     Dr = 6, Ar = null;
                     return
                 }
-            } else if (n = rpe(n, t, la), n !== null) {
+            } else if (n = rpe(n, t, sa), n !== null) {
                 Ar = n;
                 return
             }
             if (t = t.sibling, t !== null) {
                 Ar = t;
                 return
             }
@@ -6644,15 +6644,15 @@
                             }, t.updateQueue.baseState = a, t.memoizedState = a, t.flags & 256) {
                             i = Xf(Error(Qe(423)), t), t = cU(e, t, r, n, i);
                             break e
                         } else if (r !== i) {
                         i = Xf(Error(Qe(424)), t), t = cU(e, t, r, n, i);
                         break e
                     } else
-                        for (da = nu(t.stateNode.containerInfo.firstChild), pa = t, Gn = !0, xo = null, n = H8(t, null, r, n), t.child = n; n;) n.flags = n.flags & -3 | 4096, n = n.sibling;
+                        for (ca = nu(t.stateNode.containerInfo.firstChild), fa = t, Gn = !0, xo = null, n = H8(t, null, r, n), t.child = n; n;) n.flags = n.flags & -3 | 4096, n = n.sibling;
                     else {
                         if (Gf(), r === i) {
                             t = Qs(e, t, n);
                             break e
                         }
                         wi(e, t, r, n)
                     }
@@ -7132,79 +7132,79 @@
         };
     if (typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ < "u") {
         var cb = __REACT_DEVTOOLS_GLOBAL_HOOK__;
         if (!cb.isDisabled && cb.supportsFiber) try {
             n0 = cb.inject(wpe), rs = cb
         } catch {}
     }
-    va.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = _pe;
-    va.createPortal = function(e, t) {
+    ma.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = _pe;
+    ma.createPortal = function(e, t) {
         var n = 2 < arguments.length && arguments[2] !== void 0 ? arguments[2] : null;
         if (!VL(t)) throw Error(Qe(200));
         return bpe(e, t, null, n)
     };
-    va.createRoot = function(e, t) {
+    ma.createRoot = function(e, t) {
         if (!VL(e)) throw Error(Qe(299));
         var n = !1,
             r = "",
             i = $7;
         return t != null && (t.unstable_strictMode === !0 && (n = !0), t.identifierPrefix !== void 0 && (r = t.identifierPrefix), t.onRecoverableError !== void 0 && (i = t.onRecoverableError)), t = zL(e, 1, !1, null, null, n, !1, r, i), e[Xs] = t.current, vm(e.nodeType === 8 ? e.parentNode : e), new qL(t)
     };
-    va.findDOMNode = function(e) {
+    ma.findDOMNode = function(e) {
         if (e == null) return null;
         if (e.nodeType === 1) return e;
         var t = e._reactInternals;
         if (t === void 0) throw typeof e.render == "function" ? Error(Qe(188)) : (e = Object.keys(e).join(","), Error(Qe(268, e)));
         return e = a8(t), e = e === null ? null : e.stateNode, e
     };
-    va.flushSync = function(e) {
+    ma.flushSync = function(e) {
         return Oc(e)
     };
-    va.hydrate = function(e, t, n) {
+    ma.hydrate = function(e, t, n) {
         if (!g0(t)) throw Error(Qe(200));
         return m0(null, e, t, !0, n)
     };
-    va.hydrateRoot = function(e, t, n) {
+    ma.hydrateRoot = function(e, t, n) {
         if (!VL(e)) throw Error(Qe(405));
         var r = n != null && n.hydratedSources || null,
             i = !1,
             a = "",
             o = $7;
         if (n != null && (n.unstable_strictMode === !0 && (i = !0), n.identifierPrefix !== void 0 && (a = n.identifierPrefix), n.onRecoverableError !== void 0 && (o = n.onRecoverableError)), t = P7(t, null, e, 1, n ?? null, i, !1, a, o), e[Xs] = t.current, vm(e), r)
             for (e = 0; e < r.length; e++) n = r[e], i = n._getVersion, i = i(n._source), t.mutableSourceEagerHydrationData == null ? t.mutableSourceEagerHydrationData = [n, i] : t.mutableSourceEagerHydrationData.push(n, i);
         return new h0(t)
     };
-    va.render = function(e, t, n) {
+    ma.render = function(e, t, n) {
         if (!g0(t)) throw Error(Qe(200));
         return m0(null, e, t, !1, n)
     };
-    va.unmountComponentAtNode = function(e) {
+    ma.unmountComponentAtNode = function(e) {
         if (!g0(e)) throw Error(Qe(40));
         return e._reactRootContainer ? (Oc(function() {
             m0(null, null, e, !1, function() {
                 e._reactRootContainer = null, e[Xs] = null
             })
         }), !0) : !1
     };
-    va.unstable_batchedUpdates = PL;
-    va.unstable_renderSubtreeIntoContainer = function(e, t, n, r) {
+    ma.unstable_batchedUpdates = PL;
+    ma.unstable_renderSubtreeIntoContainer = function(e, t, n, r) {
         if (!g0(n)) throw Error(Qe(200));
         if (e == null || e._reactInternals === void 0) throw Error(Qe(38));
         return m0(e, t, n, !1, r)
     };
-    va.version = "18.2.0-next-9e3b772b8-20220608";
+    ma.version = "18.2.0-next-9e3b772b8-20220608";
     (function(e) {
         function t() {
             if (!(typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ > "u" || typeof __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE != "function")) try {
                 __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE(t)
             } catch (n) {
                 console.error(n)
             }
         }
-        t(), e.exports = va
+        t(), e.exports = ma
     })(Ede);
     const Sg = XD(Cc);
     var _U = Cc;
     ZI.createRoot = _U.createRoot, ZI.hydrateRoot = _U.hydrateRoot;
 
     function xpe(e) {
         const t = new Error(e);
@@ -11497,15 +11497,15 @@
             useRecoilTransactionObserver_UNSTABLE: iEe,
             snapshot_UNSTABLE: Wbe,
             useRetain: nF,
             retentionZone: Hbe
         },
         dEe = lv.RecoilRoot,
         oi = lv.atom,
-        Yt = lv.useRecoilValue,
+        Xt = lv.useRecoilValue,
         Wi = lv.useRecoilState,
         ti = lv.useSetRecoilState;
     const fEe = {
             black: "#000",
             white: "#fff"
         },
         Cm = fEe,
@@ -12249,15 +12249,15 @@
         return Cr
     }
 
     function iSe() {
         return Cr = Gi > 0 ? ei(Sp, --Gi) : 0, rp--, Cr === 10 && (rp = 1, Y0--), Cr
     }
 
-    function ha() {
+    function pa() {
         return Cr = Gi < hX ? ei(Sp, Gi++) : 0, rp++, Cr === 10 && (rp = 1, Y0++), Cr
     }
 
     function as() {
         return ei(Sp, Gi)
     }
 
@@ -12312,58 +12312,58 @@
 
     function bE(e) {
         return pX(dv(Gi - 1, rN(e === 91 ? e + 2 : e === 40 ? e + 1 : e)))
     }
 
     function aSe(e) {
         for (;
-            (Cr = as()) && Cr < 33;) ha();
+            (Cr = as()) && Cr < 33;) pa();
         return km(e) > 2 || km(Cr) > 3 ? "" : " "
     }
 
     function oSe(e, t) {
-        for (; --t && ha() && !(Cr < 48 || Cr > 102 || Cr > 57 && Cr < 65 || Cr > 70 && Cr < 97););
-        return dv(e, yE() + (t < 6 && as() == 32 && ha() == 32))
+        for (; --t && pa() && !(Cr < 48 || Cr > 102 || Cr > 57 && Cr < 65 || Cr > 70 && Cr < 97););
+        return dv(e, yE() + (t < 6 && as() == 32 && pa() == 32))
     }
 
     function rN(e) {
-        for (; ha();) switch (Cr) {
+        for (; pa();) switch (Cr) {
             case e:
                 return Gi;
             case 34:
             case 39:
                 e !== 34 && e !== 39 && rN(Cr);
                 break;
             case 40:
                 e === 41 && rN(e);
                 break;
             case 92:
-                ha();
+                pa();
                 break
         }
         return Gi
     }
 
     function sSe(e, t) {
-        for (; ha() && e + Cr !== 47 + 10;)
+        for (; pa() && e + Cr !== 47 + 10;)
             if (e + Cr === 42 + 42 && as() === 47) break;
-        return "/*" + dv(t, Gi - 1) + "*" + K0(e === 47 ? e : ha())
+        return "/*" + dv(t, Gi - 1) + "*" + K0(e === 47 ? e : pa())
     }
 
     function lSe(e) {
-        for (; !km(as());) ha();
+        for (; !km(as());) pa();
         return dv(e, Gi)
     }
 
     function uSe(e) {
         return mX(EE("", null, null, null, [""], e = gX(e), 0, [0], e))
     }
 
     function EE(e, t, n, r, i, a, o, s, l) {
-        for (var u = 0, d = 0, p = o, f = 0, g = 0, m = 0, y = 1, _ = 1, E = 1, b = 0, S = "", x = i, C = a, A = r, I = S; _;) switch (m = b, b = ha()) {
+        for (var u = 0, d = 0, p = o, f = 0, g = 0, m = 0, y = 1, _ = 1, E = 1, b = 0, S = "", x = i, C = a, A = r, I = S; _;) switch (m = b, b = pa()) {
             case 40:
                 if (m != 108 && ei(I, p - 1) == 58) {
                     nN(I += bn(bE(b), "&", "&\f"), "&\f") != -1 && (E = -1);
                     break
                 }
             case 34:
             case 39:
@@ -12379,15 +12379,15 @@
             case 92:
                 I += oSe(yE() - 1, 7);
                 continue;
             case 47:
                 switch (as()) {
                     case 42:
                     case 47:
-                        mb(cSe(sSe(ha(), yE()), t, n), l);
+                        mb(cSe(sSe(pa(), yE()), t, n), l);
                         break;
                     default:
                         I += "/"
                 }
                 break;
             case 123 * y:
                 s[u++] = Yo(I) * E;
@@ -12429,15 +12429,15 @@
                     case 38:
                         E = d > 0 ? 1 : (I += "\f", -1);
                         break;
                     case 44:
                         s[u++] = (Yo(I) - 1) * E, E = 1;
                         break;
                     case 64:
-                        as() === 45 && (I += bE(ha())), f = as(), d = p = Yo(S = I += lSe(yE())), b++;
+                        as() === 45 && (I += bE(pa())), f = as(), d = p = Yo(S = I += lSe(yE())), b++;
                         break;
                     case 45:
                         m === 45 && Yo(I) == 2 && (y = 0)
                 }
         }
         return a
     }
@@ -12486,15 +12486,15 @@
 
     function pSe(e) {
         return function(t) {
             t.root || (t = t.return) && e(t)
         }
     }
     var hSe = function(t, n, r) {
-            for (var i = 0, a = 0; i = a, a = as(), i === 38 && a === 12 && (n[r] = 1), !km(a);) ha();
+            for (var i = 0, a = 0; i = a, a = as(), i === 38 && a === 12 && (n[r] = 1), !km(a);) pa();
             return dv(t, Gi)
         },
         gSe = function(t, n) {
             var r = -1,
                 i = 44;
             do switch (km(i)) {
                 case 0:
@@ -12507,15 +12507,15 @@
                     if (i === 44) {
                         t[++r] = as() === 58 ? "&\f" : "", n[r] = t[r].length;
                         break
                     }
                 default:
                     t[r] += K0(i)
             }
-            while (i = ha());
+            while (i = pa());
             return t
         },
         mSe = function(t, n) {
             return mX(gSe(gX(t), n))
         },
         ZU = new WeakMap,
         vSe = function(t) {
@@ -12757,15 +12757,15 @@
         a_ = Vr ? Symbol.for("react.memo") : 60115,
         o_ = Vr ? Symbol.for("react.lazy") : 60116,
         xSe = Vr ? Symbol.for("react.block") : 60121,
         TSe = Vr ? Symbol.for("react.fundamental") : 60117,
         CSe = Vr ? Symbol.for("react.responder") : 60118,
         ASe = Vr ? Symbol.for("react.scope") : 60119;
 
-    function ba(e) {
+    function ya(e) {
         if (typeof e == "object" && e !== null) {
             var t = e.$$typeof;
             switch (t) {
                 case mF:
                     switch (e = e.type, e) {
                         case yF:
                         case n_:
@@ -12789,15 +12789,15 @@
                 case vF:
                     return t
             }
         }
     }
 
     function yX(e) {
-        return ba(e) === n_
+        return ya(e) === n_
     }
     Tn.AsyncMode = yF;
     Tn.ConcurrentMode = n_;
     Tn.ContextConsumer = t_;
     Tn.ContextProvider = e_;
     Tn.Element = mF;
     Tn.ForwardRef = r_;
@@ -12805,54 +12805,54 @@
     Tn.Lazy = o_;
     Tn.Memo = a_;
     Tn.Portal = vF;
     Tn.Profiler = J0;
     Tn.StrictMode = Q0;
     Tn.Suspense = i_;
     Tn.isAsyncMode = function(e) {
-        return yX(e) || ba(e) === yF
+        return yX(e) || ya(e) === yF
     };
     Tn.isConcurrentMode = yX;
     Tn.isContextConsumer = function(e) {
-        return ba(e) === t_
+        return ya(e) === t_
     };
     Tn.isContextProvider = function(e) {
-        return ba(e) === e_
+        return ya(e) === e_
     };
     Tn.isElement = function(e) {
         return typeof e == "object" && e !== null && e.$$typeof === mF
     };
     Tn.isForwardRef = function(e) {
-        return ba(e) === r_
+        return ya(e) === r_
     };
     Tn.isFragment = function(e) {
-        return ba(e) === Z0
+        return ya(e) === Z0
     };
     Tn.isLazy = function(e) {
-        return ba(e) === o_
+        return ya(e) === o_
     };
     Tn.isMemo = function(e) {
-        return ba(e) === a_
+        return ya(e) === a_
     };
     Tn.isPortal = function(e) {
-        return ba(e) === vF
+        return ya(e) === vF
     };
     Tn.isProfiler = function(e) {
-        return ba(e) === J0
+        return ya(e) === J0
     };
     Tn.isStrictMode = function(e) {
-        return ba(e) === Q0
+        return ya(e) === Q0
     };
     Tn.isSuspense = function(e) {
-        return ba(e) === i_
+        return ya(e) === i_
     };
     Tn.isValidElementType = function(e) {
         return typeof e == "string" || typeof e == "function" || e === Z0 || e === n_ || e === J0 || e === Q0 || e === i_ || e === wSe || typeof e == "object" && e !== null && (e.$$typeof === o_ || e.$$typeof === a_ || e.$$typeof === e_ || e.$$typeof === t_ || e.$$typeof === r_ || e.$$typeof === TSe || e.$$typeof === CSe || e.$$typeof === ASe || e.$$typeof === xSe)
     };
-    Tn.typeOf = ba;
+    Tn.typeOf = ya;
     (function(e) {
         e.exports = Tn
     })(_Se);
     var bX = iN,
         RSe = {
             $$typeof: !0,
             render: !0,
@@ -13583,59 +13583,59 @@
         x0e = En({
             prop: "backgroundColor",
             themeKey: "palette",
             transform: Lf
         });
     s_(_0e, w0e, x0e);
 
-    function ca(e) {
+    function ua(e) {
         return e <= 1 && e !== 0 ? `${e*100}%` : e
     }
     const T0e = En({
             prop: "width",
-            transform: ca
+            transform: ua
         }),
         CF = e => {
             if (e.maxWidth !== void 0 && e.maxWidth !== null) {
                 const t = n => {
                     var r, i, a;
                     return {
-                        maxWidth: ((r = e.theme) == null || (i = r.breakpoints) == null || (a = i.values) == null ? void 0 : a[n]) || _F[n] || ca(n)
+                        maxWidth: ((r = e.theme) == null || (i = r.breakpoints) == null || (a = i.values) == null ? void 0 : a[n]) || _F[n] || ua(n)
                     }
                 };
                 return Io(e, e.maxWidth, t)
             }
             return null
         };
     CF.filterProps = ["maxWidth"];
     const C0e = En({
             prop: "minWidth",
-            transform: ca
+            transform: ua
         }),
         A0e = En({
             prop: "height",
-            transform: ca
+            transform: ua
         }),
         R0e = En({
             prop: "maxHeight",
-            transform: ca
+            transform: ua
         }),
         k0e = En({
             prop: "minHeight",
-            transform: ca
+            transform: ua
         });
     En({
         prop: "size",
         cssProperty: "width",
-        transform: ca
+        transform: ua
     });
     En({
         prop: "size",
         cssProperty: "height",
-        transform: ca
+        transform: ua
     });
     const I0e = En({
         prop: "boxSizing"
     });
     s_(T0e, CF, C0e, A0e, R0e, k0e, I0e);
     const O0e = {
             border: {
@@ -13862,30 +13862,30 @@
             right: {},
             bottom: {},
             left: {},
             boxShadow: {
                 themeKey: "shadows"
             },
             width: {
-                transform: ca
+                transform: ua
             },
             maxWidth: {
                 style: CF
             },
             minWidth: {
-                transform: ca
+                transform: ua
             },
             height: {
-                transform: ca
+                transform: ua
             },
             maxHeight: {
-                transform: ca
+                transform: ua
             },
             minHeight: {
-                transform: ca
+                transform: ua
             },
             boxSizing: {},
             fontFamily: {
                 themeKey: "typography"
             },
             fontSize: {
                 themeKey: "typography"
@@ -24925,16 +24925,16 @@
                     elementType: it,
                     getSlotProps: Ae,
                     externalSlotProps: Fr,
                     ownerState: fe
                 });
             return O.jsxs(de, q({}, gr, {
                 children: [O.jsx(we, q({}, Sr)), O.jsx(ze, q({}, Hr)), Le.filter(kn => kn.value >= Oe && kn.value <= Fe).map((kn, In) => {
-                    const ta = c3(kn.value, Oe, Fe),
-                        ar = Ce[K].offset(ta);
+                    const ea = c3(kn.value, Oe, Fe),
+                        ar = Ce[K].offset(ea);
                     let Dt;
                     return ft === !1 ? Dt = De.indexOf(kn.value) !== -1 : Dt = ft === "normal" && (ne ? kn.value >= De[0] && kn.value <= De[De.length - 1] : kn.value <= De[0]) || ft === "inverted" && (ne ? kn.value <= De[0] || kn.value >= De[De.length - 1] : kn.value >= De[0]), O.jsxs(k.Fragment, {
                         children: [O.jsx(pt, q({
                             "data-index": In
                         }, mi, !os(pt) && {
                             markActive: Dt
                         }, {
@@ -24948,16 +24948,16 @@
                         }, {
                             style: q({}, ar, Wr.style),
                             className: ot(le.markLabel, Wr.className, Dt && le.markLabelActive),
                             children: kn.label
                         })) : null]
                     }, In)
                 }), De.map((kn, In) => {
-                    const ta = c3(kn, Oe, Fe),
-                        ar = Ce[K].offset(ta),
+                    const ea = c3(kn, Oe, Fe),
+                        ar = Ce[K].offset(ea),
                         Dt = tt === "off" ? OIe : Xe;
                     return O.jsx(k.Fragment, {
                         children: O.jsx(Dt, q({}, !os(Dt) && {
                             valueLabelFormat: rt,
                             valueLabelDisplay: tt,
                             value: typeof rt == "function" ? rt(He(kn), In) : rt,
                             index: In,
@@ -25341,23 +25341,23 @@
                     PopperComponentProp: Ie,
                     touch: Ce.current
                 }),
                 Wr = $Ie(mi),
                 pl = (r = (i = Ye.popper) != null ? i : M.Popper) != null ? r : BIe,
                 kn = (a = (o = (s = Ye.transition) != null ? s : M.Transition) != null ? o : qe) != null ? a : mN,
                 In = (l = (u = Ye.tooltip) != null ? u : M.Tooltip) != null ? l : UIe,
-                ta = (d = (p = Ye.arrow) != null ? p : M.Arrow) != null ? d : zIe,
+                ea = (d = (p = Ye.arrow) != null ? p : M.Arrow) != null ? d : zIe,
                 ar = wg(pl, q({}, Fe, (f = Oe.popper) != null ? f : U.popper, {
                     className: ot(Wr.popper, Fe == null ? void 0 : Fe.className, (g = (m = Oe.popper) != null ? m : U.popper) == null ? void 0 : g.className)
                 }), mi),
                 Dt = wg(kn, q({}, He, (y = Oe.transition) != null ? y : U.transition), mi),
                 Nu = wg(In, q({}, (_ = Oe.tooltip) != null ? _ : U.tooltip, {
                     className: ot(Wr.tooltip, (E = (b = Oe.tooltip) != null ? b : U.tooltip) == null ? void 0 : E.className)
                 }), mi),
-                cd = wg(ta, q({}, (S = Oe.arrow) != null ? S : U.arrow, {
+                cd = wg(ea, q({}, (S = Oe.arrow) != null ? S : U.arrow, {
                     className: ot(Wr.arrow, (x = (C = Oe.arrow) != null ? C : U.arrow) == null ? void 0 : x.className)
                 }), mi);
             return O.jsxs(k.Fragment, {
                 children: [k.cloneElement(F, Hr), O.jsx(pl, q({
                     as: Ie ?? QX,
                     placement: ve,
                     anchorEl: ie ? {
@@ -25378,15 +25378,15 @@
                     popperOptions: bs,
                     children: ({
                         TransitionProps: st
                     }) => O.jsx(kn, q({
                         timeout: We.transitions.duration.shorter
                     }, st, Dt, {
                         children: O.jsxs(In, q({}, Nu, {
-                            children: [Pe, I ? O.jsx(ta, q({}, cd, {
+                            children: [Pe, I ? O.jsx(ea, q({}, cd, {
                                 ref: fe
                             })) : null]
                         }))
                     }))
                 }))]
             })
         }),
@@ -28289,48 +28289,52 @@
         return O.jsx(PX, {
             theme: n,
             children: O.jsx(Hc, {
                 ...e
             })
         })
     }
-    const Xi = oi({
+    const ba = oi({
         key: "ProjectSettings",
         default: void 0
     });
 
     function ZNe({
         message: e,
         opened: t,
         onClick: n,
         loading: r
     }) {
-        var d;
-        const i = Yt(Xi),
-            a = !!((d = e.subMessages) != null && d.length),
-            o = a ? e.subMessages[0].author : void 0;
-        if (!(a || r && (!e.content || e.authorIsUser)) || i != null && i.hideCot) return null;
-        const l = r ? o ? `Using ${o}` : "Running" : `Used ${o}`;
-        let u = "";
-        return o && (u = o.trim().toLowerCase().replaceAll(" ", "-")), r ? u += "-loading" : u += "-done", O.jsx(GZ, {
-            id: u,
+        var m;
+        const i = Xt(ba),
+            a = (m = e.subMessages) == null ? void 0 : m.length,
+            o = !!a,
+            s = o ? e.subMessages[a - 1].author : void 0,
+            l = r && !e.content,
+            u = r && e.authorIsUser;
+        if (!(o || l || u) || i != null && i.hideCot) return null;
+        const p = a ? e.subMessages.filter(y => !!y.content).length : 0,
+            f = r ? s ? `Using ${s}` : "Running" : `Took ${p} step${p<=1?"":"s"}`;
+        let g = "";
+        return s && (g = s.trim().toLowerCase().replaceAll(" ", "-")), r ? g += "-loading" : g += "-done", O.jsx(GZ, {
+            id: g,
             disableElevation: !0,
             disableRipple: !0,
             sx: {
                 textTransform: "none"
             },
             color: "primary",
             startIcon: r ? O.jsx(rZ, {
                 color: "inherit",
                 size: 16
             }) : void 0,
             variant: "contained",
-            endIcon: a && o ? t ? O.jsx(WZ, {}) : O.jsx(HZ, {}) : void 0,
-            onClick: o ? n : void 0,
-            children: l
+            endIcon: o && s ? t ? O.jsx(WZ, {}) : O.jsx(HZ, {}) : void 0,
+            onClick: s ? n : void 0,
+            children: f
         })
     }
     /*!
      * Determine if an object is a Buffer
      *
      * @author   Feross Aboukhadijeh <https://feross.org>
      * @license  MIT
@@ -28956,25 +28960,25 @@
         return n.join("")
     }
 
     function vDe(e) {
         return Boolean(e && typeof e == "object")
     }
 
-    function ga(e, t, n, r) {
+    function ha(e, t, n, r) {
         const i = e.length;
         let a = 0,
             o;
         if (t < 0 ? t = -t > i ? 0 : i + t : t = t > i ? i : t, n = n > 0 ? n : 0, r.length < 1e4) o = Array.from(r), o.unshift(t, n), [].splice.apply(e, o);
         else
             for (n && [].splice.apply(e, [t, n]); a < r.length;) o = r.slice(a, a + 1e4), o.unshift(t, 0), [].splice.apply(e, o), a += 1e4, t += 1e4
     }
 
     function Pa(e, t) {
-        return e.length > 0 ? (ga(e, e.length, 0, t), e) : t
+        return e.length > 0 ? (ha(e, e.length, 0, t), e) : t
     }
     const Y3 = {}.hasOwnProperty;
 
     function eQ(e) {
         const t = {};
         let n = -1;
         for (; ++n < e.length;) yDe(t, e[n]);
@@ -28995,15 +28999,15 @@
         }
     }
 
     function bDe(e, t) {
         let n = -1;
         const r = [];
         for (; ++n < t.length;)(t[n].add === "after" ? e : r).push(t[n]);
-        ga(e, 0, 0, r)
+        ha(e, 0, 0, r)
     }
     const EDe = /[!-/:-@[-`{-~\u00A1\u00A7\u00AB\u00B6\u00B7\u00BB\u00BF\u037E\u0387\u055A-\u055F\u0589\u058A\u05BE\u05C0\u05C3\u05C6\u05F3\u05F4\u0609\u060A\u060C\u060D\u061B\u061E\u061F\u066A-\u066D\u06D4\u0700-\u070D\u07F7-\u07F9\u0830-\u083E\u085E\u0964\u0965\u0970\u09FD\u0A76\u0AF0\u0C77\u0C84\u0DF4\u0E4F\u0E5A\u0E5B\u0F04-\u0F12\u0F14\u0F3A-\u0F3D\u0F85\u0FD0-\u0FD4\u0FD9\u0FDA\u104A-\u104F\u10FB\u1360-\u1368\u1400\u166E\u169B\u169C\u16EB-\u16ED\u1735\u1736\u17D4-\u17D6\u17D8-\u17DA\u1800-\u180A\u1944\u1945\u1A1E\u1A1F\u1AA0-\u1AA6\u1AA8-\u1AAD\u1B5A-\u1B60\u1BFC-\u1BFF\u1C3B-\u1C3F\u1C7E\u1C7F\u1CC0-\u1CC7\u1CD3\u2010-\u2027\u2030-\u2043\u2045-\u2051\u2053-\u205E\u207D\u207E\u208D\u208E\u2308-\u230B\u2329\u232A\u2768-\u2775\u27C5\u27C6\u27E6-\u27EF\u2983-\u2998\u29D8-\u29DB\u29FC\u29FD\u2CF9-\u2CFC\u2CFE\u2CFF\u2D70\u2E00-\u2E2E\u2E30-\u2E4F\u2E52\u3001-\u3003\u3008-\u3011\u3014-\u301F\u3030\u303D\u30A0\u30FB\uA4FE\uA4FF\uA60D-\uA60F\uA673\uA67E\uA6F2-\uA6F7\uA874-\uA877\uA8CE\uA8CF\uA8F8-\uA8FA\uA8FC\uA92E\uA92F\uA95F\uA9C1-\uA9CD\uA9DE\uA9DF\uAA5C-\uAA5F\uAADE\uAADF\uAAF0\uAAF1\uABEB\uFD3E\uFD3F\uFE10-\uFE19\uFE30-\uFE52\uFE54-\uFE61\uFE63\uFE68\uFE6A\uFE6B\uFF01-\uFF03\uFF05-\uFF0A\uFF0C-\uFF0F\uFF1A\uFF1B\uFF1F\uFF20\uFF3B-\uFF3D\uFF3F\uFF5B\uFF5D\uFF5F-\uFF65]/,
         Ua = Cu(/[A-Za-z]/),
         kS = Cu(/\d/),
         SDe = Cu(/[\dA-Fa-f]/),
         xi = Cu(/[\dA-Za-z]/),
         _De = Cu(/[!-/:-@[-`{-~]/),
@@ -29116,15 +29120,15 @@
                 for (; C--;)
                     if (t.events[C][0] === "exit" && t.events[C][1].type === "chunkFlow") {
                         A = t.events[C][1].end;
                         break
                     } E(r);
                 let I = x;
                 for (; I < t.events.length;) t.events[I][1].end = Object.assign({}, A), I++;
-                return ga(t.events, C + 1, 0, t.events.slice(x)), t.events.length = I, u(S)
+                return ha(t.events, C + 1, 0, t.events.slice(x)), t.events.length = I, u(S)
             }
             return s(S)
         }
 
         function u(S) {
             if (r === n.length) {
                 if (!i) return f(S);
@@ -29183,15 +29187,15 @@
                     if (t.events[F][0] === "exit" && t.events[F][1].type === "chunkFlow") {
                         if (M) {
                             U = t.events[F][1].end;
                             break
                         }
                         M = !0
                     } for (E(r), A = I; A < t.events.length;) t.events[A][1].end = Object.assign({}, U), A++;
-                ga(t.events, F + 1, 0, t.events.slice(I)), t.events.length = A
+                ha(t.events, F + 1, 0, t.events.slice(I)), t.events.length = A
             }
         }
 
         function E(S) {
             let x = n.length;
             for (; x-- > S;) {
                 const C = n[x];
@@ -29268,15 +29272,15 @@
                             ["exit", a, t],
                             ["enter", s, t],
                             ["exit", s, t],
                             ["exit", i, t]
                         ]), e[n][1].end.offset - e[n][1].start.offset ? (d = 2, u = Pa(u, [
                             ["enter", e[n][1], t],
                             ["exit", e[n][1], t]
-                        ])) : d = 0, ga(e, r - 1, n - r + 3, u), n = r + u.length - d - 2;
+                        ])) : d = 0, ha(e, r - 1, n - r + 3, u), n = r + u.length - d - 2;
                         break
                     }
             } for (n = -1; ++n < e.length;) e[n][1].type === "attentionSequence" && (e[n][1].type = "data");
         return e
     }
 
     function kDe(e, t) {
@@ -29654,15 +29658,15 @@
         for (; ++n < e.length;) {
             for (; n in t;) n = t[n];
             if (r = e[n], n && r[1].type === "chunkFlow" && e[n - 1][1].type === "listItemPrefix" && (l = r[1]._tokenizer.events, a = 0, a < l.length && l[a][1].type === "lineEndingBlank" && (a += 2), a < l.length && l[a][1].type === "content"))
                 for (; ++a < l.length && l[a][1].type !== "content";) l[a][1].type === "chunkText" && (l[a][1]._isInFirstContentOfListItem = !0, a++);
             if (r[0] === "enter") r[1].contentType && (Object.assign(t, WDe(e, n)), n = t[n], u = !0);
             else if (r[1]._container) {
                 for (a = n, i = void 0; a-- && (o = e[a], o[1].type === "lineEnding" || o[1].type === "lineEndingBlank");) o[0] === "enter" && (i && (e[i][1].type = "lineEndingBlank"), o[1].type = "lineEnding", i = a);
-                i && (r[1].end = Object.assign({}, e[i][1].start), s = e.slice(i, n), s.unshift(r), ga(e, i, n - i + 1, s))
+                i && (r[1].end = Object.assign({}, e[i][1].start), s = e.slice(i, n), s.unshift(r), ha(e, i, n - i + 1, s))
             }
         }
         return !u
     }
 
     function WDe(e, t) {
         const n = e[t][1],
@@ -29682,15 +29686,15 @@
             for (; e[++i][1] !== g;);
             a.push(i), g._tokenizer || (d = r.sliceStream(g), g.next || d.push(null), p && o.defineSkip(g.start), g._isInFirstContentOfListItem && (o._gfmTasklistFirstContentOfListItem = !0), o.write(d), g._isInFirstContentOfListItem && (o._gfmTasklistFirstContentOfListItem = void 0)), p = g, g = g.next
         }
         for (g = n; ++f < s.length;) s[f][0] === "exit" && s[f - 1][0] === "enter" && s[f][1].type === s[f - 1][1].type && s[f][1].start.line !== s[f][1].end.line && (y = f + 1, _.push(y), g._tokenizer = void 0, g.previous = void 0, g = g.next);
         for (o.events = [], g ? (g._tokenizer = void 0, g.previous = void 0) : _.pop(), f = _.length; f--;) {
             const E = s.slice(_[f], _[f + 1]),
                 b = a.pop();
-            l.unshift([b, b + E.length - 1]), ga(e, b, 2, E)
+            l.unshift([b, b + E.length - 1]), ha(e, b, 2, E)
         }
         for (f = -1; ++f < l.length;) u[m + l[f][0]] = m + l[f][1], m += l[f][1] - l[f][0] - 1;
         return u
     }
     const GDe = {
             tokenize: XDe,
             resolve: YDe
@@ -29916,15 +29920,15 @@
             start: e[r][1].start,
             end: e[n][1].end
         }, a = {
             type: "chunkText",
             start: e[r][1].start,
             end: e[n][1].end,
             contentType: "text"
-        }, ga(e, r, n - r + 1, [
+        }, ha(e, r, n - r + 1, [
             ["enter", i, t],
             ["enter", a, t],
             ["exit", a, t],
             ["exit", i, t]
         ])), e
     }
 
@@ -30296,15 +30300,15 @@
         ], s = Pa(s, e.slice(a + 1, a + r + 3)), s = Pa(s, [
             ["enter", d, t]
         ]), s = Pa(s, B_(t.parser.constructs.insideSpan.null, e.slice(a + r + 4, o - 3), t)), s = Pa(s, [
             ["exit", d, t], e[o - 2], e[o - 1],
             ["exit", u, t]
         ]), s = Pa(s, e.slice(o + 1)), s = Pa(s, [
             ["exit", l, t]
-        ]), ga(e, a, e.length, s), e
+        ]), ha(e, a, e.length, s), e
     }
 
     function ELe(e, t, n) {
         const r = this;
         let i = r.events.length,
             a, o;
         for (; i--;)
@@ -30849,15 +30853,15 @@
                 function Se(ve) {
                     return re.restore(), ++Q < be.length ? ge(be[Q]) : V
                 }
             }
         }
 
         function F(j, te) {
-            j.resolveAll && !a.includes(j) && a.push(j), j.resolve && ga(u.events, te, u.events.length - te, j.resolve(u.events.slice(te), u)), j.resolveTo && (u.events = j.resolveTo(u.events, u))
+            j.resolveAll && !a.includes(j) && a.push(j), j.resolve && ha(u.events, te, u.events.length - te, j.resolve(u.events.slice(te), u)), j.resolveTo && (u.events = j.resolveTo(u.events, u))
         }
 
         function M() {
             const j = m(),
                 te = u.previous,
                 X = u.currentConstruct,
                 J = u.events.length,
@@ -32680,24 +32684,24 @@
     let aMe = 0;
     const jt = Kc(),
         wr = Kc(),
         _Q = Kc(),
         Je = Kc(),
         Un = Kc(),
         Mf = Kc(),
-        sa = Kc();
+        oa = Kc();
 
     function Kc() {
         return 2 ** ++aMe
     }
     const wN = Object.freeze(Object.defineProperty({
             __proto__: null,
             boolean: jt,
             booleanish: wr,
-            commaOrSpaceSeparated: sa,
+            commaOrSpaceSeparated: oa,
             commaSeparated: Mf,
             number: Je,
             overloadedBoolean: _Q,
             spaceSeparated: Un
         }, Symbol.toStringTag, {
             value: "Module"
         })),
@@ -33298,15 +33302,15 @@
                 writingMode: "writing-mode",
                 xHeight: "x-height",
                 playbackOrder: "playbackorder",
                 timelineBegin: "timelinebegin"
             },
             transform: TQ,
             properties: {
-                about: sa,
+                about: oa,
                 accentHeight: Je,
                 accumulate: null,
                 additive: null,
                 alignmentBaseline: null,
                 alphabetic: Je,
                 amplitude: Je,
                 arabicForm: null,
@@ -33410,15 +33414,15 @@
                 in2: null,
                 intercept: Je,
                 k: Je,
                 k1: Je,
                 k2: Je,
                 k3: Je,
                 k4: Je,
-                kernelMatrix: sa,
+                kernelMatrix: oa,
                 kernelUnitLength: null,
                 keyPoints: null,
                 keySplines: null,
                 keyTimes: null,
                 kerning: null,
                 lang: null,
                 lengthAdjust: null,
@@ -33564,29 +33568,29 @@
                 pointsAtX: Je,
                 pointsAtY: Je,
                 pointsAtZ: Je,
                 preserveAlpha: null,
                 preserveAspectRatio: null,
                 primitiveUnits: null,
                 propagate: null,
-                property: sa,
+                property: oa,
                 r: null,
                 radius: null,
                 referrerPolicy: null,
                 refX: null,
                 refY: null,
-                rel: sa,
-                rev: sa,
+                rel: oa,
+                rev: oa,
                 renderingIntent: null,
                 repeatCount: null,
                 repeatDur: null,
-                requiredExtensions: sa,
-                requiredFeatures: sa,
-                requiredFonts: sa,
-                requiredFormats: sa,
+                requiredExtensions: oa,
+                requiredFeatures: oa,
+                requiredFonts: oa,
+                requiredFormats: oa,
                 resource: null,
                 restart: null,
                 result: null,
                 rotate: null,
                 rx: null,
                 ry: null,
                 scale: null,
@@ -33606,43 +33610,43 @@
                 stitchTiles: null,
                 stopColor: null,
                 stopOpacity: null,
                 strikethroughPosition: Je,
                 strikethroughThickness: Je,
                 string: null,
                 stroke: null,
-                strokeDashArray: sa,
+                strokeDashArray: oa,
                 strokeDashOffset: null,
                 strokeLineCap: null,
                 strokeLineJoin: null,
                 strokeMiterLimit: Je,
                 strokeOpacity: Je,
                 strokeWidth: null,
                 style: null,
                 surfaceScale: Je,
                 syncBehavior: null,
                 syncBehaviorDefault: null,
                 syncMaster: null,
                 syncTolerance: null,
                 syncToleranceDefault: null,
-                systemLanguage: sa,
+                systemLanguage: oa,
                 tabIndex: Je,
                 tableValues: null,
                 target: null,
                 targetX: Je,
                 targetY: Je,
                 textAnchor: null,
                 textDecoration: null,
                 textRendering: null,
                 textLength: null,
                 timelineBegin: null,
                 title: null,
                 transformBehavior: null,
                 type: null,
-                typeOf: sa,
+                typeOf: oa,
                 to: null,
                 transform: null,
                 u1: null,
                 u2: null,
                 underlinePosition: Je,
                 underlineThickness: Je,
                 unicode: null,
@@ -34558,20 +34562,20 @@
                                 f = [
                                     ["enter", d, s],
                                     ["enter", o[u][1], s],
                                     ["exit", o[u][1], s],
                                     ["enter", p, s]
                                 ],
                                 g = s.parser.constructs.insideSpan.null;
-                            g && ga(f, f.length, 0, B_(g, o.slice(u + 1, l), s)), ga(f, f.length, 0, [
+                            g && ha(f, f.length, 0, B_(g, o.slice(u + 1, l), s)), ha(f, f.length, 0, [
                                 ["exit", p, s],
                                 ["enter", o[l][1], s],
                                 ["exit", o[l][1], s],
                                 ["exit", d, s]
-                            ]), ga(o, u - 1, l - u + 3, f), l = u + f.length - 2;
+                            ]), ha(o, u - 1, l - u + 3, f), l = u + f.length - 2;
                             break
                         }
                 } for (l = -1; ++l < o.length;) o[l][1].type === "strikethroughSequenceTemporary" && (o[l][1].type = "data");
             return o
         }
 
         function a(o, s, l) {
@@ -36676,16 +36680,16 @@
             }))
         },
         QQ = Lr;
 
     function T2e({
         action: e
     }) {
-        const t = Yt(bv),
-            n = Yt(Ap),
+        const t = Xt(bv),
+            n = Xt(Ap),
             r = k.useCallback(async () => {
                 try {
                     const s = n == null ? void 0 : n.socket.id;
                     if (!s) return;
                     await NNe(s, e)
                 } catch (s) {
                     s instanceof Error && Lr.error(s.message)
@@ -42862,15 +42866,15 @@
                 })
             })(t)
         }
         return WT
     }
     var GT, rq;
 
-    function Zi() {
+    function Xi() {
         if (rq) return GT;
         rq = 1, GT = e, e.displayName = "markupTemplating", e.aliases = [];
 
         function e(t) {
             (function(n) {
                 function r(i, a) {
                     return "___" + i.toUpperCase() + a + "___"
@@ -42925,15 +42929,15 @@
         return GT
     }
     var KT, iq;
 
     function v4e() {
         if (iq) return KT;
         iq = 1;
-        var e = Zi();
+        var e = Xi();
         KT = t, t.displayName = "django", t.aliases = ["jinja2"];
 
         function t(n) {
             n.register(e),
                 function(r) {
                     r.languages.django = {
                         comment: /^\{#[\s\S]*?#\}$/,
@@ -43265,15 +43269,15 @@
         return eC
     }
     var tC, dq;
 
     function x4e() {
         if (dq) return tC;
         dq = 1;
-        var e = Zi();
+        var e = Xi();
         tC = t, t.displayName = "ejs", t.aliases = ["eta"];
 
         function t(n) {
             n.register(e),
                 function(r) {
                     r.languages.ejs = {
                         delimiter: {
@@ -43419,15 +43423,15 @@
     }
     var iC, hq;
 
     function A4e() {
         if (hq) return iC;
         hq = 1;
         var e = G_(),
-            t = Zi();
+            t = Xi();
         iC = n, n.displayName = "erb", n.aliases = [];
 
         function n(r) {
             r.register(e), r.register(t),
                 function(i) {
                     i.languages.erb = {
                         delimiter: {
@@ -43519,15 +43523,15 @@
     }
     var sC, vq;
 
     function k4e() {
         if (vq) return sC;
         vq = 1;
         var e = RJ(),
-            t = Zi();
+            t = Xi();
         sC = n, n.displayName = "etlua", n.aliases = [];
 
         function n(r) {
             r.register(e), r.register(t),
                 function(i) {
                     i.languages.etlua = {
                         delimiter: {
@@ -44055,15 +44059,15 @@
         return hC
     }
     var gC, Tq;
 
     function P4e() {
         if (Tq) return gC;
         Tq = 1;
-        var e = Zi();
+        var e = Xi();
         gC = t, t.displayName = "ftl", t.aliases = [];
 
         function t(n) {
             n.register(e),
                 function(r) {
                     for (var i = /[^<()"']|\((?:<expr>)*\)|<(?!#--)|<#--(?:[^-]|-(?!->))*-->|"(?:[^\\"]|\\.)*"|'(?:[^\\']|\\.)*'/.source, a = 0; a < 2; a++) i = i.replace(/<expr>/g, function() {
                         return i
@@ -44861,15 +44865,15 @@
         return kC
     }
     var IC, Uq;
 
     function Q4e() {
         if (Uq) return IC;
         Uq = 1;
-        var e = Zi();
+        var e = Xi();
         IC = t, t.displayName = "handlebars", t.aliases = ["hbs"];
 
         function t(n) {
             n.register(e),
                 function(r) {
                     r.languages.handlebars = {
                         comment: /\{\{![\s\S]*?\}\}/,
@@ -47171,15 +47175,15 @@
         return vA
     }
     var yA, RV;
 
     function Y_() {
         if (RV) return yA;
         RV = 1;
-        var e = Zi();
+        var e = Xi();
         yA = t, t.displayName = "php", t.aliases = [];
 
         function t(n) {
             n.register(e),
                 function(r) {
                     var i = /\/\*[\s\S]*?\*\/|\/\/.*|#(?!\[).*/,
                         a = [{
@@ -47458,15 +47462,15 @@
         return yA
     }
     var bA, kV;
 
     function Lqe() {
         if (kV) return bA;
         kV = 1;
-        var e = Zi(),
+        var e = Xi(),
             t = Y_();
         bA = n, n.displayName = "latte", n.aliases = [];
 
         function n(r) {
             r.register(e), r.register(t),
                 function(i) {
                     i.languages.latte = {
@@ -47721,15 +47725,15 @@
         return _A
     }
     var wA, DV;
 
     function Pqe() {
         if (DV) return wA;
         DV = 1;
-        var e = Zi();
+        var e = Xi();
         wA = t, t.displayName = "liquid", t.aliases = [];
 
         function t(n) {
             n.register(e), n.languages.liquid = {
                 comment: {
                     pattern: /(^\{%\s*comment\s*%\})[\s\S]+(?=\{%\s*endcomment\s*%\}$)/,
                     lookbehind: !0
@@ -52599,15 +52603,15 @@
         return GR
     }
     var KR, iH;
 
     function l5e() {
         if (iH) return KR;
         iH = 1;
-        var e = Zi();
+        var e = Xi();
         KR = t, t.displayName = "smarty", t.aliases = [];
 
         function t(n) {
             n.register(e),
                 function(r) {
                     r.languages.smarty = {
                         comment: {
@@ -52828,15 +52832,15 @@
         return ZR
     }
     var QR, lH;
 
     function f5e() {
         if (lH) return QR;
         lH = 1;
-        var e = Zi();
+        var e = Xi();
         QR = t, t.displayName = "soy", t.aliases = [];
 
         function t(n) {
             n.register(e),
                 function(r) {
                     var i = /(["'])(?:\\(?:\r\n|[\s\S])|(?!\1)[^\\\r\n])*\1/,
                         a = /\b\d+(?:\.\d+)?(?:[eE][+-]?\d+)?\b|\b0x[\dA-F]+\b/;
@@ -54080,15 +54084,15 @@
         return yk
     }
     var bk, kH;
 
     function k5e() {
         if (kH) return bk;
         kH = 1;
-        var e = Zi();
+        var e = Xi();
         bk = t, t.displayName = "tt2", t.aliases = [];
 
         function t(n) {
             n.register(e),
                 function(r) {
                     r.languages.tt2 = r.languages.extend("clike", {
                         comment: /#.*|\[%#[\s\S]*?%\]/,
@@ -54131,15 +54135,15 @@
         return bk
     }
     var Ek, IH;
 
     function I5e() {
         if (IH) return Ek;
         IH = 1;
-        var e = Zi();
+        var e = Xi();
         Ek = t, t.displayName = "twig", t.aliases = [];
 
         function t(n) {
             n.register(e), n.languages.twig = {
                 comment: /^\{#[\s\S]*?#\}$/,
                 "tag-name": {
                     pattern: /(^\{%-?\s*)\w+/,
@@ -55601,15 +55605,15 @@
     ee.register(Uqe());
     ee.register(zqe());
     ee.register(jqe());
     ee.register(RJ());
     ee.register(qqe());
     ee.register(Vqe());
     ee.register(Hqe());
-    ee.register(Zi());
+    ee.register(Xi());
     ee.register(Wqe());
     ee.register(Gqe());
     ee.register(Kqe());
     ee.register(Yqe());
     ee.register(Xqe());
     ee.register(Zqe());
     ee.register(Qqe());
@@ -57300,15 +57304,15 @@
                 variant: "contained",
                 children: "Browse Files"
             })]
         })
     }
 
     function rWe() {
-        const e = Yt(M_);
+        const e = Xt(M_);
         return (e == null ? void 0 : e.spec.type) !== "file" ? null : O.jsx(nWe, {
             askUser: e
         })
     }
 
     function iWe({
         timestamp: e
@@ -57331,16 +57335,16 @@
         oWe = ["#67A0F8", "#25B1A7", "#FFC266", "#F09691", "#FA7F54", "#59C654", "#9695F8", "#B889F8"];
 
     function sWe(e) {
         return e.split("").reduce((n, r) => n = r.charCodeAt(0) + (n << 6) + (n << 16) - n, 0)
     }
 
     function lWe() {
-        const e = Yt(Xi),
-            n = Yt(F_) === "dark" ? oWe : aWe;
+        const e = Xt(ba),
+            n = Xt(F_) === "dark" ? oWe : aWe;
         return function(r, i, a) {
             if (a) return "error.main";
             if (r === (e == null ? void 0 : e.appTitle)) return "primary.main";
             if (i) return "text.primary";
             const o = Math.abs(sWe(r)) % n.length;
             return n[o]
         }
@@ -67306,27 +67310,27 @@
         Ov = function(e) {
             return e === void 0 && (e = ete), k.useContext(e)
         };
     const Nv = () => {
             const {
                 isAuthenticated: e,
                 ...t
-            } = Ov(), n = Yt(UZ), r = Yt(zZ);
+            } = Ov(), n = Xt(UZ), r = Xt(zZ);
             return {
                 role: r,
                 accessToken: n,
                 isAuthenticated: e,
                 isProjectMember: e && r && r !== "ANONYMOUS",
                 ...t
             }
         },
         aw = k.memo(function({
             children: t
         }) {
-            const n = Yt(Xi),
+            const n = Xt(ba),
                 {
                     isProjectMember: r,
                     accessToken: i
                 } = Nv();
             if ((n == null ? void 0 : n.public) === !0 || r === !1 || !i) return null;
             const a = new wKe({
                 uri: `${n==null?void 0:n.chainlitServer}/api/graphql`,
@@ -67580,15 +67584,15 @@
     function lte({
         messages: e,
         elements: t,
         actions: n,
         indent: r,
         isRunning: i
     }) {
-        const a = Yt(bv);
+        const a = Xt(bv);
         let o = "";
         const s = e.filter((l, u) => {
             var m;
             const d = !!l.content,
                 p = !!((m = l.subMessages) != null && m.length),
                 f = u === e.length - 1;
             return d || p || !d && (i === void 0 ? a && f : i && f)
@@ -68232,16 +68236,16 @@
                 if (typeof v.hashCode == "function") return v.hashCode();
                 if (T === "object") return Fr(v);
                 if (typeof v.toString == "function") return Cn(v.toString());
                 throw new Error("Value type " + T + " cannot be hashed.")
             }
 
             function hr(v) {
-                var T = ta[v];
-                return T === void 0 && (T = Cn(v), In === kn && (In = 0, ta = {}), In++, ta[v] = T), T
+                var T = ea[v];
+                return T === void 0 && (T = Cn(v), In === kn && (In = 0, ea = {}), In++, ea[v] = T), T
             }
 
             function Cn(v) {
                 for (var T = 0, N = 0; N < v.length; N++) T = 31 * T + v.charCodeAt(N) | 0;
                 return tn(T)
             }
 
@@ -68287,15 +68291,15 @@
             gi && (bs = new WeakMap);
             var mi = 0,
                 Wr = "__immutablehash__";
             typeof Symbol == "function" && (Wr = Symbol(Wr));
             var pl = 16,
                 kn = 255,
                 In = 0,
-                ta = {};
+                ea = {};
 
             function ar(v) {
                 je(v !== 1 / 0, "Cannot perform this action with an infinite size.")
             }
             r(Dt, it);
 
             function Dt(v) {
@@ -69117,15 +69121,15 @@
                             return ve(v, Z ? B.get(0) : B[0], Z ? B.get(1) : B[1], L)
                         }
                     }
                 })
             }, vl.prototype.cacheResult = Vt.prototype.cacheResult = yl.prototype.cacheResult = bl.prototype.cacheResult = Sa;
 
             function ey(v) {
-                var T = na(v);
+                var T = ta(v);
                 return T._iter = v, T.size = v.size, T.flip = function() {
                     return v
                 }, T.reverse = function() {
                     var N = v.reverse.apply(this);
                     return N.flip = function() {
                         return v.reverse()
                     }, N
@@ -69151,15 +69155,15 @@
                         })
                     }
                     return v.__iterator(N === re ? ie : re, L)
                 }, T
             }
 
             function ty(v, T, N) {
-                var L = na(v);
+                var L = ta(v);
                 return L.size = v.size, L.has = function(B) {
                     return v.has(B)
                 }, L.get = function(B, Z) {
                     var se = v.get(B, C);
                     return se === C ? Z : T.call(N, se, B, v)
                 }, L.__iterateUncached = function(B, Z) {
                     var se = this;
@@ -69175,15 +69179,15 @@
                             Ne = ke[0];
                         return ve(B, Ne, T.call(N, ke[1], Ne, v), Ee)
                     })
                 }, L
             }
 
             function th(v, T) {
-                var N = na(v);
+                var N = ta(v);
                 return N._iter = v, N.size = v.size, N.reverse = function() {
                     return v
                 }, v.flip && (N.flip = function() {
                     var L = ey(v);
                     return L.reverse = function() {
                         return v.flip()
                     }, L
@@ -69200,15 +69204,15 @@
                     }, !B)
                 }, N.__iterator = function(L, B) {
                     return v.__iterator(L, !B)
                 }, N
             }
 
             function nh(v, T, N, L) {
-                var B = na(v);
+                var B = ta(v);
                 return L && (B.has = function(Z) {
                     var se = v.get(Z, C);
                     return se !== C && !!T.call(N, se, Z, v)
                 }, B.get = function(Z, se) {
                     var Ee = v.get(Z, C);
                     return Ee !== C && T.call(N, Ee, Z, v) ? Ee : se
                 }), B.__iterateUncached = function(Z, se) {
@@ -69261,15 +69265,15 @@
                 if (T !== void 0 && (T = T | 0), N !== void 0 && (N = N | 0), ce(T, N, B)) return v;
                 var Z = V(T, B),
                     se = be(N, B);
                 if (Z !== Z || se !== se) return Fu(v.toSeq().cacheResult(), T, N, L);
                 var Ee = se - Z,
                     ke;
                 Ee === Ee && (ke = Ee < 0 ? 0 : Ee);
-                var Ne = na(v);
+                var Ne = ta(v);
                 return Ne.size = ke === 0 ? ke : v.size && ke || void 0, !L && xe(v) && ke >= 0 && (Ne.get = function(Y, ye) {
                     return Y = X(this, Y), Y >= 0 && Y < ke ? v.get(Y + Z, ye) : ye
                 }), Ne.__iterateUncached = function(Y, ye) {
                     var me = this;
                     if (ke === 0) return 0;
                     if (ye) return this.cacheResult().__iterate(Y, ye);
                     var Be = 0,
@@ -69289,15 +69293,15 @@
                         var _t = me.next();
                         return L || Y === re ? _t : Y === ie ? ve(Y, nt - 1, void 0, _t) : ve(Y, nt - 1, _t.value[1], _t)
                     })
                 }, Ne
             }
 
             function Ss(v, T, N) {
-                var L = na(v);
+                var L = ta(v);
                 return L.__iterateUncached = function(B, Z) {
                     var se = this;
                     if (Z) return this.cacheResult().__iterate(B, Z);
                     var Ee = 0;
                     return v.__iterate(function(ke, Ne, Y) {
                         return T.call(N, ke, Ne, Y) && ++Ee && B(ke, Ne, se)
                     }), Ee
@@ -69315,15 +69319,15 @@
                             me = Y[1];
                         return T.call(N, me, ye, se) ? B === $ ? Ne : ve(B, ye, me, Ne) : (ke = !1, Ie())
                     })
                 }, L
             }
 
             function rh(v, T, N, L) {
-                var B = na(v);
+                var B = ta(v);
                 return B.__iterateUncached = function(Z, se) {
                     var Ee = this;
                     if (se) return this.cacheResult().__iterate(Z, se);
                     var ke = !0,
                         Ne = 0;
                     return v.__iterate(function(Y, ye, me) {
                         if (!(ke && (ke = T.call(N, Y, ye, me)))) return Ne++, Z(Y, L ? ye : Ne - 1, Ee)
@@ -69364,15 +69368,15 @@
                         var ke = Ee.size;
                         if (ke !== void 0) return se + ke
                     }
                 }, 0), Z
             }
 
             function vi(v, T, N) {
-                var L = na(v);
+                var L = ta(v);
                 return L.__iterateUncached = function(B, Z) {
                     var se = 0,
                         Ee = !1;
 
                     function ke(Ne, Y) {
                         var ye = this;
                         Ne.__iterate(function(me, Be) {
@@ -69404,15 +69408,15 @@
                 var L = ay(v);
                 return v.toSeq().map(function(B, Z) {
                     return L(T.call(N, B, Z, v))
                 }).flatten(!0)
             }
 
             function ry(v, T) {
-                var N = na(v);
+                var N = ta(v);
                 return N.size = v.size && v.size * 2 - 1, N.__iterateUncached = function(L, B) {
                     var Z = this,
                         se = 0;
                     return v.__iterate(function(Ee, ke) {
                         return (!se || L(T, se++, Z) !== !1) && L(Ee, se++, Z) !== !1
                     }, B), se
                 }, N.__iteratorUncached = function(L, B) {
@@ -69456,15 +69460,15 @@
 
             function ah(v, T, N) {
                 var L = v(N, T);
                 return L === 0 && N !== T && (N == null || N !== N) || L > 0
             }
 
             function vd(v, T, N) {
-                var L = na(v);
+                var L = ta(v);
                 return L.size = new rt(N).map(function(B) {
                     return B.size
                 }).min(), L.__iterate = function(B, Z) {
                     for (var se = this.__iterator(re, Z), Ee, ke = 0; !(Ee = se.next()).done && B(Ee.value, ke++, this) !== !1;);
                     return ke
                 }, L.__iteratorUncached = function(B, Z) {
                     var se = N.map(function(Ne) {
@@ -69497,15 +69501,15 @@
                 return ar(v.size), te(v)
             }
 
             function ay(v) {
                 return u(v) ? a : d(v) ? o : s
             }
 
-            function na(v) {
+            function ta(v) {
                 return Object.create((u(v) ? Ze : d(v) ? We : ft).prototype)
             }
 
             function Sa() {
                 return this._iter.cacheResult ? (this._iter.cacheResult(), this.size = this._iter.size, this) : He.prototype.cacheResult.call(this)
             }
 
@@ -71483,15 +71487,15 @@
                 })
             },
             applyEntity: function(t, n, r) {
                 var i = sg(t, n);
                 return j7e(i, n, r)
             }
         },
-        Qi = FE;
+        Zi = FE;
 
     function Z7e(e) {
         return Object.keys(e).map(function(t) {
             return e[t]
         })
     }
     var wte = Z7e;
@@ -72066,18 +72070,18 @@
             }, e
         }(),
         aXe = iXe,
         oXe = function(t) {
             if (t != null) return t;
             throw new Error("Got unexpected null or undefined")
         },
-        Ji = oXe,
+        Qi = oXe,
         sXe = aXe,
         Mte = an,
-        lXe = Ji,
+        lXe = Qi,
         uXe = Mte.OrderedMap,
         Ub, cXe = {
             getDirectionMap: function(t, n) {
                 Ub ? Ub.reset() : Ub = new sXe;
                 var r = t.getBlockMap(),
                     i = r.valueSeq().map(function(o) {
                         return lXe(Ub).getDirection(o.getText())
@@ -72543,15 +72547,15 @@
             writable: !0
         }) : e[t] = n, e
     }
     var RXe = Dv,
         kXe = io,
         IXe = Qc,
         OXe = ao,
-        Kd = Qi,
+        Kd = Zi,
         HG = Pn,
         WG = vs,
         NXe = Iu,
         jte = an,
         qb = CXe,
         qte = NXe("draft_tree_data_support"),
         GG = qte ? OXe : IXe,
@@ -73728,15 +73732,15 @@
             isPlatform: function(t) {
                 return Yd(Ho.platformName, Ho.platformFullVersion, t, IZe)
             },
             isPlatformArchitecture: function(t) {
                 return Yd(Ho.platformArchitecture, null, t)
             }
         },
-        ea = RZe(OZe, kZe);
+        Ji = RZe(OZe, kZe);
 
     function NZe(e) {
         return !e || !e.ownerDocument ? document : e.ownerDocument
     }
     var fw = NZe;
 
     function DZe(e) {
@@ -73780,20 +73784,20 @@
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    var BZe = ea,
+    var BZe = Ji,
         UZe = pw,
         zZe = Qte,
         jZe = an,
         qZe = vn,
-        VZe = Ji,
+        VZe = Qi,
         e6 = jZe.Map,
         HZe = {
             subtree: !0,
             characterData: !0,
             childList: !0,
             characterDataOldValue: !1,
             attributes: !1
@@ -73906,15 +73910,15 @@
         var t = e.editorContainer;
         t || n6(!1), XZe(t.firstChild) || n6(!1);
         var n = t.firstChild;
         return n
     }
     var ene = ZZe,
         r6 = dl,
-        QZe = Ji;
+        QZe = Qi;
 
     function JZe(e, t, n, r, i) {
         var a = QZe(e.getSelection());
         if (!t || !r) return a;
         var o = r6.decode(t),
             s = o.blockKey,
             l = e.getBlockTree(s),
@@ -73951,15 +73955,15 @@
     }
     var tne = JZe,
         Ig = pw,
         am = Zte,
         i6 = tne,
         mI = vn,
         MP = td,
-        yc = Ji;
+        yc = Qi;
 
     function eQe(e, t, n, r, i, a) {
         var o = n.nodeType === Node.TEXT_NODE,
             s = i.nodeType === Node.TEXT_NODE;
         if (o && s) return {
             selectionState: i6(e, yc(Ig(n)), r, yc(Ig(i)), a),
             needsRecovery: !1
@@ -74098,24 +74102,24 @@
             var n = e.__get(t);
             return n.getMutability() === "MUTABLE" ? t : null
         }
         return null
     }
     var PP = fQe,
         pQe = GZe,
-        hQe = Qi,
+        hQe = Zi,
         gQe = dl,
         dg = Pn,
         vI = hw,
-        mQe = ea,
+        mQe = Ji,
         vQe = ine,
         one = ene,
         yQe = rne,
         bQe = PP,
-        EQe = Ji,
+        EQe = Qi,
         SQe = mQe.isBrowser("IE"),
         _Qe = 20,
         yI = !1,
         Gb = !1,
         om = null;
 
     function wQe(e) {
@@ -74257,15 +74261,15 @@
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
     var hp = k,
-        AQe = ea,
+        AQe = Ji,
         RQe = vn,
         kQe = td,
         $P = AQe.isBrowser("IE <= 11");
 
     function IQe(e) {
         return $P ? e.textContent === `
 ` : e.tagName === "BR"
@@ -74360,15 +74364,15 @@
             return e.activeElement || e.body
         } catch {
             return e.body
         }
     }
     var une = jQe,
         TD = Jte,
-        qQe = ea,
+        qQe = Ji,
         cne = BP,
         VQe = une,
         UP = fw,
         HQe = vn,
         dne = td,
         WQe = qQe.isBrowser("IE");
 
@@ -75076,15 +75080,15 @@
 
         function n(l, u) {
             l.prototype = Object.create(u.prototype), l.prototype.constructor = l, l.__proto__ = u
         }
         var r = AJe(),
             i = dl,
             a = k,
-            o = Ji,
+            o = Qi,
             s = function(l) {
                 n(u, l);
 
                 function u() {
                     return l.apply(this, arguments) || this
                 }
                 var d = u.prototype;
@@ -75195,15 +75199,15 @@
         MJe = cw,
         PJe = Jc,
         $Je = mne,
         BJe = mw,
         UJe = Ene,
         zJe = vn,
         jJe = Uv,
-        qJe = Ji,
+        qJe = Qi,
         E6 = 10,
         S6 = function(t, n) {
             return t.getAnchorKey() === n || t.getFocusKey() === n
         },
         VJe = function(e) {
             OJe(t, e);
 
@@ -75375,15 +75379,15 @@
             g.prototype = Object.create(m.prototype), g.prototype.constructor = g, g.__proto__ = m
         }
         var a = Sne,
             o = dl,
             s = k,
             l = Jc,
             u = HJe(),
-            d = Ji,
+            d = Qi,
             p = function(m, y, _, E) {
                 return l({
                     "public/DraftStyleDefault/unorderedListItem": m === "unordered-list-item",
                     "public/DraftStyleDefault/orderedListItem": m === "ordered-list-item",
                     "public/DraftStyleDefault/reset": _,
                     "public/DraftStyleDefault/depth0": y === 0,
                     "public/DraftStyleDefault/depth1": y === 1,
@@ -75655,23 +75659,23 @@
     var xne = het;
 
     function met(e) {
         return e === "handled" || e === !0
     }
     var yw = met,
         vet = wne,
-        Tne = Qi,
+        Tne = Zi,
         Cne = Pn,
         yet = pw,
         bet = fw,
         Eet = xne,
         _et = tne,
         wet = Qte,
         C6 = yw,
-        AI = Ji;
+        AI = Qi;
 
     function xet(e, t) {
         var n = null,
             r = null,
             i = bet(e.currentTarget);
         if (typeof i.caretRangeFromPoint == "function") {
             var a = i.caretRangeFromPoint(e.x, e.y);
@@ -75855,21 +75859,21 @@
                 setTimeout(d, 0, b)
             }
         }
         var E = Object.getPrototypeOf && Object.getPrototypeOf(e);
         E = E && E.setTimeout ? E : e, {}.toString.call(e.process) === "[object process]" ? p() : f() ? g() : e.MessageChannel ? m() : a && "onreadystatechange" in a.createElement("script") ? y() : _(), E.setImmediate = s, E.clearImmediate = l
     })(typeof self > "u" ? ni : self);
     var Iet = ni.setImmediate,
-        Oet = Qi,
+        Oet = Zi,
         RD = Pn,
-        Net = ea,
+        Net = Ji,
         k6 = PP,
         Det = yw,
         Let = ket,
-        I6 = Ji,
+        I6 = Qi,
         Fet = Iet,
         Met = "'",
         Pet = "/",
         $et = Net.isBrowser("Firefox");
 
     function Bet(e) {
         return $et && (e == Met || e == Pet)
@@ -75981,15 +75985,15 @@
             var t = e;
             if (!t.ownerDocument.defaultView) return t instanceof Node;
             if (t instanceof t.ownerDocument.defaultView.Node) return !0
         }
         return !1
     }
     var ttt = ett,
-        ntt = Qi,
+        ntt = Zi,
         rtt = Pn,
         itt = gw,
         att = Ane,
         ott = mw,
         stt = ttt;
 
     function ltt(e, t) {
@@ -76023,15 +76027,15 @@
     var ftt = dtt;
 
     function ptt(e) {
         e._internalDrag = !0, e.setMode("drag")
     }
     var htt = ptt,
         D6 = Pn,
-        gtt = ea;
+        gtt = Ji;
 
     function mtt(e, t) {
         var n = e._latestEditorState,
             r = n.getSelection();
         if (!r.getHasFocus()) {
             var i = r.set("hasFocus", !0);
             e.props.onFocus && e.props.onFocus(t), gtt.isBrowser("Chrome < 60.0.3081.0") ? e.update(D6.forceSelection(n, i)) : e.update(D6.acceptSelection(n, i))
@@ -76129,15 +76133,15 @@
         return n.merge({
             focusKey: o,
             focusOffset: s,
             isBackward: !0
         })
     }
     var qP = Att,
-        Rtt = Qi,
+        Rtt = Zi,
         ktt = Iu,
         L6 = ktt("draft_tree_data_support");
 
     function Itt(e, t, n) {
         var r = e.getSelection(),
             i = e.getCurrentContent(),
             a = r,
@@ -76176,23 +76180,23 @@
             return Dtt(r, l ? Ntt.getUTF16Length(l, 0) : 1)
         }, "backward");
         if (t === e.getCurrentContent()) return e;
         var n = e.getSelection();
         return Ott.push(e, t.set("selectionBefore", n), n.isCollapsed() ? "backspace-character" : "remove-range")
     }
     var Nne = Ftt,
-        Mtt = Qi,
+        Mtt = Zi,
         Ptt = dl,
         $tt = Pn,
-        Btt = ea,
+        Btt = Ji,
         Utt = ane,
         ztt = Utt.notEmptyKey,
         jtt = pw,
         qtt = Nne,
-        Vtt = Ji,
+        Vtt = Qi,
         Htt = Btt.isEngine("Gecko"),
         Wtt = `
 
 `;
 
     function Gtt(e, t) {
         switch (e) {
@@ -76271,15 +76275,15 @@
     var Ytt = Ktt,
         Xtt = hw;
 
     function Ztt(e) {
         return e.which === Xtt.RETURN && (e.getModifierState("Shift") || e.getModifierState("Alt") || e.getModifierState("Control"))
     }
     var Qtt = Ztt,
-        Jtt = ea,
+        Jtt = Ji,
         ent = Qtt,
         RI = Jtt.isPlatform("Mac OS X"),
         Dne = {
             isCtrlKeyCommand: function(t) {
                 return !!t.ctrlKey && !t.altKey
             },
             isOptionKeyCommand: function(t) {
@@ -76290,18 +76294,18 @@
             },
             hasCommandModifier: function(t) {
                 return RI ? !!t.metaKey && !t.altKey : Dne.isCtrlKeyCommand(t)
             },
             isSoftNewlineEvent: ent
         },
         VP = Dne,
-        F6 = Qi,
+        F6 = Zi,
         M6 = Pn,
         tnt = ow,
-        nnt = Ji,
+        nnt = Qi,
         kI = null,
         rnt = {
             cut: function(t) {
                 var n = t.getCurrentContent(),
                     r = t.getSelection(),
                     i = null;
                 if (r.isCollapsed()) {
@@ -76320,15 +76324,15 @@
             paste: function(t) {
                 if (!kI) return t;
                 var n = F6.replaceWithFragment(t.getCurrentContent(), t.getSelection(), kI);
                 return M6.push(t, n, "insert-fragment")
             }
         },
         int = rnt,
-        ant = ea,
+        ant = Ji,
         ont = vn,
         snt = ant.isBrowser("Chrome");
 
     function lnt(e) {
         for (var t = e.cloneRange(), n = [], r = e.endContainer; r != null; r = r.parentNode) {
             var i = r === e.commonAncestorContainer;
             i ? t.setStart(e.startContainer, e.startOffset) : t.setStart(t.endContainer, 0);
@@ -76496,15 +76500,15 @@
                 s = o.getBlockForKey(a).getText().slice(i),
                 l = $nt.getForward(s);
             return Unt(n, l.length || 1)
         }, "forward");
         return t === e.getCurrentContent() ? e : Bnt.push(e, t, "remove-range")
     }
     var qnt = jnt,
-        Vnt = Qi,
+        Vnt = Zi,
         Hnt = Pn;
 
     function Wnt(e) {
         var t = Vnt.splitBlock(e.getCurrentContent(), e.getSelection());
         return Hnt.push(e, t, "split-block")
     }
     var Gnt = Wnt,
@@ -76559,15 +76563,15 @@
             return nrt(r, l ? trt.getUTF16Length(l, 0) : 1)
         }, "forward");
         if (t === e.getCurrentContent()) return e;
         var n = e.getSelection();
         return ert.push(e, t.set("selectionBefore", n), n.isCollapsed() ? "delete-character" : "remove-range")
     }
     var art = irt,
-        z6 = Qi,
+        z6 = Zi,
         j6 = Pn,
         ort = ow;
 
     function srt(e) {
         var t = e.getSelection();
         if (!t.isCollapsed()) return e;
         var n = t.getAnchorOffset();
@@ -76610,20 +76614,20 @@
         n(II.set(t, {
             nativelyRenderedContent: null
         })), setTimeout(function() {
             n(r)
         }, 0)
     }
     var crt = urt,
-        drt = Qi,
+        drt = Zi,
         $ne = Pn,
         frt = VP,
         Ps = hw,
         q6 = int,
-        prt = ea,
+        prt = Ji,
         V6 = yw,
         hrt = _nt,
         grt = Mnt,
         mrt = qnt,
         vrt = Gnt,
         yrt = Xnt,
         brt = Jnt,
@@ -76731,15 +76735,15 @@
             }
             var t = e.prototype;
             return t.toString = function() {
                 return this._uri
             }, e
         }(),
         krt = Rrt,
-        Irt = ea,
+        Irt = Ji,
         Ort = vn,
         Nrt = Irt.isBrowser("IE <= 9");
 
     function Drt(e) {
         var t, n = null;
         return !Nrt && document.implementation && document.implementation.createHTMLDocument && (t = document.implementation.createHTMLDocument("foo"), t.documentElement || Ort(!1), t.documentElement.innerHTML = e, n = t.getElementsByTagName("body")[0]), n
     }
@@ -77133,18 +77137,18 @@
         return o = o.merge(s), e.merge({
             blockMap: o,
             selectionBefore: t,
             selectionAfter: t
         })
     }
     var Ait = Cit,
-        Ju = Qi,
+        Ju = Zi,
         qo = Pn,
         Rit = Ait,
-        kit = Ji,
+        kit = Qi,
         Wo = {
             currentBlockContainsLink: function(t) {
                 var n = t.getSelection(),
                     r = t.getCurrentContent(),
                     i = r.getEntityMap();
                 return r.getBlockForKey(n.getAnchorKey()).getCharacterList().slice(n.getStartOffset(), n.getEndOffset()).some(function(a) {
                     var o = a.getEntity();
@@ -77302,15 +77306,15 @@
     function Oit(e) {
         return e.split(Iit)
     }
     var Nit = Oit,
         DI = Dv,
         Q6 = io,
         Dit = wne,
-        Xne = Qi,
+        Xne = Zi,
         LI = Tit,
         Zne = Pn,
         J6 = Yne,
         eK = PP,
         Lit = xne,
         tK = yw,
         nK = Nit;
@@ -77398,15 +77402,15 @@
 
     function Mit(e, t) {
         return e.length === t.size && t.valueSeq().every(function(n, r) {
             return n.getText() === e[r]
         })
     }
     var Pit = Fit,
-        Qne = ea,
+        Qne = Ji,
         $it = zet,
         Bit = Het,
         Uit = Ket,
         zit = Jet,
         jit = ctt,
         qit = ftt,
         Vit = htt,
@@ -77470,15 +77474,15 @@
                     style: o
                 }, this.props.text))
             }, t
         }(FI.Component),
         iat = rat,
         ere = VP,
         hg = hw,
-        tre = ea,
+        tre = Ji,
         Ql = tre.isPlatform("Mac OS X"),
         aK = Ql && tre.isBrowser("Firefox < 29"),
         Vl = ere.hasCommandModifier,
         $s = ere.isCtrlKeyCommand;
 
     function nre(e) {
         return Ql && e.altKey || $s(e)
@@ -77589,23 +77593,23 @@
         gat = Qit,
         oK = tat,
         mat = iat,
         vat = Pn,
         Ml = k,
         yat = zP,
         bat = gw,
-        Eat = ea,
+        Eat = Ji,
         PI = Jc,
         Sat = vs,
         _at = rre,
         wat = mw,
         xat = Iu,
         sK = vn,
         lK = Uv,
-        Tat = Ji,
+        Tat = Qi,
         are = Eat.isBrowser("IE"),
         Cat = !are,
         uK = {
             edit: gat,
             composite: fat,
             drag: hat,
             cut: null,
@@ -78330,15 +78334,15 @@
         Wot = Qc,
         Got = IP,
         Kot = FP,
         Yot = Vte,
         Xot = Rat,
         Zot = Sne,
         Qot = sw,
-        Jot = Qi,
+        Jot = Zi,
         est = Rte,
         tst = Pn,
         nst = VP,
         rst = kat,
         ist = Yne,
         ast = lw,
         ost = Jat,
@@ -78607,28 +78611,28 @@
         }, 2)
     }
 
     function mre(e) {
         return e == null ? [] : [].concat(e)
     }
     let Hst = /\$\{\s*(\w+)\s*\}/g;
-    class ua extends Error {
+    class la extends Error {
         static formatError(t, n) {
             const r = n.label || n.path || "this";
             return r !== n.path && (n = Object.assign({}, n, {
                 path: r
             })), typeof t == "string" ? t.replace(Hst, (i, a) => xc(n[a])) : typeof t == "function" ? t(n) : t
         }
         static isError(t) {
             return t && t.name === "ValidationError"
         }
         constructor(t, n, r, i) {
             super(), this.value = void 0, this.path = void 0, this.type = void 0, this.errors = void 0, this.params = void 0, this.inner = void 0, this.name = "ValidationError", this.value = n, this.path = r, this.type = i, this.errors = [], this.inner = [], mre(t).forEach(a => {
-                ua.isError(a) ? (this.errors.push(...a.errors), this.inner = this.inner.concat(a.inner.length ? a.inner : a)) : this.errors.push(a)
-            }), this.message = this.errors.length > 1 ? `${this.errors.length} errors occurred` : this.errors[0], Error.captureStackTrace && Error.captureStackTrace(this, ua)
+                la.isError(a) ? (this.errors.push(...a.errors), this.inner = this.inner.concat(a.inner.length ? a.inner : a)) : this.errors.push(a)
+            }), this.message = this.errors.length > 1 ? `${this.errors.length} errors occurred` : this.errors[0], Error.captureStackTrace && Error.captureStackTrace(this, la)
         }
     }
     let zs = {
             default: "${path} is invalid",
             required: "${path} is a required field",
             defined: "${path} must be defined",
             notNull: "${path} cannot be null",
@@ -78783,15 +78787,15 @@
                     value: n,
                     originalValue: a,
                     label: o.spec.label,
                     path: U.path || r,
                     spec: o.spec
                 }, p, U.params);
                 for (const X of Object.keys(j)) j[X] = E(j[X]);
-                const te = new ua(ua.formatError(U.message || f, j), n, j.path, U.type || u);
+                const te = new la(la.formatError(U.message || f, j), n, j.path, U.type || u);
                 return te.params = j, te
             }
             const S = _ ? s : l;
             let x = {
                 path: r,
                 parent: m,
                 type: u,
@@ -78799,18 +78803,18 @@
                 createError: b,
                 resolve: E,
                 options: i,
                 originalValue: a,
                 schema: o
             };
             const C = U => {
-                    ua.isError(U) ? S(U) : U ? l(null) : S(b())
+                    la.isError(U) ? S(U) : U ? l(null) : S(b())
                 },
                 A = U => {
-                    ua.isError(U) ? S(U) : s(U)
+                    la.isError(U) ? S(U) : s(U)
                 },
                 I = g && ns(n);
             if (!i.sync) {
                 try {
                     Promise.resolve(I ? !0 : d.call(x, n, x)).then(C, A)
                 } catch (U) {
                     A(U)
@@ -79078,44 +79082,44 @@
             return (p, f, g) => this.resolve(d)._validate(u, d, f, g)
         }
         validate(t, n) {
             let r = this.resolve(Object.assign({}, n, {
                 value: t
             }));
             return new Promise((i, a) => r._validate(t, n, (o, s) => {
-                ua.isError(o) && (o.value = s), a(o)
+                la.isError(o) && (o.value = s), a(o)
             }, (o, s) => {
-                o.length ? a(new ua(o, s)) : i(s)
+                o.length ? a(new la(o, s)) : i(s)
             }))
         }
         validateSync(t, n) {
             let r = this.resolve(Object.assign({}, n, {
                     value: t
                 })),
                 i;
             return r._validate(t, Object.assign({}, n, {
                 sync: !0
             }), (a, o) => {
-                throw ua.isError(a) && (a.value = o), a
+                throw la.isError(a) && (a.value = o), a
             }, (a, o) => {
-                if (a.length) throw new ua(a, t);
+                if (a.length) throw new la(a, t);
                 i = o
             }), i
         }
         isValid(t, n) {
             return this.validate(t, n).then(() => !0, r => {
-                if (ua.isError(r)) return !1;
+                if (la.isError(r)) return !1;
                 throw r
             })
         }
         isValidSync(t, n) {
             try {
                 return this.validateSync(t, n), !0
             } catch (r) {
-                if (ua.isError(r)) return !1;
+                if (la.isError(r)) return !1;
                 throw r
             }
         }
         _getDefault() {
             let t = this.spec.default;
             return t == null ? t : typeof t == "function" ? t.call(this) : xf(t)
         }
@@ -80496,15 +80500,15 @@
     const zut = Uut;
     var jut = Array.isArray;
     const qv = jut;
 
     function qut() {
         return !1
     }
-    var Dre = typeof fa == "object" && fa && !fa.nodeType && fa,
+    var Dre = typeof da == "object" && da && !da.nodeType && da,
         MK = Dre && typeof Ti == "object" && Ti && !Ti.nodeType && Ti,
         Vut = MK && MK.exports === Dre,
         PK = Vut ? ys.Buffer : void 0,
         Hut = PK ? PK.isBuffer : void 0,
         Wut = Hut || qut;
     const Lre = Wut;
     var Gut = 9007199254740991,
@@ -80552,15 +80556,15 @@
     }
 
     function t$(e) {
         return function(t) {
             return e(t)
         }
     }
-    var Mre = typeof fa == "object" && fa && !fa.nodeType && fa,
+    var Mre = typeof da == "object" && da && !da.nodeType && da,
         sm = Mre && typeof Ti == "object" && Ti && !Ti.nodeType && Ti,
         _ct = sm && sm.exports === Mre,
         jI = _ct && xre.process,
         wct = function() {
             try {
                 var e = sm && sm.require && sm.require("util").types;
                 return e || jI && jI.binding && jI.binding("util")
@@ -80635,15 +80639,15 @@
     function i$(e) {
         return $re(e) ? Pre(e, !0) : $ct(e)
     }
 
     function Bct(e, t) {
         return e && Tw(t, i$(t), e)
     }
-    var Bre = typeof fa == "object" && fa && !fa.nodeType && fa,
+    var Bre = typeof da == "object" && da && !da.nodeType && da,
         BK = Bre && typeof Ti == "object" && Ti && !Ti.nodeType && Ti,
         Uct = BK && BK.exports === Bre,
         UK = Uct ? ys.Buffer : void 0,
         zK = UK ? UK.allocUnsafe : void 0;
 
     function zct(e, t) {
         if (t) return e.slice();
@@ -82433,18 +82437,18 @@
             COMPLETION: {
                 backgroundColor: "#d2f4d3",
                 color: "black"
             }
         };
 
     function tie() {
-        const e = Yt(gD),
+        const e = Xt(gD),
             t = ti(gD),
-            n = Yt(mD),
-            r = Yt(O_),
+            n = Xt(mD),
+            r = Xt(O_),
             i = ti(mD),
             [a, o] = k.useState(Dl.EditorState.createEmpty()),
             [s, l] = k.useState(!1);
         k.useEffect(() => {
             if (e != null && e.prompt) {
                 const g = Dl.EditorState.createWithContent(Dl.ContentState.createFromText(e.prompt));
                 o(d(g, e.completion))
@@ -82612,15 +82616,15 @@
                 default:
                     return null
             }
         },
         vpt = () => {
             const {
                 name: e
-            } = MZ(), n = Yt(j_).find(r => r.name === e);
+            } = MZ(), n = Xt(j_).find(r => r.name === e);
             return n ? O.jsxs(Pt, {
                 display: "flex",
                 flexDirection: "column",
                 flexGrow: 1,
                 p: 3,
                 gap: 2,
                 boxSizing: "border-box",
@@ -82707,25 +82711,25 @@
                     id: "side-view-content",
                     children: e && nie(e)
                 })]
             })
         };
 
     function _pt() {
-        const [e, t] = Wi(bv), n = Yt(Xi), r = Yt(Ap);
-        if (!e || n != null && n.hideCot) return null;
-        const i = () => {
-            t(!1), r == null || r.socket.emit("stop")
+        const [e, t] = Wi(bv), n = Xt(Ap);
+        if (!e) return null;
+        const r = () => {
+            t(!1), n == null || n.socket.emit("stop")
         };
         return O.jsx(Pt, {
             margin: "auto",
             children: O.jsx(GZ, {
                 startIcon: O.jsx(Lp, {}),
                 variant: "contained",
-                onClick: i,
+                onClick: r,
                 children: "Stop task"
             })
         })
     }
     var d$ = {},
         wpt = ir;
     Object.defineProperty(d$, "__esModule", {
@@ -83017,15 +83021,15 @@
 `;
 
     function $pt({
         onClick: e
     }) {
         const {
             user: t
-        } = Ov(), n = Yt(Xi), [r, {
+        } = Ov(), n = Xt(ba), [r, {
             data: i,
             refetch: a
         }] = UKe(Ppt, {
             variables: {
                 first: 30,
                 projectId: n == null ? void 0 : n.projectId,
                 authorEmail: t == null ? void 0 : t.email
@@ -83046,15 +83050,15 @@
                 onClick: e
             })
         })
     }
     const Upt = k.memo(function({
         onClick: t
     }) {
-        const n = Yt(Xi);
+        const n = Xt(ba);
         return (n == null ? void 0 : n.public) === !1 ? O.jsx(Bpt, {
             onClick: t
         }) : O.jsx(Mpt, {
             onClick: t
         })
     });
 
@@ -83065,17 +83069,17 @@
     }
     const jpt = ({
             onSubmit: e,
             onReply: t
         }) => {
             const n = k.useRef(null),
                 r = ti(VZ),
-                i = Yt(bv),
-                a = Yt(M_),
-                o = Yt(Ap),
+                i = Xt(bv),
+                a = Xt(M_),
+                o = Xt(Ap),
                 [s, l] = k.useState(""),
                 d = !((o == null ? void 0 : o.socket) && !(o != null && o.error)) || i || (a == null ? void 0 : a.spec.type) === "file";
             k.useEffect(() => {
                 var y;
                 n.current && !i && !d && ((y = n.current.querySelector("textarea")) == null || y.focus())
             }, [i, d]);
             const p = k.useCallback(() => {
@@ -83147,15 +83151,15 @@
         },
         qpt = "/assets/logo_dark-bc7401f6.svg",
         Vpt = "/assets/logo_light-f19fc2ea.svg",
         Hpt = ({
             width: e,
             style: t
         }) => {
-            const r = Yt(F_) === "light" ? Vpt : qpt;
+            const r = Xt(F_) === "light" ? Vpt : qpt;
             return O.jsx("img", {
                 src: r,
                 style: t,
                 width: e || 40
             })
         };
 
@@ -83185,15 +83189,15 @@
         })
     }
 
     function Gpt({
         onSubmit: e,
         onReply: t
     }) {
-        return Yt(tM), O.jsxs(Pt, {
+        return Xt(tM), O.jsxs(Pt, {
             display: "flex",
             flexDirection: "column",
             gap: 1,
             py: 2,
             sx: {
                 boxSizing: "border-box",
                 width: "100%",
@@ -83210,15 +83214,15 @@
         })
     }
     const h$ = oi({
             key: "Actions",
             default: []
         }),
         Kpt = () => {
-            const e = Yt(Xi);
+            const e = Xt(ba);
             return e != null && e.chainlitMd ? O.jsx(Pt, {
                 overflow: "auto",
                 flexGrow: 1,
                 children: O.jsx(Pt, {
                     id: "welcome-screen",
                     sx: {
                         maxWidth: "60rem",
@@ -83284,15 +83288,15 @@
             }) : this.props.children
         }
     }
     const Xpt = () => {
         const {
             user: e,
             isAuthenticated: t
-        } = Nv(), n = Yt(Ap), [r, i] = Wi(M_), [a, o] = Wi(eM), s = Yt(j_), l = Yt(h$), u = Yt(Xi), {
+        } = Nv(), n = Xt(Ap), [r, i] = Wi(M_), [a, o] = Wi(eM), s = Xt(j_), l = Xt(h$), u = Xt(ba), {
             persistChatLocally: d
         } = uie(), [p, f] = k.useState(!0), g = k.useCallback(async y => {
             const _ = n == null ? void 0 : n.socket.id;
             if (!_) return;
             const E = {
                 author: (e == null ? void 0 : e.name) || "User",
                 authorIsUser: !0,
@@ -83512,15 +83516,15 @@
 
     function ght() {
         const e = ti(eM),
             t = ti(j_),
             n = ti(h$),
             r = ti(mM),
             i = ti(tM),
-            a = Yt(Ap);
+            a = Xt(Ap);
         return () => {
             a == null || a.socket.disconnect(), a == null || a.socket.connect(), e([]), t([]), n([]), r(void 0), i(0)
         }
     }
     var b$ = {},
         mht = ir;
     Object.defineProperty(b$, "__esModule", {
@@ -83702,15 +83706,15 @@
                 }, r.to)
             })
         })
     }
 
     function mie() {
         var n;
-        const e = Yt(Xi),
+        const e = Xt(ba),
             t = !!((n = e == null ? void 0 : e.userEnv) != null && n.length);
         return O.jsx(cTe, {
             elevation: 0,
             color: "transparent",
             position: "static",
             children: O.jsxs(eOe, {
                 sx: {
@@ -83756,15 +83760,15 @@
     }) => {
         const {
             isProjectMember: t,
             isAuthenticated: n,
             isLoading: r,
             role: i,
             accessToken: a
-        } = Nv(), o = Yt(Xi), s = Gc(), l = Yt(O_), u = o && o.public === !1;
+        } = Nv(), o = Xt(ba), s = Gc(), l = Xt(O_), u = o && o.public === !1;
         if (k.useEffect(() => {
                 u && !n && !r && s("/login")
             }, [o, n, r]), k.useEffect(() => {
                 if (o != null && o.userEnv)
                     for (const p of o.userEnv) l[p] || s("/env")
             }, [o, l]), u && !a) return null;
         const d = u && i && !t;
@@ -83837,15 +83841,15 @@
         }
       }
     }
   }
 `;
 
     function Oht() {
-        const [e, t] = Wi(kw), n = Yt(Xi), {
+        const [e, t] = Wi(kw), n = Xt(ba), {
             data: r,
             loading: i,
             error: a
         } = gP(Iht, {
             variables: {
                 projectId: n == null ? void 0 : n.projectId
             }
@@ -84043,15 +84047,15 @@
                 gi = /\{(?:\n\/\* \[wrapped with .+\] \*\/)?\n?/,
                 bs = /\{\n\/\* \[wrapped with (.+)\] \*/,
                 mi = /,? & /,
                 Wr = /[^\x00-\x2f\x3a-\x40\x5b-\x60\x7b-\x7f]+/g,
                 pl = /[()=,{}\[\]\/\s]/,
                 kn = /\\(\\)?/g,
                 In = /\$\{([^\\}]*(?:\\.[^\\}]*)*)\}/g,
-                ta = /\w*$/,
+                ea = /\w*$/,
                 ar = /^[-+]0x[0-9a-f]+$/i,
                 Dt = /^0b[01]+$/i,
                 Nu = /^\[object .+?Constructor\]$/,
                 cd = /^0o[0-7]+$/i,
                 st = /^(?:0|[1-9]\d*)$/,
                 mr = /[\xc0-\xd6\xd8-\xf6\xf8-\xff\u0100-\u017f]/g,
                 oo = /($^)/,
@@ -84373,15 +84377,15 @@
             }
 
             function ay(Y, ye) {
                 for (var me = Y == null ? 0 : Y.length; me-- && ye(Y[me], me, Y) !== !1;);
                 return Y
             }
 
-            function na(Y, ye) {
+            function ta(Y, ye) {
                 for (var me = -1, Be = Y == null ? 0 : Y.length; ++me < Be;)
                     if (!ye(Y[me], me, Y)) return !1;
                 return !0
             }
 
             function Sa(Y, ye) {
                 for (var me = -1, Be = Y == null ? 0 : Y.length, nt = 0, _t = []; ++me < Be;) {
@@ -84791,21 +84795,21 @@
                             lt = 0,
                             bt = li(_e, this.__takeCount__);
                         if (!w || !R && P == _e && bt == _e) return n2(c, this.__actions__);
                         var Rt = [];
                         e: for (; _e-- && lt < bt;) {
                             Me += h;
                             for (var zt = -1, kt = c[Me]; ++zt < Ge;) {
-                                var Xt = $e[zt],
-                                    nn = Xt.iteratee,
-                                    aa = Xt.type,
+                                var Yt = $e[zt],
+                                    nn = Yt.iteratee,
+                                    ia = Yt.type,
                                     Si = nn(kt);
-                                if (aa == ce) kt = Si;
+                                if (ia == ce) kt = Si;
                                 else if (!Si) {
-                                    if (aa == J) continue e;
+                                    if (ia == J) continue e;
                                     break e
                                 }
                             }
                             Rt[lt++] = kt
                         }
                         return Rt
                     }
@@ -85066,21 +85070,21 @@
                             }
                         }
                         G || (G = new po);
                         var bt = G.get(c);
                         if (bt) return bt;
                         G.set(c, ae), J2(c) ? c.forEach(function(kt) {
                             ae.add(Ta(kt, h, w, kt, c, G))
-                        }) : Z2(c) && c.forEach(function(kt, Xt) {
-                            ae.set(Xt, Ta(kt, h, w, Xt, c, G))
+                        }) : Z2(c) && c.forEach(function(kt, Yt) {
+                            ae.set(Yt, Ta(kt, h, w, Yt, c, G))
                         });
                         var Rt = Me ? _e ? lx : sx : _e ? Ni : $r,
                             zt = $e ? n : Rt(c);
-                        return yi(zt || c, function(kt, Xt) {
-                            zt && (Xt = kt, kt = c[Xt]), bh(ae, Xt, Ta(kt, h, w, Xt, c, G))
+                        return yi(zt || c, function(kt, Yt) {
+                            zt && (Yt = kt, kt = c[Yt]), bh(ae, Yt, Ta(kt, h, w, Yt, c, G))
                         }), ae
                     }
 
                     function Lae(c) {
                         var h = $r(c);
                         return function(w) {
                             return M$(w, c, h)
@@ -85136,15 +85140,15 @@
                         }), w
                     }
 
                     function Ay(c, h, w) {
                         for (var R = -1, P = c.length; ++R < P;) {
                             var G = c[R],
                                 ae = h(G);
-                            if (ae != null && (he === n ? ae === ae && !ia(ae) : w(ae, he))) var he = ae,
+                            if (ae != null && (he === n ? ae === ae && !ra(ae) : w(ae, he))) var he = ae,
                                 _e = G
                         }
                         return _e
                     }
 
                     function Mae(c, h, w, R) {
                         var P = c.length;
@@ -85562,33 +85566,33 @@
                     function Iy(c, h, w) {
                         var R = 0,
                             P = c == null ? R : c.length;
                         if (typeof h == "number" && h === h && P <= ge) {
                             for (; R < P;) {
                                 var G = R + P >>> 1,
                                     ae = c[G];
-                                ae !== null && !ia(ae) && (w ? ae <= h : ae < h) ? R = G + 1 : P = G
+                                ae !== null && !ra(ae) && (w ? ae <= h : ae < h) ? R = G + 1 : P = G
                             }
                             return P
                         }
                         return Jw(c, h, Di, w)
                     }
 
                     function Jw(c, h, w, R) {
                         var P = 0,
                             G = c == null ? 0 : c.length;
                         if (G === 0) return 0;
                         h = w(h);
-                        for (var ae = h !== h, he = h === null, _e = ia(h), Me = h === n; P < G;) {
+                        for (var ae = h !== h, he = h === null, _e = ra(h), Me = h === n; P < G;) {
                             var $e = _y((P + G) / 2),
                                 Ge = w(c[$e]),
                                 lt = Ge !== n,
                                 bt = Ge === null,
                                 Rt = Ge === Ge,
-                                zt = ia(Ge);
+                                zt = ra(Ge);
                             if (ae) var kt = R || Rt;
                             else Me ? kt = Rt && (R || lt) : he ? kt = Rt && lt && (R || !bt) : _e ? kt = Rt && lt && !bt && (R || !zt) : bt || zt ? kt = !1 : kt = R ? Ge <= h : Ge < h;
                             kt ? P = $e + 1 : G = $e
                         }
                         return li(G, D)
                     }
 
@@ -85601,21 +85605,21 @@
                                 G[P++] = ae === 0 ? 0 : ae
                             }
                         }
                         return G
                     }
 
                     function e2(c) {
-                        return typeof c == "number" ? c : ia(c) ? re : +c
+                        return typeof c == "number" ? c : ra(c) ? re : +c
                     }
 
-                    function ra(c) {
+                    function na(c) {
                         if (typeof c == "string") return c;
-                        if (Ft(c)) return Wt(c, ra) + "";
-                        if (ia(c)) return N$ ? N$.call(c) : "";
+                        if (Ft(c)) return Wt(c, na) + "";
+                        if (ra(c)) return N$ ? N$.call(c) : "";
                         var h = c + "";
                         return h == "0" && 1 / c == -be ? "-0" : h
                     }
 
                     function xl(c, h, w) {
                         var R = -1,
                             P = Pu,
@@ -85713,15 +85717,15 @@
 
                     function aoe(c, h) {
                         var w = h ? ix(c.buffer) : c.buffer;
                         return new c.constructor(w, c.byteOffset, c.byteLength)
                     }
 
                     function ooe(c) {
-                        var h = new c.constructor(c.source, ta.exec(c));
+                        var h = new c.constructor(c.source, ea.exec(c));
                         return h.lastIndex = c.lastIndex, h
                     }
 
                     function soe(c) {
                         return yh ? Gt(yh.call(c)) : {}
                     }
 
@@ -85731,19 +85735,19 @@
                     }
 
                     function s2(c, h) {
                         if (c !== h) {
                             var w = c !== n,
                                 R = c === null,
                                 P = c === c,
-                                G = ia(c),
+                                G = ra(c),
                                 ae = h !== n,
                                 he = h === null,
                                 _e = h === h,
-                                Me = ia(h);
+                                Me = ra(h);
                             if (!he && !Me && !G && c > h || G && ae && _e && !he && !Me || R && ae && _e || !w && _e || !P) return 1;
                             if (!R && !G && !Me && c < h || Me && w && P && !R && !G || he && w && P || !ae && P || !_e) return -1
                         }
                         return 0
                     }
 
                     function loe(c, h, w) {
@@ -85952,24 +85956,24 @@
                             Ge = h & _,
                             lt = h & E,
                             bt = h & (S | x),
                             Rt = h & M,
                             zt = lt ? n : xh(c);
 
                         function kt() {
-                            for (var Xt = arguments.length, nn = me(Xt), aa = Xt; aa--;) nn[aa] = arguments[aa];
+                            for (var Yt = arguments.length, nn = me(Yt), ia = Yt; ia--;) nn[ia] = arguments[ia];
                             if (bt) var Si = Od(kt),
-                                oa = _a(nn, Si);
-                            if (R && (nn = l2(nn, R, P, bt)), G && (nn = u2(nn, G, ae, bt)), Xt -= oa, bt && Xt < Me) {
+                                aa = _a(nn, Si);
+                            if (R && (nn = l2(nn, R, P, bt)), G && (nn = u2(nn, G, ae, bt)), Yt -= aa, bt && Yt < Me) {
                                 var yr = Mo(nn, Si);
-                                return v2(c, h, Dy, kt.placeholder, w, nn, yr, he, _e, Me - Xt)
+                                return v2(c, h, Dy, kt.placeholder, w, nn, yr, he, _e, Me - Yt)
                             }
                             var go = Ge ? w : this,
                                 Os = lt ? go[c] : c;
-                            return Xt = nn.length, he ? nn = Noe(nn, he) : Rt && Xt > 1 && nn.reverse(), $e && _e < Xt && (nn.length = _e), this && this !== Ir && this instanceof kt && (Os = zt || xh(Os)), Os.apply(go, nn)
+                            return Yt = nn.length, he ? nn = Noe(nn, he) : Rt && Yt > 1 && nn.reverse(), $e && _e < Yt && (nn.length = _e), this && this !== Ir && this instanceof kt && (Os = zt || xh(Os)), Os.apply(go, nn)
                         }
                         return kt
                     }
 
                     function g2(c, h) {
                         return function(w, R) {
                             return Uae(w, c, h(R), {})
@@ -85978,15 +85982,15 @@
 
                     function Ly(c, h) {
                         return function(w, R) {
                             var P;
                             if (w === n && R === n) return h;
                             if (w !== n && (P = w), R !== n) {
                                 if (P === n) return R;
-                                typeof w == "string" || typeof R == "string" ? (w = ra(w), R = ra(R)) : (w = e2(w), R = e2(R)), P = c(w, R)
+                                typeof w == "string" || typeof R == "string" ? (w = na(w), R = na(R)) : (w = e2(w), R = e2(R)), P = c(w, R)
                             }
                             return P
                         }
                     }
 
                     function ax(c) {
                         return As(function(h) {
@@ -85996,15 +86000,15 @@
                                     return $t(P, R, w)
                                 })
                             })
                         })
                     }
 
                     function Fy(c, h) {
-                        h = h === n ? " " : ra(h);
+                        h = h === n ? " " : na(h);
                         var w = h.length;
                         if (w < 2) return w ? Qw(h, c) : h;
                         var R = Qw(h, Sy(c / T(h)));
                         return fo(h) ? Cl(N(R), 0, c).join("") : R.slice(0, c)
                     }
 
                     function poe(c, h, w, R) {
@@ -86111,16 +86115,16 @@
                             if (R) var kt = ae ? R(zt, Rt, Ge, h, c, G) : R(Rt, zt, Ge, c, h, G);
                             if (kt !== n) {
                                 if (kt) continue;
                                 lt = !1;
                                 break
                             }
                             if (bt) {
-                                if (!oh(h, function(Xt, nn) {
-                                        if (!co(bt, nn) && (Rt === Xt || P(Rt, Xt, w, R, G))) return bt.push(nn)
+                                if (!oh(h, function(Yt, nn) {
+                                        if (!co(bt, nn) && (Rt === Yt || P(Rt, Yt, w, R, G))) return bt.push(nn)
                                     })) {
                                     lt = !1;
                                     break
                                 }
                             } else if (!(Rt === zt || P(Rt, zt, w, R, G))) {
                                 lt = !1;
                                 break
@@ -86175,27 +86179,27 @@
                         var bt = G.get(c),
                             Rt = G.get(h);
                         if (bt && Rt) return bt == h && Rt == c;
                         var zt = !0;
                         G.set(c, h), G.set(h, c);
                         for (var kt = ae; ++Ge < _e;) {
                             lt = he[Ge];
-                            var Xt = c[lt],
+                            var Yt = c[lt],
                                 nn = h[lt];
-                            if (R) var aa = ae ? R(nn, Xt, lt, h, c, G) : R(Xt, nn, lt, c, h, G);
-                            if (!(aa === n ? Xt === nn || P(Xt, nn, w, R, G) : aa)) {
+                            if (R) var ia = ae ? R(nn, Yt, lt, h, c, G) : R(Yt, nn, lt, c, h, G);
+                            if (!(ia === n ? Yt === nn || P(Yt, nn, w, R, G) : ia)) {
                                 zt = !1;
                                 break
                             }
                             kt || (kt = lt == "constructor")
                         }
                         if (zt && !kt) {
                             var Si = c.constructor,
-                                oa = h.constructor;
-                            Si != oa && "constructor" in c && "constructor" in h && !(typeof Si == "function" && Si instanceof Si && typeof oa == "function" && oa instanceof oa) && (zt = !1)
+                                aa = h.constructor;
+                            Si != aa && "constructor" in c && "constructor" in h && !(typeof Si == "function" && Si instanceof Si && typeof aa == "function" && aa instanceof aa) && (zt = !1)
                         }
                         return G.delete(c), G.delete(h), zt
                     }
 
                     function As(c) {
                         return gx(A2(c, n, M2), c + "")
                     }
@@ -86395,15 +86399,15 @@
                         var R = typeof h;
                         return (R == "number" ? Oi(w) && Rs(h, w.length) : R == "string" && h in w) ? ho(w[h], c) : !1
                     }
 
                     function fx(c, h) {
                         if (Ft(c)) return !1;
                         var w = typeof c;
-                        return w == "number" || w == "symbol" || w == "boolean" || c == null || ia(c) ? !0 : hr.test(c) || !Zt.test(c) || h != null && c in Gt(h)
+                        return w == "number" || w == "symbol" || w == "boolean" || c == null || ra(c) ? !0 : hr.test(c) || !Zt.test(c) || h != null && c in Gt(h)
                     }
 
                     function Toe(c) {
                         var h = typeof c;
                         return h == "string" || h == "number" || h == "symbol" || h == "boolean" ? c !== "__proto__" : c === null
                     }
 
@@ -86536,15 +86540,15 @@
                         var h = [];
                         return c.charCodeAt(0) === 46 && h.push(""), c.replace(Cn, function(w, R, P, G) {
                             h.push(P ? G.replace(kn, "$1") : R || w)
                         }), h
                     });
 
                     function Bo(c) {
-                        if (typeof c == "string" || ia(c)) return c;
+                        if (typeof c == "string" || ra(c)) return c;
                         var h = c + "";
                         return h == "0" && 1 / c == -be ? "-0" : h
                     }
 
                     function Wu(c) {
                         if (c != null) {
                             try {
@@ -86966,15 +86970,15 @@
                         return n2(this.__wrapped__, this.__actions__)
                     }
                     var Vse = Ny(function(c, h, w) {
                         Sn.call(c, w) ? ++c[w] : Ts(c, w, 1)
                     });
 
                     function Hse(c, h, w) {
-                        var R = Ft(c) ? na : Fae;
+                        var R = Ft(c) ? ta : Fae;
                         return w && Ei(c, h, w) && (h = n), R(c, Ct(h, 3))
                     }
 
                     function Wse(c, h) {
                         var w = Ft(c) ? Sa : B$;
                         return w(c, Ct(h, 3))
                     }
@@ -87153,15 +87157,15 @@
                         function bt(yr) {
                             var go = R,
                                 Os = P;
                             return R = P = n, Me = yr, ae = c.apply(Os, go), ae
                         }
 
                         function Rt(yr) {
-                            return Me = yr, he = Ch(Xt, h), $e ? bt(yr) : ae
+                            return Me = yr, he = Ch(Yt, h), $e ? bt(yr) : ae
                         }
 
                         function zt(yr) {
                             var go = yr - _e,
                                 Os = yr - Me,
                                 pB = h - go;
                             return Ge ? li(pB, G - Os) : pB
@@ -87169,42 +87173,42 @@
 
                         function kt(yr) {
                             var go = yr - _e,
                                 Os = yr - Me;
                             return _e === n || go >= h || go < 0 || Ge && Os >= G
                         }
 
-                        function Xt() {
+                        function Yt() {
                             var yr = jy();
                             if (kt(yr)) return nn(yr);
-                            he = Ch(Xt, zt(yr))
+                            he = Ch(Yt, zt(yr))
                         }
 
                         function nn(yr) {
                             return he = n, lt && R ? bt(yr) : (R = P = n, ae)
                         }
 
-                        function aa() {
+                        function ia() {
                             he !== n && i2(he), Me = 0, R = _e = P = he = n
                         }
 
                         function Si() {
                             return he === n ? ae : nn(jy())
                         }
 
-                        function oa() {
+                        function aa() {
                             var yr = jy(),
                                 go = kt(yr);
                             if (R = arguments, P = this, _e = yr, go) {
                                 if (he === n) return Rt(_e);
-                                if (Ge) return i2(he), he = Ch(Xt, h), bt(_e)
+                                if (Ge) return i2(he), he = Ch(Yt, h), bt(_e)
                             }
-                            return he === n && (he = Ch(Xt, h)), ae
+                            return he === n && (he = Ch(Yt, h)), ae
                         }
-                        return oa.cancel = aa, oa.flush = Si, oa
+                        return aa.cancel = ia, aa.flush = Si, aa
                     }
                     var hle = Ht(function(c, h) {
                             return P$(c, 1, h)
                         }),
                         gle = Ht(function(c, h, w) {
                             return P$(c, Ra(h) || 0, w)
                         });
@@ -87458,15 +87462,15 @@
                     }
                     var J2 = ah ? si(ah) : Wae;
 
                     function Wy(c) {
                         return typeof c == "string" || !Ft(c) && sr(c) && bi(c) == xe
                     }
 
-                    function ia(c) {
+                    function ra(c) {
                         return typeof c == "symbol" || sr(c) && bi(c) == Ae
                     }
                     var Nd = vd ? si(vd) : Gae;
 
                     function Kle(c) {
                         return c === n
                     }
@@ -87509,15 +87513,15 @@
 
                     function tB(c) {
                         return c ? qu(Bt(c), 0, $) : 0
                     }
 
                     function Ra(c) {
                         if (typeof c == "number") return c;
-                        if (ia(c)) return re;
+                        if (ra(c)) return re;
                         if (Qn(c)) {
                             var h = typeof c.valueOf == "function" ? c.valueOf() : c;
                             c = Qn(h) ? h + "" : h
                         }
                         if (typeof c != "string") return c === 0 ? c : +c;
                         c = ch(c);
                         var w = Dt.test(c);
@@ -87529,15 +87533,15 @@
                     }
 
                     function Jle(c) {
                         return c ? qu(Bt(c), -Q, Q) : c === 0 ? c : 0
                     }
 
                     function yn(c) {
-                        return c == null ? "" : ra(c)
+                        return c == null ? "" : na(c)
                     }
                     var eue = kd(function(c, h) {
                             if (Th(h) || Oi(h)) {
                                 $o(h, $r(h), c);
                                 return
                             }
                             for (var w in h) Sn.call(h, w) && bh(c, w, h[w])
@@ -87762,15 +87766,15 @@
                     }
 
                     function uB(c) {
                         return c = yn(c), c && c.replace(mr, Pr).replace(gd, "")
                     }
 
                     function Mue(c, h, w) {
-                        c = yn(c), h = ra(h);
+                        c = yn(c), h = na(h);
                         var R = c.length;
                         w = w === n ? R : qu(Bt(w), 0, R);
                         var P = w;
                         return w -= h.length, w >= 0 && c.slice(w, P) == h
                     }
 
                     function Pue(c) {
@@ -87822,44 +87826,44 @@
                         return c.length < 3 ? h : h.replace(c[1], c[2])
                     }
                     var Kue = Id(function(c, h, w) {
                         return c + (w ? "_" : "") + h.toLowerCase()
                     });
 
                     function Yue(c, h, w) {
-                        return w && typeof w != "number" && Ei(c, h, w) && (h = w = n), w = w === n ? $ : w >>> 0, w ? (c = yn(c), c && (typeof h == "string" || h != null && !Sx(h)) && (h = ra(h), !h && fo(c)) ? Cl(N(c), 0, w) : c.split(h, w)) : []
+                        return w && typeof w != "number" && Ei(c, h, w) && (h = w = n), w = w === n ? $ : w >>> 0, w ? (c = yn(c), c && (typeof h == "string" || h != null && !Sx(h)) && (h = na(h), !h && fo(c)) ? Cl(N(c), 0, w) : c.split(h, w)) : []
                     }
                     var Xue = Id(function(c, h, w) {
                         return c + (w ? " " : "") + xx(h)
                     });
 
                     function Zue(c, h, w) {
-                        return c = yn(c), w = w == null ? 0 : qu(Bt(w), 0, c.length), h = ra(h), c.slice(w, w + h.length) == h
+                        return c = yn(c), w = w == null ? 0 : qu(Bt(w), 0, c.length), h = na(h), c.slice(w, w + h.length) == h
                     }
 
                     function Que(c, h, w) {
                         var R = H.templateSettings;
                         w && Ei(c, h, w) && (h = n), c = yn(c), h = Gy({}, h, R, b2);
                         var P = Gy({}, h.imports, R.imports, b2),
                             G = $r(P),
                             ae = Fo(P, G),
                             he, _e, Me = 0,
                             $e = h.interpolate || oo,
                             Ge = "__p += '",
                             lt = Sl((h.escape || oo).source + "|" + $e.source + "|" + ($e === tn ? In : oo).source + "|" + (h.evaluate || oo).source + "|$", "g"),
                             bt = "//# sourceURL=" + (Sn.call(h, "sourceURL") ? (h.sourceURL + "").replace(/\s/g, " ") : "lodash.templateSources[" + ++md + "]") + `
 `;
-                        c.replace(lt, function(kt, Xt, nn, aa, Si, oa) {
-                            return nn || (nn = aa), Ge += c.slice(Me, oa).replace(Du, Fw), Xt && (he = !0, Ge += `' +
-__e(` + Xt + `) +
+                        c.replace(lt, function(kt, Yt, nn, ia, Si, aa) {
+                            return nn || (nn = ia), Ge += c.slice(Me, aa).replace(Du, Fw), Yt && (he = !0, Ge += `' +
+__e(` + Yt + `) +
 '`), Si && (_e = !0, Ge += `';
 ` + Si + `;
 __p += '`), nn && (Ge += `' +
 ((__t = (` + nn + `)) == null ? '' : __t) +
-'`), Me = oa + kt.length, kt
+'`), Me = aa + kt.length, kt
                         }), Ge += `';
 `;
                         var Rt = Sn.call(h, "variable") && h.variable;
                         if (!Rt) Ge = `with (obj) {
 ` + Ge + `
 }
 `;
@@ -87884,44 +87888,44 @@
 
                     function ece(c) {
                         return yn(c).toUpperCase()
                     }
 
                     function tce(c, h, w) {
                         if (c = yn(c), c && (w || h === n)) return ch(c);
-                        if (!c || !(h = ra(h))) return c;
+                        if (!c || !(h = na(h))) return c;
                         var R = N(c),
                             P = N(h),
                             G = dh(R, P),
                             ae = _d(R, P) + 1;
                         return Cl(R, G, ae).join("")
                     }
 
                     function nce(c, h, w) {
                         if (c = yn(c), c && (w || h === n)) return c.slice(0, L(c) + 1);
-                        if (!c || !(h = ra(h))) return c;
+                        if (!c || !(h = na(h))) return c;
                         var R = N(c),
                             P = _d(R, N(h)) + 1;
                         return Cl(R, 0, P).join("")
                     }
 
                     function rce(c, h, w) {
                         if (c = yn(c), c && (w || h === n)) return c.replace(Sr, "");
-                        if (!c || !(h = ra(h))) return c;
+                        if (!c || !(h = na(h))) return c;
                         var R = N(c),
                             P = dh(R, N(h));
                         return Cl(R, P).join("")
                     }
 
                     function ice(c, h) {
                         var w = U,
                             R = j;
                         if (Qn(h)) {
                             var P = "separator" in h ? h.separator : P;
-                            w = "length" in h ? Bt(h.length) : w, R = "omission" in h ? ra(h.omission) : R
+                            w = "length" in h ? Bt(h.length) : w, R = "omission" in h ? na(h.omission) : R
                         }
                         c = yn(c);
                         var G = c.length;
                         if (fo(c)) {
                             var ae = N(c);
                             G = ae.length
                         }
@@ -87929,18 +87933,18 @@
                         var he = w - T(R);
                         if (he < 1) return R;
                         var _e = ae ? Cl(ae, 0, he).join("") : c.slice(0, he);
                         if (P === n) return _e + R;
                         if (ae && (he += _e.length - he), Sx(P)) {
                             if (c.slice(he).search(P)) {
                                 var Me, $e = _e;
-                                for (P.global || (P = Sl(P.source, yn(ta.exec(P)) + "g")), P.lastIndex = 0; Me = P.exec($e);) var Ge = Me.index;
+                                for (P.global || (P = Sl(P.source, yn(ea.exec(P)) + "g")), P.lastIndex = 0; Me = P.exec($e);) var Ge = Me.index;
                                 _e = _e.slice(0, Ge === n ? he : Ge)
                             }
-                        } else if (c.indexOf(ra(P), he) != he) {
+                        } else if (c.indexOf(na(P), he) != he) {
                             var lt = _e.lastIndexOf(P);
                             lt > -1 && (_e = _e.slice(0, lt))
                         }
                         return _e + R
                     }
 
                     function ace(c) {
@@ -88055,15 +88059,15 @@
 
                     function yce(c) {
                         return c = Bt(c), Ht(function(h) {
                             return K$(h, c)
                         })
                     }
                     var bce = ax(Wt),
-                        Ece = ax(na),
+                        Ece = ax(ta),
                         Sce = ax(oh);
 
                     function fB(c) {
                         return fx(c) ? ki(Bo(c)) : Zae(c)
                     }
 
                     function _ce(c) {
@@ -88100,15 +88104,15 @@
                             R = li(c, $);
                         h = Ct(h), c -= $;
                         for (var P = Bu(R, h); ++w < c;) h(w);
                         return P
                     }
 
                     function kce(c) {
-                        return Ft(c) ? Wt(c, Bo) : ia(c) ? [c] : Ii(N2(yn(c)))
+                        return Ft(c) ? Wt(c, Bo) : ra(c) ? [c] : Ii(N2(yn(c)))
                     }
 
                     function Ice(c) {
                         var h = ++zie;
                         return yn(c) + h
                     }
                     var Oce = Ly(function(c, h) {
@@ -88154,15 +88158,15 @@
                     function Vce(c) {
                         return c && c.length ? Sd(c, Di) : 0
                     }
 
                     function Hce(c, h) {
                         return c && c.length ? Sd(c, Ct(h, 2)) : 0
                     }
-                    return H.after = ple, H.ary = q2, H.assign = eue, H.assignIn = rB, H.assignInWith = Gy, H.assignWith = tue, H.at = nue, H.before = V2, H.bind = yx, H.bindAll = sce, H.bindKey = H2, H.castArray = Tle, H.chain = U2, H.chunk = Loe, H.compact = Foe, H.concat = Moe, H.cond = lce, H.conforms = uce, H.constant = Tx, H.countBy = Vse, H.create = rue, H.curry = W2, H.curryRight = G2, H.debounce = K2, H.defaults = iue, H.defaultsDeep = aue, H.defer = hle, H.delay = gle, H.difference = Poe, H.differenceBy = $oe, H.differenceWith = Boe, H.drop = Uoe, H.dropRight = zoe, H.dropRightWhile = joe, H.dropWhile = qoe, H.fill = Voe, H.filter = Wse, H.flatMap = Yse, H.flatMapDeep = Xse, H.flatMapDepth = Zse, H.flatten = M2, H.flattenDeep = Hoe, H.flattenDepth = Woe, H.flip = mle, H.flow = dce, H.flowRight = fce, H.fromPairs = Goe, H.functions = fue, H.functionsIn = pue, H.groupBy = Qse, H.initial = Yoe, H.intersection = Xoe, H.intersectionBy = Zoe, H.intersectionWith = Qoe, H.invert = gue, H.invertBy = mue, H.invokeMap = ele, H.iteratee = Cx, H.keyBy = tle, H.keys = $r, H.keysIn = Ni, H.map = zy, H.mapKeys = yue, H.mapValues = bue, H.matches = pce, H.matchesProperty = hce, H.memoize = qy, H.merge = Eue, H.mergeWith = iB, H.method = gce, H.methodOf = mce, H.mixin = Ax, H.negate = Vy, H.nthArg = yce, H.omit = Sue, H.omitBy = _ue, H.once = vle, H.orderBy = nle, H.over = bce, H.overArgs = yle, H.overEvery = Ece, H.overSome = Sce, H.partial = bx, H.partialRight = Y2, H.partition = rle, H.pick = wue, H.pickBy = aB, H.property = fB, H.propertyOf = _ce, H.pull = nse, H.pullAll = $2, H.pullAllBy = rse, H.pullAllWith = ise, H.pullAt = ase, H.range = wce, H.rangeRight = xce, H.rearg = ble, H.reject = ole, H.remove = ose, H.rest = Ele, H.reverse = mx, H.sampleSize = lle, H.set = Tue, H.setWith = Cue, H.shuffle = ule, H.slice = sse, H.sortBy = fle, H.sortedUniq = hse, H.sortedUniqBy = gse, H.split = Yue, H.spread = Sle, H.tail = mse, H.take = vse, H.takeRight = yse, H.takeRightWhile = bse, H.takeWhile = Ese, H.tap = Fse, H.throttle = _le, H.thru = Uy, H.toArray = eB, H.toPairs = oB, H.toPairsIn = sB, H.toPath = kce, H.toPlainObject = nB, H.transform = Aue, H.unary = wle, H.union = Sse, H.unionBy = _se, H.unionWith = wse, H.uniq = xse, H.uniqBy = Tse, H.uniqWith = Cse, H.unset = Rue, H.unzip = vx, H.unzipWith = B2, H.update = kue, H.updateWith = Iue, H.values = Dd, H.valuesIn = Oue, H.without = Ase, H.words = cB, H.wrap = xle, H.xor = Rse, H.xorBy = kse, H.xorWith = Ise, H.zip = Ose, H.zipObject = Nse, H.zipObjectDeep = Dse, H.zipWith = Lse, H.entries = oB, H.entriesIn = sB, H.extend = rB, H.extendWith = Gy, Ax(H, H), H.add = Oce, H.attempt = dB, H.camelCase = Fue, H.capitalize = lB, H.ceil = Nce, H.clamp = Nue, H.clone = Cle, H.cloneDeep = Rle, H.cloneDeepWith = kle, H.cloneWith = Ale, H.conformsTo = Ile, H.deburr = uB, H.defaultTo = cce, H.divide = Dce, H.endsWith = Mue, H.eq = ho, H.escape = Pue, H.escapeRegExp = $ue, H.every = Hse, H.find = Gse, H.findIndex = L2, H.findKey = oue, H.findLast = Kse, H.findLastIndex = F2, H.findLastKey = sue, H.floor = Lce, H.forEach = z2, H.forEachRight = j2, H.forIn = lue, H.forInRight = uue, H.forOwn = cue, H.forOwnRight = due, H.get = _x, H.gt = Ole, H.gte = Nle, H.has = hue, H.hasIn = wx, H.head = P2, H.identity = Di, H.includes = Jse, H.indexOf = Koe, H.inRange = Due, H.invoke = vue, H.isArguments = Gu, H.isArray = Ft, H.isArrayBuffer = Dle, H.isArrayLike = Oi, H.isArrayLikeObject = vr, H.isBoolean = Lle, H.isBuffer = Al, H.isDate = Fle, H.isElement = Mle, H.isEmpty = Ple, H.isEqual = $le, H.isEqualWith = Ble, H.isError = Ex, H.isFinite = Ule, H.isFunction = ks, H.isInteger = X2, H.isLength = Hy, H.isMap = Z2, H.isMatch = zle, H.isMatchWith = jle, H.isNaN = qle, H.isNative = Vle, H.isNil = Wle, H.isNull = Hle, H.isNumber = Q2, H.isObject = Qn, H.isObjectLike = sr, H.isPlainObject = Ah, H.isRegExp = Sx, H.isSafeInteger = Gle, H.isSet = J2, H.isString = Wy, H.isSymbol = ia, H.isTypedArray = Nd, H.isUndefined = Kle, H.isWeakMap = Yle, H.isWeakSet = Xle, H.join = Joe, H.kebabCase = Bue, H.last = Aa, H.lastIndexOf = ese, H.lowerCase = Uue, H.lowerFirst = zue, H.lt = Zle, H.lte = Qle, H.max = Fce, H.maxBy = Mce, H.mean = Pce, H.meanBy = $ce, H.min = Bce, H.minBy = Uce, H.stubArray = kx, H.stubFalse = Ix, H.stubObject = Tce, H.stubString = Cce, H.stubTrue = Ace, H.multiply = zce, H.nth = tse, H.noConflict = vce, H.noop = Rx, H.now = jy, H.pad = jue, H.padEnd = que, H.padStart = Vue, H.parseInt = Hue, H.random = Lue, H.reduce = ile, H.reduceRight = ale, H.repeat = Wue, H.replace = Gue, H.result = xue, H.round = jce, H.runInContext = Y, H.sample = sle, H.size = cle, H.snakeCase = Kue, H.some = dle, H.sortedIndex = lse, H.sortedIndexBy = use, H.sortedIndexOf = cse, H.sortedLastIndex = dse, H.sortedLastIndexBy = fse, H.sortedLastIndexOf = pse, H.startCase = Xue, H.startsWith = Zue, H.subtract = qce, H.sum = Vce, H.sumBy = Hce, H.template = Que, H.times = Rce, H.toFinite = Is, H.toInteger = Bt, H.toLength = tB, H.toLower = Jue, H.toNumber = Ra, H.toSafeInteger = Jle, H.toString = yn, H.toUpper = ece, H.trim = tce, H.trimEnd = nce, H.trimStart = rce, H.truncate = ice, H.unescape = ace, H.uniqueId = Ice, H.upperCase = oce, H.upperFirst = xx, H.each = z2, H.eachRight = j2, H.first = P2, Ax(H, function() {
+                    return H.after = ple, H.ary = q2, H.assign = eue, H.assignIn = rB, H.assignInWith = Gy, H.assignWith = tue, H.at = nue, H.before = V2, H.bind = yx, H.bindAll = sce, H.bindKey = H2, H.castArray = Tle, H.chain = U2, H.chunk = Loe, H.compact = Foe, H.concat = Moe, H.cond = lce, H.conforms = uce, H.constant = Tx, H.countBy = Vse, H.create = rue, H.curry = W2, H.curryRight = G2, H.debounce = K2, H.defaults = iue, H.defaultsDeep = aue, H.defer = hle, H.delay = gle, H.difference = Poe, H.differenceBy = $oe, H.differenceWith = Boe, H.drop = Uoe, H.dropRight = zoe, H.dropRightWhile = joe, H.dropWhile = qoe, H.fill = Voe, H.filter = Wse, H.flatMap = Yse, H.flatMapDeep = Xse, H.flatMapDepth = Zse, H.flatten = M2, H.flattenDeep = Hoe, H.flattenDepth = Woe, H.flip = mle, H.flow = dce, H.flowRight = fce, H.fromPairs = Goe, H.functions = fue, H.functionsIn = pue, H.groupBy = Qse, H.initial = Yoe, H.intersection = Xoe, H.intersectionBy = Zoe, H.intersectionWith = Qoe, H.invert = gue, H.invertBy = mue, H.invokeMap = ele, H.iteratee = Cx, H.keyBy = tle, H.keys = $r, H.keysIn = Ni, H.map = zy, H.mapKeys = yue, H.mapValues = bue, H.matches = pce, H.matchesProperty = hce, H.memoize = qy, H.merge = Eue, H.mergeWith = iB, H.method = gce, H.methodOf = mce, H.mixin = Ax, H.negate = Vy, H.nthArg = yce, H.omit = Sue, H.omitBy = _ue, H.once = vle, H.orderBy = nle, H.over = bce, H.overArgs = yle, H.overEvery = Ece, H.overSome = Sce, H.partial = bx, H.partialRight = Y2, H.partition = rle, H.pick = wue, H.pickBy = aB, H.property = fB, H.propertyOf = _ce, H.pull = nse, H.pullAll = $2, H.pullAllBy = rse, H.pullAllWith = ise, H.pullAt = ase, H.range = wce, H.rangeRight = xce, H.rearg = ble, H.reject = ole, H.remove = ose, H.rest = Ele, H.reverse = mx, H.sampleSize = lle, H.set = Tue, H.setWith = Cue, H.shuffle = ule, H.slice = sse, H.sortBy = fle, H.sortedUniq = hse, H.sortedUniqBy = gse, H.split = Yue, H.spread = Sle, H.tail = mse, H.take = vse, H.takeRight = yse, H.takeRightWhile = bse, H.takeWhile = Ese, H.tap = Fse, H.throttle = _le, H.thru = Uy, H.toArray = eB, H.toPairs = oB, H.toPairsIn = sB, H.toPath = kce, H.toPlainObject = nB, H.transform = Aue, H.unary = wle, H.union = Sse, H.unionBy = _se, H.unionWith = wse, H.uniq = xse, H.uniqBy = Tse, H.uniqWith = Cse, H.unset = Rue, H.unzip = vx, H.unzipWith = B2, H.update = kue, H.updateWith = Iue, H.values = Dd, H.valuesIn = Oue, H.without = Ase, H.words = cB, H.wrap = xle, H.xor = Rse, H.xorBy = kse, H.xorWith = Ise, H.zip = Ose, H.zipObject = Nse, H.zipObjectDeep = Dse, H.zipWith = Lse, H.entries = oB, H.entriesIn = sB, H.extend = rB, H.extendWith = Gy, Ax(H, H), H.add = Oce, H.attempt = dB, H.camelCase = Fue, H.capitalize = lB, H.ceil = Nce, H.clamp = Nue, H.clone = Cle, H.cloneDeep = Rle, H.cloneDeepWith = kle, H.cloneWith = Ale, H.conformsTo = Ile, H.deburr = uB, H.defaultTo = cce, H.divide = Dce, H.endsWith = Mue, H.eq = ho, H.escape = Pue, H.escapeRegExp = $ue, H.every = Hse, H.find = Gse, H.findIndex = L2, H.findKey = oue, H.findLast = Kse, H.findLastIndex = F2, H.findLastKey = sue, H.floor = Lce, H.forEach = z2, H.forEachRight = j2, H.forIn = lue, H.forInRight = uue, H.forOwn = cue, H.forOwnRight = due, H.get = _x, H.gt = Ole, H.gte = Nle, H.has = hue, H.hasIn = wx, H.head = P2, H.identity = Di, H.includes = Jse, H.indexOf = Koe, H.inRange = Due, H.invoke = vue, H.isArguments = Gu, H.isArray = Ft, H.isArrayBuffer = Dle, H.isArrayLike = Oi, H.isArrayLikeObject = vr, H.isBoolean = Lle, H.isBuffer = Al, H.isDate = Fle, H.isElement = Mle, H.isEmpty = Ple, H.isEqual = $le, H.isEqualWith = Ble, H.isError = Ex, H.isFinite = Ule, H.isFunction = ks, H.isInteger = X2, H.isLength = Hy, H.isMap = Z2, H.isMatch = zle, H.isMatchWith = jle, H.isNaN = qle, H.isNative = Vle, H.isNil = Wle, H.isNull = Hle, H.isNumber = Q2, H.isObject = Qn, H.isObjectLike = sr, H.isPlainObject = Ah, H.isRegExp = Sx, H.isSafeInteger = Gle, H.isSet = J2, H.isString = Wy, H.isSymbol = ra, H.isTypedArray = Nd, H.isUndefined = Kle, H.isWeakMap = Yle, H.isWeakSet = Xle, H.join = Joe, H.kebabCase = Bue, H.last = Aa, H.lastIndexOf = ese, H.lowerCase = Uue, H.lowerFirst = zue, H.lt = Zle, H.lte = Qle, H.max = Fce, H.maxBy = Mce, H.mean = Pce, H.meanBy = $ce, H.min = Bce, H.minBy = Uce, H.stubArray = kx, H.stubFalse = Ix, H.stubObject = Tce, H.stubString = Cce, H.stubTrue = Ace, H.multiply = zce, H.nth = tse, H.noConflict = vce, H.noop = Rx, H.now = jy, H.pad = jue, H.padEnd = que, H.padStart = Vue, H.parseInt = Hue, H.random = Lue, H.reduce = ile, H.reduceRight = ale, H.repeat = Wue, H.replace = Gue, H.result = xue, H.round = jce, H.runInContext = Y, H.sample = sle, H.size = cle, H.snakeCase = Kue, H.some = dle, H.sortedIndex = lse, H.sortedIndexBy = use, H.sortedIndexOf = cse, H.sortedLastIndex = dse, H.sortedLastIndexBy = fse, H.sortedLastIndexOf = pse, H.startCase = Xue, H.startsWith = Zue, H.subtract = qce, H.sum = Vce, H.sumBy = Hce, H.template = Que, H.times = Rce, H.toFinite = Is, H.toInteger = Bt, H.toLength = tB, H.toLower = Jue, H.toNumber = Ra, H.toSafeInteger = Jle, H.toString = yn, H.toUpper = ece, H.trim = tce, H.trimEnd = nce, H.trimStart = rce, H.truncate = ice, H.unescape = ace, H.uniqueId = Ice, H.upperCase = oce, H.upperFirst = xx, H.each = z2, H.eachRight = j2, H.first = P2, Ax(H, function() {
                         var c = {};
                         return Po(H, function(h, w) {
                             Sn.call(H.prototype, w) || (c[w] = h)
                         }), c
                     }(), {
                         chain: !1
                     }), H.VERSION = r, yi(["bind", "bindKey", "curry", "curryRight", "partial", "partialRight"], function(c) {
@@ -88225,16 +88229,16 @@
                             G = R || /^find/.test(h);
                         P && (H.prototype[h] = function() {
                             var ae = this.__wrapped__,
                                 he = R ? [1] : arguments,
                                 _e = ae instanceof Qt,
                                 Me = he[0],
                                 $e = _e || Ft(ae),
-                                Ge = function(Xt) {
-                                    var nn = P.apply(H, Nn([Xt], he));
+                                Ge = function(Yt) {
+                                    var nn = P.apply(H, Nn([Yt], he));
                                     return R && lt ? nn[0] : nn
                                 };
                             $e && w && typeof Me == "function" && Me.length != 1 && (_e = $e = !1);
                             var lt = this.__chain__,
                                 bt = !!this.__actions__.length,
                                 Rt = G && !lt,
                                 zt = _e && !bt;
@@ -89288,16 +89292,16 @@
                 hour: "numeric",
                 minute: "numeric"
             };
             return new Date(e).toLocaleDateString(void 0, t)
         };
 
     function bgt() {
-        const e = Yt(kw),
-            t = Yt(Xi),
+        const e = Xt(kw),
+            t = Xt(ba),
             {
                 data: n,
                 loading: r,
                 error: i,
                 refetch: a,
                 fetchMore: o
             } = gP(vgt, {
@@ -89557,15 +89561,15 @@
                     })]
                 }), O.jsx(rie, {})]
             })
         })
     }
 
     function xgt() {
-        const [e, t] = Wi(O_), n = Yt(Xi), r = Gc();
+        const [e, t] = Wi(O_), n = Xt(ba), r = Gc();
         if (!(n != null && n.userEnv) || !(n != null && n.userEnv)) return null;
         const i = n.userEnv,
             a = {},
             o = {};
         i.forEach(d => {
             a[d] = e[d] || "", o[d] = QS().required()
         });
@@ -90988,15 +90992,15 @@
         return !0
     }
     const fmt = k.memo(function() {
             const {
                 accessToken: t,
                 isAuthenticated: n,
                 isLoading: r
-            } = Nv(), i = Yt(O_), a = ti(bv), [o, s] = Wi(Ap), l = ti(eM), u = ti(tM), d = ti(M_), p = ti(j_), f = ti(h$), g = r || n && !t;
+            } = Nv(), i = Xt(O_), a = ti(bv), [o, s] = Wi(Ap), l = ti(eM), u = ti(tM), d = ti(M_), p = ti(j_), f = ti(h$), g = r || n && !t;
             return k.useEffect(() => {
                 if (g) return;
                 o != null && o.socket && (o.socket.removeAllListeners(), o.socket.close());
                 const m = qE(yv, {
                     extraHeaders: {
                         Authorization: t || "",
                         "user-env": JSON.stringify(i)
@@ -91087,16 +91091,16 @@
             element: O.jsx($Z, {
                 replace: !0,
                 to: "/"
             })
         }]);
 
     function hmt() {
-        const e = Yt(F_),
-            [t, n] = Wi(Xi),
+        const e = Xt(F_),
+            [t, n] = Wi(ba),
             [r, i] = Wi(UZ),
             a = ti(zZ),
             {
                 isAuthenticated: o,
                 getAccessTokenSilently: s,
                 logout: l
             } = Nv(),
```

### Comparing `chainlit-0.2.0/chainlit/frontend/dist/assets/index-bdffdaa0.css` & `chainlit-0.2.1/chainlit/frontend/dist/assets/index-bdffdaa0.css`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg` & `chainlit-0.2.1/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg` & `chainlit-0.2.1/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/frontend/dist/favicon.svg` & `chainlit-0.2.1/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/frontend/dist/index.html` & `chainlit-0.2.1/chainlit/frontend/dist/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     <link
       href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap"
       rel="stylesheet"
     />
     <script>
       const global = globalThis;
     </script>
-    <script type="module" crossorigin src="/assets/index-b6b4925e.js"></script>
+    <script type="module" crossorigin src="/assets/index-03f89089.js"></script>
     <link rel="stylesheet" href="/assets/index-bdffdaa0.css">
   </head>
   <body>
     <div id="root"></div>
     
   </body>
 </html>
```

### Comparing `chainlit-0.2.0/chainlit/lc/chainlit_handler.py` & `chainlit-0.2.1/chainlit/lc/chainlit_handler.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/lc/monkey.py` & `chainlit-0.2.1/chainlit/lc/monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/lc/new_monkey.py` & `chainlit-0.2.1/chainlit/lc/new_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/lc/old_monkey.py` & `chainlit-0.2.1/chainlit/lc/old_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/lc/utils.py` & `chainlit-0.2.1/chainlit/lc/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/markdown.py` & `chainlit-0.2.1/chainlit/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/sdk.py` & `chainlit-0.2.1/chainlit/sdk.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/server.py` & `chainlit-0.2.1/chainlit/server.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/session.py` & `chainlit-0.2.1/chainlit/session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/telemetry.py` & `chainlit-0.2.1/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/types.py` & `chainlit-0.2.1/chainlit/types.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/user_session.py` & `chainlit-0.2.1/chainlit/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/chainlit/watch.py` & `chainlit-0.2.1/chainlit/watch.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.0/pyproject.toml` & `chainlit-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlit"
-version = "0.2.0"
+version = "0.2.1"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'langchain']
 description = "A faster way to build chatbot UIs."
 authors = ["Chainlit"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
```

### Comparing `chainlit-0.2.0/PKG-INFO` & `chainlit-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 0.2.0
+Version: 0.2.1
 Summary: A faster way to build chatbot UIs.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,langchain
 Author: Chainlit
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

