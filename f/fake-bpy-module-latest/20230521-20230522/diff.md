# Comparing `tmp/fake-bpy-module-latest-20230521.tar.gz` & `tmp/fake-bpy-module-latest-20230522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230521.tar", last modified: Sun May 21 06:20:46 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230522.tar", last modified: Mon May 22 06:27:24 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230521.tar` & `fake-bpy-module-latest-20230522.tar`

### file list

```diff
@@ -1,353 +1,353 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-05-21 06:18:49.000000 fake-bpy-module-latest-20230521/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-21 06:20:38.000000 fake-bpy-module-latest-20230521/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-21 06:20:39.000000 fake-bpy-module-latest-20230521/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-21 06:20:39.000000 fake-bpy-module-latest-20230521/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-05-21 06:20:39.000000 fake-bpy-module-latest-20230521/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-05-21 06:20:39.000000 fake-bpy-module-latest-20230521/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-21 06:20:39.000000 fake-bpy-module-latest-20230521/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-05-21 06:20:43.000000 fake-bpy-module-latest-20230521/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-05-21 06:20:39.000000 fake-bpy-module-latest-20230521/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-05-21 06:20:43.000000 fake-bpy-module-latest-20230521/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-05-21 06:20:39.000000 fake-bpy-module-latest-20230521/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-21 06:20:43.000000 fake-bpy-module-latest-20230521/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-05-21 06:20:43.000000 fake-bpy-module-latest-20230521/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-21 06:20:40.000000 fake-bpy-module-latest-20230521/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-21 06:20:41.000000 fake-bpy-module-latest-20230521/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-21 06:20:39.000000 fake-bpy-module-latest-20230521/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-05-21 06:20:39.000000 fake-bpy-module-latest-20230521/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-05-21 06:20:42.000000 fake-bpy-module-latest-20230521/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-21 06:20:35.000000 fake-bpy-module-latest-20230521/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-21 06:20:35.000000 fake-bpy-module-latest-20230521/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-05-21 06:20:30.000000 fake-bpy-module-latest-20230521/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-21 06:20:05.000000 fake-bpy-module-latest-20230521/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-05-21 06:20:18.000000 fake-bpy-module-latest-20230521/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-05-21 06:19:50.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-21 06:18:55.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-05-21 06:19:52.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-05-21 06:18:55.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-05-21 06:20:35.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-21 06:20:20.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-05-21 06:20:35.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-21 06:20:30.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-21 06:19:05.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-05-21 06:19:57.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-05-21 06:19:06.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-21 06:20:27.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-21 06:20:22.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-05-21 06:20:19.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-21 06:20:20.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-05-21 06:20:05.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-05-21 06:20:05.000000 fake-bpy-module-latest-20230521/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-05-21 06:20:36.000000 fake-bpy-module-latest-20230521/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-05-21 06:18:56.000000 fake-bpy-module-latest-20230521/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-05-21 06:19:06.000000 fake-bpy-module-latest-20230521/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-05-21 06:19:57.000000 fake-bpy-module-latest-20230521/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-05-21 06:20:06.000000 fake-bpy-module-latest-20230521/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-05-21 06:20:23.000000 fake-bpy-module-latest-20230521/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-05-21 06:20:21.000000 fake-bpy-module-latest-20230521/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-05-21 06:20:18.000000 fake-bpy-module-latest-20230521/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-05-21 06:20:33.000000 fake-bpy-module-latest-20230521/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-05-21 06:19:56.000000 fake-bpy-module-latest-20230521/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-21 06:20:35.000000 fake-bpy-module-latest-20230521/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-05-21 06:20:08.000000 fake-bpy-module-latest-20230521/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-05-21 06:20:26.000000 fake-bpy-module-latest-20230521/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-05-21 06:20:28.000000 fake-bpy-module-latest-20230521/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-21 06:20:35.000000 fake-bpy-module-latest-20230521/bl_ui/properties_physics_geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-05-21 06:20:35.000000 fake-bpy-module-latest-20230521/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-05-21 06:20:05.000000 fake-bpy-module-latest-20230521/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-05-21 06:19:01.000000 fake-bpy-module-latest-20230521/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-05-21 06:20:38.000000 fake-bpy-module-latest-20230521/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-05-21 06:19:01.000000 fake-bpy-module-latest-20230521/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-05-21 06:19:50.000000 fake-bpy-module-latest-20230521/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-05-21 06:20:22.000000 fake-bpy-module-latest-20230521/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-21 06:19:05.000000 fake-bpy-module-latest-20230521/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-05-21 06:20:04.000000 fake-bpy-module-latest-20230521/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-05-21 06:20:26.000000 fake-bpy-module-latest-20230521/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-05-21 06:20:07.000000 fake-bpy-module-latest-20230521/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-05-21 06:20:19.000000 fake-bpy-module-latest-20230521/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-05-21 06:20:20.000000 fake-bpy-module-latest-20230521/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    53458 2023-05-21 06:19:51.000000 fake-bpy-module-latest-20230521/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-05-21 06:19:56.000000 fake-bpy-module-latest-20230521/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-05-21 06:19:05.000000 fake-bpy-module-latest-20230521/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-05-21 06:20:34.000000 fake-bpy-module-latest-20230521/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    70419 2023-05-21 06:20:07.000000 fake-bpy-module-latest-20230521/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-05-21 06:18:55.000000 fake-bpy-module-latest-20230521/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-21 06:20:38.000000 fake-bpy-module-latest-20230521/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-05-21 06:19:05.000000 fake-bpy-module-latest-20230521/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-21 06:19:51.000000 fake-bpy-module-latest-20230521/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-21 06:20:26.000000 fake-bpy-module-latest-20230521/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-05-21 06:20:22.000000 fake-bpy-module-latest-20230521/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-05-21 06:19:51.000000 fake-bpy-module-latest-20230521/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-21 06:20:35.000000 fake-bpy-module-latest-20230521/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-05-21 06:18:55.000000 fake-bpy-module-latest-20230521/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-05-21 06:20:31.000000 fake-bpy-module-latest-20230521/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-05-21 06:19:00.000000 fake-bpy-module-latest-20230521/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-05-21 06:19:49.000000 fake-bpy-module-latest-20230521/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-05-21 06:20:04.000000 fake-bpy-module-latest-20230521/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-21 06:20:04.000000 fake-bpy-module-latest-20230521/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-21 06:18:49.000000 fake-bpy-module-latest-20230521/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-21 06:18:09.000000 fake-bpy-module-latest-20230521/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-05-21 06:18:13.000000 fake-bpy-module-latest-20230521/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-05-21 06:18:21.000000 fake-bpy-module-latest-20230521/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-05-21 06:18:24.000000 fake-bpy-module-latest-20230521/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-05-21 06:18:27.000000 fake-bpy-module-latest-20230521/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-21 06:18:11.000000 fake-bpy-module-latest-20230521/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-21 06:18:20.000000 fake-bpy-module-latest-20230521/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-05-21 06:18:12.000000 fake-bpy-module-latest-20230521/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-21 06:18:24.000000 fake-bpy-module-latest-20230521/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-21 06:18:28.000000 fake-bpy-module-latest-20230521/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-05-21 06:18:13.000000 fake-bpy-module-latest-20230521/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-21 06:18:30.000000 fake-bpy-module-latest-20230521/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-21 06:18:22.000000 fake-bpy-module-latest-20230521/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-05-21 06:18:20.000000 fake-bpy-module-latest-20230521/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-05-21 06:18:22.000000 fake-bpy-module-latest-20230521/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-21 06:18:27.000000 fake-bpy-module-latest-20230521/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-21 06:18:27.000000 fake-bpy-module-latest-20230521/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-21 06:18:20.000000 fake-bpy-module-latest-20230521/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-05-21 06:18:12.000000 fake-bpy-module-latest-20230521/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-21 06:18:42.000000 fake-bpy-module-latest-20230521/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-21 06:18:42.000000 fake-bpy-module-latest-20230521/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-05-21 06:18:41.000000 fake-bpy-module-latest-20230521/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-05-21 06:18:19.000000 fake-bpy-module-latest-20230521/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-21 06:18:14.000000 fake-bpy-module-latest-20230521/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-05-21 06:18:29.000000 fake-bpy-module-latest-20230521/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-21 06:18:31.000000 fake-bpy-module-latest-20230521/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-21 06:18:21.000000 fake-bpy-module-latest-20230521/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-05-21 06:18:39.000000 fake-bpy-module-latest-20230521/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49909 2023-05-21 06:18:29.000000 fake-bpy-module-latest-20230521/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-05-21 06:18:40.000000 fake-bpy-module-latest-20230521/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-21 06:18:21.000000 fake-bpy-module-latest-20230521/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-21 06:18:27.000000 fake-bpy-module-latest-20230521/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-05-21 06:18:43.000000 fake-bpy-module-latest-20230521/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-21 06:18:23.000000 fake-bpy-module-latest-20230521/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-21 06:18:31.000000 fake-bpy-module-latest-20230521/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-05-21 06:18:21.000000 fake-bpy-module-latest-20230521/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-05-21 06:18:22.000000 fake-bpy-module-latest-20230521/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-21 06:18:09.000000 fake-bpy-module-latest-20230521/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-21 06:18:27.000000 fake-bpy-module-latest-20230521/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   180933 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-05-21 06:18:43.000000 fake-bpy-module-latest-20230521/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-05-21 06:18:19.000000 fake-bpy-module-latest-20230521/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   223124 2023-05-21 06:18:11.000000 fake-bpy-module-latest-20230521/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-05-21 06:18:23.000000 fake-bpy-module-latest-20230521/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-05-21 06:18:12.000000 fake-bpy-module-latest-20230521/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-21 06:18:25.000000 fake-bpy-module-latest-20230521/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-21 06:18:37.000000 fake-bpy-module-latest-20230521/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-05-21 06:18:20.000000 fake-bpy-module-latest-20230521/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-05-21 06:18:30.000000 fake-bpy-module-latest-20230521/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-21 06:18:11.000000 fake-bpy-module-latest-20230521/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-05-21 06:18:25.000000 fake-bpy-module-latest-20230521/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-21 06:18:31.000000 fake-bpy-module-latest-20230521/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-05-21 06:18:24.000000 fake-bpy-module-latest-20230521/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-05-21 06:18:21.000000 fake-bpy-module-latest-20230521/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-05-21 06:18:21.000000 fake-bpy-module-latest-20230521/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-21 06:18:37.000000 fake-bpy-module-latest-20230521/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46965 2023-05-21 06:18:18.000000 fake-bpy-module-latest-20230521/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-21 06:18:11.000000 fake-bpy-module-latest-20230521/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    93840 2023-05-21 06:18:17.000000 fake-bpy-module-latest-20230521/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-05-21 06:18:28.000000 fake-bpy-module-latest-20230521/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-21 06:18:22.000000 fake-bpy-module-latest-20230521/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-21 06:18:24.000000 fake-bpy-module-latest-20230521/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-05-21 06:18:31.000000 fake-bpy-module-latest-20230521/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-21 06:18:27.000000 fake-bpy-module-latest-20230521/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    71773 2023-05-21 06:18:27.000000 fake-bpy-module-latest-20230521/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-05-21 06:18:25.000000 fake-bpy-module-latest-20230521/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-21 06:18:46.000000 fake-bpy-module-latest-20230521/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    56864 2023-05-21 06:18:42.000000 fake-bpy-module-latest-20230521/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-21 06:18:31.000000 fake-bpy-module-latest-20230521/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    54854 2023-05-21 06:18:29.000000 fake-bpy-module-latest-20230521/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   245979 2023-05-21 06:18:37.000000 fake-bpy-module-latest-20230521/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-21 06:18:28.000000 fake-bpy-module-latest-20230521/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-21 06:18:11.000000 fake-bpy-module-latest-20230521/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-21 06:18:47.000000 fake-bpy-module-latest-20230521/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-05-21 06:18:47.000000 fake-bpy-module-latest-20230521/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3478772 2023-05-21 06:18:09.000000 fake-bpy-module-latest-20230521/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-21 06:18:47.000000 fake-bpy-module-latest-20230521/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-21 06:18:47.000000 fake-bpy-module-latest-20230521/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-21 06:18:47.000000 fake-bpy-module-latest-20230521/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-05-21 06:20:38.000000 fake-bpy-module-latest-20230521/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-05-21 06:18:51.000000 fake-bpy-module-latest-20230521/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-21 06:18:50.000000 fake-bpy-module-latest-20230521/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:49.000000 fake-bpy-module-latest-20230521/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-21 06:20:38.000000 fake-bpy-module-latest-20230521/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-21 06:18:54.000000 fake-bpy-module-latest-20230521/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 06:20:46.000000 fake-bpy-module-latest-20230521/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-21 06:20:45.000000 fake-bpy-module-latest-20230521/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-21 06:20:44.000000 fake-bpy-module-latest-20230521/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-05-22 06:24:38.000000 fake-bpy-module-latest-20230522/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-22 06:24:54.000000 fake-bpy-module-latest-20230522/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-22 06:24:52.000000 fake-bpy-module-latest-20230522/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-22 06:24:52.000000 fake-bpy-module-latest-20230522/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 06:24:56.000000 fake-bpy-module-latest-20230522/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-22 06:24:56.000000 fake-bpy-module-latest-20230522/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-22 06:24:52.000000 fake-bpy-module-latest-20230522/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-05-22 06:24:52.000000 fake-bpy-module-latest-20230522/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-22 06:24:51.000000 fake-bpy-module-latest-20230522/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-05-22 06:24:52.000000 fake-bpy-module-latest-20230522/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-05-22 06:24:57.000000 fake-bpy-module-latest-20230522/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-05-22 06:24:56.000000 fake-bpy-module-latest-20230522/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-22 06:24:53.000000 fake-bpy-module-latest-20230522/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-05-22 06:24:53.000000 fake-bpy-module-latest-20230522/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-05-22 06:24:54.000000 fake-bpy-module-latest-20230522/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-22 06:24:52.000000 fake-bpy-module-latest-20230522/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-22 06:24:56.000000 fake-bpy-module-latest-20230522/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-22 06:24:52.000000 fake-bpy-module-latest-20230522/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-05-22 06:24:57.000000 fake-bpy-module-latest-20230522/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-22 06:24:52.000000 fake-bpy-module-latest-20230522/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-22 06:24:56.000000 fake-bpy-module-latest-20230522/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-05-22 06:24:52.000000 fake-bpy-module-latest-20230522/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-22 06:24:56.000000 fake-bpy-module-latest-20230522/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-05-22 06:24:51.000000 fake-bpy-module-latest-20230522/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-22 06:24:56.000000 fake-bpy-module-latest-20230522/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-22 06:24:51.000000 fake-bpy-module-latest-20230522/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-22 06:24:56.000000 fake-bpy-module-latest-20230522/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-05-22 06:24:57.000000 fake-bpy-module-latest-20230522/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-05-22 06:24:56.000000 fake-bpy-module-latest-20230522/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 06:24:57.000000 fake-bpy-module-latest-20230522/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-22 06:24:57.000000 fake-bpy-module-latest-20230522/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 06:24:57.000000 fake-bpy-module-latest-20230522/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 06:24:57.000000 fake-bpy-module-latest-20230522/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-22 06:24:58.000000 fake-bpy-module-latest-20230522/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-22 06:25:18.000000 fake-bpy-module-latest-20230522/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 06:25:18.000000 fake-bpy-module-latest-20230522/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-05-22 06:25:37.000000 fake-bpy-module-latest-20230522/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-22 06:26:09.000000 fake-bpy-module-latest-20230522/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-22 06:25:56.000000 fake-bpy-module-latest-20230522/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-05-22 06:25:16.000000 fake-bpy-module-latest-20230522/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-05-22 06:24:59.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-22 06:27:20.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-05-22 06:25:28.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-05-22 06:25:16.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-05-22 06:25:48.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-22 06:25:01.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-05-22 06:27:21.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-22 06:27:23.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-22 06:26:09.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-05-22 06:26:09.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-05-22 06:25:24.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-22 06:25:57.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-22 06:25:01.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-05-22 06:25:23.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-22 06:27:20.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-05-22 06:25:58.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-05-22 06:25:19.000000 fake-bpy-module-latest-20230522/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-05-22 06:26:00.000000 fake-bpy-module-latest-20230522/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-05-22 06:27:19.000000 fake-bpy-module-latest-20230522/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-05-22 06:25:30.000000 fake-bpy-module-latest-20230522/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-05-22 06:27:16.000000 fake-bpy-module-latest-20230522/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-05-22 06:25:49.000000 fake-bpy-module-latest-20230522/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-05-22 06:25:30.000000 fake-bpy-module-latest-20230522/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-05-22 06:25:26.000000 fake-bpy-module-latest-20230522/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-05-22 06:26:07.000000 fake-bpy-module-latest-20230522/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-05-22 06:25:22.000000 fake-bpy-module-latest-20230522/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-05-22 06:25:18.000000 fake-bpy-module-latest-20230522/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-22 06:25:01.000000 fake-bpy-module-latest-20230522/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-05-22 06:25:58.000000 fake-bpy-module-latest-20230522/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-05-22 06:24:59.000000 fake-bpy-module-latest-20230522/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-05-22 06:25:01.000000 fake-bpy-module-latest-20230522/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-22 06:25:01.000000 fake-bpy-module-latest-20230522/bl_ui/properties_physics_geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-05-22 06:25:56.000000 fake-bpy-module-latest-20230522/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-05-22 06:26:09.000000 fake-bpy-module-latest-20230522/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-05-22 06:24:58.000000 fake-bpy-module-latest-20230522/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-05-22 06:27:19.000000 fake-bpy-module-latest-20230522/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-05-22 06:25:28.000000 fake-bpy-module-latest-20230522/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-05-22 06:25:25.000000 fake-bpy-module-latest-20230522/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-05-22 06:25:18.000000 fake-bpy-module-latest-20230522/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-22 06:25:25.000000 fake-bpy-module-latest-20230522/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-05-22 06:26:07.000000 fake-bpy-module-latest-20230522/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-05-22 06:27:15.000000 fake-bpy-module-latest-20230522/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-05-22 06:27:16.000000 fake-bpy-module-latest-20230522/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-05-22 06:26:10.000000 fake-bpy-module-latest-20230522/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-05-22 06:25:27.000000 fake-bpy-module-latest-20230522/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53458 2023-05-22 06:26:01.000000 fake-bpy-module-latest-20230522/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-05-22 06:26:06.000000 fake-bpy-module-latest-20230522/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-05-22 06:27:19.000000 fake-bpy-module-latest-20230522/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-05-22 06:26:07.000000 fake-bpy-module-latest-20230522/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70419 2023-05-22 06:25:50.000000 fake-bpy-module-latest-20230522/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-05-22 06:27:22.000000 fake-bpy-module-latest-20230522/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-22 06:25:18.000000 fake-bpy-module-latest-20230522/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-05-22 06:25:35.000000 fake-bpy-module-latest-20230522/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-22 06:26:09.000000 fake-bpy-module-latest-20230522/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-22 06:27:20.000000 fake-bpy-module-latest-20230522/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-05-22 06:25:29.000000 fake-bpy-module-latest-20230522/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-05-22 06:25:59.000000 fake-bpy-module-latest-20230522/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-22 06:27:20.000000 fake-bpy-module-latest-20230522/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-05-22 06:25:57.000000 fake-bpy-module-latest-20230522/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-05-22 06:27:23.000000 fake-bpy-module-latest-20230522/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-05-22 06:25:56.000000 fake-bpy-module-latest-20230522/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-05-22 06:27:11.000000 fake-bpy-module-latest-20230522/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-05-22 06:25:48.000000 fake-bpy-module-latest-20230522/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-22 06:25:18.000000 fake-bpy-module-latest-20230522/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-22 06:24:38.000000 fake-bpy-module-latest-20230522/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-22 06:24:47.000000 fake-bpy-module-latest-20230522/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-05-22 06:24:47.000000 fake-bpy-module-latest-20230522/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-22 06:24:36.000000 fake-bpy-module-latest-20230522/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-22 06:24:36.000000 fake-bpy-module-latest-20230522/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-22 06:24:36.000000 fake-bpy-module-latest-20230522/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-22 06:24:36.000000 fake-bpy-module-latest-20230522/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-22 06:24:36.000000 fake-bpy-module-latest-20230522/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-22 06:24:35.000000 fake-bpy-module-latest-20230522/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-05-22 06:15:32.000000 fake-bpy-module-latest-20230522/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-05-22 06:15:10.000000 fake-bpy-module-latest-20230522/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-05-22 06:15:51.000000 fake-bpy-module-latest-20230522/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-05-22 06:15:28.000000 fake-bpy-module-latest-20230522/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-22 06:15:52.000000 fake-bpy-module-latest-20230522/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-22 06:15:05.000000 fake-bpy-module-latest-20230522/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-05-22 06:15:27.000000 fake-bpy-module-latest-20230522/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-22 06:15:48.000000 fake-bpy-module-latest-20230522/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-22 06:15:51.000000 fake-bpy-module-latest-20230522/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-05-22 06:15:07.000000 fake-bpy-module-latest-20230522/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-22 06:15:07.000000 fake-bpy-module-latest-20230522/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-05-22 06:15:31.000000 fake-bpy-module-latest-20230522/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-05-22 06:15:28.000000 fake-bpy-module-latest-20230522/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-05-22 06:15:07.000000 fake-bpy-module-latest-20230522/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-22 06:15:46.000000 fake-bpy-module-latest-20230522/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-22 06:15:29.000000 fake-bpy-module-latest-20230522/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-22 06:15:50.000000 fake-bpy-module-latest-20230522/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-05-22 06:15:41.000000 fake-bpy-module-latest-20230522/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-22 06:15:10.000000 fake-bpy-module-latest-20230522/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-22 06:15:33.000000 fake-bpy-module-latest-20230522/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-05-22 06:15:13.000000 fake-bpy-module-latest-20230522/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-05-22 06:15:29.000000 fake-bpy-module-latest-20230522/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-22 06:15:13.000000 fake-bpy-module-latest-20230522/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-05-22 06:15:52.000000 fake-bpy-module-latest-20230522/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-22 06:15:47.000000 fake-bpy-module-latest-20230522/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-22 06:15:47.000000 fake-bpy-module-latest-20230522/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-05-22 06:15:05.000000 fake-bpy-module-latest-20230522/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49909 2023-05-22 06:15:41.000000 fake-bpy-module-latest-20230522/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-05-22 06:15:36.000000 fake-bpy-module-latest-20230522/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-22 06:15:33.000000 fake-bpy-module-latest-20230522/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-22 06:15:22.000000 fake-bpy-module-latest-20230522/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-22 06:15:30.000000 fake-bpy-module-latest-20230522/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-05-22 06:15:34.000000 fake-bpy-module-latest-20230522/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-22 06:15:50.000000 fake-bpy-module-latest-20230522/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-22 06:15:44.000000 fake-bpy-module-latest-20230522/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-05-22 06:15:10.000000 fake-bpy-module-latest-20230522/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-05-22 06:15:26.000000 fake-bpy-module-latest-20230522/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-22 06:15:27.000000 fake-bpy-module-latest-20230522/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-22 06:15:29.000000 fake-bpy-module-latest-20230522/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180933 2023-05-22 06:15:39.000000 fake-bpy-module-latest-20230522/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-05-22 06:15:33.000000 fake-bpy-module-latest-20230522/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-05-22 06:15:46.000000 fake-bpy-module-latest-20230522/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   223124 2023-05-22 06:15:26.000000 fake-bpy-module-latest-20230522/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-05-22 06:15:08.000000 fake-bpy-module-latest-20230522/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-05-22 06:15:40.000000 fake-bpy-module-latest-20230522/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-22 06:15:36.000000 fake-bpy-module-latest-20230522/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-22 06:15:22.000000 fake-bpy-module-latest-20230522/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-05-22 06:15:13.000000 fake-bpy-module-latest-20230522/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-05-22 06:15:22.000000 fake-bpy-module-latest-20230522/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-22 06:15:40.000000 fake-bpy-module-latest-20230522/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-05-22 06:15:31.000000 fake-bpy-module-latest-20230522/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-22 06:15:13.000000 fake-bpy-module-latest-20230522/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-22 06:15:03.000000 fake-bpy-module-latest-20230522/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-05-22 06:15:27.000000 fake-bpy-module-latest-20230522/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-05-22 06:15:28.000000 fake-bpy-module-latest-20230522/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-05-22 06:15:47.000000 fake-bpy-module-latest-20230522/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-22 06:15:48.000000 fake-bpy-module-latest-20230522/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46965 2023-05-22 06:15:31.000000 fake-bpy-module-latest-20230522/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-22 06:15:44.000000 fake-bpy-module-latest-20230522/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93840 2023-05-22 06:15:44.000000 fake-bpy-module-latest-20230522/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-05-22 06:15:33.000000 fake-bpy-module-latest-20230522/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-22 06:15:07.000000 fake-bpy-module-latest-20230522/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-22 06:15:52.000000 fake-bpy-module-latest-20230522/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-05-22 06:15:27.000000 fake-bpy-module-latest-20230522/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-22 06:15:40.000000 fake-bpy-module-latest-20230522/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71773 2023-05-22 06:15:50.000000 fake-bpy-module-latest-20230522/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-05-22 06:15:27.000000 fake-bpy-module-latest-20230522/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-22 06:15:10.000000 fake-bpy-module-latest-20230522/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56864 2023-05-22 06:15:10.000000 fake-bpy-module-latest-20230522/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-22 06:15:34.000000 fake-bpy-module-latest-20230522/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54854 2023-05-22 06:15:47.000000 fake-bpy-module-latest-20230522/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245979 2023-05-22 06:15:20.000000 fake-bpy-module-latest-20230522/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-22 06:15:34.000000 fake-bpy-module-latest-20230522/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-22 06:15:10.000000 fake-bpy-module-latest-20230522/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-22 06:24:35.000000 fake-bpy-module-latest-20230522/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-05-22 06:24:36.000000 fake-bpy-module-latest-20230522/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3478772 2023-05-22 06:24:35.000000 fake-bpy-module-latest-20230522/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-22 06:24:36.000000 fake-bpy-module-latest-20230522/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-22 06:24:36.000000 fake-bpy-module-latest-20230522/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-22 06:24:36.000000 fake-bpy-module-latest-20230522/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-22 06:24:57.000000 fake-bpy-module-latest-20230522/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-05-22 06:24:49.000000 fake-bpy-module-latest-20230522/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-22 06:27:23.000000 fake-bpy-module-latest-20230522/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-22 06:24:41.000000 fake-bpy-module-latest-20230522/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-05-22 06:24:44.000000 fake-bpy-module-latest-20230522/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-05-22 06:24:41.000000 fake-bpy-module-latest-20230522/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-05-22 06:24:39.000000 fake-bpy-module-latest-20230522/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 06:24:39.000000 fake-bpy-module-latest-20230522/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-22 06:24:39.000000 fake-bpy-module-latest-20230522/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-22 06:24:40.000000 fake-bpy-module-latest-20230522/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:02.000000 fake-bpy-module-latest-20230522/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-22 06:27:23.000000 fake-bpy-module-latest-20230522/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-22 06:24:57.000000 fake-bpy-module-latest-20230522/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-22 06:24:50.000000 fake-bpy-module-latest-20230522/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-22 06:27:24.000000 fake-bpy-module-latest-20230522/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-22 06:24:48.000000 fake-bpy-module-latest-20230522/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230521/PKG-INFO` & `fake-bpy-module-latest-20230522/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230521
+Version: 20230522
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230521/README.rst` & `fake-bpy-module-latest-20230522/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/addon_utils.py` & `fake-bpy-module-latest-20230522/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/animsys_refactor.py` & `fake-bpy-module-latest-20230522/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/aud.py` & `fake-bpy-module-latest-20230522/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bgl.py` & `fake-bpy-module-latest-20230522/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230522/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230522/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230522/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230522/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230522/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_math.py` & `fake-bpy-module-latest-20230522/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/__init__.py` & `fake-bpy-module-latest-20230522/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import sys
 import typing
-from . import vertexpaint_dirt
-from . import add_mesh_torus
-from . import freestyle
+from . import uvcalc_follow_active
+from . import clip
+from . import uvcalc_transform
+from . import file
+from . import userpref
+from . import rigidbody
+from . import object_align
+from . import assets
 from . import sequencer
-from . import object
+from . import anim
 from . import constraint
+from . import console
+from . import freestyle
+from . import object_randomize_transform
+from . import node
 from . import mesh
-from . import assets
-from . import view3d
-from . import rigidbody
-from . import object_quick_effects
-from . import image
+from . import object
+from . import add_mesh_torus
+from . import wm
 from . import uvcalc_lightmap
-from . import object_randomize_transform
-from . import console
-from . import bmesh
-from . import object_align
+from . import spreadsheet
 from . import screen_play_rendered_anim
-from . import anim
-from . import uvcalc_transform
-from . import wm
+from . import vertexpaint_dirt
+from . import image
+from . import object_quick_effects
+from . import bmesh
 from . import presets
-from . import spreadsheet
-from . import node
-from . import userpref
 from . import geometry_nodes
-from . import uvcalc_follow_active
-from . import file
-from . import clip
+from . import view3d
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230521/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230522/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/anim.py` & `fake-bpy-module-latest-20230522/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/assets.py` & `fake-bpy-module-latest-20230522/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230522/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/clip.py` & `fake-bpy-module-latest-20230522/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/console.py` & `fake-bpy-module-latest-20230522/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/constraint.py` & `fake-bpy-module-latest-20230522/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/file.py` & `fake-bpy-module-latest-20230522/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230522/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230522/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/image.py` & `fake-bpy-module-latest-20230522/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/mesh.py` & `fake-bpy-module-latest-20230522/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/node.py` & `fake-bpy-module-latest-20230522/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/object.py` & `fake-bpy-module-latest-20230522/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/object_align.py` & `fake-bpy-module-latest-20230522/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230522/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230522/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/presets.py` & `fake-bpy-module-latest-20230522/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230522/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230522/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230522/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230522/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/userpref.py` & `fake-bpy-module-latest-20230522/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230522/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230522/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230522/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230522/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/view3d.py` & `fake-bpy-module-latest-20230522/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_operators/wm.py` & `fake-bpy-module-latest-20230522/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230522/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/__init__.py` & `fake-bpy-module-latest-20230522/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import sys
 import typing
 import bpy_types
 
-from . import properties_animviz
-from . import properties_data_curve
-from . import space_outliner
-from . import properties_data_bone
-from . import space_toolsystem_toolbar
-from . import properties_grease_pencil_common
-from . import space_userpref
-from . import properties_scene
 from . import properties_physics_softbody
-from . import space_sequencer
-from . import properties_workspace
-from . import space_info
-from . import properties_data_light
-from . import properties_data_mesh
-from . import properties_mask_common
-from . import space_view3d
 from . import properties_data_armature
-from . import properties_texture
-from . import space_time
-from . import space_graph
-from . import space_spreadsheet
-from . import properties_data_camera
-from . import space_image
+from . import properties_physics_field
+from . import properties_physics_fluid
+from . import properties_data_empty
+from . import properties_physics_common
+from . import properties_data_modifier
+from . import properties_physics_geometry_nodes
+from . import properties_constraint
+from . import properties_data_curve
+from . import properties_view_layer
+from . import space_properties
+from . import node_add_menu
+from . import generic_ui_list
 from . import properties_physics_cloth
-from . import properties_data_lightprobe
-from . import properties_material
-from . import space_view3d_toolbar
 from . import utils
-from . import properties_world
-from . import properties_data_speaker
-from . import properties_physics_rigidbody_constraint
-from . import properties_collection
 from . import properties_data_volume
-from . import properties_material_gpencil
-from . import space_node
-from . import space_console
-from . import properties_physics_dynamicpaint
-from . import properties_constraint
-from . import properties_paint_common
+from . import properties_particle
 from . import properties_data_pointcloud
-from . import space_dopesheet
-from . import space_filebrowser
-from . import properties_data_empty
-from . import properties_data_shaderfx
+from . import properties_data_mesh
+from . import properties_texture
+from . import properties_workspace
 from . import properties_output
-from . import properties_view_layer
+from . import space_filebrowser
+from . import properties_data_camera
+from . import properties_scene
 from . import space_text
-from . import properties_data_modifier
+from . import properties_mask_common
 from . import properties_object
-from . import space_clip
-from . import properties_physics_field
-from . import space_statusbar
-from . import properties_data_metaball
-from . import properties_physics_fluid
+from . import space_sequencer
 from . import node_add_menu_geometry
-from . import properties_data_lattice
-from . import space_topbar
-from . import properties_particle
-from . import space_nla
-from . import properties_data_gpencil
-from . import properties_physics_common
+from . import space_view3d_toolbar
 from . import properties_data_curves
-from . import node_add_menu
+from . import properties_material_gpencil
+from . import space_node
+from . import space_userpref
 from . import properties_physics_rigidbody
-from . import space_toolsystem_common
-from . import generic_ui_list
-from . import properties_physics_geometry_nodes
+from . import properties_collection
+from . import properties_data_metaball
+from . import space_toolsystem_toolbar
+from . import properties_physics_dynamicpaint
+from . import properties_data_speaker
+from . import space_time
 from . import properties_freestyle
+from . import space_graph
+from . import space_image
+from . import properties_world
+from . import space_nla
+from . import properties_paint_common
+from . import properties_physics_rigidbody_constraint
+from . import properties_animviz
+from . import properties_data_light
+from . import properties_data_lightprobe
+from . import space_spreadsheet
+from . import space_dopesheet
+from . import space_view3d
+from . import space_clip
+from . import properties_material
+from . import space_console
 from . import properties_render
-from . import space_properties
+from . import properties_grease_pencil_common
+from . import space_info
+from . import space_statusbar
+from . import properties_data_bone
+from . import properties_data_shaderfx
+from . import space_toolsystem_common
+from . import properties_data_gpencil
+from . import space_outliner
+from . import space_topbar
+from . import properties_data_lattice
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230521/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230522/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230522/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_physics_geometry_nodes.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_physics_geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230522/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230522/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_console.py` & `fake-bpy-module-latest-20230522/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230522/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230522/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230522/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_image.py` & `fake-bpy-module-latest-20230522/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_info.py` & `fake-bpy-module-latest-20230522/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230522/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_node.py` & `fake-bpy-module-latest-20230522/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230522/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230522/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230522/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230522/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230522/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_text.py` & `fake-bpy-module-latest-20230522/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_time.py` & `fake-bpy-module-latest-20230522/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230522/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230522/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230522/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230522/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230522/bl_ui/space_view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230522/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bl_ui/utils.py` & `fake-bpy-module-latest-20230522/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/blf.py` & `fake-bpy-module-latest-20230522/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bmesh/__init__.py` & `fake-bpy-module-latest-20230522/bmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bmesh/geometry.py` & `fake-bpy-module-latest-20230522/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bmesh/ops.py` & `fake-bpy-module-latest-20230522/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bmesh/types.py` & `fake-bpy-module-latest-20230522/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bmesh/utils.py` & `fake-bpy-module-latest-20230522/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/app/__init__.py` & `fake-bpy-module-latest-20230522/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
-from . import handlers
-from . import timers
 from . import icons
 from . import translations
+from . import handlers
+from . import timers
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def is_job_running(job_type: typing.Optional[str]) -> typing.Any:
     ''' Check whether a job of the given type is running.
```

### Comparing `fake-bpy-module-latest-20230521/bpy/app/handlers.py` & `fake-bpy-module-latest-20230522/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/app/icons.py` & `fake-bpy-module-latest-20230522/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/app/timers.py` & `fake-bpy-module-latest-20230522/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/app/translations.py` & `fake-bpy-module-latest-20230522/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/msgbus.py` & `fake-bpy-module-latest-20230522/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230522/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 import sys
 import typing
-from . import material
-from . import object
-from . import boid
-from . import world
-from . import poselib
-from . import sculpt_curves
-from . import ed
-from . import buttons
-from . import paint
-from . import clip
-from . import action
-from . import fluid
-from . import sequencer
-from . import sculpt
-from . import node
-from . import file
-from . import particle
-from . import dpaint
+from . import collection
+from . import render
+from . import gpencil
 from . import brush
-from . import console
+from . import clip
+from . import curve
+from . import cloth
+from . import spreadsheet
+from . import outliner
+from . import uv
 from . import anim
-from . import scene
-from . import import_anim
+from . import uilist
 from . import marker
-from . import gizmogroup
-from . import screen
+from . import world
+from . import export_anim
+from . import export_scene
+from . import ptcache
+from . import particle
+from . import fluid
+from . import wm
+from . import pose
+from . import palette
+from . import import_curve
+from . import object
 from . import mask
-from . import collection
-from . import spreadsheet
-from . import curve
-from . import info
-from . import outliner
-from . import armature
-from . import surface
-from . import cachefile
-from . import rigidbody
 from . import ui
-from . import preferences
-from . import paintcurve
-from . import transform
+from . import rigidbody
+from . import buttons
+from . import material
+from . import text
+from . import scene
 from . import asset
-from . import curves
-from . import import_mesh
-from . import texture
+from . import constraint
+from . import file
 from . import mball
 from . import cycles
+from . import import_mesh
+from . import sculpt
+from . import preferences
+from . import console
+from . import action
+from . import nla
+from . import export_mesh
+from . import import_anim
 from . import sound
+from . import import_scene
 from . import workspace
-from . import camera
-from . import view3d
-from . import graph
-from . import font
-from . import pose
-from . import cloth
-from . import text
-from . import ptcache
 from . import view2d
-from . import geometry
-from . import lattice
-from . import wm
-from . import palette
-from . import script
-from . import gpencil
 from . import image
-from . import export_scene
-from . import uv
-from . import export_anim
-from . import export_mesh
-from . import nla
-from . import import_scene
+from . import paintcurve
 from . import mesh
-from . import render
-from . import uilist
-from . import import_curve
-from . import constraint
+from . import paint
+from . import poselib
+from . import texture
+from . import graph
+from . import ed
+from . import sequencer
+from . import sculpt_curves
+from . import lattice
+from . import node
+from . import curves
+from . import view3d
+from . import screen
+from . import gizmogroup
+from . import geometry
+from . import cachefile
+from . import script
+from . import transform
+from . import info
+from . import dpaint
+from . import armature
+from . import camera
+from . import font
+from . import surface
+from . import boid
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/action.py` & `fake-bpy-module-latest-20230522/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/anim.py` & `fake-bpy-module-latest-20230522/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/armature.py` & `fake-bpy-module-latest-20230522/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/asset.py` & `fake-bpy-module-latest-20230522/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/boid.py` & `fake-bpy-module-latest-20230522/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/brush.py` & `fake-bpy-module-latest-20230522/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230522/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230522/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/camera.py` & `fake-bpy-module-latest-20230522/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/clip.py` & `fake-bpy-module-latest-20230522/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230522/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/collection.py` & `fake-bpy-module-latest-20230522/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/console.py` & `fake-bpy-module-latest-20230522/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230522/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/curve.py` & `fake-bpy-module-latest-20230522/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/curves.py` & `fake-bpy-module-latest-20230522/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230522/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230522/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/ed.py` & `fake-bpy-module-latest-20230522/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230522/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230522/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230522/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/file.py` & `fake-bpy-module-latest-20230522/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230522/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/font.py` & `fake-bpy-module-latest-20230522/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230522/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230522/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230522/bpy/ops/gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/graph.py` & `fake-bpy-module-latest-20230522/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/image.py` & `fake-bpy-module-latest-20230522/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230522/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230522/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230522/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230522/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/info.py` & `fake-bpy-module-latest-20230522/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230522/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/marker.py` & `fake-bpy-module-latest-20230522/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/mask.py` & `fake-bpy-module-latest-20230522/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/material.py` & `fake-bpy-module-latest-20230522/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/mball.py` & `fake-bpy-module-latest-20230522/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230522/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/nla.py` & `fake-bpy-module-latest-20230522/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/node.py` & `fake-bpy-module-latest-20230522/bpy/ops/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/object.py` & `fake-bpy-module-latest-20230522/bpy/ops/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230522/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/paint.py` & `fake-bpy-module-latest-20230522/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230522/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/palette.py` & `fake-bpy-module-latest-20230522/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/particle.py` & `fake-bpy-module-latest-20230522/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/pose.py` & `fake-bpy-module-latest-20230522/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230522/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230522/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230522/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/render.py` & `fake-bpy-module-latest-20230522/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230522/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/scene.py` & `fake-bpy-module-latest-20230522/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/screen.py` & `fake-bpy-module-latest-20230522/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/script.py` & `fake-bpy-module-latest-20230522/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230522/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230522/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230522/bpy/ops/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/sound.py` & `fake-bpy-module-latest-20230522/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230522/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/surface.py` & `fake-bpy-module-latest-20230522/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/text.py` & `fake-bpy-module-latest-20230522/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/texture.py` & `fake-bpy-module-latest-20230522/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/transform.py` & `fake-bpy-module-latest-20230522/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/ui.py` & `fake-bpy-module-latest-20230522/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230522/bpy/ops/uilist.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/uv.py` & `fake-bpy-module-latest-20230522/bpy/ops/uv.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230522/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230522/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/wm.py` & `fake-bpy-module-latest-20230522/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230522/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/ops/world.py` & `fake-bpy-module-latest-20230522/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/path.py` & `fake-bpy-module-latest-20230522/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/props.py` & `fake-bpy-module-latest-20230522/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/types.py` & `fake-bpy-module-latest-20230522/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,1053 +1,1053 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
 00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
-00000040: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000050: 615f 6375 7276 650a 696d 706f 7274 2062  a_curve.import b
-00000060: 6c5f 7569 2e73 7061 6365 5f6f 7574 6c69  l_ui.space_outli
-00000070: 6e65 720a 696d 706f 7274 2062 6c5f 7569  ner.import bl_ui
-00000080: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-00000090: 5f62 6f6e 650a 696d 706f 7274 2062 6c5f  _bone.import bl_
-000000a0: 7569 2e73 7061 6365 5f74 6f6f 6c73 7973  ui.space_toolsys
-000000b0: 7465 6d5f 746f 6f6c 6261 720a 696d 706f  tem_toolbar.impo
-000000c0: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
-000000d0: 6672 6565 7374 796c 650a 696d 706f 7274  freestyle.import
-000000e0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000000f0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00000100: 636f 6d6d 6f6e 0a69 6d70 6f72 7420 626c  common.import bl
-00000110: 5f75 692e 7370 6163 655f 7573 6572 7072  _ui.space_userpr
-00000120: 6566 0a69 6d70 6f72 7420 626c 5f75 692e  ef.import bl_ui.
-00000130: 7072 6f70 6572 7469 6573 5f73 6365 6e65  properties_scene
-00000140: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000150: 6f70 6572 7469 6573 5f70 6879 7369 6373  operties_physics
-00000160: 5f73 6f66 7462 6f64 790a 696d 706f 7274  _softbody.import
-00000170: 2062 6c5f 7569 2e73 7061 6365 5f73 6571   bl_ui.space_seq
-00000180: 7565 6e63 6572 0a69 6d70 6f72 7420 626c  uencer.import bl
-00000190: 5f75 692e 7072 6f70 6572 7469 6573 5f77  _ui.properties_w
-000001a0: 6f72 6b73 7061 6365 0a69 6d70 6f72 7420  orkspace.import 
-000001b0: 626c 5f75 692e 7370 6163 655f 696e 666f  bl_ui.space_info
-000001c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000001d0: 6f70 6572 7469 6573 5f64 6174 615f 6c69  operties_data_li
-000001e0: 6768 740a 696d 706f 7274 2062 6c5f 7569  ght.import bl_ui
-000001f0: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-00000200: 5f6d 6573 680a 696d 706f 7274 2062 6c5f  _mesh.import bl_
-00000210: 6f70 6572 6174 6f72 732e 6f62 6a65 6374  operators.object
-00000220: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000230: 6f70 6572 7469 6573 5f6d 6173 6b5f 636f  operties_mask_co
-00000240: 6d6d 6f6e 0a69 6d70 6f72 7420 626c 5f75  mmon.import bl_u
-00000250: 692e 7370 6163 655f 7669 6577 3364 0a69  i.space_view3d.i
-00000260: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000270: 6572 7469 6573 5f64 6174 615f 6172 6d61  erties_data_arma
-00000280: 7475 7265 0a69 6d70 6f72 7420 626c 5f6f  ture.import bl_o
-00000290: 7065 7261 746f 7273 2e63 6f6e 7374 7261  perators.constra
-000002a0: 696e 740a 696d 706f 7274 2062 6c5f 7569  int.import bl_ui
-000002b0: 2e70 726f 7065 7274 6965 735f 7465 7874  .properties_text
-000002c0: 7572 650a 696d 706f 7274 2062 6c5f 7569  ure.import bl_ui
-000002d0: 2e73 7061 6365 5f74 696d 650a 696d 706f  .space_time.impo
-000002e0: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
-000002f0: 6173 7365 7473 0a69 6d70 6f72 7420 626c  assets.import bl
-00000300: 5f75 692e 7370 6163 655f 6772 6170 680a  _ui.space_graph.
-00000310: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000320: 6365 5f73 7072 6561 6473 6865 6574 0a69  ce_spreadsheet.i
-00000330: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000340: 6572 7469 6573 5f64 6174 615f 6361 6d65  erties_data_came
-00000350: 7261 0a69 6d70 6f72 7420 626c 5f75 692e  ra.import bl_ui.
-00000360: 7370 6163 655f 696d 6167 650a 696d 706f  space_image.impo
-00000370: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000380: 6965 735f 7068 7973 6963 735f 636c 6f74  ies_physics_clot
-00000390: 680a 696d 706f 7274 2062 6c5f 6f70 6572  h.import bl_oper
-000003a0: 6174 6f72 732e 7669 6577 3364 0a69 6d70  ators.view3d.imp
-000003b0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000003c0: 7469 6573 5f64 6174 615f 6c69 6768 7470  ties_data_lightp
-000003d0: 726f 6265 0a69 6d70 6f72 7420 626c 5f75  robe.import bl_u
-000003e0: 692e 7072 6f70 6572 7469 6573 5f6d 6174  i.properties_mat
-000003f0: 6572 6961 6c0a 696d 706f 7274 2062 6c5f  erial.import bl_
-00000400: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00000410: 746f 6f6c 6261 720a 696d 706f 7274 2062  toolbar.import b
-00000420: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000430: 776f 726c 640a 696d 706f 7274 2062 6c5f  world.import bl_
-00000440: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
-00000450: 7461 5f73 7065 616b 6572 0a69 6d70 6f72  ta_speaker.impor
-00000460: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000470: 6573 5f70 6879 7369 6373 5f72 6967 6964  es_physics_rigid
-00000480: 626f 6479 5f63 6f6e 7374 7261 696e 740a  body_constraint.
-00000490: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-000004a0: 7065 7274 6965 735f 636f 6c6c 6563 7469  perties_collecti
-000004b0: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
-000004c0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-000004d0: 766f 6c75 6d65 0a69 6d70 6f72 7420 626c  volume.import bl
-000004e0: 5f75 692e 7072 6f70 6572 7469 6573 5f6d  _ui.properties_m
-000004f0: 6174 6572 6961 6c5f 6770 656e 6369 6c0a  aterial_gpencil.
-00000500: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000510: 6365 5f6e 6f64 650a 696d 706f 7274 2062  ce_node.import b
-00000520: 6c5f 7569 2e73 7061 6365 5f63 6f6e 736f  l_ui.space_conso
-00000530: 6c65 0a69 6d70 6f72 7420 626c 5f75 692e  le.import bl_ui.
-00000540: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
-00000550: 6373 5f64 796e 616d 6963 7061 696e 740a  cs_dynamicpaint.
-00000560: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000570: 7065 7274 6965 735f 636f 6e73 7472 6169  perties_constrai
-00000580: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
-00000590: 7072 6f70 6572 7469 6573 5f70 6169 6e74  properties_paint
-000005a0: 5f63 6f6d 6d6f 6e0a 696d 706f 7274 2062  _common.import b
-000005b0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000005c0: 6461 7461 5f70 6f69 6e74 636c 6f75 640a  data_pointcloud.
-000005d0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000005e0: 6365 5f64 6f70 6573 6865 6574 0a69 6d70  ce_dopesheet.imp
-000005f0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000600: 6669 6c65 6272 6f77 7365 720a 696d 706f  filebrowser.impo
-00000610: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000620: 6965 735f 6461 7461 5f65 6d70 7479 0a69  ies_data_empty.i
-00000630: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000640: 6572 7469 6573 5f64 6174 615f 7368 6164  erties_data_shad
-00000650: 6572 6678 0a69 6d70 6f72 7420 626c 5f75  erfx.import bl_u
-00000660: 692e 7072 6f70 6572 7469 6573 5f6f 7574  i.properties_out
-00000670: 7075 740a 696d 706f 7274 2062 6c5f 7569  put.import bl_ui
-00000680: 2e70 726f 7065 7274 6965 735f 7669 6577  .properties_view
-00000690: 5f6c 6179 6572 0a69 6d70 6f72 7420 626c  _layer.import bl
-000006a0: 5f75 692e 7370 6163 655f 7465 7874 0a69  _ui.space_text.i
-000006b0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000006c0: 6572 7469 6573 5f64 6174 615f 6d6f 6469  erties_data_modi
-000006d0: 6669 6572 0a69 6d70 6f72 7420 626c 5f75  fier.import bl_u
-000006e0: 692e 7072 6f70 6572 7469 6573 5f6f 626a  i.properties_obj
-000006f0: 6563 740a 696d 706f 7274 2062 6c5f 7569  ect.import bl_ui
-00000700: 2e73 7061 6365 5f63 6c69 700a 696d 706f  .space_clip.impo
-00000710: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000720: 6965 735f 7068 7973 6963 735f 6669 656c  ies_physics_fiel
-00000730: 640a 696d 706f 7274 2062 6c5f 7569 2e73  d.import bl_ui.s
-00000740: 7061 6365 5f73 7461 7475 7362 6172 0a69  pace_statusbar.i
-00000750: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000760: 6572 7469 6573 5f64 6174 615f 6d65 7461  erties_data_meta
-00000770: 6261 6c6c 0a69 6d70 6f72 7420 626c 5f75  ball.import bl_u
-00000780: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-00000790: 7369 6373 5f66 6c75 6964 0a69 6d70 6f72  sics_fluid.impor
-000007a0: 7420 626c 5f75 692e 6e6f 6465 5f61 6464  t bl_ui.node_add
-000007b0: 5f6d 656e 755f 6765 6f6d 6574 7279 0a69  _menu_geometry.i
-000007c0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000007d0: 6572 7469 6573 5f64 6174 615f 6c61 7474  erties_data_latt
-000007e0: 6963 650a 696d 706f 7274 2062 6c5f 6f70  ice.import bl_op
-000007f0: 6572 6174 6f72 732e 616e 696d 0a69 6d70  erators.anim.imp
-00000800: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000810: 746f 7062 6172 0a69 6d70 6f72 7420 626c  topbar.import bl
-00000820: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
-00000830: 6172 7469 636c 650a 696d 706f 7274 2062  article.import b
-00000840: 6c5f 7569 2e73 7061 6365 5f6e 6c61 0a69  l_ui.space_nla.i
-00000850: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-00000860: 7273 2e77 6d0a 696d 706f 7274 2062 6c5f  rs.wm.import bl_
-00000870: 6f70 6572 6174 6f72 732e 7072 6573 6574  operators.preset
-00000880: 730a 696d 706f 7274 2062 6c5f 7569 2e70  s.import bl_ui.p
-00000890: 726f 7065 7274 6965 735f 6461 7461 5f67  roperties_data_g
-000008a0: 7065 6e63 696c 0a69 6d70 6f72 7420 626c  pencil.import bl
-000008b0: 5f6f 7065 7261 746f 7273 2e73 7072 6561  _operators.sprea
-000008c0: 6473 6865 6574 0a69 6d70 6f72 7420 626c  dsheet.import bl
-000008d0: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
-000008e0: 6879 7369 6373 5f63 6f6d 6d6f 6e0a 696d  hysics_common.im
-000008f0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000900: 7274 6965 735f 6461 7461 5f63 7572 7665  rties_data_curve
-00000910: 730a 696d 706f 7274 2062 6c5f 6f70 6572  s.import bl_oper
-00000920: 6174 6f72 732e 6e6f 6465 0a69 6d70 6f72  ators.node.impor
-00000930: 7420 626c 5f6f 7065 7261 746f 7273 2e75  t bl_operators.u
-00000940: 7365 7270 7265 660a 696d 706f 7274 2062  serpref.import b
-00000950: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000960: 7068 7973 6963 735f 7269 6769 6462 6f64  physics_rigidbod
-00000970: 790a 696d 706f 7274 2062 6c5f 7569 2e73  y.import bl_ui.s
-00000980: 7061 6365 5f74 6f6f 6c73 7973 7465 6d5f  pace_toolsystem_
-00000990: 636f 6d6d 6f6e 0a69 6d70 6f72 7420 626c  common.import bl
-000009a0: 5f75 690a 696d 706f 7274 2062 6c5f 7569  _ui.import bl_ui
-000009b0: 2e67 656e 6572 6963 5f75 695f 6c69 7374  .generic_ui_list
-000009c0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-000009d0: 746f 7273 2e66 696c 650a 696d 706f 7274  tors.file.import
-000009e0: 2062 6c5f 6f70 6572 6174 6f72 732e 636c   bl_operators.cl
-000009f0: 6970 0a69 6d70 6f72 7420 626c 5f75 692e  ip.import bl_ui.
-00000a00: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
-00000a10: 6373 5f67 656f 6d65 7472 795f 6e6f 6465  cs_geometry_node
-00000a20: 730a 696d 706f 7274 2062 6c5f 7569 2e70  s.import bl_ui.p
-00000a30: 726f 7065 7274 6965 735f 6672 6565 7374  roperties_freest
-00000a40: 796c 650a 696d 706f 7274 2062 6c5f 7569  yle.import bl_ui
-00000a50: 2e70 726f 7065 7274 6965 735f 7265 6e64  .properties_rend
-00000a60: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
-00000a70: 7370 6163 655f 7072 6f70 6572 7469 6573  space_properties
+00000040: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
+00000050: 7369 6373 5f73 6f66 7462 6f64 790a 696d  sics_softbody.im
+00000060: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
+00000070: 732e 636c 6970 0a69 6d70 6f72 7420 626c  s.clip.import bl
+00000080: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000090: 6174 615f 6172 6d61 7475 7265 0a69 6d70  ata_armature.imp
+000000a0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000000b0: 7469 6573 5f70 6879 7369 6373 5f66 6965  ties_physics_fie
+000000c0: 6c64 0a69 6d70 6f72 7420 626c 5f6f 7065  ld.import bl_ope
+000000d0: 7261 746f 7273 2e66 696c 650a 696d 706f  rators.file.impo
+000000e0: 7274 2062 6c5f 7569 0a69 6d70 6f72 7420  rt bl_ui.import 
+000000f0: 626c 5f6f 7065 7261 746f 7273 2e75 7365  bl_operators.use
+00000100: 7270 7265 660a 696d 706f 7274 2062 6c5f  rpref.import bl_
+00000110: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
+00000120: 7973 6963 735f 666c 7569 640a 696d 706f  ysics_fluid.impo
+00000130: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000140: 6965 735f 6461 7461 5f65 6d70 7479 0a69  ies_data_empty.i
+00000150: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000160: 6572 7469 6573 5f70 6879 7369 6373 5f63  erties_physics_c
+00000170: 6f6d 6d6f 6e0a 696d 706f 7274 2062 6c5f  ommon.import bl_
+00000180: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+00000190: 7461 5f6d 6f64 6966 6965 720a 696d 706f  ta_modifier.impo
+000001a0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000001b0: 6965 735f 7068 7973 6963 735f 6765 6f6d  ies_physics_geom
+000001c0: 6574 7279 5f6e 6f64 6573 0a69 6d70 6f72  etry_nodes.impor
+000001d0: 7420 626c 5f6f 7065 7261 746f 7273 2e61  t bl_operators.a
+000001e0: 7373 6574 730a 696d 706f 7274 2062 6c5f  ssets.import bl_
+000001f0: 7569 2e70 726f 7065 7274 6965 735f 636f  ui.properties_co
+00000200: 6e73 7472 6169 6e74 0a69 6d70 6f72 7420  nstraint.import 
+00000210: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000220: 5f64 6174 615f 6375 7276 650a 696d 706f  _data_curve.impo
+00000230: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000240: 6965 735f 7669 6577 5f6c 6179 6572 0a69  ies_view_layer.i
+00000250: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+00000260: 7273 2e61 6e69 6d0a 696d 706f 7274 2062  rs.anim.import b
+00000270: 6c5f 7569 2e73 7061 6365 5f70 726f 7065  l_ui.space_prope
+00000280: 7274 6965 730a 696d 706f 7274 2062 6c5f  rties.import bl_
+00000290: 6f70 6572 6174 6f72 732e 636f 6e73 7472  operators.constr
+000002a0: 6169 6e74 0a69 6d70 6f72 7420 626c 5f75  aint.import bl_u
+000002b0: 692e 6765 6e65 7269 635f 7569 5f6c 6973  i.generic_ui_lis
+000002c0: 740a 696d 706f 7274 2062 6c5f 7569 2e70  t.import bl_ui.p
+000002d0: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
+000002e0: 735f 636c 6f74 680a 696d 706f 7274 2062  s_cloth.import b
+000002f0: 6c5f 6f70 6572 6174 6f72 732e 6672 6565  l_operators.free
+00000300: 7374 796c 650a 696d 706f 7274 2062 6c5f  style.import bl_
+00000310: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+00000320: 7461 5f76 6f6c 756d 650a 696d 706f 7274  ta_volume.import
+00000330: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000340: 735f 7061 7274 6963 6c65 0a69 6d70 6f72  s_particle.impor
+00000350: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000360: 6573 5f64 6174 615f 706f 696e 7463 6c6f  es_data_pointclo
+00000370: 7564 0a69 6d70 6f72 7420 626c 5f75 692e  ud.import bl_ui.
+00000380: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+00000390: 6d65 7368 0a69 6d70 6f72 7420 626c 5f75  mesh.import bl_u
+000003a0: 692e 7072 6f70 6572 7469 6573 5f74 6578  i.properties_tex
+000003b0: 7475 7265 0a69 6d70 6f72 7420 626c 5f75  ture.import bl_u
+000003c0: 692e 7072 6f70 6572 7469 6573 5f77 6f72  i.properties_wor
+000003d0: 6b73 7061 6365 0a69 6d70 6f72 7420 626c  kspace.import bl
+000003e0: 5f6f 7065 7261 746f 7273 2e6e 6f64 650a  _operators.node.
+000003f0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000400: 7065 7274 6965 735f 6f75 7470 7574 0a69  perties_output.i
+00000410: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000420: 655f 6669 6c65 6272 6f77 7365 720a 696d  e_filebrowser.im
+00000430: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000440: 7274 6965 735f 6461 7461 5f63 616d 6572  rties_data_camer
+00000450: 610a 696d 706f 7274 2062 6c5f 7569 2e70  a.import bl_ui.p
+00000460: 726f 7065 7274 6965 735f 7363 656e 650a  roperties_scene.
+00000470: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+00000480: 6365 5f74 6578 740a 696d 706f 7274 2062  ce_text.import b
+00000490: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+000004a0: 6d61 736b 5f63 6f6d 6d6f 6e0a 696d 706f  mask_common.impo
+000004b0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000004c0: 6965 735f 6f62 6a65 6374 0a69 6d70 6f72  ies_object.impor
+000004d0: 7420 626c 5f6f 7065 7261 746f 7273 2e6f  t bl_operators.o
+000004e0: 626a 6563 740a 696d 706f 7274 2062 6c5f  bject.import bl_
+000004f0: 7569 2e73 7061 6365 5f73 6571 7565 6e63  ui.space_sequenc
+00000500: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
+00000510: 6e6f 6465 5f61 6464 5f6d 656e 755f 6765  node_add_menu_ge
+00000520: 6f6d 6574 7279 0a69 6d70 6f72 7420 626c  ometry.import bl
+00000530: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00000540: 5f74 6f6f 6c62 6172 0a69 6d70 6f72 7420  _toolbar.import 
+00000550: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000560: 5f64 6174 615f 6375 7276 6573 0a69 6d70  _data_curves.imp
+00000570: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000580: 7469 6573 5f6d 6174 6572 6961 6c5f 6770  ties_material_gp
+00000590: 656e 6369 6c0a 696d 706f 7274 2062 6c5f  encil.import bl_
+000005a0: 7569 2e73 7061 6365 5f6e 6f64 650a 696d  ui.space_node.im
+000005b0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+000005c0: 5f75 7365 7270 7265 660a 696d 706f 7274  _userpref.import
+000005d0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+000005e0: 735f 7068 7973 6963 735f 7269 6769 6462  s_physics_rigidb
+000005f0: 6f64 790a 696d 706f 7274 2062 6c5f 7569  ody.import bl_ui
+00000600: 2e70 726f 7065 7274 6965 735f 636f 6c6c  .properties_coll
+00000610: 6563 7469 6f6e 0a69 6d70 6f72 7420 626c  ection.import bl
+00000620: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000630: 6174 615f 6d65 7461 6261 6c6c 0a69 6d70  ata_metaball.imp
+00000640: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000650: 746f 6f6c 7379 7374 656d 5f74 6f6f 6c62  toolsystem_toolb
+00000660: 6172 0a69 6d70 6f72 7420 626c 5f75 692e  ar.import bl_ui.
+00000670: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
+00000680: 6373 5f64 796e 616d 6963 7061 696e 740a  cs_dynamicpaint.
+00000690: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+000006a0: 7065 7274 6965 735f 6461 7461 5f73 7065  perties_data_spe
+000006b0: 616b 6572 0a69 6d70 6f72 7420 626c 5f6f  aker.import bl_o
+000006c0: 7065 7261 746f 7273 2e77 6d0a 696d 706f  perators.wm.impo
+000006d0: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+000006e0: 7370 7265 6164 7368 6565 740a 696d 706f  spreadsheet.impo
+000006f0: 7274 2062 6c5f 7569 2e73 7061 6365 5f74  rt bl_ui.space_t
+00000700: 696d 650a 696d 706f 7274 2062 6c5f 7569  ime.import bl_ui
+00000710: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
+00000720: 7374 796c 650a 696d 706f 7274 2062 6c5f  style.import bl_
+00000730: 7569 2e73 7061 6365 5f67 7261 7068 0a69  ui.space_graph.i
+00000740: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000750: 655f 696d 6167 650a 696d 706f 7274 2062  e_image.import b
+00000760: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000770: 776f 726c 640a 696d 706f 7274 2062 6c5f  world.import bl_
+00000780: 7569 2e73 7061 6365 5f6e 6c61 0a69 6d70  ui.space_nla.imp
+00000790: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000007a0: 7469 6573 5f70 6169 6e74 5f63 6f6d 6d6f  ties_paint_commo
+000007b0: 6e0a 696d 706f 7274 2062 6c5f 7569 2e70  n.import bl_ui.p
+000007c0: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
+000007d0: 735f 7269 6769 6462 6f64 795f 636f 6e73  s_rigidbody_cons
+000007e0: 7472 6169 6e74 0a69 6d70 6f72 7420 626c  traint.import bl
+000007f0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000800: 6174 615f 6c69 6768 740a 696d 706f 7274  ata_light.import
+00000810: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000820: 735f 6461 7461 5f6c 6967 6874 7072 6f62  s_data_lightprob
+00000830: 650a 696d 706f 7274 2062 6c5f 7569 2e73  e.import bl_ui.s
+00000840: 7061 6365 5f73 7072 6561 6473 6865 6574  pace_spreadsheet
+00000850: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+00000860: 6163 655f 646f 7065 7368 6565 740a 696d  ace_dopesheet.im
+00000870: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000880: 5f76 6965 7733 640a 696d 706f 7274 2062  _view3d.import b
+00000890: 6c5f 6f70 6572 6174 6f72 732e 7072 6573  l_operators.pres
+000008a0: 6574 730a 696d 706f 7274 2062 6c5f 7569  ets.import bl_ui
+000008b0: 2e73 7061 6365 5f63 6c69 700a 696d 706f  .space_clip.impo
+000008c0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000008d0: 6965 735f 6d61 7465 7269 616c 0a69 6d70  ies_material.imp
+000008e0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+000008f0: 636f 6e73 6f6c 650a 696d 706f 7274 2062  console.import b
+00000900: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000910: 7265 6e64 6572 0a69 6d70 6f72 7420 626c  render.import bl
+00000920: 5f75 692e 7072 6f70 6572 7469 6573 5f67  _ui.properties_g
+00000930: 7265 6173 655f 7065 6e63 696c 5f63 6f6d  rease_pencil_com
+00000940: 6d6f 6e0a 696d 706f 7274 2062 6c5f 7569  mon.import bl_ui
+00000950: 2e73 7061 6365 5f69 6e66 6f0a 696d 706f  .space_info.impo
+00000960: 7274 2062 6c5f 7569 2e73 7061 6365 5f73  rt bl_ui.space_s
+00000970: 7461 7475 7362 6172 0a69 6d70 6f72 7420  tatusbar.import 
+00000980: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000990: 5f64 6174 615f 626f 6e65 0a69 6d70 6f72  _data_bone.impor
+000009a0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000009b0: 6573 5f64 6174 615f 7368 6164 6572 6678  es_data_shaderfx
+000009c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+000009d0: 6163 655f 746f 6f6c 7379 7374 656d 5f63  ace_toolsystem_c
+000009e0: 6f6d 6d6f 6e0a 696d 706f 7274 2062 6c5f  ommon.import bl_
+000009f0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+00000a00: 7461 5f67 7065 6e63 696c 0a69 6d70 6f72  ta_gpencil.impor
+00000a10: 7420 626c 5f75 692e 7370 6163 655f 6f75  t bl_ui.space_ou
+00000a20: 746c 696e 6572 0a69 6d70 6f72 7420 626c  tliner.import bl
+00000a30: 5f75 692e 7370 6163 655f 746f 7062 6172  _ui.space_topbar
+00000a40: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
+00000a50: 746f 7273 2e76 6965 7733 640a 696d 706f  tors.view3d.impo
+00000a60: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000a70: 6965 735f 6461 7461 5f6c 6174 7469 6365  ies_data_lattice
 00000a80: 0a0a 4765 6e65 7269 6354 7970 6520 3d20  ..GenericType = 
 00000a90: 7479 7069 6e67 2e54 7970 6556 6172 2822  typing.TypeVar("
 00000aa0: 4765 6e65 7269 6354 7970 6522 290a 0a0a  GenericType")...
-00000ab0: 636c 6173 7320 6270 795f 7374 7275 6374  class bpy_struct
-00000ac0: 3a0a 2020 2020 2727 2720 6275 696c 742d  :.    ''' built-
-00000ad0: 696e 2062 6173 6520 636c 6173 7320 666f  in base class fo
-00000ae0: 7220 616c 6c20 636c 6173 7365 7320 696e  r all classes in
-00000af0: 2062 7079 2e74 7970 6573 2e0a 2020 2020   bpy.types..    
-00000b00: 2727 270a 0a20 2020 2069 645f 6461 7461  '''..    id_data
-00000b10: 203d 204e 6f6e 650a 2020 2020 2727 2720   = None.    ''' 
-00000b20: 5468 6520 6062 7079 2e74 7970 6573 2e49  The `bpy.types.I
-00000b30: 4460 206f 626a 6563 7420 7468 6973 2064  D` object this d
-00000b40: 6174 6162 6c6f 636b 2069 7320 6672 6f6d  atablock is from
-00000b50: 206f 7220 4e6f 6e65 2c20 286e 6f74 2061   or None, (not a
-00000b60: 7661 696c 6162 6c65 2066 6f72 2061 6c6c  vailable for all
-00000b70: 2064 6174 6120 7479 7065 7329 2727 270a   data types)'''.
-00000b80: 0a20 2020 2064 6566 2061 735f 706f 696e  .    def as_poin
-00000b90: 7465 7228 7365 6c66 2920 2d3e 2069 6e74  ter(self) -> int
-00000ba0: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
-00000bb0: 7475 726e 7320 7468 6520 6d65 6d6f 7279  turns the memory
-00000bc0: 2061 6464 7265 7373 2077 6869 6368 2068   address which h
-00000bd0: 6f6c 6473 2061 2070 6f69 6e74 6572 2074  olds a pointer t
-00000be0: 6f20 426c 656e 6465 7227 7320 696e 7465  o Blender's inte
-00000bf0: 726e 616c 2064 6174 610a 0a20 2020 2020  rnal data..     
-00000c00: 2020 203a 7274 7970 653a 2069 6e74 0a20     :rtype: int. 
-00000c10: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00000c20: 696e 7420 286d 656d 6f72 7920 6164 6472  int (memory addr
-00000c30: 6573 7329 2e0a 2020 2020 2020 2020 2727  ess)..        ''
-00000c40: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00000c50: 2020 2020 6465 6620 6472 6976 6572 5f61      def driver_a
-00000c60: 6464 2873 656c 662c 0a20 2020 2020 2020  dd(self,.       
-00000c70: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00000c80: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00000c90: 6c5b 7374 725d 2c0a 2020 2020 2020 2020  l[str],.        
-00000ca0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00000cb0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00000cc0: 6c5b 696e 745d 203d 202d 3129 202d 3e20  l[int] = -1) -> 
-00000cd0: 2746 4375 7276 6527 3a0a 2020 2020 2020  'FCurve':.      
-00000ce0: 2020 2727 2720 4164 6473 2064 7269 7665    ''' Adds drive
-00000cf0: 7228 7329 2074 6f20 7468 6520 6769 7665  r(s) to the give
-00000d00: 6e20 7072 6f70 6572 7479 0a0a 2020 2020  n property..    
-00000d10: 2020 2020 3a70 6172 616d 2070 6174 683a      :param path:
-00000d20: 2070 6174 6820 746f 2074 6865 2070 726f   path to the pro
-00000d30: 7065 7274 7920 746f 2064 7269 7665 2c20  perty to drive, 
-00000d40: 616e 616c 6f67 6f75 7320 746f 2074 6865  analogous to the
-00000d50: 2066 6375 7276 6527 7320 6461 7461 2070   fcurve's data p
-00000d60: 6174 682e 0a20 2020 2020 2020 203a 7479  ath..        :ty
-00000d70: 7065 2070 6174 683a 2074 7970 696e 672e  pe path: typing.
-00000d80: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
-00000d90: 2020 2020 2020 3a70 6172 616d 2069 6e64        :param ind
-00000da0: 6578 3a20 6172 7261 7920 696e 6465 7820  ex: array index 
-00000db0: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
-00000dc0: 6472 6976 652e 2044 6566 6175 6c74 7320  drive. Defaults 
-00000dd0: 746f 202d 3120 666f 7220 616c 6c20 696e  to -1 for all in
-00000de0: 6469 6365 7320 6f72 2061 2073 696e 676c  dices or a singl
-00000df0: 6520 6368 616e 6e65 6c20 6966 2074 6865  e channel if the
-00000e00: 2070 726f 7065 7274 7920 6973 206e 6f74   property is not
-00000e10: 2061 6e20 6172 7261 792e 0a20 2020 2020   an array..     
-00000e20: 2020 203a 7479 7065 2069 6e64 6578 3a20     :type index: 
-00000e30: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00000e40: 696e 745d 0a20 2020 2020 2020 203a 7274  int].        :rt
-00000e50: 7970 653a 2027 4643 7572 7665 270a 2020  ype: 'FCurve'.  
-00000e60: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
-00000e70: 6865 2064 7269 7665 7228 7329 2061 6464  he driver(s) add
-00000e80: 6564 2e0a 2020 2020 2020 2020 2727 270a  ed..        '''.
-00000e90: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00000ea0: 2020 6465 6620 6472 6976 6572 5f72 656d    def driver_rem
-00000eb0: 6f76 6528 7365 6c66 2c0a 2020 2020 2020  ove(self,.      
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 7061 7468 3a20 7479 7069 6e67 2e4f 7074  path: typing.Opt
-00000ee0: 696f 6e61 6c5b 7374 725d 2c0a 2020 2020  ional[str],.    
-00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f00: 2020 696e 6465 783a 2074 7970 696e 672e    index: typing.
-00000f10: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00000f20: 2d31 2920 2d3e 2062 6f6f 6c3a 0a20 2020  -1) -> bool:.   
-00000f30: 2020 2020 2027 2727 2052 656d 6f76 6520       ''' Remove 
-00000f40: 6472 6976 6572 2873 2920 6672 6f6d 2074  driver(s) from t
-00000f50: 6865 2067 6976 656e 2070 726f 7065 7274  he given propert
-00000f60: 790a 0a20 2020 2020 2020 203a 7061 7261  y..        :para
-00000f70: 6d20 7061 7468 3a20 7061 7468 2074 6f20  m path: path to 
-00000f80: 7468 6520 7072 6f70 6572 7479 2074 6f20  the property to 
-00000f90: 6472 6976 652c 2061 6e61 6c6f 676f 7573  drive, analogous
-00000fa0: 2074 6f20 7468 6520 6663 7572 7665 2773   to the fcurve's
-00000fb0: 2064 6174 6120 7061 7468 2e0a 2020 2020   data path..    
-00000fc0: 2020 2020 3a74 7970 6520 7061 7468 3a20      :type path: 
-00000fd0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00000fe0: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
-00000ff0: 7261 6d20 696e 6465 783a 2061 7272 6179  ram index: array
-00001000: 2069 6e64 6578 206f 6620 7468 6520 7072   index of the pr
-00001010: 6f70 6572 7479 2064 7269 7665 2e20 4465  operty drive. De
-00001020: 6661 756c 7473 2074 6f20 2d31 2066 6f72  faults to -1 for
-00001030: 2061 6c6c 2069 6e64 6963 6573 206f 7220   all indices or 
-00001040: 6120 7369 6e67 6c65 2063 6861 6e6e 656c  a single channel
-00001050: 2069 6620 7468 6520 7072 6f70 6572 7479   if the property
-00001060: 2069 7320 6e6f 7420 616e 2061 7272 6179   is not an array
-00001070: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00001080: 696e 6465 783a 2074 7970 696e 672e 4f70  index: typing.Op
-00001090: 7469 6f6e 616c 5b69 6e74 5d0a 2020 2020  tional[int].    
-000010a0: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
-000010b0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000010c0: 3a20 5375 6363 6573 7320 6f66 2064 7269  : Success of dri
-000010d0: 7665 7220 7265 6d6f 7661 6c2e 0a20 2020  ver removal..   
-000010e0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-000010f0: 2070 6173 730a 0a20 2020 2064 6566 2067   pass..    def g
-00001100: 6574 2873 656c 662c 0a20 2020 2020 2020  et(self,.       
-00001110: 2020 2020 206b 6579 3a20 7479 7069 6e67       key: typing
-00001120: 2e4f 7074 696f 6e61 6c5b 7374 725d 2c0a  .Optional[str],.
-00001130: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-00001140: 756c 743a 2074 7970 696e 672e 4f70 7469  ult: typing.Opti
-00001150: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
-00001160: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-00001170: 2020 2727 2720 5265 7475 726e 7320 7468    ''' Returns th
-00001180: 6520 7661 6c75 6520 6f66 2074 6865 2063  e value of the c
-00001190: 7573 746f 6d20 7072 6f70 6572 7479 2061  ustom property a
-000011a0: 7373 6967 6e65 6420 746f 206b 6579 206f  ssigned to key o
-000011b0: 7220 6465 6661 756c 7420 7768 656e 206e  r default when n
-000011c0: 6f74 2066 6f75 6e64 2028 6d61 7463 6865  ot found (matche
-000011d0: 7320 5079 7468 6f6e 2773 2064 6963 7469  s Python's dicti
-000011e0: 6f6e 6172 7920 6675 6e63 7469 6f6e 206f  onary function o
-000011f0: 6620 7468 6520 7361 6d65 206e 616d 6529  f the same name)
-00001200: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00001210: 6d20 6b65 793a 2054 6865 206b 6579 2061  m key: The key a
-00001220: 7373 6f63 6961 7465 6420 7769 7468 2074  ssociated with t
-00001230: 6865 2063 7573 746f 6d20 7072 6f70 6572  he custom proper
-00001240: 7479 2e0a 2020 2020 2020 2020 3a74 7970  ty..        :typ
-00001250: 6520 6b65 793a 2074 7970 696e 672e 4f70  e key: typing.Op
-00001260: 7469 6f6e 616c 5b73 7472 5d0a 2020 2020  tional[str].    
-00001270: 2020 2020 3a70 6172 616d 2064 6566 6175      :param defau
-00001280: 6c74 3a20 4f70 7469 6f6e 616c 2061 7267  lt: Optional arg
-00001290: 756d 656e 7420 666f 7220 7468 6520 7661  ument for the va
-000012a0: 6c75 6520 746f 2072 6574 7572 6e20 6966  lue to return if
-000012b0: 202a 6b65 792a 2069 7320 6e6f 7420 666f   *key* is not fo
-000012c0: 756e 642e 0a20 2020 2020 2020 203a 7479  und..        :ty
-000012d0: 7065 2064 6566 6175 6c74 3a20 7479 7069  pe default: typi
-000012e0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-000012f0: 6e67 2e41 6e79 5d0a 2020 2020 2020 2020  ng.Any].        
-00001300: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-00001310: 0a0a 2020 2020 6465 6620 6964 5f70 726f  ..    def id_pro
-00001320: 7065 7274 6965 735f 636c 6561 7228 7365  perties_clear(se
-00001330: 6c66 293a 0a20 2020 2020 2020 2027 2727  lf):.        '''
-00001340: 200a 0a20 2020 2020 2020 2027 2727 0a20   ..        '''. 
-00001350: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00001360: 2064 6566 2069 645f 7072 6f70 6572 7469   def id_properti
-00001370: 6573 5f65 6e73 7572 6528 7365 6c66 2920  es_ensure(self) 
-00001380: 2d3e 2074 7970 696e 672e 416e 793a 0a20  -> typing.Any:. 
-00001390: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
-000013a0: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
-000013b0: 696e 672e 416e 790a 2020 2020 2020 2020  ing.Any.        
-000013c0: 3a72 6574 7572 6e3a 2074 6865 2070 6172  :return: the par
-000013d0: 656e 7420 6772 6f75 7020 666f 7220 616e  ent group for an
-000013e0: 2052 4e41 2073 7472 7563 7427 7320 6375   RNA struct's cu
-000013f0: 7374 6f6d 2049 4450 726f 7065 7274 6965  stom IDPropertie
-00001400: 732e 0a20 2020 2020 2020 2027 2727 0a20  s..        '''. 
-00001410: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00001420: 2064 6566 2069 645f 7072 6f70 6572 7469   def id_properti
-00001430: 6573 5f75 6928 7365 6c66 2c20 6b65 793a  es_ui(self, key:
-00001440: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00001450: 5b74 7970 696e 672e 416e 795d 2920 2d3e  [typing.Any]) ->
-00001460: 2074 7970 696e 672e 416e 793a 0a20 2020   typing.Any:.   
-00001470: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
-00001480: 2020 203a 7061 7261 6d20 6b65 793a 2020     :param key:  
-00001490: 5374 7269 6e67 206e 616d 6520 6f66 2074  String name of t
-000014a0: 6865 2070 726f 7065 7274 792e 0a20 2020  he property..   
-000014b0: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
-000014c0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-000014d0: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
-000014e0: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
-000014f0: 6e67 2e41 6e79 0a20 2020 2020 2020 203a  ng.Any.        :
-00001500: 7265 7475 726e 3a20 5265 7475 726e 2061  return: Return a
-00001510: 6e20 6f62 6a65 6374 2075 7365 6420 746f  n object used to
-00001520: 206d 616e 6167 6520 616e 2049 4450 726f   manage an IDPro
-00001530: 7065 7274 7927 7320 5549 2064 6174 612e  perty's UI data.
-00001540: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00001550: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00001560: 6566 2069 735f 7072 6f70 6572 7479 5f68  ef is_property_h
-00001570: 6964 6465 6e28 7365 6c66 2c20 7072 6f70  idden(self, prop
-00001580: 6572 7479 2920 2d3e 2062 6f6f 6c3a 0a20  erty) -> bool:. 
-00001590: 2020 2020 2020 2027 2727 2043 6865 636b         ''' Check
-000015a0: 2069 6620 6120 7072 6f70 6572 7479 2069   if a property i
-000015b0: 7320 6869 6464 656e 2e0a 0a20 2020 2020  s hidden...     
-000015c0: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-000015d0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-000015e0: 2054 7275 6520 7768 656e 2074 6865 2070   True when the p
-000015f0: 726f 7065 7274 7920 6973 2068 6964 6465  roperty is hidde
-00001600: 6e2e 0a20 2020 2020 2020 2027 2727 0a20  n..        '''. 
-00001610: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00001620: 2064 6566 2069 735f 7072 6f70 6572 7479   def is_property
-00001630: 5f6f 7665 7272 6964 6162 6c65 5f6c 6962  _overridable_lib
-00001640: 7261 7279 2873 656c 662c 2070 726f 7065  rary(self, prope
-00001650: 7274 7929 202d 3e20 626f 6f6c 3a0a 2020  rty) -> bool:.  
-00001660: 2020 2020 2020 2727 2720 4368 6563 6b20        ''' Check 
-00001670: 6966 2061 2070 726f 7065 7274 7920 6973  if a property is
-00001680: 206f 7665 7272 6964 6162 6c65 2e0a 0a20   overridable... 
-00001690: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-000016a0: 6f6f 6c0a 2020 2020 2020 2020 3a72 6574  ool.        :ret
-000016b0: 7572 6e3a 2054 7275 6520 7768 656e 2074  urn: True when t
-000016c0: 6865 2070 726f 7065 7274 7920 6973 206f  he property is o
-000016d0: 7665 7272 6964 6162 6c65 2e0a 2020 2020  verridable..    
-000016e0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000016f0: 7061 7373 0a0a 2020 2020 6465 6620 6973  pass..    def is
-00001700: 5f70 726f 7065 7274 795f 7265 6164 6f6e  _property_readon
-00001710: 6c79 2873 656c 662c 2070 726f 7065 7274  ly(self, propert
-00001720: 7929 202d 3e20 626f 6f6c 3a0a 2020 2020  y) -> bool:.    
-00001730: 2020 2020 2727 2720 4368 6563 6b20 6966      ''' Check if
-00001740: 2061 2070 726f 7065 7274 7920 6973 2072   a property is r
-00001750: 6561 646f 6e6c 792e 0a0a 2020 2020 2020  eadonly...      
-00001760: 2020 3a72 7479 7065 3a20 626f 6f6c 0a20    :rtype: bool. 
-00001770: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00001780: 5472 7565 2077 6865 6e20 7468 6520 7072  True when the pr
-00001790: 6f70 6572 7479 2069 7320 7265 6164 6f6e  operty is readon
-000017a0: 6c79 2028 6e6f 7420 7772 6974 6162 6c65  ly (not writable
-000017b0: 292e 0a20 2020 2020 2020 2027 2727 0a20  )..        '''. 
-000017c0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-000017d0: 2064 6566 2069 735f 7072 6f70 6572 7479   def is_property
-000017e0: 5f73 6574 2873 656c 662c 2070 726f 7065  _set(self, prope
-000017f0: 7274 792c 0a20 2020 2020 2020 2020 2020  rty,.           
-00001800: 2020 2020 2020 2020 2020 2020 2067 686f               gho
-00001810: 7374 3a20 7479 7069 6e67 2e4f 7074 696f  st: typing.Optio
-00001820: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
-00001830: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00001840: 2020 2027 2727 2043 6865 636b 2069 6620     ''' Check if 
-00001850: 6120 7072 6f70 6572 7479 2069 7320 7365  a property is se
-00001860: 742c 2075 7365 2066 6f72 2074 6573 7469  t, use for testi
-00001870: 6e67 206f 7065 7261 746f 7220 7072 6f70  ng operator prop
-00001880: 6572 7469 6573 2e0a 0a20 2020 2020 2020  erties...       
-00001890: 203a 7061 7261 6d20 6768 6f73 743a 2055   :param ghost: U
-000018a0: 7365 6420 666f 7220 6f70 6572 6174 6f72  sed for operator
-000018b0: 7320 7468 6174 2072 652d 7275 6e20 7769  s that re-run wi
-000018c0: 7468 2070 7265 7669 6f75 7320 7365 7474  th previous sett
-000018d0: 696e 6773 2e20 496e 2074 6869 7320 6361  ings. In this ca
-000018e0: 7365 2074 6865 2070 726f 7065 7274 7920  se the property 
-000018f0: 6973 206e 6f74 206d 6172 6b65 6420 6173  is not marked as
-00001900: 2073 6574 2c20 7965 7420 7468 6520 7661   set, yet the va
-00001910: 6c75 6520 6672 6f6d 2074 6865 2070 7265  lue from the pre
-00001920: 7669 6f75 7320 6578 6563 7574 696f 6e20  vious execution 
-00001930: 6973 2075 7365 642e 2049 6e20 7261 7265  is used. In rare
-00001940: 2063 6173 6573 2079 6f75 206d 6179 2077   cases you may w
-00001950: 616e 7420 746f 2073 6574 2074 6869 7320  ant to set this 
-00001960: 6f70 7469 6f6e 2074 6f20 6661 6c73 652e  option to false.
-00001970: 0a20 2020 2020 2020 203a 7479 7065 2067  .        :type g
-00001980: 686f 7374 3a20 7479 7069 6e67 2e4f 7074  host: typing.Opt
-00001990: 696f 6e61 6c5b 626f 6f6c 5d0a 2020 2020  ional[bool].    
-000019a0: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
-000019b0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000019c0: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
-000019d0: 7072 6f70 6572 7479 2068 6173 2062 6565  property has bee
-000019e0: 6e20 7365 742e 0a20 2020 2020 2020 2027  n set..        '
-000019f0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-00001a00: 0a20 2020 2064 6566 2069 7465 6d73 2873  .    def items(s
-00001a10: 656c 6629 202d 3e20 7479 7069 6e67 2e41  elf) -> typing.A
-00001a20: 6e79 3a0a 2020 2020 2020 2020 2727 2720  ny:.        ''' 
-00001a30: 5265 7475 726e 7320 7468 6520 6974 656d  Returns the item
-00001a40: 7320 6f66 2074 6869 7320 6f62 6a65 6374  s of this object
-00001a50: 7320 6375 7374 6f6d 2070 726f 7065 7274  s custom propert
-00001a60: 6965 7320 286d 6174 6368 6573 2050 7974  ies (matches Pyt
-00001a70: 686f 6e27 7320 6469 6374 696f 6e61 7279  hon's dictionary
-00001a80: 2066 756e 6374 696f 6e20 6f66 2074 6865   function of the
-00001a90: 2073 616d 6520 6e61 6d65 292e 0a0a 2020   same name)...  
-00001aa0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
-00001ab0: 7069 6e67 2e41 6e79 0a20 2020 2020 2020  ping.Any.       
-00001ac0: 203a 7265 7475 726e 3a20 6375 7374 6f6d   :return: custom
-00001ad0: 2070 726f 7065 7274 7920 6b65 792c 2076   property key, v
-00001ae0: 616c 7565 2070 6169 7273 2e0a 2020 2020  alue pairs..    
-00001af0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00001b00: 7061 7373 0a0a 2020 2020 6465 6620 6b65  pass..    def ke
-00001b10: 7966 7261 6d65 5f64 656c 6574 6528 0a20  yframe_delete(. 
-00001b20: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00001b30: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00001b40: 615f 7061 7468 3a20 7479 7069 6e67 2e4f  a_path: typing.O
-00001b50: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
-00001b60: 2020 2020 2020 2020 2020 696e 6465 783a            index:
+00000ab0: 636c 6173 7320 6270 795f 7072 6f70 5f63  class bpy_prop_c
+00000ac0: 6f6c 6c65 6374 696f 6e28 7479 7069 6e67  ollection(typing
+00000ad0: 2e47 656e 6572 6963 5b47 656e 6572 6963  .Generic[Generic
+00000ae0: 5479 7065 5d29 3a0a 2020 2020 2727 2720  Type]):.    ''' 
+00000af0: 6275 696c 742d 696e 2063 6c61 7373 2075  built-in class u
+00000b00: 7365 6420 666f 7220 616c 6c20 636f 6c6c  sed for all coll
+00000b10: 6563 7469 6f6e 732e 0a20 2020 2027 2727  ections..    '''
+00000b20: 0a0a 2020 2020 6465 6620 6669 6e64 2873  ..    def find(s
+00000b30: 656c 662c 206b 6579 3a20 7479 7069 6e67  elf, key: typing
+00000b40: 2e4f 7074 696f 6e61 6c5b 7374 725d 2920  .Optional[str]) 
+00000b50: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00000b60: 2727 2720 5265 7475 726e 7320 7468 6520  ''' Returns the 
+00000b70: 696e 6465 7820 6f66 2061 206b 6579 2069  index of a key i
+00000b80: 6e20 6120 636f 6c6c 6563 7469 6f6e 206f  n a collection o
+00000b90: 7220 2d31 2077 6865 6e20 6e6f 7420 666f  r -1 when not fo
+00000ba0: 756e 6420 286d 6174 6368 6573 2050 7974  und (matches Pyt
+00000bb0: 686f 6e27 7320 7374 7269 6e67 2066 696e  hon's string fin
+00000bc0: 6420 6675 6e63 7469 6f6e 206f 6620 7468  d function of th
+00000bd0: 6520 7361 6d65 206e 616d 6529 2e0a 0a20  e same name)... 
+00000be0: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
+00000bf0: 793a 2054 6865 2069 6465 6e74 6966 6965  y: The identifie
+00000c00: 7220 666f 7220 7468 6520 636f 6c6c 6563  r for the collec
+00000c10: 7469 6f6e 206d 656d 6265 722e 0a20 2020  tion member..   
+00000c20: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
+00000c30: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00000c40: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
+00000c50: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+00000c60: 203a 7265 7475 726e 3a20 696e 6465 7820   :return: index 
+00000c70: 6f66 2074 6865 206b 6579 2e0a 2020 2020  of the key..    
+00000c80: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00000c90: 7061 7373 0a0a 2020 2020 6465 6620 666f  pass..    def fo
+00000ca0: 7265 6163 685f 6765 7428 7365 6c66 2c20  reach_get(self, 
+00000cb0: 6174 7472 2c20 7365 7129 3a0a 2020 2020  attr, seq):.    
+00000cc0: 2020 2020 2727 2720 5468 6973 2069 7320      ''' This is 
+00000cd0: 6120 6675 6e63 7469 6f6e 2074 6f20 6769  a function to gi
+00000ce0: 7665 2066 6173 7420 6163 6365 7373 2074  ve fast access t
+00000cf0: 6f20 6174 7472 6962 7574 6573 2077 6974  o attributes wit
+00000d00: 6869 6e20 6120 636f 6c6c 6563 7469 6f6e  hin a collection
+00000d10: 2e20 4f6e 6c79 2077 6f72 6b73 2066 6f72  . Only works for
+00000d20: 2027 6261 7369 6320 7479 7065 2720 7072   'basic type' pr
+00000d30: 6f70 6572 7469 6573 2028 626f 6f6c 2c20  operties (bool, 
+00000d40: 696e 7420 616e 6420 666c 6f61 7429 2120  int and float)! 
+00000d50: 4d75 6c74 692d 6469 6d65 6e73 696f 6e61  Multi-dimensiona
+00000d60: 6c20 6172 7261 7973 2028 6c69 6b65 2061  l arrays (like a
+00000d70: 7272 6179 206f 6620 7665 6374 6f72 7329  rray of vectors)
+00000d80: 2077 696c 6c20 6265 2066 6c61 7474 656e   will be flatten
+00000d90: 6564 2069 6e74 6f20 7365 712e 0a0a 2020  ed into seq...  
+00000da0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00000db0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00000dc0: 666f 7265 6163 685f 7365 7428 7365 6c66  foreach_set(self
+00000dd0: 2c20 6174 7472 2c20 7365 7129 3a0a 2020  , attr, seq):.  
+00000de0: 2020 2020 2020 2727 2720 5468 6973 2069        ''' This i
+00000df0: 7320 6120 6675 6e63 7469 6f6e 2074 6f20  s a function to 
+00000e00: 6769 7665 2066 6173 7420 6163 6365 7373  give fast access
+00000e10: 2074 6f20 6174 7472 6962 7574 6573 2077   to attributes w
+00000e20: 6974 6869 6e20 6120 636f 6c6c 6563 7469  ithin a collecti
+00000e30: 6f6e 2e20 4f6e 6c79 2077 6f72 6b73 2066  on. Only works f
+00000e40: 6f72 2027 6261 7369 6320 7479 7065 2720  or 'basic type' 
+00000e50: 7072 6f70 6572 7469 6573 2028 626f 6f6c  properties (bool
+00000e60: 2c20 696e 7420 616e 6420 666c 6f61 7429  , int and float)
+00000e70: 2120 7365 7120 6d75 7374 2062 6520 756e  ! seq must be un
+00000e80: 692d 6469 6d65 6e73 696f 6e61 6c2c 206d  i-dimensional, m
+00000e90: 756c 7469 2d64 696d 656e 7369 6f6e 616c  ulti-dimensional
+00000ea0: 2061 7272 6179 7320 286c 696b 6520 6172   arrays (like ar
+00000eb0: 7261 7920 6f66 2076 6563 746f 7273 2920  ray of vectors) 
+00000ec0: 7769 6c6c 2062 6520 7265 2d63 7265 6174  will be re-creat
+00000ed0: 6564 2066 726f 6d20 6974 2e0a 0a20 2020  ed from it...   
+00000ee0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00000ef0: 2070 6173 730a 0a20 2020 2064 6566 2067   pass..    def g
+00000f00: 6574 2873 656c 662c 0a20 2020 2020 2020  et(self,.       
+00000f10: 2020 2020 206b 6579 3a20 7479 7069 6e67       key: typing
+00000f20: 2e4f 7074 696f 6e61 6c5b 7374 725d 2c0a  .Optional[str],.
+00000f30: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00000f40: 756c 743a 2074 7970 696e 672e 4f70 7469  ult: typing.Opti
+00000f50: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
+00000f60: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00000f70: 2020 2727 2720 5265 7475 726e 7320 7468    ''' Returns th
+00000f80: 6520 7661 6c75 6520 6f66 2074 6865 2069  e value of the i
+00000f90: 7465 6d20 6173 7369 676e 6564 2074 6f20  tem assigned to 
+00000fa0: 6b65 7920 6f72 2064 6566 6175 6c74 2077  key or default w
+00000fb0: 6865 6e20 6e6f 7420 666f 756e 6420 286d  hen not found (m
+00000fc0: 6174 6368 6573 2050 7974 686f 6e27 7320  atches Python's 
+00000fd0: 6469 6374 696f 6e61 7279 2066 756e 6374  dictionary funct
+00000fe0: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
+00000ff0: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
+00001000: 3a70 6172 616d 206b 6579 3a20 5468 6520  :param key: The 
+00001010: 6964 656e 7469 6669 6572 2066 6f72 2074  identifier for t
+00001020: 6865 2063 6f6c 6c65 6374 696f 6e20 6d65  he collection me
+00001030: 6d62 6572 2e0a 2020 2020 2020 2020 3a74  mber..        :t
+00001040: 7970 6520 6b65 793a 2074 7970 696e 672e  ype key: typing.
+00001050: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
+00001060: 2020 2020 2020 3a70 6172 616d 2064 6566        :param def
+00001070: 6175 6c74 3a20 4f70 7469 6f6e 616c 2061  ault: Optional a
+00001080: 7267 756d 656e 7420 666f 7220 7468 6520  rgument for the 
+00001090: 7661 6c75 6520 746f 2072 6574 7572 6e20  value to return 
+000010a0: 6966 202a 6b65 792a 2069 7320 6e6f 7420  if *key* is not 
+000010b0: 666f 756e 642e 0a20 2020 2020 2020 203a  found..        :
+000010c0: 7479 7065 2064 6566 6175 6c74 3a20 7479  type default: ty
+000010d0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+000010e0: 7069 6e67 2e41 6e79 5d0a 2020 2020 2020  ping.Any].      
+000010f0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00001100: 7373 0a0a 2020 2020 6465 6620 6974 656d  ss..    def item
+00001110: 7328 7365 6c66 2920 2d3e 2074 7970 696e  s(self) -> typin
+00001120: 672e 4c69 7374 3a0a 2020 2020 2020 2020  g.List:.        
+00001130: 2727 2720 5265 7475 726e 2074 6865 2069  ''' Return the i
+00001140: 6465 6e74 6966 6965 7273 206f 6620 636f  dentifiers of co
+00001150: 6c6c 6563 7469 6f6e 206d 656d 6265 7273  llection members
+00001160: 2028 6d61 7463 6869 6e67 2050 7974 686f   (matching Pytho
+00001170: 6e27 7320 6469 6374 2e69 7465 6d73 2829  n's dict.items()
+00001180: 2066 756e 6374 696f 6e61 6c69 7479 292e   functionality).
+00001190: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+000011a0: 3a20 7479 7069 6e67 2e4c 6973 740a 2020  : typing.List.  
+000011b0: 2020 2020 2020 3a72 6574 7572 6e3a 2028        :return: (
+000011c0: 6b65 792c 2076 616c 7565 2920 7061 6972  key, value) pair
+000011d0: 7320 666f 7220 6561 6368 206d 656d 6265  s for each membe
+000011e0: 7220 6f66 2074 6869 7320 636f 6c6c 6563  r of this collec
+000011f0: 7469 6f6e 2e0a 2020 2020 2020 2020 2727  tion..        ''
+00001200: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00001210: 2020 2020 6465 6620 6b65 7973 2873 656c      def keys(sel
+00001220: 6629 202d 3e20 7479 7069 6e67 2e4c 6973  f) -> typing.Lis
+00001230: 745b 7374 725d 3a0a 2020 2020 2020 2020  t[str]:.        
+00001240: 2727 2720 5265 7475 726e 2074 6865 2069  ''' Return the i
+00001250: 6465 6e74 6966 6965 7273 206f 6620 636f  dentifiers of co
+00001260: 6c6c 6563 7469 6f6e 206d 656d 6265 7273  llection members
+00001270: 2028 6d61 7463 6869 6e67 2050 7974 686f   (matching Pytho
+00001280: 6e27 7320 6469 6374 2e6b 6579 7328 2920  n's dict.keys() 
+00001290: 6675 6e63 7469 6f6e 616c 6974 7929 2e0a  functionality)..
+000012a0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000012b0: 2074 7970 696e 672e 4c69 7374 5b73 7472   typing.List[str
+000012c0: 5d0a 2020 2020 2020 2020 3a72 6574 7572  ].        :retur
+000012d0: 6e3a 2074 6865 2069 6465 6e74 6966 6965  n: the identifie
+000012e0: 7273 2066 6f72 2065 6163 6820 6d65 6d62  rs for each memb
+000012f0: 6572 206f 6620 7468 6973 2063 6f6c 6c65  er of this colle
+00001300: 6374 696f 6e2e 0a20 2020 2020 2020 2027  ction..        '
+00001310: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00001320: 0a20 2020 2064 6566 2076 616c 7565 7328  .    def values(
+00001330: 7365 6c66 2920 2d3e 2074 7970 696e 672e  self) -> typing.
+00001340: 4c69 7374 3a0a 2020 2020 2020 2020 2727  List:.        ''
+00001350: 2720 5265 7475 726e 2074 6865 2076 616c  ' Return the val
+00001360: 7565 7320 6f66 2063 6f6c 6c65 6374 696f  ues of collectio
+00001370: 6e20 286d 6174 6368 696e 6720 5079 7468  n (matching Pyth
+00001380: 6f6e 2773 2064 6963 742e 7661 6c75 6573  on's dict.values
+00001390: 2829 2066 756e 6374 696f 6e61 6c69 7479  () functionality
+000013a0: 292e 0a0a 2020 2020 2020 2020 3a72 7479  )...        :rty
+000013b0: 7065 3a20 7479 7069 6e67 2e4c 6973 740a  pe: typing.List.
+000013c0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+000013d0: 2074 6865 206d 656d 6265 7273 206f 6620   the members of 
+000013e0: 7468 6973 2063 6f6c 6c65 6374 696f 6e2e  this collection.
+000013f0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00001400: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00001410: 6566 205f 5f67 6574 6974 656d 5f5f 2873  ef __getitem__(s
+00001420: 656c 662c 206b 6579 3a20 7479 7069 6e67  elf, key: typing
+00001430: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
+00001440: 2920 2d3e 2027 4765 6e65 7269 6354 7970  ) -> 'GenericTyp
+00001450: 6527 3a0a 2020 2020 2020 2020 2727 2720  e':.        ''' 
+00001460: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00001470: 206b 6579 3a20 0a20 2020 2020 2020 203a   key: .        :
+00001480: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
+00001490: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
+000014a0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000014b0: 2027 4765 6e65 7269 6354 7970 6527 0a20   'GenericType'. 
+000014c0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+000014d0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+000014e0: 205f 5f73 6574 6974 656d 5f5f 2873 656c   __setitem__(sel
+000014f0: 662c 206b 6579 3a20 7479 7069 6e67 2e55  f, key: typing.U
+00001500: 6e69 6f6e 5b69 6e74 2c20 7374 725d 2c20  nion[int, str], 
+00001510: 7661 6c75 653a 2027 4765 6e65 7269 6354  value: 'GenericT
+00001520: 7970 6527 293a 0a20 2020 2020 2020 2027  ype'):.        '
+00001530: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
+00001540: 7261 6d20 6b65 793a 200a 2020 2020 2020  ram key: .      
+00001550: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
+00001560: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
+00001570: 7472 5d0a 2020 2020 2020 2020 3a70 6172  tr].        :par
+00001580: 616d 2076 616c 7565 3a20 0a20 2020 2020  am value: .     
+00001590: 2020 203a 7479 7065 2076 616c 7565 3a20     :type value: 
+000015a0: 2747 656e 6572 6963 5479 7065 270a 2020  'GenericType'.  
+000015b0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+000015c0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+000015d0: 5f5f 6465 6c69 7465 6d5f 5f28 7365 6c66  __delitem__(self
+000015e0: 2c20 6b65 793a 2074 7970 696e 672e 556e  , key: typing.Un
+000015f0: 696f 6e5b 696e 742c 2073 7472 5d29 202d  ion[int, str]) -
+00001600: 3e20 2747 656e 6572 6963 5479 7065 273a  > 'GenericType':
+00001610: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+00001620: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
+00001630: 793a 200a 2020 2020 2020 2020 3a74 7970  y: .        :typ
+00001640: 6520 6b65 793a 2074 7970 696e 672e 556e  e key: typing.Un
+00001650: 696f 6e5b 696e 742c 2073 7472 5d0a 2020  ion[int, str].  
+00001660: 2020 2020 2020 3a72 7479 7065 3a20 2747        :rtype: 'G
+00001670: 656e 6572 6963 5479 7065 270a 2020 2020  enericType'.    
+00001680: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00001690: 7061 7373 0a0a 2020 2020 6465 6620 5f5f  pass..    def __
+000016a0: 6974 6572 5f5f 2873 656c 6629 202d 3e20  iter__(self) -> 
+000016b0: 7479 7069 6e67 2e49 7465 7261 746f 725b  typing.Iterator[
+000016c0: 2747 656e 6572 6963 5479 7065 275d 3a0a  'GenericType']:.
+000016d0: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
+000016e0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
+000016f0: 7069 6e67 2e49 7465 7261 746f 725b 2747  ping.Iterator['G
+00001700: 656e 6572 6963 5479 7065 275d 0a20 2020  enericType'].   
+00001710: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00001720: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
+00001730: 5f6e 6578 745f 5f28 7365 6c66 2920 2d3e  _next__(self) ->
+00001740: 2027 4765 6e65 7269 6354 7970 6527 3a0a   'GenericType':.
+00001750: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
+00001760: 2020 2020 2020 3a72 7479 7065 3a20 2747        :rtype: 'G
+00001770: 656e 6572 6963 5479 7065 270a 2020 2020  enericType'.    
+00001780: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00001790: 7061 7373 0a0a 2020 2020 6465 6620 5f5f  pass..    def __
+000017a0: 6c65 6e5f 5f28 7365 6c66 2920 2d3e 2069  len__(self) -> i
+000017b0: 6e74 3a0a 2020 2020 2020 2020 2727 2720  nt:.        ''' 
+000017c0: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+000017d0: 3a20 696e 740a 2020 2020 2020 2020 2727  : int.        ''
+000017e0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+000017f0: 0a63 6c61 7373 2062 7079 5f73 7472 7563  .class bpy_struc
+00001800: 743a 0a20 2020 2027 2727 2062 7569 6c74  t:.    ''' built
+00001810: 2d69 6e20 6261 7365 2063 6c61 7373 2066  -in base class f
+00001820: 6f72 2061 6c6c 2063 6c61 7373 6573 2069  or all classes i
+00001830: 6e20 6270 792e 7479 7065 732e 0a20 2020  n bpy.types..   
+00001840: 2027 2727 0a0a 2020 2020 6964 5f64 6174   '''..    id_dat
+00001850: 6120 3d20 4e6f 6e65 0a20 2020 2027 2727  a = None.    '''
+00001860: 2054 6865 2060 6270 792e 7479 7065 732e   The `bpy.types.
+00001870: 4944 6020 6f62 6a65 6374 2074 6869 7320  ID` object this 
+00001880: 6461 7461 626c 6f63 6b20 6973 2066 726f  datablock is fro
+00001890: 6d20 6f72 204e 6f6e 652c 2028 6e6f 7420  m or None, (not 
+000018a0: 6176 6169 6c61 626c 6520 666f 7220 616c  available for al
+000018b0: 6c20 6461 7461 2074 7970 6573 2927 2727  l data types)'''
+000018c0: 0a0a 2020 2020 6465 6620 6173 5f70 6f69  ..    def as_poi
+000018d0: 6e74 6572 2873 656c 6629 202d 3e20 696e  nter(self) -> in
+000018e0: 743a 0a20 2020 2020 2020 2027 2727 2052  t:.        ''' R
+000018f0: 6574 7572 6e73 2074 6865 206d 656d 6f72  eturns the memor
+00001900: 7920 6164 6472 6573 7320 7768 6963 6820  y address which 
+00001910: 686f 6c64 7320 6120 706f 696e 7465 7220  holds a pointer 
+00001920: 746f 2042 6c65 6e64 6572 2773 2069 6e74  to Blender's int
+00001930: 6572 6e61 6c20 6461 7461 0a0a 2020 2020  ernal data..    
+00001940: 2020 2020 3a72 7479 7065 3a20 696e 740a      :rtype: int.
+00001950: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00001960: 2069 6e74 2028 6d65 6d6f 7279 2061 6464   int (memory add
+00001970: 7265 7373 292e 0a20 2020 2020 2020 2027  ress)..        '
+00001980: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00001990: 0a20 2020 2064 6566 2064 7269 7665 725f  .    def driver_
+000019a0: 6164 6428 7365 6c66 2c0a 2020 2020 2020  add(self,.      
+000019b0: 2020 2020 2020 2020 2020 2020 2070 6174               pat
+000019c0: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
+000019d0: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
+000019e0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+000019f0: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
+00001a00: 616c 5b69 6e74 5d20 3d20 2d31 2920 2d3e  al[int] = -1) ->
+00001a10: 2027 4643 7572 7665 273a 0a20 2020 2020   'FCurve':.     
+00001a20: 2020 2027 2727 2041 6464 7320 6472 6976     ''' Adds driv
+00001a30: 6572 2873 2920 746f 2074 6865 2067 6976  er(s) to the giv
+00001a40: 656e 2070 726f 7065 7274 790a 0a20 2020  en property..   
+00001a50: 2020 2020 203a 7061 7261 6d20 7061 7468       :param path
+00001a60: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
+00001a70: 6f70 6572 7479 2074 6f20 6472 6976 652c  operty to drive,
+00001a80: 2061 6e61 6c6f 676f 7573 2074 6f20 7468   analogous to th
+00001a90: 6520 6663 7572 7665 2773 2064 6174 6120  e fcurve's data 
+00001aa0: 7061 7468 2e0a 2020 2020 2020 2020 3a74  path..        :t
+00001ab0: 7970 6520 7061 7468 3a20 7479 7069 6e67  ype path: typing
+00001ac0: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
+00001ad0: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
+00001ae0: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
+00001af0: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
+00001b00: 2064 7269 7665 2e20 4465 6661 756c 7473   drive. Defaults
+00001b10: 2074 6f20 2d31 2066 6f72 2061 6c6c 2069   to -1 for all i
+00001b20: 6e64 6963 6573 206f 7220 6120 7369 6e67  ndices or a sing
+00001b30: 6c65 2063 6861 6e6e 656c 2069 6620 7468  le channel if th
+00001b40: 6520 7072 6f70 6572 7479 2069 7320 6e6f  e property is no
+00001b50: 7420 616e 2061 7272 6179 2e0a 2020 2020  t an array..    
+00001b60: 2020 2020 3a74 7970 6520 696e 6465 783a      :type index:
 00001b70: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00001b80: 5b69 6e74 5d20 3d20 2d31 2c0a 2020 2020  [int] = -1,.    
-00001b90: 2020 2020 2020 2020 6672 616d 653a 2074          frame: t
-00001ba0: 7970 696e 672e 4f70 7469 6f6e 616c 5b66  yping.Optional[f
-00001bb0: 6c6f 6174 5d20 3d20 2762 7079 2e63 6f6e  loat] = 'bpy.con
-00001bc0: 7465 7874 2e73 6365 6e65 2e66 7261 6d65  text.scene.frame
-00001bd0: 5f63 7572 7265 6e74 272c 0a20 2020 2020  _current',.     
-00001be0: 2020 2020 2020 2067 726f 7570 3a20 7479         group: ty
-00001bf0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-00001c00: 725d 203d 2022 2229 202d 3e20 626f 6f6c  r] = "") -> bool
-00001c10: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
-00001c20: 6d6f 7665 2061 206b 6579 6672 616d 6520  move a keyframe 
-00001c30: 6672 6f6d 2074 6869 7320 7072 6f70 6572  from this proper
-00001c40: 7469 6573 2066 6375 7276 652e 0a0a 2020  ties fcurve...  
-00001c50: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
-00001c60: 615f 7061 7468 3a20 7061 7468 2074 6f20  a_path: path to 
-00001c70: 7468 6520 7072 6f70 6572 7479 2074 6f20  the property to 
-00001c80: 7265 6d6f 7665 2061 206b 6579 2c20 616e  remove a key, an
-00001c90: 616c 6f67 6f75 7320 746f 2074 6865 2066  alogous to the f
-00001ca0: 6375 7276 6527 7320 6461 7461 2070 6174  curve's data pat
-00001cb0: 682e 0a20 2020 2020 2020 203a 7479 7065  h..        :type
-00001cc0: 2064 6174 615f 7061 7468 3a20 7479 7069   data_path: typi
-00001cd0: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00001ce0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001cf0: 696e 6465 783a 2061 7272 6179 2069 6e64  index: array ind
-00001d00: 6578 206f 6620 7468 6520 7072 6f70 6572  ex of the proper
-00001d10: 7479 2074 6f20 7265 6d6f 7665 2061 206b  ty to remove a k
-00001d20: 6579 2e20 4465 6661 756c 7473 2074 6f20  ey. Defaults to 
-00001d30: 2d31 2072 656d 6f76 696e 6720 616c 6c20  -1 removing all 
-00001d40: 696e 6469 6365 7320 6f72 2061 2073 696e  indices or a sin
-00001d50: 676c 6520 6368 616e 6e65 6c20 6966 2074  gle channel if t
-00001d60: 6865 2070 726f 7065 7274 7920 6973 206e  he property is n
-00001d70: 6f74 2061 6e20 6172 7261 792e 0a20 2020  ot an array..   
-00001d80: 2020 2020 203a 7479 7065 2069 6e64 6578       :type index
-00001d90: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00001da0: 6c5b 696e 745d 0a20 2020 2020 2020 203a  l[int].        :
-00001db0: 7061 7261 6d20 6672 616d 653a 2054 6865  param frame: The
-00001dc0: 2066 7261 6d65 206f 6e20 7768 6963 6820   frame on which 
-00001dd0: 7468 6520 6b65 7966 7261 6d65 2069 7320  the keyframe is 
-00001de0: 6465 6c65 7465 642c 2064 6566 6175 6c74  deleted, default
-00001df0: 696e 6720 746f 2074 6865 2063 7572 7265  ing to the curre
-00001e00: 6e74 2066 7261 6d65 2e0a 2020 2020 2020  nt frame..      
-00001e10: 2020 3a74 7970 6520 6672 616d 653a 2074    :type frame: t
-00001e20: 7970 696e 672e 4f70 7469 6f6e 616c 5b66  yping.Optional[f
-00001e30: 6c6f 6174 5d0a 2020 2020 2020 2020 3a70  loat].        :p
-00001e40: 6172 616d 2067 726f 7570 3a20 5468 6520  aram group: The 
-00001e50: 6e61 6d65 206f 6620 7468 6520 6772 6f75  name of the grou
-00001e60: 7020 7468 6520 462d 4375 7276 6520 7368  p the F-Curve sh
-00001e70: 6f75 6c64 2062 6520 6164 6465 6420 746f  ould be added to
-00001e80: 2069 6620 6974 2064 6f65 736e 2774 2065   if it doesn't e
-00001e90: 7869 7374 2079 6574 2e0a 2020 2020 2020  xist yet..      
-00001ea0: 2020 3a74 7970 6520 6772 6f75 703a 2074    :type group: t
-00001eb0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00001ec0: 7472 5d0a 2020 2020 2020 2020 3a72 7479  tr].        :rty
-00001ed0: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-00001ee0: 203a 7265 7475 726e 3a20 5375 6363 6573   :return: Succes
-00001ef0: 7320 6f66 206b 6579 6672 616d 6520 6465  s of keyframe de
-00001f00: 6c65 7469 6f6e 2e0a 2020 2020 2020 2020  letion..        
-00001f10: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-00001f20: 0a0a 2020 2020 6465 6620 6b65 7966 7261  ..    def keyfra
-00001f30: 6d65 5f69 6e73 6572 7428 0a20 2020 2020  me_insert(.     
-00001f40: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00001f50: 2020 2020 2020 2020 2064 6174 615f 7061           data_pa
-00001f60: 7468 3a20 7479 7069 6e67 2e4f 7074 696f  th: typing.Optio
-00001f70: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
-00001f80: 2020 2020 2020 696e 6465 783a 2074 7970        index: typ
-00001f90: 696e 672e 4f70 7469 6f6e 616c 5b69 6e74  ing.Optional[int
-00001fa0: 5d20 3d20 2d31 2c0a 2020 2020 2020 2020  ] = -1,.        
-00001fb0: 2020 2020 6672 616d 653a 2074 7970 696e      frame: typin
-00001fc0: 672e 4f70 7469 6f6e 616c 5b66 6c6f 6174  g.Optional[float
-00001fd0: 5d20 3d20 2762 7079 2e63 6f6e 7465 7874  ] = 'bpy.context
-00001fe0: 2e73 6365 6e65 2e66 7261 6d65 5f63 7572  .scene.frame_cur
-00001ff0: 7265 6e74 272c 0a20 2020 2020 2020 2020  rent',.         
-00002000: 2020 2067 726f 7570 3a20 7479 7069 6e67     group: typing
-00002010: 2e4f 7074 696f 6e61 6c5b 7374 725d 203d  .Optional[str] =
-00002020: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
-00002030: 206f 7074 696f 6e73 3a20 7479 7069 6e67   options: typing
-00002040: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00002050: 2e41 6e79 5d20 3d20 2773 6574 2829 2729  .Any] = 'set()')
-00002060: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00002070: 2020 2727 2720 496e 7365 7274 2061 206b    ''' Insert a k
-00002080: 6579 6672 616d 6520 6f6e 2074 6865 2070  eyframe on the p
-00002090: 726f 7065 7274 7920 6769 7665 6e2c 2061  roperty given, a
-000020a0: 6464 696e 6720 6663 7572 7665 7320 616e  dding fcurves an
-000020b0: 6420 616e 696d 6174 696f 6e20 6461 7461  d animation data
-000020c0: 2077 6865 6e20 6e65 6365 7373 6172 792e   when necessary.
-000020d0: 2054 6869 7320 6973 2074 6865 206d 6f73   This is the mos
-000020e0: 7420 7369 6d70 6c65 2065 7861 6d70 6c65  t simple example
-000020f0: 206f 6620 696e 7365 7274 696e 6720 6120   of inserting a 
-00002100: 6b65 7966 7261 6d65 2066 726f 6d20 7079  keyframe from py
-00002110: 7468 6f6e 2e20 4e6f 7465 2074 6861 7420  thon. Note that 
-00002120: 7768 656e 206b 6579 696e 6720 6461 7461  when keying data
-00002130: 2070 6174 6873 2077 6869 6368 2063 6f6e   paths which con
-00002140: 7461 696e 206e 6573 7465 6420 7072 6f70  tain nested prop
-00002150: 6572 7469 6573 2074 6869 7320 6d75 7374  erties this must
-00002160: 2062 6520 646f 6e65 2066 726f 6d20 7468   be done from th
-00002170: 6520 6049 4460 2073 7562 636c 6173 732c  e `ID` subclass,
-00002180: 2069 6e20 7468 6973 2063 6173 6520 7468   in this case th
-00002190: 6520 6041 726d 6174 7572 6560 2072 6174  e `Armature` rat
-000021a0: 6865 7220 7468 616e 2074 6865 2062 6f6e  her than the bon
-000021b0: 652e 0a0a 2020 2020 2020 2020 3a70 6172  e...        :par
-000021c0: 616d 2064 6174 615f 7061 7468 3a20 7061  am data_path: pa
-000021d0: 7468 2074 6f20 7468 6520 7072 6f70 6572  th to the proper
-000021e0: 7479 2074 6f20 6b65 792c 2061 6e61 6c6f  ty to key, analo
-000021f0: 676f 7573 2074 6f20 7468 6520 6663 7572  gous to the fcur
-00002200: 7665 2773 2064 6174 6120 7061 7468 2e0a  ve's data path..
-00002210: 2020 2020 2020 2020 3a74 7970 6520 6461          :type da
-00002220: 7461 5f70 6174 683a 2074 7970 696e 672e  ta_path: typing.
-00002230: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
-00002240: 2020 2020 2020 3a70 6172 616d 2069 6e64        :param ind
-00002250: 6578 3a20 6172 7261 7920 696e 6465 7820  ex: array index 
-00002260: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
-00002270: 746f 206b 6579 2e20 4465 6661 756c 7473  to key. Defaults
-00002280: 2074 6f20 2d31 2077 6869 6368 2077 696c   to -1 which wil
-00002290: 6c20 6b65 7920 616c 6c20 696e 6469 6365  l key all indice
-000022a0: 7320 6f72 2061 2073 696e 676c 6520 6368  s or a single ch
-000022b0: 616e 6e65 6c20 6966 2074 6865 2070 726f  annel if the pro
-000022c0: 7065 7274 7920 6973 206e 6f74 2061 6e20  perty is not an 
-000022d0: 6172 7261 792e 0a20 2020 2020 2020 203a  array..        :
-000022e0: 7479 7065 2069 6e64 6578 3a20 7479 7069  type index: typi
-000022f0: 6e67 2e4f 7074 696f 6e61 6c5b 696e 745d  ng.Optional[int]
-00002300: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00002310: 6672 616d 653a 2054 6865 2066 7261 6d65  frame: The frame
-00002320: 206f 6e20 7768 6963 6820 7468 6520 6b65   on which the ke
-00002330: 7966 7261 6d65 2069 7320 696e 7365 7274  yframe is insert
-00002340: 6564 2c20 6465 6661 756c 7469 6e67 2074  ed, defaulting t
-00002350: 6f20 7468 6520 6375 7272 656e 7420 6672  o the current fr
-00002360: 616d 652e 0a20 2020 2020 2020 203a 7479  ame..        :ty
-00002370: 7065 2066 7261 6d65 3a20 7479 7069 6e67  pe frame: typing
-00002380: 2e4f 7074 696f 6e61 6c5b 666c 6f61 745d  .Optional[float]
-00002390: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000023a0: 6772 6f75 703a 2054 6865 206e 616d 6520  group: The name 
-000023b0: 6f66 2074 6865 2067 726f 7570 2074 6865  of the group the
-000023c0: 2046 2d43 7572 7665 2073 686f 756c 6420   F-Curve should 
-000023d0: 6265 2061 6464 6564 2074 6f20 6966 2069  be added to if i
-000023e0: 7420 646f 6573 6e27 7420 6578 6973 7420  t doesn't exist 
-000023f0: 7965 742e 0a20 2020 2020 2020 203a 7479  yet..        :ty
-00002400: 7065 2067 726f 7570 3a20 7479 7069 6e67  pe group: typing
-00002410: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
-00002420: 2020 2020 2020 203a 7061 7261 6d20 666c         :param fl
-00002430: 6167 3a20 0a20 2020 2020 2020 203a 7479  ag: .        :ty
-00002440: 7065 2066 6c61 673a 2074 7970 696e 672e  pe flag: typing.
-00002450: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-00002460: 5365 745d 0a20 2020 2020 2020 203a 7061  Set].        :pa
-00002470: 7261 6d20 6f70 7469 6f6e 733a 2020 2d20  ram options:  - 
-00002480: 6060 494e 5345 5254 4b45 595f 4e45 4544  ``INSERTKEY_NEED
-00002490: 4544 6060 204f 6e6c 7920 696e 7365 7274  ED`` Only insert
-000024a0: 206b 6579 6672 616d 6573 2077 6865 7265   keyframes where
-000024b0: 2074 6865 7927 7265 206e 6565 6465 6420   they're needed 
-000024c0: 696e 2074 6865 2072 656c 6576 616e 7420  in the relevant 
-000024d0: 462d 4375 7276 6573 2e20 2d20 6060 494e  F-Curves. - ``IN
-000024e0: 5345 5254 4b45 595f 5649 5355 414c 6060  SERTKEY_VISUAL``
-000024f0: 2049 6e73 6572 7420 6b65 7966 7261 6d65   Insert keyframe
-00002500: 7320 6261 7365 6420 6f6e 2027 7669 7375  s based on 'visu
-00002510: 616c 2074 7261 6e73 666f 726d 7327 2e20  al transforms'. 
-00002520: 2d20 6060 494e 5345 5254 4b45 595f 5859  - ``INSERTKEY_XY
-00002530: 5a5f 544f 5f52 4742 6060 2043 6f6c 6f72  Z_TO_RGB`` Color
-00002540: 2066 6f72 206e 6577 6c79 2061 6464 6564   for newly added
-00002550: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
-00002560: 462d 4375 7276 6573 2028 4c6f 6361 7469  F-Curves (Locati
-00002570: 6f6e 2c20 526f 7461 7469 6f6e 2c20 5363  on, Rotation, Sc
-00002580: 616c 6529 2069 7320 6261 7365 6420 6f6e  ale) is based on
-00002590: 2074 6865 2074 7261 6e73 666f 726d 2061   the transform a
-000025a0: 7869 732e 202d 2060 6049 4e53 4552 544b  xis. - ``INSERTK
-000025b0: 4559 5f52 4550 4c41 4345 6060 204f 6e6c  EY_REPLACE`` Onl
-000025c0: 7920 7265 706c 6163 6520 616c 7265 6164  y replace alread
-000025d0: 7920 6578 6973 7469 6e67 206b 6579 6672  y existing keyfr
-000025e0: 616d 6573 2e20 2d20 6060 494e 5345 5254  ames. - ``INSERT
-000025f0: 4b45 595f 4156 4149 4c41 424c 4560 6020  KEY_AVAILABLE`` 
-00002600: 4f6e 6c79 2069 6e73 6572 7420 696e 746f  Only insert into
-00002610: 2061 6c72 6561 6479 2065 7869 7374 696e   already existin
-00002620: 6720 462d 4375 7276 6573 2e20 2d20 6060  g F-Curves. - ``
-00002630: 494e 5345 5254 4b45 595f 4359 434c 455f  INSERTKEY_CYCLE_
-00002640: 4157 4152 4560 6020 5461 6b65 2063 7963  AWARE`` Take cyc
-00002650: 6c69 6320 6578 7472 6170 6f6c 6174 696f  lic extrapolatio
-00002660: 6e20 696e 746f 2061 6363 6f75 6e74 2028  n into account (
-00002670: 4379 636c 652d 4177 6172 6520 4b65 7969  Cycle-Aware Keyi
-00002680: 6e67 206f 7074 696f 6e29 2e0a 2020 2020  ng option)..    
-00002690: 2020 2020 3a74 7970 6520 6f70 7469 6f6e      :type option
-000026a0: 733a 2074 7970 696e 672e 4f70 7469 6f6e  s: typing.Option
-000026b0: 616c 5b74 7970 696e 672e 416e 795d 0a20  al[typing.Any]. 
-000026c0: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-000026d0: 6f6f 6c0a 2020 2020 2020 2020 3a72 6574  ool.        :ret
-000026e0: 7572 6e3a 2053 7563 6365 7373 206f 6620  urn: Success of 
-000026f0: 6b65 7966 7261 6d65 2069 6e73 6572 7469  keyframe inserti
-00002700: 6f6e 2e0a 2020 2020 2020 2020 2727 270a  on..        '''.
-00002710: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00002720: 2020 6465 6620 6b65 7973 2873 656c 6629    def keys(self)
-00002730: 202d 3e20 7479 7069 6e67 2e41 6e79 3a0a   -> typing.Any:.
-00002740: 2020 2020 2020 2020 2727 2720 5265 7475          ''' Retu
-00002750: 726e 7320 7468 6520 6b65 7973 206f 6620  rns the keys of 
-00002760: 7468 6973 206f 626a 6563 7473 2063 7573  this objects cus
-00002770: 746f 6d20 7072 6f70 6572 7469 6573 2028  tom properties (
-00002780: 6d61 7463 6865 7320 5079 7468 6f6e 2773  matches Python's
-00002790: 2064 6963 7469 6f6e 6172 7920 6675 6e63   dictionary func
-000027a0: 7469 6f6e 206f 6620 7468 6520 7361 6d65  tion of the same
-000027b0: 206e 616d 6529 2e0a 0a20 2020 2020 2020   name)...       
-000027c0: 203a 7274 7970 653a 2074 7970 696e 672e   :rtype: typing.
-000027d0: 416e 790a 2020 2020 2020 2020 3a72 6574  Any.        :ret
-000027e0: 7572 6e3a 2063 7573 746f 6d20 7072 6f70  urn: custom prop
-000027f0: 6572 7479 206b 6579 732e 0a20 2020 2020  erty keys..     
-00002800: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00002810: 6173 730a 0a20 2020 2064 6566 2070 6174  ass..    def pat
-00002820: 685f 6672 6f6d 5f69 6428 7365 6c66 2c20  h_from_id(self, 
-00002830: 7072 6f70 6572 7479 3a20 7479 7069 6e67  property: typing
-00002840: 2e4f 7074 696f 6e61 6c5b 7374 725d 203d  .Optional[str] =
-00002850: 2022 2229 202d 3e20 7374 723a 0a20 2020   "") -> str:.   
-00002860: 2020 2020 2027 2727 2052 6574 7572 6e73       ''' Returns
-00002870: 2074 6865 2064 6174 6120 7061 7468 2066   the data path f
-00002880: 726f 6d20 7468 6520 4944 2074 6f20 7468  rom the ID to th
-00002890: 6973 206f 626a 6563 7420 2873 7472 696e  is object (strin
-000028a0: 6729 2e0a 0a20 2020 2020 2020 203a 7061  g)...        :pa
-000028b0: 7261 6d20 7072 6f70 6572 7479 3a20 4f70  ram property: Op
-000028c0: 7469 6f6e 616c 2070 726f 7065 7274 7920  tional property 
-000028d0: 6e61 6d65 2077 6869 6368 2063 616e 2062  name which can b
-000028e0: 6520 7573 6564 2069 6620 7468 6520 7061  e used if the pa
-000028f0: 7468 2069 7320 746f 2061 2070 726f 7065  th is to a prope
-00002900: 7274 7920 6f66 2074 6869 7320 6f62 6a65  rty of this obje
-00002910: 6374 2e0a 2020 2020 2020 2020 3a74 7970  ct..        :typ
-00002920: 6520 7072 6f70 6572 7479 3a20 7479 7069  e property: typi
-00002930: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00002940: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00002950: 2073 7472 0a20 2020 2020 2020 203a 7265   str.        :re
-00002960: 7475 726e 3a20 6062 7079 2e74 7970 6573  turn: `bpy.types
-00002970: 2e62 7079 5f73 7472 7563 742e 6964 5f64  .bpy_struct.id_d
-00002980: 6174 6160 2074 6f20 7468 6973 2073 7472  ata` to this str
-00002990: 7563 7420 616e 6420 7072 6f70 6572 7479  uct and property
-000029a0: 2028 7768 656e 2067 6976 656e 292e 0a20   (when given).. 
-000029b0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-000029c0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-000029d0: 2070 6174 685f 7265 736f 6c76 6528 7365   path_resolve(se
-000029e0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-000029f0: 2020 2020 2020 2020 2070 6174 683a 2074           path: t
-00002a00: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00002a10: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
-00002a20: 2020 2020 2020 2020 2020 636f 6572 6365            coerce
-00002a30: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00002a40: 6c5b 626f 6f6c 5d20 3d20 5472 7565 293a  l[bool] = True):
-00002a50: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
-00002a60: 7572 6e73 2074 6865 2070 726f 7065 7274  urns the propert
-00002a70: 7920 6672 6f6d 2074 6865 2070 6174 682c  y from the path,
-00002a80: 2072 6169 7365 2061 6e20 6578 6365 7074   raise an except
-00002a90: 696f 6e20 7768 656e 206e 6f74 2066 6f75  ion when not fou
-00002aa0: 6e64 2e0a 0a20 2020 2020 2020 203a 7061  nd...        :pa
-00002ab0: 7261 6d20 7061 7468 3a20 7061 7468 2077  ram path: path w
-00002ac0: 6869 6368 2074 6869 7320 7072 6f70 6572  hich this proper
-00002ad0: 7479 2072 6573 6f6c 7665 732e 0a20 2020  ty resolves..   
-00002ae0: 2020 2020 203a 7479 7065 2070 6174 683a       :type path:
-00002af0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00002b00: 5b73 7472 5d0a 2020 2020 2020 2020 3a70  [str].        :p
-00002b10: 6172 616d 2063 6f65 7263 653a 206f 7074  aram coerce: opt
-00002b20: 696f 6e61 6c20 6172 6775 6d65 6e74 2c20  ional argument, 
-00002b30: 7768 656e 2054 7275 652c 2074 6865 2070  when True, the p
-00002b40: 726f 7065 7274 7920 7769 6c6c 2062 6520  roperty will be 
-00002b50: 636f 6e76 6572 7465 6420 696e 746f 2069  converted into i
-00002b60: 7473 2050 7974 686f 6e20 7265 7072 6573  ts Python repres
-00002b70: 656e 7461 7469 6f6e 2e0a 2020 2020 2020  entation..      
-00002b80: 2020 3a74 7970 6520 636f 6572 6365 3a20    :type coerce: 
-00002b90: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00002ba0: 626f 6f6c 5d0a 2020 2020 2020 2020 2727  bool].        ''
-00002bb0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00002bc0: 2020 2020 6465 6620 706f 7028 7365 6c66      def pop(self
-00002bd0: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
-00002be0: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
-00002bf0: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
-00002c00: 2020 2020 2064 6566 6175 6c74 3a20 7479       default: ty
-00002c10: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-00002c20: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
-00002c30: 293a 0a20 2020 2020 2020 2027 2727 2052  ):.        ''' R
-00002c40: 656d 6f76 6520 616e 6420 7265 7475 726e  emove and return
-00002c50: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
-00002c60: 6520 6375 7374 6f6d 2070 726f 7065 7274  e custom propert
-00002c70: 7920 6173 7369 676e 6564 2074 6f20 6b65  y assigned to ke
-00002c80: 7920 6f72 2064 6566 6175 6c74 2077 6865  y or default whe
-00002c90: 6e20 6e6f 7420 666f 756e 6420 286d 6174  n not found (mat
-00002ca0: 6368 6573 2050 7974 686f 6e27 7320 6469  ches Python's di
-00002cb0: 6374 696f 6e61 7279 2066 756e 6374 696f  ctionary functio
-00002cc0: 6e20 6f66 2074 6865 2073 616d 6520 6e61  n of the same na
-00002cd0: 6d65 292e 0a0a 2020 2020 2020 2020 3a70  me)...        :p
-00002ce0: 6172 616d 206b 6579 3a20 5468 6520 6b65  aram key: The ke
-00002cf0: 7920 6173 736f 6369 6174 6564 2077 6974  y associated wit
-00002d00: 6820 7468 6520 6375 7374 6f6d 2070 726f  h the custom pro
-00002d10: 7065 7274 792e 0a20 2020 2020 2020 203a  perty..        :
-00002d20: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
-00002d30: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
-00002d40: 2020 2020 2020 203a 7061 7261 6d20 6465         :param de
-00002d50: 6661 756c 743a 204f 7074 696f 6e61 6c20  fault: Optional 
-00002d60: 6172 6775 6d65 6e74 2066 6f72 2074 6865  argument for the
-00002d70: 2076 616c 7565 2074 6f20 7265 7475 726e   value to return
-00002d80: 2069 6620 2a6b 6579 2a20 6973 206e 6f74   if *key* is not
-00002d90: 2066 6f75 6e64 2e0a 2020 2020 2020 2020   found..        
-00002da0: 3a74 7970 6520 6465 6661 756c 743a 2074  :type default: t
-00002db0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-00002dc0: 7970 696e 672e 416e 795d 0a20 2020 2020  yping.Any].     
-00002dd0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00002de0: 6173 730a 0a20 2020 2064 6566 2070 726f  ass..    def pro
-00002df0: 7065 7274 795f 6f76 6572 7269 6461 626c  perty_overridabl
-00002e00: 655f 6c69 6272 6172 795f 7365 7428 7365  e_library_set(se
-00002e10: 6c66 2c20 7072 6f70 6572 7479 2c20 6f76  lf, property, ov
-00002e20: 6572 7269 6461 626c 6529 202d 3e20 626f  erridable) -> bo
-00002e30: 6f6c 3a0a 2020 2020 2020 2020 2727 2720  ol:.        ''' 
-00002e40: 4465 6669 6e65 2061 2070 726f 7065 7274  Define a propert
-00002e50: 7920 6173 206f 7665 7272 6964 6162 6c65  y as overridable
-00002e60: 206f 7220 6e6f 7420 286f 6e6c 7920 666f   or not (only fo
-00002e70: 7220 6375 7374 6f6d 2070 726f 7065 7274  r custom propert
-00002e80: 6965 7321 292e 0a0a 2020 2020 2020 2020  ies!)...        
-00002e90: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
-00002ea0: 2020 2020 203a 7265 7475 726e 3a20 5472       :return: Tr
-00002eb0: 7565 2077 6865 6e20 7468 6520 6f76 6572  ue when the over
-00002ec0: 7269 6461 626c 6520 7374 6174 7573 206f  ridable status o
-00002ed0: 6620 7468 6520 7072 6f70 6572 7479 2077  f the property w
-00002ee0: 6173 2073 7563 6365 7373 6675 6c6c 7920  as successfully 
-00002ef0: 7365 742e 0a20 2020 2020 2020 2027 2727  set..        '''
-00002f00: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00002f10: 2020 2064 6566 2070 726f 7065 7274 795f     def property_
-00002f20: 756e 7365 7428 7365 6c66 2c20 7072 6f70  unset(self, prop
-00002f30: 6572 7479 293a 0a20 2020 2020 2020 2027  erty):.        '
-00002f40: 2727 2055 6e73 6574 2061 2070 726f 7065  '' Unset a prope
-00002f50: 7274 792c 2077 696c 6c20 7573 6520 6465  rty, will use de
-00002f60: 6661 756c 7420 7661 6c75 6520 6166 7465  fault value afte
-00002f70: 7277 6172 642e 0a0a 2020 2020 2020 2020  rward...        
-00002f80: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-00002f90: 0a0a 2020 2020 6465 6620 7479 7065 5f72  ..    def type_r
-00002fa0: 6563 6173 7428 7365 6c66 2920 2d3e 2027  ecast(self) -> '
-00002fb0: 6270 795f 7374 7275 6374 273a 0a20 2020  bpy_struct':.   
-00002fc0: 2020 2020 2027 2727 2052 6574 7572 6e20       ''' Return 
-00002fd0: 6120 6e65 7720 696e 7374 616e 6365 2c20  a new instance, 
-00002fe0: 7468 6973 2069 7320 6e65 6564 6564 2062  this is needed b
-00002ff0: 6563 6175 7365 2074 7970 6573 2073 7563  ecause types suc
-00003000: 6820 6173 2074 6578 7475 7265 7320 6361  h as textures ca
-00003010: 6e20 6265 2063 6861 6e67 6564 2061 7420  n be changed at 
-00003020: 7275 6e74 696d 652e 0a0a 2020 2020 2020  runtime...      
-00003030: 2020 3a72 7479 7065 3a20 2762 7079 5f73    :rtype: 'bpy_s
-00003040: 7472 7563 7427 0a20 2020 2020 2020 203a  truct'.        :
-00003050: 7265 7475 726e 3a20 6120 6e65 7720 696e  return: a new in
-00003060: 7374 616e 6365 206f 6620 7468 6973 206f  stance of this o
-00003070: 626a 6563 7420 7769 7468 2074 6865 2074  bject with the t
-00003080: 7970 6520 696e 6974 6961 6c69 7a65 6420  ype initialized 
-00003090: 6167 6169 6e2e 0a20 2020 2020 2020 2027  again..        '
-000030a0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-000030b0: 0a20 2020 2064 6566 2076 616c 7565 7328  .    def values(
-000030c0: 7365 6c66 2920 2d3e 2074 7970 696e 672e  self) -> typing.
-000030d0: 416e 793a 0a20 2020 2020 2020 2027 2727  Any:.        '''
-000030e0: 2052 6574 7572 6e73 2074 6865 2076 616c   Returns the val
-000030f0: 7565 7320 6f66 2074 6869 7320 6f62 6a65  ues of this obje
-00003100: 6374 7320 6375 7374 6f6d 2070 726f 7065  cts custom prope
-00003110: 7274 6965 7320 286d 6174 6368 6573 2050  rties (matches P
-00003120: 7974 686f 6e27 7320 6469 6374 696f 6e61  ython's dictiona
-00003130: 7279 2066 756e 6374 696f 6e20 6f66 2074  ry function of t
-00003140: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
-00003150: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00003160: 7479 7069 6e67 2e41 6e79 0a20 2020 2020  typing.Any.     
-00003170: 2020 203a 7265 7475 726e 3a20 6375 7374     :return: cust
-00003180: 6f6d 2070 726f 7065 7274 7920 7661 6c75  om property valu
-00003190: 6573 2e0a 2020 2020 2020 2020 2727 270a  es..        '''.
-000031a0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000031b0: 2020 6465 6620 5f5f 6765 7469 7465 6d5f    def __getitem_
-000031c0: 5f28 7365 6c66 2c20 6b65 793a 2074 7970  _(self, key: typ
-000031d0: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
-000031e0: 7472 5d29 202d 3e20 2774 7970 696e 672e  tr]) -> 'typing.
-000031f0: 416e 7927 3a0a 2020 2020 2020 2020 2727  Any':.        ''
-00003200: 2720 0a0a 2020 2020 2020 2020 3a70 6172  ' ..        :par
-00003210: 616d 206b 6579 3a20 0a20 2020 2020 2020  am key: .       
-00003220: 203a 7479 7065 206b 6579 3a20 7479 7069   :type key: typi
-00003230: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
-00003240: 725d 0a20 2020 2020 2020 203a 7274 7970  r].        :rtyp
-00003250: 653a 2027 7479 7069 6e67 2e41 6e79 270a  e: 'typing.Any'.
-00003260: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00003270: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00003280: 6620 5f5f 7365 7469 7465 6d5f 5f28 7365  f __setitem__(se
-00003290: 6c66 2c20 6b65 793a 2074 7970 696e 672e  lf, key: typing.
-000032a0: 556e 696f 6e5b 696e 742c 2073 7472 5d2c  Union[int, str],
-000032b0: 2076 616c 7565 3a20 2774 7970 696e 672e   value: 'typing.
-000032c0: 416e 7927 293a 0a20 2020 2020 2020 2027  Any'):.        '
-000032d0: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
-000032e0: 7261 6d20 6b65 793a 200a 2020 2020 2020  ram key: .      
-000032f0: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
-00003300: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
-00003310: 7472 5d0a 2020 2020 2020 2020 3a70 6172  tr].        :par
-00003320: 616d 2076 616c 7565 3a20 0a20 2020 2020  am value: .     
-00003330: 2020 203a 7479 7065 2076 616c 7565 3a20     :type value: 
-00003340: 2774 7970 696e 672e 416e 7927 0a20 2020  'typing.Any'.   
-00003350: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00003360: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
-00003370: 5f64 656c 6974 656d 5f5f 2873 656c 662c  _delitem__(self,
-00003380: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
-00003390: 6f6e 5b69 6e74 2c20 7374 725d 2920 2d3e  on[int, str]) ->
-000033a0: 2027 7479 7069 6e67 2e41 6e79 273a 0a20   'typing.Any':. 
-000033b0: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
-000033c0: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
-000033d0: 200a 2020 2020 2020 2020 3a74 7970 6520   .        :type 
-000033e0: 6b65 793a 2074 7970 696e 672e 556e 696f  key: typing.Unio
-000033f0: 6e5b 696e 742c 2073 7472 5d0a 2020 2020  n[int, str].    
-00003400: 2020 2020 3a72 7479 7065 3a20 2774 7970      :rtype: 'typ
-00003410: 696e 672e 416e 7927 0a20 2020 2020 2020  ing.Any'.       
-00003420: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00003430: 730a 0a0a 636c 6173 7320 6270 795f 7072  s...class bpy_pr
-00003440: 6f70 5f63 6f6c 6c65 6374 696f 6e28 7479  op_collection(ty
-00003450: 7069 6e67 2e47 656e 6572 6963 5b47 656e  ping.Generic[Gen
-00003460: 6572 6963 5479 7065 5d29 3a0a 2020 2020  ericType]):.    
-00003470: 2727 2720 6275 696c 742d 696e 2063 6c61  ''' built-in cla
-00003480: 7373 2075 7365 6420 666f 7220 616c 6c20  ss used for all 
-00003490: 636f 6c6c 6563 7469 6f6e 732e 0a20 2020  collections..   
-000034a0: 2027 2727 0a0a 2020 2020 6465 6620 6669   '''..    def fi
-000034b0: 6e64 2873 656c 662c 206b 6579 3a20 7479  nd(self, key: ty
-000034c0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-000034d0: 725d 2920 2d3e 2069 6e74 3a0a 2020 2020  r]) -> int:.    
-000034e0: 2020 2020 2727 2720 5265 7475 726e 7320      ''' Returns 
-000034f0: 7468 6520 696e 6465 7820 6f66 2061 206b  the index of a k
-00003500: 6579 2069 6e20 6120 636f 6c6c 6563 7469  ey in a collecti
-00003510: 6f6e 206f 7220 2d31 2077 6865 6e20 6e6f  on or -1 when no
-00003520: 7420 666f 756e 6420 286d 6174 6368 6573  t found (matches
-00003530: 2050 7974 686f 6e27 7320 7374 7269 6e67   Python's string
-00003540: 2066 696e 6420 6675 6e63 7469 6f6e 206f   find function o
-00003550: 6620 7468 6520 7361 6d65 206e 616d 6529  f the same name)
-00003560: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00003570: 6d20 6b65 793a 2054 6865 2069 6465 6e74  m key: The ident
-00003580: 6966 6965 7220 666f 7220 7468 6520 636f  ifier for the co
-00003590: 6c6c 6563 7469 6f6e 206d 656d 6265 722e  llection member.
-000035a0: 0a20 2020 2020 2020 203a 7479 7065 206b  .        :type k
-000035b0: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
-000035c0: 6e61 6c5b 7374 725d 0a20 2020 2020 2020  nal[str].       
-000035d0: 203a 7274 7970 653a 2069 6e74 0a20 2020   :rtype: int.   
-000035e0: 2020 2020 203a 7265 7475 726e 3a20 696e       :return: in
-000035f0: 6465 7820 6f66 2074 6865 206b 6579 2e0a  dex of the key..
-00003600: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00003610: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00003620: 6620 666f 7265 6163 685f 6765 7428 7365  f foreach_get(se
-00003630: 6c66 2c20 6174 7472 2c20 7365 7129 3a0a  lf, attr, seq):.
-00003640: 2020 2020 2020 2020 2727 2720 5468 6973          ''' This
-00003650: 2069 7320 6120 6675 6e63 7469 6f6e 2074   is a function t
-00003660: 6f20 6769 7665 2066 6173 7420 6163 6365  o give fast acce
-00003670: 7373 2074 6f20 6174 7472 6962 7574 6573  ss to attributes
-00003680: 2077 6974 6869 6e20 6120 636f 6c6c 6563   within a collec
-00003690: 7469 6f6e 2e20 4f6e 6c79 2077 6f72 6b73  tion. Only works
-000036a0: 2066 6f72 2027 6261 7369 6320 7479 7065   for 'basic type
-000036b0: 2720 7072 6f70 6572 7469 6573 2028 626f  ' properties (bo
-000036c0: 6f6c 2c20 696e 7420 616e 6420 666c 6f61  ol, int and floa
-000036d0: 7429 2120 4d75 6c74 692d 6469 6d65 6e73  t)! Multi-dimens
-000036e0: 696f 6e61 6c20 6172 7261 7973 2028 6c69  ional arrays (li
-000036f0: 6b65 2061 7272 6179 206f 6620 7665 6374  ke array of vect
-00003700: 6f72 7329 2077 696c 6c20 6265 2066 6c61  ors) will be fla
-00003710: 7474 656e 6564 2069 6e74 6f20 7365 712e  ttened into seq.
-00003720: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00003730: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00003740: 6465 6620 666f 7265 6163 685f 7365 7428  def foreach_set(
-00003750: 7365 6c66 2c20 6174 7472 2c20 7365 7129  self, attr, seq)
-00003760: 3a0a 2020 2020 2020 2020 2727 2720 5468  :.        ''' Th
-00003770: 6973 2069 7320 6120 6675 6e63 7469 6f6e  is is a function
-00003780: 2074 6f20 6769 7665 2066 6173 7420 6163   to give fast ac
-00003790: 6365 7373 2074 6f20 6174 7472 6962 7574  cess to attribut
-000037a0: 6573 2077 6974 6869 6e20 6120 636f 6c6c  es within a coll
-000037b0: 6563 7469 6f6e 2e20 4f6e 6c79 2077 6f72  ection. Only wor
-000037c0: 6b73 2066 6f72 2027 6261 7369 6320 7479  ks for 'basic ty
-000037d0: 7065 2720 7072 6f70 6572 7469 6573 2028  pe' properties (
-000037e0: 626f 6f6c 2c20 696e 7420 616e 6420 666c  bool, int and fl
-000037f0: 6f61 7429 2120 7365 7120 6d75 7374 2062  oat)! seq must b
-00003800: 6520 756e 692d 6469 6d65 6e73 696f 6e61  e uni-dimensiona
-00003810: 6c2c 206d 756c 7469 2d64 696d 656e 7369  l, multi-dimensi
-00003820: 6f6e 616c 2061 7272 6179 7320 286c 696b  onal arrays (lik
-00003830: 6520 6172 7261 7920 6f66 2076 6563 746f  e array of vecto
-00003840: 7273 2920 7769 6c6c 2062 6520 7265 2d63  rs) will be re-c
-00003850: 7265 6174 6564 2066 726f 6d20 6974 2e0a  reated from it..
-00003860: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00003870: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00003880: 6566 2067 6574 2873 656c 662c 0a20 2020  ef get(self,.   
-00003890: 2020 2020 2020 2020 206b 6579 3a20 7479           key: ty
-000038a0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-000038b0: 725d 2c0a 2020 2020 2020 2020 2020 2020  r],.            
-000038c0: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
-000038d0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-000038e0: 416e 795d 203d 204e 6f6e 6529 3a0a 2020  Any] = None):.  
-000038f0: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
-00003900: 7320 7468 6520 7661 6c75 6520 6f66 2074  s the value of t
-00003910: 6865 2069 7465 6d20 6173 7369 676e 6564  he item assigned
-00003920: 2074 6f20 6b65 7920 6f72 2064 6566 6175   to key or defau
-00003930: 6c74 2077 6865 6e20 6e6f 7420 666f 756e  lt when not foun
-00003940: 6420 286d 6174 6368 6573 2050 7974 686f  d (matches Pytho
-00003950: 6e27 7320 6469 6374 696f 6e61 7279 2066  n's dictionary f
-00003960: 756e 6374 696f 6e20 6f66 2074 6865 2073  unction of the s
-00003970: 616d 6520 6e61 6d65 292e 0a0a 2020 2020  ame name)...    
-00003980: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
-00003990: 5468 6520 6964 656e 7469 6669 6572 2066  The identifier f
-000039a0: 6f72 2074 6865 2063 6f6c 6c65 6374 696f  or the collectio
-000039b0: 6e20 6d65 6d62 6572 2e0a 2020 2020 2020  n member..      
-000039c0: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
-000039d0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-000039e0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-000039f0: 2064 6566 6175 6c74 3a20 4f70 7469 6f6e   default: Option
-00003a00: 616c 2061 7267 756d 656e 7420 666f 7220  al argument for 
-00003a10: 7468 6520 7661 6c75 6520 746f 2072 6574  the value to ret
-00003a20: 7572 6e20 6966 202a 6b65 792a 2069 7320  urn if *key* is 
-00003a30: 6e6f 7420 666f 756e 642e 0a20 2020 2020  not found..     
-00003a40: 2020 203a 7479 7065 2064 6566 6175 6c74     :type default
-00003a50: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00003a60: 6c5b 7479 7069 6e67 2e41 6e79 5d0a 2020  l[typing.Any].  
-00003a70: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00003a80: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00003a90: 6974 656d 7328 7365 6c66 2920 2d3e 2074  items(self) -> t
-00003aa0: 7970 696e 672e 4c69 7374 3a0a 2020 2020  yping.List:.    
-00003ab0: 2020 2020 2727 2720 5265 7475 726e 2074      ''' Return t
-00003ac0: 6865 2069 6465 6e74 6966 6965 7273 206f  he identifiers o
-00003ad0: 6620 636f 6c6c 6563 7469 6f6e 206d 656d  f collection mem
-00003ae0: 6265 7273 2028 6d61 7463 6869 6e67 2050  bers (matching P
-00003af0: 7974 686f 6e27 7320 6469 6374 2e69 7465  ython's dict.ite
-00003b00: 6d73 2829 2066 756e 6374 696f 6e61 6c69  ms() functionali
-00003b10: 7479 292e 0a0a 2020 2020 2020 2020 3a72  ty)...        :r
-00003b20: 7479 7065 3a20 7479 7069 6e67 2e4c 6973  type: typing.Lis
-00003b30: 740a 2020 2020 2020 2020 3a72 6574 7572  t.        :retur
-00003b40: 6e3a 2028 6b65 792c 2076 616c 7565 2920  n: (key, value) 
-00003b50: 7061 6972 7320 666f 7220 6561 6368 206d  pairs for each m
-00003b60: 656d 6265 7220 6f66 2074 6869 7320 636f  ember of this co
-00003b70: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
-00003b80: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00003b90: 7373 0a0a 2020 2020 6465 6620 6b65 7973  ss..    def keys
-00003ba0: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
-00003bb0: 2e4c 6973 745b 7374 725d 3a0a 2020 2020  .List[str]:.    
-00003bc0: 2020 2020 2727 2720 5265 7475 726e 2074      ''' Return t
-00003bd0: 6865 2069 6465 6e74 6966 6965 7273 206f  he identifiers o
-00003be0: 6620 636f 6c6c 6563 7469 6f6e 206d 656d  f collection mem
-00003bf0: 6265 7273 2028 6d61 7463 6869 6e67 2050  bers (matching P
-00003c00: 7974 686f 6e27 7320 6469 6374 2e6b 6579  ython's dict.key
-00003c10: 7328 2920 6675 6e63 7469 6f6e 616c 6974  s() functionalit
-00003c20: 7929 2e0a 0a20 2020 2020 2020 203a 7274  y)...        :rt
-00003c30: 7970 653a 2074 7970 696e 672e 4c69 7374  ype: typing.List
-00003c40: 5b73 7472 5d0a 2020 2020 2020 2020 3a72  [str].        :r
-00003c50: 6574 7572 6e3a 2074 6865 2069 6465 6e74  eturn: the ident
-00003c60: 6966 6965 7273 2066 6f72 2065 6163 6820  ifiers for each 
-00003c70: 6d65 6d62 6572 206f 6620 7468 6973 2063  member of this c
-00003c80: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
-00003c90: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00003ca0: 6173 730a 0a20 2020 2064 6566 2076 616c  ass..    def val
-00003cb0: 7565 7328 7365 6c66 2920 2d3e 2074 7970  ues(self) -> typ
-00003cc0: 696e 672e 4c69 7374 3a0a 2020 2020 2020  ing.List:.      
-00003cd0: 2020 2727 2720 5265 7475 726e 2074 6865    ''' Return the
-00003ce0: 2076 616c 7565 7320 6f66 2063 6f6c 6c65   values of colle
-00003cf0: 6374 696f 6e20 286d 6174 6368 696e 6720  ction (matching 
-00003d00: 5079 7468 6f6e 2773 2064 6963 742e 7661  Python's dict.va
-00003d10: 6c75 6573 2829 2066 756e 6374 696f 6e61  lues() functiona
-00003d20: 6c69 7479 292e 0a0a 2020 2020 2020 2020  lity)...        
-00003d30: 3a72 7479 7065 3a20 7479 7069 6e67 2e4c  :rtype: typing.L
-00003d40: 6973 740a 2020 2020 2020 2020 3a72 6574  ist.        :ret
-00003d50: 7572 6e3a 2074 6865 206d 656d 6265 7273  urn: the members
-00003d60: 206f 6620 7468 6973 2063 6f6c 6c65 6374   of this collect
-00003d70: 696f 6e2e 0a20 2020 2020 2020 2027 2727  ion..        '''
-00003d80: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00003d90: 2020 2064 6566 205f 5f67 6574 6974 656d     def __getitem
-00003da0: 5f5f 2873 656c 662c 206b 6579 3a20 7479  __(self, key: ty
-00003db0: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-00003dc0: 7374 725d 2920 2d3e 2027 4765 6e65 7269  str]) -> 'Generi
-00003dd0: 6354 7970 6527 3a0a 2020 2020 2020 2020  cType':.        
-00003de0: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
-00003df0: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
-00003e00: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
-00003e10: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-00003e20: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
-00003e30: 7970 653a 2027 4765 6e65 7269 6354 7970  ype: 'GenericTyp
-00003e40: 6527 0a20 2020 2020 2020 2027 2727 0a20  e'.        '''. 
-00003e50: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00003e60: 2064 6566 205f 5f73 6574 6974 656d 5f5f   def __setitem__
-00003e70: 2873 656c 662c 206b 6579 3a20 7479 7069  (self, key: typi
-00003e80: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
-00003e90: 725d 2c20 7661 6c75 653a 2027 4765 6e65  r], value: 'Gene
-00003ea0: 7269 6354 7970 6527 293a 0a20 2020 2020  ricType'):.     
-00003eb0: 2020 2027 2727 200a 0a20 2020 2020 2020     ''' ..       
-00003ec0: 203a 7061 7261 6d20 6b65 793a 200a 2020   :param key: .  
-00003ed0: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
-00003ee0: 2074 7970 696e 672e 556e 696f 6e5b 696e   typing.Union[in
-00003ef0: 742c 2073 7472 5d0a 2020 2020 2020 2020  t, str].        
-00003f00: 3a70 6172 616d 2076 616c 7565 3a20 0a20  :param value: . 
-00003f10: 2020 2020 2020 203a 7479 7065 2076 616c         :type val
-00003f20: 7565 3a20 2747 656e 6572 6963 5479 7065  ue: 'GenericType
-00003f30: 270a 2020 2020 2020 2020 2727 270a 2020  '.        '''.  
-00003f40: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00003f50: 6465 6620 5f5f 6465 6c69 7465 6d5f 5f28  def __delitem__(
-00003f60: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
-00003f70: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
-00003f80: 5d29 202d 3e20 2747 656e 6572 6963 5479  ]) -> 'GenericTy
-00003f90: 7065 273a 0a20 2020 2020 2020 2027 2727  pe':.        '''
-00003fa0: 200a 0a20 2020 2020 2020 203a 7061 7261   ..        :para
-00003fb0: 6d20 6b65 793a 200a 2020 2020 2020 2020  m key: .        
-00003fc0: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
-00003fd0: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
-00003fe0: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
-00003ff0: 3a20 2747 656e 6572 6963 5479 7065 270a  : 'GenericType'.
-00004000: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00004010: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00004020: 6620 5f5f 6974 6572 5f5f 2873 656c 6629  f __iter__(self)
-00004030: 202d 3e20 7479 7069 6e67 2e49 7465 7261   -> typing.Itera
-00004040: 746f 725b 2747 656e 6572 6963 5479 7065  tor['GenericType
-00004050: 275d 3a0a 2020 2020 2020 2020 2727 2720  ']:.        ''' 
-00004060: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00004070: 3a20 7479 7069 6e67 2e49 7465 7261 746f  : typing.Iterato
-00004080: 725b 2747 656e 6572 6963 5479 7065 275d  r['GenericType']
-00004090: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-000040a0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000040b0: 6566 205f 5f6e 6578 745f 5f28 7365 6c66  ef __next__(self
-000040c0: 2920 2d3e 2027 4765 6e65 7269 6354 7970  ) -> 'GenericTyp
-000040d0: 6527 3a0a 2020 2020 2020 2020 2727 2720  e':.        ''' 
-000040e0: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-000040f0: 3a20 2747 656e 6572 6963 5479 7065 270a  : 'GenericType'.
-00004100: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00004110: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00004120: 6620 5f5f 6c65 6e5f 5f28 7365 6c66 2920  f __len__(self) 
-00004130: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00004140: 2727 2720 0a0a 2020 2020 2020 2020 3a72  ''' ..        :r
-00004150: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
+00001b80: 5b69 6e74 5d0a 2020 2020 2020 2020 3a72  [int].        :r
+00001b90: 7479 7065 3a20 2746 4375 7276 6527 0a20  type: 'FCurve'. 
+00001ba0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00001bb0: 5468 6520 6472 6976 6572 2873 2920 6164  The driver(s) ad
+00001bc0: 6465 642e 0a20 2020 2020 2020 2027 2727  ded..        '''
+00001bd0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00001be0: 2020 2064 6566 2064 7269 7665 725f 7265     def driver_re
+00001bf0: 6d6f 7665 2873 656c 662c 0a20 2020 2020  move(self,.     
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2070 6174 683a 2074 7970 696e 672e 4f70   path: typing.Op
+00001c20: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 2020 2069 6e64 6578 3a20 7479 7069 6e67     index: typing
+00001c50: 2e4f 7074 696f 6e61 6c5b 696e 745d 203d  .Optional[int] =
+00001c60: 202d 3129 202d 3e20 626f 6f6c 3a0a 2020   -1) -> bool:.  
+00001c70: 2020 2020 2020 2727 2720 5265 6d6f 7665        ''' Remove
+00001c80: 2064 7269 7665 7228 7329 2066 726f 6d20   driver(s) from 
+00001c90: 7468 6520 6769 7665 6e20 7072 6f70 6572  the given proper
+00001ca0: 7479 0a0a 2020 2020 2020 2020 3a70 6172  ty..        :par
+00001cb0: 616d 2070 6174 683a 2070 6174 6820 746f  am path: path to
+00001cc0: 2074 6865 2070 726f 7065 7274 7920 746f   the property to
+00001cd0: 2064 7269 7665 2c20 616e 616c 6f67 6f75   drive, analogou
+00001ce0: 7320 746f 2074 6865 2066 6375 7276 6527  s to the fcurve'
+00001cf0: 7320 6461 7461 2070 6174 682e 0a20 2020  s data path..   
+00001d00: 2020 2020 203a 7479 7065 2070 6174 683a       :type path:
+00001d10: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00001d20: 5b73 7472 5d0a 2020 2020 2020 2020 3a70  [str].        :p
+00001d30: 6172 616d 2069 6e64 6578 3a20 6172 7261  aram index: arra
+00001d40: 7920 696e 6465 7820 6f66 2074 6865 2070  y index of the p
+00001d50: 726f 7065 7274 7920 6472 6976 652e 2044  roperty drive. D
+00001d60: 6566 6175 6c74 7320 746f 202d 3120 666f  efaults to -1 fo
+00001d70: 7220 616c 6c20 696e 6469 6365 7320 6f72  r all indices or
+00001d80: 2061 2073 696e 676c 6520 6368 616e 6e65   a single channe
+00001d90: 6c20 6966 2074 6865 2070 726f 7065 7274  l if the propert
+00001da0: 7920 6973 206e 6f74 2061 6e20 6172 7261  y is not an arra
+00001db0: 792e 0a20 2020 2020 2020 203a 7479 7065  y..        :type
+00001dc0: 2069 6e64 6578 3a20 7479 7069 6e67 2e4f   index: typing.O
+00001dd0: 7074 696f 6e61 6c5b 696e 745d 0a20 2020  ptional[int].   
+00001de0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+00001df0: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
+00001e00: 6e3a 2053 7563 6365 7373 206f 6620 6472  n: Success of dr
+00001e10: 6976 6572 2072 656d 6f76 616c 2e0a 2020  iver removal..  
+00001e20: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00001e30: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00001e40: 6765 7428 7365 6c66 2c0a 2020 2020 2020  get(self,.      
+00001e50: 2020 2020 2020 6b65 793a 2074 7970 696e        key: typin
+00001e60: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
+00001e70: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+00001e80: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
+00001e90: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
+00001ea0: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
+00001eb0: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
+00001ec0: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00001ed0: 6375 7374 6f6d 2070 726f 7065 7274 7920  custom property 
+00001ee0: 6173 7369 676e 6564 2074 6f20 6b65 7920  assigned to key 
+00001ef0: 6f72 2064 6566 6175 6c74 2077 6865 6e20  or default when 
+00001f00: 6e6f 7420 666f 756e 6420 286d 6174 6368  not found (match
+00001f10: 6573 2050 7974 686f 6e27 7320 6469 6374  es Python's dict
+00001f20: 696f 6e61 7279 2066 756e 6374 696f 6e20  ionary function 
+00001f30: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
+00001f40: 292e 0a0a 2020 2020 2020 2020 3a70 6172  )...        :par
+00001f50: 616d 206b 6579 3a20 5468 6520 6b65 7920  am key: The key 
+00001f60: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00001f70: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
+00001f80: 7274 792e 0a20 2020 2020 2020 203a 7479  rty..        :ty
+00001f90: 7065 206b 6579 3a20 7479 7069 6e67 2e4f  pe key: typing.O
+00001fa0: 7074 696f 6e61 6c5b 7374 725d 0a20 2020  ptional[str].   
+00001fb0: 2020 2020 203a 7061 7261 6d20 6465 6661       :param defa
+00001fc0: 756c 743a 204f 7074 696f 6e61 6c20 6172  ult: Optional ar
+00001fd0: 6775 6d65 6e74 2066 6f72 2074 6865 2076  gument for the v
+00001fe0: 616c 7565 2074 6f20 7265 7475 726e 2069  alue to return i
+00001ff0: 6620 2a6b 6579 2a20 6973 206e 6f74 2066  f *key* is not f
+00002000: 6f75 6e64 2e0a 2020 2020 2020 2020 3a74  ound..        :t
+00002010: 7970 6520 6465 6661 756c 743a 2074 7970  ype default: typ
+00002020: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+00002030: 696e 672e 416e 795d 0a20 2020 2020 2020  ing.Any].       
+00002040: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00002050: 730a 0a20 2020 2064 6566 2069 645f 7072  s..    def id_pr
+00002060: 6f70 6572 7469 6573 5f63 6c65 6172 2873  operties_clear(s
+00002070: 656c 6629 3a0a 2020 2020 2020 2020 2727  elf):.        ''
+00002080: 2720 0a0a 2020 2020 2020 2020 2727 270a  ' ..        '''.
+00002090: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000020a0: 2020 6465 6620 6964 5f70 726f 7065 7274    def id_propert
+000020b0: 6965 735f 656e 7375 7265 2873 656c 6629  ies_ensure(self)
+000020c0: 202d 3e20 7479 7069 6e67 2e41 6e79 3a0a   -> typing.Any:.
+000020d0: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
+000020e0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
+000020f0: 7069 6e67 2e41 6e79 0a20 2020 2020 2020  ping.Any.       
+00002100: 203a 7265 7475 726e 3a20 7468 6520 7061   :return: the pa
+00002110: 7265 6e74 2067 726f 7570 2066 6f72 2061  rent group for a
+00002120: 6e20 524e 4120 7374 7275 6374 2773 2063  n RNA struct's c
+00002130: 7573 746f 6d20 4944 5072 6f70 6572 7469  ustom IDProperti
+00002140: 6573 2e0a 2020 2020 2020 2020 2727 270a  es..        '''.
+00002150: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00002160: 2020 6465 6620 6964 5f70 726f 7065 7274    def id_propert
+00002170: 6965 735f 7569 2873 656c 662c 206b 6579  ies_ui(self, key
+00002180: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00002190: 6c5b 7479 7069 6e67 2e41 6e79 5d29 202d  l[typing.Any]) -
+000021a0: 3e20 7479 7069 6e67 2e41 6e79 3a0a 2020  > typing.Any:.  
+000021b0: 2020 2020 2020 2727 2720 0a0a 2020 2020        ''' ..    
+000021c0: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
+000021d0: 2053 7472 696e 6720 6e61 6d65 206f 6620   String name of 
+000021e0: 7468 6520 7072 6f70 6572 7479 2e0a 2020  the property..  
+000021f0: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
+00002200: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00002210: 5b74 7970 696e 672e 416e 795d 0a20 2020  [typing.Any].   
+00002220: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
+00002230: 696e 672e 416e 790a 2020 2020 2020 2020  ing.Any.        
+00002240: 3a72 6574 7572 6e3a 2052 6574 7572 6e20  :return: Return 
+00002250: 616e 206f 626a 6563 7420 7573 6564 2074  an object used t
+00002260: 6f20 6d61 6e61 6765 2061 6e20 4944 5072  o manage an IDPr
+00002270: 6f70 6572 7479 2773 2055 4920 6461 7461  operty's UI data
+00002280: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00002290: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+000022a0: 6465 6620 6973 5f70 726f 7065 7274 795f  def is_property_
+000022b0: 6869 6464 656e 2873 656c 662c 2070 726f  hidden(self, pro
+000022c0: 7065 7274 7929 202d 3e20 626f 6f6c 3a0a  perty) -> bool:.
+000022d0: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
+000022e0: 6b20 6966 2061 2070 726f 7065 7274 7920  k if a property 
+000022f0: 6973 2068 6964 6465 6e2e 0a0a 2020 2020  is hidden...    
+00002300: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00002310: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00002320: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
+00002330: 7072 6f70 6572 7479 2069 7320 6869 6464  property is hidd
+00002340: 656e 2e0a 2020 2020 2020 2020 2727 270a  en..        '''.
+00002350: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00002360: 2020 6465 6620 6973 5f70 726f 7065 7274    def is_propert
+00002370: 795f 6f76 6572 7269 6461 626c 655f 6c69  y_overridable_li
+00002380: 6272 6172 7928 7365 6c66 2c20 7072 6f70  brary(self, prop
+00002390: 6572 7479 2920 2d3e 2062 6f6f 6c3a 0a20  erty) -> bool:. 
+000023a0: 2020 2020 2020 2027 2727 2043 6865 636b         ''' Check
+000023b0: 2069 6620 6120 7072 6f70 6572 7479 2069   if a property i
+000023c0: 7320 6f76 6572 7269 6461 626c 652e 0a0a  s overridable...
+000023d0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000023e0: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
+000023f0: 7475 726e 3a20 5472 7565 2077 6865 6e20  turn: True when 
+00002400: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
+00002410: 6f76 6572 7269 6461 626c 652e 0a20 2020  overridable..   
+00002420: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00002430: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
+00002440: 735f 7072 6f70 6572 7479 5f72 6561 646f  s_property_reado
+00002450: 6e6c 7928 7365 6c66 2c20 7072 6f70 6572  nly(self, proper
+00002460: 7479 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ty) -> bool:.   
+00002470: 2020 2020 2027 2727 2043 6865 636b 2069       ''' Check i
+00002480: 6620 6120 7072 6f70 6572 7479 2069 7320  f a property is 
+00002490: 7265 6164 6f6e 6c79 2e0a 0a20 2020 2020  readonly...     
+000024a0: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+000024b0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+000024c0: 2054 7275 6520 7768 656e 2074 6865 2070   True when the p
+000024d0: 726f 7065 7274 7920 6973 2072 6561 646f  roperty is reado
+000024e0: 6e6c 7920 286e 6f74 2077 7269 7461 626c  nly (not writabl
+000024f0: 6529 2e0a 2020 2020 2020 2020 2727 270a  e)..        '''.
+00002500: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00002510: 2020 6465 6620 6973 5f70 726f 7065 7274    def is_propert
+00002520: 795f 7365 7428 7365 6c66 2c20 7072 6f70  y_set(self, prop
+00002530: 6572 7479 2c0a 2020 2020 2020 2020 2020  erty,.          
+00002540: 2020 2020 2020 2020 2020 2020 2020 6768                gh
+00002550: 6f73 743a 2074 7970 696e 672e 4f70 7469  ost: typing.Opti
+00002560: 6f6e 616c 5b62 6f6f 6c5d 203d 2054 7275  onal[bool] = Tru
+00002570: 6529 202d 3e20 626f 6f6c 3a0a 2020 2020  e) -> bool:.    
+00002580: 2020 2020 2727 2720 4368 6563 6b20 6966      ''' Check if
+00002590: 2061 2070 726f 7065 7274 7920 6973 2073   a property is s
+000025a0: 6574 2c20 7573 6520 666f 7220 7465 7374  et, use for test
+000025b0: 696e 6720 6f70 6572 6174 6f72 2070 726f  ing operator pro
+000025c0: 7065 7274 6965 732e 0a0a 2020 2020 2020  perties...      
+000025d0: 2020 3a70 6172 616d 2067 686f 7374 3a20    :param ghost: 
+000025e0: 5573 6564 2066 6f72 206f 7065 7261 746f  Used for operato
+000025f0: 7273 2074 6861 7420 7265 2d72 756e 2077  rs that re-run w
+00002600: 6974 6820 7072 6576 696f 7573 2073 6574  ith previous set
+00002610: 7469 6e67 732e 2049 6e20 7468 6973 2063  tings. In this c
+00002620: 6173 6520 7468 6520 7072 6f70 6572 7479  ase the property
+00002630: 2069 7320 6e6f 7420 6d61 726b 6564 2061   is not marked a
+00002640: 7320 7365 742c 2079 6574 2074 6865 2076  s set, yet the v
+00002650: 616c 7565 2066 726f 6d20 7468 6520 7072  alue from the pr
+00002660: 6576 696f 7573 2065 7865 6375 7469 6f6e  evious execution
+00002670: 2069 7320 7573 6564 2e20 496e 2072 6172   is used. In rar
+00002680: 6520 6361 7365 7320 796f 7520 6d61 7920  e cases you may 
+00002690: 7761 6e74 2074 6f20 7365 7420 7468 6973  want to set this
+000026a0: 206f 7074 696f 6e20 746f 2066 616c 7365   option to false
+000026b0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+000026c0: 6768 6f73 743a 2074 7970 696e 672e 4f70  ghost: typing.Op
+000026d0: 7469 6f6e 616c 5b62 6f6f 6c5d 0a20 2020  tional[bool].   
+000026e0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+000026f0: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
+00002700: 6e3a 2054 7275 6520 7768 656e 2074 6865  n: True when the
+00002710: 2070 726f 7065 7274 7920 6861 7320 6265   property has be
+00002720: 656e 2073 6574 2e0a 2020 2020 2020 2020  en set..        
+00002730: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+00002740: 0a0a 2020 2020 6465 6620 6974 656d 7328  ..    def items(
+00002750: 7365 6c66 2920 2d3e 2074 7970 696e 672e  self) -> typing.
+00002760: 416e 793a 0a20 2020 2020 2020 2027 2727  Any:.        '''
+00002770: 2052 6574 7572 6e73 2074 6865 2069 7465   Returns the ite
+00002780: 6d73 206f 6620 7468 6973 206f 626a 6563  ms of this objec
+00002790: 7473 2063 7573 746f 6d20 7072 6f70 6572  ts custom proper
+000027a0: 7469 6573 2028 6d61 7463 6865 7320 5079  ties (matches Py
+000027b0: 7468 6f6e 2773 2064 6963 7469 6f6e 6172  thon's dictionar
+000027c0: 7920 6675 6e63 7469 6f6e 206f 6620 7468  y function of th
+000027d0: 6520 7361 6d65 206e 616d 6529 2e0a 0a20  e same name)... 
+000027e0: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
+000027f0: 7970 696e 672e 416e 790a 2020 2020 2020  yping.Any.      
+00002800: 2020 3a72 6574 7572 6e3a 2063 7573 746f    :return: custo
+00002810: 6d20 7072 6f70 6572 7479 206b 6579 2c20  m property key, 
+00002820: 7661 6c75 6520 7061 6972 732e 0a20 2020  value pairs..   
+00002830: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00002840: 2070 6173 730a 0a20 2020 2064 6566 206b   pass..    def k
+00002850: 6579 6672 616d 655f 6465 6c65 7465 280a  eyframe_delete(.
+00002860: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002870: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00002880: 7461 5f70 6174 683a 2074 7970 696e 672e  ta_path: typing.
+00002890: 4f70 7469 6f6e 616c 5b73 7472 5d2c 0a20  Optional[str],. 
+000028a0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+000028b0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000028c0: 6c5b 696e 745d 203d 202d 312c 0a20 2020  l[int] = -1,.   
+000028d0: 2020 2020 2020 2020 2066 7261 6d65 3a20           frame: 
+000028e0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000028f0: 666c 6f61 745d 203d 2027 6270 792e 636f  float] = 'bpy.co
+00002900: 6e74 6578 742e 7363 656e 652e 6672 616d  ntext.scene.fram
+00002910: 655f 6375 7272 656e 7427 2c0a 2020 2020  e_current',.    
+00002920: 2020 2020 2020 2020 6772 6f75 703a 2074          group: t
+00002930: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
+00002940: 7472 5d20 3d20 2222 2920 2d3e 2062 6f6f  tr] = "") -> boo
+00002950: 6c3a 0a20 2020 2020 2020 2027 2727 2052  l:.        ''' R
+00002960: 656d 6f76 6520 6120 6b65 7966 7261 6d65  emove a keyframe
+00002970: 2066 726f 6d20 7468 6973 2070 726f 7065   from this prope
+00002980: 7274 6965 7320 6663 7572 7665 2e0a 0a20  rties fcurve... 
+00002990: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
+000029a0: 7461 5f70 6174 683a 2070 6174 6820 746f  ta_path: path to
+000029b0: 2074 6865 2070 726f 7065 7274 7920 746f   the property to
+000029c0: 2072 656d 6f76 6520 6120 6b65 792c 2061   remove a key, a
+000029d0: 6e61 6c6f 676f 7573 2074 6f20 7468 6520  nalogous to the 
+000029e0: 6663 7572 7665 2773 2064 6174 6120 7061  fcurve's data pa
+000029f0: 7468 2e0a 2020 2020 2020 2020 3a74 7970  th..        :typ
+00002a00: 6520 6461 7461 5f70 6174 683a 2074 7970  e data_path: typ
+00002a10: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+00002a20: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+00002a30: 2069 6e64 6578 3a20 6172 7261 7920 696e   index: array in
+00002a40: 6465 7820 6f66 2074 6865 2070 726f 7065  dex of the prope
+00002a50: 7274 7920 746f 2072 656d 6f76 6520 6120  rty to remove a 
+00002a60: 6b65 792e 2044 6566 6175 6c74 7320 746f  key. Defaults to
+00002a70: 202d 3120 7265 6d6f 7669 6e67 2061 6c6c   -1 removing all
+00002a80: 2069 6e64 6963 6573 206f 7220 6120 7369   indices or a si
+00002a90: 6e67 6c65 2063 6861 6e6e 656c 2069 6620  ngle channel if 
+00002aa0: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
+00002ab0: 6e6f 7420 616e 2061 7272 6179 2e0a 2020  not an array..  
+00002ac0: 2020 2020 2020 3a74 7970 6520 696e 6465        :type inde
+00002ad0: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
+00002ae0: 616c 5b69 6e74 5d0a 2020 2020 2020 2020  al[int].        
+00002af0: 3a70 6172 616d 2066 7261 6d65 3a20 5468  :param frame: Th
+00002b00: 6520 6672 616d 6520 6f6e 2077 6869 6368  e frame on which
+00002b10: 2074 6865 206b 6579 6672 616d 6520 6973   the keyframe is
+00002b20: 2064 656c 6574 6564 2c20 6465 6661 756c   deleted, defaul
+00002b30: 7469 6e67 2074 6f20 7468 6520 6375 7272  ting to the curr
+00002b40: 656e 7420 6672 616d 652e 0a20 2020 2020  ent frame..     
+00002b50: 2020 203a 7479 7065 2066 7261 6d65 3a20     :type frame: 
+00002b60: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00002b70: 666c 6f61 745d 0a20 2020 2020 2020 203a  float].        :
+00002b80: 7061 7261 6d20 6772 6f75 703a 2054 6865  param group: The
+00002b90: 206e 616d 6520 6f66 2074 6865 2067 726f   name of the gro
+00002ba0: 7570 2074 6865 2046 2d43 7572 7665 2073  up the F-Curve s
+00002bb0: 686f 756c 6420 6265 2061 6464 6564 2074  hould be added t
+00002bc0: 6f20 6966 2069 7420 646f 6573 6e27 7420  o if it doesn't 
+00002bd0: 6578 6973 7420 7965 742e 0a20 2020 2020  exist yet..     
+00002be0: 2020 203a 7479 7065 2067 726f 7570 3a20     :type group: 
+00002bf0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00002c00: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
+00002c10: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+00002c20: 2020 3a72 6574 7572 6e3a 2053 7563 6365    :return: Succe
+00002c30: 7373 206f 6620 6b65 7966 7261 6d65 2064  ss of keyframe d
+00002c40: 656c 6574 696f 6e2e 0a20 2020 2020 2020  eletion..       
+00002c50: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00002c60: 730a 0a20 2020 2064 6566 206b 6579 6672  s..    def keyfr
+00002c70: 616d 655f 696e 7365 7274 280a 2020 2020  ame_insert(.    
+00002c80: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00002c90: 2020 2020 2020 2020 2020 6461 7461 5f70            data_p
+00002ca0: 6174 683a 2074 7970 696e 672e 4f70 7469  ath: typing.Opti
+00002cb0: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2020  onal[str],.     
+00002cc0: 2020 2020 2020 2069 6e64 6578 3a20 7479         index: ty
+00002cd0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
+00002ce0: 745d 203d 202d 312c 0a20 2020 2020 2020  t] = -1,.       
+00002cf0: 2020 2020 2066 7261 6d65 3a20 7479 7069       frame: typi
+00002d00: 6e67 2e4f 7074 696f 6e61 6c5b 666c 6f61  ng.Optional[floa
+00002d10: 745d 203d 2027 6270 792e 636f 6e74 6578  t] = 'bpy.contex
+00002d20: 742e 7363 656e 652e 6672 616d 655f 6375  t.scene.frame_cu
+00002d30: 7272 656e 7427 2c0a 2020 2020 2020 2020  rrent',.        
+00002d40: 2020 2020 6772 6f75 703a 2074 7970 696e      group: typin
+00002d50: 672e 4f70 7469 6f6e 616c 5b73 7472 5d20  g.Optional[str] 
+00002d60: 3d20 2222 2c0a 2020 2020 2020 2020 2020  = "",.          
+00002d70: 2020 6f70 7469 6f6e 733a 2074 7970 696e    options: typin
+00002d80: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00002d90: 672e 416e 795d 203d 2027 7365 7428 2927  g.Any] = 'set()'
+00002da0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00002db0: 2020 2027 2727 2049 6e73 6572 7420 6120     ''' Insert a 
+00002dc0: 6b65 7966 7261 6d65 206f 6e20 7468 6520  keyframe on the 
+00002dd0: 7072 6f70 6572 7479 2067 6976 656e 2c20  property given, 
+00002de0: 6164 6469 6e67 2066 6375 7276 6573 2061  adding fcurves a
+00002df0: 6e64 2061 6e69 6d61 7469 6f6e 2064 6174  nd animation dat
+00002e00: 6120 7768 656e 206e 6563 6573 7361 7279  a when necessary
+00002e10: 2e20 5468 6973 2069 7320 7468 6520 6d6f  . This is the mo
+00002e20: 7374 2073 696d 706c 6520 6578 616d 706c  st simple exampl
+00002e30: 6520 6f66 2069 6e73 6572 7469 6e67 2061  e of inserting a
+00002e40: 206b 6579 6672 616d 6520 6672 6f6d 2070   keyframe from p
+00002e50: 7974 686f 6e2e 204e 6f74 6520 7468 6174  ython. Note that
+00002e60: 2077 6865 6e20 6b65 7969 6e67 2064 6174   when keying dat
+00002e70: 6120 7061 7468 7320 7768 6963 6820 636f  a paths which co
+00002e80: 6e74 6169 6e20 6e65 7374 6564 2070 726f  ntain nested pro
+00002e90: 7065 7274 6965 7320 7468 6973 206d 7573  perties this mus
+00002ea0: 7420 6265 2064 6f6e 6520 6672 6f6d 2074  t be done from t
+00002eb0: 6865 2060 4944 6020 7375 6263 6c61 7373  he `ID` subclass
+00002ec0: 2c20 696e 2074 6869 7320 6361 7365 2074  , in this case t
+00002ed0: 6865 2060 4172 6d61 7475 7265 6020 7261  he `Armature` ra
+00002ee0: 7468 6572 2074 6861 6e20 7468 6520 626f  ther than the bo
+00002ef0: 6e65 2e0a 0a20 2020 2020 2020 203a 7061  ne...        :pa
+00002f00: 7261 6d20 6461 7461 5f70 6174 683a 2070  ram data_path: p
+00002f10: 6174 6820 746f 2074 6865 2070 726f 7065  ath to the prope
+00002f20: 7274 7920 746f 206b 6579 2c20 616e 616c  rty to key, anal
+00002f30: 6f67 6f75 7320 746f 2074 6865 2066 6375  ogous to the fcu
+00002f40: 7276 6527 7320 6461 7461 2070 6174 682e  rve's data path.
+00002f50: 0a20 2020 2020 2020 203a 7479 7065 2064  .        :type d
+00002f60: 6174 615f 7061 7468 3a20 7479 7069 6e67  ata_path: typing
+00002f70: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
+00002f80: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
+00002f90: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
+00002fa0: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
+00002fb0: 2074 6f20 6b65 792e 2044 6566 6175 6c74   to key. Default
+00002fc0: 7320 746f 202d 3120 7768 6963 6820 7769  s to -1 which wi
+00002fd0: 6c6c 206b 6579 2061 6c6c 2069 6e64 6963  ll key all indic
+00002fe0: 6573 206f 7220 6120 7369 6e67 6c65 2063  es or a single c
+00002ff0: 6861 6e6e 656c 2069 6620 7468 6520 7072  hannel if the pr
+00003000: 6f70 6572 7479 2069 7320 6e6f 7420 616e  operty is not an
+00003010: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
+00003020: 3a74 7970 6520 696e 6465 783a 2074 7970  :type index: typ
+00003030: 696e 672e 4f70 7469 6f6e 616c 5b69 6e74  ing.Optional[int
+00003040: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+00003050: 2066 7261 6d65 3a20 5468 6520 6672 616d   frame: The fram
+00003060: 6520 6f6e 2077 6869 6368 2074 6865 206b  e on which the k
+00003070: 6579 6672 616d 6520 6973 2069 6e73 6572  eyframe is inser
+00003080: 7465 642c 2064 6566 6175 6c74 696e 6720  ted, defaulting 
+00003090: 746f 2074 6865 2063 7572 7265 6e74 2066  to the current f
+000030a0: 7261 6d65 2e0a 2020 2020 2020 2020 3a74  rame..        :t
+000030b0: 7970 6520 6672 616d 653a 2074 7970 696e  ype frame: typin
+000030c0: 672e 4f70 7469 6f6e 616c 5b66 6c6f 6174  g.Optional[float
+000030d0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+000030e0: 2067 726f 7570 3a20 5468 6520 6e61 6d65   group: The name
+000030f0: 206f 6620 7468 6520 6772 6f75 7020 7468   of the group th
+00003100: 6520 462d 4375 7276 6520 7368 6f75 6c64  e F-Curve should
+00003110: 2062 6520 6164 6465 6420 746f 2069 6620   be added to if 
+00003120: 6974 2064 6f65 736e 2774 2065 7869 7374  it doesn't exist
+00003130: 2079 6574 2e0a 2020 2020 2020 2020 3a74   yet..        :t
+00003140: 7970 6520 6772 6f75 703a 2074 7970 696e  ype group: typin
+00003150: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+00003160: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
+00003170: 6c61 673a 200a 2020 2020 2020 2020 3a74  lag: .        :t
+00003180: 7970 6520 666c 6167 3a20 7479 7069 6e67  ype flag: typing
+00003190: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+000031a0: 2e53 6574 5d0a 2020 2020 2020 2020 3a70  .Set].        :p
+000031b0: 6172 616d 206f 7074 696f 6e73 3a20 202d  aram options:  -
+000031c0: 2060 6049 4e53 4552 544b 4559 5f4e 4545   ``INSERTKEY_NEE
+000031d0: 4445 4460 6020 4f6e 6c79 2069 6e73 6572  DED`` Only inser
+000031e0: 7420 6b65 7966 7261 6d65 7320 7768 6572  t keyframes wher
+000031f0: 6520 7468 6579 2772 6520 6e65 6564 6564  e they're needed
+00003200: 2069 6e20 7468 6520 7265 6c65 7661 6e74   in the relevant
+00003210: 2046 2d43 7572 7665 732e 202d 2060 6049   F-Curves. - ``I
+00003220: 4e53 4552 544b 4559 5f56 4953 5541 4c60  NSERTKEY_VISUAL`
+00003230: 6020 496e 7365 7274 206b 6579 6672 616d  ` Insert keyfram
+00003240: 6573 2062 6173 6564 206f 6e20 2776 6973  es based on 'vis
+00003250: 7561 6c20 7472 616e 7366 6f72 6d73 272e  ual transforms'.
+00003260: 202d 2060 6049 4e53 4552 544b 4559 5f58   - ``INSERTKEY_X
+00003270: 595a 5f54 4f5f 5247 4260 6020 436f 6c6f  YZ_TO_RGB`` Colo
+00003280: 7220 666f 7220 6e65 776c 7920 6164 6465  r for newly adde
+00003290: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
+000032a0: 2046 2d43 7572 7665 7320 284c 6f63 6174   F-Curves (Locat
+000032b0: 696f 6e2c 2052 6f74 6174 696f 6e2c 2053  ion, Rotation, S
+000032c0: 6361 6c65 2920 6973 2062 6173 6564 206f  cale) is based o
+000032d0: 6e20 7468 6520 7472 616e 7366 6f72 6d20  n the transform 
+000032e0: 6178 6973 2e20 2d20 6060 494e 5345 5254  axis. - ``INSERT
+000032f0: 4b45 595f 5245 504c 4143 4560 6020 4f6e  KEY_REPLACE`` On
+00003300: 6c79 2072 6570 6c61 6365 2061 6c72 6561  ly replace alrea
+00003310: 6479 2065 7869 7374 696e 6720 6b65 7966  dy existing keyf
+00003320: 7261 6d65 732e 202d 2060 6049 4e53 4552  rames. - ``INSER
+00003330: 544b 4559 5f41 5641 494c 4142 4c45 6060  TKEY_AVAILABLE``
+00003340: 204f 6e6c 7920 696e 7365 7274 2069 6e74   Only insert int
+00003350: 6f20 616c 7265 6164 7920 6578 6973 7469  o already existi
+00003360: 6e67 2046 2d43 7572 7665 732e 202d 2060  ng F-Curves. - `
+00003370: 6049 4e53 4552 544b 4559 5f43 5943 4c45  `INSERTKEY_CYCLE
+00003380: 5f41 5741 5245 6060 2054 616b 6520 6379  _AWARE`` Take cy
+00003390: 636c 6963 2065 7874 7261 706f 6c61 7469  clic extrapolati
+000033a0: 6f6e 2069 6e74 6f20 6163 636f 756e 7420  on into account 
+000033b0: 2843 7963 6c65 2d41 7761 7265 204b 6579  (Cycle-Aware Key
+000033c0: 696e 6720 6f70 7469 6f6e 292e 0a20 2020  ing option)..   
+000033d0: 2020 2020 203a 7479 7065 206f 7074 696f       :type optio
+000033e0: 6e73 3a20 7479 7069 6e67 2e4f 7074 696f  ns: typing.Optio
+000033f0: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d0a  nal[typing.Any].
+00003400: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00003410: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
+00003420: 7475 726e 3a20 5375 6363 6573 7320 6f66  turn: Success of
+00003430: 206b 6579 6672 616d 6520 696e 7365 7274   keyframe insert
+00003440: 696f 6e2e 0a20 2020 2020 2020 2027 2727  ion..        '''
+00003450: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00003460: 2020 2064 6566 206b 6579 7328 7365 6c66     def keys(self
+00003470: 2920 2d3e 2074 7970 696e 672e 416e 793a  ) -> typing.Any:
+00003480: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
+00003490: 7572 6e73 2074 6865 206b 6579 7320 6f66  urns the keys of
+000034a0: 2074 6869 7320 6f62 6a65 6374 7320 6375   this objects cu
+000034b0: 7374 6f6d 2070 726f 7065 7274 6965 7320  stom properties 
+000034c0: 286d 6174 6368 6573 2050 7974 686f 6e27  (matches Python'
+000034d0: 7320 6469 6374 696f 6e61 7279 2066 756e  s dictionary fun
+000034e0: 6374 696f 6e20 6f66 2074 6865 2073 616d  ction of the sam
+000034f0: 6520 6e61 6d65 292e 0a0a 2020 2020 2020  e name)...      
+00003500: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
+00003510: 2e41 6e79 0a20 2020 2020 2020 203a 7265  .Any.        :re
+00003520: 7475 726e 3a20 6375 7374 6f6d 2070 726f  turn: custom pro
+00003530: 7065 7274 7920 6b65 7973 2e0a 2020 2020  perty keys..    
+00003540: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00003550: 7061 7373 0a0a 2020 2020 6465 6620 7061  pass..    def pa
+00003560: 7468 5f66 726f 6d5f 6964 2873 656c 662c  th_from_id(self,
+00003570: 2070 726f 7065 7274 793a 2074 7970 696e   property: typin
+00003580: 672e 4f70 7469 6f6e 616c 5b73 7472 5d20  g.Optional[str] 
+00003590: 3d20 2222 2920 2d3e 2073 7472 3a0a 2020  = "") -> str:.  
+000035a0: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
+000035b0: 7320 7468 6520 6461 7461 2070 6174 6820  s the data path 
+000035c0: 6672 6f6d 2074 6865 2049 4420 746f 2074  from the ID to t
+000035d0: 6869 7320 6f62 6a65 6374 2028 7374 7269  his object (stri
+000035e0: 6e67 292e 0a0a 2020 2020 2020 2020 3a70  ng)...        :p
+000035f0: 6172 616d 2070 726f 7065 7274 793a 204f  aram property: O
+00003600: 7074 696f 6e61 6c20 7072 6f70 6572 7479  ptional property
+00003610: 206e 616d 6520 7768 6963 6820 6361 6e20   name which can 
+00003620: 6265 2075 7365 6420 6966 2074 6865 2070  be used if the p
+00003630: 6174 6820 6973 2074 6f20 6120 7072 6f70  ath is to a prop
+00003640: 6572 7479 206f 6620 7468 6973 206f 626a  erty of this obj
+00003650: 6563 742e 0a20 2020 2020 2020 203a 7479  ect..        :ty
+00003660: 7065 2070 726f 7065 7274 793a 2074 7970  pe property: typ
+00003670: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+00003680: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
+00003690: 3a20 7374 720a 2020 2020 2020 2020 3a72  : str.        :r
+000036a0: 6574 7572 6e3a 2060 6270 792e 7479 7065  eturn: `bpy.type
+000036b0: 732e 6270 795f 7374 7275 6374 2e69 645f  s.bpy_struct.id_
+000036c0: 6461 7461 6020 746f 2074 6869 7320 7374  data` to this st
+000036d0: 7275 6374 2061 6e64 2070 726f 7065 7274  ruct and propert
+000036e0: 7920 2877 6865 6e20 6769 7665 6e29 2e0a  y (when given)..
+000036f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00003700: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00003710: 6620 7061 7468 5f72 6573 6f6c 7665 2873  f path_resolve(s
+00003720: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00003730: 2020 2020 2020 2020 2020 7061 7468 3a20            path: 
+00003740: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00003750: 7374 725d 2c0a 2020 2020 2020 2020 2020  str],.          
+00003760: 2020 2020 2020 2020 2020 2063 6f65 7263             coerc
+00003770: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+00003780: 616c 5b62 6f6f 6c5d 203d 2054 7275 6529  al[bool] = True)
+00003790: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
+000037a0: 7475 726e 7320 7468 6520 7072 6f70 6572  turns the proper
+000037b0: 7479 2066 726f 6d20 7468 6520 7061 7468  ty from the path
+000037c0: 2c20 7261 6973 6520 616e 2065 7863 6570  , raise an excep
+000037d0: 7469 6f6e 2077 6865 6e20 6e6f 7420 666f  tion when not fo
+000037e0: 756e 642e 0a0a 2020 2020 2020 2020 3a70  und...        :p
+000037f0: 6172 616d 2070 6174 683a 2070 6174 6820  aram path: path 
+00003800: 7768 6963 6820 7468 6973 2070 726f 7065  which this prope
+00003810: 7274 7920 7265 736f 6c76 6573 2e0a 2020  rty resolves..  
+00003820: 2020 2020 2020 3a74 7970 6520 7061 7468        :type path
+00003830: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00003840: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
+00003850: 7061 7261 6d20 636f 6572 6365 3a20 6f70  param coerce: op
+00003860: 7469 6f6e 616c 2061 7267 756d 656e 742c  tional argument,
+00003870: 2077 6865 6e20 5472 7565 2c20 7468 6520   when True, the 
+00003880: 7072 6f70 6572 7479 2077 696c 6c20 6265  property will be
+00003890: 2063 6f6e 7665 7274 6564 2069 6e74 6f20   converted into 
+000038a0: 6974 7320 5079 7468 6f6e 2072 6570 7265  its Python repre
+000038b0: 7365 6e74 6174 696f 6e2e 0a20 2020 2020  sentation..     
+000038c0: 2020 203a 7479 7065 2063 6f65 7263 653a     :type coerce:
+000038d0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+000038e0: 5b62 6f6f 6c5d 0a20 2020 2020 2020 2027  [bool].        '
+000038f0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00003900: 0a20 2020 2064 6566 2070 6f70 2873 656c  .    def pop(sel
+00003910: 662c 0a20 2020 2020 2020 2020 2020 206b  f,.            k
+00003920: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
+00003930: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
+00003940: 2020 2020 2020 6465 6661 756c 743a 2074        default: t
+00003950: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00003960: 7970 696e 672e 416e 795d 203d 204e 6f6e  yping.Any] = Non
+00003970: 6529 3a0a 2020 2020 2020 2020 2727 2720  e):.        ''' 
+00003980: 5265 6d6f 7665 2061 6e64 2072 6574 7572  Remove and retur
+00003990: 6e20 7468 6520 7661 6c75 6520 6f66 2074  n the value of t
+000039a0: 6865 2063 7573 746f 6d20 7072 6f70 6572  he custom proper
+000039b0: 7479 2061 7373 6967 6e65 6420 746f 206b  ty assigned to k
+000039c0: 6579 206f 7220 6465 6661 756c 7420 7768  ey or default wh
+000039d0: 656e 206e 6f74 2066 6f75 6e64 2028 6d61  en not found (ma
+000039e0: 7463 6865 7320 5079 7468 6f6e 2773 2064  tches Python's d
+000039f0: 6963 7469 6f6e 6172 7920 6675 6e63 7469  ictionary functi
+00003a00: 6f6e 206f 6620 7468 6520 7361 6d65 206e  on of the same n
+00003a10: 616d 6529 2e0a 0a20 2020 2020 2020 203a  ame)...        :
+00003a20: 7061 7261 6d20 6b65 793a 2054 6865 206b  param key: The k
+00003a30: 6579 2061 7373 6f63 6961 7465 6420 7769  ey associated wi
+00003a40: 7468 2074 6865 2063 7573 746f 6d20 7072  th the custom pr
+00003a50: 6f70 6572 7479 2e0a 2020 2020 2020 2020  operty..        
+00003a60: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
+00003a70: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+00003a80: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00003a90: 6566 6175 6c74 3a20 4f70 7469 6f6e 616c  efault: Optional
+00003aa0: 2061 7267 756d 656e 7420 666f 7220 7468   argument for th
+00003ab0: 6520 7661 6c75 6520 746f 2072 6574 7572  e value to retur
+00003ac0: 6e20 6966 202a 6b65 792a 2069 7320 6e6f  n if *key* is no
+00003ad0: 7420 666f 756e 642e 0a20 2020 2020 2020  t found..       
+00003ae0: 203a 7479 7065 2064 6566 6175 6c74 3a20   :type default: 
+00003af0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00003b00: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
+00003b10: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00003b20: 7061 7373 0a0a 2020 2020 6465 6620 7072  pass..    def pr
+00003b30: 6f70 6572 7479 5f6f 7665 7272 6964 6162  operty_overridab
+00003b40: 6c65 5f6c 6962 7261 7279 5f73 6574 2873  le_library_set(s
+00003b50: 656c 662c 2070 726f 7065 7274 792c 206f  elf, property, o
+00003b60: 7665 7272 6964 6162 6c65 2920 2d3e 2062  verridable) -> b
+00003b70: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
+00003b80: 2044 6566 696e 6520 6120 7072 6f70 6572   Define a proper
+00003b90: 7479 2061 7320 6f76 6572 7269 6461 626c  ty as overridabl
+00003ba0: 6520 6f72 206e 6f74 2028 6f6e 6c79 2066  e or not (only f
+00003bb0: 6f72 2063 7573 746f 6d20 7072 6f70 6572  or custom proper
+00003bc0: 7469 6573 2129 2e0a 0a20 2020 2020 2020  ties!)...       
+00003bd0: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+00003be0: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
+00003bf0: 7275 6520 7768 656e 2074 6865 206f 7665  rue when the ove
+00003c00: 7272 6964 6162 6c65 2073 7461 7475 7320  rridable status 
+00003c10: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
+00003c20: 7761 7320 7375 6363 6573 7366 756c 6c79  was successfully
+00003c30: 2073 6574 2e0a 2020 2020 2020 2020 2727   set..        ''
+00003c40: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00003c50: 2020 2020 6465 6620 7072 6f70 6572 7479      def property
+00003c60: 5f75 6e73 6574 2873 656c 662c 2070 726f  _unset(self, pro
+00003c70: 7065 7274 7929 3a0a 2020 2020 2020 2020  perty):.        
+00003c80: 2727 2720 556e 7365 7420 6120 7072 6f70  ''' Unset a prop
+00003c90: 6572 7479 2c20 7769 6c6c 2075 7365 2064  erty, will use d
+00003ca0: 6566 6175 6c74 2076 616c 7565 2061 6674  efault value aft
+00003cb0: 6572 7761 7264 2e0a 0a20 2020 2020 2020  erward...       
+00003cc0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00003cd0: 730a 0a20 2020 2064 6566 2074 7970 655f  s..    def type_
+00003ce0: 7265 6361 7374 2873 656c 6629 202d 3e20  recast(self) -> 
+00003cf0: 2762 7079 5f73 7472 7563 7427 3a0a 2020  'bpy_struct':.  
+00003d00: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
+00003d10: 2061 206e 6577 2069 6e73 7461 6e63 652c   a new instance,
+00003d20: 2074 6869 7320 6973 206e 6565 6465 6420   this is needed 
+00003d30: 6265 6361 7573 6520 7479 7065 7320 7375  because types su
+00003d40: 6368 2061 7320 7465 7874 7572 6573 2063  ch as textures c
+00003d50: 616e 2062 6520 6368 616e 6765 6420 6174  an be changed at
+00003d60: 2072 756e 7469 6d65 2e0a 0a20 2020 2020   runtime...     
+00003d70: 2020 203a 7274 7970 653a 2027 6270 795f     :rtype: 'bpy_
+00003d80: 7374 7275 6374 270a 2020 2020 2020 2020  struct'.        
+00003d90: 3a72 6574 7572 6e3a 2061 206e 6577 2069  :return: a new i
+00003da0: 6e73 7461 6e63 6520 6f66 2074 6869 7320  nstance of this 
+00003db0: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
+00003dc0: 7479 7065 2069 6e69 7469 616c 697a 6564  type initialized
+00003dd0: 2061 6761 696e 2e0a 2020 2020 2020 2020   again..        
+00003de0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+00003df0: 0a0a 2020 2020 6465 6620 7661 6c75 6573  ..    def values
+00003e00: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
+00003e10: 2e41 6e79 3a0a 2020 2020 2020 2020 2727  .Any:.        ''
+00003e20: 2720 5265 7475 726e 7320 7468 6520 7661  ' Returns the va
+00003e30: 6c75 6573 206f 6620 7468 6973 206f 626a  lues of this obj
+00003e40: 6563 7473 2063 7573 746f 6d20 7072 6f70  ects custom prop
+00003e50: 6572 7469 6573 2028 6d61 7463 6865 7320  erties (matches 
+00003e60: 5079 7468 6f6e 2773 2064 6963 7469 6f6e  Python's diction
+00003e70: 6172 7920 6675 6e63 7469 6f6e 206f 6620  ary function of 
+00003e80: 7468 6520 7361 6d65 206e 616d 6529 2e0a  the same name)..
+00003e90: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00003ea0: 2074 7970 696e 672e 416e 790a 2020 2020   typing.Any.    
+00003eb0: 2020 2020 3a72 6574 7572 6e3a 2063 7573      :return: cus
+00003ec0: 746f 6d20 7072 6f70 6572 7479 2076 616c  tom property val
+00003ed0: 7565 732e 0a20 2020 2020 2020 2027 2727  ues..        '''
+00003ee0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00003ef0: 2020 2064 6566 205f 5f67 6574 6974 656d     def __getitem
+00003f00: 5f5f 2873 656c 662c 206b 6579 3a20 7479  __(self, key: ty
+00003f10: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+00003f20: 7374 725d 2920 2d3e 2027 7479 7069 6e67  str]) -> 'typing
+00003f30: 2e41 6e79 273a 0a20 2020 2020 2020 2027  .Any':.        '
+00003f40: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
+00003f50: 7261 6d20 6b65 793a 200a 2020 2020 2020  ram key: .      
+00003f60: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
+00003f70: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
+00003f80: 7472 5d0a 2020 2020 2020 2020 3a72 7479  tr].        :rty
+00003f90: 7065 3a20 2774 7970 696e 672e 416e 7927  pe: 'typing.Any'
+00003fa0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00003fb0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00003fc0: 6566 205f 5f73 6574 6974 656d 5f5f 2873  ef __setitem__(s
+00003fd0: 656c 662c 206b 6579 3a20 7479 7069 6e67  elf, key: typing
+00003fe0: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
+00003ff0: 2c20 7661 6c75 653a 2027 7479 7069 6e67  , value: 'typing
+00004000: 2e41 6e79 2729 3a0a 2020 2020 2020 2020  .Any'):.        
+00004010: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
+00004020: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
+00004030: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
+00004040: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+00004050: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
+00004060: 7261 6d20 7661 6c75 653a 200a 2020 2020  ram value: .    
+00004070: 2020 2020 3a74 7970 6520 7661 6c75 653a      :type value:
+00004080: 2027 7479 7069 6e67 2e41 6e79 270a 2020   'typing.Any'.  
+00004090: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+000040a0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+000040b0: 5f5f 6465 6c69 7465 6d5f 5f28 7365 6c66  __delitem__(self
+000040c0: 2c20 6b65 793a 2074 7970 696e 672e 556e  , key: typing.Un
+000040d0: 696f 6e5b 696e 742c 2073 7472 5d29 202d  ion[int, str]) -
+000040e0: 3e20 2774 7970 696e 672e 416e 7927 3a0a  > 'typing.Any':.
+000040f0: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
+00004100: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
+00004110: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
+00004120: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
+00004130: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
+00004140: 2020 2020 203a 7274 7970 653a 2027 7479       :rtype: 'ty
+00004150: 7069 6e67 2e41 6e79 270a 2020 2020 2020  ping.Any'.      
 00004160: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
 00004170: 7373 0a0a 0a63 6c61 7373 2062 7079 5f70  ss...class bpy_p
 00004180: 726f 705f 6172 7261 7928 7479 7069 6e67  rop_array(typing
 00004190: 2e47 656e 6572 6963 5b47 656e 6572 6963  .Generic[Generic
 000041a0: 5479 7065 5d29 3a0a 2020 2020 6465 6620  Type]):.    def 
 000041b0: 666f 7265 6163 685f 6765 7428 7365 6c66  foreach_get(self
 000041c0: 2c20 6174 7472 2c20 7365 7129 3a0a 2020  , attr, seq):.  
@@ -23175,16 +23175,16 @@
 0005a860: 3a20 2745 7665 6e74 272c 0a20 2020 2020  : 'Event',.     
 0005a870: 2020 2020 2020 2020 2074 7765 616b 3a20           tweak: 
 0005a880: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
 0005a890: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
 0005a8a0: 7069 6e67 2e53 6574 5b69 6e74 5d5d 0a20  ping.Set[int]]. 
 0005a8b0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
 0005a8c0: 3e20 7479 7069 6e67 2e55 6e69 6f6e 5b74  > typing.Union[t
-0005a8d0: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
-0005a8e0: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
+0005a8d0: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
+0005a8e0: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
 0005a8f0: 3a0a 2020 2020 2020 2020 2727 2720 0a0a  :.        ''' ..
 0005a900: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
 0005a910: 6f6e 7465 7874 3a20 0a20 2020 2020 2020  ontext: .       
 0005a920: 203a 7479 7065 2063 6f6e 7465 7874 3a20   :type context: 
 0005a930: 2743 6f6e 7465 7874 270a 2020 2020 2020  'Context'.      
 0005a940: 2020 3a70 6172 616d 2065 7665 6e74 3a20    :param event: 
 0005a950: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
@@ -23193,42 +23193,42 @@
 0005a980: 616b 3a20 5477 6561 6b0a 2020 2020 2020  ak: Tweak.      
 0005a990: 2020 3a74 7970 6520 7477 6561 6b3a 2074    :type tweak: t
 0005a9a0: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
 0005a9b0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
 0005a9c0: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
 0005a9d0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
 0005a9e0: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-0005a9f0: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
-0005aa00: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
+0005a9f0: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
+0005aa00: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
 0005aa10: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
 0005aa20: 7375 6c74 0a20 2020 2020 2020 2027 2727  sult.        '''
 0005aa30: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
 0005aa40: 2020 2064 6566 2073 6574 7570 2873 656c     def setup(sel
 0005aa50: 6629 3a0a 2020 2020 2020 2020 2727 2720  f):.        ''' 
 0005aa60: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
 0005aa70: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
 0005aa80: 6465 6620 696e 766f 6b65 2873 656c 662c  def invoke(self,
 0005aa90: 2063 6f6e 7465 7874 3a20 2743 6f6e 7465   context: 'Conte
 0005aaa0: 7874 272c 2065 7665 6e74 3a20 2745 7665  xt', event: 'Eve
 0005aab0: 6e74 270a 2020 2020 2020 2020 2020 2020  nt'.            
 0005aac0: 2020 2029 202d 3e20 7479 7069 6e67 2e55     ) -> typing.U
 0005aad0: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-0005aae0: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
-0005aaf0: 5b69 6e74 5d5d 3a0a 2020 2020 2020 2020  [int]]:.        
+0005aae0: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
+0005aaf0: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
 0005ab00: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
 0005ab10: 6172 616d 2063 6f6e 7465 7874 3a20 0a20  aram context: . 
 0005ab20: 2020 2020 2020 203a 7479 7065 2063 6f6e         :type con
 0005ab30: 7465 7874 3a20 2743 6f6e 7465 7874 270a  text: 'Context'.
 0005ab40: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
 0005ab50: 7665 6e74 3a20 0a20 2020 2020 2020 203a  vent: .        :
 0005ab60: 7479 7065 2065 7665 6e74 3a20 2745 7665  type event: 'Eve
 0005ab70: 6e74 270a 2020 2020 2020 2020 3a72 7479  nt'.        :rty
 0005ab80: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-0005ab90: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
-0005aba0: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
+0005ab90: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
+0005aba0: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
 0005abb0: 5d5d 0a20 2020 2020 2020 203a 7265 7475  ]].        :retu
 0005abc0: 726e 3a20 7265 7375 6c74 0a20 2020 2020  rn: result.     
 0005abd0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 0005abe0: 6173 730a 0a20 2020 2064 6566 2065 7869  ass..    def exi
 0005abf0: 7428 7365 6c66 2c20 636f 6e74 6578 743a  t(self, context:
 0005ac00: 2027 436f 6e74 6578 7427 2c20 6361 6e63   'Context', canc
 0005ac10: 656c 3a20 7479 7069 6e67 2e4f 7074 696f  el: typing.Optio
@@ -27351,24 +27351,24 @@
 0006ad60: 6e5b 7374 722c 2074 7970 696e 672e 416e  n[str, typing.An
 0006ad70: 795d 203d 204e 6f6e 650a 2020 2020 2727  y] = None.    ''
 0006ad80: 2720 0a0a 2020 2020 3a74 7970 653a 2074  ' ..    :type: t
 0006ad90: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
 0006ada0: 2074 7970 696e 672e 416e 795d 0a20 2020   typing.Any].   
 0006adb0: 2027 2727 0a0a 2020 2020 626c 5f6f 7074   '''..    bl_opt
 0006adc0: 696f 6e73 3a20 7479 7069 6e67 2e55 6e69  ions: typing.Uni
-0006add0: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
-0006ade0: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
-0006adf0: 6e74 5d5d 203d 204e 6f6e 650a 2020 2020  nt]] = None.    
+0006add0: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
+0006ade0: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
+0006adf0: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
 0006ae00: 2727 2720 4b65 7969 6e67 2053 6574 206f  ''' Keying Set o
 0006ae10: 7074 696f 6e73 2074 6f20 7573 6520 7768  ptions to use wh
 0006ae20: 656e 2069 6e73 6572 7469 6e67 206b 6579  en inserting key
 0006ae30: 6672 616d 6573 0a0a 2020 2020 3a74 7970  frames..    :typ
 0006ae40: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-0006ae50: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
-0006ae60: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
+0006ae50: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
+0006ae60: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
 0006ae70: 5d0a 2020 2020 2727 270a 0a20 2020 2064  ].    '''..    d
 0006ae80: 6566 2070 6f6c 6c28 7365 6c66 2c20 636f  ef poll(self, co
 0006ae90: 6e74 6578 743a 2074 7970 696e 672e 4f70  ntext: typing.Op
 0006aea0: 7469 6f6e 616c 5b27 436f 6e74 6578 7427  tional['Context'
 0006aeb0: 5d29 3a0a 2020 2020 2020 2020 2727 2720  ]):.        ''' 
 0006aec0: 5465 7374 2069 6620 4b65 7969 6e67 2053  Test if Keying S
 0006aed0: 6574 2063 616e 2062 6520 7573 6564 206f  et can be used o
@@ -28112,23 +28112,23 @@
 0006dcf0: 7479 7069 6e67 2e41 6e79 5d20 3d20 4e6f  typing.Any] = No
 0006dd00: 6e65 0a20 2020 2027 2727 200a 0a20 2020  ne.    ''' ..   
 0006dd10: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
 0006dd20: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 0006dd30: 2e41 6e79 5d0a 2020 2020 2727 270a 0a20  .Any].    '''.. 
 0006dd40: 2020 2062 6c5f 6f70 7469 6f6e 733a 2074     bl_options: t
 0006dd50: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-0006dd60: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
-0006dd70: 696e 672e 5365 745b 696e 745d 5d20 3d20  ing.Set[int]] = 
+0006dd60: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
+0006dd70: 696e 672e 5365 745b 7374 725d 5d20 3d20  ing.Set[str]] = 
 0006dd80: 4e6f 6e65 0a20 2020 2027 2727 204f 7074  None.    ''' Opt
 0006dd90: 696f 6e73 2066 6f72 2074 6869 7320 6f70  ions for this op
 0006dda0: 6572 6174 6f72 2074 7970 650a 0a20 2020  erator type..   
 0006ddb0: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
 0006ddc0: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-0006ddd0: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
-0006dde0: 5b69 6e74 5d5d 0a20 2020 2027 2727 0a0a  [int]].    '''..
+0006ddd0: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
+0006dde0: 5b73 7472 5d5d 0a20 2020 2027 2727 0a0a  [str]].    '''..
 0006ddf0: 2020 2020 626c 5f74 7261 6e73 6c61 7469      bl_translati
 0006de00: 6f6e 5f63 6f6e 7465 7874 3a20 7479 7069  on_context: typi
 0006de10: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 7479  ng.Union[str, ty
 0006de20: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
 0006de30: 0a20 2020 2027 2727 200a 0a20 2020 203a  .    ''' ..    :
 0006de40: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
 0006de50: 6f6e 5b73 7472 2c20 7479 7069 6e67 2e41  on[str, typing.A
@@ -28163,27 +28163,27 @@
 0006e020: 5072 6f70 6572 7469 6573 2720 3d20 4e6f  Properties' = No
 0006e030: 6e65 0a20 2020 2027 2727 200a 0a20 2020  ne.    ''' ..   
 0006e040: 203a 7479 7065 3a20 274f 7065 7261 746f   :type: 'Operato
 0006e050: 7250 726f 7065 7274 6965 7327 0a20 2020  rProperties'.   
 0006e060: 2027 2727 0a0a 2020 2020 6465 6620 7265   '''..    def re
 0006e070: 706f 7274 2873 656c 662c 2074 7970 653a  port(self, type:
 0006e080: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-0006e090: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
-0006e0a0: 7970 696e 672e 5365 745b 696e 745d 5d2c  yping.Set[int]],
+0006e090: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
+0006e0a0: 7970 696e 672e 5365 745b 7374 725d 5d2c  yping.Set[str]],
 0006e0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0006e0c0: 6d65 7373 6167 653a 2074 7970 696e 672e  message: typing.
 0006e0d0: 556e 696f 6e5b 7374 722c 2074 7970 696e  Union[str, typin
 0006e0e0: 672e 416e 795d 293a 0a20 2020 2020 2020  g.Any]):.       
 0006e0f0: 2027 2727 2072 6570 6f72 740a 0a20 2020   ''' report..   
 0006e100: 2020 2020 203a 7061 7261 6d20 7479 7065       :param type
 0006e110: 3a20 5479 7065 0a20 2020 2020 2020 203a  : Type.        :
 0006e120: 7479 7065 2074 7970 653a 2074 7970 696e  type type: typin
 0006e130: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-0006e140: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
-0006e150: 5365 745b 696e 745d 5d0a 2020 2020 2020  Set[int]].      
+0006e140: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
+0006e150: 5365 745b 7374 725d 5d0a 2020 2020 2020  Set[str]].      
 0006e160: 2020 3a70 6172 616d 206d 6573 7361 6765    :param message
 0006e170: 3a20 5265 706f 7274 204d 6573 7361 6765  : Report Message
 0006e180: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
 0006e190: 6573 7361 6765 3a20 7479 7069 6e67 2e55  essage: typing.U
 0006e1a0: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 0006e1b0: 2e41 6e79 5d0a 2020 2020 2020 2020 2727  .Any].        ''
 0006e1c0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
@@ -36344,23 +36344,23 @@
 0008df70: 5b73 7472 2c20 7479 7069 6e67 2e41 6e79  [str, typing.Any
 0008df80: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 0008df90: 200a 0a20 2020 203a 7479 7065 3a20 7479   ..    :type: ty
 0008dfa0: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 0008dfb0: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
 0008dfc0: 2727 270a 0a20 2020 2062 6c5f 6f70 7469  '''..    bl_opti
 0008dfd0: 6f6e 733a 2074 7970 696e 672e 556e 696f  ons: typing.Unio
-0008dfe0: 6e5b 7479 7069 6e67 2e53 6574 5b73 7472  n[typing.Set[str
-0008dff0: 5d2c 2074 7970 696e 672e 5365 745b 696e  ], typing.Set[in
-0008e000: 745d 5d20 3d20 4e6f 6e65 0a20 2020 2027  t]] = None.    '
+0008dfe0: 6e5b 7479 7069 6e67 2e53 6574 5b69 6e74  n[typing.Set[int
+0008dff0: 5d2c 2074 7970 696e 672e 5365 745b 7374  ], typing.Set[st
+0008e000: 725d 5d20 3d20 4e6f 6e65 0a20 2020 2027  r]] = None.    '
 0008e010: 2727 204f 7074 696f 6e73 2066 6f72 2074  '' Options for t
 0008e020: 6869 7320 6f70 6572 6174 6f72 2074 7970  his operator typ
 0008e030: 650a 0a20 2020 203a 7479 7065 3a20 7479  e..    :type: ty
 0008e040: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-0008e050: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
-0008e060: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
+0008e050: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
+0008e060: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
 0008e070: 2027 2727 0a0a 2020 2020 626c 5f74 7261   '''..    bl_tra
 0008e080: 6e73 6c61 7469 6f6e 5f63 6f6e 7465 7874  nslation_context
 0008e090: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b73  : typing.Union[s
 0008e0a0: 7472 2c20 7479 7069 6e67 2e41 6e79 5d20  tr, typing.Any] 
 0008e0b0: 3d20 4e6f 6e65 0a20 2020 2027 2727 200a  = None.    ''' .
 0008e0c0: 0a20 2020 203a 7479 7065 3a20 7479 7069  .    :type: typi
 0008e0d0: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 7479  ng.Union[str, ty
@@ -36427,27 +36427,27 @@
 0008e4a0: 7274 7920 7768 656e 2065 7870 616e 6469  rty when expandi
 0008e4b0: 6e67 2061 6e20 6f70 6572 6174 6f72 2069  ng an operator i
 0008e4c0: 6e74 6f20 6120 6d65 6e75 2e0a 0a20 2020  nto a menu...   
 0008e4d0: 203a 7479 7065 3a20 7374 720a 2020 2020   :type: str.    
 0008e4e0: 2727 270a 0a20 2020 2064 6566 2072 6570  '''..    def rep
 0008e4f0: 6f72 7428 7365 6c66 2c20 7479 7065 3a20  ort(self, type: 
 0008e500: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-0008e510: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
-0008e520: 7069 6e67 2e53 6574 5b69 6e74 5d5d 2c0a  ping.Set[int]],.
+0008e510: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
+0008e520: 7069 6e67 2e53 6574 5b73 7472 5d5d 2c0a  ping.Set[str]],.
 0008e530: 2020 2020 2020 2020 2020 2020 2020 206d                 m
 0008e540: 6573 7361 6765 3a20 7479 7069 6e67 2e55  essage: typing.U
 0008e550: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 0008e560: 2e41 6e79 5d29 3a0a 2020 2020 2020 2020  .Any]):.        
 0008e570: 2727 2720 7265 706f 7274 0a0a 2020 2020  ''' report..    
 0008e580: 2020 2020 3a70 6172 616d 2074 7970 653a      :param type:
 0008e590: 2054 7970 650a 2020 2020 2020 2020 3a74   Type.        :t
 0008e5a0: 7970 6520 7479 7065 3a20 7479 7069 6e67  ype type: typing
 0008e5b0: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-0008e5c0: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
-0008e5d0: 6574 5b69 6e74 5d5d 0a20 2020 2020 2020  et[int]].       
+0008e5c0: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
+0008e5d0: 6574 5b73 7472 5d5d 0a20 2020 2020 2020  et[str]].       
 0008e5e0: 203a 7061 7261 6d20 6d65 7373 6167 653a   :param message:
 0008e5f0: 2052 6570 6f72 7420 4d65 7373 6167 650a   Report Message.
 0008e600: 2020 2020 2020 2020 3a74 7970 6520 6d65          :type me
 0008e610: 7373 6167 653a 2074 7970 696e 672e 556e  ssage: typing.Un
 0008e620: 696f 6e5b 7374 722c 2074 7970 696e 672e  ion[str, typing.
 0008e630: 416e 795d 0a20 2020 2020 2020 2027 2727  Any].        '''
 0008e640: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
@@ -36472,26 +36472,26 @@
 0008e770: 6e74 6578 7427 0a20 2020 2020 2020 2027  ntext'.        '
 0008e780: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
 0008e790: 0a20 2020 2064 6566 2065 7865 6375 7465  .    def execute
 0008e7a0: 2873 656c 662c 2063 6f6e 7465 7874 3a20  (self, context: 
 0008e7b0: 2743 6f6e 7465 7874 270a 2020 2020 2020  'Context'.      
 0008e7c0: 2020 2020 2020 2020 2020 2920 2d3e 2074            ) -> t
 0008e7d0: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-0008e7e0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
-0008e7f0: 696e 672e 5365 745b 696e 745d 5d3a 0a20  ing.Set[int]]:. 
+0008e7e0: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
+0008e7f0: 696e 672e 5365 745b 7374 725d 5d3a 0a20  ing.Set[str]]:. 
 0008e800: 2020 2020 2020 2027 2727 2045 7865 6375         ''' Execu
 0008e810: 7465 2074 6865 206f 7065 7261 746f 720a  te the operator.
 0008e820: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
 0008e830: 636f 6e74 6578 743a 200a 2020 2020 2020  context: .      
 0008e840: 2020 3a74 7970 6520 636f 6e74 6578 743a    :type context:
 0008e850: 2027 436f 6e74 6578 7427 0a20 2020 2020   'Context'.     
 0008e860: 2020 203a 7274 7970 653a 2074 7970 696e     :rtype: typin
 0008e870: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-0008e880: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
-0008e890: 5365 745b 696e 745d 5d0a 2020 2020 2020  Set[int]].      
+0008e880: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
+0008e890: 5365 745b 7374 725d 5d0a 2020 2020 2020  Set[str]].      
 0008e8a0: 2020 3a72 6574 7572 6e3a 2072 6573 756c    :return: resul
 0008e8b0: 740a 2020 2020 2020 2020 2727 270a 2020  t.        '''.  
 0008e8c0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
 0008e8d0: 6465 6620 6368 6563 6b28 7365 6c66 2c20  def check(self, 
 0008e8e0: 636f 6e74 6578 743a 2027 436f 6e74 6578  context: 'Contex
 0008e8f0: 7427 2920 2d3e 2062 6f6f 6c3a 0a20 2020  t') -> bool:.   
 0008e900: 2020 2020 2027 2727 2043 6865 636b 2074       ''' Check t
@@ -36509,53 +36509,53 @@
 0008e9c0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
 0008e9d0: 0a20 2020 2064 6566 2069 6e76 6f6b 6528  .    def invoke(
 0008e9e0: 7365 6c66 2c20 636f 6e74 6578 743a 2027  self, context: '
 0008e9f0: 436f 6e74 6578 7427 2c20 6576 656e 743a  Context', event:
 0008ea00: 2027 4576 656e 7427 0a20 2020 2020 2020   'Event'.       
 0008ea10: 2020 2020 2020 2020 2920 2d3e 2074 7970          ) -> typ
 0008ea20: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-0008ea30: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
-0008ea40: 672e 5365 745b 696e 745d 5d3a 0a20 2020  g.Set[int]]:.   
+0008ea30: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
+0008ea40: 672e 5365 745b 7374 725d 5d3a 0a20 2020  g.Set[str]]:.   
 0008ea50: 2020 2020 2027 2727 2049 6e76 6f6b 6520       ''' Invoke 
 0008ea60: 7468 6520 6f70 6572 6174 6f72 0a0a 2020  the operator..  
 0008ea70: 2020 2020 2020 3a70 6172 616d 2063 6f6e        :param con
 0008ea80: 7465 7874 3a20 0a20 2020 2020 2020 203a  text: .        :
 0008ea90: 7479 7065 2063 6f6e 7465 7874 3a20 2743  type context: 'C
 0008eaa0: 6f6e 7465 7874 270a 2020 2020 2020 2020  ontext'.        
 0008eab0: 3a70 6172 616d 2065 7665 6e74 3a20 0a20  :param event: . 
 0008eac0: 2020 2020 2020 203a 7479 7065 2065 7665         :type eve
 0008ead0: 6e74 3a20 2745 7665 6e74 270a 2020 2020  nt: 'Event'.    
 0008eae0: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
 0008eaf0: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-0008eb00: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
-0008eb10: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2020  .Set[int]].     
+0008eb00: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
+0008eb10: 2e53 6574 5b73 7472 5d5d 0a20 2020 2020  .Set[str]].     
 0008eb20: 2020 203a 7265 7475 726e 3a20 7265 7375     :return: resu
 0008eb30: 6c74 0a20 2020 2020 2020 2027 2727 0a20  lt.        '''. 
 0008eb40: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
 0008eb50: 2064 6566 206d 6f64 616c 2873 656c 662c   def modal(self,
 0008eb60: 2063 6f6e 7465 7874 3a20 2743 6f6e 7465   context: 'Conte
 0008eb70: 7874 272c 2065 7665 6e74 3a20 2745 7665  xt', event: 'Eve
 0008eb80: 6e74 270a 2020 2020 2020 2020 2020 2020  nt'.            
 0008eb90: 2020 2920 2d3e 2074 7970 696e 672e 556e    ) -> typing.Un
-0008eba0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
-0008ebb0: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
-0008ebc0: 696e 745d 5d3a 0a20 2020 2020 2020 2027  int]]:.        '
+0008eba0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
+0008ebb0: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
+0008ebc0: 7374 725d 5d3a 0a20 2020 2020 2020 2027  str]]:.        '
 0008ebd0: 2727 204d 6f64 616c 206f 7065 7261 746f  '' Modal operato
 0008ebe0: 7220 6675 6e63 7469 6f6e 0a0a 2020 2020  r function..    
 0008ebf0: 2020 2020 3a70 6172 616d 2063 6f6e 7465      :param conte
 0008ec00: 7874 3a20 0a20 2020 2020 2020 203a 7479  xt: .        :ty
 0008ec10: 7065 2063 6f6e 7465 7874 3a20 2743 6f6e  pe context: 'Con
 0008ec20: 7465 7874 270a 2020 2020 2020 2020 3a70  text'.        :p
 0008ec30: 6172 616d 2065 7665 6e74 3a20 0a20 2020  aram event: .   
 0008ec40: 2020 2020 203a 7479 7065 2065 7665 6e74       :type event
 0008ec50: 3a20 2745 7665 6e74 270a 2020 2020 2020  : 'Event'.      
 0008ec60: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
 0008ec70: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-0008ec80: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
-0008ec90: 6574 5b69 6e74 5d5d 0a20 2020 2020 2020  et[int]].       
+0008ec80: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
+0008ec90: 6574 5b73 7472 5d5d 0a20 2020 2020 2020  et[str]].       
 0008eca0: 203a 7265 7475 726e 3a20 7265 7375 6c74   :return: result
 0008ecb0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 0008ecc0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
 0008ecd0: 6566 2064 7261 7728 7365 6c66 2c20 636f  ef draw(self, co
 0008ece0: 6e74 6578 743a 2027 436f 6e74 6578 7427  ntext: 'Context'
 0008ecf0: 293a 0a20 2020 2020 2020 2027 2727 2044  ):.        ''' D
 0008ed00: 7261 7720 6675 6e63 7469 6f6e 2066 6f72  raw function for
@@ -46253,28 +46253,28 @@
 000b4ac0: 5f70 6561 6b3a 2074 7970 696e 672e 4f70  _peak: typing.Op
 000b4ad0: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
 000b4ae0: 795d 0a20 2020 2020 2020 2027 2727 0a20  y].        '''. 
 000b4af0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
 000b4b00: 2064 6566 2072 6570 6f72 7428 7365 6c66   def report(self
 000b4b10: 2c20 7479 7065 3a20 7479 7069 6e67 2e55  , type: typing.U
 000b4b20: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-000b4b30: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
-000b4b40: 5b69 6e74 5d5d 2c0a 2020 2020 2020 2020  [int]],.        
+000b4b30: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
+000b4b40: 5b73 7472 5d5d 2c0a 2020 2020 2020 2020  [str]],.        
 000b4b50: 2020 2020 2020 206d 6573 7361 6765 3a20         message: 
 000b4b60: 7479 7069 6e67 2e55 6e69 6f6e 5b73 7472  typing.Union[str
 000b4b70: 2c20 7479 7069 6e67 2e41 6e79 5d29 3a0a  , typing.Any]):.
 000b4b80: 2020 2020 2020 2020 2727 2720 5265 706f          ''' Repo
 000b4b90: 7274 2069 6e66 6f2c 2077 6172 6e69 6e67  rt info, warning
 000b4ba0: 206f 7220 6572 726f 7220 6d65 7373 6167   or error messag
 000b4bb0: 6573 0a0a 2020 2020 2020 2020 3a70 6172  es..        :par
 000b4bc0: 616d 2074 7970 653a 2054 7970 650a 2020  am type: Type.  
 000b4bd0: 2020 2020 2020 3a74 7970 6520 7479 7065        :type type
 000b4be0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b74  : typing.Union[t
-000b4bf0: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
-000b4c00: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
+000b4bf0: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
+000b4c00: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
 000b4c10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
 000b4c20: 6d65 7373 6167 653a 2052 6570 6f72 7420  message: Report 
 000b4c30: 4d65 7373 6167 650a 2020 2020 2020 2020  Message.        
 000b4c40: 3a74 7970 6520 6d65 7373 6167 653a 2074  :type message: t
 000b4c50: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
 000b4c60: 2074 7970 696e 672e 416e 795d 0a20 2020   typing.Any].   
 000b4c70: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
@@ -65979,22 +65979,22 @@
 00101ba0: 7769 7468 2074 6865 2063 7572 7265 6e74  with the current
 00101bb0: 6c79 2064 6973 706c 6179 6564 2069 6d61  ly displayed ima
 00101bc0: 6765 2061 7373 6967 6e65 640a 0a20 2020  ge assigned..   
 00101bd0: 203a 7479 7065 3a20 626f 6f6c 0a20 2020   :type: bool.   
 00101be0: 2027 2727 0a0a 2020 2020 736e 6170 5f65   '''..    snap_e
 00101bf0: 6c65 6d65 6e74 733a 2074 7970 696e 672e  lements: typing.
 00101c00: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-00101c10: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
-00101c20: 745b 696e 745d 5d20 3d20 4e6f 6e65 0a20  t[int]] = None. 
+00101c10: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
+00101c20: 745b 7374 725d 5d20 3d20 4e6f 6e65 0a20  t[str]] = None. 
 00101c30: 2020 2027 2727 2054 7970 6520 6f66 2065     ''' Type of e
 00101c40: 6c65 6d65 6e74 2074 6f20 736e 6170 2074  lement to snap t
 00101c50: 6f0a 0a20 2020 203a 7479 7065 3a20 7479  o..    :type: ty
 00101c60: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-00101c70: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
-00101c80: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
+00101c70: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
+00101c80: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
 00101c90: 2027 2727 0a0a 2020 2020 736e 6170 5f65   '''..    snap_e
 00101ca0: 6c65 6d65 6e74 735f 746f 6f6c 3a20 7479  lements_tool: ty
 00101cb0: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 00101cc0: 696e 745d 203d 204e 6f6e 650a 2020 2020  int] = None.    
 00101cd0: 2727 2720 5468 6520 7461 7267 6574 2074  ''' The target t
 00101ce0: 6f20 7573 6520 7768 696c 6520 736e 6170  o use while snap
 00101cf0: 7069 6e67 202a 2060 6047 454f 4d45 5452  ping * ``GEOMETR
@@ -107591,16 +107591,16 @@
 001a4460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a4470: 2020 2020 2020 2020 6576 656e 743a 2074          event: t
 001a4480: 7970 696e 672e 4f70 7469 6f6e 616c 5b27  yping.Optional['
 001a4490: 4576 656e 7427 5d0a 2020 2020 2020 2020  Event'].        
 001a44a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a44b0: 2020 2029 202d 3e20 7479 7069 6e67 2e55     ) -> typing.U
 001a44c0: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-001a44d0: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
-001a44e0: 5b69 6e74 5d5d 3a0a 2020 2020 2020 2020  [int]]:.        
+001a44d0: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
+001a44e0: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
 001a44f0: 2727 2720 4f70 6572 6174 6f72 2070 6f70  ''' Operator pop
 001a4500: 7570 2069 6e76 6f6b 6520 2873 686f 7720  up invoke (show 
 001a4510: 6f70 6572 6174 6f72 2070 726f 7065 7274  operator propert
 001a4520: 6965 7320 616e 6420 6578 6563 7574 6520  ies and execute 
 001a4530: 6974 2061 7574 6f6d 6174 6963 616c 6c79  it automatically
 001a4540: 206f 6e20 6368 616e 6765 7329 0a0a 2020   on changes)..  
 001a4550: 2020 2020 2020 3a70 6172 616d 206f 7065        :param ope
@@ -107611,34 +107611,34 @@
 001a45a0: 274f 7065 7261 746f 7227 5d0a 2020 2020  'Operator'].    
 001a45b0: 2020 2020 3a70 6172 616d 2065 7665 6e74      :param event
 001a45c0: 3a20 4576 656e 740a 2020 2020 2020 2020  : Event.        
 001a45d0: 3a74 7970 6520 6576 656e 743a 2074 7970  :type event: typ
 001a45e0: 696e 672e 4f70 7469 6f6e 616c 5b27 4576  ing.Optional['Ev
 001a45f0: 656e 7427 5d0a 2020 2020 2020 2020 3a72  ent'].        :r
 001a4600: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
-001a4610: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
-001a4620: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
-001a4630: 6e74 5d5d 0a20 2020 2020 2020 203a 7265  nt]].        :re
+001a4610: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
+001a4620: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
+001a4630: 7472 5d5d 0a20 2020 2020 2020 203a 7265  tr]].        :re
 001a4640: 7475 726e 3a20 7265 7375 6c74 0a20 2020  turn: result.   
 001a4650: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
 001a4660: 2070 6173 730a 0a20 2020 2040 636c 6173   pass..    @clas
 001a4670: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
 001a4680: 696e 766f 6b65 5f70 726f 7073 5f64 6961  invoke_props_dia
 001a4690: 6c6f 6728 0a20 2020 2020 2020 2020 2020  log(.           
 001a46a0: 2063 6c73 2c0a 2020 2020 2020 2020 2020   cls,.          
 001a46b0: 2020 6f70 6572 6174 6f72 3a20 7479 7069    operator: typi
 001a46c0: 6e67 2e4f 7074 696f 6e61 6c5b 274f 7065  ng.Optional['Ope
 001a46d0: 7261 746f 7227 5d2c 0a20 2020 2020 2020  rator'],.       
 001a46e0: 2020 2020 2077 6964 7468 3a20 7479 7069       width: typi
 001a46f0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
 001a4700: 6e67 2e41 6e79 5d20 3d20 3330 300a 2020  ng.Any] = 300.  
 001a4710: 2020 2920 2d3e 2074 7970 696e 672e 556e    ) -> typing.Un
-001a4720: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
-001a4730: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
-001a4740: 696e 745d 5d3a 0a20 2020 2020 2020 2027  int]]:.        '
+001a4720: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
+001a4730: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
+001a4740: 7374 725d 5d3a 0a20 2020 2020 2020 2027  str]]:.        '
 001a4750: 2727 204f 7065 7261 746f 7220 6469 616c  '' Operator dial
 001a4760: 6f67 2028 6e6f 6e2d 6175 746f 6578 6563  og (non-autoexec
 001a4770: 2070 6f70 7570 2920 696e 766f 6b65 2028   popup) invoke (
 001a4780: 7368 6f77 206f 7065 7261 746f 7220 7072  show operator pr
 001a4790: 6f70 6572 7469 6573 2061 6e64 206f 6e6c  operties and onl
 001a47a0: 7920 6578 6563 7574 6520 6974 206f 6e20  y execute it on 
 001a47b0: 636c 6963 6b20 6f6e 204f 4b20 6275 7474  click on OK butt
@@ -107652,16 +107652,16 @@
 001a4830: 6d20 7769 6474 683a 2057 6964 7468 206f  m width: Width o
 001a4840: 6620 7468 6520 706f 7075 700a 2020 2020  f the popup.    
 001a4850: 2020 2020 3a74 7970 6520 7769 6474 683a      :type width:
 001a4860: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
 001a4870: 5b74 7970 696e 672e 416e 795d 0a20 2020  [typing.Any].   
 001a4880: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
 001a4890: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-001a48a0: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
-001a48b0: 672e 5365 745b 696e 745d 5d0a 2020 2020  g.Set[int]].    
+001a48a0: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
+001a48b0: 672e 5365 745b 7374 725d 5d0a 2020 2020  g.Set[str]].    
 001a48c0: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
 001a48d0: 756c 740a 2020 2020 2020 2020 2727 270a  ult.        '''.
 001a48e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
 001a48f0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
 001a4900: 2020 2064 6566 2069 6e76 6f6b 655f 7365     def invoke_se
 001a4910: 6172 6368 5f70 6f70 7570 2863 6c73 2c20  arch_popup(cls, 
 001a4920: 6f70 6572 6174 6f72 3a20 7479 7069 6e67  operator: typing
@@ -107694,16 +107694,16 @@
 001a4ad0: 6174 6f72 275d 2c0a 2020 2020 2020 2020  ator'],.        
 001a4ae0: 2020 2020 2020 2020 2020 2020 2077 6964               wid
 001a4af0: 7468 3a20 7479 7069 6e67 2e4f 7074 696f  th: typing.Optio
 001a4b00: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d20  nal[typing.Any] 
 001a4b10: 3d20 3330 300a 2020 2020 2020 2020 2020  = 300.          
 001a4b20: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
 001a4b30: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-001a4b40: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
-001a4b50: 7069 6e67 2e53 6574 5b69 6e74 5d5d 3a0a  ping.Set[int]]:.
+001a4b40: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
+001a4b50: 7069 6e67 2e53 6574 5b73 7472 5d5d 3a0a  ping.Set[str]]:.
 001a4b60: 2020 2020 2020 2020 2727 2720 4f70 6572          ''' Oper
 001a4b70: 6174 6f72 2070 6f70 7570 2069 6e76 6f6b  ator popup invok
 001a4b80: 6520 286f 6e6c 7920 7368 6f77 7320 6f70  e (only shows op
 001a4b90: 6572 6174 6f72 2773 2070 726f 7065 7274  erator's propert
 001a4ba0: 6965 732c 2077 6974 686f 7574 2065 7865  ies, without exe
 001a4bb0: 6375 7469 6e67 2069 7429 0a0a 2020 2020  cuting it)..    
 001a4bc0: 2020 2020 3a70 6172 616d 206f 7065 7261      :param opera
@@ -107715,16 +107715,16 @@
 001a4c20: 2020 3a70 6172 616d 2077 6964 7468 3a20    :param width: 
 001a4c30: 5769 6474 6820 6f66 2074 6865 2070 6f70  Width of the pop
 001a4c40: 7570 0a20 2020 2020 2020 203a 7479 7065  up.        :type
 001a4c50: 2077 6964 7468 3a20 7479 7069 6e67 2e4f   width: typing.O
 001a4c60: 7074 696f 6e61 6c5b 7479 7069 6e67 2e41  ptional[typing.A
 001a4c70: 6e79 5d0a 2020 2020 2020 2020 3a72 7479  ny].        :rty
 001a4c80: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-001a4c90: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
-001a4ca0: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
+001a4c90: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
+001a4ca0: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
 001a4cb0: 5d5d 0a20 2020 2020 2020 203a 7265 7475  ]].        :retu
 001a4cc0: 726e 3a20 7265 7375 6c74 0a20 2020 2020  rn: result.     
 001a4cd0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 001a4ce0: 6173 730a 0a20 2020 2040 636c 6173 736d  ass..    @classm
 001a4cf0: 6574 686f 640a 2020 2020 6465 6620 696e  ethod.    def in
 001a4d00: 766f 6b65 5f63 6f6e 6669 726d 2863 6c73  voke_confirm(cls
 001a4d10: 2c20 6f70 6572 6174 6f72 3a20 7479 7069  , operator: typi
@@ -107732,16 +107732,16 @@
 001a4d30: 7261 746f 7227 5d2c 0a20 2020 2020 2020  rator'],.       
 001a4d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a4d50: 6576 656e 743a 2074 7970 696e 672e 4f70  event: typing.Op
 001a4d60: 7469 6f6e 616c 5b27 4576 656e 7427 5d0a  tional['Event'].
 001a4d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a4d80: 2020 2020 2020 2029 202d 3e20 7479 7069         ) -> typi
 001a4d90: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-001a4da0: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
-001a4db0: 2e53 6574 5b69 6e74 5d5d 3a0a 2020 2020  .Set[int]]:.    
+001a4da0: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
+001a4db0: 2e53 6574 5b73 7472 5d5d 3a0a 2020 2020  .Set[str]]:.    
 001a4dc0: 2020 2020 2727 2720 4f70 6572 6174 6f72      ''' Operator
 001a4dd0: 2063 6f6e 6669 726d 6174 696f 6e20 706f   confirmation po
 001a4de0: 7075 7020 286f 6e6c 7920 746f 206c 6574  pup (only to let
 001a4df0: 2075 7365 7220 636f 6e66 6972 6d20 7468   user confirm th
 001a4e00: 6520 6578 6563 7574 696f 6e2c 206e 6f20  e execution, no 
 001a4e10: 6f70 6572 6174 6f72 2070 726f 7065 7274  operator propert
 001a4e20: 6965 7320 7368 6f77 6e29 0a0a 2020 2020  ies shown)..    
@@ -107753,16 +107753,16 @@
 001a4e80: 7065 7261 746f 7227 5d0a 2020 2020 2020  perator'].      
 001a4e90: 2020 3a70 6172 616d 2065 7665 6e74 3a20    :param event: 
 001a4ea0: 4576 656e 740a 2020 2020 2020 2020 3a74  Event.        :t
 001a4eb0: 7970 6520 6576 656e 743a 2074 7970 696e  ype event: typin
 001a4ec0: 672e 4f70 7469 6f6e 616c 5b27 4576 656e  g.Optional['Even
 001a4ed0: 7427 5d0a 2020 2020 2020 2020 3a72 7479  t'].        :rty
 001a4ee0: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-001a4ef0: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
-001a4f00: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
+001a4ef0: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
+001a4f00: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
 001a4f10: 5d5d 0a20 2020 2020 2020 203a 7265 7475  ]].        :retu
 001a4f20: 726e 3a20 7265 7375 6c74 0a20 2020 2020  rn: result.     
 001a4f30: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 001a4f40: 6173 730a 0a20 2020 2040 636c 6173 736d  ass..    @classm
 001a4f50: 6574 686f 640a 2020 2020 6465 6620 706f  ethod.    def po
 001a4f60: 706d 656e 755f 6265 6769 6e5f 5f69 6e74  pmenu_begin__int
 001a4f70: 6572 6e61 6c28 636c 732c 0a20 2020 2020  ernal(cls,.     
@@ -113187,22 +113187,22 @@
 001ba220: 7373 6f6c 7665 2067 656f 6d65 7472 7920  ssolve geometry 
 001ba230: 746f 2066 6f72 6d20 706c 616e 6172 2070  to form planar p
 001ba240: 6f6c 7967 6f6e 732e 0a0a 2020 2020 3a74  olygons...    :t
 001ba250: 7970 653a 2074 7970 696e 672e 556e 696f  ype: typing.Unio
 001ba260: 6e5b 7374 722c 2069 6e74 5d0a 2020 2020  n[str, int].    
 001ba270: 2727 270a 0a20 2020 2064 656c 696d 6974  '''..    delimit
 001ba280: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b74  : typing.Union[t
-001ba290: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
-001ba2a0: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
+001ba290: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
+001ba2a0: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
 001ba2b0: 203d 204e 6f6e 650a 2020 2020 2727 2720   = None.    ''' 
 001ba2c0: 4c69 6d69 7420 6d65 7267 696e 6720 6765  Limit merging ge
 001ba2d0: 6f6d 6574 7279 0a0a 2020 2020 3a74 7970  ometry..    :typ
 001ba2e0: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-001ba2f0: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
-001ba300: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
+001ba2f0: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
+001ba300: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
 001ba310: 5d0a 2020 2020 2727 270a 0a20 2020 2066  ].    '''..    f
 001ba320: 6163 655f 636f 756e 743a 2069 6e74 203d  ace_count: int =
 001ba330: 204e 6f6e 650a 2020 2020 2727 2720 5468   None.    ''' Th
 001ba340: 6520 6375 7272 656e 7420 6e75 6d62 6572  e current number
 001ba350: 206f 6620 6661 6365 7320 696e 2074 6865   of faces in the
 001ba360: 2064 6563 696d 6174 6564 206d 6573 680a   decimated mesh.
 001ba370: 0a20 2020 203a 7479 7065 3a20 696e 740a  .    :type: int.
@@ -114471,21 +114471,21 @@
 001bf260: 6f20 6578 7465 726e 616c 2064 6973 706c  o external displ
 001bf270: 6163 656d 656e 7473 2066 696c 650a 0a20  acements file.. 
 001bf280: 2020 203a 7479 7065 3a20 7479 7069 6e67     :type: typing
 001bf290: 2e55 6e69 6f6e 5b73 7472 2c20 7479 7069  .Union[str, typi
 001bf2a0: 6e67 2e41 6e79 5d0a 2020 2020 2727 270a  ng.Any].    '''.
 001bf2b0: 0a20 2020 2066 6c69 705f 6178 6973 3a20  .    flip_axis: 
 001bf2c0: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-001bf2d0: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
-001bf2e0: 7069 6e67 2e53 6574 5b69 6e74 5d5d 203d  ping.Set[int]] =
+001bf2d0: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
+001bf2e0: 7069 6e67 2e53 6574 5b73 7472 5d5d 203d  ping.Set[str]] =
 001bf2f0: 204e 6f6e 650a 2020 2020 2727 2720 0a0a   None.    ''' ..
 001bf300: 2020 2020 3a74 7970 653a 2074 7970 696e      :type: typin
 001bf310: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-001bf320: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
-001bf330: 5365 745b 696e 745d 5d0a 2020 2020 2727  Set[int]].    ''
+001bf320: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
+001bf330: 5365 745b 7374 725d 5d0a 2020 2020 2727  Set[str]].    ''
 001bf340: 270a 0a20 2020 2066 6f72 7761 7264 5f61  '..    forward_a
 001bf350: 7869 733a 2074 7970 696e 672e 556e 696f  xis: typing.Unio
 001bf360: 6e5b 7374 722c 2069 6e74 5d20 3d20 4e6f  n[str, int] = No
 001bf370: 6e65 0a20 2020 2027 2727 200a 0a20 2020  ne.    ''' ..   
 001bf380: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
 001bf390: 6e69 6f6e 5b73 7472 2c20 696e 745d 0a20  nion[str, int]. 
 001bf3a0: 2020 2027 2727 0a0a 2020 2020 6672 616d     '''..    fram
```

### Comparing `fake-bpy-module-latest-20230521/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230522/bpy/utils/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
 import bpy.types
 
-from . import previews
 from . import units
+from . import previews
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def app_template_paths(*, path: typing.Optional[str] = None) -> typing.Any:
     ''' Returns valid application template paths.
```

### Comparing `fake-bpy-module-latest-20230521/bpy/utils/previews.py` & `fake-bpy-module-latest-20230522/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy/utils/units.py` & `fake-bpy-module-latest-20230522/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230522/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Object', 'bpy.types.Sequence', 'bpy.types.Action'],
+        Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Object', 'bpy.types.Sequence', 'bpy.types.Action']
+    :type object_action_pairs: typing.Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230521/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230522/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230522/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230522/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230522/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230522/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230522/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230522/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/bpy_types.py` & `fake-bpy-module-latest-20230522/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230522/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230521
+Version: 20230522
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230521/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230522/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230522/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/freestyle/functions.py` & `fake-bpy-module-latest-20230522/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/freestyle/predicates.py` & `fake-bpy-module-latest-20230522/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/freestyle/shaders.py` & `fake-bpy-module-latest-20230522/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/freestyle/types.py` & `fake-bpy-module-latest-20230522/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230522/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230522/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/gpu/capabilities.py` & `fake-bpy-module-latest-20230522/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/gpu/matrix.py` & `fake-bpy-module-latest-20230522/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/gpu/platform.py` & `fake-bpy-module-latest-20230522/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/gpu/shader.py` & `fake-bpy-module-latest-20230522/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/gpu/state.py` & `fake-bpy-module-latest-20230522/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/gpu/texture.py` & `fake-bpy-module-latest-20230522/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/gpu/types.py` & `fake-bpy-module-latest-20230522/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/gpu_extras/batch.py` & `fake-bpy-module-latest-20230522/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/gpu_extras/presets.py` & `fake-bpy-module-latest-20230522/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/idprop/types.py` & `fake-bpy-module-latest-20230522/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/imbuf/__init__.py` & `fake-bpy-module-latest-20230522/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/imbuf/types.py` & `fake-bpy-module-latest-20230522/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/keyingsets_builtins.py` & `fake-bpy-module-latest-20230522/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/keyingsets_utils.py` & `fake-bpy-module-latest-20230522/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/mathutils/__init__.py` & `fake-bpy-module-latest-20230522/mathutils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230522/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/mathutils/geometry.py` & `fake-bpy-module-latest-20230522/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/mathutils/kdtree.py` & `fake-bpy-module-latest-20230522/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/mathutils/noise.py` & `fake-bpy-module-latest-20230522/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/nodeitems_builtins.py` & `fake-bpy-module-latest-20230522/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/nodeitems_utils.py` & `fake-bpy-module-latest-20230522/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/rna_info.py` & `fake-bpy-module-latest-20230522/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/rna_keymap_ui.py` & `fake-bpy-module-latest-20230522/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/rna_prop_ui.py` & `fake-bpy-module-latest-20230522/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/rna_xml.py` & `fake-bpy-module-latest-20230522/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230521/setup.py` & `fake-bpy-module-latest-20230522/setup.py`

 * *Files identical despite different names*

