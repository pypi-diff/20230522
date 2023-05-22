# Comparing `tmp/spotPython-0.1.5.tar.gz` & `tmp/spotPython-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotPython-0.1.5.tar", last modified: Sat May 20 09:28:18 2023, max compression
+gzip compressed data, was "spotPython-0.1.7.tar", last modified: Mon May 22 11:19:27 2023, max compression
```

## Comparing `spotPython-0.1.5.tar` & `spotPython-0.1.7.tar`

### file list

```diff
@@ -1,199 +1,210 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.303011 spotPython-0.1.5/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.275191 spotPython-0.1.5/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.278902 spotPython-0.1.5/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.1.5/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)    12649 2023-05-20 04:30:20.000000 spotPython-0.1.5/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.1.5/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.284548 spotPython-0.1.5/Figures.d/
--rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.1.5/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.1.5/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.1.5/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.1.5/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.1.5/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.1.5/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     6730 2023-05-20 09:28:18.302846 spotPython-0.1.5/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     5960 2023-05-19 13:53:04.000000 spotPython-0.1.5/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.285405 spotPython-0.1.5/docs/
--rw-r--r--   0 bartz      (501) staff       (20)   137970 2023-05-20 04:16:59.000000 spotPython-0.1.5/docs/bart23e.html
--rw-r--r--   0 bartz      (501) staff       (20)   335911 2023-05-20 04:17:05.000000 spotPython-0.1.5/docs/bart23e.pdf
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.286873 spotPython-0.1.5/docs/figures/
--rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-19 17:04:41.000000 spotPython-0.1.5/docs/figures/parallel.png
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.287050 spotPython-0.1.5/docs/img/
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-19 13:48:01.000000 spotPython-0.1.5/docs/img/spotLogo.png
--rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-20 04:17:06.000000 spotPython-0.1.5/docs/index.html
--rw-r--r--   0 bartz      (501) staff       (20)    48220 2023-05-20 04:17:05.000000 spotPython-0.1.5/docs/search.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.275923 spotPython-0.1.5/docs/site_libs/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.287926 spotPython-0.1.5/docs/site_libs/bootstrap/
--rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/bootstrap/bootstrap-icons.css
--rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.1.5/docs/site_libs/bootstrap/bootstrap-icons.woff
--rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-20 04:16:58.000000 spotPython-0.1.5/docs/site_libs/bootstrap/bootstrap.min.css
--rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/bootstrap/bootstrap.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.288094 spotPython-0.1.5/docs/site_libs/clipboard/
--rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/clipboard/clipboard.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.288897 spotPython-0.1.5/docs/site_libs/quarto-html/
--rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/quarto-html/anchor.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/quarto-html/popper.min.js
--rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-19 12:56:10.000000 spotPython-0.1.5/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
--rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/quarto-html/quarto.js
--rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/quarto-html/tippy.css
--rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/quarto-html/tippy.umd.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.289053 spotPython-0.1.5/docs/site_libs/quarto-nav/
--rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/quarto-nav/quarto-nav.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.289496 spotPython-0.1.5/docs/site_libs/quarto-search/
--rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/quarto-search/autocomplete.umd.js
--rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/quarto-search/fuse.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.1.5/docs/site_libs/quarto-search/quarto-search.js
--rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-26 22:09:11.000000 spotPython-0.1.5/makeSpot.sh
--rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.1.5/mkdocs.yml
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.294189 spotPython-0.1.5/notebooks/
--rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 05:31:37.000000 spotPython-0.1.5/notebooks/00_spot_doc.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 22:27:42.000000 spotPython-0.1.5/notebooks/01_spot_intro.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 08:33:47.000000 spotPython-0.1.5/notebooks/02_spot_multidim.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 22:28:54.000000 spotPython-0.1.5/notebooks/03_spot_anisotropic.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 22:29:50.000000 spotPython-0.1.5/notebooks/04_spot_sklearn_surrogate.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 22:30:17.000000 spotPython-0.1.5/notebooks/05_spot_sklearn_optimizers.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 22:30:52.000000 spotPython-0.1.5/notebooks/06_spot_gaussian.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 22:31:54.000000 spotPython-0.1.5/notebooks/07_spot_ei.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 22:32:20.000000 spotPython-0.1.5/notebooks/08_spot_noisy.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 22:32:53.000000 spotPython-0.1.5/notebooks/09_spot_ocba.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-20 08:34:43.000000 spotPython-0.1.5/notebooks/10_spot_hpt_sklearn_classification.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    23215 2023-05-20 08:35:48.000000 spotPython-0.1.5/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    28105 2023-05-20 08:36:30.000000 spotPython-0.1.5/notebooks/12_spot_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 08:37:13.000000 spotPython-0.1.5/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    82360 2023-05-20 09:27:16.000000 spotPython-0.1.5/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 08:39:17.000000 spotPython-0.1.5/notebooks/15_spot_hpt_sklearn_regression.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   434768 2023-05-20 09:03:56.000000 spotPython-0.1.5/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.276168 spotPython-0.1.5/notebooks/data/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.294355 spotPython-0.1.5/notebooks/data/torch/
--rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.1.5/notebooks/data/torch/model_spot_trained.pt
--rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.1.5/notebooks/data.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.294882 spotPython-0.1.5/notebooks/figures/
--rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.1.5/notebooks/figures/spotModel.graffle
--rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.1.5/notebooks/figures/spotModel.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.1.5/notebooks/figures/spotModel.png
--rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-05-09 06:26:54.000000 spotPython-0.1.5/notebooks/plot.png
--rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-20 08:45:03.000000 spotPython-0.1.5/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-20 09:28:18.303053 spotPython-0.1.5/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.276486 spotPython-0.1.5/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.295047 spotPython-0.1.5/src/spotPython/
--rw-r--r--   0 bartz      (501) staff       (20)      214 2023-05-20 09:28:18.000000 spotPython-0.1.5/src/spotPython/_version.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.295811 spotPython-0.1.5/src/spotPython/budget/
--rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-04-13 18:20:56.000000 spotPython-0.1.5/src/spotPython/budget/ocba.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.296091 spotPython-0.1.5/src/spotPython/build/
--rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-13 19:26:45.000000 spotPython-0.1.5/src/spotPython/build/kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.1.5/src/spotPython/build/surrogates.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.296889 spotPython-0.1.5/src/spotPython/data/
--rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.1.5/src/spotPython/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.1.5/src/spotPython/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)    20734 2023-05-09 23:08:47.000000 spotPython-0.1.5/src/spotPython/data/sklearn_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.1.5/src/spotPython/data/sklearn_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     6154 2023-05-20 09:08:40.000000 spotPython-0.1.5/src/spotPython/data/torch_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.1.5/src/spotPython/data/torch_hyper_dict.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.297261 spotPython-0.1.5/src/spotPython/design/
--rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.1.5/src/spotPython/design/designs.py
--rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.1.5/src/spotPython/design/factorial.py
--rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.1.5/src/spotPython/design/spacefilling.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.297633 spotPython-0.1.5/src/spotPython/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     4169 2023-05-20 08:40:29.000000 spotPython-0.1.5/src/spotPython/fun/hypersklearn.py
--rw-r--r--   0 bartz      (501) staff       (20)     4769 2023-05-20 09:28:12.000000 spotPython-0.1.5/src/spotPython/fun/hypertorch.py
--rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-06 16:12:25.000000 spotPython-0.1.5/src/spotPython/fun/objectivefunctions.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.298048 spotPython-0.1.5/src/spotPython/hyperparameters/
--rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.1.5/src/spotPython/hyperparameters/categorical.py
--rw-r--r--   0 bartz      (501) staff       (20)     3849 2023-05-19 14:05:20.000000 spotPython-0.1.5/src/spotPython/hyperparameters/optimizer.py
--rw-r--r--   0 bartz      (501) staff       (20)    26028 2023-05-07 10:48:32.000000 spotPython-0.1.5/src/spotPython/hyperparameters/values.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.298316 spotPython-0.1.5/src/spotPython/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-02-02 22:52:12.000000 spotPython-0.1.5/src/spotPython/plot/contour.py
--rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 08:41:56.000000 spotPython-0.1.5/src/spotPython/plot/validation.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.298428 spotPython-0.1.5/src/spotPython/spot/
--rw-r--r--   0 bartz      (501) staff       (20)    32443 2023-05-12 15:27:01.000000 spotPython-0.1.5/src/spotPython/spot/spot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.298910 spotPython-0.1.5/src/spotPython/torch/
--rw-r--r--   0 bartz      (501) staff       (20)     1000 2023-05-20 08:56:22.000000 spotPython-0.1.5/src/spotPython/torch/netcifar10.py
--rw-r--r--   0 bartz      (501) staff       (20)      413 2023-05-20 08:56:34.000000 spotPython-0.1.5/src/spotPython/torch/netcore.py
--rw-r--r--   0 bartz      (501) staff       (20)      791 2023-05-20 08:56:44.000000 spotPython-0.1.5/src/spotPython/torch/netfashionMNIST.py
--rw-r--r--   0 bartz      (501) staff       (20)    16047 2023-05-20 09:00:48.000000 spotPython-0.1.5/src/spotPython/torch/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.300449 spotPython-0.1.5/src/spotPython/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.1.5/src/spotPython/utils/aggregate.py
--rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.1.5/src/spotPython/utils/classes.py
--rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.1.5/src/spotPython/utils/compare.py
--rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 08:44:33.000000 spotPython-0.1.5/src/spotPython/utils/convert.py
--rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-07 19:27:47.000000 spotPython-0.1.5/src/spotPython/utils/device.py
--rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-09 21:08:48.000000 spotPython-0.1.5/src/spotPython/utils/eda.py
--rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 18:22:38.000000 spotPython-0.1.5/src/spotPython/utils/file.py
--rw-r--r--   0 bartz      (501) staff       (20)     1080 2023-05-20 08:23:54.000000 spotPython-0.1.5/src/spotPython/utils/init.py
--rw-r--r--   0 bartz      (501) staff       (20)     4360 2023-05-20 05:30:54.000000 spotPython-0.1.5/src/spotPython/utils/metrics.py
--rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-13 18:37:01.000000 spotPython-0.1.5/src/spotPython/utils/progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.1.5/src/spotPython/utils/repair.py
--rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-09 23:09:07.000000 spotPython-0.1.5/src/spotPython/utils/transform.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.295692 spotPython-0.1.5/src/spotPython.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     6730 2023-05-20 09:28:18.000000 spotPython-0.1.5/src/spotPython.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     7789 2023-05-20 09:28:18.000000 spotPython-0.1.5/src/spotPython.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-20 09:28:18.000000 spotPython-0.1.5/src/spotPython.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-20 09:28:18.000000 spotPython-0.1.5/src/spotPython.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-20 09:28:18.000000 spotPython-0.1.5/src/spotPython.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-20 09:28:18.302634 spotPython-0.1.5/test/
--rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_aggregate_mean_var.py
--rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.1.5/test/test_build_Psi.py
--rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.1.5/test/test_build_U.py
--rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_build_psi_vec.py
--rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_evaluate_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_evaluate_new_solutions.py
--rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.1.5/test/test_extract_from_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_generate_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_infill.py
--rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_nat_to_cod.py
--rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_nat_to_cod_init.py
--rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_ocba.py
--rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_repair_non_numeric.py
--rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_set_de_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_show_progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_suggest_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.1.5/test/test_update_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.1.5/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.195278 spotPython-0.1.7/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.160964 spotPython-0.1.7/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.165823 spotPython-0.1.7/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.1.7/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)    12811 2023-05-22 11:17:15.000000 spotPython-0.1.7/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 11:16:54.000000 spotPython-0.1.7/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.170830 spotPython-0.1.7/Figures.d/
+-rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-05-03 09:52:04.000000 spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-08 06:28:53.000000 spotPython-0.1.7/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.1.7/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-25 06:56:48.000000 spotPython-0.1.7/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     6730 2023-05-22 11:19:27.195046 spotPython-0.1.7/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     5960 2023-05-20 12:55:59.000000 spotPython-0.1.7/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.171652 spotPython-0.1.7/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)   137970 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/bart23e.html
+-rw-r--r--   0 bartz      (501) staff       (20)   335911 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/bart23e.pdf
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.173053 spotPython-0.1.7/docs/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/figures/parallel.png
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.173235 spotPython-0.1.7/docs/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/img/spotLogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-18 12:00:38.000000 spotPython-0.1.7/docs/index.html
+-rw-r--r--   0 bartz      (501) staff       (20)    48220 2023-05-20 12:55:59.000000 spotPython-0.1.7/docs/search.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.161749 spotPython-0.1.7/docs/site_libs/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.174181 spotPython-0.1.7/docs/site_libs/bootstrap/
+-rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.1.7/docs/site_libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-18 12:00:28.000000 spotPython-0.1.7/docs/site_libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/bootstrap/bootstrap.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.174352 spotPython-0.1.7/docs/site_libs/clipboard/
+-rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/clipboard/clipboard.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.175154 spotPython-0.1.7/docs/site_libs/quarto-html/
+-rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/quarto-html/anchor.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/quarto-html/popper.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-18 11:18:42.000000 spotPython-0.1.7/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/quarto-html/quarto.js
+-rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/quarto-html/tippy.css
+-rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/quarto-html/tippy.umd.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.175300 spotPython-0.1.7/docs/site_libs/quarto-nav/
+-rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/quarto-nav/quarto-nav.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.175763 spotPython-0.1.7/docs/site_libs/quarto-search/
+-rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/quarto-search/autocomplete.umd.js
+-rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/quarto-search/fuse.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.1.7/docs/site_libs/quarto-search/quarto-search.js
+-rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-05-03 09:52:04.000000 spotPython-0.1.7/makeSpot.sh
+-rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.1.7/mkdocs.yml
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.186038 spotPython-0.1.7/notebooks/
+-rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/00_spot_doc.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 06:28:53.000000 spotPython-0.1.7/notebooks/01_spot_intro.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/02_spot_multidim.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 06:28:53.000000 spotPython-0.1.7/notebooks/03_spot_anisotropic.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 06:28:53.000000 spotPython-0.1.7/notebooks/04_spot_sklearn_surrogate.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 06:28:53.000000 spotPython-0.1.7/notebooks/05_spot_sklearn_optimizers.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 06:28:53.000000 spotPython-0.1.7/notebooks/06_spot_gaussian.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 06:28:53.000000 spotPython-0.1.7/notebooks/07_spot_ei.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 06:28:53.000000 spotPython-0.1.7/notebooks/08_spot_noisy.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 06:28:53.000000 spotPython-0.1.7/notebooks/09_spot_ocba.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-22 05:07:39.000000 spotPython-0.1.7/notebooks/10_spot_hpt_sklearn_classification.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    23215 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    28105 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/12_spot_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   604739 2023-05-22 05:07:41.000000 spotPython-0.1.7/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  1309674 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/14_spot_ray_hpt_torch_cifar10_1440.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  1309777 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/14_spot_ray_hpt_torch_cifar10_2880.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/15_spot_hpt_sklearn_regression.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  1040487 2023-05-22 11:17:26.000000 spotPython-0.1.7/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  3243561 2023-05-22 11:17:26.000000 spotPython-0.1.7/notebooks/16_spot_hpt_sklearn_multiclass_classification_1440.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.161970 spotPython-0.1.7/notebooks/data/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.186482 spotPython-0.1.7/notebooks/data/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-15 06:49:11.000000 spotPython-0.1.7/notebooks/data/torch/model_spot_trained.pt
+-rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-22 09:13:51.000000 spotPython-0.1.7/notebooks/data.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.187077 spotPython-0.1.7/notebooks/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.1.7/notebooks/figures/spotModel.graffle
+-rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.1.7/notebooks/figures/spotModel.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.1.7/notebooks/figures/spotModel.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21112 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21979 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23390 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22172 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23463 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24987 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    10009 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7783 2023-05-22 11:16:39.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-20 12:55:59.000000 spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-04-18 07:53:06.000000 spotPython-0.1.7/notebooks/plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-22 11:19:20.000000 spotPython-0.1.7/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-22 11:19:27.195321 spotPython-0.1.7/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.163715 spotPython-0.1.7/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.187246 spotPython-0.1.7/src/spotPython/
+-rw-r--r--   0 bartz      (501) staff       (20)      216 2023-05-22 11:19:26.000000 spotPython-0.1.7/src/spotPython/_version.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.188013 spotPython-0.1.7/src/spotPython/budget/
+-rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-02-02 22:52:12.000000 spotPython-0.1.7/src/spotPython/budget/ocba.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.188309 spotPython-0.1.7/src/spotPython/build/
+-rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-18 07:53:06.000000 spotPython-0.1.7/src/spotPython/build/kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.1.7/src/spotPython/build/surrogates.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.189047 spotPython-0.1.7/src/spotPython/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-25 06:56:48.000000 spotPython-0.1.7/src/spotPython/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-25 06:56:48.000000 spotPython-0.1.7/src/spotPython/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-22 11:17:26.000000 spotPython-0.1.7/src/spotPython/data/sklearn_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-25 06:56:48.000000 spotPython-0.1.7/src/spotPython/data/sklearn_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6154 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/data/torch_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      329 2023-05-03 09:52:04.000000 spotPython-0.1.7/src/spotPython/data/torch_hyper_dict.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.189432 spotPython-0.1.7/src/spotPython/design/
+-rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.1.7/src/spotPython/design/designs.py
+-rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.1.7/src/spotPython/design/factorial.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-25 06:56:48.000000 spotPython-0.1.7/src/spotPython/design/spacefilling.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.189798 spotPython-0.1.7/src/spotPython/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     6273 2023-05-22 11:17:26.000000 spotPython-0.1.7/src/spotPython/fun/hypersklearn.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4769 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/fun/hypertorch.py
+-rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-08 06:28:53.000000 spotPython-0.1.7/src/spotPython/fun/objectivefunctions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.190171 spotPython-0.1.7/src/spotPython/hyperparameters/
+-rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-31 14:57:36.000000 spotPython-0.1.7/src/spotPython/hyperparameters/categorical.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3849 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/hyperparameters/optimizer.py
+-rw-r--r--   0 bartz      (501) staff       (20)    26028 2023-05-08 06:28:53.000000 spotPython-0.1.7/src/spotPython/hyperparameters/values.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.190443 spotPython-0.1.7/src/spotPython/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-02-02 22:52:12.000000 spotPython-0.1.7/src/spotPython/plot/contour.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/plot/validation.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.190592 spotPython-0.1.7/src/spotPython/spot/
+-rw-r--r--   0 bartz      (501) staff       (20)    32443 2023-05-15 06:49:11.000000 spotPython-0.1.7/src/spotPython/spot/spot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.191121 spotPython-0.1.7/src/spotPython/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)     1000 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/torch/netcifar10.py
+-rw-r--r--   0 bartz      (501) staff       (20)      413 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/torch/netcore.py
+-rw-r--r--   0 bartz      (501) staff       (20)      791 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/torch/netfashionMNIST.py
+-rw-r--r--   0 bartz      (501) staff       (20)    16047 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/torch/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.192574 spotPython-0.1.7/src/spotPython/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-11 08:22:02.000000 spotPython-0.1.7/src/spotPython/utils/aggregate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-15 06:49:11.000000 spotPython-0.1.7/src/spotPython/utils/classes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-18 07:53:06.000000 spotPython-0.1.7/src/spotPython/utils/compare.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/utils/convert.py
+-rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-08 06:28:53.000000 spotPython-0.1.7/src/spotPython/utils/device.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-11 13:54:57.000000 spotPython-0.1.7/src/spotPython/utils/eda.py
+-rw-r--r--   0 bartz      (501) staff       (20)      461 2023-05-03 09:52:04.000000 spotPython-0.1.7/src/spotPython/utils/file.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1080 2023-05-20 12:55:59.000000 spotPython-0.1.7/src/spotPython/utils/init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-22 11:17:26.000000 spotPython-0.1.7/src/spotPython/utils/metrics.py
+-rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-18 07:53:06.000000 spotPython-0.1.7/src/spotPython/utils/progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-18 07:53:06.000000 spotPython-0.1.7/src/spotPython/utils/repair.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-11 13:54:57.000000 spotPython-0.1.7/src/spotPython/utils/transform.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.187892 spotPython-0.1.7/src/spotPython.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     6730 2023-05-22 11:19:27.000000 spotPython-0.1.7/src/spotPython.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     8634 2023-05-22 11:19:27.000000 spotPython-0.1.7/src/spotPython.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-22 11:19:27.000000 spotPython-0.1.7/src/spotPython.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-22 11:19:27.000000 spotPython-0.1.7/src/spotPython.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-22 11:19:27.000000 spotPython-0.1.7/src/spotPython.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-22 11:19:27.194631 spotPython-0.1.7/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_aggregate_mean_var.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-11 08:22:02.000000 spotPython-0.1.7/test/test_build_Psi.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-11 08:22:02.000000 spotPython-0.1.7/test/test_build_U.py
+-rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_build_psi_vec.py
+-rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_evaluate_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_evaluate_new_solutions.py
+-rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-11 08:22:02.000000 spotPython-0.1.7/test/test_extract_from_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_generate_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_infill.py
+-rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_nat_to_cod.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_nat_to_cod_init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_ocba.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_repair_non_numeric.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_set_de_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_show_progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_suggest_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.1.7/test/test_update_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-20 12:55:59.000000 spotPython-0.1.7/tox.ini
```

### Comparing `spotPython-0.1.5/.github/workflows/test.yml` & `spotPython-0.1.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/.gitignore` & `spotPython-0.1.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -209,7 +209,12 @@
 docs_old3/site_libs/quarto-html/quarto.js
 docs_old3/site_libs/quarto-html/tippy.css
 docs_old3/site_libs/quarto-html/tippy.umd.min.js
 docs_old3/site_libs/quarto-nav/quarto-nav.js
 docs_old3/site_libs/quarto-search/autocomplete.umd.js
 docs_old3/site_libs/quarto-search/fuse.min.js
 docs_old3/site_libs/quarto-search/quarto-search.js
+notebooks/data/VBDP/sample_submission.csv
+notebooks/data/VBDP/test.csv
+notebooks/data/VBDP/testt.csv
+notebooks/data/VBDP/train.csv
+notebooks/data/VBDP/trainn.csv
```

### Comparing `spotPython-0.1.5/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf` & `spotPython-0.1.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf` & `spotPython-0.1.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf` & `spotPython-0.1.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf` & `spotPython-0.1.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf` & `spotPython-0.1.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf` & `spotPython-0.1.7/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/LICENSE.txt` & `spotPython-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/PKG-INFO` & `spotPython-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.1.5
+Version: 0.1.7
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.1.5/README.md` & `spotPython-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/bart23e.html` & `spotPython-0.1.7/docs/bart23e.html`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/bart23e.pdf` & `spotPython-0.1.7/docs/bart23e.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf` & `spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf` & `spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf` & `spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf` & `spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf` & `spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf` & `spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf` & `spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf` & `spotPython-0.1.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/figures/parallel.png` & `spotPython-0.1.7/docs/figures/parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/img/spotLogo.png` & `spotPython-0.1.7/docs/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/search.json` & `spotPython-0.1.7/docs/search.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/bootstrap/bootstrap-icons.css` & `spotPython-0.1.7/docs/site_libs/bootstrap/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/bootstrap/bootstrap-icons.woff` & `spotPython-0.1.7/docs/site_libs/bootstrap/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/bootstrap/bootstrap.min.css` & `spotPython-0.1.7/docs/site_libs/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/bootstrap/bootstrap.min.js` & `spotPython-0.1.7/docs/site_libs/bootstrap/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/clipboard/clipboard.min.js` & `spotPython-0.1.7/docs/site_libs/clipboard/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-html/anchor.min.js` & `spotPython-0.1.7/docs/site_libs/quarto-html/anchor.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-html/popper.min.js` & `spotPython-0.1.7/docs/site_libs/quarto-html/popper.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-html/quarto-syntax-highlighting.css` & `spotPython-0.1.7/docs/site_libs/quarto-html/quarto-syntax-highlighting.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-html/quarto.js` & `spotPython-0.1.7/docs/site_libs/quarto-html/quarto.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-html/tippy.css` & `spotPython-0.1.7/docs/site_libs/quarto-html/tippy.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-html/tippy.umd.min.js` & `spotPython-0.1.7/docs/site_libs/quarto-html/tippy.umd.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-nav/quarto-nav.js` & `spotPython-0.1.7/docs/site_libs/quarto-nav/quarto-nav.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-search/autocomplete.umd.js` & `spotPython-0.1.7/docs/site_libs/quarto-search/autocomplete.umd.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-search/fuse.min.js` & `spotPython-0.1.7/docs/site_libs/quarto-search/fuse.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/docs/site_libs/quarto-search/quarto-search.js` & `spotPython-0.1.7/docs/site_libs/quarto-search/quarto-search.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/00_spot_doc.ipynb` & `spotPython-0.1.7/notebooks/00_spot_doc.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/01_spot_intro.ipynb` & `spotPython-0.1.7/notebooks/01_spot_intro.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/02_spot_multidim.ipynb` & `spotPython-0.1.7/notebooks/02_spot_multidim.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/03_spot_anisotropic.ipynb` & `spotPython-0.1.7/notebooks/03_spot_anisotropic.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/04_spot_sklearn_surrogate.ipynb` & `spotPython-0.1.7/notebooks/04_spot_sklearn_surrogate.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/05_spot_sklearn_optimizers.ipynb` & `spotPython-0.1.7/notebooks/05_spot_sklearn_optimizers.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/06_spot_gaussian.ipynb` & `spotPython-0.1.7/notebooks/06_spot_gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/07_spot_ei.ipynb` & `spotPython-0.1.7/notebooks/07_spot_ei.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/08_spot_noisy.ipynb` & `spotPython-0.1.7/notebooks/08_spot_noisy.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/09_spot_ocba.ipynb` & `spotPython-0.1.7/notebooks/09_spot_ocba.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/10_spot_hpt_sklearn_classification.ipynb` & `spotPython-0.1.7/notebooks/10_spot_hpt_sklearn_classification.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb` & `spotPython-0.1.7/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/12_spot_hpt_torch_cifar10.ipynb` & `spotPython-0.1.7/notebooks/12_spot_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb` & `spotPython-0.1.7/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/15_spot_hpt_sklearn_regression.ipynb` & `spotPython-0.1.7/notebooks/15_spot_hpt_sklearn_regression.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/data/torch/model_spot_trained.pt` & `spotPython-0.1.7/notebooks/data/torch/model_spot_trained.pt`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures/spotModel.graffle` & `spotPython-0.1.7/notebooks/figures/spotModel.graffle`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures/spotModel.pdf` & `spotPython-0.1.7/notebooks/figures/spotModel.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures/spotModel.png` & `spotPython-0.1.7/notebooks/figures/spotModel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf` & `spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf` & `spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf` & `spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf` & `spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf` & `spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf` & `spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf` & `spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf` & `spotPython-0.1.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/notebooks/plot.png` & `spotPython-0.1.7/notebooks/plot.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/pyproject.toml` & `spotPython-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotPython"
-version = "0.1.5"
+version = "0.1.7"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotPython - Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotPython-0.1.5/src/spotPython/budget/ocba.py` & `spotPython-0.1.7/src/spotPython/budget/ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/build/kriging.py` & `spotPython-0.1.7/src/spotPython/build/kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/data/base.py` & `spotPython-0.1.7/src/spotPython/data/base.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/data/sklearn_hyper_dict.json` & `spotPython-0.1.7/src/spotPython/data/sklearn_hyper_dict.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954545454545454%*

 * *Differences: {"'RandomForestClassifier'": "{'n_estimators': {'upper': 10}, 'min_samples_leaf': {'upper': 25}, "*

 * *                             "'oob_score': OrderedDict([('levels', [0, 1]), ('type', 'factor'), "*

 * *                             "('default', 0), ('transform', 'None'), ('core_model_parameter_type', "*

 * *                             "'bool'), ('lower', 0), ('upper', 1)])}"}*

```diff
@@ -577,15 +577,15 @@
             "upper": 0.01
         },
         "min_samples_leaf": {
             "default": 1,
             "lower": 1,
             "transform": "None",
             "type": "int",
-            "upper": 10
+            "upper": 25
         },
         "min_samples_split": {
             "default": 2,
             "lower": 2,
             "transform": "None",
             "type": "int",
             "upper": 100
@@ -598,15 +598,27 @@
             "upper": 0.01
         },
         "n_estimators": {
             "default": 7,
             "lower": 5,
             "transform": "transform_power_2_int",
             "type": "int",
-            "upper": 9
+            "upper": 10
+        },
+        "oob_score": {
+            "core_model_parameter_type": "bool",
+            "default": 0,
+            "levels": [
+                0,
+                1
+            ],
+            "lower": 0,
+            "transform": "None",
+            "type": "factor",
+            "upper": 1
         }
     },
     "RandomForestRegressor": {
         "bootstrap": {
             "core_model_parameter_type": "bool",
             "default": 1,
             "levels": [
```

### Comparing `spotPython-0.1.5/src/spotPython/data/torch_hyper_dict.json` & `spotPython-0.1.7/src/spotPython/data/torch_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/design/spacefilling.py` & `spotPython-0.1.7/src/spotPython/design/spacefilling.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/fun/hypertorch.py` & `spotPython-0.1.7/src/spotPython/fun/hypertorch.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/fun/objectivefunctions.py` & `spotPython-0.1.7/src/spotPython/fun/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/hyperparameters/categorical.py` & `spotPython-0.1.7/src/spotPython/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/hyperparameters/optimizer.py` & `spotPython-0.1.7/src/spotPython/hyperparameters/optimizer.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/hyperparameters/values.py` & `spotPython-0.1.7/src/spotPython/hyperparameters/values.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/plot/contour.py` & `spotPython-0.1.7/src/spotPython/plot/contour.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/plot/validation.py` & `spotPython-0.1.7/src/spotPython/plot/validation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/spot/spot.py` & `spotPython-0.1.7/src/spotPython/spot/spot.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/torch/netcifar10.py` & `spotPython-0.1.7/src/spotPython/torch/netcifar10.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/torch/netfashionMNIST.py` & `spotPython-0.1.7/src/spotPython/torch/netfashionMNIST.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/torch/traintest.py` & `spotPython-0.1.7/src/spotPython/torch/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/utils/aggregate.py` & `spotPython-0.1.7/src/spotPython/utils/aggregate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/utils/compare.py` & `spotPython-0.1.7/src/spotPython/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/utils/convert.py` & `spotPython-0.1.7/src/spotPython/utils/convert.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/utils/device.py` & `spotPython-0.1.7/src/spotPython/utils/device.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/utils/eda.py` & `spotPython-0.1.7/src/spotPython/utils/eda.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/utils/init.py` & `spotPython-0.1.7/src/spotPython/utils/init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/utils/metrics.py` & `spotPython-0.1.7/src/spotPython/utils/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -110,7 +110,30 @@
             0.4583333333333333
     """
     y_true = series_to_array(y_true)
     sorted_prediction_ids = np.argsort(-y_pred, axis=1)
     top_k_prediction_ids = sorted_prediction_ids[:, :k]
     score = mapk(y_true.reshape(-1, 1), top_k_prediction_ids, k=k)
     return score
+
+
+def mapk_scorer(estimator, X, y):
+    """
+    Scorer for mean average precision at k.
+    This function computes the mean average precision at k between two lists
+    of lists of items.
+    Parameters
+    ----------
+    estimator : sklearn estimator
+                The estimator to be used for prediction.
+    X : array-like of shape (n_samples, n_features)
+        The input samples.
+    y : array-like of shape (n_samples,)
+        The target values.
+    Returns
+    -------
+    score : double
+            The mean average precision at k over the input lists
+    """
+    y_pred = estimator.predict_proba(X)
+    score = mapk_score(y, y_pred, k=3)
+    return score
```

### Comparing `spotPython-0.1.5/src/spotPython/utils/progress.py` & `spotPython-0.1.7/src/spotPython/utils/progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/utils/repair.py` & `spotPython-0.1.7/src/spotPython/utils/repair.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython/utils/transform.py` & `spotPython-0.1.7/src/spotPython/utils/transform.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/src/spotPython.egg-info/PKG-INFO` & `spotPython-0.1.7/src/spotPython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.1.5
+Version: 0.1.7
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.1.5/src/spotPython.egg-info/SOURCES.txt` & `spotPython-0.1.7/src/spotPython.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -84,17 +84,28 @@
 notebooks/08_spot_noisy.ipynb
 notebooks/09_spot_ocba.ipynb
 notebooks/10_spot_hpt_sklearn_classification.ipynb
 notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
 notebooks/12_spot_hpt_torch_cifar10.ipynb
 notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
 notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+notebooks/14_spot_ray_hpt_torch_cifar10_1440.ipynb
+notebooks/14_spot_ray_hpt_torch_cifar10_2880.ipynb
 notebooks/15_spot_hpt_sklearn_regression.ipynb
 notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
+notebooks/16_spot_hpt_sklearn_multiclass_classification_1440.ipynb
 notebooks/data.json
+notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
+notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
+notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
+notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
+notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
+notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
+notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
+notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
```

### Comparing `spotPython-0.1.5/test/test_aggregate_mean_var.py` & `spotPython-0.1.7/test/test_aggregate_mean_var.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_build_Psi.py` & `spotPython-0.1.7/test/test_build_Psi.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_build_U.py` & `spotPython-0.1.7/test/test_build_U.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_build_psi_vec.py` & `spotPython-0.1.7/test/test_build_psi_vec.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_evaluate_new_X.py` & `spotPython-0.1.7/test/test_evaluate_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_evaluate_new_solutions.py` & `spotPython-0.1.7/test/test_evaluate_new_solutions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_extract_from_bounds.py` & `spotPython-0.1.7/test/test_extract_from_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_generate_design.py` & `spotPython-0.1.7/test/test_generate_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_infill.py` & `spotPython-0.1.7/test/test_infill.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_nat_to_cod.py` & `spotPython-0.1.7/test/test_nat_to_cod.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_nat_to_cod_init.py` & `spotPython-0.1.7/test/test_nat_to_cod_init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_ocba.py` & `spotPython-0.1.7/test/test_ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_repair_non_numeric.py` & `spotPython-0.1.7/test/test_repair_non_numeric.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_set_de_bounds.py` & `spotPython-0.1.7/test/test_set_de_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_show_progress.py` & `spotPython-0.1.7/test/test_show_progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_suggest_new_X.py` & `spotPython-0.1.7/test/test_suggest_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.5/test/test_update_surrogate.py` & `spotPython-0.1.7/test/test_update_surrogate.py`

 * *Files identical despite different names*

