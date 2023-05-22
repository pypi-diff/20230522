# Comparing `tmp/SRPAstro.FITS-2.9.7.tar.gz` & `tmp/SRPAstro.FITS-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SRPAstro.FITS-2.9.7.tar", last modified: Tue Mar 15 15:47:48 2022, max compression
+gzip compressed data, was "SRPAstro.FITS-3.0.1.tar", last modified: Mon May 22 10:07:50 2023, max compression
```

## Comparing `SRPAstro.FITS-2.9.7.tar` & `SRPAstro.FITS-3.0.1.tar`

### file list

```diff
@@ -1,164 +1,167 @@
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/Docs/
--rw-------   0 covino     (501) staff       (20)   142337 2017-02-21 14:33:07.000000 SRPAstro.FITS-2.9.7/Docs/SRPAstro.FITS.pdf
--rw-r--r--   0 covino     (501) staff       (20)     1081 2019-05-07 09:54:08.000000 SRPAstro.FITS-2.9.7/LICENSE.txt
--rw-r--r--   0 covino     (501) staff       (20)      258 2020-03-04 14:45:54.000000 SRPAstro.FITS-2.9.7/MANIFEST.in
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/Misc/
--rw-------   0 covino     (501) staff       (20)     1288 2019-05-22 19:31:58.000000 SRPAstro.FITS-2.9.7/Misc/ApyPhot.py
--rw-------   0 covino     (501) staff       (20)    23044 2021-02-02 11:59:14.000000 SRPAstro.FITS-2.9.7/Misc/AstrometryClass.py
--rw-r--r--   0 covino     (501) staff       (20)     1601 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/PKG-INFO
--rw-r--r--   0 covino     (501) staff       (20)      744 2019-07-22 12:26:27.000000 SRPAstro.FITS-2.9.7/README.md
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/SRPAstro.FITS.egg-info/
--rw-------   0 covino     (501) staff       (20)     1601 2022-03-15 15:47:47.000000 SRPAstro.FITS-2.9.7/SRPAstro.FITS.egg-info/PKG-INFO
--rw-------   0 covino     (501) staff       (20)     6447 2022-03-15 15:47:47.000000 SRPAstro.FITS-2.9.7/SRPAstro.FITS.egg-info/SOURCES.txt
--rw-------   0 covino     (501) staff       (20)        1 2022-03-15 15:47:47.000000 SRPAstro.FITS-2.9.7/SRPAstro.FITS.egg-info/dependency_links.txt
--rw-------   0 covino     (501) staff       (20)       62 2022-03-15 15:47:47.000000 SRPAstro.FITS-2.9.7/SRPAstro.FITS.egg-info/requires.txt
--rw-------   0 covino     (501) staff       (20)        8 2022-03-15 15:47:47.000000 SRPAstro.FITS-2.9.7/SRPAstro.FITS.egg-info/top_level.txt
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/SRPFITS/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/
--rw-r--r--   0 covino     (501) staff       (20)     8196 2020-03-04 14:48:58.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/.DS_Store
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/
--rw-------   0 covino     (501) staff       (20)       88 2010-09-28 13:27:42.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPConvIn
--rw-------   0 covino     (501) staff       (20)      332 2010-09-28 13:33:03.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPConvLSLASCIn
--rw-------   0 covino     (501) staff       (20)     2165 2010-09-28 13:30:00.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPNnwIn
--rw-------   0 covino     (501) staff       (20)      179 2013-12-06 14:18:19.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPParamIn
--rw-------   0 covino     (501) staff       (20)      750 2010-09-28 13:31:35.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexIn
--rw-------   0 covino     (501) staff       (20)      749 2010-09-28 13:33:53.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexLSLASCIn
--rw-------   0 covino     (501) staff       (20)      752 2012-01-25 16:07:42.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexREMREMIRIn
--rw-------   0 covino     (501) staff       (20)      750 2013-08-18 20:17:05.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexREMROS2In
--rw-------   0 covino     (501) staff       (20)      751 2012-04-01 19:58:22.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexREMROSSIn
--rw-------   0 covino     (501) staff       (20)      750 2010-09-28 13:53:56.000000 SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexTNGLRSIn
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/
--rw-------   0 covino     (501) staff       (20)     1930 2017-05-18 14:30:00.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/AddHeaderComment.py
--rw-------   0 covino     (501) staff       (20)     2612 2021-07-08 08:39:43.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/AddHeaderEntry.py
--rw-------   0 covino     (501) staff       (20)     1967 2015-07-23 12:13:33.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/FitsConstants.py
--rw-------   0 covino     (501) staff       (20)     8608 2021-03-02 15:35:24.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/FitsImageClass.py
--rw-------   0 covino     (501) staff       (20)      869 2015-07-23 12:13:58.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/FitsTabsAppend.py
--rw-------   0 covino     (501) staff       (20)      760 2017-05-18 14:34:24.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetData.py
--rw-------   0 covino     (501) staff       (20)      802 2017-05-18 14:35:11.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetHeader.py
--rw-------   0 covino     (501) staff       (20)      875 2017-05-18 14:35:28.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetHeaderValue.py
--rw-------   0 covino     (501) staff       (20)      997 2017-05-18 13:39:55.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetSpectrum.py
--rw-------   0 covino     (501) staff       (20)      586 2015-07-23 12:34:36.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetSpectrumPosition.py
--rw-------   0 covino     (501) staff       (20)     1424 2021-02-09 12:48:15.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetWCS.py
--rw-------   0 covino     (501) staff       (20)      702 2017-08-22 21:04:15.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/IsFits.py
--rw-------   0 covino     (501) staff       (20)      437 2021-01-14 10:07:28.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/WCSPixelScale.py
--rw-------   0 covino     (501) staff       (20)      567 2021-01-14 10:40:27.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/WCSRotationDeg.py
--rw-------   0 covino     (501) staff       (20)      804 2021-01-14 10:07:37.000000 SRPAstro.FITS-2.9.7/SRPFITS/Fits/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/
--rw-------   0 covino     (501) staff       (20)    24425 2021-03-17 08:46:10.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/AstrometryClass.py
--rw-------   0 covino     (501) staff       (20)     2810 2021-03-02 15:30:39.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/DAOObjectClass.py
--rw-------   0 covino     (501) staff       (20)      425 2015-07-23 12:15:58.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/EclipseConstants.py
--rw-------   0 covino     (501) staff       (20)     2636 2017-05-16 09:56:28.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/EclipseObjectClass.py
--rw-------   0 covino     (501) staff       (20)      853 2020-05-14 16:28:39.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/Pixel2WCS.py
--rw-------   0 covino     (501) staff       (20)     1394 2020-05-14 13:44:46.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/SExtractorConstants.py
--rw-------   0 covino     (501) staff       (20)      361 2015-07-23 12:16:42.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/SexConstants.py
--rw-------   0 covino     (501) staff       (20)     2562 2020-12-11 12:24:32.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/SexObjectClass.py
--rw-------   0 covino     (501) staff       (20)     5248 2017-05-26 14:52:54.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/SourceObjectsClass.py
--rw-------   0 covino     (501) staff       (20)      865 2020-05-14 14:24:01.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/WCS2Pixel.py
--rw-------   0 covino     (501) staff       (20)      588 2017-05-16 09:52:29.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/__init__.py
--rw-------   0 covino     (501) staff       (20)      637 2020-03-07 14:00:40.000000 SRPAstro.FITS-2.9.7/SRPFITS/Frames/getCenterRADEC.py
--rw-------   0 covino     (501) staff       (20)     1049 2017-07-03 14:29:49.000000 SRPAstro.FITS-2.9.7/SRPFITS/GetFWHM.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/SRPFITS/Math/
--rw-------   0 covino     (501) staff       (20)     8163 2021-07-06 13:46:23.000000 SRPAstro.FITS-2.9.7/SRPFITS/Math/TriangleMatch.py
--rw-------   0 covino     (501) staff       (20)      331 2017-03-14 08:48:57.000000 SRPAstro.FITS-2.9.7/SRPFITS/Math/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/
--rw-------   0 covino     (501) staff       (20)     1126 2017-04-19 13:53:05.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/ApErr.py
--rw-------   0 covino     (501) staff       (20)     2903 2020-10-05 08:41:16.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/ApyPhot.py
--rw-------   0 covino     (501) staff       (20)      520 2015-12-11 15:46:16.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/Counts2Mag.py
--rw-------   0 covino     (501) staff       (20)      884 2017-08-30 19:36:03.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/DaoPhot.py
--rw-------   0 covino     (501) staff       (20)      503 2015-07-23 12:26:20.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/Mag2Counts.py
--rw-------   0 covino     (501) staff       (20)     1086 2015-11-13 14:11:34.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/MinMax.py
--rw-------   0 covino     (501) staff       (20)      767 2017-08-24 08:25:46.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/__init__.py
--rw-------   0 covino     (501) staff       (20)     1142 2017-04-19 13:45:07.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/centerGauss.py
--rw-------   0 covino     (501) staff       (20)     1653 2020-03-07 16:49:45.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/centerMoment.py
--rw-------   0 covino     (501) staff       (20)     1563 2017-08-24 08:53:55.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/centerObj.py
--rw-------   0 covino     (501) staff       (20)     1281 2015-11-13 10:37:46.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/getBackground.py
--rw-------   0 covino     (501) staff       (20)      803 2015-11-10 10:11:17.000000 SRPAstro.FITS-2.9.7/SRPFITS/Photometry/resid.py
--rw-------   0 covino     (501) staff       (20)      521 2021-06-02 20:51:07.000000 SRPAstro.FITS-2.9.7/SRPFITS/SRPFITSPath.py
--rw-------   0 covino     (501) staff       (20)     2384 2022-03-15 15:34:28.000000 SRPAstro.FITS-2.9.7/SRPFITS/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/Scripts/
--rw-------   0 covino     (501) staff       (20)    10932 2021-09-07 09:46:26.000000 SRPAstro.FITS-2.9.7/Scripts/SRPAdvAverage
--rw-------   0 covino     (501) staff       (20)     5242 2021-05-12 11:29:46.000000 SRPAstro.FITS-2.9.7/Scripts/SRPAlignImaging
--rw-------   0 covino     (501) staff       (20)    10433 2021-05-12 11:29:59.000000 SRPAstro.FITS-2.9.7/Scripts/SRPAstrometry
--rw-------   0 covino     (501) staff       (20)     5660 2021-05-12 11:30:11.000000 SRPAstro.FITS-2.9.7/Scripts/SRPAverage
--rw-------   0 covino     (501) staff       (20)     6023 2021-11-16 10:55:28.000000 SRPAstro.FITS-2.9.7/Scripts/SRPBias
--rw-------   0 covino     (501) staff       (20)     3831 2021-05-12 11:30:35.000000 SRPAstro.FITS-2.9.7/Scripts/SRPClassify
--rw-------   0 covino     (501) staff       (20)     7083 2021-05-12 11:30:47.000000 SRPAstro.FITS-2.9.7/Scripts/SRPCut
--rw-------   0 covino     (501) staff       (20)     8464 2021-05-12 11:30:59.000000 SRPAstro.FITS-2.9.7/Scripts/SRPDao2Sky
--rw-------   0 covino     (501) staff       (20)      800 2021-05-12 11:32:34.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFITSVersion
--rw-------   0 covino     (501) staff       (20)     4492 2021-05-12 11:31:10.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFindingChart
--rw-------   0 covino     (501) staff       (20)     3692 2021-05-12 11:31:22.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFitsComposer
--rw-------   0 covino     (501) staff       (20)     6038 2021-05-12 11:31:34.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFitsExtension
--rw-------   0 covino     (501) staff       (20)     3932 2021-05-12 11:31:45.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFitsHeaders
--rw-------   0 covino     (501) staff       (20)     3610 2021-05-12 11:31:59.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFitsSpectrum2ASCII
--rw-------   0 covino     (501) staff       (20)     4314 2021-05-12 11:32:11.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFitsStats
--rw-------   0 covino     (501) staff       (20)     1629 2021-05-12 11:32:22.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFitsTableViewer
--rw-------   0 covino     (501) staff       (20)     7891 2021-11-16 10:55:33.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFlatImaging
--rw-------   0 covino     (501) staff       (20)     9184 2021-11-16 10:56:34.000000 SRPAstro.FITS-2.9.7/Scripts/SRPFlatSpectroscopy
--rw-------   0 covino     (501) staff       (20)     5995 2021-05-12 11:33:10.000000 SRPAstro.FITS-2.9.7/Scripts/SRPGAIA2Sky
--rw-------   0 covino     (501) staff       (20)     7324 2021-05-12 11:33:22.000000 SRPAstro.FITS-2.9.7/Scripts/SRPImageFilter
--rw-------   0 covino     (501) staff       (20)    18556 2022-03-15 15:41:57.000000 SRPAstro.FITS-2.9.7/Scripts/SRPImageMapping
--rw-------   0 covino     (501) staff       (20)     4975 2021-05-12 11:33:46.000000 SRPAstro.FITS-2.9.7/Scripts/SRPKeywords
--rw-------   0 covino     (501) staff       (20)     2948 2021-05-12 11:34:10.000000 SRPAstro.FITS-2.9.7/Scripts/SRPPhotParSet
--rw-------   0 covino     (501) staff       (20)    12835 2021-05-12 11:33:58.000000 SRPAstro.FITS-2.9.7/Scripts/SRPPhotometry
--rw-------   0 covino     (501) staff       (20)    10876 2021-05-12 11:34:22.000000 SRPAstro.FITS-2.9.7/Scripts/SRPQuery
--rw-------   0 covino     (501) staff       (20)     5424 2021-05-12 11:34:46.000000 SRPAstro.FITS-2.9.7/Scripts/SRPRTAlignImaging
--rw-------   0 covino     (501) staff       (20)     7670 2021-09-07 09:42:34.000000 SRPAstro.FITS-2.9.7/Scripts/SRPRotoTransla
--rw-------   0 covino     (501) staff       (20)     8456 2021-05-12 11:34:57.000000 SRPAstro.FITS-2.9.7/Scripts/SRPScienceFramesImaging
--rw-------   0 covino     (501) staff       (20)     4797 2021-05-12 11:35:11.000000 SRPAstro.FITS-2.9.7/Scripts/SRPSourceFinder
--rw-------   0 covino     (501) staff       (20)     7534 2021-05-12 11:35:23.000000 SRPAstro.FITS-2.9.7/Scripts/SRPSpectralExtraction
--rw-------   0 covino     (501) staff       (20)     5488 2021-05-12 11:35:35.000000 SRPAstro.FITS-2.9.7/Scripts/SRPWCSPixel
--rw-------   0 covino     (501) staff       (20)     7247 2021-06-02 09:56:24.000000 SRPAstro.FITS-2.9.7/Scripts/SRPZeroPoint
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/build/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/build/lib/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/
--rw-r--r--   0 covino     (501) staff       (20)     1930 2017-05-18 14:30:00.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/AddHeaderComment.py
--rw-r--r--   0 covino     (501) staff       (20)     2612 2021-07-08 08:39:43.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/AddHeaderEntry.py
--rw-r--r--   0 covino     (501) staff       (20)     1967 2015-07-23 12:13:33.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/FitsConstants.py
--rw-r--r--   0 covino     (501) staff       (20)     8608 2021-03-02 15:35:24.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/FitsImageClass.py
--rw-r--r--   0 covino     (501) staff       (20)      869 2015-07-23 12:13:58.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/FitsTabsAppend.py
--rw-r--r--   0 covino     (501) staff       (20)      760 2017-05-18 14:34:24.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetData.py
--rw-r--r--   0 covino     (501) staff       (20)      802 2017-05-18 14:35:11.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetHeader.py
--rw-r--r--   0 covino     (501) staff       (20)      875 2017-05-18 14:35:28.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetHeaderValue.py
--rw-r--r--   0 covino     (501) staff       (20)      997 2017-05-18 13:39:55.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetSpectrum.py
--rw-r--r--   0 covino     (501) staff       (20)      586 2015-07-23 12:34:36.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetSpectrumPosition.py
--rw-r--r--   0 covino     (501) staff       (20)     1424 2021-02-09 12:48:15.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetWCS.py
--rw-r--r--   0 covino     (501) staff       (20)      702 2017-08-22 21:04:15.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/IsFits.py
--rw-r--r--   0 covino     (501) staff       (20)      437 2021-01-14 10:07:28.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/WCSPixelScale.py
--rw-r--r--   0 covino     (501) staff       (20)      567 2021-01-14 10:40:27.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/WCSRotationDeg.py
--rw-r--r--   0 covino     (501) staff       (20)      804 2021-01-14 10:07:37.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/
--rw-r--r--   0 covino     (501) staff       (20)    24425 2021-03-17 08:46:10.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/AstrometryClass.py
--rw-r--r--   0 covino     (501) staff       (20)     2810 2021-03-02 15:30:39.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/DAOObjectClass.py
--rw-r--r--   0 covino     (501) staff       (20)      425 2015-07-23 12:15:58.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/EclipseConstants.py
--rw-r--r--   0 covino     (501) staff       (20)     2636 2017-05-16 09:56:28.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/EclipseObjectClass.py
--rw-r--r--   0 covino     (501) staff       (20)      853 2020-05-14 16:28:39.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/Pixel2WCS.py
--rw-r--r--   0 covino     (501) staff       (20)     1394 2020-05-14 13:44:46.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/SExtractorConstants.py
--rw-r--r--   0 covino     (501) staff       (20)      361 2015-07-23 12:16:42.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/SexConstants.py
--rw-r--r--   0 covino     (501) staff       (20)     2562 2020-12-11 12:24:32.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/SexObjectClass.py
--rw-r--r--   0 covino     (501) staff       (20)     5248 2017-05-26 14:52:54.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/SourceObjectsClass.py
--rw-r--r--   0 covino     (501) staff       (20)      865 2020-05-14 14:24:01.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/WCS2Pixel.py
--rw-r--r--   0 covino     (501) staff       (20)      588 2017-05-16 09:52:29.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/__init__.py
--rw-r--r--   0 covino     (501) staff       (20)      637 2020-03-07 14:00:40.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/getCenterRADEC.py
--rw-r--r--   0 covino     (501) staff       (20)     1049 2017-07-03 14:29:49.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/GetFWHM.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Math/
--rw-r--r--   0 covino     (501) staff       (20)     8163 2021-07-06 13:46:23.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Math/TriangleMatch.py
--rw-r--r--   0 covino     (501) staff       (20)      331 2017-03-14 08:48:57.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Math/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/
--rw-r--r--   0 covino     (501) staff       (20)     1126 2017-04-19 13:53:05.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/ApErr.py
--rw-r--r--   0 covino     (501) staff       (20)     2903 2020-10-05 08:41:16.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/ApyPhot.py
--rw-r--r--   0 covino     (501) staff       (20)      520 2015-12-11 15:46:16.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/Counts2Mag.py
--rw-r--r--   0 covino     (501) staff       (20)      884 2017-08-30 19:36:03.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/DaoPhot.py
--rw-r--r--   0 covino     (501) staff       (20)      503 2015-07-23 12:26:20.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/Mag2Counts.py
--rw-r--r--   0 covino     (501) staff       (20)     1086 2015-11-13 14:11:34.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/MinMax.py
--rw-r--r--   0 covino     (501) staff       (20)      767 2017-08-24 08:25:46.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/__init__.py
--rw-r--r--   0 covino     (501) staff       (20)     1142 2017-04-19 13:45:07.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/centerGauss.py
--rw-r--r--   0 covino     (501) staff       (20)     1653 2020-03-07 16:49:45.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/centerMoment.py
--rw-r--r--   0 covino     (501) staff       (20)     1563 2017-08-24 08:53:55.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/centerObj.py
--rw-r--r--   0 covino     (501) staff       (20)     1281 2015-11-13 10:37:46.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/getBackground.py
--rw-r--r--   0 covino     (501) staff       (20)      803 2015-11-10 10:11:17.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/resid.py
--rw-r--r--   0 covino     (501) staff       (20)      521 2021-06-02 20:51:07.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/SRPFITSPath.py
--rw-r--r--   0 covino     (501) staff       (20)     2384 2022-03-15 15:34:28.000000 SRPAstro.FITS-2.9.7/build/lib/SRPFITS/__init__.py
--rw-r--r--   0 covino     (501) staff       (20)      107 2022-03-15 15:47:48.000000 SRPAstro.FITS-2.9.7/setup.cfg
--rw-------   0 covino     (501) staff       (20)     1713 2021-07-06 09:46:21.000000 SRPAstro.FITS-2.9.7/setup.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:50.568093 SRPAstro.FITS-3.0.1/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.798141 SRPAstro.FITS-3.0.1/Docs/
+-rw-------   0 covino     (501) staff       (20)   142337 2017-02-21 14:33:07.000000 SRPAstro.FITS-3.0.1/Docs/SRPAstro.FITS.pdf
+-rw-r--r--   0 covino     (501) staff       (20)     1081 2019-05-07 09:54:08.000000 SRPAstro.FITS-3.0.1/LICENSE.txt
+-rw-r--r--   0 covino     (501) staff       (20)      258 2020-03-04 14:45:54.000000 SRPAstro.FITS-3.0.1/MANIFEST.in
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.156475 SRPAstro.FITS-3.0.1/Misc/
+-rw-------   0 covino     (501) staff       (20)     1288 2019-05-22 19:31:58.000000 SRPAstro.FITS-3.0.1/Misc/ApyPhot.py
+-rw-------   0 covino     (501) staff       (20)    23044 2021-02-02 11:59:14.000000 SRPAstro.FITS-3.0.1/Misc/AstrometryClass.py
+-rw-r--r--   0 covino     (501) staff       (20)     1507 2023-05-22 10:07:50.568275 SRPAstro.FITS-3.0.1/PKG-INFO
+-rw-r--r--   0 covino     (501) staff       (20)      744 2019-07-22 12:26:27.000000 SRPAstro.FITS-3.0.1/README.md
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.886749 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/
+-rw-------   0 covino     (501) staff       (20)     1507 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/PKG-INFO
+-rw-------   0 covino     (501) staff       (20)     6615 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/SOURCES.txt
+-rw-------   0 covino     (501) staff       (20)        1 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/dependency_links.txt
+-rw-------   0 covino     (501) staff       (20)       62 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/requires.txt
+-rw-------   0 covino     (501) staff       (20)        8 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/top_level.txt
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.209299 SRPAstro.FITS-3.0.1/SRPFITS/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.887494 SRPAstro.FITS-3.0.1/SRPFITS/Data/
+-rw-r--r--   0 covino     (501) staff       (20)     8196 2020-03-04 14:48:58.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/.DS_Store
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.943726 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/
+-rw-------   0 covino     (501) staff       (20)       88 2010-09-28 13:27:42.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPConvIn
+-rw-------   0 covino     (501) staff       (20)      332 2010-09-28 13:33:03.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPConvLSLASCIn
+-rw-------   0 covino     (501) staff       (20)     2165 2010-09-28 13:30:00.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPNnwIn
+-rw-------   0 covino     (501) staff       (20)      179 2013-12-06 14:18:19.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPParamIn
+-rw-------   0 covino     (501) staff       (20)      750 2010-09-28 13:31:35.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexIn
+-rw-------   0 covino     (501) staff       (20)      749 2010-09-28 13:33:53.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexLSLASCIn
+-rw-------   0 covino     (501) staff       (20)      752 2012-01-25 16:07:42.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMREMIRIn
+-rw-------   0 covino     (501) staff       (20)      750 2013-08-18 20:17:05.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMROS2In
+-rw-------   0 covino     (501) staff       (20)      751 2012-04-01 19:58:22.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMROSSIn
+-rw-------   0 covino     (501) staff       (20)      750 2010-09-28 13:53:56.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexTNGLRSIn
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.326117 SRPAstro.FITS-3.0.1/SRPFITS/Fits/
+-rw-------   0 covino     (501) staff       (20)     1930 2017-05-18 14:30:00.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/AddHeaderComment.py
+-rw-------   0 covino     (501) staff       (20)     2612 2021-07-08 08:39:43.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/AddHeaderEntry.py
+-rw-------   0 covino     (501) staff       (20)     1967 2015-07-23 12:13:33.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsConstants.py
+-rw-------   0 covino     (501) staff       (20)     8608 2021-03-02 15:35:24.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsImageClass.py
+-rw-------   0 covino     (501) staff       (20)      869 2015-07-23 12:13:58.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsTabsAppend.py
+-rw-------   0 covino     (501) staff       (20)      760 2017-05-18 14:34:24.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetData.py
+-rw-------   0 covino     (501) staff       (20)      802 2017-05-18 14:35:11.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetHeader.py
+-rw-------   0 covino     (501) staff       (20)      875 2017-05-18 14:35:28.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetHeaderValue.py
+-rw-------   0 covino     (501) staff       (20)      997 2017-05-18 13:39:55.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetSpectrum.py
+-rw-------   0 covino     (501) staff       (20)      586 2015-07-23 12:34:36.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetSpectrumPosition.py
+-rw-------   0 covino     (501) staff       (20)     1424 2021-02-09 12:48:15.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetWCS.py
+-rw-------   0 covino     (501) staff       (20)      702 2017-08-22 21:04:15.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/IsFits.py
+-rw-------   0 covino     (501) staff       (20)      437 2021-01-14 10:07:28.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/WCSPixelScale.py
+-rw-------   0 covino     (501) staff       (20)      567 2021-01-14 10:40:27.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/WCSRotationDeg.py
+-rw-------   0 covino     (501) staff       (20)      799 2022-08-10 13:01:02.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.483192 SRPAstro.FITS-3.0.1/SRPFITS/Frames/
+-rw-------   0 covino     (501) staff       (20)    24425 2021-03-17 08:46:10.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/AstrometryClass.py
+-rw-------   0 covino     (501) staff       (20)     2810 2021-03-02 15:30:39.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/DAOObjectClass.py
+-rw-------   0 covino     (501) staff       (20)      425 2015-07-23 12:15:58.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/EclipseConstants.py
+-rw-------   0 covino     (501) staff       (20)     2636 2017-05-16 09:56:28.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/EclipseObjectClass.py
+-rw-------   0 covino     (501) staff       (20)      853 2020-05-14 16:28:39.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/Pixel2WCS.py
+-rw-------   0 covino     (501) staff       (20)     1394 2020-05-14 13:44:46.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/SExtractorConstants.py
+-rw-------   0 covino     (501) staff       (20)      361 2015-07-23 12:16:42.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/SexConstants.py
+-rw-------   0 covino     (501) staff       (20)     2562 2020-12-11 12:24:32.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/SexObjectClass.py
+-rw-------   0 covino     (501) staff       (20)     5248 2017-05-26 14:52:54.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/SourceObjectsClass.py
+-rw-------   0 covino     (501) staff       (20)      865 2020-05-14 14:24:01.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/WCS2Pixel.py
+-rw-------   0 covino     (501) staff       (20)      588 2017-05-16 09:52:29.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/__init__.py
+-rw-------   0 covino     (501) staff       (20)      637 2020-03-07 14:00:40.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/getCenterRADEC.py
+-rw-------   0 covino     (501) staff       (20)     1086 2023-05-22 09:48:40.000000 SRPAstro.FITS-3.0.1/SRPFITS/GetFWHM.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.525095 SRPAstro.FITS-3.0.1/SRPFITS/Math/
+-rw-------   0 covino     (501) staff       (20)     8163 2021-07-06 13:46:23.000000 SRPAstro.FITS-3.0.1/SRPFITS/Math/TriangleMatch.py
+-rw-------   0 covino     (501) staff       (20)      331 2017-03-14 08:48:57.000000 SRPAstro.FITS-3.0.1/SRPFITS/Math/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.598386 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/
+-rw-------   0 covino     (501) staff       (20)     1126 2017-04-19 13:53:05.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/ApErr.py
+-rw-------   0 covino     (501) staff       (20)     2903 2020-10-05 08:41:16.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/ApyPhot.py
+-rw-------   0 covino     (501) staff       (20)      520 2015-12-11 15:46:16.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/Counts2Mag.py
+-rw-------   0 covino     (501) staff       (20)      884 2017-08-30 19:36:03.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/DaoPhot.py
+-rw-------   0 covino     (501) staff       (20)     5146 2023-05-22 10:06:44.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/FitsPhotometryClass.py
+-rw-------   0 covino     (501) staff       (20)      503 2015-07-23 12:26:20.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/Mag2Counts.py
+-rw-------   0 covino     (501) staff       (20)     1086 2015-11-13 14:11:34.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/MinMax.py
+-rw-------   0 covino     (501) staff       (20)      849 2022-08-10 13:00:32.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/__init__.py
+-rw-------   0 covino     (501) staff       (20)     1142 2017-04-19 13:45:07.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerGauss.py
+-rw-------   0 covino     (501) staff       (20)     1653 2020-03-07 16:49:45.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerMoment.py
+-rw-------   0 covino     (501) staff       (20)     1563 2017-08-24 08:53:55.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerObj.py
+-rw-------   0 covino     (501) staff       (20)     1281 2015-11-13 10:37:46.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/getBackground.py
+-rw-------   0 covino     (501) staff       (20)      803 2015-11-10 10:11:17.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/resid.py
+-rw-------   0 covino     (501) staff       (20)      521 2021-06-02 20:51:07.000000 SRPAstro.FITS-3.0.1/SRPFITS/SRPFITSPath.py
+-rw-------   0 covino     (501) staff       (20)     2481 2023-05-22 09:48:36.000000 SRPAstro.FITS-3.0.1/SRPFITS/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:50.539089 SRPAstro.FITS-3.0.1/Scripts/
+-rw-------   0 covino     (501) staff       (20)    10932 2021-09-07 09:46:26.000000 SRPAstro.FITS-3.0.1/Scripts/SRPAdvAverage
+-rw-------   0 covino     (501) staff       (20)     5242 2021-05-12 11:29:46.000000 SRPAstro.FITS-3.0.1/Scripts/SRPAlignImaging
+-rw-------   0 covino     (501) staff       (20)    10433 2021-05-12 11:29:59.000000 SRPAstro.FITS-3.0.1/Scripts/SRPAstrometry
+-rw-------   0 covino     (501) staff       (20)     5660 2021-05-12 11:30:11.000000 SRPAstro.FITS-3.0.1/Scripts/SRPAverage
+-rw-------   0 covino     (501) staff       (20)     6023 2021-11-16 10:55:28.000000 SRPAstro.FITS-3.0.1/Scripts/SRPBias
+-rw-------   0 covino     (501) staff       (20)     3831 2021-05-12 11:30:35.000000 SRPAstro.FITS-3.0.1/Scripts/SRPClassify
+-rw-------   0 covino     (501) staff       (20)     7083 2021-05-12 11:30:47.000000 SRPAstro.FITS-3.0.1/Scripts/SRPCut
+-rw-------   0 covino     (501) staff       (20)     8464 2021-05-12 11:30:59.000000 SRPAstro.FITS-3.0.1/Scripts/SRPDao2Sky
+-rw-------   0 covino     (501) staff       (20)      800 2021-05-12 11:32:34.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFITSVersion
+-rw-------   0 covino     (501) staff       (20)     4492 2021-05-12 11:31:10.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFindingChart
+-rw-------   0 covino     (501) staff       (20)     3692 2021-05-12 11:31:22.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsComposer
+-rw-------   0 covino     (501) staff       (20)     6038 2021-05-12 11:31:34.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsExtension
+-rw-------   0 covino     (501) staff       (20)     3932 2021-05-12 11:31:45.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsHeaders
+-rw-------   0 covino     (501) staff       (20)     3648 2022-12-02 13:10:06.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsSpectrum2ASCII
+-rw-------   0 covino     (501) staff       (20)     4314 2021-05-12 11:32:11.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsStats
+-rw-------   0 covino     (501) staff       (20)     1629 2021-05-12 11:32:22.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsTableViewer
+-rw-------   0 covino     (501) staff       (20)     7891 2021-11-16 10:55:33.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFlatImaging
+-rw-------   0 covino     (501) staff       (20)     9184 2021-11-16 10:56:34.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFlatSpectroscopy
+-rw-------   0 covino     (501) staff       (20)     5995 2021-05-12 11:33:10.000000 SRPAstro.FITS-3.0.1/Scripts/SRPGAIA2Sky
+-rw-------   0 covino     (501) staff       (20)     7324 2021-05-12 11:33:22.000000 SRPAstro.FITS-3.0.1/Scripts/SRPImageFilter
+-rw-------   0 covino     (501) staff       (20)    18568 2022-03-15 18:19:50.000000 SRPAstro.FITS-3.0.1/Scripts/SRPImageMapping
+-rw-------   0 covino     (501) staff       (20)     4975 2021-05-12 11:33:46.000000 SRPAstro.FITS-3.0.1/Scripts/SRPKeywords
+-rw-------   0 covino     (501) staff       (20)     2948 2021-05-12 11:34:10.000000 SRPAstro.FITS-3.0.1/Scripts/SRPPhotParSet
+-rw-------   0 covino     (501) staff       (20)    12835 2021-05-12 11:33:58.000000 SRPAstro.FITS-3.0.1/Scripts/SRPPhotometry
+-rw-------   0 covino     (501) staff       (20)    10876 2021-05-12 11:34:22.000000 SRPAstro.FITS-3.0.1/Scripts/SRPQuery
+-rw-------   0 covino     (501) staff       (20)     5424 2021-05-12 11:34:46.000000 SRPAstro.FITS-3.0.1/Scripts/SRPRTAlignImaging
+-rw-------   0 covino     (501) staff       (20)     7670 2021-09-07 09:42:34.000000 SRPAstro.FITS-3.0.1/Scripts/SRPRotoTransla
+-rw-------   0 covino     (501) staff       (20)     8456 2021-05-12 11:34:57.000000 SRPAstro.FITS-3.0.1/Scripts/SRPScienceFramesImaging
+-rw-------   0 covino     (501) staff       (20)     4835 2023-05-22 10:03:42.000000 SRPAstro.FITS-3.0.1/Scripts/SRPSourceFinder
+-rw-------   0 covino     (501) staff       (20)     3966 2023-05-22 10:05:47.000000 SRPAstro.FITS-3.0.1/Scripts/SRPSourcePhotometry
+-rw-------   0 covino     (501) staff       (20)     7534 2021-05-12 11:35:23.000000 SRPAstro.FITS-3.0.1/Scripts/SRPSpectralExtraction
+-rw-------   0 covino     (501) staff       (20)     5488 2021-05-12 11:35:35.000000 SRPAstro.FITS-3.0.1/Scripts/SRPWCSPixel
+-rw-------   0 covino     (501) staff       (20)     7247 2021-06-02 09:56:24.000000 SRPAstro.FITS-3.0.1/Scripts/SRPZeroPoint
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.097822 SRPAstro.FITS-3.0.1/build/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.097969 SRPAstro.FITS-3.0.1/build/lib/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.633581 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.741131 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/
+-rw-------   0 covino     (501) staff       (20)     1930 2017-05-18 14:30:00.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/AddHeaderComment.py
+-rw-------   0 covino     (501) staff       (20)     2612 2021-07-08 08:39:43.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/AddHeaderEntry.py
+-rw-------   0 covino     (501) staff       (20)     1967 2015-07-23 12:13:33.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsConstants.py
+-rw-------   0 covino     (501) staff       (20)     8608 2021-03-02 15:35:24.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsImageClass.py
+-rw-------   0 covino     (501) staff       (20)      869 2015-07-23 12:13:58.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsTabsAppend.py
+-rw-------   0 covino     (501) staff       (20)      760 2017-05-18 14:34:24.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetData.py
+-rw-------   0 covino     (501) staff       (20)      802 2017-05-18 14:35:11.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetHeader.py
+-rw-------   0 covino     (501) staff       (20)      875 2017-05-18 14:35:28.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetHeaderValue.py
+-rw-------   0 covino     (501) staff       (20)      997 2017-05-18 13:39:55.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetSpectrum.py
+-rw-------   0 covino     (501) staff       (20)      586 2015-07-23 12:34:36.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetSpectrumPosition.py
+-rw-------   0 covino     (501) staff       (20)     1424 2021-02-09 12:48:15.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetWCS.py
+-rw-------   0 covino     (501) staff       (20)      702 2017-08-22 21:04:15.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/IsFits.py
+-rw-------   0 covino     (501) staff       (20)      437 2021-01-14 10:07:28.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/WCSPixelScale.py
+-rw-------   0 covino     (501) staff       (20)      567 2021-01-14 10:40:27.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/WCSRotationDeg.py
+-rw-------   0 covino     (501) staff       (20)      799 2022-08-10 13:01:02.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.757997 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/
+-rw-------   0 covino     (501) staff       (20)    24425 2021-03-17 08:46:10.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/AstrometryClass.py
+-rw-------   0 covino     (501) staff       (20)     2810 2021-03-02 15:30:39.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/DAOObjectClass.py
+-rw-------   0 covino     (501) staff       (20)      425 2015-07-23 12:15:58.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/EclipseConstants.py
+-rw-------   0 covino     (501) staff       (20)     2636 2017-05-16 09:56:28.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/EclipseObjectClass.py
+-rw-------   0 covino     (501) staff       (20)      853 2020-05-14 16:28:39.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/Pixel2WCS.py
+-rw-------   0 covino     (501) staff       (20)     1394 2020-05-14 13:44:46.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SExtractorConstants.py
+-rw-------   0 covino     (501) staff       (20)      361 2015-07-23 12:16:42.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SexConstants.py
+-rw-------   0 covino     (501) staff       (20)     2562 2020-12-11 12:24:32.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SexObjectClass.py
+-rw-------   0 covino     (501) staff       (20)     5248 2017-05-26 14:52:54.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SourceObjectsClass.py
+-rw-------   0 covino     (501) staff       (20)      865 2020-05-14 14:24:01.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/WCS2Pixel.py
+-rw-------   0 covino     (501) staff       (20)      588 2017-05-16 09:52:29.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/__init__.py
+-rw-------   0 covino     (501) staff       (20)      637 2020-03-07 14:00:40.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/getCenterRADEC.py
+-rw-r--r--   0 covino     (501) staff       (20)     1086 2023-05-22 09:48:40.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/GetFWHM.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.759999 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Math/
+-rw-------   0 covino     (501) staff       (20)     8163 2021-07-06 13:46:23.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Math/TriangleMatch.py
+-rw-------   0 covino     (501) staff       (20)      331 2017-03-14 08:48:57.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Math/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.797392 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/
+-rw-------   0 covino     (501) staff       (20)     1126 2017-04-19 13:53:05.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/ApErr.py
+-rw-------   0 covino     (501) staff       (20)     2903 2020-10-05 08:41:16.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/ApyPhot.py
+-rw-------   0 covino     (501) staff       (20)      520 2015-12-11 15:46:16.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/Counts2Mag.py
+-rw-------   0 covino     (501) staff       (20)      884 2017-08-30 19:36:03.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/DaoPhot.py
+-rw-r--r--   0 covino     (501) staff       (20)     5146 2023-05-22 09:44:44.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/FitsPhotometryClass.py
+-rw-------   0 covino     (501) staff       (20)      503 2015-07-23 12:26:20.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/Mag2Counts.py
+-rw-------   0 covino     (501) staff       (20)     1086 2015-11-13 14:11:34.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/MinMax.py
+-rw-------   0 covino     (501) staff       (20)      849 2022-08-10 13:00:32.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/__init__.py
+-rw-------   0 covino     (501) staff       (20)     1142 2017-04-19 13:45:07.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerGauss.py
+-rw-------   0 covino     (501) staff       (20)     1653 2020-03-07 16:49:45.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerMoment.py
+-rw-------   0 covino     (501) staff       (20)     1563 2017-08-24 08:53:55.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerObj.py
+-rw-------   0 covino     (501) staff       (20)     1281 2015-11-13 10:37:46.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/getBackground.py
+-rw-------   0 covino     (501) staff       (20)      803 2015-11-10 10:11:17.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/resid.py
+-rw-r--r--   0 covino     (501) staff       (20)      521 2021-06-02 20:51:07.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/SRPFITSPath.py
+-rw-r--r--   0 covino     (501) staff       (20)     2481 2023-05-22 09:48:36.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/__init__.py
+-rw-r--r--   0 covino     (501) staff       (20)      107 2023-05-22 10:07:50.569128 SRPAstro.FITS-3.0.1/setup.cfg
+-rw-------   0 covino     (501) staff       (20)     1780 2023-05-22 09:42:51.000000 SRPAstro.FITS-3.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SRPAstro.FITS-2.9.7/Docs/SRPAstro.FITS.pdf` & `SRPAstro.FITS-3.0.1/Docs/SRPAstro.FITS.pdf`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/LICENSE.txt` & `SRPAstro.FITS-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Misc/ApyPhot.py` & `SRPAstro.FITS-3.0.1/Misc/ApyPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Misc/AstrometryClass.py` & `SRPAstro.FITS-3.0.1/Misc/AstrometryClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/PKG-INFO` & `SRPAstro.FITS-3.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: SRPAstro.FITS
-Version: 2.9.7
+Version: 3.0.1
 Summary: Tools for handling FITS files under SRP
 Home-page: https://pypi.python.org/pypi/SRPAstro.FITS
 Author: Stefano Covino
 Author-email: stefano.covino@inaf.it
-License: UNKNOWN
-Description: # Swift Reduction Package
-        
-        Background
-        The Swift Reduction Package (hereafter SRP) is a packet of command line tools to solve problems (e.g. basic reduction and analysis tasks of optical/NIR astronomical data, quick cosmological computations, units conversions, etc.) often met in astronomical research activities.
-        
-        SRP was originally developed in the context of the Swift follow-up activities of the Milan GRB team at the INAF/Brera Astronomical Observatory. The package is designed to be an aid to any researcher to drive further observation of a followed-up GRB counterpart and “swift” can therefore be read simply as “rapid”, “agile”, etc.
-         
-         This subpackage if the SRP suite is devoted to the management of FITS file data.
-         
-        
 Keywords: astronomy data analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Swift Reduction Package
+
+Background
+The Swift Reduction Package (hereafter SRP) is a packet of command line tools to solve problems (e.g. basic reduction and analysis tasks of optical/NIR astronomical data, quick cosmological computations, units conversions, etc.) often met in astronomical research activities.
+
+SRP was originally developed in the context of the Swift follow-up activities of the Milan GRB team at the INAF/Brera Astronomical Observatory. The package is designed to be an aid to any researcher to drive further observation of a followed-up GRB counterpart and “swift” can therefore be read simply as “rapid”, “agile”, etc.
+ 
+ This subpackage if the SRP suite is devoted to the management of FITS file data.
+
```

### Comparing `SRPAstro.FITS-2.9.7/README.md` & `SRPAstro.FITS-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPAstro.FITS.egg-info/PKG-INFO` & `SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: SRPAstro.FITS
-Version: 2.9.7
+Version: 3.0.1
 Summary: Tools for handling FITS files under SRP
 Home-page: https://pypi.python.org/pypi/SRPAstro.FITS
 Author: Stefano Covino
 Author-email: stefano.covino@inaf.it
-License: UNKNOWN
-Description: # Swift Reduction Package
-        
-        Background
-        The Swift Reduction Package (hereafter SRP) is a packet of command line tools to solve problems (e.g. basic reduction and analysis tasks of optical/NIR astronomical data, quick cosmological computations, units conversions, etc.) often met in astronomical research activities.
-        
-        SRP was originally developed in the context of the Swift follow-up activities of the Milan GRB team at the INAF/Brera Astronomical Observatory. The package is designed to be an aid to any researcher to drive further observation of a followed-up GRB counterpart and “swift” can therefore be read simply as “rapid”, “agile”, etc.
-         
-         This subpackage if the SRP suite is devoted to the management of FITS file data.
-         
-        
 Keywords: astronomy data analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Swift Reduction Package
+
+Background
+The Swift Reduction Package (hereafter SRP) is a packet of command line tools to solve problems (e.g. basic reduction and analysis tasks of optical/NIR astronomical data, quick cosmological computations, units conversions, etc.) often met in astronomical research activities.
+
+SRP was originally developed in the context of the Swift follow-up activities of the Milan GRB team at the INAF/Brera Astronomical Observatory. The package is designed to be an aid to any researcher to drive further observation of a followed-up GRB counterpart and “swift” can therefore be read simply as “rapid”, “agile”, etc.
+ 
+ This subpackage if the SRP suite is devoted to the management of FITS file data.
+
```

### Comparing `SRPAstro.FITS-2.9.7/SRPAstro.FITS.egg-info/SOURCES.txt` & `SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 ./SRPFITS/Frames/getCenterRADEC.py
 ./SRPFITS/Math/TriangleMatch.py
 ./SRPFITS/Math/__init__.py
 ./SRPFITS/Photometry/ApErr.py
 ./SRPFITS/Photometry/ApyPhot.py
 ./SRPFITS/Photometry/Counts2Mag.py
 ./SRPFITS/Photometry/DaoPhot.py
+./SRPFITS/Photometry/FitsPhotometryClass.py
 ./SRPFITS/Photometry/Mag2Counts.py
 ./SRPFITS/Photometry/MinMax.py
 ./SRPFITS/Photometry/__init__.py
 ./SRPFITS/Photometry/centerGauss.py
 ./SRPFITS/Photometry/centerMoment.py
 ./SRPFITS/Photometry/centerObj.py
 ./SRPFITS/Photometry/getBackground.py
@@ -84,14 +85,15 @@
 ./build/lib/SRPFITS/Frames/getCenterRADEC.py
 ./build/lib/SRPFITS/Math/TriangleMatch.py
 ./build/lib/SRPFITS/Math/__init__.py
 ./build/lib/SRPFITS/Photometry/ApErr.py
 ./build/lib/SRPFITS/Photometry/ApyPhot.py
 ./build/lib/SRPFITS/Photometry/Counts2Mag.py
 ./build/lib/SRPFITS/Photometry/DaoPhot.py
+./build/lib/SRPFITS/Photometry/FitsPhotometryClass.py
 ./build/lib/SRPFITS/Photometry/Mag2Counts.py
 ./build/lib/SRPFITS/Photometry/MinMax.py
 ./build/lib/SRPFITS/Photometry/__init__.py
 ./build/lib/SRPFITS/Photometry/centerGauss.py
 ./build/lib/SRPFITS/Photometry/centerMoment.py
 ./build/lib/SRPFITS/Photometry/centerObj.py
 ./build/lib/SRPFITS/Photometry/getBackground.py
@@ -155,14 +157,15 @@
 SRPFITS/Frames/getCenterRADEC.py
 SRPFITS/Math/TriangleMatch.py
 SRPFITS/Math/__init__.py
 SRPFITS/Photometry/ApErr.py
 SRPFITS/Photometry/ApyPhot.py
 SRPFITS/Photometry/Counts2Mag.py
 SRPFITS/Photometry/DaoPhot.py
+SRPFITS/Photometry/FitsPhotometryClass.py
 SRPFITS/Photometry/Mag2Counts.py
 SRPFITS/Photometry/MinMax.py
 SRPFITS/Photometry/__init__.py
 SRPFITS/Photometry/centerGauss.py
 SRPFITS/Photometry/centerMoment.py
 SRPFITS/Photometry/centerObj.py
 SRPFITS/Photometry/getBackground.py
@@ -192,10 +195,11 @@
 Scripts/SRPPhotParSet
 Scripts/SRPPhotometry
 Scripts/SRPQuery
 Scripts/SRPRTAlignImaging
 Scripts/SRPRotoTransla
 Scripts/SRPScienceFramesImaging
 Scripts/SRPSourceFinder
+Scripts/SRPSourcePhotometry
 Scripts/SRPSpectralExtraction
 Scripts/SRPWCSPixel
 Scripts/SRPZeroPoint
```

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Data/.DS_Store` & `SRPAstro.FITS-3.0.1/SRPFITS/Data/.DS_Store`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPNnwIn` & `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPNnwIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexIn` & `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexLSLASCIn` & `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexLSLASCIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexREMREMIRIn` & `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMREMIRIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexREMROS2In` & `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMROS2In`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexREMROSSIn` & `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMROSSIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Data/SExtractor/SRPSexTNGLRSIn` & `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexTNGLRSIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/AddHeaderComment.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/AddHeaderComment.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/AddHeaderEntry.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/AddHeaderEntry.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/FitsConstants.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsConstants.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/FitsImageClass.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsImageClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/FitsTabsAppend.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsTabsAppend.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetData.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetData.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetHeader.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetHeader.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetHeaderValue.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetHeaderValue.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetSpectrum.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetSpectrum.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetSpectrumPosition.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetSpectrumPosition.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/GetWCS.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetWCS.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/IsFits.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/IsFits.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/WCSRotationDeg.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/WCSRotationDeg.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Fits/__init__.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Fits/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Init file for Fits
 
 Context : SRP
 Module  : SRPFits
-Version : 1.1.0
+Version : 1.2.0
 Author  : Stefano Covino
-Date    : 14/01/2021
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 29/03/2022
+E-mail  : stefano.covino@inaf.it
 URL     : http://www.me.oa-brera.inaf.it/utenti/covino
 
 
 Usage   : to be imported
 
 Remarks :
 
@@ -21,10 +21,10 @@
         : (14/01/2021) WCSRotationDeg and WCSPixelScale added.
 """
 
 
 
 __all__ = ['AddHeaderComment', 'AddHeaderEntry', 'FitsConstant', 'FitsImageClass',
            'FitsTabsAppend', 'GetData', 'GetHeader', 'GetHeaderValue', 'GetSpectrum',
-           'GetSpectrumPosition', 'GetWCS', 'IsFits', 'WCSPixelScale', 'WCSRotationDeg']
+            'GetSpectrumPosition', 'GetWCS', 'IsFits', 'WCSPixelScale', 'WCSRotationDeg']
```

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/AstrometryClass.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/AstrometryClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/DAOObjectClass.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/DAOObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/EclipseObjectClass.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/EclipseObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/Pixel2WCS.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/Pixel2WCS.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/SExtractorConstants.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/SExtractorConstants.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/SexObjectClass.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/SexObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/SourceObjectsClass.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/SourceObjectsClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/WCS2Pixel.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/WCS2Pixel.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/__init__.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/__init__.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Frames/getCenterRADEC.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Frames/getCenterRADEC.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/GetFWHM.py` & `SRPAstro.FITS-3.0.1/SRPFITS/GetFWHM.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """ Utility functions and classes for SRP
 
 Context : SRP
 Module  : SRPGW
-Version : 1.0.2
+Version : 1.1.0
 Author  : Stefano Covino
-Date    : 03/07/2017
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 22/05/2023
+E-mail  : stefano.covino@inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 
 Usage   : GetApPhot
 
 Remarks :
 
 History : (18/12/2016) First version.
         : (21/12/2016) Minor bug.
         : (03/07/2017) size must be integer in computations.
+        : (22/05/2023) Deprecated numpy feature.
 """
 
 import numpy as np
 from astropy.io.fits import getdata
 
 
 
 def GetFWHM(x,y,fname,size=20):
     fwhm = []
     data = getdata(fname)
     szint = int(size)
     for ii,jj in zip(x,y):
         a = np.rint(ii)-1
         b = np.rint(jj)-1
-        i = a.astype(np.int)
-        l = b.astype(np.int)
+        i = a.astype(int)
+        l = b.astype(int)
         image = data[l-szint:l+szint,i-szint:i+szint]
         dat=image.flatten()
         try:
             maxi = image.max()
             floor = np.median(image)
             height = maxi - floor
             #
```

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Math/TriangleMatch.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Math/TriangleMatch.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/ApErr.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/ApErr.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/ApyPhot.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/ApyPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/Counts2Mag.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/Counts2Mag.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/DaoPhot.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/DaoPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/MinMax.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/MinMax.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/__init__.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """ Init file for SRPPolarimetry
 
 Context : SRP
 Module  : Polarimetry
-Version : 1.6.0
+Version : 1.7.0
 Author  : Stefano Covino
-Date    : 24/08/2017
+Date    : 10/08/2022
 E-mail  : stefano.covino@brera.inaf.it
 URL     : http://www.me.oa-brera.inaf.it/utenti/covino
 
 Usage   : to be imported
 
 History : (15/02/2012) First named version.
         : (10/11/2015) resid, centerGauss and getBackground added.
         : (13/11/2015) MinMax added.
         : (18/11/2015) centerMoment added.
         : (19/04/2017) ApErr added.
         : (22/08/2017) DaoPhot added.
         : (23/08/2017) ApyPhot added.
         : (24/08/2017) centerObj added.
+        : (10/08/2022) FiotsPhotometry class added.
 """
 
 
-__all__ = ['ApErr', 'ApyPhot', 'centerGauss', 'centerMoment', 'centerObj', 'Counts2Mag',
-            'DaoPhot', 'Mag2Counts', 'getBackground', 'MinMax', 'resid']
+__all__ = ['ApErr', 'ApyPhot', 'centerGauss', 'centerMoment', 'centerObj',
+            'Counts2Mag', 'DaoPhot', 'FitsPhotometry', 'Mag2Counts',
+            'getBackground', 'MinMax', 'resid']
```

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/centerGauss.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerGauss.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/centerMoment.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerMoment.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/centerObj.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerObj.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/getBackground.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/getBackground.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/Photometry/resid.py` & `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/resid.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/SRPFITSPath.py` & `SRPAstro.FITS-3.0.1/SRPFITS/SRPFITSPath.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/SRPFITS/__init__.py` & `SRPAstro.FITS-3.0.1/SRPFITS/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ 
 
 Context : SRP
 Module  : FITS
-Version : 1.8.9
+Version : 1.9.4
 Author  : Stefano Covino
-Date    : 15/03/2022
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 22/05/2023
+E-mail  : stefano.covino@inaf.it
 URL     : http://www.me.oa-brera.inaf.it/utenti/covino
 
 
 Usage   : to be imported
 
 Remarks :
 
@@ -69,17 +69,20 @@
 		: (12/05/2021) V. 2.9.0.
         : (02/06/2021) V. 2.9.1 and 2.9.2
         : (06/07/2021) V. 2.9.3.
         : (08/07/2021) V. 2.9.4.
         : (07/09/2021) V. 2.9.5.
         : (16/11/2021) V. 2.9.6.
         : (15/03/2022) V. 2.9.7.
+        : (29/03/2022) V. 3.0.0beta.
+        : (02/12/2022) V. 3.0.0.
+        : (22/05/2023) V. 3.0.1.
 """
 
-__version__ = '2.9.7'
+__version__ = '3.0.1'
 
 
 
 __all__ =  ['Fits', 'Frames', 'GetFWHM', 'Math', 'Photometry', 'SRPFITSPath']
```

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPAdvAverage` & `SRPAstro.FITS-3.0.1/Scripts/SRPAdvAverage`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPAlignImaging` & `SRPAstro.FITS-3.0.1/Scripts/SRPAlignImaging`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPAstrometry` & `SRPAstro.FITS-3.0.1/Scripts/SRPAstrometry`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPAverage` & `SRPAstro.FITS-3.0.1/Scripts/SRPAverage`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPBias` & `SRPAstro.FITS-3.0.1/Scripts/SRPBias`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPClassify` & `SRPAstro.FITS-3.0.1/Scripts/SRPClassify`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPCut` & `SRPAstro.FITS-3.0.1/Scripts/SRPCut`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPDao2Sky` & `SRPAstro.FITS-3.0.1/Scripts/SRPDao2Sky`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFITSVersion` & `SRPAstro.FITS-3.0.1/Scripts/SRPFITSVersion`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFindingChart` & `SRPAstro.FITS-3.0.1/Scripts/SRPFindingChart`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFitsComposer` & `SRPAstro.FITS-3.0.1/Scripts/SRPFitsComposer`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFitsExtension` & `SRPAstro.FITS-3.0.1/Scripts/SRPFitsExtension`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFitsHeaders` & `SRPAstro.FITS-3.0.1/Scripts/SRPFitsHeaders`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFitsSpectrum2ASCII` & `SRPAstro.FITS-3.0.1/Scripts/SRPFitsSpectrum2ASCII`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #! python
 """ Code to convert FITS spectra to ASCII.
 
 Context : SRP
 Module  : SRPFitsSpectrum2ASCII.py
-Version : 1.0.1
+Version : 1.0.2
 Author  : Stefano Covino
-Date    : 18/05/2017
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 02/12/2022
+E-mail  : stefano.covino@inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 
 Usage   : SRPFitsSpectrum2ASCII -f arg1 [-h] [-v]
             -f Input FITS file list or single FITS file
             Convert a FITS spectrum to an ASCII file
 
 History : (22/09/2011) First version.
         : (18/05/2017) Minor update.
+        : (02/12/2022) Bug correction in scidata.
 """
 
 
 
 import os
 from optparse import OptionParser
 import atpy
@@ -88,18 +89,18 @@
             reflmb = prihdr['CRVAL1']
             refdl = prihdr['CDELT1']
             frhdu.close()
             #
             # Extract spectrum
             lamb = []
             specl = []
-            for i in range(len(scidata[0])):
+            for i in range(len(scidata)):
                 lmb = ((i-refpix)*refdl + reflmb)
                 lamb.append(lmb)
-                specl.append(scidata[0][i])
+                specl.append(scidata[i])
             #
             root,ext = os.path.splitext(fr)
             newfile = root+SRPConstants.SRPASCIISpec
             if options.verbose:
                 print("Generating file %s" % newfile)
             #
             t = atpy.Table()
```

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFitsStats` & `SRPAstro.FITS-3.0.1/Scripts/SRPFitsStats`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFitsTableViewer` & `SRPAstro.FITS-3.0.1/Scripts/SRPFitsTableViewer`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFlatImaging` & `SRPAstro.FITS-3.0.1/Scripts/SRPFlatImaging`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPFlatSpectroscopy` & `SRPAstro.FITS-3.0.1/Scripts/SRPFlatSpectroscopy`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPGAIA2Sky` & `SRPAstro.FITS-3.0.1/Scripts/SRPGAIA2Sky`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPImageFilter` & `SRPAstro.FITS-3.0.1/Scripts/SRPImageFilter`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPImageMapping` & `SRPAstro.FITS-3.0.1/Scripts/SRPImageMapping`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     return area,nm,mpars[0],mpars[1],mpars[2],False
 
 
 
 
 parser = OptionParser(usage="usage: %prog [-v] [-h] [-d/-s] [-f] -i arg1 [-l arg2] [-m arg3] [-n arg4] [-o] [-p] [-t]", version="%prog 1.8.2")
 parser.add_option("-d", "--daofind", action="store_true", dest="daofind", help="Source extracted by DAOPHOT")
-parser.add_option("-f", "--fwhmfilter", action="store", dest="fwhmf", type="float", nargs=2, help="Filter for FWHM value (min max)")
+parser.add_option("-f", "--fwhmfilter", action="store", dest="fwhmf", type="float", nargs=2, help="Filter for FWHM value (pixel_min pixel_max)")
 parser.add_option("-i", "--inputlist", action="store", nargs=1, type="string", dest="fitsfilelist", help="Input FITS file list")
 parser.add_option("-l", "--level", action="store", nargs=1, type="float", dest="level", default=2.0, help="Search deepness.")
 parser.add_option("-m", "--matchstars", action="store", nargs=1, type="int", dest="matchp", default=5, help="Minimum number of stars in common area for matching")
 parser.add_option("-n", "--nobj", action="store", type="int", dest="nobj", default=10, help="Number of objects for matching search")
 parser.add_option("-o", "--outfiles", action="store_true", dest="outfiles", help="Save files with object positions")
 parser.add_option("-p", "--pureint", action="store_true", dest="pure", default=False, help="Integer pixel shift for pure translation")
 parser.add_option("-r", "--radius", action="store", nargs=1, type="float", dest="radius", default=0.0, help="Max tolerance (pixel)")
```

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPKeywords` & `SRPAstro.FITS-3.0.1/Scripts/SRPKeywords`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPPhotParSet` & `SRPAstro.FITS-3.0.1/Scripts/SRPPhotParSet`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPPhotometry` & `SRPAstro.FITS-3.0.1/Scripts/SRPPhotometry`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPQuery` & `SRPAstro.FITS-3.0.1/Scripts/SRPQuery`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPRTAlignImaging` & `SRPAstro.FITS-3.0.1/Scripts/SRPRTAlignImaging`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPRotoTransla` & `SRPAstro.FITS-3.0.1/Scripts/SRPRotoTransla`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPScienceFramesImaging` & `SRPAstro.FITS-3.0.1/Scripts/SRPScienceFramesImaging`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPSourceFinder` & `SRPAstro.FITS-3.0.1/Scripts/SRPSourceFinder`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! python
 """ Code to extract sources from a fits frame
 
 Context : SRP
 Module  : SRPSourceFinder
 Author  : Stefano Covino
-Date    : 18/05/2017
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 22/05/2023
+E-mail  : stefano.covino@inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 Purpose :
 
 Usage   : SRPSourceFinder -e/-n/-s -f arg1 [-h] [-m arg2] [-S] [-t arg3] [-v]
             -e Eclipse algorithm
             -f FITS file
             -m Minimum number of connected pixel (for native only)
@@ -24,14 +24,15 @@
         : (04/09/2010) Minor correction.
         : (27/09/2010) Eclipse sources added.
         : (18/10/2010) Import correction.
         : (07/08/2011) Better cosmetics.
         : (18/04/2013) More complete output.
         : (14/03/2016) Python3 porting.
         : (18/05/2017) Minor update.
+        : (22/05/2023) Minor bug correction.
 """
 
 
 from SRPFITS.Fits.FitsImageClass import FitsImage
 from SRPFITS.Fits import FitsConstants
 from SRPFITS.Fits.IsFits import IsFits
 from optparse import OptionParser
@@ -39,15 +40,15 @@
 
 
 parser = OptionParser(usage="usage: %prog -d/-n/-s -f arg1 [-h] [-m arg2] [-S] [-t arg3] [-v]", version="%prog 1.3.0")
 parser.add_option("-d", "--daophot", action="store_true", dest="daophot", help="Daophot algorithm")
 parser.add_option("-f", "--fits", action="store", nargs=1, type="string", dest="fits", help="FITS file")
 parser.add_option("-m", "--minpix", action="store", dest="minpix", type="int", help="Minimum number of connected pixel (for native only)")
 parser.add_option("-n", "--native", action="store_true", dest="native", help="Native algorithm")
-parser.add_option("-s", "--sexctractor", action="store_true", dest="sex", help="Sextractor algorithm (default)")
+parser.add_option("-s", "--sextractor", action="store_true", dest="sex", help="Sextractor algorithm (default)")
 parser.add_option("-S", "--skycat", action="store_true", dest="skycat", help="Skycat output")
 parser.add_option("-t", "--threshold", action="store", type="float", dest="thre", help="Threshold for pixel selection")
 parser.add_option("-v", "--verbose", action="store_true", dest="verbose", help="Fully describe operations")
 (options, args) = parser.parse_args()
```

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPSpectralExtraction` & `SRPAstro.FITS-3.0.1/Scripts/SRPSpectralExtraction`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPWCSPixel` & `SRPAstro.FITS-3.0.1/Scripts/SRPWCSPixel`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/Scripts/SRPZeroPoint` & `SRPAstro.FITS-3.0.1/Scripts/SRPZeroPoint`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/AddHeaderComment.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/AddHeaderComment.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/AddHeaderEntry.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/AddHeaderEntry.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/FitsConstants.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsConstants.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/FitsImageClass.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsImageClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/FitsTabsAppend.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsTabsAppend.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetData.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetData.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetHeader.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetHeader.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetHeaderValue.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetHeaderValue.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetSpectrum.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetSpectrum.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetSpectrumPosition.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetSpectrumPosition.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/GetWCS.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetWCS.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/IsFits.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/IsFits.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/WCSRotationDeg.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/WCSRotationDeg.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Fits/__init__.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Init file for Fits
 
 Context : SRP
 Module  : SRPFits
-Version : 1.1.0
+Version : 1.2.0
 Author  : Stefano Covino
-Date    : 14/01/2021
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 29/03/2022
+E-mail  : stefano.covino@inaf.it
 URL     : http://www.me.oa-brera.inaf.it/utenti/covino
 
 
 Usage   : to be imported
 
 Remarks :
 
@@ -21,10 +21,10 @@
         : (14/01/2021) WCSRotationDeg and WCSPixelScale added.
 """
 
 
 
 __all__ = ['AddHeaderComment', 'AddHeaderEntry', 'FitsConstant', 'FitsImageClass',
            'FitsTabsAppend', 'GetData', 'GetHeader', 'GetHeaderValue', 'GetSpectrum',
-           'GetSpectrumPosition', 'GetWCS', 'IsFits', 'WCSPixelScale', 'WCSRotationDeg']
+            'GetSpectrumPosition', 'GetWCS', 'IsFits', 'WCSPixelScale', 'WCSRotationDeg']
```

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/AstrometryClass.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/AstrometryClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/DAOObjectClass.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/DAOObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/EclipseObjectClass.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/EclipseObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/Pixel2WCS.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/Pixel2WCS.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/SExtractorConstants.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SExtractorConstants.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/SexObjectClass.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SexObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/SourceObjectsClass.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SourceObjectsClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/WCS2Pixel.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/WCS2Pixel.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/__init__.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/__init__.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Frames/getCenterRADEC.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/getCenterRADEC.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/GetFWHM.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/GetFWHM.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """ Utility functions and classes for SRP
 
 Context : SRP
 Module  : SRPGW
-Version : 1.0.2
+Version : 1.1.0
 Author  : Stefano Covino
-Date    : 03/07/2017
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 22/05/2023
+E-mail  : stefano.covino@inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 
 Usage   : GetApPhot
 
 Remarks :
 
 History : (18/12/2016) First version.
         : (21/12/2016) Minor bug.
         : (03/07/2017) size must be integer in computations.
+        : (22/05/2023) Deprecated numpy feature.
 """
 
 import numpy as np
 from astropy.io.fits import getdata
 
 
 
 def GetFWHM(x,y,fname,size=20):
     fwhm = []
     data = getdata(fname)
     szint = int(size)
     for ii,jj in zip(x,y):
         a = np.rint(ii)-1
         b = np.rint(jj)-1
-        i = a.astype(np.int)
-        l = b.astype(np.int)
+        i = a.astype(int)
+        l = b.astype(int)
         image = data[l-szint:l+szint,i-szint:i+szint]
         dat=image.flatten()
         try:
             maxi = image.max()
             floor = np.median(image)
             height = maxi - floor
             #
```

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Math/TriangleMatch.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Math/TriangleMatch.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/ApErr.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/ApErr.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/ApyPhot.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/ApyPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/Counts2Mag.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/Counts2Mag.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/DaoPhot.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/DaoPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/MinMax.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/MinMax.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/__init__.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """ Init file for SRPPolarimetry
 
 Context : SRP
 Module  : Polarimetry
-Version : 1.6.0
+Version : 1.7.0
 Author  : Stefano Covino
-Date    : 24/08/2017
+Date    : 10/08/2022
 E-mail  : stefano.covino@brera.inaf.it
 URL     : http://www.me.oa-brera.inaf.it/utenti/covino
 
 Usage   : to be imported
 
 History : (15/02/2012) First named version.
         : (10/11/2015) resid, centerGauss and getBackground added.
         : (13/11/2015) MinMax added.
         : (18/11/2015) centerMoment added.
         : (19/04/2017) ApErr added.
         : (22/08/2017) DaoPhot added.
         : (23/08/2017) ApyPhot added.
         : (24/08/2017) centerObj added.
+        : (10/08/2022) FiotsPhotometry class added.
 """
 
 
-__all__ = ['ApErr', 'ApyPhot', 'centerGauss', 'centerMoment', 'centerObj', 'Counts2Mag',
-            'DaoPhot', 'Mag2Counts', 'getBackground', 'MinMax', 'resid']
+__all__ = ['ApErr', 'ApyPhot', 'centerGauss', 'centerMoment', 'centerObj',
+            'Counts2Mag', 'DaoPhot', 'FitsPhotometry', 'Mag2Counts',
+            'getBackground', 'MinMax', 'resid']
```

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/centerGauss.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerGauss.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/centerMoment.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerMoment.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/centerObj.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerObj.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/getBackground.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/getBackground.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/Photometry/resid.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/resid.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/SRPFITSPath.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/SRPFITSPath.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-2.9.7/build/lib/SRPFITS/__init__.py` & `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ 
 
 Context : SRP
 Module  : FITS
-Version : 1.8.9
+Version : 1.9.4
 Author  : Stefano Covino
-Date    : 15/03/2022
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 22/05/2023
+E-mail  : stefano.covino@inaf.it
 URL     : http://www.me.oa-brera.inaf.it/utenti/covino
 
 
 Usage   : to be imported
 
 Remarks :
 
@@ -69,17 +69,20 @@
 		: (12/05/2021) V. 2.9.0.
         : (02/06/2021) V. 2.9.1 and 2.9.2
         : (06/07/2021) V. 2.9.3.
         : (08/07/2021) V. 2.9.4.
         : (07/09/2021) V. 2.9.5.
         : (16/11/2021) V. 2.9.6.
         : (15/03/2022) V. 2.9.7.
+        : (29/03/2022) V. 3.0.0beta.
+        : (02/12/2022) V. 3.0.0.
+        : (22/05/2023) V. 3.0.1.
 """
 
-__version__ = '2.9.7'
+__version__ = '3.0.1'
 
 
 
 __all__ =  ['Fits', 'Frames', 'GetFWHM', 'Math', 'Photometry', 'SRPFITSPath']
```

### Comparing `SRPAstro.FITS-2.9.7/setup.py` & `SRPAstro.FITS-3.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,12 +48,14 @@
         'Operating System :: POSIX',
         'Programming Language :: Python :: 3',
         ],
     keywords='astronomy data analysis',
     include_package_data=True,
     packages=find_packages(),
     python_requires='>=3',
+    #packages=['SRPFITS'],
+    #package_dir={'SRPFITS':'SRPFITS'},
     package_data={'SRPFITS':lsdtex},
     scripts=lscrex,
     install_requires=['SRPAstro >= 4.4', 'sep', 'photutils', 'astropy', 'astLib >= 0.11.5', 'astroalign'],
     )
```

