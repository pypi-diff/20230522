# Comparing `tmp/kgcnn-3.0.0.tar.gz` & `tmp/kgcnn-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgcnn-3.0.0.tar", last modified: Fri Apr 28 07:25:09 2023, max compression
+gzip compressed data, was "kgcnn-3.0.1.tar", last modified: Mon May 22 14:57:55 2023, max compression
```

## Comparing `kgcnn-3.0.0.tar` & `kgcnn-3.0.1.tar`

### file list

```diff
@@ -1,333 +1,316 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.578677 kgcnn-3.0.0/
--rw-rw-rw-   0        0        0       76 2023-04-28 07:07:15.000000 kgcnn-3.0.0/AUTHORS
--rw-rw-rw-   0        0        0     1066 2023-04-28 07:07:15.000000 kgcnn-3.0.0/LICENSE
--rw-rw-rw-   0        0        0       47 2023-04-28 07:07:15.000000 kgcnn-3.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    19415 2023-04-28 07:25:09.577678 kgcnn-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    18539 2023-04-28 07:07:15.000000 kgcnn-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.497322 kgcnn-3.0.0/kgcnn/
--rw-rw-rw-   0        0        0       43 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.564322 kgcnn-3.0.0/kgcnn/crystal/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/__init__.py
--rw-rw-rw-   0        0        0     2814 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/base.py
--rw-rw-rw-   0        0        0    32196 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/graph_builder.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.577323 kgcnn-3.0.0/kgcnn/crystal/periodic_table/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/periodic_table/__init__.py
--rw-rw-rw-   0        0        0     4029 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/periodic_table/periodic_table.py
--rw-rw-rw-   0        0        0    21221 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/preprocessor.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.658321 kgcnn-3.0.0/kgcnn/data/
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/__init__.py
--rw-rw-rw-   0        0        0    34079 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/base.py
--rw-rw-rw-   0        0        0    12744 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/crystal.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.863324 kgcnn-3.0.0/kgcnn/data/datasets/
--rw-rw-rw-   0        0        0     3036 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/ClinToxDataset.py
--rw-rw-rw-   0        0        0     3186 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/CoraDataset.py
--rw-rw-rw-   0        0        0     4761 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/CoraLuDataset.py
--rw-rw-rw-   0        0        0     1559 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/ESOLDataset.py
--rw-rw-rw-   0        0        0     1727 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/FreeSolvDataset.py
--rw-rw-rw-   0        0        0     5398 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/GraphTUDataset2020.py
--rw-rw-rw-   0        0        0     7113 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/ISO17Dataset.py
--rw-rw-rw-   0        0        0     1471 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/LipopDataset.py
--rw-rw-rw-   0        0        0     8792 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MD17Dataset.py
--rw-rw-rw-   0        0        0     6574 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MD17RevisedDataset.py
--rw-rw-rw-   0        0        0     3158 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MUTAGDataset.py
--rw-rw-rw-   0        0        0    11255 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatBenchDataset2020.py
--rw-rw-rw-   0        0        0     1469 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectDielectricDataset.py
--rw-rw-rw-   0        0        0     1388 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectEFormDataset.py
--rw-rw-rw-   0        0        0     1398 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectGapDataset.py
--rw-rw-rw-   0        0        0     1424 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectIsMetalDataset.py
--rw-rw-rw-   0        0        0     1325 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectJdft2dDataset.py
--rw-rw-rw-   0        0        0     1605 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectLogGVRHDataset.py
--rw-rw-rw-   0        0        0     1604 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectLogKVRHDataset.py
--rw-rw-rw-   0        0        0     1316 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectPerovskitesDataset.py
--rw-rw-rw-   0        0        0     1693 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectPhononsDataset.py
--rw-rw-rw-   0        0        0     8589 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MoleculeNetDataset2018.py
--rw-rw-rw-   0        0        0     4834 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MutagenicityDataset.py
--rw-rw-rw-   0        0        0     3051 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/PROTEINSDataset.py
--rw-rw-rw-   0        0        0     6575 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM7Dataset.py
--rw-rw-rw-   0        0        0     5533 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM7bDataset.py
--rw-rw-rw-   0        0        0     3922 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM8Dataset.py
--rw-rw-rw-   0        0        0    12255 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM9Dataset.py
--rw-rw-rw-   0        0        0     2952 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM9MolNetDataset.py
--rw-rw-rw-   0        0        0     2160 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/SIDERDataset.py
--rw-rw-rw-   0        0        0     2194 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/Tox21MolNetDataset.py
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    12525 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/download.py
--rw-rw-rw-   0        0        0    22993 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/moleculenet.py
--rw-rw-rw-   0        0        0    17786 2023-04-28 07:15:56.000000 kgcnn-3.0.0/kgcnn/data/qm.py
--rw-rw-rw-   0        0        0     2851 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/serial.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.866324 kgcnn-3.0.0/kgcnn/data/transform/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.918321 kgcnn-3.0.0/kgcnn/data/transform/scaler/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/__init__.py
--rw-rw-rw-   0        0        0    19619 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/force.py
--rw-rw-rw-   0        0        0    53863 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/molecule.py
--rw-rw-rw-   0        0        0     1816 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/serial.py
--rw-rw-rw-   0        0        0    27716 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/standard.py
--rw-rw-rw-   0        0        0     9408 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/tudataset.py
--rw-rw-rw-   0        0        0     5311 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.959323 kgcnn-3.0.0/kgcnn/graph/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/__init__.py
--rw-rw-rw-   0        0        0    26596 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.987324 kgcnn-3.0.0/kgcnn/graph/methods/
--rw-rw-rw-   0        0        0     1246 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/methods/__init__.py
--rw-rw-rw-   0        0        0    28421 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/methods/_adj.py
--rw-rw-rw-   0        0        0    23582 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/methods/_geom.py
--rw-rw-rw-   0        0        0     1864 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/postprocessor.py
--rw-rw-rw-   0        0        0    31335 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/preprocessor.py
--rw-rw-rw-   0        0        0     2468 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/serial.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.998321 kgcnn-3.0.0/kgcnn/hyper/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/hyper/__init__.py
--rw-rw-rw-   0        0        0      209 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/hyper/hyper.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.010321 kgcnn-3.0.0/kgcnn/io/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/io/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/io/loader.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.217322 kgcnn-3.0.0/kgcnn/layers/
--rw-rw-rw-   0        0        0     1095 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/README.md
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/__init__.py
--rw-rw-rw-   0        0        0    15544 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/attention.py
--rw-rw-rw-   0        0        0     7693 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/base.py
--rw-rw-rw-   0        0        0    12507 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/casting.py
--rw-rw-rw-   0        0        0    15115 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/conv.py
--rw-rw-rw-   0        0        0    19063 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/gather.py
--rw-rw-rw-   0        0        0    43155 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/geom.py
--rw-rw-rw-   0        0        0     4735 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/message.py
--rw-rw-rw-   0        0        0    18206 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/mlp.py
--rw-rw-rw-   0        0        0    23450 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/modules.py
--rw-rw-rw-   0        0        0    28771 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/norm.py
--rw-rw-rw-   0        0        0    35808 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/pooling.py
--rw-rw-rw-   0        0        0    11853 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/relational.py
--rw-rw-rw-   0        0        0    13549 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/set2set.py
--rw-rw-rw-   0        0        0     8702 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/update.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.219323 kgcnn-3.0.0/kgcnn/literature/
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.279322 kgcnn-3.0.0/kgcnn/literature/AttentiveFP/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/AttentiveFP/__init__.py
--rw-rw-rw-   0        0        0    12186 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/AttentiveFP/_attentivefp_conv.py
--rw-rw-rw-   0        0        0     5902 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/AttentiveFP/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.368674 kgcnn-3.0.0/kgcnn/literature/CGCNN/
--rw-rw-rw-   0        0        0      130 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CGCNN/__init__.py
--rw-rw-rw-   0        0        0     6471 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CGCNN/_cgcnn_conv.py
--rw-rw-rw-   0        0        0     9358 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CGCNN/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.382928 kgcnn-3.0.0/kgcnn/literature/CMPNN/
--rw-rw-rw-   0        0        0       98 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CMPNN/__init__.py
--rw-rw-rw-   0        0        0     8126 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CMPNN/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.407928 kgcnn-3.0.0/kgcnn/literature/DGIN/
--rw-rw-rw-   0        0        0      100 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/DGIN/__init__.py
--rw-rw-rw-   0        0        0     4927 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/DGIN/_dgin_conv.py
--rw-rw-rw-   0        0        0    10250 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/DGIN/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.433548 kgcnn-3.0.0/kgcnn/literature/DMPNN/
--rw-rw-rw-   0        0        0       98 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DMPNN/__init__.py
--rw-rw-rw-   0        0        0     2117 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DMPNN/_dmpnn_conv.py
--rw-rw-rw-   0        0        0     8366 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DMPNN/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.468547 kgcnn-3.0.0/kgcnn/literature/DimeNetPP/
--rw-rw-rw-   0        0        0      215 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DimeNetPP/__init__.py
--rw-rw-rw-   0        0        0    19372 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DimeNetPP/_dimenet_conv.py
--rw-rw-rw-   0        0        0    18270 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DimeNetPP/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.482548 kgcnn-3.0.0/kgcnn/literature/EGNN/
--rw-rw-rw-   0        0        0       98 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/EGNN/__init__.py
--rw-rw-rw-   0        0        0    10063 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/EGNN/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.496548 kgcnn-3.0.0/kgcnn/literature/GAT/
--rw-rw-rw-   0        0        0       98 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GAT/__init__.py
--rw-rw-rw-   0        0        0     5925 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GAT/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.502550 kgcnn-3.0.0/kgcnn/literature/GATv2/
--rw-rw-rw-   0        0        0       98 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GATv2/__init__.py
--rw-rw-rw-   0        0        0     6279 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GATv2/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.536548 kgcnn-3.0.0/kgcnn/literature/GCN/
--rw-rw-rw-   0        0        0      218 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GCN/__init__.py
--rw-rw-rw-   0        0        0     1874 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GCN/_gcn_conv.py
--rw-rw-rw-   0        0        0    10192 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GCN/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.563550 kgcnn-3.0.0/kgcnn/literature/GIN/
--rw-rw-rw-   0        0        0      202 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GIN/__init__.py
--rw-rw-rw-   0        0        0     6634 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GIN/_gin_conv.py
--rw-rw-rw-   0        0        0    10899 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GIN/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.616549 kgcnn-3.0.0/kgcnn/literature/GNNExplain/
--rw-rw-rw-   0        0        0      187 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/__init__.py
--rw-rw-rw-   0        0        0    30109 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_model.py
--rw-rw-rw-   0        0        0     1262 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py
--rw-rw-rw-   0        0        0     1134 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_base.py
--rw-rw-rw-   0        0        0      933 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_testing.py
--rw-rw-rw-   0        0        0      565 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.634551 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_base.py
--rw-rw-rw-   0        0        0     4459 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_testing.py
--rw-rw-rw-   0        0        0      774 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.641550 kgcnn-3.0.0/kgcnn/literature/GNNFilm/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNFilm/__init__.py
--rw-rw-rw-   0        0        0     5606 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNFilm/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.643550 kgcnn-3.0.0/kgcnn/literature/GemNet/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GemNet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.647550 kgcnn-3.0.0/kgcnn/literature/GraphSAGE/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GraphSAGE/__init__.py
--rw-rw-rw-   0        0        0     6836 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GraphSAGE/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.688549 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/
--rw-rw-rw-   0        0        0      454 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/__init__.py
--rw-rw-rw-   0        0        0    25733 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_acsf_conv.py
--rw-rw-rw-   0        0        0    15739 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_make.py
--rw-rw-rw-   0        0        0    21072 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_wacsf_conv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.748549 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/
--rw-rw-rw-   0        0        0      127 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/__init__.py
--rw-rw-rw-   0        0        0    25834 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_hdnnp_conv.py
--rw-rw-rw-   0        0        0     8160 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_make.py
--rw-rw-rw-   0        0        0     9442 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_test_hdnnp.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.777550 kgcnn-3.0.0/kgcnn/literature/HamNet/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/HamNet/__init__.py
--rw-rw-rw-   0        0        0    28565 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/HamNet/_hamnet_conv.py
--rw-rw-rw-   0        0        0     8210 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/HamNet/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.782552 kgcnn-3.0.0/kgcnn/literature/INorp/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/INorp/__init__.py
--rw-rw-rw-   0        0        0     7954 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/INorp/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.809548 kgcnn-3.0.0/kgcnn/literature/MAT/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MAT/__init__.py
--rw-rw-rw-   0        0        0     9724 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MAT/_make.py
--rw-rw-rw-   0        0        0     8758 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MAT/_mat_conv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.836547 kgcnn-3.0.0/kgcnn/literature/MEGAN/
--rw-rw-rw-   0        0        0      218 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MEGAN/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MEGAN/_make.py
--rw-rw-rw-   0        0        0    22759 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MEGAN/_model.py
--rw-rw-rw-   0        0        0     6903 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MEGAN/_test_literature_megan.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.863565 kgcnn-3.0.0/kgcnn/literature/MXMNet/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MXMNet/__init__.py
--rw-rw-rw-   0        0        0    10142 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MXMNet/_make.py
--rw-rw-rw-   0        0        0     8490 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MXMNet/_mxmnet_conv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.882571 kgcnn-3.0.0/kgcnn/literature/Megnet/
--rw-rw-rw-   0        0        0      215 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Megnet/__init__.py
--rw-rw-rw-   0        0        0    18509 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Megnet/_make.py
--rw-rw-rw-   0        0        0     7153 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Megnet/_megnet_conv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.901567 kgcnn-3.0.0/kgcnn/literature/MoGAT/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MoGAT/__init__.py
--rw-rw-rw-   0        0        0     6679 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MoGAT/_make.py
--rw-rw-rw-   0        0        0    12206 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MoGAT/_mogat_conv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.921568 kgcnn-3.0.0/kgcnn/literature/NMPN/
--rw-rw-rw-   0        0        0      215 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/NMPN/__init__.py
--rw-rw-rw-   0        0        0    17202 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/NMPN/_make.py
--rw-rw-rw-   0        0        0     4753 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/NMPN/_mpnn_conv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.947566 kgcnn-3.0.0/kgcnn/literature/PAiNN/
--rw-rw-rw-   0        0        0      215 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/PAiNN/__init__.py
--rw-rw-rw-   0        0        0    14386 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/PAiNN/_make.py
--rw-rw-rw-   0        0        0    15451 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/PAiNN/_painn_conv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.952567 kgcnn-3.0.0/kgcnn/literature/RGCN/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/RGCN/__init__.py
--rw-rw-rw-   0        0        0     5668 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/RGCN/_make.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.978566 kgcnn-3.0.0/kgcnn/literature/Schnet/
--rw-rw-rw-   0        0        0      215 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Schnet/__init__.py
--rw-rw-rw-   0        0        0    14260 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Schnet/_make.py
--rw-rw-rw-   0        0        0     8445 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Schnet/_schnet_conv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.019565 kgcnn-3.0.0/kgcnn/literature/Unet/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/__init__.py
--rw-rw-rw-   0        0        0     7194 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/_make.py
--rw-rw-rw-   0        0        0     1138 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/_test_connect.py
--rw-rw-rw-   0        0        0     4157 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/_test_topk.py
--rw-rw-rw-   0        0        0    19977 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/_topk.py
--rw-rw-rw-   0        0        0       51 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.074566 kgcnn-3.0.0/kgcnn/literature/coGN/
--rw-rw-rw-   0        0        0     2872 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/coGN/__init__.py
--rw-rw-rw-   0        0        0     7416 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_coGN_config.py
--rw-rw-rw-   0        0        0     6429 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_coNGN_config.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.099565 kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/__init__.py
--rw-rw-rw-   0        0        0     4218 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py
--rw-rw-rw-   0        0        0     6719 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py
--rw-rw-rw-   0        0        0      891 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_gates.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.125875 kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/__init__.py
--rw-rw-rw-   0        0        0    16183 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/graph_network_base.py
--rw-rw-rw-   0        0        0    23817 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/graph_networks.py
--rw-rw-rw-   0        0        0    27686 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_make.py
--rw-rw-rw-   0        0        0     2266 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_multiplicity_readout.py
--rw-rw-rw-   0        0        0     3945 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_preprocessing_layers.py
--rw-rw-rw-   0        0        0      372 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.149593 kgcnn-3.0.0/kgcnn/literature/rGIN/
--rw-rw-rw-   0        0        0       99 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/rGIN/__init__.py
--rw-rw-rw-   0        0        0     5438 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/rGIN/_make.py
--rw-rw-rw-   0        0        0     3500 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/rGIN/_rgin_conv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.164678 kgcnn-3.0.0/kgcnn/metrics/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/metrics/__init__.py
--rw-rw-rw-   0        0        0      972 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/metrics/loss.py
--rw-rw-rw-   0        0        0    10804 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.191679 kgcnn-3.0.0/kgcnn/model/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/README.md
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/__init__.py
--rw-rw-rw-   0        0        0     8946 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/force.py
--rw-rw-rw-   0        0        0       18 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/serial.py
--rw-rw-rw-   0        0        0     5430 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.255679 kgcnn-3.0.0/kgcnn/mol/
--rw-rw-rw-   0        0        0      165 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/__init__.py
--rw-rw-rw-   0        0        0       33 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/base.py
--rw-rw-rw-   0        0        0       36 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/convert.py
--rw-rw-rw-   0        0        0       36 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/encoder.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.260679 kgcnn-3.0.0/kgcnn/mol/external/
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/external/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/external/ballloon.py
--rw-rw-rw-   0        0        0       40 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/graph_babel.py
--rw-rw-rw-   0        0        0       40 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/graph_rdkit.py
--rw-rw-rw-   0        0        0       31 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/io.py
--rw-rw-rw-   0        0        0       36 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/methods.py
--rw-rw-rw-   0        0        0       35 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/serial.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.282677 kgcnn-3.0.0/kgcnn/moldyn/
--rw-rw-rw-   0        0        0      177 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/moldyn/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/moldyn/ase_calc.py
--rw-rw-rw-   0        0        0       42 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/moldyn/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.358677 kgcnn-3.0.0/kgcnn/molecule/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/__init__.py
--rw-rw-rw-   0        0        0    10057 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/base.py
--rw-rw-rw-   0        0        0    12161 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/convert.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.373677 kgcnn-3.0.0/kgcnn/molecule/dynamics/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/dynamics/__init__.py
--rw-rw-rw-   0        0        0     3911 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/dynamics/ase_calc.py
--rw-rw-rw-   0        0        0     8386 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/dynamics/base.py
--rw-rw-rw-   0        0        0     2556 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/encoder.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.399676 kgcnn-3.0.0/kgcnn/molecule/external/
--rw-rw-rw-   0        0        0      159 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/external/__init__.py
--rw-rw-rw-   0        0        0    20790 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/external/ballloon.py
--rw-rw-rw-   0        0        0    17892 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/graph_babel.py
--rw-rw-rw-   0        0        0    20750 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/graph_rdkit.py
--rw-rw-rw-   0        0        0     8960 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/io.py
--rw-rw-rw-   0        0        0     5105 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/methods.py
--rw-rw-rw-   0        0        0      702 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/serial.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.452678 kgcnn-3.0.0/kgcnn/ops/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/__init__.py
--rw-rw-rw-   0        0        0     3853 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/activ.py
--rw-rw-rw-   0        0        0     1483 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/axis.py
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/casting.py
--rw-rw-rw-   0        0        0     6991 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/initializer.py
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/numpy.py
--rw-rw-rw-   0        0        0     8292 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/partition.py
--rw-rw-rw-   0        0        0    10223 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/polynom.py
--rw-rw-rw-   0        0        0     3181 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/ragged.py
--rw-rw-rw-   0        0        0     1148 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/scatter.py
--rw-rw-rw-   0        0        0     2046 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/segment.py
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/sorting.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.497678 kgcnn-3.0.0/kgcnn/training/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/__init__.py
--rw-rw-rw-   0        0        0     1220 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/callbacks.py
--rw-rw-rw-   0        0        0     4643 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/history.py
--rw-rw-rw-   0        0        0    14935 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/hyper.py
--rw-rw-rw-   0        0        0     8691 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/optimizer.py
--rw-rw-rw-   0        0        0     2656 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/schedule.py
--rw-rw-rw-   0        0        0    16405 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.506678 kgcnn-3.0.0/kgcnn/utils/
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/utils/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/utils/devices.py
--rw-rw-rw-   0        0        0     7356 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/utils/plots.py
--rw-rw-rw-   0        0        0     2307 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/utils/serial.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.526324 kgcnn-3.0.0/kgcnn.egg-info/
--rw-rw-rw-   0        0        0    19415 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8562 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      313 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 07:25:09.579678 kgcnn-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1855 2023-04-28 07:07:15.000000 kgcnn-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.576678 kgcnn-3.0.0/test/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/__init__.py
--rw-rw-rw-   0        0        0     4986 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_data_base.py
--rw-rw-rw-   0        0        0     7931 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_data_moleculenet.py
--rw-rw-rw-   0        0        0     1255 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_graph_base.py
--rw-rw-rw-   0        0        0     4149 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_graph_methods.py
--rw-rw-rw-   0        0        0     5135 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_layers_attention.py
--rw-rw-rw-   0        0        0     4211 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_layers_gather.py
--rw-rw-rw-   0        0        0     7647 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_layers_geom.py
--rw-rw-rw-   0        0        0     2338 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_layers_pooling.py
--rw-rw-rw-   0        0        0     8078 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_range_periodic.py
--rw-rw-rw-   0        0        0      118 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.144680 kgcnn-3.0.1/
+-rw-rw-rw-   0        0        0       76 2023-05-22 05:04:06.000000 kgcnn-3.0.1/AUTHORS
+-rw-rw-rw-   0        0        0     1066 2023-05-22 05:04:06.000000 kgcnn-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-05-22 05:04:06.000000 kgcnn-3.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    19415 2023-05-22 14:57:55.143679 kgcnn-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    18539 2023-05-22 05:04:06.000000 kgcnn-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.458469 kgcnn-3.0.1/kgcnn/
+-rw-rw-rw-   0        0        0       43 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.533255 kgcnn-3.0.1/kgcnn/crystal/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/__init__.py
+-rw-rw-rw-   0        0        0     2902 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/base.py
+-rw-rw-rw-   0        0        0    31910 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/graph_builder.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.544611 kgcnn-3.0.1/kgcnn/crystal/periodic_table/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/periodic_table/__init__.py
+-rw-rw-rw-   0        0        0    15016 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/periodic_table/periodic_table.csv
+-rw-rw-rw-   0        0        0     4029 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/periodic_table/periodic_table.py
+-rw-rw-rw-   0        0        0    21221 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/preprocessor.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.626678 kgcnn-3.0.1/kgcnn/data/
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/__init__.py
+-rw-rw-rw-   0        0        0    35033 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/base.py
+-rw-rw-rw-   0        0        0    12885 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/crystal.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.838682 kgcnn-3.0.1/kgcnn/data/datasets/
+-rw-rw-rw-   0        0        0     3036 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/ClinToxDataset.py
+-rw-rw-rw-   0        0        0     3186 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/CoraDataset.py
+-rw-rw-rw-   0        0        0     4761 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/CoraLuDataset.py
+-rw-rw-rw-   0        0        0     1559 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/ESOLDataset.py
+-rw-rw-rw-   0        0        0     1727 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/FreeSolvDataset.py
+-rw-rw-rw-   0        0        0     5398 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/GraphTUDataset2020.py
+-rw-rw-rw-   0        0        0     7113 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/ISO17Dataset.py
+-rw-rw-rw-   0        0        0     1471 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/LipopDataset.py
+-rw-rw-rw-   0        0        0     8792 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MD17Dataset.py
+-rw-rw-rw-   0        0        0     6574 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MD17RevisedDataset.py
+-rw-rw-rw-   0        0        0     3158 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MUTAGDataset.py
+-rw-rw-rw-   0        0        0    11255 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatBenchDataset2020.py
+-rw-rw-rw-   0        0        0     1469 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectDielectricDataset.py
+-rw-rw-rw-   0        0        0     1388 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectEFormDataset.py
+-rw-rw-rw-   0        0        0     1398 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectGapDataset.py
+-rw-rw-rw-   0        0        0     1424 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectIsMetalDataset.py
+-rw-rw-rw-   0        0        0     1325 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectJdft2dDataset.py
+-rw-rw-rw-   0        0        0     1605 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectLogGVRHDataset.py
+-rw-rw-rw-   0        0        0     1604 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectLogKVRHDataset.py
+-rw-rw-rw-   0        0        0     1316 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectPerovskitesDataset.py
+-rw-rw-rw-   0        0        0     1693 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectPhononsDataset.py
+-rw-rw-rw-   0        0        0     8589 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MoleculeNetDataset2018.py
+-rw-rw-rw-   0        0        0     4834 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MutagenicityDataset.py
+-rw-rw-rw-   0        0        0     3051 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/PROTEINSDataset.py
+-rw-rw-rw-   0        0        0     6575 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM7Dataset.py
+-rw-rw-rw-   0        0        0     5533 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM7bDataset.py
+-rw-rw-rw-   0        0        0     3922 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM8Dataset.py
+-rw-rw-rw-   0        0        0    12255 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM9Dataset.py
+-rw-rw-rw-   0        0        0     2952 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM9MolNetDataset.py
+-rw-rw-rw-   0        0        0     2160 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/SIDERDataset.py
+-rw-rw-rw-   0        0        0     2194 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/Tox21MolNetDataset.py
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0    12525 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/download.py
+-rw-rw-rw-   0        0        0    22994 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/moleculenet.py
+-rw-rw-rw-   0        0        0    17817 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/qm.py
+-rw-rw-rw-   0        0        0     2851 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/serial.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.840683 kgcnn-3.0.1/kgcnn/data/transform/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/base.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.880678 kgcnn-3.0.1/kgcnn/data/transform/scaler/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/__init__.py
+-rw-rw-rw-   0        0        0    19619 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/force.py
+-rw-rw-rw-   0        0        0    53863 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/molecule.py
+-rw-rw-rw-   0        0        0     1865 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/serial.py
+-rw-rw-rw-   0        0        0    28142 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/standard.py
+-rw-rw-rw-   0        0        0     9408 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/tudataset.py
+-rw-rw-rw-   0        0        0     5311 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.913678 kgcnn-3.0.1/kgcnn/graph/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/__init__.py
+-rw-rw-rw-   0        0        0    26883 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/base.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.940681 kgcnn-3.0.1/kgcnn/graph/methods/
+-rw-rw-rw-   0        0        0     1316 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/methods/__init__.py
+-rw-rw-rw-   0        0        0    28421 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/methods/_adj.py
+-rw-rw-rw-   0        0        0    23582 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/methods/_geom.py
+-rw-rw-rw-   0        0        0     1864 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/postprocessor.py
+-rw-rw-rw-   0        0        0    31335 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/preprocessor.py
+-rw-rw-rw-   0        0        0     2468 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/serial.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.946680 kgcnn-3.0.1/kgcnn/io/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/io/__init__.py
+-rw-rw-rw-   0        0        0     8125 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/io/file.py
+-rw-rw-rw-   0        0        0     4556 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/io/loader.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.085678 kgcnn-3.0.1/kgcnn/layers/
+-rw-rw-rw-   0        0        0     1095 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/README.md
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/__init__.py
+-rw-rw-rw-   0        0        0    15544 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/attention.py
+-rw-rw-rw-   0        0        0     7693 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/base.py
+-rw-rw-rw-   0        0        0    12507 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/casting.py
+-rw-rw-rw-   0        0        0    15178 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/conv.py
+-rw-rw-rw-   0        0        0    17112 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/gather.py
+-rw-rw-rw-   0        0        0    43155 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/geom.py
+-rw-rw-rw-   0        0        0     4735 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/message.py
+-rw-rw-rw-   0        0        0    18206 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/mlp.py
+-rw-rw-rw-   0        0        0    23450 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/modules.py
+-rw-rw-rw-   0        0        0    28771 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/norm.py
+-rw-rw-rw-   0        0        0    35808 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/pooling.py
+-rw-rw-rw-   0        0        0    11853 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/relational.py
+-rw-rw-rw-   0        0        0    13549 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/set2set.py
+-rw-rw-rw-   0        0        0     8702 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/update.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.087682 kgcnn-3.0.1/kgcnn/literature/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.107678 kgcnn-3.0.1/kgcnn/literature/AttentiveFP/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/AttentiveFP/__init__.py
+-rw-rw-rw-   0        0        0    12186 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/AttentiveFP/_attentivefp_conv.py
+-rw-rw-rw-   0        0        0     5902 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/AttentiveFP/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.128678 kgcnn-3.0.1/kgcnn/literature/CGCNN/
+-rw-rw-rw-   0        0        0      130 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CGCNN/__init__.py
+-rw-rw-rw-   0        0        0     6471 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CGCNN/_cgcnn_conv.py
+-rw-rw-rw-   0        0        0     9358 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CGCNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.139678 kgcnn-3.0.1/kgcnn/literature/CMPNN/
+-rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CMPNN/__init__.py
+-rw-rw-rw-   0        0        0     8126 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CMPNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.169678 kgcnn-3.0.1/kgcnn/literature/DGIN/
+-rw-rw-rw-   0        0        0      100 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DGIN/__init__.py
+-rw-rw-rw-   0        0        0     4927 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DGIN/_dgin_conv.py
+-rw-rw-rw-   0        0        0    10250 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DGIN/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.189678 kgcnn-3.0.1/kgcnn/literature/DMPNN/
+-rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DMPNN/__init__.py
+-rw-rw-rw-   0        0        0     2117 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DMPNN/_dmpnn_conv.py
+-rw-rw-rw-   0        0        0     8366 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DMPNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.210678 kgcnn-3.0.1/kgcnn/literature/DimeNetPP/
+-rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DimeNetPP/__init__.py
+-rw-rw-rw-   0        0        0    19372 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DimeNetPP/_dimenet_conv.py
+-rw-rw-rw-   0        0        0    18270 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DimeNetPP/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.222678 kgcnn-3.0.1/kgcnn/literature/EGNN/
+-rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/EGNN/__init__.py
+-rw-rw-rw-   0        0        0    10063 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/EGNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.226680 kgcnn-3.0.1/kgcnn/literature/GAT/
+-rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GAT/__init__.py
+-rw-rw-rw-   0        0        0     5925 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GAT/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.239678 kgcnn-3.0.1/kgcnn/literature/GATv2/
+-rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GATv2/__init__.py
+-rw-rw-rw-   0        0        0     6279 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GATv2/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.270678 kgcnn-3.0.1/kgcnn/literature/GCN/
+-rw-rw-rw-   0        0        0      218 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GCN/__init__.py
+-rw-rw-rw-   0        0        0     1874 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GCN/_gcn_conv.py
+-rw-rw-rw-   0        0        0    10192 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GCN/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.289678 kgcnn-3.0.1/kgcnn/literature/GIN/
+-rw-rw-rw-   0        0        0      202 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GIN/__init__.py
+-rw-rw-rw-   0        0        0     6634 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GIN/_gin_conv.py
+-rw-rw-rw-   0        0        0    10899 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GIN/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.335678 kgcnn-3.0.1/kgcnn/literature/GNNExplain/
+-rw-rw-rw-   0        0        0      187 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/__init__.py
+-rw-rw-rw-   0        0        0    30109 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_model.py
+-rw-rw-rw-   0        0        0     1262 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py
+-rw-rw-rw-   0        0        0     1134 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_base.py
+-rw-rw-rw-   0        0        0      933 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_testing.py
+-rw-rw-rw-   0        0        0      565 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.360678 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_base.py
+-rw-rw-rw-   0        0        0     4459 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_testing.py
+-rw-rw-rw-   0        0        0      774 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.365680 kgcnn-3.0.1/kgcnn/literature/GNNFilm/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNFilm/__init__.py
+-rw-rw-rw-   0        0        0     5606 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNFilm/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.367679 kgcnn-3.0.1/kgcnn/literature/GemNet/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GemNet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.371679 kgcnn-3.0.1/kgcnn/literature/GraphSAGE/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GraphSAGE/__init__.py
+-rw-rw-rw-   0        0        0     6836 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GraphSAGE/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.407678 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/
+-rw-rw-rw-   0        0        0      454 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/__init__.py
+-rw-rw-rw-   0        0        0    25733 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_acsf_conv.py
+-rw-rw-rw-   0        0        0    15739 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_make.py
+-rw-rw-rw-   0        0        0    21072 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_wacsf_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.442679 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/
+-rw-rw-rw-   0        0        0      127 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/__init__.py
+-rw-rw-rw-   0        0        0    25834 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_hdnnp_conv.py
+-rw-rw-rw-   0        0        0     8160 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_make.py
+-rw-rw-rw-   0        0        0     9442 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_test_hdnnp.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.467681 kgcnn-3.0.1/kgcnn/literature/HamNet/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HamNet/__init__.py
+-rw-rw-rw-   0        0        0    28565 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HamNet/_hamnet_conv.py
+-rw-rw-rw-   0        0        0     8210 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HamNet/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.472680 kgcnn-3.0.1/kgcnn/literature/INorp/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/INorp/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/INorp/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.491678 kgcnn-3.0.1/kgcnn/literature/MAT/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MAT/__init__.py
+-rw-rw-rw-   0        0        0     9724 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MAT/_make.py
+-rw-rw-rw-   0        0        0     8758 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MAT/_mat_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.530681 kgcnn-3.0.1/kgcnn/literature/MEGAN/
+-rw-rw-rw-   0        0        0      218 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MEGAN/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MEGAN/_make.py
+-rw-rw-rw-   0        0        0    22759 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MEGAN/_model.py
+-rw-rw-rw-   0        0        0     6903 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MEGAN/_test_literature_megan.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.550680 kgcnn-3.0.1/kgcnn/literature/MXMNet/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MXMNet/__init__.py
+-rw-rw-rw-   0        0        0    10142 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MXMNet/_make.py
+-rw-rw-rw-   0        0        0     8490 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MXMNet/_mxmnet_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.571678 kgcnn-3.0.1/kgcnn/literature/Megnet/
+-rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Megnet/__init__.py
+-rw-rw-rw-   0        0        0    18509 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Megnet/_make.py
+-rw-rw-rw-   0        0        0     7153 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Megnet/_megnet_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.594678 kgcnn-3.0.1/kgcnn/literature/MoGAT/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MoGAT/__init__.py
+-rw-rw-rw-   0        0        0     6679 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MoGAT/_make.py
+-rw-rw-rw-   0        0        0    12206 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MoGAT/_mogat_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.616681 kgcnn-3.0.1/kgcnn/literature/NMPN/
+-rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/NMPN/__init__.py
+-rw-rw-rw-   0        0        0    17202 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/NMPN/_make.py
+-rw-rw-rw-   0        0        0     4753 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/NMPN/_mpnn_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.647678 kgcnn-3.0.1/kgcnn/literature/PAiNN/
+-rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/PAiNN/__init__.py
+-rw-rw-rw-   0        0        0    14386 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/PAiNN/_make.py
+-rw-rw-rw-   0        0        0    15451 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/PAiNN/_painn_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.652681 kgcnn-3.0.1/kgcnn/literature/RGCN/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/RGCN/__init__.py
+-rw-rw-rw-   0        0        0     5668 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/RGCN/_make.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.672679 kgcnn-3.0.1/kgcnn/literature/Schnet/
+-rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Schnet/__init__.py
+-rw-rw-rw-   0        0        0    14260 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Schnet/_make.py
+-rw-rw-rw-   0        0        0     8445 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Schnet/_schnet_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.710678 kgcnn-3.0.1/kgcnn/literature/Unet/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/__init__.py
+-rw-rw-rw-   0        0        0     7194 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/_make.py
+-rw-rw-rw-   0        0        0     1138 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/_test_connect.py
+-rw-rw-rw-   0        0        0     4157 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/_test_topk.py
+-rw-rw-rw-   0        0        0    19977 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/_topk.py
+-rw-rw-rw-   0        0        0       51 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.776680 kgcnn-3.0.1/kgcnn/literature/coGN/
+-rw-rw-rw-   0        0        0     2873 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/__init__.py
+-rw-rw-rw-   0        0        0     7496 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_coGN_config.py
+-rw-rw-rw-   0        0        0     6429 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_coNGN_config.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.794678 kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/__init__.py
+-rw-rw-rw-   0        0        0     4218 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py
+-rw-rw-rw-   0        0        0     6719 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py
+-rw-rw-rw-   0        0        0      891 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_gates.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.815680 kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/__init__.py
+-rw-rw-rw-   0        0        0    16183 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/graph_network_base.py
+-rw-rw-rw-   0        0        0    23941 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/graph_networks.py
+-rw-rw-rw-   0        0        0    27901 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_make.py
+-rw-rw-rw-   0        0        0     2266 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_multiplicity_readout.py
+-rw-rw-rw-   0        0        0     3945 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_preprocessing_layers.py
+-rw-rw-rw-   0        0        0     1051 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_test.py
+-rw-rw-rw-   0        0        0      372 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.826680 kgcnn-3.0.1/kgcnn/literature/rGIN/
+-rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/rGIN/__init__.py
+-rw-rw-rw-   0        0        0     5444 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/rGIN/_make.py
+-rw-rw-rw-   0        0        0     3502 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/rGIN/_rgin_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.843679 kgcnn-3.0.1/kgcnn/metrics/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/metrics/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/metrics/loss.py
+-rw-rw-rw-   0        0        0    10804 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.865680 kgcnn-3.0.1/kgcnn/model/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/README.md
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/__init__.py
+-rw-rw-rw-   0        0        0     8946 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/force.py
+-rw-rw-rw-   0        0        0       18 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/serial.py
+-rw-rw-rw-   0        0        0     5430 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.931681 kgcnn-3.0.1/kgcnn/molecule/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/__init__.py
+-rw-rw-rw-   0        0        0    10057 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/base.py
+-rw-rw-rw-   0        0        0    12505 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/convert.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.944678 kgcnn-3.0.1/kgcnn/molecule/dynamics/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/dynamics/__init__.py
+-rw-rw-rw-   0        0        0     3911 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/dynamics/ase_calc.py
+-rw-rw-rw-   0        0        0     8386 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/dynamics/base.py
+-rw-rw-rw-   0        0        0     2556 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.960678 kgcnn-3.0.1/kgcnn/molecule/external/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/external/__init__.py
+-rw-rw-rw-   0        0        0    20790 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/external/ballloon.py
+-rw-rw-rw-   0        0        0    17892 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/graph_babel.py
+-rw-rw-rw-   0        0        0    20750 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/graph_rdkit.py
+-rw-rw-rw-   0        0        0     9149 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/io.py
+-rw-rw-rw-   0        0        0     5105 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/methods.py
+-rw-rw-rw-   0        0        0      702 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/serial.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.012679 kgcnn-3.0.1/kgcnn/ops/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/__init__.py
+-rw-rw-rw-   0        0        0     3853 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/activ.py
+-rw-rw-rw-   0        0        0     1483 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/axis.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/casting.py
+-rw-rw-rw-   0        0        0     6991 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/initializer.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/numpy.py
+-rw-rw-rw-   0        0        0     8292 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/partition.py
+-rw-rw-rw-   0        0        0    10223 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/polynom.py
+-rw-rw-rw-   0        0        0     3181 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/ragged.py
+-rw-rw-rw-   0        0        0     1148 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/scatter.py
+-rw-rw-rw-   0        0        0     2046 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/segment.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/sorting.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.055678 kgcnn-3.0.1/kgcnn/training/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/__init__.py
+-rw-rw-rw-   0        0        0     1220 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/callbacks.py
+-rw-rw-rw-   0        0        0     4643 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/history.py
+-rw-rw-rw-   0        0        0    14935 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/hyper.py
+-rw-rw-rw-   0        0        0     8691 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/optimizer.py
+-rw-rw-rw-   0        0        0     3945 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/schedule.py
+-rw-rw-rw-   0        0        0    16405 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.076678 kgcnn-3.0.1/kgcnn/utils/
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/utils/__init__.py
+-rw-rw-rw-   0        0        0     2249 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/utils/devices.py
+-rw-rw-rw-   0        0        0     7356 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/utils/plots.py
+-rw-rw-rw-   0        0        0     2310 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/utils/serial.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.503404 kgcnn-3.0.1/kgcnn.egg-info/
+-rw-rw-rw-   0        0        0    19415 2023-05-22 14:57:52.000000 kgcnn-3.0.1/kgcnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2023-05-22 14:57:53.000000 kgcnn-3.0.1/kgcnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:57:52.000000 kgcnn-3.0.1/kgcnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      318 2023-05-22 14:57:52.000000 kgcnn-3.0.1/kgcnn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 14:57:53.000000 kgcnn-3.0.1/kgcnn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 14:57:55.144680 kgcnn-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1880 2023-05-22 05:04:06.000000 kgcnn-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.141679 kgcnn-3.0.1/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/__init__.py
+-rw-rw-rw-   0        0        0     4986 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_data_base.py
+-rw-rw-rw-   0        0        0     7931 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_data_moleculenet.py
+-rw-rw-rw-   0        0        0     1255 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_graph_base.py
+-rw-rw-rw-   0        0        0     4149 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_graph_methods.py
+-rw-rw-rw-   0        0        0     5135 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_layers_attention.py
+-rw-rw-rw-   0        0        0     4211 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_layers_gather.py
+-rw-rw-rw-   0        0        0     7647 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_layers_geom.py
+-rw-rw-rw-   0        0        0     2338 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_layers_pooling.py
+-rw-rw-rw-   0        0        0     8078 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_range_periodic.py
+-rw-rw-rw-   0        0        0      118 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/utils.py
```

### Comparing `kgcnn-3.0.0/LICENSE` & `kgcnn-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/PKG-INFO` & `kgcnn-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgcnn
-Version: 3.0.0
+Version: 3.0.1
 Summary: General Base Layers for Graph Convolutions with tensorflow.keras
 Home-page: https://github.com/aimat-lab/gcnn_keras
 Author: Patrick Reiser
 Author-email: patrick.reiser@kit.edu
 License: UNKNOWN
 Keywords: materials,science,machine,learning,deep,graph,networks,neural
 Platform: UNKNOWN
```

### Comparing `kgcnn-3.0.0/README.md` & `kgcnn-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/crystal/base.py` & `kgcnn-3.0.1/kgcnn/crystal/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from hashlib import md5
 # import logging
 from pymatgen.core.structure import Structure
 from typing import Callable, Union
 from networkx import MultiDiGraph
 from kgcnn.graph.base import GraphDict
 
+# A separate module logger is not need for the base class.
 # logging.basicConfig()  # Module logger
 # module_logger = logging.getLogger(__name__)
 # module_logger.setLevel(logging.INFO)
 
 
 class CrystalPreprocessor(Callable[[Structure], MultiDiGraph]):
     """Base class for crystal preprocessors.
@@ -31,15 +32,15 @@
 
         Raises:
             NotImplementedError:Should be implemented in a subclass.
 
         Returns:
             MultiDiGraph: Graph representation of the crystal.
         """
-        raise NotImplementedError("Must be implemented in sub-class.")
+        raise NotImplementedError("Must be implemented in sub-classes.")
 
     def __call__(self, structure: Structure) -> Union[MultiDiGraph, GraphDict]:
         """Should be implemented in a subclass.
 
         Args:
             structure (Structure): Crystal for which the graph representation should be calculated.
 
@@ -50,15 +51,15 @@
             MultiDiGraph: Graph representation of the crystal.
         """
         if self.output_graph_as_dict:
             nxg = self.call(structure)
             g = GraphDict()
             g.from_networkx(
                 nxg, node_attributes=self.node_attributes, edge_attributes=self.edge_attributes,
-                graph_attributes=self.graph_attributes)
+                graph_attributes=self.graph_attributes, reverse_edge_indices=True)
             return g
         return self.call(structure)
 
     def get_config(self) -> dict:
         """Returns a dictionary uniquely identifying the CrystalPreprocessor and its configuration.
 
         Returns:
```

### Comparing `kgcnn-3.0.0/kgcnn/crystal/graph_builder.py` & `kgcnn-3.0.1/kgcnn/crystal/graph_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,23 +131,27 @@
         inplace (bool, optional): Whether to add the edges to the given graph or create a copy with added edges.
             Defaults to False.
 
     Returns:
         MultiDiGraph: Graph with added edges.
     """
     lattice = _get_attr_from_graph(graph, "lattice_matrix", make_copy=True)
+    # if max_radius is None:
+    #     max_radius = _estimate_radius_from_density(lattice)
     frac_coords = np.array([data[1] for data in graph.nodes(data='frac_coords')])
     coords = frac_coords @ lattice
     # return coords, lattice
-    index1, index2, offset_vectors, distances = find_points_in_spheres(coords,
-                                                                       coords,
-                                                                       r=max_radius,
-                                                                       pbc=np.array([True] * 3, dtype=int),
-                                                                       lattice=lattice,
-                                                                       tol=1e-8)
+    index1, index2, offset_vectors, distances = find_points_in_spheres(
+        coords,
+        coords,
+        r=max_radius,
+        pbc=np.array([True] * 3, dtype=int),
+        lattice=lattice,
+        tol=1e-8
+    )
     offset_vectors = offset_vectors.astype('i2')
     # Remove self_loops:
     no_self_loops = np.argwhere(~np.isclose(distances, 0)).reshape(-1)
     index1 = index1[no_self_loops]
     index2 = index2[no_self_loops]
     offset_vectors = offset_vectors[no_self_loops]
     distances = distances[no_self_loops]
@@ -229,15 +233,15 @@
     new_graph = graph if inplace else deepcopy(graph)
 
     lattice = _get_attr_from_graph(graph, "lattice_matrix")
     frac_coords = np.array([data[1] for data in graph.nodes(data='frac_coords')])
     dim = lattice.shape[0]
     assert dim == 3
     size = np.array([1, 1, 1])
-    expanded_frac_coords = _get_super_cell_frac_coords(lattice, frac_coords, size)
+    expanded_frac_coords = _get_super_cell_grid_frac_coords(lattice, frac_coords, size)
     expanded_coords = expanded_frac_coords @ lattice
     flattened_expanded_coords = expanded_coords.reshape(-1, dim)
 
     voronoi = Voronoi(flattened_expanded_coords)
     ridge_points_unraveled = np.array(np.unravel_index(voronoi.ridge_points, expanded_coords.shape[:-1]))
     # shape: (num_ridges, 2 (source, target), 4 (3 cell_index + 1 atom_index))
     ridge_points_unraveled = np.moveaxis(ridge_points_unraveled, np.arange(dim), np.roll(np.arange(dim), 1))
@@ -683,33 +687,32 @@
     """
     dim = lattice.shape[0]
     cube = _get_cube(dim)
     max_radius = np.max(np.linalg.norm((cube - 1 / 2) @ lattice, axis=1))
     return max_radius * 2
 
 
-# def _get_super_cell_size_from_radius(lattice: np.ndarray, radius: float):
-#     dim = lattice.shape[0]
-#     max_diameter = _get_max_diameter(lattice)
-#     radius_ = radius + max_diameter
-#     cell_indices = np.ceil(np.sum(np.abs(np.linalg.inv(lattice)), axis=0) * radius_).astype(int)
-#     cells = _get_mesh(cell_indices + 1, dim)
-#     lattice_point_coords = cells @ lattice
-#     images = np.argwhere(np.linalg.norm(lattice_point_coords, axis=-1) <= radius_)
-#     super_cell_size = images.max(axis=0)
-#     return super_cell_size
+def _get_super_cell_grid_frac_coords(lattice: np.ndarray, frac_coords: np.ndarray, size: Union[int, list, np.ndarray]):
+    """Get frac coordinates for positions in a grid of unit cells that is a cubic super-cell.
 
+    ..code - block:: python
 
-def _get_super_cell_frac_coords(lattice: np.ndarray, frac_coords: np.ndarray, size: Union[int, list, np.ndarray]):
-    """Get a list of frac coordinates for all super-cell positions.
+        import numpy as np
+        from kgcnn.crystal.graph_builder import _get_super_cell_grid_frac_coords
+        coordinates = _get_super_cell_grid_frac_coords(
+            np.array([[1.0, 0.0, 0.0], [0.0, 1.0, 0.5], [0.0, 0.5, 1.5]]),
+            np.array([[0.0, 0.0, 0.0], [0.5, 0.5, 0.5]]),
+            [3, 3, 3]
+        )
+        print(coordinates.shape)  # (7, 7, 7, 2, 3)
 
     Args:
         lattice (np.ndarray): Lattice matrix.
         frac_coords (np.ndarray): Fractional coordinates of atoms in unit cell.
-        size (list): Size of the super-cell.
+        size (list): Size of the super-cell in each dimension.
 
     Returns:
         np.ndarray: List of fractional coordinates of atoms in the super-cell.
     """
     dim = lattice.shape[0]
 
     if isinstance(size, int):
```

### Comparing `kgcnn-3.0.0/kgcnn/crystal/periodic_table/periodic_table.py` & `kgcnn-3.0.1/kgcnn/crystal/periodic_table/periodic_table.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/crystal/preprocessor.py` & `kgcnn-3.0.1/kgcnn/crystal/preprocessor.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/base.py` & `kgcnn-3.0.1/kgcnn/data/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 module_logger.setLevel(logging.INFO)
 
 
 class MemoryGraphList(list):
     r"""Class to store a list of graph dictionaries in memory.
 
     Inherits from a python list. The graph properties are defined by tensor-like (numpy) arrays
-    for indices, attributes, labels, symbol etc. in :obj:`GraphDict`, which are the items of the list.
+    for indices, attributes, labels, symbol etc. in :obj:`GraphDict` , which are the items of the list.
     Access to items via `[]` indexing operator.
 
     A python list of a single named property can be obtained from each :obj:`GraphDict` in :obj:`MemoryGraphList` via
     :obj:`get` or assigned from a python list via :obj:`set` methods.
 
     The :obj:`MemoryGraphList` further provides simple map-functionality :obj:`map_list` to apply methods for
     each :obj:`GraphDict`, and to cast properties to tensor with :obj:`tensor`.
@@ -64,28 +64,28 @@
 
     def validate(self):
         for i, x in enumerate(self):
             if not isinstance(x, GraphDict):
                 self[i] = GraphDict(x)
 
     def assign_property(self, key: str, value: list):
-        """Assign a list of numpy arrays of a property to :obj:`GraphDict` s in this list.
+        """Assign a list of numpy arrays of a property to the respective :obj:`GraphDict` s in this list.
 
         Args:
             key (str): Name of the property.
             value (list): List of numpy arrays for property `key` .
 
         Returns:
             self
         """
         if value is None:
             # We could also here remove the key from all graphs.
             return self
         if not isinstance(value, list):
-            raise TypeError("Expected type 'list' to assign graph properties.")
+            raise TypeError("Expected type `list` to assign graph properties.")
         if len(self) == 0:
             self.empty(len(value))
         if len(self) != len(value):
             raise ValueError("Can only store graph attributes from list with same length.")
         for i, x in enumerate(value):
             self[i].assign_property(key, x)
         return self
@@ -119,15 +119,15 @@
             return MemoryGraphList([super(MemoryGraphList, self).__getitem__(int(i)) for i in item])
         if isinstance(item, np.ndarray):
             return MemoryGraphList([super(MemoryGraphList, self).__getitem__(int(i)) for i in item])
         raise TypeError("Unsupported type for `MemoryGraphList` items.")
 
     def __setitem__(self, key, value):
         if not isinstance(value, GraphDict):
-            raise TypeError("Require a GraphDict as list item.")
+            raise TypeError("Require a `GraphDict` as list item.")
         super(MemoryGraphList, self).__setitem__(key, value)
 
     def __repr__(self):
         return "<{} [{}]>".format(type(self).__name__, "" if len(self) == 0 else self[0].__repr__() + " ...")
 
     def append(self, graph):
         assert isinstance(graph, GraphDict), "Must append `GraphDict` to self."
@@ -204,16 +204,17 @@
                 E.g.: `[{'name': 'edge_indices', 'ragged': True}, {...}, ...]`.
             make_copy (bool): Whether to copy the data. Default is True.
 
         Returns:
             list: List of Tensors.
         """
         if isinstance(items, dict):
-            if all([isinstance(value, dict) for value in items.values()]) and "name" not in items:
-                return {key: self._to_tensor(value, make_copy=make_copy) for key, value in items.items()}
+            if all([isinstance(value, dict) for value in items.values() if value is not None]) and "name" not in items:
+                return {key: self._to_tensor(value, make_copy=make_copy) for key, value in items.items() if
+                        value is not None}
             return self._to_tensor(items, make_copy=make_copy)
         elif isinstance(items, (tuple, list)):
             return [self._to_tensor(x, make_copy=make_copy) for x in items]
         else:
             raise TypeError("Wrong type, expected e.g. [{'name': 'edge_indices', 'ragged': True}, {...}, ...]")
 
     def map_list(self, method: Union[str, Callable], **kwargs):
@@ -296,14 +297,32 @@
         else:
             self.logger.info("No invalid graphs for assigned properties found.")
         # Remove from the end via pop().
         for i in invalid_graphs:
             self.pop(int(i))
         return invalid_graphs
 
+    def rename_property_on_graphs(self, old_property_name: str, new_property_name: str) -> list:
+        """Change the name of a graph property on all graphs in the list.
+
+        Args:
+            old_property_name (str): Old property name.
+            new_property_name (str): New property name.
+
+        Returns:
+            list: List indices of replaced property names.
+        """
+        replaced_list = []
+        for i, x in enumerate(self):
+            if old_property_name in x:
+                self[i][new_property_name] = x[old_property_name]
+                self[i].pop(old_property_name)
+                replaced_list.append(i)
+        return replaced_list
+
     # Alias of internal assign and obtain property.
     set = assign_property
     get = obtain_property
 
 
 class MemoryGraphDataset(MemoryGraphList):
     r"""Dataset class for lists of graph tensor dictionaries stored on file and fit into memory.
@@ -496,19 +515,24 @@
                 hyper_input = [hyper_input]
             else:
                 # In principle keras also accepts a dictionary for model inputs. Just cast to list here.
                 hyper_input = list(hyper_input.values())
 
         # Check if we have List[dict].
         for x in hyper_input:
+            if x is None:
+                message_warning("Found 'None' in place of model input. Skipping this input.")
+                continue
             if not isinstance(x, dict):
                 message_error(
                     "Wrong type of list item in `assert_valid_model_input`. Found '%s' but must be `dict` ." % type(x))
 
         for x in hyper_input:
+            if x is None:
+                continue
             if "name" not in x:
                 message_error("Can not infer name from '%s' for model input." % x)
             data = [dataset[i].obtain_property(x["name"]) for i in range(len(dataset))]
             prop_in_data = [y is None for y in data]
             if all(prop_in_data):
                 message_error("Property %s is not defined for any graph in list. Please check property." % x["name"])
             if any(prop_in_data):
@@ -629,14 +653,15 @@
         """
         split_indices = [[]]
 
         def check_and_extend_splits(to_split):
             if to_split - len(split_indices) + 1 > 0:
                 for _ in range(to_split - len(split_indices) + 1):
                     split_indices.append([])
+
         graphs = self.obtain_property(name)
         for i, s in enumerate(graphs):
             if s is None:
                 self.error("Split assignment on graph '%s' is not defined." % i)
                 continue
             for x in s:
                 check_and_extend_splits(x)
```

### Comparing `kgcnn-3.0.0/kgcnn/data/crystal.py` & `kgcnn-3.0.1/kgcnn/data/crystal.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import defaultdict
 from typing import Dict, Callable, List, Union
 import pandas as pd
 import pymatgen
 import pymatgen.io.cif
 import pymatgen.core.structure
 import pymatgen.symmetry.structure
-
+from kgcnn.utils.serial import deserialize
 from kgcnn.data.base import MemoryGraphDataset
 from kgcnn.data.utils import save_json_file, load_json_file
 from kgcnn.crystal.base import CrystalPreprocessor
 from kgcnn.graph.base import GraphDict
 
 
 class CrystalDataset(MemoryGraphDataset):
@@ -265,14 +265,16 @@
             reset_graphs (bool): Whether to reset the graph information. Default is False.
 
         Returns:
 
         """
         if reset_graphs:
             self.clear()
+        if isinstance(pre_processor, dict):
+            pre_processor = deserialize(pre_processor)
         # Read pymatgen JSON file from file.
         structs = self.get_structures_from_json_file()
         if reset_graphs:
             self.empty(len(structs))
 
         pre_processor.output_graph_as_dict = True
```

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/ClinToxDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/ClinToxDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/CoraDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/CoraDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/CoraLuDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/CoraLuDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/ESOLDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/ESOLDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/FreeSolvDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/FreeSolvDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/GraphTUDataset2020.py` & `kgcnn-3.0.1/kgcnn/data/datasets/GraphTUDataset2020.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/ISO17Dataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/ISO17Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/LipopDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/LipopDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MD17Dataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MD17Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MD17RevisedDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MD17RevisedDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MUTAGDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MUTAGDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatBenchDataset2020.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatBenchDataset2020.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectDielectricDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectDielectricDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectEFormDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectEFormDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectGapDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectGapDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectIsMetalDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectIsMetalDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectJdft2dDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectJdft2dDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectLogGVRHDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectLogGVRHDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectLogKVRHDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectLogKVRHDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectPerovskitesDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectPerovskitesDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectPhononsDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectPhononsDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MoleculeNetDataset2018.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MoleculeNetDataset2018.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/MutagenicityDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/MutagenicityDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/PROTEINSDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/PROTEINSDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/QM7Dataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/QM7Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/QM7bDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/QM7bDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/QM8Dataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/QM8Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/QM9Dataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/QM9Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/QM9MolNetDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/QM9MolNetDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/SIDERDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/SIDERDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/datasets/Tox21MolNetDataset.py` & `kgcnn-3.0.1/kgcnn/data/datasets/Tox21MolNetDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/download.py` & `kgcnn-3.0.1/kgcnn/data/download.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/moleculenet.py` & `kgcnn-3.0.1/kgcnn/data/moleculenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     """
     # Dictionaries values are lists, one for each attribute defines in "callbacks" and each value in those
     # lists corresponds to one molecule in the dataset.
     if data is None:
         if logger is not None:
             logger.error("Received no pandas data.")
     if mol_list is None:
-        raise ValueError("Expected list of mol-string. But got '%s'" % mol_list)
+        raise ValueError("Expected list of mol-string. But got '%s'." % mol_list)
 
     value_lists = defaultdict(list)
     for index, sm in enumerate(mol_list):
 
         mg = mol_interface_class(make_directed=make_directed).from_mol_block(
             sm, keep_hs=add_hydrogen, sanitize=sanitize)
```

### Comparing `kgcnn-3.0.0/kgcnn/data/qm.py` & `kgcnn-3.0.1/kgcnn/data/qm.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,16 @@
             "edge_indices": lambda mg, ds: mg.edge_number[0],
             "edge_number": lambda mg, ds: np.array(mg.edge_number[1], dtype='int'),
             **additional_callbacks
         }
         # Label callback.
         if label_column_name:
             callbacks.update({'graph_labels': lambda mg, ds: ds[label_column_name]})
-        # Attributes callback.
+
+        # Attributes callbacks.
         if nodes:
             callbacks.update({
                 'node_attributes': lambda mg, ds: np.array(mg.node_attributes(nodes, encoder_nodes), dtype='float32')
             })
         if edges:
             callbacks.update({
                 'edge_attributes': lambda mg, ds: np.array(mg.edge_attributes(edges, encoder_edges)[1], dtype='float32')
@@ -327,13 +328,13 @@
                 encoder_edges=encoder_edges, encoder_graph=encoder_graph, add_hydrogen=add_hydrogen,
                 make_directed=make_directed, additional_callbacks=additional_callbacks, sanitize=sanitize,
                 custom_transform=custom_transform
             )
         else:
             # Try to read labels and xyz-file without mol-interface.
             self.warning("Failed to load structures SDF file. Reading geometries from XYZ file instead. Please check.")
-            self.read_in_table_file()
-            if self.data_frame is not None and label_column_name is not None:
-                labels = self.data_frame[label_column_name]
-                self.assign_property("graph_labels", [np.array(x) for _, x in labels.iterrows()])
+            data_frame = self.read_in_table_file().data_frame
+            if data_frame is not None and label_column_name is not None:
+                self.assign_property("graph_labels", [
+                    np.array(data_frame.loc[index][label_column_name]) for index in range(data_frame.shape[0])])
             self.read_in_memory_xyz()
         return self
```

### Comparing `kgcnn-3.0.0/kgcnn/data/serial.py` & `kgcnn-3.0.1/kgcnn/data/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/transform/scaler/force.py` & `kgcnn-3.0.1/kgcnn/data/transform/scaler/force.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/transform/scaler/molecule.py` & `kgcnn-3.0.1/kgcnn/data/transform/scaler/molecule.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/transform/scaler/serial.py` & `kgcnn-3.0.1/kgcnn/data/transform/scaler/serial.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import importlib
 from typing import Union
 from kgcnn.utils.serial import deserialize as deserialize_general
 
+
 module_list = {
-    "StandardScaler": "kgcnn.data.transform.standard",
-    "StandardLabelScaler": "kgcnn.data.transform.standard",
-    "ExtensiveMolecularScaler": "kgcnn.data.transform.molecule",
-    "ExtensiveMolecularLabelScaler": "kgcnn.data.transform.molecule",
-    "EnergyForceExtensiveLabelScaler": "kgcnn.data.transform.force",
-    "QMGraphLabelScaler": "kgcnn.data.transform.mol"
+    "StandardScaler": "kgcnn.data.transform.scaler.standard",
+    "StandardLabelScaler": "kgcnn.data.transform.scaler.standard",
+    "ExtensiveMolecularScaler": "kgcnn.data.transform.scaler.molecule",
+    "ExtensiveMolecularLabelScaler": "kgcnn.data.transform.scaler.molecule",
+    "EnergyForceExtensiveLabelScaler": "kgcnn.data.transform.scaler.force",
+    "QMGraphLabelScaler": "kgcnn.data.transform.scaler.molecule"
 }
 
 
 def deserialize(name: Union[str, dict], **kwargs):
     """Deserialize a scaler class.
 
     Args:
@@ -39,8 +40,8 @@
         # if given as string name. Lookup identifier.
         if name not in module_list:
             raise ValueError("Unknown name for scaler '%s'." % name)
         module_name = module_list[name]
         obj_class = getattr(importlib.import_module(str(module_name)), str(name))
         return obj_class(**kwargs)
 
-    raise TypeError("Wrong type for deserialization. Require 'str' or 'dict'.")
+    raise TypeError("Wrong type for deserialization. Require 'str' or 'dict'.")
```

### Comparing `kgcnn-3.0.0/kgcnn/data/transform/scaler/standard.py` & `kgcnn-3.0.1/kgcnn/data/transform/scaler/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class StandardScalerSklearnBase(StandardScalerSklearn):
     r"""Base standard scaler of :obj:`sklearn` with added functionality to save and load weights of this scaler similar
     to keras layers and objects.
 
     .. code-block:: python
 
         import numpy as np
-        from kgcnn.scaler.scaler import StandardScalerSklearnBase
+        from kgcnn.data.transform.scaler.standard import StandardScalerSklearnBase
         data = np.random.rand(5).reshape((5,1))
         scaler = StandardScalerSklearnBase()
         scaler.fit(X=data)
         print(scaler.get_weights())
         print(scaler.get_config())
 
     """
@@ -126,17 +126,18 @@
             X (str): Name of X information in dataset. For example "graph_properties".
             y (str): Not used.
             sample_weight (str): Name of sample weight information in dataset. For example "sample_weight".
 
         Returns:
             self.
         """
-        return self.fit(
-            X=[item[X] for item in dataset],
-            y=None,
+        return super(StandardScalerSklearnBase, self).fit(
+            [item[X] for item in dataset],
+            # We can ignore y here. None is default for sklearn StandardScaler.
+            # y=None
             sample_weight=[item[sample_weight] for item in dataset] if sample_weight is not None else None
         )
 
     # noinspection PyPep8Naming
     def transform_dataset(self, dataset: List[Dict[str, np.ndarray]],
                           X: str = None,
                           copy: bool = True,
@@ -151,16 +152,16 @@
             copy_dataset (bool): Whether to copy full dataset. Default is False.
 
         Returns:
             dataset: Transformed dataset.
         """
         if copy_dataset:
             dataset = dataset.copy()
-        out = self.transform(
-            X=[graph[X] for graph in dataset],
+        out = super(StandardScalerSklearnBase, self).transform(
+            [graph[X] for graph in dataset],
             copy=copy,
         )
         for graph, out_value in zip(dataset, out):
             graph[X] = out_value
         return dataset
 
     # noinspection PyPep8Naming
@@ -178,16 +179,16 @@
             copy_dataset (bool): Whether to copy full dataset. Default is False.
 
         Returns:
             dataset: Inverse-transformed dataset.
         """
         if copy_dataset:
             dataset = dataset.copy()
-        out = self.inverse_transform(
-            X=[graph[X] for graph in dataset],
+        out = super(StandardScalerSklearnBase, self).inverse_transform(
+            [graph[X] for graph in dataset],
             copy=copy,
         )
         for graph, out_value in zip(dataset, out):
             graph[X] = out_value
         return dataset
 
     # noinspection PyPep8Naming
@@ -218,15 +219,15 @@
 class StandardScaler(StandardScalerSklearnBase):
     r"""Standard scaler that inherits from :obj:`sklearn.preprocessing.StandardScaler` .
     Included unused kwarg 'atomic_number' to be compatible with some material oriented scaler.
 
     .. code-block:: python
 
         import numpy as np
-        from kgcnn.scaler.scaler import StandardScaler
+        from kgcnn.data.transform.scaler.standard import StandardScaler
         data = np.random.rand(5).reshape((5,1))
         scaler = StandardScaler()
         scaler.fit(X=data)
         print(scaler.get_weights())
         print(scaler.get_config())
         print(scaler.inverse_transform(scaler.transform(X=data)))
         print(data)
@@ -257,15 +258,15 @@
     # noinspection PyPep8Naming
     def partial_fit(self, X, y=None, sample_weight=None, atomic_number=None):
         r"""Online computation of mean and std on X for later scaling.
         All of X is processed as a single batch. This is intended for cases
         when :meth:`fit` is not feasible due to very large number of
         `n_samples` or because X is read from a continuous stream.
         The algorithm for incremental mean and std is given in Equation 1.5a,b
-        in `Chan, et al. (1982) <https://www.tandfonline.com/doi/abs/10.1080/00031305.1983.10483115>`_ .
+        in `Chan, et al. (1982) <https://www.tandfonline.com/doi/abs/10.1080/00031305.1983.10483115>`__ .
 
         Args:
             X (np.ndarray): Array of shape (n_samples, n_features)
                 The data used to compute the mean and standard deviation
                 used for later scaling along the feature's axis.
             y (np.ndarray, None): Ignored.
             sample_weight (np.ndarray): Array-like of shape (n_samples,), default=None
@@ -419,15 +420,15 @@
     r"""Standard scaler for labels that inherits from :obj:`sklearn.preprocessing.StandardScaler` .
     Included unused kwarg 'atomic_number' to be compatible with some material oriented scaler.
     Uses `y` argument for scaling labels and `X` is ignored.
 
     .. code-block:: python
 
         import numpy as np
-        from kgcnn.data.transform.scaler.scaler import StandardLabelScaler
+        from kgcnn.data.transform.scaler.standard import StandardLabelScaler
         data = np.random.rand(5).reshape((5,1))
         scaler = StandardLabelScaler()
         scaler.fit(y=data)
         print(scaler.fit_transform(y=data))
         print(scaler.get_weights())
         print(scaler.get_config())
         print(scaler.inverse_transform(y=scaler.transform(y=data)))
@@ -460,57 +461,61 @@
             atomic_number (list): Ignored.
 
         Returns:
             self: Fitted scaler.
         """
         # fit() of sklearn uses reset and partial fit. Just adding y in place of X.
         self._validate_input(y, X)
-        return super(StandardLabelScaler, self).fit(y, sample_weight=sample_weight)
+        self._reset()
+        return super(StandardLabelScaler, self).partial_fit(X=y, sample_weight=sample_weight)
 
     # noinspection PyPep8Naming
     def partial_fit(self, y: np.ndarray, X=None, sample_weight=None, atomic_number=None):
         r"""Online computation of mean and std on y for later scaling.
         All of y is processed as a single batch. This is intended for cases
         when :meth:`fit` is not feasible due to very large number of
         `n_samples` or because y is read from a continuous stream.
         The algorithm for incremental mean and std is given in Equation 1.5a,b
-        in `Chan, et al. (1982) <https://www.tandfonline.com/doi/abs/10.1080/00031305.1983.10483115>`_ .
+        in `Chan, et al. (1982) <https://www.tandfonline.com/doi/abs/10.1080/00031305.1983.10483115>`__ .
 
         Args:
             y (np.ndarray): Array of shape (n_samples, n_labels)
                 The data used to compute the mean and standard deviation
                 used for later scaling along the feature's axis.
             X (None): Ignored.
             sample_weight (np.ndarray): Individual weights for each sample.
             atomic_number (list): Ignored.
 
         Returns:
             self: Fitted scaler.
         """
         # For partial fit internally uses args and not kwargs.
         # Can not request kwargs after argument X, y here.
+        # Just changing order of x,y here.
         self._validate_input(y, X)
-        return super(StandardLabelScaler, self).partial_fit(y, sample_weight=sample_weight)
+        return super(StandardLabelScaler, self).partial_fit(X=y, sample_weight=sample_weight)
 
     # noinspection PyPep8Naming
-    def fit_transform(self, y: np.ndarray, *, X=None, atomic_number=None, **fit_params):
+    def fit_transform(self, y: np.ndarray, *, X=None, atomic_number=None, copy=None, **fit_params):
         r"""Perform fit and standardization by centering and scaling.
 
         Args:
             y (np.ndarray): Array of shape (n_samples, n_labels)
                 The data used to compute the mean and standard deviation
                 used for later scaling along the feature's axis.
             X (None): Ignored.
             atomic_number (list): Ignored.
+            copy (bool): Copy the input `y` or not.
             fit_params (Any): Kwargs for fit.
 
         Returns:
             y_tr (np.ndarray): Transformed array of shape (n_samples, n_labels).
         """
-        return super(StandardLabelScaler, self).fit_transform(y, **fit_params)
+        self.fit(y=y, X=X, atomic_number=atomic_number, **fit_params)
+        return self.transform(y=y, X=X, copy=copy, atomic_number=atomic_number)
 
     # noinspection PyPep8Naming
     def transform(self, y: np.ndarray, *, X=None, copy=None, atomic_number=None):
         r"""Perform standardization by centering and scaling.
 
         Args:
             y (None): Array of shape (n_samples, n_labels)
```

### Comparing `kgcnn-3.0.0/kgcnn/data/tudataset.py` & `kgcnn-3.0.1/kgcnn/data/tudataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/data/utils.py` & `kgcnn-3.0.1/kgcnn/data/utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/graph/base.py` & `kgcnn-3.0.1/kgcnn/graph/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,16 @@
 
     def from_networkx(self, graph: nx.Graph,
                       node_number: str = "node_number",
                       edge_indices: str = "edge_indices",
                       node_attributes: Union[str, List[str]] = None,
                       edge_attributes: Union[str, List[str]] = None,
                       graph_attributes: Union[str, List[str]] = None,
-                      node_labels: str = None):
+                      node_labels: str = None,
+                      reverse_edge_indices: bool = False):
         r"""Convert a networkx graph instance into a dictionary of graph-tensors. The networkx graph is always converted
         into integer node labels. The former node IDs can be hold in :obj:`node_labels`. Furthermore, node or edge
         data can be cast into attributes via :obj:`node_attributes` and :obj:`edge_attributes`.
 
         Args:
             graph (nx.Graph): A networkx graph instance to convert.
             node_number (str): The name that the node numbers are assigned to. Default is "node_number".
@@ -191,14 +192,15 @@
             node_attributes (str, list): Name of node attributes to add from node data. Can also be a list of names.
                 Default is None.
             edge_attributes (str, list): Name of edge attributes to add from edge data. Can also be a list of names.
                 Default is None.
             graph_attributes (str, list): Name of graph attributes to add from graph data. Can also be a list of names.
                 Default is None.
             node_labels (str): Name of the labels of nodes to store former node IDs into. Default is None.
+            reverse_edge_indices (bool): Whether to reverse edge indices for notation '(ij, i<-j)'. Default is False.
 
         Returns:
             self.
         """
         assert node_labels is None or isinstance(node_labels, str), "Please provide name of node labels or `None`"
         graph_int = nx.convert_node_labels_to_integers(graph, label_attribute=node_labels)
         graph_size = len(graph_int)
@@ -226,15 +228,18 @@
                 node_attr_dict[d][i] = x[1][d]
 
         # Loop over edges in graph.
         edge_id = []
         edges_attr = _attr_to_list(edge_attributes)
         edges_attr_dict = {x: [None] * graph_int.number_of_edges() for x in edges_attr}
         for i, x in enumerate(graph_int.edges.data()):
-            edge_id.append(x[:2])
+            if reverse_edge_indices:
+                edge_id.append([x[1], x[0]])
+            else:
+                edge_id.append([x[0], x[1]])
             for d in edges_attr:
                 if d not in x[2]:
                     raise KeyError("Edge does not have property '%s'." % d)
                 edges_attr_dict[d][i] = x[2][d]
 
         graph_attr = _attr_to_list(graph_attributes)
         graph_attr_dict = {x: None for x in graph_attr}
```

### Comparing `kgcnn-3.0.0/kgcnn/graph/methods/__init__.py` & `kgcnn-3.0.1/kgcnn/graph/methods/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from ._adj import (
     get_angle_indices, coordinates_to_distancematrix, invert_distance,
     define_adjacency_from_distance, sort_edge_indices, get_angle, add_edges_reverse_indices,
     rescale_edge_weights_degree_sym, add_self_loops_to_edge_indices, compute_reverse_edges_index_map,
-    distance_to_gauss_basis, get_angle_between_edges
+    distance_to_gauss_basis, get_angle_between_edges, convert_scaled_adjacency_to_list
 )
 from ._geom import (
     range_neighbour_lattice, get_principal_moments_of_inertia,
     shift_coordinates_to_unit_cell, distance_for_range_indices, distance_for_range_indices_periodic,
     coulomb_matrix_to_inverse_distance_proton, coordinates_from_distance_matrix
 )
 
 __all__ = [
     # adj
     "get_angle_indices", "coordinates_to_distancematrix", "invert_distance",
     "define_adjacency_from_distance", "sort_edge_indices", "get_angle", "add_edges_reverse_indices",
     "rescale_edge_weights_degree_sym", "add_self_loops_to_edge_indices", "compute_reverse_edges_index_map",
-    "distance_to_gauss_basis", "get_angle_between_edges",
+    "distance_to_gauss_basis", "get_angle_between_edges", "convert_scaled_adjacency_to_list",
     # geom
     "range_neighbour_lattice", "get_principal_moments_of_inertia",
     "shift_coordinates_to_unit_cell", "distance_for_range_indices", "distance_for_range_indices_periodic",
     "coulomb_matrix_to_inverse_distance_proton", "coordinates_from_distance_matrix"
 ]
```

### Comparing `kgcnn-3.0.0/kgcnn/graph/methods/_adj.py` & `kgcnn-3.0.1/kgcnn/graph/methods/_adj.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/graph/methods/_geom.py` & `kgcnn-3.0.1/kgcnn/graph/methods/_geom.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/graph/postprocessor.py` & `kgcnn-3.0.1/kgcnn/graph/postprocessor.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/graph/preprocessor.py` & `kgcnn-3.0.1/kgcnn/graph/preprocessor.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/graph/serial.py` & `kgcnn-3.0.1/kgcnn/graph/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/io/loader.py` & `kgcnn-3.0.1/kgcnn/io/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     r"""Example (minimal) implementation of a graph batch loader based on :obj:`ks.utils.Sequence` ."""
 
     def __init__(self,
                  data: Union[List[dict], MemoryGraphDataset],
                  inputs: Union[dict, List[dict]],
                  outputs: Union[dict, List[dict]],
                  batch_size: int = 32,
-                 shuffle: bool = False):
+                 shuffle: bool = False,
+                 device: str = None):
         """Initialization with data and input information.
 
         Args:
             data (list, MemoryGraphDataset): Any iterable data that implements indexing operator for graph instance.
                 Each graph instance must implement indexing operator for named property.
             inputs (dict, list):  List of dictionaries that specify graph properties in list via 'name' key.
                 The dict-items match the tensor input for :obj:`tf.keras.layers.Input` layers.
@@ -27,37 +28,42 @@
                 E.g.: `[{'name': 'edge_indices', 'ragged': True}, {...}, ...]`.
             outputs (dict, list): List of dictionaries that specify graph properties in list via 'name' key.
                 Required dict-keys should be 'name' and 'ragged'.
                 Optionally shape information can be included via 'shape'.
                 E.g.: `[{'name': 'graph_labels', 'ragged': False}, {...}, ...]`.
             batch_size (int): Batch size. Default is 32.
             shuffle (bool): Whether to shuffle data. Default is False.
+            device (str): Device to make tensor on. For multiprocessing this can cause deadlocks if e.g. set on GPU.
+                Example for CPU would be '/cpu:0' .
         """
         self.data = data
         self.inputs = inputs
         self.outputs = outputs
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.indices = np.arange(len(data))
-
+        self.device = device
         self._shuffle_indices()
 
     def __len__(self):
         """Denotes the number of batches per epoch"""
         return int(np.ceil(len(self.data) / float(self.batch_size)))
 
     def __getitem__(self, index):
         """Generate one batch of data"""
         # Generate indexes of the batch
         batch_indices = self.indices[index * self.batch_size:(index + 1) * self.batch_size]
 
         # Generate data
-        x_model, y_model = self._data_generation(batch_indices)
+        if self.device is not None:
+            with tf.device(self.device):
+                x_model, y_model = self._data_generation(batch_indices)
+        else:
+            x_model, y_model = self._data_generation(batch_indices)
 
-        # return batch_indexes
         return x_model, y_model
 
     def _shuffle_indices(self):
         if self.shuffle:
             np.random.shuffle(self.indices)
 
     def on_epoch_end(self):
@@ -67,17 +73,21 @@
     @staticmethod
     def _to_tensor(item: Union[np.ndarray, list], is_ragged: bool):
         if is_ragged:
             return ragged_tensor_from_nested_numpy(item)
         else:
             return tf.constant(np.array(item))
 
+    def _get_data(self, index):
+        # Accessing data method. E.g. loading from file etc.
+        return self.data[int(index)]
+
     def _data_generation(self, batch_indices: Union[np.ndarray, list]):
         """Generates data containing batch_size samples"""
-        graphs = [self.data[int(i)] for i in batch_indices]
+        graphs = [self._get_data(i) for i in batch_indices]
         # Inputs
         inputs = self.inputs if not isinstance(self.inputs, dict) else [self.inputs]
         x_inputs = []
         for i in inputs:
             data_list = [g[i["name"]] for g in graphs]
             is_ragged = i["ragged"] if "ragged" in i else False
             x_inputs.append(self._to_tensor(data_list, is_ragged))
```

### Comparing `kgcnn-3.0.0/kgcnn/layers/README.md` & `kgcnn-3.0.1/kgcnn/layers/README.md`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/attention.py` & `kgcnn-3.0.1/kgcnn/layers/attention.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/base.py` & `kgcnn-3.0.1/kgcnn/layers/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/casting.py` & `kgcnn-3.0.1/kgcnn/layers/casting.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/conv.py` & `kgcnn-3.0.1/kgcnn/layers/conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
                        "bias_constraint": bias_constraint, "kernel_initializer": kernel_initializer,
                        "bias_initializer": bias_initializer, "use_bias": use_bias}
 
         self.gather_nodes_outgoing = GatherNodesOutgoing()
         self.concatenate = LazyConcatenate()
         self.update_node_from_neighbors_mlp = GraphMLP(units=units, activation=activation, **kernel_args)
         self.update_node_from_self_mlp = GraphMLP(units=units, activation=activation, **kernel_args)
+        self.pooling_args = {"pooling_method": pooling_method}
         if self.pooling_args['pooling_method'] in ["LSTM", "lstm"]:
             # We do not allow full access to all parameters for the LSTM here for simplification.
             self.pooling = PoolingLocalEdgesLSTM(pooling_method=pooling_method, units=units)
         else:
             self.pooling = PoolingLocalMessages(pooling_method=pooling_method)
         self.normalize_nodes = GraphLayerNormalization(axis=-1)
```

### Comparing `kgcnn-3.0.0/kgcnn/layers/gather.py` & `kgcnn-3.0.1/kgcnn/layers/gather.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tensorflow as tf
 from kgcnn.layers.base import GraphBaseLayer
 from kgcnn.ops.partition import partition_row_indexing
+from typing import Union
 # from kgcnn.ops.axis import get_positive_axis
 ks = tf.keras
 
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='GatherEmbedding')
 class GatherEmbedding(GraphBaseLayer):
     r"""Gather node or edge embedding from an index list.
@@ -24,24 +25,26 @@
 
         Default of this layer is concatenation with :obj:`concat_axis=2`.
 
     Example of usage for :obj:`GatherEmbedding`:
 
     .. code-block:: python
 
+        import tensorflow as tf
+        from kgcnn.layers.gather import GatherEmbedding
         nodes = tf.ragged.constant([[[0.0],[1.0]],[[2.0],[3.0],[4.0]]], ragged_rank=1)
         edge_idx = tf.ragged.constant([[[0,1],[1,0]],[[0,2],[1,2]]], ragged_rank=1)
         print(GatherEmbedding()([nodes, edge_idx]))
 
     """
 
     def __init__(self,
                  axis: int = 1,
-                 concat_axis: int = 2,
-                 split_axis: int = None,
+                 concat_axis: Union[int, None] = 2,
+                 split_axis: Union[int, None] = None,
                  split_indices: list = None,
                  concat_indices: list = None,
                  **kwargs):
         r"""Initialize layer.
 
         Args:
             axis (int): The axis to gather embeddings from. Default is 1.
@@ -146,15 +149,15 @@
         return config
 
 
 GatherNodes = GatherEmbedding
 
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='GatherEmbeddingSelection')
-class GatherEmbeddingSelection(GraphBaseLayer):
+class GatherEmbeddingSelection(GatherEmbedding):
     r"""Gather node or edge embedding for a defined index in the index list.
 
     The embeddings are gather from a ragged index tensor for a list of specific indices which are given by
     :obj:`selection_index`. This can be used for ingoing or outgoing nodes or angles.
     Returns a list of embeddings for each :obj:`selection_index`. An edge is defined by index tuple :math:`(i, j)`.
     In the default definition, index :math:`i` is expected to be the receiving or target node.
     Effectively, the layer simply does:
@@ -167,89 +170,49 @@
     :obj:`axis_indices`.
     This layer always returns a list of embeddings even if :obj:`selection_index` is of type :obj:`int`.
 
     Example of usage for :obj`GatherEmbeddingSelection`:
 
     .. code-block:: python
 
+        import tensorflow as tf
+        from kgcnn.layers.gather import GatherEmbeddingSelection
         nodes = tf.ragged.constant([[[0.0],[1.0]],[[2.0],[3.0],[4.0]]], ragged_rank=1)
         edge_idx = tf.ragged.constant([[[0,1],[1,0]],[[0,2],[1,2]]], ragged_rank=1)
         print(GatherEmbeddingSelection([0, 1])([nodes, edge_idx]))
 
     """
 
     def __init__(self, selection_index, axis: int = 1, axis_indices: int = 2, **kwargs):
         r"""Initialize layer.
 
         Args:
             selection_index (list, int): Which indices to gather embeddings for.
             axis (int): Axis to gather embeddings from. Default is 1.
             axis_indices (int): From which axis to take the indices for gather. Default is 2.
         """
-        super(GatherEmbeddingSelection, self).__init__(**kwargs)
-        self.axis = axis
-        self.axis_indices = axis_indices
-        self.node_indexing = "sample"
-
         if not isinstance(selection_index, (list, tuple, int)):
             raise ValueError("Indices for selection must be list or tuple for layer `GatherEmbeddingSelection`.")
 
         if isinstance(selection_index, int):
-            self.selection_index = [selection_index]
+            selection_index = [selection_index]
         else:
-            self.selection_index = list(selection_index)
-
-    def build(self, input_shape):
-        """Build layer."""
-        super(GatherEmbeddingSelection, self).build(input_shape)
-
-    def _disjoint_implementation(self, inputs, **kwargs):
-        # The primary case for aggregation of nodes from node feature list. Case from doc-string.
-        # Faster implementation via values and indices shifted by row-partition. Equal to disjoint implementation.
-        if all([isinstance(x, tf.RaggedTensor) for x in inputs]):
-            if all([x.ragged_rank == 1 for x in inputs]) and self.axis == 1 and self.axis_indices == 2:
-                # We cast to value here
-                node, node_part = inputs[0].values, inputs[0].row_splits
-                edge_index, edge_part = inputs[1].values, inputs[1].row_lengths()
-                indexlist = partition_row_indexing(edge_index, node_part, edge_part,
-                                                   partition_type_target="row_splits",
-                                                   partition_type_index="row_length",
-                                                   to_indexing='batch',
-                                                   from_indexing=self.node_indexing)
-                out = [tf.gather(node, tf.gather(indexlist, i, axis=1), axis=0) for i in self.selection_index]
-                out = [tf.RaggedTensor.from_row_lengths(x, edge_part, validate=self.ragged_validate) for x in out]
-                return out
-
-    def call(self, inputs, **kwargs):
-        r"""Forward pass.
-
-        Args:
-            inputs (list): [embeddings, tensor_index]
-
-                - embeddings (tf.RaggedTensor): Node embeddings of shape `(batch, [N], F)`
-                - tensor_index (tf.RaggedTensor): Edge indices referring to nodes of shape `(batch, [M], 2)`
-
-        Returns:
-            list: Gathered node embeddings matching the number of edges of shape `(batch, [M], F)` for selection_index.
-        """
-        # Old disjoint implementation that could be faster.
-        out = self._disjoint_implementation(inputs, **kwargs)
-        if out is not None:
-            return out
-
-        # For arbitrary gather from ragged tensor use tf.gather with batch_dims=1.
-        # Works in tf.__version__>=2.4
-        out = [tf.gather(inputs[0], tf.gather(inputs[1], i, axis=self.axis_indices), batch_dims=1, axis=self.axis) for i
-               in self.selection_index]
-        return out
+            selection_index = list(selection_index)
+        self.selection_index = selection_index
+        self.axis_indices = axis_indices
+        # Different names as in parent class.
+        super(GatherEmbeddingSelection, self).__init__(
+            axis=axis, concat_axis=None, split_axis=axis_indices, split_indices=self.selection_index, **kwargs)
 
     def get_config(self):
-        """Update layer config."""
         config = super(GatherEmbeddingSelection, self).get_config()
-        config.update({"axis": self.axis, "axis_indices": self.axis_indices, "selection_index": self.selection_index})
+        # Different names as in parent class.
+        for x in ["split_indices", "split_axis", "concat_axis"]:
+            config.pop(x)
+        config.update({"axis_indices": self.axis_indices, "selection_index": self.selection_index})
         return config
 
 
 GatherNodesSelection = GatherEmbeddingSelection
 
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='GatherNodesIngoing')
```

### Comparing `kgcnn-3.0.0/kgcnn/layers/geom.py` & `kgcnn-3.0.1/kgcnn/layers/geom.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/message.py` & `kgcnn-3.0.1/kgcnn/layers/message.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/mlp.py` & `kgcnn-3.0.1/kgcnn/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/modules.py` & `kgcnn-3.0.1/kgcnn/layers/modules.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/norm.py` & `kgcnn-3.0.1/kgcnn/layers/norm.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/pooling.py` & `kgcnn-3.0.1/kgcnn/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/relational.py` & `kgcnn-3.0.1/kgcnn/layers/relational.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/set2set.py` & `kgcnn-3.0.1/kgcnn/layers/set2set.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/layers/update.py` & `kgcnn-3.0.1/kgcnn/layers/update.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/AttentiveFP/_attentivefp_conv.py` & `kgcnn-3.0.1/kgcnn/literature/AttentiveFP/_attentivefp_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/AttentiveFP/_make.py` & `kgcnn-3.0.1/kgcnn/literature/AttentiveFP/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/CGCNN/_cgcnn_conv.py` & `kgcnn-3.0.1/kgcnn/literature/CGCNN/_cgcnn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/CGCNN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/CGCNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/CMPNN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/CMPNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/DGIN/_dgin_conv.py` & `kgcnn-3.0.1/kgcnn/literature/DGIN/_dgin_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/DGIN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/DGIN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/DMPNN/_dmpnn_conv.py` & `kgcnn-3.0.1/kgcnn/literature/DMPNN/_dmpnn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/DMPNN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/DMPNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/DimeNetPP/_dimenet_conv.py` & `kgcnn-3.0.1/kgcnn/literature/DimeNetPP/_dimenet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/DimeNetPP/_make.py` & `kgcnn-3.0.1/kgcnn/literature/DimeNetPP/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/EGNN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/EGNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GAT/_make.py` & `kgcnn-3.0.1/kgcnn/literature/GAT/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GATv2/_make.py` & `kgcnn-3.0.1/kgcnn/literature/GATv2/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GCN/_gcn_conv.py` & `kgcnn-3.0.1/kgcnn/literature/GCN/_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GCN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/GCN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GIN/_gin_conv.py` & `kgcnn-3.0.1/kgcnn/literature/GIN/_gin_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GIN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/GIN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_model.py` & `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_model.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py` & `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_base.py` & `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_testing.py` & `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_testing.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_utils.py` & `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_base.py` & `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_testing.py` & `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_testing.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_utils.py` & `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GNNFilm/_make.py` & `kgcnn-3.0.1/kgcnn/literature/GNNFilm/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/GraphSAGE/_make.py` & `kgcnn-3.0.1/kgcnn/literature/GraphSAGE/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_acsf_conv.py` & `kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_acsf_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_make.py` & `kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_wacsf_conv.py` & `kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_wacsf_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_hdnnp_conv.py` & `kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_hdnnp_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_make.py` & `kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_test_hdnnp.py` & `kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_test_hdnnp.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/HamNet/_hamnet_conv.py` & `kgcnn-3.0.1/kgcnn/literature/HamNet/_hamnet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/HamNet/_make.py` & `kgcnn-3.0.1/kgcnn/literature/HamNet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/INorp/_make.py` & `kgcnn-3.0.1/kgcnn/literature/INorp/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/MAT/_make.py` & `kgcnn-3.0.1/kgcnn/literature/MAT/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/MAT/_mat_conv.py` & `kgcnn-3.0.1/kgcnn/literature/MAT/_mat_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/MEGAN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/MEGAN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/MEGAN/_model.py` & `kgcnn-3.0.1/kgcnn/literature/MEGAN/_model.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/MEGAN/_test_literature_megan.py` & `kgcnn-3.0.1/kgcnn/literature/MEGAN/_test_literature_megan.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/MXMNet/_make.py` & `kgcnn-3.0.1/kgcnn/literature/MXMNet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/MXMNet/_mxmnet_conv.py` & `kgcnn-3.0.1/kgcnn/literature/MXMNet/_mxmnet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/Megnet/_make.py` & `kgcnn-3.0.1/kgcnn/literature/Megnet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/Megnet/_megnet_conv.py` & `kgcnn-3.0.1/kgcnn/literature/Megnet/_megnet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/MoGAT/_make.py` & `kgcnn-3.0.1/kgcnn/literature/MoGAT/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/MoGAT/_mogat_conv.py` & `kgcnn-3.0.1/kgcnn/literature/MoGAT/_mogat_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/NMPN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/NMPN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/NMPN/_mpnn_conv.py` & `kgcnn-3.0.1/kgcnn/literature/NMPN/_mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/PAiNN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/PAiNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/PAiNN/_painn_conv.py` & `kgcnn-3.0.1/kgcnn/literature/PAiNN/_painn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/RGCN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/RGCN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/Schnet/_make.py` & `kgcnn-3.0.1/kgcnn/literature/Schnet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/Schnet/_schnet_conv.py` & `kgcnn-3.0.1/kgcnn/literature/Schnet/_schnet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/Unet/_make.py` & `kgcnn-3.0.1/kgcnn/literature/Unet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/Unet/_test_connect.py` & `kgcnn-3.0.1/kgcnn/literature/Unet/_test_connect.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/Unet/_test_topk.py` & `kgcnn-3.0.1/kgcnn/literature/Unet/_test_topk.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/Unet/_topk.py` & `kgcnn-3.0.1/kgcnn/literature/Unet/_topk.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/__init__.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 from ._coGN_config import (model_default, crystal_asymmetric_unit_graphs, molecular_graphs, crystal_unit_graphs,
                            crystal_unit_graphs_coord_input, molecular_graphs_coord_input)
 from ._coNGN_config import model_default_nested
 
 
 __all__ = [
     "make_model",
-    "make_force_model"
+    "make_force_model",
     "model_default",
     "crystal_asymmetric_unit_graphs",
     "crystal_unit_graphs",
     "crystal_unit_graphs_coord_input",
     "molecular_graphs",
     "molecular_graphs_coord_input",
     "model_default_nested"
```

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_coGN_config.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_coGN_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,15 @@
                     'multiplicity_readout': True}
 
 output_block_cfg_no_multiplicity = deepcopy(output_block_cfg)
 output_block_cfg_no_multiplicity['multiplicity_readout'] = False
 
 
 crystal_asymmetric_unit_graphs = {
+    "name": "coGN",
     "inputs": {
         "offset": {"shape": (None, 3), "name": "offset", "dtype": "float32", "ragged": True},
         "cell_translation": None,
         "affine_matrix": None,
         "voronoi_ridge_area": None,
         "atomic_number": {"shape": (None,), "name": "atomic_number", "dtype": "int32", "ragged": True},
         "frac_coords": None,
@@ -91,14 +92,15 @@
     },
     "input_block_cfg": input_block_cfg,
     "processing_blocks_cfg": [deepcopy(processing_block_cfg) for _ in range(depth)],
     "output_block_cfg": output_block_cfg,
 }
 
 crystal_unit_graphs = {
+    "name": "coGN",
     "inputs": {
         "offset": {"shape": (None, 3), "name": "offset", "dtype": "float32", "ragged": True},
         "cell_translation": None,
         "affine_matrix": None,
         "voronoi_ridge_area": None,
         "atomic_number": {"shape": (None,), "name": "atomic_number", "dtype": "int32", "ragged": True},
         "frac_coords": None,
@@ -111,14 +113,15 @@
     "input_block_cfg": input_block_cfg,
     "processing_blocks_cfg": [deepcopy(processing_block_cfg) for _ in range(depth)],
     "output_block_cfg": output_block_cfg_no_multiplicity,
 }
 molecular_graphs = crystal_unit_graphs
 
 crystal_unit_graphs_coord_input = {
+    "name": "coGN",
     "inputs": {
         "offset": None,
         "cell_translation": {"shape": (None,3), "dtype": "float32", "name": "cell_translation", "ragged": True},
         "affine_matrix": None,
         "voronoi_ridge_area": None,
         "atomic_number": {"shape": (None,), "name": "atomic_number", "dtype": "int32", "ragged": True},
         "frac_coords": {"shape": (None,3), "dtype": "float32", "name": "frac_coords", "ragged": True},
@@ -143,13 +146,14 @@
         "frac_coords": None,
         "coords": {"shape": (None,3), "dtype": "float32", "name": "coords", "ragged": True},
         "multiplicity": None,
         "lattice_matrix": None,
         "edge_indices": {"shape": (None, 2), "name": "edge_indices", "dtype": "int32", "ragged": True},
         "line_graph_edge_indices": None,
     },
+    "name": "coGN",
     "input_block_cfg": input_block_cfg,
     "processing_blocks_cfg": [deepcopy(processing_block_cfg) for _ in range(depth)],
     "output_block_cfg": output_block_cfg_no_multiplicity,
 }
 
 model_default = crystal_asymmetric_unit_graphs
```

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_coNGN_config.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_coNGN_config.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_gates.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_gates.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/graph_network_base.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/graph_network_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/graph_networks.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/graph_networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 from kgcnn.layers.base import GraphBaseLayer
-from kgcnn.layers.modules import LazyMultiply, LazyAdd
+from kgcnn.layers.modules import LazyMultiply, LazyAdd, LazyConcatenate
 from kgcnn.layers.gather import GatherState
 from kgcnn.ops.segment import segment_ops_by_name
 
 from .graph_network_base import GraphNetworkBase
 
 class GraphNetwork(GraphNetworkBase):
     """A basic concrete implementation of the GraphNetworkBase class.
@@ -101,14 +101,15 @@
 
         self.edge_gate = edge_gate
         self.node_gate = node_gate
         self.global_gate = global_gate
         self.node_mlp = node_mlp
         self.global_mlp = global_mlp
         self.lazy_add = LazyAdd()
+        self.lazy_concat = LazyConcatenate(axis=-1)
         self.lazy_multiply = LazyMultiply()
         self.gather_state = GatherState()
             
     def update_edges(self, edges, nodes_in, nodes_out, globals_, **kwargs):
 
         if self.edge_mlp is None:
             return edges
@@ -123,15 +124,15 @@
         if self.update_edges_input[2]:
             nodes_out_features = self.get_features(nodes_out)
             features_to_concat.append(nodes_out_features)
         if self.update_edges_input[3]:
             global_features = self.get_features(globals_)
             features_to_concat.append(self.gather_state([global_features, edge_features]))
         
-        concat_features = tf.concat(features_to_concat, axis=-1)
+        concat_features = self.lazy_concat(features_to_concat)
         messages = self.edge_mlp(concat_features)
 
         if self.edge_gate is not None:
             messages = tf.RaggedTensor.from_row_splits(
                     self.edge_gate(messages.values, edge_features.values)[1],
                     messages.row_splits)
         
@@ -162,21 +163,21 @@
             features_to_concat.append(aggregated_edge_features)
         if self.update_nodes_input[1]:
             features_to_concat.append(node_features)
         if self.update_nodes_input[2]:
             global_features = self.get_features(globals_)
             features_to_concat.append(self.gather_state([global_features, node_features]))
         
-        concat_features = tf.concat(features_to_concat, axis=-1)
+        concat_features = self.lazy_concat(features_to_concat)
         node_features_new = self.node_mlp(concat_features)
 
         if self.node_gate is not None:
             node_features_new = tf.RaggedTensor.from_row_splits(
                     self.node_gate(node_features_new.values, node_features.values)[1],
-                    node_features_new.row_splits)
+                    node_features_new.row_splits, validate=self.ragged_validate)
 
         if self.residual_node_update:
             node_features_new = self.lazy_add([node_features, node_features_new])
         
         nodes_new = self.update_features(nodes, node_features_new)
         
         if self.aggregate_nodes_ in self.attention_strings:
@@ -196,21 +197,21 @@
         if self.update_global_input[1]:
             aggregated_node_features = self.get_features(aggregated_nodes)
             features_to_concat.append(aggregated_node_features)
         if self.update_global_input[2]:
             global_features = self.get_features(globals_)
             features_to_concat.append(global_features)
 
-        concat_features = tf.concat(features_to_concat, axis=-1)
+        concat_features = self.lazy_concat(features_to_concat)
         global_features_new = self.global_mlp(concat_features)
 
         if self.global_gate is not None:
             global_features_new = tf.RaggedTensor.from_row_splits(
                     self.global_gate(global_features_new.values, global_features.values)[1],
-                    global_features_new.row_splits)
+                    global_features_new.row_splits, validate=self.ragged_validate)
 
         if self.residual_global_update:
             global_features = self.get_features(globals_)
             global_features_new = self.lazy_add([global_features, global_features_new])
 
         globals_new = self.update_features(globals_, global_features_new)
 
@@ -310,14 +311,15 @@
                 normalization_factor = self.get_multiplicity_normalization_factor(multiplicity)
                 aggregated_node_features_ = self.get_features(aggregated_node_features) * normalization_factor
                 aggregated_node_features = self.update_features(nodes, aggregated_node_features_)
             return aggregated_node_features
         else:
             return super().aggregate_nodes(nodes, **kwargs)
 
+
 class CrystalInputBlock(GraphNetworkBase):
     """Graph Network layer that embeds node and edges features of crystal graphs on the basis of atomic numbers (for nodes) and distances (for edges)."""
 
     def __init__(self,
             atom_embedding,
             edge_embedding,
             atom_mlp=None,
@@ -434,15 +436,15 @@
         if self.update_edges_input[2]:
             nodes_out_features = self.get_features(nodes_out)
             features_to_concat.append(nodes_out_features)
         if self.update_edges_input[3]:
             global_features = self.get_features(globals_)
             features_to_concat.append(self.gather_state([global_features, edge_features]))
         
-        concat_features = tf.concat(features_to_concat, axis=-1)
+        concat_features = self.lazy_concat(features_to_concat)
         messages = self.edge_mlp(concat_features)
 
         assert isinstance(globals_, dict)
         assert 'line_graph_edge_indices' in globals_.keys()
         line_graph_edge_indices = globals_['line_graph_edge_indices']
 
         if 'line_graph_edges' in globals_.keys():
```

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_make.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 from kgcnn.model.utils import update_model_kwargs
 from tensorflow.keras.layers import GRUCell, LSTMCell
 from ._coGN_config import model_default
 from ._preprocessing_layers import EdgeDisplacementVectorDecoder
 
 ks = tf.keras
 
+
 @update_model_kwargs(model_default)
 def make_model(inputs=None,
+               name=None,
                input_block_cfg=None,
                processing_blocks_cfg=None,
                output_block_cfg=None,):
     r"""Make connectivity optimized graph networks for crystals.
 
     Args:
         inputs (list): List of inputs kwargs.
@@ -119,15 +121,15 @@
     x = sequential_gn([edge_features, node_features, global_input, edge_indices])
     _, _, out, _ = output_block(x)
     out = output_block.get_features(out)
 
     input_list = edge_inputs + node_inputs + global_inputs + [edge_indices]
     print(input_list)
 
-    return ks.Model(inputs=input_list, outputs=out)
+    return ks.Model(inputs=input_list, outputs=out, name=name)
 
 
 def make_force_model(inner_model):
     r"""Transforms a model that predicts energies for geometric crystal/molecular graphs,
     into a model that predicts energies as well as forces on each node in the graph.
 
     Depending on the detected input names either :python:`make_molecule_force_model`
@@ -154,14 +156,16 @@
 
     Args:
         inner_model (tf.keras.models.Model): A model that predicts energies for geometric molecular graphs.
 
     Returns:
         :obj:`tf.keras.models.Model`
     """
+    # if isinstance(inner_model, dict):
+    #      inner_model = make_model(inner_model)
     input_names = [layer.name for layer in inner_model.inputs]
     if 'coords' in input_names:
         return make_molecule_force_model(inner_model)
     elif 'frac_coords' in input_names and 'lattice_matrix' in input_names:
         return make_crystal_force_model(inner_model)
     else:
         raise ValueError("""Can not create force model from given energy model.
@@ -179,14 +183,16 @@
 
     Args:
         inner_model (tf.keras.models.Model): A model that predicts energies for geometric molecular graphs.
 
     Returns:
         :obj:`tf.keras.models.Model`
     """
+    # if isinstance(inner_model, dict):
+    #      inner_model = make_model(inner_model)
     force_model_inputs = []
 
     for i, input_layer in enumerate(inner_model.inputs):
         if input_layer.name == 'coords':
             coordinate_input = i
             coords_input_layer_exists = True
         new_input_layer = ks.Input(type_spec=input_layer.type_spec, name=input_layer.name)
@@ -237,15 +243,15 @@
         force_model_inputs.append(new_input_layer)
 
     assert frac_coords_input_layer_exists
     assert lattice_matrix_input_layer_exists
 
     # Create force model
     force_model = EnergyForceModel(inner_model, coordinate_input=coordinate_input,
-                                    output_to_tensor=False, output_squeeze_states=True)
+                                   output_to_tensor=False, output_squeeze_states=True)
     outputs = force_model(force_model_inputs)
     # Since coordinates are fractional, force predictions are also fractional.
     # Convert fractional to real forces:
     frac_to_real = FracToRealCoordinates()
     outputs['force'] = frac_to_real([outputs['force'], lattice_matrix])
 
     return ks.models.Model(inputs=force_model_inputs, outputs=outputs)
```

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_multiplicity_readout.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_multiplicity_readout.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/coGN/_preprocessing_layers.py` & `kgcnn-3.0.1/kgcnn/literature/coGN/_preprocessing_layers.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/literature/rGIN/_make.py` & `kgcnn-3.0.1/kgcnn/literature/rGIN/_make.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,26 +43,26 @@
                dropout: float = None,
                name: str = None,
                verbose: int = None,
                output_embedding: str = None,
                output_to_tensor: bool = None,
                output_mlp: dict = None
                ):
-    r"""Make `rGIN https://arxiv.org/abs/2002.03155`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.rGIN.model_default`.
+    r"""Make `rGIN <https://arxiv.org/abs/2002.03155>`__ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.rGIN.model_default` .
 
     Inputs:
         list: `[node_attributes, edge_indices]`
 
             - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
               using an embedding layer.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)` .
 
     Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"` .
 
     Args:
         inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
         input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
         depth (int): Number of graph embedding units or depth of the network.
         rgin_args (dict): Dictionary of layer arguments unpacked in :obj:`GIN` convolutional layer.
         gin_mlp (dict): Dictionary of layer arguments unpacked in :obj:`MLP` for convolutional layer.
```

### Comparing `kgcnn-3.0.0/kgcnn/literature/rGIN/_rgin_conv.py` & `kgcnn-3.0.1/kgcnn/literature/rGIN/_rgin_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from kgcnn.layers.pooling import PoolingLocalEdges
 from kgcnn.layers.modules import LazyAdd, Activation, LazyConcatenate
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='rGIN')
 class rGIN(GraphBaseLayer):
     r"""Random Features Strengthen Graph Neural Networks
-    <https://arxiv.org/abs/2002.03155>`_.
+    <https://arxiv.org/abs/2002.03155>`__ .
 
     Computes graph convolution at step :math:`k` for node embeddings :math:`h_\nu` as:
 
     .. math::
         h_\nu^{(k)} = \phi^{(k)} ((1+\epsilon^{(k)}) h_\nu^{k-1} + \sum_{u\in N(\nu)}) h_u^{k-1}.
 
     with optional learnable :math:`\epsilon^{(k)}`
```

### Comparing `kgcnn-3.0.0/kgcnn/metrics/loss.py` & `kgcnn-3.0.1/kgcnn/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/metrics/metrics.py` & `kgcnn-3.0.1/kgcnn/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/model/force.py` & `kgcnn-3.0.1/kgcnn/model/force.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/model/utils.py` & `kgcnn-3.0.1/kgcnn/model/utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/molecule/base.py` & `kgcnn-3.0.1/kgcnn/molecule/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/molecule/convert.py` & `kgcnn-3.0.1/kgcnn/molecule/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,43 +12,51 @@
 
 # RDkit
 try:
     import rdkit
     import rdkit.Chem
     import rdkit.Chem.AllChem
     import rdkit.Chem.rdDetermineBonds
+    from rdkit import RDLogger
 
     def rdkit_smile_to_mol(smile: str, sanitize: bool = True, add_hydrogen: bool = True, make_conformers: bool = True,
-                           optimize_conformer: bool = True):
+                           optimize_conformer: bool = True, random_seed: int = 42, stop_logging: bool = False):
         # Order of parameters is important here.
+        if stop_logging:
+            RDLogger.DisableLog('rdApp.*')
+
         try:
             m = rdkit.Chem.MolFromSmiles(smile)
             if sanitize:
                 rdkit.Chem.SanitizeMol(m)
 
             m = rdkit.Chem.AddHs(m)
             m.SetProp("_Name", smile.strip())
 
             if make_conformers:
                 params = rdkit.Chem.AllChem.ETKDGv3()
                 params.useSmallRingTorsions = True
+                params.randomSeed = random_seed
                 # params.useRandomCoords = True
                 success = rdkit.Chem.AllChem.EmbedMolecule(m, params=params)
                 if optimize_conformer:
                     rdkit.Chem.AllChem.MMFFOptimizeMolecule(m)
                     rdkit.Chem.AssignAtomChiralTagsFromStructure(m)
                     rdkit.Chem.AssignStereochemistryFrom3D(m)
             if not add_hydrogen:
                 m = rdkit.Chem.RemoveHs(m)
 
             rdkit.Chem.AssignStereochemistry(m)
 
         except:
             m = None
 
+        if stop_logging:
+            RDLogger.EnableLog('rdApp.*')
+
         if m is not None:
             return rdkit.Chem.MolToMolBlock(m)
 
         return None
 
     def rdkit_xyz_to_mol(xyz_string: str, charge = 0):
         """Convert xyz-string to mol-string.
@@ -85,14 +93,15 @@
     if "BABEL_DATADIR" not in os.environ:
         module_logger.warning(
             "In case openbabel fails, you can set `kgcnn.mol.convert.openbabel_smile_to_mol` to `None` for disable.")
 
 
     def openbabel_smile_to_mol(smile: str, sanitize: bool = True, add_hydrogen: bool = True,
                                make_conformers: bool = True, optimize_conformer: bool = True,
+                               random_seed: int = 42,
                                stop_logging: bool = False):
         if stop_logging:
             openbabel.obErrorLog.StopLogging()
 
         try:
             m = openbabel.OBMol()
             ob_conversion = openbabel.OBConversion()
@@ -177,15 +186,15 @@
 
         if base_path is None:
             self.base_path = os.path.realpath(__file__)
 
     @staticmethod
     def _check_is_same_length(a, b):
         if len(a) != len(b):
-            module_logger.error("Mismatch in number of converted. Found '%s' vs. '%s'" % (len(a), len(b)))
+            module_logger.error("Mismatch in number of converted. Found '%s' vs. '%s'." % (len(a), len(b)))
             raise ValueError("Conversion was not successful")
 
     @staticmethod
     def _convert_parallel(conversion_method: Callable, smile_list: list, num_workers: int, *args):
         if num_workers is None:
             num_workers = os.cpu_count()
 
@@ -302,15 +311,15 @@
         """
         if openbabel_xyz_to_mol is None and rdkit_xyz_to_mol is None:
             raise ModuleNotFoundError("Can not convert XYZ to SDF format, missing package `OpenBabel` or `RDkit`.")
 
         xyz_list = read_xyz_file(xyz_path)
         mol_list = []
         for x in xyz_list:
-            xyz_str = parse_list_to_xyz_str(x)
+            xyz_str = parse_list_to_xyz_str(x, number_coordinates=3)
             # No parallel conversion here, not necessary.
             mol_str = self._single_xyz_to_mol(xyz_str, charge=0)
             mol_list.append(mol_str)
         self._check_is_same_length(xyz_list, mol_list)
         if sdf_path is not None:
             write_mol_block_list_to_sdf(mol_list, sdf_path)
         return mol_list
```

### Comparing `kgcnn-3.0.0/kgcnn/molecule/dynamics/ase_calc.py` & `kgcnn-3.0.1/kgcnn/molecule/dynamics/ase_calc.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/molecule/dynamics/base.py` & `kgcnn-3.0.1/kgcnn/molecule/dynamics/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/molecule/encoder.py` & `kgcnn-3.0.1/kgcnn/molecule/encoder.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/molecule/external/ballloon.py` & `kgcnn-3.0.1/kgcnn/molecule/external/ballloon.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/molecule/graph_babel.py` & `kgcnn-3.0.1/kgcnn/molecule/graph_babel.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/molecule/graph_rdkit.py` & `kgcnn-3.0.1/kgcnn/molecule/graph_rdkit.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/molecule/io.py` & `kgcnn-3.0.1/kgcnn/molecule/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import logging
 
 
-def parse_list_to_xyz_str(mol: list, comment: str = ""):
+def parse_list_to_xyz_str(mol: list, comment: str = "", number_coordinates: int = None):
     """Convert list of atom and coordinates list into xyz-string.
 
     Args:
         mol (list): Tuple or list of `[['C', 'H', ...], [[0.0, 0.0, 0.0], [1.0, 1.0, 1.0], ... ]]`.
         comment (str): Comment for comment line in xyz string. Default is "".
+        number_coordinates (int): Number of allowed coordinates.
 
     Returns:
         str: Information in xyz-string format.
     """
     atoms = mol[0]
     coordinates = mol[1]
     if len(atoms) != len(coordinates):
         raise ValueError("Number of atoms does not match number of coordinates for xyz string.")
     xyz_str = str(int(len(atoms))) + "\n"
     if "\n" in comment:
         raise ValueError("Line break must not be in the comment line for xyz string.")
     xyz_str = xyz_str + comment + "\n"
     for a_iter, c_iter in zip(atoms, coordinates):
         _at_str = str(a_iter)
+        if number_coordinates is not None:
+            c_iter = c_iter[:number_coordinates]
         _c_format_str = " {:.10f}" * len(c_iter) + "\n"
         xyz_str = xyz_str + _at_str + _c_format_str.format(*c_iter)
     return xyz_str
 
 
 def write_list_to_xyz_file(filepath: str, mol_list: list):
     """Write a list of nested list of atom and coordinates into xyz-string. Uses :obj:`parse_list_to_xyz_str`.
```

### Comparing `kgcnn-3.0.0/kgcnn/molecule/methods.py` & `kgcnn-3.0.1/kgcnn/molecule/methods.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/molecule/serial.py` & `kgcnn-3.0.1/kgcnn/molecule/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/ops/activ.py` & `kgcnn-3.0.1/kgcnn/ops/activ.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/ops/axis.py` & `kgcnn-3.0.1/kgcnn/ops/axis.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/ops/initializer.py` & `kgcnn-3.0.1/kgcnn/ops/initializer.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/ops/partition.py` & `kgcnn-3.0.1/kgcnn/ops/partition.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/ops/polynom.py` & `kgcnn-3.0.1/kgcnn/ops/polynom.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/ops/ragged.py` & `kgcnn-3.0.1/kgcnn/ops/ragged.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/ops/scatter.py` & `kgcnn-3.0.1/kgcnn/ops/scatter.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/ops/segment.py` & `kgcnn-3.0.1/kgcnn/ops/segment.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/training/callbacks.py` & `kgcnn-3.0.1/kgcnn/training/callbacks.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/training/history.py` & `kgcnn-3.0.1/kgcnn/training/history.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/training/hyper.py` & `kgcnn-3.0.1/kgcnn/training/hyper.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/training/optimizer.py` & `kgcnn-3.0.1/kgcnn/training/optimizer.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/training/schedule.py` & `kgcnn-3.0.1/kgcnn/training/schedule.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import tensorflow as tf
 
+ks = tf.keras
 
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='LinearWarmupExponentialDecay')
+
+@ks.utils.register_keras_serializable(package='kgcnn', name='LinearWarmupExponentialDecay')
 class LinearWarmupExponentialDecay(tf.optimizers.schedules.LearningRateSchedule):
     r"""This schedule combines a linear warmup with an exponential decay.
     Combines :obj:` tf.optimizers.schedules.PolynomialDecay` with an actual increase during warmup
     and :obj:`tf.optimizers.schedules.ExponentialDecay` after.
 
     Introduced by `DimeNetPP <https://arxiv.org/abs/2011.14115>`__ .
 
@@ -59,7 +61,35 @@
         self.decay.initial_learning_rate = value
 
     def get_config(self):
         """Get config for this class."""
         config = {}
         config.update(self._input_config_settings)
         return config
+
+
+@ks.utils.register_keras_serializable(package='kgcnn', name='KerasPolynomialDecaySchedule')
+class KerasPolynomialDecaySchedule(ks.optimizers.schedules.PolynomialDecay):
+    r"""This schedule extends :obj:` tf.optimizers.schedules.PolynomialDecay` ."""
+
+    def __init__(self, dataset_size: int, batch_size: int, epochs: int, lr_start: float = 0.0005,
+                 lr_stop: float = 1e-5):
+        """Initialize class.
+
+        Args:
+            dataset_size (int): Size of the dataset.
+            batch_size (int): Batch size for training.
+            epochs (int): Total epochs to run schedule on.
+            lr_start (int): Learning rate at the start.
+            lr_stop (int): Final learning rate.
+        """
+        self._input_config_settings = {"lr_start": lr_start, "lr_stop": lr_stop,
+                                       "epochs": epochs, "batch_size": batch_size, "dataset_size": dataset_size}
+        steps_per_epoch = dataset_size / batch_size
+        num_steps = epochs * steps_per_epoch
+        super().__init__(initial_learning_rate=lr_start, decay_steps=num_steps, end_learning_rate=lr_stop)
+
+    def get_config(self):
+        """Get config for this class."""
+        config = {}
+        config.update(self._input_config_settings)
+        return config
```

### Comparing `kgcnn-3.0.0/kgcnn/training/scheduler.py` & `kgcnn-3.0.1/kgcnn/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/utils/devices.py` & `kgcnn-3.0.1/kgcnn/utils/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         module_logger.warning("No cuda support")
         module_logger.warning("Can not set GPU")
         return
 
     try:
         gpus = tf.config.list_physical_devices('GPU')
     except:
-        module_logger.error("Can not get device list, do nothing")
+        module_logger.error("Can not get device list, do nothing.")
         return
 
     if isinstance(gpus, list):
         if len(gpus) <= 0:
             module_logger.warning("No devices found")
             module_logger.warning("Can not set GPU")
             return
```

### Comparing `kgcnn-3.0.0/kgcnn/utils/plots.py` & `kgcnn-3.0.1/kgcnn/utils/plots.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/kgcnn/utils/serial.py` & `kgcnn-3.0.1/kgcnn/utils/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,9 +59,9 @@
         else:
             # Try setting them manually.
             for method_item in method_list:
                 for method, kwargs in method_item.items():
                     if hasattr(obj, method):
                         getattr(obj, method)(**kwargs)
                     else:
-                        logging.error("Class for deserialization does not have method %s" % method)
+                        logging.error("Class for deserialization does not have method '%s'." % method)
     return obj
```

### Comparing `kgcnn-3.0.0/kgcnn.egg-info/PKG-INFO` & `kgcnn-3.0.1/kgcnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgcnn
-Version: 3.0.0
+Version: 3.0.1
 Summary: General Base Layers for Graph Convolutions with tensorflow.keras
 Home-page: https://github.com/aimat-lab/gcnn_keras
 Author: Patrick Reiser
 Author-email: patrick.reiser@kit.edu
 License: UNKNOWN
 Keywords: materials,science,machine,learning,deep,graph,networks,neural
 Platform: UNKNOWN
```

### Comparing `kgcnn-3.0.0/kgcnn.egg-info/SOURCES.txt` & `kgcnn-3.0.1/kgcnn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 kgcnn.egg-info/requires.txt
 kgcnn.egg-info/top_level.txt
 kgcnn/crystal/__init__.py
 kgcnn/crystal/base.py
 kgcnn/crystal/graph_builder.py
 kgcnn/crystal/preprocessor.py
 kgcnn/crystal/periodic_table/__init__.py
+kgcnn/crystal/periodic_table/periodic_table.csv
 kgcnn/crystal/periodic_table/periodic_table.py
 kgcnn/data/__init__.py
 kgcnn/data/base.py
 kgcnn/data/crystal.py
 kgcnn/data/download.py
 kgcnn/data/moleculenet.py
 kgcnn/data/qm.py
@@ -67,17 +68,16 @@
 kgcnn/graph/base.py
 kgcnn/graph/postprocessor.py
 kgcnn/graph/preprocessor.py
 kgcnn/graph/serial.py
 kgcnn/graph/methods/__init__.py
 kgcnn/graph/methods/_adj.py
 kgcnn/graph/methods/_geom.py
-kgcnn/hyper/__init__.py
-kgcnn/hyper/hyper.py
 kgcnn/io/__init__.py
+kgcnn/io/file.py
 kgcnn/io/loader.py
 kgcnn/layers/README.md
 kgcnn/layers/__init__.py
 kgcnn/layers/attention.py
 kgcnn/layers/base.py
 kgcnn/layers/casting.py
 kgcnn/layers/conv.py
@@ -184,14 +184,15 @@
 kgcnn/literature/coGN/__init__.py
 kgcnn/literature/coGN/_coGN_config.py
 kgcnn/literature/coGN/_coNGN_config.py
 kgcnn/literature/coGN/_gates.py
 kgcnn/literature/coGN/_make.py
 kgcnn/literature/coGN/_multiplicity_readout.py
 kgcnn/literature/coGN/_preprocessing_layers.py
+kgcnn/literature/coGN/_test.py
 kgcnn/literature/coGN/_utils.py
 kgcnn/literature/coGN/_embedding_layers/__init__.py
 kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py
 kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py
 kgcnn/literature/coGN/_graph_network/__init__.py
 kgcnn/literature/coGN/_graph_network/graph_network_base.py
 kgcnn/literature/coGN/_graph_network/graph_networks.py
@@ -202,28 +203,14 @@
 kgcnn/metrics/loss.py
 kgcnn/metrics/metrics.py
 kgcnn/model/README.md
 kgcnn/model/__init__.py
 kgcnn/model/force.py
 kgcnn/model/serial.py
 kgcnn/model/utils.py
-kgcnn/mol/__init__.py
-kgcnn/mol/base.py
-kgcnn/mol/convert.py
-kgcnn/mol/encoder.py
-kgcnn/mol/graph_babel.py
-kgcnn/mol/graph_rdkit.py
-kgcnn/mol/io.py
-kgcnn/mol/methods.py
-kgcnn/mol/serial.py
-kgcnn/mol/external/__init__.py
-kgcnn/mol/external/ballloon.py
-kgcnn/moldyn/__init__.py
-kgcnn/moldyn/ase_calc.py
-kgcnn/moldyn/base.py
 kgcnn/molecule/__init__.py
 kgcnn/molecule/base.py
 kgcnn/molecule/convert.py
 kgcnn/molecule/encoder.py
 kgcnn/molecule/graph_babel.py
 kgcnn/molecule/graph_rdkit.py
 kgcnn/molecule/io.py
```

### Comparing `kgcnn-3.0.0/setup.py` & `kgcnn-3.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name="kgcnn",
-    version="3.0.0",  # If version is updated, change version in `kgcnn.__init__` too. (and update changelog)
+    version="3.0.1",  # If version is updated, change version in `kgcnn.__init__` too. (and update changelog)
     author="Patrick Reiser",
     author_email="patrick.reiser@kit.edu",
     description="General Base Layers for Graph Convolutions with tensorflow.keras",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aimat-lab/gcnn_keras",
     install_requires=[
@@ -27,22 +27,23 @@
         "requests>=2.28.1",
         "networkx>=2.8.8",
         "sympy>=1.11.1",
         "pyyaml>=6.0",
         "ase>=3.22.1",
         "click>=7.1.2",
         "brotli>=1.0.9",
-        "pyxtal>=0.5.5"
+        "pyxtal>=0.5.5",
+        "h5py"
     ],
     extras_require={
         "openbabel": ["openbabel"],
     },
     packages=find_packages(),
     include_package_data=True,
-    package_data={"kgcnn": ["*.json", "*.yaml", "*.csv"]},
+    package_data={"kgcnn": ["*.json", "*.yaml", "*.csv", "*.md"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Chemistry",
```

### Comparing `kgcnn-3.0.0/test/test_data_base.py` & `kgcnn-3.0.1/test/test_data_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/test/test_data_moleculenet.py` & `kgcnn-3.0.1/test/test_data_moleculenet.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/test/test_graph_base.py` & `kgcnn-3.0.1/test/test_graph_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/test/test_graph_methods.py` & `kgcnn-3.0.1/test/test_graph_methods.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/test/test_layers_attention.py` & `kgcnn-3.0.1/test/test_layers_attention.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/test/test_layers_gather.py` & `kgcnn-3.0.1/test/test_layers_gather.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/test/test_layers_geom.py` & `kgcnn-3.0.1/test/test_layers_geom.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/test/test_layers_pooling.py` & `kgcnn-3.0.1/test/test_layers_pooling.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.0/test/test_range_periodic.py` & `kgcnn-3.0.1/test/test_range_periodic.py`

 * *Files identical despite different names*

