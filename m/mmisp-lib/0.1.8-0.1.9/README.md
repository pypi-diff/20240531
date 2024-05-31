# Comparing `tmp/mmisp_lib-0.1.8.tar.gz` & `tmp/mmisp_lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmisp_lib-0.1.8.tar", last modified: Tue May 21 16:03:27 2024, max compression
+gzip compressed data, was "mmisp_lib-0.1.9.tar", last modified: Wed May 22 23:00:03 2024, max compression
```

## Comparing `mmisp_lib-0.1.8.tar` & `mmisp_lib-0.1.9.tar`

### file list

```diff
@@ -1,200 +1,201 @@
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.555207 mmisp_lib-0.1.8/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1076 2024-05-14 11:01:09.000000 mmisp_lib-0.1.8/LICENSE
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3098 2024-05-21 16:03:27.555207 mmisp_lib-0.1.8/PKG-INFO
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2050 2024-04-18 07:49:23.000000 mmisp_lib-0.1.8/README.md
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1067 2024-05-21 16:03:02.000000 mmisp_lib-0.1.8/pyproject.toml
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       38 2024-05-21 16:03:27.555207 mmisp_lib-0.1.8/setup.cfg
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.535206 mmisp_lib-0.1.8/src/
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.535206 mmisp_lib-0.1.8/src/mmisp/
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.535206 mmisp_lib-0.1.8/src/mmisp/api_schemas/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/__init__.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.539206 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1147 2024-05-17 07:13:36.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/add_attribute_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      755 2024-05-17 07:13:36.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/add_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      256 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/add_remove_tag_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      135 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/delete_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      226 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/delete_selected_attribute_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      216 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/delete_selected_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      675 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/edit_attribute_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      838 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/edit_attributes_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1163 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/get_all_attributes_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      901 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/get_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1486 2024-05-02 19:26:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      813 2024-05-02 19:26:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/get_describe_types_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      469 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/restore_attribute_reponse.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3225 2024-05-02 19:26:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/search_attributes_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1119 2024-05-02 19:26:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/search_attributes_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.539206 mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      268 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/add_auth_key_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      431 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/add_auth_key_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      207 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/edit_auth_key_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      460 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/edit_auth_key_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      564 2024-05-03 14:59:12.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/search_auth_keys_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      603 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      567 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.539206 mmisp_lib-0.1.8/src/mmisp/api_schemas/authentication/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/authentication/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       97 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/authentication/exchange_token_login_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      102 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/authentication/password_login_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       81 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/authentication/start_login_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      364 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/authentication/start_login_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       80 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/authentication/token_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.539206 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      310 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/FreeTextImportWorkerBody.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      273 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      277 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     5438 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/add_edit_get_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      808 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/add_event_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      236 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/add_remove_tag_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      248 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/delete_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/edit_event_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2143 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/get_all_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      158 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/get_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      926 2024-05-02 10:34:56.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/index_events_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      881 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/index_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      247 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/publish_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1347 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/search_events_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/search_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      249 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/events/unpublish_event_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.539206 mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      190 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/cache_feed_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      924 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/create_feed_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      164 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/enable_disable_feed_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      128 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/fetch_feeds_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1234 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/get_feed_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      126 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/toggle_feed_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      893 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/update_feed_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.543206 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      229 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      179 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      238 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/delete_force_update_import_galaxy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      323 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/export_galaxies_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1139 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/export_galaxies_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      289 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/galaxy_schema.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      421 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/get_all_search_galaxies_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      866 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/get_galaxy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      298 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/import_galaxies_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      514 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/search_galaxies_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.543206 mmisp_lib-0.1.8/src/mmisp/api_schemas/noticelists/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/noticelists/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      237 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/noticelists/get_all_noticelist_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      747 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/noticelists/get_noticelist_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.543206 mmisp_lib-0.1.8/src/mmisp/api_schemas/objects/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/objects/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      535 2024-05-17 07:13:36.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/objects/create_object_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1526 2024-05-17 07:13:36.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/objects/get_object_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1539 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/objects/search_objects_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.543206 mmisp_lib-0.1.8/src/mmisp/api_schemas/organisations/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/organisations/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      583 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/organisations/organisation.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 13:02:52.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/py.typed
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.543206 mmisp_lib-0.1.8/src/mmisp/api_schemas/roles/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/roles/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2980 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/roles/role.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.543206 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      131 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      113 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      130 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      118 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      428 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/create_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      862 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      524 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      140 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/delete_sharing_group_legacy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1443 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1120 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      340 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/sharing_group.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      138 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/sharing_group_org.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      146 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/sharing_group_server.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      357 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/update_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1062 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1084 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.547206 mmisp_lib-0.1.8/src/mmisp/api_schemas/sightings/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sightings/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1487 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sightings/create_sighting_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      589 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/sightings/get_sighting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      230 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/standard_status_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.547206 mmisp_lib-0.1.8/src/mmisp/api_schemas/tags/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/tags/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      392 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/tags/create_tag_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      156 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/tags/delete_tag_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      645 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/tags/get_tag_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      690 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/tags/search_tags_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      369 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/tags/update_tag_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.547206 mmisp_lib-0.1.8/src/mmisp/api_schemas/taxonomies/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/taxonomies/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      566 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      632 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      367 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/taxonomies/get_taxonomy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      676 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.547206 mmisp_lib-0.1.8/src/mmisp/api_schemas/user_settings/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/user_settings/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      301 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/user_settings/get_uid_user_setting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      232 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/user_settings/get_user_settings_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      161 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/user_settings/search_user_setting_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      209 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/user_settings/search_user_setting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       93 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/user_settings/set_user_setting_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/user_settings/set_user_setting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/user_settings/view_user_setting_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.547206 mmisp_lib-0.1.8/src/mmisp/api_schemas/users/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/users/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      910 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/users/user.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/users/users_view_me_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.547206 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      136 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/check_value_warninglists_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/check_value_warninglists_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     7189 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/create_warninglist_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      210 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/delete_warninglist_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      341 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/get_selected_all_warninglists_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      183 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/get_selected_warninglists_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      191 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      204 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      952 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/warninglist_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.551206 mmisp_lib-0.1.8/src/mmisp/db/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      403 2024-05-19 20:40:59.000000 mmisp_lib-0.1.8/src/mmisp/db/all_models.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      322 2024-05-19 11:50:28.000000 mmisp_lib-0.1.8/src/mmisp/db/config.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2848 2024-05-19 11:50:28.000000 mmisp_lib-0.1.8/src/mmisp/db/database.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      495 2024-05-17 07:13:36.000000 mmisp_lib-0.1.8/src/mmisp/db/mixins.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.551206 mmisp_lib-0.1.8/src/mmisp/db/models/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3699 2024-05-17 07:13:36.000000 mmisp_lib-0.1.8/src/mmisp/db/models/attribute.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/auth_key.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2707 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/event.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1498 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/feed.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      858 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/galaxy.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2456 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/galaxy_cluster.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      846 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/identity_provider.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      888 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/noticelist.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1879 2024-05-19 11:50:28.000000 mmisp_lib-0.1.8/src/mmisp/db/models/object.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      989 2024-05-17 07:13:36.000000 mmisp_lib-0.1.8/src/mmisp/db/models/organisation.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1249 2024-05-14 11:01:09.000000 mmisp_lib-0.1.8/src/mmisp/db/models/role.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1495 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/server.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1798 2024-05-17 07:13:36.000000 mmisp_lib-0.1.8/src/mmisp/db/models/sharing_group.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      829 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/sighting.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      752 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/tag.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1434 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/taxonomy.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2068 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/user.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      997 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/user_setting.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1185 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/models/warninglist.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1181 2024-04-18 07:49:24.000000 mmisp_lib-0.1.8/src/mmisp/db/print_changes.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 13:02:52.000000 mmisp_lib-0.1.8/src/mmisp/db/py.typed
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.551206 mmisp_lib-0.1.8/src/mmisp/lib/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-30 12:43:28.000000 mmisp_lib-0.1.8/src/mmisp/lib/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)    53425 2024-05-17 07:13:36.000000 mmisp_lib-0.1.8/src/mmisp/lib/attributes.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2639 2024-05-14 11:01:09.000000 mmisp_lib-0.1.8/src/mmisp/lib/permissions.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 13:02:52.000000 mmisp_lib-0.1.8/src/mmisp/lib/py.typed
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.555207 mmisp_lib-0.1.8/src/mmisp_lib.egg-info/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3098 2024-05-21 16:03:27.000000 mmisp_lib-0.1.8/src/mmisp_lib.egg-info/PKG-INFO
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     8823 2024-05-21 16:03:27.000000 mmisp_lib-0.1.8/src/mmisp_lib.egg-info/SOURCES.txt
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        1 2024-05-21 16:03:27.000000 mmisp_lib-0.1.8/src/mmisp_lib.egg-info/dependency_links.txt
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      420 2024-05-21 16:03:27.000000 mmisp_lib-0.1.8/src/mmisp_lib.egg-info/requires.txt
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        6 2024-05-21 16:03:27.000000 mmisp_lib-0.1.8/src/mmisp_lib.egg-info/top_level.txt
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-21 16:03:27.551206 mmisp_lib-0.1.8/tests/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       42 2024-04-30 12:43:28.000000 mmisp_lib-0.1.8/tests/test_dummy.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.552090 mmisp_lib-0.1.9/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1076 2024-05-14 11:01:09.000000 mmisp_lib-0.1.9/LICENSE
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3098 2024-05-22 23:00:03.552090 mmisp_lib-0.1.9/PKG-INFO
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2050 2024-04-18 07:49:23.000000 mmisp_lib-0.1.9/README.md
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1085 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/pyproject.toml
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       38 2024-05-22 23:00:03.552090 mmisp_lib-0.1.9/setup.cfg
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.532089 mmisp_lib-0.1.9/src/
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.532089 mmisp_lib-0.1.9/src/mmisp/
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.536089 mmisp_lib-0.1.9/src/mmisp/api_schemas/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/__init__.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.536089 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1147 2024-05-17 07:13:36.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/add_attribute_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      755 2024-05-17 07:13:36.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/add_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      256 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/add_remove_tag_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      135 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/delete_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      226 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/delete_selected_attribute_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      216 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/delete_selected_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      675 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/edit_attribute_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      838 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/edit_attributes_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1163 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/get_all_attributes_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      901 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/get_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1486 2024-05-02 19:26:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      813 2024-05-02 19:26:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/get_describe_types_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      469 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/restore_attribute_reponse.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3225 2024-05-02 19:26:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/search_attributes_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1119 2024-05-02 19:26:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/search_attributes_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.536089 mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      268 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/add_auth_key_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      431 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/add_auth_key_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      207 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/edit_auth_key_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      460 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/edit_auth_key_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      550 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/search_auth_keys_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      603 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      567 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.536089 mmisp_lib-0.1.9/src/mmisp/api_schemas/authentication/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/authentication/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       97 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/authentication/exchange_token_login_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      102 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/authentication/password_login_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       81 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/authentication/start_login_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      364 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/authentication/start_login_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       80 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/authentication/token_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.540089 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      310 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/FreeTextImportWorkerBody.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      273 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      277 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     5438 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/add_edit_get_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      808 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/add_event_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      236 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/add_remove_tag_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      248 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/delete_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/edit_event_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2143 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/get_all_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      158 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/get_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      926 2024-05-02 10:34:56.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/index_events_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      881 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/index_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      247 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/publish_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1347 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/search_events_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/search_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      249 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/events/unpublish_event_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.540089 mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      190 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/cache_feed_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      924 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/create_feed_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      164 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/enable_disable_feed_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      128 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/fetch_feeds_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1234 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/get_feed_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      126 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/toggle_feed_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      893 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/update_feed_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.540089 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      229 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      179 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      238 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/delete_force_update_import_galaxy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      323 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/export_galaxies_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1139 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/export_galaxies_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      289 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/galaxy_schema.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      421 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/get_all_search_galaxies_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      866 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/get_galaxy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      298 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/import_galaxies_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      514 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/search_galaxies_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.540089 mmisp_lib-0.1.9/src/mmisp/api_schemas/noticelists/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/noticelists/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      237 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/noticelists/get_all_noticelist_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      788 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/noticelists/get_noticelist_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.540089 mmisp_lib-0.1.9/src/mmisp/api_schemas/objects/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/objects/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      535 2024-05-17 07:13:36.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/objects/create_object_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1526 2024-05-17 07:13:36.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/objects/get_object_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1539 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/objects/search_objects_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.540089 mmisp_lib-0.1.9/src/mmisp/api_schemas/organisations/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/organisations/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      583 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/organisations/organisation.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/py.typed
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.540089 mmisp_lib-0.1.9/src/mmisp/api_schemas/roles/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/roles/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2980 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/roles/role.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.544089 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      131 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      113 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      130 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      118 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      428 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/create_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      862 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      524 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      140 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/delete_sharing_group_legacy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1443 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1120 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      340 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/sharing_group.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      138 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/sharing_group_org.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      146 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/sharing_group_server.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      357 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/update_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1062 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1084 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.544089 mmisp_lib-0.1.9/src/mmisp/api_schemas/sightings/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sightings/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1487 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sightings/create_sighting_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      589 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/sightings/get_sighting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      230 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/standard_status_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.544089 mmisp_lib-0.1.9/src/mmisp/api_schemas/tags/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/tags/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      392 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/tags/create_tag_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      156 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/tags/delete_tag_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      645 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/tags/get_tag_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      690 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/tags/search_tags_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      369 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/tags/update_tag_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.544089 mmisp_lib-0.1.9/src/mmisp/api_schemas/taxonomies/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/taxonomies/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      566 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      632 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      367 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/taxonomies/get_taxonomy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      676 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.544089 mmisp_lib-0.1.9/src/mmisp/api_schemas/user_settings/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/user_settings/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      301 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/user_settings/get_uid_user_setting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      232 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/user_settings/get_user_settings_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      161 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/user_settings/search_user_setting_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      209 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/user_settings/search_user_setting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       93 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/user_settings/set_user_setting_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/user_settings/set_user_setting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/user_settings/view_user_setting_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.544089 mmisp_lib-0.1.9/src/mmisp/api_schemas/users/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/users/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      910 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/users/user.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/users/users_view_me_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.548090 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      136 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/check_value_warninglists_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/check_value_warninglists_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     7238 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/create_warninglist_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      210 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/delete_warninglist_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      341 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/get_selected_all_warninglists_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      183 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/get_selected_warninglists_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      191 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      204 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      952 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/warninglist_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.548090 mmisp_lib-0.1.9/src/mmisp/db/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/db/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      403 2024-05-19 20:40:59.000000 mmisp_lib-0.1.9/src/mmisp/db/all_models.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      322 2024-05-19 11:50:28.000000 mmisp_lib-0.1.9/src/mmisp/db/config.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2848 2024-05-19 11:50:28.000000 mmisp_lib-0.1.9/src/mmisp/db/database.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      495 2024-05-17 07:13:36.000000 mmisp_lib-0.1.9/src/mmisp/db/mixins.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.548090 mmisp_lib-0.1.9/src/mmisp/db/models/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/db/models/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     4231 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/attribute.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1142 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/auth_key.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3439 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/event.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2028 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/feed.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1120 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/galaxy.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3162 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/galaxy_cluster.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1098 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/identity_provider.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1129 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/noticelist.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2422 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/object.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1334 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/organisation.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1358 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/role.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2040 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/server.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1998 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/sharing_group.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1029 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/sighting.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1017 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/tag.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1954 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/taxonomy.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2765 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/user.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1137 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/user_setting.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1527 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/models/warninglist.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      193 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/mypy.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1181 2024-04-18 07:49:24.000000 mmisp_lib-0.1.9/src/mmisp/db/print_changes.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/db/py.typed
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.548090 mmisp_lib-0.1.9/src/mmisp/lib/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-30 12:43:28.000000 mmisp_lib-0.1.9/src/mmisp/lib/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)    53425 2024-05-17 07:13:36.000000 mmisp_lib-0.1.9/src/mmisp/lib/attributes.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2639 2024-05-14 11:01:09.000000 mmisp_lib-0.1.9/src/mmisp/lib/permissions.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 22:58:46.000000 mmisp_lib-0.1.9/src/mmisp/lib/py.typed
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.552090 mmisp_lib-0.1.9/src/mmisp_lib.egg-info/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3098 2024-05-22 23:00:03.000000 mmisp_lib-0.1.9/src/mmisp_lib.egg-info/PKG-INFO
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     8844 2024-05-22 23:00:03.000000 mmisp_lib-0.1.9/src/mmisp_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        1 2024-05-22 23:00:03.000000 mmisp_lib-0.1.9/src/mmisp_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      420 2024-05-22 23:00:03.000000 mmisp_lib-0.1.9/src/mmisp_lib.egg-info/requires.txt
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        6 2024-05-22 23:00:03.000000 mmisp_lib-0.1.9/src/mmisp_lib.egg-info/top_level.txt
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-22 23:00:03.548090 mmisp_lib-0.1.9/tests/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       42 2024-04-30 12:43:28.000000 mmisp_lib-0.1.9/tests/test_dummy.py
```

### Comparing `mmisp_lib-0.1.8/LICENSE` & `mmisp_lib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/PKG-INFO` & `mmisp_lib-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mmisp-lib
-Version: 0.1.8
+Version: 0.1.9
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi==0.104.1
-Requires-Dist: SQLAlchemy[asyncio]==1.4.46
+Requires-Dist: SQLAlchemy[asyncio]~=1.4.46
 Requires-Dist: pydantic==1.10.13
 Requires-Dist: uvicorn==0.24.0.post1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: alembic==1.8.1
 Requires-Dist: aiomysql==0.2.0
 Requires-Dist: aiosqlite==0.20.0
 Requires-Dist: PyJWT==2.8.0
```

### Comparing `mmisp_lib-0.1.8/README.md` & `mmisp_lib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/pyproject.toml` & `mmisp_lib-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "mmisp-lib"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = []
 readme = "README.md"
 requires-python = ">=3.11.0"
 
 
 dependencies = [
   "fastapi==0.104.1",
-  "SQLAlchemy[asyncio]==1.4.46",
+  "SQLAlchemy[asyncio]~=1.4.46",
   "pydantic==1.10.13",
   "uvicorn==0.24.0.post1",
   "python-dotenv==1.0.0",
   "alembic==1.8.1",
   "aiomysql==0.2.0",
   "aiosqlite==0.20.0",
   "PyJWT==2.8.0",
@@ -43,13 +43,15 @@
 "mmisp.api_schemas" = ["py.typed"]
 "mmisp.db" = ["py.typed"]
 
 [tool.ruff]
 fix = true
 line-length = 120
 required-version = ">=0.3.7"
+src = ["src"]
+
+[tool.ruff.lint]
 select = ["E", "F", "W", "I", "ICN", "ANN"]
 ignore = ["ANN002", "ANN003", "ANN401"]
-src = ["src"]
 
 [tool.coverage.run]
 concurrency = ["greenlet", "thread"]
```

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/add_attribute_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/add_attribute_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/add_attribute_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/add_attribute_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/edit_attribute_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/edit_attribute_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/edit_attributes_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/edit_attributes_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/get_all_attributes_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/get_all_attributes_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/get_attribute_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/get_attribute_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/get_describe_types_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/get_describe_types_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/search_attributes_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/search_attributes_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/attributes/search_attributes_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/attributes/search_attributes_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/search_auth_keys_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/events/search_events_body.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,43 @@
-from pydantic import BaseModel, PositiveInt, conint
+from pydantic import BaseModel
 
 
-class SearchAuthKeyBody(BaseModel):
-    page: PositiveInt | None = 1
-    limit: conint(gt=0, lt=500) | None = 25  # type: ignore
-    id: str | None = None
+class SearchEventsBody(BaseModel):
+    returnFormat: str
+    page: int | None = None
+    limit: int | None = None
+    value: str | None = None
+    type: str | None = None
+    category: str | None = None
+    org: str | None = None
+    tags: list[str] | None = None
+    event_tags: list[str] | None = None
+    searchall: str | None = None
+    from_: str | None = None
+    to: str | None = None
+    last: int | None = None
+    eventid: str | None = None
+    withAttachments: bool | None = None
+    sharinggroup: list[str] | None = None
+    metadata: bool | None = None
     uuid: str | None = None
-    authkey_start: str | None = None
-    authkey_end: str | None = None
-    created: str | None = None
-    expiration: str | None = None
-    read_only: bool | None = None
-    user_id: str | None = None
-    comment: str | None = None
-    allowed_ips: str | list[str] | None = None
-    last_used: str | None = None  # deprecated
+    publish_timestamp: str | None = None
+    timestamp: str | None = None
+    published: bool | None = None
+    enforceWarninglist: bool | None = None
+    sgReferenceOnly: bool | None = None
+    requested_attributes: list[str] | None = None
+    includeContext: bool | None = None
+    headerless: bool | None = None
+    includeWarninglistHits: bool | None = None
+    attackGalaxy: str | None = None
+    to_ids: bool | None = None
+    deleted: bool | None = None
+    excludeLocalTags: bool | None = None
+    date: str | None = None
+    includeSightingdb: bool | None = None
+    tag: str | None = None
+    object_relation: str | None = None
+    threat_level_id: str | None = None
+
+    class Config:
+        orm_mode = True
```

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/events/add_edit_get_event_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/events/add_edit_get_event_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/events/add_event_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/events/add_event_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/events/edit_event_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/events/edit_event_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/events/get_all_events_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/events/get_all_events_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/events/index_events_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/events/index_events_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/events/index_events_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/events/index_events_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/events/search_events_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/sightings/create_sighting_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-from pydantic import BaseModel
+from typing import Any
 
+from pydantic import BaseModel, validator
 
-class SearchEventsBody(BaseModel):
-    returnFormat: str
-    page: int | None = None
-    limit: int | None = None
-    value: str | None = None
+
+class SightingFiltersBody(BaseModel):
+    value1: str | None = None
+    value2: str | None = None
     type: str | None = None
     category: str | None = None
-    org: str | None = None
-    tags: list[str] | None = None
-    event_tags: list[str] | None = None
-    searchall: str | None = None
-    from_: str | None = None
+    from_: str | None = None  # 'from' is a reserved word in Python, so an underscore is added
     to: str | None = None
-    last: int | None = None
-    eventid: str | None = None
-    withAttachments: bool | None = None
-    sharinggroup: list[str] | None = None
-    metadata: bool | None = None
-    uuid: str | None = None
-    publish_timestamp: str | None = None
+    last: str | None = None
     timestamp: str | None = None
-    published: bool | None = None
-    enforceWarninglist: bool | None = None
-    sgReferenceOnly: bool | None = None
-    requested_attributes: list[str] | None = None
-    includeContext: bool | None = None
-    headerless: bool | None = None
-    includeWarninglistHits: bool | None = None
-    attackGalaxy: str | None = None
+    event_id: str | None = None
+    uuid: str | None = None
+    attribute_timestamp: str | None = None
     to_ids: bool | None = None
     deleted: bool | None = None
-    excludeLocalTags: bool | None = None
-    date: str | None = None
-    includeSightingdb: bool | None = None
-    tag: str | None = None
-    object_relation: str | None = None
-    threat_level_id: str | None = None
+    event_timestamp: str | None = None
+    eventinfo: str | None = None
+    sharinggroup: list[str] | None = None
+    first_seen: str | None = None
+    last_seen: str | None = None
+    requested_attributes: list[str] | None = None
+    returnFormat: str | None = "json"
+    limit: str | None = "25"
+
+    @validator("limit")
+    def check_limit(cls, value: Any) -> str:  # noqa: ANN101
+        if value is not None:
+            try:
+                limit_int = int(value)
+            except ValueError:
+                raise ValueError("limit must be a valid integer")
+
+            if not 1 <= limit_int <= 500:
+                raise ValueError("limit must be between 1 and 500")
+        return value
+
+
+class SightingCreateBody(BaseModel):
+    values: list[str]
+    source: str | None = None
+    timestamp: str | None = None
+    filters: SightingFiltersBody | None = None
 
     class Config:
         orm_mode = True
```

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/create_feed_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/create_feed_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/get_feed_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/get_feed_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/feeds/update_feed_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/feeds/update_feed_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/export_galaxies_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/export_galaxies_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/get_galaxy_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/get_galaxy_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/galaxies/search_galaxies_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/galaxies/search_galaxies_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/noticelists/get_noticelist_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/noticelists/get_noticelist_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections.abc import Sequence
 from typing import Any
 
 from pydantic import BaseModel
 
 
 class Data(BaseModel):
     scope: str | list[str] | None
@@ -24,15 +25,15 @@
     ref: list[str]
     geographical_area: list[str]
     version: str
     enabled: bool
 
 
 class NoticelistAttributesResponse(NoticelistAttributes):
-    NoticelistEntry: list[NoticelistEntryResponse]
+    NoticelistEntry: Sequence[NoticelistEntryResponse]
 
 
 class NoticelistResponse(BaseModel):
     Noticelist: NoticelistAttributesResponse
 
     class Config:
         orm_mode = True
```

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/objects/create_object_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/objects/create_object_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/objects/get_object_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/objects/get_object_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/objects/search_objects_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/objects/search_objects_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/organisations/organisation.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/organisations/organisation.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/roles/role.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/roles/role.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/sightings/get_sighting_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/sightings/get_sighting_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/tags/get_tag_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/tags/get_tag_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/tags/search_tags_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/tags/search_tags_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/users/user.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/users/user.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/create_warninglist_body.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/create_warninglist_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from enum import Enum
+from enum import StrEnum
 
 from pydantic import BaseModel, Field
 
 
-class WarninglistListType(str, Enum):
+class WarninglistListType(StrEnum):
     CIDR = "cidr"
     HOSTNAME = "hostname"
     STRING = "string"
     SUBSTRING = "substring"
     REGEX = "regex"
 
 
-class WarninglistCategory(str, Enum):
+class WarninglistCategory(StrEnum):
     FALSE_POSITIVE = "False positive"
     KNOWN_IDENTIFIER = "Known identifier"
 
 
-class ValidAttribute(str, Enum):
+# todo: use something from the mmisp.lib.attributes
+class ValidAttribute(StrEnum):
     MD5 = "md5"
     SHA12SHA256 = "sha12sha256"
     FILENAME = "filename"
     PDB = "pdb"
     FILENAME_MD5 = "filename|md5"
     FILENAME_SHA1 = "filename|sha1"
     FILENAME_SHA256 = "filename|sha256"
```

### Comparing `mmisp_lib-0.1.8/src/mmisp/api_schemas/warninglists/warninglist_response.py` & `mmisp_lib-0.1.9/src/mmisp/api_schemas/warninglists/warninglist_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/db/database.py` & `mmisp_lib-0.1.9/src/mmisp/db/database.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/db/models/attribute.py` & `mmisp_lib-0.1.9/src/mmisp/db/models/attribute.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from typing import Self, Type
 
-from sqlalchemy import BigInteger, Boolean, Column, ForeignKey, Integer, String, Text
+from sqlalchemy import BigInteger, Boolean, ForeignKey, Integer, String, Text
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.decl_api import DeclarativeMeta
 
 from mmisp.db.mixins import DictMixin
+from mmisp.db.mypy import Mapped, mapped_column
 from mmisp.lib.attributes import categories, default_category, mapper_safe_clsname_val, to_ids
 from mmisp.util.uuid import uuid
 
 from ..database import Base
 from .event import Event
 from .tag import Tag
 
 
 class Attribute(Base, DictMixin):
     __tablename__ = "attributes"
 
-    id = Column(Integer, primary_key=True, nullable=False)
-    uuid = Column(String(40), unique=True, default=uuid, index=True)
-    event_id = Column(Integer, ForeignKey("events.id", ondelete="CASCADE"), nullable=False, index=True)
-    object_id = Column(Integer, nullable=False, default=0, index=True)
-    object_relation = Column(String(255), index=True)
-    category = Column(String(255), nullable=False, index=True)
-    type = Column(String(100), nullable=False, index=True)
-    value1 = Column(Text, nullable=False)
-    value2 = Column(Text, nullable=False, default="")
-    to_ids = Column(Boolean, default=True, nullable=False)
-    timestamp = Column(Integer, nullable=False, default=0)
-    distribution = Column(Integer, nullable=False, default=0)
-    sharing_group_id = Column(Integer, index=True, default=0)
-    comment = Column(Text)
-    deleted = Column(Boolean, nullable=False, default=False)
-    disable_correlation = Column(Boolean, nullable=False, default=False)
-    first_seen = Column(BigInteger, index=True)
-    last_seen = Column(BigInteger, index=True)
+    id: Mapped[int] = mapped_column(Integer, primary_key=True, nullable=False)
+    uuid: Mapped[str] = mapped_column(String(40), unique=True, default=uuid, index=True)
+    event_id: Mapped[int] = mapped_column(
+        Integer, ForeignKey("events.id", ondelete="CASCADE"), nullable=False, index=True
+    )
+    object_id: Mapped[int] = mapped_column(Integer, nullable=False, default=0, index=True)
+    object_relation: Mapped[str] = mapped_column(String(255), index=True)
+    category: Mapped[str] = mapped_column(String(255), nullable=False, index=True)
+    type: Mapped[str] = mapped_column(String(100), nullable=False, index=True)
+    value1: Mapped[str] = mapped_column(Text, nullable=False)
+    value2: Mapped[str] = mapped_column(Text, nullable=False, default="")
+    to_ids: Mapped[bool] = mapped_column(Boolean, default=True, nullable=False)
+    timestamp: Mapped[int] = mapped_column(Integer, nullable=False, default=0)
+    distribution: Mapped[int] = mapped_column(Integer, nullable=False, default=0)
+    sharing_group_id: Mapped[int] = mapped_column(Integer, index=True, default=0)
+    comment: Mapped[str] = mapped_column(Text)
+    deleted: Mapped[bool] = mapped_column(Boolean, nullable=False, default=False)
+    disable_correlation: Mapped[bool] = mapped_column(Boolean, nullable=False, default=False)
+    first_seen: Mapped[int] = mapped_column(BigInteger, index=True)
+    last_seen: Mapped[int] = mapped_column(BigInteger, index=True)
 
     event = relationship("Event", back_populates="attributes", lazy="joined")
 
     __mapper_args__ = {"polymorphic_on": "type"}
 
     def __init__(self: Self, *arg, **kwargs) -> None:
         if kwargs["value1"] is None:
@@ -66,19 +69,21 @@
         if len(split) == 2:
             self.value2 = split[1]
 
 
 class AttributeTag(Base):
     __tablename__ = "attribute_tags"
 
-    id = Column(Integer, primary_key=True, nullable=False)
-    attribute_id = Column(Integer, ForeignKey(Attribute.id, ondelete="CASCADE"), nullable=False, index=True)
-    event_id = Column(Integer, ForeignKey(Event.id, ondelete="CASCADE"), nullable=False, index=True)
-    tag_id = Column(Integer, ForeignKey(Tag.id, ondelete="CASCADE"), nullable=False, index=True)
-    local = Column(Boolean, nullable=False, default=False)
+    id: Mapped[int] = mapped_column(Integer, primary_key=True, nullable=False)
+    attribute_id: Mapped[int] = mapped_column(
+        Integer, ForeignKey(Attribute.id, ondelete="CASCADE"), nullable=False, index=True
+    )
+    event_id: Mapped[int] = mapped_column(Integer, ForeignKey(Event.id, ondelete="CASCADE"), nullable=False, index=True)
+    tag_id: Mapped[int] = mapped_column(Integer, ForeignKey(Tag.id, ondelete="CASCADE"), nullable=False, index=True)
+    local: Mapped[bool] = mapped_column(Boolean, nullable=False, default=False)
 
 
 class AttributeMeta(DeclarativeMeta):
     def __new__(cls: Type[type], clsname: str, bases: tuple, dct: dict) -> "AttributeMeta":
         key = clsname[len("Attribute") :]
         dct["default_category"] = default_category[mapper_safe_clsname_val[key]]
         dct["categories"] = categories[mapper_safe_clsname_val[key]]
```

### Comparing `mmisp_lib-0.1.8/src/mmisp/db/models/galaxy_cluster.py` & `mmisp_lib-0.1.9/src/mmisp/db/models/galaxy_cluster.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-from sqlalchemy import Boolean, Column, ForeignKey, Integer, String, Text
+from sqlalchemy import Boolean, ForeignKey, Integer, String, Text
 
+from mmisp.db.mypy import Mapped, mapped_column
 from mmisp.util.uuid import uuid
 
 from ..database import Base
 from .galaxy import Galaxy
 
 
 class GalaxyCluster(Base):
     __tablename__ = "galaxy_clusters"
 
-    id = Column(Integer, primary_key=True, nullable=False)
-    uuid = Column(String(255), unique=True, default=uuid, index=True)
-    collection_uuid = Column(String(255), nullable=False, index=True, default="0")
-    type = Column(String(255), nullable=False, index=True)
-    value = Column(Text, nullable=False)
-    tag_name = Column(String(255), nullable=False, default="", index=True)
-    description = Column(Text, nullable=False)
-    galaxy_id = Column(Integer, ForeignKey(Galaxy.id, ondelete="CASCADE"), nullable=False, index=True)
-    source = Column(String(255), nullable=False, default="")
-    authors = Column(Text, nullable=False)
-    version = Column(Integer, default=0, index=True)
-    distribution = Column(Integer, nullable=False, default=0)
-    sharing_group_id = Column(Integer, index=True, default=0)
-    org_id = Column(Integer, nullable=False, index=True, default=0)
-    orgc_id = Column(Integer, nullable=False, index=True, default=0)
-    default = Column(Boolean, nullable=False, default=False, index=True)
-    locked = Column(Boolean, nullable=False, default=False)
-    extends_uuid = Column(String(40), index=True)
-    extends_version = Column(Integer, default=0, index=True)
-    published = Column(Boolean, nullable=False, default=False)
-    deleted = Column(Boolean, nullable=False, default=False)
+    id: Mapped[int] = mapped_column(Integer, primary_key=True, nullable=False)
+    uuid: Mapped[str] = mapped_column(String(255), unique=True, default=uuid, index=True)
+    collection_uuid: Mapped[str] = mapped_column(String(255), nullable=False, index=True, default="0")
+    type: Mapped[str] = mapped_column(String(255), nullable=False, index=True)
+    value: Mapped[str] = mapped_column(Text, nullable=False)
+    tag_name: Mapped[str] = mapped_column(String(255), nullable=False, default="", index=True)
+    description: Mapped[str] = mapped_column(Text, nullable=False)
+    galaxy_id: Mapped[int] = mapped_column(
+        Integer, ForeignKey(Galaxy.id, ondelete="CASCADE"), nullable=False, index=True
+    )
+    source: Mapped[str] = mapped_column(String(255), nullable=False, default="")
+    authors: Mapped[str] = mapped_column(Text, nullable=False)
+    version: Mapped[int] = mapped_column(Integer, default=0, index=True)
+    distribution: Mapped[int] = mapped_column(Integer, nullable=False, default=0)
+    sharing_group_id: Mapped[int] = mapped_column(Integer, index=True, default=0)
+    org_id: Mapped[int] = mapped_column(Integer, nullable=False, index=True, default=0)
+    orgc_id: Mapped[int] = mapped_column(Integer, nullable=False, index=True, default=0)
+    default: Mapped[bool] = mapped_column(Boolean, nullable=False, default=False, index=True)
+    locked: Mapped[bool] = mapped_column(Boolean, nullable=False, default=False)
+    extends_uuid: Mapped[str] = mapped_column(String(40), index=True)
+    extends_version: Mapped[int] = mapped_column(Integer, default=0, index=True)
+    published: Mapped[bool] = mapped_column(Boolean, nullable=False, default=False)
+    deleted: Mapped[bool] = mapped_column(Boolean, nullable=False, default=False)
 
 
 class GalaxyElement(Base):
     __tablename__ = "galaxy_elements"
 
-    id = Column(Integer, primary_key=True, nullable=False)
-    galaxy_cluster_id = Column(Integer, ForeignKey(GalaxyCluster.id, ondelete="CASCADE"), nullable=False, index=True)
-    key = Column(String(255), nullable=False, default="", index=True)
-    value = Column(Text, nullable=False)
+    id: Mapped[int] = mapped_column(Integer, primary_key=True, nullable=False)
+    galaxy_cluster_id: Mapped[int] = mapped_column(
+        Integer, ForeignKey(GalaxyCluster.id, ondelete="CASCADE"), nullable=False, index=True
+    )
+    key: Mapped[str] = mapped_column(String(255), nullable=False, default="", index=True)
+    value: Mapped[str] = mapped_column(Text, nullable=False)
 
 
 class GalaxyReference(Base):
     __tablename__ = "galaxy_reference"
 
-    id = Column(Integer, primary_key=True, nullable=False)
-    galaxy_cluster_id = Column(Integer, ForeignKey(GalaxyCluster.id, ondelete="CASCADE"), nullable=False, index=True)
-    referenced_galaxy_cluster_id = Column(Integer, nullable=False, index=True)
-    referenced_galaxy_cluster_uuid = Column(String(255), nullable=False, index=True)
-    referenced_galaxy_cluster_type = Column(Text, nullable=False)
-    referenced_galaxy_cluster_value = Column(Text, nullable=False)
+    id: Mapped[int] = mapped_column(Integer, primary_key=True, nullable=False)
+    galaxy_cluster_id: Mapped[int] = mapped_column(
+        Integer, ForeignKey(GalaxyCluster.id, ondelete="CASCADE"), nullable=False, index=True
+    )
+    referenced_galaxy_cluster_id: Mapped[int] = mapped_column(Integer, nullable=False, index=True)
+    referenced_galaxy_cluster_uuid: Mapped[str] = mapped_column(String(255), nullable=False, index=True)
+    referenced_galaxy_cluster_type: Mapped[str] = mapped_column(Text, nullable=False)
+    referenced_galaxy_cluster_value: Mapped[str] = mapped_column(Text, nullable=False)
```

### Comparing `mmisp_lib-0.1.8/src/mmisp/db/models/role.py` & `mmisp_lib-0.1.9/src/mmisp/db/models/role.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from typing import Self
 
-from sqlalchemy import Boolean, Column, DateTime, Integer, String
+from sqlalchemy import Boolean, DateTime, Integer, String
 
+from mmisp.db.mypy import mapped_column
 from mmisp.lib.permissions import Permission
 
 from ..database import Base
 
 RoleAttrs = {
     "__tablename__": "roles",
-    "id": Column(Integer, primary_key=True, nullable=False),
-    "name": Column(String(255), nullable=False),
-    "created": Column(DateTime, default=None),
-    "modified": Column(DateTime, default=None),
-    "default_role": Column(Boolean, nullable=False, default=False),
-    "memory_limit": Column(String(255), default=""),
-    "max_execution_time": Column(String(255), default=""),
-    "restricted_to_site_admin": Column(Boolean, nullable=False, default=False),
-    "enforce_rate_limit": Column(Boolean, nullable=False, default=False),
-    "rate_limit_count": Column(Integer, nullable=False, default=0),
-} | {f"perm_{x.value}": Column(Boolean, default=False) for x in Permission}
+    "id": mapped_column(Integer, primary_key=True, nullable=False),
+    "name": mapped_column(String(255), nullable=False),
+    "created": mapped_column(DateTime, default=None),
+    "modified": mapped_column(DateTime, default=None),
+    "default_role": mapped_column(Boolean, nullable=False, default=False),
+    "memory_limit": mapped_column(String(255), default=""),
+    "max_execution_time": mapped_column(String(255), default=""),
+    "restricted_to_site_admin": mapped_column(Boolean, nullable=False, default=False),
+    "enforce_rate_limit": mapped_column(Boolean, nullable=False, default=False),
+    "rate_limit_count": mapped_column(Integer, nullable=False, default=0),
+} | {f"perm_{x.value}": mapped_column(Boolean, default=False) for x in Permission}
 
 RoleModel = type("RoleModel", (Base,), RoleAttrs)
 
 
 class Role(RoleModel):
     def get_permissions(self: Self) -> set[Permission]:
         d: list[Permission] = []
```

### Comparing `mmisp_lib-0.1.8/src/mmisp/db/models/user_setting.py` & `mmisp_lib-0.1.9/src/mmisp/db/models/user_setting.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 from time import time
 
-from sqlalchemy import Column, ForeignKey, Integer, String, Text
+from sqlalchemy import ForeignKey, Integer, String, Text
 
 from mmisp.db.database import Base
+from mmisp.db.mypy import Mapped, mapped_column
 
 from .user import User
 
 
 class SettingName(Enum):
     PUBLISH_ALERT_FILTER = "publish_alert_filter"
     DASHBOARD_ACCESS = "dashboard_access"
@@ -18,12 +19,12 @@
     EVENT_INDEX_HIDE_COLUMNS = "event_index_hide_columns"
     PERIODIC_NOTIFICATION_FILTERS = "periodic_notification_filters"
 
 
 class UserSetting(Base):
     __tablename__ = "user_settings"
 
-    id = Column(Integer, primary_key=True, nullable=False)
-    setting = Column(String(255), nullable=False, index=True)
-    value = Column(Text, nullable=False)
-    user_id = Column(Integer, ForeignKey(User.id), nullable=False, index=True)
-    timestamp = Column(Integer, default=time, onupdate=time, nullable=False, index=True)
+    id: Mapped[int] = mapped_column(Integer, primary_key=True, nullable=False)
+    setting: Mapped[str] = mapped_column(String(255), nullable=False, index=True)
+    value: Mapped[str] = mapped_column(Text, nullable=False)
+    user_id: Mapped[int] = mapped_column(Integer, ForeignKey(User.id), nullable=False, index=True)
+    timestamp: Mapped[int] = mapped_column(Integer, default=time, onupdate=time, nullable=False, index=True)
```

### Comparing `mmisp_lib-0.1.8/src/mmisp/db/print_changes.py` & `mmisp_lib-0.1.9/src/mmisp/db/print_changes.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/lib/attributes.py` & `mmisp_lib-0.1.9/src/mmisp/lib/attributes.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp/lib/permissions.py` & `mmisp_lib-0.1.9/src/mmisp/lib/permissions.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.8/src/mmisp_lib.egg-info/PKG-INFO` & `mmisp_lib-0.1.9/src/mmisp_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mmisp-lib
-Version: 0.1.8
+Version: 0.1.9
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi==0.104.1
-Requires-Dist: SQLAlchemy[asyncio]==1.4.46
+Requires-Dist: SQLAlchemy[asyncio]~=1.4.46
 Requires-Dist: pydantic==1.10.13
 Requires-Dist: uvicorn==0.24.0.post1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: alembic==1.8.1
 Requires-Dist: aiomysql==0.2.0
 Requires-Dist: aiosqlite==0.20.0
 Requires-Dist: PyJWT==2.8.0
```

### Comparing `mmisp_lib-0.1.8/src/mmisp_lib.egg-info/SOURCES.txt` & `mmisp_lib-0.1.9/src/mmisp_lib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_response.py
 src/mmisp/api_schemas/warninglists/warninglist_response.py
 src/mmisp/db/__init__.py
 src/mmisp/db/all_models.py
 src/mmisp/db/config.py
 src/mmisp/db/database.py
 src/mmisp/db/mixins.py
+src/mmisp/db/mypy.py
 src/mmisp/db/print_changes.py
 src/mmisp/db/py.typed
 src/mmisp/db/models/__init__.py
 src/mmisp/db/models/attribute.py
 src/mmisp/db/models/auth_key.py
 src/mmisp/db/models/event.py
 src/mmisp/db/models/feed.py
```

