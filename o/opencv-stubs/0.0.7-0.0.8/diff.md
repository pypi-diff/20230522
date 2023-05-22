# Comparing `tmp/opencv_stubs-0.0.7.tar.gz` & `tmp/opencv_stubs-0.0.8.tar.gz`

## Comparing `opencv_stubs-0.0.7.tar` & `opencv_stubs-0.0.8.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/requirements/requirements-build.txt
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/requirements/requirements.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/__init__.pyi
--rw-r--r--   0        0        0   165718 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/classes.pyi
--rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/constants.pyi
--rw-r--r--   0        0        0   529741 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/functions.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/py.typed
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/__init__.py
--rw-r--r--   0        0        0    34376 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/aruco.pyi
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/barcode.pyi
--rw-r--r--   0        0        0    11107 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/bgsegm.pyi
--rw-r--r--   0        0        0    19750 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/bioinspired.pyi
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ccm.pyi
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/colored_kinfu.pyi
--rw-r--r--   0        0        0    23759 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/cuda.pyi
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/data.pyi
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/datasets.pyi
--rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/detail.pyi
--rw-r--r--   0        0        0    45108 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/dnn.pyi
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/dnn_superres.pyi
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/dpm.pyi
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/dynafu.pyi
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/error.pyi
--rw-r--r--   0        0        0    34295 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/face.pyi
--rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/fisheye.pyi
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/flann.pyi
--rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ft.pyi
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/hfs.pyi
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/img_hash.pyi
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/intensity_transform.pyi
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ipp.pyi
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/large_kinfu.pyi
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/legacy.pyi
--rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/line_descriptor.pyi
--rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/linemod.pyi
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/load_config_py3.pyi
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/mat_wrapper.pyi
--rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/mcc.pyi
--rw-r--r--   0        0        0    60302 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ml.pyi
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/motempl.pyi
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/multicalib.pyi
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ocl.pyi
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ogl.pyi
--rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/omnidir.pyi
--rw-r--r--   0        0        0    27976 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/optflow.pyi
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/parallel.pyi
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/phase_unwrapping.pyi
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/plot.pyi
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ppf_match_3d.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/qt.pyi
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/quality.pyi
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/rapid.pyi
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/reg.pyi
--rw-r--r--   0        0        0    30043 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/rgbd.pyi
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/saliency.pyi
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/samples.pyi
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/segmentation.pyi
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/stereo.pyi
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/structured_light.pyi
--rw-r--r--   0        0        0    26974 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/text.pyi
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/version.pyi
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/videoio_registry.pyi
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/videostab.pyi
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/wechat_qrcode.pyi
--rw-r--r--   0        0        0    40748 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/xfeatures2d.pyi
--rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/xphoto.pyi
--rw-r--r--   0        0        0   105878 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/core.pyi
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/ie.pyi
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/oak.pyi
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/onnx.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/own.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/render.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/video.pyi
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/streaming/__init__.pyi
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/__init__.pyi
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/draw.pyi
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/gst.pyi
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/kinfu/__init__.pyi
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/kinfu/detail.pyi
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/misc/__init__.pyi
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/misc/version.pyi
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/__init__.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/fs.pyi
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/nested.pyi
--rw-r--r--   0        0        0    80287 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ximgproc/__init__.pyi
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ximgproc/segmentation.pyi
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/add_missing_overloads.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/generate_classes.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/generate_constants.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/generate_modules.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/merge_with_microsoft_stubs.py
--rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/processing_utils.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/undefined_to_any.py
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/LICENSE
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/README.md
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/requirements/requirements-build.txt
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/requirements/requirements.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/__init__.pyi
+-rw-r--r--   0        0        0   165718 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/classes.pyi
+-rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/constants.pyi
+-rw-r--r--   0        0        0   530044 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/functions.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/py.typed
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/__init__.py
+-rw-r--r--   0        0        0    34376 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/aruco.pyi
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/barcode.pyi
+-rw-r--r--   0        0        0    11107 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/bgsegm.pyi
+-rw-r--r--   0        0        0    19750 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/bioinspired.pyi
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/ccm.pyi
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/colored_kinfu.pyi
+-rw-r--r--   0        0        0    23759 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/cuda.pyi
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/data.pyi
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/datasets.pyi
+-rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/detail.pyi
+-rw-r--r--   0        0        0    45108 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/dnn.pyi
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/dnn_superres.pyi
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/dpm.pyi
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/dynafu.pyi
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/error.pyi
+-rw-r--r--   0        0        0    34295 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/face.pyi
+-rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/fisheye.pyi
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/flann.pyi
+-rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/ft.pyi
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/hfs.pyi
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/img_hash.pyi
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/intensity_transform.pyi
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/ipp.pyi
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/large_kinfu.pyi
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/legacy.pyi
+-rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/line_descriptor.pyi
+-rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/linemod.pyi
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/load_config_py3.pyi
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/mat_wrapper.pyi
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/mcc.pyi
+-rw-r--r--   0        0        0    60302 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/ml.pyi
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/motempl.pyi
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/multicalib.pyi
+-rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/ocl.pyi
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/ogl.pyi
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/omnidir.pyi
+-rw-r--r--   0        0        0    27976 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/optflow.pyi
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/parallel.pyi
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/phase_unwrapping.pyi
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/plot.pyi
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/ppf_match_3d.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/qt.pyi
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/quality.pyi
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/rapid.pyi
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/reg.pyi
+-rw-r--r--   0        0        0    30043 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/rgbd.pyi
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/saliency.pyi
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/samples.pyi
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/segmentation.pyi
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/stereo.pyi
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/structured_light.pyi
+-rw-r--r--   0        0        0    26974 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/text.pyi
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/version.pyi
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/videoio_registry.pyi
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/videostab.pyi
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/wechat_qrcode.pyi
+-rw-r--r--   0        0        0    40748 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/xfeatures2d.pyi
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/xphoto.pyi
+-rw-r--r--   0        0        0   105878 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/core.pyi
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/ie.pyi
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/oak.pyi
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/onnx.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/own.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/render.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/video.pyi
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/streaming/__init__.pyi
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/wip/__init__.pyi
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/wip/draw.pyi
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/wip/gst.pyi
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/kinfu/__init__.pyi
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/kinfu/detail.pyi
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/misc/__init__.pyi
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/misc/version.pyi
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/utils/__init__.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/utils/fs.pyi
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/utils/nested.pyi
+-rw-r--r--   0        0        0    80287 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/ximgproc/__init__.pyi
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/src/cv2-stubs/modules/ximgproc/segmentation.pyi
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/utils/add_missing_overloads.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/utils/generate_classes.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/utils/generate_constants.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/utils/generate_modules.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/utils/merge_with_microsoft_stubs.py
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/utils/processing_utils.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/utils/undefined_to_any.py
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/README.md
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 opencv_stubs-0.0.8/PKG-INFO
```

### Comparing `opencv_stubs-0.0.7/.pre-commit-config.yaml` & `opencv_stubs-0.0.8/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   autofix_commit_msg: "ci: [pre-commit.ci] auto fixes [...]"
   autoupdate_commit_msg: "ci: [pre-commit.ci] autoupdate"
   autofix_prs: true
   autoupdate_branch: ''
   submodules: false
 
 default_language_version:
-  python: python3.10
+  python: python3.11
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
```

### Comparing `opencv_stubs-0.0.7/requirements/requirements-build.txt` & `opencv_stubs-0.0.8/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/requirements/requirements-dev.txt` & `opencv_stubs-0.0.8/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/classes.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/classes.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/constants.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/functions.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/functions.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -757,19 +757,24 @@
     "extractChannel(src, coi[, dst]) -> dst\n.   @brief Extracts a single channel from src (coi is 0-based index)\n.   @param src input array\n.   @param dst output array\n.   @param coi index of channel to extract\n.   @sa mixChannels, split"
     ...
 
 def fastAtan2(y, x) -> Any:
     "fastAtan2(y, x) -> retval\n.   @brief Calculates the angle of a 2D vector in degrees.\n.   \n.    The function fastAtan2 calculates the full-range angle of an input 2D vector. The angle is measured\n.    in degrees and varies from 0 to 360 degrees. The accuracy is about 0.3 degrees.\n.    @param x x-coordinate of the vector.\n.    @param y y-coordinate of the vector."
     ...
 
-def fastNlMeansDenoising(src: npt.NDArray[_TImg], dst: npt.NDArray[_TImg] = ..., h=..., templateWindowSize=..., searchWindowSize=...) -> npt.NDArray[_TImg]:
+@overload
+def fastNlMeansDenoising(src: npt.NDArray[np.uint8], dst: npt.NDArray[np.uint8] = ..., h: float = 3, templateWindowSize: int = 7, searchWindowSize: int = 21) -> npt.NDArray[np.uint8]:
     "fastNlMeansDenoising(src[, dst[, h[, templateWindowSize[, searchWindowSize]]]]) -> dst\n.   @brief Perform image denoising using Non-local Means Denoising algorithm\n.   <http://www.ipol.im/pub/algo/bcm_non_local_means_denoising/> with several computational\n.   optimizations. Noise expected to be a gaussian white noise\n.   \n.   @param src Input 8-bit 1-channel, 2-channel, 3-channel or 4-channel image.\n.   @param dst Output image with the same size and type as src .\n.   @param templateWindowSize Size in pixels of the template patch that is used to compute weights.\n.   Should be odd. Recommended value 7 pixels\n.   @param searchWindowSize Size in pixels of the window that is used to compute weighted average for\n.   given pixel. Should be odd. Affect performance linearly: greater searchWindowsSize - greater\n.   denoising time. Recommended value 21 pixels\n.   @param h Parameter regulating filter strength. Big h value perfectly removes noise but also\n.   removes image details, smaller h value preserves details but also preserves some noise\n.   \n.   This function expected to be applied to grayscale images. For colored images look at\n.   fastNlMeansDenoisingColored. Advanced usage of this functions can be manual denoising of colored\n.   image in different colorspaces. Such approach is used in fastNlMeansDenoisingColored by converting\n.   image to CIELAB colorspace and then separately denoise L and AB components with different h\n.   parameter.\n\n\n\nfastNlMeansDenoising(src, h[, dst[, templateWindowSize[, searchWindowSize[, normType]]]]) -> dst\n.   @brief Perform image denoising using Non-local Means Denoising algorithm\n.   <http://www.ipol.im/pub/algo/bcm_non_local_means_denoising/> with several computational\n.   optimizations. Noise expected to be a gaussian white noise\n.   \n.   @param src Input 8-bit or 16-bit (only with NORM_L1) 1-channel,\n.   2-channel, 3-channel or 4-channel image.\n.   @param dst Output image with the same size and type as src .\n.   @param templateWindowSize Size in pixels of the template patch that is used to compute weights.\n.   Should be odd. Recommended value 7 pixels\n.   @param searchWindowSize Size in pixels of the window that is used to compute weighted average for\n.   given pixel. Should be odd. Affect performance linearly: greater searchWindowsSize - greater\n.   denoising time. Recommended value 21 pixels\n.   @param h Array of parameters regulating filter strength, either one\n.   parameter applied to all channels or one per channel in dst. Big h value\n.   perfectly removes noise but also removes image details, smaller h\n.   value preserves details but also preserves some noise\n.   @param normType Type of norm used for weight calculation. Can be either NORM_L2 or NORM_L1\n.   \n.   This function expected to be applied to grayscale images. For colored images look at\n.   fastNlMeansDenoisingColored. Advanced usage of this functions can be manual denoising of colored\n.   image in different colorspaces. Such approach is used in fastNlMeansDenoisingColored by converting\n.   image to CIELAB colorspace and then separately denoise L and AB components with different h\n.   parameter."
     ...
 
-def fastNlMeansDenoisingColored(src: npt.NDArray[_TImg], dst: npt.NDArray[_TImg] = ..., h=..., hColor=..., templateWindowSize=..., searchWindowSize=...) -> npt.NDArray[_TImg]:
+@overload
+def fastNlMeansDenoising(src: npt.NDArray[np.uint8], h: Sequence[float], dst: npt.NDArray[np.uint8] = ..., templateWindowSize: int = 7, searchWindowSize: int = 21, normType: int = NORM_L2) -> npt.NDArray[np.uint8]:
+    ...
+
+def fastNlMeansDenoisingColored(src: npt.NDArray[np.uint8], dst: npt.NDArray[np.uint8] = ..., h: float = 3, hColor: int = 3, templateWindowSize: int = 7, searchWindowSize: int = 21) -> npt.NDArray[np.uint8]:
     "fastNlMeansDenoisingColored(src[, dst[, h[, hColor[, templateWindowSize[, searchWindowSize]]]]]) -> dst\n.   @brief Modification of fastNlMeansDenoising function for colored images\n.   \n.   @param src Input 8-bit 3-channel image.\n.   @param dst Output image with the same size and type as src .\n.   @param templateWindowSize Size in pixels of the template patch that is used to compute weights.\n.   Should be odd. Recommended value 7 pixels\n.   @param searchWindowSize Size in pixels of the window that is used to compute weighted average for\n.   given pixel. Should be odd. Affect performance linearly: greater searchWindowsSize - greater\n.   denoising time. Recommended value 21 pixels\n.   @param h Parameter regulating filter strength for luminance component. Bigger h value perfectly\n.   removes noise but also removes image details, smaller h value preserves details but also preserves\n.   some noise\n.   @param hColor The same as h but for color components. For most images value equals 10\n.   will be enough to remove colored noise and do not distort colors\n.   \n.   The function converts image to CIELAB colorspace and then separately denoise L and AB components\n.   with given h parameters using fastNlMeansDenoising function."
     ...
 
 def fastNlMeansDenoisingColoredMulti(srcImgs: npt.NDArray[np.uint8], imgToDenoiseIndex: int, temporalWindowSize: int, dst: npt.NDArray[np.uint8] = ..., h: float = 3, hColor: float = 3, templateWindowSize: int = 7, searchWindowSize: int = 21) -> npt.NDArray[np.uint8]:
     "fastNlMeansDenoisingColoredMulti(srcImgs, imgToDenoiseIndex, temporalWindowSize[, dst[, h[, hColor[, templateWindowSize[, searchWindowSize]]]]]) -> dst\n.   @brief Modification of fastNlMeansDenoisingMulti function for colored images sequences\n.   \n.   @param srcImgs Input 8-bit 3-channel images sequence. All images should have the same type and\n.   size.\n.   @param imgToDenoiseIndex Target image to denoise index in srcImgs sequence\n.   @param temporalWindowSize Number of surrounding images to use for target image denoising. Should\n.   be odd. Images from imgToDenoiseIndex - temporalWindowSize / 2 to\n.   imgToDenoiseIndex - temporalWindowSize / 2 from srcImgs will be used to denoise\n.   srcImgs[imgToDenoiseIndex] image.\n.   @param dst Output image with the same size and type as srcImgs images.\n.   @param templateWindowSize Size in pixels of the template patch that is used to compute weights.\n.   Should be odd. Recommended value 7 pixels\n.   @param searchWindowSize Size in pixels of the window that is used to compute weighted average for\n.   given pixel. Should be odd. Affect performance linearly: greater searchWindowsSize - greater\n.   denoising time. Recommended value 21 pixels\n.   @param h Parameter regulating filter strength for luminance component. Bigger h value perfectly\n.   removes noise but also removes image details, smaller h value preserves details but also preserves\n.   some noise.\n.   @param hColor The same as h but for color components.\n.   \n.   The function converts images to CIELAB colorspace and then separately denoise L and AB components\n.   with given h parameters using fastNlMeansDenoisingMulti function."
     ...
```

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/__init__.py` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/aruco.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/aruco.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/barcode.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/barcode.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/bgsegm.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/bgsegm.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/bioinspired.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/bioinspired.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/ccm.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/ccm.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/colored_kinfu.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/colored_kinfu.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/cuda.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/cuda.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/datasets.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/datasets.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/detail.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/detail.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/dnn.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/dnn.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/dnn_superres.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/dnn_superres.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/dynafu.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/dynafu.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/error.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/error.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/face.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/face.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/fisheye.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/fisheye.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/flann.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/flann.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/ft.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/ft.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/hfs.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/hfs.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/img_hash.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/img_hash.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/intensity_transform.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/intensity_transform.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/large_kinfu.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/large_kinfu.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/legacy.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/legacy.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/line_descriptor.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/line_descriptor.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/linemod.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/linemod.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/mcc.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/mcc.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/ml.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/ml.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/motempl.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/motempl.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/ocl.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/ocl.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/ogl.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/ogl.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/omnidir.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/omnidir.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/optflow.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/optflow.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/phase_unwrapping.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/phase_unwrapping.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/plot.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/plot.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/ppf_match_3d.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/ppf_match_3d.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/quality.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/quality.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/rapid.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/rapid.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/reg.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/reg.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/rgbd.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/rgbd.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/saliency.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/saliency.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/samples.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/samples.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/segmentation.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/segmentation.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/stereo.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/stereo.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/structured_light.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/structured_light.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/text.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/text.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/videoio_registry.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/videoio_registry.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/wechat_qrcode.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/wechat_qrcode.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/xfeatures2d.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/xfeatures2d.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/xphoto.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/xphoto.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/__init__.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/ie.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/ie.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/oak.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/oak.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/streaming/__init__.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/streaming/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/__init__.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/wip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/draw.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/gapi/wip/draw.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/kinfu/__init__.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/kinfu/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/__init__.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/nested.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/utils/nested.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/ximgproc/__init__.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/ximgproc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/src/cv2-stubs/modules/ximgproc/segmentation.pyi` & `opencv_stubs-0.0.8/src/cv2-stubs/modules/ximgproc/segmentation.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/utils/add_missing_overloads.py` & `opencv_stubs-0.0.8/utils/add_missing_overloads.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/utils/generate_classes.py` & `opencv_stubs-0.0.8/utils/generate_classes.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/utils/generate_constants.py` & `opencv_stubs-0.0.8/utils/generate_constants.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/utils/generate_modules.py` & `opencv_stubs-0.0.8/utils/generate_modules.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/utils/merge_with_microsoft_stubs.py` & `opencv_stubs-0.0.8/utils/merge_with_microsoft_stubs.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/utils/processing_utils.py` & `opencv_stubs-0.0.8/utils/processing_utils.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/utils/undefined_to_any.py` & `opencv_stubs-0.0.8/utils/undefined_to_any.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/LICENSE` & `opencv_stubs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/README.md` & `opencv_stubs-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 This package includes all the functions, classes and constants (please open an issue if you find a missing one).\
 For some functions, OpenCV may handle more types than defined in this package. If you would like a type/function to be added or modified, please open an issue or a PR. There may also be a few errors as some types have been added progrmmatically. Please open an issue if you see one.
 The typing is still a work in progress, if you want a function/method to be added first you can open an issue.
 
 The stubs include the docstrings as they are otherwise not available in the IDE (as far as I know).
 
-These stubs are a temporary help until official ones are made (see [this issue](https://github.com/opencv/opencv/issues/14590)).
+These stubs are a temporary help until official ones are made (see [this issue](https://github.com/opencv/opencv/issues/14590) and [this PR](https://github.com/opencv/opencv/pull/20370)).
 
 
 ## Installation
 
 The package is available on pypi [here](https://pypi.org/project/opencv-stubs/), you can install it with:
 
 ```
```

### Comparing `opencv_stubs-0.0.7/pyproject.toml` & `opencv_stubs-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.7/PKG-INFO` & `opencv_stubs-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv-stubs
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unofficial stubs for the opencv-python package.
 Project-URL: Homepage, https://github.com/hoel-bagard/opencv-stubs
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/opencv-stubs/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE
 Keywords: OpenCV,stubs
@@ -60,15 +60,15 @@
 
 This package includes all the functions, classes and constants (please open an issue if you find a missing one).\
 For some functions, OpenCV may handle more types than defined in this package. If you would like a type/function to be added or modified, please open an issue or a PR. There may also be a few errors as some types have been added progrmmatically. Please open an issue if you see one.
 The typing is still a work in progress, if you want a function/method to be added first you can open an issue.
 
 The stubs include the docstrings as they are otherwise not available in the IDE (as far as I know).
 
-These stubs are a temporary help until official ones are made (see [this issue](https://github.com/opencv/opencv/issues/14590)).
+These stubs are a temporary help until official ones are made (see [this issue](https://github.com/opencv/opencv/issues/14590) and [this PR](https://github.com/opencv/opencv/pull/20370)).
 
 
 ## Installation
 
 The package is available on pypi [here](https://pypi.org/project/opencv-stubs/), you can install it with:
 
 ```
```

