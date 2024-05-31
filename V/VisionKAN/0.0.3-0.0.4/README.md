# Comparing `tmp/visionkan-0.0.3.tar.gz` & `tmp/visionkan-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionkan-0.0.3.tar", max compression
+gzip compressed data, was "visionkan-0.0.4.tar", max compression
```

## Comparing `visionkan-0.0.3.tar` & `visionkan-0.0.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0     1102 2024-05-31 16:36:40.177207 visionkan-0.0.3/LICENSE
--rw-r--r--   0        0        0     4433 2024-05-31 17:24:34.327056 visionkan-0.0.3/README.md
--rw-r--r--   0        0        0       14 2024-05-31 14:53:12.873637 visionkan-0.0.3/Vision-KAN/.git/COMMIT_EDITMSG
--rw-r--r--   0        0        0      243 2024-05-31 17:22:42.364089 visionkan-0.0.3/Vision-KAN/.git/FETCH_HEAD
--rw-r--r--   0        0        0       24 2024-05-31 13:36:40.958192 visionkan-0.0.3/Vision-KAN/.git/HEAD
--rw-r--r--   0        0        0       41 2024-05-31 14:49:00.691392 visionkan-0.0.3/Vision-KAN/.git/ORIG_HEAD
--rw-r--r--   0        0        0      295 2024-05-31 14:33:25.446489 visionkan-0.0.3/Vision-KAN/.git/config
--rw-r--r--   0        0        0       73 2024-05-24 15:35:10.174032 visionkan-0.0.3/Vision-KAN/.git/description
--rwxr-xr-x   0        0        0      482 2024-05-24 15:35:10.167913 visionkan-0.0.3/Vision-KAN/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      900 2024-05-24 15:35:10.168428 visionkan-0.0.3/Vision-KAN/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4726 2024-05-24 15:35:10.171932 visionkan-0.0.3/Vision-KAN/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      193 2024-05-24 15:35:10.168734 visionkan-0.0.3/Vision-KAN/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      428 2024-05-24 15:35:10.168957 visionkan-0.0.3/Vision-KAN/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1647 2024-05-24 15:35:10.169177 visionkan-0.0.3/Vision-KAN/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      420 2024-05-24 15:35:10.169509 visionkan-0.0.3/Vision-KAN/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1378 2024-05-24 15:35:10.169703 visionkan-0.0.3/Vision-KAN/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4902 2024-05-24 15:35:10.172481 visionkan-0.0.3/Vision-KAN/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      548 2024-05-24 15:35:10.170019 visionkan-0.0.3/Vision-KAN/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1496 2024-05-24 15:35:10.172800 visionkan-0.0.3/Vision-KAN/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2787 2024-05-24 15:35:10.170207 visionkan-0.0.3/Vision-KAN/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     3654 2024-05-24 15:35:10.170529 visionkan-0.0.3/Vision-KAN/.git/hooks/update.sample
--rw-r--r--   0        0        0     1530 2024-05-31 14:53:12.871967 visionkan-0.0.3/Vision-KAN/.git/index
--rw-r--r--   0        0        0      240 2024-05-24 15:35:10.173729 visionkan-0.0.3/Vision-KAN/.git/info/exclude
--rw-r--r--   0        0        0     1768 2024-05-31 14:53:12.876899 visionkan-0.0.3/Vision-KAN/.git/logs/HEAD
--rw-r--r--   0        0        0      409 2024-05-31 13:34:21.568699 visionkan-0.0.3/Vision-KAN/.git/logs/refs/heads/main
--rw-r--r--   0        0        0     1347 2024-05-31 14:53:12.878261 visionkan-0.0.3/Vision-KAN/.git/logs/refs/heads/patch-1
--rw-r--r--   0        0        0      220 2024-05-24 15:35:10.445968 visionkan-0.0.3/Vision-KAN/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0      880 2024-05-31 16:17:30.671518 visionkan-0.0.3/Vision-KAN/.git/logs/refs/remotes/origin/main
--rw-r--r--   0        0        0     1226 2024-05-31 14:53:25.746790 visionkan-0.0.3/Vision-KAN/.git/logs/refs/remotes/origin/patch-1
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.010280 visionkan-0.0.3/Vision-KAN/.git/objects/03/5758c4872124d834ee6e539c4b85b2a6be311c
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.005345 visionkan-0.0.3/Vision-KAN/.git/objects/06/6241d382a6833daa9cd15cd1ed9f1d276e9351
--rw-r--r--   0        0        0     1287 2024-05-25 14:20:36.238615 visionkan-0.0.3/Vision-KAN/.git/objects/06/68b38d953d4aaff834ef30fcbb54ace8b44db8
--rw-r--r--   0        0        0      840 2024-05-30 13:45:38.994164 visionkan-0.0.3/Vision-KAN/.git/objects/06/74abe9ee0925ae39a471b2bcda4ef468da405a
--rw-r--r--   0        0        0     1507 2024-05-30 13:45:39.016541 visionkan-0.0.3/Vision-KAN/.git/objects/09/cabeca13a688a93d1d3268c300759fa2c66325
--rw-r--r--   0        0        0     1319 2024-05-30 13:45:39.024783 visionkan-0.0.3/Vision-KAN/.git/objects/0c/3fdd176183c8a66b347340e4d84ad918cbc18c
--rw-r--r--   0        0        0     1317 2024-05-25 16:05:34.641678 visionkan-0.0.3/Vision-KAN/.git/objects/12/9a6e0aad0a851e986186c74ddb3ce96adaf5ee
--rw-r--r--   0        0        0     6856 2024-05-31 14:32:24.518636 visionkan-0.0.3/Vision-KAN/.git/objects/13/b30851219f73fd58967c40ff74387ffb424188
--rw-r--r--   0        0        0     1506 2024-05-30 13:45:39.011851 visionkan-0.0.3/Vision-KAN/.git/objects/15/12f01aeb2737c67d44e5a2de3daab934bc00d4
--rw-r--r--   0        0        0      494 2024-05-25 14:20:36.237613 visionkan-0.0.3/Vision-KAN/.git/objects/15/882637c211157b37fd7eabb34894795520e0bb
--rw-r--r--   0        0        0     1170 2024-05-31 13:33:51.648165 visionkan-0.0.3/Vision-KAN/.git/objects/16/8c00f3102d915e4bc73d1034f91549ad22e428
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.002263 visionkan-0.0.3/Vision-KAN/.git/objects/21/fbe556dd1106f6a79eb78fac39019b38d89519
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.022019 visionkan-0.0.3/Vision-KAN/.git/objects/25/3f201824ad7beb456236e0b910d2c0a9d1df2d
--rw-r--r--   0        0        0      677 2024-05-31 14:53:04.833593 visionkan-0.0.3/Vision-KAN/.git/objects/27/9af88c958e602fe7e7836555be28ab6b2dcb20
--rw-r--r--   0        0        0     1506 2024-05-30 13:45:39.013923 visionkan-0.0.3/Vision-KAN/.git/objects/29/ff87b50e72193eec1f7a4f5385f30d66f53613
--rw-r--r--   0        0        0     1508 2024-05-30 13:45:39.009225 visionkan-0.0.3/Vision-KAN/.git/objects/2b/d3ddb40f4749eb5e1b1c3965cc8ab399c91f93
--rw-r--r--   0        0        0      494 2024-05-31 13:34:21.562548 visionkan-0.0.3/Vision-KAN/.git/objects/2c/dd22f3aa4c47e3545301d4da191b68fc94f1c5
--rw-r--r--   0        0        0      521 2024-05-31 14:33:27.090702 visionkan-0.0.3/Vision-KAN/.git/objects/35/c12e9342863df9c5d6a8ec1efb8b9cb9169b37
--rw-r--r--   0        0        0      818 2024-05-31 14:49:00.672759 visionkan-0.0.3/Vision-KAN/.git/objects/43/6f239ee660810f0025cd0baf2bd57e66fce109
--rw-r--r--   0        0        0      493 2024-05-30 14:33:26.786303 visionkan-0.0.3/Vision-KAN/.git/objects/43/d403b1cc332e3f220e936ef1b3b6fbf94448c3
--rw-r--r--   0        0        0      183 2024-05-31 14:53:12.874375 visionkan-0.0.3/Vision-KAN/.git/objects/44/70e85c1e0811b1fd6ef8ad32f01c35285a2d68
--rw-r--r--   0        0        0      837 2024-05-30 13:45:38.998331 visionkan-0.0.3/Vision-KAN/.git/objects/44/e907d19bcaf6fb23d971e191ac29d317eab980
--rw-r--r--   0        0        0      836 2024-05-30 13:45:38.992896 visionkan-0.0.3/Vision-KAN/.git/objects/46/752e8ceaeaca3e493ab2a35afb3d481dfd8a45
--rw-r--r--   0        0        0      493 2024-05-25 14:20:36.240943 visionkan-0.0.3/Vision-KAN/.git/objects/4a/1e4d2ff99d121790b8e3e21ddec07e0b064c29
--rw-r--r--   0        0        0      841 2024-05-25 14:20:36.234901 visionkan-0.0.3/Vision-KAN/.git/objects/4a/4455c1797f8ca10833017712f420b667f5e2c7
--rw-r--r--   0        0        0      819 2024-05-30 13:45:38.995549 visionkan-0.0.3/Vision-KAN/.git/objects/4e/0f0d2e944cb103da318db1efea21f0b965e2b1
--rw-r--r--   0        0        0     1466 2024-05-30 13:45:39.020279 visionkan-0.0.3/Vision-KAN/.git/objects/56/336fbf8d500db9a2c6cb3becb0953f568ac4e1
--rw-r--r--   0        0        0      824 2024-05-30 13:45:38.991028 visionkan-0.0.3/Vision-KAN/.git/objects/56/7434cb3ff4fef14ec5845ea9a9460c4cb08d9b
--rw-r--r--   0        0        0     1038 2024-05-31 14:48:55.244146 visionkan-0.0.3/Vision-KAN/.git/objects/5c/b18af65e33aa342b6cf265fdda19720883197d
--rw-r--r--   0        0        0      843 2024-05-25 14:20:36.236438 visionkan-0.0.3/Vision-KAN/.git/objects/5d/2cdd8e6f86eb49afc4b8cc6112dfc087e67b4b
--rw-r--r--   0        0        0      121 2024-05-31 14:48:55.244374 visionkan-0.0.3/Vision-KAN/.git/objects/65/0d1fd130531d23d807d0336f75f011ffd1af95
--rw-r--r--   0        0        0      897 2024-05-31 16:17:30.631689 visionkan-0.0.3/Vision-KAN/.git/objects/69/91a7f628ac78a0ea2a7cd7deca258f6ca303f7
--rw-r--r--   0        0        0     1848 2024-05-31 14:04:43.843201 visionkan-0.0.3/Vision-KAN/.git/objects/6a/00d1becfc1105d37b0bd8fe4ead459425484e3
--rw-r--r--   0        0        0      184 2024-05-31 14:49:14.673971 visionkan-0.0.3/Vision-KAN/.git/objects/6a/f10ebd18db1f3301de38d19f9689a7b2311036
--rw-r--r--   0        0        0       61 2024-05-31 13:33:51.647179 visionkan-0.0.3/Vision-KAN/.git/objects/6b/4b62ae4705d9c1f3bbbdd970f69b56552b7ad0
--rw-r--r--   0        0        0      840 2024-05-30 13:45:38.991888 visionkan-0.0.3/Vision-KAN/.git/objects/6d/4fee0c09fe53ef076b8ca569c76d8ef0e9c0be
--rw-r--r--   0        0        0      630 2024-05-31 16:17:30.632415 visionkan-0.0.3/Vision-KAN/.git/objects/70/b1eef9982cebe6f1bc10e1fd644b31c7fb40fb
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.019492 visionkan-0.0.3/Vision-KAN/.git/objects/71/4760bd63cff5586b975798a51d9f5b9abd9c98
--rw-r--r--   0        0        0      818 2024-05-30 13:45:38.996310 visionkan-0.0.3/Vision-KAN/.git/objects/77/2f83ad9b280531ffe3575c3bf3a084dde9dda8
--rw-r--r--   0        0        0      521 2024-05-31 14:32:40.853130 visionkan-0.0.3/Vision-KAN/.git/objects/79/6b48f77c56e8b31fa26df0c09faa2f58a21933
--rw-r--r--   0        0        0      275 2024-05-31 14:53:04.834456 visionkan-0.0.3/Vision-KAN/.git/objects/7b/65ba50b57d47abdb10a72e10af24141c5f1e23
--rw-r--r--   0        0        0      263 2024-05-31 13:38:09.217336 visionkan-0.0.3/Vision-KAN/.git/objects/7f/8d64c1877aae28d07cc44e14e41754783b9d1f
--rw-r--r--   0        0        0      913 2024-05-25 16:05:34.642373 visionkan-0.0.3/Vision-KAN/.git/objects/84/32edbe772c608ef21c8ea9888b4b153572b1c4
--rw-r--r--   0        0        0      494 2024-05-25 14:20:36.239279 visionkan-0.0.3/Vision-KAN/.git/objects/84/ccf3adbe9ed1f4e754ec299aadd9d01122a306
--rw-r--r--   0        0        0     2006 2024-05-31 16:17:30.633745 visionkan-0.0.3/Vision-KAN/.git/objects/86/3baf687b25c96a0475896b31920698bfb547d3
--rw-r--r--   0        0        0      819 2024-05-30 13:45:38.990222 visionkan-0.0.3/Vision-KAN/.git/objects/86/638aea647100826572038a201b3aa540ba361d
--rw-r--r--   0        0        0      494 2024-05-31 13:37:51.709443 visionkan-0.0.3/Vision-KAN/.git/objects/86/799c8a3e5fd7b900f08c88e0cca639850fc294
--rw-r--r--   0        0        0      821 2024-05-31 14:04:43.840635 visionkan-0.0.3/Vision-KAN/.git/objects/88/3f6618e8a967e22cd911a293df9f580dedfc80
--rw-r--r--   0        0        0     1865 2024-05-31 14:49:00.675912 visionkan-0.0.3/Vision-KAN/.git/objects/89/df25510efa3d32d3a185632510e51e0b5ac587
--rw-r--r--   0        0        0      839 2024-05-30 13:45:38.999243 visionkan-0.0.3/Vision-KAN/.git/objects/8a/18123c11a366bf202025fbfcad890ba85f85db
--rw-r--r--   0        0        0      838 2024-05-30 14:33:26.785333 visionkan-0.0.3/Vision-KAN/.git/objects/8a/54f42e59da31cf4fab9e75821cd6dc38de66e1
--rw-r--r--   0        0        0     1664 2024-05-30 14:33:26.787040 visionkan-0.0.3/Vision-KAN/.git/objects/98/5a41303f0b376424104732aae1cf6c26f107b0
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.007970 visionkan-0.0.3/Vision-KAN/.git/objects/a0/32cdc4f076cbbf159d16ce87dd1c004acb9cc6
--rw-r--r--   0        0        0      840 2024-05-30 13:45:39.000137 visionkan-0.0.3/Vision-KAN/.git/objects/a0/f9955482da7bbbc35d37396db4e7e5701e9c28
--rw-r--r--   0        0        0      630 2024-05-31 14:53:12.871608 visionkan-0.0.3/Vision-KAN/.git/objects/a9/7a8bfdb02e47eac5f95ffc887ff9137eb58e33
--rw-r--r--   0        0        0     6819 2024-05-31 13:33:51.687559 visionkan-0.0.3/Vision-KAN/.git/objects/b6/696a95d7f64217f0fece92139644ee203cf2b0
--rw-r--r--   0        0        0      494 2024-05-31 14:04:43.841489 visionkan-0.0.3/Vision-KAN/.git/objects/b7/4f0c2f72935f7521485b89031e8e95e2371820
--rw-r--r--   0        0        0      188 2024-05-31 13:34:21.564914 visionkan-0.0.3/Vision-KAN/.git/objects/bd/7fd2adf69a9075779ce023a53a26ffc20aebf4
--rw-r--r--   0        0        0     1506 2024-05-31 13:33:51.673512 visionkan-0.0.3/Vision-KAN/.git/objects/bf/bd0b862c1b0a15f144f53f7df02a252c37c01d
--rw-r--r--   0        0        0      493 2024-05-25 16:05:34.586080 visionkan-0.0.3/Vision-KAN/.git/objects/bf/e3c8a6391f11a33cba14538ac78722c4509966
--rw-r--r--   0        0        0      837 2024-05-25 16:05:34.584618 visionkan-0.0.3/Vision-KAN/.git/objects/c9/79bca54c422dc3a5f94ddbfcea861b354e049c
--rw-r--r--   0        0        0      561 2024-05-31 14:49:14.671088 visionkan-0.0.3/Vision-KAN/.git/objects/cc/3a210486203faf4a7d3fc808b58a427af0e996
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.012831 visionkan-0.0.3/Vision-KAN/.git/objects/cc/7b9c064b952a571a49427d736064342fc5d24c
--rw-r--r--   0        0        0      264 2024-05-31 14:33:30.522785 visionkan-0.0.3/Vision-KAN/.git/objects/cd/67ec395c8a3d6d2b6af4d25c5c4dc74388de8e
--rw-r--r--   0        0        0     1439 2024-05-30 13:45:39.018627 visionkan-0.0.3/Vision-KAN/.git/objects/cd/85a76fe43e08cf4e7b9b363dc2542ff4f39da2
--rw-r--r--   0        0        0     2006 2024-05-31 14:53:04.832605 visionkan-0.0.3/Vision-KAN/.git/objects/cd/8ac765c6d6e22fbeff50a342231d49454816fb
--rw-r--r--   0        0        0     2609 2024-05-31 13:33:51.698886 visionkan-0.0.3/Vision-KAN/.git/objects/d2/c20123b2340bec1c7f22363a5c867d66fa5c87
--rw-r--r--   0        0        0     2667 2024-05-31 14:32:24.568609 visionkan-0.0.3/Vision-KAN/.git/objects/d3/d265b925f92f1e17fba0896d3e041ea5d32aa4
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.017651 visionkan-0.0.3/Vision-KAN/.git/objects/dc/865eaf4ea0b28b422621902e9a5a0a2df5177a
--rw-r--r--   0        0        0     1462 2024-05-30 13:45:39.022977 visionkan-0.0.3/Vision-KAN/.git/objects/de/c987774b10e51d1574a82830ea20fa66e1ab9b
--rw-r--r--   0        0        0      521 2024-05-31 14:49:00.673749 visionkan-0.0.3/Vision-KAN/.git/objects/e1/dd05a85418b7679ed648eef24b113ceace9d4d
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.015287 visionkan-0.0.3/Vision-KAN/.git/objects/e9/d6a23a2cc05561da18f235fe79d1f58c9c81bb
--rw-r--r--   0        0        0      841 2024-05-25 14:20:36.235936 visionkan-0.0.3/Vision-KAN/.git/objects/ea/b5de8755717ee2c3eca3382fedb489252551cc
--rw-r--r--   0        0        0     1193 2024-05-25 14:20:36.242033 visionkan-0.0.3/Vision-KAN/.git/objects/eb/69480d3d8e32c0d18cfe47e6f3501c0a04097c
--rw-r--r--   0        0        0     1197 2024-05-25 14:20:36.240180 visionkan-0.0.3/Vision-KAN/.git/objects/ec/5afec8cf55319913cf0dffef27ed2e4513a89f
--rw-r--r--   0        0        0      493 2024-05-30 13:45:39.023865 visionkan-0.0.3/Vision-KAN/.git/objects/f4/d8d97e8689fe0ca5b1218098d7df8fdc5a66a1
--rw-r--r--   0        0        0     1670 2024-05-30 13:45:39.006098 visionkan-0.0.3/Vision-KAN/.git/objects/f7/77f1ace2c84ba7411c7b9b36f8016262bdf565
--rw-r--r--   0        0        0     1662 2024-05-30 13:45:39.004604 visionkan-0.0.3/Vision-KAN/.git/objects/f7/eebc418a1d2e4790a20aa8bd06a71612065ce1
--rw-r--r--   0        0        0      929 2024-05-30 13:45:38.994918 visionkan-0.0.3/Vision-KAN/.git/objects/fa/ef8af61c4f860b09d810bf73d34b6f1505f88f
--rw-r--r--   0        0        0      188 2024-05-31 14:32:40.856549 visionkan-0.0.3/Vision-KAN/.git/objects/fc/0f3b6701e2cf4679070f83418f6832c20dd94a
--rw-r--r--   0        0        0     5132 2024-05-24 15:35:10.437127 visionkan-0.0.3/Vision-KAN/.git/objects/pack/pack-b923ccab73ed5f6d720c7d92156d1d6412751d26.idx
--rw-r--r--   0        0        0    67923 2024-05-24 15:35:10.436764 visionkan-0.0.3/Vision-KAN/.git/objects/pack/pack-b923ccab73ed5f6d720c7d92156d1d6412751d26.pack
--rw-r--r--   0        0        0      112 2024-05-24 15:35:10.444369 visionkan-0.0.3/Vision-KAN/.git/packed-refs
--rw-r--r--   0        0        0       41 2024-05-31 13:34:21.566187 visionkan-0.0.3/Vision-KAN/.git/refs/heads/main
--rw-r--r--   0        0        0       41 2024-05-31 14:53:12.875969 visionkan-0.0.3/Vision-KAN/.git/refs/heads/patch-1
--rw-r--r--   0        0        0       30 2024-05-24 15:35:10.446019 visionkan-0.0.3/Vision-KAN/.git/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0       41 2024-05-31 16:17:30.665858 visionkan-0.0.3/Vision-KAN/.git/refs/remotes/origin/main
--rw-r--r--   0        0        0       41 2024-05-31 14:53:25.744676 visionkan-0.0.3/Vision-KAN/.git/refs/remotes/origin/patch-1
--rw-r--r--   0        0        0       49 2024-05-31 13:33:36.981809 visionkan-0.0.3/Vision-KAN/.gitignore
--rw-r--r--   0        0        0     2267 2024-05-24 15:35:10.449051 visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/README-checkpoint.md
--rw-r--r--   0        0        0     3456 2024-05-24 15:51:59.818683 visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/augment-checkpoint.py
--rw-r--r--   0        0        0     4441 2024-05-25 01:13:48.567915 visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/datasets-checkpoint.py
--rw-r--r--   0        0        0    23357 2024-05-25 17:06:25.070376 visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/main-checkpoint.py
--rw-r--r--   0        0        0    11849 2024-05-25 17:13:58.729211 visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/models_kan-checkpoint.py
--rw-r--r--   0        0        0       45 2024-05-24 15:35:10.451860 visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/requirements-checkpoint.txt
--rw-r--r--   0        0        0     1102 2024-05-31 14:52:54.053362 visionkan-0.0.3/Vision-KAN/LICENSE
--rw-r--r--   0        0        0     4431 2024-05-31 17:14:54.486745 visionkan-0.0.3/Vision-KAN/README.md
--rw-r--r--   0        0        0      156 2024-05-31 14:45:13.060714 visionkan-0.0.3/Vision-KAN/__init__.py
--rw-r--r--   0        0        0     3456 2024-05-24 15:51:59.818683 visionkan-0.0.3/Vision-KAN/augment.py
--rw-r--r--   0        0        0     4441 2024-05-25 01:13:48.567915 visionkan-0.0.3/Vision-KAN/datasets.py
--rw-r--r--   0        0        0    10325 2024-05-24 15:35:10.449538 visionkan-0.0.3/Vision-KAN/ekan.py
--rw-r--r--   0        0        0     4241 2024-05-24 15:35:10.449722 visionkan-0.0.3/Vision-KAN/engine.py
--rw-r--r--   0        0        0     5304 2024-05-24 15:35:10.449878 visionkan-0.0.3/Vision-KAN/fasterkan.py
--rw-r--r--   0        0        0      227 2024-05-24 15:35:10.449989 visionkan-0.0.3/Vision-KAN/hubconf.py
--rw-r--r--   0        0        0    23182 2024-05-24 15:35:10.451029 visionkan-0.0.3/Vision-KAN/kit.py
--rw-r--r--   0        0        0     3388 2024-05-24 15:35:10.451223 visionkan-0.0.3/Vision-KAN/losses.py
--rw-r--r--   0        0        0    23450 2024-05-31 13:58:16.520299 visionkan-0.0.3/Vision-KAN/main.py
--rw-r--r--   0        0        0     2365 2024-05-31 14:32:01.592511 visionkan-0.0.3/Vision-KAN/minimal_example.py
--rw-r--r--   0        0        0    13424 2024-05-31 14:19:18.261471 visionkan-0.0.3/Vision-KAN/models_kan.py
--rw-r--r--   0        0        0       45 2024-05-24 15:35:10.451860 visionkan-0.0.3/Vision-KAN/requirements.txt
--rw-r--r--   0        0        0     2584 2024-05-24 15:35:10.452108 visionkan-0.0.3/Vision-KAN/samplers.py
--rw-r--r--   0        0        0     7086 2024-05-24 15:35:10.452288 visionkan-0.0.3/Vision-KAN/utils.py
--rw-r--r--   0        0        0      666 2024-05-31 17:25:35.788281 visionkan-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 visionkan-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-05-31 16:36:40.177207 visionkan-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4433 2024-05-31 17:24:34.327056 visionkan-0.0.4/README.md
+-rw-r--r--   0        0        0       14 2024-05-31 14:53:12.873637 visionkan-0.0.4/VisionKAN/.git/COMMIT_EDITMSG
+-rw-r--r--   0        0        0      243 2024-05-31 18:11:51.747416 visionkan-0.0.4/VisionKAN/.git/FETCH_HEAD
+-rw-r--r--   0        0        0       24 2024-05-31 13:36:40.958192 visionkan-0.0.4/VisionKAN/.git/HEAD
+-rw-r--r--   0        0        0       41 2024-05-31 14:49:00.691392 visionkan-0.0.4/VisionKAN/.git/ORIG_HEAD
+-rw-r--r--   0        0        0      295 2024-05-31 14:33:25.446489 visionkan-0.0.4/VisionKAN/.git/config
+-rw-r--r--   0        0        0       73 2024-05-24 15:35:10.174032 visionkan-0.0.4/VisionKAN/.git/description
+-rwxr-xr-x   0        0        0      482 2024-05-24 15:35:10.167913 visionkan-0.0.4/VisionKAN/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      900 2024-05-24 15:35:10.168428 visionkan-0.0.4/VisionKAN/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4726 2024-05-24 15:35:10.171932 visionkan-0.0.4/VisionKAN/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      193 2024-05-24 15:35:10.168734 visionkan-0.0.4/VisionKAN/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      428 2024-05-24 15:35:10.168957 visionkan-0.0.4/VisionKAN/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1647 2024-05-24 15:35:10.169177 visionkan-0.0.4/VisionKAN/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      420 2024-05-24 15:35:10.169509 visionkan-0.0.4/VisionKAN/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1378 2024-05-24 15:35:10.169703 visionkan-0.0.4/VisionKAN/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4902 2024-05-24 15:35:10.172481 visionkan-0.0.4/VisionKAN/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      548 2024-05-24 15:35:10.170019 visionkan-0.0.4/VisionKAN/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1496 2024-05-24 15:35:10.172800 visionkan-0.0.4/VisionKAN/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2787 2024-05-24 15:35:10.170207 visionkan-0.0.4/VisionKAN/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     3654 2024-05-24 15:35:10.170529 visionkan-0.0.4/VisionKAN/.git/hooks/update.sample
+-rw-r--r--   0        0        0     1530 2024-05-31 14:53:12.871967 visionkan-0.0.4/VisionKAN/.git/index
+-rw-r--r--   0        0        0      240 2024-05-24 15:35:10.173729 visionkan-0.0.4/VisionKAN/.git/info/exclude
+-rw-r--r--   0        0        0     1768 2024-05-31 14:53:12.876899 visionkan-0.0.4/VisionKAN/.git/logs/HEAD
+-rw-r--r--   0        0        0      409 2024-05-31 13:34:21.568699 visionkan-0.0.4/VisionKAN/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0     1347 2024-05-31 14:53:12.878261 visionkan-0.0.4/VisionKAN/.git/logs/refs/heads/patch-1
+-rw-r--r--   0        0        0      220 2024-05-24 15:35:10.445968 visionkan-0.0.4/VisionKAN/.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0      880 2024-05-31 16:17:30.671518 visionkan-0.0.4/VisionKAN/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0        0        0     1226 2024-05-31 14:53:25.746790 visionkan-0.0.4/VisionKAN/.git/logs/refs/remotes/origin/patch-1
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.010280 visionkan-0.0.4/VisionKAN/.git/objects/03/5758c4872124d834ee6e539c4b85b2a6be311c
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.005345 visionkan-0.0.4/VisionKAN/.git/objects/06/6241d382a6833daa9cd15cd1ed9f1d276e9351
+-rw-r--r--   0        0        0     1287 2024-05-25 14:20:36.238615 visionkan-0.0.4/VisionKAN/.git/objects/06/68b38d953d4aaff834ef30fcbb54ace8b44db8
+-rw-r--r--   0        0        0      840 2024-05-30 13:45:38.994164 visionkan-0.0.4/VisionKAN/.git/objects/06/74abe9ee0925ae39a471b2bcda4ef468da405a
+-rw-r--r--   0        0        0     1507 2024-05-30 13:45:39.016541 visionkan-0.0.4/VisionKAN/.git/objects/09/cabeca13a688a93d1d3268c300759fa2c66325
+-rw-r--r--   0        0        0     1319 2024-05-30 13:45:39.024783 visionkan-0.0.4/VisionKAN/.git/objects/0c/3fdd176183c8a66b347340e4d84ad918cbc18c
+-rw-r--r--   0        0        0     1317 2024-05-25 16:05:34.641678 visionkan-0.0.4/VisionKAN/.git/objects/12/9a6e0aad0a851e986186c74ddb3ce96adaf5ee
+-rw-r--r--   0        0        0     6856 2024-05-31 14:32:24.518636 visionkan-0.0.4/VisionKAN/.git/objects/13/b30851219f73fd58967c40ff74387ffb424188
+-rw-r--r--   0        0        0     1506 2024-05-30 13:45:39.011851 visionkan-0.0.4/VisionKAN/.git/objects/15/12f01aeb2737c67d44e5a2de3daab934bc00d4
+-rw-r--r--   0        0        0      494 2024-05-25 14:20:36.237613 visionkan-0.0.4/VisionKAN/.git/objects/15/882637c211157b37fd7eabb34894795520e0bb
+-rw-r--r--   0        0        0     1170 2024-05-31 13:33:51.648165 visionkan-0.0.4/VisionKAN/.git/objects/16/8c00f3102d915e4bc73d1034f91549ad22e428
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.002263 visionkan-0.0.4/VisionKAN/.git/objects/21/fbe556dd1106f6a79eb78fac39019b38d89519
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.022019 visionkan-0.0.4/VisionKAN/.git/objects/25/3f201824ad7beb456236e0b910d2c0a9d1df2d
+-rw-r--r--   0        0        0      677 2024-05-31 14:53:04.833593 visionkan-0.0.4/VisionKAN/.git/objects/27/9af88c958e602fe7e7836555be28ab6b2dcb20
+-rw-r--r--   0        0        0     1506 2024-05-30 13:45:39.013923 visionkan-0.0.4/VisionKAN/.git/objects/29/ff87b50e72193eec1f7a4f5385f30d66f53613
+-rw-r--r--   0        0        0     1508 2024-05-30 13:45:39.009225 visionkan-0.0.4/VisionKAN/.git/objects/2b/d3ddb40f4749eb5e1b1c3965cc8ab399c91f93
+-rw-r--r--   0        0        0      494 2024-05-31 13:34:21.562548 visionkan-0.0.4/VisionKAN/.git/objects/2c/dd22f3aa4c47e3545301d4da191b68fc94f1c5
+-rw-r--r--   0        0        0      521 2024-05-31 14:33:27.090702 visionkan-0.0.4/VisionKAN/.git/objects/35/c12e9342863df9c5d6a8ec1efb8b9cb9169b37
+-rw-r--r--   0        0        0      818 2024-05-31 14:49:00.672759 visionkan-0.0.4/VisionKAN/.git/objects/43/6f239ee660810f0025cd0baf2bd57e66fce109
+-rw-r--r--   0        0        0      493 2024-05-30 14:33:26.786303 visionkan-0.0.4/VisionKAN/.git/objects/43/d403b1cc332e3f220e936ef1b3b6fbf94448c3
+-rw-r--r--   0        0        0      183 2024-05-31 14:53:12.874375 visionkan-0.0.4/VisionKAN/.git/objects/44/70e85c1e0811b1fd6ef8ad32f01c35285a2d68
+-rw-r--r--   0        0        0      837 2024-05-30 13:45:38.998331 visionkan-0.0.4/VisionKAN/.git/objects/44/e907d19bcaf6fb23d971e191ac29d317eab980
+-rw-r--r--   0        0        0      836 2024-05-30 13:45:38.992896 visionkan-0.0.4/VisionKAN/.git/objects/46/752e8ceaeaca3e493ab2a35afb3d481dfd8a45
+-rw-r--r--   0        0        0      493 2024-05-25 14:20:36.240943 visionkan-0.0.4/VisionKAN/.git/objects/4a/1e4d2ff99d121790b8e3e21ddec07e0b064c29
+-rw-r--r--   0        0        0      841 2024-05-25 14:20:36.234901 visionkan-0.0.4/VisionKAN/.git/objects/4a/4455c1797f8ca10833017712f420b667f5e2c7
+-rw-r--r--   0        0        0      819 2024-05-30 13:45:38.995549 visionkan-0.0.4/VisionKAN/.git/objects/4e/0f0d2e944cb103da318db1efea21f0b965e2b1
+-rw-r--r--   0        0        0     1466 2024-05-30 13:45:39.020279 visionkan-0.0.4/VisionKAN/.git/objects/56/336fbf8d500db9a2c6cb3becb0953f568ac4e1
+-rw-r--r--   0        0        0      824 2024-05-30 13:45:38.991028 visionkan-0.0.4/VisionKAN/.git/objects/56/7434cb3ff4fef14ec5845ea9a9460c4cb08d9b
+-rw-r--r--   0        0        0     1038 2024-05-31 14:48:55.244146 visionkan-0.0.4/VisionKAN/.git/objects/5c/b18af65e33aa342b6cf265fdda19720883197d
+-rw-r--r--   0        0        0      843 2024-05-25 14:20:36.236438 visionkan-0.0.4/VisionKAN/.git/objects/5d/2cdd8e6f86eb49afc4b8cc6112dfc087e67b4b
+-rw-r--r--   0        0        0      121 2024-05-31 14:48:55.244374 visionkan-0.0.4/VisionKAN/.git/objects/65/0d1fd130531d23d807d0336f75f011ffd1af95
+-rw-r--r--   0        0        0      897 2024-05-31 16:17:30.631689 visionkan-0.0.4/VisionKAN/.git/objects/69/91a7f628ac78a0ea2a7cd7deca258f6ca303f7
+-rw-r--r--   0        0        0     1848 2024-05-31 14:04:43.843201 visionkan-0.0.4/VisionKAN/.git/objects/6a/00d1becfc1105d37b0bd8fe4ead459425484e3
+-rw-r--r--   0        0        0      184 2024-05-31 14:49:14.673971 visionkan-0.0.4/VisionKAN/.git/objects/6a/f10ebd18db1f3301de38d19f9689a7b2311036
+-rw-r--r--   0        0        0       61 2024-05-31 13:33:51.647179 visionkan-0.0.4/VisionKAN/.git/objects/6b/4b62ae4705d9c1f3bbbdd970f69b56552b7ad0
+-rw-r--r--   0        0        0      840 2024-05-30 13:45:38.991888 visionkan-0.0.4/VisionKAN/.git/objects/6d/4fee0c09fe53ef076b8ca569c76d8ef0e9c0be
+-rw-r--r--   0        0        0      630 2024-05-31 16:17:30.632415 visionkan-0.0.4/VisionKAN/.git/objects/70/b1eef9982cebe6f1bc10e1fd644b31c7fb40fb
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.019492 visionkan-0.0.4/VisionKAN/.git/objects/71/4760bd63cff5586b975798a51d9f5b9abd9c98
+-rw-r--r--   0        0        0      818 2024-05-30 13:45:38.996310 visionkan-0.0.4/VisionKAN/.git/objects/77/2f83ad9b280531ffe3575c3bf3a084dde9dda8
+-rw-r--r--   0        0        0      521 2024-05-31 14:32:40.853130 visionkan-0.0.4/VisionKAN/.git/objects/79/6b48f77c56e8b31fa26df0c09faa2f58a21933
+-rw-r--r--   0        0        0      275 2024-05-31 14:53:04.834456 visionkan-0.0.4/VisionKAN/.git/objects/7b/65ba50b57d47abdb10a72e10af24141c5f1e23
+-rw-r--r--   0        0        0      263 2024-05-31 13:38:09.217336 visionkan-0.0.4/VisionKAN/.git/objects/7f/8d64c1877aae28d07cc44e14e41754783b9d1f
+-rw-r--r--   0        0        0      913 2024-05-25 16:05:34.642373 visionkan-0.0.4/VisionKAN/.git/objects/84/32edbe772c608ef21c8ea9888b4b153572b1c4
+-rw-r--r--   0        0        0      494 2024-05-25 14:20:36.239279 visionkan-0.0.4/VisionKAN/.git/objects/84/ccf3adbe9ed1f4e754ec299aadd9d01122a306
+-rw-r--r--   0        0        0     2006 2024-05-31 16:17:30.633745 visionkan-0.0.4/VisionKAN/.git/objects/86/3baf687b25c96a0475896b31920698bfb547d3
+-rw-r--r--   0        0        0      819 2024-05-30 13:45:38.990222 visionkan-0.0.4/VisionKAN/.git/objects/86/638aea647100826572038a201b3aa540ba361d
+-rw-r--r--   0        0        0      494 2024-05-31 13:37:51.709443 visionkan-0.0.4/VisionKAN/.git/objects/86/799c8a3e5fd7b900f08c88e0cca639850fc294
+-rw-r--r--   0        0        0      821 2024-05-31 14:04:43.840635 visionkan-0.0.4/VisionKAN/.git/objects/88/3f6618e8a967e22cd911a293df9f580dedfc80
+-rw-r--r--   0        0        0     1865 2024-05-31 14:49:00.675912 visionkan-0.0.4/VisionKAN/.git/objects/89/df25510efa3d32d3a185632510e51e0b5ac587
+-rw-r--r--   0        0        0      839 2024-05-30 13:45:38.999243 visionkan-0.0.4/VisionKAN/.git/objects/8a/18123c11a366bf202025fbfcad890ba85f85db
+-rw-r--r--   0        0        0      838 2024-05-30 14:33:26.785333 visionkan-0.0.4/VisionKAN/.git/objects/8a/54f42e59da31cf4fab9e75821cd6dc38de66e1
+-rw-r--r--   0        0        0     1664 2024-05-30 14:33:26.787040 visionkan-0.0.4/VisionKAN/.git/objects/98/5a41303f0b376424104732aae1cf6c26f107b0
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.007970 visionkan-0.0.4/VisionKAN/.git/objects/a0/32cdc4f076cbbf159d16ce87dd1c004acb9cc6
+-rw-r--r--   0        0        0      840 2024-05-30 13:45:39.000137 visionkan-0.0.4/VisionKAN/.git/objects/a0/f9955482da7bbbc35d37396db4e7e5701e9c28
+-rw-r--r--   0        0        0      630 2024-05-31 14:53:12.871608 visionkan-0.0.4/VisionKAN/.git/objects/a9/7a8bfdb02e47eac5f95ffc887ff9137eb58e33
+-rw-r--r--   0        0        0     6819 2024-05-31 13:33:51.687559 visionkan-0.0.4/VisionKAN/.git/objects/b6/696a95d7f64217f0fece92139644ee203cf2b0
+-rw-r--r--   0        0        0      494 2024-05-31 14:04:43.841489 visionkan-0.0.4/VisionKAN/.git/objects/b7/4f0c2f72935f7521485b89031e8e95e2371820
+-rw-r--r--   0        0        0      188 2024-05-31 13:34:21.564914 visionkan-0.0.4/VisionKAN/.git/objects/bd/7fd2adf69a9075779ce023a53a26ffc20aebf4
+-rw-r--r--   0        0        0     1506 2024-05-31 13:33:51.673512 visionkan-0.0.4/VisionKAN/.git/objects/bf/bd0b862c1b0a15f144f53f7df02a252c37c01d
+-rw-r--r--   0        0        0      493 2024-05-25 16:05:34.586080 visionkan-0.0.4/VisionKAN/.git/objects/bf/e3c8a6391f11a33cba14538ac78722c4509966
+-rw-r--r--   0        0        0      837 2024-05-25 16:05:34.584618 visionkan-0.0.4/VisionKAN/.git/objects/c9/79bca54c422dc3a5f94ddbfcea861b354e049c
+-rw-r--r--   0        0        0      561 2024-05-31 14:49:14.671088 visionkan-0.0.4/VisionKAN/.git/objects/cc/3a210486203faf4a7d3fc808b58a427af0e996
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.012831 visionkan-0.0.4/VisionKAN/.git/objects/cc/7b9c064b952a571a49427d736064342fc5d24c
+-rw-r--r--   0        0        0      264 2024-05-31 14:33:30.522785 visionkan-0.0.4/VisionKAN/.git/objects/cd/67ec395c8a3d6d2b6af4d25c5c4dc74388de8e
+-rw-r--r--   0        0        0     1439 2024-05-30 13:45:39.018627 visionkan-0.0.4/VisionKAN/.git/objects/cd/85a76fe43e08cf4e7b9b363dc2542ff4f39da2
+-rw-r--r--   0        0        0     2006 2024-05-31 14:53:04.832605 visionkan-0.0.4/VisionKAN/.git/objects/cd/8ac765c6d6e22fbeff50a342231d49454816fb
+-rw-r--r--   0        0        0     2609 2024-05-31 13:33:51.698886 visionkan-0.0.4/VisionKAN/.git/objects/d2/c20123b2340bec1c7f22363a5c867d66fa5c87
+-rw-r--r--   0        0        0     2667 2024-05-31 14:32:24.568609 visionkan-0.0.4/VisionKAN/.git/objects/d3/d265b925f92f1e17fba0896d3e041ea5d32aa4
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.017651 visionkan-0.0.4/VisionKAN/.git/objects/dc/865eaf4ea0b28b422621902e9a5a0a2df5177a
+-rw-r--r--   0        0        0     1462 2024-05-30 13:45:39.022977 visionkan-0.0.4/VisionKAN/.git/objects/de/c987774b10e51d1574a82830ea20fa66e1ab9b
+-rw-r--r--   0        0        0      521 2024-05-31 14:49:00.673749 visionkan-0.0.4/VisionKAN/.git/objects/e1/dd05a85418b7679ed648eef24b113ceace9d4d
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.015287 visionkan-0.0.4/VisionKAN/.git/objects/e9/d6a23a2cc05561da18f235fe79d1f58c9c81bb
+-rw-r--r--   0        0        0      841 2024-05-25 14:20:36.235936 visionkan-0.0.4/VisionKAN/.git/objects/ea/b5de8755717ee2c3eca3382fedb489252551cc
+-rw-r--r--   0        0        0     1193 2024-05-25 14:20:36.242033 visionkan-0.0.4/VisionKAN/.git/objects/eb/69480d3d8e32c0d18cfe47e6f3501c0a04097c
+-rw-r--r--   0        0        0     1197 2024-05-25 14:20:36.240180 visionkan-0.0.4/VisionKAN/.git/objects/ec/5afec8cf55319913cf0dffef27ed2e4513a89f
+-rw-r--r--   0        0        0      493 2024-05-30 13:45:39.023865 visionkan-0.0.4/VisionKAN/.git/objects/f4/d8d97e8689fe0ca5b1218098d7df8fdc5a66a1
+-rw-r--r--   0        0        0     1670 2024-05-30 13:45:39.006098 visionkan-0.0.4/VisionKAN/.git/objects/f7/77f1ace2c84ba7411c7b9b36f8016262bdf565
+-rw-r--r--   0        0        0     1662 2024-05-30 13:45:39.004604 visionkan-0.0.4/VisionKAN/.git/objects/f7/eebc418a1d2e4790a20aa8bd06a71612065ce1
+-rw-r--r--   0        0        0      929 2024-05-30 13:45:38.994918 visionkan-0.0.4/VisionKAN/.git/objects/fa/ef8af61c4f860b09d810bf73d34b6f1505f88f
+-rw-r--r--   0        0        0      188 2024-05-31 14:32:40.856549 visionkan-0.0.4/VisionKAN/.git/objects/fc/0f3b6701e2cf4679070f83418f6832c20dd94a
+-rw-r--r--   0        0        0     5132 2024-05-24 15:35:10.437127 visionkan-0.0.4/VisionKAN/.git/objects/pack/pack-b923ccab73ed5f6d720c7d92156d1d6412751d26.idx
+-rw-r--r--   0        0        0    67923 2024-05-24 15:35:10.436764 visionkan-0.0.4/VisionKAN/.git/objects/pack/pack-b923ccab73ed5f6d720c7d92156d1d6412751d26.pack
+-rw-r--r--   0        0        0      112 2024-05-24 15:35:10.444369 visionkan-0.0.4/VisionKAN/.git/packed-refs
+-rw-r--r--   0        0        0       41 2024-05-31 13:34:21.566187 visionkan-0.0.4/VisionKAN/.git/refs/heads/main
+-rw-r--r--   0        0        0       41 2024-05-31 14:53:12.875969 visionkan-0.0.4/VisionKAN/.git/refs/heads/patch-1
+-rw-r--r--   0        0        0       30 2024-05-24 15:35:10.446019 visionkan-0.0.4/VisionKAN/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0       41 2024-05-31 16:17:30.665858 visionkan-0.0.4/VisionKAN/.git/refs/remotes/origin/main
+-rw-r--r--   0        0        0       41 2024-05-31 14:53:25.744676 visionkan-0.0.4/VisionKAN/.git/refs/remotes/origin/patch-1
+-rw-r--r--   0        0        0       49 2024-05-31 13:33:36.981809 visionkan-0.0.4/VisionKAN/.gitignore
+-rw-r--r--   0        0        0     2267 2024-05-24 15:35:10.449051 visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/README-checkpoint.md
+-rw-r--r--   0        0        0     3456 2024-05-24 15:51:59.818683 visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/augment-checkpoint.py
+-rw-r--r--   0        0        0     4441 2024-05-25 01:13:48.567915 visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/datasets-checkpoint.py
+-rw-r--r--   0        0        0    23357 2024-05-25 17:06:25.070376 visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/main-checkpoint.py
+-rw-r--r--   0        0        0    11849 2024-05-25 17:13:58.729211 visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/models_kan-checkpoint.py
+-rw-r--r--   0        0        0       45 2024-05-24 15:35:10.451860 visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/requirements-checkpoint.txt
+-rw-r--r--   0        0        0     1102 2024-05-31 14:52:54.053362 visionkan-0.0.4/VisionKAN/LICENSE
+-rw-r--r--   0        0        0     4431 2024-05-31 17:14:54.486745 visionkan-0.0.4/VisionKAN/README.md
+-rw-r--r--   0        0        0      390 2024-05-31 18:12:52.441846 visionkan-0.0.4/VisionKAN/__init__.py
+-rw-r--r--   0        0        0     3456 2024-05-24 15:51:59.818683 visionkan-0.0.4/VisionKAN/augment.py
+-rw-r--r--   0        0        0     4441 2024-05-25 01:13:48.567915 visionkan-0.0.4/VisionKAN/datasets.py
+-rw-r--r--   0        0        0    10325 2024-05-24 15:35:10.449538 visionkan-0.0.4/VisionKAN/ekan.py
+-rw-r--r--   0        0        0     4243 2024-05-31 18:09:53.943416 visionkan-0.0.4/VisionKAN/engine.py
+-rw-r--r--   0        0        0     5304 2024-05-24 15:35:10.449878 visionkan-0.0.4/VisionKAN/fasterkan.py
+-rw-r--r--   0        0        0      227 2024-05-24 15:35:10.449989 visionkan-0.0.4/VisionKAN/hubconf.py
+-rw-r--r--   0        0        0    23183 2024-05-31 18:10:13.027200 visionkan-0.0.4/VisionKAN/kit.py
+-rw-r--r--   0        0        0     3388 2024-05-24 15:35:10.451223 visionkan-0.0.4/VisionKAN/losses.py
+-rw-r--r--   0        0        0    23456 2024-05-31 18:11:02.962457 visionkan-0.0.4/VisionKAN/main.py
+-rw-r--r--   0        0        0     2367 2024-05-31 18:10:46.143701 visionkan-0.0.4/VisionKAN/minimal_example.py
+-rw-r--r--   0        0        0    13424 2024-05-31 17:55:28.760189 visionkan-0.0.4/VisionKAN/models_kan.py
+-rw-r--r--   0        0        0       45 2024-05-24 15:35:10.451860 visionkan-0.0.4/VisionKAN/requirements.txt
+-rw-r--r--   0        0        0     2584 2024-05-24 15:35:10.452108 visionkan-0.0.4/VisionKAN/samplers.py
+-rw-r--r--   0        0        0     7086 2024-05-31 18:11:25.748752 visionkan-0.0.4/VisionKAN/utils.py
+-rw-r--r--   0        0        0      665 2024-05-31 18:14:24.158760 visionkan-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 visionkan-0.0.4/PKG-INFO
```

### Comparing `visionkan-0.0.3/LICENSE` & `visionkan-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/README.md` & `visionkan-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/hooks/commit-msg.sample` & `visionkan-0.0.4/VisionKAN/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/hooks/fsmonitor-watchman.sample` & `visionkan-0.0.4/VisionKAN/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/hooks/pre-commit.sample` & `visionkan-0.0.4/VisionKAN/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/hooks/pre-push.sample` & `visionkan-0.0.4/VisionKAN/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/hooks/pre-rebase.sample` & `visionkan-0.0.4/VisionKAN/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/hooks/pre-receive.sample` & `visionkan-0.0.4/VisionKAN/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/hooks/prepare-commit-msg.sample` & `visionkan-0.0.4/VisionKAN/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/hooks/push-to-checkout.sample` & `visionkan-0.0.4/VisionKAN/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/hooks/update.sample` & `visionkan-0.0.4/VisionKAN/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/index` & `visionkan-0.0.4/VisionKAN/.git/index`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/logs/HEAD` & `visionkan-0.0.4/VisionKAN/.git/logs/HEAD`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/logs/refs/heads/patch-1` & `visionkan-0.0.4/VisionKAN/.git/logs/refs/heads/patch-1`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/logs/refs/remotes/origin/main` & `visionkan-0.0.4/VisionKAN/.git/logs/refs/remotes/origin/main`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/logs/refs/remotes/origin/patch-1` & `visionkan-0.0.4/VisionKAN/.git/logs/refs/remotes/origin/patch-1`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/06/68b38d953d4aaff834ef30fcbb54ace8b44db8` & `visionkan-0.0.4/VisionKAN/.git/objects/06/68b38d953d4aaff834ef30fcbb54ace8b44db8`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/06/74abe9ee0925ae39a471b2bcda4ef468da405a` & `visionkan-0.0.4/VisionKAN/.git/objects/06/74abe9ee0925ae39a471b2bcda4ef468da405a`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/09/cabeca13a688a93d1d3268c300759fa2c66325` & `visionkan-0.0.4/VisionKAN/.git/objects/09/cabeca13a688a93d1d3268c300759fa2c66325`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/0c/3fdd176183c8a66b347340e4d84ad918cbc18c` & `visionkan-0.0.4/VisionKAN/.git/objects/0c/3fdd176183c8a66b347340e4d84ad918cbc18c`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/12/9a6e0aad0a851e986186c74ddb3ce96adaf5ee` & `visionkan-0.0.4/VisionKAN/.git/objects/12/9a6e0aad0a851e986186c74ddb3ce96adaf5ee`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/13/b30851219f73fd58967c40ff74387ffb424188` & `visionkan-0.0.4/VisionKAN/.git/objects/13/b30851219f73fd58967c40ff74387ffb424188`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/15/12f01aeb2737c67d44e5a2de3daab934bc00d4` & `visionkan-0.0.4/VisionKAN/.git/objects/15/12f01aeb2737c67d44e5a2de3daab934bc00d4`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/16/8c00f3102d915e4bc73d1034f91549ad22e428` & `visionkan-0.0.4/VisionKAN/.git/objects/16/8c00f3102d915e4bc73d1034f91549ad22e428`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/27/9af88c958e602fe7e7836555be28ab6b2dcb20` & `visionkan-0.0.4/VisionKAN/.git/objects/27/9af88c958e602fe7e7836555be28ab6b2dcb20`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/29/ff87b50e72193eec1f7a4f5385f30d66f53613` & `visionkan-0.0.4/VisionKAN/.git/objects/29/ff87b50e72193eec1f7a4f5385f30d66f53613`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/2b/d3ddb40f4749eb5e1b1c3965cc8ab399c91f93` & `visionkan-0.0.4/VisionKAN/.git/objects/2b/d3ddb40f4749eb5e1b1c3965cc8ab399c91f93`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/35/c12e9342863df9c5d6a8ec1efb8b9cb9169b37` & `visionkan-0.0.4/VisionKAN/.git/objects/35/c12e9342863df9c5d6a8ec1efb8b9cb9169b37`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/43/6f239ee660810f0025cd0baf2bd57e66fce109` & `visionkan-0.0.4/VisionKAN/.git/objects/43/6f239ee660810f0025cd0baf2bd57e66fce109`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/44/e907d19bcaf6fb23d971e191ac29d317eab980` & `visionkan-0.0.4/VisionKAN/.git/objects/44/e907d19bcaf6fb23d971e191ac29d317eab980`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/46/752e8ceaeaca3e493ab2a35afb3d481dfd8a45` & `visionkan-0.0.4/VisionKAN/.git/objects/46/752e8ceaeaca3e493ab2a35afb3d481dfd8a45`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/4a/4455c1797f8ca10833017712f420b667f5e2c7` & `visionkan-0.0.4/VisionKAN/.git/objects/4a/4455c1797f8ca10833017712f420b667f5e2c7`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/4e/0f0d2e944cb103da318db1efea21f0b965e2b1` & `visionkan-0.0.4/VisionKAN/.git/objects/4e/0f0d2e944cb103da318db1efea21f0b965e2b1`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/56/336fbf8d500db9a2c6cb3becb0953f568ac4e1` & `visionkan-0.0.4/VisionKAN/.git/objects/56/336fbf8d500db9a2c6cb3becb0953f568ac4e1`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/56/7434cb3ff4fef14ec5845ea9a9460c4cb08d9b` & `visionkan-0.0.4/VisionKAN/.git/objects/56/7434cb3ff4fef14ec5845ea9a9460c4cb08d9b`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/5c/b18af65e33aa342b6cf265fdda19720883197d` & `visionkan-0.0.4/VisionKAN/.git/objects/5c/b18af65e33aa342b6cf265fdda19720883197d`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/5d/2cdd8e6f86eb49afc4b8cc6112dfc087e67b4b` & `visionkan-0.0.4/VisionKAN/.git/objects/5d/2cdd8e6f86eb49afc4b8cc6112dfc087e67b4b`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/69/91a7f628ac78a0ea2a7cd7deca258f6ca303f7` & `visionkan-0.0.4/VisionKAN/.git/objects/69/91a7f628ac78a0ea2a7cd7deca258f6ca303f7`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/6a/00d1becfc1105d37b0bd8fe4ead459425484e3` & `visionkan-0.0.4/VisionKAN/.git/objects/6a/00d1becfc1105d37b0bd8fe4ead459425484e3`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/6d/4fee0c09fe53ef076b8ca569c76d8ef0e9c0be` & `visionkan-0.0.4/VisionKAN/.git/objects/6d/4fee0c09fe53ef076b8ca569c76d8ef0e9c0be`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/70/b1eef9982cebe6f1bc10e1fd644b31c7fb40fb` & `visionkan-0.0.4/VisionKAN/.git/objects/70/b1eef9982cebe6f1bc10e1fd644b31c7fb40fb`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/77/2f83ad9b280531ffe3575c3bf3a084dde9dda8` & `visionkan-0.0.4/VisionKAN/.git/objects/77/2f83ad9b280531ffe3575c3bf3a084dde9dda8`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/79/6b48f77c56e8b31fa26df0c09faa2f58a21933` & `visionkan-0.0.4/VisionKAN/.git/objects/79/6b48f77c56e8b31fa26df0c09faa2f58a21933`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/84/32edbe772c608ef21c8ea9888b4b153572b1c4` & `visionkan-0.0.4/VisionKAN/.git/objects/84/32edbe772c608ef21c8ea9888b4b153572b1c4`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/86/3baf687b25c96a0475896b31920698bfb547d3` & `visionkan-0.0.4/VisionKAN/.git/objects/86/3baf687b25c96a0475896b31920698bfb547d3`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/86/638aea647100826572038a201b3aa540ba361d` & `visionkan-0.0.4/VisionKAN/.git/objects/86/638aea647100826572038a201b3aa540ba361d`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/88/3f6618e8a967e22cd911a293df9f580dedfc80` & `visionkan-0.0.4/VisionKAN/.git/objects/88/3f6618e8a967e22cd911a293df9f580dedfc80`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/89/df25510efa3d32d3a185632510e51e0b5ac587` & `visionkan-0.0.4/VisionKAN/.git/objects/89/df25510efa3d32d3a185632510e51e0b5ac587`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/8a/18123c11a366bf202025fbfcad890ba85f85db` & `visionkan-0.0.4/VisionKAN/.git/objects/8a/18123c11a366bf202025fbfcad890ba85f85db`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/8a/54f42e59da31cf4fab9e75821cd6dc38de66e1` & `visionkan-0.0.4/VisionKAN/.git/objects/8a/54f42e59da31cf4fab9e75821cd6dc38de66e1`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/98/5a41303f0b376424104732aae1cf6c26f107b0` & `visionkan-0.0.4/VisionKAN/.git/objects/98/5a41303f0b376424104732aae1cf6c26f107b0`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/a0/f9955482da7bbbc35d37396db4e7e5701e9c28` & `visionkan-0.0.4/VisionKAN/.git/objects/a0/f9955482da7bbbc35d37396db4e7e5701e9c28`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/a9/7a8bfdb02e47eac5f95ffc887ff9137eb58e33` & `visionkan-0.0.4/VisionKAN/.git/objects/a9/7a8bfdb02e47eac5f95ffc887ff9137eb58e33`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/b6/696a95d7f64217f0fece92139644ee203cf2b0` & `visionkan-0.0.4/VisionKAN/.git/objects/b6/696a95d7f64217f0fece92139644ee203cf2b0`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/bf/bd0b862c1b0a15f144f53f7df02a252c37c01d` & `visionkan-0.0.4/VisionKAN/.git/objects/bf/bd0b862c1b0a15f144f53f7df02a252c37c01d`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/c9/79bca54c422dc3a5f94ddbfcea861b354e049c` & `visionkan-0.0.4/VisionKAN/.git/objects/c9/79bca54c422dc3a5f94ddbfcea861b354e049c`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/cc/3a210486203faf4a7d3fc808b58a427af0e996` & `visionkan-0.0.4/VisionKAN/.git/objects/cc/3a210486203faf4a7d3fc808b58a427af0e996`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/cd/85a76fe43e08cf4e7b9b363dc2542ff4f39da2` & `visionkan-0.0.4/VisionKAN/.git/objects/cd/85a76fe43e08cf4e7b9b363dc2542ff4f39da2`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/cd/8ac765c6d6e22fbeff50a342231d49454816fb` & `visionkan-0.0.4/VisionKAN/.git/objects/cd/8ac765c6d6e22fbeff50a342231d49454816fb`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/d2/c20123b2340bec1c7f22363a5c867d66fa5c87` & `visionkan-0.0.4/VisionKAN/.git/objects/d2/c20123b2340bec1c7f22363a5c867d66fa5c87`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/d3/d265b925f92f1e17fba0896d3e041ea5d32aa4` & `visionkan-0.0.4/VisionKAN/.git/objects/d3/d265b925f92f1e17fba0896d3e041ea5d32aa4`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/de/c987774b10e51d1574a82830ea20fa66e1ab9b` & `visionkan-0.0.4/VisionKAN/.git/objects/de/c987774b10e51d1574a82830ea20fa66e1ab9b`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/e1/dd05a85418b7679ed648eef24b113ceace9d4d` & `visionkan-0.0.4/VisionKAN/.git/objects/e1/dd05a85418b7679ed648eef24b113ceace9d4d`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/ea/b5de8755717ee2c3eca3382fedb489252551cc` & `visionkan-0.0.4/VisionKAN/.git/objects/ea/b5de8755717ee2c3eca3382fedb489252551cc`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/eb/69480d3d8e32c0d18cfe47e6f3501c0a04097c` & `visionkan-0.0.4/VisionKAN/.git/objects/eb/69480d3d8e32c0d18cfe47e6f3501c0a04097c`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/ec/5afec8cf55319913cf0dffef27ed2e4513a89f` & `visionkan-0.0.4/VisionKAN/.git/objects/ec/5afec8cf55319913cf0dffef27ed2e4513a89f`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/f7/77f1ace2c84ba7411c7b9b36f8016262bdf565` & `visionkan-0.0.4/VisionKAN/.git/objects/f7/77f1ace2c84ba7411c7b9b36f8016262bdf565`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/f7/eebc418a1d2e4790a20aa8bd06a71612065ce1` & `visionkan-0.0.4/VisionKAN/.git/objects/f7/eebc418a1d2e4790a20aa8bd06a71612065ce1`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/fa/ef8af61c4f860b09d810bf73d34b6f1505f88f` & `visionkan-0.0.4/VisionKAN/.git/objects/fa/ef8af61c4f860b09d810bf73d34b6f1505f88f`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/pack/pack-b923ccab73ed5f6d720c7d92156d1d6412751d26.idx` & `visionkan-0.0.4/VisionKAN/.git/objects/pack/pack-b923ccab73ed5f6d720c7d92156d1d6412751d26.idx`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.git/objects/pack/pack-b923ccab73ed5f6d720c7d92156d1d6412751d26.pack` & `visionkan-0.0.4/VisionKAN/.git/objects/pack/pack-b923ccab73ed5f6d720c7d92156d1d6412751d26.pack`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/README-checkpoint.md` & `visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/README-checkpoint.md`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/augment-checkpoint.py` & `visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/augment-checkpoint.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/datasets-checkpoint.py` & `visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/datasets-checkpoint.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/main-checkpoint.py` & `visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/main-checkpoint.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/.ipynb_checkpoints/models_kan-checkpoint.py` & `visionkan-0.0.4/VisionKAN/.ipynb_checkpoints/models_kan-checkpoint.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/LICENSE` & `visionkan-0.0.4/VisionKAN/LICENSE`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/README.md` & `visionkan-0.0.4/VisionKAN/README.md`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/augment.py` & `visionkan-0.0.4/VisionKAN/augment.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/datasets.py` & `visionkan-0.0.4/VisionKAN/datasets.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/ekan.py` & `visionkan-0.0.4/VisionKAN/ekan.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/engine.py` & `visionkan-0.0.4/VisionKAN/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from typing import Iterable, Optional
 
 import torch
 
 from timm.data import Mixup
 from timm.utils import accuracy, ModelEma
 
-from losses import DistillationLoss
-import utils
+from .losses import DistillationLoss
+import .utils
 
 
 def train_one_epoch(model: torch.nn.Module, criterion: DistillationLoss,
                     data_loader: Iterable, optimizer: torch.optim.Optimizer,
                     device: torch.device, epoch: int, loss_scaler, max_norm: float = 0,
                     model_ema: Optional[ModelEma] = None, mixup_fn: Optional[Mixup] = None,
                     set_training_mode=True, args = None):
```

### Comparing `visionkan-0.0.3/Vision-KAN/fasterkan.py` & `visionkan-0.0.4/VisionKAN/fasterkan.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/kit.py` & `visionkan-0.0.4/VisionKAN/kit.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # All rights reserved.
 
 import torch
 import torch.nn as nn
 from functools import partial
 
 from timm.models.vision_transformer import Mlp, PatchEmbed, _cfg
-from ekan import KAN
+from .ekan import KAN
 
 from timm.models.layers import DropPath, to_2tuple, trunc_normal_
 from timm.models.registry import register_model
 __all__ = [
     'deit_tiny_patch16_LS'
 ]
```

### Comparing `visionkan-0.0.3/Vision-KAN/losses.py` & `visionkan-0.0.4/VisionKAN/losses.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/main.py` & `visionkan-0.0.4/VisionKAN/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 # from timm.models import create_model
 from models_kan import create_model
 from timm.loss import LabelSmoothingCrossEntropy, SoftTargetCrossEntropy
 from timm.scheduler import create_scheduler
 from timm.optim import create_optimizer
 from timm.utils import NativeScaler, get_state_dict, ModelEma
 
-from datasets import build_dataset
-from engine import train_one_epoch, evaluate
-from losses import DistillationLoss
-from samplers import RASampler
-from augment import new_data_aug_generator
+from .datasets import build_dataset
+from .engine import train_one_epoch, evaluate
+from .losses import DistillationLoss
+from .samplers import RASampler
+from .augment import new_data_aug_generator
 
 # import models
 # import models_v2
 import kit
 
-import utils
+import .utils
 
 
 def get_args_parser():
     parser = argparse.ArgumentParser('DeiT training and evaluation script', add_help=False)
     parser.add_argument('--batch-size', default=144, type=int)
     parser.add_argument('--epochs', default=300, type=int)
     parser.add_argument('--bce-loss', action='store_true')
```

### Comparing `visionkan-0.0.3/Vision-KAN/minimal_example.py` & `visionkan-0.0.4/VisionKAN/minimal_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from models_kan import create_model
+from .models_kan import create_model
 import torch.optim as optim
 import torch
 import torchvision
 import torchvision.transforms as transforms
 import torch.nn as nn
-from engine import train_one_epoch, evaluate
+from .engine import train_one_epoch, evaluate
 
 KAN_model = create_model(
     model_name='deit_tiny_patch16_224_KAN',
     pretrained=False,
     hdim_kan=192,
     num_classes=10,
     drop_rate=0.0,
```

### Comparing `visionkan-0.0.3/Vision-KAN/models_kan.py` & `visionkan-0.0.4/VisionKAN/models_kan.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/samplers.py` & `visionkan-0.0.4/VisionKAN/samplers.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/Vision-KAN/utils.py` & `visionkan-0.0.4/VisionKAN/utils.py`

 * *Files identical despite different names*

### Comparing `visionkan-0.0.3/pyproject.toml` & `visionkan-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "VisionKAN"
-version = "0.0.3"
+version = "0.0.4"
 description = "Vision Transformers implemented using KAN layers"
 repository = "https://github.com/chenziwenhaoshuai/Vision-KAN"
 readme = ["README.md"]
 authors = [
     "Ziwen Chen <chenziwen@dlou.edu.cn>", 
     "Saaketh Koundinya <three2saki@gmail.com>"
 ]
 
 license = "MIT"
 
 packages = [
-    { include = "Vision-KAN" }
+    { include = "VisionKAN" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 torch = ">=1.13.1"
 torchvision = ">=0.8.1"
 timm = ">=0.3.2"
```

### Comparing `visionkan-0.0.3/PKG-INFO` & `visionkan-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionKAN
-Version: 0.0.3
+Version: 0.0.4
 Summary: Vision Transformers implemented using KAN layers
 Home-page: https://github.com/chenziwenhaoshuai/Vision-KAN
 License: MIT
 Author: Ziwen Chen
 Author-email: chenziwen@dlou.edu.cn
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

