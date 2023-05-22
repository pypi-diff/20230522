# Comparing `tmp/ytdl-sub-2023.5.19.tar.gz` & `tmp/ytdl-sub-2023.5.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.5.19.tar", last modified: Fri May 19 16:07:14 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.5.22.tar", last modified: Mon May 22 17:24:09 2023, max compression
```

## Comparing `ytdl-sub-2023.5.19.tar` & `ytdl-sub-2023.5.22.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.108177 ytdl-sub-2023.5.19/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-19 16:07:14.108177 ytdl-sub-2023.5.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-19 16:07:14.108177 ytdl-sub-2023.5.19/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.080177 ytdl-sub-2023.5.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.084177 ytdl-sub-2023.5.19/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.088177 ytdl-sub-2023.5.19/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.088177 ytdl-sub-2023.5.19/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.092177 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/base_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.092177 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.092177 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.092177 ytdl-sub-2023.5.19/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.092177 ytdl-sub-2023.5.19/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.096177 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.096177 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.096177 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.096177 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.100177 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.100177 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.100177 ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.100177 ytdl-sub-2023.5.19/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.104177 ytdl-sub-2023.5.19/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.104177 ytdl-sub-2023.5.19/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.108177 ytdl-sub-2023.5.19/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-19 16:06:53.000000 ytdl-sub-2023.5.19/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:07:14.088177 ytdl-sub-2023.5.19/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-19 16:07:14.000000 ytdl-sub-2023.5.19/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-19 16:07:14.000000 ytdl-sub-2023.5.19/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:07:14.000000 ytdl-sub-2023.5.19/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-19 16:07:14.000000 ytdl-sub-2023.5.19/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-19 16:07:14.000000 ytdl-sub-2023.5.19/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 16:07:14.000000 ytdl-sub-2023.5.19/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.862057 ytdl-sub-2023.5.22/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-22 17:24:09.862057 ytdl-sub-2023.5.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-22 17:24:09.862057 ytdl-sub-2023.5.22/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.846057 ytdl-sub-2023.5.22/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.850057 ytdl-sub-2023.5.22/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.850057 ytdl-sub-2023.5.22/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.850057 ytdl-sub-2023.5.22/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.850057 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/base_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.850057 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.854057 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.854057 ytdl-sub-2023.5.22/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.854057 ytdl-sub-2023.5.22/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.854057 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.854057 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.854057 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.854057 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.854057 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.858057 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.858057 ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.858057 ytdl-sub-2023.5.22/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.858057 ytdl-sub-2023.5.22/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.862057 ytdl-sub-2023.5.22/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.862057 ytdl-sub-2023.5.22/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-22 17:23:54.000000 ytdl-sub-2023.5.22/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:24:09.850057 ytdl-sub-2023.5.22/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-22 17:24:09.000000 ytdl-sub-2023.5.22/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-22 17:24:09.000000 ytdl-sub-2023.5.22/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:24:09.000000 ytdl-sub-2023.5.22/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-22 17:24:09.000000 ytdl-sub-2023.5.22/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 17:24:09.000000 ytdl-sub-2023.5.22/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 17:24:09.000000 ytdl-sub-2023.5.22/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.5.19/LICENSE` & `ytdl-sub-2023.5.22/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/PKG-INFO` & `ytdl-sub-2023.5.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.5.19
+Version: 2023.5.22
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.5.19/README.md` & `ytdl-sub-2023.5.22/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/pyproject.toml` & `ytdl-sub-2023.5.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/setup.cfg` & `ytdl-sub-2023.5.22/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/main.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/regex.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,53 +20,70 @@
 from ytdl_sub.validators.validators import BoolValidator
 
 logger = Logger.get(name="regex")
 
 
 class SourceVariableRegex(StrictDictValidator):
 
-    _required_keys = {"match"}
-    _optional_keys = {"capture_group_defaults", "capture_group_names"}
+    _optional_keys = {"match", "exclude", "capture_group_defaults", "capture_group_names"}
 
     def __init__(self, name, value):
         super().__init__(name, value)
-        self._match = self._validate_key(key="match", validator=RegexListValidator)
+        self._match = self._validate_key_if_present(key="match", validator=RegexListValidator)
+        self._exclude = self._validate_key_if_present(key="exclude", validator=RegexListValidator)
         self._capture_group_defaults = self._validate_key_if_present(
             key="capture_group_defaults", validator=ListFormatterValidator
         )
         self._capture_group_names = self._validate_key_if_present(
             key="capture_group_names", validator=SourceVariableNameListValidator, default=[]
         )
 
+        if self._match is None and self._exclude is None:
+            raise self._validation_exception("must specify either `match` or `exclude`")
+
+        if self._match is None and (self._capture_group_defaults or self._capture_group_names.list):
+            raise self._validation_exception(
+                "capture group parameters requires at least one `match` to be specified"
+            )
+
         # If defaults are to be used, ensure there are the same number of defaults as there are
         # capture groups
         if self._capture_group_defaults is not None and self._match.num_capture_groups != len(
             self._capture_group_defaults.list
         ):
             raise self._validation_exception(
                 f"number of defaults must match number of capture groups, "
                 f"{len(self._capture_group_defaults.list)} != {self._match.num_capture_groups}"
             )
 
         # If there are capture groups, ensure there are capture group names
-        if len(self._capture_group_names.list) != self._match.num_capture_groups:
+        if self._match and (len(self._capture_group_names.list) != self._match.num_capture_groups):
             raise self._validation_exception(
                 f"number of capture group names must match number of capture groups, "
                 f"{len(self._capture_group_names.list)} != {self._match.num_capture_groups}"
             )
 
     @property
-    def match(self) -> RegexListValidator:
+    def match(self) -> Optional[RegexListValidator]:
         """
-        Required. List of regex strings to try to match against a source variable. Each regex
+        List of regex strings to try to match against a source variable. Each regex
         string must have the same number of capture groups.
         """
         return self._match
 
     @property
+    def exclude(self) -> Optional[RegexListValidator]:
+        """
+        List of regex strings to try to match against a source variable. If one of the regex strings
+        match, then the entry will be skipped. If both ``exclude`` and ``match`` are specified,
+        entries will get skipped if the regex matches against both ``exclude`` and ``match``.
+        """
+        return self._exclude
+
+    @property
     def capture_group_names(self) -> Optional[List[str]]:
         """
         Optional (only when no capture groups are in the regex string). List of names to store the
         capture group values to. These and ``_sanitized`` versions will be available to use as
         source variables. The list's length must be equal to the number of match capture groups.
         """
         return [validator.value for validator in self._capture_group_names.list]
@@ -125,30 +142,33 @@
              from:
                # For each entry's `title` value...
                title:
                  # Perform this regex match on it to act as a filter.
                  # This will only download videos with "[Official Video]" in it. Note that we
                  # double backslash to make YAML happy
                  match:
-                  - '\\[Official Video\\]'
+                   - '\\[Official Video\\]'
 
                # For each entry's `description` value...
                description:
                  # Match with capture groups and defaults.
                  # This tries to scrape a date from the description and produce new
                  # source variables
                  match:
-                  - "([0-9]{4})-([0-9]{2})-([0-9]{2})"
+                   - "([0-9]{4})-([0-9]{2})-([0-9]{2})"
+                 # Exclude any entry where the description contains #short
+                 exclude:
+                   - "#short"
 
                  # Each capture group creates these new source variables, respectively,
                  # as well a sanitized version, i.e. `captured_upload_year_sanitized`
                  capture_group_names:
-                  - "captured_upload_year"
-                  - "captured_upload_month"
-                  - "captured_upload_day"
+                   - "captured_upload_year"
+                   - "captured_upload_month"
+                   - "captured_upload_day"
 
                  # And if the string does not match, use these as respective default
                  # values for the new source variables.
                  capture_group_defaults:
                    - "{upload_year}"
                    - "{upload_month}"
                    - "{upload_day}"
@@ -253,14 +273,27 @@
 
         entry.kwargs(YTDL_SUB_REGEX_SOURCE_VARS).append(source_var)
 
     @classmethod
     def _contains_processed_regex_source_var(cls, entry: Entry, source_var: str) -> bool:
         return source_var in entry.kwargs_get(YTDL_SUB_REGEX_SOURCE_VARS, [])
 
+    def _try_skip_entry(self, entry: Entry, source_var: str) -> None:
+        # Skip the entry if toggled
+        if self.plugin_options.skip_if_match_fails:
+            logger.info(
+                "Regex failed to match '%s' from '%s', skipping.",
+                source_var,
+                entry.title,
+            )
+            return None
+
+        # Otherwise, error
+        raise RegexNoMatchException(f"Regex failed to match '{source_var}' from '{entry.title}'")
+
     def _modify_entry_metadata(self, entry: Entry, is_metadata_stage: bool) -> Optional[Entry]:
         """
         Parameters
         ----------
         entry
             Entry to add source variables to
         is_metadata_stage
@@ -288,78 +321,78 @@
 
             # Continue if the source var isn't in the dict since entry variables could be added
             # after the metadata stage
             if is_metadata_stage and source_var not in entry_variable_dict:
                 continue
 
             self._add_processed_regex_source_var(entry, source_var)
-            maybe_capture = regex_options.match.match_any(input_str=entry_variable_dict[source_var])
-
-            # If no capture
-            if maybe_capture is None:
-                # and no defaults
-                if not regex_options.has_defaults:
-                    # Skip the entry if toggled
-                    if self.plugin_options.skip_if_match_fails:
-                        logger.info(
-                            "Regex failed to match '%s' from '%s', skipping.",
-                            source_var,
-                            entry.title,
-                        )
-                        return None
-
-                    # Otherwise, error
-                    raise RegexNoMatchException(
-                        f"Regex failed to match '{source_var}' from '{entry.title}'"
-                    )
 
-                # otherwise, use defaults (apply them using the original entry source dict)
-                source_variables_and_overrides_dict = dict(
-                    entry_variable_dict, **self.overrides.dict_with_format_strings
+            if (
+                regex_options.exclude is not None
+                and regex_options.exclude.match_any(input_str=entry_variable_dict[source_var])
+                is not None
+            ):
+                return self._try_skip_entry(entry=entry, source_var=source_var)
+
+            # If match is present
+            if regex_options.match is not None:
+                maybe_capture = regex_options.match.match_any(
+                    input_str=entry_variable_dict[source_var]
                 )
 
-                # add both the default...
-                entry.add_variables(
-                    variables_to_add={
-                        regex_options.capture_group_names[i]: default.apply_formatter(
-                            variable_dict=source_variables_and_overrides_dict
-                        )
-                        for i, default in enumerate(regex_options.capture_group_defaults)
-                    },
-                )
-                # and sanitized default
-                entry.add_variables(
-                    variables_to_add={
-                        f"{regex_options.capture_group_names[i]}_sanitized": sanitize_filename(
-                            default.apply_formatter(
+                # And nothing matched
+                if maybe_capture is None:
+                    # and no defaults
+                    if not regex_options.has_defaults:
+                        return self._try_skip_entry(entry=entry, source_var=source_var)
+
+                    # otherwise, use defaults (apply them using the original entry source dict)
+                    source_variables_and_overrides_dict = dict(
+                        entry_variable_dict, **self.overrides.dict_with_format_strings
+                    )
+
+                    # add both the default...
+                    entry.add_variables(
+                        variables_to_add={
+                            regex_options.capture_group_names[i]: default.apply_formatter(
                                 variable_dict=source_variables_and_overrides_dict
                             )
-                        )
-                        for i, default in enumerate(regex_options.capture_group_defaults)
-                    },
-                )
-            # There is a capture, add the source variables to the entry as
-            # {source_var}_capture_1, {source_var}_capture_2, ...
-            else:
-                # Add the value...
-                entry.add_variables(
-                    variables_to_add={
-                        regex_options.capture_group_names[i]: capture
-                        for i, capture in enumerate(maybe_capture)
-                    },
-                )
-                # And the sanitized value
-                entry.add_variables(
-                    variables_to_add={
-                        f"{regex_options.capture_group_names[i]}_sanitized": sanitize_filename(
-                            capture
-                        )
-                        for i, capture in enumerate(maybe_capture)
-                    },
-                )
+                            for i, default in enumerate(regex_options.capture_group_defaults)
+                        },
+                    )
+                    # and sanitized default
+                    entry.add_variables(
+                        variables_to_add={
+                            f"{regex_options.capture_group_names[i]}_sanitized": sanitize_filename(
+                                default.apply_formatter(
+                                    variable_dict=source_variables_and_overrides_dict
+                                )
+                            )
+                            for i, default in enumerate(regex_options.capture_group_defaults)
+                        },
+                    )
+                # There is a capture, add the source variables to the entry as
+                # {source_var}_capture_1, {source_var}_capture_2, ...
+                else:
+                    # Add the value...
+                    entry.add_variables(
+                        variables_to_add={
+                            regex_options.capture_group_names[i]: capture
+                            for i, capture in enumerate(maybe_capture)
+                        },
+                    )
+                    # And the sanitized value
+                    entry.add_variables(
+                        variables_to_add={
+                            f"{regex_options.capture_group_names[i]}_sanitized": sanitize_filename(
+                                capture
+                            )
+                            for i, capture in enumerate(maybe_capture)
+                        },
+                    )
 
         return entry
 
     def modify_entry_metadata(self, entry: Entry) -> Optional[Entry]:
         """
         Perform regex at the metadata stage
         """
```

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.5.22/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.5.22/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.5.22/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.5.19
+Version: 2023.5.22
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.5.19/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.5.22/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

