# Comparing `tmp/lampsible-1.0.0.tar.gz` & `tmp/lampsible-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lampsible-1.0.0.tar", last modified: Wed May  1 19:11:14 2024, max compression
+gzip compressed data, was "lampsible-1.1.0.tar", last modified: Fri May 31 11:09:18 2024, max compression
```

## Comparing `lampsible-1.0.0.tar` & `lampsible-1.1.0.tar`

### file list

```diff
@@ -1,91 +1,95 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/
--rw-rw-r--   0 brian     (1000) brian     (1000)       54 2024-05-01 19:10:38.000000 lampsible-1.0.0/.gitignore
--rw-rw-r--   0 brian     (1000) brian     (1000)    11358 2024-05-01 19:10:38.000000 lampsible-1.0.0/LICENSE
--rw-r--r--   0 brian     (1000) brian     (1000)     2694 2024-05-01 19:11:14.293008 lampsible-1.0.0/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     1817 2024-05-01 19:10:38.000000 lampsible-1.0.0/README.md
--rw-rw-r--   0 brian     (1000) brian     (1000)     1069 2024-05-01 19:10:38.000000 lampsible-1.0.0/pyproject.toml
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2024-05-01 19:11:14.293008 lampsible-1.0.0/setup.cfg
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.249013 lampsible-1.0.0/src/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/
--rw-rw-r--   0 brian     (1000) brian     (1000)       22 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    21636 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/arg_validator.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2137 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/constants.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    16544 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/lampsible.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/
--rw-rw-r--   0 brian     (1000) brian     (1000)       94 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/ansible-galaxy-requirements.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      659 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/apache.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      702 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/lamp-stack.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      720 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/laravel.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      291 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/mysql.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      239 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/php.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.249013 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      391 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      832 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.249013 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      517 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1507 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)     6434 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.249013 lampsible-1.0.0/src/lampsible/project/roles/apache2/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache2/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      322 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache2/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/apt-update/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/apt-update/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      175 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apt-update/tasks/main.yaml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/domain-for-wordpress/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/domain-for-wordpress/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      409 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      299 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      971 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/laravel/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/laravel/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      798 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/laravel/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/laravel/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1068 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/laravel/templates/.env.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/mysql/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/mysql/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1368 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/mysql/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/php/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/php/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      241 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/php/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      495 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     7260 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf
--rw-rw-r--   0 brian     (1000) brian     (1000)    73018 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/pip/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/pip/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)       62 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/pip/tasks/main.yaml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/ssl-certbot/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/ssl-certbot/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      264 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/ssl-certbot/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/ssl-selfsigned/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/ssl-selfsigned/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      837 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      262 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      582 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/templates/.htaccess
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/wordpress-cli/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/wordpress-cli/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     2644 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/wordpress-cli/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/wordpress-manual/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/wordpress-manual/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     2416 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/wordpress-manual/tasks/main.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)     1657 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/wordpress.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)     2694 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     2031 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       55 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/entry_points.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       42 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       10 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       54 2024-05-31 11:08:29.000000 lampsible-1.1.0/.gitignore
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11358 2024-05-31 11:08:29.000000 lampsible-1.1.0/LICENSE
+-rw-r--r--   0 brian     (1000) brian     (1000)     2871 2024-05-31 11:09:18.717093 lampsible-1.1.0/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1973 2024-05-31 11:08:29.000000 lampsible-1.1.0/README.md
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1090 2024-05-31 11:08:29.000000 lampsible-1.1.0/pyproject.toml
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2024-05-31 11:09:18.717093 lampsible-1.1.0/setup.cfg
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       22 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    25058 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/arg_validator.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2235 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/constants.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    17292 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/lampsible.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       94 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/ansible-galaxy-requirements.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      652 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/apache.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      712 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/joomla.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      695 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/lamp-stack.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      713 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/laravel.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      284 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/mysql.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      232 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/php.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/lampsible/project/roles/apache-conf/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/apache-conf/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      391 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/apache-conf/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/apache-conf/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      832 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/lampsible/project/roles/apache-vhosts/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/apache-vhosts/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      517 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/apache-vhosts/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1507 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6434 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/lampsible/project/roles/apache2/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/apache2/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      322 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/apache2/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/lampsible/project/roles/apt/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/apt/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      364 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/apt/tasks/main.yaml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/lampsible/project/roles/domain-for-wordpress/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/domain-for-wordpress/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      409 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/lampsible/project/roles/fail2ban/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/fail2ban/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      299 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/fail2ban/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/fail2ban/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      971 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/lampsible/project/roles/joomla/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/joomla/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2115 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/joomla/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/lampsible/project/roles/laravel/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/laravel/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      798 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/laravel/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/laravel/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1115 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/laravel/templates/.env.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.709093 lampsible-1.1.0/src/lampsible/project/roles/mysql/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/mysql/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1368 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/mysql/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/php/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/php/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      241 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/php/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/phpmyadmin/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/phpmyadmin/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      495 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/phpmyadmin/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/phpmyadmin/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7260 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73018 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/pip/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/pip/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       62 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/pip/tasks/main.yaml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/ssl-certbot/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/ssl-certbot/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      264 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/ssl-certbot/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/ssl-selfsigned/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/ssl-selfsigned/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      837 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/wordpress-block-xmlrpc/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/wordpress-block-xmlrpc/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      259 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/wordpress-block-xmlrpc/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/wordpress-block-xmlrpc/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      582 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/wordpress-block-xmlrpc/templates/.htaccess
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/wordpress-cli/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/wordpress-cli/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2586 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/wordpress-cli/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.713093 lampsible-1.1.0/src/lampsible/project/roles/wordpress-manual/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible/project/roles/wordpress-manual/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2416 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/roles/wordpress-manual/tasks/main.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1650 2024-05-31 11:08:29.000000 lampsible-1.1.0/src/lampsible/project/wordpress.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-31 11:09:18.717093 lampsible-1.1.0/src/lampsible.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)     2871 2024-05-31 11:09:18.000000 lampsible-1.1.0/src/lampsible.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2107 2024-05-31 11:09:18.000000 lampsible-1.1.0/src/lampsible.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2024-05-31 11:09:18.000000 lampsible-1.1.0/src/lampsible.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       55 2024-05-31 11:09:18.000000 lampsible-1.1.0/src/lampsible.egg-info/entry_points.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       50 2024-05-31 11:09:18.000000 lampsible-1.1.0/src/lampsible.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       10 2024-05-31 11:09:18.000000 lampsible-1.1.0/src/lampsible.egg-info/top_level.txt
```

### Comparing `lampsible-1.0.0/LICENSE` & `lampsible-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/PKG-INFO` & `lampsible-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: lampsible
-Version: 1.0.0
+Version: 1.1.0
 Summary: Deploy and set up LAMP stacks with Ansible
 Author-email: "Brian St. Hilaire" <brian.st-hilaire@sanctus-tech.com>
 Project-URL: Homepage, https://github.com/saint-hilaire/lampsible
 Project-URL: Issues, https://github.com/saint-hilaire/lampsible/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ansible-core
 Requires-Dist: ansible-runner
-Requires-Dist: requests
+Requires-Dist: requests>=2.32.3
 Requires-Dist: fqdn
 
 # Lampsible
 
 ## About
 
 Lampsible - LAMP stacks with Ansible and a super simple CLI. This tool can automate anything from
@@ -58,27 +58,35 @@
 
 ```
 lampsible someuser@somehost.com wordpress \
     --ssl-certbot \
     --email-for-ssl you@yourdomain.com
 ```
 
+Install a production ready Joomla site:
+
+```
+lampsible someuser@somehost.com joomla \
+    --ssl-certbot \
+    --email-for-ssl you@yourdomain.com
+```
+
 Install a Laravel app on a test server:
 
 ```
 lampsible someuser@somehost.com laravel \
     --ssl-certbot \
     --test-cert \
     --apache-server-admin you@yourdomain.com \
     --app-name cool-laravel-app \
     --app-build-path /path/to/your/local/cool-laravel-app-0.7rc.tar.gz \
     --laravel-artisan-commands key:generate,migrate
 ```
 
-Set up a LAMP with various custom configuration and a self signed SSL certificate on some local VM:
+Set up a LAMP stack with various custom configuration and a self signed SSL certificate on some local VM:
 
 ```
 lampsible someuser@192.168.123.123 lamp-stack \
     --ask-remote-sudo \
     --ssl-selfsigned \
     --database-username dbuser \
     --database-name testdb \
@@ -89,8 +97,8 @@
 ```
 
 
 Run `lampsible --help` for a full list of options.
 
 ## Contributing 
 
-PLease do! I'd be more than happy to see Issues, Pull Requests and any other kind of feedback ;-)
+Please do! I'd be more than happy to see Issues, Pull Requests and any other kind of feedback ;-)
```

### Comparing `lampsible-1.0.0/README.md` & `lampsible-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,27 +35,35 @@
 
 ```
 lampsible someuser@somehost.com wordpress \
     --ssl-certbot \
     --email-for-ssl you@yourdomain.com
 ```
 
+Install a production ready Joomla site:
+
+```
+lampsible someuser@somehost.com joomla \
+    --ssl-certbot \
+    --email-for-ssl you@yourdomain.com
+```
+
 Install a Laravel app on a test server:
 
 ```
 lampsible someuser@somehost.com laravel \
     --ssl-certbot \
     --test-cert \
     --apache-server-admin you@yourdomain.com \
     --app-name cool-laravel-app \
     --app-build-path /path/to/your/local/cool-laravel-app-0.7rc.tar.gz \
     --laravel-artisan-commands key:generate,migrate
 ```
 
-Set up a LAMP with various custom configuration and a self signed SSL certificate on some local VM:
+Set up a LAMP stack with various custom configuration and a self signed SSL certificate on some local VM:
 
 ```
 lampsible someuser@192.168.123.123 lamp-stack \
     --ask-remote-sudo \
     --ssl-selfsigned \
     --database-username dbuser \
     --database-name testdb \
@@ -66,8 +74,8 @@
 ```
 
 
 Run `lampsible --help` for a full list of options.
 
 ## Contributing 
 
-PLease do! I'd be more than happy to see Issues, Pull Requests and any other kind of feedback ;-)
+Please do! I'd be more than happy to see Issues, Pull Requests and any other kind of feedback ;-)
```

### Comparing `lampsible-1.0.0/pyproject.toml` & `lampsible-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,29 @@
     "setuptools>=69.0",
     "setuptools-scm>=8.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lampsible"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
     {name="Brian St. Hilaire", email="brian.st-hilaire@sanctus-tech.com"}
 ]
 description = "Deploy and set up LAMP stacks with Ansible"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "ansible-core",
     "ansible-runner",
-    "requests",
+    "requests>=2.32.3",
     "fqdn",
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Ansible",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `lampsible-1.0.0/src/lampsible/arg_validator.py` & `lampsible-1.1.0/src/lampsible/arg_validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,18 +18,14 @@
         return self.args
 
 
     def get_apache_vhosts(self):
         return self.apache_vhosts
 
 
-    def get_apache_document_root(self):
-        return self.apache_document_root
-
-
     def get_apache_custom_conf_name(self):
         try:
             return self.apache_custom_conf_name
         except AttributeError:
             return ''
 
 
@@ -98,59 +94,69 @@
 
     def get_certbot_test_cert_string(self):
         return '--test-cert' if self.args.test_cert else ''
 
 
     def get_extravars_dict(self):
         extravars = {
+            'web_host': self.web_host,
             'apache_vhosts': self.get_apache_vhosts(),
+            'apache_document_root': self.apache_document_root,
+            'apache_vhost_name': self.apache_vhost_name,
             'apache_custom_conf_name': self.get_apache_custom_conf_name(),
             'database_username': self.args.database_username,
             'database_password': self.args.database_password,
             'database_host': DEFAULT_DATABASE_HOST,
             'database_name': self.args.database_name,
             'database_table_prefix': self.args.database_table_prefix,
             'php_version': self.args.php_version,
             'php_extensions': self.php_extensions,
             'ssl_certbot': self.args.ssl_certbot,
             'ssl_selfsigned': self.args.ssl_selfsigned,
             'email_for_ssl': self.args.email_for_ssl,
             'certbot_domains_string': self.get_certbot_domains_string(),
             'certbot_test_cert_string': self.get_certbot_test_cert_string(),
             'insecure_skip_fail2ban': self.args.insecure_skip_fail2ban,
+            'extra_packages': self.args.extra_packages,
         }
         if self.args.remote_sudo_password:
             # TODO: It would be better to not include this as an extravar, but to
             # make use of Ansible Runner's password feature in the
             # Input Directory Hierarchy.
             extravars['ansible_sudo_pass'] = self.args.remote_sudo_password
 
+        if self.args.action in [
+            'wordpress',
+            'joomla',
+        ]:
+            extravars['site_title'] = self.args.site_title
+            extravars['admin_username'] = self.args.admin_username
+            extravars['admin_email'] = self.args.admin_email
+            extravars['admin_password'] = self.args.admin_password
+
         if self.args.action == 'wordpress':
             extravars['wordpress_version'] = self.args.wordpress_version
             extravars['wordpress_locale'] = self.args.wordpress_locale
-            extravars['wordpress_site_title'] = self.args.wordpress_site_title
-            extravars['wordpress_admin_username'] = \
-                self.args.wordpress_admin_username
-            extravars['wordpress_admin_password'] = \
-                self.args.wordpress_admin_password
-            extravars['wordpress_admin_email'] = \
-                self.args.wordpress_admin_email
 
             # TODO: This should be deprecated in favor of
             # letting WP-CLI handlethese.
             extravars['wordpress_auth_vars'] = self.get_wordpress_auth_vars()
 
             extravars['wordpress_insecure_allow_xmlrpc'] = \
                 self.args.wordpress_insecure_allow_xmlrpc
             extravars['wordpress_url'] = self.get_wordpress_url()
-            extravars['wp_apache_document_root'] = \
-                self.get_apache_document_root()
             extravars['wordpress_manual_install'] = \
                 self.args.wordpress_manual_install
 
+        elif self.args.action == 'joomla':
+            # TODO: We could do something like 'cms_version' instead.
+            extravars['joomla_version'] = self.args.joomla_version
+            extravars['joomla_admin_full_name'] = \
+                self.args.joomla_admin_full_name
+
         elif self.args.action in ['laravel']:
             extravars['app_build_path'] = self.args.app_build_path
             extravars['app_source_root'] = self.app_source_root
             extravars['app_local_env'] = self.args.app_local_env
             extravars['laravel_artisan_commands'] = \
                 self.args.laravel_artisan_commands
 
@@ -275,18 +281,53 @@
 
         server_name = self.web_host
         try:
             assert FQDN(server_name).is_valid
         except AssertionError:
             server_name = DEFAULT_APACHE_SERVER_NAME
 
+        if self.args.action in [
+            'wordpress',
+            'joomla',
+        ]:
+            if self.args.apache_document_root == DEFAULT_APACHE_DOCUMENT_ROOT:
+                self.apache_document_root = '{}/{}'.format(
+                    DEFAULT_APACHE_DOCUMENT_ROOT,
+                    self.args.action
+                )
+            else:
+                self.apache_document_root = self.args.apache_document_root
+
+            if self.args.apache_vhost_name == DEFAULT_APACHE_VHOST_NAME:
+                self.apache_vhost_name = self.args.action
+            else:
+                self.apache_vhost_name = self.args.apache_vhost_name
+
+        elif self.args.action == 'laravel':
+            if self.args.apache_document_root == DEFAULT_APACHE_DOCUMENT_ROOT:
+                self.apache_document_root = '{}/{}/public'.format(
+                    DEFAULT_APACHE_DOCUMENT_ROOT,
+                    self.args.app_name
+                )
+            else:
+                self.apache_document_root = self.args.apache_document_root
+
+            if self.args.apache_vhost_name == DEFAULT_APACHE_VHOST_NAME:
+                self.apache_vhost_name = self.args.app_name
+            else:
+                self.apache_vhost_name = self.args.apache_vhost_name
+
+        else:
+            self.apache_document_root = self.args.apache_document_root
+            self.apache_vhost_name = self.args.apache_vhost_name
+
         base_vhost_dict = {
             'base_vhost_file': '{}.conf'.format(DEFAULT_APACHE_VHOST_NAME),
-            'document_root':  self.args.apache_document_root,
-            'vhost_name':     self.args.apache_vhost_name,
+            'document_root':  self.apache_document_root,
+            'vhost_name':     self.apache_vhost_name,
             'server_name':    server_name,
             'server_admin':   self.args.apache_server_admin,
             'allow_override': self.get_apache_allow_override(),
         }
 
         self.apache_vhosts = [base_vhost_dict]
 
@@ -303,20 +344,57 @@
                 self.apache_custom_conf_name = 'ssl-params'
 
         return 0
 
 
     def validate_database_args(self):
 
+        default_database_names = {
+            'wordpress': 'wordpress',
+            'joomla':    'joomla',
+            'laravel':   self.args.app_name,
+        }
+
+        default_database_table_prefixes = {
+            'wordpress': 'wp_',
+            # TODO?
+            'joomla':    '',
+            'laravel':   '',
+        }
         if self.args.database_password \
             and not self.args.insecure_cli_password:
 
             print(INSECURE_CLI_PASS_WARNING)
             return 1
 
+        if self.args.action in [
+            'wordpress',
+            'joomla',
+            'laravel',
+        ]:
+            self.handle_defaults([
+                {
+                    'arg_name': 'database_name',
+                    'cli_default_value': None,
+                    'override_default_value': default_database_names[
+                        self.args.action],
+                },
+                {
+                    'arg_name': 'database_username',
+                    'cli_default_value': None,
+                    'override_default_value': DEFAULT_DATABASE_USERNAME,
+                },
+                {
+                    'arg_name': 'database_table_prefix',
+                    'cli_default_value': DEFAULT_DATABASE_TABLE_PREFIX,
+                    'override_default_value': default_database_table_prefixes[
+                        self.args.action],
+                },
+            ], True, True)
+
         if self.args.database_username and not self.args.database_password:
             self.args.database_password = self.get_pass_and_check(
                 'Please enter a database password: ',
                 0,
                 True
             )
 
@@ -358,29 +436,46 @@
         # TODO: If we can get the ansible_facts back into a Python variable,
         # we can validate this stuff too.
         # NOTE:
         # * Ubuntu versions 20 and older do not support PHP versions 8.0 or newer
         # * Ubuntu 22 does not support PHP 8.0. PHP 8.1 is supported.
         # To work around the above points, you would have to manually configure the
         # APT repository.
+        # TODO: Joomla 5 requires minimum PHP 8.1.
         if self.args.php_extensions:
             extensions = [
                 extension.strip()
                 for extension in self.args.php_extensions.split(',')
             ]
+        elif self.args.action == 'lamp-stack':
+            extensions = ['mysql']
+
+        elif self.args.action == 'wordpress':
+            extensions = ['mysql']
+
+        elif self.args.action == 'joomla':
+            # TODO
+            extensions = [
+                'simplexml',
+                'dom',
+                'zip',
+                'gd',
+                'mysql',
+            ]
+
         elif self.args.action == 'laravel':
             extensions = [
                 'mysql',
                 'xml',
                 'mbstring'
             ]
-        elif self.args.action == 'wordpress':
-            extensions = ['mysql']
+
         else:
             extensions = []
+
         self.php_extensions = [
             'php{}-{}'.format(
                 self.args.php_version,
                 extension
             ) for extension in extensions
         ]
 
@@ -391,75 +486,53 @@
         if self.args.action != 'wordpress':
             return 0
 
         if not self.is_valid_wordpress_version(self.args.wordpress_version):
             print('\nInvalid WordPress version! Leave --wordpress-version blank to default to \'{}\''.format(DEFAULT_WORDPRESS_VERSION))
             return 1
 
-        if self.args.apache_document_root == DEFAULT_APACHE_DOCUMENT_ROOT:
-            wp_apache_document_root = '{}/wordpress'.format(
-                DEFAULT_APACHE_DOCUMENT_ROOT
-            )
-        else:
-            wp_apache_document_root = self.args.apache_document_root
-
-        if self.args.apache_vhost_name == DEFAULT_APACHE_VHOST_NAME:
-            wp_apache_vhost_name = 'wordpress'
-        else:
-            wp_apache_vhost_name = self.args.apache_vhost_name
-
-        for i in range(len(self.apache_vhosts)):
-            self.apache_vhosts[i]['document_root'] = wp_apache_document_root
-            self.apache_vhosts[i]['vhost_name'] = wp_apache_vhost_name
-
-        self.apache_document_root = wp_apache_document_root
+        # TODO: These are for backwards compatibility, in case a user still uses
+        # the deprecated flag instead of the one valid for all CMS.
+        # Support for deprecated flags will be dropped in a future version.
+        if self.args.wordpress_site_title and not self.args.site_title:
+            self.args.site_title = self.args.wordpress_site_title
+        if self.args.wordpress_admin_username and not self.args.admin_username:
+            self.args.admin_username = self.args.wordpress_admin_username
+        if self.args.wordpress_admin_email and not self.args.admin_email:
+            self.args.admin_email = self.args.wordpress_admin_email
+        if self.args.wordpress_admin_password and not self.args.admin_password:
+            self.args.admin_password = self.args.wordpress_admin_password
+        ####
 
         self.handle_defaults([
             {
-                'arg_name': 'database_name',
+                'arg_name': 'site_title',
                 'cli_default_value': None,
-                'override_default_value': 'wordpress',
+                'override_default_value': DEFAULT_SITE_TITLE,
             },
             {
-                'arg_name': 'database_username',
+                'arg_name': 'admin_username',
                 'cli_default_value': None,
-                'override_default_value': DEFAULT_DATABASE_USERNAME,
+                'override_default_value': DEFAULT_ADMIN_USERNAME,
             },
             {
-                'arg_name': 'database_table_prefix',
-                'cli_default_value': DEFAULT_DATABASE_TABLE_PREFIX,
-                'override_default_value': 'wp_',
-            },
-            {
-                'arg_name': 'wordpress_site_title',
-                'cli_default_value': None,
-                'override_default_value': DEFAULT_WORDPRESS_SITE_TITLE,
-            },
-            {
-                'arg_name': 'wordpress_admin_username',
-                'cli_default_value': None,
-                'override_default_value': DEFAULT_WORDPRESS_ADMIN_USERNAME,
-            },
-            {
-                'arg_name': 'wordpress_admin_email',
+                'arg_name': 'admin_email',
                 'cli_default_value': None,
-                'override_default_value': DEFAULT_WORDPRESS_ADMIN_EMAIL,
+                'override_default_value': DEFAULT_ADMIN_EMAIL,
             },
         ], True, True)
 
-        self.validate_database_args()
-
-        if self.args.wordpress_admin_password \
+        if self.args.admin_password \
             and not self.args.insecure_cli_password:
             print(INSECURE_CLI_PASS_WARNING)
             return 1
 
-        if not self.args.wordpress_admin_password:
-            self.args.wordpress_admin_password = self.get_pass_and_check(
-                'Please choose a password for the WordPress admin: ',
+        if not self.args.admin_password:
+            self.args.admin_password = self.get_pass_and_check(
+                "Please choose a password for the website's admin user: ",
                 0,
                 True
             )
 
         if self.args.ssl_certbot:
             if self.web_host[:4] == 'www.':
                 www_domain = self.web_host
@@ -498,14 +571,58 @@
             )
             assert r.status_code == 200
             return True
         except AssertionError:
             return False
 
 
+    def validate_joomla_args(self):
+        if self.args.action != 'joomla':
+            return 0
+
+        self.handle_defaults([
+            {
+                'arg_name': 'site_title',
+                'cli_default_value': None,
+                'override_default_value': DEFAULT_SITE_TITLE,
+            },
+            {
+                'arg_name': 'admin_username',
+                'cli_default_value': None,
+                'override_default_value': DEFAULT_ADMIN_USERNAME,
+            },
+            {
+                'arg_name': 'admin_email',
+                'cli_default_value': None,
+                'override_default_value': DEFAULT_ADMIN_EMAIL,
+            },
+            {
+                'arg_name': 'joomla_admin_full_name',
+                'cli_default_value': None,
+                'override_default_value': DEFAULT_JOOMLA_ADMIN_FULL_NAME,
+            },
+        ], True, True)
+
+        # TODO: If instead of returning 1 we throw an exception, we could make
+        # a small helper function out of this, see validate_wordpress_args.
+        if self.args.admin_password \
+            and not self.args.insecure_cli_password:
+            print(INSECURE_CLI_PASS_WARNING)
+            return 1
+
+        if not self.args.admin_password:
+            self.args.admin_password = self.get_pass_and_check(
+                "Please choose a password for the website's admin user: ",
+                12,
+                True
+            )
+
+        return 0
+
+
     def validate_app_args(self):
         if self.args.action not in [
             'laravel',
         ]:
             return 0
 
         try:
@@ -516,49 +633,30 @@
             return 1
         except AssertionError:
             print('FATAL! {} not found on local file system.'.format(
                 self.args.app_build_path
             ))
             return 1
 
-        if self.args.apache_vhost_name == DEFAULT_APACHE_VHOST_NAME:
-            app_apache_vhost_name = self.args.app_name
-        else:
-            app_apache_vhost_name = self.args.apache_vhost_name
-
         self.app_source_root = '/var/www/html/{}'.format(self.args.app_name)
-        app_apache_document_root = '{}/public'.format(self.app_source_root)
-
-        self.apache_document_root = app_apache_document_root
-
-        for i in range(len(self.apache_vhosts)):
-            self.apache_vhosts[i]['vhost_name'] = app_apache_vhost_name
-            self.apache_vhosts[i]['document_root'] = app_apache_document_root
-
-        self.handle_defaults([
-            {
-                'arg_name': 'database_name',
-                'cli_default_value': None,
-                'override_default_value': self.args.app_name,
-            },
-            {
-                'arg_name': 'database_username',
-                'cli_default_value': None,
-                'override_default_value': DEFAULT_DATABASE_USERNAME,
-            },
-            ], True, True
-        )
-        self.validate_database_args()
 
         self.args.laravel_artisan_commands = \
             self.args.laravel_artisan_commands.split(',')
 
         return 0
 
 
+    def validate_misc_args(self):
+        try:
+            self.args.extra_packages = self.args.extra_packages.split(',')
+        except AttributeError:
+            self.args.extra_packages = []
+        return 0
+
+
     def print_warnings(self):
         if self.args.insecure_skip_fail2ban:
             print('\nWarning! Will not install fail2ban! Your site will potentially be vulnerable to various brute force attacks. You should only pass the \'--insecure-skip-fail2ban\' flag if you have a good reason to do so. On production servers, always install fail2ban!')
 
         if self.args.wordpress_insecure_allow_xmlrpc:
             print('\nWarning! Your WordPress site\'s xmlrpc.php endpoint will be enabled - this is insecure! The endpoint xmlrpc.php is a feature from older WordPress versions which allowed programmatic access to the WordPress backend. Although it has numerous known security vulnerabilities, namely a brute force and a DoS vulnerability, it is still, for some reason, enabled by default in current WordPress versions. Lampsible will, by default, block this endpoint with an .htaccess configuration, unless you specify otherwise, which you just did. You should not be doing this, unless you have some good reason to do so!')
 
@@ -574,15 +672,17 @@
         validate_methods = [
             'validate_ansible_runner_args',
             'validate_apache_args',
             'validate_database_args',
             'validate_ssl_args',
             'validate_php_args',
             'validate_wordpress_args',
+            'validate_joomla_args',
             'validate_app_args',
+            'validate_misc_args',
         ]
         for method_name in validate_methods:
             method = getattr(self, method_name)
             result = method()
             if result != 0:
                 return result
```

### Comparing `lampsible-1.0.0/src/lampsible/constants.py` & `lampsible-1.1.0/src/lampsible/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     # LAMP-Stack basics
     'lamp-stack',
     'apache',
     'mysql',
     'php',
     # PHP CMS
     'wordpress',
+    'joomla',
     # PHP frameworks
     'laravel',
     # Local debugging
     'dump-ansible-facts',
 ]
 
 # Script paths
@@ -52,21 +53,29 @@
 DEFAULT_DATABASE_HOST         = 'localhost'
 DEFAULT_DATABASE_TABLE_PREFIX = ''
 
 # PHP
 # ---
 DEFAULT_PHP_VERSION = '8.2'
 
+# All CMS
+# -------
+DEFAULT_SITE_TITLE     = 'Sample Site'
+DEFAULT_ADMIN_USERNAME = 'admin'
+DEFAULT_ADMIN_EMAIL    = 'admin@example.com'
+
 # WordPress
 # ---------
-DEFAULT_WORDPRESS_VERSION        = 'latest'
-DEFAULT_WORDPRESS_LOCALE         = 'en_US'
-DEFAULT_WORDPRESS_SITE_TITLE     = 'Sample Site'
-DEFAULT_WORDPRESS_ADMIN_USERNAME = 'admin'
-DEFAULT_WORDPRESS_ADMIN_EMAIL    = 'admin@example.com'
+DEFAULT_WORDPRESS_VERSION = 'latest'
+DEFAULT_WORDPRESS_LOCALE  = 'en_US'
+
+# Joomla
+# ------
+DEFAULT_JOOMLA_VERSION         = '5.1.0'
+DEFAULT_JOOMLA_ADMIN_FULL_NAME = 'Sample User'
 
 # Web applications
 # ----------------
 DEFAULT_LARAVEL_ARTISAN_COMMANDS = [
     'key:generate',
     'migrate',
     'db:seed',
```

### Comparing `lampsible-1.0.0/src/lampsible/lampsible.py` & `lampsible-1.1.0/src/lampsible/lampsible.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,14 +147,31 @@
         help="the version of PHP to be installed, defaults to '{}'".format(
             DEFAULT_PHP_VERSION
         )
     )
     # TODO
     # parser.add_argument('--php-my-admin', action='store_true')
 
+    # All CMS
+    # -------
+    parser.add_argument('--site-title', '-t',
+        help="The \"Site Title\" configuration of your website. If you leave this blank, you will be prompted to enter a value, or default to '{}'".format(
+            DEFAULT_SITE_TITLE
+        )
+    )
+    parser.add_argument('--admin-username',
+        help="The admin username of your website. If you leave this blank, you will be prompted to enter a value, or default to '{}'".format(
+            DEFAULT_ADMIN_USERNAME
+        )
+    )
+    parser.add_argument('--admin-email',
+        help="The email address of your website's admin username. If you leave this blank, you will be prompted to enter a value, or default to '{}'".format(
+            DEFAULT_ADMIN_EMAIL
+        )
+    )
 
     # WordPress
     # ---------
     parser.add_argument('-w', '--wordpress-version',
         default=DEFAULT_WORDPRESS_VERSION,
         help="the version of WordPress to be installed, defaults to '{}'".format(
             DEFAULT_WORDPRESS_VERSION
@@ -162,29 +179,21 @@
     )
     parser.add_argument('--wordpress-locale',
         default=DEFAULT_WORDPRESS_LOCALE,
         help="the locale of your WordPress site, defaults to '{}'".format(
             DEFAULT_WORDPRESS_LOCALE
         )
     )
-    parser.add_argument('--wordpress-site-title',
-        help="The \"Site Title\" configuration of your WordPress site. If you leave this blank, you will be prompted to enter a value, or default to '{}'".format(
-            DEFAULT_WORDPRESS_SITE_TITLE
-        )
-    )
-    parser.add_argument('--wordpress-admin-username',
-        help="The admin username of your WordPress site. If you leave this blank, you will be prompted to enter a value, or default to '{}'".format(
-            DEFAULT_WORDPRESS_ADMIN_USERNAME
-        )
-    )
-    parser.add_argument('--wordpress-admin-email',
-        help="The email address of your WordPress site's admin username. If you leave this blank, you will be prompted to enter a value, or default to '{}'".format(
-            DEFAULT_WORDPRESS_ADMIN_EMAIL
-        )
-    )
+
+    # Joomla
+    # ------
+
+    parser.add_argument('--joomla-version', '-j',
+        default=DEFAULT_JOOMLA_VERSION)
+    parser.add_argument('--joomla-admin-full-name', '-J')
 
     # Web applications
     # ----------------
     parser.add_argument('--app-name', default='laravel-app', help="the name of your Laravel app, if you're installing one. Leave blank to default to 'laravel-app'")
     parser.add_argument('--app-build-path', help="If you are installing a Laravel app, use this option to specify the local path of a production ready build-archive of your app, for example /path/to/some-app-2.0.tar.gz")
 
     # SSL
@@ -201,15 +210,15 @@
     #  Advanced Options    -
     #                      -
     # ----------------------
 
     # Ansible Runner
     # --------------
     parser.add_argument('--remote-sudo-password', help="sudo password of the remote server, this only works if you also pass '--insecure-cli-password'. This is not recommended, you should use '--ask-remote-sudo' instead.")
-    parser.add_argument('--ssh-key-file', help='path to your private SSH key')
+    parser.add_argument('--ssh-key-file', '-i',  help='path to your private SSH key')
     parser.add_argument('--private-data-dir',
         default=DEFAULT_PRIVATE_DATA_DIR,
         help="the \"private data directory\" that Ansible Runner will use. Default is '{}'. You can use this flag to pass an alternative value. However, it's best to just leave this blank. Be advised that Ansible Runner will write sensitive data here, like your private SSH key and passwords, but Lampsible will delete this directory when it finishes."
     )
     # parser.add_argument('--project-dir', '-Z', default=DEFAULT_PROJECT_DIR)
 
     # Apache
@@ -233,35 +242,50 @@
         )
     )
 
     # PHP
     # ---
     parser.add_argument('--php-extensions', help="A comma separated list of PHP extensions to install. For example, if you pass '--php-version 8.2 --php-extensions mysql,mbstring', Lampsible will install the packages php8.2-mysql and php8.2-mbstring. However, it's best to leave this blank, and let Lampsible pick sensible defaults depending on what you are installing.")
 
+    # All CMS
+    # -------
+    parser.add_argument('--admin-password',
+        help="Use this flag to provide the admin password of your CMS directly. This is not advised, and will only work if you also pass '--insecure-cli-password'. You should leave this blank instead, and Lampsible will prompt you for a password."
+    )
+
     # WordPress
     # ---------
     parser.add_argument('--wordpress-admin-password',
-        help="Use this flag to pass in the WordPress admin password directly. This is not advised, and will only work if you also pass '--insecure-cli-password'. You should leave this blank instead, and Lampsible will prompt you for a password."
+        help="deprecated, use '--admin-password' instead"
+    )
+    parser.add_argument('--wordpress-insecure-allow-xmlrpc',
+        action='store_true',
+        help="Pass this flag if you want your WordPress site's insecure(!) endpoint xmlrpc.php to be reachable. This will make your site vulnerable to various exploits, and you really shouldn't do this if you don't have a good reason for this."
     )
     # NOTE: Manually installing WordPress and passing the authentication salts
     # will be deprecated.
     parser.add_argument('--wordpress-manual-install', action='store_true',
         help="Pass this flag if you prefer to complete the \"Famous 5 Minute WordPress Install\" manually. This is not advised, and will be deprecated."
     )
     parser.add_argument('--wordpress-auth-key', help="deprecated")
     parser.add_argument('--wordpress-secure-auth-key', help="deprecated")
     parser.add_argument('--wordpress-logged-in-key', help="deprecated")
     parser.add_argument('--wordpress-nonce-key', help="deprecated")
     parser.add_argument('--wordpress-auth-salt', help="deprecated")
     parser.add_argument('--wordpress-secure-auth-salt', help="deprecated")
     parser.add_argument('--wordpress-logged-in-salt', help="deprecated")
     parser.add_argument('--wordpress-nonce-salt', help="deprecated")
-    parser.add_argument('--wordpress-insecure-allow-xmlrpc',
-        action='store_true',
-        help="Pass this flag if you want your WordPress site's insecure(!) endpoint xmlrpc.php to be reachable. This will make your site vulnerable to various exploits, and you really shouldn't do this if you don't have a good reason for this."
+    parser.add_argument('--wordpress-site-title',
+        help="deprecated, use '--site-title' instead."
+    )
+    parser.add_argument('--wordpress-admin-username',
+        help="deprecated, use '--admin-username' instead"
+    )
+    parser.add_argument('--wordpress-admin-email',
+        help="deprecated, use '--admin-email' instead"
     )
     # TODO
     # parser.add_argument('--wordpress-skip-content', action='store_true')
 
     # Web applications
     # ----------------
     parser.add_argument('--app-local-env', action='store_true',
@@ -284,14 +308,15 @@
     parser.add_argument('--domains-for-ssl', help="a comma separated list of domains that will be passed to Certbot. If left blank, Lampsible will figure out what to use based on your host and action.")
     parser.add_argument('--test-cert', action='store_true', help="Pass this flag along with '--ssl-certbot' if you are testing and want to avoid being rate limited by Let's Encrypt.")
 
     # Misc
     # ----
     parser.add_argument('--insecure-cli-password', action='store_true', help="If you want to pass passwords directly over the CLI, you have to pass this flag as well, otherwise Lampsible will refuse to run. This is not advised.")
     parser.add_argument('--insecure-skip-fail2ban', action='store_true', help="Pass this flag if you don't want to install fail2ban on your server. This is insecure not advised.")
+    parser.add_argument('--extra-packages', help="comma separated list of any extra packages to be installed on the remote server")
 
     # Metadata
     # --------
     parser.add_argument('-V', '--version', action='version', version=__version__)
 
 
     args = parser.parse_args()
```

### Comparing `lampsible-1.0.0/src/lampsible/project/apache.yml` & `lampsible-1.1.0/src/lampsible/project/lamp-stack.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 ---
 - hosts: all
   become: true
   gather_facts: true
-
   tasks:
     - include_role:
         name: "{{ item }}"
       loop:
-        - apt-update
+        - apt
         - apache2
+        - php
+        - pip
+        - mysql
 
     - include_role:
         name: ssl-selfsigned
       when: ssl_selfsigned
 
     # It's important that this runs after the selfsigned certificates,
     # if those are being used, but before Certbot, if that's being used.
```

### Comparing `lampsible-1.0.0/src/lampsible/project/lamp-stack.yml` & `lampsible-1.1.0/src/lampsible/project/joomla.yml`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 - hosts: all
   become: true
   gather_facts: true
   tasks:
     - include_role:
         name: "{{ item }}"
       loop:
-        - apt-update
+        - apt
         - apache2
         - php
         - pip
         - mysql
+        - joomla
 
     - include_role:
         name: ssl-selfsigned
       when: ssl_selfsigned
 
     # It's important that this runs after the selfsigned certificates,
     # if those are being used, but before Certbot, if that's being used.
```

### Comparing `lampsible-1.0.0/src/lampsible/project/laravel.yml` & `lampsible-1.1.0/src/lampsible/project/laravel.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 - hosts: all
   become: true
   gather_facts: true
   tasks:
     - include_role:
         name: "{{ item }}"
       loop:
-        - apt-update
+        - apt
         - apache2
         - php
         - pip
         - mysql
         - laravel
 
     - include_role:
```

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2` & `lampsible-1.1.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml` & `lampsible-1.1.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2` & `lampsible-1.1.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2` & `lampsible-1.1.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2` & `lampsible-1.1.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/laravel/tasks/main.yml` & `lampsible-1.1.0/src/lampsible/project/roles/laravel/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/laravel/templates/.env.j2` & `lampsible-1.1.0/src/lampsible/project/roles/laravel/templates/.env.j2`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 APP_NAME=Laravel
 APP_ENV={{ 'local' if app_local_env else 'production' }}
 APP_KEY=
 APP_DEBUG={{ 'true' if app_local_env else 'false' }}
-{# TODO? #}
-APP_URL=http://localhost
+APP_URL={{ 'https' if ssl_certbot or ssl_selfsigned else 'http' }}://{{ web_host }}
 
 LOG_CHANNEL=stack
 LOG_DEPRECATIONS_CHANNEL=null
 LOG_LEVEL=debug
 
 DB_CONNECTION=mysql
 DB_HOST={{ database_host }}
```

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/mysql/tasks/main.yml` & `lampsible-1.1.0/src/lampsible/project/roles/mysql/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf` & `lampsible-1.1.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini` & `lampsible-1.1.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml` & `lampsible-1.1.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/templates/.htaccess` & `lampsible-1.1.0/src/lampsible/project/roles/wordpress-block-xmlrpc/templates/.htaccess`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/wordpress-cli/tasks/main.yml` & `lampsible-1.1.0/src/lampsible/project/roles/wordpress-cli/tasks/main.yml`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   args:
     argv:
       - wp
       - core
       - download
       - --allow-root
       - --force
-      - "--path={{ wp_apache_document_root }}"
+      - "--path={{ apache_document_root }}"
       - "--locale={{ wordpress_locale }}"
       - "--version={{ wordpress_version }}"
 
 # https://developer.wordpress.org/cli/commands/config/create/
 - name: Create wp-config.php
   # TODO: We can add --dbcharset and --dbcollate.
   # TODO: Maybe parameterize the --force flag, to be on the safe side.
@@ -30,15 +30,15 @@
   args:
     argv:
       - wp
       - config
       - create
       - --allow-root
       - --force
-      - "--path={{ wp_apache_document_root }}"
+      - "--path={{ apache_document_root }}"
       - "--dbname={{ database_name }}"
       - "--dbuser={{ database_username }}"
       - "--dbpass={{ database_password }}"
       - "--dbhost={{ database_host }}"
       - "--dbprefix={{ database_table_prefix }}"
       - "--locale={{ wordpress_locale }}"
       - --extra-php
@@ -50,15 +50,15 @@
   command:
   args:
     argv:
       - wp
       - db
       - create
       - --allow-root
-      - "--path={{ wp_apache_document_root }}"
+      - "--path={{ apache_document_root }}"
       - "--dbname={{ database_name }}"
       - "--dbuser={{ database_username }}"
       - "--dbpass={{ database_password }}"
       - "--dbhost={{ database_host }}"
   ignore_errors: true
 
 # https://developer.wordpress.org/cli/commands/core/install/
@@ -66,30 +66,30 @@
   command:
   args:
     argv:
       - wp
       - core
       - install
       - --allow-root
-      - "--path={{ wp_apache_document_root }}"
+      - "--path={{ apache_document_root }}"
       - "--url={{ wordpress_url }}"
-      - "--title={{ wordpress_site_title }}"
-      - "--admin_user={{ wordpress_admin_username }}"
-      - "--admin_password={{ wordpress_admin_password }}"
-      - "--admin_email={{ wordpress_admin_email }}"
+      - "--title={{ site_title }}"
+      - "--admin_user={{ admin_username }}"
+      - "--admin_password={{ admin_password }}"
+      - "--admin_email={{ admin_email }}"
       - "--locale={{ wordpress_locale }}"
 
 - name: Set file ownership for WordPress directory
   file:
-    path: "{{ wp_apache_document_root }}"
+    path: "{{ apache_document_root }}"
     state: directory
     recurse: yes
     owner: nobody
     group: nogroup
 
 - name: Set file ownership for wp-content/
   file:
-    path: "{{ wp_apache_document_root }}/wp-content"
+    path: "{{ apache_document_root }}/wp-content"
     state: directory
     recurse: yes
     owner: www-data
     group: www-data
```

### Comparing `lampsible-1.0.0/src/lampsible/project/roles/wordpress-manual/tasks/main.yml` & `lampsible-1.1.0/src/lampsible/project/roles/wordpress-manual/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `lampsible-1.0.0/src/lampsible/project/wordpress.yml` & `lampsible-1.1.0/src/lampsible/project/wordpress.yml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 - hosts: all
   become: true
   gather_facts: true
   tasks:
     - include_role:
         name: "{{ item }}"
       loop:
-        - apt-update
+        - apt
         - apache2
         - php
         - pip
         - mysql
         - "{{ 'wordpress-manual' if wordpress_manual_install else 'wordpress-cli' }}"
 
     - include_role:
```

### Comparing `lampsible-1.0.0/src/lampsible.egg-info/PKG-INFO` & `lampsible-1.1.0/src/lampsible.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: lampsible
-Version: 1.0.0
+Version: 1.1.0
 Summary: Deploy and set up LAMP stacks with Ansible
 Author-email: "Brian St. Hilaire" <brian.st-hilaire@sanctus-tech.com>
 Project-URL: Homepage, https://github.com/saint-hilaire/lampsible
 Project-URL: Issues, https://github.com/saint-hilaire/lampsible/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ansible-core
 Requires-Dist: ansible-runner
-Requires-Dist: requests
+Requires-Dist: requests>=2.32.3
 Requires-Dist: fqdn
 
 # Lampsible
 
 ## About
 
 Lampsible - LAMP stacks with Ansible and a super simple CLI. This tool can automate anything from
@@ -58,27 +58,35 @@
 
 ```
 lampsible someuser@somehost.com wordpress \
     --ssl-certbot \
     --email-for-ssl you@yourdomain.com
 ```
 
+Install a production ready Joomla site:
+
+```
+lampsible someuser@somehost.com joomla \
+    --ssl-certbot \
+    --email-for-ssl you@yourdomain.com
+```
+
 Install a Laravel app on a test server:
 
 ```
 lampsible someuser@somehost.com laravel \
     --ssl-certbot \
     --test-cert \
     --apache-server-admin you@yourdomain.com \
     --app-name cool-laravel-app \
     --app-build-path /path/to/your/local/cool-laravel-app-0.7rc.tar.gz \
     --laravel-artisan-commands key:generate,migrate
 ```
 
-Set up a LAMP with various custom configuration and a self signed SSL certificate on some local VM:
+Set up a LAMP stack with various custom configuration and a self signed SSL certificate on some local VM:
 
 ```
 lampsible someuser@192.168.123.123 lamp-stack \
     --ask-remote-sudo \
     --ssl-selfsigned \
     --database-username dbuser \
     --database-name testdb \
@@ -89,8 +97,8 @@
 ```
 
 
 Run `lampsible --help` for a full list of options.
 
 ## Contributing 
 
-PLease do! I'd be more than happy to see Issues, Pull Requests and any other kind of feedback ;-)
+Please do! I'd be more than happy to see Issues, Pull Requests and any other kind of feedback ;-)
```

### Comparing `lampsible-1.0.0/src/lampsible.egg-info/SOURCES.txt` & `lampsible-1.1.0/src/lampsible.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,29 +10,31 @@
 src/lampsible.egg-info/SOURCES.txt
 src/lampsible.egg-info/dependency_links.txt
 src/lampsible.egg-info/entry_points.txt
 src/lampsible.egg-info/requires.txt
 src/lampsible.egg-info/top_level.txt
 src/lampsible/project/ansible-galaxy-requirements.yml
 src/lampsible/project/apache.yml
+src/lampsible/project/joomla.yml
 src/lampsible/project/lamp-stack.yml
 src/lampsible/project/laravel.yml
 src/lampsible/project/mysql.yml
 src/lampsible/project/php.yml
 src/lampsible/project/wordpress.yml
 src/lampsible/project/roles/apache-conf/tasks/main.yml
 src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2
 src/lampsible/project/roles/apache-vhosts/tasks/main.yml
 src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2
 src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2
 src/lampsible/project/roles/apache2/tasks/main.yml
-src/lampsible/project/roles/apt-update/tasks/main.yaml
+src/lampsible/project/roles/apt/tasks/main.yaml
 src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml
 src/lampsible/project/roles/fail2ban/tasks/main.yml
 src/lampsible/project/roles/fail2ban/templates/jail.local.j2
+src/lampsible/project/roles/joomla/tasks/main.yml
 src/lampsible/project/roles/laravel/tasks/main.yml
 src/lampsible/project/roles/laravel/templates/.env.j2
 src/lampsible/project/roles/mysql/tasks/main.yml
 src/lampsible/project/roles/php/tasks/main.yml
 src/lampsible/project/roles/phpmyadmin/tasks/main.yml
 src/lampsible/project/roles/phpmyadmin/templates/apache2.conf
 src/lampsible/project/roles/phpmyadmin/templates/php.ini
```

