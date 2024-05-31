# Comparing `tmp/djehuty-24.4.tar.gz` & `tmp/djehuty-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djehuty-24.4.tar", last modified: Fri Apr 26 13:35:33 2024, max compression
+gzip compressed data, was "djehuty-24.5.tar", last modified: Fri May 31 09:51:51 2024, max compression
```

## Comparing `djehuty-24.4.tar` & `djehuty-24.5.tar`

### file list

```diff
@@ -1,347 +1,348 @@
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.559275 djehuty-24.4/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      689 2024-02-01 14:42:06.000000 djehuty-24.4/LICENSE
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      390 2024-02-01 14:42:06.000000 djehuty-24.4/MANIFEST.in
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3553 2024-04-26 13:35:33.559275 djehuty-24.4/PKG-INFO
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2894 2024-02-01 14:42:06.000000 djehuty-24.4/README.md
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.532276 djehuty-24.4/doc/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6256 2024-02-01 14:42:06.000000 djehuty-24.4/doc/contributing.tex
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6289 2024-04-26 13:34:55.000000 djehuty-24.4/doc/djehuty.sty
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6146 2024-02-01 14:42:06.000000 djehuty-24.4/doc/djehuty.tex
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/doc/figures/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13201 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/account.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14498 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/dataset-container.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17205 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/dataset.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13387 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/funding.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    97787 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/logo.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14790 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/rdf-list-abbrev.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    28697 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/references-graph.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9279 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/typed-literals-notation.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8596 2024-02-01 14:42:06.000000 djehuty-24.4/doc/figures/typed-notation.pdf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3436 2024-02-01 14:42:06.000000 djehuty-24.4/doc/introduction.tex
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4689 2024-02-01 14:42:06.000000 djehuty-24.4/doc/knowledge-graph.tex
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      719 2024-02-01 14:42:06.000000 djehuty-24.4/doc/references.bib
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/etc/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/etc/djehuty/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3616 2024-04-24 20:01:44.000000 djehuty-24.4/etc/djehuty/djehuty-example-config.xml
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      338 2024-04-24 20:01:44.000000 djehuty-24.4/etc/djehuty.service
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      834 2024-04-26 13:34:55.000000 djehuty-24.4/pyproject.toml
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.530276 djehuty-24.4/rpmbuild/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/rpmbuild/SPECS/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1366 2024-04-26 13:34:55.000000 djehuty-24.4/rpmbuild/SPECS/djehuty.spec
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       38 2024-04-26 13:35:33.559275 djehuty-24.4/setup.cfg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       92 2024-02-01 14:42:06.000000 djehuty-24.4/setup.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.531276 djehuty-24.4/src/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.533276 djehuty-24.4/src/djehuty/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/__init__.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.534276 djehuty-24.4/src/djehuty/backup/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    54348 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/database.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    23959 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/figshare.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.535276 djehuty-24.4/src/djehuty/backup/resources/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   947483 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/contributors_organizations.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4941 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/dois.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3073 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/groups.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4870 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/languages.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4397 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/licenses.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    59038 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/public_collections.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    31365 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/resources/root_categories.json
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8742 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/backup/ui.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6304 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/ui.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.535276 djehuty-24.4/src/djehuty/utils/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2084 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/utils/constants.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8336 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/utils/convenience.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6595 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/utils/rdf.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.536276 djehuty-24.4/src/djehuty/web/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4162 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/cache.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   146479 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/database.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3011 2024-03-08 13:06:17.000000 djehuty-24.4/src/djehuty/web/email_handler.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    26886 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/formatter.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1431 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/locks.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.531276 djehuty-24.4/src/djehuty/web/resources/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.538276 djehuty-24.4/src/djehuty/web/resources/html_templates/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      100 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/400.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      117 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/403.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      122 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/404.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      137 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/410.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1041 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/activate_2fa_session.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.539276 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      702 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/dashboard.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1666 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/exploratory.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2637 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/maintenance.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2119 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/quota_requests.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.539276 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1915 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/dashboard.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2249 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/embargoed_datasets.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2091 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/restricted_datasets.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1616 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/sparql.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2778 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/admin/users.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5068 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/author.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1966 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/badge.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4651 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/categories.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2053 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/category.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      695 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/collection.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2790 2024-04-26 13:32:51.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/colors.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4530 2024-04-26 13:32:51.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/dataset.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1176 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/dataset_access_request.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.540276 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1092 2024-02-15 12:37:40.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/collection-private-links.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4216 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/dashboard.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1450 2024-02-15 12:37:40.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/dataset-private-links.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13903 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-collection.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    31761 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-dataset.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2405 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-session.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8403 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/language-selector.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3319 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/my-collections.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4959 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/my-data.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2263 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/new_private_link.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5658 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/profile.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      572 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/published-collection.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      625 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/submitted-for-review.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.542276 djehuty-24.4/src/djehuty/web/resources/html_templates/email/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      188 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/2fa_token.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      129 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/2fa_token.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      450 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/data_access_request.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      334 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/data_access_request.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      887 2024-04-26 13:03:07.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_approved.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      691 2024-04-26 13:03:07.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_approved.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      401 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_declined.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      274 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_declined.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      557 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_submitted.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      412 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_submitted.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      291 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/declined_dataset_notification.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      158 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/declined_dataset_notification.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      209 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/feedback.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      128 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/feedback.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      345 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/layout.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      292 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/published_dataset_notification.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      159 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/published_dataset_notification.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      439 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/quota_approved.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      316 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/quota_approved.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      317 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/quota_request.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      212 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/quota_request.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      451 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      319 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2910 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/feedback.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      256 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/git_instructions.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4465 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/institutions.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6362 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/layout.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3547 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/loader.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      162 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/maintenance.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1585 2024-03-12 09:27:51.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/opendap_to_doi.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11949 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/portal.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      180 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/private_link_is_expired.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13781 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/public_metadata.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.542276 djehuty-24.4/src/djehuty/web/resources/html_templates/review/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5734 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/review/overview.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      479 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/review/published.html
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    15954 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/html_templates/search.html
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.549276 djehuty-24.4/src/djehuty/web/resources/sparql_templates/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1775 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_by_email.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2145 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_by_session_token.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      969 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_categories.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1074 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_sessions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      700 2024-03-12 07:51:39.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_storage_used.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      438 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_uuid_by_orcid.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3493 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/accounts.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      387 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/append_to_list.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      641 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/associated_authors.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1800 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/author_profile.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1349 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/author_public_items.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3119 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/authors.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2209 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/categories.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      555 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/categories_tree.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      660 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/category_by_id.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1624 2024-02-22 12:19:50.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collaborators.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      212 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_dataset_containers.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      867 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_datasets.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      301 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_datasets_count.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      908 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_versions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5885 2024-03-12 07:51:39.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      596 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections_by_account.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      809 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections_from_dataset.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      423 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/contact_info_from_container.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1534 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/container.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1906 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/container_items.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      348 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/container_uuid_by_id.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1282 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/custom_fields.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3555 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_files.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      277 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_is_under_review.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1214 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_statistics.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      781 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_statistics_timeline.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      374 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_storage_used.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      919 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_versions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    10888 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/datasets.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      634 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/datasets_missing_dois.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1007 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/decline_draft_dataset.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      347 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_account_property.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1038 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_associations.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1101 2024-02-22 12:19:50.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_collaborator.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      870 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_collection_draft.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      826 2024-03-12 07:51:39.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_dataset_draft.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      816 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_dataset_embargo.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      382 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_inactive_session_by_uuid.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      813 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_item_categories.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      760 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_item_from_list.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      647 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_items_all_from_list.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      852 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_private_links.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      365 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_session.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      421 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_session_by_uuid.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      276 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_sessions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      251 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/derived_from.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      249 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/explorer_properties.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      336 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/explorer_property_types.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      179 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/explorer_types.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1457 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/funding.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      547 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/group.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      490 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/group_by_name.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1000 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/item_collaborative_permissions.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      629 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/latest_datasets_portal.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      476 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/licenses.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      609 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/missing_checksummed_files_for_container.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1274 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/opendap_to_doi.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      254 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/prefixes.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1155 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/private_links.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2418 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/publish_draft_collection.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2827 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/publish_draft_dataset.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      945 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/quota_requests.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      232 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/record_uri.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1188 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/references.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3263 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/reviews.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      703 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/root_categories.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      463 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/search_tags.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      389 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      329 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics_authors.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      485 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics_collections.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      473 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics_datasets.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      955 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics_files.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      718 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1332 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/tags.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5688 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_account.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1982 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_author.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5781 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_collection.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11656 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_dataset.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1022 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_dataset_thumb.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      422 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_doi_after_publishing.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4214 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_file.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      560 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_git_uuid.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      846 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_orcid_for_account.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1670 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_private_link.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1696 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_quota_request.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1279 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_review.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1008 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_session.sparql
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1699 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_view_and_download_counts.sparql
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.531276 djehuty-24.4/src/djehuty/web/resources/static/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.549276 djehuty-24.4/src/djehuty/web/resources/static/css/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9840 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/css/dropzone.min.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5058 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/static/css/form.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13823 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/css/jquery.dataTables.min.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    16381 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/static/css/main.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3791 2024-04-26 13:32:51.000000 djehuty-24.4/src/djehuty/web/resources/static/css/pub.css
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    24375 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/css/quill.4tu.css
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.552276 djehuty-24.4/src/djehuty/web/resources/static/fonts/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   174632 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/FiraMono-Regular.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   247784 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Bold.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   109604 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Italic.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   248504 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Regular.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   208302 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.eot
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   207972 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   120496 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.woff
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   117400 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.woff2
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   420030 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.eot
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   419720 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.ttf
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   170112 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.woff
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   156496 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.woff2
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.553276 djehuty-24.4/src/djehuty/web/resources/static/images/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   136306 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/CoreTrustSeal.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1838 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/collection-thumb.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3137 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/dataset-thumb.svg
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.554276 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      160 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_asc.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      148 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_asc_disabled.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      201 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_both.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      158 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_desc.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      146 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/datatables/sort_desc_disabled.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1817 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/ext-link.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   156038 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/favicon.ico
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3519 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/favicon.png
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.554276 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5427 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/apache.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2672 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-0.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1773 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc-nd.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1888 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc-sa.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1709 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1562 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nd.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1697 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-sa.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1468 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2666 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/licenses/gnu-gpl-v3.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13671 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-delft.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5737 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-eindhoven.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    29080 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-gray.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4815 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-other.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     7852 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-twente.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4593 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo-wageningen.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17172 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logo.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      539 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tudelft.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      479 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tueindhoven.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      920 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tutwente.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      764 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-wageningen.png
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2311 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/nikhef-black.svg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      967 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/orcid.svg
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.557276 djehuty-24.4/src/djehuty/web/resources/static/images/portal/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    45036 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/aerospace-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    56826 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/agricultural-and-veterinary-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    32670 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/atmospheric-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    64498 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/biology.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    67098 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/built-environment-and-design.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    48523 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/business-and-management.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    74133 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/chemistry.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    45270 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/civil-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    56936 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/earth-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    57174 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/electrical-and-electronic-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    46321 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/environmental-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    47125 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/geomatic-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    81026 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/information-and-computing-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    71960 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/materials-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    43103 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/mathematics.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    40696 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/mechanical-engineering.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    46816 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/medical-and-health-sciences.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    75625 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/nanotechnology.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8616 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/other-institutions.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    38216 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/physical-geography-and-environmental-geoscience.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    50449 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/physics.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13023 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/tudelft.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17442 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/tueindhoven.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9400 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/utwente.jpg
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    16609 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/images/portal/wageningen.jpg
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.558276 djehuty-24.4/src/djehuty/web/resources/static/js/
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.559275 djehuty-24.4/src/djehuty/web/resources/static/js/ace/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   371331 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/ace.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    39763 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/ext-language_tools.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11910 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/ext-searchbox.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8183 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/mode-sparql.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3150 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ace/theme-crimson_editor.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   275533 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/d3.v7.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2556 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/dataset_landing_page.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1427 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/depositor-dashboard.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   114702 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/dropzone.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    24869 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/edit-collection.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    61653 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/static/js/edit-dataset.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3600 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/edit-profile.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6093 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/exploratory.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    89501 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    88377 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/jquery.dataTables.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3519 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/query-editor.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   327924 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/quill.min.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3027 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/resources/static/js/ranking.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4167 2024-03-08 13:06:17.000000 djehuty-24.4/src/djehuty/web/resources/static/js/review-overview.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    29712 2024-03-27 09:02:41.000000 djehuty-24.4/src/djehuty/web/resources/static/js/search.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8788 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/resources/static/js/utils.js
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    47651 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/ui.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    16169 2024-03-08 13:06:17.000000 djehuty-24.4/src/djehuty/web/validator.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   415838 2024-04-24 20:01:44.000000 djehuty-24.4/src/djehuty/web/wsgi.py
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14835 2024-02-01 14:42:06.000000 djehuty-24.4/src/djehuty/web/xml_formatter.py
-drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-04-26 13:35:33.559275 djehuty-24.4/src/djehuty.egg-info/
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3553 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/PKG-INFO
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    18514 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/SOURCES.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        1 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/dependency_links.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       44 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/entry_points.txt
--rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        8 2024-04-26 13:35:33.000000 djehuty-24.4/src/djehuty.egg-info/top_level.txt
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.062121 djehuty-24.5/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      689 2024-02-01 14:42:06.000000 djehuty-24.5/LICENSE
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      390 2024-02-01 14:42:06.000000 djehuty-24.5/MANIFEST.in
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3553 2024-05-31 09:51:51.061121 djehuty-24.5/PKG-INFO
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2894 2024-02-01 14:42:06.000000 djehuty-24.5/README.md
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.914127 djehuty-24.5/doc/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6256 2024-02-01 14:42:06.000000 djehuty-24.5/doc/contributing.tex
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6289 2024-05-31 09:51:19.000000 djehuty-24.5/doc/djehuty.sty
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6146 2024-02-01 14:42:06.000000 djehuty-24.5/doc/djehuty.tex
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.915127 djehuty-24.5/doc/figures/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13201 2024-02-01 14:42:06.000000 djehuty-24.5/doc/figures/account.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14498 2024-02-01 14:42:06.000000 djehuty-24.5/doc/figures/dataset-container.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17205 2024-02-01 14:42:06.000000 djehuty-24.5/doc/figures/dataset.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13387 2024-02-01 14:42:06.000000 djehuty-24.5/doc/figures/funding.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    97787 2024-02-01 14:42:06.000000 djehuty-24.5/doc/figures/logo.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14790 2024-02-01 14:42:06.000000 djehuty-24.5/doc/figures/rdf-list-abbrev.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    28697 2024-02-01 14:42:06.000000 djehuty-24.5/doc/figures/references-graph.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9279 2024-02-01 14:42:06.000000 djehuty-24.5/doc/figures/typed-literals-notation.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8596 2024-02-01 14:42:06.000000 djehuty-24.5/doc/figures/typed-notation.pdf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3436 2024-02-01 14:42:06.000000 djehuty-24.5/doc/introduction.tex
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4689 2024-02-01 14:42:06.000000 djehuty-24.5/doc/knowledge-graph.tex
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      719 2024-02-01 14:42:06.000000 djehuty-24.5/doc/references.bib
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.915127 djehuty-24.5/etc/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.915127 djehuty-24.5/etc/djehuty/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3616 2024-04-24 20:01:44.000000 djehuty-24.5/etc/djehuty/djehuty-example-config.xml
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      338 2024-04-24 20:01:44.000000 djehuty-24.5/etc/djehuty.service
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      834 2024-05-31 09:51:19.000000 djehuty-24.5/pyproject.toml
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.909127 djehuty-24.5/rpmbuild/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.916127 djehuty-24.5/rpmbuild/SPECS/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1366 2024-05-31 09:51:19.000000 djehuty-24.5/rpmbuild/SPECS/djehuty.spec
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       38 2024-05-31 09:51:51.062121 djehuty-24.5/setup.cfg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       92 2024-02-01 14:42:06.000000 djehuty-24.5/setup.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.910127 djehuty-24.5/src/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.916127 djehuty-24.5/src/djehuty/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/__init__.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.917127 djehuty-24.5/src/djehuty/backup/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    54454 2024-04-30 18:24:52.000000 djehuty-24.5/src/djehuty/backup/database.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    23959 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/backup/figshare.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.918126 djehuty-24.5/src/djehuty/backup/resources/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   947483 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/backup/resources/contributors_organizations.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4941 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/backup/resources/dois.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3073 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/backup/resources/groups.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4870 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/backup/resources/languages.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5045 2024-04-30 18:24:52.000000 djehuty-24.5/src/djehuty/backup/resources/licenses.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    59038 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/backup/resources/public_collections.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    31365 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/backup/resources/root_categories.json
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8742 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/backup/ui.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6304 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/ui.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.919126 djehuty-24.5/src/djehuty/utils/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2084 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/utils/constants.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9104 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/utils/convenience.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     7566 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/utils/rdf.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.920127 djehuty-24.5/src/djehuty/web/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4162 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/cache.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   147486 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/web/database.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3011 2024-03-08 13:06:17.000000 djehuty-24.5/src/djehuty/web/email_handler.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    26886 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/formatter.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1431 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/locks.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.912127 djehuty-24.5/src/djehuty/web/resources/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.924126 djehuty-24.5/src/djehuty/web/resources/html_templates/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      100 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/400.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      117 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/403.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      122 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/404.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      137 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/410.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      586 2024-04-29 09:44:21.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/activate_2fa_session.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.925126 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      585 2024-04-30 06:11:46.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/dashboard.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1666 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/exploratory.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2395 2024-04-30 06:11:46.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/maintenance.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2119 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/quota_requests.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.926126 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/reports/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1915 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/reports/dashboard.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2249 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/reports/embargoed_datasets.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2091 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/reports/restricted_datasets.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1616 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/sparql.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2778 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/admin/users.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5067 2024-04-30 06:11:46.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/author.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1966 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/badge.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3081 2024-04-29 09:44:21.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/categories.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      983 2024-04-29 09:44:21.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/category.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      695 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/collection.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2930 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/colors.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4557 2024-05-08 12:30:11.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/dataset.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1176 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/dataset_access_request.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.927126 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1092 2024-02-15 12:37:40.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/collection-private-links.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4551 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/dashboard.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1450 2024-02-15 12:37:40.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/dataset-private-links.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13903 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/edit-collection.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    32134 2024-05-13 13:46:19.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/edit-dataset.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2405 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/edit-session.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8403 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/language-selector.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3319 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/my-collections.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4959 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/my-data.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2263 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/new_private_link.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5658 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/profile.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      572 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/published-collection.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      625 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/submitted-for-review.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.931126 djehuty-24.5/src/djehuty/web/resources/html_templates/email/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      188 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/2fa_token.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      129 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/2fa_token.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      450 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/data_access_request.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      334 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/data_access_request.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1149 2024-05-16 11:56:14.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/dataset_approved.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      940 2024-05-16 11:56:14.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/dataset_approved.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      401 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/dataset_declined.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      274 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/dataset_declined.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      588 2024-05-07 05:10:19.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/dataset_submitted.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      404 2024-05-07 05:10:19.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/dataset_submitted.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      291 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/declined_dataset_notification.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      158 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/declined_dataset_notification.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      209 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/feedback.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      128 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/feedback.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      345 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/layout.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      292 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/published_dataset_notification.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      159 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/published_dataset_notification.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      439 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/quota_approved.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      316 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/quota_approved.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      317 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/quota_request.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      212 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/quota_request.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      451 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      319 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/email/submitted_for_review_notification.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2479 2024-04-29 12:14:55.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/feedback.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      256 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/git_instructions.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2287 2024-04-29 09:44:21.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/institutions.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6396 2024-04-29 09:44:21.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/layout.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3547 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/loader.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      162 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/maintenance.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1585 2024-03-12 09:27:51.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/opendap_to_doi.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11949 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/portal.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      180 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/private_link_is_expired.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13550 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/public_metadata.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.931126 djehuty-24.5/src/djehuty/web/resources/html_templates/review/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5734 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/review/overview.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      479 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/review/published.html
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    15653 2024-04-29 09:44:21.000000 djehuty-24.5/src/djehuty/web/resources/html_templates/search.html
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.014123 djehuty-24.5/src/djehuty/web/resources/sparql_templates/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1775 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_by_email.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2145 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_by_session_token.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      969 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_categories.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1074 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_sessions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      700 2024-03-12 07:51:39.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_storage_used.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      438 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_uuid_by_orcid.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3493 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/accounts.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      387 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/append_to_list.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      641 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/associated_authors.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1800 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/author_profile.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1307 2024-05-07 05:10:19.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/author_public_items.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3119 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/authors.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2209 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/categories.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      555 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/categories_tree.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      660 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/category_by_id.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1624 2024-02-22 12:19:50.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/collaborators.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      212 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/collection_dataset_containers.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      867 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/collection_datasets.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      301 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/collection_datasets_count.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      908 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/collection_versions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5885 2024-03-12 07:51:39.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/collections.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      596 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/collections_by_account.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      809 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/collections_from_dataset.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      423 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/contact_info_from_container.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1534 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/container.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1906 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/container_items.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      348 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/container_uuid_by_id.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1282 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/custom_fields.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3555 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_files.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      277 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_is_under_review.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1214 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_statistics.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      781 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_statistics_timeline.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      374 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_storage_used.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      919 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_versions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11173 2024-05-08 12:30:11.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/datasets.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      634 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/datasets_missing_dois.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1007 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/decline_draft_dataset.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      347 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_account_property.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1038 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_associations.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1101 2024-02-22 12:19:50.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_collaborator.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      870 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_collection_draft.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      826 2024-03-12 07:51:39.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_dataset_draft.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      816 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_dataset_embargo.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      382 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_inactive_session_by_uuid.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      813 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_item_categories.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      760 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_item_from_list.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      647 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_items_all_from_list.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      852 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_private_links.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      365 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_session.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      421 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_session_by_uuid.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      276 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_sessions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      251 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/derived_from.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      249 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/explorer_properties.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      336 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/explorer_property_types.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      179 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/explorer_types.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1457 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/funding.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      547 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/group.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      490 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/group_by_name.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1000 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/item_collaborative_permissions.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      629 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/latest_datasets_portal.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      476 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/licenses.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      609 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/missing_checksummed_files_for_container.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1274 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/opendap_to_doi.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      254 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/prefixes.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1344 2024-05-02 14:16:23.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/private_links.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2418 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/publish_draft_collection.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2827 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/publish_draft_dataset.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1043 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/quota_requests.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      232 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/record_uri.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1188 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/references.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3263 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/reviews.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      703 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/root_categories.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      463 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/search_tags.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      389 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/statistics.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      329 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/statistics_authors.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      485 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/statistics_collections.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      394 2024-05-02 14:16:23.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/statistics_datalink.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      473 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/statistics_datasets.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      955 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/statistics_files.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      718 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1332 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/tags.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5688 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_account.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1982 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_author.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5781 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_collection.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11997 2024-05-08 12:30:11.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_dataset.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1022 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_dataset_thumb.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      422 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_doi_after_publishing.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4214 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_file.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      560 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_git_uuid.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      846 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_orcid_for_account.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1670 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_private_link.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1696 2024-03-27 09:02:41.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_quota_request.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1279 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_review.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1008 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_session.sparql
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1699 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_view_and_download_counts.sparql
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:50.912127 djehuty-24.5/src/djehuty/web/resources/static/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.015123 djehuty-24.5/src/djehuty/web/resources/static/css/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9840 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/css/dropzone.min.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5058 2024-04-24 20:01:44.000000 djehuty-24.5/src/djehuty/web/resources/static/css/form.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13823 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17934 2024-04-29 09:44:21.000000 djehuty-24.5/src/djehuty/web/resources/static/css/main.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3784 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/web/resources/static/css/pub.css
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    24375 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/css/quill.4tu.css
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.023123 djehuty-24.5/src/djehuty/web/resources/static/fonts/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   174632 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/FiraMono-Regular.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   247784 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/SourceSansPro-Bold.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   109604 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/SourceSansPro-Italic.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   248504 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/SourceSansPro-Regular.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   208302 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-brands-400.eot
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   207972 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-brands-400.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   120496 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-brands-400.woff
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   117400 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-brands-400.woff2
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   420030 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-solid-900.eot
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   419720 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-solid-900.ttf
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   170112 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-solid-900.woff
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   156496 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-solid-900.woff2
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.035122 djehuty-24.5/src/djehuty/web/resources/static/images/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   136306 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/CoreTrustSeal.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1838 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/collection-thumb.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3137 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/dataset-thumb.svg
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.038122 djehuty-24.5/src/djehuty/web/resources/static/images/datatables/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      160 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/datatables/sort_asc.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      148 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/datatables/sort_asc_disabled.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      201 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/datatables/sort_both.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      158 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/datatables/sort_desc.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      146 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/datatables/sort_desc_disabled.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1817 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/ext-link.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   156038 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/favicon.ico
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3519 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/favicon.png
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.042122 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5427 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/apache.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2672 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-0.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1773 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-nc-nd.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1888 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-nc-sa.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1709 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-nc.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1562 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-nd.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1697 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-sa.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1468 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2666 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/licenses/gnu-gpl-v3.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13671 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logo-delft.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     5737 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logo-eindhoven.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    29080 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logo-gray.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4815 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logo-other.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     7852 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logo-twente.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4593 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logo-wageningen.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17172 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logo.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      539 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logosleft-white-tudelft.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      479 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logosleft-white-tueindhoven.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      920 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logosleft-white-tutwente.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      764 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/logosleft-white-wageningen.png
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2311 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/nikhef-black.svg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)      967 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/orcid.svg
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.050122 djehuty-24.5/src/djehuty/web/resources/static/images/portal/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    45036 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/aerospace-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    56826 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/agricultural-and-veterinary-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    32670 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/atmospheric-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    64498 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/biology.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    67098 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/built-environment-and-design.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    48523 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/business-and-management.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    74133 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/chemistry.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    45270 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/civil-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    56936 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/earth-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    57174 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/electrical-and-electronic-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    46321 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/environmental-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    47125 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/geomatic-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    81026 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/information-and-computing-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    71960 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/materials-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    43103 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/mathematics.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    40696 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/mechanical-engineering.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    46816 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/medical-and-health-sciences.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    75625 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/nanotechnology.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8616 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/other-institutions.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    38216 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/physical-geography-and-environmental-geoscience.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    50449 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/physics.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    13023 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/tudelft.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    17442 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/tueindhoven.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     9400 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/utwente.jpg
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    16609 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/images/portal/wageningen.jpg
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.055122 djehuty-24.5/src/djehuty/web/resources/static/js/
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.059121 djehuty-24.5/src/djehuty/web/resources/static/js/ace/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   371331 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/ace/ace.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    39763 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/ace/ext-language_tools.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    11910 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/ace/ext-searchbox.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8183 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/ace/mode-sparql.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3150 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/ace/theme-crimson_editor.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   275533 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/d3.v7.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     2560 2024-04-29 12:14:55.000000 djehuty-24.5/src/djehuty/web/resources/static/js/dataset_landing_page.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     1599 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/web/resources/static/js/depositor-dashboard.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   114702 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/dropzone.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    24875 2024-04-29 12:14:55.000000 djehuty-24.5/src/djehuty/web/resources/static/js/edit-collection.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    61702 2024-05-08 12:30:11.000000 djehuty-24.5/src/djehuty/web/resources/static/js/edit-dataset.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3602 2024-04-29 12:14:55.000000 djehuty-24.5/src/djehuty/web/resources/static/js/edit-profile.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     6098 2024-04-29 12:14:55.000000 djehuty-24.5/src/djehuty/web/resources/static/js/exploratory.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    89501 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    88377 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3486 2024-04-30 06:20:34.000000 djehuty-24.5/src/djehuty/web/resources/static/js/query-editor.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   327924 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/resources/static/js/quill.min.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3030 2024-04-29 12:14:55.000000 djehuty-24.5/src/djehuty/web/resources/static/js/ranking.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     4168 2024-04-29 12:14:55.000000 djehuty-24.5/src/djehuty/web/resources/static/js/review-overview.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    27690 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/web/resources/static/js/search.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     8749 2024-04-29 12:14:55.000000 djehuty-24.5/src/djehuty/web/resources/static/js/utils.js
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    47965 2024-05-08 20:42:44.000000 djehuty-24.5/src/djehuty/web/ui.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    18203 2024-05-02 14:16:23.000000 djehuty-24.5/src/djehuty/web/validator.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)   422497 2024-05-31 09:50:01.000000 djehuty-24.5/src/djehuty/web/wsgi.py
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    14835 2024-02-01 14:42:06.000000 djehuty-24.5/src/djehuty/web/xml_formatter.py
+drwxr-xr-x   0 rrejanssen  (1000) rrejanssen  (1000)        0 2024-05-31 09:51:51.060121 djehuty-24.5/src/djehuty.egg-info/
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)     3553 2024-05-31 09:51:50.000000 djehuty-24.5/src/djehuty.egg-info/PKG-INFO
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)    18584 2024-05-31 09:51:50.000000 djehuty-24.5/src/djehuty.egg-info/SOURCES.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        1 2024-05-31 09:51:50.000000 djehuty-24.5/src/djehuty.egg-info/dependency_links.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)       44 2024-05-31 09:51:50.000000 djehuty-24.5/src/djehuty.egg-info/entry_points.txt
+-rw-r--r--   0 rrejanssen  (1000) rrejanssen  (1000)        8 2024-05-31 09:51:50.000000 djehuty-24.5/src/djehuty.egg-info/top_level.txt
```

### Comparing `djehuty-24.4/LICENSE` & `djehuty-24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/PKG-INFO` & `djehuty-24.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djehuty
-Version: 24.4
+Version: 24.5
 Summary: The 4TU.ResearchData repository system
 Author-email: Roel Janssen <r.r.e.janssen@tudelft.nl>
 Project-URL: Homepage, https://data.4tu.nl
 Project-URL: Source Code, https://github.com/4TUResearchData/djehuty
 Project-URL: Bug Tracker, https://github.com/4TUResearchData/djehuty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `djehuty-24.4/README.md` & `djehuty-24.5/README.md`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/contributing.tex` & `djehuty-24.5/doc/contributing.tex`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/djehuty.sty` & `djehuty-24.5/doc/djehuty.sty`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 \definecolor{DarkGray}{rgb}{0.40, 0.40, 0.40}
 
 % When highlighting text, make sure the highlighting box doesn't
 % add padding space.
 \setlength{\fboxsep}{0pt}
 
 %% Create a variable that holds the current version of djehuty.
-\def \djehutyversion {24.4}
+\def \djehutyversion {24.5}
 
 \newcommand\VRule[1][\arrayrulewidth]{\vrule width #1}
 \newcommand{\oddcell}{\cellcolor{OddRowColor}}
 \newcommand{\oddrow}{\rowcolor{OddRowColor}}
 \newcommand{\evenrow}{\rowcolor{EvenRowColor}}
 \newcommand{\headrow}{\rowcolor{Gray}}
 \newcommand{\B}{$\bullet{}$}
```

### Comparing `djehuty-24.4/doc/djehuty.tex` & `djehuty-24.5/doc/djehuty.tex`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/figures/account.pdf` & `djehuty-24.5/doc/figures/account.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/figures/dataset-container.pdf` & `djehuty-24.5/doc/figures/dataset-container.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/figures/dataset.pdf` & `djehuty-24.5/doc/figures/dataset.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/figures/funding.pdf` & `djehuty-24.5/doc/figures/funding.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/figures/logo.pdf` & `djehuty-24.5/doc/figures/logo.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/figures/rdf-list-abbrev.pdf` & `djehuty-24.5/doc/figures/rdf-list-abbrev.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/figures/references-graph.pdf` & `djehuty-24.5/doc/figures/references-graph.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/figures/typed-literals-notation.pdf` & `djehuty-24.5/doc/figures/typed-literals-notation.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/figures/typed-notation.pdf` & `djehuty-24.5/doc/figures/typed-notation.pdf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/introduction.tex` & `djehuty-24.5/doc/introduction.tex`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/knowledge-graph.tex` & `djehuty-24.5/doc/knowledge-graph.tex`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/doc/references.bib` & `djehuty-24.5/doc/references.bib`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/etc/djehuty/djehuty-example-config.xml` & `djehuty-24.5/etc/djehuty/djehuty-example-config.xml`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/pyproject.toml` & `djehuty-24.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend   = "setuptools.build_meta"
 
 [project]
 name            = "djehuty"
-version         = "24.4"
+version         = "24.5"
 authors         = [{ name="Roel Janssen", email="r.r.e.janssen@tudelft.nl" }]
 description     = "The 4TU.ResearchData repository system"
 readme          = "README.md"
 requires-python = ">=3.7"
 classifiers     = [
     "Programming Language :: Python :: 3",
     "Environment :: Web Environment",
```

### Comparing `djehuty-24.4/rpmbuild/SPECS/djehuty.spec` & `djehuty-24.5/rpmbuild/SPECS/djehuty.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:        djehuty
-Version:     24.4
+Version:     24.5
 Release:     1%{?dist}
 Summary:     Repository system for 4TU.ResearchData
 Source0:     %{name}-%{version}.tar.gz
 License:     AGPLv3+
 Group:       System Environment/Daemons
 BuildRoot:   %{_tmppath}/%{name}-%{version}-%{release}-buildroot
 Prefix:      %{_prefix}
@@ -44,11 +44,11 @@
 %clean
 rm -rf $RPM_BUILD_ROOT
 
 %files
 %defattr(-,root,root)
 %doc README.md
 %{python3_sitelib}/%{name}/
-%{python3_sitelib}/%{name}-24.4*
+%{python3_sitelib}/%{name}-24.5*
 %{_unitdir}/%{name}.service
 /etc/%{name}/djehuty-example-config.xml
 /usr/bin/djehuty
```

### Comparing `djehuty-24.4/src/djehuty/backup/database.py` & `djehuty-24.5/src/djehuty/backup/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -657,14 +657,16 @@
             if license_spdx is not None:
                 self.store.add ((license_uri, rdf.DJHT["spdx"],
                                  URIRef(license_spdx)))
 
             license_type_uri = None
             if license_type == "software":
                 license_type_uri = rdf.DJHT["SoftwareLicense"]
+            if license_type == "hardware":
+                license_type_uri = rdf.DJHT["HardwareLicense"]
             elif license_type == "data":
                 license_type_uri = rdf.DJHT["DataLicense"]
             elif license_type == "legacy":
                 license_type_uri = rdf.DJHT["LegacyLicense"]
 
             rdf.add (self.store, license_uri, rdf.DJHT["type"], license_type_uri, "url")
             rdf.add (self.store, license_type_uri, RDFS.label,  license_type, XSD.string)
```

### Comparing `djehuty-24.4/src/djehuty/backup/figshare.py` & `djehuty-24.5/src/djehuty/backup/figshare.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/backup/resources/contributors_organizations.json` & `djehuty-24.5/src/djehuty/backup/resources/contributors_organizations.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/backup/resources/dois.json` & `djehuty-24.5/src/djehuty/backup/resources/dois.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/backup/resources/groups.json` & `djehuty-24.5/src/djehuty/backup/resources/groups.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/backup/resources/languages.json` & `djehuty-24.5/src/djehuty/backup/resources/languages.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/backup/resources/licenses.json` & `djehuty-24.5/src/djehuty/backup/resources/licenses.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {'insert': "[(0, OrderedDict([('url', 'https://opensource.org/license/cern-ohl-s'), ('value', "*

 * *           "996), ('name', 'CERN-OHL-S-2.0'), ('spdx', "*

 * *           "'https://spdx.org/licenses/CERN-OHL-S-2.0'), ('type', 'hardware')])), (1, "*

 * *           "OrderedDict([('url', 'https://opensource.org/license/cern-ohl-w'), ('value', 995), "*

 * *           "('name', 'CERN-OHL-W-2.0'), ('spdx', 'https://spdx.org/licenses/CERN-OHL-W-2.0'), "*

 * *           "('type', 'hardware')])), (2, OrderedDict([('url', "*

 * *           "'h […]*

```diff
@@ -1,9 +1,30 @@
 [
     {
+        "name": "CERN-OHL-S-2.0",
+        "spdx": "https://spdx.org/licenses/CERN-OHL-S-2.0",
+        "type": "hardware",
+        "url": "https://opensource.org/license/cern-ohl-s",
+        "value": 996
+    },
+    {
+        "name": "CERN-OHL-W-2.0",
+        "spdx": "https://spdx.org/licenses/CERN-OHL-W-2.0",
+        "type": "hardware",
+        "url": "https://opensource.org/license/cern-ohl-w",
+        "value": 995
+    },
+    {
+        "name": "CERN-OHL-P-2.0",
+        "spdx": "https://spdx.org/licenses/CERN-OHL-P-2.0",
+        "type": "hardware",
+        "url": "https://opensource.org/license/cern-ohl-p",
+        "value": 994
+    },
+    {
         "name": "EUPL-1.2",
         "spdx": "https://spdx.org/licenses/EUPL-1.2",
         "type": "software",
         "url": "https://opensource.org/licenses/EUPL-1.2",
         "value": 99
     },
     {
```

### Comparing `djehuty-24.4/src/djehuty/backup/resources/public_collections.json` & `djehuty-24.5/src/djehuty/backup/resources/public_collections.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/backup/resources/root_categories.json` & `djehuty-24.5/src/djehuty/backup/resources/root_categories.json`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/backup/ui.py` & `djehuty-24.5/src/djehuty/backup/ui.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/ui.py` & `djehuty-24.5/src/djehuty/ui.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/utils/constants.py` & `djehuty-24.5/src/djehuty/utils/constants.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/utils/convenience.py` & `djehuty-24.5/src/djehuty/utils/convenience.py`

 * *Files 7% similar despite different names*

```diff
@@ -226,13 +226,32 @@
         parts[0] += '.'
     else:
         parts = name.split(' ', 1)
     parts = [part.strip() for part in parts]
     parts = ([''] + parts)[-2:]
     return parts
 
-def split_delimited_string (input_string, delimiter=","):
-    """Returns a list of strings from a delimited string."""
+def split_string (input_string, delimiter='\\s' , is_quoted=False, maxsplit=-1):
+    """Splits a string by a delimiter character and strips whitespace."""
     if not isinstance(input_string, str) or input_string == "":
         return None
+    if input_string.count(delimiter) == 0:
+        return [input_string]
+    regex_pattern = re.compile(fr'''((?:[^{delimiter}])+)''')
+    if is_quoted:
+        regex_pattern = re.compile(fr'''((?:[^{delimiter}"']|"[^"]*"|'[^']*')+)''')
+    words = regex_pattern.split(input_string)[1::2]
+    if maxsplit == 0:
+        return [input_string]
+    if 0 < maxsplit < len(words):
+        tmp_words = []
+        tmp_words = words[:maxsplit]
+        tmp_words.append(delimiter.join(words[maxsplit:]))
+        words = tmp_words
+    words[:] = [word.strip() for word in words]
+    words[:] = [word for word in words if word]
+    if is_quoted:
+        for index, word in enumerate(words):
+            if word[0] == word[-1] and word[0] in ['"', "'"]:
+                words[index] = word[1:-1]
 
-    return [item.strip() for item in input_string.split(delimiter)]
+    return words
```

### Comparing `djehuty-24.4/src/djehuty/utils/rdf.py` & `djehuty-24.5/src/djehuty/utils/rdf.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,14 +75,42 @@
         # Wrapping the xsd:string in STR ensures compatibility with Virtuoso.
         literal = f"STR({escape_value (value, XSD.string)})" if escape else value
         symbol  = f"STR(?{name})" if escape else f"?{name}"
         query  += f"FILTER ({symbol}={literal})\n"
 
     return query
 
+def sparql_contains_filter (names, values, lcase=True, andgate=False):
+    """Returns a FILTER statement for CONTAINS() with multiple names and values."""
+    query   = ""
+    names  = [names]  if isinstance(names,  str) and names  != "" else names
+    values = [values] if isinstance(values, str) and values != "" else values
+
+    if not isinstance(names, list) or not isinstance(values, list):
+        return query
+
+    if not values or not names:
+        return query
+
+    operator = "&&" if andgate else "||"
+
+    query = "FILTER ("
+    for name in names:
+        for value in values:
+            symbol  = f"STR(?{name})"
+            literal = f"STR({escape_value (value, XSD.string)})"
+            if lcase:
+                symbol  = f"LCASE(STR(?{name}))"
+                literal = f"STR({escape_value (value.lower(), XSD.string)})"
+            query  += f"CONTAINS({symbol},{literal}) {operator} "
+
+    query = query[:-len(operator) - 2] + ")"
+
+    return query
+
 def escape_value (value, datatype=None):
     """Returns VALUE wrapped in double quotes with type annotation DATATYPE."""
     if value is None:
         return None
 
     return Literal(value, datatype=datatype).n3()
```

### Comparing `djehuty-24.4/src/djehuty/web/cache.py` & `djehuty-24.5/src/djehuty/web/cache.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/database.py` & `djehuty-24.5/src/djehuty/web/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,20 @@
     def __insert_query_for_graph (self, graph):
         if self.enable_query_audit_log:
             query = rdf.insert_query (self.state_graph, graph)
             self.__log_query (query, "Query Audit Log")
             return query
         return rdf.insert_query (self.state_graph, graph)
 
+    def __last_item_by_order_index (self, results):
+        try:
+            return max(results, key = lambda item: item["order_index"])
+        except (ValueError, KeyError):
+            return None
+
     ## ------------------------------------------------------------------------
     ## GET METHODS
     ## ------------------------------------------------------------------------
 
     def dataset_storage_used (self, dataset_uuid):
         """Returns the number of bytes used by a dataset."""
 
@@ -294,17 +300,17 @@
             "item_uuid":      item_uuid,
             "is_latest":      is_latest,
             "is_published":   is_published
         })
 
         return self.__run_query (query)
 
-    def __search_query_to_sparql_filters (self, search_for, search_format):
+    def __search_query_to_sparql_filters_v2 (self, search_for, search_format):
         """
-        Procedure to parse search queries and return SPARQL FILTER statements.
+        Procedure to parse v2 search queries and return SPARQL FILTER statements.
         """
 
         filters = ""
         if search_for is None:
             return filters
 
         if isinstance (search_for, str):
@@ -369,18 +375,19 @@
         return filters
 
     def datasets (self, account_uuid=None, categories=None, collection_uri=None,
                   container_uuid=None, dataset_id=None, dataset_uuid=None, doi=None,
                   exclude_ids=None, groups=None, handle=None, institution=None,
                   is_latest=False, item_type=None, limit=None, modified_since=None,
                   offset=None, order=None, order_direction=None, published_since=None,
-                  resource_doi=None, return_count=False, search_for=None, search_format=False,
-                  version=None, is_published=True, is_under_review=None, git_uuid=None,
+                  resource_doi=None, return_count=False, search_for=None,
+                  search_format=False, version=None, search_scope=None,
+                  is_published=True, is_under_review=None, git_uuid=None,
                   private_link_id_string=None, use_cache=True, is_restricted=None,
-                  is_embargoed=None, is_software=None):
+                  is_embargoed=None, is_software=None, organizations=None):
         """Procedure to retrieve version(s) of datasets."""
 
         filters  = rdf.sparql_filter ("container_uri",  rdf.uuid_to_uri (container_uuid, "container"), is_uri=True)
         filters += rdf.sparql_filter ("dataset",        rdf.uuid_to_uri (dataset_uuid, "dataset"), is_uri=True)
         filters += rdf.sparql_filter ("institution_id", institution)
         filters += rdf.sparql_filter ("defined_type",   item_type)
         filters += rdf.sparql_filter ("dataset_id",     dataset_id)
@@ -390,15 +397,22 @@
         filters += rdf.sparql_filter ("doi",            doi,          escape=True)
         filters += rdf.sparql_filter ("handle",         handle,       escape=True)
         filters += rdf.sparql_filter ("is_restricted",          is_restricted)
         filters += rdf.sparql_filter ("is_embargoed",           is_embargoed)
         filters += rdf.sparql_filter ("private_link_id_string", private_link_id_string, escape=True)
         filters += rdf.sparql_in_filter ("group_id",    groups)
         filters += rdf.sparql_in_filter ("dataset_id", exclude_ids, negate=True)
-        filters += self.__search_query_to_sparql_filters (search_for, search_format)
+
+        filters += rdf.sparql_contains_filter("organizations", organizations)
+        filters += rdf.sparql_contains_filter("format", search_format)
+
+        if isinstance (search_for, dict):
+            filters += self.__search_query_to_sparql_filters_v2 (search_for, search_format)
+        else:
+            filters += rdf.sparql_contains_filter(search_scope, search_for)
 
         if is_software is not None:
             if is_software:
                 filters += rdf.sparql_filter ("defined_type_name", "software", escape=True)
             else:
                 filters += rdf.sparql_filter ("defined_type_name", "dataset", escape=True)
 
@@ -455,33 +469,50 @@
         })
 
         if use_cache:
             return self.__run_query (query, query, "repository_statistics")
 
         return self.__run_query (query)
 
+    def repository_datalink_statistics (self, use_cache=False):
+        """Returns datalink sizes."""
+
+        # Since the post-figshare djht:data_link_size is used.
+        filters = 'FILTER (?created > "2021-03-17"^^xsd:date)'
+        query = self.__query_from_template ("statistics_datalink", {
+            "filters": filters})
+
+        if use_cache:
+            return self.__run_query (query, query, "repository_statistics")
+
+        return self.__run_query (query)
+
     def repository_statistics (self):
         """Procedure to retrieve repository-wide statistics."""
 
         datasets_query    = self.__query_from_template ("statistics_datasets")
         collections_query = self.__query_from_template ("statistics_collections")
         authors_query     = self.__query_from_template ("statistics_authors")
 
         row = { "datasets": 0, "authors": 0, "collections": 0, "files": 0, "bytes": 0 }
         try:
             datasets    = self.__run_query (datasets_query, datasets_query, "repository_statistics")
             authors     = self.__run_query (authors_query, authors_query, "repository_statistics")
             collections = self.__run_query (collections_query, collections_query, "repository_statistics")
             files       = self.repository_file_statistics (use_cache=True)
+            datalinks   = self.repository_datalink_statistics (use_cache=True)
             number_of_files = 0
             number_of_bytes = 0
             for entry in files:
                 number_of_files += 1
                 number_of_bytes += int(float(entry["bytes"]))
 
+            for entry in datalinks:
+                number_of_bytes += int(float(entry["bytes"]))
+
             files_results = {
                 "files": number_of_files,
                 "bytes": number_of_bytes
             }
             row = { **datasets[0], **authors[0], **collections[0], **files_results }
         except (IndexError, KeyError):
             pass
@@ -1329,24 +1360,25 @@
             "status": None if status_uri is None else rdf.urify_value (status_uri),
             "assign_to_account": status == "approved"
         })
 
         self.cache.invalidate_by_prefix ("accounts")
         return self.__run_logged_query (query)
 
-    def quota_requests (self, status=None, quota_request_uuid=None):
+    def quota_requests (self, status=None, quota_request_uuid=None, account_uuid=None):
         """Procedure to return a list of quota requests."""
 
         status_uri = None
         if status is not None:
             status_uri = rdf.urify_value (rdf.DJHT[f"QuotaRequest{status.capitalize()}"])
 
         query = self.__query_from_template ("quota_requests", {
             "status": status_uri,
-            "quota_request_uuid": quota_request_uuid
+            "quota_request_uuid": quota_request_uuid,
+            "account_uuid": account_uuid
         })
         return self.__run_query (query)
 
     def update_account (self, account_uuid, active=None, email=None, job_title=None,
                         first_name=None, last_name=None, institution_user_id=None,
                         institution_id=None,
                         maximum_file_size=None, modified_date=None, created_date=None,
@@ -1586,24 +1618,14 @@
         rdf.add (graph, funding_uri, rdf.DJHT["created_by"],      account_uri,     "uri")
 
         if self.add_triples_from_graph (graph):
             return rdf.uri_to_uuid (funding_uri)
 
         return None
 
-    def append_to_list (self, node_to_be_appended_to, node_to_append):
-        """Procedure to append a blank node to an existing list."""
-
-        query = self.__query_from_template ("append_to_list", {
-            "last_blank_node":   node_to_be_appended_to,
-            "append_blank_node": node_to_append
-        })
-
-        return self.__run_logged_query (query)
-
     def delete_item_from_list (self, subject, predicate, rdf_first_value, value_type="uri"):
         """
         Removes node from list where RDF_FIRST_VALUE is the rdf:first property
         in the list pointed to by SUBJECT and PREDICATE.
         """
 
         first = None
@@ -1629,14 +1651,42 @@
         query = self.__query_from_template ("delete_items_all_from_list", {
             "subject":   subject,
             "predicate": rdf.DJHT[predicate].n3(),
         })
 
         return self.__run_logged_query (query)
 
+    def __append_to_existing_list (self, base_item_uri, existing_items):
+        """
+        Procedure to append to a list when the 'existing_items' contain
+        'originating_blank_node' and 'order_index' properties.
+        """
+        last_item = self.__last_item_by_order_index (existing_items)
+        if last_item is None:
+            self.log.error ("Unable to find item to append to (%s)", base_item_uri)
+            return None
+
+        new_index = conv.value_or (last_item, "order_index", 0) + 1
+        last_node = conv.value_or_none (last_item, "originating_blank_node")
+        new_node  = self.wrap_in_blank_node (base_item_uri, index=new_index)
+        if new_node is None:
+            self.log.error ("Failed preparation to append %s.", base_item_uri)
+            return None
+
+        query = self.__query_from_template ("append_to_list", {
+            "last_blank_node":   last_node,
+            "append_blank_node": new_node
+        })
+
+        if self.__run_logged_query (query):
+            return rdf.uri_to_uuid (base_item_uri)
+
+        self.log.error ("Failed to append %s to the item list.", base_item_uri)
+        return None
+
     def insert_file (self, file_id=None, name=None, size=None,
                      is_link_only=None, download_url=None, supplied_md5=None,
                      computed_md5=None, viewer_type=None, preview_state=None,
                      status=None, upload_url=None, upload_token=None,
                      dataset_uri=None, account_uuid=None, file_uuid=None):
         """Procedure to add an file to the state graph."""
 
@@ -1674,33 +1724,20 @@
             existing_files = self.dataset_files (dataset_uri  = dataset_uri,
                                                  limit        = None,
                                                  account_uuid = account_uuid)
 
             # In the case where there are already files in the dataset,
             # we can append to the last blank node.
             if existing_files:
-                last_file = existing_files[-1]
-                new_index = conv.value_or (last_file, "order_index", 0) + 1
-                if new_index < 1:
-                    self.log.error ("Expected larger index for to-be-appended file.")
-
-                last_node = conv.value_or_none (last_file, "originating_blank_node")
-                new_node  = self.wrap_in_blank_node (file_uri, index=new_index)
-                if new_node is None:
-                    self.log.error ("Failed preparation to append %s.", file_uri)
-                    return None
-
-                self.cache.invalidate_by_prefix (f"{account_uuid}_storage")
-                self.cache.invalidate_by_prefix (f"{dataset_uuid}_dataset_storage")
+                output = self.__append_to_existing_list (file_uri, existing_files)
+                if output is not None:
+                    self.cache.invalidate_by_prefix (f"{account_uuid}_storage")
+                    self.cache.invalidate_by_prefix (f"{dataset_uuid}_dataset_storage")
 
-                if self.append_to_list (last_node, new_node):
-                    return rdf.uri_to_uuid (file_uri)
-
-                self.log.error ("Failed to append %s to the file list.", file_uri)
-                return None
+                return output
 
             files = [URIRef(file_uri)]
             if self.update_item_list (dataset_uuid, account_uuid, files, "files"):
                 self.cache.invalidate_by_prefix (f"{account_uuid}_storage")
                 self.cache.invalidate_by_prefix (f"{dataset_uuid}_dataset_storage")
                 return rdf.uri_to_uuid (file_uri)
 
@@ -1799,24 +1836,15 @@
         rdf.add (graph, collaborator_uri, rdf.DJHT["data_remove"],   data_remove,   XSD.boolean)
         rdf.add (graph, collaborator_uri, rdf.DJHT["item"],          rdf.uuid_to_uri(dataset_uuid, "dataset"), "uri")
         rdf.add (graph, collaborator_uri, rdf.DJHT["account"],       rdf.uuid_to_uri(collaborator_uuid, "account"),  "uri")
 
         if self.add_triples_from_graph (graph):
             existing_collaborators = self.collaborators (dataset_uuid)
             if existing_collaborators:
-                last_collaborator = existing_collaborators [-1]
-                last_node = conv.value_or_none(last_collaborator, "originating_blank_node")
-                new_index = conv.value_or (last_collaborator, "order_index", 0) +1
-                new_node = self.wrap_in_blank_node(collaborator_uri, index=new_index)
-
-                if self.append_to_list(last_node, new_node):
-                    return rdf.uri_to_uuid (collaborator_uri)
-
-                self.log.error ("failed to append %s to list of collaborators ", collaborator_uri)
-                return None
+                return self.__append_to_existing_list (collaborator_uri, existing_collaborators)
 
             collaborators = [URIRef(collaborator_uri)]
             if self.update_item_list (dataset_uuid, account_uuid, collaborators, "collaborators"):
                 collaborators = self.collaborators(dataset_uuid)
                 for collaborator in collaborators:
                     self.cache.invalidate_by_prefix(f"datasets_{collaborator['account_uuid']}")
 
@@ -1859,20 +1887,18 @@
         rdf.add (graph, link_uri, rdf.DJHT["is_active"],    is_active)
         rdf.add (graph, link_uri, rdf.DJHT["expires_date"], expires_date, XSD.dateTime)
         rdf.add (graph, link_uri, rdf.DJHT["whom"], whom,  XSD.string)
         rdf.add (graph, link_uri, rdf.DJHT["anonymize"], anonymize,  XSD.boolean)
         rdf.add (graph, link_uri, rdf.DJHT["purpose"], purpose,  XSD.string)
 
         if self.add_triples_from_graph (graph):
-            item_uri    = rdf.uuid_to_uri (item_uuid, item_type)
+            item_uri       = rdf.uuid_to_uri (item_uuid, item_type)
             existing_links = self.private_links (item_uri=item_uri, account_uuid=account_uuid)
-            existing_links = list(map (lambda item: URIRef(rdf.uuid_to_uri(item["uuid"], "private_link")),
-                                               existing_links))
-
-            new_links    = existing_links + [URIRef(link_uri)]
+            if existing_links:
+                return self.__append_to_existing_list (link_uri, existing_links)
 
             item = None
             if item_type == "dataset":
                 item      = self.datasets (dataset_uuid = item_uuid,
                                            account_uuid = account_uuid,
                                            # Ignoring is_published and is_latest
                                            # enabled both published and draft
@@ -1886,20 +1912,21 @@
                                               account_uuid = account_uuid,
                                               # See above.
                                               is_published = None,
                                               is_latest    = None,
                                               limit        = 1)[0]
 
             if item is None:
-                self.log.error ("Could not find item to insert a private link for.")
+                self.log.error ("Could not find item to insert a private link %s for.",
+                                link_uri)
                 return None
 
             if self.update_item_list (item["uuid"],
                                       account_uuid,
-                                      new_links,
+                                      [URIRef(link_uri)],
                                       "private_links"):
                 return link_uri
 
         return None
 
     def insert_custom_field_value (self, name=None, value=None,
                                    item_uri=None, graph=None):
@@ -2261,15 +2288,16 @@
                         same_as=None, organizations=None, categories=None,
                         defined_type=None, defined_type_name=None,
                         embargo_until_date=None, embargo_type=None,
                         embargo_title=None, embargo_reason=None, eula=None,
                         is_embargoed=False, is_restricted=False,
                         agreed_to_deposit_agreement=False, agreed_to_publish=False,
                         is_metadata_record=False, metadata_reason=None,
-                        container_doi=None, is_first_online=False):
+                        container_doi=None, is_first_online=False,
+                        git_repository_name=None):
         """Procedure to overwrite parts of a dataset."""
 
         modified_date_str = datetime.strftime (datetime.now(), "%Y-%m-%dT%H:%M:%SZ")
         first_online_date_str = modified_date_str if is_first_online else None
 
         query   = self.__query_from_template ("update_dataset", {
             "account_uuid":    account_uuid,
@@ -2306,14 +2334,15 @@
             "embargo_type":    rdf.escape_string_value (embargo_type),
             "embargo_title":   rdf.escape_string_value (embargo_title),
             "embargo_reason":  rdf.escape_string_value (embargo_reason),
             "eula":            rdf.escape_string_value (eula),
             "agreed_to_deposit_agreement":
                                rdf.escape_boolean_value (agreed_to_deposit_agreement),
             "agreed_to_publish": rdf.escape_boolean_value (agreed_to_publish),
+            "git_repository_name": rdf.escape_string_value (git_repository_name),
             "container_doi":   rdf.escape_string_value (container_doi),
             "first_online_date": first_online_date_str
         })
 
         collaborators = self.collaborators(dataset_uuid)
         for collaborator in collaborators:
             self.cache.invalidate_by_prefix(f"datasets_{collaborator['account_uuid']}")
```

### Comparing `djehuty-24.4/src/djehuty/web/email_handler.py` & `djehuty-24.5/src/djehuty/web/email_handler.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/formatter.py` & `djehuty-24.5/src/djehuty/web/formatter.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/locks.py` & `djehuty-24.5/src/djehuty/web/locks.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/dashboard.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/admin/dashboard.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 {% extends "layout.html" %}
-{% block headers %}
-<style>
-#session-table tbody tr td:nth-child(2) { white-space: nowrap; }
-</style>
-{% endblock %}
 {% block submenu %}
 <ul>
   <li class="active corporate-identity-submenu-active">Dashboard
   <li><a href="/admin/users">Users</a>
   <li><a href="/admin/maintenance">Maintenance</a>
   <li><a href="/admin/exploratory">Exploratory</a>
   <li><a href="/admin/reports">Reports</a>
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-{% extends "layout.html" %} {% block headers %}
-{% endblock %} {% block submenu %}
+{% extends "layout.html" %} {% block submenu %}
     * Dashboard
     * _U_s_e_r_s
     * _M_a_i_n_t_e_n_a_n_c_e
     * _E_x_p_l_o_r_a_t_o_r_y
     * _R_e_p_o_r_t_s {% if may_query %}
     * _Q_u_e_r_y{% endif %} {% if may_review_quotas %}
     * _Q_u_o_t_a_ _r_e_q_u_e_s_t_s{% endif %}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/exploratory.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/admin/exploratory.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/maintenance.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/admin/maintenance.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 {% extends "layout.html" %}
 {% block headers %}
 <script src="/static/js/jquery-3.6.0.min.js"></script>
 <script src="/static/js/utils.js"></script>
-<style>
-#users-table .fa-user-secret { color: #000; }
-#users-table .fa-user-secret:hover { color: #666; }
-#users-table .fa-user-secret:active { color: #999; }
-#users-table { display: none; }
-#users-table_wrapper { margin-top: 1em; }
-</style>
 <script>
 jQuery(document).ready(function () {
     jQuery(".hide-for-javascript").removeClass("hide-for-javascript");
     jQuery("#users-table").show();
     jQuery("#recalculate-statistics").on("click", function (event) {
         event.preventDefault();
         event.stopPropagation();
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/quota_requests.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/admin/quota_requests.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/dashboard.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/admin/reports/dashboard.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/embargoed_datasets.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/admin/reports/embargoed_datasets.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/reports/restricted_datasets.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/admin/reports/restricted_datasets.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/sparql.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/admin/sparql.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/admin/users.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/admin/users.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/author.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/author.html`

 * *Files 2% similar despite different names*

```diff
@@ -55,22 +55,22 @@
 {% endif %}
 {% if profile.website %}
     <div id="location">
         <div class="label">website</div>
         <div><a class="corporate-identity" href="{{profile.website}}" target="_blank">{{profile.website}}</a></div>
     </div>
 {% endif %}
-{% if profile.location %}
+{% if profile.linkedin %}
     <div id="linkedin">
         <div class="label">linkedin</div>
         <div><a class="corporate-identity" href="{{profile.linkedin}}" target="_blank">{{profile.linkedin}}</a></div>
     </div>
 {% endif %}
 {% if profile.twitter %}
-    <div id="location">
+    <div id="twitter">
         <div class="label">twitter</div>
         <div><a class="corporate-identity" href="{{profile.twitter}}" target="_blank">{{profile.twitter}}</a></div>
     </div>
 {% endif %}
 {% if categories %}
     <div id="categories">
         <div class="label">categories</div>
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 {% endfor %}
 {% endif %} {% if profile.location %}
 location
 {{profile.location}}
 {% endif %} {% if profile.website %}
 website
 _{_{_p_r_o_f_i_l_e_._w_e_b_s_i_t_e_}_}
-{% endif %} {% if profile.location %}
+{% endif %} {% if profile.linkedin %}
 linkedin
 _{_{_p_r_o_f_i_l_e_._l_i_n_k_e_d_i_n_}_}
 {% endif %} {% if profile.twitter %}
 twitter
 _{_{_p_r_o_f_i_l_e_._t_w_i_t_t_e_r_}_}
 {% endif %} {% if categories %}
 categories
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/badge.svg` & `djehuty-24.5/src/djehuty/web/resources/html_templates/badge.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/collection.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/collection.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/colors.css` & `djehuty-24.5/src/djehuty/web/resources/html_templates/colors.css`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 .corporate-identity-h4 { border-bottom: 2px dotted {{primary_color}}; }
 .corporate-identity-background { background: {{primary_color}}; }
 .corporate-identity-header { border-top: 4px solid {{primary_color}}; }
 .corporate-identity-footer { color: #fff; border-bottom: 3px solid {{primary_color}}; background: {{footer_background_color}}; }
 .corporate-identity-border { border: solid 2pt {{primary_color}}; }
 .corporate-identity-table { width: 100%; max-width: 880pt; border: solid 2pt {{primary_color}}; border-radius: .5em; }
 .corporate-identity-table thead tr { background: {{primary_color}}; border-radius: .5em .5em 0em 0em; }
-.corporate-identity-standard-button { background: {{primary_color}}; color: #fff; font-weight: bold; text-decoration: none; }
-.corporate-identity-standard-button:hover { background: {{primary_color_hover}}; cursor: pointer; color: #fff; text-decoration: none; }
-.corporate-identity-standard-button:active { background: {{primary_color_active}}; cursor: pointer; color: #fff; text-decoration: none; }
+.corporate-identity-standard-button { background: {{primary_color}} !important; color: #fff; font-weight: bold; text-decoration: none; border: 0 !important; }
+.corporate-identity-standard-button:hover { background: {{primary_color_hover}} !important; cursor: pointer; color: #fff; text-decoration: none; border: 0 !important; }
+.corporate-identity-standard-button:active { background: {{primary_color_active}} !important; cursor: pointer; color: #fff; text-decoration: none; border: 0 !important; }
 .corporate-identity-privilege-button { background: {{privilege_button_color}}; }
 #login-button { margin-right: 25px; background: {{primary_color}}; color: #ffffff; }
 #login-button:hover { background: {{primary_color_hover}}; cursor: pointer; }
 #login-button:active { background: {{primary_color_active}}; cursor: pointer; }
 #primary-menu .menu-item-has-children:hover { color: {{primary_color_hover}}; }
 #primary-menu li a:hover { color: {{primary_color_hover}}; }
 .publish-button a { background: {{primary_color}} !important; }
 .publish-button a:hover { background: {{primary_color_hover}} !important; }
 .publish-button a:active { background: {{primary_color_active}} !important; }
 ul.latest-datasets li a { color: {{primary_color}}; }
 ul.latest-datasets li a:hover { color: {{primary_color_hover}}; }
 ul.latest-datasets li a:active { color: {{primary_color_active}}; }
+#files div.label { margin-bottom: 1em; }
 #files ul li a { color: {{primary_color}}; }
 #files ul li a:hover { color: {{primary_color_hover}}; }
 #files ul li a:active { color: {{primary_color_active}}; }
 #files ul li.zip { background: {{primary_color}}; margin-top: 1em; padding: .25em; width: 180px; text-align: center; border-radius: .5em; }
 #files ul li.zip a { font-weight: bold; color: #fff; }
 #total_size { font-size:12px; color: #fff; font-weight: normal; }
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/dataset.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/dataset.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 {% block headers %}
 <script src="/static/js/jquery-3.6.0.min.js"></script>
 <script src="/static/js/dataset_landing_page.js"></script>
 <script src="/static/js/quill.min.js"></script>
 <script src="/static/js/utils.js"></script>
 <link rel="stylesheet" type="text/css" href="/static/css/pub.css" />
 <link href="/static/css/quill.4tu.css" rel="stylesheet">
+<link href="/static/css/form.css" rel="stylesheet">
 <style>
 #access-request-wrapper { display: none; }
 #content-wrapper {padding: 0}
 </style>
 {% endblock %}
 
 {% block body %}
@@ -34,15 +35,14 @@
             {{item.confidential_reason}}
         {% endif %}
         {% endautoescape %}
     {% endif %}
        </div>
 {% elif item.is_restricted %}
     <h3>DATA - restricted access</h3>
-{# test 12999575 #}
         <div id="limited_access">
             <h4>Reason</h4>
     {% autoescape false %}
     {% if item.embargo_reason %}
             {{item.embargo_reason}}
     {% elif item.confidential_reason %}
             {{item.confidential_reason}}
@@ -53,15 +53,14 @@
             <h4>End User Licence Agreement</h4>
             {{item.eula}}
     {% endif %}
     {% endautoescape %}
         </div>
         {% include 'dataset_access_request.html' %}
 {% elif item.is_metadata_record %}
-{# test 18586031 #}
     <h3>DATA - not available</h3>
         <div id="metadata_only">
     {% if item.metadata_reason %}
             {{item.metadata_reason}}
     {% else %}
             Data is undisclosed.
     {% endif %}
@@ -73,26 +72,24 @@
     <div id="private_view">As you are on a private link, you have access to the data files.</div>
 {% endif %}
 {% if not(item.is_restricted or item.is_embargoed) %}
     <h3>DATA</h3>
 {% endif %}
 {% if is_own_item or private_view or not(item.is_restricted or item.is_embargoed) %}
 {% if services %}
-{# test 12717890 #}
     <div id="services">
         <div class="label">data service</div>
         <ul>
     {% for url in services %}
             <li><a class="corporate-identity" href="{{url}}" target="_blank" rel="noopener noreferrer" title="opens in new window">{{url}}</a></li>
     {% endfor %}
         </ul>
     </div>
 {% endif%}
 {% if opendap %}
-{# test 17122553 #}
     <div id="opendap">
         <div class="label">OPeNDAP data service</div>
         <ul>
     {% for url in opendap %}
             <li>
                 <a class="corporate-identity" href="{{url}}" target="_blank" rel="noopener noreferrer" title="opens in new window">{{url}}</a>
                 [<a class="corporate-identity" href="{{url|replace('.html','.xml')}}" target="_blank" rel="noopener noreferrer">xml</a>]
@@ -100,19 +97,18 @@
     {% endfor %}
         </ul>
     </div>
 {% endif%}
 {%- if git_repository_url %}
     <div id="git-repository">
       <p>To access the source code, use the following command:</p>
-      <pre>git clone {{git_repository_url}}</pre>
+      <pre>git clone {{git_repository_url}}{% if item.git_repository_name %} "{{item.git_repository_name}}"{% endif %}</pre>
     </div>
 {%- endif %}
 {% if files %}
-{# test 16545714 #}
     <div id="files">
         <div class="label">files ({{files|length}})</div>
         <ul>
     {% for file in files %}
             <li>
               <span class="size">{{'{:,}'.format(file.size)}} bytes</span><!--
               --><span class="md5">MD5:<code>{{file.computed_md5}}</code></span>
```

#### html2text {}

```diff
@@ -9,47 +9,46 @@
 {% if item.embargo_reason or item.confidential_reason %}
 ****** RReeaassoonn ******
 {% autoescape false %} {% if item.embargo_reason %} {{item.embargo_reason}} {%
 else %} {{item.confidential_reason}} {% endif %} {% endautoescape %} {% endif
 %}
 {% elif item.is_restricted %}
 ******** DDAATTAA -- rreessttrriicctteedd aacccceessss ********
-{# test 12999575 #}
 ****** RReeaassoonn ******
 {% autoescape false %} {% if item.embargo_reason %} {{item.embargo_reason}} {%
 elif item.confidential_reason %} {{item.confidential_reason}} {% else %} Data
 is confidential. {% endif %} {% if item.eula %}
 ****** EEnndd UUsseerr LLiicceennccee AAggrreeeemmeenntt ******
 {{item.eula}} {% endif %} {% endautoescape %}
 {% include 'dataset_access_request.html' %} {% elif item.is_metadata_record %}
-{# test 18586031 #}
 ******** DDAATTAA -- nnoott aavvaaiillaabbllee ********
 {% if item.metadata_reason %} {{item.metadata_reason}} {% else %} Data is
 undisclosed. {% endif %}
 {% endif %} {% if is_own_item and (item.is_restricted or item.is_embargoed) %}
 As the owner of this dataset, you have access to the data files.
 {% elif private_view and (item.is_restricted or item.is_embargoed) %}
 As you are on a private link, you have access to the data files.
 {% endif %} {% if not(item.is_restricted or item.is_embargoed) %}
 ******** DDAATTAA ********
 {% endif %} {% if is_own_item or private_view or not(item.is_restricted or
-item.is_embargoed) %} {% if services %} {# test 12717890 #}
+item.is_embargoed) %} {% if services %}
 data service
     * {% for url in services %}
     * _{_{_u_r_l_}_}
     * {% endfor %}
-{% endif%} {% if opendap %} {# test 17122553 #}
+{% endif%} {% if opendap %}
 OPeNDAP data service
     * {% for url in opendap %}
     * _{_{_u_r_l_}_} [_x_m_l]
     * {% endfor %}
 {% endif%} {%- if git_repository_url %}
 To access the source code, use the following command:
-git clone {{git_repository_url}}
-{%- endif %} {% if files %} {# test 16545714 #}
+git clone {{git_repository_url}}{% if item.git_repository_name %} "{
+{item.git_repository_name}}"{% endif %}
+{%- endif %} {% if files %}
 files ({{files|length}})
     * {% for file in files %}
     * {{'{:,}'.format(file.size)}} bytesMD5:{{file.computed_md5}} _{_{_f_i_l_e_._n_a_m_e_}_}
     * {% endfor %}
     * _d_o_w_n_l_o_a_d_ _a_l_l_ _f_i_l_e_s_ _(_z_i_p_)
       {{'{:,}'.format(files_size)}} bytes unzipped
 {% endif %} {% endif %}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/dataset_access_request.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/dataset_access_request.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/collection-private-links.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/collection-private-links.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/dashboard.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/dashboard.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends "layout.html" %}
 {% block headers %}
 <script src="/static/js/jquery-3.6.0.min.js"></script>
 <script src="/static/js/quill.min.js"></script>
 <script src="/static/js/utils.js"></script>
-<script src="/static/js/depositor-dashboard.js"></script>
+<script src="/static/js/depositor-dashboard.js?cache=1715649348"></script>
 <link href="/static/css/quill.4tu.css" rel="stylesheet">
 <style>
 #session-table tbody tr td:nth-child(2) { white-space: nowrap; }
 #create-new-dataset { margin: auto; }
 #create-new-collection { margin: auto; }
 #storage-request-wrapper { display: none; }
 #content-wrapper input[type="text"],
@@ -36,14 +36,22 @@
     display: inline-block;
     background: #ffeecc;
     color: #000;
     padding: .5em .5em .25em .5em;
     border-radius: .5em .5em 0em 0em;
     font-weight: bold;
 }
+.quota-requested {
+    background: #ffeecc;
+    padding: .25em;
+    border-radius: .25em;
+    user-select: none;
+    margin-right: .25em;
+}
+.storage-usage { margin-right: .25em; }
 </style>
 {% endblock %}
 {% block submenu %}
 <ul>
   <li class="active corporate-identity-submenu-active">My Dashboard
   <li class="create-button"><a href="/my/sessions/new">Create API token</a>
   <li><a href="/my/datasets">My Datasets</a>
@@ -54,15 +62,15 @@
 <h1>Dashboard</h1>
 <h2>Quick actions</h2>
 <div class="center">
   <a id="create-new-dataset" href="/my/datasets/new" class="button corporate-identity-standard-button">Add new dataset</a>
   <a id="create-new-collection" href="/my/collections/new" class="button corporate-identity-standard-button">Create new collection</a>
 </div>
 <h2>Storage usage</h2>
-<p>Using {{storage_used}} of {{quota}} ({{percentage_used}}%). <a id="request-more-storage" href="#">Request more storage.</a></p>
+<p><span class="storage-usage">Using {{storage_used}} of {{quota}} ({{percentage_used}}%).</span>{% if requested_quota %}<span class="quota-requested">Request pending for {{requested_quota}}</span>{% endif %}<a id="request-more-storage" href="#">Request more storage.</a></p>
 <div id="storage-request-wrapper">
   <label for="new-quota">New quota</label>
   <input type="text" id="new-quota" name="new-quota" placeholder="New quota in gigabytes (for example: 50)." />
   <label for="quota-reason">Reason</label>
   <div id="quota-reason" class="texteditor"></div>
   <p>Your request will be reviewed by our team (usually within one working day) and you will be contacted by e-mail about its status.</p>
   <div class="center">
@@ -91,15 +99,15 @@
 
 <div class="notice-box">
 <h3>API documentation</h3>
 <p>This repository implements a compatible API to version <code>v2</code> of
   the <a href="https://docs.figshare.com">Figshare API</a> with the following
   differences:</p>
 <ol>
-  <li>The <strong>Base URL</strong> is <code>https://data.4tu.nl/v2</code>
+  <li>The <strong>Base URL</strong> is <code>{{base_url}}/v2</code>
     instead of <code>https://api.figshare.com/v2</code>.</li>
   <li>Previously generated API tokens are no longer valid.
     <a href="/my/sessions/new">Generate a new token</a>.
   <li>Numerical identifiers (<code>id</code>) properties are deprecated for
     newly created datasets/collections and superseded by the <code>uuid</code> property.</li>
 </ol>
 </div>
```

#### html2text {}

```diff
@@ -5,16 +5,17 @@
     * _M_y_ _D_a_t_a_s_e_t_s
     * _M_y_ _C_o_l_l_e_c_t_i_o_n_s
 {% endblock %} {% block body %}
 ************ DDaasshhbbooaarrdd ************
 ********** QQuuiicckk aaccttiioonnss **********
 _A_d_d_ _n_e_w_ _d_a_t_a_s_e_t _C_r_e_a_t_e_ _n_e_w_ _c_o_l_l_e_c_t_i_o_n
 ********** SSttoorraaggee uussaaggee **********
-Using {{storage_used}} of {{quota}} ({{percentage_used}}%). _R_e_q_u_e_s_t_ _m_o_r_e
-_s_t_o_r_a_g_e_.
+Using {{storage_used}} of {{quota}} ({{percentage_used}}%).{% if
+requested_quota %}Request pending for {{requested_quota}}{% endif %}_R_e_q_u_e_s_t
+_m_o_r_e_ _s_t_o_r_a_g_e_.
 New quota [new-quota           ]Reason
 Your request will be reviewed by our team (usually within one working day) and
 you will be contacted by e-mail about its status.
 Send request for more storage
 ********** SSeessssiioonnss aanndd AAPPII ttookkeennss **********
 NNaammee                       CCrreeaatteedd aatt               AAccttiioonnss
 {% if session.editable %}
@@ -26,14 +27,13 @@
 session_token ==
 session.token %} Current
 session{% endif %} {%
 endif %}
 ******** AAPPII ddooccuummeennttaattiioonn ********
 This repository implements a compatible API to version v2 of the _F_i_g_s_h_a_r_e_ _A_P_I
 with the following differences:
-   1. The BBaassee UURRLL is https://data.4tu.nl/v2 instead of https://
-      api.figshare.com/v2.
+   1. The BBaassee UURRLL is {{base_url}}/v2 instead of https://api.figshare.com/v2.
    2. Previously generated API tokens are no longer valid. _G_e_n_e_r_a_t_e_ _a_ _n_e_w
       _t_o_k_e_n.
    3. Numerical identifiers (id) properties are deprecated for newly created
       datasets/collections and superseded by the uuid property.
 {% endblock %}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/dataset-private-links.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/dataset-private-links.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-collection.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/edit-collection.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-dataset.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/edit-dataset.html`

 * *Files 1% similar despite different names*

```diff
@@ -471,14 +471,16 @@
     So when your dataset has been published, remove the remote:</p>
   <pre>git remote remove 4tu</pre>
   <h4 class="corporate-identity-h4">Git repository files and branches <span class="no-select"> &nbsp;<a id="refresh-git-files" href="#" class="fas fa-sync"></a></span></h4>
   <label>Git default branch</label><div class="fas fa-question-circle help-icon"><span class="help-text">The selected branch will be the branch a user is in after pulling the Git repository.</span></div>
   <select id="git-branches">
     <option value="" disabled="disabled">Select branch</option>
   </select>
+  <label for="git-repository-name">Git repository name</label><div class="fas fa-question-circle help-icon"><span class="help-text">This will be used as the folder name when cloning the repository.</span></div>
+  <input type="text" id="git-repository-name" name="git-repository-name" value="{{article["git_repository_name"]}}" />
   <label id="git-files-label">Git file list</label>
   <div id="git-files-wrapper" class="options-wrapper">
     <ul id="git-files"></ul>
   </div>
   <h4 class="corporate-identity-h4">Distribution artefacts</h4>
   <p>
     Software packages oftentimes have separate distribution tarballs
@@ -514,13 +516,13 @@
 </div>
 <h3 class="corporate-identity-h3">Terms and agreement</h3>
 <input type="checkbox" name="deposit_agreement" id="deposit_agreement">
 <label class="no-head" for="deposit_agreement">I agree with the <a target="_blank" rel="noopener noreferrer" href="/s/docs/deposit-agreement.pdf">Deposit Agreement</a>.</label><span class="required-field">&#8727;</span><br />
 <input type="checkbox" name="publish_agreement" id="publish_agreement">
 <label class="no-head" for="publish_agreement">I agree that my dataset will be published once
   the review is complete.</label><span class="required-field">&#8727;</span>
-</div>
 {%- if not article.is_shared_with_me or permissions.metadata_edit %}
-<a class="hide-for-javascript save-button button"id="save_bottom" href="#">Save draft</a>
+<p style="margin: 0em; padding: 0em;"><a class="hide-for-javascript save-button button" id="save_bottom" href="#">Save draft</a></p>
 {%- endif %}
 </div>
+</div>
 {% endblock %}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/edit-session.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/edit-session.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/language-selector.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/language-selector.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/my-collections.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/my-collections.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/my-data.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/my-data.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/new_private_link.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/new_private_link.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/profile.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/profile.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/published-collection.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/published-collection.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/depositor/submitted-for-review.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/depositor/submitted-for-review.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_approved.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/email/dataset_approved.html`

 * *Files 22% similar despite different names*

```diff
@@ -7,9 +7,12 @@
 
 <p>To refer to your published dataset, we recommend to use the appropriate DOI.</p>
 
 <p>When referring to the dataset or a future update of this dataset, we recommend to use:<br /><code>https://doi.org/{{container_doi}}</code></p>
 
 <p>In case you want to refer to this specific version of your dataset, we recommend to use:<br /><code>https://doi.org/{{versioned_doi}}</code></p>
 
+<p>In case you have published additional documents referring to your dataset, you can add them to the metadata yourself. Find more information about modifying and versioning on <a href="{{base_url}}/info/en/use/publish-cite/after-uploading">this page</a>.</p>
+
 <p>This is an automated message. For further correspondence, either use the <a href="{{base_url}}/feedback">feedback form</a> or contact us by e-mail at <a href="mailto:{{support_email}}">{{support_email}}</a></p>
+
 {% endblock %}
```

#### html2text {}

```diff
@@ -5,10 +5,13 @@
 To refer to your published dataset, we recommend to use the appropriate DOI.
 When referring to the dataset or a future update of this dataset, we recommend
 to use:
 https://doi.org/{{container_doi}}
 In case you want to refer to this specific version of your dataset, we
 recommend to use:
 https://doi.org/{{versioned_doi}}
+In case you have published additional documents referring to your dataset, you
+can add them to the metadata yourself. Find more information about modifying
+and versioning on _t_h_i_s_ _p_a_g_e.
 This is an automated message. For further correspondence, either use the
 _f_e_e_d_b_a_c_k_ _f_o_r_m or contact us by e-mail at _{_{_s_u_p_p_o_r_t___e_m_a_i_l_}_}
 {% endblock %}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_approved.txt` & `djehuty-24.5/src/djehuty/web/resources/html_templates/email/dataset_approved.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,11 +8,15 @@
 
 When referring to the specific version of your dataset, we recommend to use:
   https://doi.org/{{versioned_doi}}
 
 When referring to the dataset, or an update of this dataset, we recommend to use:
   https://doi.org/{{container_doi}}
 
+In case you have published additional documents referring to your dataset, you can add them to the metadata yourself. Find more information about modifying and versioning on this page [3].
+
 This is an automated message. For further correspondence, either use the feedback form [2] or contact us by e-mail at {{support_email}}</p>
 
 [1] {{base_url}}/datasets/{{container_uuid}}
 [2] {{base_url}}/feedback
+[3] {{base_url}}/info/en/use/publish-cite/after-uploading
+
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/email/dataset_submitted.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/email/dataset_submitted.html`

 * *Files 16% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 00000090: 2c20 4661 6c73 6529 7d7d 207b 7b61 6363  , False)}} {{acc
 000000a0: 6f75 6e74 2e6c 6173 745f 6e61 6d65 207c  ount.last_name |
 000000b0: 2064 6566 6175 6c74 2822 222c 2046 616c   default("", Fal
 000000c0: 7365 297d 7d2c 3c2f 703e 0a3c 703e 5468  se)}},</p>.<p>Th
 000000d0: 616e 6b20 796f 7520 666f 7220 7375 626d  ank you for subm
 000000e0: 6974 7469 6e67 2079 6f75 7220 6461 7461  itting your data
 000000f0: 7365 7420 277b 7b64 6174 6173 6574 2e74  set '{{dataset.t
-00000100: 6974 6c65 7d7d 2720 746f 2034 5455 2e52  itle}}' to 4TU.R
-00000110: 6573 6561 7263 6844 6174 612e 2020 5765  esearchData.  We
-00000120: 2068 6572 6562 7920 636f 6e66 6972 6d20   hereby confirm 
-00000130: 7765 2068 6176 6520 7265 6365 6976 6564  we have received
-00000140: 2079 6f75 7220 6461 7461 7365 7420 7375   your dataset su
-00000150: 626d 6973 7369 6f6e 2e3c 2f70 3e0a 3c70  bmission.</p>.<p
-00000160: 3e41 2072 6576 6965 7765 7220 7769 6c6c  >A reviewer will
-00000170: 2063 6f6e 7461 6374 2079 6f75 2061 626f   contact you abo
-00000180: 7574 2070 7562 6c69 7368 696e 6720 6974  ut publishing it
-00000190: 2069 6e20 7468 6520 3454 552e 5265 7365   in the 4TU.Rese
-000001a0: 6172 6368 4461 7461 2072 6570 6f73 6974  archData reposit
-000001b0: 6f72 792e 3c2f 703e 0a3c 703e 5468 6973  ory.</p>.<p>This
-000001c0: 2069 7320 616e 2061 7574 6f6d 6174 6564   is an automated
-000001d0: 206d 6573 7361 6765 2e20 2049 6620 796f   message.  If yo
-000001e0: 7520 6861 7665 2061 6e79 2071 7565 7374  u have any quest
-000001f0: 696f 6e73 2c20 706c 6561 7365 2063 6f6e  ions, please con
-00000200: 7461 6374 2072 6573 6561 7263 6864 6174  tact researchdat
-00000210: 6140 3474 752e 6e6c 2e3c 2f70 3e0a 7b25  a@4tu.nl.</p>.{%
-00000220: 2065 6e64 626c 6f63 6b20 257d 0a          endblock %}.
+00000100: 6974 6c65 7d7d 2720 746f 207b 7b73 6974  itle}}' to {{sit
+00000110: 655f 6e61 6d65 7d7d 2e20 2057 6520 6865  e_name}}.  We he
+00000120: 7265 6279 2063 6f6e 6669 726d 2077 6520  reby confirm we 
+00000130: 6861 7665 2072 6563 6569 7665 6420 796f  have received yo
+00000140: 7572 2064 6174 6173 6574 2073 7562 6d69  ur dataset submi
+00000150: 7373 696f 6e2e 3c2f 703e 0a3c 703e 4120  ssion.</p>.<p>A 
+00000160: 7265 7669 6577 6572 2077 696c 6c20 636f  reviewer will co
+00000170: 6e74 6163 7420 796f 7520 6162 6f75 7420  ntact you about 
+00000180: 7075 626c 6973 6869 6e67 2069 7420 696e  publishing it in
+00000190: 2074 6865 207b 7b73 6974 655f 6e61 6d65   the {{site_name
+000001a0: 7d7d 2072 6570 6f73 6974 6f72 792e 3c2f  }} repository.</
+000001b0: 703e 0a3c 703e 5468 6973 2069 7320 616e  p>.<p>This is an
+000001c0: 2061 7574 6f6d 6174 6564 206d 6573 7361   automated messa
+000001d0: 6765 2e20 2049 6620 796f 7520 6861 7665  ge.  If you have
+000001e0: 2061 6e79 2071 7565 7374 696f 6e73 2c20   any questions, 
+000001f0: 706c 6561 7365 2063 6f6e 7461 6374 203c  please contact <
+00000200: 6120 6872 6566 3d22 6d61 696c 746f 3a7b  a href="mailto:{
+00000210: 7b73 7570 706f 7274 5f65 6d61 696c 7d7d  {support_email}}
+00000220: 223e 7b7b 7375 7070 6f72 745f 656d 6169  ">{{support_emai
+00000230: 6c7d 7d3c 2f61 3e2e 3c2f 703e 0a7b 2520  l}}</a>.</p>.{% 
+00000240: 656e 6462 6c6f 636b 2025 7d0a            endblock %}.
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/feedback.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/feedback.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,34 +3,14 @@
 <script src="/static/js/jquery-3.6.0.min.js"></script>
 <script src="/static/js/quill.min.js"></script>
 <script src="/static/js/utils.js"></script>
 <link href="/static/css/quill.4tu.css" rel="stylesheet">
 <link href="/static/css/form.css" rel="stylesheet">
 <style>
 .info { margin-left: 5pt; color: #555; }
-#submit-feedback {
-    background: #f39000;
-    color: #fff;
-    border: none !important;
-}
-#submit-feedback:hover {
-    border: none;
-    background: #d26000;
-    cursor: pointer;
-    color: #fff;
-    text-decoration: none;
-}
-#submit-feedback:active {
-    border: none !important;
-    background: #9d4800 !important;
-    cursor: pointer;
-    color: #fff;
-    text-decoration: none;
-}
-input[type="submit"]:active { color: green; }
 .ql-toolbar.ql-4tu, .texteditor { width: 852pt !important; }
 .texteditor { border-radius: 0em 0em .5em .5em !important; border-top: none !important; }
 #description { height: 500px !important; }
 </style>
 <script>
 jQuery(document).ready(function () {
     new Quill('#description', { theme: '4tu' });
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/layout.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     <meta charset="UTF-8">
     <meta name="description" content="{{site_description}}">
     <meta name="keywords" content="{{site_shorttag}}, {{site_name}}, data repository">
     <meta name="author" content="{{site_name}}">
     <meta http-equiv="Content-Security-Policy" content="default-src 'self' api.figshare.com ndownloader.figshare.com s3-eu-west-1.amazonaws.com 'unsafe-inline'; frame-src https://www.youtube.com">
     <title>{% if page_title %}{{page_title|safe}}{% else %}{{site_name | default("Djehuty", True)}}{% endif %}</title>
     <link rel='shortcut icon' type='image/x-icon' href='/static/images/favicon.ico'>
-    <link rel="stylesheet" type="text/css" href="/theme/colors.css">
-    <link rel="stylesheet" type="text/css" href="/static/css/main.css">
+    <link rel="stylesheet" type="text/css" href="/theme/colors.css?cache=1714383498">
+    <link rel="stylesheet" type="text/css" href="/static/css/main.css?cache=1714383498">
     {% block headers %}{% endblock %}
   </head>
   <body>
     <div id="wrapper" {%- if path == "/" %} class="footer1"{% else %} class="footer2"{% endif %}>
       {%- if sandbox_message %}
       <div id="sandbox-message" class="pre-header" {% if sandbox_message_css %}style="{{sandbox_message_css | safe}}"{% endif %}>
         <p>{{sandbox_message | safe}}</p>
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/loader.svg` & `djehuty-24.5/src/djehuty/web/resources/html_templates/loader.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/opendap_to_doi.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/opendap_to_doi.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/portal.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/portal.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/public_metadata.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/public_metadata.html`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     {% set dtype = item.defined_type_name|capitalize %}
 {% else %}
     {% set dtype = "Collection" %}
 {% endif %}
     <div id="type_versions">
         <div id="type">{{ dtype }}</div>
 {% if not private_view and versions[1:2] %}
-{# test 12763700 #}
         <button id="versions_show" onclick="document.getElementById('versions').style.display='block'" title="Choose another version."
             {% if old %}style="background-color: #ff0"{% endif %}>version {{thisversion}}
             {% if old %} (old){% endif %} &#x1F53B; </button>
         <div id ="versions">
             <button id="versions_hide" class="cancel-button" onclick='this.parentElement.style.display="none"'>x</button>
             choose version:
     {% for ver in versions %}
@@ -78,15 +77,14 @@
     <div id="right_column">
 {% if member != "other" and not anonymize %}
         <div id="member">
             <a class="corporate-identity" href="/institutions/{{member_url_name}}"><img src="/static/images/logo-{{member}}.png" alt="{{member_url_name.replace('_',' ')}} logo" /></a>
         </div>
 {% endif %}
 {% if statistics %}
-{# test 12763700 #}
         <div id="usage">
             <div class="label">usage stats</div>
     {% for metric in statistics %}
             <div class="metric">
                 <div class="number">{{statistics[metric]}}</div>
                 {{metric.replace("cites", "citations")}}
             </div>
@@ -102,23 +100,22 @@
             </ul>
         </div>
         <div id="tags">
             <div class="label">keywords</div>
                 {# The query below searches for full text. Field search does not yet work for keywords #}
 {% for tag in tags|sort %}
     {% set query = '"'~tag~'"' %}
-            <a class="corporate-identity" href="/search?search={{query|urlencode}}">{{tag}}</a>
+            <a class="corporate-identity" href="/search?searchscope=tag&search={{query|urlencode}}">{{tag}}</a>
     {%- if loop.revindex0 %}, {% endif %}
 {% endfor %}
         </div>
 {% set geo = item.geolocation %}
 {% set lat = coordinates.lat %}
 {% set lon = coordinates.lon %}
 {% if geo or lat or lon %}
-{# test 12683045 #}
     {% set vlat = coordinates.lat_valid %}
     {% set vlon = coordinates.lon_valid %}
         <div id="geo">
             <div class="label">geolocation</div>
     {% if geo %}
             <div id = "geo_name">{{geo}}</div>
     {% endif %}
@@ -153,15 +150,14 @@
     {% set lic_img = lic_imgs[item.license_name] %}
         <div id="licence">
             <div class="label">licence</div>
             <a class="corporate-identity" href="{{item.license_url}}" target="_blank" rel="noopener noreferrer" title="opens in new window">
                 {%- if lic_img %}<img src="/static/images/licenses/{{lic_img}}" alt="{{lic_img}} logo"/>{% endif %}
                 {{item.license_name}}</a>
     {% if item.license_remarks %}
-    {# test 12776162 #}
             <div>{{item.license_remarks}}</div>
     {% endif %}
         </div>
     {% if collections %}
         <div id="collections">
             <div class="label">collection{% if collections[1:] %}s{% endif %}</div>
             <ul>
@@ -223,15 +219,14 @@
 {% if item.format %}
         <div id="format">
             <div class="label">format</div>
             {{ item.format.replace('\\n', '\n') }}
         </div>
 {% endif %}
 {% if item.resource_doi %}
-{# test 16825843 #}
         <div id="peer">
             <div class="label">associated peer-reviewed publication</div>
             <a class="corporate-identity" href="https://doi.org/{{item.resource_doi}}" target="_blank" rel="noopener noreferrer" title="opens in new window">{{item.resource_title}}</a>
         </div>
 {% endif %}
 {% if references %}
         <div id="references">
@@ -240,49 +235,44 @@
     {% for r in references %}
                 <li><a class="corporate-identity" href="{{r.url}}" target="_blank" rel="noopener noreferrer" title="opens in new window">{{r.url}}</a></li>
     {% endfor %}
             </ul>
         </div>
 {% endif %}
 {% if derived_from %}
-{# test 12716117 #}
         <div id="derived_from">
             <div class="label">derived from</div>
             <ul>
     {% for d in derived_from %}
                 <li><a class="corporate-identity" href="{{d}}" target="_blank" rel="noopener noreferrer" title="opens in new window">{{d}}</a></li>
     {% endfor %}
             </ul>
         </div>
 {% endif %}
 {% if item.same_as %}
-{# test 18865355 #}
         <div id="same_as">
             <div class="label">same as</div>
             <a class="corporate-identity" href="{{item.same_as}}" target="_blank" rel="noopener noreferrer" title="opens in new window">{{item.same_as}}</a>
         </div>
 {% endif %}
 {% if item.data_link %}
-{# test 14377295 #}
         <div id="data_link">
             <div class="label">data link</div>
             <a class="corporate-identity" href="{{item.data_link}}" target="_blank" rel="noopener noreferrer" title="opens in new window">{{item.data_link}}</a>
         </div>
 {% endif %}
 {% if item.language %}
-{# test 17081387 #}
     {% if item.language != 'en' %}
         <div id="language">
             <div class="label">language</div>
             {{item.language}}
         </div>
     {% endif %}
 {% endif %}
 {% if fundings %}
-{# test 19114712 #}
         <div id="funding">
             <div class="label">funding</div>
             <ul>
     {% for funding in fundings %}
                 <li>
         {% if funding.title %}
                     <span class="funding_title">{{funding.title}}</span>
@@ -298,24 +288,22 @@
         {% endif %}
                 </li>
     {% endfor %}
           </ul>
         </div>
 {% endif %}
 {% if item.organizations %}
-{# test 12705164 #}
     {% autoescape false %}
         <div id="organizations">
             <div class="label">organizations</div>
             {{ item.organizations.replace('\n', '<br />') }}
         </div>
     {% endautoescape %}
 {% endif %}
 {% if contributors %}
-{# test 12721421 v1 #}
         <div id="contributors">
             <div class="label">contributors</div>
             <ul>
     {% for c in contributors %}
                 <li>
                     {{c.name}} 
         {% if c.orcid %}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/review/overview.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/review/overview.html`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/html_templates/search.html` & `djehuty-24.5/src/djehuty/web/resources/html_templates/search.html`

 * *Files 7% similar despite different names*

```diff
@@ -51,26 +51,14 @@
     background: #f9f9f9;
     cursor: pointer;
     text-decoration: none;
     border: none;
 }
 .search-terms li button:hover { background: #eeeeee; }
 .search-terms li button:active { background: #e9e9e9; }
-.tabs ul { margin: 0em; padding: 0em; }
-.tabs li {
-    display: inline-block;
-    list-style-type: none;
-    text-decoration: none;
-    color: #000000;
-    font-size: 12pt;
-    padding: .5em .75em .5em .75em;
-    margin: 0pt 5pt 0pt 0pt;
-    user-select: none;
-    border-radius: .5em .5em 0em 0em;
-}
 #search-loader {
     background-image: url('/theme/loader.svg');
     background-position: center;
     background-repeat: no-repeat;
     color: darkgrey;
     display: inline-block;
     font-size: 2.5em;
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_by_email.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_by_email.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_by_session_token.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_by_session_token.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_categories.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_categories.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_sessions.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_sessions.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/account_storage_used.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/account_storage_used.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/accounts.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/accounts.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/associated_authors.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/associated_authors.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/author_profile.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/author_profile.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/author_public_items.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/author_public_items.sparql`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {# Find for each item the latest version authored by a given author. #}
 {% extends "prefixes.sparql" %}
 {% block query %}
-SELECT DISTINCT ((?item_type = <https://ontologies.data.4tu.nl/djehuty/0.0.1/Dataset>) AS ?is_dataset)
+SELECT DISTINCT ((?item_type = djht:Dataset) AS ?is_dataset)
                 (STRAFTER(STR(?container), ":") AS ?container_uuid)
                 ?version ?posted_date ?title
                 ?downloads ?views ?shares ?cites
 WHERE {
   GRAPH <{{state_graph}}> {
     ?item  rdf:type          ?item_type ;
            djht:container    ?container ;
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/authors.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/authors.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/categories.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/categories.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/categories_tree.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/categories_tree.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/category_by_id.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/category_by_id.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collaborators.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/collaborators.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_datasets.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/collection_datasets.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collection_versions.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/collection_versions.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/collections.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections_by_account.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/collections_by_account.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/collections_from_dataset.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/collections_from_dataset.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/container.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/container.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/container_items.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/container_items.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/custom_fields.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/custom_fields.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_files.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_files.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_statistics.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_statistics.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_statistics_timeline.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_statistics_timeline.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/dataset_versions.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/dataset_versions.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/datasets.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/datasets.sparql`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 ?url_public_html ?version (STR(?language_ut) AS ?language) ?time_coverage
                 ?geolocation ?longitude ?latitude ?format ?organizations
                 ?data_link ?same_as ?contributors ?review_status
                 ?license_remarks ?container_uri (?dataset AS ?uri) ?uuid
                 ?is_under_review (?review AS ?review_uri) ?review_submit_date
                 ?totals_created_at ?total_downloads ?total_views ?total_shares
                 ?total_cites ?git_uuid ?agreed_to_deposit_agreement ?agreed_to_publish
-                ?private_link_is_expired ?is_shared_with_me ?anonymize
+                ?private_link_is_expired ?is_shared_with_me ?anonymize ?git_repository_name
 {%endif%}
 WHERE {
   GRAPH <{{state_graph}}> {
     ?container_uri      rdf:type                  djht:DatasetContainer .
     OPTIONAL { ?container_uri djht:dataset_id     ?dataset_id . }
 
     {%- if is_published is none and is_latest is none: %}
@@ -143,14 +143,15 @@
     OPTIONAL { ?dataset djht:organizations         ?organizations . }
     OPTIONAL { ?dataset djht:data_link             ?data_link . }
     OPTIONAL { ?dataset djht:same_as               ?same_as . }
     OPTIONAL { ?dataset djht:contributors          ?contributors . }
     OPTIONAL { ?dataset djht:license_remarks       ?license_remarks . }
     OPTIONAL { ?dataset djht:agreed_to_deposit_agreement ?agreed_to_deposit_agreement . }
     OPTIONAL { ?dataset djht:agreed_to_publish     ?agreed_to_publish . }
+    OPTIONAL { ?dataset djht:git_repository_name   ?git_repository_name . }
 
     ?container_uri      djht:account              ?account .
     {%- if not disable_collaboration %}
     OPTIONAL {
       ?collaborator       rdf:type            djht:Collaborator .
       ?collaborator       djht:item           ?dataset .
       ?collaborator       djht:account        ?collaborator_account .
@@ -174,15 +175,20 @@
     # Wrapping the xsd:dateTime in strings is needed because Virtuoso seems to
     # return 1 for 2023-07-07 < 2023-07-06. String comparison works because the
     # xsd:dateTime format is YYYY-MM-DD.
     BIND((BOUND(?private_link_expires_date) && STR(?private_link_expires_date) < STR(NOW())) AS ?private_link_is_expired)
     {%- else %}
     BIND("false"^^xsd:boolean AS ?private_link_is_expired)
     {%- endif %}
-    BIND(xsd:boolean(?collaborator_account = <account:{{account_uuid}}>) AS ?is_shared_with_me)
+    {%- if account_uuid is not none %}
+    BIND(xsd:boolean(?collaborator_account = <account:{{account_uuid}}> &&
+                     ?account != <account:{{account_uuid}}>) AS ?is_shared_with_me)
+    {%- else %}
+    BIND("false"^^xsd:boolean AS ?is_shared_with_me)
+    {%- endif %}
   }
 {%- if is_under_review is not none: %}
 {%- if is_under_review: %}
 FILTER (?is_under_review = "true"^^xsd:boolean)
 {%- else %}
 FILTER (?is_under_review = "false"^^xsd:boolean)
 {%- endif %}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/datasets_missing_dois.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/datasets_missing_dois.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/decline_draft_dataset.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/decline_draft_dataset.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_associations.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_associations.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_collaborator.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_collaborator.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_collection_draft.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_collection_draft.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_dataset_draft.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_dataset_draft.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_dataset_embargo.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_dataset_embargo.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_item_categories.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_item_categories.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_item_from_list.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_item_from_list.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_items_all_from_list.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_items_all_from_list.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/delete_private_links.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/delete_private_links.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/funding.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/funding.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/group.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/group.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/item_collaborative_permissions.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/item_collaborative_permissions.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/latest_datasets_portal.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/latest_datasets_portal.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/missing_checksummed_files_for_container.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/missing_checksummed_files_for_container.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/opendap_to_doi.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/opendap_to_doi.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/private_links.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/private_links.sparql`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 {% extends "prefixes.sparql" %}
 {% block query %}
-SELECT DISTINCT ?id_string ?is_active ?whom ?purpose ?expires_date ?uuid (?link AS ?uri)
+SELECT DISTINCT ?id_string ?is_active ?whom ?purpose ?expires_date ?uuid
+                (?link AS ?uri) (?rest AS ?originating_blank_node)
+                ?order_index
 WHERE {
   GRAPH <{{state_graph}}> {
-    ?item_uri          djht:private_links/rdf:rest*/rdf:first ?link .
+    ?item_uri          djht:private_links/rdf:rest* ?rest .
+    ?rest              rdf:first                ?link ;
+                       djht:index               ?order_index .
     ?item_uri          djht:container           ?container .
     ?container         rdf:type/rdfs:subClassOf djht:Container .
     ?link              rdf:type                 djht:PrivateLink ;
                        djht:id                   ?id_string .
     OPTIONAL { ?link   djht:is_active            ?is_active . }
     OPTIONAL { ?link   djht:whom                 ?whom . }
     OPTIONAL { ?link   djht:purpose              ?purpose . }
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/publish_draft_collection.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/publish_draft_collection.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/publish_draft_dataset.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/publish_draft_dataset.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/quota_requests.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/quota_requests.sparql`

 * *Files 8% similar despite different names*

```diff
@@ -16,11 +16,13 @@
     OPTIONAL { ?account djht:last_name      ?last_name . }
   }
   BIND (STRAFTER(STR(?request), "quota-request:") AS ?uuid)
   {%- if status is not none: %}
   FILTER (?status = {{status | safe}})
   {%- endif %}{% if quota_request_uuid is not none: %}
   FILTER (?request = <quota-request:{{quota_request_uuid}}>)
+  {%- endif %}{% if account_uuid is not none: %}
+  FILTER (?account = <account:{{account_uuid}}>)
   {%- endif %}
 }
 ORDER BY DESC(?created_date)
 {% endblock %}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/references.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/references.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/reviews.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/reviews.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/root_categories.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/root_categories.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/statistics_files.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/statistics_files.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/tags.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/tags.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_account.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_account.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_author.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_author.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_collection.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_collection.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_dataset.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_dataset.sparql`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     ?dataset           djht:embargo_reason       ?embargo_reason .
     {%- endif%}{% if eula is not none or not (is_embargoed or is_restricted) %}
     ?dataset           djht:eula                 ?eula .
     {%- endif%}{% if agreed_to_deposit_agreement is not none %}
     ?dataset           djht:agreed_to_deposit_agreement ?agreed_to_deposit_agreement .
     {%- endif%}{% if agreed_to_publish is not none %}
     ?dataset           djht:agreed_to_publish    ?agreed_to_publish .
+    {%- endif%}{% if git_repository_name is not none %}
+    ?dataset           djht:git_repository_name  ?git_repository_name .
     {%- endif%}{% if container_doi is not none %}
     ?container         djht:doi                  ?container_doi .
     {%- endif%}{% if first_online_date is not none %}
     ?container         djht:first_online_date    ?first_online_date .
     {%- endif%}
     ?dataset           djht:modified_date        ?modified_date .
   }
@@ -132,14 +134,16 @@
     ?dataset           djht:embargo_reason       {{embargo_reason | safe}} .
     {%- endif%}{% if eula is not none and (is_embargoed or is_restricted) %}
     ?dataset           djht:eula                 {{eula | safe}} .
     {%- endif%}{% if agreed_to_deposit_agreement is not none %}
     ?dataset           djht:agreed_to_deposit_agreement {{agreed_to_deposit_agreement | safe}} .
     {%- endif%}{% if agreed_to_publish is not none %}
     ?dataset           djht:agreed_to_publish    {{agreed_to_publish | safe}} .
+    {%- endif%}{% if git_repository_name is not none %}
+    ?dataset          djht:git_repository_name  {{git_repository_name | safe}} .
     {%- endif%}{% if container_doi is not none %}
     ?container         djht:doi                  {{container_doi | safe}} .
     {%- endif%}{% if first_online_date is not none %}
     ?container         djht:first_online_date    "{{first_online_date | safe}}"^^xsd:dateTime .
     {%- endif%}
     ?dataset           djht:modified_date        "{{modified_date | safe}}"^^xsd:dateTime .
   }
@@ -190,14 +194,15 @@
     OPTIONAL { ?dataset djht:embargo_until_date    ?embargo_until_date . }
     OPTIONAL { ?dataset djht:embargo_type          ?embargo_type . }
     OPTIONAL { ?dataset djht:embargo_title         ?embargo_title . }
     OPTIONAL { ?dataset djht:embargo_reason        ?embargo_reason . }
     OPTIONAL { ?dataset djht:eula                  ?eula . }
     OPTIONAL { ?dataset djht:agreed_to_deposit_agreement ?agreed_to_deposit_agreement . }
     OPTIONAL { ?dataset djht:agreed_to_publish     ?agreed_to_publish . }
+    OPTIONAL { ?dataset djht:git_repository_name   ?git_repository_name . }
     OPTIONAL { ?container djht:doi                 ?container_doi . }
     OPTIONAL { ?container djht:first_online_date   ?first_online_date . }
   }
 {%- if account_uuid is not none: %}
   {%- if disable_collaboration %}
   FILTER (?account = <account:{{account_uuid}}>)
   {%- else %}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_dataset_thumb.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_dataset_thumb.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_file.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_file.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_git_uuid.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_git_uuid.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_orcid_for_account.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_orcid_for_account.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_private_link.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_private_link.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_quota_request.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_quota_request.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_review.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_review.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_session.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_session.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/sparql_templates/update_view_and_download_counts.sparql` & `djehuty-24.5/src/djehuty/web/resources/sparql_templates/update_view_and_download_counts.sparql`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/css/dropzone.min.css` & `djehuty-24.5/src/djehuty/web/resources/static/css/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/css/form.css` & `djehuty-24.5/src/djehuty/web/resources/static/css/form.css`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/css/jquery.dataTables.min.css` & `djehuty-24.5/src/djehuty/web/resources/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/css/main.css` & `djehuty-24.5/src/djehuty/web/resources/static/css/main.css`

 * *Files 5% similar despite different names*

```diff
@@ -600,7 +600,62 @@
 }
 .notice-box {
     border: solid 2pt #ffeecc;
     background: #fffaea;
     padding: 0em 0.5em 0em 0.5em;
     margin: 1em 0em 0em 0em;
 }
+#top-datasets th { text-align: left; white-space: nowrap; color: #ffffff; padding: .5em; }
+#top-datasets-wrapper table { width: 100%; max-width: 880pt; }
+#top-datasets tbody tr td { padding: .5em; z-index: 50; }
+#top-datasets tbody tr:nth-child(odd) { background: #fafafa; }
+#top-datasets tbody tr td:last-child { text-align: right; width: 130pt; }
+#top-datasets thead tr th:last-child { text-align: right; }
+#top-datasets tbody tr td:nth-child(1) {
+    text-overflow: ellipsis;
+    overflow: hidden;
+    white-space: nowrap;
+    max-width: 750pt;
+}
+#top-datasets td { text-align: left; }
+.tile-item {
+    display: inline-block;
+    margin: 0pt 10pt 10pt 0pt;
+    padding: 10pt;
+    width: 135pt;
+    border-radius: 10pt;
+    cursor: pointer;
+    background: #f9f9f9;
+}
+.tile-item:hover { background: #eeeeee; }
+.tile-item:active { background: #e9e9e9; }
+.tile-title {
+    display: -webkit-box;
+    -webkit-line-clamp: 3;
+    -webkit-box-orient: vertical;
+    text-overflow: ellipsis;
+    overflow: hidden;
+    max-width: 150pt;
+    height: 4em;
+    font-size: 1.3em;
+    font-weight: bold;
+}
+.tile-title a:hover { color: #666666; }
+.tile-preview {
+    overflow: hidden;
+    width: 100%;
+    height: 130pt;
+    margin: 0 auto;
+    user-select: none;
+}
+.tabs ul { margin: 0em; padding: 0em; }
+.tabs li {
+    display: inline-block;
+    list-style-type: none;
+    text-decoration: none;
+    color: #000000;
+    font-size: 12pt;
+    padding: .5em .75em .5em .75em;
+    margin: 0pt 5pt 0pt 0pt;
+    user-select: none;
+    border-radius: .5em .5em 0em 0em;
+}
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/css/pub.css` & `djehuty-24.5/src/djehuty/web/resources/static/css/pub.css`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #wrapper #content #funding .funder_name { display: block; color: #999 }
 #wrapper #content #files .size  { display: inline-block; width:120px; font-size:12px; color: #999; text-align:right; margin-right:5px }
 #wrapper #content #files .md5   { font-size: 75%;  color: #333; font-family: monospace; margin: auto 1em auto 1em; }
 #wrapper #content #metadata #left_column  { width: 65%; margin-bottom:10px }
 #wrapper #content #metadata #right_column { float: right; width: 33%; margin-bottom:10px }
 #wrapper #content .warning      { background-color: #ff0 }
 #wrapper #content .label        { text-transform: uppercase }
-#wrapper #content ul            { list-style-type: none; padding:0; margin-top:20px}
+#wrapper #content ul            { list-style-type: none; padding:0; margin:0}
 #wrapper #content #data         { clear: right; border-top: 1px solid #000; margin-bottom: 10px }
 #wrapper #content #collect,      #cite,      #versions      { display: none; border: 3px solid #f39000; padding: 10px; margin-bottom:10px; border-radius: 10px }
 #wrapper #content #collect_show, #cite_show                 { border: none; padding:3px; margin-bottom: 10px; border-radius: 10px; text-aligh: center; width:70px }
 #wrapper #content #collect_hide, #cite_hide, #versions_hide { border: none }
 #wrapper #content #citation     { font-weight: bold }
 #wrapper #content #type_versions { margin-bottom:10px }
 #wrapper #content #versions     { width: 220px; position:absolute; background-color: #fff }
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/css/quill.4tu.css` & `djehuty-24.5/src/djehuty/web/resources/static/css/quill.4tu.css`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/FiraMono-Regular.ttf` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/FiraMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Bold.ttf` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/SourceSansPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Italic.ttf` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/SourceSansPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/SourceSansPro-Regular.ttf` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/SourceSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.eot` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.ttf` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.woff` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-brands-400.woff2` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.eot` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.ttf` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.woff` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/fonts/fa-solid-900.woff2` & `djehuty-24.5/src/djehuty/web/resources/static/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/CoreTrustSeal.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/CoreTrustSeal.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/collection-thumb.svg` & `djehuty-24.5/src/djehuty/web/resources/static/images/collection-thumb.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/dataset-thumb.svg` & `djehuty-24.5/src/djehuty/web/resources/static/images/dataset-thumb.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/ext-link.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/ext-link.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/favicon.ico` & `djehuty-24.5/src/djehuty/web/resources/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/favicon.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/apache.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/licenses/apache.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-0.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-0.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc-nd.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-nc-nd.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc-sa.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-nc-sa.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nc.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-nc.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-nd.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-nd.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by-sa.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by-sa.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/cc-by.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/licenses/cc-by.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/licenses/gnu-gpl-v3.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/licenses/gnu-gpl-v3.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logo-delft.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/logo-delft.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logo-eindhoven.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/logo-eindhoven.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logo-gray.svg` & `djehuty-24.5/src/djehuty/web/resources/static/images/logo-gray.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logo-other.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/logo-other.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logo-twente.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/logo-twente.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logo-wageningen.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/logo-wageningen.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logo.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tudelft.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/logosleft-white-tudelft.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-tutwente.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/logosleft-white-tutwente.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/logosleft-white-wageningen.png` & `djehuty-24.5/src/djehuty/web/resources/static/images/logosleft-white-wageningen.png`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/nikhef-black.svg` & `djehuty-24.5/src/djehuty/web/resources/static/images/nikhef-black.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/orcid.svg` & `djehuty-24.5/src/djehuty/web/resources/static/images/orcid.svg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/aerospace-engineering.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/aerospace-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/agricultural-and-veterinary-sciences.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/agricultural-and-veterinary-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/atmospheric-sciences.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/atmospheric-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/biology.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/biology.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/built-environment-and-design.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/built-environment-and-design.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/business-and-management.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/business-and-management.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/chemistry.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/chemistry.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/civil-engineering.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/civil-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/earth-sciences.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/earth-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/electrical-and-electronic-engineering.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/electrical-and-electronic-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/environmental-sciences.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/environmental-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/geomatic-engineering.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/geomatic-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/information-and-computing-sciences.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/information-and-computing-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/materials-engineering.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/materials-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/mathematics.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/mathematics.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/mechanical-engineering.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/mechanical-engineering.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/medical-and-health-sciences.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/medical-and-health-sciences.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/nanotechnology.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/nanotechnology.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/other-institutions.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/other-institutions.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/physical-geography-and-environmental-geoscience.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/physical-geography-and-environmental-geoscience.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/physics.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/physics.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/tudelft.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/tudelft.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/tueindhoven.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/tueindhoven.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/utwente.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/utwente.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/images/portal/wageningen.jpg` & `djehuty-24.5/src/djehuty/web/resources/static/images/portal/wageningen.jpg`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/ace/ace.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/ace/ace.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/ace/ext-language_tools.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/ace/ext-searchbox.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/ace/ext-searchbox.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/ace/mode-sparql.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/ace/mode-sparql.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/ace/theme-crimson_editor.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/ace/theme-crimson_editor.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/d3.v7.min.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/d3.v7.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/dataset_landing_page.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/dataset_landing_page.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
         contentType: "application/json",
         accept: "application/json",
         data: JSON.stringify({
             "articles": [dataset_id]
         }),
     }).done(function() {
         show_message("success", "<p>Dataset succesfully added to collection.</p>");
-        document.getElementById("collect").style.display = "none"
+        document.getElementById("collect").style.display = "none";
     }).fail(function() {
         console.log(`Failed to add ${dataset_id}`);
         show_message("failure", "<p>Failed to add dataset to collection.</p>");
     });
 }
 
 function toggle_access_request(event) {
@@ -38,15 +38,15 @@
     event.stopPropagation();
     let data = {
         "email": or_null(jQuery("#access-request-email").val()),
         "name": or_null(jQuery("#access-request-name").val()),
         "dataset_id": or_null(jQuery("#access-request-dataset-id").val()),
         "version": or_null(jQuery("#access-request-version").val()),
         "reason": or_null(jQuery("#access-request-reason .ql-editor").html())
-    }
+    };
     jQuery.ajax({
         url: `/data_access_request`,
         type: "POST",
         contentType: "application/json",
         accept: "application/json",
         data: JSON.stringify(data),
         dataType: "json"
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/depositor-dashboard.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/depositor-dashboard.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -12,24 +12,26 @@
 
 }
 
 function submit_storage_request(event) {
     let data = {
         "new-quota": or_null(jQuery("#new-quota").val()),
         "reason": or_null(jQuery("#quota-reason .ql-editor").html())
-    }
+    };
     jQuery.ajax({
         url: `/v3/profile/quota-request`,
         type: "POST",
         contentType: "application/json",
         accept: "application/json",
         data: JSON.stringify(data),
         dataType: "json"
     }).done(function() {
         show_message("success", "<p>Quota request has been sent.</p>");
+        jQuery(".quota-requested").remove();
+        jQuery(".storage-usage").after(`<span class="quota-requested">Request pending for ${data["new-quota"]}.00GB</span>`);
         toggle_storage_request(null);
     }).fail(function() {
         show_message("failure", "<p>Quota request could not be sent.</p>");
     });
 }
 
 jQuery(document).ready(function() {
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/dropzone.min.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/edit-collection.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/edit-collection.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -315,33 +315,33 @@
 
 function delete_collection(collection_id, event) {
     event.preventDefault();
     event.stopPropagation();
     if (confirm("Deleting this draft collection is unrecoverable. " +
             "Do you want to continue?")) {
         jQuery.ajax({
-                url: `/v2/account/collections/${collection_id}`,
                 type: "DELETE",
+                url: `/v2/account/collections/${collection_id}`
             }).done(function() {
-                window.location.pathname = '/my/collections'
+                window.location.pathname = "/my/collections";
             })
             .fail(function() {
                 show_message("failure", "<p>Failed to delete collection.</p>");
             });
     }
 }
 
 function gather_form_data() {
     let categories = jQuery("input[name='categories']:checked");
-    let category_ids = []
+    let category_ids = [];
     for (let category of categories) {
         category_ids.push(jQuery(category).val());
     }
 
-    let group_id = jQuery("input[name='groups']:checked")[0]
+    let group_id = jQuery("input[name='groups']:checked")[0];
     if (group_id !== undefined) {
         group_id = group_id["value"];
     } else {
         group_id = null;
     }
 
     let form_data = {
@@ -354,15 +354,15 @@
         "latitude": or_null(jQuery("#latitude").val()),
         "organizations": or_null(jQuery("#organizations").val()),
         "publisher": or_null(jQuery("#publisher").val()),
         "language": or_null(jQuery("#language").val()),
         "time_coverage": or_null(jQuery("#time_coverage").val()),
         "group_id": group_id,
         "categories": category_ids
-    }
+    };
 
     return form_data;
 }
 
 function save_collection(collection_id, event, notify = true, on_success = jQuery.noop) {
     event.preventDefault();
     event.stopPropagation();
@@ -431,15 +431,15 @@
         type: "POST",
         accept: "application/json",
     }).done(function(record) {
         jQuery("#doi-wrapper p").replaceWith(
             `<p>The DOI of your collection will be: <strong>${record["doi"]}</strong></p>`
         );
     }).fail(function() {
-        show_message("failure", "<p>Failed to reserve DOI. Please try again later.</p>")
+        show_message("failure", "<p>Failed to reserve DOI. Please try again later.</p>");
     });
 }
 
 function autocomplete_dataset(event, collection_id) {
     let current_text = jQuery.trim(jQuery("#article-search").val());
     if (current_text == "") {
         jQuery("#articles-ac").remove();
@@ -500,16 +500,16 @@
                 if (item["orcid_id"] != null && item["orcid_id"] != "") {
                     html += ` (${item["orcid_id"]})`;
                 }
                 html += "</a>";
             }
             html += "</ul>";
 
-            html += `<div id="new-author" class="a-button"><a href="#" `
-            html += `onclick="javascript:new_author('${collection_id}'); `
+            html += `<div id="new-author" class="a-button"><a href="#" `;
+            html += `onclick="javascript:new_author('${collection_id}'); `;
             html += `return false;">Create new author record</a></div>`;
             jQuery("#authors")
                 .addClass("input-for-ac")
                 .after(`<div id="authors-ac" class="autocomplete">${html}</div>`);
         });
     }
 }
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/edit-dataset.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/edit-dataset.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 function delete_dataset(dataset_uuid, event) {
     event.preventDefault();
     event.stopPropagation();
     if (confirm("Deleting this draft dataset is unrecoverable. " +
             "Do you want to continue?")) {
         jQuery.ajax({
-                url: `/v2/account/articles/${dataset_uuid}`,
                 type: "DELETE",
+                url: `/v2/account/articles/${dataset_uuid}`
             }).done(function() {
-                window.location.pathname = '/my/datasets'
+                window.location.pathname = "/my/datasets";
             })
             .fail(function(jqXHR, textStatus, errorThrown) {
                 if (jqXHR.status == 403) {
                     show_message("failure", "<p>No permission to remove dataset.</p>");
                 } else {
                     show_message("failure", "<p>Failed to remove dataset.</p>");
                 }
@@ -20,27 +20,27 @@
 }
 
 function decline_dataset(dataset_uuid, event) {
     event.preventDefault();
     event.stopPropagation();
 
     jQuery("#content").addClass("loader-top");
-    jQuery("#content-wrapper").css('opacity', '0.15');
+    jQuery("#content-wrapper").css("opacity", "0.15");
     save_dataset(dataset_uuid, event, false, function() {
         jQuery.ajax({
-            url: `/v3/datasets/${dataset_uuid}/decline`,
-            type: "POST",
             accept: "application/json",
+            type: "POST",
+            url: `/v3/datasets/${dataset_uuid}/decline`
         }).done(function() {
             window.location.replace("/logout");
         }).fail(function(response, text_status, error_code) {
             show_message("failure",
                 `<p>Could not decline due to error ` +
                 `<code>${error_code}</code>.</p>`);
-            jQuery("#content-wrapper").css('opacity', '1.0');
+            jQuery("#content-wrapper").css("opacity", "1.0");
             jQuery("#content").removeClass("loader-top");
         });
     });
 }
 
 function preview_dataset(dataset_uuid, event) {
     event.preventDefault();
@@ -54,21 +54,21 @@
     }
     if (day < 10) {
         day = `0${day}`;
     }
 
     save_dataset(dataset_uuid, event, false, function() {
         jQuery.ajax({
-            url: `/v2/account/articles/${dataset_uuid}/private_links`,
-            type: "POST",
-            contentType: "application/json",
             accept: "application/json",
+            contentType: "application/json",
             data: JSON.stringify({
                 "expires_date": `${year}-${month}-${day}`
             }),
+            type: "POST",
+            url: `/v2/account/articles/${dataset_uuid}/private_links`
         }).done(function(data) {
             let preview_window = window.open(data["location"], '_blank');
             if (preview_window) {
                 preview_window.focus();
             } else {
                 show_message("failure",
                     "<p>Cannot open preview window because your " +
@@ -80,27 +80,27 @@
                 `<code>${error_code}</code>.</p>`);
         });
     });
 }
 
 function gather_form_data() {
     let categories = jQuery("input[name='categories']:checked");
-    let category_ids = []
+    let category_ids = [];
     for (let category of categories) {
         category_ids.push(jQuery(category).val());
     }
 
     let defined_type_name = null;
     if (jQuery("#upload_software").prop("checked")) {
         defined_type_name = "software";
     } else {
         defined_type_name = "dataset";
     }
 
-    let group_id = jQuery("input[name='groups']:checked")[0]
+    let group_id = jQuery("input[name='groups']:checked")[0];
     if (group_id !== undefined) {
         group_id = group_id["value"];
     } else {
         group_id = null;
     }
 
     let is_embargoed = jQuery("#embargoed_access").prop("checked");
@@ -121,23 +121,24 @@
         "data_link": or_null(jQuery("#data_link").val()),
         "derived_from": or_null(jQuery("#derived_from").val()),
         "same_as": or_null(jQuery("#same_as").val()),
         "organizations": or_null(jQuery("#organizations").val()),
         "publisher": or_null(jQuery("#publisher").val()),
         "time_coverage": or_null(jQuery("#time_coverage").val()),
         "language": or_null(jQuery("#language").val()),
+        "git_repository_name": or_null(jQuery("#git-repository-name").val()),
         "is_metadata_record": is_metadata_record,
         "metadata_reason": or_null(jQuery("#metadata_only_reason").val()),
         "defined_type": defined_type_name,
         "is_embargoed": is_embargoed || is_restricted,
         "group_id": group_id,
         "agreed_to_deposit_agreement": agreed_to_da,
         "agreed_to_publish": agreed_to_publish,
         "categories": category_ids
-    }
+    };
 
     if (is_embargoed) {
         form_data["embargo_until_date"] = or_null(jQuery("#embargo_until_date").val());
         form_data["embargo_title"] = "Under embargo";
         form_data["embargo_reason"] = or_null(jQuery("#embargo_reason .ql-editor").html());
         form_data["license_id"] = or_null(jQuery("#license_embargoed").val());
         if (jQuery("#files_only_embargo").prop("checked")) {
@@ -151,15 +152,15 @@
         form_data["embargo_until_date"] = null;
         form_data["embargo_title"] = "Restricted access";
         form_data["embargo_reason"] = or_null(jQuery("#restricted_access_reason .ql-editor").html());
         form_data["eula"] = or_null(jQuery("#restricted_access_eula .ql-editor").html());
         form_data["embargo_options"] = [{
             "id": 1000,
             "type": "restricted_access"
-        }]
+        }];
     } else {
         form_data["license_id"] = or_null(jQuery("#license_open").val());
     }
 
     return form_data;
 }
 
@@ -210,30 +211,30 @@
         jQuery.ajax({
             url: `/v3/datasets/${dataset_uuid}/repair_md5s`,
             type: "GET",
             accept: "application/json",
         }).done(function(record) {
             location.reload();
         }).fail(function() {
-            show_message("failure", "<p>Failed to repair MD5 checksums.</p>")
+            show_message("failure", "<p>Failed to repair MD5 checksums.</p>");
         });
     });
 }
 
 function reserve_doi(dataset_uuid) {
     jQuery.ajax({
         url: `/v2/account/articles/${dataset_uuid}/reserve_doi`,
         type: "POST",
         accept: "application/json",
     }).done(function(record) {
         jQuery("#doi-wrapper p").replaceWith(
             `<p>The DOI of your dataset will be: <strong>${record["doi"]}</strong></p>`
         );
     }).fail(function() {
-        show_message("failure", "<p>Failed to reserve DOI. Please try again later.</p>")
+        show_message("failure", "<p>Failed to reserve DOI. Please try again later.</p>");
     });
 }
 
 function render_licenses(dataset) {
     let chosen_license = null;
     // When the dataset hasn't been given a license yet, accessing
     // license.value will throw a TypeError. This is expected.
@@ -261,15 +262,15 @@
                 continue;
             }
             let selected = ((chosen_license == license.value) ? " selected" : "");
             let html = `<option value="${license.value}"${selected}>${license.name}</option>`;
             jQuery(".license-selector").append(html);
         }
     }).fail(function() {
-        show_message("failure", "<p>Failed to retrieve license list.</p>")
+        show_message("failure", "<p>Failed to retrieve license list.</p>");
     });
 }
 
 function render_categories_for_dataset(dataset_uuid) {
     jQuery.ajax({
         url: `/v2/account/articles/${dataset_uuid}/categories`,
         data: {
@@ -280,15 +281,15 @@
     }).done(function(categories) {
         for (let category of categories) {
             jQuery(`#category_${category["uuid"]}`).prop("checked", true);
             jQuery(`#category_${category["parent_uuid"]}`).prop("checked", true);
             jQuery(`#subcategories_${category["parent_uuid"]}`).show();
         }
     }).fail(function() {
-        show_message("failure", "<p>Failed to retrieve categories.</p>")
+        show_message("failure", "<p>Failed to retrieve categories.</p>");
     });
 }
 
 function render_references_for_dataset(dataset_uuid) {
     jQuery.ajax({
         url: `/v3/datasets/${dataset_uuid}/references`,
         data: {
@@ -322,26 +323,26 @@
             "order": "asc",
             "order_direction": "id"
         },
         type: "GET",
         accept: "application/json",
     }).done(function(collaborators) {
         jQuery("#collaborators-form tbody").empty();
-        let row = '<tr>';
+        let row = "<tr>";
         if (may_edit_metadata) {
             row += '<td><input type="text" id="add_collaborator" name="add_collaborator" value=""/>';
             row += '<input type="hidden" id="account_uuid" name="account_uuid" value=""/></td>';
             row += '<td class="type-begin"><input class="subitem-checkbox-metadata" name="read" type="checkbox" checked="checked" disabled="disabled"></td>';
             row += '<td class="type-end"><input class="subitem-checkbox-metadata" name="edit" type="checkbox"></td>';
             row += '<td><input class="subitem-checkbox-data" name="read" type="checkbox"></td>';
             row += '<td><input class="subitem-checkbox-data" name="edit" type="checkbox"></td>';
             row += '<td class="type-end"><input class="subitem-checkbox-data" name="remove" type="checkbox"></td>';
             row += '<td><a id="add-collaborator-button" class="fas fa-plus" href="#" ';
             row += 'title="Add collaborator"></a></td>';
-            row += '</tr>';
+            row += "</tr>";
             jQuery("#collaborators-form tbody").append(row);
             jQuery("#add-collaborator-button").on("click", function(event) {
                 event.preventDefault();
                 event.stopPropagation();
                 add_collaborator(dataset_uuid, may_edit_metadata);
             });
         }
@@ -387,15 +388,15 @@
         },
         "data": {
             "read": jQuery("input[name='read'].subitem-checkbox-data").prop("checked"),
             "edit": jQuery("input[name='edit'].subitem-checkbox-data").prop("checked"),
             "remove": jQuery("input[name='remove'].subitem-checkbox-data").prop("checked"),
         },
         "account": or_null(jQuery("#account_uuid").val())
-    }
+    };
 
     jQuery.ajax({
         url: `/v3/datasets/${dataset_uuid}/collaborators`,
         type: "POST",
         contentType: "application/json",
         accept: "application/json",
         data: JSON.stringify(form_data),
@@ -454,27 +455,27 @@
 
 function update_author(author_uuid, dataset_uuid) {
     let record = {
         "first_name": jQuery("#edit_author_first_name").val(),
         "last_name": jQuery("#edit_author_last_name").val(),
         "email": jQuery("#edit_author_email").val(),
         "orcid": jQuery("#edit_author_orcid").val()
-    }
+    };
     jQuery.ajax({
         url: `/v3/authors/${author_uuid}`,
         data: JSON.stringify(record),
         type: "PUT",
         contentType: "application/json",
         accept: "application/json",
     }).done(function() {
         cancel_edit_author(author_uuid, dataset_uuid);
         render_authors_for_dataset(dataset_uuid);
     }).fail(function() {
         show_message("failure", "<p>Failed to update author details.</p>");
-    })
+    });
 }
 
 function edit_author(author_uuid, dataset_uuid) {
     jQuery.ajax({
         url: `/v3/datasets/${dataset_uuid}/authors/${author_uuid}`,
         type: "GET",
         accept: "application/json",
@@ -777,15 +778,15 @@
                     accept: "application/json",
                     data: JSON.stringify({
                         "uuid": `${selected_thumb.val()}`
                     })
                 }).fail(function() {
                     show_message("failure", "<p>Failed to set thumbnail.</p>");
                 });
-            })
+            });
         } else {
             jQuery("#thumbnails-wrapper").hide();
             jQuery("#thumbnail-files-wrapper").hide();
         }
     }).fail(function() {
         show_message("failure", "<p>Failed to retrieve thumbnail file details.</p>");
     });
@@ -1187,15 +1188,15 @@
                 done();
                 fileUploader.processQueue();
             },
             complete: function(file) {
                 if (fileUploader.getUploadingFiles().length === 0 &&
                     fileUploader.getQueuedFiles().length === 0) {
                     let rejected_files = fileUploader.getRejectedFiles();
-                    for (rejected of rejected_files) {
+                    for (let rejected of rejected_files) {
                         if (rejected.status == "error") {
                             show_message("failure", `<p>Failed to upload '${rejected.upload.filename}'.</p>`);
                         }
                     }
                     render_files_for_dataset(dataset_uuid, fileUploader);
                 } else {
                     fileUploader.processQueue();
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/edit-profile.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/edit-profile.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,26 @@
 function save_profile(notify = true, on_success = jQuery.noop) {
 
     let categories = jQuery("input[name='categories']:checked");
-    let category_ids = []
+    let category_ids = [];
     for (let category of categories) {
         category_ids.push(jQuery(category).val());
     }
 
     let form_data = {
         "first_name": or_null(jQuery("#first_name").val()),
         "last_name": or_null(jQuery("#last_name").val()),
         "job_title": or_null(jQuery("#job_title").val()),
         "location": or_null(jQuery("#location").val()),
         "biography": or_null(jQuery("#biography").val()),
         "twitter": or_null(jQuery("#twitter").val()),
         "linkedin": or_null(jQuery("#linkedin").val()),
         "website": or_null(jQuery("#website").val()),
         "categories": category_ids
-    }
+    };
 
     jQuery.ajax({
         url: "/v3/profile",
         type: "PUT",
         contentType: "application/json",
         accept: "application/json",
         data: JSON.stringify(form_data),
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/exploratory.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/exploratory.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -11,17 +11,17 @@
 }
 
 function draw_grid() {
     let explorer = d3.select("#data-model-explorer");
     let width = parseInt(explorer.style("width"));
     let height = parseInt(explorer.style("height"));
 
-    explorer.select("#grid").remove()
-    let grid = explorer.append("g").attr("id", "grid")
-    grid.lower()
+    explorer.select("#grid").remove();
+    let grid = explorer.append("g").attr("id", "grid");
+    grid.lower();
     for (let x = 10; x < width; x += 10) {
         // Vertical lines
         grid.append("line")
             .attr("x1", x)
             .attr("y1", 0)
             .attr("x2", x)
             .attr("y2", height + 1)
@@ -35,22 +35,22 @@
             .classed(((x == 40) ? "highlighted-grid-line" : "grid-line"), true);
     }
 }
 
 function draw_column_title(column, value) {
     let translate_x = 20 + column * 290;
     let explorer = d3.select("#data-model-explorer");
-    explorer.selectAll(`.node-${column}-column-title`).remove()
+    explorer.selectAll(`.node-${column}-column-title`).remove();
     let title_group = explorer.append("g")
         .attr("transform", "translate(" + translate_x + ",20)")
         .classed(`node-${column}-column-title`, true);
     title_group
         .append("text").text(value)
         .attr("transform", "translate(0, 11)")
-        .classed("node-column-title", true)
+        .classed("node-column-title", true);
 }
 
 function resize_svg() {
     let explorer = d3.select("#data-model-explorer");
 
     // Determine the maximum rows to adjust for.
     let column_0_rows = explorer.selectAll(".column-0").size();
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/jquery-3.6.0.min.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/jquery.dataTables.min.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/query-editor.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/query-editor.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,10 @@
 var editor = null;
 
 function execute_query(editor) {
-
-    url = window.location.href;
     jQuery("#button-wrapper").after(
         "<div class=\"query-data-loader\">" +
         "<div class=\"title\">Loading data ...</div>" +
         "<div class=\"content\">Please wait for the results to appear.</div>" +
         "</div>");
 
     /* Remove the previous query results. */
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/quill.min.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/quill.min.js`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/ranking.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/ranking.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
-const capitalize = (i) => (i[0].toUpperCase() + i.substring(1))
+const capitalize = (i) => (i[0].toUpperCase() + i.substring(1));
 
 function parameters_for_api_calls(order) {
     let parameters = {
         "limit": 10,
         "order_direction": "desc",
         "order": order
-    }
+    };
 
     // This procedure is used by both institutional pages which filter by 'group_ids'
     // and category pages which filter by 'categories'.  So one of these variables
     // won't be defined, but that's expected.
     try {
         if (categories !== "") {
             jQuery.extend(parameters, {
@@ -72,15 +72,15 @@
             output += '<a href="/datasets/' + data[index].container_uuid + '">';
             output += data[index].title + '</a>';
             output += '</td>';
             output += '<td>' + data[index][item_type] + '</td></tr>';
         });
 
         output += "</tbody></table>";
-        jQuery("#top-datasets").remove()
+        jQuery("#top-datasets").remove();
         jQuery("#top-datasets-wrapper").removeClass("loader");
         jQuery("#top-datasets-wrapper").append(output);
     }).fail(function() {
         jQuery("#top-datasets-wrapper").append("<p>Could not load the top datasets.</p>");
     });
 }
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/review-overview.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/review-overview.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -40,15 +40,15 @@
     let value = jQuery(".reviewer-filter option:selected").val();
     let name = cleanup_name(jQuery(".reviewer-filter option:selected").text());
     jQuery('#overview-table tr').each(function(index, element) {
         let reviewer_element = jQuery(element).find(`td .reviewer-selector option:selected`);
         let status = jQuery(element).find(`td:nth-child(6)`).text().trim();
         if (jQuery(element).find("th").length > 0) {} // Skip the header.
         else if (value == "all") {} else if (value == "unassigned" && reviewer_element.length > 0 && reviewer_element.val() == "") {} else if (reviewer_element.length > 0 && reviewer_element.val().split(":").pop() == value) {} else if (status == "approved") {
-            let reviewer = jQuery(element).find(`td:nth-child(10)`).text()
+            let reviewer = jQuery(element).find(`td:nth-child(10)`).text();
             let reviewer_name = cleanup_name(reviewer);
             if (reviewer_name != name) {
                 jQuery(element).hide();
             }
         } else {
             jQuery(element).hide();
         }
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/search.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/search.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -361,14 +361,15 @@
                     search_for = search_for.substring(0, max_parameter_length);
                     jQuery("#search-box").val(search_for);
                 }
             }
 
             if (filter_name in filter_info) {
                 for (let value of values) {
+                    value = value.replace(/[^a-zA-Z0-9-_]/g, '');
                     let checkbox_id = `checkbox_${filter_name}_${value}`;
                     let checkbox_id_element = jQuery(`#${checkbox_id}`);
                     if (checkbox_id_element.length > 0) {
                         jQuery(`#${checkbox_id}`).prop("checked", true);
                         if (filter_name == "categories") {
                             toggle_filter_categories_showmore(true);
                             if (enable_subcategories) {
@@ -408,128 +409,81 @@
                 continue;
             }
         }
     }
 }
 
 function load_search_results() {
-    let api_dataset_url = "/v2/articles/search";
     let api_collection_url = "/v2/collections/search";
-    let request_params = parse_url_params();
+    let api_dataset_url = "/v3/datasets/search";
     let target_api_url = null;
+    let url_params = parse_url_params();
+    let request_params = {};
 
-    if ("datatypes" in request_params && request_params["datatypes"] === "collection") {
+    if ("datatypes" in url_params && url_params["datatypes"] === "collection") {
         target_api_url = api_collection_url;
     } else {
         target_api_url = api_dataset_url;
-        request_params["item_type"] = request_params["datatypes"];
+        request_params["item_type"] = url_params["datatypes"];
     }
 
-    let search_for = "";
-    if ("searchscope" in request_params && typeof(request_params["searchscope"]) === "string" && request_params["searchscope"].length > 0) {
-
-        // If there's no search terms, show an error message.
-        if (!("search" in request_params) || typeof(request_params["search"]) === "string" && request_params["search"].length == 0) {
-            let error_message = `Search Scope requires search terms(s).`;
-            jQuery("#search-error").html(error_message);
-            jQuery("#search-error").show();
-            return;
-        }
-
-        let temp_search_for = "";
-        let items = request_params["searchscope"];
-        let iterated = 0;
-        for (let scope of items.split(",")) {
-            iterated += 1;
-            temp_search_for += `:${scope}: ${request_params["search"]} OR `;
-        }
-        if (temp_search_for.endsWith(" OR ")) {
-            temp_search_for = temp_search_for.slice(0, -4);
-        }
-        if (temp_search_for.length > 0) {
-            if (iterated > 1) {
-                search_for = `( ${temp_search_for} )`;
-            } else {
-                search_for = `${temp_search_for}`;
-            }
+    if ("searchscope" in url_params && typeof(url_params["searchscope"]) === "string" && url_params["searchscope"].length > 0) {
+        let value = url_params["searchscope"];
+        let scopes = [];
+        for (let scope of value.split(",")) {
+            scopes.push(scope);
         }
+        request_params["search_scope"] = scopes;
     } else {
         // If searchscope is not selected, search in title, description, and tags.
-        if ("search" in request_params && typeof(request_params["search"]) === "string" && request_params["search"].length > 0) {
-            search_for = `( :title: ${request_params["search"]} OR :description: ${request_params["search"]} OR :tag: ${request_params["search"]} )`;
-        }
+        request_params["search_scope"] = ["title", "description", "tag"];
     }
 
-    if (("filetypes" in request_params && typeof(request_params["filetypes"]) === "string" && request_params["filetypes"].length > 0) || ("filetypes_other" in request_params && typeof(request_params["filetypes_other"]) === "string" && request_params["filetypes_other"].length > 0)) {
-        let temp_search_for = "";
-        let items = request_params["filetypes"];
-        let iterated = 0;
-        if (items && items.length > 0) {
-            for (let scope of items.split(",")) {
-                iterated += 1;
-                temp_search_for += `:format: ${scope} OR `;
+    if (("filetypes" in url_params && typeof(url_params["filetypes"]) === "string" && url_params["filetypes"].length > 0) || ("filetypes_other" in url_params && typeof(url_params["filetypes_other"]) === "string" && url_params["filetypes_other"].length > 0)) {
+        let value = url_params["filetypes"];
+        let formats = [];
+        if (value && value.length > 0) {
+            for (let format of value.split(",")) {
+                formats.push(format);
             }
         }
-        if ("filetypes_other" in request_params && typeof(request_params["filetypes_other"]) === "string" && request_params["filetypes_other"].length > 0) {
-            let filetypes_other = request_params["filetypes_other"];
+        if ("filetypes_other" in url_params && typeof(url_params["filetypes_other"]) === "string" && url_params["filetypes_other"].length > 0) {
+            let filetypes_other = url_params["filetypes_other"];
             filetypes_other = trim_single_word(filetypes_other);
-            temp_search_for += `:format: ${filetypes_other} OR `;
-        }
-        if (temp_search_for.endsWith(" OR ")) {
-            temp_search_for = temp_search_for.slice(0, -4);
-        }
-        if (temp_search_for.length > 0) {
-            if (search_for) {
-                if (iterated > 1) {
-                    search_for += ` AND ( ${temp_search_for} )`;
-                } else {
-                    search_for += ` AND ${temp_search_for}`;
-                }
-            } else {
-                search_for += `${temp_search_for}`;
-            }
+            formats.push(filetypes_other);
         }
+
+        request_params["search_format"] = formats;
     }
 
-    if ("publisheddate" in request_params && typeof(request_params["publisheddate"]) === "string" && request_params["publisheddate"].length > 0) {
+    if ("publisheddate" in url_params && typeof(url_params["publisheddate"]) === "string" && url_params["publisheddate"].length > 0) {
         let today = new Date();
-        let year = today.getFullYear() - request_params["publisheddate"];
+        let year = today.getFullYear() - url_params["publisheddate"];
         let new_date = new Date(year, 0, 1);
         let since_date = new_date.toISOString();
         request_params["published_since"] = `${since_date}`;
-    } else if ("publisheddate_other" in request_params && typeof(request_params["publisheddate_other"]) === "string" && request_params["publisheddate_other"].length > 0) {
-        let new_date = new Date(request_params["publisheddate_other"]);
+    } else if ("publisheddate_other" in url_params && typeof(url_params["publisheddate_other"]) === "string" && url_params["publisheddate_other"].length > 0) {
+        let new_date = new Date(url_params["publisheddate_other"]);
         let since_date = new_date.toISOString();
         request_params["published_since"] = `${since_date}`;
     }
 
-    if ("institutions_other" in request_params && typeof(request_params["institutions_other"]) === "string" && request_params["institutions_other"].length > 0) {
-        let institutions_other = request_params["institutions_other"];
-        institutions_other = trim_single_word(institutions_other);
-        if (search_for) {
-            search_for += ` AND :organizations: ${institutions_other}`;
-        } else {
-            search_for += `:organizations: ${institutions_other}`;
-        }
+    if ("institutions_other" in url_params && typeof(url_params["institutions_other"]) === "string" && url_params["institutions_other"].length > 0) {
+        request_params["organizations"] = trim_single_word(url_params["institutions_other"]);
     }
 
-    if (search_for.length > 0) {
-        request_params["search_for"] = search_for;
-    } else {
-        if ("search" in request_params && typeof(request_params["search"]) === "string" && request_params["search"].length > 0) {
-            request_params["search_for"] = request_params["search"];
-        }
+    request_params["search_for"] = url_params["search"];
+    if (url_params["q"]) {
+        request_params["search_for"] = url_params["q"];
     }
 
-    request_params["group"] = request_params["institutions"];
+    request_params["group"] = url_params["institutions"];
     request_params["page_size"] = page_size;
     request_params["is_latest"] = 1;
-    if (!("page" in request_params)) {
-        request_params["page"] = 1;
-    }
+    request_params["page"] = "page" in url_params ? url_params["page"] : 1;
 
     jQuery("#search-loader").show();
     jQuery("#search-error").hide();
 
     jQuery.ajax({
         url: target_api_url,
         type: "POST",
```

### Comparing `djehuty-24.4/src/djehuty/web/resources/static/js/utils.js` & `djehuty-24.5/src/djehuty/web/resources/static/js/utils.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 function render_in_form(text) {
-    return [text].join('');
+    return [text].join("");
 }
 
 function or_null(value) {
     return (value == "" || value == "<p><br></p>") ? null : value;
 }
 
 function or_empty(value) {
@@ -23,17 +23,16 @@
             jQuery("#message").removeClass(type).addClass("transparent").html("<p>&nbsp;</p>").show();
         });
     }, 20000);
 }
 
 function install_sticky_header() {
     var submenu_offset = jQuery("#submenu").offset().top;
-    jQuery(window).on('resize scroll', function() {
-        let scroll_offset = jQuery(window).scrollTop();
-        if (submenu_offset <= scroll_offset) {
+    jQuery(window).on("resize scroll", function() {
+        if (submenu_offset <= jQuery(window).scrollTop()) {
             jQuery("#submenu").addClass("sticky");
             jQuery("#message").addClass("sticky-message");
             jQuery("h1").addClass("sticky-margin");
             jQuery("#message").width(jQuery("#content-wrapper").width());
         } else {
             jQuery("#submenu").removeClass("sticky");
             jQuery("#message").removeClass("sticky-message");
@@ -180,18 +179,18 @@
                 if (item["orcid_id"] != null && item["orcid_id"] != "") {
                     html += ` (${item["orcid_id"]})`;
                 }
                 html += "</a>";
             }
             html += "</ul>";
 
-            html += `<span id="new-author-description" style='padding: 1em;'><i><center>${new_author_description}</center></i></span>`
+            html += `<span id="new-author-description" style='padding: 1em;'><i><center>${new_author_description}</center></i></span>`;
 
-            html += `<div id="new-author" class="a-button"><a href="#" `
-            html += `onclick="javascript:new_author('${item_id}'); `
+            html += `<div id="new-author" class="a-button"><a href="#" `;
+            html += `onclick="javascript:new_author('${item_id}'); `;
             html += `return false;">Create new author record</a></div>`;
             jQuery("#authors")
                 .addClass("input-for-ac")
                 .after(`<div id="authors-ac" class="autocomplete">${html}</div>`);
         });
     }
 }
@@ -217,16 +216,16 @@
             for (let item of data) {
                 html += `<li><a href="#" `;
                 html += `onclick="javascript:add_funding('${item["uuid"]}', `;
                 html += `'${item_id}'); return false;">${item["title"]}</a>`;
             }
             html += "</ul>";
 
-            html += `<div id="new-funding" class="a-button"><a href="#" `
-            html += `onclick="javascript:new_funding('${item_id}'); `
+            html += `<div id="new-funding" class="a-button"><a href="#" `;
+            html += `onclick="javascript:new_funding('${item_id}'); `;
             html += `return false;">Create funding record</a></div>`;
             jQuery("#funding")
                 .addClass("input-for-ac")
                 .after(`<div id="funding-ac" class="autocomplete">${html}</div>`);
         });
     }
 }
```

### Comparing `djehuty-24.4/src/djehuty/web/ui.py` & `djehuty-24.5/src/djehuty/web/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,14 +482,15 @@
 def read_orcid_configuration (server, xml_root):
     """Procedure to parse and set the ORCID API configuration."""
     orcid = xml_root.find("authentication/orcid")
     if orcid:
         server.orcid_client_id     = config_value (orcid, "client-id")
         server.orcid_client_secret = config_value (orcid, "client-secret")
         server.orcid_endpoint      = config_value (orcid, "endpoint")
+        server.orcid_read_public_token = config_value (orcid, "read-public-token")
 
         # SAML takes precedence over ORCID authentication.
         if server.identity_provider != "saml":
             server.identity_provider   = "orcid"
 
 def read_email_configuration (server, xml_root, logger):
     """Procedure to parse and set the email server configuration."""
@@ -972,14 +973,18 @@
                 logger.warning ("No menu structure provided.")
 
             if shutil.which ("git") is None:
                 logger.error ("Cannot find the 'git' executable.  Please install it.")
                 if server.in_production:
                     raise DependencyNotAvailable
 
+            if server.orcid_client_id is not None and server.orcid_read_public_token is None:
+                if server.obtain_orcid_read_public_token ():
+                    logger.info ("Obtained read-public token from ORCID.")
+
             logger.info ("SPARQL endpoint:  %s.", server.db.endpoint)
             logger.info ("SPARQL update_endpoint:  %s.", server.db.update_endpoint)
             logger.info ("State graph:  %s.", server.db.state_graph)
             logger.info ("Storage path: %s.", server.db.storage)
             logger.info ("Secondary storage path: %s.", server.db.secondary_storage)
             logger.info ("Cache storage path: %s.", server.db.cache.storage)
             logger.info ("Running on %s", server.base_url)
```

### Comparing `djehuty-24.4/src/djehuty/web/validator.py` & `djehuty-24.5/src/djehuty/web/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,14 +196,60 @@
     """Validation procedure for the institution parameter."""
     return integer_value (value, "institution", required=required)
 
 def group (value, required=False):
     """Validation procedure for the group parameter."""
     return integer_value (value, "group", required=required)
 
+def search_filters (value, error_list=None):
+    """Validation procedure for the search_filters parameter."""
+
+    if value is None:
+        return None
+
+    __typed_value (value, "scopes",      list, "list",   error_list=error_list)
+    __typed_value (value, "formats",     list, "list",   error_list=error_list)
+    __typed_value (value, "operator",    str,  "string", error_list=error_list)
+    __typed_value (value, "institution", str,  "string", error_list=error_list)
+
+    for k, v in value.items():
+        if k == "scopes":
+            for elem in v:
+                string_value ({ "value": elem }, "value", 1, 20, required=True)
+                if elem not in ["title", "description", "tag"]:
+                    return raise_or_return_error (error_list,
+                                InvalidValue(
+                                    field_name = "search_filters",
+                                    message = "Invalid value in 'scopes'.",
+                                    code    = "InvalidValue"))
+        elif k == "formats":
+            for elem in v:
+                string_value ({ "value": elem }, "value", 1, 20, required=True)
+
+        elif k == "institution":
+            string_value ({ "value": v }, "value", 1, 50, required=True)
+
+        elif k == "operator":
+            string_value ({ "value": v }, "value", 1, 5, required=True)
+            if v not in ["and", "or", "exact"]:
+                return raise_or_return_error (error_list,
+                            InvalidValueType(
+                                field_name = "search_filters",
+                                message = "Invalid value in 'operator'.",
+                                code    = "WrongValueType"))
+
+        else:
+            return raise_or_return_error (error_list,
+                        InvalidValue(
+                            field_name = "search_filters",
+                            message = f"Invalid key '{k}' in 'search_filters'.",
+                            code    = "InvalidValue"))
+
+    return value
+
 def index_exists (value, index):
     """Procedure to test whether a list or string has a certain length."""
 
     try:
         value[index]
     except IndexError:
         return False
```

### Comparing `djehuty-24.4/src/djehuty/web/wsgi.py` & `djehuty-24.5/src/djehuty/web/wsgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from djehuty.web import database
 from djehuty.web import email_handler
 from djehuty.web import locks
 from djehuty.utils.convenience import pretty_print_size, decimal_coords
 from djehuty.utils.convenience import value_or, value_or_none, deduplicate_list
 from djehuty.utils.convenience import self_or_value_or_none, parses_to_int
 from djehuty.utils.convenience import make_citation, is_opendap_url, landing_page_url
-from djehuty.utils.convenience import split_author_name, split_delimited_string
+from djehuty.utils.convenience import split_author_name, split_string
 from djehuty.utils.constants import group_to_member, member_url_names, filetypes_by_extension
 from djehuty.utils.rdf import uuid_to_uri, uri_to_uuid, uris_from_records
 
 ## Error handling for loading python3-saml is done in 'ui'.
 ## So if it fails here, we can safely assume we don't need it.
 try:
     from onelogin.saml2.auth import OneLogin_Saml2_Auth
@@ -90,14 +90,15 @@
             '</p></div>'
         )
         self.large_footer     = self.small_footer
 
         self.orcid_client_id     = None
         self.orcid_client_secret = None
         self.orcid_endpoint      = None
+        self.orcid_read_public_token = None
         self.identity_provider   = None
 
         self.saml_config_path    = None
         self.saml_config         = None
         self.saml_attribute_email = "urn:mace:dir:attribute-def:mail"
         self.saml_attribute_first_name = "urn:mace:dir:attribute-def:givenName"
         self.saml_attribute_last_name = "urn:mace:dir:attribute-def:sn"
@@ -317,14 +318,15 @@
             R("/v2/account",                                                     self.api_account),
 
             ## ----------------------------------------------------------------
             ## V3 API
             ## ----------------------------------------------------------------
             R("/v3/datasets",                                                    self.api_v3_datasets),
             R("/v3/datasets/codemeta",                                           self.api_v3_datasets_codemeta),
+            R("/v3/datasets/search",                                             self.api_v3_datasets_search),
             R("/v3/datasets/top/<item_type>",                                    self.api_v3_datasets_top),
             R("/v3/datasets/<dataset_id>/submit-for-review",                     self.api_v3_dataset_submit),
             R("/v3/datasets/<dataset_id>/publish",                               self.api_v3_dataset_publish),
             R("/v3/datasets/<dataset_id>/decline",                               self.api_v3_dataset_decline),
             R("/v3/datasets/<container_uuid>/repair_md5s",                       self.api_v3_repair_md5s),
             R("/v3/datasets/<dataset_id>/doi-badge-v<version>.svg",              self.api_v3_doi_badge),
             R("/v3/datasets/<dataset_id>/doi-badge.svg",                         self.api_v3_doi_badge),
@@ -506,42 +508,52 @@
         template = self.jinja.get_template (template_name)
         return self.response (template.render (context), mimetype="text/css")
 
     def __render_template (self, request, template_name, **context):
         template      = self.jinja.get_template (template_name)
         token         = self.token_from_cookie (request)
         account       = self.db.account_by_session_token (token)
-        impersonator_token = self.__impersonator_token (request)
         parameters    = {
-            "base_url":        self.base_url,
-            "site_name":       self.site_name,
-            "site_description": self.site_description,
-            "site_shorttag":   self.site_shorttag,
-            "small_footer":    self.small_footer,
-            "large_footer":    self.large_footer,
-            "path":            request.path,
-            "in_production":   self.in_production,
-            "maintenance_mode": self.maintenance_mode,
-            "sandbox_message": self.sandbox_message,
+            "base_url":            self.base_url,
+            "identity_provider":   self.identity_provider,
+            "in_production":       self.in_production,
+            "is_logged_in":        account is not None,
+            "large_footer":        self.large_footer,
+            "maintenance_mode":    self.maintenance_mode,
+            "menu":                self.menu,
+            "orcid_client_id":     self.orcid_client_id,
+            "orcid_endpoint":      self.orcid_endpoint,
+            "path":                request.path,
+            "sandbox_message":     self.sandbox_message,
             "sandbox_message_css": self.sandbox_message_css,
-            "identity_provider": self.identity_provider,
-            "orcid_client_id": self.orcid_client_id,
-            "orcid_endpoint":  self.orcid_endpoint,
-            "session_token":   self.token_from_request (request),
-            "is_logged_in":    account is not None,
-            "is_reviewing":    self.db.may_review (impersonator_token),
-            "may_review":      self.db.may_review (token, account),
-            "may_review_integrity": self.db.may_review_integrity (token, account),
-            "may_review_quotas": self.db.may_review_quotas (token, account),
-            "may_administer":  self.db.may_administer (token, account),
-            "may_query":       self.db.may_query (token, account),
-            "may_impersonate":  self.db.may_impersonate (token, account),
-            "impersonating_account": self.__impersonating_account (request),
-            "menu":            self.menu,
+            "site_description":    self.site_description,
+            "site_name":           self.site_name,
+            "site_shorttag":       self.site_shorttag,
+            "small_footer":        self.small_footer,
         }
+        if account is None:
+            parameters = { **parameters,
+                "session_token": None,
+                "impersonating_account": None,
+                "is_reviewing": None
+            }
+        else:
+            impersonator_token = self.__impersonator_token (request)
+            parameters = { **parameters,
+                "impersonating_account": self.__impersonating_account (request),
+                "is_reviewing":          self.db.may_review (impersonator_token),
+                "may_administer":        self.db.may_administer (token, account),
+                "may_impersonate":       self.db.may_impersonate (token, account),
+                "may_query":             self.db.may_query (token, account),
+                "may_review":            self.db.may_review (token, account),
+                "may_review_integrity":  self.db.may_review_integrity (token, account),
+                "may_review_quotas":     self.db.may_review_quotas (token, account),
+                "session_token":         self.token_from_request (request),
+            }
+
         return self.response (template.render({ **context, **parameters }),
                               mimetype='text/html')
 
     def __render_email_templates (self, template_name, **context):
         """Render a plaintext and an HTML body for sending in an e-mail."""
 
         html_template = self.jinja.get_template (f"{template_name}.html")
@@ -955,17 +967,17 @@
         record["published_since"] = self.get_parameter (request, "published_since")
         record["modified_since"]  = self.get_parameter (request, "modified_since")
         record["group"]           = self.get_parameter (request, "group")
         record["resource_doi"]    = self.get_parameter (request, "resource_doi")
         record["item_type"]       = self.get_parameter (request, "item_type")
         record["doi"]             = self.get_parameter (request, "doi")
         record["handle"]          = self.get_parameter (request, "handle")
-        record["search_for"]      = self.parse_search_terms(self.get_parameter (request, "search_for"))
+        record["search_for"]      = self.parse_search_terms (self.get_parameter (request, "search_for"))
         record["search_format"]   = self.get_parameter (request, "search_format")
-        record["categories"]      = split_delimited_string(self.get_parameter (request, "categories"), ",")
+        record["categories"]      = split_string (self.get_parameter (request, "categories"), delimiter=",")
         record["is_latest"]       = self.get_parameter (request, "is_latest")
 
         offset, limit = self.__paging_offset_and_limit (request)
         record["offset"] = offset
         record["limit"]  = limit
 
         validator.string_value  (record, "order", 0, 32)
@@ -1124,14 +1136,47 @@
 
         self.log.error ("Unknown report format '%s'.", report_format)
         return self.error_400 (request, "Unknown report format.", 400)
 
     ## AUTHENTICATION HANDLERS
     ## ------------------------------------------------------------------------
 
+    def obtain_orcid_read_public_token (self):
+        """Requests a read-public token from ORCID."""
+
+        url_parameters = {
+            "client_id":     self.orcid_client_id,
+            "client_secret": self.orcid_client_secret,
+            "grant_type":    "client_credentials",
+            "scope":         "/read-public"
+        }
+        headers = {
+            "Accept": "application/json",
+            "Content-Type": "application/x-www-form-urlencoded"
+        }
+        response = requests.post(f"{self.orcid_endpoint}/token",
+                                 params  = url_parameters,
+                                 headers = headers,
+                                 timeout = 10)
+
+        if response.status_code != 200:
+            self.log.error ("Failed to obtain read-public token from ORCID (%d).",
+                            response.status_code)
+            return False
+
+        record = response.json()
+        token = value_or_none (record, "access_token")
+        if token is not None:
+            self.orcid_read_public_token = token
+            return True
+
+        self.log.error ("Unexpected response for read-public token from ORCID.")
+        self.log.error ("Response was:\n---\n%s\n---", json.dumps(record))
+        return False
+
     def authenticate_using_orcid (self, request, redirect_path="/login"):
         """Returns a record upon success, None upon failure."""
 
         record = { "code": self.get_parameter (request, "code") }
         try:
             url_parameters = {
                 "client_id":     self.orcid_client_id,
@@ -1729,28 +1774,36 @@
 
         account_uuid, error_response = self.__depositor_account_uuid (request)
         if error_response is not None:
             return error_response
 
         account      = self.db.account_by_uuid (account_uuid)
         storage_used = self.db.account_storage_used (account_uuid)
+        pending_quota_requests = self.db.quota_requests (status       = "unresolved",
+                                                         account_uuid = account_uuid)
 
         account_quota   = 0
         percentage_used = 0
+        requested_quota = None
         try:
             account_quota   = account["quota"]
             percentage_used = round(storage_used / account_quota * 100, 2)
+
+            if pending_quota_requests:
+                requested_bytes = int(pending_quota_requests[0]["requested_size"])
+                requested_quota = pretty_print_size (requested_bytes)
         except (TypeError, KeyError):
             pass
 
         sessions     = self.db.sessions (account_uuid)
         return self.__render_template (
             request, "depositor/dashboard.html",
             storage_used = pretty_print_size (storage_used),
             quota        = pretty_print_size (account_quota),
+            requested_quota = requested_quota,
             percentage_used = percentage_used,
             sessions     = sessions)
 
     def __datasets_with_storage_usage (self, datasets):
         for dataset in datasets:
             used = 0
             if not value_or (dataset, "is_metadata_record", False):
@@ -3783,19 +3836,15 @@
     def ui_search (self, request):
         """Implements /search."""
         if not self.accepts_html (request):
             return self.error_406 ("text/html")
 
         search_for = self.get_parameter(request, "search")
         if search_for is None:
-            # 'q' is used by visitors from library.tudelft.nl. This can be
-            # removed once the library.tudelft.nl search has been updated.
-            search_for = self.get_parameter(request, "q")
-            if search_for is None:
-                search_for = ""
+            search_for = ""
 
         search_for = search_for.strip()
         categories = self.db.categories(limit=None)
         return self.__render_template (request, "search.html",
                                        search_for=search_for,
                                        categories=categories,
                                        page_title=f"{search_for} (search)")
@@ -4288,17 +4337,18 @@
                     is_metadata_record = validator.boolean_value (record, "is_metadata_record", when_none=False),
                     metadata_reason = validator.string_value  (record, "metadata_reason",  0, 512),
                     embargo_until_date = validator.date_value (record, "embargo_until_date",
                                                                is_temporary_embargo),
                     embargo_type    = validator.options_value (record, "embargo_type", validator.embargo_types),
                     embargo_title   = validator.string_value  (record, "embargo_title", 0, 1000),
                     embargo_reason  = validator.string_value  (record, "embargo_reason", 0, 10000),
-                    eula            = validator.string_value  (record, "eula", 0, 10000),
+                    eula            = validator.string_value  (record, "eula", 0, 50000),
                     defined_type_name = defined_type_name,
                     defined_type    = defined_type,
+                    git_repository_name = validator.string_value  (record, "git_repository_name",  0, 255),
                     agreed_to_deposit_agreement = validator.boolean_value (record, "agreed_to_deposit_agreement", False, False),
                     agreed_to_publish = validator.boolean_value (record, "agreed_to_publish", False, False),
                     categories      = validator.array_value   (record, "categories"),
                 )
                 if not result:
                     return self.error_500()
 
@@ -4418,18 +4468,16 @@
                         is_published = False,
                         limit        = 10000)
 
                     existing_authors = list(map (lambda item: URIRef(uuid_to_uri(item["uuid"], "author")),
                                                  existing_authors))
 
                 authors = existing_authors + new_authors
-                if not self.db.update_item_list (dataset["uuid"],
-                                                 account_uuid,
-                                                 authors,
-                                                 "authors"):
+                if not self.db.update_item_list (dataset["uuid"], account_uuid,
+                                                 authors, "authors"):
                     self.log.error ("Adding a single author failed.")
                     return self.error_500()
 
                 return self.respond_205()
 
             except KeyError:
                 return self.error_400 (request, "Expected an 'authors' field.", "NoAuthorsField")
@@ -4470,18 +4518,15 @@
 
             if parses_to_int (author_id):
                 authors.remove (next (filter (lambda item: item['id'] == author_id, authors)))
             else:
                 authors.remove (next (filter (lambda item: item['uuid'] == author_id, authors)))
 
             authors = list(map (lambda item: URIRef(uuid_to_uri(item["uuid"], "author")), authors))
-            if self.db.update_item_list (dataset["uuid"],
-                                         account_uuid,
-                                         authors,
-                                         "authors"):
+            if self.db.update_item_list (dataset["uuid"], account_uuid, authors, "authors"):
                 return self.respond_204()
 
             return self.error_500()
         except (IndexError, KeyError):
             return self.error_500 ()
 
     def __api_private_item_funding (self, request, item_id, item_type,
@@ -4567,18 +4612,16 @@
                         is_published = False,
                         limit        = 10000)
 
                     existing_fundings = list(map (lambda item: URIRef(uuid_to_uri(item["uuid"],"funding")),
                                                  existing_fundings))
 
                 fundings = existing_fundings + new_fundings
-                if not self.db.update_item_list (item["uuid"],
-                                                 account_uuid,
-                                                 fundings,
-                                                 "funding_list"):
+                if not self.db.update_item_list (item["uuid"], account_uuid,
+                                                 fundings, "funding_list"):
                     self.log.error ("Adding a single funder failed.")
                     return self.error_500()
 
                 return self.respond_205()
 
             except KeyError:
                 return self.error_400 (request, "Expected a 'funders' field.", "NoFundersField")
@@ -4628,18 +4671,16 @@
                                          is_published = False,
                                          item_type    = item_type,
                                          limit        = 10000)
 
             fundings.remove (next (filter (lambda item: item['uuid'] == funding_id, fundings)))
 
             fundings = list(map (lambda item: URIRef(uuid_to_uri(item["uuid"], "funding")), fundings))
-            if self.db.update_item_list (item["uuid"],
-                                         account_uuid,
-                                         fundings,
-                                         "funding_list"):
+            if self.db.update_item_list (item["uuid"], account_uuid,
+                                         fundings, "funding_list"):
                 return self.respond_204()
 
             return self.error_500()
         except (IndexError, KeyError):
             return self.error_500 ()
 
     def api_private_dataset_funding_delete (self, request, dataset_id, funding_id):
@@ -4681,18 +4722,16 @@
                 authors.remove (next (filter (lambda item: item['id'] == author_id, authors)))
             else:
                 authors.remove (next (filter (lambda item: item['uuid'] == author_id, authors)))
 
             authors = list(map(lambda item: URIRef(uuid_to_uri(item["uuid"], "author")),
                                 authors))
 
-            if self.db.update_item_list (collection["uuid"],
-                                         account_uuid,
-                                         authors,
-                                         "authors"):
+            if self.db.update_item_list (collection["uuid"], account_uuid,
+                                         authors, "authors"):
                 return self.respond_204()
 
             return self.error_500()
         except (IndexError, KeyError):
             return self.error_500 ()
 
     def api_private_collection_dataset_delete (self, request, collection_id, dataset_id):
@@ -4782,18 +4821,16 @@
 
                     existing_categories = list(map(lambda category: category["uuid"], existing_categories))
 
                     # Merge and remove duplicates
                     categories = list(dict.fromkeys(existing_categories + categories))
 
                 categories = uris_from_records (categories, "category")
-                if self.db.update_item_list (dataset["uuid"],
-                                             account_uuid,
-                                             categories,
-                                             "categories"):
+                if self.db.update_item_list (dataset["uuid"], account_uuid,
+                                             categories, "categories"):
                     return self.respond_205()
 
                 return self.error_500()
 
             except IndexError:
                 return self.error_500 ()
             except KeyError:
@@ -5113,18 +5150,16 @@
                     return self.error_500()
 
                 links    = self.db.private_links (item_uri   = dataset["uri"],
                                                   account_uuid = account_uuid)
                 links    = list(map (lambda item: URIRef(item["uri"]), links))
                 links    = links + [ URIRef(link_uri) ]
 
-                if not self.db.update_item_list (dataset["uuid"],
-                                                 account_uuid,
-                                                 links,
-                                                 "private_links"):
+                if not self.db.update_item_list (dataset["uuid"], account_uuid,
+                                                 links, "private_links"):
                     self.log.error ("Updating private links failed for %s.",
                                     dataset["container_uuid"])
 
                     return self.error_500()
 
                 return self.response(json.dumps({
                     "location": f"{self.base_url}/private_datasets/{id_string}"
@@ -5831,18 +5866,16 @@
                         is_published = False,
                         limit        = 10000)
 
                     existing_authors = list(map (lambda item: URIRef(uuid_to_uri(item["uuid"], "author")),
                                                  existing_authors))
 
                 authors = existing_authors + new_authors
-                if not self.db.update_item_list (collection["uuid"],
-                                                 account_uuid,
-                                                 authors,
-                                                 "authors"):
+                if not self.db.update_item_list (collection["uuid"], account_uuid,
+                                                 authors, "authors"):
                     self.log.error ("Adding a single author failed.")
                     return self.error_500()
 
                 return self.respond_205()
 
             except IndexError:
                 return self.error_500 ()
@@ -5957,18 +5990,16 @@
                                                            is_latest    = True,
                                                            is_published = True)
                     if dataset is None:
                         return self.error_500 ()
 
                     datasets[index] = URIRef(dataset["container_uri"])
 
-                if self.db.update_item_list (collection["uuid"],
-                                             account_uuid,
-                                             datasets,
-                                             "datasets"):
+                if self.db.update_item_list (collection["uuid"], account_uuid,
+                                             datasets, "datasets"):
                     self.db.cache.invalidate_by_prefix ("datasets")
                     return self.respond_205()
 
             except (IndexError, TypeError):
                 return self.error_500 ()
             except KeyError:
                 return self.error_400 (request, "Expected an array for 'articles'.", "NoArticlesField")
@@ -6076,21 +6107,21 @@
         record["offset"]          = self.get_parameter (request, "offset")
         record["order"]           = self.get_parameter (request, "order")
         record["order_direction"] = self.get_parameter (request, "order_direction")
         record["institution"]     = self.get_parameter (request, "institution")
         record["published_since"] = self.get_parameter (request, "published_since")
         record["modified_since"]  = self.get_parameter (request, "modified_since")
         record["group"]           = self.get_parameter (request, "group")
-        record["group_ids"]       = self.get_parameter (request, "group_ids")
+        record["group_ids"]       = split_string (self.get_parameter (request, "group_ids"), delimiter=",")
+        record["categories"]      = split_string (self.get_parameter (request, "categories"), delimiter=",")
         record["resource_doi"]    = self.get_parameter (request, "resource_doi")
         record["item_type"]       = self.get_parameter (request, "item_type")
         record["doi"]             = self.get_parameter (request, "doi")
         record["handle"]          = self.get_parameter (request, "handle")
         record["return_count"]    = self.get_parameter (request, "return_count")
-        record["categories"]      = self.get_parameter (request, "categories")
 
         try:
             validator.integer_value (record, "limit")
             validator.integer_value (record, "offset")
             validator.string_value  (record, "order",           maximum_length=32)
             validator.order_direction (record, "order_direction")
             validator.integer_value (record, "institution")
@@ -6100,21 +6131,19 @@
             validator.string_value  (record, "resource_doi",    maximum_length=255)
             validator.integer_value (record, "item_type")
             validator.string_value  (record, "doi",             maximum_length=255)
             validator.string_value  (record, "handle",          maximum_length=255)
             validator.boolean_value (record, "return_count")
 
             if record["categories"] is not None:
-                record["categories"] = record["categories"].split(",")
                 validator.array_value   (record, "categories")
                 for index, _ in enumerate(record["categories"]):
                     record["categories"][index] = validator.integer_value (record["categories"], index)
 
             if record["group_ids"] is not None:
-                record["group_ids"] = record["group_ids"].split(",")
                 validator.array_value   (record, "group_ids")
                 for index, _ in enumerate(record["group_ids"]):
                     record["group_ids"][index] = validator.integer_value (record["group_ids"], index)
 
         except validator.ValidationException as error:
             return self.error_400 (request, error.message, error.code)
 
@@ -6149,14 +6178,22 @@
             return self.error_404 (request)
 
         account_uuid = self.default_authenticated_error_handling (request, "GET",
                                                                   "application/json")
         if isinstance (account_uuid, Response):
             return account_uuid
 
+        order = validator.string_value (request.args, "order", 0, 32)
+        if order is None:
+            order = "order_index"
+
+        order_direction = validator.order_direction (request.args, "order_direction")
+        if order_direction is None:
+            order_direction = "asc"
+
         try:
             dataset = self.db.datasets (container_uuid = container_uuid,
                                         account_uuid   = account_uuid,
                                         is_published   = False,
                                         is_latest      = False,
                                         limit          = 1)[0]
 
@@ -6168,16 +6205,16 @@
             authors = self.db.authors (
                 item_uri     = dataset["uri"],
                 account_uuid = account_uuid,
                 author_uuid  = author_uuid,
                 is_published = False,
                 item_type    = "dataset",
                 limit        = validator.integer_value (request.args, "limit"),
-                order        = validator.string_value (request.args, "order", 0, 32),
-                order_direction = validator.order_direction (request.args, "order_direction"))
+                order        = order,
+                order_direction = order_direction)
 
             if author_uuid is not None:
                 return self.response (json.dumps(formatter.format_author_record_v3 (authors[0])))
 
             return self.default_list_response (authors, formatter.format_author_record_v3)
         except (IndexError, KeyError, TypeError) as error:
             self.log.error ("Unable to retrieve authors: %s", error)
@@ -6256,23 +6293,85 @@
                                                is_published = True,
                                                item_type = "dataset",
                                                limit = 10000)))
             return self.response (json.dumps(output))
         except validator.ValidationException as error:
             return self.error_400 (request, error.message, error.code)
 
+    def api_v3_datasets_search (self, request):
+        """Implements /v3/datasets/search."""
+        handler = self.default_error_handling (request, "POST", "application/json")
+        if handler is not None:
+            return handler
+
+        parameters = request.get_json()
+
+        try:
+            record = {}
+            record["order"]           = self.get_parameter (parameters, "order")
+            record["order_direction"] = self.get_parameter (parameters, "order_direction")
+            record["institution"]     = self.get_parameter (parameters, "institution")
+            record["published_since"] = self.get_parameter (parameters, "published_since")
+            record["modified_since"]  = self.get_parameter (parameters, "modified_since")
+            record["group"]           = self.get_parameter (parameters, "group")
+            record["resource_doi"]    = self.get_parameter (parameters, "resource_doi")
+            record["item_type"]       = self.get_parameter (parameters, "item_type")
+            record["doi"]             = self.get_parameter (parameters, "doi")
+            record["handle"]          = self.get_parameter (parameters, "handle")
+            record["search_for"]      = self.get_parameter (parameters, "search_for")
+            record["search_format"]   = self.get_parameter (parameters, "search_format")
+            record["search_scope"]    = self.get_parameter (parameters, "search_scope")
+            record["organizations"]   = self.get_parameter (parameters, "organizations")
+            record["categories"]      = split_string (self.get_parameter (parameters, "categories"), delimiter=",")
+            record["is_latest"]       = self.get_parameter (parameters, "is_latest")
+
+            offset, limit = self.__paging_offset_and_limit (parameters)
+            record["offset"] = offset
+            record["limit"]  = limit
+
+            validator.string_value   (record, "order", 0, 32)
+            validator.order_direction (record, "order_direction")
+            validator.integer_value  (record, "institution")
+            validator.string_value   (record, "published_since", maximum_length=32)
+            validator.string_value   (record, "modified_since",  maximum_length=32)
+            validator.integer_value  (record, "group")
+            validator.string_value   (record, "resource_doi",    maximum_length=255)
+            validator.integer_value  (record, "item_type")
+            validator.string_value   (record, "doi",             maximum_length=255)
+            validator.string_value   (record, "handle",          maximum_length=255)
+            validator.string_value   (record, "search_for",      maximum_length=1024)
+            validator.string_value   (record, "organizations",   maximum_length=255)
+            validator.boolean_value  (record, "is_latest")
+            validator.array_value    (record, "search_format")
+            validator.array_value    (record, "search_scope")
+
+            if "categories" in record and record["categories"] is not None:
+                for category_id in record["categories"]:
+                    validator.integer_value (record, "category_id", category_id)
+
+            # Rewrite the group parameter to match the database's plural form.
+            record["groups"]  = [record["group"]] if record["group"] is not None else None
+            del record["group"]
+
+            records = self.db.datasets (**record)
+            return self.default_list_response (records, formatter.format_dataset_record,
+                                               base_url = self.base_url)
+
+        except validator.ValidationException as error:
+            return self.error_400 (request, error.message, error.code)
+
     def __api_v3_datasets_parameters (self, request, item_type):
         record = {}
         record["dataset_id"]      = self.get_parameter (request, "id")
         record["limit"]           = self.get_parameter (request, "limit")
         record["offset"]          = self.get_parameter (request, "offset")
         record["order"]           = self.get_parameter (request, "order")
         record["order_direction"] = self.get_parameter (request, "order_direction")
-        record["group_ids"]       = self.get_parameter(request, "group_ids")
-        record["categories"]      = self.get_parameter (request, "categories")
+        record["group_ids"]       = split_string (self.get_parameter (request, "group_ids"), delimiter=",")
+        record["categories"]      = split_string (self.get_parameter (request, "categories"), delimiter=",")
         record["item_type"]       = item_type
 
         validator.integer_value (record, "dataset_id")
         validator.integer_value (record, "limit")
         validator.integer_value (record, "offset")
         validator.string_value  (record, "order", maximum_length=32)
         validator.order_direction (record, "order_direction")
@@ -6282,31 +6381,22 @@
             raise validator.InvalidValue(
                 field_name = "item_type",
                 message = ("The last URL parameter must be one of "
                            "'downloads', 'views', 'shares' or 'cites'."),
                 code    = "InvalidURLParameterValue")
 
         if record["categories"] is not None:
-            categories = record["categories"]
-            if categories == "":
-                categories = None
-            else:
-                categories = categories.split(",")
-                record["categories"] = categories
-                validator.array_value   (record, "categories")
-                for index, _ in enumerate(categories):
-                    category_id = validator.integer_value (categories, index)
-                    categories[index] = category_id
-                record["categories"] = categories
+            validator.array_value (record, "categories")
+            for index, _ in enumerate(record["categories"]):
+                record["categories"][index] = validator.integer_value (record["categories"], index)
 
         if record["group_ids"] is not None:
-            record["group_ids"] = record["group_ids"].split(",")
-            validator.array_value(record, "group_ids")
+            validator.array_value (record, "group_ids")
             for index, _ in enumerate(record["group_ids"]):
-                record["group_ids"][index] = validator.integer_value(record["group_ids"], index)
+                record["group_ids"][index] = validator.integer_value (record["group_ids"], index)
 
         return record
 
     def api_v3_datasets_top (self, request, item_type):
         """Implements /v3/datasets/top/<type>."""
         handler = self.default_error_handling (request, "GET", "application/json")
         if handler is not None:
@@ -6863,15 +6953,15 @@
                 "is_restricted":      is_restricted,
                 "is_metadata_record": validator.boolean_value (record, "is_metadata_record", when_none=False),
                 "metadata_reason":    validator.string_value  (record, "metadata_reason",  0, 512),
                 "embargo_until_date": validator.date_value    (record, "embargo_until_date", is_temporary_embargo, errors),
                 "embargo_type":       validator.options_value (record, "embargo_type", validator.embargo_types, is_temporary_embargo, errors),
                 "embargo_title":      validator.string_value  (record, "embargo_title", 0, 1000, is_embargoed, errors),
                 "embargo_reason":     validator.string_value  (record, "embargo_reason", 0, 10000, is_embargoed, errors),
-                "eula":               validator.string_value  (record, "eula", 0, 10000, is_restricted, errors),
+                "eula":               validator.string_value  (record, "eula", 0, 50000, is_restricted, errors),
                 "defined_type_name":  dataset_type,
                 "defined_type":       defined_type,
                 "agreed_to_deposit_agreement": agreed_to_deposit_agreement,
                 "agreed_to_publish":  agreed_to_publish,
                 "categories":         validator.array_value   (record, "categories", True, errors)
             }
 
@@ -6907,15 +6997,17 @@
                 # When in pre-production state, don't send e-mails to depositors.
                 if self.in_production and not self.in_preproduction and "email" in account:
                     self.__send_templated_email (
                         [account["email"]],
                         f"Submission of {dataset['title']}.",
                         "dataset_submitted",
                         dataset = dataset,
-                        account = account)
+                        account = account,
+                        support_email = self.support_email_address,
+                        site_name = self.site_name)
 
                 self.locks.unlock (locks.LockTypes.SUBMIT_DATASET)
                 return self.respond_204 ()
 
         except validator.ValidationException as error:
             self.locks.unlock (locks.LockTypes.SUBMIT_DATASET)
             return self.error_400 (request, error.message, error.code)
@@ -7359,18 +7451,16 @@
 
             references     = list(map(lambda reference: reference["url"], references))
 
             if request.method == 'DELETE':
                 url_encoded = validator.string_value (request.args, "url", 0, 1024, True)
                 url         = unquote(url_encoded)
                 references.remove (next (filter (lambda item: item == url, references)))
-                if not self.db.update_item_list (item["uuid"],
-                                                 account_uuid,
-                                                 references,
-                                                 "references"):
+                if not self.db.update_item_list (item["uuid"], account_uuid,
+                                                 references, "references"):
                     self.log.error ("Deleting a reference failed.")
                     return self.error_500()
 
                 return self.respond_204()
 
             ## For POST and PUT requests, the 'parameters' will be a dictionary
             ## containing a key "references", which can contain multiple
@@ -7463,18 +7553,15 @@
 
             tags     = list(map(lambda tag: tag["tag"], tags))
 
             if request.method == 'DELETE':
                 tag_encoded = validator.string_value (request.args, "tag", 0, 1024, True)
                 tag         = unquote(tag_encoded)
                 tags.remove (next (filter (lambda item: item == tag, tags)))
-                if not self.db.update_item_list (item["uuid"],
-                                                 account_uuid,
-                                                 tags,
-                                                 "tags"):
+                if not self.db.update_item_list (item["uuid"], account_uuid, tags, "tags"):
                     self.log.error ("Deleting a tag failed.")
                     return self.error_500()
 
                 return self.respond_204()
 
             ## For POST and PUT requests, the 'parameters' will be a dictionary
             ## containing a key "references", which can contain multiple
@@ -7492,18 +7579,15 @@
 
                 # Drop the index field.
                 existing_tags = list (map (lambda item: item["tag"], existing_tags))
 
                 # Remove duplicates.
                 tags = deduplicate_list(existing_tags + new_tags)
 
-            if not self.db.update_item_list (item["uuid"],
-                                             account_uuid,
-                                             tags,
-                                             "tags"):
+            if not self.db.update_item_list (item["uuid"], account_uuid, tags, "tags"):
                 self.log.error ("Updating tags failed.")
                 return self.error_500()
 
             return self.respond_205()
 
         except IndexError:
             return self.error_500 ()
@@ -7748,59 +7832,96 @@
                 self.__log_event (request, dataset["container_uuid"], "dataset", "gitDownload")
                 return self.__git_passthrough (request)
         except IndexError:
             pass
 
         return self.error_403 (request)
 
-    def __git_contributors (self, git_repository):
+    def __git_contributors (self, git_uuid, git_repository):
         """Returns a list of contributors including their commit statistics."""
         history = git_repository.walk (git_repository.head.target,
                                        pygit2.enums.SortMode.REVERSE)
+
+        cache_key = f"{git_uuid}_{git_repository.head.target}"
+        cache_prefix = "git_contributors"
+        cached_value = self.db.cache.cached_value (cache_prefix, cache_key)
+        if cached_value:
+            return cached_value
+
         commits = list(history)
         if not commits:
             return None
 
         # Accounting for the initial commit.
+        contributors = {}
         previous_commit = commits[0]
         stats = self.__git_files_by_type (previous_commit.tree)
         total_lines = 0
         for extension in stats:
             for entry in stats[extension]:
                 total_lines += value_or (entry, "lines", 0)
 
-        contributors = {
-            previous_commit.author.email: {
+        week = datetime.fromtimestamp(previous_commit.commit_time).isocalendar()
+        week = int(datetime.fromisocalendar(week[0], week[1], 1).timestamp())
+
+        contributors[previous_commit.author.email] = {
+            "total": 1,
+            "additions": total_lines,
+            "deletions": 0,
+            "weeks": { week: { "w": week, "a": total_lines, "d": 0, "c": 1 } },
+            "author": {
                 "name": previous_commit.author.name,
-                "email": previous_commit.author.email,
-                "commits": 1,
-                "additions": total_lines,
-                "deletions": 0
+                "email": previous_commit.author.email
             }
         }
 
         # Walk the repository's history.
         for commit in commits[1:]:
             stats = git_repository.diff(previous_commit, commit).stats
-            if commit.author.email in contributors:
-                record = contributors[commit.author.email]
-                record["commits"] += 1
+            week = datetime.fromtimestamp(commit.commit_time).isocalendar()
+            week = int(datetime.fromisocalendar(week[0], week[1], 1).timestamp())
+            if commit.author.email not in contributors:
+                contributors[commit.author.email] = {
+                    "total": 0,
+                    "additions": 0,
+                    "deletions": 0,
+                    "weeks": { week: { "w": week, "c": 0, "a": 0, "d": 0 } },
+                    "author": {
+                        "name": commit.author.name,
+                        "email": commit.author.email
+                    }
+                }
+            record = contributors[commit.author.email]
+            if "weeks" in record and week in record["weeks"]:
+                record["weeks"][week]["c"] += 1
+                record["weeks"][week]["a"] += stats.insertions
+                record["weeks"][week]["d"] += stats.deletions
+                record["total"] += 1
                 record["additions"] += stats.insertions
                 record["deletions"] += stats.deletions
             else:
-                contributors[commit.author.email] = {
-                    "name": commit.author.name,
-                    "email": commit.author.email,
-                    "commits": 1,
-                    "additions": stats.insertions,
-                    "deletions": stats.deletions
+                record["weeks"][week] = {
+                    "w": week,
+                    "c": 1,
+                    "a": stats.insertions,
+                    "d": stats.deletions
                 }
+                record["total"] += 1
+                record["additions"] += stats.insertions
+                record["deletions"] += stats.deletions
+
             previous_commit = commit
 
-        return list(contributors.values())
+        # Flatten the structure
+        contributors = list(contributors.values())
+        for contributor in contributors:
+            contributor["weeks"] = list(contributor["weeks"].values())
+
+        self.db.cache.cache_value (cache_prefix, cache_key, contributors)
+        return contributors
 
     def __git_files_by_type (self, tree, path="", output=None):
         """
         Returns a dictionary with the file extension as key and the list of
         file statistics as value for the git repository TREE.
         """
         if output is None:
@@ -7808,14 +7929,18 @@
 
         for entry in tree:
             # Walk the directory tree
             if isinstance (entry, pygit2.Tree):  # pylint: disable=no-member
                 self.__git_files_by_type (list(entry), f"{path}{entry.name}/", output)
                 continue
 
+            # Submodules are represented as commits.
+            if isinstance (entry, pygit2.Commit):  # pylint: disable=no-member
+                continue
+
             record = { "filename": f"{path}{entry.name}", "size": entry.size }
 
             # Skip over binary files and large files.
             if entry.is_binary or entry.size > 5000000:
                 extension = "binary" if entry.is_binary else "large-text-file"
                 if extension in output:
                     output[extension].append(record)
@@ -7872,14 +7997,20 @@
     def api_v3_dataset_git_languages (self, request, git_uuid):
         """Implements /v3/datasets/<id>/languages."""
 
         git_repository, branch = self.__git_statistics_error_handling (request, git_uuid)
         if isinstance (git_repository, Response):
             return git_repository
 
+        cache_key = f"{git_uuid}_{git_repository.head.target}"
+        cache_prefix = "git_languages"
+        cached_value = self.db.cache.cached_value (cache_prefix, cache_key)
+        if cached_value:
+            return self.response (cached_value)
+
         tree = git_repository.revparse_single(branch).tree # pylint: disable=no-member
         statistics = self.__git_files_by_type (tree)
 
         # Drop the binary count from the statistics, because we only
         # generate a summary with line counts below.
         statistics.pop("binary", None)
 
@@ -7896,24 +8027,25 @@
                     num_bytes_for_extension += num_bytes
 
             summary[extension] = num_bytes_for_extension
 
         sorted_summary = dict(sorted(summary.items(),
                                      key=lambda item: item[1],
                                      reverse=True))
+        self.db.cache.cache_value (cache_prefix, cache_key, json.dumps (sorted_summary))
         return self.response (json.dumps (sorted_summary))
 
     def api_v3_dataset_git_contributors (self, request, git_uuid):
         """Implements /v3/datasets/<id>/contributors."""
 
         git_repository, _ = self.__git_statistics_error_handling (request, git_uuid)
         if isinstance (git_repository, Response):
             return git_repository
 
-        contributors = self.__git_contributors (git_repository)
+        contributors = self.__git_contributors (git_uuid, git_repository)
         if contributors is None:
             return self.error_404 (request)
 
         return self.response (json.dumps(contributors))
 
     def api_v3_profile (self, request):
         """Implements /v3/profile."""
```

### Comparing `djehuty-24.4/src/djehuty/web/xml_formatter.py` & `djehuty-24.5/src/djehuty/web/xml_formatter.py`

 * *Files identical despite different names*

### Comparing `djehuty-24.4/src/djehuty.egg-info/PKG-INFO` & `djehuty-24.5/src/djehuty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djehuty
-Version: 24.4
+Version: 24.5
 Summary: The 4TU.ResearchData repository system
 Author-email: Roel Janssen <r.r.e.janssen@tudelft.nl>
 Project-URL: Homepage, https://data.4tu.nl
 Project-URL: Source Code, https://github.com/4TUResearchData/djehuty
 Project-URL: Bug Tracker, https://github.com/4TUResearchData/djehuty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `djehuty-24.4/src/djehuty.egg-info/SOURCES.txt` & `djehuty-24.5/src/djehuty.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -193,14 +193,15 @@
 src/djehuty/web/resources/sparql_templates/references.sparql
 src/djehuty/web/resources/sparql_templates/reviews.sparql
 src/djehuty/web/resources/sparql_templates/root_categories.sparql
 src/djehuty/web/resources/sparql_templates/search_tags.sparql
 src/djehuty/web/resources/sparql_templates/statistics.sparql
 src/djehuty/web/resources/sparql_templates/statistics_authors.sparql
 src/djehuty/web/resources/sparql_templates/statistics_collections.sparql
+src/djehuty/web/resources/sparql_templates/statistics_datalink.sparql
 src/djehuty/web/resources/sparql_templates/statistics_datasets.sparql
 src/djehuty/web/resources/sparql_templates/statistics_files.sparql
 src/djehuty/web/resources/sparql_templates/subcategories_by_category.sparql
 src/djehuty/web/resources/sparql_templates/tags.sparql
 src/djehuty/web/resources/sparql_templates/update_account.sparql
 src/djehuty/web/resources/sparql_templates/update_author.sparql
 src/djehuty/web/resources/sparql_templates/update_collection.sparql
```

