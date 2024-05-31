# Comparing `tmp/imio.news.core-1.2.8.tar.gz` & `tmp/imio_news_core-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.news.core-1.2.8.tar", last modified: Thu May  2 10:47:53 2024, max compression
+gzip compressed data, was "imio_news_core-1.2.9.tar", last modified: Mon May 27 08:39:33 2024, max compression
```

## Comparing `imio.news.core-1.2.8.tar` & `imio_news_core-1.2.9.tar`

### file list

```diff
@@ -1,152 +1,163 @@
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/
--rw-r--r--   0 laurent    (501) staff       (20)     3564 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/CHANGES.rst
--rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/CONTRIBUTORS.rst
--rw-r--r--   0 laurent    (501) staff       (20)      522 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/DEVELOP.rst
--rw-r--r--   0 laurent    (501) staff       (20)    18092 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/LICENSE.GPL
--rw-r--r--   0 laurent    (501) staff       (20)      665 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/LICENSE.rst
--rw-r--r--   0 laurent    (501) staff       (20)      106 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/MANIFEST.in
--rw-r--r--   0 laurent    (501) staff       (20)     6862 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     2209 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/README.rst
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/docs/
--rw-r--r--   0 laurent    (501) staff       (20)     7986 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/docs/conf.py
--rw-r--r--   0 laurent    (501) staff       (20)       65 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/docs/index.rst
--rw-r--r--   0 laurent    (501) staff       (20)       64 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/requirements.txt
--rw-r--r--   0 laurent    (501) staff       (20)      518 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/setup.cfg
--rw-r--r--   0 laurent    (501) staff       (20)     2328 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/setup.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/
--rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/
--rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/
--rw-r--r--   0 laurent    (501) staff       (20)      259 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/browser/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      392 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     3557 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py
--rw-r--r--   0 laurent    (501) staff       (20)      595 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/browser/overrides/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/overrides/.gitkeep
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/browser/static/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/static/.gitkeep
--rw-r--r--   0 laurent    (501) staff       (20)      791 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/
--rw-r--r--   0 laurent    (501) staff       (20)      226 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/entity/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/entity/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)       70 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/entity/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1742 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/entity/content.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/folder/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/folder/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)       70 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/folder/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      314 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/folder/content.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)       70 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1236 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/content.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      690 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     5073 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     5483 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/serializer.py
--rw-r--r--   0 laurent    (501) staff       (20)     5608 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     2415 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/views.py
--rw-r--r--   0 laurent    (501) staff       (20)      487 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/converters.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/faceted/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/faceted/config/
--rw-r--r--   0 laurent    (501) staff       (20)     6592 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/faceted/config/news.xml
--rw-r--r--   0 laurent    (501) staff       (20)     4199 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/indexers.py
--rw-r--r--   0 laurent    (501) staff       (20)     1543 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/indexers.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      199 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/interfaces.py
--rw-r--r--   0 laurent    (501) staff       (20)      347 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/overrides.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      762 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/permissions.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/
--rw-r--r--   0 laurent    (501) staff       (20)      167 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/browserlayer.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2007 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/catalog.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2843 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/contentrules.xml
--rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/diff_tool.xml
--rw-r--r--   0 laurent    (501) staff       (20)      449 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/metadata.xml
--rw-r--r--   0 laurent    (501) staff       (20)      743 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/registry.xml
--rw-r--r--   0 laurent    (501) staff       (20)      252 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/repositorytool.xml
--rw-r--r--   0 laurent    (501) staff       (20)      980 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/rolemap.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/
--rw-r--r--   0 laurent    (501) staff       (20)      295 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1613 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.Entity.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1372 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.Folder.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1432 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1554 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml
--rw-r--r--   0 laurent    (501) staff       (20)      361 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/uninstall/
--rw-r--r--   0 laurent    (501) staff       (20)      124 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 laurent    (501) staff       (20)      876 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/serializer/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/serializer/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      175 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/serializer/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      579 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/serializer/newsitem.py
--rw-r--r--   0 laurent    (501) staff       (20)      663 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/setuphandlers.py
--rw-r--r--   0 laurent    (501) staff       (20)     6032 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/subscribers.py
--rw-r--r--   0 laurent    (501) staff       (20)     1342 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/subscribers.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1805 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/testing.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/tests/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/tests/resources/
--rw-r--r--   0 laurent    (501) staff       (20)    24753 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/resources/plone.png
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/tests/robot/
--rw-r--r--   0 laurent    (501) staff       (20)     1987 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/robot/test_example.robot
--rw-r--r--   0 laurent    (501) staff       (20)     2801 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_bring_news_into_news_folders.py
--rw-r--r--   0 laurent    (501) staff       (20)     1598 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_cropping.py
--rw-r--r--   0 laurent    (501) staff       (20)     3380 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_entity.py
--rw-r--r--   0 laurent    (501) staff       (20)     3550 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_indexer.py
--rw-r--r--   0 laurent    (501) staff       (20)     2222 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_local_roles.py
--rw-r--r--   0 laurent    (501) staff       (20)     8040 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_multilingual.py
--rw-r--r--   0 laurent    (501) staff       (20)     9084 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_newsfolder.py
--rw-r--r--   0 laurent    (501) staff       (20)    14324 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_newsitem.py
--rw-r--r--   0 laurent    (501) staff       (20)      929 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_robot.py
--rw-r--r--   0 laurent    (501) staff       (20)     1950 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_setup.py
--rw-r--r--   0 laurent    (501) staff       (20)     3490 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_utils.py
--rw-r--r--   0 laurent    (501) staff       (20)     5134 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_vocabularies.py
--rw-r--r--   0 laurent    (501) staff       (20)      273 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/utils.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     5055 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1003_to_1004/
--rw-r--r--   0 laurent    (501) staff       (20)     1066 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/
--rw-r--r--   0 laurent    (501) staff       (20)     2843 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml
--rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/diff_tool.xml
--rw-r--r--   0 laurent    (501) staff       (20)      252 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/repositorytool.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/types/
--rw-r--r--   0 laurent    (501) staff       (20)      282 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/types/imio.news.NewsItem.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1007_to_1008/
--rw-r--r--   0 laurent    (501) staff       (20)      743 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/
--rw-r--r--   0 laurent    (501) staff       (20)      305 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Entity.xml
--rw-r--r--   0 laurent    (501) staff       (20)      305 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Folder.xml
--rw-r--r--   0 laurent    (501) staff       (20)      309 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsFolder.xml
--rw-r--r--   0 laurent    (501) staff       (20)      307 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsItem.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1009_to_1010/
--rw-r--r--   0 laurent    (501) staff       (20)      218 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1009_to_1010/rolemap.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2185 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/upgrades.py
--rw-r--r--   0 laurent    (501) staff       (20)     1660 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/utils.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      519 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/news/
--rw-r--r--   0 laurent    (501) staff       (20)      357 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/news/button_to_bring_news.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1069 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/news.py
--rw-r--r--   0 laurent    (501) staff       (20)     4363 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/vocabularies.py
--rw-r--r--   0 laurent    (501) staff       (20)     1003 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/vocabularies.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/
--rw-r--r--   0 laurent    (501) staff       (20)     6862 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     4992 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/SOURCES.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/dependency_links.txt
--rw-r--r--   0 laurent    (501) staff       (20)       15 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/namespace_packages.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/not-zip-safe
--rw-r--r--   0 laurent    (501) staff       (20)      278 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/requires.txt
--rw-r--r--   0 laurent    (501) staff       (20)        5 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/top_level.txt
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.345597 imio_news_core-1.2.9/
+-rw-r--r--   0 laurent    (501) staff       (20)     3869 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/CHANGES.rst
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/CONTRIBUTORS.rst
+-rw-r--r--   0 laurent    (501) staff       (20)      522 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/DEVELOP.rst
+-rw-r--r--   0 laurent    (501) staff       (20)    18092 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/LICENSE.GPL
+-rw-r--r--   0 laurent    (501) staff       (20)      665 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/LICENSE.rst
+-rw-r--r--   0 laurent    (501) staff       (20)      106 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/MANIFEST.in
+-rw-r--r--   0 laurent    (501) staff       (20)     7808 2024-05-27 08:39:33.345521 imio_news_core-1.2.9/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     2209 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/README.rst
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.330502 imio_news_core-1.2.9/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     7986 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/docs/conf.py
+-rw-r--r--   0 laurent    (501) staff       (20)       65 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/docs/index.rst
+-rw-r--r--   0 laurent    (501) staff       (20)       64 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/requirements.txt
+-rw-r--r--   0 laurent    (501) staff       (20)      518 2024-05-27 08:39:33.345852 imio_news_core-1.2.9/setup.cfg
+-rw-r--r--   0 laurent    (501) staff       (20)     2403 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.325069 imio_news_core-1.2.9/src/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.330623 imio_news_core-1.2.9/src/imio/
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.331505 imio_news_core-1.2.9/src/imio/news/
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.333717 imio_news_core-1.2.9/src/imio/news/core/
+-rw-r--r--   0 laurent    (501) staff       (20)      168 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.333902 imio_news_core-1.2.9/src/imio/news/core/browser/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/browser/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.334194 imio_news_core-1.2.9/src/imio/news/core/browser/bring_news_into_news_folders/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/browser/bring_news_into_news_folders/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      392 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/browser/bring_news_into_news_folders/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     3557 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py
+-rw-r--r--   0 laurent    (501) staff       (20)      595 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/browser/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.334306 imio_news_core-1.2.9/src/imio/news/core/browser/overrides/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/browser/overrides/.gitkeep
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.334391 imio_news_core-1.2.9/src/imio/news/core/browser/static/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/browser/static/.gitkeep
+-rw-r--r--   0 laurent    (501) staff       (20)      892 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.334592 imio_news_core-1.2.9/src/imio/news/core/contents/
+-rw-r--r--   0 laurent    (501) staff       (20)      226 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.334878 imio_news_core-1.2.9/src/imio/news/core/contents/entity/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/entity/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)       70 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/entity/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     2486 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/entity/content.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.335172 imio_news_core-1.2.9/src/imio/news/core/contents/folder/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/folder/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)       70 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/folder/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      314 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/folder/content.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.335496 imio_news_core-1.2.9/src/imio/news/core/contents/newsfolder/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/newsfolder/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)       70 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/newsfolder/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     1236 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/newsfolder/content.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.336162 imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      690 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     5073 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/content.py
+-rw-r--r--   0 laurent    (501) staff       (20)     6097 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/serializer.py
+-rw-r--r--   0 laurent    (501) staff       (20)     5608 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/view.pt
+-rw-r--r--   0 laurent    (501) staff       (20)     2415 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/views.py
+-rw-r--r--   0 laurent    (501) staff       (20)      552 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/converters.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.325844 imio_news_core-1.2.9/src/imio/news/core/faceted/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.336278 imio_news_core-1.2.9/src/imio/news/core/faceted/config/
+-rw-r--r--   0 laurent    (501) staff       (20)     6592 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/faceted/config/news.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     5219 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/indexers.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2122 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/indexers.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      199 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/interfaces.py
+-rw-r--r--   0 laurent    (501) staff       (20)      347 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/overrides.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      762 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/permissions.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.326076 imio_news_core-1.2.9/src/imio/news/core/profiles/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.337266 imio_news_core-1.2.9/src/imio/news/core/profiles/default/
+-rw-r--r--   0 laurent    (501) staff       (20)      167 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/browserlayer.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     2379 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/catalog.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     2843 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/contentrules.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/diff_tool.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      592 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/metadata.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1676 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/registry.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      252 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/repositorytool.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      980 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/rolemap.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.337803 imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      295 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1613 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/imio.news.Entity.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1372 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/imio.news.Folder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1432 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1554 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      361 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/default/types.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.337909 imio_news_core-1.2.9/src/imio/news/core/profiles/uninstall/
+-rw-r--r--   0 laurent    (501) staff       (20)      124 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      876 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/profiles.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.338458 imio_news_core-1.2.9/src/imio/news/core/rest/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/rest/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      679 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/rest/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     6767 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/rest/odwb_endpoint.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.338843 imio_news_core-1.2.9/src/imio/news/core/serializer/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/serializer/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      175 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/serializer/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      579 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/serializer/newsitem.py
+-rw-r--r--   0 laurent    (501) staff       (20)      663 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/setuphandlers.py
+-rw-r--r--   0 laurent    (501) staff       (20)     7170 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/subscribers.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1723 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/subscribers.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     1805 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/testing.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.340489 imio_news_core-1.2.9/src/imio/news/core/tests/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.340597 imio_news_core-1.2.9/src/imio/news/core/tests/resources/
+-rw-r--r--   0 laurent    (501) staff       (20)    24753 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/resources/plone.png
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.340743 imio_news_core-1.2.9/src/imio/news/core/tests/robot/
+-rw-r--r--   0 laurent    (501) staff       (20)     1987 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/robot/test_example.robot
+-rw-r--r--   0 laurent    (501) staff       (20)     2801 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_bring_news_into_news_folders.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1598 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_cropping.py
+-rw-r--r--   0 laurent    (501) staff       (20)     3380 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_entity.py
+-rw-r--r--   0 laurent    (501) staff       (20)     9140 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_indexes.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2222 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_local_roles.py
+-rw-r--r--   0 laurent    (501) staff       (20)     8040 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_multilingual.py
+-rw-r--r--   0 laurent    (501) staff       (20)     9084 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_newsfolder.py
+-rw-r--r--   0 laurent    (501) staff       (20)    11044 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_newsitem.py
+-rw-r--r--   0 laurent    (501) staff       (20)     5204 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_odwb.py
+-rw-r--r--   0 laurent    (501) staff       (20)      929 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_robot.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1950 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_setup.py
+-rw-r--r--   0 laurent    (501) staff       (20)     3490 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_utils.py
+-rw-r--r--   0 laurent    (501) staff       (20)     5313 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/test_vocabularies.py
+-rw-r--r--   0 laurent    (501) staff       (20)      273 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/tests/utils.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.341059 imio_news_core-1.2.9/src/imio/news/core/upgrades/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)     7437 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.327234 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.341172 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1003_to_1004/
+-rw-r--r--   0 laurent    (501) staff       (20)     1066 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.341532 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1006_to_1007/
+-rw-r--r--   0 laurent    (501) staff       (20)     2843 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1006_to_1007/diff_tool.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      252 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1006_to_1007/repositorytool.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.342320 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1006_to_1007/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      282 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1006_to_1007/types/imio.news.NewsItem.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.342754 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1007_to_1008/
+-rw-r--r--   0 laurent    (501) staff       (20)      743 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.326938 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1008_to_1009/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.343671 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1008_to_1009/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      305 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Entity.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      305 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Folder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      309 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsFolder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      307 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsItem.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.343785 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1009_to_1010/
+-rw-r--r--   0 laurent    (501) staff       (20)      218 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1009_to_1010/rolemap.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.344023 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1011_to_1012/
+-rw-r--r--   0 laurent    (501) staff       (20)     1065 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1011_to_1012/registry.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.344226 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1012_to_1013/
+-rw-r--r--   0 laurent    (501) staff       (20)      329 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1012_to_1013/catalog.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.344371 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1013_to_1014/
+-rw-r--r--   0 laurent    (501) staff       (20)      174 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1013_to_1014/catalog.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     2747 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/upgrades/upgrades.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1660 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/utils.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.344682 imio_news_core-1.2.9/src/imio/news/core/viewlets/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/viewlets/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      519 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/viewlets/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.344790 imio_news_core-1.2.9/src/imio/news/core/viewlets/news/
+-rw-r--r--   0 laurent    (501) staff       (20)      357 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/viewlets/news/button_to_bring_news.pt
+-rw-r--r--   0 laurent    (501) staff       (20)     1069 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/viewlets/news.py
+-rw-r--r--   0 laurent    (501) staff       (20)     4419 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/vocabularies.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1003 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio/news/core/vocabularies.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-27 08:39:33.344981 imio_news_core-1.2.9/src/imio.news.core.egg-info/
+-rw-r--r--   0 laurent    (501) staff       (20)     7808 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio.news.core.egg-info/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     5333 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio.news.core.egg-info/SOURCES.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio.news.core.egg-info/dependency_links.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       15 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio.news.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio.news.core.egg-info/not-zip-safe
+-rw-r--r--   0 laurent    (501) staff       (20)      331 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio.news.core.egg-info/requires.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        5 2024-05-27 08:39:33.000000 imio_news_core-1.2.9/src/imio.news.core.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imio.news.core-1.2.8/CHANGES.rst` & `imio_news_core-1.2.9/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 Changelog
 =========
 
 
+1.2.9 (2024-05-27)
+------------------
+
+- WEB-4101 : Add index for local category search
+  [laulaz]
+
+- Fix bad permission name
+  [laulaz]
+
+- WEB-4088 : Cover use case for sending data in odwb for a staging environment
+  [boulch]
+
+- WEB-4088 : Add some odwb endpoints (for news , for entities)
+  [boulch]
+
+
 1.2.8 (2024-05-02)
 ------------------
 
 - WEB-4101 : Use local category (if any) instead of category in `category_title` indexer
   [laulaz]
```

### Comparing `imio.news.core-1.2.8/DEVELOP.rst` & `imio_news_core-1.2.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/LICENSE.GPL` & `imio_news_core-1.2.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/LICENSE.rst` & `imio_news_core-1.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/PKG-INFO` & `imio_news_core-1.2.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 Metadata-Version: 2.1
 Name: imio.news.core
-Version: 1.2.8
+Version: 1.2.9
 Summary: Core product for iMio news website
 Home-page: https://github.com/collective/imio.news.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.news.core
 Project-URL: Source, https://github.com/imio/imio.news.core
 Project-URL: Tracker, https://github.com/imio/imio.news.core/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: embeddify
+Requires-Dist: z3c.jbot
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.gallery
+Requires-Dist: plone.restapi
+Requires-Dist: plone.app.dexterity
+Requires-Dist: plone.app.imagecropping
+Requires-Dist: collective.taxonomy
+Requires-Dist: collective.z3cform.datagridfield
+Requires-Dist: eea.facetednavigation
+Requires-Dist: embeddify
+Requires-Dist: imio.smartweb.common
+Requires-Dist: imio.smartweb.locales
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: mock; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 
 .. image:: https://github.com/IMIO/imio.news.core/workflows/Tests/badge.svg
@@ -129,14 +146,30 @@
 - Christophe Boulanger, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2024-05-27)
+------------------
+
+- WEB-4101 : Add index for local category search
+  [laulaz]
+
+- Fix bad permission name
+  [laulaz]
+
+- WEB-4088 : Cover use case for sending data in odwb for a staging environment
+  [boulch]
+
+- WEB-4088 : Add some odwb endpoints (for news , for entities)
+  [boulch]
+
+
 1.2.8 (2024-05-02)
 ------------------
 
 - WEB-4101 : Use local category (if any) instead of category in `category_title` indexer
   [laulaz]
 
 
@@ -313,9 +346,7 @@
 
 
 1.0a1 (2022-01-25)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.news.core-1.2.8/README.rst` & `imio_news_core-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/docs/conf.py` & `imio_news_core-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/setup.cfg` & `imio_news_core-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/setup.py` & `imio_news_core-1.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.news.core",
-    version="1.2.8",
+    version="1.2.9",
     description="Core product for iMio news website",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -52,14 +52,16 @@
         "embeddify",
         "z3c.jbot",
         "plone.api>=1.8.4",
         "plone.gallery",
         "plone.restapi",
         "plone.app.dexterity",
         "plone.app.imagecropping",
+        "collective.taxonomy",
+        "collective.z3cform.datagridfield",
         "eea.facetednavigation",
         "embeddify",
         "imio.smartweb.common",
         "imio.smartweb.locales",
     ],
     extras_require={
         "test": [
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py` & `imio_news_core-1.2.9/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/browser/configure.zcml` & `imio_news_core-1.2.9/src/imio/news/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/content.py` & `imio_news_core-1.2.9/src/imio/news/core/contents/newsfolder/content.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/configure.zcml` & `imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/content.py` & `imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/content.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/serializer.py` & `imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/serializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from plone.restapi.serializer.converters import json_compatible
 from plone.restapi.serializer.dxcontent import SerializeFolderToJson
 from plone.restapi.serializer.summary import DefaultJSONSummarySerializer
 from Products.CMFCore.WorkflowCore import WorkflowException
 from zope.component import adapter
+from zope.component import getUtility
 from zope.interface import implementer
 from zope.interface import Interface
+from zope.schema.interfaces import IVocabularyFactory
 
 
 def get_container_uid(event_uid, summary=None):
     if summary is not None:
         container_uid = summary.get("UID") or summary.get("container_uid")
         if container_uid:
             return container_uid
@@ -41,14 +43,24 @@
         text = result["text"]
         desc = result["description"]
 
         if lang and lang != "fr":
             result["title"] = result[f"title_{lang}"]
             result["description"] = result[f"description_{lang}"]
             result["text"] = result[f"text_{lang}"]
+            if self.context.local_category:
+                factory = getUtility(
+                    IVocabularyFactory, "imio.news.vocabulary.NewsLocalCategories"
+                )
+                vocabulary = factory(self.context, lang=lang)
+                term = vocabulary.getTerm(self.context.local_category)
+                result["local_category"] = {
+                    "token": self.context.local_category,
+                    "title": term.title,
+                }
 
         # Getting news folder title/id to use it in rest views
         if query.get("metadata_fields") is not None and "container_uid" in query.get(
             "metadata_fields"
         ):
             newsfolder = None
             news_uid = self.context.UID()
@@ -104,18 +116,18 @@
             summary["usefull_container_title"] = news_folder.title
         lang = get_restapi_query_lang(query)
         if lang == "fr":
             # nothing to go, fr is the default language
             return summary
 
         obj = IContentListingObject(self.context)
-        for orig_field in ["title", "description"]:
+        for orig_field in ["title", "description", "category_title", "local_category"]:
             field = f"{orig_field}_{lang}"
             accessor = self.field_accessors.get(field, field)
-            value = getattr(obj, accessor, None)
+            value = getattr(obj, accessor, None) or None
             try:
                 if callable(value):
                     value = value()
             except WorkflowException:
                 summary[orig_field] = None
                 continue
             if orig_field == "description" and value is not None:
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/view.pt` & `imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/view.pt`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/views.py` & `imio_news_core-1.2.9/src/imio/news/core/contents/newsitem/views.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/faceted/config/news.xml` & `imio_news_core-1.2.9/src/imio/news/core/faceted/config/news.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/indexers.py` & `imio_news_core-1.2.9/src/imio/news/core/indexers.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from imio.smartweb.common.utils import translate_vocabulary_term
 from plone import api
 from plone.app.contenttypes.behaviors.richtext import IRichText
 from plone.app.contenttypes.indexers import _unicode_save_string_concat
 from plone.app.textfield.value import IRichTextValue
 from plone.indexer import indexer
 from Products.CMFPlone.utils import safe_unicode
+from zope.component import getUtility
+from zope.schema.interfaces import IVocabularyFactory
 
 import copy
 
 
 @indexer(INewsItem)
 def translated_in_nl(obj):
     return bool(obj.title_nl)
@@ -24,22 +26,64 @@
 
 
 @indexer(INewsItem)
 def translated_in_en(obj):
     return bool(obj.title_en)
 
 
-@indexer(INewsItem)
-def category_title(obj):
-    if obj.local_category is not None:
-        return obj.local_category
+def get_category_title(obj, lang):
     if obj.category is not None:
         return translate_vocabulary_term(
-            "imio.news.vocabulary.NewsCategories", obj.category
+            "imio.news.vocabulary.NewsCategories", obj.category, lang
         )
+    raise AttributeError
+
+
+@indexer(INewsItem)
+def category_title_fr(obj):
+    return get_category_title(obj, "fr")
+
+
+@indexer(INewsItem)
+def category_title_nl(obj):
+    return get_category_title(obj, "nl")
+
+
+@indexer(INewsItem)
+def category_title_de(obj):
+    return get_category_title(obj, "de")
+
+
+@indexer(INewsItem)
+def category_title_en(obj):
+    return get_category_title(obj, "en")
+
+
+def get_local_category(obj, lang):
+    if not obj.local_category:
+        raise AttributeError
+    factory = getUtility(IVocabularyFactory, "imio.news.vocabulary.NewsLocalCategories")
+    vocabulary = factory(obj, lang=lang)
+    term = vocabulary.getTerm(obj.local_category)
+    return term.title
+
+
+@indexer(INewsItem)
+def local_category_nl(obj):
+    return get_local_category(obj, "nl")
+
+
+@indexer(INewsItem)
+def local_category_de(obj):
+    return get_local_category(obj, "de")
+
+
+@indexer(INewsItem)
+def local_category_en(obj):
+    return get_local_category(obj, "en")
 
 
 @indexer(INewsItem)
 def title_nl(obj):
     if not obj.title_nl:
         raise AttributeError
     return obj.title_nl
@@ -119,20 +163,20 @@
                 .getData()
                 .strip()
             )
         return text
 
     topics = []
     for topic in getattr(obj.aq_base, "topics", []) or []:
-        topics.append(
-            translate_vocabulary_term("imio.smartweb.vocabulary.Topics", topic)
-        )
+        term = translate_vocabulary_term("imio.smartweb.vocabulary.Topics", topic, lang)
+        topics.append(term)
 
-    category = translate_vocabulary_term(
-        "imio.news.vocabulary.NewsCategories", getattr(obj.aq_base, "category", None)
+    category = getattr(obj.aq_base, "category", None)
+    category_term = translate_vocabulary_term(
+        "imio.news.vocabulary.NewsCategories", category, lang
     )
     subjects = obj.Subject()
     title_field_name = "title"
     description_field_name = "description"
     if lang != "fr":
         title_field_name = f"{title_field_name}_{lang}"
         description_field_name = f"{description_field_name}_{lang}"
@@ -140,15 +184,15 @@
     result = " ".join(
         (
             safe_unicode(getattr(obj, title_field_name)) or "",
             safe_unicode(getattr(obj, description_field_name)) or "",
             safe_unicode(get_text(lang)) or "",
             *topics,
             *subjects,
-            safe_unicode(category),
+            safe_unicode(category_term),
         )
     )
     return _unicode_save_string_concat(result)
 
 
 @indexer(INewsItem)
 def SearchableText_fr_news(obj):
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/indexers.zcml` & `imio_news_core-1.2.9/src/imio/news/core/indexers.zcml`

 * *Files 14% similar despite different names*

```diff
@@ -43,16 +43,46 @@
 
   <adapter
       name="description_en"
       factory=".indexers.description_en"
       />
 
   <adapter
+      name="local_category_nl"
+      factory=".indexers.local_category_nl"
+      />
+
+  <adapter
+      name="local_category_de"
+      factory=".indexers.local_category_de"
+      />
+
+  <adapter
+      name="local_category_en"
+      factory=".indexers.local_category_en"
+      />
+
+  <adapter
       name="category_title"
-      factory=".indexers.category_title"
+      factory=".indexers.category_title_fr"
+      />
+
+  <adapter
+      name="category_title_nl"
+      factory=".indexers.category_title_nl"
+      />
+
+  <adapter
+      name="category_title_de"
+      factory=".indexers.category_title_de"
+      />
+
+  <adapter
+      name="category_title_en"
+      factory=".indexers.category_title_en"
       />
 
   <adapter
       name="category_and_topics"
       factory=".indexers.category_and_topics_indexer"
       />
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/permissions.zcml` & `imio_news_core-1.2.9/src/imio/news/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles/default/catalog.xml` & `imio_news_core-1.2.9/src/imio/news/core/profiles/default/catalog.xml`

 * *Files 6% similar despite different names*

#### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles/default/catalog.xml` & `imio_news_core-1.2.9/src/imio/news/core/profiles/default/catalog.xml`

```diff
@@ -2,14 +2,17 @@
 <object name="portal_catalog">
   <index name="category" meta_type="KeywordIndex">
     <indexed_attr value="category"/>
   </index>
   <index name="category_title" meta_type="FieldIndex">
     <indexed_attr value="category_title"/>
   </index>
+  <index name="local_category" meta_type="FieldIndex">
+    <indexed_attr value="local_category"/>
+  </index>
   <index name="category_and_topics" meta_type="KeywordIndex">
     <indexed_attr value="category_and_topics"/>
   </index>
   <index name="container_uid" meta_type="FieldIndex">
     <indexed_attr value="container_uid"/>
   </index>
   <index name="selected_news_folders" meta_type="KeywordIndex">
@@ -37,17 +40,24 @@
   <index name="SearchableText_en" meta_type="ZCTextIndex">
     <indexed_attr value="SearchableText_en"/>
     <extra name="index_type" value="Okapi BM25 Rank"/>
     <extra name="lexicon_id" value="plone_lexicon"/>
   </index>
   <column value="category"/>
   <column value="category_title"/>
+  <column value="category_title_nl"/>
+  <column value="category_title_de"/>
+  <column value="category_title_en"/>
   <column value="category_and_topics"/>
   <column value="container_uid"/>
   <column value="selected_news_folders"/>
   <column value="title_nl"/>
   <column value="title_de"/>
   <column value="title_en"/>
   <column value="description_nl"/>
   <column value="description_de"/>
   <column value="description_en"/>
+  <column value="local_category"/>
+  <column value="local_category_nl"/>
+  <column value="local_category_de"/>
+  <column value="local_category_en"/>
 </object>
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles/default/contentrules.xml` & `imio_news_core-1.2.9/src/imio/news/core/profiles/default/contentrules.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles/default/registry.xml` & `imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles/default/rolemap.xml` & `imio_news_core-1.2.9/src/imio/news/core/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.Entity.xml` & `imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/imio.news.Entity.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.Folder.xml` & `imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/imio.news.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml` & `imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml` & `imio_news_core-1.2.9/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/profiles.zcml` & `imio_news_core-1.2.9/src/imio/news/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/serializer/newsitem.py` & `imio_news_core-1.2.9/src/imio/news/core/serializer/newsitem.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/setuphandlers.py` & `imio_news_core-1.2.9/src/imio/news/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/subscribers.py` & `imio_news_core-1.2.9/src/imio/news/core/subscribers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
-
+from imio.news.core.rest.odwb_endpoint import OdwbEndpointGet
 from imio.news.core.utils import get_entity_for_obj
 from imio.news.core.utils import get_news_folder_for_news_item
 from imio.news.core.utils import reload_faceted_config
 from imio.smartweb.common.utils import remove_cropping
 from plone import api
+from plone.api.content import get_state
+from Products.DCWorkflow.interfaces import IAfterTransitionEvent
 from z3c.relationfield import RelationValue
 from z3c.relationfield.interfaces import IRelationList
 from zope.component import getUtility
 from zope.globalrequest import getRequest
 from zope.intid.interfaces import IIntIds
 from zope.lifecycleevent import Attributes
 from zope.lifecycleevent import modified
@@ -68,14 +70,15 @@
 
 def removed_newsfolder(obj, event):
     try:
         brains = api.content.find(selected_news_folders=obj.UID())
     except api.exc.CannotGetPortalError:
         # This happen when we try to remove plone object
         return
+    # We remove reference to this news folder out of all news items
     for brain in brains:
         news = brain.getObject()
         news.selected_news_folders = [
             uid for uid in news.selected_news_folders if uid != obj.UID()
         ]
         news.reindexObject(idxs=["selected_news_folders"])
     request = getRequest()
@@ -95,25 +98,52 @@
         return
     for d in event.descriptions:
         if IAttributes.providedBy(d) and "ILeadImageBehavior.image" in d.attributes:
             # we need to remove cropping information of previous image
             remove_cropping(
                 obj, "image", ["portrait_affiche", "paysage_affiche", "carre_affiche"]
             )
+    if get_state(obj) == "published":
+        request = getRequest()
+        endpoint = OdwbEndpointGet(obj, request)
+        endpoint.reply()
 
 
 def moved_news_item(obj, event):
     if event.oldParent == event.newParent and event.oldName != event.newName:
         # item was simply renamed
         return
     if type(event) is ObjectRemovedEvent:
         # We don't have anything to do if news item is being removed
         return
     container_newsfolder = get_news_folder_for_news_item(obj)
     set_uid_of_referrer_newsfolders(obj, container_newsfolder)
+    if event.oldParent is not None and get_state(obj) == "published":
+        request = getRequest()
+        endpoint = OdwbEndpointGet(obj, request)
+        endpoint.reply()
+
+
+def removed_news_item(obj, event):
+    request = getRequest()
+    endpoint = OdwbEndpointGet(obj, request)
+    endpoint.remove()
+
+
+def published_news_item_transition(obj, event):
+    if not IAfterTransitionEvent.providedBy(event):
+        return
+    if event.new_state.id == "published":
+        request = getRequest()
+        endpoint = OdwbEndpointGet(obj, request)
+        endpoint.reply()
+    if event.new_state.id == "private" and event.old_state.id != event.new_state.id:
+        request = getRequest()
+        endpoint = OdwbEndpointGet(obj, request)
+        endpoint.remove()
 
 
 def mark_current_newsfolder_in_news_from_other_newsfolder(obj, event):
     changed = False
     newsfolders_to_treat = []
     for d in event.descriptions:
         if not IAttributes.providedBy(d):
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/subscribers.zcml` & `imio_news_core-1.2.9/src/imio/news/core/subscribers.zcml`

 * *Files 20% similar despite different names*

```diff
@@ -25,8 +25,16 @@
                    zope.lifecycleevent.interfaces.IObjectModifiedEvent"
               handler=".subscribers.modified_news_item" />
 
   <subscriber for="imio.news.core.contents.INewsItem
                    zope.lifecycleevent.interfaces.IObjectMovedEvent"
               handler=".subscribers.moved_news_item" />
 
+  <subscriber for="imio.news.core.contents.INewsItem
+                   zope.lifecycleevent.interfaces.IObjectRemovedEvent"
+              handler=".subscribers.removed_news_item" />
+
+  <subscriber for="imio.news.core.contents.INewsItem
+                   Products.DCWorkflow.interfaces.IAfterTransitionEvent"
+              handler=".subscribers.published_news_item_transition" />
+
 </configure>
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/testing.py` & `imio_news_core-1.2.9/src/imio/news/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/resources/plone.png` & `imio_news_core-1.2.9/src/imio/news/core/tests/resources/plone.png`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/robot/test_example.robot` & `imio_news_core-1.2.9/src/imio/news/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_bring_news_into_news_folders.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_bring_news_into_news_folders.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_cropping.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_entity.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_local_roles.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_multilingual.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_newsfolder.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_newsfolder.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_newsitem.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_newsitem.py`

 * *Files 24% similar despite different names*

```diff
@@ -87,15 +87,19 @@
         )
         factory = getUtility(
             IVocabularyFactory, "imio.news.vocabulary.NewsLocalCategories"
         )
         vocabulary = factory(news)
         self.assertEqual(len(vocabulary), 0)
 
-        self.entity.local_categories = "First\nSecond\nThird"
+        self.entity.local_categories = [
+            {"fr": "First", "nl": "", "de": "", "en": ""},
+            {"fr": "Second", "nl": "", "de": "", "en": ""},
+            {"fr": "Third", "nl": "", "de": "", "en": ""},
+        ]
         vocabulary = factory(news)
         self.assertEqual(len(vocabulary), 3)
 
     def test_view(self):
         newsitem = api.content.create(
             container=self.news_folder,
             type="imio.news.NewsItem",
@@ -133,70 +137,14 @@
         news_item = api.content.create(
             container=self.news_folder,
             type="imio.news.NewsItem",
             title="My news item",
         )
         self.assertEqual(news_item.selected_news_folders, [self.news_folder.UID()])
 
-    def test_indexes(self):
-        news_item1 = api.content.create(
-            container=self.news_folder,
-            type="imio.news.NewsItem",
-            title="NewsItem1",
-        )
-        news_folder2 = api.content.create(
-            container=self.entity,
-            type="imio.news.NewsFolder",
-            title="NewsFolder2",
-        )
-        news_item2 = api.content.create(
-            container=news_folder2,
-            type="imio.news.NewsItem",
-            title="NewsItem2",
-        )
-        catalog = api.portal.get_tool("portal_catalog")
-        brain = api.content.find(UID=news_item1.UID())[0]
-        indexes = catalog.getIndexDataForRID(brain.getRID())
-        self.assertEqual(indexes.get("container_uid"), self.news_folder.UID())
-
-        # On va requêter sur self.news_folder et trouver les 2 événements car news_item2 vient de s'ajouter dedans aussi.
-        news_item2.selected_news_folders = [self.news_folder.UID()]
-        news_item2.reindexObject()
-        brains = api.content.find(selected_news_folders=self.news_folder.UID())
-        lst = [brain.UID for brain in brains]
-        self.assertEqual(lst, [news_item1.UID(), news_item2.UID()])
-
-        # On va requêter sur news_folder2 et trouver uniquement news_item2 car news_item2 est dans les 2 news folders mais news_item1 n'est que dans self.news_folder
-        news_item2.selected_news_folders = [news_folder2.UID(), self.news_folder.UID()]
-        news_item2.reindexObject()
-        brains = api.content.find(selected_news_folders=news_folder2.UID())
-        lst = [brain.UID for brain in brains]
-        self.assertEqual(lst, [news_item2.UID()])
-
-        # Via une recherche catalog sur les news_folder, on va trouver les 2 événements
-        brains = api.content.find(
-            selected_news_folders=[news_folder2.UID(), self.news_folder.UID()]
-        )
-        lst = [brain.UID for brain in brains]
-        self.assertEqual(lst, [news_item1.UID(), news_item2.UID()])
-
-        # On va requêter sur les 2 news folders et trouver les 2 événements car 1 dans chaque
-        news_item2.selected_news_folders = [news_folder2.UID()]
-        news_item2.reindexObject()
-        brains = api.content.find(
-            selected_news_folders=[news_folder2.UID(), self.news_folder.UID()]
-        )
-        lst = [brain.UID for brain in brains]
-        self.assertEqual(lst, [news_item1.UID(), news_item2.UID()])
-
-        api.content.move(news_item1, news_folder2)
-        brain = api.content.find(UID=news_item1.UID())[0]
-        indexes = catalog.getIndexDataForRID(brain.getRID())
-        self.assertEqual(indexes.get("container_uid"), news_folder2.UID())
-
     def test_searchable_text(self):
         news_item = api.content.create(
             container=self.news_folder,
             type="imio.news.NewsItem",
             title="Title",
         )
         catalog = api.portal.get_tool("portal_catalog")
@@ -220,32 +168,14 @@
                 "description",
                 "text",
                 "agriculture",
                 "travaux",
             ],
         )
 
-    def test_category_title_index(self):
-        news_item = api.content.create(
-            container=self.news_folder,
-            type="imio.news.NewsItem",
-            title="Title",
-        )
-        news_item.category = "works"
-        news_item.reindexObject()
-        catalog = api.portal.get_tool("portal_catalog")
-        brain = api.content.find(UID=news_item.UID())[0]
-        indexes = catalog.getIndexDataForRID(brain.getRID())
-        self.assertEqual(indexes.get("category_title"), "Travaux")
-        news_item.local_category = "Local category"
-        news_item.reindexObject()
-        brain = api.content.find(UID=news_item.UID())[0]
-        indexes = catalog.getIndexDataForRID(brain.getRID())
-        self.assertEqual(indexes.get("category_title"), "Local category")
-
     def test_referrer_newsfolders(self):
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         intids = getUtility(IIntIds)
         entity2 = api.content.create(
             container=self.portal,
             type="imio.news.Entity",
             id="entity2",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_robot.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_setup.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_utils.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/tests/test_vocabularies.py` & `imio_news_core-1.2.9/src/imio/news/core/tests/test_vocabularies.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.assertEqual(len(vocabulary), 0)
 
     def test_news_categories_topics_basic(self):
         entity = api.content.create(
             container=self.portal,
             type="imio.news.Entity",
             title="Entity",
-            local_categories="",
+            local_categories=[],
         )
         newsfolder = api.content.create(
             container=entity,
             type="imio.news.NewsFolder",
             title="News folder",
         )
 
@@ -53,15 +53,19 @@
         self.assertEqual(len(vocabulary), 21)  # must be updated if add new vocabulary
 
     def test_news_categories_topics_local_cat(self):
         entity = api.content.create(
             container=self.portal,
             type="imio.news.Entity",
             title="Entity",
-            local_categories="Foo\r\nbaz\r\nbar",
+            local_categories=[
+                {"fr": "Foo", "nl": "", "de": "", "en": ""},
+                {"fr": "baz", "nl": "", "de": "", "en": ""},
+                {"fr": "bar", "nl": "", "de": "", "en": ""},
+            ],
         )
         newsfolder = api.content.create(
             container=entity,
             type="imio.news.NewsFolder",
             title="News folder",
         )
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/upgrades/configure.zcml` & `imio_news_core-1.2.9/src/imio/news/core/upgrades/configure.zcml`

 * *Files 21% similar despite different names*

```diff
@@ -39,14 +39,38 @@
       name="upgrade_1009_to_1010"
       title="Upgrade core from 1009 to 1010"
       directory="profiles/1009_to_1010"
       description="Add new permission to manager : imio.news.core.BringNewsIntoPersonnalNewsFolder"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
 
+  <genericsetup:registerProfile
+      name="upgrade_1011_to_1012"
+      title="Upgrade core from 1011 to 1012"
+      directory="profiles/1011_to_1012"
+      description="Add two new registry key to store push keys for ODWB"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
+  <genericsetup:registerProfile
+      name="upgrade_1012_to_1013"
+      title="Upgrade core from 1012 to 1013"
+      directory="profiles/1012_to_1013"
+      description="Add metadatas for (local) categories translations"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
+  <genericsetup:registerProfile
+      name="upgrade_1013_to_1014"
+      title="Upgrade core from 1013 to 1014"
+      directory="profiles/1013_to_1014"
+      description="Add index for local category search"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
   <genericsetup:upgradeStep
       title="Refresh faceted"
       description="Refresh faceted configurations on all entities / news folders"
       source="1000"
       destination="1001"
       handler=".upgrades.refresh_objects_faceted"
       profile="imio.news.core:default"
@@ -148,8 +172,54 @@
       profile="imio.news.core:default">
     <genericsetup:upgradeStep
         title="Reindex catalog for category_title (local category OR category)"
         handler=".upgrades.reindex_catalog"
         />
   </genericsetup:upgradeSteps>
 
+  <genericsetup:upgradeSteps
+      source="1011"
+      destination="1012"
+      profile="imio.news.core:default">
+    <genericsetup:upgradeDepends
+        title="Add two new registry key to store push keys for ODWB"
+        import_profile="imio.news.core.upgrades:upgrade_1011_to_1012"
+        />
+  </genericsetup:upgradeSteps>
+
+  <genericsetup:upgradeSteps
+      source="1012"
+      destination="1013"
+      profile="imio.news.core:default">
+    <genericsetup:upgradeDepends
+        title="Install collective.z3cform.datagridfield"
+        import_profile="collective.z3cform.datagridfield:default"
+        />
+    <genericsetup:upgradeStep
+        title="Migrate local_categories to datagridfield"
+        handler=".upgrades.migrate_local_categories"
+        />
+    <genericsetup:upgradeDepends
+        title="Add metadatas for (local) categories translations"
+        import_profile="imio.news.core.upgrades:upgrade_1012_to_1013"
+        />
+    <genericsetup:upgradeStep
+        title="Reindex catalog"
+        handler=".upgrades.reindex_catalog"
+        />
+  </genericsetup:upgradeSteps>
+
+  <genericsetup:upgradeSteps
+      source="1013"
+      destination="1014"
+      profile="imio.news.core:default">
+    <genericsetup:upgradeDepends
+        title="Add index for local category search"
+        import_profile="imio.news.core.upgrades:upgrade_1013_to_1014"
+        />
+    <genericsetup:upgradeStep
+        title="Reindex catalog"
+        handler=".upgrades.reindex_catalog"
+        />
+  </genericsetup:upgradeSteps>
+
 </configure>
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml` & `imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml` & `imio_news_core-1.2.9/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/upgrades/upgrades.py` & `imio_news_core-1.2.9/src/imio/news/core/upgrades/upgrades.py`

 * *Files 23% similar despite different names*

```diff
@@ -63,7 +63,22 @@
     catalog.manage_delIndex("SearchableText_fr")
 
 
 def remove_title_description_fr(context):
     catalog = api.portal.get_tool("portal_catalog")
     catalog.delColumn("title_fr")
     catalog.delColumn("description_fr")
+
+
+def migrate_local_categories(context):
+    brains = api.content.find(portal_type=["imio.news.Entity"])
+    for brain in brains:
+        obj = brain.getObject()
+        if obj.local_categories:
+            categories = obj.local_categories.splitlines()
+            datagrid_categories = [
+                {"fr": cat, "nl": "", "de": "", "en": ""} for cat in categories
+            ]
+            obj.local_categories = datagrid_categories
+            logger.info(
+                "Categories migrated to Datagrid for entity {}".format(obj.Title())
+            )
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/utils.py` & `imio_news_core-1.2.9/src/imio/news/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/viewlets/configure.zcml` & `imio_news_core-1.2.9/src/imio/news/core/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/viewlets/news.py` & `imio_news_core-1.2.9/src/imio/news/core/viewlets/news.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio/news/core/vocabularies.py` & `imio_news_core-1.2.9/src/imio/news/core/vocabularies.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,26 @@
         return SimpleVocabulary(terms)
 
 
 NewsCategoriesVocabulary = NewsCategoriesVocabularyFactory()
 
 
 class NewsLocalCategoriesVocabularyFactory:
-    def __call__(self, context=None):
+    def __call__(self, context=None, lang="fr"):
         if IPloneSiteRoot.providedBy(context):
             # ex: call on @types or @vocabularies from RESTAPI
             return SimpleVocabulary([])
         obj = context
         while not IEntity.providedBy(obj) and obj is not None:
             obj = parent(obj)
         if not obj.local_categories:
             return SimpleVocabulary([])
 
-        values = obj.local_categories.splitlines()
-        terms = [SimpleTerm(value=t, token=t, title=t) for t in values]
+        values = {cat["fr"]: cat[lang] or cat["fr"] for cat in obj.local_categories}
+        terms = [SimpleTerm(value=k, token=k, title=v) for k, v in values.items()]
         return SimpleVocabulary(terms)
 
 
 NewsLocalCategoriesVocabulary = NewsLocalCategoriesVocabularyFactory()
 
 
 class NewsCategoriesAndTopicsVocabularyFactory:
```

### Comparing `imio.news.core-1.2.8/src/imio/news/core/vocabularies.zcml` & `imio_news_core-1.2.9/src/imio/news/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.8/src/imio.news.core.egg-info/PKG-INFO` & `imio_news_core-1.2.9/src/imio.news.core.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 Metadata-Version: 2.1
 Name: imio.news.core
-Version: 1.2.8
+Version: 1.2.9
 Summary: Core product for iMio news website
 Home-page: https://github.com/collective/imio.news.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.news.core
 Project-URL: Source, https://github.com/imio/imio.news.core
 Project-URL: Tracker, https://github.com/imio/imio.news.core/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: embeddify
+Requires-Dist: z3c.jbot
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.gallery
+Requires-Dist: plone.restapi
+Requires-Dist: plone.app.dexterity
+Requires-Dist: plone.app.imagecropping
+Requires-Dist: collective.taxonomy
+Requires-Dist: collective.z3cform.datagridfield
+Requires-Dist: eea.facetednavigation
+Requires-Dist: embeddify
+Requires-Dist: imio.smartweb.common
+Requires-Dist: imio.smartweb.locales
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: mock; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 
 .. image:: https://github.com/IMIO/imio.news.core/workflows/Tests/badge.svg
@@ -129,14 +146,30 @@
 - Christophe Boulanger, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2024-05-27)
+------------------
+
+- WEB-4101 : Add index for local category search
+  [laulaz]
+
+- Fix bad permission name
+  [laulaz]
+
+- WEB-4088 : Cover use case for sending data in odwb for a staging environment
+  [boulch]
+
+- WEB-4088 : Add some odwb endpoints (for news , for entities)
+  [boulch]
+
+
 1.2.8 (2024-05-02)
 ------------------
 
 - WEB-4101 : Use local category (if any) instead of category in `category_title` indexer
   [laulaz]
 
 
@@ -313,9 +346,7 @@
 
 
 1.0a1 (2022-01-25)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.news.core-1.2.8/src/imio.news.core.egg-info/SOURCES.txt` & `imio_news_core-1.2.9/src/imio.news.core.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -71,26 +71,30 @@
 src/imio/news/core/profiles/default/types.xml
 src/imio/news/core/profiles/default/types/Plone_Site.xml
 src/imio/news/core/profiles/default/types/imio.news.Entity.xml
 src/imio/news/core/profiles/default/types/imio.news.Folder.xml
 src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml
 src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml
 src/imio/news/core/profiles/uninstall/browserlayer.xml
+src/imio/news/core/rest/__init__.py
+src/imio/news/core/rest/configure.zcml
+src/imio/news/core/rest/odwb_endpoint.py
 src/imio/news/core/serializer/__init__.py
 src/imio/news/core/serializer/configure.zcml
 src/imio/news/core/serializer/newsitem.py
 src/imio/news/core/tests/__init__.py
 src/imio/news/core/tests/test_bring_news_into_news_folders.py
 src/imio/news/core/tests/test_cropping.py
 src/imio/news/core/tests/test_entity.py
-src/imio/news/core/tests/test_indexer.py
+src/imio/news/core/tests/test_indexes.py
 src/imio/news/core/tests/test_local_roles.py
 src/imio/news/core/tests/test_multilingual.py
 src/imio/news/core/tests/test_newsfolder.py
 src/imio/news/core/tests/test_newsitem.py
+src/imio/news/core/tests/test_odwb.py
 src/imio/news/core/tests/test_robot.py
 src/imio/news/core/tests/test_setup.py
 src/imio/news/core/tests/test_utils.py
 src/imio/news/core/tests/test_vocabularies.py
 src/imio/news/core/tests/utils.py
 src/imio/news/core/tests/resources/plone.png
 src/imio/news/core/tests/robot/test_example.robot
@@ -104,11 +108,14 @@
 src/imio/news/core/upgrades/profiles/1006_to_1007/types/imio.news.NewsItem.xml
 src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml
 src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Entity.xml
 src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Folder.xml
 src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsFolder.xml
 src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsItem.xml
 src/imio/news/core/upgrades/profiles/1009_to_1010/rolemap.xml
+src/imio/news/core/upgrades/profiles/1011_to_1012/registry.xml
+src/imio/news/core/upgrades/profiles/1012_to_1013/catalog.xml
+src/imio/news/core/upgrades/profiles/1013_to_1014/catalog.xml
 src/imio/news/core/viewlets/__init__.py
 src/imio/news/core/viewlets/configure.zcml
 src/imio/news/core/viewlets/news.py
 src/imio/news/core/viewlets/news/button_to_bring_news.pt
```

