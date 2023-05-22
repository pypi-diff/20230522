# Comparing `tmp/mlfactory-0.0.2.tar.gz` & `tmp/mlfactory-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfactory-0.0.2.tar", last modified: Sun May 14 18:12:53 2023, max compression
+gzip compressed data, was "mlfactory-0.0.3.tar", last modified: Mon May 22 13:29:58 2023, max compression
```

## Comparing `mlfactory-0.0.2.tar` & `mlfactory-0.0.3.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.278678 mlfactory-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1418 2023-05-14 18:12:53.278678 mlfactory-0.0.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      879 2023-05-14 18:12:13.000000 mlfactory-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.258678 mlfactory-0.0.2/mlfactory/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 17:49:33.000000 mlfactory-0.0.2/mlfactory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.262678 mlfactory-0.0.2/mlfactory/applications/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/applications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.262678 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15529 2023-04-26 14:00:26.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/main.py
--rw-r--r--   0 root         (0) root         (0)     1785 2023-04-21 14:15:08.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/read_video.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.262678 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7012 2023-03-24 18:19:17.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py
--rw-r--r--   0 root         (0) root         (0)     2502 2023-03-19 11:53:53.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-03-24 18:22:37.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     8391 2023-03-24 16:41:20.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py
--rw-r--r--   0 root         (0) root         (0)     1324 2022-08-18 10:40:00.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py
--rw-r--r--   0 root         (0) root         (0)     4761 2023-04-21 14:19:44.000000 mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.262678 mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2947 2023-04-20 19:13:46.000000 mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-04-02 23:52:08.000000 mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/datahandler.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-04-02 23:52:08.000000 mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/main.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-04-02 23:52:08.000000 mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/model.py
--rw-r--r--   0 root         (0) root         (0)     5507 2023-04-02 23:52:08.000000 mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/segdataset.py
--rw-r--r--   0 root         (0) root         (0)     6809 2023-04-20 20:15:23.000000 mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/test.py
--rw-r--r--   0 root         (0) root         (0)     3578 2023-04-02 23:52:08.000000 mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.266678 mlfactory-0.0.2/mlfactory/applications/superglue_inference/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/applications/superglue_inference/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8134 2023-04-16 21:03:54.000000 mlfactory-0.0.2/mlfactory/applications/superglue_inference/match_pair.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.266678 mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/
--rw-r--r--   0 root         (0) root         (0)        0 2022-10-07 16:11:34.000000 mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3417 2022-10-07 16:11:34.000000 mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/matching.py
--rw-r--r--   0 root         (0) root         (0)    11781 2022-10-07 16:11:34.000000 mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/superglue.py
--rw-r--r--   0 root         (0) root         (0)     8142 2022-10-07 16:11:34.000000 mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/superpoint.py
--rw-r--r--   0 root         (0) root         (0)    20039 2022-10-07 16:11:34.000000 mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.266678 mlfactory-0.0.2/mlfactory/custom_losses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/custom_losses/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.266678 mlfactory-0.0.2/mlfactory/custom_losses/pytorch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/custom_losses/pytorch/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4036 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/custom_losses/pytorch/depth.py
--rw-r--r--   0 root         (0) root         (0)     1448 2022-10-05 16:29:32.000000 mlfactory-0.0.2/mlfactory/custom_losses/pytorch/pointnetloss.py
--rwxr-xr-x   0 root         (0) root         (0)      190 2023-04-15 14:33:36.000000 mlfactory-0.0.2/mlfactory/custom_losses/pytorch/regress.py
--rwxr-xr-x   0 root         (0) root         (0)      957 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/custom_losses/pytorch/segment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.266678 mlfactory-0.0.2/mlfactory/custom_losses/tensorflow/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/custom_losses/tensorflow/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1445 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/custom_losses/tensorflow/feature_detect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.266678 mlfactory-0.0.2/mlfactory/datacreators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/datacreators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.270678 mlfactory-0.0.2/mlfactory/datacreators/ai2thor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/datacreators/ai2thor/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7962 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/datacreators/ai2thor/create_dataset.py
--rwxr-xr-x   0 root         (0) root         (0)     5970 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/datacreators/ai2thor/register_pcds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.270678 mlfactory-0.0.2/mlfactory/datacreators/lidar_contours/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/datacreators/lidar_contours/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6484 2022-11-05 15:28:48.000000 mlfactory-0.0.2/mlfactory/datacreators/lidar_contours/human_contours.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.270678 mlfactory-0.0.2/mlfactory/datacreators/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/datacreators/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-14 17:50:57.000000 mlfactory-0.0.2/mlfactory/datacreators/utils/colab_poly_anot.py
--rwxr-xr-x   0 root         (0) root         (0)    10241 2022-11-04 20:33:18.000000 mlfactory-0.0.2/mlfactory/datacreators/utils/cv_annotator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.274678 mlfactory-0.0.2/mlfactory/dataloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/dataloaders/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    11455 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/dataloaders/ade20k.py
--rwxr-xr-x   0 root         (0) root         (0)     3651 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/dataloaders/cihp.py
--rwxr-xr-x   0 root         (0) root         (0)     9524 2023-04-13 01:43:27.000000 mlfactory-0.0.2/mlfactory/dataloaders/coco.py
--rwxr-xr-x   0 root         (0) root         (0)     7066 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/dataloaders/diode.py
--rwxr-xr-x   0 root         (0) root         (0)    11385 2022-11-06 16:02:08.000000 mlfactory-0.0.2/mlfactory/dataloaders/imgcsvloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.274678 mlfactory-0.0.2/mlfactory/dataloaders/lidar_datasets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/dataloaders/lidar_datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18754 2022-10-05 16:29:32.000000 mlfactory-0.0.2/mlfactory/dataloaders/lidar_datasets/loader.py
--rw-r--r--   0 root         (0) root         (0)    21285 2022-09-09 17:47:12.000000 mlfactory-0.0.2/mlfactory/dataloaders/lidar_datasets/nuscenes.py
--rwxr-xr-x   0 root         (0) root         (0)     8461 2022-09-28 13:48:03.000000 mlfactory-0.0.2/mlfactory/dataloaders/modelnet.py
--rwxr-xr-x   0 root         (0) root         (0)    13990 2023-03-31 14:21:57.000000 mlfactory-0.0.2/mlfactory/dataloaders/nyuv2.py
--rwxr-xr-x   0 root         (0) root         (0)    11237 2023-04-23 12:18:32.000000 mlfactory-0.0.2/mlfactory/dataloaders/ouster_extract.py
--rwxr-xr-x   0 root         (0) root         (0)    10154 2022-09-28 13:48:03.000000 mlfactory-0.0.2/mlfactory/dataloaders/shapenet.py
--rwxr-xr-x   0 root         (0) root         (0)    12429 2023-04-15 20:17:10.000000 mlfactory-0.0.2/mlfactory/dataloaders/tum_rgbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.274678 mlfactory-0.0.2/mlfactory/dataloaders/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/dataloaders/utils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3421 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/dataloaders/utils/augmentations.py
--rwxr-xr-x   0 root         (0) root         (0)     6487 2022-09-28 13:48:03.000000 mlfactory-0.0.2/mlfactory/dataloaders/utils/pointcloud_voxelize.py
--rwxr-xr-x   0 root         (0) root         (0)    12996 2022-11-04 23:51:47.000000 mlfactory-0.0.2/mlfactory/dataloaders/utils/read_supervisely.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.278678 mlfactory-0.0.2/mlfactory/misctools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/misctools/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5880 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/misctools/median_filter.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-03-30 12:42:54.000000 mlfactory-0.0.2/mlfactory/misctools/pretrained_od.py
--rwxr-xr-x   0 root         (0) root         (0)     5121 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/misctools/random_homography.py
--rwxr-xr-x   0 root         (0) root         (0)     1663 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/misctools/sift_matching.py
--rwxr-xr-x   0 root         (0) root         (0)     6140 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/misctools/trifocal_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-03-30 12:42:54.000000 mlfactory-0.0.2/mlfactory/misctools/video_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.278678 mlfactory-0.0.2/mlfactory/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.278678 mlfactory-0.0.2/mlfactory/models/pytorch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/models/pytorch/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10250 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/models/pytorch/deeplabv3.py
--rwxr-xr-x   0 root         (0) root         (0)     4228 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/models/pytorch/feature_pyramid.py
--rw-r--r--   0 root         (0) root         (0)    10977 2022-09-28 13:48:03.000000 mlfactory-0.0.2/mlfactory/models/pytorch/pointnet.py
--rwxr-xr-x   0 root         (0) root         (0)     3269 2023-04-15 19:06:02.000000 mlfactory-0.0.2/mlfactory/models/pytorch/regressor.py
--rwxr-xr-x   0 root         (0) root         (0)     1305 2022-11-28 13:47:33.000000 mlfactory-0.0.2/mlfactory/models/pytorch/simple_conv.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/models/pytorch/unet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.278678 mlfactory-0.0.2/mlfactory/trainers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/trainers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.278678 mlfactory-0.0.2/mlfactory/trainers/pytorch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/trainers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5027 2022-10-05 16:29:32.000000 mlfactory-0.0.2/mlfactory/trainers/pytorch/train_pointcloud.py
--rwxr-xr-x   0 root         (0) root         (0)     2632 2023-04-15 19:06:56.000000 mlfactory-0.0.2/mlfactory/trainers/pytorch/train_reg.py
--rwxr-xr-x   0 root         (0) root         (0)     3375 2022-08-06 01:28:36.000000 mlfactory-0.0.2/mlfactory/trainers/pytorch/train_seg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.278678 mlfactory-0.0.2/mlfactory/trainers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/trainers/tensorflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.278678 mlfactory-0.0.2/mlfactory/trainers/tensorflow/object_detection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/trainers/tensorflow/object_detection/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5095 2022-11-05 18:56:21.000000 mlfactory-0.0.2/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.278678 mlfactory-0.0.2/mlfactory/visualizers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.2/mlfactory/visualizers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     9415 2023-04-19 21:27:23.000000 mlfactory-0.0.2/mlfactory/visualizers/pointcloud.py
--rw-r--r--   0 root         (0) root         (0)    12514 2023-04-19 22:14:46.000000 mlfactory-0.0.2/mlfactory/visualizers/project_rgbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:12:53.262678 mlfactory-0.0.2/mlfactory.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1418 2023-05-14 18:12:53.000000 mlfactory-0.0.2/mlfactory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4314 2023-05-14 18:12:53.000000 mlfactory-0.0.2/mlfactory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 18:12:53.000000 mlfactory-0.0.2/mlfactory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 18:12:53.000000 mlfactory-0.0.2/mlfactory.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-14 18:12:44.000000 mlfactory-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 18:12:53.278678 mlfactory-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      811 2023-05-14 18:12:37.000000 mlfactory-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.233199 mlfactory-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-05-22 13:29:58.233199 mlfactory-0.0.3/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     2254 2023-05-22 12:56:59.000000 mlfactory-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.213199 mlfactory-0.0.3/mlfactory/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 19:40:33.000000 mlfactory-0.0.3/mlfactory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.213199 mlfactory-0.0.3/mlfactory/applications/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 19:40:15.000000 mlfactory-0.0.3/mlfactory/applications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.213199 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-17 19:41:17.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19178 2023-05-22 12:51:07.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/mapper.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-04-21 14:15:08.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/read_video.py
+-rw-r--r--   0 root         (0) root         (0)    16458 2023-05-17 23:39:19.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.213199 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5309 2023-05-21 17:44:26.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-03-24 18:19:17.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-03-19 11:53:53.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-03-24 18:22:37.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     8395 2023-05-18 14:13:47.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py
+-rw-r--r--   0 root         (0) root         (0)     1324 2022-08-18 10:40:00.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-04-21 14:19:44.000000 mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.217199 mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2947 2023-04-20 19:13:46.000000 mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-04-02 23:52:08.000000 mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/datahandler.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-04-02 23:52:08.000000 mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/main.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-04-02 23:52:08.000000 mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/model.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2023-04-02 23:52:08.000000 mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/segdataset.py
+-rw-r--r--   0 root         (0) root         (0)     6809 2023-04-20 20:15:23.000000 mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/test.py
+-rw-r--r--   0 root         (0) root         (0)     3578 2023-04-02 23:52:08.000000 mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.217199 mlfactory-0.0.3/mlfactory/applications/superglue_inference/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 19:44:47.000000 mlfactory-0.0.3/mlfactory/applications/superglue_inference/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8594 2023-05-22 13:08:37.000000 mlfactory-0.0.3/mlfactory/applications/superglue_inference/match_pair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.217199 mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-10-07 16:11:34.000000 mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2022-10-07 16:11:34.000000 mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/matching.py
+-rw-r--r--   0 root         (0) root         (0)    11781 2022-10-07 16:11:34.000000 mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/superglue.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2022-10-07 16:11:34.000000 mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/superpoint.py
+-rw-r--r--   0 root         (0) root         (0)    20039 2022-10-07 16:11:34.000000 mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.217199 mlfactory-0.0.3/mlfactory/custom_losses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/custom_losses/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.221199 mlfactory-0.0.3/mlfactory/custom_losses/pytorch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/custom_losses/pytorch/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4036 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/custom_losses/pytorch/depth.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2022-10-05 16:29:32.000000 mlfactory-0.0.3/mlfactory/custom_losses/pytorch/pointnetloss.py
+-rwxr-xr-x   0 root         (0) root         (0)      190 2023-04-15 14:33:36.000000 mlfactory-0.0.3/mlfactory/custom_losses/pytorch/regress.py
+-rwxr-xr-x   0 root         (0) root         (0)      957 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/custom_losses/pytorch/segment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.221199 mlfactory-0.0.3/mlfactory/custom_losses/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/custom_losses/tensorflow/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1445 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/custom_losses/tensorflow/feature_detect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.221199 mlfactory-0.0.3/mlfactory/datacreators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/datacreators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.221199 mlfactory-0.0.3/mlfactory/datacreators/ai2thor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/datacreators/ai2thor/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7962 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/datacreators/ai2thor/create_dataset.py
+-rwxr-xr-x   0 root         (0) root         (0)     5970 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/datacreators/ai2thor/register_pcds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.221199 mlfactory-0.0.3/mlfactory/datacreators/lidar_contours/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/datacreators/lidar_contours/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6484 2022-11-05 15:28:48.000000 mlfactory-0.0.3/mlfactory/datacreators/lidar_contours/human_contours.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.221199 mlfactory-0.0.3/mlfactory/datacreators/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/datacreators/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-14 17:50:57.000000 mlfactory-0.0.3/mlfactory/datacreators/utils/colab_poly_anot.py
+-rwxr-xr-x   0 root         (0) root         (0)    10241 2022-11-04 20:33:18.000000 mlfactory-0.0.3/mlfactory/datacreators/utils/cv_annotator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.225199 mlfactory-0.0.3/mlfactory/dataloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/dataloaders/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    11455 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/dataloaders/ade20k.py
+-rwxr-xr-x   0 root         (0) root         (0)     3651 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/dataloaders/cihp.py
+-rwxr-xr-x   0 root         (0) root         (0)     9524 2023-04-13 01:43:27.000000 mlfactory-0.0.3/mlfactory/dataloaders/coco.py
+-rwxr-xr-x   0 root         (0) root         (0)     7066 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/dataloaders/diode.py
+-rwxr-xr-x   0 root         (0) root         (0)    11385 2022-11-06 16:02:08.000000 mlfactory-0.0.3/mlfactory/dataloaders/imgcsvloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.229199 mlfactory-0.0.3/mlfactory/dataloaders/lidar_datasets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/dataloaders/lidar_datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18754 2022-10-05 16:29:32.000000 mlfactory-0.0.3/mlfactory/dataloaders/lidar_datasets/loader.py
+-rw-r--r--   0 root         (0) root         (0)    21285 2022-09-09 17:47:12.000000 mlfactory-0.0.3/mlfactory/dataloaders/lidar_datasets/nuscenes.py
+-rwxr-xr-x   0 root         (0) root         (0)     8461 2022-09-28 13:48:03.000000 mlfactory-0.0.3/mlfactory/dataloaders/modelnet.py
+-rwxr-xr-x   0 root         (0) root         (0)    13990 2023-03-31 14:21:57.000000 mlfactory-0.0.3/mlfactory/dataloaders/nyuv2.py
+-rwxr-xr-x   0 root         (0) root         (0)    11237 2023-04-23 12:18:32.000000 mlfactory-0.0.3/mlfactory/dataloaders/ouster_extract.py
+-rwxr-xr-x   0 root         (0) root         (0)    10154 2022-09-28 13:48:03.000000 mlfactory-0.0.3/mlfactory/dataloaders/shapenet.py
+-rwxr-xr-x   0 root         (0) root         (0)    12429 2023-04-15 20:17:10.000000 mlfactory-0.0.3/mlfactory/dataloaders/tum_rgbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.229199 mlfactory-0.0.3/mlfactory/dataloaders/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/dataloaders/utils/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3421 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/dataloaders/utils/augmentations.py
+-rwxr-xr-x   0 root         (0) root         (0)     6487 2022-09-28 13:48:03.000000 mlfactory-0.0.3/mlfactory/dataloaders/utils/pointcloud_voxelize.py
+-rwxr-xr-x   0 root         (0) root         (0)    12996 2022-11-04 23:51:47.000000 mlfactory-0.0.3/mlfactory/dataloaders/utils/read_supervisely.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.229199 mlfactory-0.0.3/mlfactory/misctools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/misctools/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5880 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/misctools/median_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-03-30 12:42:54.000000 mlfactory-0.0.3/mlfactory/misctools/pretrained_od.py
+-rwxr-xr-x   0 root         (0) root         (0)     5121 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/misctools/random_homography.py
+-rwxr-xr-x   0 root         (0) root         (0)     1663 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/misctools/sift_matching.py
+-rwxr-xr-x   0 root         (0) root         (0)     6140 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/misctools/trifocal_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-03-30 12:42:54.000000 mlfactory-0.0.3/mlfactory/misctools/video_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.229199 mlfactory-0.0.3/mlfactory/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.233199 mlfactory-0.0.3/mlfactory/models/pytorch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/models/pytorch/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10250 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/models/pytorch/deeplabv3.py
+-rwxr-xr-x   0 root         (0) root         (0)     4228 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/models/pytorch/feature_pyramid.py
+-rw-r--r--   0 root         (0) root         (0)    10977 2022-09-28 13:48:03.000000 mlfactory-0.0.3/mlfactory/models/pytorch/pointnet.py
+-rwxr-xr-x   0 root         (0) root         (0)     3269 2023-04-15 19:06:02.000000 mlfactory-0.0.3/mlfactory/models/pytorch/regressor.py
+-rwxr-xr-x   0 root         (0) root         (0)     1305 2022-11-28 13:47:33.000000 mlfactory-0.0.3/mlfactory/models/pytorch/simple_conv.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/models/pytorch/unet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.233199 mlfactory-0.0.3/mlfactory/trainers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/trainers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.233199 mlfactory-0.0.3/mlfactory/trainers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/trainers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2022-10-05 16:29:32.000000 mlfactory-0.0.3/mlfactory/trainers/pytorch/train_pointcloud.py
+-rwxr-xr-x   0 root         (0) root         (0)     2632 2023-04-15 19:06:56.000000 mlfactory-0.0.3/mlfactory/trainers/pytorch/train_reg.py
+-rwxr-xr-x   0 root         (0) root         (0)     3375 2022-08-06 01:28:36.000000 mlfactory-0.0.3/mlfactory/trainers/pytorch/train_seg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.233199 mlfactory-0.0.3/mlfactory/trainers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/trainers/tensorflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.233199 mlfactory-0.0.3/mlfactory/trainers/tensorflow/object_detection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/trainers/tensorflow/object_detection/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5095 2022-11-05 18:56:21.000000 mlfactory-0.0.3/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.233199 mlfactory-0.0.3/mlfactory/visualizers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.3/mlfactory/visualizers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     9415 2023-04-19 21:27:23.000000 mlfactory-0.0.3/mlfactory/visualizers/pointcloud.py
+-rw-r--r--   0 root         (0) root         (0)    12514 2023-04-19 22:14:46.000000 mlfactory-0.0.3/mlfactory/visualizers/project_rgbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:29:58.213199 mlfactory-0.0.3/mlfactory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-05-22 13:29:58.000000 mlfactory-0.0.3/mlfactory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4456 2023-05-22 13:29:58.000000 mlfactory-0.0.3/mlfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 13:29:58.000000 mlfactory-0.0.3/mlfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-22 13:29:58.000000 mlfactory-0.0.3/mlfactory.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-22 13:28:56.000000 mlfactory-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 13:29:58.233199 mlfactory-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      811 2023-05-22 13:29:10.000000 mlfactory-0.0.3/setup.py
```

### Comparing `mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/main.py` & `mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,35 +3,59 @@
 import numpy as np
 from scipy.spatial.transform import Rotation as R
 
 import time
 import copy
 import math
 
-from tools import project_rgbd
-from tools import sift_matching
-
 import os
 import sys
 from datetime import datetime as dt
 
-cimportpath = os.getcwd()
-if cimportpath[cimportpath.rfind("/")+1:]=="deep_modular_scene_mapper": #if this module is called from dataloaders code
-    os.environ['top'] = '../../'
-    os.environ['applications'] = '../../applications'
-    sys.path.append(os.path.join(os.environ['top']))
-    sys.path.append(os.path.join(os.environ['applications']))
+
+
+# An installation agnostic method to find and link to root of the package which is mlfactory
+#==========================================================
+import re
+try: #testing the functions locally without pip install
+  import __init__
+  cimportpath = os.path.abspath(__init__.__file__)
+except: #testing while mlfactory is installed using pip
+  import mlfactory
+  cimportpath = os.path.abspath(mlfactory.__file__)+'/applications/deep_modular_scene_mapper/__init__.py'
+
+idxlist = [m.start() for m in re.finditer(r"/", cimportpath)]
+invoking_submodule = cimportpath[idxlist[-2]+1:idxlist[-1]]
+print("In deep_modular_scene_mapper/main.py got invoking submodule using re",invoking_submodule)
+main_package_loc = cimportpath[:cimportpath.rfind('mlfactory')+len('mlfactory')]
+print("In deep_modular_scene_mapper/main.py got main package location ",main_package_loc)
+
+
+os.environ['applications'] = main_package_loc+'/applications'
+os.environ['top'] = main_package_loc
+sys.path.append(os.path.join(os.environ['applications']))
+sys.path.append(os.path.join(os.environ['top']))
+#==========================================================
+
 
 
 #from superglue_inference.match_pair import matcher
+
 from applications.superglue_inference import match_pair
 from applications.deep_modular_scene_mapper.tools.rigid_transform_3D import rigid_transform_3D
 from applications.deep_modular_scene_mapper.tools import point_plane_icp
 from applications.deep_modular_scene_mapper.tools.depth_estimator import monodepth
 
+from applications.deep_modular_scene_mapper.tools import project_rgbd
+from applications.deep_modular_scene_mapper.tools import sift_matching
+
+#from tools import project_rgbd
+#from tools import sift_matching
+
+
 
 
 
 data_location = '/datasets/sample_videos/extracted/'
 feature_matcher = match_pair.matcher()
 md = monodepth()
```

### Comparing `mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/read_video.py` & `mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/read_video.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py` & `mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py` & `mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py` & `mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py` & `mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,40 +117,40 @@
 
     #X =  (imgrid[1,:,:] - camera_params["centerX"])  / camera_params["fx"] 
     #Y =  (imgrid[0,:,:] - camera_params["centerY"])  / camera_params["fy"] 
 
 
 
     
-    print("X Y Z shapes ",X.shape,Y.shape,Z.shape)
+    #print("X Y Z shapes ",X.shape,Y.shape,Z.shape)
 
     #convert X,Y,Z points to a pcd
     xyz = np.dstack([X,Y,Z]).reshape((X.shape[0]*X.shape[1],3))/ normalizer
-    print("XYZ shape ",xyz.shape)
+    #print("XYZ shape ",xyz.shape)
     colors = color.reshape((X.shape[0]*X.shape[1],3))/255.0
     pcd = o3d.geometry.PointCloud()
     pcd.points = o3d.utility.Vector3dVector(xyz)
     pcd.colors = o3d.utility.Vector3dVector(colors)
 
 
     #rotate the pcd along x axis by 180 degrees to get normal orientation pcd
     R = pcd.get_rotation_matrix_from_xyz((np.pi , 0, 0))
     pcd = pcd.rotate(R, center=(0,0,0))
 
 
     #recover rotated X,Y,Z from the rotated pcd
     rpts = np.array(pcd.points).reshape((X.shape[0],X.shape[1],3))
     X,Y,Z = rpts[:,:,0], rpts[:,:,1], rpts[:,:,2]
-    print("X Y Z shapes ",X.shape,Y.shape,Z.shape)
+    #print("X Y Z shapes ",X.shape,Y.shape,Z.shape)
     colors = np.array(pcd.colors).reshape((X.shape[0],X.shape[1],3))*255.0
     
 
     #for each pixel location in the RGB image stores the corresponding 3d coordinate it is mapped to
     pixel_points = np.dstack([X.T,Y.T,Z.T])
-    print("pixel points shape ",pixel_points.shape)
+    #print("pixel points shape ",pixel_points.shape)
     return pcd, pixel_points
 
 
 
             
 def show_pcd_from_rgbd(rgb, d, camera_params, save_loc = ""):
```

### Comparing `mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py` & `mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py` & `mlfactory-0.0.3/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py` & `mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/datahandler.py` & `mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/datahandler.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/main.py` & `mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/main.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/model.py` & `mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/model.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/segdataset.py` & `mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/segdataset.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/test.py` & `mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/test.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/segmentation_finetune/trainer.py` & `mlfactory-0.0.3/mlfactory/applications/segmentation_finetune/trainer.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/superglue_inference/match_pair.py` & `mlfactory-0.0.3/mlfactory/applications/superglue_inference/match_pair.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 import os
 import sys
 
-cimportpath = os.getcwd()
-if cimportpath[cimportpath.rfind("/")+1:]=="dataloaders": #if this module is called from dataloaders code
-    os.environ['superglue'] = '../applications/superglue_inference'
-    sys.path.append(os.path.join(os.environ['superglue']))
-
-if cimportpath[cimportpath.rfind("/")+1:]=="examples": #if this module is called from dataloaders code
-    os.environ['superglue'] = '../applications/superglue_inference'
-    sys.path.append(os.path.join(os.environ['superglue']))
-
-if cimportpath[cimportpath.rfind("/")+1:]=="deep_modular_scene_mapper": #if this module is called from dataloaders code
-    os.environ['superglue'] = '../../applications/superglue_inference'
-    sys.path.append(os.path.join(os.environ['superglue']))
-
-if cimportpath[cimportpath.rfind("/")+1:]=="sfm3d": #if this module is called from dataloaders code
-    os.environ['superglue'] = '../../applications/superglue_inference'
-    sys.path.append(os.path.join(os.environ['superglue']))
-
-if cimportpath[cimportpath.rfind("/")+1:]=="superglue_inference":
-    os.environ['superglue'] = '../superglue_inference'
-    sys.path.append(os.path.join(os.environ['superglue']))
-    os.environ['supergluetop'] = '../'
-    sys.path.append(os.path.join(os.environ['supergluetop']))
 
 
+# An installation agnostic method to find and link to root of the package which is mlfactory
+#==========================================================
+import re
+
+try: #testing the functions locally without pip install
+  import __init__
+  cimportpath = os.path.abspath(__init__.__file__)
+except: #testing while mlfactory is installed using pip
+  import mlfactory
+  cimportpath = os.path.abspath(mlfactory.__file__)+'/applications/superglue_inference/__init__.py'
+
+idxlist = [m.start() for m in re.finditer(r"/", cimportpath)]
+invoking_submodule = cimportpath[idxlist[-2]+1:idxlist[-1]]
+print("In superglue_inference/match_pair.py got invoking submodule using re",invoking_submodule)
+main_package_loc = cimportpath[:cimportpath.rfind('mlfactory')+len('mlfactory')]
+print("In superglue_inference/match_pair.py got main package location ",main_package_loc)
+
+
+os.environ['superglue'] = main_package_loc+'/applications/superglue_inference'
+os.environ['top'] = main_package_loc
+sys.path.append(os.path.join(os.environ['superglue']))
+sys.path.append(os.path.join(os.environ['top']))
+#==========================================================
 
 
 from pathlib import Path
 import argparse
 import cv2
 import matplotlib.cm as cm
 import torch
 
-import superglue_inference
-from superglue_inference.models.matching import Matching
-from superglue_inference.models.utils import (AverageTimer, VideoStreamer,make_matching_plot_fast, frame2tensor)
+#import superglue_inference
+from applications.superglue_inference.models.matching import Matching
+from applications.superglue_inference.models.utils import (AverageTimer, VideoStreamer,make_matching_plot_fast, frame2tensor)
+
+#from models.matching import Matching
+#from models.utils import (AverageTimer, VideoStreamer,make_matching_plot_fast, frame2tensor)
+
 
 import numpy as np
 #torch.set_grad_enabled(False)
 
 from skimage.measure import ransac
 from skimage.transform import ProjectiveTransform, AffineTransform
 
 def check_weights():
     gpath = os.environ['superglue']
     if os.path.exists(gpath+"/models/weights")==False:
+    #if os.path.exists("models/weights")==False:
         print("pretrained weights need to be downloaded and extracted ")
         os.system("pip install gdown")
         os.system("gdown --id 1RU5jIDkvaXE_h0fEew-xYCiJs87QDMEG")
         os.system("unzip superglueweights.zip -d"+gpath+"/models/")
         print("done extracting !")
         os.system("rm -rf superglueweights.zip")
 
@@ -63,14 +69,15 @@
         nms_radius = 4
         keypoint_threshold = 0.005
         max_keypoints = -1 #detect as many as possible
         superglue = 'indoor'
         sinkhorn_iterations = 20
         match_threshold = 0.2
         show_keypoints = False
+        self.viz_plt = False
 
 
 
         device = 'cuda' if torch.cuda.is_available() and not force_cpu else 'cpu'
         print('Running inference on device \"{}\"'.format(device))
         config = {
             'superpoint': {
@@ -214,30 +221,40 @@
                     last_frame, frame, kpts0, kpts1, mkpts0[inliers], mkpts1[inliers], color, text,
                     path=None, show_keypoints=self.show_keypoints, small_text=small_text)
             else:
                 out = make_matching_plot_fast(
                     last_frame, frame, kpts0, kpts1, mkpts0, mkpts1, color, text,
                     path=None, show_keypoints=self.show_keypoints, small_text=small_text)
 
-            cv2.imshow('SuperGlue matches', out)
-            cv2.waitKey(10)
+            if self.viz_plt:
+                import matplotlib
+                #matplotlib.use('TkAgg')
+                from matplotlib import pyplot as plt
+                fig, ax = plt.subplots()
+                ax.set_axis_off()
+                ax.imshow(out)
+                #plt.show()
+            else:
+                cv2.imshow('SuperGlue matches', out)
+                cv2.waitKey(0)
 
 
 
         torch.set_grad_enabled(True)
 
 
 
 
         return mkpts0, mkpts1
 
 
 
 if __name__ == '__main__':
     m = matcher()
+    #m.viz_plt = True
     im1 = np.array(cv2.imread("sample1.png",0))
     im2 = np.array(cv2.imread("sample2.png",0))
     m.match(im1,im2)
```

### Comparing `mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/matching.py` & `mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/matching.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/superglue.py` & `mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/superglue.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/superpoint.py` & `mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/applications/superglue_inference/models/utils.py` & `mlfactory-0.0.3/mlfactory/applications/superglue_inference/models/utils.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/custom_losses/pytorch/depth.py` & `mlfactory-0.0.3/mlfactory/custom_losses/pytorch/depth.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/custom_losses/pytorch/pointnetloss.py` & `mlfactory-0.0.3/mlfactory/custom_losses/pytorch/pointnetloss.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/custom_losses/pytorch/segment.py` & `mlfactory-0.0.3/mlfactory/custom_losses/pytorch/segment.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/custom_losses/tensorflow/feature_detect.py` & `mlfactory-0.0.3/mlfactory/custom_losses/tensorflow/feature_detect.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/datacreators/ai2thor/create_dataset.py` & `mlfactory-0.0.3/mlfactory/datacreators/ai2thor/create_dataset.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/datacreators/ai2thor/register_pcds.py` & `mlfactory-0.0.3/mlfactory/datacreators/ai2thor/register_pcds.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/datacreators/lidar_contours/human_contours.py` & `mlfactory-0.0.3/mlfactory/datacreators/lidar_contours/human_contours.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/datacreators/utils/colab_poly_anot.py` & `mlfactory-0.0.3/mlfactory/datacreators/utils/colab_poly_anot.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/datacreators/utils/cv_annotator.py` & `mlfactory-0.0.3/mlfactory/datacreators/utils/cv_annotator.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/ade20k.py` & `mlfactory-0.0.3/mlfactory/dataloaders/ade20k.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/cihp.py` & `mlfactory-0.0.3/mlfactory/dataloaders/cihp.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/coco.py` & `mlfactory-0.0.3/mlfactory/dataloaders/coco.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/diode.py` & `mlfactory-0.0.3/mlfactory/dataloaders/diode.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/imgcsvloader.py` & `mlfactory-0.0.3/mlfactory/dataloaders/imgcsvloader.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/lidar_datasets/loader.py` & `mlfactory-0.0.3/mlfactory/dataloaders/lidar_datasets/loader.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/lidar_datasets/nuscenes.py` & `mlfactory-0.0.3/mlfactory/dataloaders/lidar_datasets/nuscenes.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/modelnet.py` & `mlfactory-0.0.3/mlfactory/dataloaders/modelnet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/nyuv2.py` & `mlfactory-0.0.3/mlfactory/dataloaders/nyuv2.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/ouster_extract.py` & `mlfactory-0.0.3/mlfactory/dataloaders/ouster_extract.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/shapenet.py` & `mlfactory-0.0.3/mlfactory/dataloaders/shapenet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/tum_rgbd.py` & `mlfactory-0.0.3/mlfactory/dataloaders/tum_rgbd.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/utils/augmentations.py` & `mlfactory-0.0.3/mlfactory/dataloaders/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/utils/pointcloud_voxelize.py` & `mlfactory-0.0.3/mlfactory/dataloaders/utils/pointcloud_voxelize.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/dataloaders/utils/read_supervisely.py` & `mlfactory-0.0.3/mlfactory/dataloaders/utils/read_supervisely.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/misctools/median_filter.py` & `mlfactory-0.0.3/mlfactory/misctools/median_filter.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/misctools/pretrained_od.py` & `mlfactory-0.0.3/mlfactory/misctools/pretrained_od.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/misctools/random_homography.py` & `mlfactory-0.0.3/mlfactory/misctools/random_homography.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/misctools/sift_matching.py` & `mlfactory-0.0.3/mlfactory/misctools/sift_matching.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/misctools/trifocal_tensor.py` & `mlfactory-0.0.3/mlfactory/misctools/trifocal_tensor.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/misctools/video_writer.py` & `mlfactory-0.0.3/mlfactory/misctools/video_writer.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/models/pytorch/deeplabv3.py` & `mlfactory-0.0.3/mlfactory/models/pytorch/deeplabv3.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/models/pytorch/feature_pyramid.py` & `mlfactory-0.0.3/mlfactory/models/pytorch/feature_pyramid.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/models/pytorch/pointnet.py` & `mlfactory-0.0.3/mlfactory/models/pytorch/pointnet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/models/pytorch/regressor.py` & `mlfactory-0.0.3/mlfactory/models/pytorch/regressor.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/models/pytorch/simple_conv.py` & `mlfactory-0.0.3/mlfactory/models/pytorch/simple_conv.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/models/pytorch/unet.py` & `mlfactory-0.0.3/mlfactory/models/pytorch/unet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/trainers/pytorch/train_pointcloud.py` & `mlfactory-0.0.3/mlfactory/trainers/pytorch/train_pointcloud.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/trainers/pytorch/train_reg.py` & `mlfactory-0.0.3/mlfactory/trainers/pytorch/train_reg.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/trainers/pytorch/train_seg.py` & `mlfactory-0.0.3/mlfactory/trainers/pytorch/train_seg.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py` & `mlfactory-0.0.3/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/visualizers/pointcloud.py` & `mlfactory-0.0.3/mlfactory/visualizers/pointcloud.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory/visualizers/project_rgbd.py` & `mlfactory-0.0.3/mlfactory/visualizers/project_rgbd.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.2/mlfactory.egg-info/SOURCES.txt` & `mlfactory-0.0.3/mlfactory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 mlfactory/__init__.py
 mlfactory.egg-info/PKG-INFO
 mlfactory.egg-info/SOURCES.txt
 mlfactory.egg-info/dependency_links.txt
 mlfactory.egg-info/top_level.txt
 mlfactory/applications/__init__.py
 mlfactory/applications/deep_modular_scene_mapper/__init__.py
-mlfactory/applications/deep_modular_scene_mapper/main.py
+mlfactory/applications/deep_modular_scene_mapper/mapper.py
 mlfactory/applications/deep_modular_scene_mapper/read_video.py
+mlfactory/applications/deep_modular_scene_mapper/test_mapper.py
 mlfactory/applications/deep_modular_scene_mapper/tools/__init__.py
+mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py
 mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py
 mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py
 mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py
 mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py
 mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py
 mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py
 mlfactory/applications/segmentation_finetune/__init__.py
```

### Comparing `mlfactory-0.0.2/pyproject.toml` & `mlfactory-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "mlfactory"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Homagni Saha", email="homagnisaha@gmail.com" },
 ]
 description = "Collection of several machine learning modules which can be applied to diverse projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mlfactory-0.0.2/setup.py` & `mlfactory-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='mlfactory',  
-     version='0.0.2',
+     version='0.0.3',
      author="Homagni Saha",
      author_email="homagnisaha@gmail.com",
      description="Collection of several machine learning modules which can be applied to diverse projects",
      long_description=long_description,
    long_description_content_type="text/markdown",
      url="https://github.com/Homagn/mlfactory",
      packages=setuptools.find_packages(exclude=["mlfactory/applications/superglue_inference/models/weights","mlfactory/applications/segmentation_finetune/CFExp"]),
```

