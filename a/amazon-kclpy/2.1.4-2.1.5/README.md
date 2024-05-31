# Comparing `tmp/amazon_kclpy-2.1.4.tar.gz` & `tmp/amazon_kclpy-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_kclpy-2.1.4.tar", last modified: Wed Apr 24 23:20:02 2024, max compression
+gzip compressed data, was "amazon_kclpy-2.1.5.tar", last modified: Thu May 30 23:58:48 2024, max compression
```

## Comparing `amazon_kclpy-2.1.4.tar` & `amazon_kclpy-2.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/
--rw-r--r--   0 vvilo    (25800068) amazon     (100)    10142 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/LICENSE.txt
--rw-r--r--   0 vvilo    (25800068) amazon     (100)       72 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/MANIFEST.in
--rw-r--r--   0 vvilo    (25800068) amazon     (100)      114 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/NOTICE.txt
--rw-r--r--   0 vvilo    (25800068) amazon     (100)      351 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/PKG-INFO
--rw-r--r--   0 vvilo    (25800068) amazon     (100)    18562 2024-04-23 23:03:52.000000 amazon_kclpy-2.1.4/README.md
-drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy/
--rw-r--r--   0 vvilo    (25800068) amazon     (100)      827 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/__init__.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)      781 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/checkpoint_error.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     1839 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/dispatch.py
-drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy/jars/
--rw-r--r--   0 vvilo    (25800068) amazon     (100)        0 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/jars/__init__.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)    12498 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/kcl.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)    13819 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/messages.py
-drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy/v2/
--rw-r--r--   0 vvilo    (25800068) amazon     (100)      820 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/v2/__init__.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     5308 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/v2/processor.py
-drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy/v3/
--rw-r--r--   0 vvilo    (25800068) amazon     (100)      820 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/v3/__init__.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     5583 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/v3/processor.py
-drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/
--rw-r--r--   0 vvilo    (25800068) amazon     (100)      351 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/PKG-INFO
--rw-r--r--   0 vvilo    (25800068) amazon     (100)      776 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/SOURCES.txt
--rw-r--r--   0 vvilo    (25800068) amazon     (100)        1 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/dependency_links.txt
--rw-r--r--   0 vvilo    (25800068) amazon     (100)        1 2024-04-23 21:56:05.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/not-zip-safe
--rw-r--r--   0 vvilo    (25800068) amazon     (100)       14 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/requires.txt
--rw-r--r--   0 vvilo    (25800068) amazon     (100)       53 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/top_level.txt
--rw-r--r--   0 vvilo    (25800068) amazon     (100)    14133 2024-04-23 23:03:52.000000 amazon_kclpy-2.1.4/pom.xml
-drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/samples/
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     2741 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/__init__.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     7176 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/amazon_kclpy_helper.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     4755 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/sample.properties
--rwxr-xr-x   0 vvilo    (25800068) amazon     (100)     6915 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/sample_kclpy_app.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     5706 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/sample_kinesis_wordputter.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)      104 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/setup.cfg
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     8728 2024-04-23 23:03:52.000000 amazon_kclpy-2.1.4/setup.py
-drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/test/
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     3791 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/test/test_amazon_kclpy.py
--rw-r--r--   0 vvilo    (25800068) amazon     (100)     3926 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/test/test_amazon_kclpy_input_output_integration.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    10142 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/LICENSE.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)       72 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/MANIFEST.in
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      114 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/NOTICE.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      351 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/PKG-INFO
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    19193 2024-05-30 23:56:00.000000 amazon_kclpy-2.1.5/README.md
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/amazon_kclpy/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      827 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      781 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/checkpoint_error.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     1839 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/dispatch.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/amazon_kclpy/jars/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)        0 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/jars/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    12498 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/kcl.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    13819 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/messages.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/amazon_kclpy/v2/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      820 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/v2/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     5308 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/v2/processor.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/amazon_kclpy/v3/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      820 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/v3/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     5583 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/amazon_kclpy/v3/processor.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/amazon_kclpy.egg-info/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      351 2024-05-30 23:58:47.000000 amazon_kclpy-2.1.5/amazon_kclpy.egg-info/PKG-INFO
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      776 2024-05-30 23:58:47.000000 amazon_kclpy-2.1.5/amazon_kclpy.egg-info/SOURCES.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)        1 2024-05-30 23:58:47.000000 amazon_kclpy-2.1.5/amazon_kclpy.egg-info/dependency_links.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)        1 2024-04-23 21:56:05.000000 amazon_kclpy-2.1.5/amazon_kclpy.egg-info/not-zip-safe
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)       15 2024-05-30 23:58:47.000000 amazon_kclpy-2.1.5/amazon_kclpy.egg-info/requires.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)       53 2024-05-30 23:58:47.000000 amazon_kclpy-2.1.5/amazon_kclpy.egg-info/top_level.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    15271 2024-05-30 23:56:00.000000 amazon_kclpy-2.1.5/pom.xml
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/samples/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     2741 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/samples/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     7176 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/samples/amazon_kclpy_helper.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     4755 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/samples/sample.properties
+-rwxr-xr-x   0 vvilo    (25800068) amazon     (100)     6915 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/samples/sample_kclpy_app.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     5706 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/samples/sample_kinesis_wordputter.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      104 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/setup.cfg
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     8729 2024-05-30 23:56:00.000000 amazon_kclpy-2.1.5/setup.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-05-30 23:58:48.018028 amazon_kclpy-2.1.5/test/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     3791 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/test/test_amazon_kclpy.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     3926 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.5/test/test_amazon_kclpy_input_output_integration.py
```

### Comparing `amazon_kclpy-2.1.4/LICENSE.txt` & `amazon_kclpy-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/README.md` & `amazon_kclpy-2.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,21 @@
 * The [Amazon KCL for Java][kinesis-github]
 * The [Amazon KCL for Ruby][amazon-kinesis-ruby-github]
 * The [Amazon Kinesis Documentation][amazon-kinesis-docs]
 * The [Amazon Kinesis Forum][kinesis-forum]
 
 ## Release Notes
 
+### Release 2.1.5 (May 29, 2024)
+* Fixed CI due to different macOS architecture [PR #246](https://github.com/awslabs/amazon-kinesis-client-python/pull/246)
+* Added necessary Java SDKs to run sample [PR #248](https://github.com/awslabs/amazon-kinesis-client-python/pull/248)
+* Upgraded boto dependency to boto3 [PR #245](https://github.com/awslabs/amazon-kinesis-client-python/pull/245)
+* Upgraded AWS SDK from 2.19.2 to 2.25.11 [PR #248](https://github.com/awslabs/amazon-kinesis-client-python/pull/248)
+* Upgraded aws-java-sdk from 1.12.370 to 1.12.668 [PR #248](https://github.com/awslabs/amazon-kinesis-client-python/pull/248)
+
 ### Release 2.1.4 (April 23, 2024)
 * Upgraded KCL and KCL-Multilang dependencies from 2.5.2 to 2.5.8 [PR #239](https://github.com/awslabs/amazon-kinesis-client-python/pull/239)
 * Upgraded ion-java from 1.5.1 to 1.11.4 [PR #243](https://github.com/awslabs/amazon-kinesis-client-python/pull/243)
 * Upgraded logback version from 1.3.0 to 1.3.12 [PR #242](https://github.com/awslabs/amazon-kinesis-client-python/pull/242)
 * Upgraded io.netty dependency from 4.1.86.Final to 4.1.94.Final [PR #234](https://github.com/awslabs/amazon-kinesis-client-python/pull/234)
 * Upgraded Google Guava dependency from 32.0.0-jre to 32.1.1-jre [PR #234](https://github.com/awslabs/amazon-kinesis-client-python/pull/234)
 * Upgraded jackson-databind from 2.13.4 to 2.13.5 [PR #234](https://github.com/awslabs/amazon-kinesis-client-python/pull/234)
```

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy/__init__.py` & `amazon_kclpy-2.1.5/amazon_kclpy/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy/checkpoint_error.py` & `amazon_kclpy-2.1.5/amazon_kclpy/checkpoint_error.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy/dispatch.py` & `amazon_kclpy-2.1.5/amazon_kclpy/dispatch.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy/kcl.py` & `amazon_kclpy-2.1.5/amazon_kclpy/kcl.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy/messages.py` & `amazon_kclpy-2.1.5/amazon_kclpy/messages.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy/v2/__init__.py` & `amazon_kclpy-2.1.5/amazon_kclpy/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy/v2/processor.py` & `amazon_kclpy-2.1.5/amazon_kclpy/v2/processor.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy/v3/__init__.py` & `amazon_kclpy-2.1.5/amazon_kclpy/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy/v3/processor.py` & `amazon_kclpy-2.1.5/amazon_kclpy/v3/processor.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/amazon_kclpy.egg-info/SOURCES.txt` & `amazon_kclpy-2.1.5/amazon_kclpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/pom.xml` & `amazon_kclpy-2.1.5/pom.xml`

 * *Files 2% similar despite different names*

#### Comparing `amazon_kclpy-2.1.4/pom.xml` & `amazon_kclpy-2.1.5/pom.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <properties>
-    <awssdk.version>2.19.2</awssdk.version>
-    <aws-java-sdk.version>1.12.370</aws-java-sdk.version>
+    <awssdk.version>2.25.11</awssdk.version>
+    <aws-java-sdk.version>1.12.668</aws-java-sdk.version>
     <kcl.version>2.5.8</kcl.version>
     <netty.version>4.1.108.Final</netty.version>
     <netty-reactive.version>2.0.6</netty-reactive.version>
     <fasterxml-jackson.version>2.13.5</fasterxml-jackson.version>
     <logback.version>1.3.12</logback.version>
   </properties>
   <dependencies>
@@ -138,14 +138,44 @@
     </dependency>
     <dependency>
       <groupId>software.amazon.awssdk</groupId>
       <artifactId>arns</artifactId>
       <version>${awssdk.version}</version>
     </dependency>
     <dependency>
+      <groupId>software.amazon.awssdk</groupId>
+      <artifactId>http-auth-spi</artifactId>
+      <version>${awssdk.version}</version>
+    </dependency>
+    <dependency>
+      <groupId>software.amazon.awssdk</groupId>
+      <artifactId>http-auth</artifactId>
+      <version>${awssdk.version}</version>
+    </dependency>
+    <dependency>
+      <groupId>software.amazon.awssdk</groupId>
+      <artifactId>http-auth-aws</artifactId>
+      <version>${awssdk.version}</version>
+    </dependency>
+    <dependency>
+      <groupId>software.amazon.awssdk</groupId>
+      <artifactId>checksums-spi</artifactId>
+      <version>${awssdk.version}</version>
+    </dependency>
+    <dependency>
+      <groupId>software.amazon.awssdk</groupId>
+      <artifactId>checksums</artifactId>
+      <version>${awssdk.version}</version>
+    </dependency>
+    <dependency>
+      <groupId>software.amazon.awssdk</groupId>
+      <artifactId>identity-spi</artifactId>
+      <version>${awssdk.version}</version>
+    </dependency>
+    <dependency>
       <groupId>io.netty</groupId>
       <artifactId>netty-codec-http</artifactId>
       <version>${netty.version}</version>
     </dependency>
     <dependency>
       <groupId>io.netty</groupId>
       <artifactId>netty-codec-http2</artifactId>
```

### Comparing `amazon_kclpy-2.1.4/samples/__init__.py` & `amazon_kclpy-2.1.5/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/samples/amazon_kclpy_helper.py` & `amazon_kclpy-2.1.5/samples/amazon_kclpy_helper.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/samples/sample.properties` & `amazon_kclpy-2.1.5/samples/sample.properties`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/samples/sample_kclpy_app.py` & `amazon_kclpy-2.1.5/samples/sample_kclpy_app.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/samples/sample_kinesis_wordputter.py` & `amazon_kclpy-2.1.5/samples/sample_kinesis_wordputter.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/setup.py` & `amazon_kclpy-2.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 #
 # Will retrieve the configured jars from maven and then advise the user
 # to rerun the install command.
 #
 
 PACKAGE_NAME = 'amazon_kclpy'
 JAR_DIRECTORY = os.path.join(PACKAGE_NAME, 'jars')
-PACKAGE_VERSION = '2.1.4'
+PACKAGE_VERSION = '2.1.5'
 PYTHON_REQUIREMENTS = [
-    'boto',
+    'boto3',
     # argparse is part of python2.7 but must be declared for python2.6
     'argparse',
 ]
 REMOTE_MAVEN_PACKAGES_FILE = 'pom.xml'
 
 class MavenJarDownloader:
```

### Comparing `amazon_kclpy-2.1.4/test/test_amazon_kclpy.py` & `amazon_kclpy-2.1.5/test/test_amazon_kclpy.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.4/test/test_amazon_kclpy_input_output_integration.py` & `amazon_kclpy-2.1.5/test/test_amazon_kclpy_input_output_integration.py`

 * *Files identical despite different names*

