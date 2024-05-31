# Comparing `tmp/grad-cam-1.5.0.tar.gz` & `tmp/grad-cam-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grad-cam-1.5.0.tar", last modified: Tue Dec 19 13:17:54 2023, max compression
+gzip compressed data, was "grad-cam-1.5.2.tar", last modified: Tue May 28 19:02:08 2024, max compression
```

## Comparing `grad-cam-1.5.0.tar` & `grad-cam-1.5.2.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:54.015463 grad-cam-1.5.0/
--rw-rw-rw-   0        0        0       45 2021-12-30 18:15:48.000000 grad-cam-1.5.0/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:53.805191 grad-cam-1.5.0/.github/
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:53.831205 grad-cam-1.5.0/.github/workflows/
--rw-rw-rw-   0        0        0     1181 2022-08-01 03:43:36.000000 grad-cam-1.5.0/.github/workflows/python-app.yml
--rw-rw-rw-   0        0        0       33 2021-04-03 13:55:26.000000 grad-cam-1.5.0/.gitignore
--rw-rw-rw-   0        0        0     1094 2021-09-13 05:28:59.000000 grad-cam-1.5.0/LICENSE
--rw-rw-rw-   0        0        0       15 2022-08-01 09:16:16.000000 grad-cam-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0    17196 2023-12-19 13:17:54.014814 grad-cam-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    16015 2023-12-19 13:14:22.000000 grad-cam-1.5.0/README.md
--rw-rw-rw-   0        0        0     5485 2023-12-19 13:12:13.000000 grad-cam-1.5.0/cam.py
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:53.935838 grad-cam-1.5.0/examples/
--rw-rw-rw-   0        0        0    18447 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/augsmooth.jpg
--rw-rw-rw-   0        0        0    90226 2021-04-02 11:03:17.000000 grad-cam-1.5.0/examples/both.png
--rw-rw-rw-   0        0        0    74805 2021-12-30 15:52:29.000000 grad-cam-1.5.0/examples/both_detection.png
--rw-rw-rw-   0        0        0    10719 2021-04-02 11:03:17.000000 grad-cam-1.5.0/examples/cam_gb_dog.jpg
--rw-rw-rw-   0        0        0   286808 2021-12-30 15:52:29.000000 grad-cam-1.5.0/examples/cars_segmentation.png
--rw-rw-rw-   0        0        0    19413 2021-04-02 11:03:17.000000 grad-cam-1.5.0/examples/cat.jpg
--rw-rw-rw-   0        0        0   626320 2022-08-01 10:18:31.000000 grad-cam-1.5.0/examples/dff1.png
--rw-rw-rw-   0        0        0   596116 2022-08-01 10:18:51.000000 grad-cam-1.5.0/examples/dff2.png
--rw-rw-rw-   0        0        0    18669 2021-04-02 11:03:17.000000 grad-cam-1.5.0/examples/dog.jpg
--rw-rw-rw-   0        0        0     8608 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/dog_cat.jfif
--rw-rw-rw-   0        0        0   272570 2021-04-03 13:55:26.000000 grad-cam-1.5.0/examples/dogs.png
--rw-rw-rw-   0        0        0    29005 2021-04-03 13:55:26.000000 grad-cam-1.5.0/examples/dogs_gradcam++_resnet50.jpg
--rw-rw-rw-   0        0        0    29106 2021-04-03 13:55:26.000000 grad-cam-1.5.0/examples/dogs_gradcam++_vgg16.jpg
--rw-rw-rw-   0        0        0    28798 2021-04-03 13:55:26.000000 grad-cam-1.5.0/examples/dogs_gradcam_resnet50.jpg
--rw-rw-rw-   0        0        0    29319 2021-04-03 13:55:26.000000 grad-cam-1.5.0/examples/dogs_gradcam_vgg16.jpg
--rw-rw-rw-   0        0        0    28993 2021-04-03 13:55:26.000000 grad-cam-1.5.0/examples/dogs_scorecam_resnet50.jpg
--rw-rw-rw-   0        0        0    28384 2021-04-03 13:55:26.000000 grad-cam-1.5.0/examples/dogs_scorecam_vgg16.jpg
--rw-rw-rw-   0        0        0    18219 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/eigenaug.jpg
--rw-rw-rw-   0        0        0    18207 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/eigensmooth.jpg
--rw-rw-rw-   0        0        0  2201243 2022-07-09 09:36:24.000000 grad-cam-1.5.0/examples/embeddings.png
--rw-rw-rw-   0        0        0    50158 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/horses.jpg
--rw-rw-rw-   0        0        0   352428 2022-07-09 13:05:02.000000 grad-cam-1.5.0/examples/metrics.png
--rw-rw-rw-   0        0        0    18414 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/nosmooth.jpg
--rw-rw-rw-   0        0        0    17530 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet50_cat_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17490 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet50_cat_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    17436 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet50_cat_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    17810 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet50_dog_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17780 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet50_dog_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    17754 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet50_dog_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    71715 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet_horses_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    71843 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet_horses_gradcam++_cam.jpg
--rw-rw-rw-   0        0        0    71766 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet_horses_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    71262 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet_horses_horses_eigencam_cam.jpg
--rw-rw-rw-   0        0        0    71917 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/resnet_horses_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    80319 2022-07-09 09:55:24.000000 grad-cam-1.5.0/examples/road.png
--rw-rw-rw-   0        0        0    17331 2021-05-14 10:33:52.000000 grad-cam-1.5.0/examples/swinT_cat_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17400 2021-05-14 10:33:52.000000 grad-cam-1.5.0/examples/swinT_cat_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    17627 2021-05-14 10:33:52.000000 grad-cam-1.5.0/examples/swinT_cat_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    18105 2021-05-14 10:33:52.000000 grad-cam-1.5.0/examples/swinT_dog_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17649 2021-05-14 10:33:52.000000 grad-cam-1.5.0/examples/swinT_dog_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    17720 2021-05-14 10:33:52.000000 grad-cam-1.5.0/examples/swinT_dog_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    71353 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vgg_horses_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    71040 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vgg_horses_eigencam_cam.jpg
--rw-rw-rw-   0        0        0    71326 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vgg_horses_gradcam++_cam.jpg
--rw-rw-rw-   0        0        0    71409 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vgg_horses_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    71522 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vgg_horses_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    18096 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vit_cat_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17951 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vit_cat_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    18218 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vit_cat_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    19807 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vit_dog_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    19396 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vit_dog_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    18240 2021-05-01 13:07:59.000000 grad-cam-1.5.0/examples/vit_dog_scorecam_cam.jpg
--rw-rw-rw-   0        0        0  1788713 2022-08-01 05:50:56.000000 grad-cam-1.5.0/examples/yolo_eigencam.png
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:53.958770 grad-cam-1.5.0/grad_cam.egg-info/
--rw-rw-rw-   0        0        0    17196 2023-12-19 13:17:53.000000 grad-cam-1.5.0/grad_cam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3342 2023-12-19 13:17:53.000000 grad-cam-1.5.0/grad_cam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-19 13:17:53.000000 grad-cam-1.5.0/grad_cam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-12-19 13:17:53.000000 grad-cam-1.5.0/grad_cam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-12-19 13:17:53.000000 grad-cam-1.5.0/grad_cam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-03 13:55:26.000000 grad-cam-1.5.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:53.978876 grad-cam-1.5.0/pytorch_grad_cam/
--rw-rw-rw-   0        0        0     1196 2022-10-18 07:37:44.000000 grad-cam-1.5.0/pytorch_grad_cam/__init__.py
--rw-rw-rw-   0        0        0     6754 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/ablation_cam.py
--rw-rw-rw-   0        0        0     5034 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/ablation_cam_multilayer.py
--rw-rw-rw-   0        0        0     6325 2022-08-01 05:50:56.000000 grad-cam-1.5.0/pytorch_grad_cam/ablation_layer.py
--rw-rw-rw-   0        0        0     1771 2022-10-17 11:35:47.000000 grad-cam-1.5.0/pytorch_grad_cam/activations_and_gradients.py
--rw-rw-rw-   0        0        0     8436 2023-12-19 12:16:34.000000 grad-cam-1.5.0/pytorch_grad_cam/base_cam.py
--rw-rw-rw-   0        0        0      775 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/eigen_cam.py
--rw-rw-rw-   0        0        0      754 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/eigen_grad_cam.py
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:53.980839 grad-cam-1.5.0/pytorch_grad_cam/feature_factorization/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:14:13.000000 grad-cam-1.5.0/pytorch_grad_cam/feature_factorization/__init__.py
--rw-rw-rw-   0        0        0     5541 2022-10-18 07:37:44.000000 grad-cam-1.5.0/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py
--rw-rw-rw-   0        0        0      771 2022-10-18 07:37:44.000000 grad-cam-1.5.0/pytorch_grad_cam/feature_factorization/utils.py
--rw-rw-rw-   0        0        0     4057 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/fullgrad_cam.py
--rw-rw-rw-   0        0        0      579 2023-12-19 13:13:43.000000 grad-cam-1.5.0/pytorch_grad_cam/grad_cam.py
--rw-rw-rw-   0        0        0      898 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/grad_cam_elementwise.py
--rw-rw-rw-   0        0        0     1204 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/grad_cam_plusplus.py
--rw-rw-rw-   0        0        0     3218 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/guided_backprop.py
--rw-rw-rw-   0        0        0      981 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/hirescam.py
--rw-rw-rw-   0        0        0      972 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/layer_cam.py
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:53.984811 grad-cam-1.5.0/pytorch_grad_cam/metrics/
--rw-rw-rw-   0        0        0        0 2022-08-25 06:44:39.000000 grad-cam-1.5.0/pytorch_grad_cam/metrics/__init__.py
--rw-rw-rw-   0        0        0     1222 2022-08-01 05:50:56.000000 grad-cam-1.5.0/pytorch_grad_cam/metrics/cam_mult_image.py
--rw-rw-rw-   0        0        0     3621 2022-08-01 05:50:56.000000 grad-cam-1.5.0/pytorch_grad_cam/metrics/perturbation_confidence.py
--rw-rw-rw-   0        0        0     7897 2022-08-01 05:50:56.000000 grad-cam-1.5.0/pytorch_grad_cam/metrics/road.py
--rw-rw-rw-   0        0        0      620 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/random_cam.py
--rw-rw-rw-   0        0        0     2216 2023-12-19 10:13:50.000000 grad-cam-1.5.0/pytorch_grad_cam/score_cam.py
--rw-rw-rw-   0        0        0      375 2022-08-01 05:50:56.000000 grad-cam-1.5.0/pytorch_grad_cam/sobel_cam.py
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:53.990814 grad-cam-1.5.0/pytorch_grad_cam/utils/
--rw-rw-rw-   0        0        0      236 2022-08-25 06:44:06.000000 grad-cam-1.5.0/pytorch_grad_cam/utils/__init__.py
--rw-rw-rw-   0        0        0     1083 2022-08-01 05:50:56.000000 grad-cam-1.5.0/pytorch_grad_cam/utils/find_layers.py
--rw-rw-rw-   0        0        0     7237 2022-10-18 07:37:45.000000 grad-cam-1.5.0/pytorch_grad_cam/utils/image.py
--rw-rw-rw-   0        0        0     3295 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/utils/model_targets.py
--rw-rw-rw-   0        0        0     1044 2022-10-16 13:31:03.000000 grad-cam-1.5.0/pytorch_grad_cam/utils/reshape_transforms.py
--rw-rw-rw-   0        0        0      829 2022-07-30 18:19:49.000000 grad-cam-1.5.0/pytorch_grad_cam/utils/svd_on_activations.py
--rw-rw-rw-   0        0        0      810 2023-12-19 10:12:18.000000 grad-cam-1.5.0/pytorch_grad_cam/xgrad_cam.py
--rw-rw-rw-   0        0        0      101 2022-08-01 05:50:56.000000 grad-cam-1.5.0/requirements.txt
--rw-rw-rw-   0        0        0      711 2023-12-19 13:17:54.020857 grad-cam-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1044 2023-12-19 13:13:45.000000 grad-cam-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:53.994164 grad-cam-1.5.0/tests/
--rw-rw-rw-   0        0        0     2077 2023-12-19 10:12:18.000000 grad-cam-1.5.0/tests/test_context_release.py
--rw-rw-rw-   0        0        0     1366 2023-12-19 10:12:18.000000 grad-cam-1.5.0/tests/test_one_channel.py
--rw-rw-rw-   0        0        0     2459 2023-12-19 10:12:18.000000 grad-cam-1.5.0/tests/test_run_all_models.py
-drwxrwxrwx   0        0        0        0 2023-12-19 13:17:54.013854 grad-cam-1.5.0/usage_examples/
--rw-rw-rw-   0        0        0     4245 2022-10-18 07:37:46.000000 grad-cam-1.5.0/usage_examples/swinT_example.py
--rw-rw-rw-   0        0        0     4471 2022-10-18 07:37:46.000000 grad-cam-1.5.0/usage_examples/vit_example.py
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.402458 grad-cam-1.5.2/
+-rw-rw-rw-   0        0        0       45 2021-12-30 18:15:48.000000 grad-cam-1.5.2/.gitattributes
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.108030 grad-cam-1.5.2/.github/
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.132020 grad-cam-1.5.2/.github/workflows/
+-rw-rw-rw-   0        0        0     1181 2022-08-01 03:43:36.000000 grad-cam-1.5.2/.github/workflows/python-app.yml
+-rw-rw-rw-   0        0        0       33 2021-04-03 13:55:26.000000 grad-cam-1.5.2/.gitignore
+-rw-rw-rw-   0        0        0     1094 2021-09-13 05:28:59.000000 grad-cam-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0       15 2022-08-01 09:16:16.000000 grad-cam-1.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    17340 2024-05-28 19:02:08.402003 grad-cam-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16155 2024-05-28 18:53:02.000000 grad-cam-1.5.2/README.md
+-rw-rw-rw-   0        0        0     5485 2023-12-19 13:12:13.000000 grad-cam-1.5.2/cam.py
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.226037 grad-cam-1.5.2/examples/
+-rw-rw-rw-   0        0        0    18447 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/augsmooth.jpg
+-rw-rw-rw-   0        0        0    90226 2021-04-02 11:03:17.000000 grad-cam-1.5.2/examples/both.png
+-rw-rw-rw-   0        0        0    74805 2021-12-30 15:52:29.000000 grad-cam-1.5.2/examples/both_detection.png
+-rw-rw-rw-   0        0        0    10719 2021-04-02 11:03:17.000000 grad-cam-1.5.2/examples/cam_gb_dog.jpg
+-rw-rw-rw-   0        0        0   286808 2021-12-30 15:52:29.000000 grad-cam-1.5.2/examples/cars_segmentation.png
+-rw-rw-rw-   0        0        0    19413 2021-04-02 11:03:17.000000 grad-cam-1.5.2/examples/cat.jpg
+-rw-rw-rw-   0        0        0   626320 2022-08-01 10:18:31.000000 grad-cam-1.5.2/examples/dff1.png
+-rw-rw-rw-   0        0        0   596116 2022-08-01 10:18:51.000000 grad-cam-1.5.2/examples/dff2.png
+-rw-rw-rw-   0        0        0    18669 2021-04-02 11:03:17.000000 grad-cam-1.5.2/examples/dog.jpg
+-rw-rw-rw-   0        0        0     8608 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/dog_cat.jfif
+-rw-rw-rw-   0        0        0   272570 2021-04-03 13:55:26.000000 grad-cam-1.5.2/examples/dogs.png
+-rw-rw-rw-   0        0        0    29005 2021-04-03 13:55:26.000000 grad-cam-1.5.2/examples/dogs_gradcam++_resnet50.jpg
+-rw-rw-rw-   0        0        0    29106 2021-04-03 13:55:26.000000 grad-cam-1.5.2/examples/dogs_gradcam++_vgg16.jpg
+-rw-rw-rw-   0        0        0    28798 2021-04-03 13:55:26.000000 grad-cam-1.5.2/examples/dogs_gradcam_resnet50.jpg
+-rw-rw-rw-   0        0        0    29319 2021-04-03 13:55:26.000000 grad-cam-1.5.2/examples/dogs_gradcam_vgg16.jpg
+-rw-rw-rw-   0        0        0    28993 2021-04-03 13:55:26.000000 grad-cam-1.5.2/examples/dogs_scorecam_resnet50.jpg
+-rw-rw-rw-   0        0        0    28384 2021-04-03 13:55:26.000000 grad-cam-1.5.2/examples/dogs_scorecam_vgg16.jpg
+-rw-rw-rw-   0        0        0    18219 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/eigenaug.jpg
+-rw-rw-rw-   0        0        0    18207 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/eigensmooth.jpg
+-rw-rw-rw-   0        0        0  2201243 2022-07-09 09:36:24.000000 grad-cam-1.5.2/examples/embeddings.png
+-rw-rw-rw-   0        0        0    50158 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/horses.jpg
+-rw-rw-rw-   0        0        0   352428 2022-07-09 13:05:02.000000 grad-cam-1.5.2/examples/metrics.png
+-rw-rw-rw-   0        0        0    18414 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/nosmooth.jpg
+-rw-rw-rw-   0        0        0    17530 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet50_cat_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17490 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet50_cat_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17436 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet50_cat_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    17810 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet50_dog_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17780 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet50_dog_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17754 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet50_dog_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    71715 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet_horses_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    71843 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet_horses_gradcam++_cam.jpg
+-rw-rw-rw-   0        0        0    71766 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet_horses_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    71262 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet_horses_horses_eigencam_cam.jpg
+-rw-rw-rw-   0        0        0    71917 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/resnet_horses_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    80319 2022-07-09 09:55:24.000000 grad-cam-1.5.2/examples/road.png
+-rw-rw-rw-   0        0        0    17331 2021-05-14 10:33:52.000000 grad-cam-1.5.2/examples/swinT_cat_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17400 2021-05-14 10:33:52.000000 grad-cam-1.5.2/examples/swinT_cat_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17627 2021-05-14 10:33:52.000000 grad-cam-1.5.2/examples/swinT_cat_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    18105 2021-05-14 10:33:52.000000 grad-cam-1.5.2/examples/swinT_dog_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17649 2021-05-14 10:33:52.000000 grad-cam-1.5.2/examples/swinT_dog_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17720 2021-05-14 10:33:52.000000 grad-cam-1.5.2/examples/swinT_dog_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    71353 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vgg_horses_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    71040 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vgg_horses_eigencam_cam.jpg
+-rw-rw-rw-   0        0        0    71326 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vgg_horses_gradcam++_cam.jpg
+-rw-rw-rw-   0        0        0    71409 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vgg_horses_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    71522 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vgg_horses_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    18096 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vit_cat_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17951 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vit_cat_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    18218 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vit_cat_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    19807 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vit_dog_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    19396 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vit_dog_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    18240 2021-05-01 13:07:59.000000 grad-cam-1.5.2/examples/vit_dog_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0  1788713 2022-08-01 05:50:56.000000 grad-cam-1.5.2/examples/yolo_eigencam.png
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.399995 grad-cam-1.5.2/grad_cam.egg-info/
+-rw-rw-rw-   0        0        0    17340 2024-05-28 19:02:08.000000 grad-cam-1.5.2/grad_cam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3342 2024-05-28 19:02:08.000000 grad-cam-1.5.2/grad_cam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 19:02:08.000000 grad-cam-1.5.2/grad_cam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-28 19:02:08.000000 grad-cam-1.5.2/grad_cam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-28 19:02:08.000000 grad-cam-1.5.2/grad_cam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-03 13:55:26.000000 grad-cam-1.5.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.340579 grad-cam-1.5.2/pytorch_grad_cam/
+-rw-rw-rw-   0        0        0     1196 2022-10-18 07:37:44.000000 grad-cam-1.5.2/pytorch_grad_cam/__init__.py
+-rw-rw-rw-   0        0        0     6754 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/ablation_cam.py
+-rw-rw-rw-   0        0        0     5034 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/ablation_cam_multilayer.py
+-rw-rw-rw-   0        0        0     6325 2022-08-01 05:50:56.000000 grad-cam-1.5.2/pytorch_grad_cam/ablation_layer.py
+-rw-rw-rw-   0        0        0     1771 2022-10-17 11:35:47.000000 grad-cam-1.5.2/pytorch_grad_cam/activations_and_gradients.py
+-rw-rw-rw-   0        0        0     7943 2024-05-28 18:47:41.000000 grad-cam-1.5.2/pytorch_grad_cam/base_cam.py
+-rw-rw-rw-   0        0        0      775 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/eigen_cam.py
+-rw-rw-rw-   0        0        0      754 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/eigen_grad_cam.py
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.347994 grad-cam-1.5.2/pytorch_grad_cam/feature_factorization/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:14:13.000000 grad-cam-1.5.2/pytorch_grad_cam/feature_factorization/__init__.py
+-rw-rw-rw-   0        0        0     5541 2022-10-18 07:37:44.000000 grad-cam-1.5.2/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py
+-rw-rw-rw-   0        0        0      771 2022-10-18 07:37:44.000000 grad-cam-1.5.2/pytorch_grad_cam/feature_factorization/utils.py
+-rw-rw-rw-   0        0        0     4057 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/fullgrad_cam.py
+-rw-rw-rw-   0        0        0      913 2024-05-28 18:47:41.000000 grad-cam-1.5.2/pytorch_grad_cam/grad_cam.py
+-rw-rw-rw-   0        0        0      898 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/grad_cam_elementwise.py
+-rw-rw-rw-   0        0        0     1204 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/grad_cam_plusplus.py
+-rw-rw-rw-   0        0        0     3218 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/guided_backprop.py
+-rw-rw-rw-   0        0        0      981 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/hirescam.py
+-rw-rw-rw-   0        0        0      972 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/layer_cam.py
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.369002 grad-cam-1.5.2/pytorch_grad_cam/metrics/
+-rw-rw-rw-   0        0        0        0 2022-08-25 06:44:39.000000 grad-cam-1.5.2/pytorch_grad_cam/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1222 2022-08-01 05:50:56.000000 grad-cam-1.5.2/pytorch_grad_cam/metrics/cam_mult_image.py
+-rw-rw-rw-   0        0        0     3621 2022-08-01 05:50:56.000000 grad-cam-1.5.2/pytorch_grad_cam/metrics/perturbation_confidence.py
+-rw-rw-rw-   0        0        0     7897 2022-08-01 05:50:56.000000 grad-cam-1.5.2/pytorch_grad_cam/metrics/road.py
+-rw-rw-rw-   0        0        0      620 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/random_cam.py
+-rw-rw-rw-   0        0        0     2216 2023-12-19 10:13:50.000000 grad-cam-1.5.2/pytorch_grad_cam/score_cam.py
+-rw-rw-rw-   0        0        0      375 2022-08-01 05:50:56.000000 grad-cam-1.5.2/pytorch_grad_cam/sobel_cam.py
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.387022 grad-cam-1.5.2/pytorch_grad_cam/utils/
+-rw-rw-rw-   0        0        0      236 2022-08-25 06:44:06.000000 grad-cam-1.5.2/pytorch_grad_cam/utils/__init__.py
+-rw-rw-rw-   0        0        0     1083 2022-08-01 05:50:56.000000 grad-cam-1.5.2/pytorch_grad_cam/utils/find_layers.py
+-rw-rw-rw-   0        0        0     7293 2024-05-28 18:50:08.000000 grad-cam-1.5.2/pytorch_grad_cam/utils/image.py
+-rw-rw-rw-   0        0        0     3295 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/utils/model_targets.py
+-rw-rw-rw-   0        0        0     1044 2022-10-16 13:31:03.000000 grad-cam-1.5.2/pytorch_grad_cam/utils/reshape_transforms.py
+-rw-rw-rw-   0        0        0      829 2022-07-30 18:19:49.000000 grad-cam-1.5.2/pytorch_grad_cam/utils/svd_on_activations.py
+-rw-rw-rw-   0        0        0      810 2023-12-19 10:12:18.000000 grad-cam-1.5.2/pytorch_grad_cam/xgrad_cam.py
+-rw-rw-rw-   0        0        0      101 2022-08-01 05:50:56.000000 grad-cam-1.5.2/requirements.txt
+-rw-rw-rw-   0        0        0      711 2024-05-28 19:02:08.403993 grad-cam-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2024-05-28 18:51:20.000000 grad-cam-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.396030 grad-cam-1.5.2/tests/
+-rw-rw-rw-   0        0        0     2077 2023-12-19 10:12:18.000000 grad-cam-1.5.2/tests/test_context_release.py
+-rw-rw-rw-   0        0        0     1366 2023-12-19 10:12:18.000000 grad-cam-1.5.2/tests/test_one_channel.py
+-rw-rw-rw-   0        0        0     2459 2023-12-19 10:12:18.000000 grad-cam-1.5.2/tests/test_run_all_models.py
+drwxrwxrwx   0        0        0        0 2024-05-28 19:02:08.399030 grad-cam-1.5.2/usage_examples/
+-rw-rw-rw-   0        0        0     4245 2022-10-18 07:37:46.000000 grad-cam-1.5.2/usage_examples/swinT_example.py
+-rw-rw-rw-   0        0        0     4471 2022-10-18 07:37:46.000000 grad-cam-1.5.2/usage_examples/vit_example.py
```

### Comparing `grad-cam-1.5.0/.github/workflows/python-app.yml` & `grad-cam-1.5.2/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/LICENSE` & `grad-cam-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/PKG-INFO` & `grad-cam-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grad-cam
-Version: 1.5.0
+Version: 1.5.2
 Summary: Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more
 Home-page: https://github.com/jacobgil/pytorch-grad-cam
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/pytorch-grad-cam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -77,14 +77,18 @@
  <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/dog.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cat.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cam_gb_dog.jpg?raw=true" width="256" height="256"> |
 
 ## Object Detection and Semantic Segmentation
 | Object Detection | Semantic Segmentation |
 | -----------------|-----------------------|
 | <img src="./examples/both_detection.png" width="256" height="256"> | <img src="./examples/cars_segmentation.png" width="256" height="200"> |
 
+| 3D Medical Semantic Segmentation (3D) |
+| -------------------------- |
+| <img src="./examples/multiorgan_segmentation.gif" width="539">|
+
 ## Explaining similarity to other images / embeddings
 <img src="./examples/embeddings.png">
 
 ## Deep Feature Factorization
 <img src="./examples/dff1.png">
 <img src="./examples/dff2.png">
```

### Comparing `grad-cam-1.5.0/README.md` & `grad-cam-1.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,18 @@
  <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/dog.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cat.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cam_gb_dog.jpg?raw=true" width="256" height="256"> |
 
 ## Object Detection and Semantic Segmentation
 | Object Detection | Semantic Segmentation |
 | -----------------|-----------------------|
 | <img src="./examples/both_detection.png" width="256" height="256"> | <img src="./examples/cars_segmentation.png" width="256" height="200"> |
 
+| 3D Medical Semantic Segmentation (3D) |
+| -------------------------- |
+| <img src="./examples/multiorgan_segmentation.gif" width="539">|
+
 ## Explaining similarity to other images / embeddings
 <img src="./examples/embeddings.png">
 
 ## Deep Feature Factorization
 <img src="./examples/dff1.png">
 <img src="./examples/dff2.png">
```

### Comparing `grad-cam-1.5.0/cam.py` & `grad-cam-1.5.2/cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/augsmooth.jpg` & `grad-cam-1.5.2/examples/augsmooth.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/both.png` & `grad-cam-1.5.2/examples/both.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/both_detection.png` & `grad-cam-1.5.2/examples/both_detection.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/cam_gb_dog.jpg` & `grad-cam-1.5.2/examples/cam_gb_dog.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/cars_segmentation.png` & `grad-cam-1.5.2/examples/cars_segmentation.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/cat.jpg` & `grad-cam-1.5.2/examples/cat.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dff1.png` & `grad-cam-1.5.2/examples/dff1.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dff2.png` & `grad-cam-1.5.2/examples/dff2.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dog.jpg` & `grad-cam-1.5.2/examples/dog.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dog_cat.jfif` & `grad-cam-1.5.2/examples/dog_cat.jfif`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dogs.png` & `grad-cam-1.5.2/examples/dogs.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dogs_gradcam++_resnet50.jpg` & `grad-cam-1.5.2/examples/dogs_gradcam++_resnet50.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dogs_gradcam++_vgg16.jpg` & `grad-cam-1.5.2/examples/dogs_gradcam++_vgg16.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dogs_gradcam_resnet50.jpg` & `grad-cam-1.5.2/examples/dogs_gradcam_resnet50.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dogs_gradcam_vgg16.jpg` & `grad-cam-1.5.2/examples/dogs_gradcam_vgg16.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dogs_scorecam_resnet50.jpg` & `grad-cam-1.5.2/examples/dogs_scorecam_resnet50.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/dogs_scorecam_vgg16.jpg` & `grad-cam-1.5.2/examples/dogs_scorecam_vgg16.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/eigenaug.jpg` & `grad-cam-1.5.2/examples/eigenaug.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/eigensmooth.jpg` & `grad-cam-1.5.2/examples/eigensmooth.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/embeddings.png` & `grad-cam-1.5.2/examples/embeddings.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/horses.jpg` & `grad-cam-1.5.2/examples/horses.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/metrics.png` & `grad-cam-1.5.2/examples/metrics.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/nosmooth.jpg` & `grad-cam-1.5.2/examples/nosmooth.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet50_cat_ablationcam_cam.jpg` & `grad-cam-1.5.2/examples/resnet50_cat_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet50_cat_gradcam_cam.jpg` & `grad-cam-1.5.2/examples/resnet50_cat_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet50_cat_scorecam_cam.jpg` & `grad-cam-1.5.2/examples/resnet50_cat_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet50_dog_ablationcam_cam.jpg` & `grad-cam-1.5.2/examples/resnet50_dog_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet50_dog_gradcam_cam.jpg` & `grad-cam-1.5.2/examples/resnet50_dog_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet50_dog_scorecam_cam.jpg` & `grad-cam-1.5.2/examples/resnet50_dog_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet_horses_ablationcam_cam.jpg` & `grad-cam-1.5.2/examples/resnet_horses_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet_horses_gradcam++_cam.jpg` & `grad-cam-1.5.2/examples/resnet_horses_gradcam++_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet_horses_gradcam_cam.jpg` & `grad-cam-1.5.2/examples/resnet_horses_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet_horses_horses_eigencam_cam.jpg` & `grad-cam-1.5.2/examples/resnet_horses_horses_eigencam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/resnet_horses_scorecam_cam.jpg` & `grad-cam-1.5.2/examples/resnet_horses_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/road.png` & `grad-cam-1.5.2/examples/road.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/swinT_cat_ablationcam_cam.jpg` & `grad-cam-1.5.2/examples/swinT_cat_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/swinT_cat_gradcam_cam.jpg` & `grad-cam-1.5.2/examples/swinT_cat_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/swinT_cat_scorecam_cam.jpg` & `grad-cam-1.5.2/examples/swinT_cat_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/swinT_dog_ablationcam_cam.jpg` & `grad-cam-1.5.2/examples/swinT_dog_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/swinT_dog_gradcam_cam.jpg` & `grad-cam-1.5.2/examples/swinT_dog_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/swinT_dog_scorecam_cam.jpg` & `grad-cam-1.5.2/examples/swinT_dog_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vgg_horses_ablationcam_cam.jpg` & `grad-cam-1.5.2/examples/vgg_horses_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vgg_horses_eigencam_cam.jpg` & `grad-cam-1.5.2/examples/vgg_horses_eigencam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vgg_horses_gradcam++_cam.jpg` & `grad-cam-1.5.2/examples/vgg_horses_gradcam++_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vgg_horses_gradcam_cam.jpg` & `grad-cam-1.5.2/examples/vgg_horses_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vgg_horses_scorecam_cam.jpg` & `grad-cam-1.5.2/examples/vgg_horses_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vit_cat_ablationcam_cam.jpg` & `grad-cam-1.5.2/examples/vit_cat_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vit_cat_gradcam_cam.jpg` & `grad-cam-1.5.2/examples/vit_cat_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vit_cat_scorecam_cam.jpg` & `grad-cam-1.5.2/examples/vit_cat_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vit_dog_ablationcam_cam.jpg` & `grad-cam-1.5.2/examples/vit_dog_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vit_dog_gradcam_cam.jpg` & `grad-cam-1.5.2/examples/vit_dog_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/vit_dog_scorecam_cam.jpg` & `grad-cam-1.5.2/examples/vit_dog_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/examples/yolo_eigencam.png` & `grad-cam-1.5.2/examples/yolo_eigencam.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/grad_cam.egg-info/PKG-INFO` & `grad-cam-1.5.2/grad_cam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grad-cam
-Version: 1.5.0
+Version: 1.5.2
 Summary: Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more
 Home-page: https://github.com/jacobgil/pytorch-grad-cam
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/pytorch-grad-cam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -77,14 +77,18 @@
  <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/dog.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cat.jpg?raw=true" width="256" height="256"> | <img src="https://github.com/jacobgil/pytorch-grad-cam/blob/master/examples/cam_gb_dog.jpg?raw=true" width="256" height="256"> |
 
 ## Object Detection and Semantic Segmentation
 | Object Detection | Semantic Segmentation |
 | -----------------|-----------------------|
 | <img src="./examples/both_detection.png" width="256" height="256"> | <img src="./examples/cars_segmentation.png" width="256" height="200"> |
 
+| 3D Medical Semantic Segmentation (3D) |
+| -------------------------- |
+| <img src="./examples/multiorgan_segmentation.gif" width="539">|
+
 ## Explaining similarity to other images / embeddings
 <img src="./examples/embeddings.png">
 
 ## Deep Feature Factorization
 <img src="./examples/dff1.png">
 <img src="./examples/dff2.png">
```

### Comparing `grad-cam-1.5.0/grad_cam.egg-info/SOURCES.txt` & `grad-cam-1.5.2/grad_cam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/__init__.py` & `grad-cam-1.5.2/pytorch_grad_cam/__init__.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/ablation_cam.py` & `grad-cam-1.5.2/pytorch_grad_cam/ablation_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/ablation_cam_multilayer.py` & `grad-cam-1.5.2/pytorch_grad_cam/ablation_cam_multilayer.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/ablation_layer.py` & `grad-cam-1.5.2/pytorch_grad_cam/ablation_layer.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/activations_and_gradients.py` & `grad-cam-1.5.2/pytorch_grad_cam/activations_and_gradients.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/base_cam.py` & `grad-cam-1.5.2/pytorch_grad_cam/base_cam.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+from typing import Callable, List, Optional, Tuple
+
 import numpy as np
 import torch
 import ttach as tta
-from typing import Callable, List, Tuple, Optional
+
 from pytorch_grad_cam.activations_and_gradients import ActivationsAndGradients
-from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
 from pytorch_grad_cam.utils.image import scale_cam_image
 from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
+from pytorch_grad_cam.utils.svd_on_activations import get_2d_projection
 
 
 class BaseCAM:
-    def __init__(self,
-                 model: torch.nn.Module,
-                 target_layers: List[torch.nn.Module],
-                 reshape_transform: Callable = None,
-                 compute_input_gradient: bool = False,
-                 uses_gradients: bool = True,
-                 tta_transforms: Optional[tta.Compose] = None) -> None:
+    def __init__(
+        self,
+        model: torch.nn.Module,
+        target_layers: List[torch.nn.Module],
+        reshape_transform: Callable = None,
+        compute_input_gradient: bool = False,
+        uses_gradients: bool = True,
+        tta_transforms: Optional[tta.Compose] = None,
+    ) -> None:
         self.model = model.eval()
         self.target_layers = target_layers
 
         # Use the same device as the model.
         self.device = next(self.model.parameters()).device
         self.reshape_transform = reshape_transform
         self.compute_input_gradient = compute_input_gradient
@@ -30,178 +34,166 @@
                     tta.HorizontalFlip(),
                     tta.Multiply(factors=[0.9, 1, 1.1]),
                 ]
             )
         else:
             self.tta_transforms = tta_transforms
 
-        self.activations_and_grads = ActivationsAndGradients(
-            self.model, target_layers, reshape_transform)
+        self.activations_and_grads = ActivationsAndGradients(self.model, target_layers, reshape_transform)
 
     """ Get a vector of weights for every channel in the target layer.
         Methods that return weights channels,
         will typically need to only implement this function. """
 
-    def get_cam_weights(self,
-                        input_tensor: torch.Tensor,
-                        target_layers: List[torch.nn.Module],
-                        targets: List[torch.nn.Module],
-                        activations: torch.Tensor,
-                        grads: torch.Tensor) -> np.ndarray:
+    def get_cam_weights(
+        self,
+        input_tensor: torch.Tensor,
+        target_layers: List[torch.nn.Module],
+        targets: List[torch.nn.Module],
+        activations: torch.Tensor,
+        grads: torch.Tensor,
+    ) -> np.ndarray:
         raise Exception("Not Implemented")
 
-    def get_cam_image(self,
-                      input_tensor: torch.Tensor,
-                      target_layer: torch.nn.Module,
-                      targets: List[torch.nn.Module],
-                      activations: torch.Tensor,
-                      grads: torch.Tensor,
-                      eigen_smooth: bool = False) -> np.ndarray:
-
-        weights = self.get_cam_weights(input_tensor,
-                                       target_layer,
-                                       targets,
-                                       activations,
-                                       grads)
-        weighted_activations = weights[:, :, None, None] * activations
+    def get_cam_image(
+        self,
+        input_tensor: torch.Tensor,
+        target_layer: torch.nn.Module,
+        targets: List[torch.nn.Module],
+        activations: torch.Tensor,
+        grads: torch.Tensor,
+        eigen_smooth: bool = False,
+    ) -> np.ndarray:
+        weights = self.get_cam_weights(input_tensor, target_layer, targets, activations, grads)
+        # 2D conv
+        if len(activations.shape) == 4:
+            weighted_activations = weights[:, :, None, None] * activations
+        # 3D conv
+        elif len(activations.shape) == 5:
+            weighted_activations = weights[:, :, None, None, None] * activations
+        else:
+            raise ValueError(f"Invalid activation shape. Get {len(activations.shape)}.")
+
         if eigen_smooth:
             cam = get_2d_projection(weighted_activations)
         else:
             cam = weighted_activations.sum(axis=1)
         return cam
 
-    def forward(self,
-                input_tensor: torch.Tensor,
-                targets: List[torch.nn.Module],
-                eigen_smooth: bool = False) -> np.ndarray:
-
+    def forward(
+        self, input_tensor: torch.Tensor, targets: List[torch.nn.Module], eigen_smooth: bool = False
+    ) -> np.ndarray:
         input_tensor = input_tensor.to(self.device)
 
         if self.compute_input_gradient:
-            input_tensor = torch.autograd.Variable(input_tensor,
-                                                   requires_grad=True)
+            input_tensor = torch.autograd.Variable(input_tensor, requires_grad=True)
 
         self.outputs = outputs = self.activations_and_grads(input_tensor)
 
         if targets is None:
             target_categories = np.argmax(outputs.cpu().data.numpy(), axis=-1)
-            targets = [ClassifierOutputTarget(
-                category) for category in target_categories]
+            targets = [ClassifierOutputTarget(category) for category in target_categories]
 
         if self.uses_gradients:
             self.model.zero_grad()
-            loss = sum([target(output)
-                       for target, output in zip(targets, outputs)])
+            loss = sum([target(output) for target, output in zip(targets, outputs)])
             loss.backward(retain_graph=True)
 
         # In most of the saliency attribution papers, the saliency is
         # computed with a single target layer.
         # Commonly it is the last convolutional layer.
         # Here we support passing a list with multiple target layers.
         # It will compute the saliency image for every image,
         # and then aggregate them (with a default mean aggregation).
         # This gives you more flexibility in case you just want to
         # use all conv layers for example, all Batchnorm layers,
         # or something else.
-        cam_per_layer = self.compute_cam_per_layer(input_tensor,
-                                                   targets,
-                                                   eigen_smooth)
+        cam_per_layer = self.compute_cam_per_layer(input_tensor, targets, eigen_smooth)
         return self.aggregate_multi_layers(cam_per_layer)
 
-    def get_target_width_height(self,
-                                input_tensor: torch.Tensor) -> Tuple[int, int]:
-        width, height = input_tensor.size(-1), input_tensor.size(-2)
-        return width, height
+    def get_target_width_height(self, input_tensor: torch.Tensor) -> Tuple[int, int]:
+        if len(input_tensor.shape) == 4:
+            width, height = input_tensor.size(-1), input_tensor.size(-2)
+            return width, height
+        elif len(input_tensor.shape) == 5:
+            depth, width, height = input_tensor.size(-1), input_tensor.size(-2), input_tensor.size(-3)
+            return depth, width, height
+        else:
+            raise ValueError("Invalid input_tensor shape. Only 2D or 3D images are supported.")
 
     def compute_cam_per_layer(
-            self,
-            input_tensor: torch.Tensor,
-            targets: List[torch.nn.Module],
-            eigen_smooth: bool) -> np.ndarray:
-        activations_list = [a.cpu().data.numpy()
-                            for a in self.activations_and_grads.activations]
-        grads_list = [g.cpu().data.numpy()
-                      for g in self.activations_and_grads.gradients]
+        self, input_tensor: torch.Tensor, targets: List[torch.nn.Module], eigen_smooth: bool
+    ) -> np.ndarray:
+        activations_list = [a.cpu().data.numpy() for a in self.activations_and_grads.activations]
+        grads_list = [g.cpu().data.numpy() for g in self.activations_and_grads.gradients]
         target_size = self.get_target_width_height(input_tensor)
 
         cam_per_target_layer = []
         # Loop over the saliency image from every layer
         for i in range(len(self.target_layers)):
             target_layer = self.target_layers[i]
             layer_activations = None
             layer_grads = None
             if i < len(activations_list):
                 layer_activations = activations_list[i]
             if i < len(grads_list):
                 layer_grads = grads_list[i]
 
-            cam = self.get_cam_image(input_tensor,
-                                     target_layer,
-                                     targets,
-                                     layer_activations,
-                                     layer_grads,
-                                     eigen_smooth)
+            cam = self.get_cam_image(input_tensor, target_layer, targets, layer_activations, layer_grads, eigen_smooth)
             cam = np.maximum(cam, 0)
             scaled = scale_cam_image(cam, target_size)
             cam_per_target_layer.append(scaled[:, None, :])
 
         return cam_per_target_layer
 
-    def aggregate_multi_layers(
-            self,
-            cam_per_target_layer: np.ndarray) -> np.ndarray:
+    def aggregate_multi_layers(self, cam_per_target_layer: np.ndarray) -> np.ndarray:
         cam_per_target_layer = np.concatenate(cam_per_target_layer, axis=1)
         cam_per_target_layer = np.maximum(cam_per_target_layer, 0)
         result = np.mean(cam_per_target_layer, axis=1)
         return scale_cam_image(result)
 
-    def forward_augmentation_smoothing(self,
-                                       input_tensor: torch.Tensor,
-                                       targets: List[torch.nn.Module],
-                                       eigen_smooth: bool = False) -> np.ndarray:
+    def forward_augmentation_smoothing(
+        self, input_tensor: torch.Tensor, targets: List[torch.nn.Module], eigen_smooth: bool = False
+    ) -> np.ndarray:
         cams = []
         for transform in self.tta_transforms:
             augmented_tensor = transform.augment_image(input_tensor)
-            cam = self.forward(augmented_tensor,
-                               targets,
-                               eigen_smooth)
+            cam = self.forward(augmented_tensor, targets, eigen_smooth)
 
             # The ttach library expects a tensor of size BxCxHxW
             cam = cam[:, None, :, :]
             cam = torch.from_numpy(cam)
             cam = transform.deaugment_mask(cam)
 
             # Back to numpy float32, HxW
             cam = cam.numpy()
             cam = cam[:, 0, :, :]
             cams.append(cam)
 
         cam = np.mean(np.float32(cams), axis=0)
         return cam
 
-    def __call__(self,
-                 input_tensor: torch.Tensor,
-                 targets: List[torch.nn.Module] = None,
-                 aug_smooth: bool = False,
-                 eigen_smooth: bool = False) -> np.ndarray:
-
+    def __call__(
+        self,
+        input_tensor: torch.Tensor,
+        targets: List[torch.nn.Module] = None,
+        aug_smooth: bool = False,
+        eigen_smooth: bool = False,
+    ) -> np.ndarray:
         # Smooth the CAM result with test time augmentation
         if aug_smooth is True:
-            return self.forward_augmentation_smoothing(
-                input_tensor, targets, eigen_smooth)
+            return self.forward_augmentation_smoothing(input_tensor, targets, eigen_smooth)
 
-        return self.forward(input_tensor,
-                            targets, eigen_smooth)
+        return self.forward(input_tensor, targets, eigen_smooth)
 
     def __del__(self):
         self.activations_and_grads.release()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         self.activations_and_grads.release()
         if isinstance(exc_value, IndexError):
             # Handle IndexError here...
-            print(
-                f"An exception occurred in CAM with block: {exc_type}. Message: {exc_value}")
+            print(f"An exception occurred in CAM with block: {exc_type}. Message: {exc_value}")
             return True
```

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/eigen_cam.py` & `grad-cam-1.5.2/pytorch_grad_cam/eigen_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/eigen_grad_cam.py` & `grad-cam-1.5.2/pytorch_grad_cam/eigen_grad_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py` & `grad-cam-1.5.2/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/feature_factorization/utils.py` & `grad-cam-1.5.2/pytorch_grad_cam/feature_factorization/utils.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/fullgrad_cam.py` & `grad-cam-1.5.2/pytorch_grad_cam/fullgrad_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/grad_cam.py` & `grad-cam-1.5.2/pytorch_grad_cam/random_cam.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
 from pytorch_grad_cam.base_cam import BaseCAM
 
 
-class GradCAM(BaseCAM):
-    def __init__(self, model, target_layers,
+class RandomCAM(BaseCAM):
+    def __init__(self, model, target_layers, 
                  reshape_transform=None):
         super(
-            GradCAM,
+            RandomCAM,
             self).__init__(
             model,
             target_layers,
             reshape_transform)
 
     def get_cam_weights(self,
                         input_tensor,
                         target_layer,
                         target_category,
                         activations,
                         grads):
-        return np.mean(grads, axis=(2, 3))
+        return np.random.uniform(-1, 1, size=(grads.shape[0], grads.shape[1]))
```

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/grad_cam_elementwise.py` & `grad-cam-1.5.2/pytorch_grad_cam/grad_cam_elementwise.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/grad_cam_plusplus.py` & `grad-cam-1.5.2/pytorch_grad_cam/grad_cam_plusplus.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/guided_backprop.py` & `grad-cam-1.5.2/pytorch_grad_cam/guided_backprop.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/hirescam.py` & `grad-cam-1.5.2/pytorch_grad_cam/hirescam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/layer_cam.py` & `grad-cam-1.5.2/pytorch_grad_cam/layer_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/metrics/cam_mult_image.py` & `grad-cam-1.5.2/pytorch_grad_cam/metrics/cam_mult_image.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/metrics/perturbation_confidence.py` & `grad-cam-1.5.2/pytorch_grad_cam/metrics/perturbation_confidence.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/metrics/road.py` & `grad-cam-1.5.2/pytorch_grad_cam/metrics/road.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/score_cam.py` & `grad-cam-1.5.2/pytorch_grad_cam/score_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/utils/find_layers.py` & `grad-cam-1.5.2/pytorch_grad_cam/utils/find_layers.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/utils/image.py` & `grad-cam-1.5.2/pytorch_grad_cam/utils/image.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,190 @@
-import matplotlib
-from matplotlib import pyplot as plt
-from matplotlib.lines import Line2D
-import cv2
-import numpy as np
-import torch
-from torchvision.transforms import Compose, Normalize, ToTensor
-from typing import List, Dict
-import math
-
-
-def preprocess_image(
-    img: np.ndarray, mean=[
-        0.5, 0.5, 0.5], std=[
-            0.5, 0.5, 0.5]) -> torch.Tensor:
-    preprocessing = Compose([
-        ToTensor(),
-        Normalize(mean=mean, std=std)
-    ])
-    return preprocessing(img.copy()).unsqueeze(0)
-
-
-def deprocess_image(img):
-    """ see https://github.com/jacobgil/keras-grad-cam/blob/master/grad-cam.py#L65 """
-    img = img - np.mean(img)
-    img = img / (np.std(img) + 1e-5)
-    img = img * 0.1
-    img = img + 0.5
-    img = np.clip(img, 0, 1)
-    return np.uint8(img * 255)
-
-
-def show_cam_on_image(img: np.ndarray,
-                      mask: np.ndarray,
-                      use_rgb: bool = False,
-                      colormap: int = cv2.COLORMAP_JET,
-                      image_weight: float = 0.5) -> np.ndarray:
-    """ This function overlays the cam mask on the image as an heatmap.
-    By default the heatmap is in BGR format.
-
-    :param img: The base image in RGB or BGR format.
-    :param mask: The cam mask.
-    :param use_rgb: Whether to use an RGB or BGR heatmap, this should be set to True if 'img' is in RGB format.
-    :param colormap: The OpenCV colormap to be used.
-    :param image_weight: The final result is image_weight * img + (1-image_weight) * mask.
-    :returns: The default image with the cam overlay.
-    """
-    heatmap = cv2.applyColorMap(np.uint8(255 * mask), colormap)
-    if use_rgb:
-        heatmap = cv2.cvtColor(heatmap, cv2.COLOR_BGR2RGB)
-    heatmap = np.float32(heatmap) / 255
-
-    if np.max(img) > 1:
-        raise Exception(
-            "The input image should np.float32 in the range [0, 1]")
-
-    if image_weight < 0 or image_weight > 1:
-        raise Exception(
-            f"image_weight should be in the range [0, 1].\
-                Got: {image_weight}")
-
-    cam = (1 - image_weight) * heatmap + image_weight * img
-    cam = cam / np.max(cam)
-    return np.uint8(255 * cam)
-
-
-def create_labels_legend(concept_scores: np.ndarray,
-                         labels: Dict[int, str],
-                         top_k=2):
-    concept_categories = np.argsort(concept_scores, axis=1)[:, ::-1][:, :top_k]
-    concept_labels_topk = []
-    for concept_index in range(concept_categories.shape[0]):
-        categories = concept_categories[concept_index, :]
-        concept_labels = []
-        for category in categories:
-            score = concept_scores[concept_index, category]
-            label = f"{','.join(labels[category].split(',')[:3])}:{score:.2f}"
-            concept_labels.append(label)
-        concept_labels_topk.append("\n".join(concept_labels))
-    return concept_labels_topk
-
-
-def show_factorization_on_image(img: np.ndarray,
-                                explanations: np.ndarray,
-                                colors: List[np.ndarray] = None,
-                                image_weight: float = 0.5,
-                                concept_labels: List = None) -> np.ndarray:
-    """ Color code the different component heatmaps on top of the image.
-        Every component color code will be magnified according to the heatmap itensity
-        (by modifying the V channel in the HSV color space),
-        and optionally create a lagend that shows the labels.
-
-        Since different factorization component heatmaps can overlap in principle,
-        we need a strategy to decide how to deal with the overlaps.
-        This keeps the component that has a higher value in it's heatmap.
-
-    :param img: The base image RGB format.
-    :param explanations: A tensor of shape num_componetns x height x width, with the component visualizations.
-    :param colors: List of R, G, B colors to be used for the components.
-                   If None, will use the gist_rainbow cmap as a default.
-    :param image_weight: The final result is image_weight * img + (1-image_weight) * visualization.
-    :concept_labels: A list of strings for every component. If this is paseed, a legend that shows
-                     the labels and their colors will be added to the image.
-    :returns: The visualized image.
-    """
-    n_components = explanations.shape[0]
-    if colors is None:
-        # taken from https://github.com/edocollins/DFF/blob/master/utils.py
-        _cmap = plt.cm.get_cmap('gist_rainbow')
-        colors = [
-            np.array(
-                _cmap(i)) for i in np.arange(
-                0,
-                1,
-                1.0 /
-                n_components)]
-    concept_per_pixel = explanations.argmax(axis=0)
-    masks = []
-    for i in range(n_components):
-        mask = np.zeros(shape=(img.shape[0], img.shape[1], 3))
-        mask[:, :, :] = colors[i][:3]
-        explanation = explanations[i]
-        explanation[concept_per_pixel != i] = 0
-        mask = np.uint8(mask * 255)
-        mask = cv2.cvtColor(mask, cv2.COLOR_RGB2HSV)
-        mask[:, :, 2] = np.uint8(255 * explanation)
-        mask = cv2.cvtColor(mask, cv2.COLOR_HSV2RGB)
-        mask = np.float32(mask) / 255
-        masks.append(mask)
-
-    mask = np.sum(np.float32(masks), axis=0)
-    result = img * image_weight + mask * (1 - image_weight)
-    result = np.uint8(result * 255)
-
-    if concept_labels is not None:
-        px = 1 / plt.rcParams['figure.dpi']  # pixel in inches
-        fig = plt.figure(figsize=(result.shape[1] * px, result.shape[0] * px))
-        plt.rcParams['legend.fontsize'] = int(
-            14 * result.shape[0] / 256 / max(1, n_components / 6))
-        lw = 5 * result.shape[0] / 256
-        lines = [Line2D([0], [0], color=colors[i], lw=lw)
-                 for i in range(n_components)]
-        plt.legend(lines,
-                   concept_labels,
-                   mode="expand",
-                   fancybox=True,
-                   shadow=True)
-
-        plt.tight_layout(pad=0, w_pad=0, h_pad=0)
-        plt.axis('off')
-        fig.canvas.draw()
-        data = np.frombuffer(fig.canvas.tostring_rgb(), dtype=np.uint8)
-        plt.close(fig=fig)
-        data = data.reshape(fig.canvas.get_width_height()[::-1] + (3,))
-        data = cv2.resize(data, (result.shape[1], result.shape[0]))
-        result = np.hstack((result, data))
-    return result
-
-
-def scale_cam_image(cam, target_size=None):
-    result = []
-    for img in cam:
-        img = img - np.min(img)
-        img = img / (1e-7 + np.max(img))
-        if target_size is not None:
-            img = cv2.resize(img, target_size)
-        result.append(img)
-    result = np.float32(result)
-
-    return result
-
-
-def scale_accross_batch_and_channels(tensor, target_size):
-    batch_size, channel_size = tensor.shape[:2]
-    reshaped_tensor = tensor.reshape(
-        batch_size * channel_size, *tensor.shape[2:])
-    result = scale_cam_image(reshaped_tensor, target_size)
-    result = result.reshape(
-        batch_size,
-        channel_size,
-        target_size[1],
-        target_size[0])
-    return result
+import math
+from typing import Dict, List
+
+import cv2
+import matplotlib
+import numpy as np
+import torch
+from matplotlib import pyplot as plt
+from matplotlib.lines import Line2D
+from scipy.ndimage import zoom
+from torchvision.transforms import Compose, Normalize, ToTensor
+
+
+def preprocess_image(
+    img: np.ndarray, mean=[
+        0.5, 0.5, 0.5], std=[
+            0.5, 0.5, 0.5]) -> torch.Tensor:
+    preprocessing = Compose([
+        ToTensor(),
+        Normalize(mean=mean, std=std)
+    ])
+    return preprocessing(img.copy()).unsqueeze(0)
+
+
+def deprocess_image(img):
+    """ see https://github.com/jacobgil/keras-grad-cam/blob/master/grad-cam.py#L65 """
+    img = img - np.mean(img)
+    img = img / (np.std(img) + 1e-5)
+    img = img * 0.1
+    img = img + 0.5
+    img = np.clip(img, 0, 1)
+    return np.uint8(img * 255)
+
+
+def show_cam_on_image(img: np.ndarray,
+                      mask: np.ndarray,
+                      use_rgb: bool = False,
+                      colormap: int = cv2.COLORMAP_JET,
+                      image_weight: float = 0.5) -> np.ndarray:
+    """ This function overlays the cam mask on the image as an heatmap.
+    By default the heatmap is in BGR format.
+
+    :param img: The base image in RGB or BGR format.
+    :param mask: The cam mask.
+    :param use_rgb: Whether to use an RGB or BGR heatmap, this should be set to True if 'img' is in RGB format.
+    :param colormap: The OpenCV colormap to be used.
+    :param image_weight: The final result is image_weight * img + (1-image_weight) * mask.
+    :returns: The default image with the cam overlay.
+    """
+    heatmap = cv2.applyColorMap(np.uint8(255 * mask), colormap)
+    if use_rgb:
+        heatmap = cv2.cvtColor(heatmap, cv2.COLOR_BGR2RGB)
+    heatmap = np.float32(heatmap) / 255
+
+    if np.max(img) > 1:
+        raise Exception(
+            "The input image should np.float32 in the range [0, 1]")
+
+    if image_weight < 0 or image_weight > 1:
+        raise Exception(
+            f"image_weight should be in the range [0, 1].\
+                Got: {image_weight}")
+
+    cam = (1 - image_weight) * heatmap + image_weight * img
+    cam = cam / np.max(cam)
+    return np.uint8(255 * cam)
+
+
+def create_labels_legend(concept_scores: np.ndarray,
+                         labels: Dict[int, str],
+                         top_k=2):
+    concept_categories = np.argsort(concept_scores, axis=1)[:, ::-1][:, :top_k]
+    concept_labels_topk = []
+    for concept_index in range(concept_categories.shape[0]):
+        categories = concept_categories[concept_index, :]
+        concept_labels = []
+        for category in categories:
+            score = concept_scores[concept_index, category]
+            label = f"{','.join(labels[category].split(',')[:3])}:{score:.2f}"
+            concept_labels.append(label)
+        concept_labels_topk.append("\n".join(concept_labels))
+    return concept_labels_topk
+
+
+def show_factorization_on_image(img: np.ndarray,
+                                explanations: np.ndarray,
+                                colors: List[np.ndarray] = None,
+                                image_weight: float = 0.5,
+                                concept_labels: List = None) -> np.ndarray:
+    """ Color code the different component heatmaps on top of the image.
+        Every component color code will be magnified according to the heatmap itensity
+        (by modifying the V channel in the HSV color space),
+        and optionally create a lagend that shows the labels.
+
+        Since different factorization component heatmaps can overlap in principle,
+        we need a strategy to decide how to deal with the overlaps.
+        This keeps the component that has a higher value in it's heatmap.
+
+    :param img: The base image RGB format.
+    :param explanations: A tensor of shape num_componetns x height x width, with the component visualizations.
+    :param colors: List of R, G, B colors to be used for the components.
+                   If None, will use the gist_rainbow cmap as a default.
+    :param image_weight: The final result is image_weight * img + (1-image_weight) * visualization.
+    :concept_labels: A list of strings for every component. If this is paseed, a legend that shows
+                     the labels and their colors will be added to the image.
+    :returns: The visualized image.
+    """
+    n_components = explanations.shape[0]
+    if colors is None:
+        # taken from https://github.com/edocollins/DFF/blob/master/utils.py
+        _cmap = plt.cm.get_cmap('gist_rainbow')
+        colors = [
+            np.array(
+                _cmap(i)) for i in np.arange(
+                0,
+                1,
+                1.0 /
+                n_components)]
+    concept_per_pixel = explanations.argmax(axis=0)
+    masks = []
+    for i in range(n_components):
+        mask = np.zeros(shape=(img.shape[0], img.shape[1], 3))
+        mask[:, :, :] = colors[i][:3]
+        explanation = explanations[i]
+        explanation[concept_per_pixel != i] = 0
+        mask = np.uint8(mask * 255)
+        mask = cv2.cvtColor(mask, cv2.COLOR_RGB2HSV)
+        mask[:, :, 2] = np.uint8(255 * explanation)
+        mask = cv2.cvtColor(mask, cv2.COLOR_HSV2RGB)
+        mask = np.float32(mask) / 255
+        masks.append(mask)
+
+    mask = np.sum(np.float32(masks), axis=0)
+    result = img * image_weight + mask * (1 - image_weight)
+    result = np.uint8(result * 255)
+
+    if concept_labels is not None:
+        px = 1 / plt.rcParams['figure.dpi']  # pixel in inches
+        fig = plt.figure(figsize=(result.shape[1] * px, result.shape[0] * px))
+        plt.rcParams['legend.fontsize'] = int(
+            14 * result.shape[0] / 256 / max(1, n_components / 6))
+        lw = 5 * result.shape[0] / 256
+        lines = [Line2D([0], [0], color=colors[i], lw=lw)
+                 for i in range(n_components)]
+        plt.legend(lines,
+                   concept_labels,
+                   mode="expand",
+                   fancybox=True,
+                   shadow=True)
+
+        plt.tight_layout(pad=0, w_pad=0, h_pad=0)
+        plt.axis('off')
+        fig.canvas.draw()
+        data = np.frombuffer(fig.canvas.tostring_rgb(), dtype=np.uint8)
+        plt.close(fig=fig)
+        data = data.reshape(fig.canvas.get_width_height()[::-1] + (3,))
+        data = cv2.resize(data, (result.shape[1], result.shape[0]))
+        result = np.hstack((result, data))
+    return result
+
+
+def scale_cam_image(cam, target_size=None):
+    result = []
+    for img in cam:
+        img = img - np.min(img)
+        img = img / (1e-7 + np.max(img))
+        if target_size is not None:
+            if len(img.shape) > 3:
+                img = zoom(np.float32(img), [
+                           (t_s / i_s) for i_s, t_s in zip(img.shape, target_size[::-1])])
+            else:
+                img = cv2.resize(np.float32(img), target_size)
+
+        result.append(img)
+    result = np.float32(result)
+
+    return result
+
+
+def scale_accross_batch_and_channels(tensor, target_size):
+    batch_size, channel_size = tensor.shape[:2]
+    reshaped_tensor = tensor.reshape(
+        batch_size * channel_size, *tensor.shape[2:])
+    result = scale_cam_image(reshaped_tensor, target_size)
+    result = result.reshape(
+        batch_size,
+        channel_size,
+        target_size[1],
+        target_size[0])
+    return result
```

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/utils/model_targets.py` & `grad-cam-1.5.2/pytorch_grad_cam/utils/model_targets.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/utils/reshape_transforms.py` & `grad-cam-1.5.2/pytorch_grad_cam/utils/reshape_transforms.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/utils/svd_on_activations.py` & `grad-cam-1.5.2/pytorch_grad_cam/utils/svd_on_activations.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/pytorch_grad_cam/xgrad_cam.py` & `grad-cam-1.5.2/pytorch_grad_cam/xgrad_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/setup.cfg` & `grad-cam-1.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/setup.py` & `grad-cam-1.5.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name='grad-cam',
-    version='1.5.0',
+    version='1.5.2',
     author='Jacob Gildenblat',
     author_email='jacob.gildenblat@gmail.com',
     description='Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jacobgil/pytorch-grad-cam',
     project_urls={
```

### Comparing `grad-cam-1.5.0/tests/test_context_release.py` & `grad-cam-1.5.2/tests/test_context_release.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/tests/test_one_channel.py` & `grad-cam-1.5.2/tests/test_one_channel.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/tests/test_run_all_models.py` & `grad-cam-1.5.2/tests/test_run_all_models.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/usage_examples/swinT_example.py` & `grad-cam-1.5.2/usage_examples/swinT_example.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.5.0/usage_examples/vit_example.py` & `grad-cam-1.5.2/usage_examples/vit_example.py`

 * *Files identical despite different names*

