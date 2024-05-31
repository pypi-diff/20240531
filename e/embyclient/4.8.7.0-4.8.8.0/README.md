# Comparing `tmp/embyclient-4.8.7.0.tar.gz` & `tmp/embyclient-4.8.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embyclient-4.8.7.0.tar", last modified: Fri May 17 00:17:09 2024, max compression
+gzip compressed data, was "embyclient-4.8.8.0.tar", last modified: Fri May 31 00:17:01 2024, max compression
```

## Comparing `embyclient-4.8.7.0.tar` & `embyclient-4.8.8.0.tar`

### file list

```diff
@@ -1,337 +1,337 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:17:09.689081 embyclient-4.8.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-17 00:17:09.689081 embyclient-4.8.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:17:09.629081 embyclient-4.8.7.0/embyclient/
--rw-r--r--   0 runner    (1001) docker     (127)    28759 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24584 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:17:09.689081 embyclient-4.8.7.0/embyclient/models/
--rw-r--r--   0 runner    (1001) docker     (127)    22941 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/access_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/actions_postback_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/activity_log_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/album_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/all_theme_media_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_available_recording_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_base_items_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_configuration_page_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_epg_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_listing_provider_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_name_id_description_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_on_playback_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_set_channel_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_set_channel_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_set_channel_sort_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/api_tag_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/artist_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/attributes_simple_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/attributes_value_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/authenticate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/authenticate_user_by_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/authentication_authentication_result.py
--rw-r--r--   0 runner    (1001) docker     (127)   126488 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/base_item_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/base_item_person.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/bit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/book_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/branding_branding_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/channel_management_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/chapter_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/codec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/codec_directions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/codec_kinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/codec_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/codec_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/collections_collection_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/color_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/common_editor_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/common_interfaces_i_codec_device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/common_plugins_i_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/conditions_property_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/conditions_property_condition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/connect_connect_authentication_exchange_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/connect_user_link_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/connect_user_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/container_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/create_user_by_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/day_of_week.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/default_directory_browser_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13068 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/device_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/devices_content_upload_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/devices_device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/devices_device_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/devices_local_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/direct_play_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/display_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/dlna_profile_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/dlna_profiles_device_identification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/dlna_profiles_device_profile_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    37624 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/dlna_profiles_dlna_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/dlna_profiles_header_match_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/dlna_profiles_http_header_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/dlna_profiles_protocol_info_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/drawing_image_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/dynamic_day_of_week.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/edit_object_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/editors_editor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/editors_editor_button_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/editors_editor_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/encoding_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/enums_ui_command_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/enums_ui_view_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/extended_video_sub_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/extended_video_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/external_id_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/external_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/feature_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/feature_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/forgot_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/forgot_password_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/forgot_password_pin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/forgot_password_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/game_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/general_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/generic_edit_i_edit_object_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/get_directory_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/globalization_country_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/globalization_culture_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/globalization_localizaton_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/image_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/image_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/image_saving_convention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/image_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/installation_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/io_file_system_entry_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/io_file_system_entry_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/item_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/item_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/item_file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/item_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/level_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_add_media_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_add_virtual_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_delete_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_item_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_library_option_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_library_options_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_library_type_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_media_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_media_update_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    60338 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_post_updated_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_remove_media_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_remove_virtual_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_rename_virtual_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_sub_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_update_library_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_update_media_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/library_user_copy_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_stream_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_channel_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_guide_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_keep_until.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_keyword_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_keyword_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18555 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_listings_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_live_tv_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_recording_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_series_timer_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_series_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    24849 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_timer_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/live_tv_tuner_host_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/location_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/log_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/logging_log_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/marker_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/mb_backup_api_all_backups_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/mb_backup_api_data_restore_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/mb_backup_api_restore_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/mb_backup_api_user_restore_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/mb_backup_backup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/media_encoding_codec_parameter_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/media_path_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/media_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    40118 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/media_source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/media_source_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    58923 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/media_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/media_stream_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/media_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/metadata_editor_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/metadata_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/metadata_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/metadata_refresh_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/movie_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/music_video_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/name_id_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/name_long_id_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/name_value_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/net_end_point_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/net_sockets_address_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/notification_category_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/notification_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/package_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/package_target_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/package_version_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/package_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/parental_rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/path_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/persistence_intro_debug_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/person_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/person_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/pin_redeem_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/play_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/play_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/play_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playback_error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    19970 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playback_info_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playback_info_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    25054 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playback_progress_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playback_start_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playback_stop_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/player_state_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playlists_add_to_playlist_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playlists_playlist_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playstate_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/playstate_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/plugins_configuration_page_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/plugins_plugin_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/process_run_metrics_process_metric_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/process_run_metrics_process_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/profile_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/profile_condition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/profile_condition_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/profile_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/profile_level_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/progress_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/provider_id_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/proxy_header_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/public_system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_activity_log_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_api_epg_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_base_item_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_channel_management_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_devices_device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_live_tv_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_log_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_sync_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_sync_job_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_user_library_official_rating_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_user_library_tag_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/query_result_virtual_folder_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/queue_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/rating_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/recommendation_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/recommendation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_image_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_album_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_artist_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_book_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_game_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_item_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_movie_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_music_video_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_person_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_series_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_query_trailer_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_search_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/remote_subtitle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/repeat_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/resolution_with_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/response_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/roku_metadata_api_thumbnail_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/run_ui_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/secondary_frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/segment_skip_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/series_display_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/series_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    66579 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/server_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    23279 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/session_session_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/session_user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/song_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/subtitle_delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/subtitle_location_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/subtitle_playback_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/subtitle_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/subtitles_subtitle_download_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_data_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_data_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_dialog_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_job_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_job_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_job_item_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_job_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_profile_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_quality_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/sync_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/synced_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/synced_item_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/system_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    34832 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/task_completion_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/task_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/task_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/task_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/task_trigger_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/theme_media_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/trailer_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/transcode_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/transcode_seek_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    29815 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/transcoding_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    19145 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/transcoding_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/transcoding_vp_step_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/transcoding_vp_step_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/transport_stream_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/tuple_double_double.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/type_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/ui_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/ui_tab_page_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/ui_view_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/unrated_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/update_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_action_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    19873 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_item_data_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_item_share_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_library_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_library_leave_shared_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_library_official_rating_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_library_remove_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_library_tag_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_library_update_user_item_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_notification_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    45913 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/user_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/video3_d_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    22765 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/video_codec_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/video_media_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/virtual_folder_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/models/wake_on_lan_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/embyclient/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:17:09.689081 embyclient-4.8.7.0/embyclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-17 00:17:09.000000 embyclient-4.8.7.0/embyclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-05-17 00:17:09.000000 embyclient-4.8.7.0/embyclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 00:17:09.000000 embyclient-4.8.7.0/embyclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 00:17:09.000000 embyclient-4.8.7.0/embyclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 00:17:09.000000 embyclient-4.8.7.0/embyclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 00:17:09.689081 embyclient-4.8.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-17 00:17:02.000000 embyclient-4.8.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:01.019743 embyclient-4.8.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 00:17:01.019743 embyclient-4.8.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:00.963742 embyclient-4.8.8.0/embyclient/
+-rw-r--r--   0 runner    (1001) docker     (127)    28759 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24584 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:01.019743 embyclient-4.8.8.0/embyclient/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    22941 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/access_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/actions_postback_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/activity_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/album_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/all_theme_media_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_available_recording_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_base_items_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_configuration_page_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_epg_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_listing_provider_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_name_id_description_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_on_playback_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_set_channel_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_set_channel_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_set_channel_sort_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/api_tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/artist_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/attributes_simple_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/attributes_value_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/authenticate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/authenticate_user_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/authentication_authentication_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126488 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/base_item_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/base_item_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/bit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/book_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/branding_branding_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/channel_management_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/chapter_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/codec_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/codec_directions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/codec_kinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/codec_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/codec_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/collections_collection_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/color_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/common_editor_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/common_interfaces_i_codec_device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/common_plugins_i_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/conditions_property_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/conditions_property_condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/connect_connect_authentication_exchange_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/connect_user_link_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/connect_user_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/container_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/create_user_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/day_of_week.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/default_directory_browser_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13068 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/device_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/devices_content_upload_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/devices_device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/devices_device_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/devices_local_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/direct_play_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/display_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/dlna_profile_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/dlna_profiles_device_identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/dlna_profiles_device_profile_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37624 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/dlna_profiles_dlna_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/dlna_profiles_header_match_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/dlna_profiles_http_header_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/dlna_profiles_protocol_info_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/drawing_image_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/dynamic_day_of_week.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/edit_object_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/editors_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/editors_editor_button_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/editors_editor_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/encoding_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/enums_ui_command_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/enums_ui_view_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/extended_video_sub_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/extended_video_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/external_id_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/external_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/feature_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/forgot_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/forgot_password_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/forgot_password_pin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/forgot_password_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/game_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/general_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/generic_edit_i_edit_object_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/get_directory_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/globalization_country_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/globalization_culture_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/globalization_localizaton_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/image_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/image_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/image_saving_convention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/installation_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/io_file_system_entry_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/io_file_system_entry_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/item_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/item_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/item_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/item_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/level_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_add_media_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_add_virtual_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_delete_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_item_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_library_option_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_library_options_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_library_type_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_media_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_media_update_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60338 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_post_updated_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_remove_media_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_remove_virtual_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_rename_virtual_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_sub_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_update_library_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_update_media_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/library_user_copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_stream_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_channel_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_guide_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_keep_until.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_keyword_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_keyword_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18555 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_listings_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_live_tv_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_recording_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_series_timer_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_series_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24849 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_timer_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/live_tv_tuner_host_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/location_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/log_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/logging_log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/marker_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/mb_backup_api_all_backups_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/mb_backup_api_data_restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/mb_backup_api_restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/mb_backup_api_user_restore_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/mb_backup_backup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/media_encoding_codec_parameter_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/media_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/media_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40118 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/media_source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/media_source_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58923 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/media_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/media_stream_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/media_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/metadata_editor_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/metadata_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/metadata_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/metadata_refresh_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/movie_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/music_video_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/name_id_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/name_long_id_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/name_value_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/net_end_point_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/net_sockets_address_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/notification_category_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/notification_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/package_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/package_target_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/package_version_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/package_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/parental_rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/path_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/persistence_intro_debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/person_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/person_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/pin_redeem_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/play_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/play_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/play_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playback_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19970 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playback_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playback_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25726 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playback_progress_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playback_start_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playback_stop_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/player_state_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playlists_add_to_playlist_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playlists_playlist_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playstate_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/playstate_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/plugins_configuration_page_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/plugins_plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/process_run_metrics_process_metric_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/process_run_metrics_process_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/profile_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/profile_condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/profile_condition_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/profile_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/profile_level_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/progress_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/provider_id_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/proxy_header_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/public_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_activity_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_api_epg_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_base_item_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_channel_management_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_devices_device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_live_tv_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_log_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_sync_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_sync_job_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_user_library_official_rating_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_user_library_tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/query_result_virtual_folder_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/queue_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/rating_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/recommendation_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/recommendation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_image_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_album_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_artist_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_book_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_game_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_item_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_movie_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_music_video_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_person_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_series_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_query_trailer_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/remote_subtitle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/repeat_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/resolution_with_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/response_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/roku_metadata_api_thumbnail_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/run_ui_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/secondary_frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/segment_skip_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/series_display_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/series_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66579 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/server_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23279 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/session_session_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/session_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/song_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/subtitle_delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/subtitle_location_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/subtitle_playback_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/subtitle_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/subtitles_subtitle_download_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_dialog_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_job_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_job_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_job_item_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_job_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_profile_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_quality_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/sync_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/synced_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/synced_item_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/system_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34832 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/task_completion_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/task_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/task_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/task_trigger_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/theme_media_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/trailer_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/transcode_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/transcode_seek_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29815 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/transcoding_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19145 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/transcoding_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/transcoding_vp_step_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/transcoding_vp_step_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/transport_stream_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/tuple_double_double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/type_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/ui_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/ui_tab_page_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/ui_view_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/unrated_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/update_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19873 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_item_data_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_item_share_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_library_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_library_leave_shared_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_library_official_rating_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_library_remove_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_library_tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_library_update_user_item_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_notification_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45913 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/user_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/video3_d_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22765 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/video_codec_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/video_media_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/virtual_folder_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/models/wake_on_lan_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/embyclient/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:01.019743 embyclient-4.8.8.0/embyclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 00:17:00.000000 embyclient-4.8.8.0/embyclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-05-31 00:17:00.000000 embyclient-4.8.8.0/embyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:17:00.000000 embyclient-4.8.8.0/embyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 00:17:00.000000 embyclient-4.8.8.0/embyclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 00:17:00.000000 embyclient-4.8.8.0/embyclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:17:01.019743 embyclient-4.8.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-31 00:16:52.000000 embyclient-4.8.8.0/setup.py
```

### Comparing `embyclient-4.8.7.0/PKG-INFO` & `embyclient-4.8.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embyclient
-Version: 4.8.7.0
+Version: 4.8.8.0
 Summary: A Python client for Emby Media Server's API
 Home-page: https://emby.media
 Keywords: Emby,Rest,API,client,media,server,JSON
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia
```

### Comparing `embyclient-4.8.7.0/README.md` & `embyclient-4.8.8.0/README.md`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/__init__.py` & `embyclient-4.8.8.0/embyclient/__init__.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/api_client.py` & `embyclient-4.8.8.0/embyclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = '/4.8.7.0/python'
+        self.user_agent = '/4.8.8.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `embyclient-4.8.7.0/embyclient/configuration.py` & `embyclient-4.8.8.0/embyclient/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,10 +234,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.8.7.0\n"\
-               "SDK Package Version: 4.8.7.0".\
+               "Version of the API: 4.8.8.0\n"\
+               "SDK Package Version: 4.8.8.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `embyclient-4.8.7.0/embyclient/models/__init__.py` & `embyclient-4.8.8.0/embyclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/access_schedule.py` & `embyclient-4.8.8.0/embyclient/models/access_schedule.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/actions_postback_action.py` & `embyclient-4.8.8.0/embyclient/models/actions_postback_action.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/activity_log_entry.py` & `embyclient-4.8.8.0/embyclient/models/activity_log_entry.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/album_info.py` & `embyclient-4.8.8.0/embyclient/models/album_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/all_theme_media_result.py` & `embyclient-4.8.8.0/embyclient/models/all_theme_media_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_available_recording_options.py` & `embyclient-4.8.8.0/embyclient/models/api_available_recording_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_base_items_request.py` & `embyclient-4.8.8.0/embyclient/models/api_base_items_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_configuration_page_info.py` & `embyclient-4.8.8.0/embyclient/models/api_configuration_page_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_epg_row.py` & `embyclient-4.8.8.0/embyclient/models/api_epg_row.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_listing_provider_type_info.py` & `embyclient-4.8.8.0/embyclient/models/api_listing_provider_type_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_name_id_description_pair.py` & `embyclient-4.8.8.0/embyclient/models/api_name_id_description_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_on_playback_progress.py` & `embyclient-4.8.8.0/embyclient/models/api_on_playback_progress.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,33 +20,38 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'playlist_index': 'int',
         'playlist_length': 'int',
+        'shuffle': 'bool',
         'event_name': 'ProgressEvent'
     }
 
     attribute_map = {
         'playlist_index': 'PlaylistIndex',
         'playlist_length': 'PlaylistLength',
+        'shuffle': 'Shuffle',
         'event_name': 'EventName'
     }
 
-    def __init__(self, playlist_index=None, playlist_length=None, event_name=None):  # noqa: E501
+    def __init__(self, playlist_index=None, playlist_length=None, shuffle=None, event_name=None):  # noqa: E501
         """ApiOnPlaybackProgress - a model defined in Swagger"""  # noqa: E501
         self._playlist_index = None
         self._playlist_length = None
+        self._shuffle = None
         self._event_name = None
         self.discriminator = None
         if playlist_index is not None:
             self.playlist_index = playlist_index
         if playlist_length is not None:
             self.playlist_length = playlist_length
+        if shuffle is not None:
+            self.shuffle = shuffle
         if event_name is not None:
             self.event_name = event_name
 
     @property
     def playlist_index(self):
         """Gets the playlist_index of this ApiOnPlaybackProgress.  # noqa: E501
 
@@ -85,14 +90,35 @@
         :param playlist_length: The playlist_length of this ApiOnPlaybackProgress.  # noqa: E501
         :type: int
         """
 
         self._playlist_length = playlist_length
 
     @property
+    def shuffle(self):
+        """Gets the shuffle of this ApiOnPlaybackProgress.  # noqa: E501
+
+
+        :return: The shuffle of this ApiOnPlaybackProgress.  # noqa: E501
+        :rtype: bool
+        """
+        return self._shuffle
+
+    @shuffle.setter
+    def shuffle(self, shuffle):
+        """Sets the shuffle of this ApiOnPlaybackProgress.
+
+
+        :param shuffle: The shuffle of this ApiOnPlaybackProgress.  # noqa: E501
+        :type: bool
+        """
+
+        self._shuffle = shuffle
+
+    @property
     def event_name(self):
         """Gets the event_name of this ApiOnPlaybackProgress.  # noqa: E501
 
 
         :return: The event_name of this ApiOnPlaybackProgress.  # noqa: E501
         :rtype: ProgressEvent
         """
```

### Comparing `embyclient-4.8.7.0/embyclient/models/api_set_channel_disabled.py` & `embyclient-4.8.8.0/embyclient/models/api_set_channel_disabled.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_set_channel_mapping.py` & `embyclient-4.8.8.0/embyclient/models/api_set_channel_mapping.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_set_channel_sort_index.py` & `embyclient-4.8.8.0/embyclient/models/api_set_channel_sort_index.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/api_tag_item.py` & `embyclient-4.8.8.0/embyclient/models/api_tag_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/artist_info.py` & `embyclient-4.8.8.0/embyclient/models/artist_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/attributes_simple_condition.py` & `embyclient-4.8.8.0/embyclient/models/attributes_simple_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/attributes_value_condition.py` & `embyclient-4.8.8.0/embyclient/models/attributes_value_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/authenticate_user.py` & `embyclient-4.8.8.0/embyclient/models/authenticate_user.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/authenticate_user_by_name.py` & `embyclient-4.8.8.0/embyclient/models/authenticate_user_by_name.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/authentication_authentication_result.py` & `embyclient-4.8.8.0/embyclient/models/authentication_authentication_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/base_item_dto.py` & `embyclient-4.8.8.0/embyclient/models/base_item_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/base_item_person.py` & `embyclient-4.8.8.0/embyclient/models/base_item_person.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/bit_rate.py` & `embyclient-4.8.8.0/embyclient/models/bit_rate.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/book_info.py` & `embyclient-4.8.8.0/embyclient/models/book_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/branding_branding_options.py` & `embyclient-4.8.8.0/embyclient/models/branding_branding_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/channel_management_info.py` & `embyclient-4.8.8.0/embyclient/models/channel_management_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/chapter_info.py` & `embyclient-4.8.8.0/embyclient/models/chapter_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/client_capabilities.py` & `embyclient-4.8.8.0/embyclient/models/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/codec_configuration.py` & `embyclient-4.8.8.0/embyclient/models/codec_configuration.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/codec_directions.py` & `embyclient-4.8.8.0/embyclient/models/codec_directions.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/codec_kinds.py` & `embyclient-4.8.8.0/embyclient/models/codec_kinds.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/codec_profile.py` & `embyclient-4.8.8.0/embyclient/models/codec_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/codec_type.py` & `embyclient-4.8.8.0/embyclient/models/codec_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/collections_collection_creation_result.py` & `embyclient-4.8.8.0/embyclient/models/collections_collection_creation_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/color_formats.py` & `embyclient-4.8.8.0/embyclient/models/color_formats.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/common_editor_types.py` & `embyclient-4.8.8.0/embyclient/models/common_editor_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py` & `embyclient-4.8.8.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/common_interfaces_i_codec_device_info.py` & `embyclient-4.8.8.0/embyclient/models/common_interfaces_i_codec_device_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/common_plugins_i_plugin.py` & `embyclient-4.8.8.0/embyclient/models/common_plugins_i_plugin.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/conditions_property_condition.py` & `embyclient-4.8.8.0/embyclient/models/conditions_property_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/conditions_property_condition_type.py` & `embyclient-4.8.8.0/embyclient/models/conditions_property_condition_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py` & `embyclient-4.8.8.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/connect_connect_authentication_exchange_result.py` & `embyclient-4.8.8.0/embyclient/models/connect_connect_authentication_exchange_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/connect_user_link_result.py` & `embyclient-4.8.8.0/embyclient/models/connect_user_link_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/connect_user_link_type.py` & `embyclient-4.8.8.0/embyclient/models/connect_user_link_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/container_profile.py` & `embyclient-4.8.8.0/embyclient/models/container_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/create_user_by_name.py` & `embyclient-4.8.8.0/embyclient/models/create_user_by_name.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/day_of_week.py` & `embyclient-4.8.8.0/embyclient/models/day_of_week.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/default_directory_browser_info.py` & `embyclient-4.8.8.0/embyclient/models/default_directory_browser_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/device_profile.py` & `embyclient-4.8.8.0/embyclient/models/device_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/devices_content_upload_history.py` & `embyclient-4.8.8.0/embyclient/models/devices_content_upload_history.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/devices_device_info.py` & `embyclient-4.8.8.0/embyclient/models/devices_device_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/devices_device_options.py` & `embyclient-4.8.8.0/embyclient/models/devices_device_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/devices_local_file_info.py` & `embyclient-4.8.8.0/embyclient/models/devices_local_file_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/direct_play_profile.py` & `embyclient-4.8.8.0/embyclient/models/direct_play_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/display_preferences.py` & `embyclient-4.8.8.0/embyclient/models/display_preferences.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/dlna_profile_type.py` & `embyclient-4.8.8.0/embyclient/models/dlna_profile_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/dlna_profiles_device_identification.py` & `embyclient-4.8.8.0/embyclient/models/dlna_profiles_device_identification.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/dlna_profiles_device_profile_type.py` & `embyclient-4.8.8.0/embyclient/models/dlna_profiles_device_profile_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/dlna_profiles_dlna_profile.py` & `embyclient-4.8.8.0/embyclient/models/dlna_profiles_dlna_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/dlna_profiles_header_match_type.py` & `embyclient-4.8.8.0/embyclient/models/dlna_profiles_header_match_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/dlna_profiles_http_header_info.py` & `embyclient-4.8.8.0/embyclient/models/dlna_profiles_http_header_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/dlna_profiles_protocol_info_detection.py` & `embyclient-4.8.8.0/embyclient/models/dlna_profiles_protocol_info_detection.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/drawing_image_orientation.py` & `embyclient-4.8.8.0/embyclient/models/drawing_image_orientation.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/dynamic_day_of_week.py` & `embyclient-4.8.8.0/embyclient/models/dynamic_day_of_week.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/edit_object_container.py` & `embyclient-4.8.8.0/embyclient/models/edit_object_container.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/editors_editor_base.py` & `embyclient-4.8.8.0/embyclient/models/editors_editor_base.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/editors_editor_button_item.py` & `embyclient-4.8.8.0/embyclient/models/editors_editor_button_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/editors_editor_root.py` & `embyclient-4.8.8.0/embyclient/models/editors_editor_root.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/encoding_context.py` & `embyclient-4.8.8.0/embyclient/models/encoding_context.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/enums_ui_command_type.py` & `embyclient-4.8.8.0/embyclient/models/enums_ui_command_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/enums_ui_view_type.py` & `embyclient-4.8.8.0/embyclient/models/enums_ui_view_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/extended_video_sub_types.py` & `embyclient-4.8.8.0/embyclient/models/extended_video_sub_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/extended_video_types.py` & `embyclient-4.8.8.0/embyclient/models/extended_video_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/external_id_info.py` & `embyclient-4.8.8.0/embyclient/models/external_id_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/external_url.py` & `embyclient-4.8.8.0/embyclient/models/external_url.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/feature_info.py` & `embyclient-4.8.8.0/embyclient/models/feature_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/feature_type.py` & `embyclient-4.8.8.0/embyclient/models/feature_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/forgot_password.py` & `embyclient-4.8.8.0/embyclient/models/forgot_password.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/forgot_password_action.py` & `embyclient-4.8.8.0/embyclient/models/forgot_password_action.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/forgot_password_pin.py` & `embyclient-4.8.8.0/embyclient/models/forgot_password_pin.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/forgot_password_result.py` & `embyclient-4.8.8.0/embyclient/models/forgot_password_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/game_info.py` & `embyclient-4.8.8.0/embyclient/models/game_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/general_command.py` & `embyclient-4.8.8.0/embyclient/models/general_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/generic_edit_i_edit_object_container.py` & `embyclient-4.8.8.0/embyclient/models/generic_edit_i_edit_object_container.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/get_directory_contents.py` & `embyclient-4.8.8.0/embyclient/models/get_directory_contents.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/globalization_country_info.py` & `embyclient-4.8.8.0/embyclient/models/globalization_country_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/globalization_culture_dto.py` & `embyclient-4.8.8.0/embyclient/models/globalization_culture_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/globalization_localizaton_option.py` & `embyclient-4.8.8.0/embyclient/models/globalization_localizaton_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/image_info.py` & `embyclient-4.8.8.0/embyclient/models/image_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/image_option.py` & `embyclient-4.8.8.0/embyclient/models/image_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/image_provider_info.py` & `embyclient-4.8.8.0/embyclient/models/image_provider_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/image_saving_convention.py` & `embyclient-4.8.8.0/embyclient/models/image_saving_convention.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/image_type.py` & `embyclient-4.8.8.0/embyclient/models/image_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/installation_info.py` & `embyclient-4.8.8.0/embyclient/models/installation_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/io_file_system_entry_info.py` & `embyclient-4.8.8.0/embyclient/models/io_file_system_entry_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/io_file_system_entry_type.py` & `embyclient-4.8.8.0/embyclient/models/io_file_system_entry_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/item_counts.py` & `embyclient-4.8.8.0/embyclient/models/item_counts.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/item_file_info.py` & `embyclient-4.8.8.0/embyclient/models/item_file_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/item_file_type.py` & `embyclient-4.8.8.0/embyclient/models/item_file_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/item_lookup_info.py` & `embyclient-4.8.8.0/embyclient/models/item_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/level_information.py` & `embyclient-4.8.8.0/embyclient/models/level_information.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_add_media_path.py` & `embyclient-4.8.8.0/embyclient/models/library_add_media_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_add_virtual_folder.py` & `embyclient-4.8.8.0/embyclient/models/library_add_virtual_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_delete_info.py` & `embyclient-4.8.8.0/embyclient/models/library_delete_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_item_link_type.py` & `embyclient-4.8.8.0/embyclient/models/library_item_link_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_library_option_info.py` & `embyclient-4.8.8.0/embyclient/models/library_library_option_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_library_options_result.py` & `embyclient-4.8.8.0/embyclient/models/library_library_options_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_library_type_options.py` & `embyclient-4.8.8.0/embyclient/models/library_library_type_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_media_folder.py` & `embyclient-4.8.8.0/embyclient/models/library_media_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_media_update_info.py` & `embyclient-4.8.8.0/embyclient/models/library_media_update_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_options.py` & `embyclient-4.8.8.0/embyclient/models/library_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_post_updated_media.py` & `embyclient-4.8.8.0/embyclient/models/library_post_updated_media.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_remove_media_path.py` & `embyclient-4.8.8.0/embyclient/models/library_remove_media_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_remove_virtual_folder.py` & `embyclient-4.8.8.0/embyclient/models/library_remove_virtual_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_rename_virtual_folder.py` & `embyclient-4.8.8.0/embyclient/models/library_rename_virtual_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_sub_folder.py` & `embyclient-4.8.8.0/embyclient/models/library_sub_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_update_library_options.py` & `embyclient-4.8.8.0/embyclient/models/library_update_library_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_update_media_path.py` & `embyclient-4.8.8.0/embyclient/models/library_update_media_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/library_user_copy_options.py` & `embyclient-4.8.8.0/embyclient/models/library_user_copy_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_stream_request.py` & `embyclient-4.8.8.0/embyclient/models/live_stream_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_stream_response.py` & `embyclient-4.8.8.0/embyclient/models/live_stream_response.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_channel_type.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_channel_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_guide_info.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_guide_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_keep_until.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_keep_until.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_keyword_info.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_keyword_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_keyword_type.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_keyword_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_listings_provider_info.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_listings_provider_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_live_tv_info.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_live_tv_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_recording_status.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_recording_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_series_timer_info.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_series_timer_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_series_timer_info_dto.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_series_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_timer_info_dto.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_timer_type.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_timer_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/live_tv_tuner_host_info.py` & `embyclient-4.8.8.0/embyclient/models/live_tv_tuner_host_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/location_type.py` & `embyclient-4.8.8.0/embyclient/models/location_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/log_file.py` & `embyclient-4.8.8.0/embyclient/models/log_file.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/logging_log_severity.py` & `embyclient-4.8.8.0/embyclient/models/logging_log_severity.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/marker_type.py` & `embyclient-4.8.8.0/embyclient/models/marker_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/mb_backup_api_all_backups_info.py` & `embyclient-4.8.8.0/embyclient/models/mb_backup_api_all_backups_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/mb_backup_api_data_restore_options.py` & `embyclient-4.8.8.0/embyclient/models/mb_backup_api_data_restore_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/mb_backup_api_restore_options.py` & `embyclient-4.8.8.0/embyclient/models/mb_backup_api_restore_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/mb_backup_api_user_restore_info.py` & `embyclient-4.8.8.0/embyclient/models/mb_backup_api_user_restore_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/mb_backup_backup_info.py` & `embyclient-4.8.8.0/embyclient/models/mb_backup_backup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/media_encoding_codec_parameter_context.py` & `embyclient-4.8.8.0/embyclient/models/media_encoding_codec_parameter_context.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/media_path_info.py` & `embyclient-4.8.8.0/embyclient/models/media_path_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/media_protocol.py` & `embyclient-4.8.8.0/embyclient/models/media_protocol.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/media_source_info.py` & `embyclient-4.8.8.0/embyclient/models/media_source_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/media_source_type.py` & `embyclient-4.8.8.0/embyclient/models/media_source_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/media_stream.py` & `embyclient-4.8.8.0/embyclient/models/media_stream.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/media_stream_type.py` & `embyclient-4.8.8.0/embyclient/models/media_stream_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/media_url.py` & `embyclient-4.8.8.0/embyclient/models/media_url.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/metadata_editor_info.py` & `embyclient-4.8.8.0/embyclient/models/metadata_editor_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/metadata_features.py` & `embyclient-4.8.8.0/embyclient/models/metadata_features.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/metadata_fields.py` & `embyclient-4.8.8.0/embyclient/models/metadata_fields.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/metadata_refresh_mode.py` & `embyclient-4.8.8.0/embyclient/models/metadata_refresh_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/movie_info.py` & `embyclient-4.8.8.0/embyclient/models/movie_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/music_video_info.py` & `embyclient-4.8.8.0/embyclient/models/music_video_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/name_id_pair.py` & `embyclient-4.8.8.0/embyclient/models/name_id_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/name_long_id_pair.py` & `embyclient-4.8.8.0/embyclient/models/name_long_id_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/name_value_pair.py` & `embyclient-4.8.8.0/embyclient/models/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/net_end_point_info.py` & `embyclient-4.8.8.0/embyclient/models/net_end_point_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/net_sockets_address_family.py` & `embyclient-4.8.8.0/embyclient/models/net_sockets_address_family.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/notification_category_info.py` & `embyclient-4.8.8.0/embyclient/models/notification_category_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/notification_type_info.py` & `embyclient-4.8.8.0/embyclient/models/notification_type_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/operating_system.py` & `embyclient-4.8.8.0/embyclient/models/operating_system.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/package_info.py` & `embyclient-4.8.8.0/embyclient/models/package_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/package_target_system.py` & `embyclient-4.8.8.0/embyclient/models/package_target_system.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/package_version_class.py` & `embyclient-4.8.8.0/embyclient/models/package_version_class.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/package_version_info.py` & `embyclient-4.8.8.0/embyclient/models/package_version_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/parental_rating.py` & `embyclient-4.8.8.0/embyclient/models/parental_rating.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/path_substitution.py` & `embyclient-4.8.8.0/embyclient/models/path_substitution.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/persistence_intro_debug_info.py` & `embyclient-4.8.8.0/embyclient/models/persistence_intro_debug_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/person_lookup_info.py` & `embyclient-4.8.8.0/embyclient/models/person_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/person_type.py` & `embyclient-4.8.8.0/embyclient/models/person_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/pin_redeem_result.py` & `embyclient-4.8.8.0/embyclient/models/pin_redeem_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/play_command.py` & `embyclient-4.8.8.0/embyclient/models/play_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/play_method.py` & `embyclient-4.8.8.0/embyclient/models/play_method.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/play_request.py` & `embyclient-4.8.8.0/embyclient/models/play_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/playback_error_code.py` & `embyclient-4.8.8.0/embyclient/models/playback_error_code.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/playback_info_request.py` & `embyclient-4.8.8.0/embyclient/models/playback_info_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/playback_info_response.py` & `embyclient-4.8.8.0/embyclient/models/playback_info_response.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/playback_progress_info.py` & `embyclient-4.8.8.0/embyclient/models/playback_progress_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         'brightness': 'int',
         'aspect_ratio': 'str',
         'event_name': 'ProgressEvent',
         'play_method': 'PlayMethod',
         'live_stream_id': 'str',
         'play_session_id': 'str',
         'repeat_mode': 'RepeatMode',
+        'shuffle': 'bool',
         'subtitle_offset': 'int',
         'playback_rate': 'float',
         'playlist_item_ids': 'list[str]'
     }
 
     attribute_map = {
         'can_seek': 'CanSeek',
@@ -72,20 +73,21 @@
         'brightness': 'Brightness',
         'aspect_ratio': 'AspectRatio',
         'event_name': 'EventName',
         'play_method': 'PlayMethod',
         'live_stream_id': 'LiveStreamId',
         'play_session_id': 'PlaySessionId',
         'repeat_mode': 'RepeatMode',
+        'shuffle': 'Shuffle',
         'subtitle_offset': 'SubtitleOffset',
         'playback_rate': 'PlaybackRate',
         'playlist_item_ids': 'PlaylistItemIds'
     }
 
-    def __init__(self, can_seek=None, item=None, now_playing_queue=None, playlist_item_id=None, item_id=None, session_id=None, media_source_id=None, audio_stream_index=None, subtitle_stream_index=None, is_paused=None, playlist_index=None, playlist_length=None, is_muted=None, position_ticks=None, run_time_ticks=None, playback_start_time_ticks=None, volume_level=None, brightness=None, aspect_ratio=None, event_name=None, play_method=None, live_stream_id=None, play_session_id=None, repeat_mode=None, subtitle_offset=None, playback_rate=None, playlist_item_ids=None):  # noqa: E501
+    def __init__(self, can_seek=None, item=None, now_playing_queue=None, playlist_item_id=None, item_id=None, session_id=None, media_source_id=None, audio_stream_index=None, subtitle_stream_index=None, is_paused=None, playlist_index=None, playlist_length=None, is_muted=None, position_ticks=None, run_time_ticks=None, playback_start_time_ticks=None, volume_level=None, brightness=None, aspect_ratio=None, event_name=None, play_method=None, live_stream_id=None, play_session_id=None, repeat_mode=None, shuffle=None, subtitle_offset=None, playback_rate=None, playlist_item_ids=None):  # noqa: E501
         """PlaybackProgressInfo - a model defined in Swagger"""  # noqa: E501
         self._can_seek = None
         self._item = None
         self._now_playing_queue = None
         self._playlist_item_id = None
         self._item_id = None
         self._session_id = None
@@ -103,14 +105,15 @@
         self._brightness = None
         self._aspect_ratio = None
         self._event_name = None
         self._play_method = None
         self._live_stream_id = None
         self._play_session_id = None
         self._repeat_mode = None
+        self._shuffle = None
         self._subtitle_offset = None
         self._playback_rate = None
         self._playlist_item_ids = None
         self.discriminator = None
         if can_seek is not None:
             self.can_seek = can_seek
         if item is not None:
@@ -155,14 +158,16 @@
             self.play_method = play_method
         if live_stream_id is not None:
             self.live_stream_id = live_stream_id
         if play_session_id is not None:
             self.play_session_id = play_session_id
         if repeat_mode is not None:
             self.repeat_mode = repeat_mode
+        if shuffle is not None:
+            self.shuffle = shuffle
         if subtitle_offset is not None:
             self.subtitle_offset = subtitle_offset
         if playback_rate is not None:
             self.playback_rate = playback_rate
         if playlist_item_ids is not None:
             self.playlist_item_ids = playlist_item_ids
 
@@ -691,14 +696,35 @@
         :param repeat_mode: The repeat_mode of this PlaybackProgressInfo.  # noqa: E501
         :type: RepeatMode
         """
 
         self._repeat_mode = repeat_mode
 
     @property
+    def shuffle(self):
+        """Gets the shuffle of this PlaybackProgressInfo.  # noqa: E501
+
+
+        :return: The shuffle of this PlaybackProgressInfo.  # noqa: E501
+        :rtype: bool
+        """
+        return self._shuffle
+
+    @shuffle.setter
+    def shuffle(self, shuffle):
+        """Sets the shuffle of this PlaybackProgressInfo.
+
+
+        :param shuffle: The shuffle of this PlaybackProgressInfo.  # noqa: E501
+        :type: bool
+        """
+
+        self._shuffle = shuffle
+
+    @property
     def subtitle_offset(self):
         """Gets the subtitle_offset of this PlaybackProgressInfo.  # noqa: E501
 
 
         :return: The subtitle_offset of this PlaybackProgressInfo.  # noqa: E501
         :rtype: int
         """
```

### Comparing `embyclient-4.8.7.0/embyclient/models/playback_start_info.py` & `embyclient-4.8.8.0/embyclient/models/playback_start_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         'brightness': 'int',
         'aspect_ratio': 'str',
         'event_name': 'ProgressEvent',
         'play_method': 'PlayMethod',
         'live_stream_id': 'str',
         'play_session_id': 'str',
         'repeat_mode': 'RepeatMode',
+        'shuffle': 'bool',
         'subtitle_offset': 'int',
         'playback_rate': 'float',
         'playlist_item_ids': 'list[str]'
     }
 
     attribute_map = {
         'can_seek': 'CanSeek',
@@ -72,20 +73,21 @@
         'brightness': 'Brightness',
         'aspect_ratio': 'AspectRatio',
         'event_name': 'EventName',
         'play_method': 'PlayMethod',
         'live_stream_id': 'LiveStreamId',
         'play_session_id': 'PlaySessionId',
         'repeat_mode': 'RepeatMode',
+        'shuffle': 'Shuffle',
         'subtitle_offset': 'SubtitleOffset',
         'playback_rate': 'PlaybackRate',
         'playlist_item_ids': 'PlaylistItemIds'
     }
 
-    def __init__(self, can_seek=None, item=None, now_playing_queue=None, playlist_item_id=None, item_id=None, session_id=None, media_source_id=None, audio_stream_index=None, subtitle_stream_index=None, is_paused=None, playlist_index=None, playlist_length=None, is_muted=None, position_ticks=None, run_time_ticks=None, playback_start_time_ticks=None, volume_level=None, brightness=None, aspect_ratio=None, event_name=None, play_method=None, live_stream_id=None, play_session_id=None, repeat_mode=None, subtitle_offset=None, playback_rate=None, playlist_item_ids=None):  # noqa: E501
+    def __init__(self, can_seek=None, item=None, now_playing_queue=None, playlist_item_id=None, item_id=None, session_id=None, media_source_id=None, audio_stream_index=None, subtitle_stream_index=None, is_paused=None, playlist_index=None, playlist_length=None, is_muted=None, position_ticks=None, run_time_ticks=None, playback_start_time_ticks=None, volume_level=None, brightness=None, aspect_ratio=None, event_name=None, play_method=None, live_stream_id=None, play_session_id=None, repeat_mode=None, shuffle=None, subtitle_offset=None, playback_rate=None, playlist_item_ids=None):  # noqa: E501
         """PlaybackStartInfo - a model defined in Swagger"""  # noqa: E501
         self._can_seek = None
         self._item = None
         self._now_playing_queue = None
         self._playlist_item_id = None
         self._item_id = None
         self._session_id = None
@@ -103,14 +105,15 @@
         self._brightness = None
         self._aspect_ratio = None
         self._event_name = None
         self._play_method = None
         self._live_stream_id = None
         self._play_session_id = None
         self._repeat_mode = None
+        self._shuffle = None
         self._subtitle_offset = None
         self._playback_rate = None
         self._playlist_item_ids = None
         self.discriminator = None
         if can_seek is not None:
             self.can_seek = can_seek
         if item is not None:
@@ -155,14 +158,16 @@
             self.play_method = play_method
         if live_stream_id is not None:
             self.live_stream_id = live_stream_id
         if play_session_id is not None:
             self.play_session_id = play_session_id
         if repeat_mode is not None:
             self.repeat_mode = repeat_mode
+        if shuffle is not None:
+            self.shuffle = shuffle
         if subtitle_offset is not None:
             self.subtitle_offset = subtitle_offset
         if playback_rate is not None:
             self.playback_rate = playback_rate
         if playlist_item_ids is not None:
             self.playlist_item_ids = playlist_item_ids
 
@@ -691,14 +696,35 @@
         :param repeat_mode: The repeat_mode of this PlaybackStartInfo.  # noqa: E501
         :type: RepeatMode
         """
 
         self._repeat_mode = repeat_mode
 
     @property
+    def shuffle(self):
+        """Gets the shuffle of this PlaybackStartInfo.  # noqa: E501
+
+
+        :return: The shuffle of this PlaybackStartInfo.  # noqa: E501
+        :rtype: bool
+        """
+        return self._shuffle
+
+    @shuffle.setter
+    def shuffle(self, shuffle):
+        """Sets the shuffle of this PlaybackStartInfo.
+
+
+        :param shuffle: The shuffle of this PlaybackStartInfo.  # noqa: E501
+        :type: bool
+        """
+
+        self._shuffle = shuffle
+
+    @property
     def subtitle_offset(self):
         """Gets the subtitle_offset of this PlaybackStartInfo.  # noqa: E501
 
 
         :return: The subtitle_offset of this PlaybackStartInfo.  # noqa: E501
         :rtype: int
         """
```

### Comparing `embyclient-4.8.7.0/embyclient/models/playback_stop_info.py` & `embyclient-4.8.8.0/embyclient/models/playback_stop_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/player_state_info.py` & `embyclient-4.8.8.0/embyclient/models/player_state_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         'volume_level': 'int',
         'audio_stream_index': 'int',
         'subtitle_stream_index': 'int',
         'media_source_id': 'str',
         'play_method': 'PlayMethod',
         'repeat_mode': 'RepeatMode',
         'subtitle_offset': 'int',
+        'shuffle': 'bool',
         'playback_rate': 'float'
     }
 
     attribute_map = {
         'position_ticks': 'PositionTicks',
         'can_seek': 'CanSeek',
         'is_paused': 'IsPaused',
@@ -44,30 +45,32 @@
         'volume_level': 'VolumeLevel',
         'audio_stream_index': 'AudioStreamIndex',
         'subtitle_stream_index': 'SubtitleStreamIndex',
         'media_source_id': 'MediaSourceId',
         'play_method': 'PlayMethod',
         'repeat_mode': 'RepeatMode',
         'subtitle_offset': 'SubtitleOffset',
+        'shuffle': 'Shuffle',
         'playback_rate': 'PlaybackRate'
     }
 
-    def __init__(self, position_ticks=None, can_seek=None, is_paused=None, is_muted=None, volume_level=None, audio_stream_index=None, subtitle_stream_index=None, media_source_id=None, play_method=None, repeat_mode=None, subtitle_offset=None, playback_rate=None):  # noqa: E501
+    def __init__(self, position_ticks=None, can_seek=None, is_paused=None, is_muted=None, volume_level=None, audio_stream_index=None, subtitle_stream_index=None, media_source_id=None, play_method=None, repeat_mode=None, subtitle_offset=None, shuffle=None, playback_rate=None):  # noqa: E501
         """PlayerStateInfo - a model defined in Swagger"""  # noqa: E501
         self._position_ticks = None
         self._can_seek = None
         self._is_paused = None
         self._is_muted = None
         self._volume_level = None
         self._audio_stream_index = None
         self._subtitle_stream_index = None
         self._media_source_id = None
         self._play_method = None
         self._repeat_mode = None
         self._subtitle_offset = None
+        self._shuffle = None
         self._playback_rate = None
         self.discriminator = None
         if position_ticks is not None:
             self.position_ticks = position_ticks
         if can_seek is not None:
             self.can_seek = can_seek
         if is_paused is not None:
@@ -84,14 +87,16 @@
             self.media_source_id = media_source_id
         if play_method is not None:
             self.play_method = play_method
         if repeat_mode is not None:
             self.repeat_mode = repeat_mode
         if subtitle_offset is not None:
             self.subtitle_offset = subtitle_offset
+        if shuffle is not None:
+            self.shuffle = shuffle
         if playback_rate is not None:
             self.playback_rate = playback_rate
 
     @property
     def position_ticks(self):
         """Gets the position_ticks of this PlayerStateInfo.  # noqa: E501
 
@@ -335,14 +340,35 @@
         :param subtitle_offset: The subtitle_offset of this PlayerStateInfo.  # noqa: E501
         :type: int
         """
 
         self._subtitle_offset = subtitle_offset
 
     @property
+    def shuffle(self):
+        """Gets the shuffle of this PlayerStateInfo.  # noqa: E501
+
+
+        :return: The shuffle of this PlayerStateInfo.  # noqa: E501
+        :rtype: bool
+        """
+        return self._shuffle
+
+    @shuffle.setter
+    def shuffle(self, shuffle):
+        """Sets the shuffle of this PlayerStateInfo.
+
+
+        :param shuffle: The shuffle of this PlayerStateInfo.  # noqa: E501
+        :type: bool
+        """
+
+        self._shuffle = shuffle
+
+    @property
     def playback_rate(self):
         """Gets the playback_rate of this PlayerStateInfo.  # noqa: E501
 
 
         :return: The playback_rate of this PlayerStateInfo.  # noqa: E501
         :rtype: float
         """
```

### Comparing `embyclient-4.8.7.0/embyclient/models/playlists_add_to_playlist_result.py` & `embyclient-4.8.8.0/embyclient/models/playlists_add_to_playlist_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/playlists_playlist_creation_result.py` & `embyclient-4.8.8.0/embyclient/models/playlists_playlist_creation_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/playstate_command.py` & `embyclient-4.8.8.0/embyclient/models/playstate_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/playstate_request.py` & `embyclient-4.8.8.0/embyclient/models/playstate_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/plugins_configuration_page_type.py` & `embyclient-4.8.8.0/embyclient/models/plugins_configuration_page_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/plugins_plugin_info.py` & `embyclient-4.8.8.0/embyclient/models/plugins_plugin_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/process_run_metrics_process_metric_point.py` & `embyclient-4.8.8.0/embyclient/models/process_run_metrics_process_metric_point.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/process_run_metrics_process_statistics.py` & `embyclient-4.8.8.0/embyclient/models/process_run_metrics_process_statistics.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/profile_condition.py` & `embyclient-4.8.8.0/embyclient/models/profile_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/profile_condition_type.py` & `embyclient-4.8.8.0/embyclient/models/profile_condition_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/profile_condition_value.py` & `embyclient-4.8.8.0/embyclient/models/profile_condition_value.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/profile_information.py` & `embyclient-4.8.8.0/embyclient/models/profile_information.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/profile_level_information.py` & `embyclient-4.8.8.0/embyclient/models/profile_level_information.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/progress_event.py` & `embyclient-4.8.8.0/embyclient/models/progress_event.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     PLAYLISTITEMMOVE = "PlaylistItemMove"
     PLAYLISTITEMREMOVE = "PlaylistItemRemove"
     PLAYLISTITEMADD = "PlaylistItemAdd"
     QUALITYCHANGE = "QualityChange"
     STATECHANGE = "StateChange"
     SUBTITLEOFFSETCHANGE = "SubtitleOffsetChange"
     PLAYBACKRATECHANGE = "PlaybackRateChange"
+    SHUFFLECHANGE = "ShuffleChange"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `embyclient-4.8.7.0/embyclient/models/provider_id_dictionary.py` & `embyclient-4.8.8.0/embyclient/models/provider_id_dictionary.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/proxy_header_mode.py` & `embyclient-4.8.8.0/embyclient/models/proxy_header_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/public_system_info.py` & `embyclient-4.8.8.0/embyclient/models/public_system_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_activity_log_entry.py` & `embyclient-4.8.8.0/embyclient/models/query_result_activity_log_entry.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_api_epg_row.py` & `embyclient-4.8.8.0/embyclient/models/query_result_api_epg_row.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_base_item_dto.py` & `embyclient-4.8.8.0/embyclient/models/query_result_base_item_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_channel_management_info.py` & `embyclient-4.8.8.0/embyclient/models/query_result_channel_management_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_devices_device_info.py` & `embyclient-4.8.8.0/embyclient/models/query_result_devices_device_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py` & `embyclient-4.8.8.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_live_tv_timer_info_dto.py` & `embyclient-4.8.8.0/embyclient/models/query_result_live_tv_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_log_file.py` & `embyclient-4.8.8.0/embyclient/models/query_result_log_file.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_string.py` & `embyclient-4.8.8.0/embyclient/models/query_result_string.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_sync_job.py` & `embyclient-4.8.8.0/embyclient/models/query_result_sync_job.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_sync_job_item.py` & `embyclient-4.8.8.0/embyclient/models/query_result_sync_job_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_user_dto.py` & `embyclient-4.8.8.0/embyclient/models/query_result_user_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_user_library_official_rating_item.py` & `embyclient-4.8.8.0/embyclient/models/query_result_user_library_official_rating_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_user_library_tag_item.py` & `embyclient-4.8.8.0/embyclient/models/query_result_user_library_tag_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/query_result_virtual_folder_info.py` & `embyclient-4.8.8.0/embyclient/models/query_result_virtual_folder_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/queue_item.py` & `embyclient-4.8.8.0/embyclient/models/queue_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/rating_type.py` & `embyclient-4.8.8.0/embyclient/models/rating_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/recommendation_dto.py` & `embyclient-4.8.8.0/embyclient/models/recommendation_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/recommendation_type.py` & `embyclient-4.8.8.0/embyclient/models/recommendation_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_image_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_image_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_image_result.py` & `embyclient-4.8.8.0/embyclient/models/remote_image_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_album_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_album_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_artist_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_artist_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_book_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_book_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_game_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_game_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_item_lookup_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_item_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_movie_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_movie_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_music_video_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_music_video_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_person_lookup_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_person_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_series_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_series_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_query_trailer_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_query_trailer_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_search_result.py` & `embyclient-4.8.8.0/embyclient/models/remote_search_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/remote_subtitle_info.py` & `embyclient-4.8.8.0/embyclient/models/remote_subtitle_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/repeat_mode.py` & `embyclient-4.8.8.0/embyclient/models/repeat_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/resolution.py` & `embyclient-4.8.8.0/embyclient/models/resolution.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/resolution_with_rate.py` & `embyclient-4.8.8.0/embyclient/models/resolution_with_rate.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/response_profile.py` & `embyclient-4.8.8.0/embyclient/models/response_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/roku_metadata_api_thumbnail_info.py` & `embyclient-4.8.8.0/embyclient/models/roku_metadata_api_thumbnail_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py` & `embyclient-4.8.8.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/run_ui_command.py` & `embyclient-4.8.8.0/embyclient/models/run_ui_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/secondary_frameworks.py` & `embyclient-4.8.8.0/embyclient/models/secondary_frameworks.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/segment_skip_mode.py` & `embyclient-4.8.8.0/embyclient/models/segment_skip_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/series_display_order.py` & `embyclient-4.8.8.0/embyclient/models/series_display_order.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/series_info.py` & `embyclient-4.8.8.0/embyclient/models/series_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/server_configuration.py` & `embyclient-4.8.8.0/embyclient/models/server_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         'enable_sq_lite_mmio': 'bool',
         'playlists_upgraded_to_m3_u': 'bool',
         'image_extractor_upgraded1': 'bool',
         'enable_people_letter_sub_folders': 'bool',
         'optimize_database_on_shutdown': 'bool',
         'database_analysis_limit': 'int',
         'disable_async_io': 'bool',
-        'migrated_to_user_item_shares7': 'bool',
+        'migrated_to_user_item_shares8': 'bool',
         'migrated_library_options_to_db': 'bool',
         'allow_legacy_local_network_password': 'bool',
         'enable_saved_metadata_for_people': 'bool',
         'tv_channels_refreshed': 'bool',
         'proxy_header_mode': 'ProxyHeaderMode',
         'enable_debug_level_logging': 'bool',
         'revert_debug_logging': 'str',
@@ -134,30 +134,30 @@
         'enable_sq_lite_mmio': 'EnableSqLiteMmio',
         'playlists_upgraded_to_m3_u': 'PlaylistsUpgradedToM3U',
         'image_extractor_upgraded1': 'ImageExtractorUpgraded1',
         'enable_people_letter_sub_folders': 'EnablePeopleLetterSubFolders',
         'optimize_database_on_shutdown': 'OptimizeDatabaseOnShutdown',
         'database_analysis_limit': 'DatabaseAnalysisLimit',
         'disable_async_io': 'DisableAsyncIO',
-        'migrated_to_user_item_shares7': 'MigratedToUserItemShares7',
+        'migrated_to_user_item_shares8': 'MigratedToUserItemShares8',
         'migrated_library_options_to_db': 'MigratedLibraryOptionsToDb',
         'allow_legacy_local_network_password': 'AllowLegacyLocalNetworkPassword',
         'enable_saved_metadata_for_people': 'EnableSavedMetadataForPeople',
         'tv_channels_refreshed': 'TvChannelsRefreshed',
         'proxy_header_mode': 'ProxyHeaderMode',
         'enable_debug_level_logging': 'EnableDebugLevelLogging',
         'revert_debug_logging': 'RevertDebugLogging',
         'enable_auto_update': 'EnableAutoUpdate',
         'log_file_retention_days': 'LogFileRetentionDays',
         'run_at_startup': 'RunAtStartup',
         'is_startup_wizard_completed': 'IsStartupWizardCompleted',
         'cache_path': 'CachePath'
     }
 
-    def __init__(self, enable_u_pn_p=None, public_port=None, public_https_port=None, http_server_port_number=None, https_port_number=None, enable_https=None, certificate_path=None, certificate_password=None, is_port_authorized=None, auto_run_web_app=None, enable_remote_access=None, log_all_query_times=None, enable_case_sensitive_item_ids=None, metadata_path=None, metadata_network_path=None, preferred_metadata_language=None, metadata_country_code=None, sort_remove_words=None, library_monitor_delay_seconds=None, enable_dashboard_response_caching=None, dashboard_source_path=None, image_saving_convention=None, enable_automatic_restart=None, server_name=None, preferred_detected_remote_address_family=None, wan_ddns=None, ui_culture=None, remote_client_bitrate_limit=None, local_network_subnets=None, local_network_addresses=None, enable_external_content_in_suggestions=None, require_https=None, is_behind_proxy=None, remote_ip_filter=None, is_remote_ip_filter_blacklist=None, image_extraction_timeout_ms=None, path_substitutions=None, uninstalled_plugins=None, collapse_video_folders=None, enable_original_track_titles=None, vacuum_database_on_startup=None, simultaneous_stream_limit=None, database_cache_size_mb=None, enable_sq_lite_mmio=None, playlists_upgraded_to_m3_u=None, image_extractor_upgraded1=None, enable_people_letter_sub_folders=None, optimize_database_on_shutdown=None, database_analysis_limit=None, disable_async_io=None, migrated_to_user_item_shares7=None, migrated_library_options_to_db=None, allow_legacy_local_network_password=None, enable_saved_metadata_for_people=None, tv_channels_refreshed=None, proxy_header_mode=None, enable_debug_level_logging=None, revert_debug_logging=None, enable_auto_update=None, log_file_retention_days=None, run_at_startup=None, is_startup_wizard_completed=None, cache_path=None):  # noqa: E501
+    def __init__(self, enable_u_pn_p=None, public_port=None, public_https_port=None, http_server_port_number=None, https_port_number=None, enable_https=None, certificate_path=None, certificate_password=None, is_port_authorized=None, auto_run_web_app=None, enable_remote_access=None, log_all_query_times=None, enable_case_sensitive_item_ids=None, metadata_path=None, metadata_network_path=None, preferred_metadata_language=None, metadata_country_code=None, sort_remove_words=None, library_monitor_delay_seconds=None, enable_dashboard_response_caching=None, dashboard_source_path=None, image_saving_convention=None, enable_automatic_restart=None, server_name=None, preferred_detected_remote_address_family=None, wan_ddns=None, ui_culture=None, remote_client_bitrate_limit=None, local_network_subnets=None, local_network_addresses=None, enable_external_content_in_suggestions=None, require_https=None, is_behind_proxy=None, remote_ip_filter=None, is_remote_ip_filter_blacklist=None, image_extraction_timeout_ms=None, path_substitutions=None, uninstalled_plugins=None, collapse_video_folders=None, enable_original_track_titles=None, vacuum_database_on_startup=None, simultaneous_stream_limit=None, database_cache_size_mb=None, enable_sq_lite_mmio=None, playlists_upgraded_to_m3_u=None, image_extractor_upgraded1=None, enable_people_letter_sub_folders=None, optimize_database_on_shutdown=None, database_analysis_limit=None, disable_async_io=None, migrated_to_user_item_shares8=None, migrated_library_options_to_db=None, allow_legacy_local_network_password=None, enable_saved_metadata_for_people=None, tv_channels_refreshed=None, proxy_header_mode=None, enable_debug_level_logging=None, revert_debug_logging=None, enable_auto_update=None, log_file_retention_days=None, run_at_startup=None, is_startup_wizard_completed=None, cache_path=None):  # noqa: E501
         """ServerConfiguration - a model defined in Swagger"""  # noqa: E501
         self._enable_u_pn_p = None
         self._public_port = None
         self._public_https_port = None
         self._http_server_port_number = None
         self._https_port_number = None
         self._enable_https = None
@@ -201,15 +201,15 @@
         self._enable_sq_lite_mmio = None
         self._playlists_upgraded_to_m3_u = None
         self._image_extractor_upgraded1 = None
         self._enable_people_letter_sub_folders = None
         self._optimize_database_on_shutdown = None
         self._database_analysis_limit = None
         self._disable_async_io = None
-        self._migrated_to_user_item_shares7 = None
+        self._migrated_to_user_item_shares8 = None
         self._migrated_library_options_to_db = None
         self._allow_legacy_local_network_password = None
         self._enable_saved_metadata_for_people = None
         self._tv_channels_refreshed = None
         self._proxy_header_mode = None
         self._enable_debug_level_logging = None
         self._revert_debug_logging = None
@@ -315,16 +315,16 @@
             self.enable_people_letter_sub_folders = enable_people_letter_sub_folders
         if optimize_database_on_shutdown is not None:
             self.optimize_database_on_shutdown = optimize_database_on_shutdown
         if database_analysis_limit is not None:
             self.database_analysis_limit = database_analysis_limit
         if disable_async_io is not None:
             self.disable_async_io = disable_async_io
-        if migrated_to_user_item_shares7 is not None:
-            self.migrated_to_user_item_shares7 = migrated_to_user_item_shares7
+        if migrated_to_user_item_shares8 is not None:
+            self.migrated_to_user_item_shares8 = migrated_to_user_item_shares8
         if migrated_library_options_to_db is not None:
             self.migrated_library_options_to_db = migrated_library_options_to_db
         if allow_legacy_local_network_password is not None:
             self.allow_legacy_local_network_password = allow_legacy_local_network_password
         if enable_saved_metadata_for_people is not None:
             self.enable_saved_metadata_for_people = enable_saved_metadata_for_people
         if tv_channels_refreshed is not None:
@@ -1425,33 +1425,33 @@
         :param disable_async_io: The disable_async_io of this ServerConfiguration.  # noqa: E501
         :type: bool
         """
 
         self._disable_async_io = disable_async_io
 
     @property
-    def migrated_to_user_item_shares7(self):
-        """Gets the migrated_to_user_item_shares7 of this ServerConfiguration.  # noqa: E501
+    def migrated_to_user_item_shares8(self):
+        """Gets the migrated_to_user_item_shares8 of this ServerConfiguration.  # noqa: E501
 
 
-        :return: The migrated_to_user_item_shares7 of this ServerConfiguration.  # noqa: E501
+        :return: The migrated_to_user_item_shares8 of this ServerConfiguration.  # noqa: E501
         :rtype: bool
         """
-        return self._migrated_to_user_item_shares7
+        return self._migrated_to_user_item_shares8
 
-    @migrated_to_user_item_shares7.setter
-    def migrated_to_user_item_shares7(self, migrated_to_user_item_shares7):
-        """Sets the migrated_to_user_item_shares7 of this ServerConfiguration.
+    @migrated_to_user_item_shares8.setter
+    def migrated_to_user_item_shares8(self, migrated_to_user_item_shares8):
+        """Sets the migrated_to_user_item_shares8 of this ServerConfiguration.
 
 
-        :param migrated_to_user_item_shares7: The migrated_to_user_item_shares7 of this ServerConfiguration.  # noqa: E501
+        :param migrated_to_user_item_shares8: The migrated_to_user_item_shares8 of this ServerConfiguration.  # noqa: E501
         :type: bool
         """
 
-        self._migrated_to_user_item_shares7 = migrated_to_user_item_shares7
+        self._migrated_to_user_item_shares8 = migrated_to_user_item_shares8
 
     @property
     def migrated_library_options_to_db(self):
         """Gets the migrated_library_options_to_db of this ServerConfiguration.  # noqa: E501
 
 
         :return: The migrated_library_options_to_db of this ServerConfiguration.  # noqa: E501
```

### Comparing `embyclient-4.8.7.0/embyclient/models/session_session_info.py` & `embyclient-4.8.8.0/embyclient/models/session_session_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/session_user_info.py` & `embyclient-4.8.8.0/embyclient/models/session_user_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/song_info.py` & `embyclient-4.8.8.0/embyclient/models/song_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sort_order.py` & `embyclient-4.8.8.0/embyclient/models/sort_order.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/subtitle_delivery_method.py` & `embyclient-4.8.8.0/embyclient/models/subtitle_delivery_method.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/subtitle_location_type.py` & `embyclient-4.8.8.0/embyclient/models/subtitle_location_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/subtitle_playback_mode.py` & `embyclient-4.8.8.0/embyclient/models/subtitle_playback_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/subtitle_profile.py` & `embyclient-4.8.8.0/embyclient/models/subtitle_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/subtitles_subtitle_download_result.py` & `embyclient-4.8.8.0/embyclient/models/subtitles_subtitle_download_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_category.py` & `embyclient-4.8.8.0/embyclient/models/sync_category.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_data_request.py` & `embyclient-4.8.8.0/embyclient/models/sync_data_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_data_response.py` & `embyclient-4.8.8.0/embyclient/models/sync_data_response.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_dialog_options.py` & `embyclient-4.8.8.0/embyclient/models/sync_dialog_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_job.py` & `embyclient-4.8.8.0/embyclient/models/sync_job.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_job_creation_result.py` & `embyclient-4.8.8.0/embyclient/models/sync_job_creation_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_job_item.py` & `embyclient-4.8.8.0/embyclient/models/sync_job_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_job_item_status.py` & `embyclient-4.8.8.0/embyclient/models/sync_job_item_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_job_option.py` & `embyclient-4.8.8.0/embyclient/models/sync_job_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_job_request.py` & `embyclient-4.8.8.0/embyclient/models/sync_job_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_job_status.py` & `embyclient-4.8.8.0/embyclient/models/sync_job_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_profile_option.py` & `embyclient-4.8.8.0/embyclient/models/sync_profile_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_quality_option.py` & `embyclient-4.8.8.0/embyclient/models/sync_quality_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/sync_target.py` & `embyclient-4.8.8.0/embyclient/models/sync_target.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/synced_item.py` & `embyclient-4.8.8.0/embyclient/models/synced_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/synced_item_progress.py` & `embyclient-4.8.8.0/embyclient/models/synced_item_progress.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/system_event.py` & `embyclient-4.8.8.0/embyclient/models/system_event.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/system_info.py` & `embyclient-4.8.8.0/embyclient/models/system_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/task_completion_status.py` & `embyclient-4.8.8.0/embyclient/models/task_completion_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/task_info.py` & `embyclient-4.8.8.0/embyclient/models/task_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/task_result.py` & `embyclient-4.8.8.0/embyclient/models/task_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/task_state.py` & `embyclient-4.8.8.0/embyclient/models/task_state.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/task_trigger_info.py` & `embyclient-4.8.8.0/embyclient/models/task_trigger_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/theme_media_result.py` & `embyclient-4.8.8.0/embyclient/models/theme_media_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/trailer_info.py` & `embyclient-4.8.8.0/embyclient/models/trailer_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/transcode_reason.py` & `embyclient-4.8.8.0/embyclient/models/transcode_reason.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/transcode_seek_info.py` & `embyclient-4.8.8.0/embyclient/models/transcode_seek_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/transcoding_info.py` & `embyclient-4.8.8.0/embyclient/models/transcoding_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/transcoding_profile.py` & `embyclient-4.8.8.0/embyclient/models/transcoding_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/transcoding_vp_step_info.py` & `embyclient-4.8.8.0/embyclient/models/transcoding_vp_step_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/transcoding_vp_step_types.py` & `embyclient-4.8.8.0/embyclient/models/transcoding_vp_step_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/transport_stream_timestamp.py` & `embyclient-4.8.8.0/embyclient/models/transport_stream_timestamp.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/tuple_double_double.py` & `embyclient-4.8.8.0/embyclient/models/tuple_double_double.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/type_options.py` & `embyclient-4.8.8.0/embyclient/models/type_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/ui_command.py` & `embyclient-4.8.8.0/embyclient/models/ui_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/ui_tab_page_info.py` & `embyclient-4.8.8.0/embyclient/models/ui_tab_page_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/ui_view_info.py` & `embyclient-4.8.8.0/embyclient/models/ui_view_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/unrated_item.py` & `embyclient-4.8.8.0/embyclient/models/unrated_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/update_user_password.py` & `embyclient-4.8.8.0/embyclient/models/update_user_password.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_action.py` & `embyclient-4.8.8.0/embyclient/models/user_action.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_action_type.py` & `embyclient-4.8.8.0/embyclient/models/user_action_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_configuration.py` & `embyclient-4.8.8.0/embyclient/models/user_configuration.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_dto.py` & `embyclient-4.8.8.0/embyclient/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_item_data_dto.py` & `embyclient-4.8.8.0/embyclient/models/user_item_data_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_item_share_level.py` & `embyclient-4.8.8.0/embyclient/models/user_item_share_level.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_library_add_tags.py` & `embyclient-4.8.8.0/embyclient/models/user_library_add_tags.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_library_leave_shared_items.py` & `embyclient-4.8.8.0/embyclient/models/user_library_leave_shared_items.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_library_official_rating_item.py` & `embyclient-4.8.8.0/embyclient/models/user_library_official_rating_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_library_remove_tags.py` & `embyclient-4.8.8.0/embyclient/models/user_library_remove_tags.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_library_tag_item.py` & `embyclient-4.8.8.0/embyclient/models/user_library_tag_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_library_update_user_item_access.py` & `embyclient-4.8.8.0/embyclient/models/user_library_update_user_item_access.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_notification_info.py` & `embyclient-4.8.8.0/embyclient/models/user_notification_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/user_policy.py` & `embyclient-4.8.8.0/embyclient/models/user_policy.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/validate_path.py` & `embyclient-4.8.8.0/embyclient/models/validate_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/version.py` & `embyclient-4.8.8.0/embyclient/models/version.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/video3_d_format.py` & `embyclient-4.8.8.0/embyclient/models/video3_d_format.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/video_codec_base.py` & `embyclient-4.8.8.0/embyclient/models/video_codec_base.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/video_media_types.py` & `embyclient-4.8.8.0/embyclient/models/video_media_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/virtual_folder_info.py` & `embyclient-4.8.8.0/embyclient/models/virtual_folder_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/models/wake_on_lan_info.py` & `embyclient-4.8.8.0/embyclient/models/wake_on_lan_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient/rest.py` & `embyclient-4.8.8.0/embyclient/rest.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/embyclient.egg-info/PKG-INFO` & `embyclient-4.8.8.0/embyclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embyclient
-Version: 4.8.7.0
+Version: 4.8.8.0
 Summary: A Python client for Emby Media Server's API
 Home-page: https://emby.media
 Keywords: Emby,Rest,API,client,media,server,JSON
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia
```

### Comparing `embyclient-4.8.7.0/embyclient.egg-info/SOURCES.txt` & `embyclient-4.8.8.0/embyclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.7.0/setup.py` & `embyclient-4.8.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
-VERSION = "4.8.7.0"
+VERSION = "4.8.8.0"
 REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
 
 
 classifiers = [
     'Intended Audience :: Developers',  # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'Topic :: Multimedia :: Video',
```

