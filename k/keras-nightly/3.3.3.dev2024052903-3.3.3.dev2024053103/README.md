# Comparing `tmp/keras_nightly-3.3.3.dev2024052903.tar.gz` & `tmp/keras_nightly-3.3.3.dev2024053103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.3.dev2024052903.tar", last modified: Wed May 29 03:22:41 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.3.dev2024053103.tar", last modified: Fri May 31 03:22:02 2024, max compression
```

## Comparing `keras_nightly-3.3.3.dev2024052903.tar` & `keras_nightly-3.3.3.dev2024053103.tar`

### file list

```diff
@@ -1,698 +1,698 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.200194 keras_nightly-3.3.3.dev2024052903/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-29 03:22:41.200194 keras_nightly-3.3.3.dev2024052903/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.112193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.116193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.120193 keras_nightly-3.3.3.dev2024052903/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-29 03:22:36.000000 keras_nightly-3.3.3.dev2024052903/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.124193 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.128193 keras_nightly-3.3.3.dev2024052903/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.132193 keras_nightly-3.3.3.dev2024052903/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.136193 keras_nightly-3.3.3.dev2024052903/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16902 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25341 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40735 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15581 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23651 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30917 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.136193 keras_nightly-3.3.3.dev2024052903/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.136193 keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.140193 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    31232 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.140193 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.144193 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    28526 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    78825 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.148193 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17887 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    27152 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    48087 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.148193 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.152193 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.152193 keras_nightly-3.3.3.dev2024052903/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.152193 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.152193 keras_nightly-3.3.3.dev2024052903/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.152193 keras_nightly-3.3.3.dev2024052903/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.152193 keras_nightly-3.3.3.dev2024052903/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33373 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.156193 keras_nightly-3.3.3.dev2024052903/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.156193 keras_nightly-3.3.3.dev2024052903/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.156193 keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.156193 keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    28502 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.160194 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.160194 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    42056 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    64242 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.164193 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.164193 keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.164193 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.168193 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41996 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17745 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.172194 keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.172194 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.176194 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.176194 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.176194 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.176194 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.180194 keras_nightly-3.3.3.dev2024052903/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    70024 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.180194 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61530 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.180194 keras_nightly-3.3.3.dev2024052903/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    30043 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22783 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.184194 keras_nightly-3.3.3.dev2024052903/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27019 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    37642 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    21256 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   196613 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.184194 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.188194 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.188194 keras_nightly-3.3.3.dev2024052903/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.188194 keras_nightly-3.3.3.dev2024052903/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.188194 keras_nightly-3.3.3.dev2024052903/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.188194 keras_nightly-3.3.3.dev2024052903/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/saving/keras_saveable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.188194 keras_nightly-3.3.3.dev2024052903/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.188194 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.192194 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.192194 keras_nightly-3.3.3.dev2024052903/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/tree/tree_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.196194 keras_nightly-3.3.3.dev2024052903/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-29 03:21:17.000000 keras_nightly-3.3.3.dev2024052903/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-29 03:22:39.000000 keras_nightly-3.3.3.dev2024052903/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:22:41.196194 keras_nightly-3.3.3.dev2024052903/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-29 03:22:41.000000 keras_nightly-3.3.3.dev2024052903/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-29 03:22:41.000000 keras_nightly-3.3.3.dev2024052903/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:22:41.000000 keras_nightly-3.3.3.dev2024052903/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-29 03:22:41.000000 keras_nightly-3.3.3.dev2024052903/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 03:22:41.000000 keras_nightly-3.3.3.dev2024052903/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:22:41.200194 keras_nightly-3.3.3.dev2024052903/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-29 03:22:39.000000 keras_nightly-3.3.3.dev2024052903/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.684319 keras_nightly-3.3.3.dev2024053103/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-31 03:22:02.684319 keras_nightly-3.3.3.dev2024053103/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.580319 keras_nightly-3.3.3.dev2024053103/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.580319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.580319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.580319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.580319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.584319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.588319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-31 03:21:57.000000 keras_nightly-3.3.3.dev2024053103/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.592319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.596319 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.600319 keras_nightly-3.3.3.dev2024053103/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.604319 keras_nightly-3.3.3.dev2024053103/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.608319 keras_nightly-3.3.3.dev2024053103/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16902 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25341 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40735 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15581 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23651 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30917 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.608319 keras_nightly-3.3.3.dev2024053103/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.612319 keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.612319 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15500 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31232 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.616319 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13818 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.620319 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28526 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78854 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.620319 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17887 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27152 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48087 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.624319 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.624319 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.628319 keras_nightly-3.3.3.dev2024053103/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.628319 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.628319 keras_nightly-3.3.3.dev2024053103/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.628319 keras_nightly-3.3.3.dev2024053103/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.628319 keras_nightly-3.3.3.dev2024053103/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33373 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.628319 keras_nightly-3.3.3.dev2024053103/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.632319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.632319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.632319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28502 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.636319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.636319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42056 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64242 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.640319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.640319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.644319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.648319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29986 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41996 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14668 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17745 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.648319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.652319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.656319 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.656319 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.656319 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.656319 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.660319 keras_nightly-3.3.3.dev2024053103/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70024 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.660319 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61530 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.660319 keras_nightly-3.3.3.dev2024053103/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30043 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22783 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.664319 keras_nightly-3.3.3.dev2024053103/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27019 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37793 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21256 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196613 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.668319 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.668319 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.668319 keras_nightly-3.3.3.dev2024053103/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.668319 keras_nightly-3.3.3.dev2024053103/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.668319 keras_nightly-3.3.3.dev2024053103/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.672319 keras_nightly-3.3.3.dev2024053103/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/saving/keras_saveable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.672319 keras_nightly-3.3.3.dev2024053103/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.672319 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.676319 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.676319 keras_nightly-3.3.3.dev2024053103/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/tree/tree_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.680319 keras_nightly-3.3.3.dev2024053103/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-31 03:20:42.000000 keras_nightly-3.3.3.dev2024053103/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-31 03:22:00.000000 keras_nightly-3.3.3.dev2024053103/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:22:02.680319 keras_nightly-3.3.3.dev2024053103/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-31 03:22:02.000000 keras_nightly-3.3.3.dev2024053103/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-31 03:22:02.000000 keras_nightly-3.3.3.dev2024053103/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:22:02.000000 keras_nightly-3.3.3.dev2024053103/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-31 03:22:02.000000 keras_nightly-3.3.3.dev2024053103/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 03:22:02.000000 keras_nightly-3.3.3.dev2024053103/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:22:02.684319 keras_nightly-3.3.3.dev2024053103/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-31 03:22:00.000000 keras_nightly-3.3.3.dev2024053103/setup.py
```

### Comparing `keras_nightly-3.3.3.dev2024052903/PKG-INFO` & `keras_nightly-3.3.3.dev2024053103/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024052903
+Version: 3.3.3.dev2024053103
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024052903/README.md` & `keras_nightly-3.3.3.dev2024053103/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/activations/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/applications/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/backend/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/config/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/layers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/losses/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/ops/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/random/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/saving/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/tree/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/api/utils/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/activations/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/activations/activations.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/api_export.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/convnext.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/densenet.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/nasnet.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/resnet.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/vgg16.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/vgg19.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/applications/xception.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/common/variables.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/config.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/exports.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/core.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/image.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import functools
-
 import jax
-import jax.numpy as jnp
+import numpy as np
 
-from keras.src.backend.jax.core import convert_to_tensor
+from keras.src import backend
+from keras.src.backend.numpy.core import convert_to_tensor
+from keras.src.utils.module_utils import scipy
 
 RESIZE_INTERPOLATIONS = (
     "bilinear",
     "nearest",
     "lanczos3",
     "lanczos5",
     "bicubic",
 )
 
 
-def rgb_to_grayscale(image, data_format="channels_last"):
-    if data_format == "channels_first":
-        if len(image.shape) == 4:
-            image = jnp.transpose(image, (0, 2, 3, 1))
-        elif len(image.shape) == 3:
-            image = jnp.transpose(image, (1, 2, 0))
-        else:
-            raise ValueError(
-                "Invalid input rank: expected rank 3 (single image) "
-                "or rank 4 (batch of images). Received input with shape: "
-                f"image.shape={image.shape}"
-            )
-    red, green, blue = image[..., 0], image[..., 1], image[..., 2]
-    grayscale_image = 0.2989 * red + 0.5870 * green + 0.1140 * blue
-    grayscale_image = jnp.expand_dims(grayscale_image, axis=-1)
-    if data_format == "channels_first":
-        if len(image.shape) == 4:
-            grayscale_image = jnp.transpose(grayscale_image, (0, 3, 1, 2))
-        elif len(image.shape) == 3:
-            grayscale_image = jnp.transpose(grayscale_image, (2, 0, 1))
-    return jnp.array(grayscale_image)
+def rgb_to_grayscale(images, data_format=None):
+    images = convert_to_tensor(images)
+    data_format = backend.standardize_data_format(data_format)
+    channels_axis = -1 if data_format == "channels_last" else -3
+    if len(images.shape) not in (3, 4):
+        raise ValueError(
+            "Invalid images rank: expected rank 3 (single image) "
+            "or rank 4 (batch of images). Received input with shape: "
+            f"images.shape={images.shape}"
+        )
+    # Convert to floats
+    original_dtype = images.dtype
+    compute_dtype = backend.result_type(images.dtype, float)
+    images = images.astype(compute_dtype)
+
+    # Ref: tf.image.rgb_to_grayscale
+    rgb_weights = np.array([0.2989, 0.5870, 0.1140], dtype=images.dtype)
+    grayscales = np.tensordot(images, rgb_weights, axes=(channels_axis, -1))
+    grayscales = np.expand_dims(grayscales, axis=channels_axis)
+    return grayscales.astype(original_dtype)
 
 
 def resize(
-    image,
+    images,
     size,
     interpolation="bilinear",
     antialias=False,
     crop_to_aspect_ratio=False,
     pad_to_aspect_ratio=False,
     fill_mode="constant",
     fill_value=0.0,
-    data_format="channels_last",
+    data_format=None,
 ):
+    data_format = backend.standardize_data_format(data_format)
     if interpolation not in RESIZE_INTERPOLATIONS:
         raise ValueError(
             "Invalid value for argument `interpolation`. Expected of one "
             f"{RESIZE_INTERPOLATIONS}. Received: interpolation={interpolation}"
         )
     if fill_mode != "constant":
         raise ValueError(
@@ -66,219 +66,156 @@
     if not len(size) == 2:
         raise ValueError(
             "Argument `size` must be a tuple of two elements "
             f"(height, width). Received: size={size}"
         )
     size = tuple(size)
     target_height, target_width = size
-    if len(image.shape) == 4:
+    if len(images.shape) == 4:
         if data_format == "channels_last":
-            size = (image.shape[0],) + size + (image.shape[-1],)
+            size = (images.shape[0],) + size + (images.shape[-1],)
         else:
-            size = (image.shape[0], image.shape[1]) + size
-        batch_size = image.shape[0]
-    elif len(image.shape) == 3:
+            size = (images.shape[0], images.shape[1]) + size
+    elif len(images.shape) == 3:
         if data_format == "channels_last":
-            size = size + (image.shape[-1],)
+            size = size + (images.shape[-1],)
         else:
-            size = (image.shape[0],) + size
+            size = (images.shape[0],) + size
     else:
         raise ValueError(
-            "Invalid input rank: expected rank 3 (single image) "
+            "Invalid images rank: expected rank 3 (single image) "
             "or rank 4 (batch of images). Received input with shape: "
-            f"image.shape={image.shape}"
+            f"images.shape={images.shape}"
         )
 
     if crop_to_aspect_ratio:
-        shape = image.shape
+        shape = images.shape
         if data_format == "channels_last":
             height, width = shape[-3], shape[-2]
         else:
             height, width = shape[-2], shape[-1]
         crop_height = int(float(width * target_height) / target_width)
         crop_height = min(height, crop_height)
         crop_width = int(float(height * target_width) / target_height)
         crop_width = min(width, crop_width)
         crop_box_hstart = int(float(height - crop_height) / 2)
         crop_box_wstart = int(float(width - crop_width) / 2)
         if data_format == "channels_last":
-            if len(image.shape) == 4:
-                image = image[
+            if len(images.shape) == 4:
+                images = images[
                     :,
                     crop_box_hstart : crop_box_hstart + crop_height,
                     crop_box_wstart : crop_box_wstart + crop_width,
                     :,
                 ]
             else:
-                image = image[
+                images = images[
                     crop_box_hstart : crop_box_hstart + crop_height,
                     crop_box_wstart : crop_box_wstart + crop_width,
                     :,
                 ]
         else:
-            if len(image.shape) == 4:
-                image = image[
+            if len(images.shape) == 4:
+                images = images[
                     :,
                     :,
                     crop_box_hstart : crop_box_hstart + crop_height,
                     crop_box_wstart : crop_box_wstart + crop_width,
                 ]
             else:
-                image = image[
+                images = images[
                     :,
                     crop_box_hstart : crop_box_hstart + crop_height,
                     crop_box_wstart : crop_box_wstart + crop_width,
                 ]
     elif pad_to_aspect_ratio:
-        shape = image.shape
+        shape = images.shape
+        batch_size = images.shape[0]
         if data_format == "channels_last":
             height, width, channels = shape[-3], shape[-2], shape[-1]
         else:
-            height, width, channels = shape[-2], shape[-1], shape[-3]
-
+            channels, height, width = shape[-3], shape[-2], shape[-1]
         pad_height = int(float(width * target_height) / target_width)
         pad_height = max(height, pad_height)
         pad_width = int(float(height * target_width) / target_height)
         pad_width = max(width, pad_width)
         img_box_hstart = int(float(pad_height - height) / 2)
         img_box_wstart = int(float(pad_width - width) / 2)
         if data_format == "channels_last":
-            if img_box_hstart > 0:
-                if len(image.shape) == 4:
-                    padded_img = jnp.concatenate(
-                        [
-                            jnp.ones(
-                                (batch_size, img_box_hstart, width, channels),
-                                dtype=image.dtype,
-                            )
-                            * fill_value,
-                            image,
-                            jnp.ones(
-                                (batch_size, img_box_hstart, width, channels),
-                                dtype=image.dtype,
-                            )
-                            * fill_value,
-                        ],
-                        axis=1,
-                    )
-                else:
-                    padded_img = jnp.concatenate(
-                        [
-                            jnp.ones(
-                                (img_box_hstart, width, channels),
-                                dtype=image.dtype,
-                            )
-                            * fill_value,
-                            image,
-                            jnp.ones(
-                                (img_box_hstart, width, channels),
-                                dtype=image.dtype,
-                            )
-                            * fill_value,
-                        ],
-                        axis=0,
-                    )
-            elif img_box_wstart > 0:
-                if len(image.shape) == 4:
-                    padded_img = jnp.concatenate(
-                        [
-                            jnp.ones(
-                                (batch_size, height, img_box_wstart, channels),
-                                dtype=image.dtype,
-                            )
-                            * fill_value,
-                            image,
-                            jnp.ones(
-                                (batch_size, height, img_box_wstart, channels),
-                                dtype=image.dtype,
-                            )
-                            * fill_value,
-                        ],
-                        axis=2,
-                    )
-                else:
-                    padded_img = jnp.concatenate(
-                        [
-                            jnp.ones(
-                                (height, img_box_wstart, channels),
-                                dtype=image.dtype,
-                            )
-                            * fill_value,
-                            image,
-                            jnp.ones(
-                                (height, img_box_wstart, channels),
-                                dtype=image.dtype,
-                            )
-                            * fill_value,
-                        ],
-                        axis=1,
+            if len(images.shape) == 4:
+                padded_img = (
+                    np.ones(
+                        (
+                            batch_size,
+                            pad_height + height,
+                            pad_width + width,
+                            channels,
+                        ),
+                        dtype=images.dtype,
                     )
+                    * fill_value
+                )
+                padded_img[
+                    :,
+                    img_box_hstart : img_box_hstart + height,
+                    img_box_wstart : img_box_wstart + width,
+                    :,
+                ] = images
             else:
-                padded_img = image
-        else:
-            if img_box_hstart > 0:
-                if len(image.shape) == 4:
-                    padded_img = jnp.concatenate(
-                        [
-                            jnp.ones(
-                                (batch_size, channels, img_box_hstart, width)
-                            )
-                            * fill_value,
-                            image,
-                            jnp.ones(
-                                (batch_size, channels, img_box_hstart, width)
-                            )
-                            * fill_value,
-                        ],
-                        axis=2,
-                    )
-                else:
-                    padded_img = jnp.concatenate(
-                        [
-                            jnp.ones((channels, img_box_hstart, width))
-                            * fill_value,
-                            image,
-                            jnp.ones((channels, img_box_hstart, width))
-                            * fill_value,
-                        ],
-                        axis=1,
-                    )
-            elif img_box_wstart > 0:
-                if len(image.shape) == 4:
-                    padded_img = jnp.concatenate(
-                        [
-                            jnp.ones(
-                                (batch_size, channels, height, img_box_wstart)
-                            )
-                            * fill_value,
-                            image,
-                            jnp.ones(
-                                (batch_size, channels, height, img_box_wstart)
-                            )
-                            * fill_value,
-                        ],
-                        axis=3,
+                padded_img = (
+                    np.ones(
+                        (pad_height + height, pad_width + width, channels),
+                        dtype=images.dtype,
                     )
-                else:
-                    padded_img = jnp.concatenate(
-                        [
-                            jnp.ones((channels, height, img_box_wstart))
-                            * fill_value,
-                            image,
-                            jnp.ones((channels, height, img_box_wstart))
-                            * fill_value,
-                        ],
-                        axis=2,
+                    * fill_value
+                )
+                padded_img[
+                    img_box_hstart : img_box_hstart + height,
+                    img_box_wstart : img_box_wstart + width,
+                    :,
+                ] = images
+        else:
+            if len(images.shape) == 4:
+                padded_img = (
+                    np.ones(
+                        (
+                            batch_size,
+                            channels,
+                            pad_height + height,
+                            pad_width + width,
+                        ),
+                        dtype=images.dtype,
                     )
+                    * fill_value
+                )
+                padded_img[
+                    :,
+                    :,
+                    img_box_hstart : img_box_hstart + height,
+                    img_box_wstart : img_box_wstart + width,
+                ] = images
             else:
-                padded_img = image
-        image = padded_img
-
-    return jax.image.resize(
-        image, size, method=interpolation, antialias=antialias
+                padded_img = (
+                    np.ones(
+                        (channels, pad_height + height, pad_width + width),
+                        dtype=images.dtype,
+                    )
+                    * fill_value
+                )
+                padded_img[
+                    :,
+                    img_box_hstart : img_box_hstart + height,
+                    img_box_wstart : img_box_wstart + width,
+                ] = images
+        images = padded_img
+
+    return np.array(
+        jax.image.resize(
+            images, size, method=interpolation, antialias=antialias
+        )
     )
 
 
 AFFINE_TRANSFORM_INTERPOLATIONS = {  # map to order
     "nearest": 0,
     "bilinear": 1,
 }
@@ -288,129 +225,179 @@
     "wrap",
     "mirror",
     "reflect",
 }
 
 
 def affine_transform(
-    image,
+    images,
     transform,
     interpolation="bilinear",
     fill_mode="constant",
     fill_value=0,
-    data_format="channels_last",
+    data_format=None,
 ):
+    data_format = backend.standardize_data_format(data_format)
     if interpolation not in AFFINE_TRANSFORM_INTERPOLATIONS.keys():
         raise ValueError(
             "Invalid value for argument `interpolation`. Expected of one "
             f"{set(AFFINE_TRANSFORM_INTERPOLATIONS.keys())}. Received: "
             f"interpolation={interpolation}"
         )
     if fill_mode not in AFFINE_TRANSFORM_FILL_MODES:
         raise ValueError(
             "Invalid value for argument `fill_mode`. Expected of one "
             f"{AFFINE_TRANSFORM_FILL_MODES}. Received: fill_mode={fill_mode}"
         )
 
     transform = convert_to_tensor(transform)
 
-    if len(image.shape) not in (3, 4):
+    if len(images.shape) not in (3, 4):
         raise ValueError(
-            "Invalid image rank: expected rank 3 (single image) "
+            "Invalid images rank: expected rank 3 (single image) "
             "or rank 4 (batch of images). Received input with shape: "
-            f"image.shape={image.shape}"
+            f"images.shape={images.shape}"
         )
     if len(transform.shape) not in (1, 2):
         raise ValueError(
             "Invalid transform rank: expected rank 1 (single transform) "
             "or rank 2 (batch of transforms). Received input with shape: "
             f"transform.shape={transform.shape}"
         )
 
+    # scipy.ndimage.map_coordinates lacks support for half precision.
+    input_dtype = images.dtype
+    if input_dtype == "float16":
+        images = images.astype("float32")
+
     # unbatched case
     need_squeeze = False
-    if len(image.shape) == 3:
-        image = jnp.expand_dims(image, axis=0)
+    if len(images.shape) == 3:
+        images = np.expand_dims(images, axis=0)
         need_squeeze = True
     if len(transform.shape) == 1:
-        transform = jnp.expand_dims(transform, axis=0)
+        transform = np.expand_dims(transform, axis=0)
 
     if data_format == "channels_first":
-        image = jnp.transpose(image, (0, 2, 3, 1))
+        images = np.transpose(images, (0, 2, 3, 1))
 
-    batch_size = image.shape[0]
+    batch_size = images.shape[0]
 
     # get indices
-    meshgrid = jnp.meshgrid(
-        *[jnp.arange(size) for size in image.shape[1:]], indexing="ij"
+    meshgrid = np.meshgrid(
+        *[np.arange(size) for size in images.shape[1:]], indexing="ij"
     )
-    indices = jnp.concatenate(
-        [jnp.expand_dims(x, axis=-1) for x in meshgrid], axis=-1
+    indices = np.concatenate(
+        [np.expand_dims(x, axis=-1) for x in meshgrid], axis=-1
     )
-    indices = jnp.tile(indices, (batch_size, 1, 1, 1, 1))
+    indices = np.tile(indices, (batch_size, 1, 1, 1, 1))
 
     # swap the values
-    a0 = transform[:, 0]
-    a2 = transform[:, 2]
-    b1 = transform[:, 4]
-    b2 = transform[:, 5]
-    transform = transform.at[:, 0].set(b1)
-    transform = transform.at[:, 2].set(b2)
-    transform = transform.at[:, 4].set(a0)
-    transform = transform.at[:, 5].set(a2)
+    a0 = transform[:, 0].copy()
+    a2 = transform[:, 2].copy()
+    b1 = transform[:, 4].copy()
+    b2 = transform[:, 5].copy()
+    transform[:, 0] = b1
+    transform[:, 2] = b2
+    transform[:, 4] = a0
+    transform[:, 5] = a2
 
     # deal with transform
-    transform = jnp.pad(
-        transform, pad_width=[[0, 0], [0, 1]], constant_values=1
-    )
-    transform = jnp.reshape(transform, (batch_size, 3, 3))
-    offset = transform[:, 0:2, 2]
-    offset = jnp.pad(offset, pad_width=[[0, 0], [0, 1]])
-    transform = transform.at[:, 0:2, 2].set(0)
+    transform = np.pad(transform, pad_width=[[0, 0], [0, 1]], constant_values=1)
+    transform = np.reshape(transform, (batch_size, 3, 3))
+    offset = transform[:, 0:2, 2].copy()
+    offset = np.pad(offset, pad_width=[[0, 0], [0, 1]])
+    transform[:, 0:2, 2] = 0
 
     # transform the indices
-    coordinates = jnp.einsum("Bhwij, Bjk -> Bhwik", indices, transform)
-    coordinates = jnp.moveaxis(coordinates, source=-1, destination=1)
-    coordinates += jnp.reshape(a=offset, newshape=(*offset.shape, 1, 1, 1))
+    coordinates = np.einsum("Bhwij, Bjk -> Bhwik", indices, transform)
+    coordinates = np.moveaxis(coordinates, source=-1, destination=1)
+    coordinates += np.reshape(a=offset, newshape=(*offset.shape, 1, 1, 1))
 
     # apply affine transformation
-    _map_coordinates = functools.partial(
-        jax.scipy.ndimage.map_coordinates,
-        order=AFFINE_TRANSFORM_INTERPOLATIONS[interpolation],
-        mode=fill_mode,
-        cval=fill_value,
+    affined = np.stack(
+        [
+            map_coordinates(
+                images[i],
+                coordinates[i],
+                order=AFFINE_TRANSFORM_INTERPOLATIONS[interpolation],
+                fill_mode=fill_mode,
+                fill_value=fill_value,
+            )
+            for i in range(batch_size)
+        ],
+        axis=0,
     )
-    affined = jax.vmap(_map_coordinates)(image, coordinates)
 
     if data_format == "channels_first":
-        affined = jnp.transpose(affined, (0, 3, 1, 2))
+        affined = np.transpose(affined, (0, 3, 1, 2))
     if need_squeeze:
-        affined = jnp.squeeze(affined, axis=0)
+        affined = np.squeeze(affined, axis=0)
+    if input_dtype == "float16":
+        affined = affined.astype(input_dtype)
     return affined
 
 
 MAP_COORDINATES_FILL_MODES = {
     "constant",
     "nearest",
     "wrap",
     "mirror",
     "reflect",
 }
 
 
 def map_coordinates(
-    input, coordinates, order, fill_mode="constant", fill_value=0.0
+    inputs, coordinates, order, fill_mode="constant", fill_value=0.0
 ):
+    inputs = convert_to_tensor(inputs)
+    coordinates = convert_to_tensor(coordinates)
+    if coordinates.shape[0] != len(inputs.shape):
+        raise ValueError(
+            "First dim of `coordinates` must be the same as the rank of "
+            "`inputs`. "
+            f"Received inputs with shape: {inputs.shape} and coordinate "
+            f"leading dim of {coordinates.shape[0]}"
+        )
+    if len(coordinates.shape) < 2:
+        raise ValueError(
+            "Invalid coordinates rank: expected at least rank 2."
+            f" Received input with shape: {coordinates.shape}"
+        )
     if fill_mode not in MAP_COORDINATES_FILL_MODES:
         raise ValueError(
             "Invalid value for argument `fill_mode`. Expected one of "
-            f"{set(MAP_COORDINATES_FILL_MODES)}. Received: "
+            f"{set(MAP_COORDINATES_FILL_MODES.keys())}. Received: "
             f"fill_mode={fill_mode}"
         )
     if order not in range(2):
         raise ValueError(
             "Invalid value for argument `order`. Expected one of "
             f"{[0, 1]}. Received: order={order}"
         )
-    return jax.scipy.ndimage.map_coordinates(
-        input, coordinates, order, fill_mode, fill_value
+    # SciPy's implementation of map_coordinates handles boundaries incorrectly,
+    # unless mode='reflect'. For order=1, this only affects interpolation
+    # outside the bounds of the original array.
+    # https://github.com/scipy/scipy/issues/2640
+    padding = [
+        (
+            max(-np.floor(c.min()).astype(int) + 1, 0),
+            max(np.ceil(c.max()).astype(int) + 1 - size, 0),
+        )
+        for c, size in zip(coordinates, inputs.shape)
+    ]
+    shifted_coords = [c + p[0] for p, c in zip(padding, coordinates)]
+    pad_mode = {
+        "nearest": "edge",
+        "mirror": "reflect",
+        "reflect": "symmetric",
+    }.get(fill_mode, fill_mode)
+    if fill_mode == "constant":
+        padded = np.pad(
+            inputs, padding, mode=pad_mode, constant_values=fill_value
+        )
+    else:
+        padded = np.pad(inputs, padding, mode=pad_mode)
+    result = scipy.ndimage.map_coordinates(
+        padded, shifted_coords, order=order, mode=fill_mode, cval=fill_value
     )
+    return result
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/math.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/random.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,73 @@
-import jax
-import numpy as np
+import functools
+import itertools
+import operator
 
-from keras.src.backend.numpy.core import convert_to_tensor
-from keras.src.utils.module_utils import scipy
+import torch
 
-RESIZE_INTERPOLATIONS = (
-    "bilinear",
-    "nearest",
+from keras.src import backend
+from keras.src.backend.torch.core import convert_to_tensor
+from keras.src.utils.module_utils import torchvision
+
+RESIZE_INTERPOLATIONS = {}  # populated after torchvision import
+
+UNSUPPORTED_INTERPOLATIONS = (
     "lanczos3",
     "lanczos5",
-    "bicubic",
 )
 
 
-def rgb_to_grayscale(image, data_format="channels_last"):
-    if data_format == "channels_first":
-        if len(image.shape) == 4:
-            image = np.transpose(image, (0, 2, 3, 1))
-        elif len(image.shape) == 3:
-            image = np.transpose(image, (1, 2, 0))
+def rgb_to_grayscale(images, data_format=None):
+    images = convert_to_tensor(images)
+    data_format = backend.standardize_data_format(data_format)
+    if data_format == "channels_last":
+        if images.ndim == 4:
+            images = images.permute((0, 3, 1, 2))
+        elif images.ndim == 3:
+            images = images.permute((2, 0, 1))
         else:
             raise ValueError(
-                "Invalid input rank: expected rank 3 (single image) "
+                "Invalid images rank: expected rank 3 (single image) "
                 "or rank 4 (batch of images). Received input with shape: "
-                f"image.shape={image.shape}"
+                f"images.shape={images.shape}"
             )
-    red, green, blue = image[..., 0], image[..., 1], image[..., 2]
-    grayscale_image = 0.2989 * red + 0.5870 * green + 0.1140 * blue
-    grayscale_image = np.expand_dims(grayscale_image, axis=-1)
-    if data_format == "channels_first":
-        if len(image.shape) == 4:
-            grayscale_image = np.transpose(grayscale_image, (0, 3, 1, 2))
-        elif len(image.shape) == 3:
-            grayscale_image = np.transpose(grayscale_image, (2, 0, 1))
-    return np.array(grayscale_image)
+    images = torchvision.transforms.functional.rgb_to_grayscale(img=images)
+    if data_format == "channels_last":
+        if len(images.shape) == 4:
+            images = images.permute((0, 2, 3, 1))
+        elif len(images.shape) == 3:
+            images = images.permute((1, 2, 0))
+    return images
 
 
 def resize(
-    image,
+    images,
     size,
     interpolation="bilinear",
     antialias=False,
     crop_to_aspect_ratio=False,
     pad_to_aspect_ratio=False,
     fill_mode="constant",
     fill_value=0.0,
-    data_format="channels_last",
+    data_format=None,
 ):
+    data_format = backend.standardize_data_format(data_format)
+    RESIZE_INTERPOLATIONS.update(
+        {
+            "bilinear": torchvision.transforms.InterpolationMode.BILINEAR,
+            "nearest": torchvision.transforms.InterpolationMode.NEAREST_EXACT,
+            "bicubic": torchvision.transforms.InterpolationMode.BICUBIC,
+        }
+    )
+    if interpolation in UNSUPPORTED_INTERPOLATIONS:
+        raise ValueError(
+            "Resizing with Lanczos interpolation is "
+            "not supported by the PyTorch backend. "
+            f"Received: interpolation={interpolation}."
+        )
     if interpolation not in RESIZE_INTERPOLATIONS:
         raise ValueError(
             "Invalid value for argument `interpolation`. Expected of one "
             f"{RESIZE_INTERPOLATIONS}. Received: interpolation={interpolation}"
         )
     if fill_mode != "constant":
         raise ValueError(
@@ -64,322 +81,350 @@
         )
     if not len(size) == 2:
         raise ValueError(
             "Argument `size` must be a tuple of two elements "
             f"(height, width). Received: size={size}"
         )
     size = tuple(size)
-    target_height, target_width = size
-    if len(image.shape) == 4:
-        if data_format == "channels_last":
-            size = (image.shape[0],) + size + (image.shape[-1],)
-        else:
-            size = (image.shape[0], image.shape[1]) + size
-    elif len(image.shape) == 3:
-        if data_format == "channels_last":
-            size = size + (image.shape[-1],)
-        else:
-            size = (image.shape[0],) + size
-    else:
+    images = convert_to_tensor(images)
+    if images.ndim not in (3, 4):
         raise ValueError(
-            "Invalid input rank: expected rank 3 (single image) "
+            "Invalid images rank: expected rank 3 (single image) "
             "or rank 4 (batch of images). Received input with shape: "
-            f"image.shape={image.shape}"
+            f"images.shape={images.shape}"
         )
+    if data_format == "channels_last":
+        if images.ndim == 4:
+            images = images.permute((0, 3, 1, 2))
+        else:
+            images = images.permute((2, 0, 1))
 
     if crop_to_aspect_ratio:
-        shape = image.shape
-        if data_format == "channels_last":
-            height, width = shape[-3], shape[-2]
-        else:
-            height, width = shape[-2], shape[-1]
+        shape = images.shape
+        height, width = shape[-2], shape[-1]
+        target_height, target_width = size
         crop_height = int(float(width * target_height) / target_width)
         crop_height = min(height, crop_height)
         crop_width = int(float(height * target_width) / target_height)
         crop_width = min(width, crop_width)
         crop_box_hstart = int(float(height - crop_height) / 2)
         crop_box_wstart = int(float(width - crop_width) / 2)
-        if data_format == "channels_last":
-            if len(image.shape) == 4:
-                image = image[
-                    :,
-                    crop_box_hstart : crop_box_hstart + crop_height,
-                    crop_box_wstart : crop_box_wstart + crop_width,
-                    :,
-                ]
-            else:
-                image = image[
-                    crop_box_hstart : crop_box_hstart + crop_height,
-                    crop_box_wstart : crop_box_wstart + crop_width,
-                    :,
-                ]
+        if len(images.shape) == 4:
+            images = images[
+                :,
+                :,
+                crop_box_hstart : crop_box_hstart + crop_height,
+                crop_box_wstart : crop_box_wstart + crop_width,
+            ]
         else:
-            if len(image.shape) == 4:
-                image = image[
-                    :,
-                    :,
-                    crop_box_hstart : crop_box_hstart + crop_height,
-                    crop_box_wstart : crop_box_wstart + crop_width,
-                ]
-            else:
-                image = image[
-                    :,
-                    crop_box_hstart : crop_box_hstart + crop_height,
-                    crop_box_wstart : crop_box_wstart + crop_width,
-                ]
+            images = images[
+                :,
+                crop_box_hstart : crop_box_hstart + crop_height,
+                crop_box_wstart : crop_box_wstart + crop_width,
+            ]
     elif pad_to_aspect_ratio:
-        shape = image.shape
-        batch_size = image.shape[0]
-        if data_format == "channels_last":
-            height, width, channels = shape[-3], shape[-2], shape[-1]
-        else:
-            channels, height, width = shape[-3], shape[-2], shape[-1]
+        shape = images.shape
+        height, width = shape[-2], shape[-1]
+        target_height, target_width = size
         pad_height = int(float(width * target_height) / target_width)
         pad_height = max(height, pad_height)
         pad_width = int(float(height * target_width) / target_height)
         pad_width = max(width, pad_width)
         img_box_hstart = int(float(pad_height - height) / 2)
         img_box_wstart = int(float(pad_width - width) / 2)
-        if data_format == "channels_last":
-            if len(image.shape) == 4:
-                padded_img = (
-                    np.ones(
-                        (
-                            batch_size,
-                            pad_height + height,
-                            pad_width + width,
-                            channels,
-                        ),
-                        dtype=image.dtype,
-                    )
-                    * fill_value
-                )
-                padded_img[
-                    :,
-                    img_box_hstart : img_box_hstart + height,
-                    img_box_wstart : img_box_wstart + width,
-                    :,
-                ] = image
-            else:
-                padded_img = (
-                    np.ones(
-                        (pad_height + height, pad_width + width, channels),
-                        dtype=image.dtype,
-                    )
-                    * fill_value
+        if len(images.shape) == 4:
+            batch_size = images.shape[0]
+            channels = images.shape[1]
+            padded_img = (
+                torch.ones(
+                    (
+                        batch_size,
+                        channels,
+                        pad_height + height,
+                        pad_width + width,
+                    ),
+                    dtype=images.dtype,
                 )
-                padded_img[
-                    img_box_hstart : img_box_hstart + height,
-                    img_box_wstart : img_box_wstart + width,
-                    :,
-                ] = image
+                * fill_value
+            )
+            padded_img[
+                :,
+                :,
+                img_box_hstart : img_box_hstart + height,
+                img_box_wstart : img_box_wstart + width,
+            ] = images
         else:
-            if len(image.shape) == 4:
-                padded_img = (
-                    np.ones(
-                        (
-                            batch_size,
-                            channels,
-                            pad_height + height,
-                            pad_width + width,
-                        ),
-                        dtype=image.dtype,
-                    )
-                    * fill_value
-                )
-                padded_img[
-                    :,
-                    :,
-                    img_box_hstart : img_box_hstart + height,
-                    img_box_wstart : img_box_wstart + width,
-                ] = image
-            else:
-                padded_img = (
-                    np.ones(
-                        (channels, pad_height + height, pad_width + width),
-                        dtype=image.dtype,
-                    )
-                    * fill_value
+            channels = images.shape[0]
+            padded_img = (
+                torch.ones(
+                    (channels, pad_height + height, pad_width + width),
+                    dtype=images.dtype,
                 )
-                padded_img[
-                    :,
-                    img_box_hstart : img_box_hstart + height,
-                    img_box_wstart : img_box_wstart + width,
-                ] = image
-        image = padded_img
-
-    return np.array(
-        jax.image.resize(image, size, method=interpolation, antialias=antialias)
+                * fill_value
+            )
+            padded_img[
+                :,
+                img_box_hstart : img_box_hstart + height,
+                img_box_wstart : img_box_wstart + width,
+            ] = images
+        images = padded_img
+
+    resized = torchvision.transforms.functional.resize(
+        img=images,
+        size=size,
+        interpolation=RESIZE_INTERPOLATIONS[interpolation],
+        antialias=antialias,
     )
+    if data_format == "channels_last":
+        if len(images.shape) == 4:
+            resized = resized.permute((0, 2, 3, 1))
+        elif len(images.shape) == 3:
+            resized = resized.permute((1, 2, 0))
+    return resized
 
 
-AFFINE_TRANSFORM_INTERPOLATIONS = {  # map to order
+AFFINE_TRANSFORM_INTERPOLATIONS = {
     "nearest": 0,
     "bilinear": 1,
 }
 AFFINE_TRANSFORM_FILL_MODES = {
     "constant",
     "nearest",
     "wrap",
     "mirror",
     "reflect",
 }
 
 
 def affine_transform(
-    image,
+    images,
     transform,
     interpolation="bilinear",
     fill_mode="constant",
     fill_value=0,
-    data_format="channels_last",
+    data_format=None,
 ):
+    data_format = backend.standardize_data_format(data_format)
     if interpolation not in AFFINE_TRANSFORM_INTERPOLATIONS.keys():
         raise ValueError(
             "Invalid value for argument `interpolation`. Expected of one "
             f"{set(AFFINE_TRANSFORM_INTERPOLATIONS.keys())}. Received: "
             f"interpolation={interpolation}"
         )
     if fill_mode not in AFFINE_TRANSFORM_FILL_MODES:
         raise ValueError(
             "Invalid value for argument `fill_mode`. Expected of one "
             f"{AFFINE_TRANSFORM_FILL_MODES}. Received: fill_mode={fill_mode}"
         )
 
+    images = convert_to_tensor(images)
     transform = convert_to_tensor(transform)
 
-    if len(image.shape) not in (3, 4):
+    if images.ndim not in (3, 4):
         raise ValueError(
-            "Invalid image rank: expected rank 3 (single image) "
+            "Invalid images rank: expected rank 3 (single image) "
             "or rank 4 (batch of images). Received input with shape: "
-            f"image.shape={image.shape}"
+            f"images.shape={images.shape}"
         )
-    if len(transform.shape) not in (1, 2):
+    if transform.ndim not in (1, 2):
         raise ValueError(
             "Invalid transform rank: expected rank 1 (single transform) "
             "or rank 2 (batch of transforms). Received input with shape: "
             f"transform.shape={transform.shape}"
         )
 
-    # scipy.ndimage.map_coordinates lacks support for half precision.
-    input_dtype = image.dtype
-    if input_dtype == "float16":
-        image = image.astype("float32")
-
     # unbatched case
     need_squeeze = False
-    if len(image.shape) == 3:
-        image = np.expand_dims(image, axis=0)
+    if images.ndim == 3:
+        images = images.unsqueeze(dim=0)
         need_squeeze = True
-    if len(transform.shape) == 1:
-        transform = np.expand_dims(transform, axis=0)
+    if transform.ndim == 1:
+        transform = transform.unsqueeze(dim=0)
 
     if data_format == "channels_first":
-        image = np.transpose(image, (0, 2, 3, 1))
+        images = images.permute((0, 2, 3, 1))
 
-    batch_size = image.shape[0]
+    batch_size = images.shape[0]
 
     # get indices
-    meshgrid = np.meshgrid(
-        *[np.arange(size) for size in image.shape[1:]], indexing="ij"
+    meshgrid = torch.meshgrid(
+        *[
+            torch.arange(size, dtype=transform.dtype, device=transform.device)
+            for size in images.shape[1:]
+        ],
+        indexing="ij",
     )
-    indices = np.concatenate(
-        [np.expand_dims(x, axis=-1) for x in meshgrid], axis=-1
+    indices = torch.concatenate(
+        [torch.unsqueeze(x, dim=-1) for x in meshgrid], dim=-1
     )
-    indices = np.tile(indices, (batch_size, 1, 1, 1, 1))
+    indices = torch.tile(indices, (batch_size, 1, 1, 1, 1))
 
     # swap the values
-    a0 = transform[:, 0].copy()
-    a2 = transform[:, 2].copy()
-    b1 = transform[:, 4].copy()
-    b2 = transform[:, 5].copy()
+    a0 = transform[:, 0].clone()
+    a2 = transform[:, 2].clone()
+    b1 = transform[:, 4].clone()
+    b2 = transform[:, 5].clone()
     transform[:, 0] = b1
     transform[:, 2] = b2
     transform[:, 4] = a0
     transform[:, 5] = a2
 
     # deal with transform
-    transform = np.pad(transform, pad_width=[[0, 0], [0, 1]], constant_values=1)
-    transform = np.reshape(transform, (batch_size, 3, 3))
-    offset = transform[:, 0:2, 2].copy()
-    offset = np.pad(offset, pad_width=[[0, 0], [0, 1]])
+    transform = torch.nn.functional.pad(
+        transform, pad=[0, 1, 0, 0], mode="constant", value=1
+    )
+    transform = torch.reshape(transform, (batch_size, 3, 3))
+    offset = transform[:, 0:2, 2].clone()
+    offset = torch.nn.functional.pad(offset, pad=[0, 1, 0, 0])
     transform[:, 0:2, 2] = 0
 
     # transform the indices
-    coordinates = np.einsum("Bhwij, Bjk -> Bhwik", indices, transform)
-    coordinates = np.moveaxis(coordinates, source=-1, destination=1)
-    coordinates += np.reshape(a=offset, newshape=(*offset.shape, 1, 1, 1))
+    coordinates = torch.einsum("Bhwij, Bjk -> Bhwik", indices, transform)
+    coordinates = torch.moveaxis(coordinates, source=-1, destination=1)
+    coordinates += torch.reshape(a=offset, shape=(*offset.shape, 1, 1, 1))
 
-    # apply affine transformation
-    affined = np.stack(
+    # Note: torch.stack is faster than torch.vmap when the batch size is small.
+    affined = torch.stack(
         [
             map_coordinates(
-                image[i],
+                images[i],
                 coordinates[i],
                 order=AFFINE_TRANSFORM_INTERPOLATIONS[interpolation],
                 fill_mode=fill_mode,
                 fill_value=fill_value,
             )
-            for i in range(batch_size)
+            for i in range(len(images))
         ],
-        axis=0,
     )
 
     if data_format == "channels_first":
-        affined = np.transpose(affined, (0, 3, 1, 2))
+        affined = affined.permute((0, 3, 1, 2))
     if need_squeeze:
-        affined = np.squeeze(affined, axis=0)
-    if input_dtype == "float16":
-        affined = affined.astype(input_dtype)
+        affined = affined.squeeze(dim=0)
     return affined
 
 
-MAP_COORDINATES_FILL_MODES = {
-    "constant",
-    "nearest",
-    "wrap",
-    "mirror",
-    "reflect",
+def _mirror_index_fixer(index, size):
+    s = size - 1  # Half-wavelength of triangular wave
+    # Scaled, integer-valued version of the triangular wave |x - round(x)|
+    return torch.abs((index + s) % (2 * s) - s)
+
+
+def _reflect_index_fixer(index, size):
+    return torch.floor_divide(
+        _mirror_index_fixer(2 * index + 1, 2 * size + 1) - 1, 2
+    )
+
+
+_INDEX_FIXERS = {
+    # we need to take care of out-of-bound indices in torch
+    "constant": lambda index, size: torch.clip(index, 0, size - 1),
+    "nearest": lambda index, size: torch.clip(index, 0, size - 1),
+    "wrap": lambda index, size: index % size,
+    "mirror": _mirror_index_fixer,
+    "reflect": _reflect_index_fixer,
 }
 
 
+def _is_integer(a):
+    if not torch.is_floating_point(a) and not torch.is_complex(a):
+        return True
+    return False
+
+
+def _nearest_indices_and_weights(coordinate):
+    coordinate = (
+        coordinate if _is_integer(coordinate) else torch.round(coordinate)
+    )
+    index = coordinate.to(torch.int32)
+    return [(index, 1)]
+
+
+def _linear_indices_and_weights(coordinate):
+    lower = torch.floor(coordinate)
+    upper_weight = coordinate - lower
+    lower_weight = 1 - upper_weight
+    index = lower.to(torch.int32)
+    return [(index, lower_weight), (index + 1, upper_weight)]
+
+
 def map_coordinates(
-    input, coordinates, order, fill_mode="constant", fill_value=0.0
+    inputs, coordinates, order, fill_mode="constant", fill_value=0.0
 ):
-    if fill_mode not in MAP_COORDINATES_FILL_MODES:
+    input_arr = convert_to_tensor(inputs)
+    coordinate_arrs = [convert_to_tensor(c) for c in coordinates]
+
+    if len(coordinate_arrs) != len(input_arr.shape):
         raise ValueError(
-            "Invalid value for argument `fill_mode`. Expected one of "
-            f"{set(MAP_COORDINATES_FILL_MODES.keys())}. Received: "
-            f"fill_mode={fill_mode}"
+            "First dim of `coordinates` must be the same as the rank of "
+            "`inputs`. "
+            f"Received inputs with shape: {input_arr.shape} and coordinate "
+            f"leading dim of {len(coordinate_arrs)}"
         )
-    if order not in range(2):
+    if len(coordinate_arrs[0].shape) < 1:
+        dim = len(coordinate_arrs)
+        shape = (dim,) + coordinate_arrs[0].shape
         raise ValueError(
-            "Invalid value for argument `order`. Expected one of "
-            f"{[0, 1]}. Received: order={order}"
+            "Invalid coordinates rank: expected at least rank 2."
+            f" Received input with shape: {shape}"
         )
-    # SciPy's implementation of map_coordinates handles boundaries incorrectly,
-    # unless mode='reflect'. For order=1, this only affects interpolation
-    # outside the bounds of the original array.
-    # https://github.com/scipy/scipy/issues/2640
-    padding = [
-        (
-            max(-np.floor(c.min()).astype(int) + 1, 0),
-            max(np.ceil(c.max()).astype(int) + 1 - size, 0),
-        )
-        for c, size in zip(coordinates, input.shape)
-    ]
-    shifted_coords = [c + p[0] for p, c in zip(padding, coordinates)]
-    pad_mode = {
-        "nearest": "edge",
-        "mirror": "reflect",
-        "reflect": "symmetric",
-    }.get(fill_mode, fill_mode)
-    if fill_mode == "constant":
-        padded = np.pad(
-            input, padding, mode=pad_mode, constant_values=fill_value
+
+    # skip tensor creation as possible
+    if isinstance(fill_value, (int, float)) and _is_integer(input_arr):
+        fill_value = int(fill_value)
+
+    if len(coordinates) != len(input_arr.shape):
+        raise ValueError(
+            "coordinates must be a sequence of length inputs.shape, but "
+            f"{len(coordinates)} != {len(input_arr.shape)}"
         )
+
+    index_fixer = _INDEX_FIXERS.get(fill_mode)
+    if index_fixer is None:
+        raise ValueError(
+            "Invalid value for argument `fill_mode`. Expected one of "
+            f"{set(_INDEX_FIXERS.keys())}. Received: fill_mode={fill_mode}"
+        )
+
+    if order == 0:
+        interp_fun = _nearest_indices_and_weights
+    elif order == 1:
+        interp_fun = _linear_indices_and_weights
     else:
-        padded = np.pad(input, padding, mode=pad_mode)
-    result = scipy.ndimage.map_coordinates(
-        padded, shifted_coords, order=order, mode=fill_mode, cval=fill_value
-    )
-    return result
+        raise NotImplementedError("map_coordinates currently requires order<=1")
+
+    if fill_mode == "constant":
+
+        def is_valid(index, size):
+            return (0 <= index) & (index < size)
+
+    else:
+
+        def is_valid(index, size):
+            return True
+
+    valid_1d_interpolations = []
+    for coordinate, size in zip(coordinate_arrs, input_arr.shape):
+        interp_nodes = interp_fun(coordinate)
+        valid_interp = []
+        for index, weight in interp_nodes:
+            fixed_index = index_fixer(index, size)
+            valid = is_valid(index, size)
+            valid_interp.append((fixed_index, valid, weight))
+        valid_1d_interpolations.append(valid_interp)
+
+    outputs = []
+    for items in itertools.product(*valid_1d_interpolations):
+        indices, validities, weights = zip(*items)
+        if all(valid is True for valid in validities):
+            # fast path
+            contribution = input_arr[indices]
+        else:
+            all_valid = functools.reduce(operator.and_, validities)
+            contribution = torch.where(
+                all_valid, input_arr[indices], fill_value
+            )
+        outputs.append(functools.reduce(operator.mul, weights) * contribution)
+    result = functools.reduce(operator.add, outputs)
+    if _is_integer(input_arr):
+        result = result if _is_integer(result) else torch.round(result)
+    return result.to(input_arr.dtype)
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 import functools
 import itertools
 import operator
 
 import tensorflow as tf
 
+from keras.src import backend
 from keras.src.backend.tensorflow.core import convert_to_tensor
 
 RESIZE_INTERPOLATIONS = (
     "bilinear",
     "nearest",
     "lanczos3",
     "lanczos5",
     "bicubic",
 )
 
 
-def rgb_to_grayscale(image, data_format="channels_last"):
-    if data_format == "channels_first":
-        if len(image.shape) == 4:
-            image = tf.transpose(image, (0, 2, 3, 1))
-        elif len(image.shape) == 3:
-            image = tf.transpose(image, (1, 2, 0))
-        else:
-            raise ValueError(
-                "Invalid input rank: expected rank 3 (single image) "
-                "or rank 4 (batch of images). Received input with shape: "
-                f"image.shape={image.shape}"
-            )
-    grayscale_image = tf.image.rgb_to_grayscale(image)
-    if data_format == "channels_first":
-        if len(image.shape) == 4:
-            grayscale_image = tf.transpose(grayscale_image, (0, 3, 1, 2))
-        elif len(image.shape) == 3:
-            grayscale_image = tf.transpose(grayscale_image, (2, 0, 1))
-    return tf.cast(grayscale_image, image.dtype)
+def rgb_to_grayscale(images, data_format=None):
+    images = convert_to_tensor(images)
+    data_format = backend.standardize_data_format(data_format)
+    channels_axis = -1 if data_format == "channels_last" else -3
+    if len(images.shape) not in (3, 4):
+        raise ValueError(
+            "Invalid images rank: expected rank 3 (single image) "
+            "or rank 4 (batch of images). Received input with shape: "
+            f"images.shape={images.shape}"
+        )
+    # Convert to floats
+    original_dtype = images.dtype
+    compute_dtype = backend.result_type(images.dtype, float)
+    images = backend.cast(images, compute_dtype)
+
+    # Ref: tf.image.rgb_to_grayscale
+    rgb_weights = convert_to_tensor(
+        [0.2989, 0.5870, 0.1140], dtype=images.dtype
+    )
+    images = tf.tensordot(images, rgb_weights, axes=(channels_axis, -1))
+    images = tf.expand_dims(images, axis=channels_axis)
+    return tf.cast(images, original_dtype)
 
 
 def resize(
-    image,
+    images,
     size,
     interpolation="bilinear",
     antialias=False,
     crop_to_aspect_ratio=False,
     pad_to_aspect_ratio=False,
     fill_mode="constant",
     fill_value=0.0,
-    data_format="channels_last",
+    data_format=None,
 ):
+    data_format = backend.standardize_data_format(data_format)
     if interpolation not in RESIZE_INTERPOLATIONS:
         raise ValueError(
             "Invalid value for argument `interpolation`. Expected of one "
             f"{RESIZE_INTERPOLATIONS}. Received: interpolation={interpolation}"
         )
     if fill_mode != "constant":
         raise ValueError(
@@ -64,27 +69,28 @@
         )
     if not len(size) == 2:
         raise ValueError(
             "Argument `size` must be a tuple of two elements "
             f"(height, width). Received: size={size}"
         )
     size = tuple(size)
+    if len(images.shape) not in (3, 4):
+        raise ValueError(
+            "Invalid images rank: expected rank 3 (single image) "
+            "or rank 4 (batch of images). Received input with shape: "
+            f"images.shape={images.shape}"
+        )
     if data_format == "channels_first":
-        if len(image.shape) == 4:
-            image = tf.transpose(image, (0, 2, 3, 1))
-        elif len(image.shape) == 3:
-            image = tf.transpose(image, (1, 2, 0))
+        if len(images.shape) == 4:
+            images = tf.transpose(images, (0, 2, 3, 1))
         else:
-            raise ValueError(
-                "Invalid input rank: expected rank 3 (single image) "
-                "or rank 4 (batch of images). Received input with shape: "
-                f"image.shape={image.shape}"
-            )
+            images = tf.transpose(images, (1, 2, 0))
+
     if crop_to_aspect_ratio:
-        shape = tf.shape(image)
+        shape = tf.shape(images)
         height, width = shape[-3], shape[-2]
         target_height, target_width = size
         crop_height = tf.cast(
             tf.cast(width * target_height, "float32") / target_width,
             "int32",
         )
         crop_height = tf.minimum(height, crop_height)
@@ -98,29 +104,29 @@
 
         crop_box_hstart = tf.cast(
             tf.cast(height - crop_height, "float32") / 2, "int32"
         )
         crop_box_wstart = tf.cast(
             tf.cast(width - crop_width, "float32") / 2, "int32"
         )
-        if len(image.shape) == 4:
-            image = image[
+        if len(images.shape) == 4:
+            images = images[
                 :,
                 crop_box_hstart : crop_box_hstart + crop_height,
                 crop_box_wstart : crop_box_wstart + crop_width,
                 :,
             ]
         else:
-            image = image[
+            images = images[
                 crop_box_hstart : crop_box_hstart + crop_height,
                 crop_box_wstart : crop_box_wstart + crop_width,
                 :,
             ]
     elif pad_to_aspect_ratio:
-        shape = tf.shape(image)
+        shape = tf.shape(images)
         height, width = shape[-3], shape[-2]
         target_height, target_width = size
         pad_height = tf.cast(
             tf.cast(width * target_height, "float32") / target_width,
             "int32",
         )
         pad_height = tf.maximum(height, pad_height)
@@ -134,110 +140,110 @@
 
         img_box_hstart = tf.cast(
             tf.cast(pad_height - height, "float32") / 2, "int32"
         )
         img_box_wstart = tf.cast(
             tf.cast(pad_width - width, "float32") / 2, "int32"
         )
-        if len(image.shape) == 4:
-            batch_size = tf.shape(image)[0]
-            channels = tf.shape(image)[3]
+        if len(images.shape) == 4:
+            batch_size = tf.shape(images)[0]
+            channels = tf.shape(images)[3]
             padded_img = tf.cond(
                 img_box_hstart > 0,
                 lambda: tf.concat(
                     [
                         tf.ones(
                             (batch_size, img_box_hstart, width, channels),
-                            dtype=image.dtype,
+                            dtype=images.dtype,
                         )
                         * fill_value,
-                        image,
+                        images,
                         tf.ones(
                             (batch_size, img_box_hstart, width, channels),
-                            dtype=image.dtype,
+                            dtype=images.dtype,
                         )
                         * fill_value,
                     ],
                     axis=1,
                 ),
-                lambda: image,
+                lambda: images,
             )
             padded_img = tf.cond(
                 img_box_wstart > 0,
                 lambda: tf.concat(
                     [
                         tf.ones(
                             (batch_size, height, img_box_wstart, channels),
-                            dtype=image.dtype,
+                            dtype=images.dtype,
                         )
                         * fill_value,
                         padded_img,
                         tf.ones(
                             (batch_size, height, img_box_wstart, channels),
-                            dtype=image.dtype,
+                            dtype=images.dtype,
                         )
                         * fill_value,
                     ],
                     axis=2,
                 ),
                 lambda: padded_img,
             )
         else:
-            channels = tf.shape(image)[2]
+            channels = tf.shape(images)[2]
             padded_img = tf.cond(
                 img_box_hstart > 0,
                 lambda: tf.concat(
                     [
                         tf.ones(
                             (img_box_hstart, width, channels),
-                            dtype=image.dtype,
+                            dtype=images.dtype,
                         )
                         * fill_value,
-                        image,
+                        images,
                         tf.ones(
                             (img_box_hstart, width, channels),
-                            dtype=image.dtype,
+                            dtype=images.dtype,
                         )
                         * fill_value,
                     ],
                     axis=0,
                 ),
-                lambda: image,
+                lambda: images,
             )
             padded_img = tf.cond(
                 img_box_wstart > 0,
                 lambda: tf.concat(
                     [
                         tf.ones(
                             (height, img_box_wstart, channels),
-                            dtype=image.dtype,
+                            dtype=images.dtype,
                         )
                         * fill_value,
                         padded_img,
                         tf.ones(
                             (height, img_box_wstart, channels),
-                            dtype=image.dtype,
+                            dtype=images.dtype,
                         )
                         * fill_value,
                     ],
                     axis=1,
                 ),
                 lambda: padded_img,
             )
-        image = padded_img
+        images = padded_img
 
     resized = tf.image.resize(
-        image, size, method=interpolation, antialias=antialias
+        images, size, method=interpolation, antialias=antialias
     )
     if data_format == "channels_first":
-        if len(image.shape) == 4:
+        if len(images.shape) == 4:
             resized = tf.transpose(resized, (0, 3, 1, 2))
-        elif len(image.shape) == 3:
+        elif len(images.shape) == 3:
             resized = tf.transpose(resized, (2, 0, 1))
-    return tf.cast(resized, image.dtype)
+    return tf.cast(resized, images.dtype)
 
 
 AFFINE_TRANSFORM_INTERPOLATIONS = (
     "nearest",
     "bilinear",
 )
 AFFINE_TRANSFORM_FILL_MODES = (
@@ -246,64 +252,65 @@
     "wrap",
     # "mirror", not supported by TF
     "reflect",
 )
 
 
 def affine_transform(
-    image,
+    images,
     transform,
     interpolation="bilinear",
     fill_mode="constant",
     fill_value=0,
-    data_format="channels_last",
+    data_format=None,
 ):
+    data_format = backend.standardize_data_format(data_format)
     if interpolation not in AFFINE_TRANSFORM_INTERPOLATIONS:
         raise ValueError(
             "Invalid value for argument `interpolation`. Expected of one "
             f"{AFFINE_TRANSFORM_INTERPOLATIONS}. Received: "
             f"interpolation={interpolation}"
         )
     if fill_mode not in AFFINE_TRANSFORM_FILL_MODES:
         raise ValueError(
             "Invalid value for argument `fill_mode`. Expected of one "
             f"{AFFINE_TRANSFORM_FILL_MODES}. Received: fill_mode={fill_mode}"
         )
-    if len(image.shape) not in (3, 4):
+    if len(images.shape) not in (3, 4):
         raise ValueError(
-            "Invalid image rank: expected rank 3 (single image) "
+            "Invalid images rank: expected rank 3 (single image) "
             "or rank 4 (batch of images). Received input with shape: "
-            f"image.shape={image.shape}"
+            f"images.shape={images.shape}"
         )
     if len(transform.shape) not in (1, 2):
         raise ValueError(
             "Invalid transform rank: expected rank 1 (single transform) "
             "or rank 2 (batch of transforms). Received input with shape: "
             f"transform.shape={transform.shape}"
         )
     # unbatched case
     need_squeeze = False
-    if len(image.shape) == 3:
-        image = tf.expand_dims(image, axis=0)
+    if len(images.shape) == 3:
+        images = tf.expand_dims(images, axis=0)
         need_squeeze = True
     if len(transform.shape) == 1:
         transform = tf.expand_dims(transform, axis=0)
 
     if data_format == "channels_first":
-        image = tf.transpose(image, (0, 2, 3, 1))
+        images = tf.transpose(images, (0, 2, 3, 1))
 
     affined = tf.raw_ops.ImageProjectiveTransformV3(
-        images=image,
+        images=images,
         transforms=tf.cast(transform, dtype=tf.float32),
-        output_shape=tf.shape(image)[1:-1],
+        output_shape=tf.shape(images)[1:-1],
         fill_value=fill_value,
         interpolation=interpolation.upper(),
         fill_mode=fill_mode.upper(),
     )
-    affined = tf.ensure_shape(affined, image.shape)
+    affined = tf.ensure_shape(affined, images.shape)
 
     if data_format == "channels_first":
         affined = tf.transpose(affined, (0, 3, 1, 2))
     if need_squeeze:
         affined = tf.squeeze(affined, axis=0)
     return affined
 
@@ -343,27 +350,35 @@
     upper_weight = coordinate - lower
     lower_weight = 1 - upper_weight
     index = tf.cast(lower, tf.int32)
     return [(index, lower_weight), (index + 1, upper_weight)]
 
 
 def map_coordinates(
-    input, coordinates, order, fill_mode="constant", fill_value=0.0
+    inputs, coordinates, order, fill_mode="constant", fill_value=0.0
 ):
-    input_arr = convert_to_tensor(input)
+    input_arr = convert_to_tensor(inputs)
     coordinate_arrs = convert_to_tensor(coordinates)
-    # unstack into a list of tensors for following operations
-    coordinate_arrs = tf.unstack(coordinate_arrs, axis=0)
-    fill_value = convert_to_tensor(tf.cast(fill_value, input_arr.dtype))
 
-    if len(coordinates) != len(input_arr.shape):
+    if coordinate_arrs.shape[0] != len(input_arr.shape):
         raise ValueError(
-            "coordinates must be a sequence of length input.shape, but "
-            f"{len(coordinates)} != {len(input_arr.shape)}"
+            "First dim of `coordinates` must be the same as the rank of "
+            "`inputs`. "
+            f"Received inputs with shape: {input_arr.shape} and coordinate "
+            f"leading dim of {coordinate_arrs.shape[0]}"
         )
+    if len(coordinate_arrs.shape) < 2:
+        raise ValueError(
+            "Invalid coordinates rank: expected at least rank 2."
+            f" Received input with shape: {coordinate_arrs.shape}"
+        )
+
+    # unstack into a list of tensors for following operations
+    coordinate_arrs = tf.unstack(coordinate_arrs, axis=0)
+    fill_value = convert_to_tensor(tf.cast(fill_value, input_arr.dtype))
 
     index_fixer = _INDEX_FIXERS.get(fill_mode)
     if index_fixer is None:
         raise ValueError(
             "Invalid value for argument `fill_mode`. Expected one of "
             f"{set(_INDEX_FIXERS.keys())}. Received: "
             f"fill_mode={fill_mode}"
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1306,38 +1306,38 @@
     x2 = tf.cast(x2, dtype)
     return tf.less_equal(x1, x2)
 
 
 def linspace(
     start, stop, num=50, endpoint=True, retstep=False, dtype=None, axis=0
 ):
+    if num < 0:
+        raise ValueError(
+            f"`num` must be a non-negative integer. Received: num={num}"
+        )
     if dtype is None:
         dtypes_to_resolve = [
             getattr(start, "dtype", type(start)),
             getattr(stop, "dtype", type(stop)),
             float,
         ]
         dtype = dtypes.result_type(*dtypes_to_resolve)
     else:
         dtype = standardize_dtype(dtype)
     start = convert_to_tensor(start, dtype=dtype)
     stop = convert_to_tensor(stop, dtype=dtype)
-    if num < 0:
-        raise ValueError(
-            f"`num` must be a non-negative integer. Received: num={num}"
-        )
-    step = tf.convert_to_tensor(np.nan)
+    step = convert_to_tensor(np.nan)
     if endpoint:
         result = tf.linspace(start, stop, num, axis=axis)
         if num > 1:
-            step = (stop - start) / (num - 1)
+            step = (stop - start) / (tf.cast(num, dtype) - 1)
     else:
         # tf.linspace doesn't support endpoint=False, so we manually handle it
         if num > 0:
-            step = (stop - start) / num
+            step = (stop - start) / tf.cast(num, dtype)
         if num > 1:
             new_stop = tf.cast(stop, step.dtype) - step
             start = tf.cast(start, new_stop.dtype)
             result = tf.linspace(start, new_stop, num, axis=axis)
         else:
             result = tf.linspace(start, stop, num, axis=axis)
     if dtype is not None:
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/core.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/image.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/dot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,428 +1,376 @@
-import functools
-import itertools
-import operator
-
-import torch
-
-from keras.src.backend.torch.core import convert_to_tensor
-
-RESIZE_INTERPOLATIONS = {}  # populated after torchvision import
-
-UNSUPPORTED_INTERPOLATIONS = (
-    "lanczos3",
-    "lanczos5",
-)
-
-
-def rgb_to_grayscale(image, data_format="channel_last"):
-    try:
-        import torchvision
-    except:
-        raise ImportError(
-            "The torchvision package is necessary to use "
-            "`rgb_to_grayscale` with the torch backend. "
-            "Please install torchvision. "
+from keras.src import ops
+from keras.src.api_export import keras_export
+from keras.src.layers.merging.base_merge import Merge
+from keras.src.utils.numerical_utils import normalize
+
+
+def batch_dot(x, y, axes=None):
+    """Batchwise dot product.
+
+    `batch_dot` is used to compute dot product of `x` and `y` when
+    `x` and `y` are data in batch, i.e. in a shape of `(batch_size, :)`.
+    `batch_dot` results in a tensor or variable with less dimensions
+    than the input. If the number of dimensions is reduced to 1,
+    we use `expand_dims` to make sure that ndim is at least 2.
+
+    Shape inference:
+
+    Let `x`'s shape be `(100, 20)` and `y`'s shape be `(100, 30, 20)`.
+    If `axes` is (1, 2), to find the output shape of resultant tensor,
+    loop through each dimension in `x`'s shape and `y`'s shape:
+
+    * `x.shape[0]` : 100 : append to output shape
+    * `x.shape[1]` : 20 : do not append to output shape, dimension 1 of
+        `x` has been summed over. (`dot_axes[0]` = 1)
+    * `y.shape[0]` : 100 : do not append to output shape, always ignore
+        first dimension of `y`
+    * `y.shape[1]` : 30 : append to output shape
+    * `y.shape[2]` : 20 : do not append to output shape, dimension 2 of
+        `y` has been summed over.
+        (`dot_axes[1]` = 2) `output_shape` = `(100, 30)`
+
+    Example:
+
+    >>> x_batch = np.ones(shape=(32, 20, 1))
+    >>> y_batch = np.ones(shape=(32, 30, 20))
+    >>> xy_batch_dot = batch_dot(x_batch, y_batch, axes=(1, 2))
+
+    Args:
+        x: Keras tensor or variable with `ndim >= 2`.
+        y: Keras tensor or variable with `ndim >= 2`.
+        axes: Tuple or list of integers with target dimensions, or single
+            integer. The sizes of `x.shape[axes[0]]` and `y.shape[axes[1]]`
+            should be equal.
+
+    Returns:
+        A tensor with shape equal to the concatenation of `x`'s shape
+        (less the dimension that was summed over) and `y`'s shape (less the
+        batch dimension and the dimension that was summed over). If the final
+        rank is 1, we reshape it to `(batch_size, 1)`.
+    """
+
+    x_shape = x.shape
+    y_shape = y.shape
+
+    x_ndim = len(x_shape)
+    y_ndim = len(y_shape)
+
+    if x_ndim < 2 or y_ndim < 2:
+        raise ValueError(
+            f"Cannot do batch_dot on inputs "
+            f"with rank < 2. "
+            f"Received inputs with shapes "
+            f"{x_shape} and {y_shape}."
         )
-    image = convert_to_tensor(image)
-    if data_format == "channels_last":
-        if image.ndim == 4:
-            image = image.permute((0, 3, 1, 2))
-        elif image.ndim == 3:
-            image = image.permute((2, 0, 1))
-        else:
-            raise ValueError(
-                "Invalid input rank: expected rank 3 (single image) "
-                "or rank 4 (batch of images). Received input with shape: "
-                f"image.shape={image.shape}"
-            )
-    grayscale_image = torchvision.transforms.functional.rgb_to_grayscale(
-        img=image,
-    )
-    if data_format == "channels_last":
-        if len(image.shape) == 4:
-            grayscale_image = grayscale_image.permute((0, 2, 3, 1))
-        elif len(image.shape) == 3:
-            grayscale_image = grayscale_image.permute((1, 2, 0))
-    return grayscale_image
-
-
-def resize(
-    image,
-    size,
-    interpolation="bilinear",
-    antialias=False,
-    crop_to_aspect_ratio=False,
-    pad_to_aspect_ratio=False,
-    fill_mode="constant",
-    fill_value=0.0,
-    data_format="channels_last",
-):
-    try:
-        import torchvision
-        from torchvision.transforms import InterpolationMode as im
-
-        RESIZE_INTERPOLATIONS.update(
-            {
-                "bilinear": im.BILINEAR,
-                "nearest": im.NEAREST_EXACT,
-                "bicubic": im.BICUBIC,
-            }
-        )
-    except:
-        raise ImportError(
-            "The torchvision package is necessary to use `resize` with the "
-            "torch backend. Please install torchvision."
-        )
-    if interpolation in UNSUPPORTED_INTERPOLATIONS:
-        raise ValueError(
-            "Resizing with Lanczos interpolation is "
-            "not supported by the PyTorch backend. "
-            f"Received: interpolation={interpolation}."
-        )
-    if interpolation not in RESIZE_INTERPOLATIONS:
-        raise ValueError(
-            "Invalid value for argument `interpolation`. Expected of one "
-            f"{RESIZE_INTERPOLATIONS}. Received: interpolation={interpolation}"
-        )
-    if fill_mode != "constant":
-        raise ValueError(
-            "Invalid value for argument `fill_mode`. Only `'constant'` "
-            f"is supported. Received: fill_mode={fill_mode}"
-        )
-    if pad_to_aspect_ratio and crop_to_aspect_ratio:
-        raise ValueError(
-            "Only one of `pad_to_aspect_ratio` & `crop_to_aspect_ratio` "
-            "can be `True`."
-        )
-    if not len(size) == 2:
-        raise ValueError(
-            "Argument `size` must be a tuple of two elements "
-            f"(height, width). Received: size={size}"
-        )
-    size = tuple(size)
-    image = convert_to_tensor(image)
-    if data_format == "channels_last":
-        if image.ndim == 4:
-            image = image.permute((0, 3, 1, 2))
-        elif image.ndim == 3:
-            image = image.permute((2, 0, 1))
-        else:
-            raise ValueError(
-                "Invalid input rank: expected rank 3 (single image) "
-                "or rank 4 (batch of images). Received input with shape: "
-                f"image.shape={image.shape}"
-            )
 
-    if crop_to_aspect_ratio:
-        shape = image.shape
-        height, width = shape[-2], shape[-1]
-        target_height, target_width = size
-        crop_height = int(float(width * target_height) / target_width)
-        crop_height = min(height, crop_height)
-        crop_width = int(float(height * target_width) / target_height)
-        crop_width = min(width, crop_width)
-        crop_box_hstart = int(float(height - crop_height) / 2)
-        crop_box_wstart = int(float(width - crop_width) / 2)
-        if len(image.shape) == 4:
-            image = image[
-                :,
-                :,
-                crop_box_hstart : crop_box_hstart + crop_height,
-                crop_box_wstart : crop_box_wstart + crop_width,
-            ]
-        else:
-            image = image[
-                :,
-                crop_box_hstart : crop_box_hstart + crop_height,
-                crop_box_wstart : crop_box_wstart + crop_width,
-            ]
-    elif pad_to_aspect_ratio:
-        shape = image.shape
-        height, width = shape[-2], shape[-1]
-        target_height, target_width = size
-        pad_height = int(float(width * target_height) / target_width)
-        pad_height = max(height, pad_height)
-        pad_width = int(float(height * target_width) / target_height)
-        pad_width = max(width, pad_width)
-        img_box_hstart = int(float(pad_height - height) / 2)
-        img_box_wstart = int(float(pad_width - width) / 2)
-        if len(image.shape) == 4:
-            batch_size = image.shape[0]
-            channels = image.shape[1]
-            padded_img = (
-                torch.ones(
-                    (
-                        batch_size,
-                        channels,
-                        pad_height + height,
-                        pad_width + width,
-                    ),
-                    dtype=image.dtype,
-                )
-                * fill_value
-            )
-            padded_img[
-                :,
-                :,
-                img_box_hstart : img_box_hstart + height,
-                img_box_wstart : img_box_wstart + width,
-            ] = image
-        else:
-            channels = image.shape[0]
-            padded_img = (
-                torch.ones(
-                    (channels, pad_height + height, pad_width + width),
-                    dtype=image.dtype,
-                )
-                * fill_value
-            )
-            padded_img[
-                :,
-                img_box_hstart : img_box_hstart + height,
-                img_box_wstart : img_box_wstart + width,
-            ] = image
-        image = padded_img
-
-    resized = torchvision.transforms.functional.resize(
-        img=image,
-        size=size,
-        interpolation=RESIZE_INTERPOLATIONS[interpolation],
-        antialias=antialias,
-    )
-    if data_format == "channels_last":
-        if len(image.shape) == 4:
-            resized = resized.permute((0, 2, 3, 1))
-        elif len(image.shape) == 3:
-            resized = resized.permute((1, 2, 0))
-    return resized
-
-
-AFFINE_TRANSFORM_INTERPOLATIONS = {
-    "nearest": 0,
-    "bilinear": 1,
-}
-AFFINE_TRANSFORM_FILL_MODES = {
-    "constant",
-    "nearest",
-    "wrap",
-    "mirror",
-    "reflect",
-}
-
-
-def affine_transform(
-    image,
-    transform,
-    interpolation="bilinear",
-    fill_mode="constant",
-    fill_value=0,
-    data_format="channels_last",
-):
-    if interpolation not in AFFINE_TRANSFORM_INTERPOLATIONS.keys():
-        raise ValueError(
-            "Invalid value for argument `interpolation`. Expected of one "
-            f"{set(AFFINE_TRANSFORM_INTERPOLATIONS.keys())}. Received: "
-            f"interpolation={interpolation}"
-        )
-    if fill_mode not in AFFINE_TRANSFORM_FILL_MODES:
-        raise ValueError(
-            "Invalid value for argument `fill_mode`. Expected of one "
-            f"{AFFINE_TRANSFORM_FILL_MODES}. Received: fill_mode={fill_mode}"
-        )
+    x_batch_size = x_shape[0]
+    y_batch_size = y_shape[0]
 
-    image = convert_to_tensor(image)
-    transform = convert_to_tensor(transform)
-
-    if image.ndim not in (3, 4):
-        raise ValueError(
-            "Invalid image rank: expected rank 3 (single image) "
-            "or rank 4 (batch of images). Received input with shape: "
-            f"image.shape={image.shape}"
-        )
-    if transform.ndim not in (1, 2):
-        raise ValueError(
-            "Invalid transform rank: expected rank 1 (single transform) "
-            "or rank 2 (batch of transforms). Received input with shape: "
-            f"transform.shape={transform.shape}"
-        )
-
-    # unbatched case
-    need_squeeze = False
-    if image.ndim == 3:
-        image = image.unsqueeze(dim=0)
-        need_squeeze = True
-    if transform.ndim == 1:
-        transform = transform.unsqueeze(dim=0)
-
-    if data_format == "channels_first":
-        image = image.permute((0, 2, 3, 1))
-
-    batch_size = image.shape[0]
-
-    # get indices
-    meshgrid = torch.meshgrid(
-        *[
-            torch.arange(size, dtype=transform.dtype, device=transform.device)
-            for size in image.shape[1:]
-        ],
-        indexing="ij",
-    )
-    indices = torch.concatenate(
-        [torch.unsqueeze(x, dim=-1) for x in meshgrid], dim=-1
-    )
-    indices = torch.tile(indices, (batch_size, 1, 1, 1, 1))
-
-    # swap the values
-    a0 = transform[:, 0].clone()
-    a2 = transform[:, 2].clone()
-    b1 = transform[:, 4].clone()
-    b2 = transform[:, 5].clone()
-    transform[:, 0] = b1
-    transform[:, 2] = b2
-    transform[:, 4] = a0
-    transform[:, 5] = a2
-
-    # deal with transform
-    transform = torch.nn.functional.pad(
-        transform, pad=[0, 1, 0, 0], mode="constant", value=1
-    )
-    transform = torch.reshape(transform, (batch_size, 3, 3))
-    offset = transform[:, 0:2, 2].clone()
-    offset = torch.nn.functional.pad(offset, pad=[0, 1, 0, 0])
-    transform[:, 0:2, 2] = 0
-
-    # transform the indices
-    coordinates = torch.einsum("Bhwij, Bjk -> Bhwik", indices, transform)
-    coordinates = torch.moveaxis(coordinates, source=-1, destination=1)
-    coordinates += torch.reshape(a=offset, shape=(*offset.shape, 1, 1, 1))
-
-    # Note: torch.stack is faster than torch.vmap when the batch size is small.
-    affined = torch.stack(
-        [
-            map_coordinates(
-                image[i],
-                coordinates[i],
-                order=AFFINE_TRANSFORM_INTERPOLATIONS[interpolation],
-                fill_mode=fill_mode,
-                fill_value=fill_value,
+    if x_batch_size is not None and y_batch_size is not None:
+        if x_batch_size != y_batch_size:
+            raise ValueError(
+                f"Cannot do batch_dot on inputs "
+                f"with different batch sizes. "
+                f"Received inputs with shapes "
+                f"{x_shape} and {y_shape}."
             )
-            for i in range(len(image))
-        ],
-    )
-
-    if data_format == "channels_first":
-        affined = affined.permute((0, 3, 1, 2))
-    if need_squeeze:
-        affined = affined.squeeze(dim=0)
-    return affined
-
-
-def _mirror_index_fixer(index, size):
-    s = size - 1  # Half-wavelength of triangular wave
-    # Scaled, integer-valued version of the triangular wave |x - round(x)|
-    return torch.abs((index + s) % (2 * s) - s)
-
-
-def _reflect_index_fixer(index, size):
-    return torch.floor_divide(
-        _mirror_index_fixer(2 * index + 1, 2 * size + 1) - 1, 2
-    )
-
-
-_INDEX_FIXERS = {
-    # we need to take care of out-of-bound indices in torch
-    "constant": lambda index, size: torch.clip(index, 0, size - 1),
-    "nearest": lambda index, size: torch.clip(index, 0, size - 1),
-    "wrap": lambda index, size: index % size,
-    "mirror": _mirror_index_fixer,
-    "reflect": _reflect_index_fixer,
-}
-
-
-def _is_integer(a):
-    if not torch.is_floating_point(a) and not torch.is_complex(a):
-        return True
-    return False
-
-
-def _nearest_indices_and_weights(coordinate):
-    coordinate = (
-        coordinate if _is_integer(coordinate) else torch.round(coordinate)
-    )
-    index = coordinate.to(torch.int32)
-    return [(index, 1)]
-
-
-def _linear_indices_and_weights(coordinate):
-    lower = torch.floor(coordinate)
-    upper_weight = coordinate - lower
-    lower_weight = 1 - upper_weight
-    index = lower.to(torch.int32)
-    return [(index, lower_weight), (index + 1, upper_weight)]
-
-
-def map_coordinates(
-    input, coordinates, order, fill_mode="constant", fill_value=0.0
-):
-    input_arr = convert_to_tensor(input)
-    coordinate_arrs = [convert_to_tensor(c) for c in coordinates]
-    # skip tensor creation as possible
-    if isinstance(fill_value, (int, float)) and _is_integer(input_arr):
-        fill_value = int(fill_value)
+    if isinstance(axes, int):
+        axes = [axes, axes]
 
-    if len(coordinates) != len(input_arr.shape):
-        raise ValueError(
-            "coordinates must be a sequence of length input.shape, but "
-            f"{len(coordinates)} != {len(input_arr.shape)}"
-        )
+    if axes is None:
+        if y_ndim == 2:
+            axes = [x_ndim - 1, y_ndim - 1]
+        else:
+            axes = [x_ndim - 1, y_ndim - 2]
 
-    index_fixer = _INDEX_FIXERS.get(fill_mode)
-    if index_fixer is None:
+    if any(isinstance(a, (list, tuple)) for a in axes):
         raise ValueError(
-            "Invalid value for argument `fill_mode`. Expected one of "
-            f"{set(_INDEX_FIXERS.keys())}. Received: fill_mode={fill_mode}"
-        )
-
-    if order == 0:
-        interp_fun = _nearest_indices_and_weights
-    elif order == 1:
-        interp_fun = _linear_indices_and_weights
+            f"Multiple target dimensions are not supported. "
+            f"Expected: None, int, (int, int), "
+            f"Provided: {axes} "
+        )
+
+    # if tuple, convert to list.
+    axes = list(axes)
+
+    # convert negative indices.
+    if axes[0] < 0:
+        axes[0] += x_ndim
+    if axes[1] < 0:
+        axes[1] += y_ndim
+
+    # sanity checks
+    if 0 in axes:
+        raise ValueError(
+            "Cannot perform batch_dot over axis 0. "
+            "If your inputs are not batched, "
+            "add a dummy batch dimension to your "
+            "inputs using keras.ops.expand_dims(x, 0)"
+        )
+    a0, a1 = axes
+    d1 = x_shape[a0]
+    d2 = y_shape[a1]
+
+    if d1 is not None and d2 is not None and d1 != d2:
+        raise ValueError(
+            f"Cannot do batch_dot on inputs with shapes "
+            f"{x_shape} and {y_shape} with axes={axes}. "
+            f"x.shape[{axes[0]}] != y.shape[{axes[1]}] ({d1} != {d2})."
+        )
+
+    # backup ndims. Need them later.
+    orig_x_ndim = x_ndim
+    orig_y_ndim = y_ndim
+
+    # if rank is 2, expand to 3.
+    if x_ndim == 2:
+        x = ops.expand_dims(x, 1)
+        a0 += 1
+        x_ndim += 1
+    if y_ndim == 2:
+        y = ops.expand_dims(y, 2)
+        y_ndim += 1
+
+    # bring x's dimension to be reduced to last axis.
+    if a0 != x_ndim - 1:
+        pattern = list(range(x_ndim))
+        for i in range(a0, x_ndim - 1):
+            pattern[i] = pattern[i + 1]
+        pattern[-1] = a0
+        x = ops.transpose(x, pattern)
+
+    # bring y's dimension to be reduced to axis 1.
+    if a1 != 1:
+        pattern = list(range(y_ndim))
+        for i in range(a1, 1, -1):
+            pattern[i] = pattern[i - 1]
+        pattern[1] = a1
+        y = ops.transpose(y, pattern)
+
+    # normalize both inputs to rank 3.
+    if x_ndim > 3:
+        # squash middle dimensions of x.
+        x_shape = ops.shape(x)
+        x_mid_dims = x_shape[1:-1]
+        x_squashed_shape = (x_shape[0], -1, x_shape[-1])
+        x = ops.reshape(x, x_squashed_shape)
+        x_squashed = True
     else:
-        raise NotImplementedError("map_coordinates currently requires order<=1")
+        x_squashed = False
 
-    if fill_mode == "constant":
+    if y_ndim > 3:
+        # squash trailing dimensions of y.
+        y_shape = ops.shape(y)
+        y_trail_dims = y_shape[2:]
+        y_squashed_shape = (y_shape[0], y_shape[1], -1)
+        y = ops.reshape(y, y_squashed_shape)
+        y_squashed = True
+    else:
+        y_squashed = False
 
-        def is_valid(index, size):
-            return (0 <= index) & (index < size)
+    result = ops.matmul(x, y)
 
-    else:
+    # if inputs were squashed, we have to reshape the matmul output.
+    output_shape = ops.shape(result)
+    do_reshape = False
+
+    if x_squashed:
+        output_shape = output_shape[:1] + x_mid_dims + output_shape[-1:]
+        do_reshape = True
+
+    if y_squashed:
+        output_shape = output_shape[:-1] + y_trail_dims
+        do_reshape = True
+
+    if do_reshape:
+        result = ops.reshape(result, output_shape)
+
+    # if the inputs were originally rank 2, we remove the added 1 dim.
+    if orig_x_ndim == 2:
+        result = ops.squeeze(result, 1)
+    elif orig_y_ndim == 2:
+        result = ops.squeeze(result, -1)
+
+    return result
+
+
+@keras_export("keras.layers.Dot")
+class Dot(Merge):
+    """Computes element-wise dot product of two tensors.
+
+    It takes a list of inputs of size 2, and the axes
+    corresponding to each input along with the dot product
+    is to be performed.
+
+    Let's say `x` and `y` are the two input tensors with shapes
+    `(2, 3, 5)` and `(2, 10, 3)`. The batch dimension should be
+    of same size for both the inputs, and `axes` should correspond
+    to the dimensions that have the same size in the corresponding
+    inputs. e.g. with `axes=(1, 2)`, the dot product of `x`, and `y`
+    will result in a tensor with shape `(2, 5, 10)`
+
+    Example:
+
+    >>> x = np.arange(10).reshape(1, 5, 2)
+    >>> y = np.arange(10, 20).reshape(1, 2, 5)
+    >>> keras.layers.Dot(axes=(1, 2))([x, y])
+
+    Usage in a Keras model:
+
+    >>> x1 = keras.layers.Dense(8)(np.arange(10).reshape(5, 2))
+    >>> x2 = keras.layers.Dense(8)(np.arange(10, 20).reshape(5, 2))
+    >>> y = keras.layers.Dot(axes=1)([x1, x2])
+
+    Args:
+        axes: Integer or tuple of integers, axis or axes along which to
+            take the dot product. If a tuple, should be two integers
+            corresponding to the desired axis from the first input and the
+            desired axis from the second input, respectively. Note that the
+            size of the two selected axes must match.
+        normalize: Whether to L2-normalize samples along the dot product axis
+            before taking the dot product. If set to `True`, then
+            the output of the dot product is the cosine proximity
+            between the two samples.
+        **kwargs: Standard layer keyword arguments.
+
+    Returns:
+        A tensor, the dot product of the samples from the inputs.
+    """
+
+    def __init__(self, axes, normalize=False, **kwargs):
+        super().__init__(**kwargs)
+        if not isinstance(axes, int):
+            if not isinstance(axes, (list, tuple)):
+                raise TypeError(
+                    f"Invalid type for argument `axes`: it should be "
+                    f"a list or an int. Received: axes={axes}"
+                )
+            if len(axes) != 2:
+                raise ValueError(
+                    f"Invalid format for argument `axes`: it should contain "
+                    f"two elements. Received: axes={axes}"
+                )
+            if not isinstance(axes[0], int) or not isinstance(axes[1], int):
+                raise ValueError(
+                    f"Invalid format for argument `axes`: list elements should "
+                    f"be integers. Received: axes={axes}"
+                )
+        self.axes = axes
+        self.normalize = normalize
+        self.supports_masking = True
+        self._reshape_required = False
+
+    def build(self, input_shape):
+        # Used purely for shape validation.
+        if (
+            not isinstance(input_shape[0], (tuple, list))
+            or len(input_shape) != 2
+        ):
+            raise ValueError(
+                f"A `Dot` layer should be called on a list of 2 inputs. "
+                f"Received: input_shape={input_shape}"
+            )
+        shape1 = input_shape[0]
+        shape2 = input_shape[1]
+        if shape1 is None or shape2 is None:
+            return
+        if isinstance(self.axes, int):
+            if self.axes < 0:
+                axes = [self.axes % len(shape1), self.axes % len(shape2)]
+            else:
+                axes = [self.axes] * 2
+        else:
+            axes = self.axes
+        if shape1[axes[0]] != shape2[axes[1]]:
+            raise ValueError(
+                f"Incompatible input shapes: "
+                f"axis values {shape1[axes[0]]} (at axis {axes[0]}) != "
+                f"{shape2[axes[1]]} (at axis {axes[1]}). "
+                f"Full input shapes: {shape1}, {shape2}"
+            )
+        self.built = True
 
-        def is_valid(index, size):
-            return True
+    def _merge_function(self, inputs):
+        if len(inputs) != 2:
+            raise ValueError(
+                f"A `Dot` layer should be called on exactly 2 inputs. "
+                f"Received: inputs={inputs}"
+            )
+        x1 = inputs[0]
+        x2 = inputs[1]
 
-    valid_1d_interpolations = []
-    for coordinate, size in zip(coordinate_arrs, input_arr.shape):
-        interp_nodes = interp_fun(coordinate)
-        valid_interp = []
-        for index, weight in interp_nodes:
-            fixed_index = index_fixer(index, size)
-            valid = is_valid(index, size)
-            valid_interp.append((fixed_index, valid, weight))
-        valid_1d_interpolations.append(valid_interp)
-
-    outputs = []
-    for items in itertools.product(*valid_1d_interpolations):
-        indices, validities, weights = zip(*items)
-        if all(valid is True for valid in validities):
-            # fast path
-            contribution = input_arr[indices]
+        if isinstance(self.axes, int):
+            if self.axes < 0:
+                axes = [
+                    self.axes % len(x1.shape),
+                    self.axes % len(x2.shape),
+                ]
+            else:
+                axes = [self.axes] * 2
         else:
-            all_valid = functools.reduce(operator.and_, validities)
-            contribution = torch.where(
-                all_valid, input_arr[indices], fill_value
+            axes = []
+            for i in range(len(self.axes)):
+                if self.axes[i] < 0:
+                    axes.append(self.axes[i] % len(inputs[i].shape))
+                else:
+                    axes.append(self.axes[i])
+
+        if self.normalize:
+            x1 = normalize(x1, axis=axes[0])
+            x2 = normalize(x2, axis=axes[1])
+        output = batch_dot(x1, x2, axes)
+        return output
+
+    def compute_output_shape(self, input_shape):
+        if not isinstance(input_shape, (tuple, list)) or len(input_shape) != 2:
+            raise ValueError(
+                f"A `Dot` layer should be called on a list of 2 inputs. "
+                f"Received: input_shape={input_shape}"
             )
-        outputs.append(functools.reduce(operator.mul, weights) * contribution)
-    result = functools.reduce(operator.add, outputs)
-    if _is_integer(input_arr):
-        result = result if _is_integer(result) else torch.round(result)
-    return result.to(input_arr.dtype)
+        shape1 = list(input_shape[0])
+        shape2 = list(input_shape[1])
+        if isinstance(self.axes, int):
+            if self.axes < 0:
+                axes = [self.axes % len(shape1), self.axes % len(shape2)]
+            else:
+                axes = [self.axes] * 2
+        else:
+            axes = self.axes
+        shape1.pop(axes[0])
+        shape2.pop(axes[1])
+        shape2.pop(0)
+        output_shape = shape1 + shape2
+        if len(output_shape) == 1:
+            output_shape += [1]
+        return tuple(output_shape)
+
+    def compute_mask(self, inputs, mask=None):
+        return None
+
+    def get_config(self):
+        config = {
+            "axes": self.axes,
+            "normalize": self.normalize,
+        }
+        base_config = super().get_config()
+        return dict(list(base_config.items()) + list(config.items()))
+
+
+@keras_export("keras.layers.dot")
+def dot(inputs, axes=-1, **kwargs):
+    """Functional interface to the `Dot` layer.
+
+    Args:
+        inputs: A list of input tensors (at least 2).
+        axes: Integer or tuple of integers,
+            axis or axes along which to take the dot product.
+        normalize: Whether to L2-normalize samples along the
+            dot product axis before taking the dot product.
+            If set to `True`, then the output of the dot product
+            is the cosine proximity between the two samples.
+        **kwargs: Standard layer keyword arguments.
+
+    Returns:
+        A tensor, the dot product of the samples from the inputs.
+    """
+    return Dot(axes=axes, **kwargs)(inputs)
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/math.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/random.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/callback.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/history.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/constraints/constraints.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/datasets/cifar.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/datasets/imdb.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/datasets/mnist.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/datasets/reuters.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/export/export_lib.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/initializers/initializer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/dense.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/identity.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/masking.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/input_spec.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/layer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/add.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/average.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/discretization.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,376 +1,337 @@
-from keras.src import ops
-from keras.src.api_export import keras_export
-from keras.src.layers.merging.base_merge import Merge
-from keras.src.utils.numerical_utils import normalize
-
+import numpy as np
 
-def batch_dot(x, y, axes=None):
-    """Batchwise dot product.
+from keras.src import backend
+from keras.src.api_export import keras_export
+from keras.src.layers.preprocessing.tf_data_layer import TFDataLayer
+from keras.src.utils import argument_validation
+from keras.src.utils import numerical_utils
+from keras.src.utils.module_utils import tensorflow as tf
+
+
+@keras_export("keras.layers.Discretization")
+class Discretization(TFDataLayer):
+    """A preprocessing layer which buckets continuous features by ranges.
+
+    This layer will place each element of its input data into one of several
+    contiguous ranges and output an integer index indicating which range each
+    element was placed in.
+
+    **Note:** This layer is safe to use inside a `tf.data` pipeline
+    (independently of which backend you're using).
+
+    Input shape:
+        Any array of dimension 2 or higher.
+
+    Output shape:
+        Same as input shape.
+
+    Arguments:
+        bin_boundaries: A list of bin boundaries.
+            The leftmost and rightmost bins
+            will always extend to `-inf` and `inf`,
+            so `bin_boundaries=[0., 1., 2.]`
+            generates bins `(-inf, 0.)`, `[0., 1.)`, `[1., 2.)`,
+            and `[2., +inf)`.
+            If this option is set, `adapt()` should not be called.
+        num_bins: The integer number of bins to compute.
+            If this option is set,
+            `adapt()` should be called to learn the bin boundaries.
+        epsilon: Error tolerance, typically a small fraction
+            close to zero (e.g. 0.01). Higher values of epsilon increase
+            the quantile approximation, and hence result in more
+            unequal buckets, but could improve performance
+            and resource consumption.
+        output_mode: Specification for the output of the layer.
+            Values can be `"int"`, `"one_hot"`, `"multi_hot"`, or
+            `"count"` configuring the layer as follows:
+            - `"int"`: Return the discretized bin indices directly.
+            - `"one_hot"`: Encodes each individual element in the
+                input into an array the same size as `num_bins`,
+                containing a 1 at the input's bin
+                index. If the last dimension is size 1, will encode on that
+                dimension.  If the last dimension is not size 1,
+                will append a new dimension for the encoded output.
+            - `"multi_hot"`: Encodes each sample in the input into a
+                single array the same size as `num_bins`,
+                containing a 1 for each bin index
+                index present in the sample.
+                Treats the last dimension as the sample
+                dimension, if input shape is `(..., sample_length)`,
+                output shape will be `(..., num_tokens)`.
+            - `"count"`: As `"multi_hot"`, but the int array contains
+                a count of the number of times the bin index appeared
+                in the sample.
+            Defaults to `"int"`.
+        sparse: Boolean. Only applicable to `"one_hot"`, `"multi_hot"`,
+            and `"count"` output modes. Only supported with TensorFlow
+            backend. If `True`, returns a `SparseTensor` instead of
+            a dense `Tensor`. Defaults to `False`.
+
+    Examples:
+
+    Discretize float values based on provided buckets.
+    >>> input = np.array([[-1.5, 1.0, 3.4, .5], [0.0, 3.0, 1.3, 0.0]])
+    >>> layer = Discretization(bin_boundaries=[0., 1., 2.])
+    >>> layer(input)
+    array([[0, 2, 3, 1],
+           [1, 3, 2, 1]])
+
+    Discretize float values based on a number of buckets to compute.
+    >>> input = np.array([[-1.5, 1.0, 3.4, .5], [0.0, 3.0, 1.3, 0.0]])
+    >>> layer = Discretization(num_bins=4, epsilon=0.01)
+    >>> layer.adapt(input)
+    >>> layer(input)
+    array([[0, 2, 3, 2],
+           [1, 3, 3, 1]])
+    """
 
-    `batch_dot` is used to compute dot product of `x` and `y` when
-    `x` and `y` are data in batch, i.e. in a shape of `(batch_size, :)`.
-    `batch_dot` results in a tensor or variable with less dimensions
-    than the input. If the number of dimensions is reduced to 1,
-    we use `expand_dims` to make sure that ndim is at least 2.
-
-    Shape inference:
-
-    Let `x`'s shape be `(100, 20)` and `y`'s shape be `(100, 30, 20)`.
-    If `axes` is (1, 2), to find the output shape of resultant tensor,
-    loop through each dimension in `x`'s shape and `y`'s shape:
-
-    * `x.shape[0]` : 100 : append to output shape
-    * `x.shape[1]` : 20 : do not append to output shape, dimension 1 of
-        `x` has been summed over. (`dot_axes[0]` = 1)
-    * `y.shape[0]` : 100 : do not append to output shape, always ignore
-        first dimension of `y`
-    * `y.shape[1]` : 30 : append to output shape
-    * `y.shape[2]` : 20 : do not append to output shape, dimension 2 of
-        `y` has been summed over.
-        (`dot_axes[1]` = 2) `output_shape` = `(100, 30)`
-
-    Example:
-
-    >>> x_batch = np.ones(shape=(32, 20, 1))
-    >>> y_batch = np.ones(shape=(32, 30, 20))
-    >>> xy_batch_dot = batch_dot(x_batch, y_batch, axes=(1, 2))
+    def __init__(
+        self,
+        bin_boundaries=None,
+        num_bins=None,
+        epsilon=0.01,
+        output_mode="int",
+        sparse=False,
+        dtype=None,
+        name=None,
+    ):
+        if dtype is None:
+            dtype = "int64" if output_mode == "int" else backend.floatx()
 
-    Args:
-        x: Keras tensor or variable with `ndim >= 2`.
-        y: Keras tensor or variable with `ndim >= 2`.
-        axes: Tuple or list of integers with target dimensions, or single
-            integer. The sizes of `x.shape[axes[0]]` and `y.shape[axes[1]]`
-            should be equal.
+        super().__init__(name=name, dtype=dtype)
 
-    Returns:
-        A tensor with shape equal to the concatenation of `x`'s shape
-        (less the dimension that was summed over) and `y`'s shape (less the
-        batch dimension and the dimension that was summed over). If the final
-        rank is 1, we reshape it to `(batch_size, 1)`.
-    """
+        if sparse and not backend.SUPPORTS_SPARSE_TENSORS:
+            raise ValueError(
+                f"`sparse=True` cannot be used with backend {backend.backend()}"
+            )
+        if sparse and output_mode == "int":
+            raise ValueError(
+                "`sparse=True` may only be used if `output_mode` is "
+                "`'one_hot'`, `'multi_hot'`, or `'count'`. "
+                f"Received: sparse={sparse} and "
+                f"output_mode={output_mode}"
+            )
 
-    x_shape = x.shape
-    y_shape = y.shape
+        argument_validation.validate_string_arg(
+            output_mode,
+            allowable_strings=(
+                "int",
+                "one_hot",
+                "multi_hot",
+                "count",
+            ),
+            caller_name=self.__class__.__name__,
+            arg_name="output_mode",
+        )
 
-    x_ndim = len(x_shape)
-    y_ndim = len(y_shape)
+        if num_bins is not None and num_bins < 0:
+            raise ValueError(
+                "`num_bins` must be greater than or equal to 0. "
+                f"Received: `num_bins={num_bins}`"
+            )
+        if num_bins is not None and bin_boundaries is not None:
+            if len(bin_boundaries) != num_bins - 1:
+                raise ValueError(
+                    "Both `num_bins` and `bin_boundaries` should not be "
+                    f"set. Received: `num_bins={num_bins}` and "
+                    f"`bin_boundaries={bin_boundaries}`"
+                )
 
-    if x_ndim < 2 or y_ndim < 2:
-        raise ValueError(
-            f"Cannot do batch_dot on inputs "
-            f"with rank < 2. "
-            f"Received inputs with shapes "
-            f"{x_shape} and {y_shape}."
+        self.input_bin_boundaries = bin_boundaries
+        self.bin_boundaries = (
+            bin_boundaries if bin_boundaries is not None else []
         )
+        self.num_bins = num_bins
+        self.epsilon = epsilon
+        self.output_mode = output_mode
+        self.sparse = sparse
+
+        if self.bin_boundaries:
+            self.summary = None
+        else:
+            self.summary = np.array([[], []], dtype="float32")
 
-    x_batch_size = x_shape[0]
-    y_batch_size = y_shape[0]
+    def build(self, input_shape=None):
+        self.built = True
 
-    if x_batch_size is not None and y_batch_size is not None:
-        if x_batch_size != y_batch_size:
+    @property
+    def input_dtype(self):
+        return backend.floatx()
+
+    def adapt(self, data, steps=None):
+        """Computes bin boundaries from quantiles in a input dataset.
+
+        Calling `adapt()` on a `Discretization` layer is an alternative to
+        passing in a `bin_boundaries` argument during construction. A
+        `Discretization` layer should always be either adapted over a dataset or
+        passed `bin_boundaries`.
+
+        During `adapt()`, the layer will estimate the quantile boundaries of the
+        input dataset. The number of quantiles can be controlled via the
+        `num_bins` argument, and the error tolerance for quantile boundaries can
+        be controlled via the `epsilon` argument.
+
+        Arguments:
+            data: The data to train on. It can be passed either as a
+                batched `tf.data.Dataset`,
+                or as a NumPy array.
+            steps: Integer or `None`.
+                Total number of steps (batches of samples) to process.
+                If `data` is a `tf.data.Dataset`, and `steps` is `None`,
+                `adapt()` will run until the input dataset is exhausted.
+                When passing an infinitely
+                repeating dataset, you must specify the `steps` argument. This
+                argument is not supported with array inputs or list inputs.
+        """
+        if self.input_bin_boundaries is not None:
             raise ValueError(
-                f"Cannot do batch_dot on inputs "
-                f"with different batch sizes. "
-                f"Received inputs with shapes "
-                f"{x_shape} and {y_shape}."
+                "Cannot adapt a Discretization layer that has been initialized "
+                "with `bin_boundaries`, use `num_bins` instead."
             )
-    if isinstance(axes, int):
-        axes = [axes, axes]
-
-    if axes is None:
-        if y_ndim == 2:
-            axes = [x_ndim - 1, y_ndim - 1]
+        self.reset_state()
+        if isinstance(data, tf.data.Dataset):
+            if steps is not None:
+                data = data.take(steps)
+            for batch in data:
+                self.update_state(batch)
         else:
-            axes = [x_ndim - 1, y_ndim - 2]
+            self.update_state(data)
+        self.finalize_state()
 
-    if any(isinstance(a, (list, tuple)) for a in axes):
-        raise ValueError(
-            f"Multiple target dimensions are not supported. "
-            f"Expected: None, int, (int, int), "
-            f"Provided: {axes} "
-        )
+    def update_state(self, data):
+        data = np.array(data).astype("float32")
+        summary = summarize(data, self.epsilon)
+        self.summary = merge_summaries(summary, self.summary, self.epsilon)
+
+    def finalize_state(self):
+        if self.input_bin_boundaries is not None:
+            return
+        self.bin_boundaries = get_bin_boundaries(
+            self.summary, self.num_bins
+        ).tolist()
+
+    def reset_state(self):
+        if self.input_bin_boundaries is not None:
+            return
+        self.summary = np.array([[], []], dtype="float32")
 
-    # if tuple, convert to list.
-    axes = list(axes)
+    def compute_output_spec(self, inputs):
+        return backend.KerasTensor(shape=inputs.shape, dtype=self.compute_dtype)
 
-    # convert negative indices.
-    if axes[0] < 0:
-        axes[0] += x_ndim
-    if axes[1] < 0:
-        axes[1] += y_ndim
-
-    # sanity checks
-    if 0 in axes:
-        raise ValueError(
-            "Cannot perform batch_dot over axis 0. "
-            "If your inputs are not batched, "
-            "add a dummy batch dimension to your "
-            "inputs using keras.ops.expand_dims(x, 0)"
-        )
-    a0, a1 = axes
-    d1 = x_shape[a0]
-    d2 = y_shape[a1]
-
-    if d1 is not None and d2 is not None and d1 != d2:
-        raise ValueError(
-            f"Cannot do batch_dot on inputs with shapes "
-            f"{x_shape} and {y_shape} with axes={axes}. "
-            f"x.shape[{axes[0]}] != y.shape[{axes[1]}] ({d1} != {d2})."
+    def load_own_variables(self, store):
+        if len(store) == 1:
+            # Legacy format case
+            self.summary = store["0"]
+        return
+
+    def call(self, inputs):
+        indices = self.backend.numpy.digitize(inputs, self.bin_boundaries)
+        return numerical_utils.encode_categorical_inputs(
+            indices,
+            output_mode=self.output_mode,
+            depth=len(self.bin_boundaries) + 1,
+            dtype=self.compute_dtype,
+            sparse=self.sparse,
+            backend_module=self.backend,
         )
 
-    # backup ndims. Need them later.
-    orig_x_ndim = x_ndim
-    orig_y_ndim = y_ndim
-
-    # if rank is 2, expand to 3.
-    if x_ndim == 2:
-        x = ops.expand_dims(x, 1)
-        a0 += 1
-        x_ndim += 1
-    if y_ndim == 2:
-        y = ops.expand_dims(y, 2)
-        y_ndim += 1
-
-    # bring x's dimension to be reduced to last axis.
-    if a0 != x_ndim - 1:
-        pattern = list(range(x_ndim))
-        for i in range(a0, x_ndim - 1):
-            pattern[i] = pattern[i + 1]
-        pattern[-1] = a0
-        x = ops.transpose(x, pattern)
-
-    # bring y's dimension to be reduced to axis 1.
-    if a1 != 1:
-        pattern = list(range(y_ndim))
-        for i in range(a1, 1, -1):
-            pattern[i] = pattern[i - 1]
-        pattern[1] = a1
-        y = ops.transpose(y, pattern)
-
-    # normalize both inputs to rank 3.
-    if x_ndim > 3:
-        # squash middle dimensions of x.
-        x_shape = ops.shape(x)
-        x_mid_dims = x_shape[1:-1]
-        x_squashed_shape = (x_shape[0], -1, x_shape[-1])
-        x = ops.reshape(x, x_squashed_shape)
-        x_squashed = True
-    else:
-        x_squashed = False
-
-    if y_ndim > 3:
-        # squash trailing dimensions of y.
-        y_shape = ops.shape(y)
-        y_trail_dims = y_shape[2:]
-        y_squashed_shape = (y_shape[0], y_shape[1], -1)
-        y = ops.reshape(y, y_squashed_shape)
-        y_squashed = True
-    else:
-        y_squashed = False
-
-    result = ops.matmul(x, y)
-
-    # if inputs were squashed, we have to reshape the matmul output.
-    output_shape = ops.shape(result)
-    do_reshape = False
-
-    if x_squashed:
-        output_shape = output_shape[:1] + x_mid_dims + output_shape[-1:]
-        do_reshape = True
-
-    if y_squashed:
-        output_shape = output_shape[:-1] + y_trail_dims
-        do_reshape = True
-
-    if do_reshape:
-        result = ops.reshape(result, output_shape)
-
-    # if the inputs were originally rank 2, we remove the added 1 dim.
-    if orig_x_ndim == 2:
-        result = ops.squeeze(result, 1)
-    elif orig_y_ndim == 2:
-        result = ops.squeeze(result, -1)
-
-    return result
-
-
-@keras_export("keras.layers.Dot")
-class Dot(Merge):
-    """Computes element-wise dot product of two tensors.
-
-    It takes a list of inputs of size 2, and the axes
-    corresponding to each input along with the dot product
-    is to be performed.
-
-    Let's say `x` and `y` are the two input tensors with shapes
-    `(2, 3, 5)` and `(2, 10, 3)`. The batch dimension should be
-    of same size for both the inputs, and `axes` should correspond
-    to the dimensions that have the same size in the corresponding
-    inputs. e.g. with `axes=(1, 2)`, the dot product of `x`, and `y`
-    will result in a tensor with shape `(2, 5, 10)`
-
-    Example:
-
-    >>> x = np.arange(10).reshape(1, 5, 2)
-    >>> y = np.arange(10, 20).reshape(1, 2, 5)
-    >>> keras.layers.Dot(axes=(1, 2))([x, y])
-
-    Usage in a Keras model:
-
-    >>> x1 = keras.layers.Dense(8)(np.arange(10).reshape(5, 2))
-    >>> x2 = keras.layers.Dense(8)(np.arange(10, 20).reshape(5, 2))
-    >>> y = keras.layers.Dot(axes=1)([x1, x2])
+    def get_config(self):
+        return {
+            "bin_boundaries": self.bin_boundaries,
+            "num_bins": self.num_bins,
+            "epsilon": self.epsilon,
+            "output_mode": self.output_mode,
+            "sparse": self.sparse,
+            "name": self.name,
+            "dtype": self.dtype,
+        }
+
+
+def summarize(values, epsilon):
+    """Reduce a 1D sequence of values to a summary.
+
+    This algorithm is based on numpy.quantiles but modified to allow for
+    intermediate steps between multiple data sets. It first finds the target
+    number of bins as the reciprocal of epsilon and then takes the individual
+    values spaced at appropriate intervals to arrive at that target.
+    The final step is to return the corresponding counts between those values
+    If the target num_bins is larger than the size of values, the whole array is
+    returned (with weights of 1).
 
     Args:
-        axes: Integer or tuple of integers, axis or axes along which to
-            take the dot product. If a tuple, should be two integers
-            corresponding to the desired axis from the first input and the
-            desired axis from the second input, respectively. Note that the
-            size of the two selected axes must match.
-        normalize: Whether to L2-normalize samples along the dot product axis
-            before taking the dot product. If set to `True`, then
-            the output of the dot product is the cosine proximity
-            between the two samples.
-        **kwargs: Standard layer keyword arguments.
+        values: 1D `np.ndarray` to be summarized.
+        epsilon: A `'float32'` that determines the approximate desired
+        precision.
 
     Returns:
-        A tensor, the dot product of the samples from the inputs.
+        A 2D `np.ndarray` that is a summary of the inputs. First column is the
+        interpolated partition values, the second is the weights (counts).
     """
+    values = np.reshape(values, [-1])
+    values = np.sort(values)
+    elements = np.size(values)
+    num_buckets = 1.0 / epsilon
+    increment = elements / num_buckets
+    start = increment
+    step = max(increment, 1)
+    boundaries = values[int(start) :: int(step)]
+    weights = np.ones_like(boundaries)
+    weights = weights * step
+    return np.stack([boundaries, weights])
 
-    def __init__(self, axes, normalize=False, **kwargs):
-        super().__init__(**kwargs)
-        if not isinstance(axes, int):
-            if not isinstance(axes, (list, tuple)):
-                raise TypeError(
-                    f"Invalid type for argument `axes`: it should be "
-                    f"a list or an int. Received: axes={axes}"
-                )
-            if len(axes) != 2:
-                raise ValueError(
-                    f"Invalid format for argument `axes`: it should contain "
-                    f"two elements. Received: axes={axes}"
-                )
-            if not isinstance(axes[0], int) or not isinstance(axes[1], int):
-                raise ValueError(
-                    f"Invalid format for argument `axes`: list elements should "
-                    f"be integers. Received: axes={axes}"
-                )
-        self.axes = axes
-        self.normalize = normalize
-        self.supports_masking = True
-        self._reshape_required = False
-
-    def build(self, input_shape):
-        # Used purely for shape validation.
-        if (
-            not isinstance(input_shape[0], (tuple, list))
-            or len(input_shape) != 2
-        ):
-            raise ValueError(
-                f"A `Dot` layer should be called on a list of 2 inputs. "
-                f"Received: input_shape={input_shape}"
-            )
-        shape1 = input_shape[0]
-        shape2 = input_shape[1]
-        if shape1 is None or shape2 is None:
-            return
-        if isinstance(self.axes, int):
-            if self.axes < 0:
-                axes = [self.axes % len(shape1), self.axes % len(shape2)]
-            else:
-                axes = [self.axes] * 2
-        else:
-            axes = self.axes
-        if shape1[axes[0]] != shape2[axes[1]]:
-            raise ValueError(
-                f"Incompatible input shapes: "
-                f"axis values {shape1[axes[0]]} (at axis {axes[0]}) != "
-                f"{shape2[axes[1]]} (at axis {axes[1]}). "
-                f"Full input shapes: {shape1}, {shape2}"
-            )
-        self.built = True
 
-    def _merge_function(self, inputs):
-        if len(inputs) != 2:
-            raise ValueError(
-                f"A `Dot` layer should be called on exactly 2 inputs. "
-                f"Received: inputs={inputs}"
-            )
-        x1 = inputs[0]
-        x2 = inputs[1]
+def merge_summaries(prev_summary, next_summary, epsilon):
+    """Weighted merge sort of summaries.
 
-        if isinstance(self.axes, int):
-            if self.axes < 0:
-                axes = [
-                    self.axes % len(x1.shape),
-                    self.axes % len(x2.shape),
-                ]
-            else:
-                axes = [self.axes] * 2
-        else:
-            axes = []
-            for i in range(len(self.axes)):
-                if self.axes[i] < 0:
-                    axes.append(self.axes[i] % len(inputs[i].shape))
-                else:
-                    axes.append(self.axes[i])
-
-        if self.normalize:
-            x1 = normalize(x1, axis=axes[0])
-            x2 = normalize(x2, axis=axes[1])
-        output = batch_dot(x1, x2, axes)
-        return output
+    Given two summaries of distinct data, this function merges (and compresses)
+    them to stay within `epsilon` error tolerance.
 
-    def compute_output_shape(self, input_shape):
-        if not isinstance(input_shape, (tuple, list)) or len(input_shape) != 2:
-            raise ValueError(
-                f"A `Dot` layer should be called on a list of 2 inputs. "
-                f"Received: input_shape={input_shape}"
-            )
-        shape1 = list(input_shape[0])
-        shape2 = list(input_shape[1])
-        if isinstance(self.axes, int):
-            if self.axes < 0:
-                axes = [self.axes % len(shape1), self.axes % len(shape2)]
-            else:
-                axes = [self.axes] * 2
-        else:
-            axes = self.axes
-        shape1.pop(axes[0])
-        shape2.pop(axes[1])
-        shape2.pop(0)
-        output_shape = shape1 + shape2
-        if len(output_shape) == 1:
-            output_shape += [1]
-        return tuple(output_shape)
+    Args:
+        prev_summary: 2D `np.ndarray` summary to be merged with `next_summary`.
+        next_summary: 2D `np.ndarray` summary to be merged with `prev_summary`.
+        epsilon: A float that determines the approximate desired precision.
 
-    def compute_mask(self, inputs, mask=None):
-        return None
+    Returns:
+        A 2-D `np.ndarray` that is a merged summary. First column is the
+        interpolated partition values, the second is the weights (counts).
+    """
+    merged = np.concatenate((prev_summary, next_summary), axis=1)
+    merged = np.take(merged, np.argsort(merged[0]), axis=1)
+    return compress_summary(merged, epsilon)
 
-    def get_config(self):
-        config = {
-            "axes": self.axes,
-            "normalize": self.normalize,
-        }
-        base_config = super().get_config()
-        return dict(list(base_config.items()) + list(config.items()))
 
+def get_bin_boundaries(summary, num_bins):
+    return compress_summary(summary, 1.0 / num_bins)[0, :-1]
 
-@keras_export("keras.layers.dot")
-def dot(inputs, axes=-1, **kwargs):
-    """Functional interface to the `Dot` layer.
+
+def compress_summary(summary, epsilon):
+    """Compress a summary to within `epsilon` accuracy.
+
+    The compression step is needed to keep the summary sizes small after
+    merging, and also used to return the final target boundaries. It finds the
+    new bins based on interpolating cumulative weight percentages from the large
+    summary.  Taking the difference of the cumulative weights from the previous
+    bin's cumulative weight will give the new weight for that bin.
 
     Args:
-        inputs: A list of input tensors (at least 2).
-        axes: Integer or tuple of integers,
-            axis or axes along which to take the dot product.
-        normalize: Whether to L2-normalize samples along the
-            dot product axis before taking the dot product.
-            If set to `True`, then the output of the dot product
-            is the cosine proximity between the two samples.
-        **kwargs: Standard layer keyword arguments.
+        summary: 2D `np.ndarray` summary to be compressed.
+        epsilon: A `'float32'` that determines the approximate desired
+        precision.
 
     Returns:
-        A tensor, the dot product of the samples from the inputs.
+        A 2D `np.ndarray` that is a compressed summary. First column is the
+        interpolated partition values, the second is the weights (counts).
     """
-    return Dot(axes=axes, **kwargs)(inputs)
+    if summary.shape[1] * epsilon < 1:
+        return summary
+
+    percents = epsilon + np.arange(0.0, 1.0, epsilon)
+    cum_weights = summary[1].cumsum()
+    cum_weight_percents = cum_weights / cum_weights[-1]
+    new_bins = np.interp(percents, cum_weight_percents, summary[0])
+    cum_weights = np.interp(percents, cum_weight_percents, cum_weights)
+    new_weights = cum_weights - np.concatenate(
+        (np.array([0]), cum_weights[:-1])
+    )
+    summary = np.stack((new_bins, new_weights))
+    return summary.astype("float32")
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,337 +1,376 @@
+import functools
+import math
+
 import numpy as np
 
-from keras.src import backend
-from keras.src.api_export import keras_export
-from keras.src.layers.preprocessing.tf_data_layer import TFDataLayer
-from keras.src.utils import argument_validation
-from keras.src.utils import numerical_utils
-from keras.src.utils.module_utils import tensorflow as tf
-
-
-@keras_export("keras.layers.Discretization")
-class Discretization(TFDataLayer):
-    """A preprocessing layer which buckets continuous features by ranges.
-
-    This layer will place each element of its input data into one of several
-    contiguous ranges and output an integer index indicating which range each
-    element was placed in.
-
-    **Note:** This layer is safe to use inside a `tf.data` pipeline
-    (independently of which backend you're using).
-
-    Input shape:
-        Any array of dimension 2 or higher.
-
-    Output shape:
-        Same as input shape.
-
-    Arguments:
-        bin_boundaries: A list of bin boundaries.
-            The leftmost and rightmost bins
-            will always extend to `-inf` and `inf`,
-            so `bin_boundaries=[0., 1., 2.]`
-            generates bins `(-inf, 0.)`, `[0., 1.)`, `[1., 2.)`,
-            and `[2., +inf)`.
-            If this option is set, `adapt()` should not be called.
-        num_bins: The integer number of bins to compute.
-            If this option is set,
-            `adapt()` should be called to learn the bin boundaries.
-        epsilon: Error tolerance, typically a small fraction
-            close to zero (e.g. 0.01). Higher values of epsilon increase
-            the quantile approximation, and hence result in more
-            unequal buckets, but could improve performance
-            and resource consumption.
-        output_mode: Specification for the output of the layer.
-            Values can be `"int"`, `"one_hot"`, `"multi_hot"`, or
-            `"count"` configuring the layer as follows:
-            - `"int"`: Return the discretized bin indices directly.
-            - `"one_hot"`: Encodes each individual element in the
-                input into an array the same size as `num_bins`,
-                containing a 1 at the input's bin
-                index. If the last dimension is size 1, will encode on that
-                dimension.  If the last dimension is not size 1,
-                will append a new dimension for the encoded output.
-            - `"multi_hot"`: Encodes each sample in the input into a
-                single array the same size as `num_bins`,
-                containing a 1 for each bin index
-                index present in the sample.
-                Treats the last dimension as the sample
-                dimension, if input shape is `(..., sample_length)`,
-                output shape will be `(..., num_tokens)`.
-            - `"count"`: As `"multi_hot"`, but the int array contains
-                a count of the number of times the bin index appeared
-                in the sample.
-            Defaults to `"int"`.
-        sparse: Boolean. Only applicable to `"one_hot"`, `"multi_hot"`,
-            and `"count"` output modes. Only supported with TensorFlow
-            backend. If `True`, returns a `SparseTensor` instead of
-            a dense `Tensor`. Defaults to `False`.
-
-    Examples:
-
-    Discretize float values based on provided buckets.
-    >>> input = np.array([[-1.5, 1.0, 3.4, .5], [0.0, 3.0, 1.3, 0.0]])
-    >>> layer = Discretization(bin_boundaries=[0., 1., 2.])
-    >>> layer(input)
-    array([[0, 2, 3, 1],
-           [1, 3, 2, 1]])
-
-    Discretize float values based on a number of buckets to compute.
-    >>> input = np.array([[-1.5, 1.0, 3.4, .5], [0.0, 3.0, 1.3, 0.0]])
-    >>> layer = Discretization(num_bins=4, epsilon=0.01)
-    >>> layer.adapt(input)
-    >>> layer(input)
-    array([[0, 2, 3, 2],
-           [1, 3, 3, 1]])
-    """
+from keras.src import tree
+from keras.src.trainers.data_adapters import array_slicing
+from keras.src.trainers.data_adapters import data_adapter_utils
+from keras.src.trainers.data_adapters.data_adapter import DataAdapter
+
+
+class ArrayDataAdapter(DataAdapter):
+    """Adapter for array-like objects, e.g. TF/JAX Tensors, NumPy arrays."""
 
     def __init__(
         self,
-        bin_boundaries=None,
-        num_bins=None,
-        epsilon=0.01,
-        output_mode="int",
-        sparse=False,
-        dtype=None,
-        name=None,
+        x,
+        y=None,
+        sample_weight=None,
+        batch_size=None,
+        steps=None,
+        shuffle=False,
+        class_weight=None,
     ):
-        if dtype is None:
-            dtype = "int64" if output_mode == "int" else backend.floatx()
-
-        super().__init__(name=name, dtype=dtype)
-
-        if sparse and not backend.SUPPORTS_SPARSE_TENSORS:
+        if not can_convert_arrays((x, y, sample_weight)):
             raise ValueError(
-                f"`sparse=True` cannot be used with backend {backend.backend()}"
+                "Expected all elements of `x` to be array-like. "
+                f"Received invalid types: x={x}"
             )
-        if sparse and output_mode == "int":
-            raise ValueError(
-                "`sparse=True` may only be used if `output_mode` is "
-                "`'one_hot'`, `'multi_hot'`, or `'count'`. "
-                f"Received: sparse={sparse} and "
-                f"output_mode={output_mode}"
-            )
-
-        argument_validation.validate_string_arg(
-            output_mode,
-            allowable_strings=(
-                "int",
-                "one_hot",
-                "multi_hot",
-                "count",
-            ),
-            caller_name=self.__class__.__name__,
-            arg_name="output_mode",
-        )
 
-        if num_bins is not None and num_bins < 0:
-            raise ValueError(
-                "`num_bins` must be greater than or equal to 0. "
-                f"Received: `num_bins={num_bins}`"
-            )
-        if num_bins is not None and bin_boundaries is not None:
-            if len(bin_boundaries) != num_bins - 1:
+        if sample_weight is not None:
+            if class_weight is not None:
                 raise ValueError(
-                    "Both `num_bins` and `bin_boundaries` should not be "
-                    f"set. Received: `num_bins={num_bins}` and "
-                    f"`bin_boundaries={bin_boundaries}`"
+                    "You cannot `class_weight` and `sample_weight` "
+                    "at the same time."
                 )
+            if tree.is_nested(y):
+                if isinstance(sample_weight, (list, tuple, dict)):
+                    try:
+                        tree.assert_same_structure(y, sample_weight)
+                    except ValueError:
+                        raise ValueError(
+                            "You should provide one `sample_weight` array per "
+                            "output in `y`. The two structures did not match:\n"
+                            f"- y: {y}\n"
+                            f"- sample_weight: {sample_weight}\n"
+                        )
+                else:
+                    is_samplewise = len(sample_weight.shape) == 1 or (
+                        len(sample_weight.shape) == 2
+                        and sample_weight.shape[1] == 1
+                    )
+                    if not is_samplewise:
+                        raise ValueError(
+                            "For a model with multiple outputs, when providing "
+                            "a single `sample_weight` array, it should only "
+                            "have one scalar score per sample "
+                            "(i.e. shape `(num_samples,)`). If you want to use "
+                            "non-scalar sample weights, pass a `sample_weight` "
+                            "argument with one array per model output."
+                        )
+                    # Replicate the same sample_weight array on all outputs.
+                    sample_weight = tree.map_structure(
+                        lambda _: sample_weight, y
+                    )
+        if class_weight is not None:
+            if tree.is_nested(y):
+                raise ValueError(
+                    "`class_weight` is only supported for Models with a single "
+                    "output."
+                )
+            sample_weight = data_adapter_utils.class_weight_to_sample_weights(
+                y, class_weight
+            )
 
-        self.input_bin_boundaries = bin_boundaries
-        self.bin_boundaries = (
-            bin_boundaries if bin_boundaries is not None else []
+        inputs = data_adapter_utils.pack_x_y_sample_weight(x, y, sample_weight)
+
+        data_adapter_utils.check_data_cardinality(inputs)
+        num_samples = set(i.shape[0] for i in tree.flatten(inputs)).pop()
+        self._num_samples = num_samples
+        self._inputs = inputs
+
+        # If batch_size is not passed but steps is, calculate from the input
+        # data.  Defaults to `32` for backwards compatibility.
+        if not batch_size:
+            batch_size = int(math.ceil(num_samples / steps)) if steps else 32
+
+        self._size = int(math.ceil(num_samples / batch_size))
+        self._batch_size = batch_size
+        self._partial_batch_size = num_samples % batch_size
+        self._shuffle = shuffle
+
+    def get_numpy_iterator(self):
+        inputs = array_slicing.convert_to_sliceable(
+            self._inputs, target_backend="numpy"
         )
-        self.num_bins = num_bins
-        self.epsilon = epsilon
-        self.output_mode = output_mode
-        self.sparse = sparse
 
-        if self.bin_boundaries:
-            self.summary = None
-        else:
-            self.summary = np.array([[], []], dtype="float32")
+        def slice_and_convert_to_numpy(sliceable, indices=None):
+            x = sliceable[indices]
+            x = sliceable.convert_to_numpy(x)
+            return x
+
+        return self._get_iterator(slice_and_convert_to_numpy, inputs)
+
+    def get_tf_dataset(self):
+        from keras.src.utils.module_utils import tensorflow as tf
+
+        shuffle = self._shuffle
+        batch_size = self._batch_size
+        num_samples = self._num_samples
+        num_full_batches = int(self._num_samples // batch_size)
+
+        # Vectorized version of shuffle.
+        # This is a performance improvement over using `from_tensor_slices`.
+        # The indices of the data are shuffled and batched, and these indices
+        # are then zipped with the data and used to extract a batch of the data
+        # at each step. The performance improvements here come from:
+        # 1. vectorized batch using gather
+        # 2. parallelized map
+        # 3. pipelined permutation generation
+        # 4. optimized permutation batching
+        # 5. disabled static optimizations
+
+        indices_dataset = tf.data.Dataset.range(1)
+
+        def permutation(_):
+            # It turns out to be more performant to make a new set of indices
+            # rather than reusing the same range Tensor. (presumably because of
+            # buffer forwarding.)
+            indices = tf.range(num_samples, dtype=tf.int64)
+            if shuffle and shuffle != "batch":
+                indices = tf.random.shuffle(indices)
+            return indices
+
+        # We prefetch a single element. Computing large permutations can take
+        # quite a while so we don't want to wait for prefetching over an epoch
+        # boundary to trigger the next permutation. On the other hand, too many
+        # simultaneous shuffles can contend on a hardware level and degrade all
+        # performance.
+        indices_dataset = indices_dataset.map(permutation).prefetch(1)
+
+        def slice_batch_indices(indices):
+            """Convert a Tensor of indices into a dataset of batched indices.
+
+            This step can be accomplished in several ways. The most natural is
+            to slice the Tensor in a Dataset map. (With a condition on the upper
+            index to handle the partial batch.) However it turns out that
+            coercing the Tensor into a shape which is divisible by the batch
+            size (and handling the last partial batch separately) allows for a
+            much more favorable memory access pattern and improved performance.
+
+            Args:
+                indices: Tensor which determines the data order for an entire
+                    epoch.
+
+            Returns:
+                A Dataset of batched indices.
+            """
+            num_in_full_batch = num_full_batches * batch_size
+            first_k_indices = tf.slice(indices, [0], [num_in_full_batch])
+            first_k_indices = tf.reshape(
+                first_k_indices, [num_full_batches, batch_size]
+            )
 
-    def build(self, input_shape=None):
-        self.built = True
+            flat_dataset = tf.data.Dataset.from_tensor_slices(first_k_indices)
+            if self._partial_batch_size:
+                index_remainder = tf.data.Dataset.from_tensors(
+                    tf.slice(
+                        indices, [num_in_full_batch], [self._partial_batch_size]
+                    )
+                )
+                flat_dataset = flat_dataset.concatenate(index_remainder)
 
-    @property
-    def input_dtype(self):
-        return backend.floatx()
+            return flat_dataset
 
-    def adapt(self, data, steps=None):
-        """Computes bin boundaries from quantiles in a input dataset.
+        def slice_inputs(indices_dataset, inputs):
+            """Slice inputs into a Dataset of batches.
 
-        Calling `adapt()` on a `Discretization` layer is an alternative to
-        passing in a `bin_boundaries` argument during construction. A
-        `Discretization` layer should always be either adapted over a dataset or
-        passed `bin_boundaries`.
-
-        During `adapt()`, the layer will estimate the quantile boundaries of the
-        input dataset. The number of quantiles can be controlled via the
-        `num_bins` argument, and the error tolerance for quantile boundaries can
-        be controlled via the `epsilon` argument.
-
-        Arguments:
-            data: The data to train on. It can be passed either as a
-                batched `tf.data.Dataset`,
-                or as a NumPy array.
-            steps: Integer or `None`.
-                Total number of steps (batches of samples) to process.
-                If `data` is a `tf.data.Dataset`, and `steps` is `None`,
-                `adapt()` will run until the input dataset is exhausted.
-                When passing an infinitely
-                repeating dataset, you must specify the `steps` argument. This
-                argument is not supported with array inputs or list inputs.
-        """
-        if self.input_bin_boundaries is not None:
-            raise ValueError(
-                "Cannot adapt a Discretization layer that has been initialized "
-                "with `bin_boundaries`, use `num_bins` instead."
+            Given a Dataset of batch indices and the unsliced inputs,
+            this step slices the inputs in a parallelized fashion
+            and produces a dataset of input batches.
+
+            Args:
+                indices_dataset: A Dataset of batched indices.
+                inputs: A python data structure that contains the inputs,
+                    targets, and possibly sample weights.
+
+            Returns:
+                A Dataset of input batches matching the batch indices.
+            """
+            inputs = array_slicing.convert_to_sliceable(
+                self._inputs, target_backend="tensorflow"
             )
-        self.reset_state()
-        if isinstance(data, tf.data.Dataset):
-            if steps is not None:
-                data = data.take(steps)
-            for batch in data:
-                self.update_state(batch)
-        else:
-            self.update_state(data)
-        self.finalize_state()
+            inputs = tree.lists_to_tuples(inputs)
+
+            dataset = tf.data.Dataset.zip(
+                (indices_dataset, tf.data.Dataset.from_tensors(inputs).repeat())
+            )
+
+            def grab_batch(i, data):
+
+                def grab_one(x):
+                    if isinstance(x, array_slicing.TensorflowSparseWrapper):
+                        return array_slicing.slice_tensorflow_sparse_wrapper(
+                            x, i
+                        )
+                    if isinstance(x, (list, tuple, dict)):
+                        return None
+                    if tf.is_tensor(x):
+                        return tf.gather(x, i, axis=0)
+                    return x
+
+                return tree.traverse(grab_one, data)
 
-    def update_state(self, data):
-        data = np.array(data).astype("float32")
-        summary = summarize(data, self.epsilon)
-        self.summary = merge_summaries(summary, self.summary, self.epsilon)
-
-    def finalize_state(self):
-        if self.input_bin_boundaries is not None:
-            return
-        self.bin_boundaries = get_bin_boundaries(
-            self.summary, self.num_bins
-        ).tolist()
-
-    def reset_state(self):
-        if self.input_bin_boundaries is not None:
-            return
-        self.summary = np.array([[], []], dtype="float32")
-
-    def compute_output_spec(self, inputs):
-        return backend.KerasTensor(shape=inputs.shape, dtype=self.compute_dtype)
-
-    def load_own_variables(self, store):
-        if len(store) == 1:
-            # Legacy format case
-            self.summary = store["0"]
-        return
-
-    def call(self, inputs):
-        indices = self.backend.numpy.digitize(inputs, self.bin_boundaries)
-        return numerical_utils.encode_categorical_inputs(
-            indices,
-            output_mode=self.output_mode,
-            depth=len(self.bin_boundaries) + 1,
-            dtype=self.compute_dtype,
-            sparse=self.sparse,
-            backend_module=self.backend,
+            dataset = dataset.map(
+                grab_batch, num_parallel_calls=tf.data.AUTOTUNE
+            )
+
+            # Default optimizations are disabled to avoid the overhead of
+            # (unnecessary) input pipeline graph serialization & deserialization
+            options = tf.data.Options()
+            options.experimental_optimization.apply_default_optimizations = (
+                False
+            )
+            if self._shuffle:
+                options.experimental_external_state_policy = (
+                    tf.data.experimental.ExternalStatePolicy.IGNORE
+                )
+            dataset = dataset.with_options(options)
+            return dataset
+
+        indices_dataset = indices_dataset.flat_map(slice_batch_indices)
+        if shuffle == "batch":
+            indices_dataset = indices_dataset.map(tf.random.shuffle)
+
+        dataset = slice_inputs(indices_dataset, self._inputs)
+
+        options = tf.data.Options()
+        options.experimental_distribute.auto_shard_policy = (
+            tf.data.experimental.AutoShardPolicy.DATA
         )
+        dataset = dataset.with_options(options)
+        return dataset.prefetch(tf.data.AUTOTUNE)
 
-    def get_config(self):
-        return {
-            "bin_boundaries": self.bin_boundaries,
-            "num_bins": self.num_bins,
-            "epsilon": self.epsilon,
-            "output_mode": self.output_mode,
-            "sparse": self.sparse,
-            "name": self.name,
-            "dtype": self.dtype,
-        }
-
-
-def summarize(values, epsilon):
-    """Reduce a 1D sequence of values to a summary.
-
-    This algorithm is based on numpy.quantiles but modified to allow for
-    intermediate steps between multiple data sets. It first finds the target
-    number of bins as the reciprocal of epsilon and then takes the individual
-    values spaced at appropriate intervals to arrive at that target.
-    The final step is to return the corresponding counts between those values
-    If the target num_bins is larger than the size of values, the whole array is
-    returned (with weights of 1).
+    def get_jax_iterator(self):
+        from keras.src.backend.jax.core import convert_to_tensor
 
-    Args:
-        values: 1D `np.ndarray` to be summarized.
-        epsilon: A `'float32'` that determines the approximate desired
-        precision.
+        inputs = array_slicing.convert_to_sliceable(
+            self._inputs, target_backend="jax"
+        )
 
-    Returns:
-        A 2D `np.ndarray` that is a summary of the inputs. First column is the
-        interpolated partition values, the second is the weights (counts).
-    """
-    values = np.reshape(values, [-1])
-    values = np.sort(values)
-    elements = np.size(values)
-    num_buckets = 1.0 / epsilon
-    increment = elements / num_buckets
-    start = increment
-    step = max(increment, 1)
-    boundaries = values[int(start) :: int(step)]
-    weights = np.ones_like(boundaries)
-    weights = weights * step
-    return np.stack([boundaries, weights])
+        def slice_and_convert_to_jax(sliceable, indices=None):
+            x = sliceable[indices]
+            x = sliceable.convert_to_jax_compatible(x)
+            x = convert_to_tensor(x)
+            return x
+
+        return self._get_iterator(slice_and_convert_to_jax, inputs)
+
+    def get_torch_dataloader(self):
+        import torch
+
+        from keras.src.backend.torch.core import convert_to_tensor
+
+        class ArrayDataset(torch.utils.data.Dataset):
+            def __init__(self, array):
+                self.array = array
+
+            def __getitems__(self, indices):
+                def slice_and_convert(sliceable):
+                    x = sliceable[indices]
+                    x = sliceable.convert_to_torch_compatible(x)
+                    x = convert_to_tensor(x)
+                    return x
+
+                return tree.map_structure(slice_and_convert, self.array)
+
+            def __len__(self):
+                return len(self.array[0])
+
+        class RandomBatchSampler(torch.utils.data.Sampler):
+            def __init__(self, sampler):
+                self.sampler = sampler
+
+            def __iter__(self):
+                for batch in self.sampler:
+                    yield [batch[i] for i in torch.randperm(len(batch))]
+
+            def __len__(self):
+                return len(self.sampler)
+
+        if self._shuffle == "batch":
+            batch_sampler = RandomBatchSampler(
+                torch.utils.data.BatchSampler(
+                    range(self._num_samples),
+                    batch_size=self._batch_size,
+                    drop_last=False,
+                )
+            )
+        elif self._shuffle:
+            batch_sampler = torch.utils.data.BatchSampler(
+                torch.utils.data.RandomSampler(range(self._num_samples)),
+                batch_size=self._batch_size,
+                drop_last=False,
+            )
+        else:
+            batch_sampler = torch.utils.data.BatchSampler(
+                torch.utils.data.SequentialSampler(range(self._num_samples)),
+                batch_size=self._batch_size,
+                drop_last=False,
+            )
 
+        # Because ArrayDataset.__getitems__ returns full batches organized in
+        # the expected structure, there is nothing to collate.
+        def no_op_collate(batch):
+            return batch
 
-def merge_summaries(prev_summary, next_summary, epsilon):
-    """Weighted merge sort of summaries.
+        inputs = array_slicing.convert_to_sliceable(
+            self._inputs, target_backend="torch"
+        )
+        dataset = ArrayDataset(inputs)
+        return torch.utils.data.DataLoader(
+            dataset, batch_sampler=batch_sampler, collate_fn=no_op_collate
+        )
 
-    Given two summaries of distinct data, this function merges (and compresses)
-    them to stay within `epsilon` error tolerance.
+    def _get_iterator(self, slice_and_convert_fn, inputs):
+        global_permutation = None
+        if self._shuffle and self._shuffle != "batch":
+            global_permutation = np.random.permutation(self._num_samples)
+
+        for i in range(self._size):
+            start = i * self._batch_size
+            stop = min((i + 1) * self._batch_size, self._num_samples)
+            if self._shuffle == "batch":
+                indices = np.random.permutation(stop - start) + start
+            elif self._shuffle:
+                indices = global_permutation[start:stop]
+            else:
+                indices = slice(start, stop)
 
-    Args:
-        prev_summary: 2D `np.ndarray` summary to be merged with `next_summary`.
-        next_summary: 2D `np.ndarray` summary to be merged with `prev_summary`.
-        epsilon: A float that determines the approximate desired precision.
+            slice_indices_and_convert_fn = functools.partial(
+                slice_and_convert_fn, indices=indices
+            )
+            yield tree.map_structure(slice_indices_and_convert_fn, inputs)
 
-    Returns:
-        A 2-D `np.ndarray` that is a merged summary. First column is the
-        interpolated partition values, the second is the weights (counts).
-    """
-    merged = np.concatenate((prev_summary, next_summary), axis=1)
-    merged = np.take(merged, np.argsort(merged[0]), axis=1)
-    return compress_summary(merged, epsilon)
+    @property
+    def num_batches(self):
+        return self._size
 
+    @property
+    def batch_size(self):
+        return self._batch_size
 
-def get_bin_boundaries(summary, num_bins):
-    return compress_summary(summary, 1.0 / num_bins)[0, :-1]
+    @property
+    def has_partial_batch(self):
+        return self._partial_batch_size > 0
 
+    @property
+    def partial_batch_size(self):
+        return self._partial_batch_size or None
 
-def compress_summary(summary, epsilon):
-    """Compress a summary to within `epsilon` accuracy.
 
-    The compression step is needed to keep the summary sizes small after
-    merging, and also used to return the final target boundaries. It finds the
-    new bins based on interpolating cumulative weight percentages from the large
-    summary.  Taking the difference of the cumulative weights from the previous
-    bin's cumulative weight will give the new weight for that bin.
+def can_convert_arrays(arrays):
+    """Check if array like-inputs can be handled by `ArrayDataAdapter`
 
     Args:
-        summary: 2D `np.ndarray` summary to be compressed.
-        epsilon: A `'float32'` that determines the approximate desired
-        precision.
+        inputs: Structure of `Tensor`s, NumPy arrays, or tensor-like.
 
     Returns:
-        A 2D `np.ndarray` that is a compressed summary. First column is the
-        interpolated partition values, the second is the weights (counts).
+        `True` if `arrays` can be handled by `ArrayDataAdapter`, `False`
+        otherwise.
     """
-    if summary.shape[1] * epsilon < 1:
-        return summary
 
-    percents = epsilon + np.arange(0.0, 1.0, epsilon)
-    cum_weights = summary[1].cumsum()
-    cum_weight_percents = cum_weights / cum_weights[-1]
-    new_bins = np.interp(percents, cum_weight_percents, summary[0])
-    cum_weights = np.interp(percents, cum_weight_percents, cum_weights)
-    new_weights = cum_weights - np.concatenate(
-        (np.array([0]), cum_weights[:-1])
+    return all(
+        tree.flatten(tree.map_structure(array_slicing.can_slice_array, arrays))
     )
-    summary = np.stack((new_bins, new_weights))
-    return summary.astype("float32")
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/feature_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from keras.src import backend
 from keras.src import layers
 from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
+from keras.src.layers.preprocessing.tf_data_layer import TFDataLayer
 from keras.src.saving import saving_lib
 from keras.src.saving import serialization_lib
 from keras.src.utils import backend_utils
 from keras.src.utils.module_utils import tensorflow as tf
 from keras.src.utils.naming import auto_name
 
 
@@ -273,20 +274,16 @@
 
     @classmethod
     def feature(cls, dtype, preprocessor, output_mode):
         return Feature(dtype, preprocessor, output_mode)
 
     @classmethod
     def float(cls, name=None):
-        from keras.src.layers.core import identity
-
         name = name or auto_name("float")
-        preprocessor = identity.Identity(
-            dtype="float32", name=f"{name}_preprocessor"
-        )
+        preprocessor = TFDIdentity(dtype="float32", name=f"{name}_preprocessor")
         return Feature(
             dtype="float32", preprocessor=preprocessor, output_mode="float"
         )
 
     @classmethod
     def float_rescaled(cls, scale=1.0, offset=0.0, name=None):
         name = name or auto_name("float_rescaled")
@@ -663,15 +660,15 @@
                         "Consider using `output_mode='dict'`."
                     )
                 features_to_concat.append(feature)
             else:
                 output_dict[name] = feature
 
         if self.output_mode == "concat":
-            self.concat = layers.Concatenate(axis=-1)
+            self.concat = TFDConcat(axis=-1)
             return self.concat(features_to_concat)
         else:
             return output_dict
 
     def _check_if_adapted(self):
         if not self._is_adapted:
             if not self._list_adaptable_preprocessors():
@@ -730,15 +727,18 @@
             )
 
             merged_data = self._merge_features(preprocessed_data, crossed_data)
 
         if rebatched:
             if self.output_mode == "concat":
                 assert merged_data.shape[0] == 1
-                if backend.backend() != "tensorflow":
+                if (
+                    backend.backend() != "tensorflow"
+                    and not backend_utils.in_tf_graph()
+                ):
                     merged_data = backend.convert_to_numpy(merged_data)
                 merged_data = tf.squeeze(merged_data, axis=0)
             else:
                 for name, x in merged_data.items():
                     if len(x.shape) == 2 and x.shape[0] == 1:
                         merged_data[name] = tf.squeeze(x, axis=0)
 
@@ -792,7 +792,21 @@
         saving_lib.save_model(self, filepath)
 
     def save_own_variables(self, store):
         return
 
     def load_own_variables(self, store):
         return
+
+
+class TFDConcat(TFDataLayer):
+    def __init__(self, axis, **kwargs):
+        super().__init__(**kwargs)
+        self.axis = axis
+
+    def call(self, xs):
+        return self.backend.numpy.concatenate(xs, axis=self.axis)
+
+
+class TFDIdentity(TFDataLayer):
+    def call(self, x):
+        return x
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/normalization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import math
 
 import numpy as np
 
 from keras.src import backend
 from keras.src import ops
 from keras.src.api_export import keras_export
-from keras.src.layers.layer import Layer
+from keras.src.layers.preprocessing.tf_data_layer import TFDataLayer
 from keras.src.utils.module_utils import tensorflow as tf
 
 
 @keras_export("keras.layers.Normalization")
-class Normalization(Layer):
+class Normalization(TFDataLayer):
     """A preprocessing layer that normalizes continuous features.
 
     This layer will shift and scale inputs into a distribution centered around
     0 with standard deviation 1. It accomplishes this by precomputing the mean
     and variance of the data, and calling `(input - mean) / sqrt(var)` at
     runtime.
 
@@ -102,25 +102,27 @@
             axis = ()
         elif isinstance(axis, int):
             axis = (axis,)
         else:
             axis = tuple(axis)
         self.axis = axis
 
+        self.input_mean = mean
+        self.input_variance = variance
+        self.invert = invert
+        self.supports_masking = True
+        self._build_input_shape = None
+        self.mean = None
+
         # Set `mean` and `variance` if passed.
         if (mean is not None) != (variance is not None):
             raise ValueError(
                 "When setting values directly, both `mean` and `variance` "
                 f"must be set. Received: mean={mean} and variance={variance}"
             )
-        self.input_mean = mean
-        self.input_variance = variance
-        self.invert = invert
-        self.supports_masking = True
-        self._build_input_shape = None
 
     def build(self, input_shape):
         if input_shape is None:
             return
 
         ndim = len(input_shape)
         self._build_input_shape = input_shape
@@ -288,27 +290,43 @@
         # proper broadcast shape and dtype each time `finalize_state` is called.
         self.mean = ops.reshape(self.adapt_mean, self._broadcast_shape)
         self.mean = ops.cast(self.mean, self.compute_dtype)
         self.variance = ops.reshape(self.adapt_variance, self._broadcast_shape)
         self.variance = ops.cast(self.variance, self.compute_dtype)
 
     def call(self, inputs):
-        inputs = backend.convert_to_tensor(inputs, dtype=self.compute_dtype)
+        # This layer can be called in tf.data
+        # even with another backend after it has been adapted.
+        # However it must use backend-native logic for adapt().
+        if self.mean is None:
+            # May happen when in tf.data when mean/var was passed explicitly
+            raise ValueError(
+                "You must call `.build(input_shape)` "
+                "on the layer before using it."
+            )
+        inputs = self.backend.core.convert_to_tensor(
+            inputs, dtype=self.compute_dtype
+        )
         if self.invert:
-            return ops.add(
+            return self.backend.numpy.add(
                 self.mean,
-                ops.multiply(
+                self.backend.numpy.multiply(
                     inputs,
-                    ops.maximum(ops.sqrt(self.variance), backend.epsilon()),
+                    self.backend.numpy.maximum(
+                        self.backend.numpy.sqrt(self.variance),
+                        backend.epsilon(),
+                    ),
                 ),
             )
         else:
-            return ops.divide(
-                ops.subtract(inputs, self.mean),
-                ops.maximum(ops.sqrt(self.variance), backend.epsilon()),
+            return self.backend.numpy.divide(
+                self.backend.numpy.subtract(inputs, self.mean),
+                self.backend.numpy.maximum(
+                    self.backend.numpy.sqrt(self.variance), backend.epsilon()
+                ),
             )
 
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         config = super().get_config()
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         return outputs
 
     def call(self, inputs, training=True):
         inputs = self.backend.cast(inputs, self.compute_dtype)
         if training:
             rotation_matrix = self._get_rotation_matrix(inputs)
             transformed_image = self.backend.image.affine_transform(
-                image=inputs,
+                images=inputs,
                 transform=rotation_matrix,
                 interpolation=self.interpolation,
                 fill_mode=self.fill_mode,
                 fill_value=self.fill_value,
                 data_format=self.data_format,
             )
             return transformed_image
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/string_lookup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -312,14 +312,15 @@
                 "Layer StringLookup requires TensorFlow. "
                 "Install it via `pip install tensorflow`."
             )
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
                 "`sparse=True` can only be used with the " "TensorFlow backend."
             )
+        self.encoding = encoding
         super().__init__(
             max_tokens=max_tokens,
             num_oov_indices=num_oov_indices,
             mask_token=mask_token,
             oov_token=oov_token,
             vocabulary=vocabulary,
             idf_weights=idf_weights,
@@ -327,15 +328,14 @@
             output_mode=output_mode,
             pad_to_max_tokens=pad_to_max_tokens,
             sparse=sparse,
             name=name,
             vocabulary_dtype="string",
             **kwargs,
         )
-        self.encoding = encoding
         self._convert_input_args = False
         self._allow_non_tensor_positional_args = True
         self.supports_jit = False
 
     def adapt(self, data, steps=None):
         """Computes a vocabulary of integer terms from tokens in a dataset.
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/backend.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/layers.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/losses.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/losses/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/losses/loss.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/losses/losses.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/metric.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/models/cloning.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/models/functional.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/models/model.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/models/sequential.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/core.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/function.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/image.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/image.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,77 +4,54 @@
 from keras.src.backend import KerasTensor
 from keras.src.backend import any_symbolic_tensors
 from keras.src.ops.operation import Operation
 from keras.src.ops.operation_utils import compute_conv_output_shape
 
 
 class RGBToGrayscale(Operation):
-    def __init__(
-        self,
-        data_format="channels_last",
-    ):
+    def __init__(self, data_format=None):
         super().__init__()
-        self.data_format = data_format
+        self.data_format = backend.standardize_data_format(data_format)
 
-    def call(self, image):
+    def call(self, images):
         return backend.image.rgb_to_grayscale(
-            image,
-            data_format=self.data_format,
+            images, data_format=self.data_format
         )
 
-    def compute_output_spec(self, image):
-        if len(image.shape) not in (3, 4):
+    def compute_output_spec(self, images):
+        images_shape = list(images.shape)
+        if len(images_shape) not in (3, 4):
             raise ValueError(
-                "Invalid image rank: expected rank 3 (single image) "
-                "or rank 4 (batch of images). Received input with shape: "
-                f"image.shape={image.shape}"
+                "Invalid images rank: expected rank 3 (single image) "
+                "or rank 4 (batch of images). "
+                f"Received: images.shape={images_shape}"
             )
-
-        if len(image.shape) == 3:
-            if self.data_format == "channels_last":
-                return KerasTensor(image.shape[:-1] + (1,), dtype=image.dtype)
-            else:
-                return KerasTensor((1,) + image.shape[1:], dtype=image.dtype)
-        elif len(image.shape) == 4:
-            if self.data_format == "channels_last":
-                return KerasTensor(
-                    (image.shape[0],) + image.shape[1:-1] + (1,),
-                    dtype=image.dtype,
-                )
-            else:
-                return KerasTensor(
-                    (
-                        image.shape[0],
-                        1,
-                    )
-                    + image.shape[2:],
-                    dtype=image.dtype,
-                )
+        if self.data_format == "channels_last":
+            images_shape[-1] = 1
+        else:
+            images_shape[-3] = 1
+        return KerasTensor(shape=images_shape, dtype=images.dtype)
 
 
 @keras_export("keras.ops.image.rgb_to_grayscale")
-def rgb_to_grayscale(
-    image,
-    data_format="channels_last",
-):
+def rgb_to_grayscale(images, data_format=None):
     """Convert RGB images to grayscale.
 
     This function converts RGB images to grayscale images. It supports both
     3D and 4D tensors, where the last dimension represents channels.
 
     Args:
-        image: Input RGB image or batch of RGB images. Must be a 3D tensor
-            with shape `(height, width, channels)` or a 4D tensor with shape
-            `(batch, height, width, channels)`.
+        images: Input image or batch of images. Must be 3D or 4D.
         data_format: A string specifying the data format of the input tensor.
             It can be either `"channels_last"` or `"channels_first"`.
             `"channels_last"` corresponds to inputs with shape
             `(batch, height, width, channels)`, while `"channels_first"`
             corresponds to inputs with shape `(batch, channels, height, width)`.
-            Defaults to `"channels_last"`.
+            If not specified, the value will be interpreted by
+            `keras.config.image_data_format`. Defaults to `None`.
 
     Returns:
         Grayscale image or batch of grayscale images.
 
     Examples:
 
     >>> import numpy as np
@@ -90,98 +67,87 @@
     (4, 4, 1)
 
     >>> x = np.random.random((2, 3, 4, 4))
     >>> y = ops.image.rgb_to_grayscale(x, data_format="channels_first")
     >>> y.shape
     (2, 1, 4, 4)
     """
-    if any_symbolic_tensors((image,)):
-        return RGBToGrayscale(
-            data_format=data_format,
-        ).symbolic_call(image)
-    return backend.image.rgb_to_grayscale(
-        image,
-        data_format=data_format,
-    )
+    if any_symbolic_tensors((images,)):
+        return RGBToGrayscale(data_format=data_format).symbolic_call(images)
+    return backend.image.rgb_to_grayscale(images, data_format=data_format)
 
 
 class Resize(Operation):
     def __init__(
         self,
         size,
         interpolation="bilinear",
         antialias=False,
         crop_to_aspect_ratio=False,
         pad_to_aspect_ratio=False,
         fill_mode="constant",
         fill_value=0.0,
-        data_format="channels_last",
+        data_format=None,
     ):
         super().__init__()
         self.size = tuple(size)
         self.interpolation = interpolation
         self.antialias = antialias
-        self.data_format = data_format
         self.crop_to_aspect_ratio = crop_to_aspect_ratio
         self.pad_to_aspect_ratio = pad_to_aspect_ratio
         self.fill_mode = fill_mode
         self.fill_value = fill_value
+        self.data_format = backend.standardize_data_format(data_format)
 
-    def call(self, image):
+    def call(self, images):
         return backend.image.resize(
-            image,
+            images,
             self.size,
             interpolation=self.interpolation,
             antialias=self.antialias,
             data_format=self.data_format,
             crop_to_aspect_ratio=self.crop_to_aspect_ratio,
             pad_to_aspect_ratio=self.pad_to_aspect_ratio,
             fill_mode=self.fill_mode,
             fill_value=self.fill_value,
         )
 
-    def compute_output_spec(self, image):
-        if len(image.shape) == 3:
-            return KerasTensor(
-                self.size + (image.shape[-1],), dtype=image.dtype
+    def compute_output_spec(self, images):
+        images_shape = list(images.shape)
+        if len(images_shape) not in (3, 4):
+            raise ValueError(
+                "Invalid images rank: expected rank 3 (single image) "
+                "or rank 4 (batch of images). Received input with shape: "
+                f"images.shape={images.shape}"
             )
-        elif len(image.shape) == 4:
-            if self.data_format == "channels_last":
-                return KerasTensor(
-                    (image.shape[0],) + self.size + (image.shape[-1],),
-                    dtype=image.dtype,
-                )
-            else:
-                return KerasTensor(
-                    (image.shape[0], image.shape[1]) + self.size,
-                    dtype=image.dtype,
-                )
-        raise ValueError(
-            "Invalid input rank: expected rank 3 (single image) "
-            "or rank 4 (batch of images). Received input with shape: "
-            f"image.shape={image.shape}"
-        )
+        if self.data_format == "channels_last":
+            height_axis, width_axis = -3, -2
+        else:
+            height_axis, width_axis = -2, -1
+        images_shape[height_axis] = self.size[0]
+        images_shape[width_axis] = self.size[1]
+        return KerasTensor(shape=images_shape, dtype=images.dtype)
 
 
 @keras_export("keras.ops.image.resize")
 def resize(
-    image,
+    images,
     size,
     interpolation="bilinear",
     antialias=False,
     crop_to_aspect_ratio=False,
     pad_to_aspect_ratio=False,
     fill_mode="constant",
     fill_value=0.0,
-    data_format="channels_last",
+    data_format=None,
 ):
     """Resize images to size using the specified interpolation method.
 
     Args:
-        image: Input image or batch of images. Must be 3D or 4D.
+        images: Input image or batch of images. Must be 3D or 4D.
         size: Size of output image in `(height, width)` format.
         interpolation: Interpolation method. Available methods are `"nearest"`,
             `"bilinear"`, and `"bicubic"`. Defaults to `"bilinear"`.
         antialias: Whether to use an antialiasing filter when downsampling an
             image. Defaults to `False`.
         crop_to_aspect_ratio: If `True`, resize the images without aspect
             ratio distortion. When the original aspect ratio differs
@@ -195,22 +161,21 @@
             from the target aspect ratio, the output image will be
             evenly padded on the short side.
         fill_mode: When using `pad_to_aspect_ratio=True`, padded areas
             are filled according to the given mode. Only `"constant"` is
             supported at this time
             (fill with constant value, equal to `fill_value`).
         fill_value: Float. Padding value to use when `pad_to_aspect_ratio=True`.
-        data_format: string, either `"channels_last"` or `"channels_first"`.
-            The ordering of the dimensions in the inputs. `"channels_last"`
-            corresponds to inputs with shape `(batch, height, width, channels)`
-            while `"channels_first"` corresponds to inputs with shape
-            `(batch, channels, height, weight)`. It defaults to the
-            `image_data_format` value found in your Keras config file at
-            `~/.keras/keras.json`. If you never set it, then it will be
-            `"channels_last"`.
+        data_format: A string specifying the data format of the input tensor.
+            It can be either `"channels_last"` or `"channels_first"`.
+            `"channels_last"` corresponds to inputs with shape
+            `(batch, height, width, channels)`, while `"channels_first"`
+            corresponds to inputs with shape `(batch, channels, height, width)`.
+            If not specified, the value will be interpreted by
+            `keras.config.image_data_format`. Defaults to `None`.
 
     Returns:
         Resized image or batch of images.
 
     Examples:
 
     >>> x = np.random.random((2, 4, 4, 3)) # batch of 2 RGB images
@@ -230,38 +195,38 @@
     (2, 3, 2, 2)
     """
     if len(size) != 2:
         raise ValueError(
             "Expected `size` to be a tuple of 2 integers. "
             f"Received: size={size}"
         )
-    if len(image.shape) < 3 or len(image.shape) > 4:
+    if len(images.shape) < 3 or len(images.shape) > 4:
         raise ValueError(
-            "Expected an image array with shape `(height, width, "
-            "channels)`, or `(batch_size, height, width, channels)`, but "
-            f"got input with incorrect rank, of shape {image.shape}."
+            "Invalid images rank: expected rank 3 (single image) "
+            "or rank 4 (batch of images). Received input with shape: "
+            f"images.shape={images.shape}"
         )
     if pad_to_aspect_ratio and crop_to_aspect_ratio:
         raise ValueError(
             "Only one of `pad_to_aspect_ratio` & `crop_to_aspect_ratio` "
             "can be `True`."
         )
-    if any_symbolic_tensors((image,)):
+    if any_symbolic_tensors((images,)):
         return Resize(
             size,
             interpolation=interpolation,
             antialias=antialias,
             data_format=data_format,
             crop_to_aspect_ratio=crop_to_aspect_ratio,
             pad_to_aspect_ratio=pad_to_aspect_ratio,
             fill_mode=fill_mode,
             fill_value=fill_value,
-        ).symbolic_call(image)
+        ).symbolic_call(images)
     return backend.image.resize(
-        image,
+        images,
         size,
         interpolation=interpolation,
         antialias=antialias,
         crop_to_aspect_ratio=crop_to_aspect_ratio,
         data_format=data_format,
         pad_to_aspect_ratio=pad_to_aspect_ratio,
         fill_mode=fill_mode,
@@ -271,61 +236,61 @@
 
 class AffineTransform(Operation):
     def __init__(
         self,
         interpolation="bilinear",
         fill_mode="constant",
         fill_value=0,
-        data_format="channels_last",
+        data_format=None,
     ):
         super().__init__()
         self.interpolation = interpolation
         self.fill_mode = fill_mode
         self.fill_value = fill_value
-        self.data_format = data_format
+        self.data_format = backend.standardize_data_format(data_format)
 
-    def call(self, image, transform):
+    def call(self, images, transform):
         return backend.image.affine_transform(
-            image,
+            images,
             transform,
             interpolation=self.interpolation,
             fill_mode=self.fill_mode,
             fill_value=self.fill_value,
             data_format=self.data_format,
         )
 
-    def compute_output_spec(self, image, transform):
-        if len(image.shape) not in (3, 4):
+    def compute_output_spec(self, images, transform):
+        if len(images.shape) not in (3, 4):
             raise ValueError(
-                "Invalid image rank: expected rank 3 (single image) "
+                "Invalid images rank: expected rank 3 (single image) "
                 "or rank 4 (batch of images). Received input with shape: "
-                f"image.shape={image.shape}"
+                f"images.shape={images.shape}"
             )
         if len(transform.shape) not in (1, 2):
             raise ValueError(
                 "Invalid transform rank: expected rank 1 (single transform) "
                 "or rank 2 (batch of transforms). Received input with shape: "
                 f"transform.shape={transform.shape}"
             )
-        return KerasTensor(image.shape, dtype=image.dtype)
+        return KerasTensor(images.shape, dtype=images.dtype)
 
 
 @keras_export("keras.ops.image.affine_transform")
 def affine_transform(
-    image,
+    images,
     transform,
     interpolation="bilinear",
     fill_mode="constant",
     fill_value=0,
-    data_format="channels_last",
+    data_format=None,
 ):
     """Applies the given transform(s) to the image(s).
 
     Args:
-        image: Input image or batch of images. Must be 3D or 4D.
+        images: Input image or batch of images. Must be 3D or 4D.
         transform: Projective transform matrix/matrices. A vector of length 8 or
             tensor of size N x 8. If one row of transform is
             `[a0, a1, a2, b0, b1, b2, c0, c1]`, then it maps the output point
             `(x, y)` to a transformed input point
             `(x', y') = ((a0 x + a1 y + a2) / k, (b0 x + b1 y + b2) / k)`,
             where `k = c0 x + c1 y + 1`. The transform is inverted compared to
             the transform mapping input points to output points. Note that
@@ -346,22 +311,21 @@
                 `fill_value`.
             - `"wrap"`: `(a b c d | a b c d | a b c d)`
                 The input is extended by wrapping around to the opposite edge.
             - `"nearest"`: `(a a a a | a b c d | d d d d)`
                 The input is extended by the nearest pixel.
         fill_value: Value used for points outside the boundaries of the input if
             `fill_mode="constant"`. Defaults to `0`.
-        data_format: string, either `"channels_last"` or `"channels_first"`.
-            The ordering of the dimensions in the inputs. `"channels_last"`
-            corresponds to inputs with shape `(batch, height, width, channels)`
-            while `"channels_first"` corresponds to inputs with shape
-            `(batch, channels, height, weight)`. It defaults to the
-            `image_data_format` value found in your Keras config file at
-            `~/.keras/keras.json`. If you never set it, then it will be
-            `"channels_last"`.
+        data_format: A string specifying the data format of the input tensor.
+            It can be either `"channels_last"` or `"channels_first"`.
+            `"channels_last"` corresponds to inputs with shape
+            `(batch, height, width, channels)`, while `"channels_first"`
+            corresponds to inputs with shape `(batch, channels, height, width)`.
+            If not specified, the value will be interpreted by
+            `keras.config.image_data_format`. Defaults to `None`.
 
     Returns:
         Applied affine transform image or batch of images.
 
     Examples:
 
     >>> x = np.random.random((2, 64, 80, 3)) # batch of 2 RGB images
@@ -389,23 +353,23 @@
     ...     ]
     ... )
     >>> y = keras.ops.image.affine_transform(x, transform,
     ...     data_format="channels_first")
     >>> y.shape
     (2, 3, 64, 80)
     """
-    if any_symbolic_tensors((image, transform)):
+    if any_symbolic_tensors((images, transform)):
         return AffineTransform(
             interpolation=interpolation,
             fill_mode=fill_mode,
             fill_value=fill_value,
             data_format=data_format,
-        ).symbolic_call(image, transform)
+        ).symbolic_call(images, transform)
     return backend.image.affine_transform(
-        image,
+        images,
         transform,
         interpolation=interpolation,
         fill_mode=fill_mode,
         fill_value=fill_value,
         data_format=data_format,
     )
 
@@ -413,90 +377,90 @@
 class ExtractPatches(Operation):
     def __init__(
         self,
         size,
         strides=None,
         dilation_rate=1,
         padding="valid",
-        data_format="channels_last",
+        data_format=None,
     ):
         super().__init__()
         if isinstance(size, int):
             size = (size, size)
         self.size = size
         self.strides = strides
         self.dilation_rate = dilation_rate
         self.padding = padding
-        self.data_format = data_format
+        self.data_format = backend.standardize_data_format(data_format)
 
-    def call(self, image):
+    def call(self, images):
         return _extract_patches(
-            image=image,
+            images=images,
             size=self.size,
             strides=self.strides,
             dilation_rate=self.dilation_rate,
             padding=self.padding,
             data_format=self.data_format,
         )
 
-    def compute_output_spec(self, image):
-        image_shape = image.shape
+    def compute_output_spec(self, images):
+        images_shape = list(images.shape)
+        original_ndim = len(images_shape)
         if not self.strides:
             strides = (self.size[0], self.size[1])
         if self.data_format == "channels_last":
-            channels_in = image.shape[-1]
+            channels_in = images_shape[-1]
         else:
-            channels_in = image.shape[-3]
-        if len(image.shape) == 3:
-            image_shape = (1,) + image_shape
+            channels_in = images_shape[-3]
+        if original_ndim == 3:
+            images_shape = [1] + images_shape
         filters = self.size[0] * self.size[1] * channels_in
         kernel_size = (self.size[0], self.size[1])
         out_shape = compute_conv_output_shape(
-            image_shape,
+            images_shape,
             filters,
             kernel_size,
             strides=strides,
             padding=self.padding,
             data_format=self.data_format,
             dilation_rate=self.dilation_rate,
         )
-        if len(image.shape) == 3:
+        if original_ndim == 3:
             out_shape = out_shape[1:]
-        return KerasTensor(shape=out_shape, dtype=image.dtype)
+        return KerasTensor(shape=out_shape, dtype=images.dtype)
 
 
 @keras_export("keras.ops.image.extract_patches")
 def extract_patches(
-    image,
+    images,
     size,
     strides=None,
     dilation_rate=1,
     padding="valid",
-    data_format="channels_last",
+    data_format=None,
 ):
     """Extracts patches from the image(s).
 
     Args:
-        image: Input image or batch of images. Must be 3D or 4D.
+        images: Input image or batch of images. Must be 3D or 4D.
         size: Patch size int or tuple (patch_height, patch_widht)
         strides: strides along height and width. If not specified, or
             if `None`, it defaults to the same value as `size`.
         dilation_rate: This is the input stride, specifying how far two
             consecutive patch samples are in the input. For value other than 1,
             strides must be 1. NOTE: `strides > 1` is not supported in
             conjunction with `dilation_rate > 1`
         padding: The type of padding algorithm to use: `"same"` or `"valid"`.
-        data_format: string, either `"channels_last"` or `"channels_first"`.
-            The ordering of the dimensions in the inputs. `"channels_last"`
-            corresponds to inputs with shape `(batch, height, width, channels)`
-            while `"channels_first"` corresponds to inputs with shape
-            `(batch, channels, height, weight)`. It defaults to the
-            `image_data_format` value found in your Keras config file at
-            `~/.keras/keras.json`. If you never set it, then it will be
-            `"channels_last"`.
+        data_format: A string specifying the data format of the input tensor.
+            It can be either `"channels_last"` or `"channels_first"`.
+            `"channels_last"` corresponds to inputs with shape
+            `(batch, height, width, channels)`, while `"channels_first"`
+            corresponds to inputs with shape `(batch, channels, height, width)`.
+            If not specified, the value will be interpreted by
+            `keras.config.image_data_format`. Defaults to `None`.
 
     Returns:
         Extracted patches 3D (if not batched) or 4D (if batched)
 
     Examples:
 
     >>> image = np.random.random(
@@ -506,246 +470,246 @@
     >>> patches.shape
     (2, 4, 4, 75)
     >>> image = np.random.random((20, 20, 3)).astype("float32") # 1 RGB image
     >>> patches = keras.ops.image.extract_patches(image, (3, 3), (1, 1))
     >>> patches.shape
     (18, 18, 27)
     """
-    if any_symbolic_tensors((image,)):
+    if any_symbolic_tensors((images,)):
         return ExtractPatches(
             size=size,
             strides=strides,
             dilation_rate=dilation_rate,
             padding=padding,
             data_format=data_format,
-        ).symbolic_call(image)
+        ).symbolic_call(images)
 
     return _extract_patches(
-        image, size, strides, dilation_rate, padding, data_format=data_format
+        images, size, strides, dilation_rate, padding, data_format=data_format
     )
 
 
 def _extract_patches(
-    image,
+    images,
     size,
     strides=None,
     dilation_rate=1,
     padding="valid",
-    data_format="channels_last",
+    data_format=None,
 ):
     if isinstance(size, int):
         patch_h = patch_w = size
     elif len(size) == 2:
         patch_h, patch_w = size[0], size[1]
     else:
         raise TypeError(
             "Invalid `size` argument. Expected an "
             f"int or a tuple of length 2. Received: size={size}"
         )
+    data_format = backend.standardize_data_format(data_format)
     if data_format == "channels_last":
-        channels_in = image.shape[-1]
+        channels_in = images.shape[-1]
     elif data_format == "channels_first":
-        channels_in = image.shape[-3]
+        channels_in = images.shape[-3]
     if not strides:
         strides = size
     out_dim = patch_h * patch_w * channels_in
-    kernel = backend.numpy.eye(out_dim, dtype=image.dtype)
+    kernel = backend.numpy.eye(out_dim, dtype=images.dtype)
     kernel = backend.numpy.reshape(
         kernel, (patch_h, patch_w, channels_in, out_dim)
     )
     _unbatched = False
-    if len(image.shape) == 3:
+    if len(images.shape) == 3:
         _unbatched = True
-        image = backend.numpy.expand_dims(image, axis=0)
+        images = backend.numpy.expand_dims(images, axis=0)
     patches = backend.nn.conv(
-        inputs=image,
+        inputs=images,
         kernel=kernel,
         strides=strides,
         padding=padding,
         data_format=data_format,
         dilation_rate=dilation_rate,
     )
     if _unbatched:
         patches = backend.numpy.squeeze(patches, axis=0)
     return patches
 
 
 class MapCoordinates(Operation):
-    def __init__(self, order=1, fill_mode="constant", fill_value=0):
+    def __init__(self, order, fill_mode="constant", fill_value=0):
         super().__init__()
         self.order = order
         self.fill_mode = fill_mode
         self.fill_value = fill_value
 
-    def call(self, image, coordinates):
+    def call(self, inputs, coordinates):
         return backend.image.map_coordinates(
-            image,
+            inputs,
             coordinates,
             order=self.order,
             fill_mode=self.fill_mode,
             fill_value=self.fill_value,
         )
 
-    def compute_output_spec(self, image, coordinates):
-        if coordinates.shape[0] != len(image.shape):
+    def compute_output_spec(self, inputs, coordinates):
+        if coordinates.shape[0] != len(inputs.shape):
             raise ValueError(
                 "First dim of `coordinates` must be the same as the rank of "
-                "`image`. "
-                f"Received image with shape: {image.shape} and coordinate "
+                "`inputs`. "
+                f"Received inputs with shape: {inputs.shape} and coordinate "
                 f"leading dim of {coordinates.shape[0]}"
             )
         if len(coordinates.shape) < 2:
             raise ValueError(
                 "Invalid coordinates rank: expected at least rank 2."
                 f" Received input with shape: {coordinates.shape}"
             )
-        return KerasTensor(coordinates.shape[1:], dtype=image.dtype)
+        return KerasTensor(coordinates.shape[1:], dtype=inputs.dtype)
 
 
 @keras_export("keras.ops.image.map_coordinates")
 def map_coordinates(
-    input, coordinates, order, fill_mode="constant", fill_value=0
+    inputs, coordinates, order, fill_mode="constant", fill_value=0
 ):
-    """Map the input array to new coordinates by interpolation..
+    """Map the input array to new coordinates by interpolation.
 
     Note that interpolation near boundaries differs from the scipy function,
     because we fixed an outstanding bug
     [scipy/issues/2640](https://github.com/scipy/scipy/issues/2640).
 
     Args:
-        input: The input array.
-        coordinates: The coordinates at which input is evaluated.
+        inputs: The input array.
+        coordinates: The coordinates at which inputs is evaluated.
         order: The order of the spline interpolation. The order must be `0` or
             `1`. `0` indicates the nearest neighbor and `1` indicates the linear
             interpolation.
-        fill_mode: Points outside the boundaries of the input are filled
+        fill_mode: Points outside the boundaries of the inputs are filled
             according to the given mode. Available methods are `"constant"`,
             `"nearest"`, `"wrap"` and `"mirror"` and `"reflect"`. Defaults to
             `"constant"`.
             - `"constant"`: `(k k k k | a b c d | k k k k)`
-                The input is extended by filling all values beyond
+                The inputs is extended by filling all values beyond
                 the edge with the same constant value k specified by
                 `fill_value`.
             - `"nearest"`: `(a a a a | a b c d | d d d d)`
-                The input is extended by the nearest pixel.
+                The inputs is extended by the nearest pixel.
             - `"wrap"`: `(a b c d | a b c d | a b c d)`
-                The input is extended by wrapping around to the opposite edge.
+                The inputs is extended by wrapping around to the opposite edge.
             - `"mirror"`: `(c d c b | a b c d | c b a b)`
-                The input is extended by mirroring about the edge.
+                The inputs is extended by mirroring about the edge.
             - `"reflect"`: `(d c b a | a b c d | d c b a)`
-                The input is extended by reflecting about the edge of the last
+                The inputs is extended by reflecting about the edge of the last
                 pixel.
-        fill_value: Value used for points outside the boundaries of the input if
-            `fill_mode="constant"`. Defaults to `0`.
+        fill_value: Value used for points outside the boundaries of the inputs
+            if `fill_mode="constant"`. Defaults to `0`.
 
     Returns:
-        Output image or batch of images.
+        Output input or batch of inputs.
 
     """
-    if any_symbolic_tensors((input, coordinates)):
+    if any_symbolic_tensors((inputs, coordinates)):
         return MapCoordinates(
             order,
             fill_mode,
             fill_value,
-        ).symbolic_call(input, coordinates)
+        ).symbolic_call(inputs, coordinates)
     return backend.image.map_coordinates(
-        input,
+        inputs,
         coordinates,
         order,
         fill_mode,
         fill_value,
     )
 
 
 class PadImages(Operation):
     def __init__(
         self,
         top_padding=None,
-        bottom_padding=None,
         left_padding=None,
+        bottom_padding=None,
         right_padding=None,
         target_height=None,
         target_width=None,
+        data_format=None,
     ):
         super().__init__()
         self.top_padding = top_padding
-        self.bottom_padding = bottom_padding
         self.left_padding = left_padding
+        self.bottom_padding = bottom_padding
         self.right_padding = right_padding
         self.target_height = target_height
         self.target_width = target_width
+        self.data_format = backend.standardize_data_format(data_format)
 
     def call(self, images):
         return _pad_images(
             images,
             self.top_padding,
-            self.bottom_padding,
             self.left_padding,
+            self.bottom_padding,
             self.right_padding,
             self.target_height,
             self.target_width,
+            self.data_format,
         )
 
     def compute_output_spec(self, images):
-        images_shape = ops.shape(images)
-        if self.target_height is None:
-            height_axis = 0 if len(images_shape) == 3 else 1
-            self.target_height = (
-                self.top_padding
-                + images_shape[height_axis]
-                + self.bottom_padding
-            )
-        if self.target_width is None:
-            width_axis = 0 if len(images_shape) == 3 else 2
-            self.target_width = (
-                self.left_padding
-                + images_shape[width_axis]
-                + self.right_padding
-            )
-        out_shape = (
-            images_shape[0],
-            self.target_height,
-            self.target_width,
-            images_shape[-1],
-        )
-        if len(images_shape) == 3:
-            out_shape = out_shape[1:]
-        return KerasTensor(
-            shape=out_shape,
-            dtype=images.dtype,
-        )
+        images_shape = list(images.shape)
+
+        if self.data_format == "channels_last":
+            height_axis, width_axis = -3, -2
+            height, width = images_shape[height_axis], images_shape[width_axis]
+        else:
+            height_axis, width_axis = -2, -1
+            height, width = images_shape[height_axis], images_shape[width_axis]
+
+        target_height = self.target_height
+        if target_height is None and height is not None:
+            target_height = self.top_padding + height + self.bottom_padding
+        target_width = self.target_width
+        if target_width is None and width is not None:
+            target_width = self.left_padding + width + self.right_padding
+
+        images_shape[height_axis] = target_height
+        images_shape[width_axis] = target_width
+        return KerasTensor(shape=images_shape, dtype=images.dtype)
 
 
 @keras_export("keras.ops.image.pad_images")
 def pad_images(
     images,
     top_padding=None,
     left_padding=None,
-    target_height=None,
-    target_width=None,
     bottom_padding=None,
     right_padding=None,
+    target_height=None,
+    target_width=None,
+    data_format=None,
 ):
     """Pad `images` with zeros to the specified `height` and `width`.
 
     Args:
-        images: 4D Tensor of shape `(batch, height, width, channels)` or 3D
-            Tensor of shape `(height, width, channels)`.
+        images: Input image or batch of images. Must be 3D or 4D.
         top_padding: Number of rows of zeros to add on top.
-        bottom_padding: Number of rows of zeros to add at the bottom.
         left_padding: Number of columns of zeros to add on the left.
+        bottom_padding: Number of rows of zeros to add at the bottom.
         right_padding: Number of columns of zeros to add on the right.
         target_height: Height of output images.
         target_width: Width of output images.
+        data_format: A string specifying the data format of the input tensor.
+            It can be either `"channels_last"` or `"channels_first"`.
+            `"channels_last"` corresponds to inputs with shape
+            `(batch, height, width, channels)`, while `"channels_first"`
+            corresponds to inputs with shape `(batch, channels, height, width)`.
+            If not specified, the value will be interpreted by
+            `keras.config.image_data_format`. Defaults to `None`.
 
     Returns:
-        If `images` were 4D, a 4D float Tensor of shape
-            `(batch, target_height, target_width, channels)`
-        If `images` were 3D, a 3D float Tensor of shape
-            `(target_height, target_width, channels)`
+        Padded image or batch of images.
 
     Example:
 
     >>> images = np.random.random((15, 25, 3))
     >>> padded_images = keras.ops.image.pad_images(
     ...     images, 2, 3, target_height=20, target_width=30
     ... )
@@ -758,56 +722,55 @@
     ... )
     >>> padded_batch.shape
     (2, 20, 30, 3)"""
 
     if any_symbolic_tensors((images,)):
         return PadImages(
             top_padding,
-            bottom_padding,
             left_padding,
+            bottom_padding,
             right_padding,
             target_height,
             target_width,
+            data_format,
         ).symbolic_call(images)
 
     return _pad_images(
         images,
         top_padding,
-        bottom_padding,
         left_padding,
+        bottom_padding,
         right_padding,
         target_height,
         target_width,
+        data_format,
     )
 
 
 def _pad_images(
     images,
     top_padding,
-    bottom_padding,
     left_padding,
+    bottom_padding,
     right_padding,
     target_height,
     target_width,
+    data_format=None,
 ):
+    data_format = backend.standardize_data_format(data_format)
     images = backend.convert_to_tensor(images)
-    is_batch = True
     images_shape = ops.shape(images)
-    if len(images_shape) == 3:
-        is_batch = False
-        images = backend.numpy.expand_dims(images, 0)
-    elif len(images_shape) != 4:
+
+    # Check
+    if len(images_shape) not in (3, 4):
         raise ValueError(
             f"Invalid shape for argument `images`: "
             "it must have rank 3 or 4. "
             f"Received: images.shape={images_shape}"
         )
-
-    batch, height, width, depth = ops.shape(images)
-
     if [top_padding, bottom_padding, target_height].count(None) != 1:
         raise ValueError(
             "Must specify exactly two of "
             "top_padding, bottom_padding, target_height. "
             f"Received: top_padding={top_padding}, "
             f"bottom_padding={bottom_padding}, "
             f"target_height={target_height}"
@@ -817,26 +780,33 @@
             "Must specify exactly two of "
             "left_padding, right_padding, target_width. "
             f"Received: left_padding={left_padding}, "
             f"right_padding={right_padding}, "
             f"target_width={target_width}"
         )
 
+    is_batch = False if len(images_shape) == 3 else True
+    if data_format == "channels_last":
+        height, width = images_shape[-3], images_shape[-2]
+    else:
+        height, width = images_shape[-2], images_shape[-1]
+
+    # Infer padding
     if top_padding is None:
         top_padding = target_height - bottom_padding - height
     if bottom_padding is None:
         bottom_padding = target_height - top_padding - height
     if left_padding is None:
         left_padding = target_width - right_padding - width
     if right_padding is None:
         right_padding = target_width - left_padding - width
 
     if top_padding < 0:
         raise ValueError(
-            "top_padding must be >= 0. " f"Received: top_padding={top_padding}"
+            f"top_padding must be >= 0. Received: top_padding={top_padding}"
         )
     if left_padding < 0:
         raise ValueError(
             "left_padding must be >= 0. "
             f"Received: left_padding={left_padding}"
         )
     if right_padding < 0:
@@ -846,135 +816,126 @@
         )
     if bottom_padding < 0:
         raise ValueError(
             "bottom_padding must be >= 0. "
             f"Received: bottom_padding={bottom_padding}"
         )
 
-    paddings = backend.numpy.reshape(
-        backend.numpy.stack(
-            [
-                0,
-                0,
-                top_padding,
-                bottom_padding,
-                left_padding,
-                right_padding,
-                0,
-                0,
-            ]
-        ),
-        [4, 2],
-    )
-    padded = backend.numpy.pad(images, paddings)
+    # Compute pad_width
+    pad_width = [[top_padding, bottom_padding], [left_padding, right_padding]]
+    if data_format == "channels_last":
+        pad_width = pad_width + [[0, 0]]
+    else:
+        pad_width = [[0, 0]] + pad_width
+    if is_batch:
+        pad_width = [[0, 0]] + pad_width
 
-    if target_height is None:
-        target_height = top_padding + height + bottom_padding
-    if target_width is None:
-        target_width = left_padding + width + right_padding
-    padded_shape = [batch, target_height, target_width, depth]
-    padded = backend.numpy.reshape(padded, padded_shape)
-
-    if not is_batch:
-        padded = backend.numpy.squeeze(padded, axis=[0])
-    return padded
+    padded_images = backend.numpy.pad(images, pad_width)
+    return padded_images
 
 
 class CropImages(Operation):
     def __init__(
         self,
         top_cropping,
-        bottom_cropping,
         left_cropping,
+        bottom_cropping,
         right_cropping,
         target_height,
         target_width,
+        data_format=None,
     ):
         super().__init__()
         self.top_cropping = top_cropping
         self.bottom_cropping = bottom_cropping
         self.left_cropping = left_cropping
         self.right_cropping = right_cropping
         self.target_height = target_height
         self.target_width = target_width
+        self.data_format = backend.standardize_data_format(data_format)
 
     def call(self, images):
         return _crop_images(
             images,
             self.top_cropping,
-            self.bottom_cropping,
             self.left_cropping,
+            self.bottom_cropping,
             self.right_cropping,
             self.target_height,
             self.target_width,
+            self.data_format,
         )
 
     def compute_output_spec(self, images):
-        images_shape = ops.shape(images)
-        out_shape = (
-            images_shape[0],
-            self.target_height,
-            self.target_width,
-            images_shape[-1],
-        )
-        if self.target_height is None:
-            height_axis = 0 if len(images_shape) == 3 else 1
-            self.target_height = (
-                self.top_cropping
-                - images_shape[height_axis]
-                - self.bottom_cropping
+        images_shape = list(images.shape)
+
+        if self.data_format == "channels_last":
+            height_axis, width_axis = -3, -2
+        else:
+            height_axis, width_axis = -2, -1
+        height, width = images_shape[height_axis], images_shape[width_axis]
+
+        if height is None and self.target_height is None:
+            raise ValueError(
+                "When the height of the images is unknown, `target_height` "
+                "must be specified."
+                f"Received images.shape={images_shape} and "
+                f"target_height={self.target_height}"
             )
-        if self.target_width is None:
-            width_axis = 0 if len(images_shape) == 3 else 2
-            self.target_width = (
-                self.left_cropping
-                - images_shape[width_axis]
-                - self.right_cropping
+        if width is None and self.target_width is None:
+            raise ValueError(
+                "When the width of the images is unknown, `target_width` "
+                "must be specified."
+                f"Received images.shape={images_shape} and "
+                f"target_width={self.target_width}"
             )
-        out_shape = (
-            images_shape[0],
-            self.target_height,
-            self.target_width,
-            images_shape[-1],
-        )
-        if len(images_shape) == 3:
-            out_shape = out_shape[1:]
-        return KerasTensor(
-            shape=out_shape,
-            dtype=images.dtype,
-        )
+
+        target_height = self.target_height
+        if target_height is None:
+            target_height = height - self.top_cropping - self.bottom_cropping
+        target_width = self.target_width
+        if target_width is None:
+            target_width = width - self.left_cropping - self.right_cropping
+
+        images_shape[height_axis] = target_height
+        images_shape[width_axis] = target_width
+        return KerasTensor(shape=images_shape, dtype=images.dtype)
 
 
 @keras_export("keras.ops.image.crop_images")
 def crop_images(
     images,
     top_cropping=None,
     left_cropping=None,
-    target_height=None,
-    target_width=None,
     bottom_cropping=None,
     right_cropping=None,
+    target_height=None,
+    target_width=None,
+    data_format=None,
 ):
     """Crop `images` to a specified `height` and `width`.
 
     Args:
-        images: 4-D batch of images of shape `(batch, height, width, channels)`
-             or 3-D single image of shape `(height, width, channels)`.
+        images: Input image or batch of images. Must be 3D or 4D.
         top_cropping: Number of columns to crop from the top.
-        bottom_cropping: Number of columns to crop from the bottom.
         left_cropping: Number of columns to crop from the left.
+        bottom_cropping: Number of columns to crop from the bottom.
         right_cropping: Number of columns to crop from the right.
         target_height: Height of the output images.
         target_width: Width of the output images.
+        data_format: A string specifying the data format of the input tensor.
+            It can be either `"channels_last"` or `"channels_first"`.
+            `"channels_last"` corresponds to inputs with shape
+            `(batch, height, width, channels)`, while `"channels_first"`
+            corresponds to inputs with shape `(batch, channels, height, width)`.
+            If not specified, the value will be interpreted by
+            `keras.config.image_data_format`. Defaults to `None`.
 
     Returns:
-        If `images` were 4D, a 4D float Tensor of shape
-            `(batch, target_height, target_width, channels)`
-        If `images` were 3D, a 3D float Tensor of shape
-            `(target_height, target_width, channels)`
+        Cropped image or batch of images.
 
     Example:
 
     >>> images = np.reshape(np.arange(1, 28, dtype="float32"), [3, 3, 3])
     >>> images[:,:,0] # print the first channel of the images
     array([[ 1.,  4.,  7.],
            [10., 13., 16.],
@@ -983,56 +944,55 @@
     >>> cropped_images[:,:,0] # print the first channel of the cropped images
     array([[ 1.,  4.],
            [10., 13.]], dtype=float32)"""
 
     if any_symbolic_tensors((images,)):
         return CropImages(
             top_cropping,
-            bottom_cropping,
             left_cropping,
+            bottom_cropping,
             right_cropping,
             target_height,
             target_width,
+            data_format,
         ).symbolic_call(images)
 
     return _crop_images(
         images,
         top_cropping,
-        bottom_cropping,
         left_cropping,
+        bottom_cropping,
         right_cropping,
         target_height,
         target_width,
+        data_format,
     )
 
 
 def _crop_images(
     images,
     top_cropping,
-    bottom_cropping,
     left_cropping,
+    bottom_cropping,
     right_cropping,
     target_height,
     target_width,
+    data_format=None,
 ):
+    data_format = backend.standardize_data_format(data_format)
     images = backend.convert_to_tensor(images)
-    is_batch = True
     images_shape = ops.shape(images)
-    if len(images_shape) == 3:
-        is_batch = False
-        images = backend.numpy.expand_dims(images, 0)
-    elif len(images_shape) != 4:
+
+    # Check
+    if len(images_shape) not in (3, 4):
         raise ValueError(
             f"Invalid shape for argument `images`: "
             "it must have rank 3 or 4. "
             f"Received: images.shape={images_shape}"
         )
-
-    batch, height, width, depth = ops.shape(images)
-
     if [top_cropping, bottom_cropping, target_height].count(None) != 1:
         raise ValueError(
             "Must specify exactly two of "
             "top_cropping, bottom_cropping, target_height. "
             f"Received: top_cropping={top_cropping}, "
             f"bottom_cropping={bottom_cropping}, "
             f"target_height={target_height}"
@@ -1042,14 +1002,23 @@
             "Must specify exactly two of "
             "left_cropping, right_cropping, target_width. "
             f"Received: left_cropping={left_cropping}, "
             f"right_cropping={right_cropping}, "
             f"target_width={target_width}"
         )
 
+    is_batch = False if len(images_shape) == 3 else True
+    if data_format == "channels_last":
+        height, width = images_shape[-3], images_shape[-2]
+        channels = images_shape[-1]
+    else:
+        height, width = images_shape[-2], images_shape[-1]
+        channels = images_shape[-3]
+
+    # Infer padding
     if top_cropping is None:
         top_cropping = height - target_height - bottom_cropping
     if target_height is None:
         target_height = height - bottom_cropping - top_cropping
     if left_cropping is None:
         left_cropping = width - target_width - right_cropping
     if target_width is None:
@@ -1072,30 +1041,23 @@
         )
     if target_width < 0:
         raise ValueError(
             "target_width must be >= 0. "
             f"Received: target_width={target_width}"
         )
 
-    if isinstance(top_cropping, int) and isinstance(left_cropping, int):
-        start_indices = [0, top_cropping, left_cropping, 0]
-    else:
-        start_indices = backend.numpy.stack([0, top_cropping, left_cropping, 0])
-    if (
-        isinstance(batch, int)
-        and isinstance(target_height, int)
-        and isinstance(target_width, int)
-        and isinstance(depth, int)
-    ):
-        shape = [batch, target_height, target_width, depth]
+    # Compute start_indices and shape
+    start_indices = [top_cropping, left_cropping]
+    shape = [target_height, target_width]
+    if data_format == "channels_last":
+        start_indices = start_indices + [0]
+        shape = shape + [channels]
     else:
-        shape = backend.numpy.stack([batch, target_height, target_width, depth])
-    cropped = ops.slice(
-        images,
-        start_indices,
-        shape,
-    )
+        start_indices = [0] + start_indices
+        shape = [channels] + shape
+    if is_batch:
+        batch_size = images_shape[0]
+        start_indices = [0] + start_indices
+        shape = [batch_size] + shape
 
-    cropped = backend.numpy.reshape(cropped, shape)
-    if not is_batch:
-        cropped = backend.numpy.squeeze(cropped, axis=[0])
-    return cropped
+    cropped_images = ops.slice(images, start_indices, shape)
+    return cropped_images
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/linalg.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/math.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/nn.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/node.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/numpy.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/operation.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adam.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/lion.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/random/random.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/random/seed_generator.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/saving/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/saving/keras_saveable.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/saving/keras_saveable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/saving/object_registration.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/saving/saving_api.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/testing/test_case.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/testing/test_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/trainers/trainer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/tree/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/tree/tree_api.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/__init__.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/code_stats.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/file_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/image_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/io_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/module_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/module_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,9 +37,10 @@
 
 
 tensorflow = LazyModule("tensorflow")
 gfile = LazyModule("tensorflow.io.gfile", pip_name="tensorflow")
 tensorflow_io = LazyModule("tensorflow_io")
 scipy = LazyModule("scipy")
 jax = LazyModule("jax")
+torchvision = LazyModule("torchvision")
 optree = LazyModule("optree")
 dmtree = LazyModule("tree")
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/naming.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/progbar.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/python_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras/src/utils/tracking.py` & `keras_nightly-3.3.3.dev2024053103/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.3.dev2024053103/keras_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024052903
+Version: 3.3.3.dev2024053103
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024052903/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.3.dev2024053103/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052903/setup.py` & `keras_nightly-3.3.3.dev2024053103/setup.py`

 * *Files identical despite different names*

