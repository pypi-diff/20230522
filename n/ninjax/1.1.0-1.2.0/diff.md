# Comparing `tmp/ninjax-1.1.0.tar.gz` & `tmp/ninjax-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjax-1.1.0.tar", last modified: Fri May 19 19:50:55 2023, max compression
+gzip compressed data, was "ninjax-1.2.0.tar", last modified: Mon May 22 09:42:34 2023, max compression
```

## Comparing `ninjax-1.1.0.tar` & `ninjax-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 19:50:55.316253 ninjax-1.1.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1071 2022-08-08 16:14:32.000000 ninjax-1.1.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9671 2023-05-19 19:50:55.316253 ninjax-1.1.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9261 2023-02-22 13:32:36.000000 ninjax-1.1.0/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 19:50:55.312253 ninjax-1.1.0/ninjax/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      507 2022-11-24 15:49:52.000000 ninjax-1.1.0/ninjax/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    17996 2023-05-19 19:50:00.000000 ninjax-1.1.0/ninjax/ninjax.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 19:50:55.312253 ninjax-1.1.0/ninjax.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9671 2023-05-19 19:50:55.000000 ninjax-1.1.0/ninjax.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      182 2023-05-19 19:50:55.000000 ninjax-1.1.0/ninjax.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-05-19 19:50:55.000000 ninjax-1.1.0/ninjax.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        7 2023-05-19 19:50:55.000000 ninjax-1.1.0/ninjax.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-05-19 19:50:55.316253 ninjax-1.1.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)      585 2022-11-24 15:49:52.000000 ninjax-1.1.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-22 09:42:34.452268 ninjax-1.2.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1071 2022-08-08 16:14:32.000000 ninjax-1.2.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9671 2023-05-22 09:42:34.452268 ninjax-1.2.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9261 2023-02-22 13:32:36.000000 ninjax-1.2.0/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-22 09:42:34.448269 ninjax-1.2.0/ninjax/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      507 2023-05-19 21:26:15.000000 ninjax-1.2.0/ninjax/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    17283 2023-05-22 09:29:01.000000 ninjax-1.2.0/ninjax/ninjax.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-22 09:42:34.452268 ninjax-1.2.0/ninjax.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9671 2023-05-22 09:42:34.000000 ninjax-1.2.0/ninjax.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      211 2023-05-22 09:42:34.000000 ninjax-1.2.0/ninjax.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-05-22 09:42:34.000000 ninjax-1.2.0/ninjax.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        4 2023-05-22 09:42:34.000000 ninjax-1.2.0/ninjax.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        7 2023-05-22 09:42:34.000000 ninjax-1.2.0/ninjax.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-05-22 09:42:34.452268 ninjax-1.2.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      615 2023-05-19 21:32:30.000000 ninjax-1.2.0/setup.py
```

### Comparing `ninjax-1.1.0/LICENSE` & `ninjax-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjax-1.1.0/PKG-INFO` & `ninjax-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjax
-Version: 1.1.0
+Version: 1.2.0
 Summary: General Modules for JAX
 Home-page: http://github.com/danijar/ninjax
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `ninjax-1.1.0/README.md` & `ninjax-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ninjax-1.1.0/ninjax/ninjax.py` & `ninjax-1.2.0/ninjax/ninjax.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import threading
 from functools import partial as bind
 
 import jax
 import jax.numpy as jnp
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
 
 ###############################################################################
 # State
 ###############################################################################
 
 
@@ -80,27 +80,24 @@
     if not isinstance(state, dict):
       raise ValueError('Must provide a dict as state.')
     if context and (not nested):
       raise RuntimeError(
           f'You are trying to call pure {fun.__name__}() inside pure '
           f'{context.name}(). Is that intentional? If you want to nest pure '
           f'functions, use pure(..., nested=True) for the inner function.')
-      # raise RuntimeError(
-      #     f'If you want to nest run() calls, use nested=True. ({context})')
     before = context
     try:
       name = fun.__name__
       context = Context(state.copy(), rng, create, modify, ignore, [], name)
       CONTEXT[threading.get_ident()] = context
       out = fun(*args, **kwargs)
       state = dict(context)
       return out, state
     finally:
       CONTEXT[threading.get_ident()] = before
-  purified.pure = True
   return purified
 
 
 def context():
   """Access and modify the global context from within an impure function. For
   advanced users only. Prefer to use module methods to access and modify state
   and rng() to get the next RNG key."""
@@ -141,16 +138,14 @@
 @jax.named_scope('grad')
 def grad(fun, keys, has_aux=False):
   """Compute the gradient of an impure function with respect to the specified
   state entries or modules. The transformed function returns a tuple containing
   the computed value, selected state entries, their gradients, and if
   applicable auxiliary outputs of the function."""
   keys = keys if hasattr(keys, '__len__') else (keys,)
-  if getattr(fun, 'pure', False):
-    raise ValueError('Use plain jax.grad() for pure functions.')
   if not has_aux:
     fun = lambda *args, _fun=fun, **kwargs: (_fun(*args, *kwargs), {})
   fun = pure(fun, nested=True)
   def forward(x1, x2, rng, *args, **kwargs):
     (y, aux), state = fun({**x1, **x2}, rng, *args, create=False, **kwargs)
     return y, (aux, state)
   backward = jax.value_and_grad(forward, has_aux=True)
@@ -166,104 +161,86 @@
     x2 = {k: v for k, v in context().items() if k not in strs}
     (y, (aux, state)), dx = backward(x1, x2, rng(), *args, **kwargs)
     context().update(state)
     return (y, x1, dx, aux) if has_aux else (y, x1, dx)
   return wrapper
 
 
-def static_support(transform):
-  def new_transform(fun, *args, static=(), **kwargs):
-    assert isinstance(static, (list, tuple)), static
-    cache = {}
-    def new_function(*args2, **kwargs2):
-      sta = {k: v for k, v in kwargs2.items() if k in static}
-      dyn = {k: v for k, v in kwargs2.items() if k not in static}
-      key = hash(tuple(sta.get(n, '_default') for n in static))
-      if key not in cache:
-        specialized = bind(fun, **sta)
-        specialized.__name__ = fun.__name__
-        if hasattr(fun, 'pure'):
-          specialized.pure = fun.pure
-        cache[key] = transform(specialized, *args, **kwargs)
-      return cache[key](*args2, **dyn)
-    return new_function
-  return new_transform
-
-
-@static_support
-def jit(fun, **jitkw):
+def jit(fun, static=(), donate=(), **jit_kwargs):
   """Compiles a pure function for fast execution. Only the first call of the
   function is allowed to create state entries."""
-  if not getattr(fun, 'pure', False):
-    raise ValueError('Use pure() before applying jit().')
+  jit_kwargs['static_argnums'] = [0]
+  jit_kwargs['donate_argnums'] = [1]
 
-  def init(rng, *args, **kwargs):
-    @bind(jax.jit, **jitkw)
-    def jitted(rng, *args, **kwargs):
-      # Return only state so JIT can remove dead code for fast initialization.
-      return fun({}, rng, *args, ignore=True, **kwargs)[1]
-    state = jitted(rng, *args, **kwargs)
-    wrapper.keys = state.keys()
-    return state
-
-  def apply(state, rng, *args, **kwargs):
-    keys = wrapper.keys if hasattr(wrapper, 'keys') else state.keys()
-    selected = {k: v for k, v in state.items() if k in keys}
-    @bind(jax.jit, **jitkw)
-    def jitted(state, rng, *args, **kwargs):
-      return fun(state, rng, *args, create=False, **kwargs)
-    out, updated = jitted(selected, rng, *args, **kwargs)
-    return out, {**state, **updated}
+  @bind(jax.jit, **jit_kwargs)
+  def _init(_static, _donate, *args, **kwargs):
+    _static = dict(_static)
+    _donate = {k: v for k, v in zip(donate, _donate)}
+    return fun({}, *args, ignore=True, **_static, **_donate, **kwargs)[1]
+
+  @bind(jax.jit, **jit_kwargs)
+  def _apply(_static, _donate, *args, **kwargs):
+    _static = dict(_static)
+    _donate = {k: v for k, v in zip(donate, _donate)}
+    return fun(*args, create=False, **_static, **_donate, **kwargs)
 
   @functools.wraps(fun)
-  def wrapper(state, rng, *args, **kwargs):
+  def wrapper(state, *args, init=True, apply=True, **kwargs):
+    _static = tuple((k, kwargs.pop(k)) for k in static if k in kwargs)
+    _donate = tuple(kwargs.pop(k) for k in donate)
     if not hasattr(wrapper, 'keys'):
-      defaults = init(rng, *args, **kwargs)
-      state = {**defaults, **state}
-    return apply(state, rng, *args, **kwargs)
-
-  wrapper.init = init
-  wrapper.apply = apply
+      if init:
+        created = _init(_static, _donate, *args, **kwargs)
+        wrapper.keys = set(created.keys())
+        state = {**created, **state}
+      else:
+        wrapper.keys = set(state.keys())
+    if not apply:
+      return state
+    selected = {k: v for k, v in state.items() if k in wrapper.keys}
+    out, updated = _apply(_static, _donate, selected, *args, **kwargs)
+    return out, {**state, **updated}
   return wrapper
 
 
-@static_support
-def pmap(fun, axis_name=None, **pmapkw):
+def pmap(fun, axis_name=None, static=(), donate=(), **pmap_kwargs):
   """Compiles n pure function for fast execution across multiple devices. Only
   the first call of the function is allowed to create state entries."""
-  if not getattr(fun, 'pure', False):
-    raise ValueError('Use pure() before applying pmap().')
-
-  def init(rng, *args, **kwargs):
-    @bind(jax.pmap, axis_name=axis_name, **pmapkw)
-    def pmapted(rng, *args, **kwargs):
-      # Return only state so pmap can remove dead code for fast initialization.
-      return fun({}, rng, *args, ignore=True, **kwargs)[1]
-    state = pmapted(rng, *args, **kwargs)
-    wrapper.keys = state.keys()
-    return state
-
-  def apply(state, rng, *args, **kwargs):
-    keys = wrapper.keys if hasattr(wrapper, 'keys') else state.keys()
-    selected = {k: v for k, v in state.items() if k in keys}
-    @bind(jax.pmap, axis_name=axis_name, **pmapkw)
-    def pmapted(state, rng, *args, **kwargs):
-      return fun(state, rng, *args, create=False, **kwargs)
-    out, updated = pmapted(selected, rng, *args, **kwargs)
-    return out, {**state, **updated}
+  pmap_kwargs['axis_name'] = axis_name
+  pmap_kwargs['static_broadcasted_argnums'] = [0]
+  pmap_kwargs['donate_argnums'] = [1]
+
+  @bind(jax.pmap, **pmap_kwargs)
+  def _init(_static, _donate, *args, **kwargs):
+    _static = dict(_static)
+    _donate = {k: v for k, v in zip(donate, _donate)}
+    return fun({}, *args, ignore=True, **_static, **_donate, **kwargs)[1]
+
+  @bind(jax.pmap, **pmap_kwargs)
+  def _apply(_static, _donate, *args, **kwargs):
+    _static = dict(_static)
+    _donate = {k: v for k, v in zip(donate, _donate)}
+    return fun(*args, create=False, **_static, **_donate, **kwargs)
 
   @functools.wraps(fun)
-  def wrapper(state, rng, *args, **kwargs):
+  def wrapper(state, *args, init=True, apply=True, **kwargs):
+    _static = tuple((k, kwargs.pop(k)) for k in static if k in kwargs)
+    _donate = tuple(kwargs.pop(k) for k in donate)
     if not hasattr(wrapper, 'keys'):
-      defaults = init(rng, *args, **kwargs)
-      state = {**defaults, **state}
-    return apply(state, rng, *args, **kwargs)
-
-  wrapper.init = init
-  wrapper.apply = apply
+      if init:
+        created = _init(_static, _donate, *args, **kwargs)
+        wrapper.keys = set(created.keys())
+        state = {**created, **state}
+      else:
+        wrapper.keys = set(state.keys())
+    if not apply:
+      return state
+    selected = {k: v for k, v in state.items() if k in wrapper.keys}
+    out, updated = _apply(_static, _donate, selected, *args, **kwargs)
+    return out, {**state, **updated}
   return wrapper
 
 
 @jax.named_scope('cond')
 def cond(pred, true_fun, false_fun, *operands):
   true_fun = pure(true_fun, nested=True)
   false_fun = pure(false_fun, nested=True)
```

### Comparing `ninjax-1.1.0/ninjax.egg-info/PKG-INFO` & `ninjax-1.2.0/ninjax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjax
-Version: 1.1.0
+Version: 1.2.0
 Summary: General Modules for JAX
 Home-page: http://github.com/danijar/ninjax
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `ninjax-1.1.0/setup.py` & `ninjax-1.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     name='ninjax',
     version=ninjax.__version__,
     description='General Modules for JAX',
     url='http://github.com/danijar/ninjax',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     packages=['ninjax'],
+    install_requires=['jax'],
     classifiers=[
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
 )
```

