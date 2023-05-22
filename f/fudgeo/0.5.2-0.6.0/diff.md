# Comparing `tmp/fudgeo-0.5.2-py3-none-any.whl.zip` & `tmp/fudgeo-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 31166 bytes, number of entries: 20
--rw-r--r--  2.0 unx      117 b- defN 23-May-18 20:04 fudgeo/__init__.py
--rw-r--r--  2.0 unx     2852 b- defN 23-May-18 20:04 fudgeo/constant.py
+Zip file size: 35310 bytes, number of entries: 21
+-rw-r--r--  2.0 unx      117 b- defN 23-May-22 19:54 fudgeo/__init__.py
+-rw-r--r--  2.0 unx     2962 b- defN 23-May-22 19:54 fudgeo/constant.py
 -rw-r--r--  2.0 unx     1157 b- defN 23-Jan-04 21:53 fudgeo/enumeration.py
--rw-r--r--  2.0 unx    20081 b- defN 23-May-12 12:57 fudgeo/geopkg.py
--rw-r--r--  2.0 unx     2673 b- defN 23-May-06 22:48 fudgeo/geopkg.sql
--rw-r--r--  2.0 unx     7768 b- defN 23-May-06 22:48 fudgeo/sql.py
+-rw-r--r--  2.0 unx    24486 b- defN 23-May-22 19:54 fudgeo/geopkg.py
+-rw-r--r--  2.0 unx     4118 b- defN 23-May-22 19:54 fudgeo/geopkg.sql
+-rw-r--r--  2.0 unx     4772 b- defN 23-May-22 19:54 fudgeo/spatial.py
+-rw-r--r--  2.0 unx    12069 b- defN 23-May-22 19:54 fudgeo/sql.py
 -rw-r--r--  2.0 unx      974 b- defN 23-May-06 22:48 fudgeo/geometry/__init__.py
--rw-r--r--  2.0 unx     2042 b- defN 23-May-18 20:04 fudgeo/geometry/base.py
--rw-r--r--  2.0 unx     8392 b- defN 23-May-18 20:04 fudgeo/geometry/linestring.py
--rw-r--r--  2.0 unx     6742 b- defN 23-May-18 20:04 fudgeo/geometry/linestring.pyi
--rw-r--r--  2.0 unx    14895 b- defN 23-May-18 20:04 fudgeo/geometry/point.py
--rw-r--r--  2.0 unx     6425 b- defN 23-May-18 20:04 fudgeo/geometry/point.pyi
--rw-r--r--  2.0 unx    10787 b- defN 23-May-18 20:04 fudgeo/geometry/polygon.py
--rw-r--r--  2.0 unx     9350 b- defN 23-May-18 20:04 fudgeo/geometry/polygon.pyi
--rw-r--r--  2.0 unx    17249 b- defN 23-May-18 20:04 fudgeo/geometry/util.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    13095 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1575 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/RECORD
-20 files, 127361 bytes uncompressed, 28642 bytes compressed:  77.5%
+-rw-r--r--  2.0 unx     2042 b- defN 23-May-18 20:08 fudgeo/geometry/base.py
+-rw-r--r--  2.0 unx     8502 b- defN 23-May-22 19:54 fudgeo/geometry/linestring.py
+-rw-r--r--  2.0 unx     6742 b- defN 23-May-18 20:08 fudgeo/geometry/linestring.pyi
+-rw-r--r--  2.0 unx    14814 b- defN 23-May-22 19:54 fudgeo/geometry/point.py
+-rw-r--r--  2.0 unx     6409 b- defN 23-May-22 19:54 fudgeo/geometry/point.pyi
+-rw-r--r--  2.0 unx    10897 b- defN 23-May-22 19:54 fudgeo/geometry/polygon.py
+-rw-r--r--  2.0 unx     9350 b- defN 23-May-18 20:08 fudgeo/geometry/polygon.pyi
+-rw-r--r--  2.0 unx    17251 b- defN 23-May-22 19:54 fudgeo/geometry/util.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-22 21:22 fudgeo-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15166 b- defN 23-May-22 21:22 fudgeo-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 21:22 fudgeo-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-22 21:22 fudgeo-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1650 b- defN 23-May-22 21:22 fudgeo-0.6.0.dist-info/RECORD
+21 files, 144665 bytes uncompressed, 32676 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: fudgeo/geopkg.py
 Comment: 
 
 Filename: fudgeo/geopkg.sql
 Comment: 
 
+Filename: fudgeo/spatial.py
+Comment: 
+
 Filename: fudgeo/sql.py
 Comment: 
 
 Filename: fudgeo/geometry/__init__.py
 Comment: 
 
 Filename: fudgeo/geometry/base.py
@@ -39,23 +42,23 @@
 
 Filename: fudgeo/geometry/polygon.pyi
 Comment: 
 
 Filename: fudgeo/geometry/util.py
 Comment: 
 
-Filename: fudgeo-0.5.2.dist-info/LICENSE
+Filename: fudgeo-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: fudgeo-0.5.2.dist-info/METADATA
+Filename: fudgeo-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: fudgeo-0.5.2.dist-info/WHEEL
+Filename: fudgeo-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: fudgeo-0.5.2.dist-info/top_level.txt
+Filename: fudgeo-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fudgeo-0.5.2.dist-info/RECORD
+Filename: fudgeo-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fudgeo/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Package Initialization
 """
 
 
-__version__ = '0.5.2'
+__version__ = '0.6.0'
 
 
 if __name__ == '__main__':
     pass
```

## fudgeo/constant.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Constants
 """
 
 
 from struct import pack
-from typing import ClassVar, Dict, List, Tuple, Union
+from typing import ClassVar, Dict, List, Set, Tuple, Union
 
 
 DOUBLE = Tuple[float, float]
 TRIPLE = Tuple[float, float, float]
 QUADRUPLE = Tuple[float, float, float, float]
 COORDINATES = Union[List[DOUBLE], List[TRIPLE], List[QUADRUPLE]]
 
@@ -60,20 +60,22 @@
 
 WKB_MULTI_POLYGON_PRE: bytes = pack(BYTE_CODE, 1, 6)
 WKB_MULTI_POLYGON_Z_PRE: bytes = pack(BYTE_CODE, 1, 1006)
 WKB_MULTI_POLYGON_M_PRE: bytes = pack(BYTE_CODE, 1, 2006)
 WKB_MULTI_POLYGON_ZM_PRE: bytes = pack(BYTE_CODE, 1, 3006)
 
 
-POINT_PREFIX: Dict[Tuple[bool, bool], bytes] = {
+POINT_PREFIX_ZM: Dict[Tuple[bool, bool], bytes] = {
     (False, False): WKB_POINT_PRE,
     (True, False): WKB_POINT_Z_PRE,
     (False, True): WKB_POINT_M_PRE,
     (True, True): WKB_POINT_ZM_PRE,
 }
+POINT_PREFIXES: Set[bytes] = {
+    WKB_POINT_PRE, WKB_POINT_Z_PRE, WKB_POINT_M_PRE, WKB_POINT_ZM_PRE}
 
 
 class EnvelopeCode:
     """
     Envelope Code
     """
     empty: ClassVar[int] = 0
```

## fudgeo/geopkg.py

```diff
@@ -6,44 +6,52 @@
 
 from datetime import datetime, timedelta, timezone
 from math import nan
 from os import PathLike
 from pathlib import Path
 from re import IGNORECASE, compile as recompile
 from sqlite3 import (
-    Connection, Cursor, DatabaseError, OperationalError, PARSE_COLNAMES,
+    DatabaseError, IntegrityError, OperationalError, PARSE_COLNAMES,
     PARSE_DECLTYPES, connect, register_adapter, register_converter)
-from typing import Callable, Dict, List, Optional, Tuple, Type, Union
+from typing import (
+    Callable, Dict, List, Optional, TYPE_CHECKING, Tuple, Type, Union)
 
 from fudgeo.enumeration import (
     DataType, GPKGFlavors, GeometryType, SQLFieldType)
 from fudgeo.geometry import (
     Point, PointZ, PointM, PointZM, MultiPoint, MultiPointZ, MultiPointM,
     MultiPointZM, LineString, LineStringZ, LineStringM, LineStringZM,
     MultiLineString, MultiLineStringZ, MultiLineStringM, MultiLineStringZM,
     Polygon, PolygonZ, PolygonM, PolygonZM, MultiPolygon, MultiPolygonZ,
     MultiPolygonM, MultiPolygonZM)
+from fudgeo.spatial import ST_FUNCS
 from fudgeo.sql import (
     CHECK_SRS_EXISTS, CREATE_FEATURE_TABLE, CREATE_OGR_CONTENTS, CREATE_TABLE,
     DEFAULT_EPSG_RECS, DEFAULT_ESRI_RECS, DELETE_OGR_CONTENTS,
     GPKG_OGR_CONTENTS_DELETE_TRIGGER, GPKG_OGR_CONTENTS_INSERT_TRIGGER,
     HAS_OGR_CONTENTS, INSERT_GPKG_CONTENTS_SHORT, INSERT_GPKG_GEOM_COL,
     INSERT_GPKG_OGR_CONTENTS, INSERT_GPKG_SRS, KEYWORDS, REMOVE_FEATURE_CLASS,
     REMOVE_TABLE, SELECT_EXTENT, SELECT_GEOMETRY_COLUMN, SELECT_GEOMETRY_TYPE,
-    SELECT_HAS_ZM, SELECT_SRS, SELECT_TABLES_BY_TYPE, TABLE_EXISTS,
-    UPDATE_EXTENT)
+    SELECT_HAS_ZM, SELECT_SRS, SELECT_TABLES_BY_TYPE,
+    SPATIAL_INDEX_CREATE_TABLE, SPATIAL_INDEX_EXTENSION, SPATIAL_INDEX_INSERT,
+    SPATIAL_INDEX_RECORD, SPATIAL_INDEX_TRIGGERS, TABLE_EXISTS, UPDATE_EXTENT)
+
+
+if TYPE_CHECKING:
+    from sqlite3 import Connection, Cursor
+    from fudgeo.geometry.base import AbstractGeometry
 
 
 FIELDS = Union[Tuple['Field', ...], List['Field']]
 NAME_MATCHER: Callable = recompile(r'^[A-Z]\w*$', IGNORECASE).match
 
 
-COMMA_SPACE = ', '
-GPKG_EXT = '.gpkg'
-SHAPE = 'SHAPE'
+COMMA_SPACE: str = ', '
+GPKG_EXT: str = '.gpkg'
+SHAPE: str = 'SHAPE'
 
 
 def _escape_name(name: str) -> str:
     """
     Escape Name
     """
     if name.upper() in KEYWORDS or not NAME_MATCHER(name):
@@ -56,15 +64,15 @@
     """
     Formatted Now
     """
     return datetime.now().strftime('%Y-%m-%dT%H:%M:%S.%fZ')
 # End _now method
 
 
-def _adapt_geometry(val) -> bytes:
+def _adapt_geometry(val: 'AbstractGeometry') -> bytes:
     """
     Adapt Geometry to Geopackage
     """
     return val.to_gpkg()
 # End _adapt_geometry function
 
 
@@ -72,15 +80,15 @@
     """
     Heavily Influenced by convert_timestamp from ../sqlite3/dbapi2.py,
     Added in support for timezone handling although the practice should
     be to resolve to UTC.
     """
     colon = b':'
     dash = b'-'
-    # To split timestamps like that b'2022-09-06T13:50:33'
+    # NOTE To split timestamps like that b'2022-09-06T13:50:33'
     for separator in (b' ', b'T'):
         try:
             dt, tm = val.split(separator)
             break
         except ValueError:
             pass
     else:
@@ -107,15 +115,15 @@
     else:
         tzinfo = None
     return datetime(year, month, day, hours, minutes, seconds,
                     micro, tzinfo=tzinfo)
 # End _convert_datetime function
 
 
-def _register_geometry():
+def _register_geometry() -> None:
     """
     Register adapters and converters for geometry / geopackage
     """
     classes = (
         Point, PointZ, PointM, PointZM, MultiPoint, MultiPointZ, MultiPointM,
         MultiPointZM, LineString, LineStringZ, LineStringM, LineStringZM,
         MultiLineString, MultiLineStringZ, MultiLineStringM, MultiLineStringZM,
@@ -123,25 +131,34 @@
         MultiPolygonM, MultiPolygonZM)
     for cls in classes:
         register_adapter(cls, _adapt_geometry)
         register_converter(cls.__name__, cls.from_gpkg)
 # End _register_geometry function
 
 
+def _add_st_functions(conn: 'Connection') -> None:
+    """
+    Add ST Functions
+    """
+    for name, func in ST_FUNCS.items():
+        conn.create_function(name=name, narg=1, func=func)
+# End _add_st_functions function
+
+
 class GeoPackage:
     """
     GeoPackage
     """
     def __init__(self, path: Union[PathLike, str]) -> None:
         """
         Initialize the GeoPackage class
         """
         super().__init__()
         self._path: Path = Path(path)
-        self._conn: Optional[Connection] = None
+        self._conn: Optional['Connection'] = None
     # End init built-in
 
     def __repr__(self) -> str:
         """
         String Representation
         """
         return f'GeoPackage(path={self._path!r})'
@@ -152,32 +169,33 @@
         """
         Path
         """
         return self._path
     # End path property
 
     @property
-    def connection(self) -> Connection:
+    def connection(self) -> 'Connection':
         """
         Connection
         """
         if self._conn is None:
             self._conn = connect(
                 str(self._path), isolation_level='EXCLUSIVE',
                 detect_types=PARSE_DECLTYPES | PARSE_COLNAMES)
             _register_geometry()
+            _add_st_functions(self._conn)
             register_converter('timestamp', _convert_datetime)
             register_converter('datetime', _convert_datetime)
         return self._conn
     # End connection property
 
     @classmethod
     def create(cls, path: Union[PathLike, str],
                flavor: str = GPKGFlavors.esri,
-               ogr_contents: bool = True) -> 'GeoPackage':
+               ogr_contents: bool = False) -> 'GeoPackage':
         """
         Create a new GeoPackage
         """
         path = Path(path).with_suffix(GPKG_EXT)
         if path.is_file():
             raise ValueError(f'GeoPackage already exists: {path}')
         if not path.parent.is_dir():
@@ -224,23 +242,25 @@
         return fields
     # End _validate_inputs method
 
     def create_feature_class(self, name: str, srs: 'SpatialReferenceSystem',
                              shape_type: str = GeometryType.point,
                              z_enabled: bool = False, m_enabled: bool = False,
                              fields: FIELDS = (), description: str = '',
-                             overwrite: bool = False) -> 'FeatureClass':
+                             overwrite: bool = False,
+                             spatial_index: bool = False) -> 'FeatureClass':
         """
         Creates a feature class in the GeoPackage per the options given.
         """
         fields = self._validate_inputs(fields, name, overwrite)
         return FeatureClass.create(
             geopackage=self, name=name, shape_type=shape_type, srs=srs,
             z_enabled=z_enabled, m_enabled=m_enabled, fields=fields,
-            description=description, overwrite=overwrite)
+            description=description, overwrite=overwrite,
+            spatial_index=spatial_index)
     # End create_feature_class method
 
     def create_table(self, name: str, fields: FIELDS = (),
                      description: str = '', overwrite: bool = False) -> 'Table':
         """
         Creates a feature class in the GeoPackage per the options given.
         """
@@ -289,23 +309,71 @@
         Initialize the BaseTable class
         """
         super().__init__()
         self.geopackage: GeoPackage = geopackage
         self.name: str = name
     # End init built-in
 
+    @staticmethod
+    def _column_names(fields: FIELDS) -> str:
+        """
+        Column Names
+        """
+        if not fields:
+            return ''
+        return f'{COMMA_SPACE}{COMMA_SPACE.join(repr(f) for f in fields)}'
+    # End _column_names method
+
+    @staticmethod
+    def _drop(conn: 'Connection', sql: str, name: str, escaped_name: str,
+              geom_name: str, has_ogr_contents: bool) -> None:
+        """
+        Drop Table from Geopackage
+        """
+        conn.executescript(sql.format(name, escaped_name, geom_name))
+        if has_ogr_contents:
+            conn.execute(DELETE_OGR_CONTENTS.format(name))
+    # End _drop method
+
+    @property
+    def count(self) -> int:
+        """
+        Number of records
+        """
+        cursor = self.geopackage.connection.execute(
+            f"""SELECT COUNT(1) AS C FROM {self.escaped_name}""")
+        count, = cursor.fetchone()
+        return count
+    # End count property
+
     @property
     def escaped_name(self) -> str:
         """
         Escaped Name
         """
         return _escape_name(self.name)
     # End escaped_name property
 
     @property
+    def primary_key_field(self) -> Optional['Field']:
+        """
+        Primary Key Field
+        """
+        cursor = self.geopackage.connection.execute(f"""
+            SELECT name, type
+            FROM pragma_table_info('{self.name}')
+            WHERE upper(type) = '{SQLFieldType.integer}' AND 
+                  "notnull" = 1 AND pk = 1""")
+        result = cursor.fetchone()
+        if not result:
+            return
+        return Field(*result)
+    # End primary_key_field property
+
+    @property
     def fields(self) -> List['Field']:
         """
         Fields
         """
         cursor = self.geopackage.connection.execute(
             f"""PRAGMA table_info({self.escaped_name})""")
         return [Field(name=name, data_type=type_)
@@ -335,40 +403,39 @@
 
     @classmethod
     def create(cls, geopackage: GeoPackage, name: str, fields: FIELDS,
                description: str = '', overwrite: bool = False) -> 'Table':
         """
         Create a regular non-spatial table in the geopackage
         """
-        cols = f', {", ".join(repr(f) for f in fields)}' if fields else ''
+        cols = cls._column_names(fields)
         with geopackage.connection as conn:
             escaped_name = _escape_name(name)
             has_ogr_contents = _has_ogr_contents(conn)
             if overwrite:
-                conn.executescript(REMOVE_TABLE.format(name, escaped_name))
-                if has_ogr_contents:
-                    conn.execute(DELETE_OGR_CONTENTS.format(name))
+                cls._drop(conn=conn, sql=REMOVE_TABLE, geom_name='',
+                          name=name, escaped_name=escaped_name,
+                          has_ogr_contents=has_ogr_contents)
             conn.execute(CREATE_TABLE.format(
                 name=escaped_name, other_fields=cols))
             conn.execute(INSERT_GPKG_CONTENTS_SHORT, (
                 name, DataType.attributes, name, description, _now(), None))
             if has_ogr_contents:
                 _add_ogr_contents(conn, name=name, escaped_name=escaped_name)
         return cls(geopackage=geopackage, name=name)
     # End create method
 
     def drop(self) -> None:
         """
         Drop table from Geopackage
         """
         with self.geopackage.connection as conn:
-            conn.executescript(
-                REMOVE_TABLE.format(self.name, self.escaped_name))
-            if _has_ogr_contents(conn):
-                conn.execute(DELETE_OGR_CONTENTS.format(self.name))
+            self._drop(conn=conn, sql=REMOVE_TABLE, geom_name='',
+                       name=self.name, escaped_name=self.escaped_name,
+                       has_ogr_contents=_has_ogr_contents(conn))
     # End drop method
 # End Table class
 
 
 class FeatureClass(BaseTable):
     """
     GeoPackage Feature Class
@@ -377,59 +444,87 @@
         """
         String Representation
         """
         return (f'FeatureClass(geopackage={self.geopackage!r}, '
                 f'name={self.name!r})')
     # End repr built-in
 
+    @staticmethod
+    def _find_geometry_column_name(geopackage: 'GeoPackage', name: str) -> str:
+        """
+        Find Geometry Column Name for an Existing Feature Class
+        """
+        sans_case = {k.casefold(): v
+                     for k, v in geopackage.feature_classes.items()}
+        existing = sans_case.get(name.casefold())
+        if not existing:
+            return ''
+        return existing.geometry_column_name
+    # End _find_geometry_column_name method
+
+    def add_spatial_index(self) -> bool:
+        """
+        Add Spatial Index if does not already exist
+        """
+        if self.has_spatial_index:
+            return False
+        with self.geopackage.connection as conn:
+            _add_spatial_index(conn=conn, feature_class=self)
+        return True
+    # End add_spatial_index method
+
     @classmethod
     def create(cls, geopackage: GeoPackage, name: str, shape_type: str,
                srs: 'SpatialReferenceSystem', z_enabled: bool = False,
                m_enabled: bool = False, fields: FIELDS = (),
-               description: str = '',
-               overwrite: bool = False) -> 'FeatureClass':
+               description: str = '', overwrite: bool = False,
+               spatial_index: bool = False) -> 'FeatureClass':
         """
         Create Feature Class
         """
-        cols = f', {", ".join(repr(f) for f in fields)}' if fields else ''
+        cols = cls._column_names(fields)
         with geopackage.connection as conn:
             escaped_name = _escape_name(name)
             has_ogr_contents = _has_ogr_contents(conn)
             if overwrite:
-                conn.executescript(
-                    REMOVE_FEATURE_CLASS.format(name, escaped_name))
-                if has_ogr_contents:
-                    conn.execute(DELETE_OGR_CONTENTS.format(name))
+                geom_name = cls._find_geometry_column_name(geopackage, name)
+                cls._drop(conn=conn, sql=REMOVE_FEATURE_CLASS,
+                          name=name, escaped_name=escaped_name,
+                          geom_name=geom_name,
+                          has_ogr_contents=has_ogr_contents)
             conn.execute(CREATE_FEATURE_TABLE.format(
                 name=escaped_name, feature_type=shape_type, other_fields=cols))
             if not geopackage.check_srs_exists(srs.srs_id):
                 conn.execute(INSERT_GPKG_SRS, srs.as_record())
             conn.execute(INSERT_GPKG_GEOM_COL,
                          (name, SHAPE, shape_type, srs.srs_id,
                           int(z_enabled), int(m_enabled)))
             conn.execute(INSERT_GPKG_CONTENTS_SHORT, (
                 name, DataType.features, name, description, _now(), srs.srs_id))
             if has_ogr_contents:
                 _add_ogr_contents(conn, name=name, escaped_name=escaped_name)
-        return cls(geopackage=geopackage, name=name)
+            feature_class = cls(geopackage=geopackage, name=name)
+            if spatial_index:
+                _add_spatial_index(conn=conn, feature_class=feature_class)
+        return feature_class
     # End create method
 
     def drop(self) -> None:
         """
         Drop feature class from Geopackage
         """
         with self.geopackage.connection as conn:
-            conn.executescript(
-                REMOVE_FEATURE_CLASS.format(self.name, self.escaped_name))
-            if _has_ogr_contents(conn):
-                conn.execute(DELETE_OGR_CONTENTS.format(self.name))
+            self._drop(conn=conn, sql=REMOVE_FEATURE_CLASS,
+                       geom_name=self.geometry_column_name,
+                       name=self.name, escaped_name=self.escaped_name,
+                       has_ogr_contents=_has_ogr_contents(conn))
     # End drop method
 
     @staticmethod
-    def _check_result(cursor: Cursor) -> Optional[str]:
+    def _check_result(cursor: 'Cursor') -> Optional[str]:
         """
         Check Result
         """
         result = cursor.fetchone()
         if not result:
             return
         if None in result:
@@ -486,14 +581,24 @@
         cursor = self.geopackage.connection.execute(
             SELECT_HAS_ZM, (self.name,))
         _, m = cursor.fetchone()
         return bool(m)
     # End has_m property
 
     @property
+    def has_spatial_index(self) -> bool:
+        """
+        Has Spatial Index
+        """
+        table_name = f'rtree_{self.name}_{self.geometry_column_name}'
+        cursor = self.geopackage.connection.execute(TABLE_EXISTS, (table_name,))
+        return bool(cursor.fetchall())
+    # End has_spatial_index property
+
+    @property
     def extent(self) -> Tuple[float, float, float, float]:
         """
         Extent property
         """
         empty = nan, nan, nan, nan
         cursor = self.geopackage.connection.execute(SELECT_EXTENT, (self.name,))
         result = cursor.fetchone()
@@ -599,19 +704,40 @@
         cursor = conn.execute(HAS_OGR_CONTENTS)
     except (DatabaseError, OperationalError):
         return False
     return bool(cursor.fetchone())
 # End _has_ogr_contents function
 
 
-def _add_ogr_contents(conn: Connection, name: str, escaped_name: str) -> None:
+def _add_ogr_contents(conn: 'Connection', name: str, escaped_name: str) -> None:
     """
     Add OGR Contents Table Entry and Triggers
     """
     conn.execute(INSERT_GPKG_OGR_CONTENTS, (name, 0))
     conn.execute(GPKG_OGR_CONTENTS_INSERT_TRIGGER.format(name, escaped_name))
     conn.execute(GPKG_OGR_CONTENTS_DELETE_TRIGGER.format(name, escaped_name))
 # End _add_ogr_contents function
 
 
+def _add_spatial_index(conn: 'Connection', feature_class: FeatureClass) -> None:
+    """
+    Add Spatial Index Table, Table Entry, and Triggers.  Load Spatial Index
+    Table if Feature Class has features.
+    """
+    name = feature_class.name
+    geom_name = feature_class.geometry_column_name
+    pk_name = feature_class.primary_key_field.escaped_name
+    record = name, geom_name, *SPATIAL_INDEX_RECORD
+    conn.execute(SPATIAL_INDEX_CREATE_TABLE.format(name, geom_name))
+    conn.executescript(SPATIAL_INDEX_TRIGGERS.format(name, geom_name, pk_name))
+    try:
+        conn.execute(SPATIAL_INDEX_EXTENSION, record)
+    except IntegrityError:
+        pass
+    if not feature_class.count:
+        return
+    conn.execute(SPATIAL_INDEX_INSERT.format(name, geom_name, pk_name))
+# End _add_spatial_index function
+
+
 if __name__ == '__main__':
     pass
```

## fudgeo/geopkg.sql

```diff
@@ -1,80 +1,131 @@
-PRAGMA application_id=0x47504b47;
-PRAGMA user_version=10300;
+PRAGMA application_id=0x47504B47;
+PRAGMA user_version=10301;
 
+-- TABLES
 
 CREATE TABLE gpkg_spatial_ref_sys (
     srs_name                 TEXT    NOT NULL,
     srs_id                   INTEGER NOT NULL PRIMARY KEY,
     organization             TEXT    NOT NULL,
     organization_coordsys_id INTEGER NOT NULL,
     definition               TEXT    NOT NULL,
     description              TEXT
 );
 
+
 CREATE TABLE gpkg_contents (
     table_name  TEXT     NOT NULL PRIMARY KEY,
     data_type   TEXT     NOT NULL,
     identifier  TEXT UNIQUE,
     description TEXT              DEFAULT '',
     last_change DATETIME NOT NULL DEFAULT (strftime('%Y-%m-%dT%H:%M:%S.%fZ', 'now')),
     min_x       DOUBLE,
     min_y       DOUBLE,
     max_x       DOUBLE,
     max_y       DOUBLE,
     srs_id      INTEGER,
     CONSTRAINT fk_gc_r_srs_id
-        FOREIGN KEY (srs_id) REFERENCES gpkg_spatial_ref_sys(srs_id)
+        FOREIGN KEY (srs_id) REFERENCES gpkg_spatial_ref_sys (srs_id)
 );
 
 
 CREATE TABLE gpkg_geometry_columns (
     table_name         TEXT    NOT NULL,
     column_name        TEXT    NOT NULL,
     geometry_type_name TEXT    NOT NULL,
     srs_id             INTEGER NOT NULL,
     z                  TINYINT NOT NULL,
     m                  TINYINT NOT NULL,
     CONSTRAINT pk_geom_cols PRIMARY KEY (table_name, column_name),
     CONSTRAINT uk_gc_table_name UNIQUE (table_name),
     CONSTRAINT fk_gc_tn FOREIGN KEY (table_name)
-        REFERENCES gpkg_contents(table_name),
+        REFERENCES gpkg_contents (table_name),
     CONSTRAINT fk_gc_srs FOREIGN KEY (srs_id)
-        REFERENCES gpkg_spatial_ref_sys(srs_id)
+        REFERENCES gpkg_spatial_ref_sys (srs_id)
 );
 
 
 CREATE TABLE gpkg_tile_matrix_set (
     table_name TEXT    NOT NULL PRIMARY KEY,
     srs_id     INTEGER NOT NULL,
     min_x      DOUBLE  NOT NULL,
     min_y      DOUBLE  NOT NULL,
     max_x      DOUBLE  NOT NULL,
     max_y      DOUBLE  NOT NULL,
     CONSTRAINT fk_gtms_table_name FOREIGN KEY (table_name)
-        REFERENCES gpkg_contents(table_name),
+        REFERENCES gpkg_contents (table_name),
     CONSTRAINT fk_gtms_srs FOREIGN KEY (srs_id)
-        REFERENCES gpkg_spatial_ref_sys(srs_id)
+        REFERENCES gpkg_spatial_ref_sys (srs_id)
 );
 
+
 CREATE TABLE gpkg_tile_matrix (
     table_name    TEXT    NOT NULL,
     zoom_level    INTEGER NOT NULL,
     matrix_width  INTEGER NOT NULL,
     matrix_height INTEGER NOT NULL,
     tile_width    INTEGER NOT NULL,
     tile_height   INTEGER NOT NULL,
     pixel_x_size  DOUBLE  NOT NULL,
     pixel_y_size  DOUBLE  NOT NULL,
     CONSTRAINT pk_ttm PRIMARY KEY (table_name, zoom_level),
     CONSTRAINT fk_tmm_table_name FOREIGN KEY (table_name)
-        REFERENCES gpkg_contents(table_name)
+        REFERENCES gpkg_contents (table_name)
 );
 
+
 CREATE TABLE gpkg_extensions (
     table_name     TEXT,
     column_name    TEXT,
     extension_name TEXT NOT NULL,
     definition     TEXT NOT NULL,
     scope          TEXT NOT NULL,
     CONSTRAINT ge_tce UNIQUE (table_name, column_name, extension_name)
 );
+
+-- VIEWS
+
+CREATE VIEW st_spatial_ref_sys AS
+SELECT srs_name,
+       srs_id,
+       organization,
+       organization_coordsys_id,
+       definition,
+       description
+FROM gpkg_spatial_ref_sys;
+
+
+CREATE VIEW spatial_ref_sys AS
+SELECT srs_id                   AS srid,
+       organization             AS auth_name,
+       organization_coordsys_id AS auth_srid,
+       definition               AS srtext
+FROM gpkg_spatial_ref_sys;
+
+
+CREATE VIEW st_geometry_columns AS
+SELECT table_name,
+       column_name,
+       'ST_' || geometry_type_name AS geometry_type_name,
+       g.srs_id,
+       srs_name
+FROM gpkg_geometry_columns as g
+         JOIN gpkg_spatial_ref_sys AS s
+WHERE g.srs_id = s.srs_id;
+
+
+CREATE VIEW geometry_columns AS
+SELECT table_name                                      AS f_table_name,
+       column_name                                     AS f_geometry_column,
+       case geometry_type_name
+           WHEN 'POINT' THEN 1
+           WHEN 'LINESTRING' THEN 2
+           WHEN 'POLYGON' THEN 3
+           WHEN 'MULTIPOINT' THEN 4
+           WHEN 'MULTILINESTRING' THEN 5
+           WHEN 'MULTIPOLYGON' THEN 6
+           ELSE 0 END                                  AS geometry_type,
+       2 + (CASE z WHEN 1 THEN 1 WHEN 2 THEN 1 ELSE 0 END) +
+       (CASE m WHEN 1 THEN 1 WHEN 2 THEN 1 ELSE 0 END) AS coord_dimension,
+       srs_id                                          AS srid
+FROM gpkg_geometry_columns;
```

## fudgeo/sql.py

```diff
@@ -57,41 +57,54 @@
 
 
 DELETE_OGR_CONTENTS: str = """
     DELETE FROM gpkg_ogr_contents WHERE lower(table_name) = lower('{0}');
 """
 
 
+# NOTE 0 - table name, 1 - escaped name, 2 - geometry column name
 REMOVE_FEATURE_CLASS: str = """
     DELETE FROM gpkg_contents WHERE lower(table_name) = lower('{0}');
     DELETE FROM gpkg_geometry_columns WHERE lower(table_name) = lower('{0}');
-    DROP TRIGGER IF EXISTS trigger_insert_feature_count_{0};
-    DROP TRIGGER IF EXISTS trigger_delete_feature_count_{0};
+    DELETE FROM gpkg_extensions 
+    WHERE lower(table_name) = lower('{0}') AND 
+          lower(extension_name) = 'gpkg_rtree_index';
+    DROP TRIGGER IF EXISTS "trigger_insert_feature_count_{0}";
+    DROP TRIGGER IF EXISTS "trigger_delete_feature_count_{0}";
+    DROP TRIGGER IF EXISTS "rtree_{0}_{2}_insert";
+    DROP TRIGGER IF EXISTS "rtree_{0}_{2}_update1";
+    DROP TRIGGER IF EXISTS "rtree_{0}_{2}_update2";
+    DROP TRIGGER IF EXISTS "rtree_{0}_{2}_update3";
+    DROP TRIGGER IF EXISTS "rtree_{0}_{2}_update4";
     DROP TABLE IF EXISTS {1};
+    DROP TABLE IF EXISTS "rtree_{0}_{2}";
 """
 
 
+# NOTE 0 - name, 1 - escaped name
 REMOVE_TABLE: str = """
     DELETE FROM gpkg_contents WHERE lower(table_name) = lower('{0}');
-    DROP TRIGGER IF EXISTS trigger_insert_feature_count_{0};
-    DROP TRIGGER IF EXISTS trigger_delete_feature_count_{0};
+    DROP TRIGGER IF EXISTS "trigger_insert_feature_count_{0}";
+    DROP TRIGGER IF EXISTS "trigger_delete_feature_count_{0}";
     DROP TABLE IF EXISTS {1};
 """
 
 
+# NOTE 0 - name, 1 - escaped name
 GPKG_OGR_CONTENTS_INSERT_TRIGGER: str = """
-    CREATE TRIGGER trigger_insert_feature_count_{0}
+    CREATE TRIGGER "trigger_insert_feature_count_{0}"
     AFTER INSERT ON {1}
     BEGIN UPDATE gpkg_ogr_contents SET feature_count = feature_count + 1 
           WHERE lower(table_name) = lower('{0}'); END;
 """
 
 
+# NOTE 0 - name, 1 - escaped name
 GPKG_OGR_CONTENTS_DELETE_TRIGGER: str = """
-    CREATE TRIGGER trigger_delete_feature_count_{0}
+    CREATE TRIGGER "trigger_delete_feature_count_{0}"
     AFTER DELETE ON {1}
     BEGIN UPDATE gpkg_ogr_contents SET feature_count = feature_count - 1 
           WHERE lower(table_name) = lower('{0}'); END;
 """
 
 
 INSERT_GPKG_GEOM_COL: str = """
@@ -161,15 +174,15 @@
     SELECT column_name
     FROM gpkg_geometry_columns
     WHERE lower(table_name) = lower(?)
 """
 
 
 SELECT_GEOMETRY_TYPE: str = """
-    SELECT GEOM || Z || M
+    SELECT GEOM || Z || M AS GT
     FROM (SELECT CASE
                      WHEN geometry_type_name == 'POINT'
                          THEN 'Point'
                      WHEN geometry_type_name == 'LINESTRING'
                          THEN 'LineString'
                      WHEN geometry_type_name == 'POLYGON'
                          THEN 'Polygon'
@@ -207,28 +220,135 @@
 SELECT_EXTENT: str = """
     SELECT min_x, min_y, max_x, max_y
     FROM gpkg_contents
     WHERE lower(table_name) = lower(?)
 """
 
 
-SELECT_TABLES_BY_TYPE: str = (
-    """SELECT table_name FROM gpkg_contents WHERE data_type = ?""")
+SELECT_TABLES_BY_TYPE: str = """
+    SELECT table_name 
+    FROM gpkg_contents 
+    WHERE data_type = ?
+"""
 
 
 DEFAULT_SRS_RECS: Tuple[Tuple[str, int, str, int, str, str], ...] = (
     ('Undefined Cartesian SRS', -1, 'NONE', -1, 'undefined',
      'undefined cartesian coordinate reference system'),
     ('Undefined Geographic SRS', 0, 'NONE', 0, 'undefined',
      'undefined geographic coordinate reference system'))
 
+
 EPSG_4326: str = """GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563,AUTHORITY["EPSG","7030"]],AUTHORITY["EPSG","6326"]],PRIMEM["Greenwich",0,AUTHORITY["EPSG","8901"]],UNIT["degree",0.01745329251994328,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]]"""
 ESRI_4326: str = """GEOGCS["GCS_WGS_1984",DATUM["D_WGS_1984",SPHEROID["WGS_1984",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["Degree",0.017453292519943295]]"""
 
+
 DEFAULT_EPSG_RECS: Tuple[Tuple[str, int, str, int, str, str], ...] = (
         DEFAULT_SRS_RECS + (('WGS 84', 4326, 'EPSG', 4326, EPSG_4326, ''),))
 DEFAULT_ESRI_RECS: Tuple[Tuple[str, int, str, int, str, str], ...] = (
         DEFAULT_SRS_RECS + (('GCS_WGS_1984', 4326, 'EPSG', 4326, ESRI_4326, ''),))
 
 
+# NOTE 0 - table name, 1 - geometry column name, 2 - primary key column name
+SPATIAL_INDEX_CREATE_TABLE: str = """
+    CREATE VIRTUAL TABLE "rtree_{0}_{1}" 
+    USING rtree(id, minx, maxx, miny, maxy)
+"""
+
+
+# NOTE 0 - table name, 1 - geometry column name, 2 - primary key column name
+SPATIAL_INDEX_INSERT: str = """
+    INSERT OR REPLACE INTO "rtree_{0}_{1}"
+        SELECT {2}, ST_MinX("{1}"), ST_MaxX("{1}"), ST_MinY("{1}"), ST_MaxY("{1}") 
+        FROM "{0}" WHERE "{1}" NOT NULL AND NOT ST_IsEmpty("{1}");
+"""
+
+
+# NOTE 0 - table name, 1 - geometry column name, 2 - primary key column name
+SPATIAL_INDEX_TRIGGERS: str = """
+    /* Conditions: Insertion of non-empty geometry
+       Actions   : Insert record into rtree */
+    CREATE TRIGGER "rtree_{0}_{1}_insert" AFTER INSERT ON "{0}"
+      WHEN (NEW."{1}" NOT NULL AND NOT ST_IsEmpty(NEW."{1}"))
+    BEGIN
+      INSERT OR REPLACE INTO "rtree_{0}_{1}" VALUES (
+        NEW."{2}",
+        ST_MinX(NEW."{1}"), ST_MaxX(NEW."{1}"),
+        ST_MinY(NEW."{1}"), ST_MaxY(NEW."{1}")
+      );
+    END;
+    
+    /* Conditions: Update of geometry column to non-empty geometry
+                   No row ID change
+       Actions   : Update record in rtree */
+    CREATE TRIGGER "rtree_{0}_{1}_update1" AFTER UPDATE OF "{1}" ON "{0}"
+      WHEN OLD."{2}" = NEW."{2}" AND
+           (NEW."{1}" NOTNULL AND NOT ST_IsEmpty(NEW."{1}"))
+    BEGIN
+      INSERT OR REPLACE INTO "rtree_{0}_{1}" VALUES (
+        NEW."{2}",
+        ST_MinX(NEW."{1}"), ST_MaxX(NEW."{1}"),
+        ST_MinY(NEW."{1}"), ST_MaxY(NEW."{1}")
+      );
+    END;
+    
+    /* Conditions: Update of geometry column to empty geometry
+                   No row ID change
+       Actions   : Remove record from rtree */
+    CREATE TRIGGER "rtree_{0}_{1}_update2" AFTER UPDATE OF "{1}" ON "{0}"
+      WHEN OLD."{2}" = NEW."{2}" AND
+           (NEW."{1}" ISNULL OR ST_IsEmpty(NEW."{1}"))
+    BEGIN
+      DELETE FROM "rtree_{0}_{1}" WHERE id = OLD."{2}";
+    END;
+    
+    /* Conditions: Update of any column
+                   Row ID change
+                   Non-empty geometry
+       Actions   : Remove record from rtree for old identifier
+                   Insert record into rtree for new identifier */
+    CREATE TRIGGER "rtree_{0}_{1}_update3" AFTER UPDATE ON "{0}"
+      WHEN OLD."{2}" != NEW."{2}" AND
+           (NEW."{1}" NOTNULL AND NOT ST_IsEmpty(NEW."{1}"))
+    BEGIN
+      DELETE FROM "rtree_{0}_{1}" WHERE id = OLD."{2}";
+      INSERT OR REPLACE INTO "rtree_{0}_{1}" VALUES (
+        NEW."{2}",
+        ST_MinX(NEW."{1}"), ST_MaxX(NEW."{1}"),
+        ST_MinY(NEW."{1}"), ST_MaxY(NEW."{1}")
+      );
+    END;
+    
+    /* Conditions: Update of any column
+                   Row ID change
+                   Empty geometry
+       Actions   : Remove record from rtree for old and new identifier */
+    CREATE TRIGGER "rtree_{0}_{1}_update4" AFTER UPDATE ON "{0}"
+      WHEN OLD."{2}" != NEW."{2}" AND
+           (NEW."{1}" ISNULL OR ST_IsEmpty(NEW."{1}"))
+    BEGIN
+      DELETE FROM "rtree_{0}_{1}" WHERE id IN (OLD."{2}", NEW."{2}");
+    END;
+    
+    /* Conditions: Row deleted
+       Actions   : Remove record from rtree for old identifier */
+    CREATE TRIGGER "rtree_{0}_{1}_delete" AFTER DELETE ON "{0}"
+      WHEN OLD."{1}" NOT NULL
+    BEGIN
+      DELETE FROM "rtree_{0}_{1}" WHERE id = OLD."{2}";
+    END;
+"""
+
+
+SPATIAL_INDEX_EXTENSION: str = """
+    INSERT INTO gpkg_extensions (table_name, column_name, extension_name, 
+                                 definition, scope) VALUES (?, ?, ?, ?, ?)
+"""
+
+
+SPATIAL_INDEX_RECORD: Tuple[str, str, str] = (
+    'gpkg_rtree_index', 'https://www.geopackage.org/spec131/#extension_rtree',
+    'write-only')
+
+
 if __name__ == '__main__':
     pass
```

## fudgeo/geometry/linestring.py

```diff
@@ -68,15 +68,17 @@
     # End coordinates property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return self._is_empty or not len(self.coordinates)
+        if self._is_empty is not None:
+            return self._is_empty
+        return not len(self.coordinates)
     # End is_empty property
 
     @property
     def points(self) -> List:
         """
         Points
         """
@@ -225,15 +227,17 @@
     # End lines property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return self._is_empty or not (bool(self._args) or bool(self.lines))
+        if self._is_empty is not None:
+            return self._is_empty
+        return not (bool(self._args) or bool(self.lines))
     # End is_empty property
 
     def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
```

## fudgeo/geometry/point.py

```diff
@@ -54,19 +54,19 @@
         """
         Is Empty
         """
         return isnan(self.x) and isnan(self.y)
     # End is_empty property
 
     @staticmethod
-    def _unpack(view: memoryview) -> DOUBLE:
+    def _unpack(value: bytes) -> DOUBLE:
         """
         Unpack Values
         """
-        *_, x, y = unpack(TWO_D_UNPACK_CODE, view)
+        *_, x, y = unpack(TWO_D_UNPACK_CODE, value)
         return x, y
     # End _unpack method
 
     def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes:
         """
         To WKB
         """
@@ -90,19 +90,18 @@
     # End to_gpkg method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'Point':
         """
         From Geopackage
         """
-        view = memoryview(value)
-        srs_id, _, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
+        srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
         if is_empty:
             return cls.empty(srs_id)
-        x, y = cls._unpack(view[offset:])
+        x, y = cls._unpack(value[offset:])
         return cls(x=x, y=y, srs_id=srs_id)
     # End from_gpkg method
 
     @classmethod
     def from_tuple(cls, xy: DOUBLE, srs_id: int) -> 'Point':
         """
         From Tuple
@@ -153,19 +152,19 @@
         """
         Is Empty
         """
         return isnan(self.x) and isnan(self.y) and isnan(self.z)
     # End is_empty property
 
     @staticmethod
-    def _unpack(view: memoryview) -> TRIPLE:
+    def _unpack(value: bytes) -> TRIPLE:
         """
         Unpack Values
         """
-        *_, x, y, z = unpack(THREE_D_UNPACK_CODE, view)
+        *_, x, y, z = unpack(THREE_D_UNPACK_CODE, value)
         return x, y, z
     # End _unpack method
 
     def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes:
         """
         To WKB
         """
@@ -189,19 +188,18 @@
     # End to_gpkg method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointZ':
         """
         From Geopackage
         """
-        view = memoryview(value)
-        srs_id, _, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
+        srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
         if is_empty:
             return cls.empty(srs_id)
-        x, y, z = cls._unpack(view[offset:])
+        x, y, z = cls._unpack(value[offset:])
         return cls(x=x, y=y, z=z, srs_id=srs_id)
     # End from_gpkg method
 
     @classmethod
     def from_tuple(cls, xyz: TRIPLE, srs_id: int) -> 'PointZ':
         """
         From Tuple
@@ -252,19 +250,19 @@
         """
         Is Empty
         """
         return isnan(self.x) and isnan(self.y) and isnan(self.m)
     # End is_empty property
 
     @staticmethod
-    def _unpack(view: memoryview) -> TRIPLE:
+    def _unpack(value: bytes) -> TRIPLE:
         """
         Unpack Values
         """
-        *_, x, y, m = unpack(THREE_D_UNPACK_CODE, view)
+        *_, x, y, m = unpack(THREE_D_UNPACK_CODE, value)
         return x, y, m
     # End _unpack method
 
     def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes:
         """
         To WKB
         """
@@ -288,19 +286,18 @@
     # End to_gpkg method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointM':
         """
         From Geopackage
         """
-        view = memoryview(value)
-        srs_id, _, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
+        srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
         if is_empty:
             return cls.empty(srs_id)
-        x, y, m = cls._unpack(view[offset:])
+        x, y, m = cls._unpack(value[offset:])
         return cls(x=x, y=y, m=m, srs_id=srs_id)
     # End from_gpkg method
 
     @classmethod
     def from_tuple(cls, xym: TRIPLE, srs_id: int) -> 'PointM':
         """
         From Tuple
@@ -355,19 +352,19 @@
         Is Empty
         """
         return (isnan(self.x) and isnan(self.y) and
                 isnan(self.z) and isnan(self.m))
     # End is_empty property
 
     @staticmethod
-    def _unpack(view: memoryview) -> QUADRUPLE:
+    def _unpack(value: bytes) -> QUADRUPLE:
         """
         Unpack Values
         """
-        *_, x, y, z, m = unpack(FOUR_D_UNPACK_CODE, view)
+        *_, x, y, z, m = unpack(FOUR_D_UNPACK_CODE, value)
         return x, y, z, m
     # End _unpack method
 
     def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes:
         """
         To WKB
         """
@@ -392,19 +389,18 @@
     # End to_gpkg method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointZM':
         """
         From Geopackage
         """
-        view = memoryview(value)
-        srs_id, _, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
+        srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
         if is_empty:
             return cls.empty(srs_id)
-        x, y, z, m = cls._unpack(view[offset:])
+        x, y, z, m = cls._unpack(value[offset:])
         return cls(x=x, y=y, z=z, m=m, srs_id=srs_id)
     # End from_gpkg method
 
     @classmethod
     def from_tuple(cls, xyzm: QUADRUPLE, srs_id: int) -> 'PointZM':
         """
         From Tuple
@@ -468,15 +464,17 @@
     # End coordinates property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return self._is_empty or not len(self.coordinates)
+        if self._is_empty is not None:
+            return self._is_empty
+        return not len(self.coordinates)
     # End is_empty property
 
     @property
     def points(self) -> List:
         """
         Points
         """
```

## fudgeo/geometry/point.pyi

```diff
@@ -21,15 +21,15 @@
     y: float
 
     def __init__(self, *, x: float, y: float, srs_id: int) -> None: ...
     def __eq__(self, other: 'Point') -> bool: ...
     @property
     def is_empty(self) -> bool: ...
     @staticmethod
-    def _unpack(view: memoryview) -> DOUBLE: ...
+    def _unpack(value: bytes) -> DOUBLE: ...
     def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes: ...
     @property
     def envelope(self) -> Envelope: ...
     def to_gpkg(self) -> bytes: ...
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'Point': ...
     @classmethod
@@ -48,15 +48,15 @@
     z: float
 
     def __init__(self, *, x: float, y: float, z: float, srs_id: int) -> None: ...
     def __eq__(self, other: 'PointZ') -> bool: ...
     @property
     def is_empty(self) -> bool: ...
     @staticmethod
-    def _unpack(view: memoryview) -> TRIPLE: ...
+    def _unpack(value: bytes) -> TRIPLE: ...
     def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes: ...
     @property
     def envelope(self) -> Envelope: ...
     def to_gpkg(self) -> bytes: ...
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointZ': ...
     @classmethod
@@ -75,15 +75,15 @@
     m: float
 
     def __init__(self, *, x: float, y: float, m: float, srs_id: int) -> None: ...
     def __eq__(self, other: 'PointM') -> bool: ...
     @property
     def is_empty(self) -> bool: ...
     @staticmethod
-    def _unpack(view: memoryview) -> TRIPLE: ...
+    def _unpack(value: bytes) -> TRIPLE: ...
     def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes: ...
     @property
     def envelope(self) -> Envelope: ...
     def to_gpkg(self) -> bytes: ...
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointM': ...
     @classmethod
@@ -103,15 +103,15 @@
     m: float
 
     def __init__(self, *, x: float, y: float, z: float, m: float, srs_id: int) -> None: ...
     def __eq__(self, other: 'PointZM') -> bool: ...
     @property
     def is_empty(self) -> bool: ...
     @staticmethod
-    def _unpack(view: memoryview) -> QUADRUPLE: ...
+    def _unpack(value: bytes) -> QUADRUPLE: ...
     def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes: ...
     @property
     def envelope(self) -> Envelope: ...
     def to_gpkg(self) -> bytes: ...
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointZM': ...
     @classmethod
```

## fudgeo/geometry/polygon.py

```diff
@@ -196,15 +196,17 @@
     # End rings property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return self._is_empty or not (bool(self._args) or bool(self.rings))
+        if self._is_empty is not None:
+            return self._is_empty
+        return not (bool(self._args) or bool(self.rings))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
@@ -339,15 +341,17 @@
     # End polygons property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return self._is_empty or not (bool(self._args) or bool(self.polygons))
+        if self._is_empty is not None:
+            return self._is_empty
+        return not (bool(self._args) or bool(self.polygons))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
```

## fudgeo/geometry/util.py

```diff
@@ -11,16 +11,15 @@
 from typing import Any, Callable, Dict, List, TYPE_CHECKING, Tuple, Union
 
 from numpy import array, frombuffer, ndarray
 from bottleneck import nanmax, nanmin
 
 from fudgeo.constant import (
     COUNT_CODE, EMPTY, ENVELOPE_COUNT, ENVELOPE_OFFSET, EnvelopeCode, GP_MAGIC,
-    HEADER_CODE,
-    HEADER_OFFSET, POINT_PREFIX)
+    HEADER_CODE, HEADER_OFFSET, POINT_PREFIX_ZM)
 
 
 if TYPE_CHECKING:  # pragma: no cover
     # noinspection PyUnresolvedReferences
     from fudgeo.geometry.linestring import (
         LineString, LineStringZ, LineStringM, LineStringZM)
     # noinspection PyUnresolvedReferences
@@ -261,15 +260,15 @@
     data = coordinates.tobytes()
     if not use_point_prefix or not count:
         ary.extend(data)
         return ary
     length = len(data)
     view = memoryview(data)
     step = length // count
-    prefix = POINT_PREFIX.get((has_z, has_m))
+    prefix = POINT_PREFIX_ZM.get((has_z, has_m))
     for i in range(0, length, step):
         ary.extend(prefix)
         ary.extend(view[i:i + step])
     return ary
 # End pack_coordinates function
```

## Comparing `fudgeo-0.5.2.dist-info/LICENSE` & `fudgeo-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fudgeo-0.5.2.dist-info/METADATA` & `fudgeo-0.6.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fudgeo
-Version: 0.5.2
-Summary: GeoPackage support from Python.  fudgeo is a simple package for creating OGC GeoPackages, Feature Classes, Tables, and geometries (read and write).
+Version: 0.6.0
+Summary: GeoPackage support from Python.  fudgeo is a lightweight package for creating OGC GeoPackages, Feature Classes, and Tables.  Easily read and write geometries and attributes to Feature Classes and Tables using regular Python objects and SQLite syntax.
 Author-email: "Integrated Informatics Inc." <contact@integrated-informatics.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Integrated Informatics Inc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,153 +46,169 @@
 Requires-Dist: coverage ; extra == 'dev'
 Requires-Dist: twine ; extra == 'dev'
 Requires-Dist: build ; extra == 'dev'
 
 # fudgeo
 
 `fudgeo` removes the *fear uncertainty doubt* from using GeoPackages with 
-Python. `fudgeo` is a simple package for creating OGC GeoPackages, Feature 
-Classes, Tables, and geometries (read and write).
+`Python`. `fudgeo` is a lightweight package for creating OGC GeoPackages, Feature 
+Classes, and Tables.  Easily read and write geometries and attributes to
+Feature Classes and Tables using regular `Python` objects and `SQLite` syntax.
 
 For details on OGC GeoPackages, please see the [OGC web page](http://www.geopackage.org/).
 
 
 ## Installation
 
 `fudgeo` is available from the [Python Package Index](https://pypi.org/project/fudgeo/).
 
 
-### Python Compatibility
+## Python Compatibility
 
 The `fudgeo` library is compatible with Python 3.7 to 3.11.
 
 
 ## Usage
 
 `fudgeo` can be used to: 
-* Create a new empty `GeoPackage`
-* Open an existing `GeoPackage`
+* Create a new empty `GeoPackage` or open an existing `GeoPackage`
 * Create new `FeatureClass` or `Table` with optional overwrite
 * Create `SpatialReferenceSystem` for a `FeatureClass`
-* Insert record (attributes) into a `Table`
-* Insert feature (geometry and attributes) into a `FeatureClass`
+* Build geometry objects from lists of coordinate values
 * Work with data in `Table` or `FeatureClass` in a normal `SQLite` manner (e.g. `SELECT`, `INSERT`, `UPDATE`, `DELETE`)
-* Drop `FeatureClass` or `Table`
 * Retrieve fields from a `FeatureClass` or `Table`
+* Access primary key field of `FeatureClass` or `Table` 
+* Access geometry column name and geometry type for `FeatureClass`
+* Add spatial index on `FeatureClass`
+* Drop `FeatureClass` or `Table`
 
 
 ### Create an Empty GeoPackage / Open GeoPackage
 
 ```python
 from fudgeo.geopkg import GeoPackage
 
 # Creates an empty geopackage
 gpkg = GeoPackage.create(r'c:\data\example.gpkg')
 
 # Opens an existing Geopackage (no validation)
 gpkg = GeoPackage(r'c:\data\example.gpkg')
 ```
 
-Geopackages are created with *three* default Spatial References defined
-automatically, a pair of Spatial References to handle undefined cases,
-and a WGS 84 entry. 
+`GeoPackage`s are created with *three* default Spatial References defined
+automatically, a pair of Spatial References to handle **undefined** cases,
+and a **WGS 84** entry. 
 
 The definition of the WGS84 entry is flexible - meaning that the 
 *WKT for WGS84* can be setup per the users liking. As an example, 
 use with Esri's ArcGIS means either using the *EPSG WKT* or the *ESRI WKT*. By
 default the *ESRI WKT* is used - However, if *EPSG WKT* is desired, you
 may provide a ``flavor`` parameter to the create method specifying EPSG.
 
 ```python
 # Creates an empty geopackage
 gpkg = GeoPackage.create(r'c:\temp\test.gpkg', flavor='EPSG')
 ```
 
-
 ### Create a Feature Class
 
 Use the `create_feature_class` method of a GeoPackage to make
 a new feature class.  Feature classes require a name and a Spatial 
 Reference, the name must follow SQLite naming requirements.  Each
 feature class is defined with `fid` and `SHAPE` fields, additional
 fields can be defined during creation.
 
 A Feature Class can be created with *Z* or *M* (or both) enabled. If 
 either of these options are enabled, the geometry inserted into the 
 Feature Class **must** include a value for the option specified.
 
 ```python
-from fudgeo.geopkg import GeoPackage, SpatialReferenceSystem, Field
-from fudgeo.enumeration import GeometryType, SQLFieldType
+from typing import Tuple
 
-gpkg = GeoPackage.create(r'c:\temp\test.gpkg')
+from fudgeo.geopkg import FeatureClass, Field, GeoPackage, SpatialReferenceSystem
+from fudgeo.enumeration import GeometryType, SQLFieldType
 
-srs_wkt = (
+SRS_WKT: str = (
     'PROJCS["WGS_1984_UTM_Zone_23N",'
     'GEOGCS["GCS_WGS_1984",'
     'DATUM["D_WGS_1984",'
     'SPHEROID["WGS_1984",6378137.0,298.257223563]],'
     'PRIMEM["Greenwich",0.0],'
     'UNIT["Degree",0.0174532925199433]],'
     'PROJECTION["Transverse_Mercator"],'
     'PARAMETER["False_Easting",500000.0],'
     'PARAMETER["False_Northing",0.0],'
     'PARAMETER["Central_Meridian",-45.0],'
     'PARAMETER["Scale_Factor",0.9996],'
     'PARAMETER["Latitude_Of_Origin",0.0],'
     'UNIT["Meter",1.0]]')
 
-srs = SpatialReferenceSystem(
-    'WGS_1984_UTM_Zone_23N', 'EPSG', 32623, srs_wkt)
-fields = (
-    Field('heart_rate', SQLFieldType.integer),
-    Field('power', SQLFieldType.double),
-    Field('comment', SQLFieldType.text, 100),
-    Field('is_valid', SQLFieldType.boolean))
-
-fc = gpkg.create_feature_class(
-    'test', srs, fields=fields, shape_type=GeometryType.point)
+SRS: SpatialReferenceSystem = SpatialReferenceSystem(
+    name='WGS_1984_UTM_Zone_23N', organization='EPSG',
+    org_coord_sys_id=32623, definition=SRS_WKT)
+fields: Tuple[Field, ...] = (
+    Field('road_id', SQLFieldType.integer),
+    Field('name', SQLFieldType.text, size=100),
+    Field('begin_easting', SQLFieldType.double),
+    Field('begin_northing', SQLFieldType.double),
+    Field('end_easting', SQLFieldType.double),
+    Field('end_northing', SQLFieldType.double),
+    Field('is_one_way', SQLFieldType.boolean))
+
+gpkg: GeoPackage = GeoPackage.create(r'c:\temp\test.gpkg')
+fc: FeatureClass = gpkg.create_feature_class(
+    'road_l', srs=SRS, fields=fields, shape_type=GeometryType.linestring,
+    z_enabled=False, m_enabled=True, overwrite=True, spatial_index=True)
 ```
 
-Read more about spatial references in GeoPackages [here](https://github.com/realiii/pygeopkg/blob/master/README.md#about-spatial-references-for-geopackages)
+### About Spatial References For GeoPackages
 
+Spatial References in GeoPackages can use any definition from any 
+authority - be that `EPSG`, `ESRI`, or another authority. `fudgeo` imposes no 
+restriction and performs no checks on the definitions provided. Take care 
+to ensure that the definitions are compatible with the platform / software 
+you intend to utilize with the `GeoPackage`.
 
 ### Insert Features into a Feature Class (SQL)
 
 Features can be inserted into a Feature Class using SQL.
 
 This example shows the creation of a random point Feature Class and
 builds upon the code from previous examples. Note that the create Feature Class
 portion of the code is omitted...
 
 ```python
 from random import choice, randint
 from string import ascii_uppercase, digits
-from fudgeo.geometry import Point
-from fudgeo.geopkg import GeoPackage
+from typing import List, Tuple
 
-# NOTE Builds from previous examples 
-gpkg = GeoPackage(r'c:\data\example.gpkg')
+from fudgeo.geometry import LineStringM
+from fudgeo.geopkg import GeoPackage
 
 # Generate some random points and attributes
-rows = []
+rows: List[Tuple[LineStringM, int, str, float, float, float, float, bool]] = []
 for i in range(10000):
-    rand_str = ''.join(choice(ascii_uppercase + digits) for _ in range(10))
-    rand_int = randint(0, 1000)
-    rand_x = randint(300000, 600000)
-    rand_y = randint(1, 100000)
-    rows.append((Point(x=rand_x, y=rand_y, srs_id=32623), rand_int, rand_str))
+    name = ''.join(choice(ascii_uppercase + digits) for _ in range(10))
+    road_id = randint(0, 1000)
+    eastings = [randint(300000, 600000) for _ in range(20)]
+    northings = [randint(1, 100000) for _ in range(20)]
+    coords = [(x, y, m) for m, (x, y) in enumerate(zip(eastings, northings))]
+    road = LineStringM(coords, srs_id=32623)
+    rows.append((road, road_id, name, eastings[0], northings[0],
+                 eastings[-1], northings[-1], False))
 
+# NOTE Builds from previous examples
+gpkg: GeoPackage = GeoPackage(r'c:\data\example.gpkg')   
 with gpkg.connection as conn:
-    conn.executemany(
-        """INSERT INTO test (SHAPE, heart_rate, comment) 
-           VALUES (?, ?, ?)""", rows)
+    conn.executemany("""
+        INSERT INTO road_l (SHAPE, road_id, name, begin_easting, begin_northing, 
+                            end_easting, end_northing, is_one_way) 
+           VALUES (?, ?, ?, ?, ?, ?, ?, ?)""", rows)
 ```
 
-
 ### Geometry Examples
 
 Review the tests for `fudgeo` for a comprehensive look into 
 creating geometries, below are some examples showing the simplicity
 of this package.
 
 
@@ -212,60 +228,70 @@
           (700000, 1), (300000, 1)]]
 poly = Polygon(rings, srs_id=32623)
 ```
 
 ### Select Features from GeoPackage (SQL)
 
 When selecting features from a GeoPackage feature class use SQL.  For 
-the most part (mainly simple geometries) this can be done via a basic
-select statement like:
+the most part (mainly simple geometries e.g. those without *Z* or *M*) this 
+can be done via a basic `SELECT` statement like:
 
 ```python
-gpkg = GeoPackage(r'c:\data\example.gpkg')
-cursor = gpkg.connection.execute(
-    """SELECT SHAPE, heart_rate FROM test""")
+gpkg = GeoPackage(...)
+cursor = gpkg.connection.execute("""SELECT SHAPE, example_id FROM point_fc""")
 features = cursor.fetchall()
 ```
 
 This will return a list of tuples where each tuple contains a `Point`
-object and an integer (heart rate).
+object and an integer for `example_id` field.
 
 When working with extended geometry types (those with *Z* and/or *M*) 
-then the approach is to ensure SQLite knows how to convert the 
-geopackage stored geometry to a `fudgeo` geometry, this is done like
-so (pretending here that we created `test` table as a point geometry
-with z enabled):
+then the approach is to ensure `SQLite` knows how to convert the 
+geopackage stored geometry to a `fudgeo` geometry, this is done like so:
 
 ```python
 gpkg = GeoPackage(r'c:\data\example.gpkg')
 cursor = gpkg.connection.execute(
-    """SELECT SHAPE "[PointZ]", heart_rate FROM test""")
+    """SELECT SHAPE "[LineStringM]", road_id FROM test""")
 features = cursor.fetchall()
 ```
 
-or a little more general, accounting for extended geometry types and possibility of the 
-geometry column being something other tha SHAPE:
+or a little more general, accounting for extended geometry types and
+possibility of the geometry column being something other tha `SHAPE`:
 
 ```python
 from fudgeo.geopkg import FeatureClass
 
 gpkg = GeoPackage(r'c:\data\example.gpkg')
-fc = FeatureClass(geopackage=gpkg, name='test')
+fc = FeatureClass(geopackage=gpkg, name='road_l')
 cursor = gpkg.connection.execute(f"""
-    SELECT {fc.geometry_column_name} "[{fc.geometry_type}]", heart_rate 
-    FROM {fc.name}""")
+    SELECT {fc.geometry_column_name} "[{fc.geometry_type}]", road_id 
+    FROM {fc.escaped_name}""")
 features = cursor.fetchall()
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Release History
 
+### v0.6.0
+* change `ogr_contents` default value to `False` (breaking change)
+* add `spatial_index` option to `FeatureClass` creation, default to `False`
+* add `add_spatial_index` method to `FeatureClass` for adding spatial index post creation
+* add `has_spatial_index` property to `FeatureClass`
+* add `count` property to `Table` and `FeatureClass`
+* add `primary_key_field` property to `Table` and `FeatureClass`
+* small speed-up to `Point` unpacking
+* update `is_empty` to rely on internal attribute data type
+* improvements to SQL statements to handle names that must be escaped
+* bump `user_version` to reflect adopted version 1.3.1 of OGC GeoPackage
+* add optional views for geometry columns and spatial references
+
 ### v0.5.2
 * store empty state on the instance during geometry read
 * introduce base classes for common capability and parametrize via class attributes
 * add stub files to provide type hinting specialization 
 
 ### v0.5.1
 * small performance improvements by reducing `bytes` concatenation and building up `bytearray`
```

