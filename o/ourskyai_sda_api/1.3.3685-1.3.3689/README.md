# Comparing `tmp/ourskyai_sda_api-1.3.3685.tar.gz` & `tmp/ourskyai_sda_api-1.3.3689.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_sda_api-1.3.3685.tar", max compression
+gzip compressed data, was "ourskyai_sda_api-1.3.3689.tar", max compression
```

## Comparing `ourskyai_sda_api-1.3.3685.tar` & `ourskyai_sda_api-1.3.3689.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    10151 2024-05-29 22:34:23.829472 ourskyai_sda_api-1.3.3685/README.md
--rw-r--r--   0        0        0     5222 2024-05-29 22:34:26.669480 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/__init__.py
--rw-r--r--   0        0        0      104 2024-05-29 22:34:26.705480 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/api/__init__.py
--rw-r--r--   0        0        0   220784 2024-05-29 22:34:26.809480 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/api/default_api.py
--rw-r--r--   0        0        0    30830 2024-05-29 22:34:26.845480 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-29 22:34:26.881481 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/api_response.py
--rw-r--r--   0        0        0    15175 2024-05-29 22:34:26.945481 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/configuration.py
--rw-r--r--   0        0        0     5923 2024-05-29 22:34:27.001481 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/exceptions.py
--rw-r--r--   0        0        0     4601 2024-05-29 22:34:27.037481 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/__init__.py
--rw-r--r--   0        0        0     4311 2024-05-29 22:34:27.069481 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/astrometric_offsets.py
--rw-r--r--   0        0        0     2394 2024-05-29 22:34:27.193482 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/empty_success.py
--rw-r--r--   0        0        0     1676 2024-05-29 22:34:27.257482 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/filter_type.py
--rw-r--r--   0        0        0     2420 2024-05-29 22:34:27.313482 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/fits_header.py
--rw-r--r--   0        0        0     2645 2024-05-29 22:34:27.377482 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/location.py
--rw-r--r--   0        0        0     1237 2024-05-29 22:34:27.429482 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/mount_type.py
--rw-r--r--   0        0        0     2756 2024-05-29 22:34:27.473482 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/observation_bounding_box.py
--rw-r--r--   0        0        0     3713 2024-05-29 22:34:27.577483 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/observation_quality.py
--rw-r--r--   0        0        0     6381 2024-05-29 22:34:27.629483 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/observation_result.py
--rw-r--r--   0        0        0     1320 2024-05-29 22:34:27.677483 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/observation_state.py
--rw-r--r--   0        0        0     1529 2024-05-29 22:34:27.725484 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/orbit_type.py
--rw-r--r--   0        0        0     1361 2024-05-29 22:34:27.765484 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/satellite_target_tracking_status.py
--rw-r--r--   0        0        0     1241 2024-05-29 22:34:27.813484 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/shutter_type.py
--rw-r--r--   0        0        0     2382 2024-05-29 22:34:27.845484 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/successful_create.py
--rw-r--r--   0        0        0     1258 2024-05-29 22:34:27.893484 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/tracking_type.py
--rw-r--r--   0        0        0     2534 2024-05-29 22:34:27.961484 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2605 2024-05-29 22:34:28.021484 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     3169 2024-05-29 22:34:28.073485 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2609 2024-05-29 22:34:28.113485 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_organization_target_request.py
--rw-r--r--   0        0        0     2761 2024-05-29 22:34:28.165485 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_satellite_target_request.py
--rw-r--r--   0        0        0     3373 2024-05-29 22:34:28.241485 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_search_instruction_request.py
--rw-r--r--   0        0        0     3353 2024-05-29 22:34:28.285485 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
--rw-r--r--   0        0        0     3017 2024-05-29 22:34:28.341486 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
--rw-r--r--   0        0        0     4457 2024-05-29 22:34:28.389486 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3922 2024-05-29 22:34:28.441486 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_image_set.py
--rw-r--r--   0        0        0     6285 2024-05-29 22:34:28.501486 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     4676 2024-05-29 22:34:28.541486 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_observation_feature.py
--rw-r--r--   0        0        0     3748 2024-05-29 22:34:28.601487 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_observation_sequence_result.py
--rw-r--r--   0        0        0     4306 2024-05-29 22:34:28.661487 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
--rw-r--r--   0        0        0     4637 2024-05-29 22:34:28.725487 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_observation_status.py
--rw-r--r--   0        0        0     3192 2024-05-29 22:34:28.817487 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_organization_target.py
--rw-r--r--   0        0        0     3644 2024-05-29 22:34:28.853488 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_satellite_potential.py
--rw-r--r--   0        0        0     3528 2024-05-29 22:34:28.889488 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_satellite_target.py
--rw-r--r--   0        0        0     3733 2024-05-29 22:34:28.949488 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_search_instruction.py
--rw-r--r--   0        0        0     3407 2024-05-29 22:34:29.009488 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_search_instruction_step.py
--rw-r--r--   0        0        0     3634 2024-05-29 22:34:29.073488 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_survey_instruction.py
--rw-r--r--   0        0        0     2799 2024-05-29 22:34:29.173489 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_survey_instruction_step.py
--rw-r--r--   0        0        0     3716 2024-05-29 22:34:29.237489 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_target_correlation.py
--rw-r--r--   0        0        0     3185 2024-05-29 22:34:29.293489 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_tdm.py
--rw-r--r--   0        0        0     2575 2024-05-29 22:34:29.405490 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_update_email_configuration_request.py
--rw-r--r--   0        0        0     2913 2024-05-29 22:34:29.449490 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_update_satellite_target_request.py
--rw-r--r--   0        0        0     3146 2024-05-29 22:34:29.501490 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
--rw-r--r--   0        0        0     2963 2024-05-29 22:34:29.581490 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_webhook_configuration.py
--rw-r--r--   0        0        0     1386 2024-05-29 22:34:29.621490 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/weather_condition.py
--rw-r--r--   0        0        0     1350 2024-05-29 22:34:29.661490 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/webhook_auth_type.py
--rw-r--r--   0        0        0     1734 2024-05-29 22:34:29.705490 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/webhook_event.py
--rw-r--r--   0        0        0        0 2024-05-29 22:34:29.733491 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/py.typed
--rw-r--r--   0        0        0    13423 2024-05-29 22:34:29.773491 ourskyai_sda_api-1.3.3685/ourskyai_sda_api/rest.py
--rw-r--r--   0        0        0      731 2024-05-29 22:34:29.865491 ourskyai_sda_api-1.3.3685/pyproject.toml
--rw-r--r--   0        0        0    11113 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3685/PKG-INFO
+-rw-r--r--   0        0        0    10151 2024-05-30 16:20:53.181807 ourskyai_sda_api-1.3.3689/README.md
+-rw-r--r--   0        0        0     5222 2024-05-30 16:20:55.777752 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-30 16:20:55.805751 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/api/__init__.py
+-rw-r--r--   0        0        0   220784 2024-05-30 16:20:55.897750 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/api/default_api.py
+-rw-r--r--   0        0        0    30830 2024-05-30 16:20:55.953748 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-30 16:20:55.989748 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/api_response.py
+-rw-r--r--   0        0        0    15175 2024-05-30 16:20:56.089745 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/configuration.py
+-rw-r--r--   0        0        0     5923 2024-05-30 16:20:56.133745 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/exceptions.py
+-rw-r--r--   0        0        0     4601 2024-05-30 16:20:56.189743 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/__init__.py
+-rw-r--r--   0        0        0     4311 2024-05-30 16:20:56.241742 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/astrometric_offsets.py
+-rw-r--r--   0        0        0     2394 2024-05-30 16:20:56.317741 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/empty_success.py
+-rw-r--r--   0        0        0     1676 2024-05-30 16:20:56.361740 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/filter_type.py
+-rw-r--r--   0        0        0     2420 2024-05-30 16:20:56.417739 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/fits_header.py
+-rw-r--r--   0        0        0     2645 2024-05-30 16:20:56.465737 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/location.py
+-rw-r--r--   0        0        0     1237 2024-05-30 16:20:56.509737 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/mount_type.py
+-rw-r--r--   0        0        0     2756 2024-05-30 16:20:56.553736 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/observation_bounding_box.py
+-rw-r--r--   0        0        0     3713 2024-05-30 16:20:56.593735 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/observation_quality.py
+-rw-r--r--   0        0        0     6381 2024-05-30 16:20:56.665733 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/observation_result.py
+-rw-r--r--   0        0        0     1320 2024-05-30 16:20:56.709732 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/observation_state.py
+-rw-r--r--   0        0        0     1529 2024-05-30 16:20:56.809730 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/orbit_type.py
+-rw-r--r--   0        0        0     1361 2024-05-30 16:20:56.857729 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/satellite_target_tracking_status.py
+-rw-r--r--   0        0        0     1241 2024-05-30 16:20:56.961727 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/shutter_type.py
+-rw-r--r--   0        0        0     2382 2024-05-30 16:20:57.013726 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/successful_create.py
+-rw-r--r--   0        0        0     1258 2024-05-30 16:20:57.041725 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2534 2024-05-30 16:20:57.081725 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2605 2024-05-30 16:20:57.129723 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     3169 2024-05-30 16:20:57.181722 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2609 2024-05-30 16:20:57.301720 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_organization_target_request.py
+-rw-r--r--   0        0        0     2761 2024-05-30 16:20:57.353719 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_satellite_target_request.py
+-rw-r--r--   0        0        0     3373 2024-05-30 16:20:57.393718 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_search_instruction_request.py
+-rw-r--r--   0        0        0     3353 2024-05-30 16:20:57.433717 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
+-rw-r--r--   0        0        0     3017 2024-05-30 16:20:57.485716 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
+-rw-r--r--   0        0        0     4457 2024-05-30 16:20:57.533715 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3922 2024-05-30 16:20:57.625713 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     6285 2024-05-30 16:20:57.717711 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     4676 2024-05-30 16:20:57.765710 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_observation_feature.py
+-rw-r--r--   0        0        0     3748 2024-05-30 16:20:57.833709 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_observation_sequence_result.py
+-rw-r--r--   0        0        0     4306 2024-05-30 16:20:57.877708 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
+-rw-r--r--   0        0        0     4637 2024-05-30 16:20:57.929707 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_observation_status.py
+-rw-r--r--   0        0        0     3192 2024-05-30 16:20:57.977706 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_organization_target.py
+-rw-r--r--   0        0        0     3644 2024-05-30 16:20:58.029704 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_satellite_potential.py
+-rw-r--r--   0        0        0     3528 2024-05-30 16:20:58.077703 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_satellite_target.py
+-rw-r--r--   0        0        0     3733 2024-05-30 16:20:58.117703 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_search_instruction.py
+-rw-r--r--   0        0        0     3407 2024-05-30 16:20:58.233700 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_search_instruction_step.py
+-rw-r--r--   0        0        0     3634 2024-05-30 16:20:58.297699 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_survey_instruction.py
+-rw-r--r--   0        0        0     2799 2024-05-30 16:20:58.397697 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_survey_instruction_step.py
+-rw-r--r--   0        0        0     3716 2024-05-30 16:20:58.441696 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_target_correlation.py
+-rw-r--r--   0        0        0     3185 2024-05-30 16:20:58.497695 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_tdm.py
+-rw-r--r--   0        0        0     2575 2024-05-30 16:20:58.537694 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_update_email_configuration_request.py
+-rw-r--r--   0        0        0     2913 2024-05-30 16:20:58.625692 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_update_satellite_target_request.py
+-rw-r--r--   0        0        0     3146 2024-05-30 16:20:58.693690 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
+-rw-r--r--   0        0        0     2963 2024-05-30 16:20:58.737690 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_webhook_configuration.py
+-rw-r--r--   0        0        0     1386 2024-05-30 16:20:58.773689 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/weather_condition.py
+-rw-r--r--   0        0        0     1350 2024-05-30 16:20:58.837687 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/webhook_auth_type.py
+-rw-r--r--   0        0        0     1734 2024-05-30 16:20:58.897686 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/webhook_event.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:20:58.921686 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/py.typed
+-rw-r--r--   0        0        0    13423 2024-05-30 16:20:58.973684 ourskyai_sda_api-1.3.3689/ourskyai_sda_api/rest.py
+-rw-r--r--   0        0        0      731 2024-05-30 16:20:59.025683 ourskyai_sda_api-1.3.3689/pyproject.toml
+-rw-r--r--   0        0        0    11113 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3689/PKG-INFO
```

### Comparing `ourskyai_sda_api-1.3.3685/README.md` & `ourskyai_sda_api-1.3.3689/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3685
-- Package version: 1.3.3685
+- API version: 1.3.3689
+- Package version: 1.3.3689
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/__init__.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3685"
+__version__ = "1.3.3689"
 
 # import apis into sdk package
 from ourskyai_sda_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_sda_api.api_response import ApiResponse
 from ourskyai_sda_api.api_client import ApiClient
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/api/default_api.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/api_client.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3685/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3689/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/api_response.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/configuration.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3685\n"\
-               "SDK Package Version: 1.3.3685".\
+               "Version of the API: 1.3.3689\n"\
+               "SDK Package Version: 1.3.3689".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/exceptions.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/__init__.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/astrometric_offsets.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/astrometric_offsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/empty_success.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/empty_success.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/filter_type.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/fits_header.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/fits_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/location.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/mount_type.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/mount_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/observation_bounding_box.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/observation_bounding_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/observation_quality.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/observation_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/observation_result.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/observation_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/observation_state.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/observation_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/orbit_type.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/orbit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/satellite_target_tracking_status.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/satellite_target_tracking_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/shutter_type.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/shutter_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/successful_create.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/tracking_type.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/tracking_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_image_set_image_request.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_image_set_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_image_set_image_response.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_image_set_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_image_set_request.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_organization_target_request.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_organization_target_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_satellite_target_request.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_satellite_target_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_search_instruction_request.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_search_instruction_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_create_survey_instruction_request.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_create_survey_instruction_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_get_satellite_targets_response.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_get_satellite_targets_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_ground_station_participant.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_ground_station_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_image_set.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_image_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_image_set_image.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_observation_feature.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_observation_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_observation_sequence_result.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_observation_sequence_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_observation_status.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_observation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_organization_target.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_organization_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_satellite_potential.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_satellite_potential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_satellite_target.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_satellite_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_search_instruction.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_search_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_search_instruction_step.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_search_instruction_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_survey_instruction.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_survey_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_survey_instruction_step.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_survey_instruction_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_target_correlation.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_target_correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_tdm.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_tdm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_update_email_configuration_request.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_update_email_configuration_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_update_satellite_target_request.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_update_satellite_target_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/v1_webhook_configuration.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/v1_webhook_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/weather_condition.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/weather_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/webhook_auth_type.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/webhook_auth_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/models/webhook_event.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/models/webhook_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3685/ourskyai_sda_api/rest.py` & `ourskyai_sda_api-1.3.3689/ourskyai_sda_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3685
+    The version of the OpenAPI document: 1.3.3689
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_sda_api-1.3.3685/pyproject.toml` & `ourskyai_sda_api-1.3.3689/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_sda_api"
-version = "1.3.3685"
+version = "1.3.3689"
 description = "OurSky SDA"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky SDA"]
 include = ["ourskyai_sda_api/py.typed"]
```

### Comparing `ourskyai_sda_api-1.3.3685/PKG-INFO` & `ourskyai_sda_api-1.3.3689/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_sda_api
-Version: 1.3.3685
+Version: 1.3.3689
 Summary: OurSky SDA
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky SDA
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -27,16 +27,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3685
-- Package version: 1.3.3685
+- API version: 1.3.3689
+- Package version: 1.3.3689
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

