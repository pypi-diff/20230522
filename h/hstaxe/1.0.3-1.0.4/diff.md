# Comparing `tmp/hstaxe-1.0.3.tar.gz` & `tmp/hstaxe-1.0.4.tar.gz`

## Comparing `hstaxe-1.0.3.tar` & `hstaxe-1.0.4.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/Makefile.am
--rwxr-xr-x   0        0        0    47386 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/autogen.sh
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/configure.ac
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/Makefile.am
--rw-r--r--   0        0        0    13666 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_AF2PET.c
--rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_BE.c
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_CHECK.c
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_DIRIMAGE.c
--rw-r--r--   0        0        0    12938 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_DRZ2PET.c
--rw-r--r--   0        0        0    21905 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_DRZPREP.c
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_FILET.c
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_FILET2.c
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_FRIGEN.c
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_FRINGECORR.c
--rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_GOL2AF.c
--rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_GPS.c
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_INTPIXCORR.c
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_NICBACK.c
--rw-r--r--   0        0        0    22007 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_PET2SPC.c
--rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_PETCONT.c
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_PETFF.c
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_PETIPC.c
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_SCALEBCK.c
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_SEX2GOL.c
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_STAMPS.c
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_TEST.c
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_TFIT.c
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_errors.c
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_errors.h
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_grism.h
--rw-r--r--   0        0        0    59634 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_utils.c
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aXe_utils.h
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aper_check.c
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aper_check.h
--rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aper_conf.c
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/aper_conf.h
--rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/crossdisp_utils.c
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/crossdisp_utils.h
--rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/dirimage_model.c
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/dirimage_model.h
--rw-r--r--   0        0        0    15253 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/disp_conf.c
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/disp_conf.h
--rw-r--r--   0        0        0    23363 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/drizzle_utils.c
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/drizzle_utils.h
--rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/drz2pet_utils.c
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/drz2pet_utils.h
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/fringe_conf.c
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/fringe_conf.h
--rw-r--r--   0        0        0    36951 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/fringe_model.c
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/fringe_model.h
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/fringe_utils.c
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/fringe_utils.h
--rw-r--r--   0        0        0    19909 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/inima_utils.c
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/inima_utils.h
--rw-r--r--   0        0        0    36861 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/inout_aper.c
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/inout_aper.h
--rw-r--r--   0        0        0    40593 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/ipixcorr_utils.c
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/ipixcorr_utils.h
--rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/lm_eval.c
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/lm_eval.h
--rw-r--r--   0        0        0    40331 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/lmmin.c
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/lmmin.h
--rw-r--r--   0        0        0    66123 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/model_utils.c
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/model_utils.h
--rw-r--r--   0        0        0    16948 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/nicback_utils.c
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/nicback_utils.h
--rw-r--r--   0        0        0    19499 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/scaleback_utils.c
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/scaleback_utils.h
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_CD.c
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_CD.h
--rw-r--r--   0        0        0    26558 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_FITScards.c
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_FITScards.h
--rw-r--r--   0        0        0    53062 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_back.c
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_back.h
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_cfg.c
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_cfg.h
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_driz.c
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_driz.h
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_extract.c
--rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_flatfield.c
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_flatfield.h
--rw-r--r--   0        0        0    19760 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_fluxcube.c
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_fluxcube.h
--rw-r--r--   0        0        0    61035 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_model.c
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_model.h
--rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_optimum.c
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_optimum.h
--rw-r--r--   0        0        0    38085 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_resp.c
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_resp.h
--rw-r--r--   0        0        0    68507 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_sex.c
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_sex.h
--rw-r--r--   0        0        0    45638 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_spc.c
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_spc.h
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_trace_functions.c
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_trace_functions.h
--rw-r--r--   0        0        0    31304 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_utils.c
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_utils.h
--rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_wl_calib.c
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spc_wl_calib.h
--rw-r--r--   0        0        0    31020 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_PET.c
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_PET.h
--rw-r--r--   0        0        0    19966 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_binning.c
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_binning.h
--rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_fitting.c
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_fitting.h
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_is_in.c
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_is_in.h
--rw-r--r--   0        0        0    35494 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_output.c
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_output.h
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_pathlength.c
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_pathlength.h
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_pgp.c
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_pgp.h
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_sect.c
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/spce_sect.h
--rw-r--r--   0        0        0    19457 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/specmodel_utils.c
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/specmodel_utils.h
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/test_aper_check.c
--rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/trace_conf.c
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/trace_conf.h
--rw-r--r--   0        0        0    40360 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/trfit_utils.c
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 hstaxe-1.0.3/cextern/src/trfit_utils.h
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/_version.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axeException.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axeerror.py
--rw-r--r--   0        0        0    11465 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/config.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/utils.py
--rw-r--r--   0        0        0    37795 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/WCSdata.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/axesim_verify.py
--rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/axesimtasks.py
--rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/imagemaker.py
--rw-r--r--   0        0        0    27358 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/interpolator.py
--rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/modspeclist.py
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/realworld.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/templateimages.py
--rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesim/templatespectra.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/__init__.py
--rw-r--r--   0        0        0    16180 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/axecommands.py
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/axeinputs.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/axeiol.py
--rw-r--r--   0        0        0    63267 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/axelowlev.py
--rw-r--r--   0        0        0    22525 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/axepreptor.py
--rw-r--r--   0        0        0     8556 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/axesingextr.py
--rw-r--r--   0        0        0    30236 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/axetasks.py
--rw-r--r--   0        0        0    46459 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/configfile.py
--rw-r--r--   0        0        0    25545 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/dither.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/dppdumps.py
--rw-r--r--   0        0        0    59735 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/drizzleobjects.py
--rwxr-xr-x   0        0        0    34257 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/fcubeobjs.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/imagemaker.py
--rw-r--r--   0        0        0    25721 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/inputchecks.py
--rw-r--r--   0        0        0    15477 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/iolmaking.py
--rw-r--r--   0        0        0    18520 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/mefobjects.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/nlincoeffs.py
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/axesrc/pysex2gol.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/coveragerc
--rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/run_acs_cookbook.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/run_cookbook.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/run_cookbook_part2.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_af2pet.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_axecore.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_axeprep.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_be.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_gol2af.py
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_iolprep.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_pet2spc.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_petcont.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_petff.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_scalebck.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_sex2gol.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hstaxe/tests/test_stamps.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 hstaxe-1.0.3/.gitignore
--rw-r--r--   0        0        0    36800 2020-02-02 00:00:00.000000 hstaxe-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 hstaxe-1.0.3/README.md
--rwxr-xr-x   0        0        0     6331 2020-02-02 00:00:00.000000 hstaxe-1.0.3/hatch_build.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 hstaxe-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 hstaxe-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/Makefile.am
+-rwxr-xr-x   0        0        0    47386 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/autogen.sh
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/configure.ac
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/Makefile.am
+-rw-r--r--   0        0        0    13666 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_AF2PET.c
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_BE.c
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_CHECK.c
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_DIRIMAGE.c
+-rw-r--r--   0        0        0    12938 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_DRZ2PET.c
+-rw-r--r--   0        0        0    21905 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_DRZPREP.c
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_FILET.c
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_FILET2.c
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_FRIGEN.c
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_FRINGECORR.c
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_GOL2AF.c
+-rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_GPS.c
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_INTPIXCORR.c
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_NICBACK.c
+-rw-r--r--   0        0        0    22007 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_PET2SPC.c
+-rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_PETCONT.c
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_PETFF.c
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_PETIPC.c
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_SCALEBCK.c
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_SEX2GOL.c
+-rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_STAMPS.c
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_TEST.c
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_TFIT.c
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_errors.c
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_errors.h
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_grism.h
+-rw-r--r--   0        0        0    59634 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_utils.c
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_utils.h
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aper_check.c
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aper_check.h
+-rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aper_conf.c
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aper_conf.h
+-rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/crossdisp_utils.c
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/crossdisp_utils.h
+-rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/dirimage_model.c
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/dirimage_model.h
+-rw-r--r--   0        0        0    15253 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/disp_conf.c
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/disp_conf.h
+-rw-r--r--   0        0        0    23363 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/drizzle_utils.c
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/drizzle_utils.h
+-rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/drz2pet_utils.c
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/drz2pet_utils.h
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_conf.c
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_conf.h
+-rw-r--r--   0        0        0    36951 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_model.c
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_model.h
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_utils.c
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_utils.h
+-rw-r--r--   0        0        0    19909 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/inima_utils.c
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/inima_utils.h
+-rw-r--r--   0        0        0    36861 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/inout_aper.c
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/inout_aper.h
+-rw-r--r--   0        0        0    40593 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/ipixcorr_utils.c
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/ipixcorr_utils.h
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/lm_eval.c
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/lm_eval.h
+-rw-r--r--   0        0        0    40331 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/lmmin.c
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/lmmin.h
+-rw-r--r--   0        0        0    66123 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/model_utils.c
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/model_utils.h
+-rw-r--r--   0        0        0    16948 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/nicback_utils.c
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/nicback_utils.h
+-rw-r--r--   0        0        0    19499 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/scaleback_utils.c
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/scaleback_utils.h
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_CD.c
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_CD.h
+-rw-r--r--   0        0        0    26558 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_FITScards.c
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_FITScards.h
+-rw-r--r--   0        0        0    53062 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_back.c
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_back.h
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_cfg.c
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_cfg.h
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_driz.c
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_driz.h
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_extract.c
+-rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_flatfield.c
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_flatfield.h
+-rw-r--r--   0        0        0    19760 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_fluxcube.c
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_fluxcube.h
+-rw-r--r--   0        0        0    61035 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_model.c
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_model.h
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_optimum.c
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_optimum.h
+-rw-r--r--   0        0        0    38085 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_resp.c
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_resp.h
+-rw-r--r--   0        0        0    68507 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_sex.c
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_sex.h
+-rw-r--r--   0        0        0    45638 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_spc.c
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_spc.h
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_trace_functions.c
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_trace_functions.h
+-rw-r--r--   0        0        0    31304 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_utils.c
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_utils.h
+-rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_wl_calib.c
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_wl_calib.h
+-rw-r--r--   0        0        0    31020 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_PET.c
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_PET.h
+-rw-r--r--   0        0        0    19966 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_binning.c
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_binning.h
+-rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_fitting.c
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_fitting.h
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_is_in.c
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_is_in.h
+-rw-r--r--   0        0        0    35494 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_output.c
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_output.h
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_pathlength.c
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_pathlength.h
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_pgp.c
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_pgp.h
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_sect.c
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_sect.h
+-rw-r--r--   0        0        0    19457 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/specmodel_utils.c
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/specmodel_utils.h
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/test_aper_check.c
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/trace_conf.c
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/trace_conf.h
+-rw-r--r--   0        0        0    40360 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/trfit_utils.c
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/trfit_utils.h
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/_version.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axeException.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axeerror.py
+-rw-r--r--   0        0        0    11529 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/config.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/utils.py
+-rw-r--r--   0        0        0    37795 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/WCSdata.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/axesim_verify.py
+-rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/axesimtasks.py
+-rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/imagemaker.py
+-rw-r--r--   0        0        0    27371 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/interpolator.py
+-rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/modspeclist.py
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/realworld.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/templateimages.py
+-rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/templatespectra.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/__init__.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axecommands.py
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axeinputs.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axeiol.py
+-rw-r--r--   0        0        0    63246 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axelowlev.py
+-rw-r--r--   0        0        0    22432 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axepreptor.py
+-rw-r--r--   0        0        0     8556 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axesingextr.py
+-rw-r--r--   0        0        0    30236 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axetasks.py
+-rw-r--r--   0        0        0    46451 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/configfile.py
+-rw-r--r--   0        0        0    25435 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/dither.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/dppdumps.py
+-rw-r--r--   0        0        0    59736 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/drizzleobjects.py
+-rwxr-xr-x   0        0        0    34257 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/fcubeobjs.py
+-rw-r--r--   0        0        0     8263 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/imagemaker.py
+-rw-r--r--   0        0        0    25721 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/inputchecks.py
+-rw-r--r--   0        0        0    15477 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/iolmaking.py
+-rw-r--r--   0        0        0    18555 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/mefobjects.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/nlincoeffs.py
+-rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/pysex2gol.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/coveragerc
+-rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/run_acs_cookbook.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/run_cookbook.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/run_cookbook_part2.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_af2pet.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_axecore.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_axeprep.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_be.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_gol2af.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_iolprep.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_pet2spc.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_petcont.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_petff.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_scalebck.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_sex2gol.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_stamps.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 hstaxe-1.0.4/.gitignore
+-rw-r--r--   0        0        0    36800 2020-02-02 00:00:00.000000 hstaxe-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 hstaxe-1.0.4/README.md
+-rwxr-xr-x   0        0        0     6331 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hatch_build.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 hstaxe-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 hstaxe-1.0.4/PKG-INFO
```

### Comparing `hstaxe-1.0.3/cextern/autogen.sh` & `hstaxe-1.0.4/cextern/autogen.sh`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/configure.ac` & `hstaxe-1.0.4/cextern/configure.ac`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/Makefile.am` & `hstaxe-1.0.4/cextern/src/Makefile.am`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_AF2PET.c` & `hstaxe-1.0.4/cextern/src/aXe_AF2PET.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_BE.c` & `hstaxe-1.0.4/cextern/src/aXe_BE.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_CHECK.c` & `hstaxe-1.0.4/cextern/src/aXe_CHECK.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_DIRIMAGE.c` & `hstaxe-1.0.4/cextern/src/aXe_DIRIMAGE.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_DRZ2PET.c` & `hstaxe-1.0.4/cextern/src/aXe_DRZ2PET.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_DRZPREP.c` & `hstaxe-1.0.4/cextern/src/aXe_DRZPREP.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_FILET.c` & `hstaxe-1.0.4/cextern/src/aXe_FILET.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_FILET2.c` & `hstaxe-1.0.4/cextern/src/aXe_FILET2.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_FRIGEN.c` & `hstaxe-1.0.4/cextern/src/aXe_FRIGEN.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_FRINGECORR.c` & `hstaxe-1.0.4/cextern/src/aXe_FRINGECORR.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_GOL2AF.c` & `hstaxe-1.0.4/cextern/src/aXe_GOL2AF.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_GPS.c` & `hstaxe-1.0.4/cextern/src/aXe_GPS.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_INTPIXCORR.c` & `hstaxe-1.0.4/cextern/src/aXe_INTPIXCORR.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_NICBACK.c` & `hstaxe-1.0.4/cextern/src/aXe_NICBACK.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_PET2SPC.c` & `hstaxe-1.0.4/cextern/src/aXe_PET2SPC.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_PETCONT.c` & `hstaxe-1.0.4/cextern/src/aXe_PETCONT.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_PETFF.c` & `hstaxe-1.0.4/cextern/src/aXe_PETFF.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_PETIPC.c` & `hstaxe-1.0.4/cextern/src/aXe_PETIPC.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_SCALEBCK.c` & `hstaxe-1.0.4/cextern/src/aXe_SCALEBCK.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_SEX2GOL.c` & `hstaxe-1.0.4/cextern/src/aXe_SEX2GOL.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_STAMPS.c` & `hstaxe-1.0.4/cextern/src/aXe_STAMPS.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_TEST.c` & `hstaxe-1.0.4/cextern/src/aXe_TEST.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_TFIT.c` & `hstaxe-1.0.4/cextern/src/aXe_TFIT.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_errors.c` & `hstaxe-1.0.4/cextern/src/aXe_errors.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_grism.h` & `hstaxe-1.0.4/cextern/src/aXe_grism.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_utils.c` & `hstaxe-1.0.4/cextern/src/aXe_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aXe_utils.h` & `hstaxe-1.0.4/cextern/src/aXe_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aper_check.c` & `hstaxe-1.0.4/cextern/src/aper_check.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aper_conf.c` & `hstaxe-1.0.4/cextern/src/aper_conf.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/aper_conf.h` & `hstaxe-1.0.4/cextern/src/aper_conf.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/crossdisp_utils.c` & `hstaxe-1.0.4/cextern/src/crossdisp_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/crossdisp_utils.h` & `hstaxe-1.0.4/cextern/src/crossdisp_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/dirimage_model.c` & `hstaxe-1.0.4/cextern/src/dirimage_model.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/dirimage_model.h` & `hstaxe-1.0.4/cextern/src/dirimage_model.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/disp_conf.c` & `hstaxe-1.0.4/cextern/src/disp_conf.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/disp_conf.h` & `hstaxe-1.0.4/cextern/src/disp_conf.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/drizzle_utils.c` & `hstaxe-1.0.4/cextern/src/drizzle_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/drizzle_utils.h` & `hstaxe-1.0.4/cextern/src/drizzle_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/drz2pet_utils.c` & `hstaxe-1.0.4/cextern/src/drz2pet_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/drz2pet_utils.h` & `hstaxe-1.0.4/cextern/src/drz2pet_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/fringe_conf.c` & `hstaxe-1.0.4/cextern/src/fringe_conf.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/fringe_conf.h` & `hstaxe-1.0.4/cextern/src/fringe_conf.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/fringe_model.c` & `hstaxe-1.0.4/cextern/src/fringe_model.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/fringe_model.h` & `hstaxe-1.0.4/cextern/src/fringe_model.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/fringe_utils.c` & `hstaxe-1.0.4/cextern/src/fringe_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/fringe_utils.h` & `hstaxe-1.0.4/cextern/src/fringe_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/inima_utils.c` & `hstaxe-1.0.4/cextern/src/inima_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/inima_utils.h` & `hstaxe-1.0.4/cextern/src/inima_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/inout_aper.c` & `hstaxe-1.0.4/cextern/src/inout_aper.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/inout_aper.h` & `hstaxe-1.0.4/cextern/src/inout_aper.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/ipixcorr_utils.c` & `hstaxe-1.0.4/cextern/src/ipixcorr_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/ipixcorr_utils.h` & `hstaxe-1.0.4/cextern/src/ipixcorr_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/lm_eval.c` & `hstaxe-1.0.4/cextern/src/lm_eval.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/lm_eval.h` & `hstaxe-1.0.4/cextern/src/lm_eval.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/lmmin.c` & `hstaxe-1.0.4/cextern/src/lmmin.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/lmmin.h` & `hstaxe-1.0.4/cextern/src/lmmin.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/model_utils.c` & `hstaxe-1.0.4/cextern/src/model_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/model_utils.h` & `hstaxe-1.0.4/cextern/src/model_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/nicback_utils.c` & `hstaxe-1.0.4/cextern/src/nicback_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/nicback_utils.h` & `hstaxe-1.0.4/cextern/src/nicback_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/scaleback_utils.c` & `hstaxe-1.0.4/cextern/src/scaleback_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/scaleback_utils.h` & `hstaxe-1.0.4/cextern/src/scaleback_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_CD.c` & `hstaxe-1.0.4/cextern/src/spc_CD.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_CD.h` & `hstaxe-1.0.4/cextern/src/spc_CD.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_FITScards.c` & `hstaxe-1.0.4/cextern/src/spc_FITScards.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_FITScards.h` & `hstaxe-1.0.4/cextern/src/spc_FITScards.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_back.c` & `hstaxe-1.0.4/cextern/src/spc_back.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_back.h` & `hstaxe-1.0.4/cextern/src/spc_back.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_cfg.c` & `hstaxe-1.0.4/cextern/src/spc_cfg.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_cfg.h` & `hstaxe-1.0.4/cextern/src/spc_cfg.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_driz.c` & `hstaxe-1.0.4/cextern/src/spc_driz.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_extract.c` & `hstaxe-1.0.4/cextern/src/spc_extract.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_flatfield.c` & `hstaxe-1.0.4/cextern/src/spc_flatfield.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_flatfield.h` & `hstaxe-1.0.4/cextern/src/spc_flatfield.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_fluxcube.c` & `hstaxe-1.0.4/cextern/src/spc_fluxcube.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_fluxcube.h` & `hstaxe-1.0.4/cextern/src/spc_fluxcube.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_model.c` & `hstaxe-1.0.4/cextern/src/spc_model.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_model.h` & `hstaxe-1.0.4/cextern/src/spc_model.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_optimum.c` & `hstaxe-1.0.4/cextern/src/spc_optimum.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_optimum.h` & `hstaxe-1.0.4/cextern/src/spc_optimum.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_resp.c` & `hstaxe-1.0.4/cextern/src/spc_resp.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_resp.h` & `hstaxe-1.0.4/cextern/src/spc_resp.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_sex.c` & `hstaxe-1.0.4/cextern/src/spc_sex.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_sex.h` & `hstaxe-1.0.4/cextern/src/spc_sex.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_spc.c` & `hstaxe-1.0.4/cextern/src/spc_spc.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_spc.h` & `hstaxe-1.0.4/cextern/src/spc_spc.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_trace_functions.c` & `hstaxe-1.0.4/cextern/src/spc_trace_functions.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_trace_functions.h` & `hstaxe-1.0.4/cextern/src/spc_trace_functions.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_utils.c` & `hstaxe-1.0.4/cextern/src/spc_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_utils.h` & `hstaxe-1.0.4/cextern/src/spc_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_wl_calib.c` & `hstaxe-1.0.4/cextern/src/spc_wl_calib.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spc_wl_calib.h` & `hstaxe-1.0.4/cextern/src/spc_wl_calib.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_PET.c` & `hstaxe-1.0.4/cextern/src/spce_PET.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_PET.h` & `hstaxe-1.0.4/cextern/src/spce_PET.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_binning.c` & `hstaxe-1.0.4/cextern/src/spce_binning.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_binning.h` & `hstaxe-1.0.4/cextern/src/spce_binning.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_fitting.c` & `hstaxe-1.0.4/cextern/src/spce_fitting.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_fitting.h` & `hstaxe-1.0.4/cextern/src/spce_fitting.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_is_in.c` & `hstaxe-1.0.4/cextern/src/spce_is_in.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_is_in.h` & `hstaxe-1.0.4/cextern/src/spce_is_in.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_output.c` & `hstaxe-1.0.4/cextern/src/spce_output.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_output.h` & `hstaxe-1.0.4/cextern/src/spce_output.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_pathlength.c` & `hstaxe-1.0.4/cextern/src/spce_pathlength.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_pgp.c` & `hstaxe-1.0.4/cextern/src/spce_pgp.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_pgp.h` & `hstaxe-1.0.4/cextern/src/spce_pgp.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_sect.c` & `hstaxe-1.0.4/cextern/src/spce_sect.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/spce_sect.h` & `hstaxe-1.0.4/cextern/src/spce_sect.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/specmodel_utils.c` & `hstaxe-1.0.4/cextern/src/specmodel_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/specmodel_utils.h` & `hstaxe-1.0.4/cextern/src/specmodel_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/test_aper_check.c` & `hstaxe-1.0.4/cextern/src/test_aper_check.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/trace_conf.c` & `hstaxe-1.0.4/cextern/src/trace_conf.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/trace_conf.h` & `hstaxe-1.0.4/cextern/src/trace_conf.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/trfit_utils.c` & `hstaxe-1.0.4/cextern/src/trfit_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/cextern/src/trfit_utils.h` & `hstaxe-1.0.4/cextern/src/trfit_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axeException.py` & `hstaxe-1.0.4/hstaxe/axeException.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axeerror.py` & `hstaxe-1.0.4/hstaxe/axeerror.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/config.py` & `hstaxe-1.0.4/hstaxe/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,27 +165,27 @@
 
 
 def getOUTSIM(name=None):
     # return either AXE_OUTSIM_PATH or
     # the pathname to the output file
     # in AXE_OUTSIM_PATH
     if name is None:
-        return AXE_OUTSIM_PATH
+        return __user_paths['AXE_OUTSIM_PATH']
     else:
-        return os.path.join(AXE_OUTSIM_PATH, name)
+        return os.path.join(__user_paths['AXE_OUTSIM_PATH'], name)
 
 
 def getSIMDATA(name=None):
     # return either AXE_SIMDATA_PATH or
     # the pathname to the input file
     # in AXE_SIMDATA_PATH
     if name is None:
-        return AXE_SIMDATA_PATH
+        return __user_paths['AXE_SIMDATA_PATH']
     else:
-        return os.path.join(AXE_SIMDATA_PATH, name)
+        return os.path.join(__user_paths['AXE_SIMDATA_PATH'], name)
 
 
 def getDRIZZLE(name=None):
     # return either AXE_DRIZZLE_PATH or
     # the pathname to the input file
     # in AXE_DRIZZLE_PATH
     if name is None:
```

### Comparing `hstaxe-1.0.3/hstaxe/utils.py` & `hstaxe-1.0.4/hstaxe/utils.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesim/WCSdata.py` & `hstaxe-1.0.4/hstaxe/axesim/WCSdata.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesim/axesim_verify.py` & `hstaxe-1.0.4/hstaxe/axesim/axesim_verify.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesim/axesimtasks.py` & `hstaxe-1.0.4/hstaxe/axesim/axesimtasks.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesim/imagemaker.py` & `hstaxe-1.0.4/hstaxe/axesim/imagemaker.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,52 +38,52 @@
         self.conf = configfile.ConfigFile(confname)
 
         # load the pre-defined image information
         image_data = self._get_image_data(self.conf)
 
         # check whether a grism image
         # shall be created
-        if image_data['grism'] != None and griname != None:
+        if image_data['grism'] is not None and griname is not None:
             self.griname  = griname
             self.gridata  = image_data['grism']
             self.WCSimage = griname
             self.WCSext   = '[SCI]'
         else:
             self.griname = None
             self.gridata = None
 
         # check whether a direct image
         # shall be created
-        if dirname != None:
+        if dirname is not None:
             self.dirname  = dirname
             self.WCSimage = dirname
             self.WCSext   = '[SCI]'
 
-            if image_data['direct'] != None:
+            if image_data['direct'] is not None:
                 self.dirdata  = image_data['direct']
             else:
                 self.dirdata  = image_data['grism']
         else:
             self.dirname = None
             self.dirdata = None
 
         # store the drizzle metadata
         if 'drizzle' in image_data:
             self.drzdata  = image_data['drizzle']
         else:
             self.drzdata  = None
 
         # store the x-dimension
-        if nx != None:
+        if nx is not None:
             self.nx = nx
         else:
             self.nx = image_data['dimension'][0]
 
         # store the y-dimension
-        if ny != None:
+        if ny is not None:
             self.ny = ny
         else:
             self.ny = image_data['dimension'][1]
 
     def _get_image_data(self, conf):
         """
         Determines the pre-defined image information
@@ -96,15 +96,15 @@
         """
         from . import WCSdata
 
         # load the WCS for the various grism modes
         if self.conf['CAMERA'] == 'HRC':
             # in case that several orders exist OR
             # the XOFFSET value is larger than -100, its HRG/G800L
-            if self.conf['B'] != None or float(self.conf['A']['XOFF_'].split()[0]) > -100.0:
+            if self.conf['B'] is not None or float(self.conf['A']['XOFF_'].split()[0]) > -100.0:
                 image_data = WCSdata.get_HRC_G800L_WCS()
             else:
                 image_data = WCSdata.get_HRC_PR200L_WCS()
 
         elif self.conf['CAMERA'] == 'SBC':
             # in case that the singularity is more than
             # -90 away from the reference point, its PR110L
@@ -139,40 +139,40 @@
     def deleteImages(self):
         """
         Deletes all images
 
         The method deletes the dummy images of the class instance.
         """
         # check whether there should exist a grism image
-        if self.griname != None:
+        if self.griname is not None:
             # check whether it exists and delete it
             if os.path.isfile(self.griname):
                 os.unlink(self.griname)
 
         # check whether there should exist a direct image
-        if self.dirname != None:
+        if self.dirname is not None:
             # check whether it exists and delete it
             if os.path.isfile(self.dirname):
                 os.unlink(self.dirname)
 
     def makeImages(self):
         """
         Makes all images
 
         The method lets all images be generated.
         """
         # check whether a grism image
         # shall be created
-        if self.griname != None:
+        if self.griname is not None:
             # make the grism image
             self.makeOneImage(self.griname, self.nx, self.ny, self.gridata, self.drzdata)
 
         # check whether a direct image
         # shall be created
-        if self.dirname != None:
+        if self.dirname is not None:
             # make the direct image
             self.makeOneImage(self.dirname, self.nx, self.ny, self.dirdata, self.drzdata)
 
 
     def makeOneImage(self, imgname, nx, ny, metadata, drzmeta=None):
         """
         Creates one dummy image
@@ -208,15 +208,15 @@
         mex_hdu.append(hdrpr)
 
         # go the the header and put
         # the exposure time
         hdr = mex_hdu[0].header
         hdr.update('EXPTIME', 1.0, 'dummy exposure time')
 
-        if drzmeta != None:
+        if drzmeta is not None:
             # update the header
             for item in drzmeta:
                 hdr.update(item[0], item[1], item[2])
 
 
         # write the image and close it
         mex_hdu.writeto(imgname)
```

### Comparing `hstaxe-1.0.3/hstaxe/axesim/interpolator.py` & `hstaxe-1.0.4/hstaxe/axesim/interpolator.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import copy
 import math
 import logging
 
 from astropy.io import fits
 from .. import axe_asciidata
-from ..axeerror import aXeError
+from ..axeerror import aXeError, aXeSIMError
 
 from hstaxe.utils import set_logging
 
 # make sure there is a logger
 _log = logging.getLogger(__name__)
 _log = set_logging()  # defaults to INFO
```

### Comparing `hstaxe-1.0.3/hstaxe/axesim/modspeclist.py` & `hstaxe-1.0.4/hstaxe/axesim/modspeclist.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesim/realworld.py` & `hstaxe-1.0.4/hstaxe/axesim/realworld.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesim/templateimages.py` & `hstaxe-1.0.4/hstaxe/axesim/templateimages.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesim/templatespectra.py` & `hstaxe-1.0.4/hstaxe/axesim/templatespectra.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/axecommands.py` & `hstaxe-1.0.4/hstaxe/axesrc/axecommands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 See LICENSE.txt
 """
-import sys
-import shutil
+import os
 import logging
+import shutil
+import sys
 
 from astropy.io import fits
 
 from hstaxe import config as config_util
 
 from . import axetasks
 from .axeerror import aXeSIMError
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/axeinputs.py` & `hstaxe-1.0.4/hstaxe/axesrc/axeinputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 
         columns.reverse()
         name = columns.pop()
         if ((np.issubsctype(self._inimlist[name], np.str)) and
                 ('fits' in self._inimlist[name][0])):
             self._inimlist.rename_column(name, 'grisim')
         else:
-            err_msg = (f"Column 1 should be the names of the grism"
-                       " fits files: {self._inimlist}")
+            err_msg = ("Column 1 should be the names of the grism"
+                       f" fits files: {self._inimlist}")
             raise aXeError(err_msg)
 
         # check whether second column has type string
         name = columns.pop()
         if np.issubsctype(self._inimlist[name], np.str):
             self._inimlist.rename_column(name, 'objcat')
         else:
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/axeiol.py` & `hstaxe-1.0.4/hstaxe/axesrc/axeiol.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/axelowlev.py` & `hstaxe-1.0.4/hstaxe/axesrc/axelowlev.py`

 * *Files 0% similar despite different names*

```diff
@@ -1343,15 +1343,15 @@
 
         # put the config file name to the list
         self.command_list.append(config)
 
         # check for the 'FFNAME' name
         if ffname:
             # put the name to the list
-            self.command_list.append('-FFNAME={0:s}'.format(params['ffname']))
+            self.command_list.append(f'-FFNAME={ffname}')
 
         # append the flag 'bck'
         if back:
             # put the according flag to the list
             self.command_list.append('-bck')
 
 
@@ -1518,18 +1518,18 @@
         # check for the 'out_STP' name
         if (params['out_stp'] is not None):
             # put the name to the list
             self.command_list.append('-out_STP={0:s}'
                                      .format(params['out_stp']))
 
         # append the flag 'drz'
-        if (params['sampling'] is 'drizzle'):
+        if (params['sampling'] == 'drizzle'):
             # put the flagg to the list
             self.command_list.append('-drzstamp')
-        elif (params['sampling'] is 'rectified'):
+        elif (params['sampling'] == 'rectified'):
             # put the flagg to the list
             self.command_list.append('-rectified')
 
         # append the flag 'drz'
         if (params['drzpath']):
             # put the according flag to the list
             self.command_list.append('-drz')
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/axepreptor.py` & `hstaxe-1.0.4/hstaxe/axesrc/axepreptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     -----
     axeprep provides three different processing steps:
 
     background subtraction:  Provided that an Input Object List is given for
         the grism image, axeprep uses the tasks sex2gol, gol2af and backest
         to mark the beam areas on the grism image as well as on the master
         background image. The median pixel values are derived for the unmarked
-        pixels on both the grism image and on the master background image. 
+        pixels on both the grism image and on the master background image.
         The master background, scaled to the level of the grism image, is
         finally subtracted from the grism image.
 
     exposure time normalization:
         The input file is normalized by the exposure time to transform the
         images into counts per second.
 
@@ -176,21 +176,21 @@
         axe_names = config_util.get_axe_names(self.grisim, ext_info)
         msk_image_sc = axe_names['MSK'] + '[SCI]'
 
         # check for a previous background subtraction
         with fits.open(self.grisim, mode='update') as grism_file:
             if 'AXEPRBCK' in grism_file[ext_info['fits_ext']].header:
                 # warn that this is the second time
-                _log.info("WARNING: Image %25s seems to be already background "
-                      "subtracted!".format(self.grisim))
+                _log.info(f"WARNING: Image {self.grisim} seems to be already "
+                          "background subtracted!")
 
             # Compute the ratio of the grism SCI image to the background image
             sci_data = grism_file['SCI', ext_info['ext_version']].data
             sci_header = grism_file['SCI', ext_info['ext_version']].header
-            npix = int(sci_header["NAXIS1"]) * int(sci_header["NAXIS2"]) 
+            npix = int(sci_header["NAXIS1"]) * int(sci_header["NAXIS2"])
 
             bck_data = fits.getdata(self.master_bck)
             ratio_data = sci_data / bck_data
 
             # Flag pixels in the ratio image based on the grism image DQ array
             grism_dq_data = grism_file['DQ', ext_info['ext_version']].data
             ratio_data[grism_dq_data > 0.5] = flag
@@ -219,15 +219,15 @@
                                           upper=None, nclip=3, lsig=3.0, usig=3.0,
                                           binwidth=0.01)
 
             # Subtract the scaled background from the grism image
             # Reload a clean version of background
             bck_data = fits.getdata(self.master_bck)
 
-            grism_file['SCI', ext_info['ext_version']].data -= bck_data * stats.midpt 
+            grism_file['SCI', ext_info['ext_version']].data -= bck_data * stats.midpt
             grism_header = grism_file['SCI', ext_info['ext_version']].header
 
             # write some header iformation
             grism_header['SKY_SCAL'] = (float(stats.midpt),  'scaling value for the master background')
             grism_header['SKY_MAST'] = (float(bstats.midpt),  'average value of the master background')
             grism_header['SKY_IMG'] = (self.master_bck, 'name of the master background image')
             grism_header['F_SKYPIX'] = (float(stats.npix)/float(npix), 'fraction of pixels used for scaling')
@@ -392,23 +392,23 @@
 
         else:
             # make normal background subtraction
             goodreturn = self._subtract_sky(ext_info)
 
         if goodreturn:
             pstring = (f"AXEPREP: Image {self.grisim}[SCI,{str(ext_info['ext_version'])}] sky-subtracted.")
-                       
+
             _log.info(pstring)
 
     def _check_low_skyfrac(self, frac):
         """Check for a low fraction of background pixels"""
 
         msg = (f"\nAXEPREP Image {self.grisim}: Only {frac*100.0} percent of the pixels "
                "were used in the background scaling!")
-                                                             
+
         raise aXeError(msg)
 
     def _check_second_normalization(self):
         """Check whether the data is already normalized.
         """
 
         msg = (f"AXEPREP: Image {self.grisim} has already been normalized! Will not renormalize")
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/axesingextr.py` & `hstaxe-1.0.4/hstaxe/axesrc/axesingextr.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/axetasks.py` & `hstaxe-1.0.4/hstaxe/axesrc/axetasks.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/configfile.py` & `hstaxe-1.0.4/hstaxe/axesrc/configfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             # check for existence
             if index > -1:
 
                 # extract the keyvalue
                 kvalue = self.gkeys[index].keyvalue
 
                 # if the keyvalue is NOT None but the file does not exist
-                if ((kvalue.upper() is not 'NONE') and
+                if ((kvalue.upper() != 'NONE') and
                     (not os.path.isfile(config_util.getCONF(kvalue)))):
                     # report an error
                     err_msg = ("The file: {0:s} does not exist!"
                                .format(config_util.getCONF(kvalue)))
                     raise aXeError(err_msg)
 
     def get_gkey(self, keyword):
@@ -951,15 +951,15 @@
 
             # go over all beam keys
             for bkey in self.beamkeys:
 
                 # check whether the current keyword is right
                 # and whether the keyvalue is not 'None'
                 if ((bkey.keyword is full_keyword) and
-                     (bkey.keyvalue.upper() is not 'NONE')):
+                     (bkey.keyvalue.upper() != 'NONE')):
                     # check for the file
                     if not os.path.isfile(config_util.getCONF(bkey.keyvalue)):
                         # report an error
                         err_msg = ("The file: {0:s} does not exist!"
                                    .format(config_util.getCONF(bkey.keyvalue)))
                         raise aXeError(err_msg)
                     else:
@@ -1378,15 +1378,15 @@
                     if start:
                         # strip the line
                         str_line = line.strip()
 
                         # check whether the first character
                         # is a comment, which qualifies
                         # the line as part of the header
-                        if ((len(str_line) > 0) and (str_line[0] is '#')):
+                        if ((len(str_line) > 0) and (str_line[0] == '#')):
                             # append the line to the header data
                             self.header.append(line.strip()+'\n')
                         else:
                             # set the starter pointer to 0,
                             # thus indicating the end of the header
                             start = 0
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/dither.py` & `hstaxe-1.0.4/hstaxe/axesrc/dither.py`

 * *Files 4% similar despite different names*

```diff
@@ -381,30 +381,30 @@
     def _absoluteSubtract(self, array, tmpArray, outArray):
         """
         Subtract the absolute value of two images
         """
         # subtract shifted image from imput image
         tmpArray = array - tmpArray
         # take the absolute value of tmpArray
-        tmpArray = numpy.fabs(tmpArray)
+        tmpArray = np.fabs(tmpArray)
         # save maximum value of outArray or tmpArray and save in outArray
-        outArray = numpy.maximum(tmpArray, outArray)
+        outArray = np.maximum(tmpArray, outArray)
         # zero out tmpArray before reuse
         tmpArray = tmpArray * 0.
 
         return (tmpArray, outArray)
 
     def _qderiv(self, array):
         """
         Take the absolute derivate of an image in memory
         """
 
         # Create 2 empty arrays in memory of the same dimensions as 'array'
-        tmpArray = numpy.zeros(array.shape, dtype=numpy.float64)
-        outArray = numpy.zeros(array.shape, dtype=numpy.float64)
+        tmpArray = np.zeros(array.shape, dtype=np.float64)
+        outArray = np.zeros(array.shape, dtype=np.float64)
 
         # Get the length of an array side
         (naxis1, naxis2) = array.shape
 
         # Main derivate loop:
         # Shift images +/- 1 in Y.
         for y in range(-1, 2, 2):
@@ -440,15 +440,15 @@
                                                           tmpArray,
                                                           outArray)
 
         # delete the tmp-array
         del tmpArray
 
         # return the result
-        return outArray.astype(numpy.float32)
+        return outArray.astype(np.float32)
 
     def run(self, in_name, out_name):
         """Code stolen from Multidrizzle.deriv()"""
         # store the names
         self.in_name = in_name
         self.out_name = out_name
 
@@ -501,56 +501,56 @@
         """Identify cosmic rays and other deviant pixels.
 
         The code was taken from muldidrizzle.DrizCR. Small adjustments and
         re-factoring was done.
         """
 
         # create an empty file
-        __crMask = numpy.zeros(in_img.shape, dtype=numpy.uint8)
+        __crMask = np.zeros(in_img.shape, dtype=np.uint8)
 
         # Part 1 of computation:
         # flag the central pixels
         # Create a temp array mask
-        __t1 = numpy.absolute(in_img - blot_img)
-        __ta = numpy.sqrt(numpy.absolute(blot_img * exptime
+        __t1 = np.absolute(in_img - blot_img)
+        __ta = np.sqrt(np.absolute(blot_img * exptime
                                          + sky_val * exptime) +
                           self.rdnoise*self.rdnoise)
         __t2 = self.driz_cr_scale[0] * blotder_img + self.driz_cr_snr[0] * __ta / exptime
-        __tmp1 = numpy.logical_not(numpy.greater(__t1, __t2))
+        __tmp1 = np.logical_not(np.greater(__t1, __t2))
 
         # mop up
         del __ta
         del __t1
         del __t2
 
         # Create a convolution kernel that is 3 x 3 of 1's
-        __kernel = numpy.ones((3, 3), dtype=numpy.uint8)
+        __kernel = np.ones((3, 3), dtype=np.uint8)
         # Create an output tmp file the same size as the input temp mask array
-        __tmp2 = numpy.zeros(__tmp1.shape, dtype=numpy.int16)
+        __tmp2 = np.zeros(__tmp1.shape, dtype=np.int16)
         # Convolve the mask with the kernel
         convolve.convolve2d(__tmp1,
                             __kernel,
                             output=__tmp2,
                             fft=0,
                             mode='nearest',
                             cval=0)
         del __kernel
         del __tmp1
 
         # Part 2 of computation
         # flag the neighboring pixels
         # Create the CR Mask
-        __xt1 = numpy.absolute(in_img - blot_img)
-        __xta = numpy.sqrt(numpy.absolute(blot_img * exptime +
+        __xt1 = np.absolute(in_img - blot_img)
+        __xta = np.sqrt(np.absolute(blot_img * exptime +
                                           sky_val * exptime) +
                            self.rdnoise*self.rdnoise)
         __xt2 = self.driz_cr_scale[1] * blotder_img + self.driz_cr_snr[1] * __xta / exptime
 
         # It is necessary to use a bitwise 'and' to create the mask with numarray objects.
-        __crMask = numpy.logical_not(numpy.greater(__xt1, __xt2) & numpy.less(__tmp2,9) )
+        __crMask = np.logical_not(np.greater(__xt1, __xt2) & np.less(__tmp2,9) )
 
         del __xta
         del __xt1
         del __xt2
         del __tmp2
 
         # Part 3 of computation - flag additional cte 'radial'
@@ -562,26 +562,26 @@
         # from which 2 new arrays are created having 0->bad and 1->good.
         # These 2 new arrays are then 'anded'
         # to create a new __crMask.
 
         # recast __crMask to int for manipulations below;
         # will recast to Bool at end
         __crMask_orig_bool = __crMask.copy()
-        __crMask = __crMask_orig_bool.astype(numpy.int8)
+        __crMask = __crMask_orig_bool.astype(np.int8)
 
         # make radial convolution kernel and convolve it with original __crMask
         # kernel for radial masking of CR pixel
-        cr_grow_kernel = numpy.ones((self.driz_cr_grow, self.driz_cr_grow))
+        cr_grow_kernel = np.ones((self.driz_cr_grow, self.driz_cr_grow))
         cr_grow_kernel_conv = __crMask.copy()   # for output of convolution
         convolve.convolve2d(__crMask,
                             cr_grow_kernel,
                             output=cr_grow_kernel_conv)
 
         # make tail convolution kernel and convolve it with original __crMask
-        cr_ctegrow_kernel = numpy.zeros((2*self.driz_cr_ctegrow+1,
+        cr_ctegrow_kernel = np.zeros((2*self.driz_cr_ctegrow+1,
                                          2*self.driz_cr_ctegrow+1))  # kernel for tail masking of CR pixel
         cr_ctegrow_kernel_conv = __crMask.copy()  # for output convolution
 
         # which pixels are masked by tail kernel depends on sign of
         # ctedir (i.e., readout direction):
         ctedir = 0
         if (ctedir == 1):  # HRC: amp C or D ; WFC: chip = sci,1 ; WFPC2
@@ -591,19 +591,19 @@
         if (ctedir == 0):  # NICMOS: no cte tail correction
             pass
 
         # do the convolution
         convolve.convolve2d(__crMask, cr_ctegrow_kernel, output = cr_ctegrow_kernel_conv)
 
         # select high pixels from both convolution outputs; then 'and' them to create new __crMask
-        where_cr_grow_kernel_conv = numpy.where(cr_grow_kernel_conv < self.driz_cr_grow*self.driz_cr_grow,0,1 )        # radial
-        where_cr_ctegrow_kernel_conv = numpy.where(cr_ctegrow_kernel_conv < self.driz_cr_ctegrow, 0, 1 )     # length
-        __crMask = numpy.logical_and(where_cr_ctegrow_kernel_conv, where_cr_grow_kernel_conv) # combine masks
+        where_cr_grow_kernel_conv = np.where(cr_grow_kernel_conv < self.driz_cr_grow*self.driz_cr_grow,0,1 )        # radial
+        where_cr_ctegrow_kernel_conv = np.where(cr_ctegrow_kernel_conv < self.driz_cr_ctegrow, 0, 1 )     # length
+        __crMask = np.logical_and(where_cr_ctegrow_kernel_conv, where_cr_grow_kernel_conv) # combine masks
 
-        __crMask = __crMask.astype(numpy.uint8)  # cast back to Bool
+        __crMask = __crMask.astype(np.uint8)  # cast back to Bool
 
         del __crMask_orig_bool
         del cr_grow_kernel
         del cr_grow_kernel_conv
         del cr_ctegrow_kernel
         del cr_ctegrow_kernel_conv
         del where_cr_grow_kernel_conv
@@ -614,33 +614,33 @@
 
     def _createcrmaskfile(self, crName = None, crmask = None, header = None, in_imag=None):
         """
         Create a fits file containing the generated cosmic ray mask.
         """
 
         # migrate the data over
-        _cr_file = numpy.zeros(in_imag.shape,numpy.uint8)
-        _cr_file = numpy.where(crmask,1,0).astype(numpy.uint8)
+        _cr_file = np.zeros(in_imag.shape,np.uint8)
+        _cr_file = np.where(crmask,1,0).astype(np.uint8)
 
         # rmove file if it exists
         if os.path.isfile(crName):
             os.unlink(crName)
 
         # Create the output file
         fitsobj = fits.HDUList()
 
         if (header is not None):
-            del(header['NAXIS1'])
-            del(header['NAXIS2'])
+            del header['NAXIS1']
+            del header['NAXIS2']
             if 'XTENSION' in header:
-                del(header['XTENSION'])
+                del header['XTENSION']
             if 'EXTNAME' in header:
-                del(header['EXTNAME'])
+                del header['EXTNAME']
             if 'EXTVER' in header:
-                del(header['EXTVER'])
+                del header['EXTVER']
             if 'NEXTEND' in header:
                 header['NEXTEND'] = 0
 
             hdu = fits.PrimaryHDU(data=_cr_file, header=header)
             del hdu.header['PCOUNT']
             del hdu.header['GCOUNT']
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/dppdumps.py` & `hstaxe-1.0.4/hstaxe/axesrc/dppdumps.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/drizzleobjects.py` & `hstaxe-1.0.4/hstaxe/axesrc/drizzleobjects.py`

 * *Files 0% similar despite different names*

```diff
@@ -978,15 +978,15 @@
             # get the number
             num_driz = header['NUM_DRIZ']
 
             # go over all images
             for index in range(num_driz):
 
                 # form the keyword
-                img_kword = "IMG{0:04d".format(index + 1)
+                img_kword = "IMG{0:04d}".format(index + 1)
 
                 # check whether the image name is reported and
                 # whether there is data on the rejection
                 if img_kword in header and header[img_kword] in reject_info:
 
                     # store the number of pixels
                     kword1 = "NRE{0:04d}".format(index + 1)
@@ -1427,15 +1427,15 @@
                                                  .format(file_root, objID))
             ext_names['SING_WHT'] = os.path.join(drztmp_dir,
                                                  '{0:s}_single_wht_{1:s}.fits'
                                                  .format(file_root, objID))
 
             # name of the drizzle coefficients file
             ext_names['CFF'] = os.path.join(drztmp_dir,
-                                            '{0:s}_flt_coeffs{0:s}.dat'
+                                            '{0:s}_flt_coeffs{1:s}.dat'
                                             .format(file_root, objID))
 
         # return the dictionary
         return ext_names
 
     def _get_header_info(self):
         """Set the exposure time from the object contributor."""
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/fcubeobjs.py` & `hstaxe-1.0.4/hstaxe/axesrc/fcubeobjs.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             blot_wcs = HSTWCS(image_to_blot,
                               ext=(str(self.fcube_info["ext_nam"]),
                                    str(self.fcube_info["ext_ver"])))
             image_data = fits.getdata(image_to_blot,
                                       extname=str(self.fcube_info["ext_nam"]),
                                       extver=int(self.fcube_info["ext_nam"]))
 
-        elif (ftype is 'simple'):
+        elif (ftype == 'simple'):
             blot_wcs = HSTWCS(image_to_blot)  # assume simple
             image_data = fits.getdata(image_to_blot)
 
         else:
             return IOError("File type of fits image is not "
                            "supported {0:s}".format(image_to_blot))
 
@@ -310,30 +310,30 @@
         flt_header = fits.getheader(input_image)
         flt_wcs = HSTWCS(self.data)
 
         # check to see if this is a simple fits or MEF and grab
         # the science information.
         ftype = fileutil.isFits(self.grism_image_name)[1]
 
-        if (ftype is 'mef'):
+        if (ftype == 'mef'):
             grism_wcs = HSTWCS(self.grism_image_name,
                                ext=(str(self.fcube_info["ext_nam"]),
                                     self.fcube_info["ext_ver"]))
-        elif (ftype is 'simple'):
+        elif (ftype == 'simple'):
             grism_wcs = HSTWCS(self.grism_image_name)
         else:
             return IOError("File type of fits image is not "
                            "supported {0:s}".format(image_to_blot))
 
         ftype = fileutil.isFits(image_to_blot)[1]
-        if (ftype is 'mef'):
+        if (ftype == 'mef'):
             image_data = fits.getdata(image_to_blot,
                                       ext=(str(self.fcube_info["ext_nam"]),
                                            self.fcube_info["ext_ver"]))
-        elif (ftype is 'simple'):
+        elif (ftype == 'simple'):
             image_data = fits.getdata(image_to_blot)
         else:
             return IOError("Input image is not a supported FITS "
                            "type: {0:s}".format(image_to_blot))
 
         # edit the wcs header information to add any dim_info shifts that we
         # need the segment image needs to be the same sky area cut without
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/imagemaker.py` & `hstaxe-1.0.4/hstaxe/axesrc/imagemaker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 See LICENSE.txt
 """
 import logging
+import os
 
 from astropy.io import fits
 
 from hstaxe import axeerror
+from hstaxe.config import get_random_filename
 
 from . import configfile
 
 # make sure there is a logger
 _log = logging.getLogger(__name__)
 
+
 class DummyImages:
     """
     Small class to create dummy images for the simulations
 
     This class creates empty dispersed and direct images as dummies.
     Since all aXe C-executables need the dispersed image as an input,
     such an image must exist for making the simualtions.
@@ -44,15 +47,15 @@
         self.conf = configfile.ConfigFile(confname)
 
         # load the pre-defined image information
         image_data = self._get_image_data(self.conf)
 
         # check whether a grism image
         # shall be created
-        if image_data['grism'] != None and griname != None:
+        if image_data['grism'] is not None and griname is not None:
             self.griname  = griname
             self.gridata  = image_data['grism']
             self.WCSimage = griname
             self.WCSext   = '[SCI]'
         else:
             self.griname = None
             self.gridata = None
@@ -102,15 +105,15 @@
         """
         from . import WCSdata
 
         # load the WCS for the various grism modes
         if self.conf['CAMERA'] == 'HRC':
             # in case that several orders exist OR
             # the XOFFSET value is larger than -100, its HRG/G800L
-            if self.conf['B'] != None or float(self.conf['A']['XOFF_'].split()[0]) > -100.0:
+            if self.conf['B'] is not None or float(self.conf['A']['XOFF_'].split()[0]) > -100.0:
                 image_data = WCSdata.get_HRC_G800L_WCS()
             else:
                 image_data = WCSdata.get_HRC_PR200L_WCS()
 
         elif self.conf['CAMERA'] == 'SBC':
             # in case that the singularity is more than
             # -90 away from the reference point, its PR110L
@@ -213,15 +216,15 @@
         mex_hdu.append(hdrpr)
 
         # go the the header and put
         # the exposure time
         hdr = mex_hdu[0].header
         hdr['EXPTIME'] = (1.0, 'dummy exposure time')
 
-        if drzmeta != None:
+        if drzmeta is not None:
             # update the header
             for item in drzmeta:
                 hdr[item[0]] = (item[1], item[2])
 
         # write the image and close it
         mex_hdu.writeto(imgname)
         mex_hdu.close()
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/inputchecks.py` & `hstaxe-1.0.4/hstaxe/axesrc/inputchecks.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,35 +193,35 @@
         Comprises all file and file format checks for AXECORE
         """
 
         # check the IOL's
         self._check_IOL()
 
         # check the fluxcubes, if necessary
-        if cont_model.lower() is 'fluxcube':
+        if cont_model.lower() == 'fluxcube':
             self._check_fluxcubes()
 
         # check whether it is prism data
         if self._is_prism_data():
             #
             # NOTE: these checks are not exactly
             #       related to files.....
             #
             # make sure that there are
             # direct images
             self._force_dirim()
 
             # the fluxcube contamination does not work for prism data
-            if cont_model.lower() is "fluxcube":
+            if cont_model.lower() == "fluxcube":
                 err_msg = ("{0:s}: Fluxcube contamination is not possible for "
                            "prism data!".format(self.taskname))
                 raise aXeError(err_msg)
 
             # drizzled stamp images are not supported for prism data
-            if sampling.lower() is "drizzle":
+            if sampling.lower() == "drizzle":
                 err_msg = ("{0:s}: Drizzle sampling for the stamp images is "
                            "not possible for prism data!".format(self.taskname))
                 raise aXeError(err_msg)
 
         # the extraction width must be set!
         if not extrfwhm:
             err_msg = ("{0:s}: extrfwhm must be > 0.0 to create PETs, but "
@@ -289,15 +289,15 @@
         if back and interp is None:
             err_msg = ("{0:s}: The parameter 'interp' must be set for the "
                        "background PETs!".format(self.taskname))
             raise aXeError(err_msg)
 
         # check for proper contamination
         # to allow optimal extraction
-        if ((cont_model is "geometric") and (weights)):
+        if ((cont_model == "geometric") and (weights)):
             err_msg = ("{0:s}: Optimal weigthing needs quantitative "
                        "contamination! Please change to either the 'gauss'"
                        " or 'fluxcube' contamination model or drop optimal "
                        "weighting!".format(self.taskname))
             raise aXeError(err_msg)
 
     def check_axedrizzle(self, infwhm, outfwhm, back=False):
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/iolmaking.py` & `hstaxe-1.0.4/hstaxe/axesrc/iolmaking.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/mefobjects.py` & `hstaxe-1.0.4/hstaxe/axesrc/mefobjects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
 See LICENSE.txt
 """
 import os
+
 import numpy as np
+from astropy.table import Table
 from astropy.io import fits
+
 from hstaxe import config as config_utils
 from hstaxe.axeerror import aXeError
+
 from . import configfile
 
 
 class MEFExtractor:
     """Multi-Extension FITS Extractor class"""
     def __init__(self, drizzle_params, obj_dol=None, bck_dol=None, opt_extr=None):
         """
```

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/nlincoeffs.py` & `hstaxe-1.0.4/hstaxe/axesrc/nlincoeffs.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/axesrc/pysex2gol.py` & `hstaxe-1.0.4/hstaxe/axesrc/pysex2gol.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,21 +98,21 @@
     def __str__(self):
         """String method for the class"""
         # define the prefix
         prefix = "py_SEX2GOL: "
 
         # compose the feedback
         big_str = "{0:s}  Setup:\n".format(prefix)
-        big_str += "{0:s}  Input g/prism image:      {0:s} \n".format(prefix, self.grisim)
-        big_str += "{0:s}  Configuration file name:  {0:s} \n".format(prefix, self.config)
-        big_str += "{0:s}  Direct image:             {0:s} \n".format(prefix, self.dirname)
-        big_str += "{0:s}  G/Prism extension:        {0:s} \n".format(prefix, self.grism_extinfo['axe_ext'])
-        big_str += "{0:s}  Direct image extension:   {0:s} \n".format(prefix, self.dirname_extinfo['axe_ext'])
-        big_str += "{0:s}  Input catalog name:       {0:s} \n".format(prefix, self.in_sex)
-        big_str += "{0:s}  Output catalog name:      {0:s}   ".format(prefix, self.out_sex)
+        big_str += "{0:s}  Input g/prism image:      {1:s} \n".format(prefix, self.grisim)
+        big_str += "{0:s}  Configuration file name:  {1:s} \n".format(prefix, self.config)
+        big_str += "{0:s}  Direct image:             {1:s} \n".format(prefix, self.dirname)
+        big_str += "{0:s}  G/Prism extension:        {1:s} \n".format(prefix, self.grism_extinfo['axe_ext'])
+        big_str += "{0:s}  Direct image extension:   {1:s} \n".format(prefix, self.dirname_extinfo['axe_ext'])
+        big_str += "{0:s}  Input catalog name:       {1:s} \n".format(prefix, self.in_sex)
+        big_str += "{0:s}  Output catalog name:      {1:s}   ".format(prefix, self.out_sex)
 
         # return the string
         return big_str
 
     def _cleanup(self):
         """Clean up files created for stdout
```

### Comparing `hstaxe-1.0.3/hstaxe/tests/coveragerc` & `hstaxe-1.0.4/hstaxe/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/run_acs_cookbook.py` & `hstaxe-1.0.4/hstaxe/tests/run_acs_cookbook.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/run_cookbook.py` & `hstaxe-1.0.4/hstaxe/tests/run_cookbook.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/run_cookbook_part2.py` & `hstaxe-1.0.4/hstaxe/tests/run_cookbook_part2.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_af2pet.py` & `hstaxe-1.0.4/hstaxe/tests/test_af2pet.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_axecore.py` & `hstaxe-1.0.4/hstaxe/tests/test_axecore.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_axeprep.py` & `hstaxe-1.0.4/hstaxe/tests/test_axeprep.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_be.py` & `hstaxe-1.0.4/hstaxe/tests/test_be.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_gol2af.py` & `hstaxe-1.0.4/hstaxe/tests/test_gol2af.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_iolprep.py` & `hstaxe-1.0.4/hstaxe/tests/test_iolprep.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_pet2spc.py` & `hstaxe-1.0.4/hstaxe/tests/test_pet2spc.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_petcont.py` & `hstaxe-1.0.4/hstaxe/tests/test_petcont.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_petff.py` & `hstaxe-1.0.4/hstaxe/tests/test_petff.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_scalebck.py` & `hstaxe-1.0.4/hstaxe/tests/test_scalebck.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_sex2gol.py` & `hstaxe-1.0.4/hstaxe/tests/test_sex2gol.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/hstaxe/tests/test_stamps.py` & `hstaxe-1.0.4/hstaxe/tests/test_stamps.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/.gitignore` & `hstaxe-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/LICENSE.txt` & `hstaxe-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/README.md` & `hstaxe-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,25 @@
 employed under Linux, Solaris, and MacOS X.
 
 HSTaXe is the successor to aXe, a similar package written on PyRAF/IRAF.
 
 
 Quickstart
 ----------
-To install the latest release of ``hstaxe``::
+To install the latest release of ``hstaxe``, we recommend the following steps::
 
     conda create --name hstaxe-env "python>=3.8, <3.11"
     conda activate hstaxe-env
     conda install gsl cfitsio make automake autoconf libtool pkg-config -y
     conda install wcstools -c https://conda.anaconda.org/conda-forge/ --override-channels -y
-    pip install hstaxe
+    pip install hstaxe --no-cache-dir
 
 For additional installation instructions, including instructions on installing older
 or development versions of hstaxe, visit our full documentation:
 https://hstaxe.readthedocs.io/en/latest/hstaxe/installing.html
 
 Example notebooks can also be found on our full documentation:
 https://hstaxe.readthedocs.io/en/latest/hstaxe/examples.html
+
+To run the notebooks, you will need to install jupyter::
+
+    pip install jupyter
```

### Comparing `hstaxe-1.0.3/hatch_build.py` & `hstaxe-1.0.4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/pyproject.toml` & `hstaxe-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.3/PKG-INFO` & `hstaxe-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstaxe
-Version: 1.0.3
+Version: 1.0.4
 Summary: Spectral extraction tools for Hubble Space Telescope Grisms
 Project-URL: Homepage, https://github.com/spacetelescope/hstaxe
 Author-email: hstaxe and aXe developers <help@stsci.edu>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -47,21 +47,25 @@
 employed under Linux, Solaris, and MacOS X.
 
 HSTaXe is the successor to aXe, a similar package written on PyRAF/IRAF.
 
 
 Quickstart
 ----------
-To install the latest release of ``hstaxe``::
+To install the latest release of ``hstaxe``, we recommend the following steps::
 
     conda create --name hstaxe-env "python>=3.8, <3.11"
     conda activate hstaxe-env
     conda install gsl cfitsio make automake autoconf libtool pkg-config -y
     conda install wcstools -c https://conda.anaconda.org/conda-forge/ --override-channels -y
-    pip install hstaxe
+    pip install hstaxe --no-cache-dir
 
 For additional installation instructions, including instructions on installing older
 or development versions of hstaxe, visit our full documentation:
 https://hstaxe.readthedocs.io/en/latest/hstaxe/installing.html
 
 Example notebooks can also be found on our full documentation:
 https://hstaxe.readthedocs.io/en/latest/hstaxe/examples.html
+
+To run the notebooks, you will need to install jupyter::
+
+    pip install jupyter
```

