# Comparing `tmp/fw_gear_splitter-1.4.3-py3-none-any.whl.zip` & `tmp/fw_gear_splitter-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 16353 bytes, number of entries: 12
+Zip file size: 17114 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      135 b- defN 80-Jan-01 00:00 fw_gear_splitter/__init__.py
--rw-r--r--  2.0 unx    13074 b- defN 80-Jan-01 00:00 fw_gear_splitter/main.py
--rw-r--r--  2.0 unx     7724 b- defN 80-Jan-01 00:00 fw_gear_splitter/metadata.py
--rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_splitter/parser.py
+-rw-r--r--  2.0 unx    14140 b- defN 80-Jan-01 00:00 fw_gear_splitter/main.py
+-rw-r--r--  2.0 unx     8402 b- defN 80-Jan-01 00:00 fw_gear_splitter/metadata.py
+-rw-r--r--  2.0 unx     1241 b- defN 80-Jan-01 00:00 fw_gear_splitter/parser.py
 -rw-r--r--  2.0 unx       38 b- defN 80-Jan-01 00:00 fw_gear_splitter/splitter/__init__.py
 -rw-r--r--  2.0 unx     6372 b- defN 80-Jan-01 00:00 fw_gear_splitter/splitter/base.py
--rw-r--r--  2.0 unx    13883 b- defN 80-Jan-01 00:00 fw_gear_splitter/splitters.py
--rw-r--r--  2.0 unx     1747 b- defN 80-Jan-01 00:00 fw_gear_splitter/utils.py
--rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_splitter-1.4.3.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 fw_gear_splitter-1.4.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2731 b- defN 16-Jan-01 00:00 fw_gear_splitter-1.4.3.dist-info/METADATA
-?rw-r--r--  2.0 unx     1015 b- defN 16-Jan-01 00:00 fw_gear_splitter-1.4.3.dist-info/RECORD
-12 files, 48991 bytes uncompressed, 14643 bytes compressed:  70.1%
+-rw-r--r--  2.0 unx    13776 b- defN 80-Jan-01 00:00 fw_gear_splitter/splitters.py
+-rw-r--r--  2.0 unx     2243 b- defN 80-Jan-01 00:00 fw_gear_splitter/utils.py
+-rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_splitter-1.5.0.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 fw_gear_splitter-1.5.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2816 b- defN 16-Jan-01 00:00 fw_gear_splitter-1.5.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     1015 b- defN 16-Jan-01 00:00 fw_gear_splitter-1.5.0.dist-info/RECORD
+12 files, 51358 bytes uncompressed, 15404 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: fw_gear_splitter/splitters.py
 Comment: 
 
 Filename: fw_gear_splitter/utils.py
 Comment: 
 
-Filename: fw_gear_splitter-1.4.3.dist-info/LICENSE
+Filename: fw_gear_splitter-1.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: fw_gear_splitter-1.4.3.dist-info/WHEEL
+Filename: fw_gear_splitter-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: fw_gear_splitter-1.4.3.dist-info/METADATA
+Filename: fw_gear_splitter-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: fw_gear_splitter-1.4.3.dist-info/RECORD
+Filename: fw_gear_splitter-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_gear_splitter/main.py

```diff
@@ -14,14 +14,17 @@
     EuclideanSplitter,
     JensenShannonDICOMSplitter,
     UniqueTagMultiSplitter,
     UniqueTagSingleSplitter,
 )
 from .utils import collection_from_df, collection_to_df
 
+# Override dicom validation logging level
+validation_log = logging.getLogger("fw_file.dicom.validation")
+validation_log.setLevel(logging.INFO)
 log = logging.getLogger(__name__)
 
 SCORE_THRESH = 0.5
 
 
 def run_individual_split(
     splitter: SingleSplitter, dataframe: pd.DataFrame, **kwargs: t.Any
@@ -166,15 +169,15 @@
     return (dicom_coll, localizer_coll)
 
 
 def split_dicom(  # pylint: disable=too-many-locals,too-many-statements
     dcm: DICOMCollection,
     group_by: t.Optional[t.List[str]],
     split_localizer: bool,
-) -> t.Dict[SeriesName, DICOMCollection]:
+) -> t.Optional[t.Dict[SeriesName, DICOMCollection]]:
     """Split the dicom archive by tags or localizer.
 
     Args:
         dcm (DICOMCollection): Dicom archive
         group_by (t.Optional[t.List[str]]): List of tags to split by.
         split_localizer (bool): Whether or not to split localizer.
 
@@ -199,30 +202,30 @@
             series = primary.get("SeriesNumber")
         except ValueError:
             log.error(
                 "Multiple SeriesNumbers found on primary split. "
                 "Please split on SeriesInstanceUID."
             )
             # Don't split if we find multiple SeriesNumbers here.
-            return {}
+            return None
         name = SeriesName.gen_name(primary, series_number=series)
         log.info("Naming primary collection: %s", str(name))
         outputs[name] = primary
         if len(out_dfs) > 1:
             for i, out_df in enumerate(out_dfs[1:]):
                 secondary = collection_from_df(dcm, out_df)
                 try:
                     series = secondary.get("SeriesNumber")
                 except ValueError:
                     log.error(
                         "Multiple SeriesNumbers found on secondary split."
                         " Please split on SeriesInstanceUID."
                     )
                     # Don't split if we find multiple SeriesNumbers here.
-                    return {}
+                    return None
                 name = SeriesName.gen_name(
                     secondary,
                     series_number=(series if series else str(i + 1000)),
                 )
                 counter = 1
                 while name in outputs:
                     name.number = counter
@@ -235,15 +238,15 @@
         try:
             series = dcm.get("SeriesNumber")
         except ValueError:
             log.error(
                 "Multiple SeriesNumbers found. Please split on SeriesInstanceUID."
             )
             # Don't split if we find multiple SeriesNumbers here.
-            return {}
+            return None
         name = SeriesName.gen_name(dcm, series_number=series)
         outputs[name] = dcm
 
     if len(outputs) > 1:
         # Generating unique attributes for the new grouped series
         for name, collection in outputs.items():
             orig_series_uid = collection.get("SeriesInstanceUID")
@@ -251,87 +254,103 @@
             update_localizer_frames(collection, orig_series_uid, orig_series_num)
 
     if split_localizer:
         # <dcm>.get() will raise ValueError if there are multiple unique values.
         #   let it raise here.
         localizer_outputs = {}
         for name, archive in outputs.items():
-            log.info("Splitting collection %s", name)
-            dicom, localizer = run_split_localizer(archive)
-            localizer_outputs[name] = dicom
-            if localizer and len(localizer) > 0:
-                log.info("Found %s localizer frame(s)", str(len(localizer)))
-                orig_series_uid = dicom.get("SeriesInstanceUID")
-                orig_series_num = name.series_number
-                new_series_num = update_localizer_frames(
-                    localizer, orig_series_uid, orig_series_num
+            # split_localizer only available for MR or CT modalities
+            if archive.get("Modality") not in ["MR", "CT"]:
+                log.info(
+                    "Split localizer option is only applicable for MR or CT DICOMs. "
+                    "%s DICOM modality is %s.",
+                    name,
+                    archive.get("Modality"),
                 )
-                new_name = SeriesName.from_name(name)
-                new_name.series_number = new_series_num
-                new_name.localizer = True
-                localizer_outputs[new_name] = localizer
+            else:
+                log.info("Splitting collection %s", name)
+                dicom, localizer = run_split_localizer(archive)
+                localizer_outputs[name] = dicom
+                if localizer and len(localizer) > 0:
+                    log.info("Found %s localizer frame(s)", str(len(localizer)))
+                    orig_series_uid = dicom.get("SeriesInstanceUID")
+                    orig_series_num = name.series_number
+                    new_series_num = update_localizer_frames(
+                        localizer, orig_series_uid, orig_series_num
+                    )
+                    new_name = SeriesName.from_name(name)
+                    new_name.series_number = new_series_num
+                    new_name.localizer = True
+                    localizer_outputs[new_name] = localizer
         outputs.update(localizer_outputs)
 
     return outputs
 
 
 # Most of this function is already tested in fw_file
 def run(
     dcm_path: Path,
     output_dir: Path,
     group_by: t.List[str],
     split_localizer: bool,
     zip_single: bool,
-) -> t.Tuple[Path, ...]:  # pragma: no cover
+) -> t.Tuple[t.Tuple[Path, ...], bool]:  # pragma: no cover
     """Main function of module.
 
     Args:
         dcm_path (Path): Dicom file path
         output_dir (Path): Gear output directory.
         group_by (t.List[str]): List of tags to split by.
         split_localizer (bool): Whether or not to split localizer out.
         zip_single (bool): Zip single dicom or not
 
     Returns:
         t.Tuple[Path]: Tuple of saved output paths.
+        bool: Whether or not splitter completed successfully
     """
     if sniff_dcm(dcm_path):
         log.info("Input is a single DICOM, nothing to split. Exiting")
-        return tuple()
+        return tuple(), True
     if not zipfile.is_zipfile(dcm_path):
         log.info("Not a zip file, nothing to split. Exiting")
-        return tuple()
+        return tuple(), True
     with DICOMCollection.from_zip(dcm_path, force=True, stop_when=None) as dcm:
         suffix = ".dicom.zip"
         # Don't try to split if there is only one slice.
         if len(dcm) == 1:
             log.info("Only one slice present in archive.")
-            return tuple()
+            return tuple(), True
 
         collections = split_dicom(dcm, group_by, split_localizer)
+        # If collections = None, splitter encountered an error (see log)
+        if collections == None:
+            log.info("Archive was not split due to an error.")
+            return tuple(), False
         # If nothing was split out
-        if len(collections.items()) in (0, 1):
-            log.info("Archive was not split.")
+        elif len(collections.items()) in (0, 1):
+            log.info("Archive was not split, nothing to split on found.")
             # Return an empty tuple
-            return tuple()
+            return tuple(), True
         # Otherwise populate output dir and return saved paths.
         save_paths = []
         for name, collection in collections.items():
             log.info(
                 "Adding contributing equipment to collection: %s",
                 str(name),
             )
             add_contributing_equipment(collection)
 
             if len(collection) > 1 or zip_single:
                 # save and name
                 save_path = output_dir / (str(name) + suffix)
+                log.info(f"Saving {name} to {save_path}")
                 save_paths.append(save_path)
                 collection.to_zip(save_path)
             else:
                 # remove .zip when only one slice in DICOMCollection
                 suffix = suffix.replace(".zip", "")
                 save_path = output_dir / (str(name) + suffix)
+                log.info(f"Saving {name} to {save_path}")
                 save_paths.append(save_path)
                 collection[0].save(save_path)
 
-        return tuple(save_paths)
+        return tuple(save_paths), True
```

## fw_gear_splitter/metadata.py

```diff
@@ -159,15 +159,17 @@
 def gen_series_uid(dcm: DICOMCollection) -> str:
     """Simple helper to generate and set uid."""
     uid = generate_uid()
     dcm.set("SeriesInstanceUID", uid)
     return uid
 
 
-def populate_qc(context: GearToolkitContext, file_name: str, split: bool) -> None:
+def populate_qc(
+    context: GearToolkitContext, file_name: str, split: bool, success: bool
+) -> None:
     """Utility to populate splitter specific qc info on an output filename."""
     dicom = context.get_input("dicom")
     get_parent_fn = getattr(context.client, f"get_{dicom['hierarchy']['type']}")
     parent = get_parent_fn(dicom["hierarchy"]["id"])
     orig = parent.get_file(dicom["location"]["name"])
 
     original = {
@@ -176,44 +178,52 @@
             "file_id": getattr(orig, "file_id", ""),
         }
     }
 
     context.metadata.add_qc_result(
         file_name,
         "split",
-        state=("PASS" if split else "FAIL"),
+        state=("PASS" if success else "FAIL"),
         data=(original if split else {}),
     )
 
 
 def populate_tags(
     context: GearToolkitContext,
     output_paths: t.Tuple,
-    set_deleted: bool = False,
+    set_deleted: t.Optional[str] = None,
 ) -> None:
     """Populate splitter specific tags on output files and input file."""
 
     tag: str = context.config.get("tag", "")
     tag_single: str = context.config.get("tag-single-output", "")
-    input_tags = [tag]
-    if set_deleted:
-        input_tags.append("delete")
-
-    # input file
-    context.metadata.add_file_tags(context.get_input("dicom"), input_tags)
-
-    # output files
-    # Sort alphabetically by file name
-    paths = sorted(list(output_paths))
-    for i, path in enumerate(paths):
-        file_ = Path(path).name
-        tags = [tag]
-        if i == 0 and len(tag_single) > 0:
-            tags.append(tag_single)
-        context.metadata.add_file_tags(file_, tags)
+
+    if not set_deleted:
+        # set_deleted==None occurs when the DICOM was not split.
+        # Here, the input file is simply tagged with the configured tag(s)
+        context.metadata.add_file_tags(context.get_input("dicom"), [tag])
+    else:
+        # If set_deleted is not None, the DICOM was split.
+        if set_deleted == "retained":
+            # Input file is tagged with configured tags as well as "delete",
+            # to match gear functioning before gear rules r/w was supported.
+            input_tags = [tag]
+            input_tags.append("delete")
+            context.metadata.add_file_tags(context.get_input("dicom"), input_tags)
+        # If set_deleted == "deleted", the input file no longer exists,
+        # so there is no input file to tag and we move on.
+
+        # Output files are sorted alphabetically by file name
+        paths = sorted(list(output_paths))
+        for i, path in enumerate(paths):
+            file_ = Path(path).name
+            tags = [tag]
+            if i == 0 and len(tag_single) > 0:
+                tags.append(tag_single)
+            context.metadata.add_file_tags(file_, tags)
 
 
 def update_localizer_frames(
     dcm: DICOMCollection,
     orig_series_uid: t.Optional[str],
     orig_series_num: t.Optional[str],
 ) -> str:
```

## fw_gear_splitter/parser.py

```diff
@@ -12,23 +12,25 @@
 
     Returns:
         Tuple[Path, bool, t.List[str]]: tuple containing,
             - Path of dicom input
             - extract_localizer
             - group_by (unique tags to split archive on)
             - zip_single (Zip single dicoms)
+            - delete_input (whether or not to delete input after splitting)
     """
 
     # INPUTS
     dcm_path = Path(gear_context.get_input_path("dicom"))
 
     # CONFIG
     extract_localizer = gear_context.config.get("extract_localizer")
     zip_single_raw = gear_context.config.get("zip-single-dicom", "match")
     # Zip single is set to True on "match", False otherwise ("no")
     zip_single = zip_single_raw == "match"
     if gear_context.config.get("group_by", ""):
         group_by = gear_context.config.get("group_by").split(",")
     else:
         group_by = None
+    delete_input = gear_context.config.get("delete_input")
 
-    return (dcm_path, extract_localizer, group_by, zip_single)
+    return (dcm_path, extract_localizer, group_by, zip_single, delete_input)
```

## fw_gear_splitter/splitters.py

```diff
@@ -368,11 +368,9 @@
                 1. Dataframe containing paths of dicom frames that belong
                     in main archive
                 ... Dataframes of other unique groups
         """
         if not drop_cols:
             drop_cols = ["value", "p"]
 
-        unique = dataframe.groupby(self.tags)
-        # pylint: disable=consider-using-generator
-        return tuple([unique.get_group(g) for g in unique.groups])
-        # pylint: enable=consider-using-generator
+        unique = dataframe.groupby(self.tags, dropna=False)
+        return tuple(df for val, df in unique)
```

## fw_gear_splitter/utils.py

```diff
@@ -1,11 +1,12 @@
 """Splitter utilities."""
 import typing as t
 
 import pandas as pd
+from flywheel_gear_toolkit import GearToolkitContext
 from fw_file.dicom import DICOMCollection
 
 
 def quote_val(val: t.Any) -> str:
     """Add quotes around a string value."""
     if isinstance(val, str):
         return f"'{val}'"
@@ -57,7 +58,20 @@
     """
     file_coll = files.__class__()
     for idx in list(dataframe.index):
         file = files[idx]
         file_coll.append(file)
 
     return file_coll
+
+
+def delete_input(context: GearToolkitContext):
+    """Delete input file for use after successful split.
+
+    Args:
+        context (GearToolkitContext): Gear configuration
+    """
+    dicom = context.get_input("dicom")
+    get_parent_fn = getattr(context.client, f"get_{dicom['hierarchy']['type']}")
+    parent = get_parent_fn(dicom["hierarchy"]["id"])
+    orig = parent.get_file(dicom["location"]["name"])
+    parent.delete_file(orig.name)
```

## Comparing `fw_gear_splitter-1.4.3.dist-info/LICENSE` & `fw_gear_splitter-1.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_gear_splitter-1.4.3.dist-info/METADATA` & `fw_gear_splitter-1.5.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fw-gear-splitter
-Version: 1.4.3
+Version: 1.5.0
 Summary: DICOM splitter based on unique tags, or localizers
 License: MIT
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flywheel-gear-toolkit (>=0.6,<0.7)
 Requires-Dist: flywheel-sdk (>=16.0.0,<17.0.0)
-Requires-Dist: fw-file (>=2.1,<3.0)
+Requires-Dist: fw-file (>=2,<3)
 Requires-Dist: importlib-metadata (>=3.7.0,<4.0.0)
 Requires-Dist: pandas (>=1.2.1,<2.0.0)
 Requires-Dist: pylibjpeg (>=1.1.1,<2.0.0)
 Requires-Dist: pylibjpeg-libjpeg (>=1.1.0,<2.0.0)
 Requires-Dist: pylibjpeg-openjpeg (>=1.0.1,<2.0.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Description-Content-Type: text/markdown
@@ -48,14 +48,15 @@
 * __extract_localizer__ (boolean, default True): Whether or not to extract localizer
 from archive.
 * __group_by__ (string, default "SeriesInstanceUID"): Comma separated list of dicom
 tags to split the archvie on.
 * __tag__ (string, default "splitter"): The tag to be added on input file upon run
 completion.
 * __debug__ (boolean, default False): Include debug output.
+* __delete_input__ (boolean, default True): Delete input if DICOM is successfully split.
 
 ### Outputs
 
 The gear will output nothing if no splitting action was taken.  Otherwise it will output
 a variable number of archives depending on the input and configuration named with the
 following pattern:
```

## Comparing `fw_gear_splitter-1.4.3.dist-info/RECORD` & `fw_gear_splitter-1.5.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 fw_gear_splitter/__init__.py,sha256=ga8HPszNy5k9r2PR-_xTwZq5q20wru1BHO6M4mqLbi8,135
-fw_gear_splitter/main.py,sha256=UGHF9ZJDLj4WDbBL4Gz-lx9WrauVbSOejNANTZEyfdg,13074
-fw_gear_splitter/metadata.py,sha256=KBy5LwfHxHb2Fq3WlmmiBA14dwuLpVakxDZkqhyFYUo,7724
-fw_gear_splitter/parser.py,sha256=KafXjY8YD1IT5AWvs3aCUkNRogSOs02Q7v1ah8aUXjo,1092
+fw_gear_splitter/main.py,sha256=9yQGh95TImX2EKKkWw7nNk3Hjglul0gY3UlinYfCdlo,14140
+fw_gear_splitter/metadata.py,sha256=Sk521ApLySyYsbgZKnJ9-FcrPyYl-ndINejklp7kTjw,8402
+fw_gear_splitter/parser.py,sha256=aEAjrG1fn3_D_kp8Yu4HTFUk-2jw6OEKjKc7ekXcGDo,1241
 fw_gear_splitter/splitter/__init__.py,sha256=PeCzMJ2dMdzODEJ4CP7foHb3a-hk-L5OgPzeDFkv97s,38
 fw_gear_splitter/splitter/base.py,sha256=cnM0d8l46dZqwbDjw_mEsBsH8QJLrfGin5np6VbHD6U,6372
-fw_gear_splitter/splitters.py,sha256=y4qkjmWlNGEvfB-lmJ-NXU9IgpxYAIVIRPSKbdQD6Jc,13883
-fw_gear_splitter/utils.py,sha256=PjMDclHUXBwtWsgXn7cE22zAk2T4XOSu1Kvc4i6l17k,1747
-fw_gear_splitter-1.4.3.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
-fw_gear_splitter-1.4.3.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-fw_gear_splitter-1.4.3.dist-info/METADATA,sha256=iSdJRPaUtPWM-rCX6V5VhteaBSgYfQbzV0DcSri4XHc,2731
-fw_gear_splitter-1.4.3.dist-info/RECORD,,
+fw_gear_splitter/splitters.py,sha256=8be2O88OPcbYDyb1GsVFgb1tUyzuhCf4ox2M5earvTg,13776
+fw_gear_splitter/utils.py,sha256=MmXOTS5Ktj53Eo2TTuvHnwLvRj8qtS3fBRkHFqnCOd4,2243
+fw_gear_splitter-1.5.0.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
+fw_gear_splitter-1.5.0.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
+fw_gear_splitter-1.5.0.dist-info/METADATA,sha256=XZvENNKaugu8_kFY7EHgerIQSRgSNHIzR0MmQ79lClM,2816
+fw_gear_splitter-1.5.0.dist-info/RECORD,,
```

