# Comparing `tmp/blendedux-0.1.1.tar.gz` & `tmp/blendedux-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendedux-0.1.1.tar", last modified: Fri Jul 14 06:00:48 2023, max compression
+gzip compressed data, was "dist\blendedux-0.1.2.tar", last modified: Fri May 31 05:51:25 2024, max compression
```

## Comparing `blendedux-0.1.1.tar` & `blendedux-0.1.2.tar`

### file list

```diff
@@ -1,155 +1,302 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.907767 blendedux-0.1.1/
--rw-rw-rw-   0        0        0     1096 2022-08-25 09:38:05.000000 blendedux-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       33 2023-07-14 05:47:24.000000 blendedux-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5403 2023-07-14 06:00:48.906755 blendedux-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5116 2023-07-14 05:59:53.000000 blendedux-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.103981 blendedux-0.1.1/blendedUx/
--rw-rw-rw-   0        0        0      107 2023-07-13 12:14:39.000000 blendedux-0.1.1/blendedUx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.132701 blendedux-0.1.1/blendedUx/blended_flask/
--rw-rw-rw-   0        0        0      160 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/__init__.py
--rw-rw-rw-   0        0        0     1208 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/app.py
--rw-rw-rw-   0        0        0     3758 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/bl_flask_app.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.143709 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.198975 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/backend/
--rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/backend/__init__.py
--rw-rw-rw-   0        0        0    44898 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/backend/backend.py
--rw-rw-rw-   0        0        0     8056 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py
--rw-rw-rw-   0        0        0     1016 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/backend/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.203000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/controller/
--rw-rw-rw-   0        0        0       27 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/controller/__init__.py
--rw-rw-rw-   0        0        0   150877 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/controller/controller.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.210977 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/exceptions/
--rw-rw-rw-   0        0        0       25 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/exceptions/__init__.py
--rw-rw-rw-   0        0        0      456 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.214978 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/functions/
--rw-rw-rw-   0        0        0       26 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/functions/__init__.py
--rw-rw-rw-   0        0        0      655 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/functions/functions.py
--rw-rw-rw-   0        0        0    24684 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/initializer.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.220990 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/network/
--rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/network/__init__.py
--rw-rw-rw-   0        0        0    36830 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/network/network.py
--rw-rw-rw-   0        0        0      102 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/network/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.245253 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/
--rw-rw-rw-   0        0        0     6577 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py
--rw-rw-rw-   0        0        0    21458 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.256270 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/
--rw-rw-rw-   0        0        0      152 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/__init__.py
--rw-rw-rw-   0        0        0   141226 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py
--rw-rw-rw-   0        0        0   242470 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py
--rw-rw-rw-   0        0        0     7574 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.845140 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/
--rw-rw-rw-   0        0        0     5530 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py
--rw-rw-rw-   0        0        0     8007 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py
--rw-rw-rw-   0        0        0     5983 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py
--rw-rw-rw-   0        0        0     4369 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py
--rw-rw-rw-   0        0        0     4168 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py
--rw-rw-rw-   0        0        0    10818 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py
--rw-rw-rw-   0        0        0     3597 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py
--rw-rw-rw-   0        0        0    10364 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py
--rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py
--rw-rw-rw-   0        0        0     7352 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py
--rw-rw-rw-   0        0        0     3547 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py
--rw-rw-rw-   0        0        0     3489 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py
--rw-rw-rw-   0        0        0     4114 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py
--rw-rw-rw-   0        0        0     5149 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py
--rw-rw-rw-   0        0        0     3543 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py
--rw-rw-rw-   0        0        0     7377 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py
--rw-rw-rw-   0        0        0    22811 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py
--rw-rw-rw-   0        0        0     3503 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py
--rw-rw-rw-   0        0        0     3727 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py
--rw-rw-rw-   0        0        0     7110 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py
--rw-rw-rw-   0        0        0    12189 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py
--rw-rw-rw-   0        0        0    18472 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py
--rw-rw-rw-   0        0        0     3615 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py
--rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py
--rw-rw-rw-   0        0        0     5504 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py
--rw-rw-rw-   0        0        0     4973 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py
--rw-rw-rw-   0        0        0     4853 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py
--rw-rw-rw-   0        0        0     7008 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py
--rw-rw-rw-   0        0        0     5695 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py
--rw-rw-rw-   0        0        0     4261 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py
--rw-rw-rw-   0        0        0    11135 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py
--rw-rw-rw-   0        0        0     5279 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py
--rw-rw-rw-   0        0        0     4151 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py
--rw-rw-rw-   0        0        0     4125 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py
--rw-rw-rw-   0        0        0     5150 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py
--rw-rw-rw-   0        0        0     5198 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py
--rw-rw-rw-   0        0        0     9159 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py
--rw-rw-rw-   0        0        0     9152 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py
--rw-rw-rw-   0        0        0     6037 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py
--rw-rw-rw-   0        0        0     8824 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py
--rw-rw-rw-   0        0        0     4246 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py
--rw-rw-rw-   0        0        0     3645 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py
--rw-rw-rw-   0        0        0     7652 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py
--rw-rw-rw-   0        0        0     4399 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py
--rw-rw-rw-   0        0        0     9790 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py
--rw-rw-rw-   0        0        0     4256 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py
--rw-rw-rw-   0        0        0     4308 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py
--rw-rw-rw-   0        0        0     4239 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py
--rw-rw-rw-   0        0        0     4201 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py
--rw-rw-rw-   0        0        0     4286 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py
--rw-rw-rw-   0        0        0    10246 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py
--rw-rw-rw-   0        0        0     4251 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py
--rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py
--rw-rw-rw-   0        0        0     5230 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py
--rw-rw-rw-   0        0        0     4598 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py
--rw-rw-rw-   0        0        0     5095 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py
--rw-rw-rw-   0        0        0     3651 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py
--rw-rw-rw-   0        0        0     4919 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py
--rw-rw-rw-   0        0        0     2986 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py
--rw-rw-rw-   0        0        0     6127 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py
--rw-rw-rw-   0        0        0     5293 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py
--rw-rw-rw-   0        0        0     4181 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py
--rw-rw-rw-   0        0        0     5560 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py
--rw-rw-rw-   0        0        0     4212 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py
--rw-rw-rw-   0        0        0    10618 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py
--rw-rw-rw-   0        0        0    14020 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py
--rw-rw-rw-   0        0        0    17540 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py
--rw-rw-rw-   0        0        0     8618 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py
--rw-rw-rw-   0        0        0     8540 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py
--rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py
--rw-rw-rw-   0        0        0     4368 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py
--rw-rw-rw-   0        0        0     5025 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py
--rw-rw-rw-   0        0        0     7275 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py
--rw-rw-rw-   0        0        0     5218 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py
--rw-rw-rw-   0        0        0    13040 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py
--rw-rw-rw-   0        0        0     4502 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py
--rw-rw-rw-   0        0        0     3659 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py
--rw-rw-rw-   0        0        0     5940 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py
--rw-rw-rw-   0        0        0     3624 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py
--rw-rw-rw-   0        0        0    16618 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py
--rw-rw-rw-   0        0        0     5002 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py
--rw-rw-rw-   0        0        0     5133 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py
--rw-rw-rw-   0        0        0     4390 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py
--rw-rw-rw-   0        0        0     9362 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py
--rw-rw-rw-   0        0        0     4385 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py
--rw-rw-rw-   0        0        0     9033 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py
--rw-rw-rw-   0        0        0     4935 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py
--rw-rw-rw-   0        0        0     3569 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py
--rw-rw-rw-   0        0        0     6351 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py
--rw-rw-rw-   0        0        0     4537 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py
--rw-rw-rw-   0        0        0     3780 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py
--rw-rw-rw-   0        0        0     4799 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py
--rw-rw-rw-   0        0        0    12227 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py
--rw-rw-rw-   0        0        0     4121 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py
--rw-rw-rw-   0        0        0     8930 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py
--rw-rw-rw-   0        0        0     6347 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py
--rw-rw-rw-   0        0        0     6614 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py
--rw-rw-rw-   0        0        0     9282 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py
--rw-rw-rw-   0        0        0    17690 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py
--rw-rw-rw-   0        0        0     4152 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py
--rw-rw-rw-   0        0        0     9542 2023-04-24 05:51:06.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py
--rw-rw-rw-   0        0        0     3319 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/tests.py
--rw-rw-rw-   0        0        0    11975 2023-07-06 12:33:23.000000 blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/transform_image.py
--rw-rw-rw-   0        0        0     4612 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/functions.py
--rw-rw-rw-   0        0        0      329 2023-05-03 09:50:10.000000 blendedux-0.1.1/blendedUx/blended_flask/settings.py
--rw-rw-rw-   0        0        0     3799 2023-07-13 13:32:53.000000 blendedux-0.1.1/blendedUx/blended_flask/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:00:48.902745 blendedux-0.1.1/blendedux.egg-info/
--rw-rw-rw-   0        0        0     5403 2023-07-14 06:00:47.000000 blendedux-0.1.1/blendedux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10128 2023-07-14 06:00:47.000000 blendedux-0.1.1/blendedux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 06:00:47.000000 blendedux-0.1.1/blendedux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      234 2023-07-14 06:00:47.000000 blendedux-0.1.1/blendedux.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 06:00:47.000000 blendedux-0.1.1/blendedux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 06:00:48.909770 blendedux-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1060 2023-07-14 06:00:24.000000 blendedux-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:25.406752 blendedux-0.1.2/
+-rw-rw-rw-   0        0        0       33 2023-07-14 05:47:24.000000 blendedux-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6565 2024-05-31 05:51:25.406752 blendedux-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5116 2023-07-14 05:59:53.000000 blendedux-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:17.398157 blendedux-0.1.2/blendedUx/
+-rw-rw-rw-   0        0        0      107 2023-07-13 12:14:39.000000 blendedux-0.1.2/blendedUx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:17.406171 blendedux-0.1.2/blendedUx/blended_django/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:51:07.000000 blendedux-0.1.2/blendedUx/blended_django/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:17.828193 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:51:09.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/__init__.py
+-rw-rw-rw-   0        0        0       63 2024-05-29 11:51:07.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/admin.py
+-rw-rw-rw-   0        0        0     1782 2024-05-29 11:51:07.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/context.py
+-rw-rw-rw-   0        0        0     9999 2024-05-29 11:51:07.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/functions.py
+-rw-rw-rw-   0        0        0      466 2024-05-29 11:51:08.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:17.829624 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/migrations/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:51:09.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/migrations/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-05-29 11:51:08.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/models.py
+-rw-rw-rw-   0        0        0       60 2024-05-29 11:51:08.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/tests.py
+-rw-rw-rw-   0        0        0    15942 2024-05-29 11:51:08.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/transform.py
+-rw-rw-rw-   0        0        0      147 2024-05-29 11:51:08.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/urls.py
+-rw-rw-rw-   0        0        0      324 2024-05-29 11:51:08.000000 blendedux-0.1.2/blendedUx/blended_django/blended_django_app/views.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:17.979565 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:51:11.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:18.119705 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/backend/
+-rw-rw-rw-   0        0        0       24 2024-05-29 11:51:12.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/backend/__init__.py
+-rw-rw-rw-   0        0        0    44889 2024-05-29 11:51:11.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/backend/backend.py
+-rw-rw-rw-   0        0        0     8047 2024-05-29 11:51:11.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/backend/intermediary.py
+-rw-rw-rw-   0        0        0     1016 2024-05-29 11:51:12.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/backend/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:18.216562 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/controller/
+-rw-rw-rw-   0        0        0       27 2024-05-29 11:51:13.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/controller/__init__.py
+-rw-rw-rw-   0        0        0   150892 2024-05-29 11:51:12.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/controller/controller.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:18.257488 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/exceptions/
+-rw-rw-rw-   0        0        0       25 2024-05-29 11:51:13.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      456 2024-05-29 11:51:13.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:18.305757 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/functions/
+-rw-rw-rw-   0        0        0       26 2024-05-29 11:51:14.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/functions/__init__.py
+-rw-rw-rw-   0        0        0      655 2024-05-29 11:51:14.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/functions/functions.py
+-rw-rw-rw-   0        0        0    24648 2024-05-29 11:51:11.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/initializer.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:18.396263 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/network/
+-rw-rw-rw-   0        0        0       24 2024-05-29 11:51:15.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/network/__init__.py
+-rw-rw-rw-   0        0        0    36794 2024-05-29 11:51:14.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/network/network.py
+-rw-rw-rw-   0        0        0      102 2024-05-29 11:51:14.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/network/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:18.718088 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/
+-rw-rw-rw-   0        0        0     6577 2024-05-29 11:51:16.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/__init__.py
+-rw-rw-rw-   0        0        0    21458 2024-05-29 11:51:16.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/api_client.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:18.961301 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/apis/
+-rw-rw-rw-   0        0        0      152 2024-05-29 11:51:16.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/apis/__init__.py
+-rw-rw-rw-   0        0        0   141226 2024-05-29 11:51:16.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/apis/accounts_api.py
+-rw-rw-rw-   0        0        0   242470 2024-05-29 11:51:16.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/apis/packages_api.py
+-rw-rw-rw-   0        0        0     7574 2024-05-29 11:51:16.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:22.665995 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/
+-rw-rw-rw-   0        0        0     5530 2024-05-29 11:51:27.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/__init__.py
+-rw-rw-rw-   0        0        0     8007 2024-05-29 11:51:17.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/account.py
+-rw-rw-rw-   0        0        0     5983 2024-05-29 11:51:17.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/account_invite_pending.py
+-rw-rw-rw-   0        0        0     4369 2024-05-29 11:51:17.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/account_invites_pending_list.py
+-rw-rw-rw-   0        0        0     4168 2024-05-29 11:51:17.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/accounts.py
+-rw-rw-rw-   0        0        0    10818 2024-05-29 11:51:17.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/acquisition.py
+-rw-rw-rw-   0        0        0     3597 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/acquisition_response.py
+-rw-rw-rw-   0        0        0    10364 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/acquisition_response_data.py
+-rw-rw-rw-   0        0        0     4303 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/activationchallenge.py
+-rw-rw-rw-   0        0        0     7352 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/active_account.py
+-rw-rw-rw-   0        0        0     3547 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_account.py
+-rw-rw-rw-   0        0        0     3489 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_admin.py
+-rw-rw-rw-   0        0        0     4114 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_license.py
+-rw-rw-rw-   0        0        0     5149 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_pending.py
+-rw-rw-rw-   0        0        0     3543 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_rating.py
+-rw-rw-rw-   0        0        0     7377 2024-05-29 11:51:18.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/all_license_price.py
+-rw-rw-rw-   0        0        0    22811 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/blended_package.py
+-rw-rw-rw-   0        0        0     3503 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/body.py
+-rw-rw-rw-   0        0        0     3727 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/body_1.py
+-rw-rw-rw-   0        0        0     7110 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/bundled_packages.py
+-rw-rw-rw-   0        0        0    12189 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/bundled_packages_error.py
+-rw-rw-rw-   0        0        0    18472 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/canonical_version.py
+-rw-rw-rw-   0        0        0     3615 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/change_current_account.py
+-rw-rw-rw-   0        0        0     3735 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/change_privilege.py
+-rw-rw-rw-   0        0        0     5504 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/create_account.py
+-rw-rw-rw-   0        0        0     4973 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/create_canonical.py
+-rw-rw-rw-   0        0        0     4853 2024-05-29 11:51:19.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/create_package.py
+-rw-rw-rw-   0        0        0     7008 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/create_version.py
+-rw-rw-rw-   0        0        0     5695 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/dependencies.py
+-rw-rw-rw-   0        0        0     4261 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/dependencies_list.py
+-rw-rw-rw-   0        0        0    11135 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/dependency_package_detail.py
+-rw-rw-rw-   0        0        0     5279 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py
+-rw-rw-rw-   0        0        0     4151 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/documents.py
+-rw-rw-rw-   0        0        0     4125 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error.py
+-rw-rw-rw-   0        0        0     5150 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response400.py
+-rw-rw-rw-   0        0        0     5198 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response401.py
+-rw-rw-rw-   0        0        0     9159 2024-05-29 11:51:20.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response409.py
+-rw-rw-rw-   0        0        0     9152 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response412.py
+-rw-rw-rw-   0        0        0     6037 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response500.py
+-rw-rw-rw-   0        0        0     8824 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/failed_dependency_error.py
+-rw-rw-rw-   0        0        0     4246 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_account.py
+-rw-rw-rw-   0        0        0     3645 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py
+-rw-rw-rw-   0        0        0     7652 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_current_account.py
+-rw-rw-rw-   0        0        0     4399 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py
+-rw-rw-rw-   0        0        0     9790 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_draft.py
+-rw-rw-rw-   0        0        0     4256 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_licenses.py
+-rw-rw-rw-   0        0        0     4308 2024-05-29 11:51:21.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_pending_user.py
+-rw-rw-rw-   0        0        0     4239 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_ratings.py
+-rw-rw-rw-   0        0        0     4201 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_user.py
+-rw-rw-rw-   0        0        0     4286 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_validators.py
+-rw-rw-rw-   0        0        0    10246 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/initial_package.py
+-rw-rw-rw-   0        0        0     4251 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/initial_packages.py
+-rw-rw-rw-   0        0        0     3735 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/inline_response_200.py
+-rw-rw-rw-   0        0        0     5230 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/license.py
+-rw-rw-rw-   0        0        0     4598 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/like.py
+-rw-rw-rw-   0        0        0     5095 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/login.py
+-rw-rw-rw-   0        0        0     3651 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/logout.py
+-rw-rw-rw-   0        0        0     4919 2024-05-29 11:51:22.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/new_draft.py
+-rw-rw-rw-   0        0        0     2986 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/operands.py
+-rw-rw-rw-   0        0        0     6127 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/package_detail_data.py
+-rw-rw-rw-   0        0        0     5293 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/package_images.py
+-rw-rw-rw-   0        0        0     4181 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/packages.py
+-rw-rw-rw-   0        0        0     5560 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/pending_user.py
+-rw-rw-rw-   0        0        0     4212 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/pending_users.py
+-rw-rw-rw-   0        0        0    10618 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication.py
+-rw-rw-rw-   0        0        0    14020 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_error.py
+-rw-rw-rw-   0        0        0    17540 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_validation_error.py
+-rw-rw-rw-   0        0        0     8618 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_version.py
+-rw-rw-rw-   0        0        0     8540 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_version_error.py
+-rw-rw-rw-   0        0        0     4303 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_versions.py
+-rw-rw-rw-   0        0        0     4368 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_versions_error.py
+-rw-rw-rw-   0        0        0     5025 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publications.py
+-rw-rw-rw-   0        0        0     7275 2024-05-29 11:51:23.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publications_error.py
+-rw-rw-rw-   0        0        0     5218 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/rating.py
+-rw-rw-rw-   0        0        0    13040 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/reject_acquisition_package.py
+-rw-rw-rw-   0        0        0     4502 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/remove_pending.py
+-rw-rw-rw-   0        0        0     3659 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/resend_account_verification_link.py
+-rw-rw-rw-   0        0        0     5940 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/resend_invite.py
+-rw-rw-rw-   0        0        0     3624 2024-05-29 11:51:24.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/reset_password.py
+-rw-rw-rw-   0        0        0    16618 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/search_result.py
+-rw-rw-rw-   0        0        0     5002 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/search_results.py
+-rw-rw-rw-   0        0        0     5133 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/session_data.py
+-rw-rw-rw-   0        0        0     4390 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/share_approval_list_error.py
+-rw-rw-rw-   0        0        0     9362 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/shared_package_account.py
+-rw-rw-rw-   0        0        0     4385 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/shared_package_accounts_list.py
+-rw-rw-rw-   0        0        0     9033 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_account.py
+-rw-rw-rw-   0        0        0     4935 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_draft.py
+-rw-rw-rw-   0        0        0     3569 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_license.py
+-rw-rw-rw-   0        0        0     6351 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_package.py
+-rw-rw-rw-   0        0        0     4537 2024-05-29 11:51:25.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_publication.py
+-rw-rw-rw-   0        0        0     3780 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_version.py
+-rw-rw-rw-   0        0        0     4799 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/upload_media.py
+-rw-rw-rw-   0        0        0    12227 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/user.py
+-rw-rw-rw-   0        0        0     4121 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/users.py
+-rw-rw-rw-   0        0        0     8930 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/validator.py
+-rw-rw-rw-   0        0        0     6347 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/validator_detail.py
+-rw-rw-rw-   0        0        0     6614 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/validator_plan.py
+-rw-rw-rw-   0        0        0     9282 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/validator_sets_in_badge.py
+-rw-rw-rw-   0        0        0    17690 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/version.py
+-rw-rw-rw-   0        0        0     4152 2024-05-29 11:51:26.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/versions.py
+-rw-rw-rw-   0        0        0     9542 2024-05-29 11:51:16.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/rest.py
+-rw-rw-rw-   0        0        0     3283 2024-05-29 11:51:11.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/tests.py
+-rw-rw-rw-   0        0        0    11926 2024-05-29 11:51:11.000000 blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/transform_image.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:22.852554 blendedux-0.1.2/blendedUx/blended_flask/
+-rw-rw-rw-   0        0        0      160 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/__init__.py
+-rw-rw-rw-   0        0        0     1208 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/app.py
+-rw-rw-rw-   0        0        0     3758 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/bl_flask_app.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:22.927037 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:23.008665 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/backend/
+-rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/backend/__init__.py
+-rw-rw-rw-   0        0        0    44898 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/backend/backend.py
+-rw-rw-rw-   0        0        0     8056 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py
+-rw-rw-rw-   0        0        0     1016 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/backend/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:23.096326 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/controller/
+-rw-rw-rw-   0        0        0       27 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/controller/__init__.py
+-rw-rw-rw-   0        0        0   150877 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/controller/controller.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:23.111078 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/exceptions/
+-rw-rw-rw-   0        0        0       25 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      456 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:23.122806 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/functions/
+-rw-rw-rw-   0        0        0       26 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/functions/__init__.py
+-rw-rw-rw-   0        0        0      655 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/functions/functions.py
+-rw-rw-rw-   0        0        0    24684 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/initializer.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:23.205968 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/network/
+-rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/network/__init__.py
+-rw-rw-rw-   0        0        0    36830 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/network/network.py
+-rw-rw-rw-   0        0        0      102 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/network/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:23.292168 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/
+-rw-rw-rw-   0        0        0     6577 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py
+-rw-rw-rw-   0        0        0    21458 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:23.422231 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/
+-rw-rw-rw-   0        0        0      152 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/__init__.py
+-rw-rw-rw-   0        0        0   141226 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py
+-rw-rw-rw-   0        0        0   242470 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py
+-rw-rw-rw-   0        0        0     7574 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:25.195910 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/
+-rw-rw-rw-   0        0        0     5530 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py
+-rw-rw-rw-   0        0        0     8007 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py
+-rw-rw-rw-   0        0        0     5983 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py
+-rw-rw-rw-   0        0        0     4369 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py
+-rw-rw-rw-   0        0        0     4168 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py
+-rw-rw-rw-   0        0        0    10818 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py
+-rw-rw-rw-   0        0        0     3597 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py
+-rw-rw-rw-   0        0        0    10364 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py
+-rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py
+-rw-rw-rw-   0        0        0     7352 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py
+-rw-rw-rw-   0        0        0     3547 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py
+-rw-rw-rw-   0        0        0     3489 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py
+-rw-rw-rw-   0        0        0     4114 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py
+-rw-rw-rw-   0        0        0     5149 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py
+-rw-rw-rw-   0        0        0     3543 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py
+-rw-rw-rw-   0        0        0     7377 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py
+-rw-rw-rw-   0        0        0    22811 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py
+-rw-rw-rw-   0        0        0     3503 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py
+-rw-rw-rw-   0        0        0     3727 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py
+-rw-rw-rw-   0        0        0     7110 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py
+-rw-rw-rw-   0        0        0    12189 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py
+-rw-rw-rw-   0        0        0    18472 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py
+-rw-rw-rw-   0        0        0     3615 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py
+-rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py
+-rw-rw-rw-   0        0        0     5504 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py
+-rw-rw-rw-   0        0        0     4973 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py
+-rw-rw-rw-   0        0        0     4853 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py
+-rw-rw-rw-   0        0        0     7008 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py
+-rw-rw-rw-   0        0        0     5695 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py
+-rw-rw-rw-   0        0        0     4261 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py
+-rw-rw-rw-   0        0        0    11135 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py
+-rw-rw-rw-   0        0        0     5279 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py
+-rw-rw-rw-   0        0        0     4151 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py
+-rw-rw-rw-   0        0        0     4125 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py
+-rw-rw-rw-   0        0        0     5150 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py
+-rw-rw-rw-   0        0        0     5198 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py
+-rw-rw-rw-   0        0        0     9159 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py
+-rw-rw-rw-   0        0        0     9152 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py
+-rw-rw-rw-   0        0        0     6037 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py
+-rw-rw-rw-   0        0        0     8824 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py
+-rw-rw-rw-   0        0        0     4246 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py
+-rw-rw-rw-   0        0        0     3645 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py
+-rw-rw-rw-   0        0        0     7652 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py
+-rw-rw-rw-   0        0        0     4399 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py
+-rw-rw-rw-   0        0        0     9790 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py
+-rw-rw-rw-   0        0        0     4256 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py
+-rw-rw-rw-   0        0        0     4308 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py
+-rw-rw-rw-   0        0        0     4239 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py
+-rw-rw-rw-   0        0        0     4201 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py
+-rw-rw-rw-   0        0        0     4286 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py
+-rw-rw-rw-   0        0        0    10246 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py
+-rw-rw-rw-   0        0        0     4251 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py
+-rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py
+-rw-rw-rw-   0        0        0     5230 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py
+-rw-rw-rw-   0        0        0     4598 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py
+-rw-rw-rw-   0        0        0     5095 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py
+-rw-rw-rw-   0        0        0     3651 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py
+-rw-rw-rw-   0        0        0     4919 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py
+-rw-rw-rw-   0        0        0     2986 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py
+-rw-rw-rw-   0        0        0     6127 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py
+-rw-rw-rw-   0        0        0     5293 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py
+-rw-rw-rw-   0        0        0     4181 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py
+-rw-rw-rw-   0        0        0     5560 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py
+-rw-rw-rw-   0        0        0     4212 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py
+-rw-rw-rw-   0        0        0    10618 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py
+-rw-rw-rw-   0        0        0    14020 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py
+-rw-rw-rw-   0        0        0    17540 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py
+-rw-rw-rw-   0        0        0     8618 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py
+-rw-rw-rw-   0        0        0     8540 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py
+-rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py
+-rw-rw-rw-   0        0        0     4368 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py
+-rw-rw-rw-   0        0        0     5025 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py
+-rw-rw-rw-   0        0        0     7275 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py
+-rw-rw-rw-   0        0        0     5218 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py
+-rw-rw-rw-   0        0        0    13040 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py
+-rw-rw-rw-   0        0        0     4502 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py
+-rw-rw-rw-   0        0        0     3659 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py
+-rw-rw-rw-   0        0        0     5940 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py
+-rw-rw-rw-   0        0        0     3624 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py
+-rw-rw-rw-   0        0        0    16618 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py
+-rw-rw-rw-   0        0        0     5002 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py
+-rw-rw-rw-   0        0        0     5133 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py
+-rw-rw-rw-   0        0        0     4390 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py
+-rw-rw-rw-   0        0        0     9362 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py
+-rw-rw-rw-   0        0        0     4385 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py
+-rw-rw-rw-   0        0        0     9033 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py
+-rw-rw-rw-   0        0        0     4935 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py
+-rw-rw-rw-   0        0        0     3569 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py
+-rw-rw-rw-   0        0        0     6351 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py
+-rw-rw-rw-   0        0        0     4537 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py
+-rw-rw-rw-   0        0        0     3780 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py
+-rw-rw-rw-   0        0        0     4799 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py
+-rw-rw-rw-   0        0        0    12227 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py
+-rw-rw-rw-   0        0        0     4121 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py
+-rw-rw-rw-   0        0        0     8930 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py
+-rw-rw-rw-   0        0        0     6347 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py
+-rw-rw-rw-   0        0        0     6614 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py
+-rw-rw-rw-   0        0        0     9282 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py
+-rw-rw-rw-   0        0        0    17690 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py
+-rw-rw-rw-   0        0        0     4152 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py
+-rw-rw-rw-   0        0        0     9542 2023-04-24 05:51:06.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py
+-rw-rw-rw-   0        0        0     3319 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/tests.py
+-rw-rw-rw-   0        0        0    11975 2023-07-06 12:33:23.000000 blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/transform_image.py
+-rw-rw-rw-   0        0        0     4612 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/functions.py
+-rw-rw-rw-   0        0        0      329 2023-05-03 09:50:10.000000 blendedux-0.1.2/blendedUx/blended_flask/settings.py
+-rw-rw-rw-   0        0        0     3799 2023-07-13 13:32:53.000000 blendedux-0.1.2/blendedUx/blended_flask/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:51:25.403818 blendedux-0.1.2/blendedux.egg-info/
+-rw-rw-rw-   0        0        0     6565 2024-05-31 05:51:17.000000 blendedux-0.1.2/blendedux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    20594 2024-05-31 05:51:17.000000 blendedux-0.1.2/blendedux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:51:17.000000 blendedux-0.1.2/blendedux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      234 2024-05-31 05:51:17.000000 blendedux-0.1.2/blendedux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-31 05:51:17.000000 blendedux-0.1.2/blendedux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:51:25.426118 blendedux-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2024-05-31 05:45:23.000000 blendedux-0.1.2/setup.py
```

### Comparing `blendedux-0.1.1/PKG-INFO` & `blendedux-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: blendedux
-Version: 0.1.1
-Summary: A cross-platform design theme framework.
-Home-page: UNKNOWN
-Author: Himanshu
-Author-email: <hbhadu@cognam.com>
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Blended python flask is a web framework, it is a python module that lets you develop web applications easily. Flask is very Pythonic. It is easy to get started with Flask, because it does not have a huge learning curve. On top of that it is very explicit, which increases readability. Simply, you can install the blended python flask, specify the path of your theme, run the server and can browse your website which is running on a Blended theme.
 
 ## Installation
 
 pip install blendedux
 
 ## Usages
@@ -153,9 +141,7 @@
 ```
 Note: It is registering the root URL for your application. This route is rendering a home.html template file by accepting the Blended theme context object. The home.html is a Blended host template and you can add many more as per your requirements in templates directory and then define a route for that template based on above code snippet in app.py. 
  
 For more details go to [Quickstart Python Flask](https://hub.blended.co/learn/quickstart_blended_flask/)
 
 ## License
 MIT
-
-
```

### Comparing `blendedux-0.1.1/README.md` & `blendedux-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,158 @@
-Blended python flask is a web framework, it is a python module that lets you develop web applications easily. Flask is very Pythonic. It is easy to get started with Flask, because it does not have a huge learning curve. On top of that it is very explicit, which increases readability. Simply, you can install the blended python flask, specify the path of your theme, run the server and can browse your website which is running on a Blended theme.
-
-## Installation
-
-pip install blendedux
-
-## Usages
-
-#### Setup of Blended Python Flask
-
-Run the following commands sequentially. First will create virtual environment, second will take you to the newly created virtual environment, third will activate the virtual environment and fourth will install blendedux inside the virtual environment.
-```
-python -m virtualenv env_name
-cd env_name
-Scripts\activate
-pip install blendedux
-```
-
-#### Create a file name app.py in the root directory and paste below line of code and save.
-
-```
-from flask import Flask
-from blendedUx import *
-from blendedUx.blended_flask.bl_flask_app import Bl_Flask
-
-PACKAGE_DIR = "themes-directory"
-
-app = Bl_Flask(__name__, package_dir= PACKAGE_DIR)
-
-user_name = 'user_name'
-theme_name = 'theme_name'
-password = ''
-
-theme = app.load(theme_name, user_name)
-
-@app.route("/css/<path:path>")
-@get_css('css_path')
-def css():
-   pass
-@app.route("/media/<path:path>")
-@get_media('media_path')
-def media():
-    pass
-@app.route("/js/<path:path>")
-@get_js('js_path')
-def js():
-    pass
-
-@app.route('/')
-def home(**kwargs):
-    """
-    """
-    context = theme
-    file_content = get_template('home.html')
-    try:
-        return render_code(file_content, context)
-    except UnicodeDecodeError:
-        return render_code(file_content.decode('utf-8'), context)
-
-if __name__ == "__main__":
-    app.run()
-```
-Note: Please specify your path in the package directory. You can point to your working directory which you have set up during cli and make sure that blended directory structures is there and it has a valid blended theme. Password is optional.
-For an example:
-```
-PACKAGE_DIR = "C:/Users/themes" 
-user_name = 'blended' 
-theme_name = 'base_theme' 
-password = '' 
-```
-#### How to Include the theme into your flask application?
-
-Create a templates directory in the root and create a home.html inside the templates directory and paste below line of code in the home.html and save.
-
-```
-{% extends theme.template.home|template %} 
-{% block title %}
-<title>My Blended Site </title> 
-{% endblock title %} 
-{% block css %}
-<link rel="stylesheet" href="{{css(theme)}}">
-{% endblock %}
-```
-Note: It is extending the home template of the theme. Extending a predefined Blended template should allow you to add a new page in your flask application. This host template is extending the theme base template named as home.html. Base templates are part of Blended theme which resides in the html directory.For an example:
-```
-{% extends theme.template.home|template %}
-```
-#### Run the Flask Server
-
-python app.py
-
-Just load the below URL (http://localhost:5000/) in a browser to see the output.
-
-
-## API
-
-#### CSS ENDPOINT
-By default, the /static directory will serve the static contents. If you want to provide the path of CSS then you can change this by following API:
-```
-  @app.route("/css/<path:path>")
-  @get_css("css_path") 
-  def css(): 
-    pass
-```
-Note: User will need to give the absolute path in the css_path like this @get_css("C:/blendedUx/static/css")
-
-#### Js ENDPOINT
-By default, the /static directory will serve the static contents. If you want to provide the path of js then you can change this by following API:
-```
-  @app.route("/js/<path:path>")
-  @get_js("js_path") 
-  def js(): 
-    pass
-```
-Note: User will need to give the absolute path in the js_path like this @get_js("C:/blendedUx/static/js")    
-
-#### Media ENDPOINT
-
-Add Media Endpoint
-By default application will host the media at /static directory in the root but you can change this by following API:
-```
-  @app.route("/media/<path:path>")
-  @get_media("media_path") 
-  def media(): 
-     pass
-```
-Note: User will need to give the absolute path in the media_path like this @get_media("C:/blendedUx/static/media") 
-
-#### Add Route
-```
-  @app.route("/")
-  def home(**kwargs):
-    """
-    """
-    context = theme 
-    file_content = get_template("home.html")
-    try:
-      return render_code(file_content, context)
-    except UnicodeDecodeError:
-      return render_code(file_content.decode("utf-8"), context)
-```
-Note: It is registering the root URL for your application. This route is rendering a home.html template file by accepting the Blended theme context object. The home.html is a Blended host template and you can add many more as per your requirements in templates directory and then define a route for that template based on above code snippet in app.py. 
- 
-For more details go to [Quickstart Python Flask](https://hub.blended.co/learn/quickstart_blended_flask/)
-
-## License
-MIT
+Metadata-Version: 2.1
+Name: blendedux
+Version: 0.1.2
+Summary: A cross-platform design theme framework.
+Home-page: UNKNOWN
+Author: Himanshu
+Author-email: <hbhadu@cognam.com>
+License: UNKNOWN
+Description: Blended python flask is a web framework, it is a python module that lets you develop web applications easily. Flask is very Pythonic. It is easy to get started with Flask, because it does not have a huge learning curve. On top of that it is very explicit, which increases readability. Simply, you can install the blended python flask, specify the path of your theme, run the server and can browse your website which is running on a Blended theme.
+        
+        ## Installation
+        
+        pip install blendedux
+        
+        ## Usages
+        
+        #### Setup of Blended Python Flask
+        
+        Run the following commands sequentially. First will create virtual environment, second will take you to the newly created virtual environment, third will activate the virtual environment and fourth will install blendedux inside the virtual environment.
+        ```
+        python -m virtualenv env_name
+        cd env_name
+        Scripts\activate
+        pip install blendedux
+        ```
+        
+        #### Create a file name app.py in the root directory and paste below line of code and save.
+        
+        ```
+        from flask import Flask
+        from blendedUx import *
+        from blendedUx.blended_flask.bl_flask_app import Bl_Flask
+        
+        PACKAGE_DIR = "themes-directory"
+        
+        app = Bl_Flask(__name__, package_dir= PACKAGE_DIR)
+        
+        user_name = 'user_name'
+        theme_name = 'theme_name'
+        password = ''
+        
+        theme = app.load(theme_name, user_name)
+        
+        @app.route("/css/<path:path>")
+        @get_css('css_path')
+        def css():
+           pass
+        @app.route("/media/<path:path>")
+        @get_media('media_path')
+        def media():
+            pass
+        @app.route("/js/<path:path>")
+        @get_js('js_path')
+        def js():
+            pass
+        
+        @app.route('/')
+        def home(**kwargs):
+            """
+            """
+            context = theme
+            file_content = get_template('home.html')
+            try:
+                return render_code(file_content, context)
+            except UnicodeDecodeError:
+                return render_code(file_content.decode('utf-8'), context)
+        
+        if __name__ == "__main__":
+            app.run()
+        ```
+        Note: Please specify your path in the package directory. You can point to your working directory which you have set up during cli and make sure that blended directory structures is there and it has a valid blended theme. Password is optional.
+        For an example:
+        ```
+        PACKAGE_DIR = "C:/Users/themes" 
+        user_name = 'blended' 
+        theme_name = 'base_theme' 
+        password = '' 
+        ```
+        #### How to Include the theme into your flask application?
+        
+        Create a templates directory in the root and create a home.html inside the templates directory and paste below line of code in the home.html and save.
+        
+        ```
+        {% extends theme.template.home|template %} 
+        {% block title %}
+        <title>My Blended Site </title> 
+        {% endblock title %} 
+        {% block css %}
+        <link rel="stylesheet" href="{{css(theme)}}">
+        {% endblock %}
+        ```
+        Note: It is extending the home template of the theme. Extending a predefined Blended template should allow you to add a new page in your flask application. This host template is extending the theme base template named as home.html. Base templates are part of Blended theme which resides in the html directory.For an example:
+        ```
+        {% extends theme.template.home|template %}
+        ```
+        #### Run the Flask Server
+        
+        python app.py
+        
+        Just load the below URL (http://localhost:5000/) in a browser to see the output.
+        
+        
+        ## API
+        
+        #### CSS ENDPOINT
+        By default, the /static directory will serve the static contents. If you want to provide the path of CSS then you can change this by following API:
+        ```
+          @app.route("/css/<path:path>")
+          @get_css("css_path") 
+          def css(): 
+            pass
+        ```
+        Note: User will need to give the absolute path in the css_path like this @get_css("C:/blendedUx/static/css")
+        
+        #### Js ENDPOINT
+        By default, the /static directory will serve the static contents. If you want to provide the path of js then you can change this by following API:
+        ```
+          @app.route("/js/<path:path>")
+          @get_js("js_path") 
+          def js(): 
+            pass
+        ```
+        Note: User will need to give the absolute path in the js_path like this @get_js("C:/blendedUx/static/js")    
+        
+        #### Media ENDPOINT
+        
+        Add Media Endpoint
+        By default application will host the media at /static directory in the root but you can change this by following API:
+        ```
+          @app.route("/media/<path:path>")
+          @get_media("media_path") 
+          def media(): 
+             pass
+        ```
+        Note: User will need to give the absolute path in the media_path like this @get_media("C:/blendedUx/static/media") 
+        
+        #### Add Route
+        ```
+          @app.route("/")
+          def home(**kwargs):
+            """
+            """
+            context = theme 
+            file_content = get_template("home.html")
+            try:
+              return render_code(file_content, context)
+            except UnicodeDecodeError:
+              return render_code(file_content.decode("utf-8"), context)
+        ```
+        Note: It is registering the root URL for your application. This route is rendering a home.html template file by accepting the Blended theme context object. The home.html is a Blended host template and you can add many more as per your requirements in templates directory and then define a route for that template based on above code snippet in app.py. 
+         
+        For more details go to [Quickstart Python Flask](https://hub.blended.co/learn/quickstart_blended_flask/)
+        
+        ## License
+        MIT
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/app.py` & `blendedux-0.1.2/blendedUx/blended_flask/app.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/bl_flask_app.py` & `blendedux-0.1.2/blendedUx/blended_flask/bl_flask_app.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/backend/backend.py` & `blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/backend/backend.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py` & `blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/backend/settings.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/backend/settings.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/controller/controller.py` & `blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/controller/controller.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/functions/functions.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/functions/functions.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/initializer.py` & `blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/initializer.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/network/network.py` & `blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/network/network.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/apis/accounts_api.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/apis/packages_api.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/account_invite_pending.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/account_invites_pending_list.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/accounts.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/acquisition_response.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/acquisition_response_data.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/activationchallenge.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/active_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_admin.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_license.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_pending.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/add_rating.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/all_license_price.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/blended_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/body.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/body_1.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/bundled_packages.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/bundled_packages_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/canonical_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/change_current_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/change_privilege.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/create_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/create_canonical.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/create_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/create_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/dependencies.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/dependencies_list.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/dependency_package_detail.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/documents.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response400.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response401.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response409.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response412.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/error_response500.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/failed_dependency_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_current_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_draft.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_licenses.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_pending_user.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_ratings.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_user.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/hyper_link_validators.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/initial_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/initial_packages.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/inline_response_200.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/license.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/like.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/login.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/logout.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/new_draft.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/operands.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/package_detail_data.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/package_images.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/packages.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/pending_user.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/pending_users.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_validation_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_version_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_versions.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publication_versions_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publications.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/publications_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/rating.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/reject_acquisition_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/remove_pending.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/resend_account_verification_link.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/resend_invite.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/reset_password.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/search_result.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/search_results.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/session_data.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/share_approval_list_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/shared_package_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/shared_package_accounts_list.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_draft.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_license.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_publication.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/update_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/upload_media.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/user.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/users.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/validator.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/validator_detail.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/validator_plan.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/validator_sets_in_badge.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/models/versions.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py` & `blendedux-0.1.2/blendedUx/blended_django/blended_hostlib/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/tests.py` & `blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/tests.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/blended_hostlib/transform_image.py` & `blendedux-0.1.2/blendedUx/blended_flask/blended_hostlib/transform_image.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/functions.py` & `blendedux-0.1.2/blendedUx/blended_flask/functions.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/blendedUx/blended_flask/utils.py` & `blendedux-0.1.2/blendedUx/blended_flask/utils.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.1.1/setup.py` & `blendedux-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'A cross-platform design theme framework.'
 
 
 
 # Setting up
 setup(
     name="blendedux",
@@ -34,10 +34,10 @@
         'MarkupSafe==2.1.2',
         'Pillow==9.5.0',
         'python-dateutil==2.8.2',
         'six==1.16.0',
         'urllib3==1.26.15',
         'Werkzeug==2.2.3',
         'blinker==1.6.2',
-        'blendedUx-Lang==1.1.0'
+        'blendedUx-Lang==1.1.1'
     ]
 )
```

