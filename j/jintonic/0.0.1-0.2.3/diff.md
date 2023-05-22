# Comparing `tmp/jintonic-0.0.1.tar.gz` & `tmp/jintonic-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jintonic-0.0.1.tar", last modified: Fri Nov 16 20:15:42 2018, max compression
+gzip compressed data, was "jintonic-0.2.3.tar", last modified: Mon May 22 17:34:01 2023, max compression
```

## Comparing `jintonic-0.0.1.tar` & `jintonic-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 daedalus  (1000) daedalus  (1000)        0 2018-11-16 20:15:42.000000 jintonic-0.0.1/
-drwxr-xr-x   0 daedalus  (1000) daedalus  (1000)        0 2018-11-16 20:15:42.000000 jintonic-0.0.1/jintonic.egg-info/
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      288 2018-11-16 20:15:42.000000 jintonic-0.0.1/jintonic.egg-info/SOURCES.txt
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1373 2018-11-16 20:15:42.000000 jintonic-0.0.1/jintonic.egg-info/PKG-INFO
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)        1 2018-11-16 20:15:42.000000 jintonic-0.0.1/jintonic.egg-info/dependency_links.txt
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)        9 2018-11-16 20:15:42.000000 jintonic-0.0.1/jintonic.egg-info/top_level.txt
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1373 2018-11-16 20:15:42.000000 jintonic-0.0.1/PKG-INFO
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)       38 2018-11-16 20:15:42.000000 jintonic-0.0.1/setup.cfg
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      772 2018-11-16 20:13:43.000000 jintonic-0.0.1/README.md
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      639 2018-11-16 20:12:36.000000 jintonic-0.0.1/setup.py
-drwxr-xr-x   0 daedalus  (1000) daedalus  (1000)        0 2018-11-16 20:15:42.000000 jintonic-0.0.1/jintonic/
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)        0 2018-11-02 13:47:23.000000 jintonic-0.0.1/jintonic/__init__.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)    16752 2018-11-12 01:36:48.000000 jintonic-0.0.1/jintonic/scales.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1630 2018-11-09 01:58:09.000000 jintonic-0.0.1/jintonic/primes.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     9187 2018-11-12 01:36:48.000000 jintonic-0.0.1/jintonic/chords.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)    14095 2018-11-08 22:28:05.000000 jintonic-0.0.1/jintonic/intervals.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     7105 2018-11-08 22:31:07.000000 jintonic-0.0.1/jintonic/lattice.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     2898 2018-11-09 01:56:06.000000 jintonic-0.0.1/jintonic/harmonics.py
+drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-05-22 17:34:01.597189 jintonic-0.2.3/
+-rw-r--r--   0 daedalus   (501) staff       (20)     1068 2023-05-21 09:38:33.000000 jintonic-0.2.3/LICENSE
+-rw-r--r--   0 daedalus   (501) staff       (20)     1036 2023-05-22 17:34:01.597051 jintonic-0.2.3/PKG-INFO
+-rw-r--r--   0 daedalus   (501) staff       (20)      659 2023-05-21 19:08:21.000000 jintonic-0.2.3/README.md
+-rw-r--r--   0 daedalus   (501) staff       (20)      848 2023-05-22 17:33:51.000000 jintonic-0.2.3/pyproject.toml
+-rw-r--r--   0 daedalus   (501) staff       (20)        0 2023-05-21 09:39:10.000000 jintonic-0.2.3/requirements.txt
+-rw-r--r--   0 daedalus   (501) staff       (20)       38 2023-05-22 17:34:01.597226 jintonic-0.2.3/setup.cfg
+drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-05-22 17:34:01.594329 jintonic-0.2.3/src/
+drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-05-22 17:34:01.595709 jintonic-0.2.3/src/jintonic/
+-rw-r--r--   0 daedalus   (501) staff       (20)      243 2023-05-21 09:39:35.000000 jintonic-0.2.3/src/jintonic/__init__.py
+-rw-r--r--   0 daedalus   (501) staff       (20)       35 2023-05-21 09:39:35.000000 jintonic-0.2.3/src/jintonic/__main__.py
+-rw-r--r--   0 daedalus   (501) staff       (20)     9898 2023-05-22 17:26:57.000000 jintonic-0.2.3/src/jintonic/chords.py
+-rw-r--r--   0 daedalus   (501) staff       (20)     2876 2023-05-22 17:16:30.000000 jintonic-0.2.3/src/jintonic/harmonics.py
+-rw-r--r--   0 daedalus   (501) staff       (20)    14037 2023-05-22 17:16:30.000000 jintonic-0.2.3/src/jintonic/intervals.py
+-rw-r--r--   0 daedalus   (501) staff       (20)     7899 2023-05-22 17:16:30.000000 jintonic-0.2.3/src/jintonic/lattice.py
+-rw-r--r--   0 daedalus   (501) staff       (20)     1773 2023-05-22 17:16:30.000000 jintonic-0.2.3/src/jintonic/primes.py
+-rw-r--r--   0 daedalus   (501) staff       (20)    15260 2023-05-22 17:32:07.000000 jintonic-0.2.3/src/jintonic/scales.py
+drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-05-22 17:34:01.596851 jintonic-0.2.3/src/jintonic.egg-info/
+-rw-r--r--   0 daedalus   (501) staff       (20)     1036 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/PKG-INFO
+-rw-r--r--   0 daedalus   (501) staff       (20)      427 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/SOURCES.txt
+-rw-r--r--   0 daedalus   (501) staff       (20)        1 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/dependency_links.txt
+-rw-r--r--   0 daedalus   (501) staff       (20)       52 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/entry_points.txt
+-rw-r--r--   0 daedalus   (501) staff       (20)        9 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jintonic-0.0.1/jintonic.egg-info/PKG-INFO` & `jintonic-0.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: jintonic
-Version: 0.0.1
-Summary: Just Intonation with Python
-Home-page: https://github.com/inegm/jintonic
+Version: 0.2.3
+Summary: Utilities for computer assisted composition in just intonation
 Author: Ismail Negm
-Author-email: ismailnegm@protonmail.com
-License: MIT License
-Description: # jintonic #
-        
-        A package of tools for composition in just intonation with Python.
-        
-        Full documentation is available [here](https://jintonic.readthedocs.io/en/latest/).
-        
-        David B. Doty's technical definition of just intonation :
-        
-          *Just Intonation is any system of tuning in which all of the intervals can
-          be represented by whole-number frequency ratios, with a strongly implied
-          preference for the simplest ratios compatible with a given musical purpose.*
-        
-        You can find a more lyrical definition in the first chapter of his primer,
-        which is available online [here](http://www.dbdoty.com/Words/Primer_2.1.html)
-        
-        I strongly recommend his book : "The Just Intonation Primer". It is listed in
-        the references below.
-        
-        **References**
-        
-        - http://www.dbdoty.com/Words/Primer1.html
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# jintonic
+
+A package of tools for composition in just intonation with Python.
+
+David B. Doty's technical definition of just intonation :
+
+_Just Intonation is any system of tuning in which all of the intervals can be
+represented by whole-number frequency ratios, with a strongly implied preference
+for the simplest ratios compatible with a given musical purpose._
+
+You can find a more lyrical definition in the first chapter of his primer, which
+is [available online](http://www.dbdoty.com/Words/Primer_2.1.html).
+
+I strongly recommend his book :
+[Just Intonation Primer](http://www.dbdoty.com/Words/Primer1.html).
+
+## Installing
+
+```
+pip install jintonic
+```
```

### Comparing `jintonic-0.0.1/PKG-INFO` & `jintonic-0.2.3/src/jintonic.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: jintonic
-Version: 0.0.1
-Summary: Just Intonation with Python
-Home-page: https://github.com/inegm/jintonic
+Version: 0.2.3
+Summary: Utilities for computer assisted composition in just intonation
 Author: Ismail Negm
-Author-email: ismailnegm@protonmail.com
-License: MIT License
-Description: # jintonic #
-        
-        A package of tools for composition in just intonation with Python.
-        
-        Full documentation is available [here](https://jintonic.readthedocs.io/en/latest/).
-        
-        David B. Doty's technical definition of just intonation :
-        
-          *Just Intonation is any system of tuning in which all of the intervals can
-          be represented by whole-number frequency ratios, with a strongly implied
-          preference for the simplest ratios compatible with a given musical purpose.*
-        
-        You can find a more lyrical definition in the first chapter of his primer,
-        which is available online [here](http://www.dbdoty.com/Words/Primer_2.1.html)
-        
-        I strongly recommend his book : "The Just Intonation Primer". It is listed in
-        the references below.
-        
-        **References**
-        
-        - http://www.dbdoty.com/Words/Primer1.html
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# jintonic
+
+A package of tools for composition in just intonation with Python.
+
+David B. Doty's technical definition of just intonation :
+
+_Just Intonation is any system of tuning in which all of the intervals can be
+represented by whole-number frequency ratios, with a strongly implied preference
+for the simplest ratios compatible with a given musical purpose._
+
+You can find a more lyrical definition in the first chapter of his primer, which
+is [available online](http://www.dbdoty.com/Words/Primer_2.1.html).
+
+I strongly recommend his book :
+[Just Intonation Primer](http://www.dbdoty.com/Words/Primer1.html).
+
+## Installing
+
+```
+pip install jintonic
+```
```

### Comparing `jintonic-0.0.1/jintonic/scales.py` & `jintonic-0.2.3/src/jintonic/scales.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,535 +1,466 @@
 """Implements just intonation arbitrary and tetrachordal scales."""
+from __future__ import annotations
 
 from itertools import permutations, product
+from typing import List, Optional, Tuple, Union
 
 from .intervals import JustInterval
 from .primes import is_prime
 
 
-__version__ = '0.0.1'
-
-
-class JustScale():
+class JustScale:
     """This class implements arbitrary just intonation scales."""
 
-    def __init__(self, tones=None):
+    def __init__(self, tones: List[JustInterval]):
         """Initializes a JustScale.
 
-        :param tones: A list of intervals or an object containing
-            a list of intervals (that implements the attribute intervals)
-        :type tones: list
-
-        **Examples**
-
-        >>> scale = JustScale([JustInterval(1, 1)])
-        >>> scale.append(JustInterval(3, 2))
-        >>> scale.append(JustInterval(2, 1))
-        >>> scale
-        JustScale([1/1, 3/2, 2/1])
+        Parameters:
+            tones: A list of intervals or an object containing a list of
+                intervals (that implements the attribute intervals)
+
+        Examples:
+            >>> scale = JustScale([JustInterval(1, 1)])
+            >>> scale.append(JustInterval(3, 2))
+            >>> scale.append(JustInterval(2, 1))
+            >>> scale
+            JustScale([1/1, 3/2, 2/1])
         """
-        self._tones = None
-        self._pitch_mapping = None
-
-        try:
-            self.tones = tones.intervals
-        except AttributeError:
-            self.tones = tones
+        self._tones = tones
 
-    def append(self, other):
+    def append(self, tone: JustInterval):
         """Appends tones to the scale.
 
-        :param other: A new tone
-        :type other: JustInterval
+        Parameters:
+            tone: A new tone
 
-        **Examples**
-
-        >>> scale = JustScale([JustInterval(3, 2)])
-        >>> scale.append(JustInterval(4, 3))
-        >>> scale.tones
-        [JustInterval(4, 3), JustInterval(3, 2)]
+        Examples:
+            >>> scale = JustScale([JustInterval(3, 2)])
+            >>> scale.append(JustInterval(4, 3))
+            >>> scale.tones
+            [JustInterval(4, 3), JustInterval(3, 2)]
         """
-        if not isinstance(other, JustInterval):
-            msg = 'cannot append type {}. '.format(type(other))
+        if not isinstance(tone, JustInterval):
+            msg = "cannot append type {}. ".format(type(tone))
             msg += 'Expecting type "JustInterval"'
             raise ValueError(msg)
-        self._tones.append(other)
+        self._tones.append(tone)
 
-    def hertz(self, fundamental):
+    def hertz(self, fundamental: float) -> List[float]:
         """Translates scale intervals to pitches in Hertz over a fundamental
 
-        .. note::
-
+        Note:
             Here, the fundamental is always 1/1 and is not to be mistaken with
             the first tone of the scale. If 1/1 is not part of the scale's
             tones, the fundamental will not be part of the scale.
 
-        :param fundamental: The scale's 0 degree (fundamental) pitch in Hertz.
-        :type fundamental: float
+        Parameters:
+            fundamental: The scale's 0 degree (fundamental) pitch in Hertz.
+
+        Returns:
+            Scale pitches as Hertz
         """
         return [fundamental * tone for tone in self.tones]
 
     @property
-    def tones(self):
+    def tones(self) -> List[JustInterval]:
         """JustScale tones.
 
-        :param values: A list of tones
-        :type values: list of JustInterval
+        Returns:
+            Scale tones
         """
         return sorted(self._tones)
 
     @tones.setter
-    def tones(self, values):
-        """Sets JustScale tones."""
+    def tones(self, values: List[JustInterval]):
+        """Sets JustScale tones.
+
+        Parameters:
+            values: A list of tones
+        """
         for tone in values:
             if not isinstance(tone, JustInterval):
-                msg = 'tones must be a list of JustIntervals. '
+                msg = "tones must be a list of JustIntervals. "
                 msg += "Got '{}'".format(values)
                 raise ValueError(msg)
         self._tones = values
 
     @property
-    def intervals(self):
+    def intervals(self) -> List[JustInterval]:
         """JustScale intervals.
 
-        **Examples**
+        Returns:
+            Scale intervals
 
-        >>> scale = JustScale([JustInterval(1, 1)])
-        >>> scale.append(JustInterval(3, 2))
-        >>> scale.append(JustInterval(2, 1))
-        >>> scale.intervals
-        [JustInterval(3, 2), JustInterval(4, 3)]
+        Examples:
+            >>> scale = JustScale([JustInterval(1, 1)])
+            >>> scale.append(JustInterval(3, 2))
+            >>> scale.append(JustInterval(2, 1))
+            >>> scale.intervals
+            [JustInterval(3, 2), JustInterval(4, 3)]
         """
-        return [
-            tone - self.tones[i-1]
-            for i, tone in enumerate(self.tones)
-        ][1:]
+        return [tone - self.tones[i - 1] for i, tone in enumerate(self.tones)][1:]
 
     @property
-    def complement(self):
+    def complement(self) -> JustScale:
         """JustScale complement
 
-        :rtype: JustScale
+        Returns:
+            The complement scale
 
-        **Examples**
-
-        >>> scale = JustScale([JustInterval(1, 1)])
-        >>> scale.append(JustInterval(3, 2))
-        >>> scale.append(JustInterval(2, 1))
-        >>> scale.complement
-        JustScale([1/1, 4/3, 2/1])
+        Examples:
+            >>> scale = JustScale([JustInterval(1, 1)])
+            >>> scale.append(JustInterval(3, 2))
+            >>> scale.append(JustInterval(2, 1))
+            >>> scale.complement
+            JustScale([1/1, 4/3, 2/1])
         """
         tones = [tone.complement for tone in self.tones]
         return JustScale(tones)
 
     @property
-    def prime_limit(self):
-        """JustScale prime limit
-
-        :rtype: int
-        """
+    def prime_limit(self) -> int:
+        """JustScale prime limit"""
         return max([tone.prime_limit for tone in self.tones])
 
-    @property
-    def pitch_mapping(self):
-        """Mapping of pitches to notation strings.
-
-        :param values: A list, equal in length to the scale's list of
-            intervals, containing lilypond string representations of the notes
-            to be used in notation for each pitch.
-        :type values: list of str
-        """
-        # TODO Default pitch mapper
-        # Create a default pitch mapper. For example: if there are 8 pitches,
-        # use the diatonic C representations. If 12, then use chromatic with
-        # the lilpypond default for twelve-tone (all sharps ?). Otherwise,
-        # keep the fifth and "perfect" intervals, then use accidentals. Etc.
-        return self.pitch_mapping
-
-    @pitch_mapping.setter
-    def pitch_mapping(self, values):
-        """Set a scale's pitch mapping."""
-        if len(values) != self.tones:
-            msg = 'length mismatch. Must map one to one with intervals.'
-            raise ValueError(msg)
-        for value in values:
-            if not isinstance(value, str):
-                # TODO Validate lilypond note values
-                raise ValueError('invalid mapping.')
-
     def __repr__(self):
         """repr(self)"""
-        pitches = ', '.join([
-            '/'.join([str(tone.numerator), str(tone.denominator)])
-            for tone in self.tones
-        ])
+        pitches = ", ".join(
+            [
+                "/".join([str(tone.numerator), str(tone.denominator)])
+                for tone in self.tones
+            ]
+        )
         return "{}([{}])".format(self.__class__.__name__, pitches)
 
 
-class JustTetrachord():
+class JustTetrachord:
     """This class implements disjunct just intonation tetrachords."""
 
-    def __init__(self, intervals=None, genus=None, prime_limit=7):
+    def __init__(
+        self,
+        intervals: Optional[List[JustInterval]] = None,
+        genus: Optional[str] = None,
+        prime_limit: int = 7,
+    ):
         """Initializes a JustTetrachord.
 
         A JustTetrachord can be constructed in one of two ways :
 
             - from a genus name (with naive division)
             - from a list of intervals between each successive tone
 
-        :param intervals: A list of intervals
-        :type intervals: :class:`justintonation.intervals.JustInterval`
-        :param genus: One of 'enharmonic', 'chromatic', or 'diatonic'
-        :type genus: str
-        :param prime_limit: The prime limit to respect
-        :type prime_limit: int
-
-        **Examples**
-
-        >>> JustTetrachord(genus='chromatic')
-        JustTetrachord('chromatic' [27:28, 14:15, 5:6])
-
-        >>> JustTetrachord(genus='enharmonic')
-        JustTetrachord('enharmonic' [45:46, 23:24, 4:5])
-        >>> JustTetrachord(genus='enharmonic').prime_limit
-        23
-
-        >>> intervals = []
-        >>> intervals.append(JustInterval(32, 31))
-        >>> intervals.append(JustInterval(31, 30))
-        >>> intervals.append(JustInterval(5, 4))
-        >>> JustTetrachord(intervals)
-        JustTetrachord('enharmonic' [31:32, 30:31, 4:5])
-        >>> JustTetrachord(intervals).prime_limit
-        31
+        Parameters:
+            intervals: A list of intervals
+            genus: One of 'enharmonic', 'chromatic', or 'diatonic'
+            prime_limit: The prime limit to respect
+
+        Examples:
+            >>> JustTetrachord(genus='chromatic')
+            JustTetrachord('chromatic' [27:28, 14:15, 5:6])
+
+            >>> JustTetrachord(genus='enharmonic')
+            JustTetrachord('enharmonic' [45:46, 23:24, 4:5])
+            >>> JustTetrachord(genus='enharmonic').prime_limit
+            23
+
+            >>> intervals = []
+            >>> intervals.append(JustInterval(32, 31))
+            >>> intervals.append(JustInterval(31, 30))
+            >>> intervals.append(JustInterval(5, 4))
+            >>> JustTetrachord(intervals)
+            JustTetrachord('enharmonic' [31:32, 30:31, 4:5])
+            >>> JustTetrachord(intervals).prime_limit
+            31
         """
         if not is_prime(prime_limit):
-            msg = 'The prime limit must be a prime number. '
+            msg = "The prime limit must be a prime number. "
             msg += "Got: '{}'".format(prime_limit)
             raise ValueError(msg)
         self._prime_limit = prime_limit
 
         if intervals is not None:
             self.intervals = intervals
         elif genus is not None:
             self.genus = genus.strip().lower()
         else:
-            self._intervals = []
+            self._intervals: List[JustInterval] = []
 
     @classmethod
-    def validate_tetrachord(cls, value):
-        """Validates a tetrachord."""
-        if len(value) != 3:
-            msg = 'Tetrachords must be formed of exactly three intervals. '
-            msg += 'Got: "{}"'.format(value)
+    def validate_tetrachord(cls, tetrachord: Union[JustTetrachord, List[JustInterval]]):
+        """Validates a tetrachord.
+
+        Parameters:
+            tetrachord: The tetrachord to validate
+
+        Raises:
+            ValueError: If the given tetrachord is invalid
+        """
+        if len(tetrachord) != 3:
+            msg = "Tetrachords must be formed of exactly three intervals. "
+            msg += 'Got: "{}"'.format(tetrachord)
             raise ValueError(msg)
-        try:
-            total_interval = sum(value)
-        except TypeError:
-            total_interval = sum(value.intervals)
+        # TODO implement __add__ and __radd__ to avoid needing these sum loops
+        total_interval = JustInterval(1, 1)
+        if isinstance(tetrachord, JustTetrachord):
+            for interval in tetrachord.intervals:
+                total_interval += interval
+        else:
+            for interval in tetrachord:
+                total_interval += interval
         if total_interval != JustInterval(4, 3):
-            msg = 'Tetrachord intervals must sum to JustInterval(4, 3). '
-            msg += 'Got: "{}"'.format(sum(value))
+            msg = "Tetrachord intervals must sum to JustInterval(4, 3). "
+            msg += 'Got: "{}"'.format(total_interval)
             raise ValueError(msg)
 
     @property
-    def intervals(self):
+    def intervals(self) -> List[JustInterval]:
         """JustTetrachord intervals.
+        Returns:
+            The tetrachord's intervals
 
-        :param value: A list of exactly three intervals which sum to 4:3
-        :type value: list of JustInterval
-
-        **Examples**
-
-        >>> JustTetrachord(genus='enharmonic').intervals
-        [JustInterval(46, 45), JustInterval(24, 23), JustInterval(5, 4)]
+        Examples:
+            >>> JustTetrachord(genus='enharmonic').intervals
+            [JustInterval(46, 45), JustInterval(24, 23), JustInterval(5, 4)]
         """
         return self._intervals
 
     @intervals.setter
     def intervals(self, values):
-        """Set JustTetrachord intervals."""
+        """Set JustTetrachord intervals.
+
+        Parameters:
+            value: A list of exactly three intervals which sum to 4:3
+        """
         self.validate_tetrachord(values)
         self._prime_limit = max(
-            values[0].prime_limit,
-            values[1].prime_limit,
-            values[2].prime_limit
+            values[0].prime_limit, values[1].prime_limit, values[2].prime_limit
         )
         self._intervals = values
 
     @property
-    def genus(self):
-        """JustTetrachord genus.
+    def genus(self) -> str:
+        """JustTetrachord genus."""
+        if not self.intervals:
+            raise ValueError("Undefined intervals")
+        end_intervals = [JustInterval(5, 4), JustInterval(6, 5), JustInterval(10, 9)]
+        genera = ["enharmonic", "chromatic", "diatonic"]
+        try:
+            return genera[end_intervals.index(self.intervals[-1])]
+        except ValueError:
+            return "non-classical"
 
-        .. note::
+    @genus.setter
+    def genus(self, value: str):
+        """Set JustTetrachord genus.
 
+        Note:
             When setting the genus, the movable tone is set to its most basic
             position by dividing by two the interval remaining after taking the
             characteristic interval.
 
-        :param value: A valid classical genus from ['enharmonic', 'chromatic',
-            'diatonic']
-        :type value: str
+        Parameters:
+            value: A valid classical genus from ['enharmonic', 'chromatic', 'diatonic']
         """
-        if not self.intervals:
-            raise ValueError('Undefined intervals')
-        end_intervals = [
-            JustInterval(5, 4),
-            JustInterval(6, 5),
-            JustInterval(10, 9)
-        ]
-        genera = ['enharmonic', 'chromatic', 'diatonic']
-        try:
-            return genera[end_intervals.index(self.intervals[-1])]
-        except ValueError:
-            return 'non-classical'
-
-    @genus.setter
-    def genus(self, value):
-        """Set JustTetrachord genus."""
         characteristic_intervals = {
-            'enharmonic': JustInterval(5, 4),
-            'chromatic': JustInterval(6, 5),
-            'diatonic': JustInterval(10, 9)
+            "enharmonic": JustInterval(5, 4),
+            "chromatic": JustInterval(6, 5),
+            "diatonic": JustInterval(10, 9),
         }
         characteristic = characteristic_intervals[value]
         remainder = JustInterval(4, 3) - characteristic
         intervals = remainder.divisions(2, self.prime_limit)
         intervals.append(characteristic)
         self.intervals = intervals
 
     @property
-    def prime_limit(self):
+    def prime_limit(self) -> int:
         """JustTetrachord prime limit."""
         return self._prime_limit
 
     @property
-    def permutations(self):
+    def permutations(self) -> List[JustTetrachord]:
         """All (there are six) possible permutations of the JustTetrachord.
 
-        :rtype: list of JustTetrachord
+        Returns:
+            The permutations of the JustTetrachord
         """
         return [
-            JustTetrachord(intervals=permutation)
+            JustTetrachord(intervals=list(permutation))
             for permutation in permutations(self.intervals)
         ]
 
     def __repr__(self):
         """repr(self)"""
         return "{}('{}' [{}:{}, {}:{}, {}:{}])".format(
             self.__class__.__name__,
             self.genus,
             self.intervals[0].denominator,
             self.intervals[0].numerator,
             self.intervals[1].denominator,
             self.intervals[1].numerator,
             self.intervals[2].denominator,
-            self.intervals[2].numerator
+            self.intervals[2].numerator,
         )
 
     def __eq__(self, other):
         """self == other"""
         return self.intervals == other.intervals
 
     def __len__(self):
         """len(self)"""
         return len(self.intervals)
 
 
-class JustTetrachordalScale():
+class JustTetrachordalScale:
     """This class implements disjunct just intonation tetrachordal scales."""
 
-    def __init__(self, lower, upper=None):
+    def __init__(
+        self,
+        lower: JustTetrachord,
+        upper: Optional[JustTetrachord] = None,
+    ):
         """Initializes a JustTetrachordalScale.
 
-        :param lower: The lower tetrachord
-        :type lower: JustTetrachord
-        :param upper: The upper tetrachord. If None is passed, the lower
-            tetrachord is also used for the upper, creating an 'equal'
-            tetrachordal scale.
-        :type upper: JustTetrachord
-
-        **Examples**
+        Parameters:
+            lower: The lower tetrachord
+            upper: The upper tetrachord. If None is passed, the lower tetrachord
+                is also used for the upper, creating an 'equal' tetrachordal scale.
 
-        >>> JustTetrachordalScale(JustTetrachord(genus='enharmonic'))
-         JustTetrachordalScale([46/45, 24/23, 5/4, 9/8, 46/45, 24/23, 5/4])
+        Examples:
+            >>> JustTetrachordalScale(JustTetrachord(genus='enharmonic'))
+            JustTetrachordalScale([46/45, 24/23, 5/4, 9/8, 46/45, 24/23, 5/4])
         """
-        self._lower = None
-        self._upper = None
 
-        self.lower = lower
+        self._lower = lower
         if upper is None:
-            self.upper = lower
+            self._upper = lower
         else:
-            self.upper = upper
+            self._upper = upper
 
     @property
-    def lower(self):
-        """Lower JustTetrachord.
-
-        :param value: JustTetrachord
-        """
+    def lower(self) -> JustTetrachord:
+        """Lower JustTetrachord."""
         return self._lower
 
     @lower.setter
-    def lower(self, value):
+    def lower(self, value: JustTetrachord):
         """Set lower JustTetrachord."""
         JustTetrachord.validate_tetrachord(value)
         self._lower = value
 
     @property
-    def upper(self):
-        """Upper JustTetrachord.
-
-        :param value: JustTetrachord
-        """
+    def upper(self) -> JustTetrachord:
+        """Upper JustTetrachord."""
         return self._upper
 
     @upper.setter
-    def upper(self, value):
+    def upper(self, value: JustTetrachord):
         """Set upper JustTetrachord."""
         JustTetrachord.validate_tetrachord(value)
         self._upper = value
 
     @property
-    def intervals(self):
+    def intervals(self) -> List[JustInterval]:
         """JustTetrachordalScale intervals.
 
-        **Examples**
-
-        >>> JustTetrachordalScale(JustTetrachord(genus='diatonic')).intervals
-        [JustInterval(16, 15), JustInterval(9, 8), JustInterval(10, 9),
-        JustInterval(9, 8), JustInterval(16, 15), JustInterval(9, 8),
-        JustInterval(10, 9)]
-        """
-        return (
-            self.lower.intervals +
-            [JustInterval(9, 8)] +
-            self.upper.intervals
-        )
+        Examples:
+            >>> JustTetrachordalScale(JustTetrachord(genus='diatonic')).intervals
+            [JustInterval(16, 15), JustInterval(9, 8), JustInterval(10, 9),
+            JustInterval(9, 8), JustInterval(16, 15), JustInterval(9, 8),
+            JustInterval(10, 9)]
+        """
+        return self.lower.intervals + [JustInterval(9, 8)] + self.upper.intervals
 
     @property
-    def complement(self):
+    def complement(self) -> JustScale:
         """JustTetrachordalScale complement
 
-        :rtype: JustScale
-
-        .. note::
+        Note:
+            Returns a JustScale! The result will not be Tetrachordal.
 
-            Returns a JustScale ! The result will not be Tetrachordal.
+        Returns:
+            The JustScale that is the complement
 
-        **Examples**
-
-        >>> JustTetrachordalScale(JustTetrachord(genus='chromatic')).complement
-        JustScale([1/1, 6/5, 9/7, 4/3, 3/2, 9/5, 27/14, 2/1])
+        Examples:
+            >>> JustTetrachordalScale(JustTetrachord(genus='chromatic')).complement
+            JustScale([1/1, 6/5, 9/7, 4/3, 3/2, 9/5, 27/14, 2/1])
         """
         tones = [tone.complement for tone in self.tones]
         return JustScale(tones)
 
     @property
-    def tones(self):
+    def tones(self) -> List[JustInterval]:
         """JustTetrachordalScale tones.
 
-        >>> JustTetrachordalScale(JustTetrachord(genus='diatonic')).tones
-        [JustInterval(1, 1), JustInterval(16, 15), JustInterval(6, 5),
-        JustInterval(4, 3), JustInterval(3, 2), JustInterval(8, 5),
-        JustInterval(9, 5), JustInterval(2, 1)]
+        Examples:
+            >>> JustTetrachordalScale(JustTetrachord(genus='diatonic')).tones
+            [JustInterval(1, 1), JustInterval(16, 15), JustInterval(6, 5),
+            JustInterval(4, 3), JustInterval(3, 2), JustInterval(8, 5),
+            JustInterval(9, 5), JustInterval(2, 1)]
         """
         tones = [JustInterval(1, 1)]
         tones += [
-            JustInterval(1, 1) + sum(self.intervals[:i])
-            for i in range(1, len(self.intervals))]
+            sum(self.intervals[:i], start=JustInterval(1, 1))
+            for i in range(1, len(self.intervals))
+        ]
         tones += [JustInterval(2, 1)]
         return tones
 
-    def hertz(self, fundamental):
+    def hertz(self, fundamental: float) -> List[float]:
         """Translates scale intervals to pitches in Hertz over a fundamental
 
-        :param fundamental: The scale's 0 degree (fundamental) pitch in Hertz.
-        :type fundamental: float
+        Parameters:
+            fundamental: The scale's 0 degree (fundamental) pitch in Hertz.
 
-        :rtype: list of float
+        Returns:
+            The scale's pitches as Hertz
 
-        **Examples**
-
-        >>> JustTetrachordalScale(JustTetrachord(genus='diatonic')).hertz(60.)
-        [60.0, 64.0, 72.0, 80.0, 90.0, 96.0, 108.0, 120.0]
+        Examples:
+            >>> JustTetrachordalScale(JustTetrachord(genus='diatonic')).hertz(60.)
+            [60.0, 64.0, 72.0, 80.0, 90.0, 96.0, 108.0, 120.0]
         """
         return [fundamental * tone for tone in self.tones]
 
     @property
-    def genera(self):
+    def genera(self) -> Tuple[str, ...]:
         """JustTetrachordalScale genera for each constituent tetrachord.
 
-        :rtype: tuple
-
-        **Examples**
-
-        >>> intervals = []
-        >>> intervals.append(JustInterval(32, 31))
-        >>> intervals.append(JustInterval(31, 30))
-        >>> intervals.append(JustInterval(5, 4))
-        >>> scale = JustTetrachordalScale(JustTetrachord(intervals))
-        >>> scale.upper = JustTetrachord(genus='diatonic')
-        >>> scale.genera
-        ('enharmonic', 'diatonic')
+        Examples:
+            >>> intervals = []
+            >>> intervals.append(JustInterval(32, 31))
+            >>> intervals.append(JustInterval(31, 30))
+            >>> intervals.append(JustInterval(5, 4))
+            >>> scale = JustTetrachordalScale(JustTetrachord(intervals))
+            >>> scale.upper = JustTetrachord(genus='diatonic')
+            >>> scale.genera
+            ('enharmonic', 'diatonic')
         """
         return (self.lower.genus, self.upper.genus)
 
     @property
-    def is_equal(self):
+    def is_equal(self) -> bool:
         """Evaluates whether the JustTetrachordalScale is equal or mixed."""
         return self.lower == self.upper
 
     @property
-    def prime_limit(self):
+    def prime_limit(self) -> int:
         """JustTetrachordalScale prime limit."""
         return max(self.lower.prime_limit, self.upper.prime_limit)
 
     @property
-    def permutations(self):
-        """All (thirty-six) possible permutations of the JustTetrachordalScale.
-
-        :rtype: list of JustTetrachordalScale
-        """
+    def permutations(self) -> List[JustTetrachordalScale]:
+        """All (thirty-six) possible permutations of the JustTetrachordalScale."""
         return [
             JustTetrachordalScale(pair[0], pair[1])
-            for pair in product(
-                self.lower.permutations,
-                self.upper.permutations
-            )
+            for pair in product(self.lower.permutations, self.upper.permutations)
         ]
 
-    @property
-    def pitch_mapping(self):
-        """Mapping of pitches to notation strings.
-
-        :param values: A list, equal in length to the scale's list of
-            intervals, containing lilypond string representations of the notes
-            to be used in notation for each pitch.
-        :type values: list of str
-        """
-        # TODO Default pitch mapper
-        # Create a default pitch mapper. For example: if there are 8 pitches,
-        # use the diatonic C representations. If 12, then use chromatic with
-        # the lilpypond default for twelve-tone (all sharps ?). Otherwise,
-        # keep the fifth and "perfect" intervals, then use accidentals. Etc.
-        return self.pitch_mapping
-
-    @pitch_mapping.setter
-    def pitch_mapping(self, values):
-        """Set a scale's pitch mapping."""
-        if len(values) != self.tones:
-            msg = 'length mismatch. Must map one to one with intervals.'
-            raise ValueError(msg)
-        for value in values:
-            if not isinstance(value, str):
-                # TODO Validate lilypond note values
-                raise ValueError('invalid mapping.')
-
     def __repr__(self):
         """repr(self)"""
-        pitches = ', '.join([
-            '/'.join([str(interval.numerator), str(interval.denominator)])
-            for interval in self.intervals
-        ])
+        pitches = ", ".join(
+            [
+                "/".join([str(interval.numerator), str(interval.denominator)])
+                for interval in self.intervals
+            ]
+        )
         return "{}([{}])".format(self.__class__.__name__, pitches)
```

### Comparing `jintonic-0.0.1/jintonic/primes.py` & `jintonic-0.2.3/src/jintonic/primes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 """Prime number operations used for just intonation."""
 
-from math import gcd
 from functools import reduce
+from math import gcd
+from typing import List
 
 
-__version__ = '0.0.1'
-
-
-def is_prime(number):
+def is_prime(number: int) -> bool:
     """States if a number is prime.
 
-    :param number: A number
-    :type number: int
+    Parameters:
+        number: A number
 
-    :rtype: bool
+    Returns:
+        Whether or not the number is prime
 
-    **Examples**
+    Examples:
+        >>> is_prime(31)
+        True
 
-    >>> is_prime(31)
-    True
-
-    >>> is_prime(42)
-    False
+        >>> is_prime(42)
+        False
     """
     for factor in range(2, number):
         if not number % factor:
             return False
     return True
 
 
-def generate_primes(limit):
+def generate_primes(limit: int) -> List[int]:
     """Generates primes up to a given limit.
 
-    :param limit: The limit.
-    :type limit: int
-
-    :rtype: list of int
+    Parameters:
+        limit: The limit.
 
-    **Examples**
+    Returns:
+        Primes
 
-    >>> generate_primes(31)
-    [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31]
+    Examples:
+        >>> generate_primes(31)
+        [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31]
     """
     return [n for n in range(2, limit + 1) if is_prime(n)]
 
 
-def prime_factors(number):
+def prime_factors(number: int) -> List[int]:
     """Finds prime factors of an integer (by trial-division).
 
-    :param number: The integer to factor
-    :type number: int
+    Parameters:
+        number: The integer to factor
 
-    :rtype: list of ints
+    Returns:
+        Prime factors
 
-    **Examples**
+    Examples:
+        >>> prime_factors(314)
+        [2, 157]
 
-    >>> prime_factors(314)
-    [2, 157]
-
-    >>> prime_factors(31)
-    [31]
+        >>> prime_factors(31)
+        [31]
     """
     factor = 2
     factors = []
     while factor * factor <= number:
         if number % factor:
             factor += 1
         else:
@@ -71,24 +69,24 @@
             factors.append(factor)
     if number > 1:
         factors.append(number)
 
     return factors
 
 
-def lcm(numbers):
+def lcm(numbers: List[int]) -> int:
     """Least common multiple of a list of integers.
 
-    :param numbers: List of integers
-    :type numbers: list of int
-
-    :rtype: int
+    Parameters:
+        numbers: List of integers
 
-    **Examples**
+    Returns:
+        Least common multiple
 
-    >>> lcm([15, 3, 5])
-    15
+    Examples:
+        >>> lcm([15, 3, 5])
+        15
 
-    >>> lcm([21, 6, 7])
-    42
+        >>> lcm([21, 6, 7])
+        42
     """
     return reduce(lambda x, y: x * y // gcd(x, y), numbers)
```

### Comparing `jintonic-0.0.1/jintonic/chords.py` & `jintonic-0.2.3/src/jintonic/chords.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,321 +1,309 @@
 """Implements just intonation chords."""
+from __future__ import annotations
 
 from copy import deepcopy
+from typing import List
 
+from .harmonics import harmonic_segment_to_identities, tones_to_harmonic_segment
 from .intervals import JustInterval
-from .primes import generate_primes
 from .lattice import JustLattice
-from .harmonics import tones_to_harmonic_segment
-from .harmonics import harmonic_segment_to_identities
-
-
-__version__ = '0.0.1'
+from .primes import generate_primes
 
 
-class JustLatticeChord():
+class JustLatticeChord:
     """This class implements chords based on lattice coordinates."""
 
-    def __init__(self, nodes, fundamental=60, root=(0, )):
+    def __init__(
+        self,
+        fundamental: float,
+        root: List[int],
+        nodes: List[List[int]],
+    ):
         """Initializes a JustLatticeChord.
 
-        :param nodes: Lattice nodes of each constituent chord tone.
-        :type nodes: list of tuple
-        :param fundamental: Fundamental pitch in Hertz.
-        :type fundamental: float
-        :param root: Root lattice node (the chord's root tone)
-        :type root: tuple
-
-        **Examples**
-
-        >>> nodes = [(-1, 0, 1), (1, ), (0, 0, 1)]
-        >>> JustLatticeChord(nodes, fundamental=100, root=(1, ))
-        JustLatticeChord(100 - [3/2, 7/4, 9/8, 21/16], [3-7-9-21])
-        """
-        self._fundamental = None
-        self._root = None
-        self._nodes = None
-
-        self.fundamental = fundamental
-        self.nodes = nodes
-        self.root = root
-        self.lattice = JustLattice(fundamental=self.fundamental)
+        Parameters:
+            fundamental: Fundamental pitch in Hertz.
+            root: Root lattice node (the chord's root tone)
+            nodes: Lattice nodes of each constituent chord tone.
+
+        Examples:
+            >>> nodes = [[-1, 0, 1], [1, 0, 0], [0, 0, 1]]
+            >>> JustLatticeChord(fundamental=100.0, root=[1, 0, 0], nodes=nodes)
+            JustLatticeChord(100.0 Hz, [3/2, 7/4, 9/8, 21/16], [3-7-9-21])
+        """
+        self._fundamental: float = float(fundamental)
+        self._nodes = nodes
+        self._root = root
+        self.lattice = JustLattice(fundamental=self._fundamental)
 
     @classmethod
-    def from_name(cls, name, fundamental=60, root=(0, )):
+    def from_name(
+        cls,
+        fundamental: float,
+        root: List[int],
+        name: str,
+    ) -> JustLatticeChord:
         """Initializes a JustLatticeChord from a conventional chord name.
 
-        **Examples**
-
-        >>> JustLatticeChord.from_name('minor triad')
-        JustLatticeChord(60 - [1/1, 6/5, 3/2], [5-3-15])
-
-        >>> JustLatticeChord.from_name('major triad', root=(-1, ))
-        JustLatticeChord(60 - [4/3, 5/3, 1/1], [1-5-3])
-        """
-        names = {
-            'sub-minor triad': cls(
-                [(1, ), (-1, 0, 1)],
-                fundamental, root),
-            'minor triad': cls(
-                [(1, -1), (1, )],
-                fundamental, root),
-            'diminished triad': cls(
-                [(1, -1), (0, -1, 1)],
-                fundamental, root),
-            'major triad': cls(
-                [(0, 1), (1, )],
-                fundamental, root),
-            'sub-minor seventh': cls(
-                [(-1, 0, 1), (1, ), (0, 0, 1)],
-                fundamental, root),
-            'minor seventh': cls(
-                [(1, -1), (1, ), (2, -1)],
-                fundamental, root),
-            'half-diminished seventh': cls(
-                [(1, -1), (0, -1, 1), (2, -1)],
-                fundamental, root),
-            'major seventh': cls(
-                [(0, 1), (1, ), (1, 1)],
-                fundamental, root),
-            'super-major seventh': cls(
-                [(2, 0, -1), (1, ), (3, 0, -1)],
-                fundamental, root),
-            'dominant seventh': cls(
-                [(0, 1), (1, ), (1, 1), (0, 0, 1)],
-                fundamental, root),
-            'added second': cls(
-                [(0, 1), (1, ), (2, -1)],
-                fundamental, root),
-            'minor ninth': cls(
-                [(1, -1), (1, ), (2, -1), (2, )],
-                fundamental, root),
-            'major ninth': cls(
-                [(0, 1), (1, ), (1, 1), (2, )],
-                fundamental, root),
-            'dominant ninth': cls(
-                [(0, 1), (1, ), (0, 0, 1), (2, )],
-                fundamental, root),
-            '4-6-7': cls(
-                [(1, ), (0, 0, 1)],
-                fundamental, root),
-            '5-7-9': cls(
-                [(0, -1, 1), (2, -1)],
-                fundamental, root),
+        Parameters:
+            fundamental: The fundamental frequency in Hertz
+            root: The root node lattice coordinates
+            name: The chord name
+
+        Returns:
+            A JustLatticeChord
+
+        The list of valid names is:
+            - "sub-minor triad"
+            - "minor triad"
+            - "diminished triad"
+            - "major triad"
+            - "sub-minor seventh"
+            - "minor seventh"
+            - "half-diminished seventh"
+            - "major seventh"
+            - "super-major seventh"
+            - "dominant seventh"
+            - "added second"
+            - "minor ninth"
+            - "major ninth"
+            - "dominant ninth"
+            - "4-6-7"
+            - "5-7-9"
+
+        Examples:
+
+            >>> JustLatticeChord.from_name(60, [0, 0, 0], 'minor triad')
+            JustLatticeChord(60.0 Hz, [1/1, 6/5, 3/2], [5-3-15])
+
+            >>> JustLatticeChord.from_name(60, [-1, 0, 0], 'major triad')
+            JustLatticeChord(60.0 Hz, [4/3, 5/3, 1/1], [1-5-3])
+        """
+        nodes = {
+            "sub-minor triad": [[1, 0, 0], [-1, 0, 1]],
+            "minor triad": [[1, -1, 0], [1, 0, 0]],
+            "diminished triad": [[1, -1, 0], [0, -1, 1]],
+            "major triad": [[0, 1, 0], [1, 0, 0]],
+            "sub-minor seventh": [[-1, 0, 1], [1, 0, 0], [0, 0, 1]],
+            "minor seventh": [[1, -1, 0], [1, 0, 0], [2, -1, 0]],
+            "half-diminished seventh": [[1, -1, 0], [0, -1, 1], [2, -1, 0]],
+            "major seventh": [[0, 1, 0], [1, 0, 0], [1, 1, 0]],
+            "super-major seventh": [[2, 0, -1], [1, 0, 0], [3, 0, -1]],
+            "dominant seventh": [[0, 1, 0], [1, 0, 0], [1, 1, 0], [0, 0, 1]],
+            "added second": [[0, 1, 0], [1, 0, 0], [2, -1, 0]],
+            "minor ninth": [[1, -1, 0], [1, 0, 0], [2, -1, 0], [2, 0, 0]],
+            "major ninth": [[0, 1, 0], [1, 0, 0], [1, 1, 0], [2, 0, 0]],
+            "dominant ninth": [[0, 1, 0], [1, 0, 0], [0, 0, 1], [2, 0, 0]],
+            "4-6-7": [[1, 0, 0], [0, 0, 1]],
+            "5-7-9": [[0, -1, 1], [2, -1, 0]],
         }
         try:
-            return names[name.lower()]
+            return cls(fundamental, root, nodes[name.lower()])
         except KeyError:
             return NotImplemented
 
-    def transpose(self, node):
+    def transpose(self, node: List[int]) -> JustLatticeChord:
         """JustLatticeChord transposition.
 
-        Returns a copy
-
-        :param node: The target root node of the transposed chord.
-        :type node: tuple
+        Parameters:
+            node: The target root node of the transposed chord.
 
-        :rtype: JustLatticeChord
+        Returns:
+            A transposed JustLatticeChord
 
-        **Examples**
+        Note:
+            Returns a copy
 
-        >>> chord = JustLatticeChord.from_name('minor triad')
-        >>> node = (1, )
-        >>> chord.transpose(node)
-        JustLatticeChord(60 - [3/2, 9/5, 9/8], [5-3-15])
+        Examples:
+            >>> chord = JustLatticeChord.from_name(60, [0, 0, 0], 'minor triad')
+            >>> node = [1, 0, 0]
+            >>> chord.transpose(node)
+            JustLatticeChord(60.0 Hz, [3/2, 9/5, 9/8], [5-3-15])
         """
         chord = deepcopy(self)
         chord.root = node
-        chord.lattice.to_node(*node)
+        chord.lattice.to_node((node))
 
         return chord
 
-    def pivot(self, axis=3):
-        """Pivots the JustLatticeChord wither vertically or horizontally.
-
-        Returns a copy.
+    def pivot(self, axis: int = 3) -> JustLatticeChord:
+        """Pivots the JustLatticeChord along the given axis.
 
-        :param axis: Prime limit axis (a prime number)
-        :type axis: int
+        Parameters:
+            axis: Prime limit axis (a prime number)
 
-        :rtype: JustLatticeChord
+        Returns:
+            A pivoted JustLatticeChord
 
-        **Examples**
-
-        >>> chord = JustLatticeChord.from_name('major triad')
-        >>> chord.pivot(3)
-        JustLatticeChord(60 - [1/1, 8/5, 3/2], [5-1-15])
-        """
+        Note:
+            Returns a copy
+
+        Examples:
+            >>> chord = JustLatticeChord.from_name(60, [0, 0, 0], 'major triad')
+            >>> chord.pivot(3)
+            JustLatticeChord(60.0 Hz, [1/1, 5/4, 4/3], [3-15-1])
+        """
+        if axis > self.prime_limit:
+            raise ValueError(
+                "Cannot pivot on an axis greater than the chord's prime limit."
+            )
         chord = deepcopy(self)
-        axis_ix = generate_primes(chord.prime_limit)[1:].index(axis) + 1
-        base = min(node[axis_ix] for node in chord.nodes)
-        for i, node in enumerate(chord.nodes):
-            node = list(node)
+        axis_ix = generate_primes(chord.prime_limit)[1:].index(axis)
+        base = min(node[axis_ix] for node in chord._nodes)
+        base = 0
+        for i, node in enumerate(chord._nodes):
             node[axis_ix] = base - node[axis_ix]
-            chord.nodes[i] = tuple(node)
+            chord._nodes[i] = node
         return chord
 
     @property
-    def nodes(self):
-        """JustLatticeChord nodes.
+    def fundamental(self):
+        return self._fundamental
 
-        :param values: Constituent lattice nodes.
-        :type values: list of tuple
-
-        :rtype: list of tuple
-        """
+    @property
+    def nodes(self):
+        """JustLatticeChord nodes."""
         return self._nodes
 
     @nodes.setter
-    def nodes(self, values):
+    def nodes(self, values: List[List[int]]):
+        """JustLatticeChord nodes.
+
+        Parameters:
+            values: Constituent lattice nodes.
+        """
         """Sets (and expands) JustLatticeChord nodes."""
         max_len = max((len(node) for node in values))
         self._nodes = []
         for node in values:
-            self._nodes.append(
-                node + tuple((max_len - len(node)) * [0])
-            )
+            self._nodes.append(node + (max_len - len(node)) * [0])
 
     @property
     def root(self):
-        """JustLatticeChord root node.
-
-        :param value: Root lattice node
-        :type value: tuple
-
-
-        :rtype: tuple
-        """
+        """JustLatticeChord root node."""
         return self._root
 
     @root.setter
-    def root(self, value):
-        """Sets (and expands) JustLatticeChord root node."""
-        max_len = max((len(node) for node in self.nodes))
-        self._root = value + tuple((max_len - len(value)) * [0])
+    def root(self, value: List[int]):
+        """Sets (and expands) JustLatticeChord root node.
+
+        Parameters:
+            value: Root lattice node
+        """
+        max_len = max((len(node) for node in self._nodes))
+        self._root = value + (max_len - len(value)) * [0]
 
     @property
-    def tones(self):
+    def tones(self) -> List[JustInterval]:
         """JustLatticeChord constituent intervals from root (tones).
 
-        :rtype: list of JustInterval
+        Returns:
+            The tones of the chord as JustIntervals from the fundamental.
 
-        **Examples**
-
-
-        >>> chord = JustLatticeChord.from_name('major triad')
-        >>> chord.tones
-        [JustInterval(1, 1), JustInterval(5, 4), JustInterval(3, 2)]
+        Examples:
+            >>> chord = JustLatticeChord.from_name(60, [0, 0, 0], 'major triad')
+            >>> chord.tones
+            [JustInterval(1, 1), JustInterval(5, 4), JustInterval(3, 2)]
         """
         tones = []
-        self.lattice.to_node(*self.root)
+        self.lattice.to_node(self._root)
         root_tone = self.lattice.tone
         tones.append(root_tone)
-        for node in self.nodes:
-            self.lattice.to_node(*self.root)
-            constituent = self.lattice.traverse(*node)
+        for node in self._nodes:
+            self.lattice.to_node(self._root)
+            constituent = self.lattice.traverse(node)
             constituent_tone = constituent.tone
             tones.append(constituent_tone)
-        self.lattice.to_node(*self.root)
+        self.lattice.to_node(self._root)
 
         return tones
 
     @property
-    def prime_limit(self):
-        """JustLatticeChord prime limit.
-
-        :rtype: int
-        """
+    def prime_limit(self) -> int:
+        """JustLatticeChord prime limit."""
         return max([tone.prime_limit for tone in self.tones])
 
     @property
-    def harmonics(self):
+    def harmonics(self) -> List[int]:
         """JustLatticeChord harmonics (relative frequencies).
 
-        :rtype: list of int
-
-        **Examples**
+        Returns:
+            The lattice's prime limit
 
-
-        >>> chord = JustLatticeChord.from_name('minor triad')
-        >>> chord.harmonics
-        [10, 12, 15]
+        Examples:
+            >>> chord = JustLatticeChord.from_name(60, [0, 0, 0], 'minor triad')
+            >>> chord.harmonics
+            [10, 12, 15]
         """
         return tones_to_harmonic_segment(self.tones)
 
     @property
-    def identities(self):
+    def identities(self) -> List[int]:
         """JustLatticeChord constituent identities.
 
-        :rtype: list of int
-
-        **Examples**
-
+        Returns:
+            The constituent identities
 
-        >>> chord = JustLatticeChord.from_name('minor triad')
-        >>> chord.identities
-        [5, 3, 15]
+        Examples:
+            >>> chord = JustLatticeChord.from_name(60, [0, 0, 0], 'minor triad')
+            >>> chord.identities
+            [5, 3, 15]
         """
         return harmonic_segment_to_identities(self.harmonics)
 
     @property
-    def hertz(self):
+    def hertz(self) -> List[float]:
         """JustLatticeChord constituent Hertz values.
 
-        :rtype: list of float
+        Returns:
+            The frequencies in Hertz of the constituent pitches
 
-        **Examples**
-
-
-        >>> chord = JustLatticeChord.from_name('minor triad')
-        >>> chord.hertz
-        [60.0, 72.0, 90.0]
+        Examples:
+            >>> chord = JustLatticeChord.from_name(60, [0, 0, 0], 'minor triad')
+            >>> chord.hertz
+            [60.0, 72.0, 90.0]
         """
         tones = [self.tones[0]]
         for tone in self.tones[1:]:
             while tone < tones[-1]:
                 tone += JustInterval(2, 1)
             tones.append(tone)
-        return [self.fundamental * tone for tone in tones]
+        return [self._fundamental * tone for tone in tones]
 
     @property
-    def complement(self):
+    def complement(self) -> JustLatticeChord:
         """JustLatticeChord complement.
 
         Every node's relationship to the root node is inverted.
 
-        Returns a copy.
-
-        :rtype: JustLatticeChord
+        Returns:
+            A JustLatticeChord that is the complement of this one
 
-        **Examples**
+        Note:
+            Returns a copy.
 
-        >>> chord = JustLatticeChord([(2, ), (0, 1), (-1, ), (1, )])
-        >>> chord.complement
-        JustLatticeChord(60 - [1/1, 16/9, 8/5, 3/2, 4/3], [45-5-9-135-15])
+        Examples:
+            >>> nodes = [[2, 0], [0, 1], [-1, 0], [1, 0]]
+            >>> chord = JustLatticeChord(60, [0, 0, 0], nodes)
+            >>> chord.complement
+            JustLatticeChord(60.0 Hz, [1/1, 16/9, 8/5, 3/2, 4/3], [45-5-9-135-15])
         """
         nodes = []
-        for node in self.nodes:
-            nodes.append(
-                tuple(map(lambda x, y: y - x, node, self.root))
-            )
-        return JustLatticeChord(nodes, self.fundamental, self.root)
+        for node in self._nodes:
+            nodes.append(list(map(lambda x, y: y - x, node, self._root)))
+        return JustLatticeChord(self._fundamental, self._root, nodes)
 
     def __repr__(self):
-        """repr(self)
-
-        (<fundamental> - [<tones>], [<identities>])
-        """
-        tones = ', '.join([
-            '/'.join([str(tone.numerator), str(tone.denominator)])
-            for tone in self.tones
-        ])
-        identities = ', '.join([
-            '-'.join([str(identity) for identity in self.identities])
-        ])
-        return "{}({} - [{}], [{}])".format(
-            self.__class__.__name__,
-            self.fundamental,
-            tones,
-            identities
+        """repr(self)"""
+        tones = ", ".join(
+            [
+                "/".join([str(tone.numerator), str(tone.denominator)])
+                for tone in self.tones
+            ]
+        )
+        identities = ", ".join(
+            ["-".join([str(identity) for identity in self.identities])]
+        )
+        return "{}({} Hz, [{}], [{}])".format(
+            self.__class__.__name__, self._fundamental, tones, identities
         )
```

### Comparing `jintonic-0.0.1/jintonic/intervals.py` & `jintonic-0.2.3/src/jintonic/intervals.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,211 +1,197 @@
 """Implements just intonation intervals (ratios)."""
+from __future__ import annotations
 
+import operator
 import re
-from decimal import Decimal
-from math import gcd, log
 from copy import deepcopy
-import operator
+from math import gcd, log
+from typing import Any, Callable, List, Tuple
 
 from .primes import is_prime, prime_factors
 
-
-__version__ = '0.0.1'
-
-
 # String format for just ratios (JustInterval). eg: '3:2'
-_RATIO_FORMAT = re.compile(r"""
+_RATIO_FORMAT = re.compile(
+    r"""
     \A\s*
     (?P<num>\d*):(?P<denom>\d*)
     \s*\Z
-""", re.VERBOSE | re.IGNORECASE)
+""",
+    re.VERBOSE | re.IGNORECASE,
+)
 
 
-def primary_interval(prime_limit, max_pot_exp=500):
+def primary_interval(
+    prime_limit: int,
+    sub_harmonic: bool = False,
+    max_pot_exp: int = 500,
+) -> JustInterval:
     """Returns the primary interval for a given prime limit.
 
-    :param prime_limit: A prime number
-    :type prime_limit: int
-    :param max_pot_exp: Maximum power of two exponent to limit iterations
-    :type max_pot_exp: int
-
-    :rtype: JustInterval
+    Parameters:
+        prime_limit: A prime number
+        sub_harmonic: Whether the primary interval is a harmonic primary
+            (the default) or a sub-harmonic primary.
+        max_pot_exp: Maximum power of two exponent to limit iterations
+
+    Examples:
+        >>> primary_interval(7)
+        JustInterval(7, 4)
 
-    **Examples**
+        >>> primary_interval(19)
+        JustInterval(19, 16)
 
-    >>> primary_interval(7)
-    JustInterval(7, 4)
-
-    >>> primary_interval(19)
-    JustInterval(19, 16)
+        >>> primary_interval(3, sub_harmonic=True)
+        JustInterval(4, 3)
     """
     pot = 2
     exp = 2
     max_pot = 2**max_pot_exp
     while (pot**exp < prime_limit) and (pot < max_pot):
         exp += 1
-    pot = pot**(exp-1)
+    pot = pot ** (exp - 1)
+    if sub_harmonic:
+        return JustInterval(prime_limit, pot).complement
     return JustInterval(prime_limit, pot)
 
 
-class JustInterval():
+class JustInterval:
     """This class implements just intonation intervals."""
 
-    def __init__(self, numerator, denominator=None):
+    def __init__(self, numerator: int, denominator: int):
         """Initializes a JustInterval.
 
-        Takes a string like '3:2' or '4:3' or a pair of numerator, denominator
-        integers.
-
-        :param numerator: String representation or integer numerator
-        :type numerator: str or int
-        :param denominator: Denominator
-        :type denominator: int
-
-        **Examples**
-
-        >>> JustInterval('3:2')
-        JustInterval(3, 2)
-
-        >>> JustInterval('3:3')
-        JustInterval(1, 1)
-
-        >>> JustInterval('6:3')
-        JustInterval(2, 1)
-
-        >>> JustInterval(4, 3)
-        JustInterval(4, 3)
-        """
-
-        if denominator is None:
-            if isinstance(numerator, int):
-                denominator = 1
-
-            elif isinstance(numerator, str):
-                re_match = _RATIO_FORMAT.match(numerator)
-                if re_match is None:
-                    msg = 'Invalid literal for JustRatio: {}'.format(numerator)
-                    raise ValueError(msg)
-                try:
-                    numerator = int(re_match.group('num'))
-                    denominator = int(re_match.group('denom'))
-                except ValueError:
-                    msg = 'Invalid literal for JustRatio: {}'.format(numerator)
-                    raise ValueError(msg)
-
-            elif isinstance(numerator, (float, Decimal)):
-                numerator, denominator = numerator.as_integer_ratio()
-
-            else:
-                msg = 'Numerator should be a string or a Rational instance.'
-                msg += 'Got: {}'.format(type(numerator))
-                raise TypeError(msg)
-
-        elif isinstance(numerator, int) and isinstance(denominator, int):
-            pass
-
-        else:
-            msg = 'Both components must be integers. '
-            msg += 'Got numerator: {}, denominator: {}'.format(
+        Parameters:
+            numerator: Numerator
+            denominator: Denominator
+
+        Examples:
+            >>> JustInterval(4, 3)
+            JustInterval(4, 3)
+        """
+        if not (isinstance(numerator, int) and isinstance(denominator, int)):
+            msg = "Both components must be integers. "
+            msg += "Got numerator: {}, denominator: {}".format(
                 type(numerator), type(denominator)
             )
             raise TypeError(msg)
 
         if denominator > numerator:
-            msg = 'Numerator must be greater than or equal to denominator. '
-            msg += 'Got numerator: {}, denominator: {}'.format(
-                numerator, denominator
-            )
+            msg = "Numerator must be greater than or equal to denominator. "
+            msg += "Got numerator: {}, denominator: {}".format(numerator, denominator)
             raise ValueError(msg)
 
         if denominator == 0:
-            raise ZeroDivisionError('JustRatio({}, 0)'.format(numerator))
+            raise ZeroDivisionError("JustRatio({}, 0)".format(numerator))
 
         if denominator < 1:
-            msg = 'Denominator must be greater than 0. '
-            msg += 'Got: {}'.format(numerator)
+            msg = "Denominator must be greater than 0. "
+            msg += "Got: {}".format(numerator)
             raise ValueError(msg)
 
         common = gcd(numerator, denominator)
         numerator //= common
         denominator //= common
 
         self._numerator = numerator
         self._denominator = denominator
 
     @classmethod
-    def from_two_hertz(cls, apitch, bpitch):
-        """Creates a JustInterval from two Hertz values.
+    def from_string(cls, interval: str) -> JustInterval:
+        """Creates a JustInterval from a string representation.
 
-        :param apitch: A value in Hertz
-        :type apitch: int
-        :param bpitch: A value in Hertz
-        :type bpitch: int
+        Parameters:
+            interval: A string representation of an interval in the
+                `numerator:denominator` format.
 
-        :rtype: JustInterval
+        Returns:
+            A JustInterval
 
-        **Examples**
+        Examples:
+            >>> JustInterval.from_string('3:2')
+            JustInterval(3, 2)
 
-        >>> JustInterval.from_two_hertz(220, 440)
-        JustInterval(2, 1)
+            >>> JustInterval.from_string('3:3')
+            JustInterval(1, 1)
+
+            >>> JustInterval.from_string('6:3')
+            JustInterval(2, 1)
         """
-        if isinstance(apitch, int) and isinstance(bpitch, int):
-            pass
+        re_match = _RATIO_FORMAT.match(interval)
+        if re_match is None:
+            msg = "Invalid literal for JustRatio: {}".format(interval)
+            raise ValueError(msg)
+        try:
+            numerator = int(re_match.group("num"))
+            denominator = int(re_match.group("denom"))
+            return JustInterval(numerator=numerator, denominator=denominator)
+        except ValueError:
+            msg = "Invalid literal for JustRatio: {}".format(interval)
+            raise ValueError(msg)
 
-        else:
-            try:
-                apitch = apitch.frequency
-                bpitch = bpitch.frequency
-            except AttributeError:
-                msg = 'Arguments must either be integers or '
-                msg += 'have a hertz attribute. '
-                msg += 'Got: {} and {}'.format(type(apitch), type(bpitch))
-                raise ValueError(msg)
+    @classmethod
+    def from_two_hertz(cls, apitch: float, bpitch: float) -> JustInterval:
+        """Creates a JustInterval from two Hertz values.
 
+        Parameters:
+            apitch: A value in Hertz (which will be truncated to an int)
+            bpitch: A value in Hertz (which will be truncated to an int)
+
+        Returns:
+            A JustInterval
+
+        Examples:
+            >>> JustInterval.from_two_hertz(220, 440)
+            JustInterval(2, 1)
+        """
         smaller = apitch if apitch <= bpitch else bpitch
         greater = apitch if apitch > bpitch else bpitch
 
-        return cls(greater, smaller)
+        return cls(int(greater), int(smaller))
 
-    def divisions(self, divisor, prime_limit=7, max_iterations=30):
+    def divisions(
+        self,
+        divisor: int,
+        prime_limit: int = 7,
+        max_iterations: int = 30,
+    ) -> List[JustInterval]:
         """Divides a just interval into intervals that respect a prime limit.
 
-        :param divisor: Number of divisions.
-        :type divisor: int
-        :param prime_limit: The prime limit, a prime number.
-        :type prime_limit: int
-        :param max_iterations: A limit to how many divisions this method will
-            try before giving up on dividing within the prime limit.
-        :type max_iterations: int
-
-        :rtype: list of JustInterval
-
-        **Examples**
-
-        >>> JustInterval(2, 1).divisions(4, 5)
-        [JustInterval(10, 9), JustInterval(9, 8), JustInterval(6, 5),
-        JustInterval(4, 3)]
+        Parameters:
+            divisor: Number of divisions.
+            prime_limit: The prime limit, a prime number.
+            max_iterations: A limit to how many divisions this method will
+                try before giving up on dividing within the prime limit.
+
+        Returns:
+            The resulting JustIntervals
+
+        Examples:
+            >>> JustInterval(2, 1).divisions(4, 5)
+            [JustInterval(10, 9), JustInterval(9, 8), JustInterval(6, 5),
+            JustInterval(4, 3)]
 
-        >>> JustInterval(16, 15).divisions(2, 31)
-        [JustInterval(32, 31), JustInterval(31, 30)]
+            >>> JustInterval(16, 15).divisions(2, 31)
+            [JustInterval(32, 31), JustInterval(31, 30)]
         """
         if not is_prime(prime_limit):
-            msg = 'The prime limit must be a prime number. '
+            msg = "The prime limit must be a prime number. "
             msg += "Got: '{}'".format(prime_limit)
             raise ValueError(msg)
 
         factor = divisor
-        divisions = []
+        divisions: List[JustInterval] = []
+        divrange: List[int] = []
         i = 0
         while i <= max_iterations:
             num = self.numerator * factor
             denom = self.denominator * factor
 
             divrange = list(range(denom, num + 1))
-            primes = []
+            primes: List[int] = []
             for number in divrange:
                 if is_prime(number) and (number > prime_limit):
                     primes.append(number)
             for prime in primes:
                 divrange.remove(prime)
             if len(divrange) != divisor + 1:
                 factor += 1
@@ -220,280 +206,257 @@
                 divisions.append(JustInterval(number, divrange[j + 1]))
             except IndexError:
                 continue
 
         return sorted(divisions)
 
     @property
-    def numerator(self):
+    def numerator(self) -> int:
         """JustInterval numerator."""
         return self._numerator
 
     @property
-    def denominator(self):
+    def denominator(self) -> int:
         """JustInterval denominator."""
         return self._denominator
 
     @property
-    def prime_limit(self):
+    def prime_limit(self) -> int:
         """JustInterval prime limit.
 
-        :rtype: int
-
-        **Examples**
-
-        >>> JustInterval(64, 49).prime_limit
-        7
+        Examples:
+            >>> JustInterval(64, 49).prime_limit
+            7
         """
         if self.base_octave == JustInterval(1, 1):
             return 1
         num = max(prime_factors(self.numerator))
         denom = max(prime_factors(self.denominator))
 
         return max(num, denom)
 
     @property
-    def is_superparticular(self):
+    def is_superparticular(self) -> bool:
         """Superparticular just intervals are of the form x+1:x
 
-        :rtype: bool
-
-        **Examples**
-
-        >>> JustInterval(3, 2).is_superparticular
-        True
+        Examples:
+            >>> JustInterval(3, 2).is_superparticular
+            True
         """
         return self.numerator == self.denominator + 1
 
     @property
-    def base_octave(self):
+    def base_octave(self) -> JustInterval:
         """The interval within the range 1:1 to 2:1
 
-        :rtype: JustInterval
-
-        **Examples**
-
-        >>> JustInterval('9:4').base_octave
-        JustInterval(9, 8)
+        Examples:
+            >>> JustInterval.from_string('9:4').base_octave
+            JustInterval(9, 8)
         """
         cself = deepcopy(self)
         while cself >= JustInterval(2, 1):
             cself -= JustInterval(2, 1)
         return cself
 
     @property
-    def complement(self):
+    def complement(self) -> JustInterval:
         """JustInterval complement.
 
-        Returns the interval which, when added to this interval, yields an
+        The interval which, when added to this interval, yields an
         octave. This only applies to intervals smaller than the octave and
         will return `NotImplemented` if self is an interval larger than an
         octave.
 
-        :rtype: JustInterval
+        Returns:
+            The interval's complement
 
-        **Examples**
+        Note:
+            Returns a copy
 
-        >>> JustInterval(3, 2).complement
-        JustInterval(4, 3)
+        Examples:
+            >>> JustInterval(3, 2).complement
+            JustInterval(4, 3)
         """
         octave = JustInterval(2, 1)
         if self < octave:
             return octave - self
         if self == octave:
             return JustInterval(1, 1)
         return NotImplemented
 
     @property
-    def cents(self):
+    def cents(self) -> float:
         """JustInterval expressed in Cents.
 
-        :rtype: float
-
-        **Examples**
+        Returns:
+            The interval in Cents
 
-        >>> round(JustInterval(3, 2).cents, 3)
-        701.955
+        Examples:
+            >>> round(JustInterval(3, 2).cents, 3)
+            701.955
         """
-        return (
-            log(self.numerator / self.denominator, 10) *
-            (1200 / log(2, 10))
-        )
+        return log(self.numerator / self.denominator, 10) * (1200 / log(2, 10))
 
-    def _prepare_division(self, number):
+    def _prepare_division(self, number: int) -> Tuple[int, int]:
         """Helper for JustInterval division."""
         if not isinstance(number, int):
-            msg = 'Must be int, not {}'.format(type(number))
+            msg = "Must be int, not {}".format(type(number))
             raise TypeError(msg)
 
         if not self.is_superparticular:
             if number % (self.numerator - self.denominator):
-                msg = '{} is not divisible by {}'.format(self, number)
+                msg = "{} is not divisible by {}".format(self, number)
                 raise ValueError(msg)
             factor = number // (self.numerator - self.denominator)
             num = self.numerator * factor
             denom = self.denominator * factor
 
         else:
             num = self.numerator * number
             denom = self.denominator * number
 
         return num, denom
 
     def __repr__(self):
         """repr(self)"""
-        return '{}({}, {})'.format(
-            self.__class__.__name__,
-            self._numerator,
-            self.denominator)
+        return "{}({}, {})".format(
+            self.__class__.__name__, self._numerator, self.denominator
+        )
 
-    def __add__(self, other):
+    def __add__(self, other: JustInterval) -> JustInterval:
         """JustInterval addition.
 
-        :rtype: JustInterval
-
-        **Examples**
+        Examples:
 
         >>> JustInterval(3, 2) + JustInterval(4, 3)
         JustInterval(2, 1)
         """
         if not isinstance(other, JustInterval):
             other = JustInterval(other.numerator, other.denominator)
         return JustInterval(
-            self.numerator * other.numerator,
-            self.denominator * other.denominator
+            self.numerator * other.numerator, self.denominator * other.denominator
         )
 
-    def __radd__(self, other):
+    def __radd__(self, other: JustInterval) -> JustInterval:
         """JustInterval right of operator addition.
 
-        **Examples**
+        Examples:
 
         >>> sum((JustInterval(3, 2), JustInterval(4, 3)))
         JustInterval(2, 1)
         """
         if other == 0:
             other = JustInterval(1, 1)
         return self + other
 
-    def __sub__(self, other):
+    def __sub__(self, other: JustInterval) -> JustInterval:
         """JustInterval substraction.
 
-        :rtype: JustInterval
-
-        **Examples**
+        Examples:
 
         >>> JustInterval(3, 2) - JustInterval(9, 8)
         JustInterval(4, 3)
         >>> JustInterval(1, 1) - JustInterval(3, 2)
         JustInterval(4, 3)
         """
-        if not isinstance(other, JustInterval):
-            other = JustInterval(other.numerator, other.denominator)
         if other > self:
             cself = deepcopy(self)
             cself += JustInterval(2, 1)
             return cself - other
         return JustInterval(
-            self.numerator * other.denominator,
-            self.denominator * other.numerator
+            self.numerator * other.denominator, self.denominator * other.numerator
         )
 
     def __mul__(self, other):
         """JustInterval left of operator multiplication."""
         return NotImplemented
 
-    def __rmul__(self, other):
+    def __rmul__(self, other: float) -> float:
         """JustInterval right of operator multiplication.
 
         This is used to calculate the absolute frequency of a pitch _this_
         interval above it.
 
-        :rtype: float
-
-        **Examples**
+        Examples:
 
         >>> 440 * JustInterval(3, 2)
         660.0
         """
         try:
             return other * (self.numerator / self.denominator)
         except TypeError:
             msg = "Can't multiply sequence by non-int of type '{}'".format(
                 self.__class__.__name__
             )
             raise TypeError(msg)
 
-    def __pow__(self, other):
+    def __pow__(self, other: int) -> JustInterval:
         """JustInterval raised to a power. Used for chaining an interval.
 
-        :rtype: JustInterval
+        Examples:
 
-        **Examples**
-
-        >>> JustInterval('3:2') ** 3
+        >>> JustInterval(3, 2) ** 3
         JustInterval(27, 8)
         """
         if other < 0:
-            msg = 'JustInterval can only be raised to positive powers. '
+            msg = "JustInterval can only be raised to positive powers. "
             msg += "Got '{}'".format(other)
             raise ValueError(msg)
         elif other == 0:
             return JustInterval(1, 1)
-        return sum([self] * other)
+        return sum([self] * other)  # type: ignore
 
-    def __truediv__(self, other):
+    def __truediv__(self, other: int) -> List[JustInterval]:
         """Naive JustInterval division.
 
         For divisions within a given prime limit, use self.divisions()
 
         :rtype: JustInterval
 
-        **Examples**
+        Examples:
 
         >>> JustInterval(2, 1) / 2
         [JustInterval(4, 3), JustInterval(3, 2)]
         >>> JustInterval(2, 1) / 3
         [JustInterval(6, 5), JustInterval(5, 4), JustInterval(4, 3)]
         >>> JustInterval(7, 4) / 3
         [JustInterval(7, 6), JustInterval(6, 5), JustInterval(5, 4)]
         """
         num, denom = self._prepare_division(other)
 
-        return sorted(
-            [JustInterval(n, n - 1) for n in range(denom + 1, num + 1)]
-        )
+        return sorted([JustInterval(n, n - 1) for n in range(denom + 1, num + 1)])
 
     def __rtruediv__(self, other):
         """There's no sense dividing something by a JustInterval."""
         return NotImplemented
 
-    def _richcmp(self, other, oper):
+    def _richcmp(self, other: JustInterval, oper: Callable) -> bool:
         """Helper for comparison operators, for internal use only."""
         return oper(
-            self.numerator / self.denominator,
-            other.numerator / other.denominator
+            self.numerator / self.denominator, other.numerator / other.denominator
         )
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """self == other"""
+        if not isinstance(other, JustInterval):
+            return False
         return self._richcmp(other, operator.eq)
 
-    def __lt__(self, other):
+    def __lt__(self, other: JustInterval) -> bool:
         """self < other"""
         return self._richcmp(other, operator.lt)
 
-    def __gt__(self, other):
+    def __gt__(self, other: JustInterval) -> bool:
         """self > other"""
         return self._richcmp(other, operator.gt)
 
-    def __le__(self, other):
+    def __le__(self, other: JustInterval) -> bool:
         """self <= other"""
         return self._richcmp(other, operator.le)
 
-    def __ge__(self, other):
+    def __ge__(self, other: JustInterval) -> bool:
         """self >= other"""
         return self._richcmp(other, operator.ge)
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         """self != 0"""
         return self._numerator != 0
```

### Comparing `jintonic-0.0.1/jintonic/lattice.py` & `jintonic-0.2.3/src/jintonic/lattice.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,269 +1,275 @@
 """Implements the just intonation lattice."""
+from __future__ import annotations
 
-from .primes import is_prime, generate_primes
-from .intervals import JustInterval, primary_interval
+from typing import List
 
-__version__ = '0.0.1'
+from .intervals import JustInterval, primary_interval
+from .primes import generate_primes, is_prime
 
 
-class JustLattice():
+class JustLattice:
     """This class implements just intonation lattices."""
 
-    def __init__(self, fundamental=None, prime_limit=7):
+    def __init__(self, fundamental: float, prime_limit: int = 7):
         """Initializes a JustLattice.
 
-        :param prime_limit: The prime limit. A prime number.
-        :type prime_limit: int
-        :param fundamental: The 1/1 pitch in Hertz
-        :type fundamental: float
-
-        **Examples**
-
-        >>> JustLattice(60)
-        JustLattice(60.0 - 1/1 (60.0))
-        """
-        self._prime_limit = None
-        self.prime_limit = prime_limit
-
-        self._fundamental = None
-        self._pitch = None
-        self._cents = None
-        self._tone = JustInterval(1, 1)
-        self._node = (0, 0, 0)
-        self._path = [self._node]
-
-        if fundamental is not None:
-            self.fundamental = fundamental
+        Parameters:
+            prime_limit: The prime limit. A prime number.
+            fundamental: The 1/1 pitch in Hertz
+
+        Examples:
+            >>> JustLattice(60)
+            JustLattice(60.0 Hz, 1/1, 60.0 Hz)
+        """
+        self._fundamental: float = float(fundamental)
+        self._prime_limit: int = prime_limit
+
+        self._tone: JustInterval = JustInterval(1, 1)
+        self._node: List[int] = [0, 0, 0]
+        self._path: List[List[int]] = [self._node]
 
-    def traverse(self, *vector):
+    def traverse(self, vector: List[int]):
         """Traverses a just intonation lattice.
 
-        :param vector: Number of steps along each axis. Steps are assigned to
-            an axis based on position. The first argument is on the three-limit
-            axis, the second on the five-limit, third on the seven-limit,
-            etc. To stay in place on an axis, pass 0 for that axis.
-        :type arg: tuple of int
-
-        **Examples**
-
-        >>> lattice = JustLattice(60)
-        >>> lattice.traverse(1, 0, 0)
-        JustLattice(60.0 - 3/2 (90.0))
-        >>> lattice.traverse(-2, 0, 0)
-        JustLattice(60.0 - 4/3 (80.0))
-        >>> lattice.traverse(1, 1, 0)
-        JustLattice(60.0 - 5/4 (75.0))
-        >>> lattice.traverse(0, -2, 0)
-        JustLattice(60.0 - 8/5 (96.0))
-        >>> lattice.traverse(0, 1, 1)
-        JustLattice(60.0 - 7/4 (105.0))
-        >>> lattice.traverse(0, 0, -2)
-        JustLattice(60.0 - 8/7 (68.5714))
-        >>> lattice.traverse(2, 0, 1)
-        JustLattice(60.0 - 9/8 (67.5))
-        >>> lattice.traverse(-4, 0, 0)
-        JustLattice(60.0 - 16/9 (106.6667))
+        Parameters:
+            vector: Number of steps along each axis. Steps are assigned to
+                an axis based on position. The first argument is on the three-limit
+                axis, the second on the five-limit, third on the seven-limit,
+                etc. To stay in place on an axis, pass 0 for that axis.
+
+        Examples:
+            >>> lattice = JustLattice(60)
+            >>> lattice.traverse([1, 0, 0])
+            JustLattice(60.0 Hz, 3/2, 90.0 Hz)
+            >>> lattice.traverse([-2, 0, 0])
+            JustLattice(60.0 Hz, 4/3, 80.0 Hz)
+            >>> lattice.traverse([1, 1, 0])
+            JustLattice(60.0 Hz, 5/4, 75.0 Hz)
+            >>> lattice.traverse([0, -2, 0])
+            JustLattice(60.0 Hz, 8/5, 96.0 Hz)
+            >>> lattice.traverse([0, 1, 1])
+            JustLattice(60.0 Hz, 7/4, 105.0 Hz)
+            >>> lattice.traverse([0, 0, -2])
+            JustLattice(60.0 Hz, 8/7, 68.5714 Hz)
+            >>> lattice.traverse([2, 0, 1])
+            JustLattice(60.0 Hz, 9/8, 67.5 Hz)
+            >>> lattice.traverse([-4, 0, 0])
+            JustLattice(60.0 Hz, 16/9, 106.6667 Hz)
         """
         primary_intervals = [
-            primary_interval(prime)
-            for prime in generate_primes(self.prime_limit)[1:]
+            primary_interval(prime) for prime in generate_primes(self.prime_limit)[1:]
         ]
         if len(vector) > len(primary_intervals):
             return NotImplemented
 
         for axis, steps in enumerate(list(vector)):
-            interval = primary_intervals[axis]**abs(steps)
+            interval = primary_intervals[axis] ** abs(steps)
             if steps > 0:
                 self._tone += interval
             elif steps < 0:
                 self._tone -= interval
             else:
                 continue
 
         self._tone = self._tone.base_octave
         self._node = vector
         self._path.append(vector)
 
         return self
 
-    def undo(self, steps=1):
+    def undo(self, steps: int = 1):
         """Undo a traversal.
 
-        :param steps: Number of steps to undo
-        :type steps: int
+        Parameters:
+            steps: Number of steps to undo
 
-        **Examples**
-
-        >>> lattice = JustLattice(60)
-        >>> lattice.traverse(1, 0, 0)
-        JustLattice(60.0 - 3/2 (90.0))
-        >>> lattice.undo(1)
-        JustLattice(60.0 - 1/1 (60.0))
+        Examples:
+            >>> lattice = JustLattice(60)
+            >>> lattice.traverse([1, 0, 0])
+            JustLattice(60.0 Hz, 3/2, 90.0 Hz)
+            >>> lattice.undo(1)
+            JustLattice(60.0 Hz, 1/1, 60.0 Hz)
         """
         for _ in range(steps):
             vector = self._path.pop()
-            self.traverse(*(-1 * distance for distance in vector))
+            self.traverse([-1 * distance for distance in vector])
 
         return self
 
     def to_fundamental(self):
         """Return to 1/1 without losing path history.
 
-        **Examples**
-
-        >>> lattice = JustLattice(60)
-        >>> lattice.traverse(1, 0, 0)
-        JustLattice(60.0 - 3/2 (90.0))
-        >>> lattice.to_fundamental()
-        JustLattice(60.0 - 1/1 (60.0))
+        Examples:
+            >>> lattice = JustLattice(60)
+            >>> lattice.traverse([1, 0, 0])
+            JustLattice(60.0 Hz, 3/2, 90.0 Hz)
+            >>> lattice.to_fundamental()
+            JustLattice(60.0 Hz, 1/1, 60.0 Hz)
         """
         axes = len(self._node)
-        root_node = (0, ) * axes
+        root_node = [0] * axes
         self._node = root_node
         self._tone = JustInterval(1, 1)
         self._path.append(root_node)
         self._pitch = self._fundamental
 
         return self
 
     def reset_path(self):
         """Clear path history and return to 1/1."""
         self.to_fundamental()
         axes = len(self._node)
-        root_node = (0, ) * axes
-        self._path = root_node
+        root_node = [0] * axes
+        self._path = [root_node]
 
         return self
 
-    def to_node(self, *node):
+    def to_node(self, node: List[int]):
         """Traverse to a specific node.
 
-        **Examples**
-
-        >>> lattice = JustLattice(60)
-        >>> lattice.traverse(1, 0, 0)
-        JustLattice(60.0 - 3/2 (90.0))
-        >>> lattice.to_node(0, 0, 0)
-        JustLattice(60.0 - 1/1 (60.0))
+        Examples:
+            >>> lattice = JustLattice(60)
+            >>> lattice.traverse([1, 0, 0])
+            JustLattice(60.0 Hz, 3/2, 90.0 Hz)
+            >>> lattice.to_node([0, 0, 0])
+            JustLattice(60.0 Hz, 1/1, 60.0 Hz)
         """
         self.to_fundamental()
-        self.traverse(*node)
+        self.traverse(node)
 
         return self
 
     @property
-    def prime_limit(self):
+    def prime_limit(self) -> int:
         """The prime limit.
 
-        :param value: A prime number.
-        :type value: int
+        Returns:
+            The prime limit of the lattice
 
-        **Examples**
-
-        >>> JustLattice(60).prime_limit
-        7
+        Examples:
+            >>> JustLattice(60).prime_limit
+            7
         """
         return self._prime_limit
 
     @prime_limit.setter
-    def prime_limit(self, value):
-        """Sets the prime limit."""
+    def prime_limit(self, value: int):
+        """The prime limit.
+
+        Parameters:
+            value: A prime number.
+
+        Returns:
+            The prime limit of the lattice
+
+        Examples:
+            >>> JustLattice(60).prime_limit
+            7
+        """
         if not is_prime(value):
-            msg = 'Prime limit must be a prime number. '
+            msg = "Prime limit must be a prime number. "
             msg += "Got '{}'".format(value)
         self._prime_limit = value
 
     @property
-    def fundamental(self):
+    def fundamental(self) -> float:
         """Fundamental (1/1) pitch in Hertz.
 
-        :param value: Fundamental (1/1) pitch in Hertz
-        :type value: float
-
-        **Examples**
+        Returns:
+            The fundamental's frequency in Hertz
 
-        >>> JustLattice(60).fundamental
-        60.0
+        Examples:
+            >>> JustLattice(60.0).fundamental
+            60.0
         """
         return self._fundamental
 
     @fundamental.setter
-    def fundamental(self, value):
+    def fundamental(self, value: float):
         """Set the fundamental (1/1) pitch in Hertz."""
         try:
             self._fundamental = float(value)
             self._pitch = self._fundamental * self._tone
         except ValueError:
-            msg = "Fundamental must be numeric. Got '{}'.".format(
-                type(value))
+            msg = "Fundamental must be numeric. Got '{}'.".format(type(value))
             raise ValueError(msg)
 
     @property
-    def hertz(self):
+    def hertz(self) -> float:
         """Current node's pitch in Hertz.
 
-        **Examples**
+        Returns:
+            The current node's pitch in Hertz
 
-        >>> lattice = JustLattice(60)
-        >>> lattice.traverse(1, 0, 0).hertz
-        90.0
+        Examples:
+            >>> lattice = JustLattice(60)
+            >>> lattice.traverse([1, 0, 0]).hertz
+            90.0
         """
         return self._fundamental * self._tone
 
     @property
-    def cents(self):
+    def cents(self) -> float:
         """Current node's interval in Cents.
 
-        **Examples**
+        Returns:
+            The current node's interval in Cents
 
-        >>> lattice = JustLattice(60)
-        >>> round(lattice.traverse(1, 0, 0).cents, 3)
-        701.955
+        Examples:
+            >>> lattice = JustLattice(60)
+            >>> round(lattice.traverse([1, 0, 0]).cents, 3)
+            701.955
         """
         return self._tone.cents
 
     @property
-    def tone(self):
+    def tone(self) -> JustInterval:
         """Current node's tone.
 
-        **Examples**
+        Returns:
+            The current node's tone as a JustInterval
 
-        >>> lattice = JustLattice(60)
-        >>> lattice.traverse(1, 0, 0).tone
-        JustInterval(3, 2)
+        Examples:
+            >>> lattice = JustLattice(60)
+            >>> lattice.traverse([1, 0, 0]).tone
+            JustInterval(3, 2)
         """
         return self._tone
 
     @property
-    def node(self):
-        """Current node as a tuple with length equivalent to number of axes.
+    def node(self) -> List[int]:
+        """Current node as a vector with length equivalent to number of axes.
 
-        **Examples**
+        Returns:
+            The current node as a vector with length equivalent to number of axes
 
-        >>> lattice = JustLattice(60)
-        >>> lattice.traverse(0, 2, 3).node
-        (0, 2, 3)
+        Examples:
+            >>> lattice = JustLattice(60)
+            >>> lattice.traverse([0, 2, 3]).node
+            [0, 2, 3]
         """
         return self._node
 
     @property
-    def path(self):
+    def path(self) -> List[List[int]]:
         """Current traversal history.
 
-        **Examples**
+        Returns:
+            The traversal history across the lattice
 
-        >>> lattice = JustLattice(60)
-        >>> lattice.traverse(0, 2, 3).path
-        [(0, 0, 0), (0, 2, 3)]
+        Examples:
+            >>> lattice = JustLattice(60)
+            >>> lattice.traverse([0, 2, 3]).path
+            [[0, 0, 0], [0, 2, 3]]
         """
         return self._path
 
     def __repr__(self):
         """repr(self)"""
-        return '{}({} - {}/{} ({}))'.format(
+        return "{}({} Hz, {}/{}, {} Hz)".format(
             self.__class__.__name__,
             self.fundamental,
             self.tone.numerator,
             self.tone.denominator,
-            round(self.hertz, 4)
+            round(self.hertz, 4),
         )
```

