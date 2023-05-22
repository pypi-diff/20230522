# Comparing `tmp/lk_logger-5.5.2-py3-none-any.whl.zip` & `tmp/lk_logger-5.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 36997 bytes, number of entries: 25
+Zip file size: 37921 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
 -rw-r--r--  2.0 unx      591 b- defN 80-Jan-01 00:00 lk_logger/_print.py
--rw-r--r--  2.0 unx     1672 b- defN 80-Jan-01 00:00 lk_logger/cache.py
+-rw-r--r--  2.0 unx     1815 b- defN 80-Jan-01 00:00 lk_logger/cache.py
 -rw-r--r--  2.0 unx     5487 b- defN 80-Jan-01 00:00 lk_logger/config.py
 -rw-r--r--  2.0 unx     1563 b- defN 80-Jan-01 00:00 lk_logger/console.py
--rw-r--r--  2.0 unx     4503 b- defN 80-Jan-01 00:00 lk_logger/control.py
--rw-r--r--  2.0 unx     6459 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
--rw-r--r--  2.0 unx    13051 b- defN 80-Jan-01 00:00 lk_logger/logger.py
+-rw-r--r--  2.0 unx     4540 b- defN 80-Jan-01 00:00 lk_logger/control.py
+-rw-r--r--  2.0 unx     7360 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
+-rw-r--r--  2.0 unx    13617 b- defN 80-Jan-01 00:00 lk_logger/logger.py
 -rw-r--r--  2.0 unx    10446 b- defN 80-Jan-01 00:00 lk_logger/markup.py
--rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
--rw-r--r--  2.0 unx     9899 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
+-rw-r--r--  2.0 unx     7383 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
+-rw-r--r--  2.0 unx    10793 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
 -rw-r--r--  2.0 unx     4034 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
 -rw-r--r--  2.0 unx     2559 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
 -rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 lk_logger/scanner/__init__.py
 -rw-r--r--  2.0 unx     6247 b- defN 80-Jan-01 00:00 lk_logger/scanner/analyser.py
 -rw-r--r--  2.0 unx     1128 b- defN 80-Jan-01 00:00 lk_logger/scanner/const.py
 -rw-r--r--  2.0 unx     1780 b- defN 80-Jan-01 00:00 lk_logger/scanner/exceptions.py
 -rw-r--r--  2.0 unx     9594 b- defN 80-Jan-01 00:00 lk_logger/scanner/scanner.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 lk_logger/scanner/symbols.py
 -rw-r--r--  2.0 unx    19638 b- defN 80-Jan-01 00:00 lk_logger/scanner/text_scanner.py
 -rw-r--r--  2.0 unx      491 b- defN 80-Jan-01 00:00 lk_logger/scanner/typehint.py
--rw-r--r--  2.0 unx      769 b- defN 80-Jan-01 00:00 lk_logger/shunt.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx     4884 b- defN 80-Jan-01 00:00 lk_logger-5.5.2.dist-info/METADATA
-?rw-r--r--  2.0 unx     1995 b- defN 16-Jan-01 00:00 lk_logger-5.5.2.dist-info/RECORD
-25 files, 117044 bytes uncompressed, 33817 bytes compressed:  71.1%
+-rw-r--r--  2.0 unx      860 b- defN 80-Jan-01 00:00 lk_logger/shunt.py
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4884 b- defN 80-Jan-01 00:00 lk_logger-5.6.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     1996 b- defN 16-Jan-01 00:00 lk_logger-5.6.0.dist-info/RECORD
+25 files, 120795 bytes uncompressed, 34741 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -60,17 +60,17 @@
 
 Filename: lk_logger/scanner/typehint.py
 Comment: 
 
 Filename: lk_logger/shunt.py
 Comment: 
 
-Filename: lk_logger-5.5.2.dist-info/WHEEL
+Filename: lk_logger-5.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: lk_logger-5.5.2.dist-info/METADATA
+Filename: lk_logger-5.6.0.dist-info/METADATA
 Comment: 
 
-Filename: lk_logger-5.5.2.dist-info/RECORD
+Filename: lk_logger-5.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_logger/__init__.py

```diff
@@ -17,8 +17,8 @@
 def __init():
     import traceback
     pipeline.add(traceback, bprint)
     setup(quiet=True)
 
 
 __init()
-__version__ = '5.5.2'
+__version__ = '5.6.0'
```

## lk_logger/cache.py

```diff
@@ -1,28 +1,33 @@
 import typing as t
+
 from .markup import T as T0
+from .message_builder import T as T1
 
 
 class T:  # Typehint
     FrameId = str
+    Info = T1.Info
     MarkupPos = int
     Markup = str
     
-    Cache = t.Dict[FrameId, t.TypedDict('_SubDict0', {
-        'markup_pos'   : MarkupPos,  # noqa
-        'marks_meaning': T0.MarksMeaning,  # noqa
-        'info'         : t.Dict[Markup, dict]
+    # noinspection PyTypedDict
+    Cache = t.Dict[FrameId, t.TypedDict('CacheValue', {
+        'markup_pos'   : MarkupPos,
+        'marks_meaning': T0.MarksMeaning,
+        'info'         : t.Dict[Markup, T1.Info],
     })]
 
 
 class LoggingCache:
     _cache: T.Cache
     
     def __init__(self) -> None:
         from collections import defaultdict
+        # noinspection PyTypeChecker
         self._cache = defaultdict(lambda: {
             'markup_pos'   : None,
             'marks_meaning': {},
             'info'         : {},
         })
     
     def clear_cache(self) -> None:
@@ -35,18 +40,19 @@
     
     def is_cached(self, frame_id: T.FrameId, markup: T.Markup) -> bool:
         return (
                 frame_id in self._cache and
                 markup in self._cache[frame_id]['info']
         )
     
-    def get_cache(self, frame_id: T.FrameId, markup: T.Markup) -> dict:
+    def get_cache(self, frame_id: T.FrameId, markup: T.Markup) -> T.Info:
         # suggest checking `self.is_cached` before calling this method.
         return self._cache[frame_id]['info'][markup]
     
     # -------------------------------------------------------------------------
     
     def record_markup_pos(self, frame_id: T.FrameId, pos: T.MarkupPos) -> None:
         self._cache[frame_id]['markup_pos'] = pos
     
-    def store_info(self, frame_id: T.FrameId, markup: T.Markup, info) -> None:
+    def store_info(self, frame_id: T.FrameId, markup: T.Markup,
+                   info: T.Info) -> None:
         self._cache[frame_id]['info'][markup] = info
```

## lk_logger/control.py

```diff
@@ -1,11 +1,9 @@
-from __future__ import annotations
-
 import builtins
-from typing import Any
+import typing as t
 
 from ._print import bprint
 from ._print import debug  # noqa
 from .logger import lk
 
 STATUS = 'unloaded'  # literal['enabled', 'disabled', 'unloaded']
 _HAS_WELCOME_MESSAGE_SHOWN = False
@@ -52,40 +50,42 @@
         
         # debug(slogan)
         print(slogan, ':rsp')
     
     STATUS = 'enabled'
 
 
-def update(clear_preset=False, **kwargs):
+def update(clear_preset=False, **kwargs) -> None:
     lk.configure(clear_preset, **kwargs)
 
 
-def unload():
+def unload() -> None:
     setattr(builtins, 'print', bprint)
     global STATUS
     STATUS = 'unloaded'
 
 
-def enable():
+def enable() -> None:
     setattr(builtins, 'print', lk.log)
     global STATUS
     STATUS = 'enabled'
 
 
-def disable():
+def disable() -> None:
     setattr(builtins, 'print', lambda *_, **__: None)
     global STATUS
     STATUS = 'disabled'
 
 
 # -----------------------------------------------------------------------------
 # other
 
-def start_ipython(user_ns: dict[str, Any] = None) -> None:
+def start_ipython(
+        user_ns: t.Dict[str, t.Any] = None
+) -> None:
     if _is_ipython_mode():
         return
     try:
         import IPython
     except (ImportError, ModuleNotFoundError) as e:
         print('ipython is not installed!', ':pv4')
         raise e
@@ -104,15 +104,17 @@
         'sys.argv'       : sys.argv.copy(),
     }
     
     setup(quiet=True, clear_preset=True,
           show_source=False, show_funcname=False, show_varnames=False)
     sys.argv = ['']  # avoid ipython to parse `sys.argv`.
     
-    app = TerminalIPythonApp.instance(user_ns=user_ns or {'print': lk.log})
+    app = TerminalIPythonApp.instance(
+        user_ns={'print': lk.log, **(user_ns or {})}
+    )
     app.initialize()
     
     # setup except hook for ipython
     setattr(builtins, 'get_ipython', get_ipython)
     install(console=console)
     
     app.start()
@@ -122,15 +124,15 @@
     sys.argv = backups['sys.argv']
     del backups
 
 
 # -----------------------------------------------------------------------------
 # neutral functions
 
-def _blend_text(message: str, color_pair: tuple[str, str]):
+def _blend_text(message: str, color_pair: t.Tuple[str, str]) -> str:
     """ blend text from one color to another.
     
     source: [lib:rich_cli/__main__.py : blend_text()]
     """
     from rich.color import Color
     from rich.text import Text
```

## lk_logger/frame_info.py

```diff
@@ -1,10 +1,12 @@
 import inspect
 import re
 import typing as t
+from os.path import abspath
+from textwrap import dedent
 from types import FrameType
 
 from .scanner import get_all_blocks
 from .scanner import get_variables
 from .scanner.const import SUBSCRIPTABLE
 from .scanner.const import VARIABLE_NAME
 from .scanner.exceptions import ScanningError
@@ -137,26 +139,47 @@
 
 
 class FrameInfo:
     
     def __init__(self, frame: FrameType):
         self._frame = frame
     
+    def __str__(self) -> str:
+        return self.info
+    
+    @property
+    def info(self) -> str:
+        return dedent(f'''
+            <FrameInfo object>
+                filepath: {self.filepath}
+                lineno: {self.lineno}
+                funcname: {self.funcname}
+        ''').rstrip()
+    
     @property
     def id(self) -> str:
         return f'{self.filepath}:{self.lineno}'
     
     @property
     def filepath(self) -> str:
         """
-        notice: the returned value may be '<string>', '<unknown>' etc.
+        notice:
+            - the returned value may be '<string>', '<unknown>' etc.
+            - (2023-05-22):
+                we do not use `__file__` anymore, because it may cause markup
+                analyser broken when the `__file__` is not real (for example
+                when caller passes `globals()` to `exec` function).
+                see also `examples/start_ipython.py : line 11`.
+            - in python 3.8, `co_filename` may be a relative path, so we need
+                to convert it to absolute.
         """
-        return self._frame.f_globals.get(
-            '__file__', self._frame.f_code.co_filename
-        ).replace('\\', '/')
+        # from ._print import debug
+        # debug(self._frame.f_code.co_filename,
+        #       self._frame.f_globals.get('__file__'))
+        return abspath(self._frame.f_code.co_filename).replace('\\', '/')
     
     @property
     def lineno(self) -> int:
         return self._frame.f_lineno
     
     @property
     def indentation(self) -> int:
```

## lk_logger/logger.py

```diff
@@ -2,68 +2,67 @@
 from atexit import register
 from collections import deque
 from inspect import currentframe
 from threading import Thread
 from time import sleep
 
 from rich.console import RenderableType
-from rich.text import Text
 from rich.traceback import Traceback
 
 from ._print import bprint
 from ._print import debug  # noqa
 from .cache import LoggingCache
 from .config import LoggingConfig
 from .console import con_print
 from .frame_info import FrameInfo
 from .markup import MarkMeaning
 from .markup import MarkupAnalyser
 from .markup import T as T0
-from .message_builder import MessageBuilder
+from .message_builder import MessageStruct
+from .message_builder import T as T1
+from .message_builder import builder as message_builder
 from .path_helper import path_helper
 from .pipeline import pipeline
 from .shunt import Shunt
-from .shunt import T as T1
+from .shunt import T as T2
 
 __all__ = ['LKLogger', 'lk']
 
 
 class _RawArgs:  # a workaround. see its usage below.
     def __init__(self, args: t.Tuple[t.Any, ...]):
         self.args = args
 
 
+class _NoMessage:
+    pass
+
+
 class T:  # Typehint
     Args = t.Tuple[t.Any, ...]
-    Markup = T0.Markup
-    MarkupPos = int  # -1, 0, 1
-    Pipe = T1.Pipe
-    PipeId = T1.PipeId
-    
-    Info = t.TypedDict('Info', {
-        'file_path'      : str,
-        'function_name'  : str,
-        'is_external_lib': bool,
-        'line_number'    : str,
-        'variable_names' : t.Iterable[str],
-    })
-    
-    ComposedMessage = t.Union[str, RenderableType, Traceback, _RawArgs]
+    ComposedMessage = t.Union[
+        RenderableType, T1.MessageStruct, Traceback,
+        t.Type[_NoMessage], _RawArgs
+    ]
     FlushScheme = int
     #   0: no flush
     #   1: instant flush
     #   2: instant flush and drain
     #   3: wait for flush
+    Info = T1.Info
+    Markup = T0.Markup
+    MarkupPos = int  # -1, 0, 1
+    Pipe = T2.Pipe
+    PipeId = T2.PipeId
 
 
 class LKLogger:
     
     def __init__(self):
         self._analyser = MarkupAnalyser()
-        self._builder = MessageBuilder()
         self._cache = LoggingCache()
         self._config = LoggingConfig()
         
         self._shunt = Shunt()
         # self._shunt.add(con_print)
         self.add_pipe = self._shunt.add
         self.remove_pipe = self._shunt.remove
@@ -78,19 +77,16 @@
     def configure(self, clear_preset=False, **kwargs) -> None:
         self._cache.clear_cache()
         if clear_preset:
             self._config.reset()
         if 'show_varname' in kwargs:  # workaround for compatibility
             kwargs['show_varnames'] = kwargs.pop('show_varname')
         self._config.update(**kwargs)
-        self._builder.update_config(
+        message_builder.update_config(
             separator=self._config.separator,
-            show_source=self._config.show_source,
-            show_funcname=self._config.show_funcname,
-            show_varnames=self._config.show_varnames,
         )
     
     @property
     def config(self) -> dict:
         return self._config.to_dict()
     
     def _start_running(self) -> None:
@@ -104,17 +100,16 @@
                 if not self._message_queue: break
                 msg, kwargs, custom_print = self._message_queue.popleft()
                 if custom_print:
                     # debug(custom_print, msg, kwargs)
                     kwargs.pop('file', None)
                     custom_print(*msg, **kwargs)
                 else:
-                    con_print(msg, **kwargs)
-                    if self._shunt:
-                        self._shunt(self._purify(msg))
+                    self._cprint(msg, **kwargs)
+                    self._dprint(msg)
         
         self._running = True
         while self._running:
             if self._message_queue:
                 consume()
             else:
                 sleep(10E-3)
@@ -133,24 +128,26 @@
             self,
             *args: t.Any,
             _frame_info: FrameInfo = None,
             **kwargs
     ) -> None:
         if _frame_info is None:
             _frame_info = FrameInfo(currentframe().f_back)
+            # debug(_frame_info.info)
         
         if (path := _frame_info.filepath) \
                 and (custom_print := pipeline.get(path)):
             if self._config.async_:
                 self._message_queue.append((args, kwargs, custom_print))
             else:
                 custom_print(*args, **kwargs)
             return
         
         msg, flush_scheme = self._build_message(_frame_info, *args)
+        if msg is _NoMessage: return
         is_raw = isinstance(msg, _RawArgs)
         # debug(msg)
         
         self._print(msg, flush_scheme, _is_raw=is_raw, **kwargs)
     
     def _print(
             self,
@@ -163,68 +160,73 @@
             if self._config.async_:
                 if _is_raw:
                     self._message_queue.append((msg.args, kwargs, bprint))
                 else:
                     self._message_queue.append((msg, kwargs, None))
             else:
                 if _is_raw:
-                    bprint(*msg.args, **kwargs)
+                    self._bprint(msg, **kwargs)
                 else:
-                    con_print(msg, **kwargs)
-                    if self._shunt:
-                        self._shunt(self._purify(msg))
+                    self._cprint(msg, **kwargs)
+                    self._dprint(msg)
         elif flush_scheme == 1:
             while self._message_queue:
                 sleep(10E-3)
             if _is_raw:
-                bprint(*msg.args, **kwargs)
+                self._bprint(msg, **kwargs)
             else:
-                con_print(msg, **kwargs)
-                if self._shunt:
-                    self._shunt(self._purify(msg))
+                self._cprint(msg, **kwargs)
+                self._dprint(msg)
         elif flush_scheme == 2:
             if skipped_count := len(self._message_queue):
                 self._message_queue.clear()
-                print(':frp', f'[red dim](... skipped '
-                              f'{skipped_count} messages)[/]')
+                print(':frp2', f'[red dim](... skipped '
+                               f'{skipped_count} messages)[/]')
             if _is_raw:
-                bprint(*msg.args, **kwargs)
+                self._bprint(msg, **kwargs)
             else:
-                con_print(msg, **kwargs)
-                if self._shunt:
-                    self._shunt(self._purify(msg))
+                self._cprint(msg, **kwargs)
+                self._dprint(msg)
         elif flush_scheme == 3:
             if _is_raw:
-                bprint(*msg.args, **kwargs)
+                self._bprint(msg, **kwargs)
             else:
-                con_print(msg, **kwargs)
-                if self._shunt:
-                    self._shunt(self._purify(msg))
+                self._cprint(msg, **kwargs)
+                self._dprint(msg)
+        else:
+            raise ValueError(flush_scheme)
+    
+    @staticmethod
+    def _bprint(msg: _RawArgs, **kwargs) -> None:
+        bprint(*msg.args, **kwargs)
     
     @staticmethod
-    def _purify(msg: T.ComposedMessage) -> t.Optional[str]:
-        if isinstance(msg, str):
-            text = Text.from_markup(msg)
-            return text.plain
-        return None
+    def _cprint(msg: T.ComposedMessage, **kwargs) -> None:
+        if isinstance(msg, MessageStruct):
+            con_print(msg.text, **kwargs)
+        else:
+            con_print(msg, **kwargs)
+    
+    def _dprint(self, msg: T.ComposedMessage) -> None:
+        if self._shunt:
+            if isinstance(msg, MessageStruct):
+                for caller in self._shunt:
+                    caller(msg.body.plain)
     
+    # FIXME
     def fmt(self, _frame_info: FrameInfo = None, *args, **_) -> str:
         return str(self._build_message(
             _frame_info or FrameInfo(currentframe().f_back), *args
         )[0])
     
+    # -------------------------------------------------------------------------
+    
     def _build_message(
             self, frame_info: FrameInfo, *args
     ) -> t.Tuple[T.ComposedMessage, T.FlushScheme]:
-        """
-        return: (str message, bool is_flush, bool is_drain)
-            flush: print the message immediately.
-            drain: drain the message queue.
-                if drain is True, the flush must be True.
-        """
         args, markup_pos, markup = \
             self._extract_markup_from_arguments(frame_info.id, args)
         marks = self._analyser.extract(markup)
         
         get_varnames = frame_info.collect_varnames  # backup method pointer
         if marks['p']: frame_info = frame_info.get_parent(marks['p'])
         marks_meaning = self._analyser.analyse(marks, frame_info=frame_info)
@@ -237,46 +239,64 @@
             flush_scheme = 2
         elif MarkMeaning.FLUSH_EDDY in marks_meaning:
             flush_scheme = 3
         
         # check cache
         if self._cache.is_cached(frame_info.id, markup):
             cached_info = self._cache.get_cache(frame_info.id, markup)
-            return self._builder.compose(
-                args, marks_meaning, cached_info
+            return message_builder.compose(
+                args, marks_meaning, cached_info,
+                self._config.show_source,
+                self._config.show_funcname,
+                self._config.show_varnames,
             ), flush_scheme
         
         # ---------------------------------------------------------------------
         
-        if MarkMeaning.AGRESSIVE_PRUNE in marks_meaning:
-            return self._builder.quick_compose(args), flush_scheme
-        elif MarkMeaning.BUILTIN_PRINT in marks_meaning:
+        if not args:
+            if MarkMeaning.MODERATE_PRUNE in marks_meaning or \
+                    MarkMeaning.AGRESSIVE_PRUNE in marks_meaning:
+                return _NoMessage, flush_scheme
+        if MarkMeaning.BUILTIN_PRINT in marks_meaning:
             return _RawArgs(args), flush_scheme
         elif MarkMeaning.RICH_OBJECT in marks_meaning:
             assert len(args) == 1 and isinstance(args[0], RenderableType)
             return args[0], flush_scheme
         elif MarkMeaning.TRACEBACK_EXCEPTION in marks_meaning:
             assert len(args) == 1 and isinstance(args[0], BaseException)
-            return self._builder.compose_exception(args[0], False), flush_scheme
+            return message_builder.compose_exception(
+                args[0], show_locals=False
+            ), flush_scheme
         elif MarkMeaning.TRACEBACK_EXCEPTION_WITH_LOCALS in marks_meaning:
             assert len(args) == 1 and isinstance(args[0], BaseException)
-            return self._builder.compose_exception(args[0], True), flush_scheme
+            return message_builder.compose_exception(
+                args[0], show_locals=True
+            ), flush_scheme
         
         info: T.Info = {
             'file_path'      : '',
             'line_number'    : '0',
             'is_external_lib': False,
             'function_name'  : '',
             'variable_names' : (),
         }
         
-        show_source = self._config.show_source
-        show_funcname = self._config.show_funcname
-        show_varnames = self._config.show_varnames and \
-                        MarkMeaning.MODERATE_PRUNE not in marks_meaning
+        show_source = (
+                self._config.show_source and
+                (MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning)
+        )
+        show_funcname = (
+                self._config.show_funcname and
+                (MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning)
+        )
+        show_varnames = (
+                self._config.show_varnames and
+                MarkMeaning.MODERATE_PRUNE not in marks_meaning and
+                MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
+        )
         
         if any((show_source, show_funcname, show_varnames)):
             if show_source:
                 def update_sourcemap():
                     """
                     this function updates follows:
                         info['is_external_lib']
@@ -312,16 +332,19 @@
                 elif markup_pos == 1:
                     info['variable_names'] = varnames[1:]
                 else:
                     info['variable_names'] = varnames[:-1]
         
         self._cache.store_info(frame_info.id, markup, info)
         
-        return self._builder.compose(
-            args, marks_meaning, info
+        return message_builder.compose(
+            args, marks_meaning, info,
+            show_source=show_source,
+            show_funcname=show_funcname,
+            show_varnames=show_varnames,
         ), flush_scheme
     
     def _extract_markup_from_arguments(
             self, frame_id: str, args: T.Args
     ) -> t.Tuple[T.Args, T.MarkupPos, T.Markup]:
         """
         return: (args, markup_pos, markup)
```

## lk_logger/message_builder.py

```diff
@@ -1,178 +1,220 @@
-from __future__ import annotations
-
 import typing as t
 
+from rich.text import Text
 from rich.traceback import Traceback
 
 from .markup import MarkMeaning
-from .message_formatter import MessageFormatter
+from .markup import T as T0
+from .message_formatter import formatter
+
+
+class MessageStruct:
+    head: t.Optional[Text]
+    body: Text
+    
+    def __init__(self, head: t.Optional[Text], body: Text):
+        self.head = head if (head and len(head)) else None
+        self.body = body
+    
+    @property
+    def text(self) -> Text:
+        if self.head:
+            return Text.assemble(self.head, self.body)
+        else:
+            return self.body
 
 
 class T:
-    from .markup import T as _TMarkup  # noqa
     Args = t.Tuple[t.Any, ...]
-    Markup = _TMarkup.Markup
-    MarksMeaning = _TMarkup.MarksMeaning
+    Markup = T0.Markup
+    MarksMeaning = T0.MarksMeaning
+    MessageStruct = MessageStruct
+    RichText = Text
+    
+    Info = t.TypedDict('Info', {
+        'file_path'      : str,
+        'function_name'  : str,
+        'is_external_lib': bool,
+        'line_number'    : str,
+        'variable_names' : t.Tuple[str, ...],
+    })
 
 
 class MessageBuilder:
+    _separator_a: Text
+    _separator_b: Text
     
-    def __init__(self, **kwargs):
-        self._formatter = MessageFormatter()
+    def __init__(self, **kwargs) -> None:
         self.update_config(**kwargs)
     
-    # noinspection PyAttributeOutsideInit
-    def update_config(self, **config):
-        self._separator = config.get('separator', ';   ')
-        self._show_source = config.get('show_source', False)
-        self._show_funcname = config.get('show_funcname', False)
-        self._show_varnames = config.get('show_varnames', False)
+    def update_config(self, **config) -> None:
+        # https://fsymbols.com/signs/arrow/
+        self._separator_a = Text(' ➤ ', 'bright_black')
+        #   alternatives: ➤ ⪢ >> ⮕ -> ~> | │
+        self._separator_b = Text(
+            config.get('separator', ';   '), 'bright_black')
     
     # -------------------------------------------------------------------------
     
-    def quick_compose(self, args: T.Args) -> str:
-        return (
-            '[bright_black]{separator}[/]'.format(
-                separator=self._separator
-            ).join(map(str, args))
-        )
-    
     def compose(
             self,
             args: T.Args,
             marks_meaning: T.MarksMeaning,
-            info: dict
-    ) -> str:
-        if MarkMeaning.AGRESSIVE_PRUNE in marks_meaning:
-            return self.quick_compose(args)
-        
-        message_elements = []
+            info: T.Info,
+            show_source: bool = True,
+            show_funcname: bool = True,
+            show_varnames: bool = False,
+    ) -> T.MessageStruct:
+        show_source = show_source and \
+                      MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
+        show_funcname = show_funcname and \
+                        MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
+        show_varnames = show_varnames and \
+                        MarkMeaning.MODERATE_PRUNE not in marks_meaning and \
+                        MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
+        
+        head = Text()
+        body = Text()
+        # body_parts: t.List[T.RichText] = [Text(), None, Text()]
+        # body = body_parts[0]
         
         # 1. source
-        if self._show_source:
-            message_elements.append(
-                self._formatter.fmt_source(
+        if show_source:
+            head.append_text(
+                formatter.fmt_source(
                     info['file_path'],
                     info['line_number'],
                     is_external_lib=info['is_external_lib'],
                     fmt_width=True,
                 )
             )
-            message_elements.append(
-                self._formatter.fmt_separator('  >>  ')
-            )
+            head.append_text(self._separator_a)
         
         # 2. funcname
-        if self._show_funcname:
+        if show_funcname:
             assert info['function_name']
-            message_elements.append(
-                self._formatter.fmt_funcname(
+            head.append_text(
+                formatter.fmt_funcname(
                     info['function_name'],
                     fmt_width=True,
                 )
             )
-            message_elements.append(
-                self._formatter.fmt_separator('  >>  ')
-            )
+            head.append_text(self._separator_a)
+        
+        # if not self._show_source and not self._show_funcname:
+        #     head = None
+        # if len(head) == 0:
+        #     head = None
+        
+        # ---------------------------------------------------------------------
         
         # 3. verbosity
         if MarkMeaning.VERBOSITY in marks_meaning:
             if MarkMeaning.MODERATE_PRUNE not in marks_meaning:
-                message_elements.append(
-                    self._formatter.fmt_level(
+                if x := formatter.fmt_level(
                         marks_meaning[MarkMeaning.VERBOSITY],
-                    )
-                )
-                message_elements.append(' ')
+                ):
+                    body.append_text(x)
+                    body.append(' ')
         
         # 4. index
         if MarkMeaning.RESET_INDEX in marks_meaning:
             if MarkMeaning.MODERATE_PRUNE in marks_meaning:
                 pass
             else:
-                message_elements.append(self._formatter.fmt_index(0))
-                message_elements.append(' ')
+                body.append_text(formatter.fmt_index(0))
+                body.append(' ')
                 if not args:
                     args = ('[grey50]reset index[/]',)
         elif MarkMeaning.SIMPLE_COUNTER in marks_meaning:
-            message_elements.append(
-                self._formatter.fmt_index(
+            body.append_text(
+                formatter.fmt_index(
                     marks_meaning[MarkMeaning.SIMPLE_COUNTER]
                 )
             )
-            message_elements.append(' ')
+            body.append(' ')
         elif MarkMeaning.SCOPED_COUNTER in marks_meaning:
-            message_elements.append(
-                self._formatter.fmt_scoped_index(
+            body.append_text(
+                formatter.fmt_scoped_index(
                     *marks_meaning[MarkMeaning.SCOPED_COUNTER]
                 )
             )
-            message_elements.append(' ')
+            body.append(' ')
         
         # 5. timestamp
         if MarkMeaning.RESET_TIMER in marks_meaning:
             if not args:
                 args = ('[grey50]reset timer: [/] {}'.format(
-                    self._formatter.fmt_time(
+                    formatter.fmt_time(
                         marks_meaning[MarkMeaning.RESET_TIMER],
                         color_s='green dim'
                     )
                 ),)
             else:
-                args = (self._formatter.fmt_time(
+                args = (formatter.fmt_time(
                     marks_meaning[MarkMeaning.RESET_TIMER],
                     color_s='green dim'
                 ), *args)
         elif MarkMeaning.START_TIMER in marks_meaning:
             args = ('[cyan]start timer:[/] {}'.format(
-                self._formatter.fmt_time(
+                formatter.fmt_time(
                     marks_meaning[MarkMeaning.RESET_TIMER]
                 )
             ), *args)
         elif MarkMeaning.STOP_TIMER in marks_meaning:
             s, e = marks_meaning[MarkMeaning.STOP_TIMER]
-            args = (self._formatter.fmt_time(s, e), *args)
+            args = (formatter.fmt_time(s, e), *args)
         
         # # 6. divider
         # if MarkMeaning.DIVIDER_LINE in marks_meaning:
         #     pattern = marks_meaning[MarkMeaning.DIVIDER_LINE]
         #     message_elements.append(
-        #         self._formatter.fmt_divider(pattern)
+        #         formatter.fmt_divider(pattern)
         #     )
         #     message_elements.append(' ')
         
         # 7. arguments
-        message_elements.append(
-            self._formatter.fmt_message(
-                arguments=args,
-                varnames=info['variable_names'] if self._show_varnames else (),
-                rich=MarkMeaning.RICH_FORMAT in marks_meaning,
-                expand=MarkMeaning.EXPAND_MULTIPLE_LINES in marks_meaning,
-                separator=self._separator,
-            )
+        # body.append_text(
+        #     formatter.fmt_message(
+        #         arguments=args,
+        #         varnames=info['variable_names'] if self._show_varnames else (),
+        #         rich=MarkMeaning.RICH_FORMAT in marks_meaning,
+        #         expand=MarkMeaning.EXPAND_MULTIPLE_LINES in marks_meaning,
+        #         separator=self._separator_b,
+        #         overall_style=marks_meaning.get(MarkMeaning.VERBOSITY, None),
+        #     )
+        # )
+        temp = formatter.fmt_message(
+            arguments=args,
+            varnames=info['variable_names'] if show_varnames else (),
+            rich=MarkMeaning.RICH_FORMAT in marks_meaning,
+            expand=MarkMeaning.EXPAND_MULTIPLE_LINES in marks_meaning,
+            separator=self._separator_b,
+            overall_style=marks_meaning.get(MarkMeaning.VERBOSITY, None),
         )
-        if MarkMeaning.VERBOSITY in marks_meaning and \
-                MarkMeaning.EXPAND_MULTIPLE_LINES not in marks_meaning:
-            message_elements[-1] = self._formatter.fmt_level(
-                marks_meaning[MarkMeaning.VERBOSITY],
-                text=message_elements[-1]
-            )
         
-        # PERF: this is not a good design.
-        # 6. divider
+        # PERF: this is compromised design.
+        # 8. divider
         if MarkMeaning.DIVIDER_LINE in marks_meaning:
-            message_elements.insert(len(message_elements) - 1, ' ')
             pattern = marks_meaning[MarkMeaning.DIVIDER_LINE]
-            divider = self._formatter.fmt_divider(
-                pattern, context=message_elements
+            divider = formatter.fmt_divider(
+                pattern, context=(head, body, temp)
             )
-            message_elements.insert(len(message_elements) - 2, divider)
+            body.append_text(divider)
+            body.append(' ')
+            body.append_text(temp)
+        else:
+            body.append_text(temp)
+        del temp
         
-        return ''.join(message_elements)
+        return MessageStruct(head, body)
     
+    @staticmethod
     def compose_exception(
-            self,
             e: BaseException,
             show_locals: bool
     ) -> Traceback:
-        return self._formatter.fmt_exception(e, show_locals)
+        return formatter.fmt_exception(e, show_locals)
+
+
+builder = MessageBuilder()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## lk_logger/message_formatter.py

```diff
@@ -1,24 +1,36 @@
-from __future__ import annotations
-
 import typing as t
+from dataclasses import dataclass
+from functools import partial
 from math import ceil
 from textwrap import indent
 from time import localtime
 from time import strftime as _strftime
 from traceback import format_exception
 
+# from rich.padding import Padding
 from rich.pretty import pretty_repr
+from rich.text import Text
 from rich.traceback import Traceback
 
 from ._print import debug  # noqa
 from .console import console
 
-strftime = lambda t: _strftime('%H:%M:%S', localtime(t)) \
-    if t is not None else ''
+strftime = lambda t: (t and _strftime('%H:%M:%S', localtime(t))) or ''
+
+
+@dataclass
+class MarkupText:
+    text: str
+    mark: str = None
+
+
+class T:
+    Level = t.Literal['trace', 'debug', 'info', 'warning', 'error', 'fatal']
+    RichText = Text
 
 
 class Color:  # TODO: not used yet (and not ready).
     SEPARATOR = 'bright_black'
     
     # time
     TIME_START = 'green'
@@ -34,51 +46,37 @@
     V_ERROR = 'red'
     V_FATAL = 'bold #ffffff on red'
 
 
 class MessageFormatter:
     
     @staticmethod
-    def markup(*markups: tuple[str, str]) -> str:
-        """
-        this method produces the final strings that could be directly printed.
-
-        args:
-            markups: tuple[tuple[str text, str mark], ...]
-                mark:
-                    any valid patterns of pytermgui markups. for example, 'red',
-                    'bold', 'dim', '#00FF00', ...
-                    ps: mark allows empty.
-        """
-        out = []
-        for text, mark in markups:
-            if mark:
-                out.append('[{}]{}[/]'.format(mark, text))
-            else:
-                out.append(text)
-        return ''.join(out)
+    def markup(*markups: t.Tuple[str, str]) -> T.RichText:
+        # text = Text()
+        # for t, m in markups:
+        #     text.append(t, m)
+        # return text
+        return Text.assemble(*markups)
     
     # -------------------------------------------------------------------------
     
     def fmt_divider(
-            self, pattern: str = '-', length: int = None,
-            context: list[str] = None
-    ) -> str:  # PERF: not a good design.
+            self,
+            pattern: str = '-',
+            length: int = None,
+            context: t.Tuple[T.RichText, ...] = None,
+    ) -> T.RichText:
         if length is None:
             if context:
-                measure = console.measure(''.join(context))
-                # length = console.width - measure.maximum
-                length = min((console.width, 200)) - measure.maximum
-                # if length > 80:
-                #     length = 80
+                length = min((console.width, 200)) - sum(map(len, context))
+                # if length > 80: length = 80
                 if length <= 0:
                     if len(context) > 1 and context[-1]:
                         # strip the last element and try again
-                        measure = console.measure(''.join(context[:-1]))
-                        length = console.width - measure.maximum
+                        length = console.width - sum(map(len, context[:-1]))
                         if length > 0:
                             # return self.markup((
                             #     pattern * length + '\n' + pattern * 3,
                             #     'yellow'
                             # ))
                             return self.markup(
                                 (pattern * length, 'yellow'),
@@ -98,127 +96,157 @@
     def fmt_exception(e: BaseException, show_locals=False) -> Traceback:
         trace = Traceback.from_exception(
             type(e), e, e.__traceback__,
             show_locals=show_locals
         )
         return trace
     
-    def fmt_funcname(self, funcname: str, fmt_width=False) -> str:
+    def fmt_funcname(self, funcname: str, fmt_width=False) -> T.RichText:
         is_func = not funcname.startswith('<')
         if is_func:
             funcname += '()'
         else:
             funcname = funcname[1:-1]
         if fmt_width:
             funcname = self._fmt_width(
-                funcname, min_width=8, unit_spaces=4
+                funcname, min_width=8, step_space=4
             )
-        if is_func:
-            return self.markup((funcname, 'green'))
-        else:
-            return self.markup((funcname, 'magenta'))
+        return Text(funcname, 'green' if is_func else 'magenta')
     
-    def fmt_index(self, idx: int) -> str:
-        return self.markup(
-            (f'[{idx}]', 'grey50' if idx == 0 else 'red')
-        )
+    @staticmethod
+    def fmt_index(idx: int) -> T.RichText:
+        return Text(f'[{idx}]', 'grey50' if idx == 0 else 'red')
     
-    def fmt_level(self, level: str, text='') -> str:
-        if level == 'trace':
-            return ''
-        labels = {
-            'trace': '',
-            'debug': '[DEBUG]',
-            'info' : '[ INFO]',
-            'warn' : '[ WARN]',
-            'error': '[ERROR]',
-            'fatal': '[FATAL]',
-        }
-        colors = {
-            'trace': '',
-            'debug': 'grey50',
-            'info' : 'blue',
-            'warn' : 'yellow',
-            'error': 'red',
-            'fatal': 'bold #ffffff on red',
-        }
-        if not text: text = labels[level]
-        return self.markup((text, colors[level]))
+    _level_2_color = {
+        'trace': '',
+        'debug': 'grey50',
+        'info' : 'blue',
+        'warn' : 'yellow',
+        'error': 'red',
+        'fatal': 'bold #ffffff on red',
+    }
+    _level_2_label = {
+        'trace': '',
+        'debug': '[DEBUG]',
+        'info' : '[ INFO]',
+        'warn' : '[ WARN]',
+        'error': '[ERROR]',
+        'fatal': '[FATAL]',
+    }
+    
+    def fmt_level(self, level: T.Level) -> t.Optional[T.RichText]:
+        if level == 'trace': return None
+        label = self._level_2_label[level]
+        color = self._level_2_color[level]
+        return Text(label, color)
     
     def fmt_message(
-            self, arguments: t.Iterable[t.Any], varnames: tuple[str],
-            rich: bool, expand=False, separator=';   '
-    ) -> str:
+            self,
+            arguments: t.Iterable[t.Any],
+            varnames: t.Tuple[str, ...],
+            rich: bool,
+            expand: bool = False,
+            separator: T.RichText = None,
+            overall_style: T.Level = None,
+    ) -> T.RichText:
         """
         notice the process sequence:
             1. expand
             2. varnames
             3. rich
         """
         if expand:
-            arguments = tuple(map(self._expand_object, arguments))
+            # arguments = tuple(map(self._expand_object, arguments))
+            arguments = map(self._expand_object, arguments)
         if varnames:
-            arguments = self._mix_arguments_with_varnames(arguments, varnames)
+            arguments = self._mix_arguments_with_varnames(
+                tuple(arguments), varnames
+            )
         else:
             arguments = map(str, arguments)
         if not rich:
             arguments = (x.replace('[', '\\[') for x in arguments)
         
+        # ---------------------------------------------------------------------
+        
+        if overall_style:
+            parse_text = partial(
+                Text.from_markup,
+                style=self._level_2_color[overall_style]
+            )
+        else:
+            # parse_text = Text.from_markup
+            parse_text = partial(
+                Text.from_markup,
+                style='default'
+            )
+        
         if expand:
-            return '\n' + indent('\n'.join(arguments), '    ')
+            _indent = partial(indent, prefix='    ')
+            text = Text.assemble(
+                Text('\n'),
+                Text('\n').join(
+                    map(parse_text, map(_indent, arguments))
+                )
+            )
         else:
-            return self.markup((separator, 'bright_black')).join(arguments)
+            # text = Text(separator, 'bright_black').join(
+            #     map(Text.from_markup, arguments)
+            # )
+            assert separator
+            text = separator.join(
+                map(parse_text, arguments)
+            )
+        
+        return text
     
-    def fmt_scoped_index(self, idx: int, uid: str, color: str = '') -> str:
-        # return self.markup(
-        #     ('\\[', 'magenta'),
-        #     (f'{idx}', 'magenta'),
-        #     (f'/{uid}', 'magenta dim'),
-        #     (']', 'magenta'),
-        # )
+    def fmt_scoped_index(
+            self,
+            idx: int,
+            uid: str,
+            color: str = ''
+    ) -> T.RichText:
         return self.markup(
-            (f'\\[{uid}]', f'{color} dim'),
-            (f'\\[{idx}]', f'{color}'),
+            (f'[{uid}]', f'{color} dim'),
+            (f'[{idx}]', f'{color}'),
         )
     
-    def fmt_separator(self, sep: str = ' >> ', color='bright_black') -> str:
+    def fmt_separator(
+            self,
+            sep: str = ' >> ',
+            color='bright_black'
+    ) -> T.RichText:
         return self.markup((sep, color))
     
     def fmt_source(
             self, filepath: str, lineno: t.Union[int, str],
             is_external_lib: bool = False, fmt_width=False
-    ) -> str:
-        if fmt_width:
-            text_a = f'{filepath}:{lineno}'
-            text_b = self._fmt_width(text_a, min_width=12)
-            additional_space = ' ' * (len(text_b) - len(text_a))
-        else:
-            additional_space = ''
+    ) -> T.RichText:
+        text = Text()
+        
         if is_external_lib:
             assert filepath.startswith('[')
             a, b = filepath[1:].split(']', 1)
-            filepath = self.markup(
-                ('\\[{}]'.format(a),
-                 'bold {}'.format('red' if filepath.startswith('[unknown]')
-                                  else 'magenta')),
-                (f'{b}', 'bold blue'),
-            )
-            return self.markup(
-                (filepath, ''),
-                (':', 'bright_black'),
-                (str(lineno), 'bold blue'),
-                (additional_space, ''),
-            )
+            text.append(f'[{a}]', 'bold {}'.format(
+                'red' if filepath.startswith('[unknown]') else 'magenta'
+            ))
+            text.append(b, 'bold blue')
         else:
-            return self.markup(
-                (filepath.replace('[', '\\['), 'bold blue'),
-                (':', 'bright_black'),
-                (str(lineno), 'bold blue'),
-                (additional_space, ''),
-            )
+            text.append(filepath, 'bold blue')
+        
+        text.append(':', 'bright_black')
+        text.append(str(lineno), 'bold blue')
+        
+        if fmt_width:
+            text_a = f'{filepath}:{lineno}'
+            text_b = self._fmt_width(text_a, min_width=12)
+            additional_space = ' ' * (len(text_b) - len(text_a))
+            text.append(additional_space)
+        
+        return text
     
     @staticmethod
     def fmt_time(start: float, end: float = None, color_s='green') -> str:
         if end is None:
             return '[{}]\\[{}][/]'.format(color_s, strftime(start))
         
         diff = end - start  # float >= 0
@@ -264,32 +292,54 @@
         )
     
     # -------------------------------------------------------------------------
     
     @staticmethod
     def _expand_object(obj: t.Any) -> str:
         if isinstance(obj, Exception):
-            return '\n' + indent(''.join(format_exception(obj)), '│ ')
+            return '\n' + indent(
+                ''.join(format_exception(obj)), '│ '
+            )
         else:
             return pretty_repr(obj)
     
     @staticmethod
     def _mix_arguments_with_varnames(
-            arguments: t.Sequence[str], varnames: tuple[str, ...],
+            arguments: t.Sequence[str],
+            varnames: t.Tuple[str, ...],
     ) -> t.Iterable[str]:
         if not arguments:
             return ()
         try:
             assert len(varnames) == len(arguments), (varnames, arguments)
         except AssertionError:
             # debug('failed extracting varnames')
             return map(str, arguments)
         else:
             return (f'{v} = {a}' if v else str(a)
                     for v, a in zip(varnames, arguments))
     
+    # @staticmethod
+    # def _mix_arguments_with_varnames(
+    #         arguments: t.Sequence[str],
+    #         varnames: t.Tuple[str, ...],
+    # ) -> t.Iterator[t.Tuple[str, t.Any]]:
+    #     if not arguments:
+    #         return
+    #     try:
+    #         assert len(varnames) == len(arguments), (varnames, arguments)
+    #     except AssertionError:
+    #         # debug('failed extracting varnames')
+    #         for arg in arguments:
+    #             yield '', arg
+    #     else:
+    #         yield from zip(varnames, arguments)
+    
     @staticmethod
-    def _fmt_width(text: str, min_width: int = None, unit_spaces=4) -> str:
+    def _fmt_width(text: str, min_width: int = None, step_space=4) -> str:
         if len(text) <= min_width:
             return text.ljust(min_width)
         else:
-            return text.ljust(ceil(len(text) / unit_spaces) * unit_spaces)
+            return text.ljust(ceil(len(text) / step_space) * step_space)
+
+
+formatter = MessageFormatter()
```

## lk_logger/shunt.py

```diff
@@ -17,14 +17,17 @@
     def __bool__(self):
         return bool(self._pipes)
         
     def __call__(self, msg: t.Union[str, t.Any], **kwargs) -> None:
         for p in self._pipes.values():
             p(msg, **kwargs)
     
+    def __iter__(self) -> t.Iterator[T.Pipe]:
+        yield from self._pipes.values()
+    
     def add(self, pipe: T.Pipe, name: str = '') -> T.PipeId:
         self._pipes[(id := name or self._random_id())] = pipe
         return id
     
     def remove(self, id: T.PipeId) -> None:
         self._pipes.pop(id)
```

## Comparing `lk_logger-5.5.2.dist-info/METADATA` & `lk_logger-5.6.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lk-logger
-Version: 5.5.2
+Version: 5.6.0
 Summary: Python advanced print with varnames.
 Home-page: https://github.com/likianta/lk-logger
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `lk_logger-5.5.2.dist-info/RECORD` & `lk_logger-5.6.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-lk_logger/__init__.py,sha256=QurUBVXay6P0mgoM5M1tvAT_4KcB8yAKvJktKevHJds,592
+lk_logger/__init__.py,sha256=PDvdrJlKEL6SPrj_2Xyww6DTCcWX27aaPBGzsdV8O2w,592
 lk_logger/_print.py,sha256=Q0WdJ-TxOcQy1aKxEgaxaCrixq9GdXqQVF7YTw-jELo,591
-lk_logger/cache.py,sha256=ayisqijEVWmUatnNqrooM8urR0hIAzYkzcJTUt_8248,1672
+lk_logger/cache.py,sha256=83bH8DTfZszNt5X59nLQcvYG07h23J83HB4FpQ7UoOY,1815
 lk_logger/config.py,sha256=mmM6x2vlR5setLz_5dhWKHzwL4tvY-oESsNDl5FOLr4,5487
 lk_logger/console.py,sha256=GSoFWXBybfNuF7S7b3_OJL70h52OSlTPnCbpay1pL60,1563
-lk_logger/control.py,sha256=Fk8o5aGjTAAxhJs6G1EvTUZ3ERvlQ13H-cpX_Mn5CSQ,4503
-lk_logger/frame_info.py,sha256=tkraucs-K_hCvtp9IB8dvLkuZ8wG8kAQt0swz8b2mZQ,6459
-lk_logger/logger.py,sha256=NvF5IYj1Yq5lR8WPTMoxkZFhC75Ai5NK-sNX4Mp3xL0,13051
+lk_logger/control.py,sha256=wEGJzOOb4KE2dMVBnpC-IHRDCaMBCx7N3Tii8NUd8qU,4540
+lk_logger/frame_info.py,sha256=PzuZL0DkCmly8z061ZyeAMdgEY9cfurL4WhlBGa4cB0,7360
+lk_logger/logger.py,sha256=w1sPcYrzdcuxIkvpJ78gUnJLE4HgvuZ4cgjMlKK2Cv0,13617
 lk_logger/markup.py,sha256=FIDjNJ-q-Fb3T2FDCjhMDwyUrkH1mdY5_nFE1bSze20,10446
-lk_logger/message_builder.py,sha256=Jj6YEmEbwjaiIXndS32vMToXBAfgHKXw3wDGdoqCCgI,6265
-lk_logger/message_formatter.py,sha256=lIdEoMdKDOfdduTq9wfKvL5Q7el9GQRMQeX4p63wu0k,9899
+lk_logger/message_builder.py,sha256=TvhZayAp5a2wDULiW84_Lg4zXg98h-aFSI9Xz0FmrLA,7383
+lk_logger/message_formatter.py,sha256=ZStrTjNUh0owDYnz-6jjzz347mC3jsLIklMFNqvkNhI,10793
 lk_logger/path_helper.py,sha256=LAZOe5XK_51I0YPA6rUuY0_DKtaMtHyz52xcHqRbxY0,4034
 lk_logger/pipeline.py,sha256=bo-Z9367i2TxxJOCS5_Rk_6CFccFyJYgp3-uw9q9LzQ,2559
 lk_logger/scanner/__init__.py,sha256=er6nQAKVaYpdk30878kEDo5vKTSa6CzR-CdxNJiaODo,71
 lk_logger/scanner/analyser.py,sha256=tbI48nDcBPthZoD8jlnpap7S6FIHs4u8pUMQpsmh6r4,6247
 lk_logger/scanner/const.py,sha256=pRfHUK2huF2oLkd-ZpGtGUKQ2T4K3EnlSI0pUGGnp6Q,1128
 lk_logger/scanner/exceptions.py,sha256=G1wpgEIzTLLrD6Q_m0qGD85v5KnlPm3CV1ZxgvGCVd8,1780
 lk_logger/scanner/scanner.py,sha256=7Ase1WyHD87cBr4k9zYehe9LgL91r0L1_XlgKHg1_Eg,9594
 lk_logger/scanner/symbols.py,sha256=ibW1-n7Xigo9LvowUSn6dIrx-UmiJyuxN321bSCilSg,3238
 lk_logger/scanner/text_scanner.py,sha256=84ese30Bh-H1ZVxT0jcNhsTwM1nLDkZOrUO1LSdjV6k,19638
 lk_logger/scanner/typehint.py,sha256=Vr929B1w9UGiLVEMIJJIyE6gULjd_NxmNVpssyZW_JI,491
-lk_logger/shunt.py,sha256=X3wqfprKLsmSUgZifte0Ao9CB7MDh2A45IqC1Gt8f2Y,769
-lk_logger-5.5.2.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-lk_logger-5.5.2.dist-info/METADATA,sha256=g9Hl7zTksuqHijr3O6tXnfpFY2WH_NGgJEcWmlhlJgU,4884
-lk_logger-5.5.2.dist-info/RECORD,,
+lk_logger/shunt.py,sha256=-2uc2STfSIABrY-yAC7qIBh3uBgEx0iL1CGB_9rcwzg,860
+lk_logger-5.6.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+lk_logger-5.6.0.dist-info/METADATA,sha256=qx90GAC-In2d5a4QaG0LVwiBgjJ9EPs0HE0WpIUPMrs,4884
+lk_logger-5.6.0.dist-info/RECORD,,
```

