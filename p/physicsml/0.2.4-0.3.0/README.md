# Comparing `tmp/physicsml-0.2.4.tar.gz` & `tmp/physicsml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicsml-0.2.4.tar", last modified: Thu Apr 25 13:13:24 2024, max compression
+gzip compressed data, was "physicsml-0.3.0.tar", last modified: Fri Apr 26 08:47:02 2024, max compression
```

## Comparing `physicsml-0.2.4.tar` & `physicsml-0.3.0.tar`

### file list

```diff
@@ -1,456 +1,456 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.958828 physicsml-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-25 13:13:12.000000 physicsml-0.2.4/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.874827 physicsml-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/dev-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/docs-build-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/latest-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/main-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/pinned-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/publish-package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/quality-typing-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/release-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-25 13:13:12.000000 physicsml-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-25 13:13:12.000000 physicsml-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-25 13:13:12.000000 physicsml-0.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 13:13:12.000000 physicsml-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-25 13:13:24.958828 physicsml-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-25 13:13:12.000000 physicsml-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo-01.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.878827 physicsml-0.2.4/docs/source/pages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/docs/source/pages/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/datasets/qm_datasets.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/features/
--rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/features/gdb9_trunc.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/features/how_to_add_reps.md
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/features/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/allegro.md
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/ani.md
--rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/egnn.md
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/how_to_add_models.md
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/mace.md
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/nequip.md
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/tensor_net.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/philosophy/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/philosophy/molflux.md
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/philosophy/philosophy.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/plugins/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/plugins/ase.md
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/plugins/openmm.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/structure/
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/lightning_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/molflux_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/physicsml_structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/torch_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/transfer_learning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.898828 physicsml-0.2.4/docs/source/pages/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/ani1x_energy_forces_training.md
--rw-r--r--   0 runner    (1001) docker     (127)  1610932 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/ani1x_truncated.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/gdb9_training.md
--rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/gdb9_trunc.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/gdb9_uncertainty.md
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/transfer_learning.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 13:13:12.000000 physicsml-0.2.4/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-04-25 13:13:12.000000 physicsml-0.2.4/init_conda_venv.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-25 13:13:12.000000 physicsml-0.2.4/init_python_venv.sh
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-25 13:13:12.000000 physicsml-0.2.4/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.878827 physicsml-0.2.4/pinned-versions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/pinned-versions/3.10/
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/pinned-versions/3.11/
--rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/pinned-versions/3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/pinned-versions/3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.rdkit.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-25 13:13:12.000000 physicsml-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:13:24.958828 physicsml-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.878827 physicsml-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/src/physicsml/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/backends/backend_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/backends/openeye_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/backends/rdkit_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/featurisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/atom_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/bond_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/physicsml_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/graph_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.910828 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.910828 physicsml-0.2.4/src/physicsml/lightning/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/construct_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/loss_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/masked_mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/multitask_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/stock_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/weighted_mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/model_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/pre_batching_in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/pre_batching_on_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.910828 physicsml-0.2.4/src/physicsml/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.910828 physicsml-0.2.4/src/physicsml/models/allegro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/allegro_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.914828 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.914828 physicsml-0.2.4/src/physicsml/models/allegro/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24182 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/allegro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/cutoffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/fc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/spmm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.914828 physicsml-0.2.4/src/physicsml/models/allegro/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/supervised/allegro_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/supervised/allegro_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/supervised/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.914828 physicsml-0.2.4/src/physicsml/models/ani/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ani_1_2_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ani_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ani_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ani_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/ani/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ensemble/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ensemble/ensemble_ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ensemble/ensemble_ani_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/ani/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/mean_var/mean_var_ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/mean_var/mean_var_ani_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/ani/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27070 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/modules/aev.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/ani/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/supervised/ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/supervised/ani_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/supervised/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/egnn/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/egnn_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/egnn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/egnn/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/egnn/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/supervised/egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/supervised/egnn_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/mace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/mace/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mace_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/mace/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mean_var/mean_var_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mean_var/mean_var_mace_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/mace/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/cg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/irreps_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/symmetric_contraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/mace/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/mace/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/supervised/mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/supervised/mace_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/nequip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/nequip/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/nequip/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/convnet_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/interaction_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/scale_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/nequip_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/nequip/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/nequip/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/supervised/nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/supervised/nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/tensor_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/tensor_net_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/tensor_net_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/plugins/ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/ase_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/ase_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/plugins/openmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/physicsml_potential.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/src/physicsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16518 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.938828 physicsml-0.2.4/tests/ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/ase/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/ase/test_ase_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/ase/test_ase_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.938828 physicsml-0.2.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/alanine-dipeptide-truncated.pdb
--rw-r--r--   0 runner    (1001) docker     (127)   698696 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/ani1x.h5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.938828 physicsml-0.2.4/tests/data/ani_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/ani_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.938828 physicsml-0.2.4/tests/data/ani_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)  1320280 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/ani_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/egnn_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/egnn_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/egnn_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)    52081 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/egnn_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/gdb9.csv
--rw-r--r--   0 runner    (1001) docker     (127)    98022 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/gdb9.sdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/mace_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/mace_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/mace_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)   117170 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/mace_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/nequip_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/nequip_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/nequip_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/nequip_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/openeye/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/openeye/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/openeye/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/data/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/data/test_graph_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/core/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/featurisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/featurisation/test_physicsml_featurisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/integration/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/prism/test_egnn_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/integration/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/integration/training/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/training/egnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/training/egnn/test_egnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    16422 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_nnp_potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/rdkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/rdkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/rdkit/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/data/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/data/test_graph_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/rdkit/core/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/featurisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/featurisation/test_physicsml_featurisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_allegro_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_ani_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_egnn_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_mace_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_nequip_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/training/allegro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allergo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/training/ani/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_mean_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/tests/rdkit/integration/training/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_adapter_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_ssf_egnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/tests/rdkit/integration/training/mace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_adapter_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_ssf_mace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/tests/rdkit/integration/training/nequip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_adapter_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_ssf_nequip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.808412 physicsml-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-26 08:46:54.000000 physicsml-0.3.0/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.720412 physicsml-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.736412 physicsml-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-26 08:46:54.000000 physicsml-0.3.0/.github/workflows/dev-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-26 08:46:54.000000 physicsml-0.3.0/.github/workflows/docs-build-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-26 08:46:54.000000 physicsml-0.3.0/.github/workflows/latest-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-26 08:46:54.000000 physicsml-0.3.0/.github/workflows/main-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-26 08:46:54.000000 physicsml-0.3.0/.github/workflows/pinned-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 08:46:54.000000 physicsml-0.3.0/.github/workflows/publish-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 08:46:54.000000 physicsml-0.3.0/.github/workflows/quality-typing-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 08:46:54.000000 physicsml-0.3.0/.github/workflows/release-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-26 08:46:54.000000 physicsml-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-26 08:46:54.000000 physicsml-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-26 08:46:54.000000 physicsml-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 08:46:54.000000 physicsml-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-26 08:47:02.808412 physicsml-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-26 08:46:54.000000 physicsml-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.736412 physicsml-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.736412 physicsml-0.3.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.736412 physicsml-0.3.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/_static/PhysicsML_Logo-01.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.724412 physicsml-0.3.0/docs/source/pages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.736412 physicsml-0.3.0/docs/source/pages/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/datasets/qm_datasets.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.740412 physicsml-0.3.0/docs/source/pages/features/
+-rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/features/gdb9_trunc.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/features/how_to_add_reps.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/features/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.740412 physicsml-0.3.0/docs/source/pages/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/models/allegro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/models/ani.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/models/egnn.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/models/how_to_add_models.md
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/models/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/models/mace.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/models/nequip.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/models/tensor_net.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.740412 physicsml-0.3.0/docs/source/pages/philosophy/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/philosophy/molflux.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/philosophy/philosophy.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.740412 physicsml-0.3.0/docs/source/pages/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/plugins/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/plugins/ase.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/plugins/openmm.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.740412 physicsml-0.3.0/docs/source/pages/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/structure/lightning_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/structure/molflux_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/structure/physicsml_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/structure/torch_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/structure/transfer_learning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.744412 physicsml-0.3.0/docs/source/pages/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/tutorials/ani1x_energy_forces_training.md
+-rw-r--r--   0 runner    (1001) docker     (127)  1610932 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/tutorials/ani1x_truncated.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/tutorials/gdb9_training.md
+-rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/tutorials/gdb9_trunc.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/tutorials/gdb9_uncertainty.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-04-26 08:46:54.000000 physicsml-0.3.0/docs/source/pages/tutorials/transfer_learning.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-26 08:46:54.000000 physicsml-0.3.0/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-04-26 08:46:54.000000 physicsml-0.3.0/init_conda_venv.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-26 08:46:54.000000 physicsml-0.3.0/init_python_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-26 08:46:54.000000 physicsml-0.3.0/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.724412 physicsml-0.3.0/pinned-versions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.748412 physicsml-0.3.0/pinned-versions/3.10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.10/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.10/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.10/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.10/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.10/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.748412 physicsml-0.3.0/pinned-versions/3.11/
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.11/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.11/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.11/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.11/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.11/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.748412 physicsml-0.3.0/pinned-versions/3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.8/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.8/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.8/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.8/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.8/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.748412 physicsml-0.3.0/pinned-versions/3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.9/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.9/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.9/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.9/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-04-26 08:46:54.000000 physicsml-0.3.0/pinned-versions/3.9/lockfile.rdkit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-26 08:46:54.000000 physicsml-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:47:02.808412 physicsml-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.724412 physicsml-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.752412 physicsml-0.3.0/src/physicsml/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.752412 physicsml-0.3.0/src/physicsml/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/backends/backend_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/backends/openeye_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/backends/rdkit_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.752412 physicsml-0.3.0/src/physicsml/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/featurisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.752412 physicsml-0.3.0/src/physicsml/featurisation/physicsml_features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/featurisation/physicsml_features/atom_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/featurisation/physicsml_features/bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/featurisation/physicsml_features/physicsml_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.752412 physicsml-0.3.0/src/physicsml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.756412 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14207 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/graph_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.756412 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.756412 physicsml-0.3.0/src/physicsml/lightning/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/losses/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/losses/construct_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/losses/loss_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/losses/masked_mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/losses/multitask_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/losses/stock_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/losses/weighted_mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/model_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/pre_batching_in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/lightning/pre_batching_on_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.756412 physicsml-0.3.0/src/physicsml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.760412 physicsml-0.3.0/src/physicsml/models/allegro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/allegro_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.760412 physicsml-0.3.0/src/physicsml/models/allegro/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.760412 physicsml-0.3.0/src/physicsml/models/allegro/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24182 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/allegro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/cutoffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/modules/spmm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.760412 physicsml-0.3.0/src/physicsml/models/allegro/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/supervised/allegro_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/supervised/allegro_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/allegro/supervised/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.764412 physicsml-0.3.0/src/physicsml/models/ani/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/ani_1_2_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/ani_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/ani_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/ani_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.764412 physicsml-0.3.0/src/physicsml/models/ani/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/ensemble/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/ensemble/ensemble_ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/ensemble/ensemble_ani_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.764412 physicsml-0.3.0/src/physicsml/models/ani/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/mean_var/mean_var_ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/mean_var/mean_var_ani_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.764412 physicsml-0.3.0/src/physicsml/models/ani/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27070 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/modules/aev.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.764412 physicsml-0.3.0/src/physicsml/models/ani/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/supervised/ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/supervised/ani_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/ani/supervised/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.764412 physicsml-0.3.0/src/physicsml/models/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.768412 physicsml-0.3.0/src/physicsml/models/egnn/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/adapter/adapter_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/adapter/adapter_egnn_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/adapter/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/egnn_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/egnn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.768412 physicsml-0.3.0/src/physicsml/models/egnn/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.768412 physicsml-0.3.0/src/physicsml/models/egnn/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/ssf/ssf_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/ssf/ssf_egnn_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.768412 physicsml-0.3.0/src/physicsml/models/egnn/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/supervised/egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/egnn/supervised/egnn_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.768412 physicsml-0.3.0/src/physicsml/models/mace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.768412 physicsml-0.3.0/src/physicsml/models/mace/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/adapter/adapter_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/adapter/adapter_mace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/adapter/adapter_mace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/adapter/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/mace_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.772412 physicsml-0.3.0/src/physicsml/models/mace/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/mean_var/mean_var_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/mean_var/mean_var_mace_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.772412 physicsml-0.3.0/src/physicsml/models/mace/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/modules/_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/modules/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/modules/cg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/modules/irreps_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/modules/mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/modules/symmetric_contraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.772412 physicsml-0.3.0/src/physicsml/models/mace/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/ssf/ssf_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/ssf/ssf_mace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/ssf/ssf_mace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.772412 physicsml-0.3.0/src/physicsml/models/mace/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/supervised/mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/mace/supervised/mace_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.772412 physicsml-0.3.0/src/physicsml/models/nequip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.776412 physicsml-0.3.0/src/physicsml/models/nequip/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/adapter/adapter_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/adapter/adapter_nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/adapter/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.776412 physicsml-0.3.0/src/physicsml/models/nequip/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.776412 physicsml-0.3.0/src/physicsml/models/nequip/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/modules/_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/modules/_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/modules/convnet_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/modules/interaction_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/modules/nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/modules/scale_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/nequip_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.776412 physicsml-0.3.0/src/physicsml/models/nequip/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/ssf/ssf_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/ssf/ssf_nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.780412 physicsml-0.3.0/src/physicsml/models/nequip/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/supervised/nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/nequip/supervised/nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.780412 physicsml-0.3.0/src/physicsml/models/tensor_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.780412 physicsml-0.3.0/src/physicsml/models/tensor_net/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/modules/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/modules/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/modules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.780412 physicsml-0.3.0/src/physicsml/models/tensor_net/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/supervised/tensor_net_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/tensor_net/supervised/tensor_net_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.780412 physicsml-0.3.0/src/physicsml/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.780412 physicsml-0.3.0/src/physicsml/plugins/ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/ase/ase_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/ase/ase_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/ase/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/ase/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.780412 physicsml-0.3.0/src/physicsml/plugins/openmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/openmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/openmm/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/openmm/openmm_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/openmm/openmm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/openmm/openmm_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/plugins/openmm/physicsml_potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-26 08:46:54.000000 physicsml-0.3.0/src/physicsml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 08:47:02.000000 physicsml-0.3.0/src/physicsml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.804412 physicsml-0.3.0/src/physicsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-26 08:47:02.000000 physicsml-0.3.0/src/physicsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16518 2024-04-26 08:47:02.000000 physicsml-0.3.0/src/physicsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:47:02.000000 physicsml-0.3.0/src/physicsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-26 08:47:02.000000 physicsml-0.3.0/src/physicsml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-26 08:47:02.000000 physicsml-0.3.0/src/physicsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 08:47:02.000000 physicsml-0.3.0/src/physicsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.784412 physicsml-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.784412 physicsml-0.3.0/tests/ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/ase/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/ase/test_ase_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/ase/test_ase_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.784412 physicsml-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/alanine-dipeptide-truncated.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)   698696 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/ani1x.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.784412 physicsml-0.3.0/tests/data/ani_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/ani_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.784412 physicsml-0.3.0/tests/data/ani_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)  1320280 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/ani_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.788412 physicsml-0.3.0/tests/data/egnn_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/egnn_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.788412 physicsml-0.3.0/tests/data/egnn_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    52081 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/egnn_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/gdb9.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    98022 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/gdb9.sdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.788412 physicsml-0.3.0/tests/data/mace_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/mace_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.788412 physicsml-0.3.0/tests/data/mace_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)   117170 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/mace_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.788412 physicsml-0.3.0/tests/data/nequip_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/nequip_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.788412 physicsml-0.3.0/tests/data/nequip_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/data/nequip_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.788412 physicsml-0.3.0/tests/openeye/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/openeye/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/openeye/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/core/data/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/core/data/test_graph_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/openeye/core/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/core/featurisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/core/featurisation/test_physicsml_featurisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/openeye/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/openeye/integration/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/integration/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/integration/prism/test_egnn_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/openeye/integration/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/integration/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/openeye/integration/training/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/integration/training/egnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openeye/integration/training/egnn/test_egnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/openmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openmm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openmm/test_openmm_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openmm/test_openmm_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16422 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openmm/test_openmm_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openmm/test_openmm_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/openmm/test_openmm_nnp_potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.792412 physicsml-0.3.0/tests/rdkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.796412 physicsml-0.3.0/tests/rdkit/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/core/data/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/core/data/test_graph_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.796412 physicsml-0.3.0/tests/rdkit/core/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/core/featurisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/core/featurisation/test_physicsml_featurisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.796412 physicsml-0.3.0/tests/rdkit/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.796412 physicsml-0.3.0/tests/rdkit/integration/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/prism/test_allegro_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/prism/test_ani_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/prism/test_egnn_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/prism/test_mace_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/prism/test_nequip_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.796412 physicsml-0.3.0/tests/rdkit/integration/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.796412 physicsml-0.3.0/tests/rdkit/integration/training/allegro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/allegro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/allegro/test_allegro_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/allegro/test_allergo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.796412 physicsml-0.3.0/tests/rdkit/integration/training/ani/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/ani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/ani/test_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/ani/test_ani_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/ani/test_ani_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/ani/test_ani_mean_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.800412 physicsml-0.3.0/tests/rdkit/integration/training/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/egnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_adapter_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_egnn_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_ssf_egnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.800412 physicsml-0.3.0/tests/rdkit/integration/training/mace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/mace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/mace/test_adapter_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/mace/test_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/mace/test_mace_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/mace/test_mace_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/mace/test_mace_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/mace/test_ssf_mace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.800412 physicsml-0.3.0/tests/rdkit/integration/training/nequip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/nequip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_adapter_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_nequip_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_ssf_nequip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:47:02.804412 physicsml-0.3.0/tests/rdkit/integration/training/tensor_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/tensor_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/tensor_net/test_tensor_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-26 08:46:54.000000 physicsml-0.3.0/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py
```

### Comparing `physicsml-0.2.4/.envrc` & `physicsml-0.3.0/.envrc`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/.github/workflows/docs-build-deploy.yaml` & `physicsml-0.3.0/.github/workflows/docs-build-deploy.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/.github/workflows/latest-tests.yaml` & `physicsml-0.3.0/.github/workflows/latest-tests.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/.github/workflows/pinned-tests.yaml` & `physicsml-0.3.0/.github/workflows/pinned-tests.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/.github/workflows/publish-package.yaml` & `physicsml-0.3.0/.github/workflows/publish-package.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/.github/workflows/quality-typing-checks.yaml` & `physicsml-0.3.0/.github/workflows/quality-typing-checks.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/.gitignore` & `physicsml-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/.pre-commit-config.yaml` & `physicsml-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/CHANGELOG.md` & `physicsml-0.3.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project
 adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 ---------------------------------------------------------
 
 ## [Unreleased]
 
 ---------------------------------------------------------
- ## [0.2.4] - 2024-04-24
+ ## [0.3.0] - 2024-04-25
+
+### Added
+
+* Added graph attrs in graph datasets/loaders
+
+## [0.2.4] - 2024-04-24
 
 ### Fixed
 
 * Added coordinate wrapping in the neighbour list computations of ANI and graphs
 
 ## [0.2.3] - 2024-04-09
```

### Comparing `physicsml-0.2.4/LICENSE` & `physicsml-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/PKG-INFO` & `physicsml-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsml
-Version: 0.2.4
+Version: 0.3.0
 Summary: A package for all physics based/related models
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/physicsml/issues
 Project-URL: repository, https://github.com/exscientia/physicsml.git
 Project-URL: issue-tracker, https://github.com/exscientia/physicsml/issues
 Project-URL: changelog, https://github.com/exscientia/physicsml/src/main/CHANGELOG.md
```

### Comparing `physicsml-0.2.4/README.md` & `physicsml-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/Makefile` & `physicsml-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/make.bat` & `physicsml-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo-01.svg` & `physicsml-0.3.0/docs/source/_static/PhysicsML_Logo-01.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg` & `physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg` & `physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg` & `physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg` & `physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg` & `physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg` & `physicsml-0.3.0/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/conf.py` & `physicsml-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/index.md` & `physicsml-0.3.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/datasets/qm_datasets.md` & `physicsml-0.3.0/docs/source/pages/datasets/qm_datasets.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/features/gdb9_trunc.parquet` & `physicsml-0.3.0/docs/source/pages/features/gdb9_trunc.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/features/how_to_add_reps.md` & `physicsml-0.3.0/docs/source/pages/features/how_to_add_reps.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/features/intro.md` & `physicsml-0.3.0/docs/source/pages/features/intro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/models/allegro.md` & `physicsml-0.3.0/docs/source/pages/models/allegro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/models/ani.md` & `physicsml-0.3.0/docs/source/pages/models/ani.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/models/egnn.md` & `physicsml-0.3.0/docs/source/pages/models/egnn.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/models/how_to_add_models.md` & `physicsml-0.3.0/docs/source/pages/models/how_to_add_models.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/models/intro.md` & `physicsml-0.3.0/docs/source/pages/models/intro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/models/mace.md` & `physicsml-0.3.0/docs/source/pages/models/mace.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/models/nequip.md` & `physicsml-0.3.0/docs/source/pages/models/nequip.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/models/tensor_net.md` & `physicsml-0.3.0/docs/source/pages/models/tensor_net.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/philosophy/molflux.md` & `physicsml-0.3.0/docs/source/pages/philosophy/molflux.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/philosophy/philosophy.md` & `physicsml-0.3.0/docs/source/pages/philosophy/philosophy.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb` & `physicsml-0.3.0/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/plugins/ase.md` & `physicsml-0.3.0/docs/source/pages/plugins/ase.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/plugins/openmm.md` & `physicsml-0.3.0/docs/source/pages/plugins/openmm.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/structure/lightning_layer.md` & `physicsml-0.3.0/docs/source/pages/structure/lightning_layer.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 * ``num_workers: Optional[str, int] = 0``
 
     The number of workers to use. Can set to ``"all"`` to use all workers. If running on CPU only machine make sure to
     set to 0 (otherwise processes can hang).
 * ``num_elements: int = 0``
 
     The number of atomic elements used (for example 4 in ANI1x).
+* ``graph_attrs_cols: Optional[List[str]] = None
+
+    The names of the graph attributes in the input dataset to be concatenated and added to the batch.
 * ``y_node_scalars: Optional[List[str]] = None``
 
     The subset of ``y_features`` which are node level scalars (for example partial charges).
 * ``y_node_vector: Optional[str] = None``
 
     The feature from``y_features`` which is a node level vector.
 * ``y_edge_scalars: Optional[List[str]] = None``
```

### Comparing `physicsml-0.2.4/docs/source/pages/structure/molflux_layer.md` & `physicsml-0.3.0/docs/source/pages/structure/molflux_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/structure/physicsml_structure.md` & `physicsml-0.3.0/docs/source/pages/structure/physicsml_structure.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/structure/torch_layer.md` & `physicsml-0.3.0/docs/source/pages/structure/torch_layer.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 
     The node attributes (i.e. initial node features). It is a good idea to keep these distinct from node features
     (for downstream operations which require the original node attributes).
 * ``edge_attrs: Shape = torch.Size([num_edges, dim_edge_attrs]) Type = torch.float32``
 
     The edge attributes (i.e. initial edge features). It is a good idea to keep these distinct from edge features
     (for downstream operations which require the original edge attributes).
+* ``graph_attrs: Shape = torch.Size([num_graphs, dim_graph_attrs]) Type = torch.float32``
+
+    The graph attributes.
 * ``coordinates: Shape = torch.Size([num_nodes, 3]) Type = torch.float32``
 
     The coordinates.
 * ``total_atomic_energy: Shape = torch.Size([num_graphs]) Type = torch.float32``
 
     The summed up atomic energies.
 * ``raw_atomic_numbers: Shape = torch.Size([num_nodes]) Type = torch.int64``
```

### Comparing `physicsml-0.2.4/docs/source/pages/structure/transfer_learning.md` & `physicsml-0.3.0/docs/source/pages/structure/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/tutorials/ani1x_energy_forces_training.md` & `physicsml-0.3.0/docs/source/pages/tutorials/ani1x_energy_forces_training.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/tutorials/ani1x_truncated.parquet` & `physicsml-0.3.0/docs/source/pages/tutorials/ani1x_truncated.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/tutorials/gdb9_training.md` & `physicsml-0.3.0/docs/source/pages/tutorials/gdb9_training.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/tutorials/gdb9_trunc.parquet` & `physicsml-0.3.0/docs/source/pages/tutorials/gdb9_trunc.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/tutorials/gdb9_uncertainty.md` & `physicsml-0.3.0/docs/source/pages/tutorials/gdb9_uncertainty.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/docs/source/pages/tutorials/transfer_learning.md` & `physicsml-0.3.0/docs/source/pages/tutorials/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/init_conda_venv.sh` & `physicsml-0.3.0/init_conda_venv.sh`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/init_python_venv.sh` & `physicsml-0.3.0/init_python_venv.sh`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/noxfile.py` & `physicsml-0.3.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.10/lockfile.ase.txt` & `physicsml-0.3.0/pinned-versions/3.10/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.10/lockfile.core.txt` & `physicsml-0.3.0/pinned-versions/3.10/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.10/lockfile.openeye.txt` & `physicsml-0.3.0/pinned-versions/3.10/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.10/lockfile.openmm.txt` & `physicsml-0.3.0/pinned-versions/3.10/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.10/lockfile.rdkit.txt` & `physicsml-0.3.0/pinned-versions/3.10/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.11/lockfile.ase.txt` & `physicsml-0.3.0/pinned-versions/3.11/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.11/lockfile.core.txt` & `physicsml-0.3.0/pinned-versions/3.11/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.11/lockfile.openeye.txt` & `physicsml-0.3.0/pinned-versions/3.11/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.11/lockfile.openmm.txt` & `physicsml-0.3.0/pinned-versions/3.11/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.11/lockfile.rdkit.txt` & `physicsml-0.3.0/pinned-versions/3.11/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.8/lockfile.ase.txt` & `physicsml-0.3.0/pinned-versions/3.8/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.8/lockfile.core.txt` & `physicsml-0.3.0/pinned-versions/3.8/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.8/lockfile.openeye.txt` & `physicsml-0.3.0/pinned-versions/3.8/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.8/lockfile.openmm.txt` & `physicsml-0.3.0/pinned-versions/3.8/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.8/lockfile.rdkit.txt` & `physicsml-0.3.0/pinned-versions/3.8/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.9/lockfile.ase.txt` & `physicsml-0.3.0/pinned-versions/3.9/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.9/lockfile.core.txt` & `physicsml-0.3.0/pinned-versions/3.9/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.9/lockfile.openeye.txt` & `physicsml-0.3.0/pinned-versions/3.9/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.9/lockfile.openmm.txt` & `physicsml-0.3.0/pinned-versions/3.9/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pinned-versions/3.9/lockfile.rdkit.txt` & `physicsml-0.3.0/pinned-versions/3.9/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/pyproject.toml` & `physicsml-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/backends/backend_selector.py` & `physicsml-0.3.0/src/physicsml/backends/backend_selector.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/backends/openeye_backend.py` & `physicsml-0.3.0/src/physicsml/backends/openeye_backend.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/backends/rdkit_backend.py` & `physicsml-0.3.0/src/physicsml/backends/rdkit_backend.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/atom_features.py` & `physicsml-0.3.0/src/physicsml/featurisation/physicsml_features/atom_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/bond_features.py` & `physicsml-0.3.0/src/physicsml/featurisation/physicsml_features/bond_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/physicsml_features.py` & `physicsml-0.3.0/src/physicsml/featurisation/physicsml_features/physicsml_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/config.py` & `physicsml-0.3.0/src/physicsml/lightning/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     y_graph_vector: Optional[str] = None
     atomic_numbers_col: str = "physicsml_atom_numbers"
     coordinates_col: str = "physicsml_coordinates"
     node_attrs_col: str = "physicsml_atom_features"
     edge_attrs_col: str = "physicsml_bond_features"
     node_idxs_col: str = "physicsml_atom_idxs"
     edge_idxs_col: str = "physicsml_bond_idxs"
+    graph_attrs_cols: Optional[List[str]] = None
     total_atomic_energy_col: str = "physicsml_total_atomic_energy"
     cut_off: float = 5.0
     pbc: Optional[Tuple[bool, bool, bool]] = None
     cell: Optional[List[List[float]]] = None
     self_interaction: bool = False
     use_scaled_positions: bool = False
     max_nbins: int = int(1e6)
```

### Comparing `physicsml-0.2.4/src/physicsml/lightning/datamodule.py` & `physicsml-0.3.0/src/physicsml/lightning/datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
             with_y_features=(split != "predict"),
             atomic_numbers_col=self.model_config.datamodule.atomic_numbers_col,
             node_attrs_col=self.model_config.datamodule.node_attrs_col,
             edge_attrs_col=self.model_config.datamodule.edge_attrs_col,
             node_idxs_col=self.model_config.datamodule.node_idxs_col,
             edge_idxs_col=self.model_config.datamodule.edge_idxs_col,
             coordinates_col=self.model_config.datamodule.coordinates_col,
+            graph_attrs_cols=self.model_config.datamodule.graph_attrs_cols,
             total_atomic_energy_col=self.model_config.datamodule.total_atomic_energy_col,
             y_node_scalars=self.model_config.datamodule.y_node_scalars,
             y_node_vector=self.model_config.datamodule.y_node_vector,
             y_edge_scalars=self.model_config.datamodule.y_edge_scalars,
             y_edge_vector=self.model_config.datamodule.y_edge_vector,
             y_graph_scalars=self.model_config.datamodule.y_graph_scalars,
             y_graph_vector=self.model_config.datamodule.y_graph_vector,
```

### Comparing `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/graph_dataset.py` & `physicsml-0.3.0/src/physicsml/lightning/graph_datasets/graph_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     num_graphs: Optional[torch.Tensor]
     batch: Optional[torch.Tensor]
     raw_atomic_numbers: Optional[torch.Tensor]
     atomic_numbers: Optional[torch.Tensor]
     edge_index: Optional[torch.Tensor]
     node_attrs: Optional[torch.Tensor]
     edge_attrs: Optional[torch.Tensor]
+    graph_attrs: Optional[torch.Tensor]
     y_node_scalars: Optional[torch.Tensor]
     y_node_vector: Optional[torch.Tensor]
     y_edge_scalars: Optional[torch.Tensor]
     y_edge_vector: Optional[torch.Tensor]
     y_graph_scalars: Optional[torch.Tensor]
     y_graph_vector: Optional[torch.Tensor]
     cell: Optional[torch.Tensor]
@@ -32,14 +33,15 @@
     def __init__(
         self,
         raw_atomic_numbers: Optional[torch.Tensor],  # [n_nodes]
         atomic_numbers: Optional[torch.Tensor],  # [n_nodes]
         edge_index: Optional[torch.Tensor],  # [2, n_edges]
         node_attrs: Optional[torch.Tensor],  # [n_nodes, n_node_attrs]
         edge_attrs: Optional[torch.Tensor],  # [n_edges, n_edge_attrs]
+        graph_attrs: Optional[torch.Tensor],  # [1, n_graph_attrs]
         y_node_scalars: Optional[torch.Tensor],  # [n_nodes, n_scalars]
         y_node_vector: Optional[torch.Tensor],  # [n_nodes, dim_vector]
         y_edge_scalars: Optional[torch.Tensor],  # [n_edges, n_scalars]
         y_edge_vector: Optional[torch.Tensor],  # [n_edges, dim_vector]
         y_graph_scalars: Optional[torch.Tensor],  # [n_scalars]
         y_graph_vector: Optional[torch.Tensor],  # [dim_vector]
         cell: Optional[torch.Tensor],  # [3, 3]
@@ -78,14 +80,15 @@
         data = {
             "num_nodes": num_nodes,
             "raw_atomic_numbers": raw_atomic_numbers,
             "atomic_numbers": atomic_numbers,
             "edge_index": edge_index,
             "node_attrs": node_attrs,
             "edge_attrs": edge_attrs,
+            "graph_attrs": graph_attrs,
             "y_node_scalars": y_node_scalars,
             "y_node_vector": y_node_vector,
             "y_edge_scalars": y_edge_scalars,
             "y_edge_vector": y_edge_vector,
             "y_graph_scalars": y_graph_scalars,
             "y_graph_vector": y_graph_vector,
             "cell": cell,
@@ -148,14 +151,15 @@
         y_features: Optional[List],
         with_y_features: bool,
         atomic_numbers_col: str,
         node_attrs_col: str,
         edge_attrs_col: str,
         node_idxs_col: str,
         edge_idxs_col: str,
+        graph_attrs_cols: Optional[List[str]],
         coordinates_col: str,
         total_atomic_energy_col: str,
         y_node_scalars: Optional[List[str]],
         y_node_vector: Optional[str],
         y_edge_scalars: Optional[List[str]],
         y_edge_vector: Optional[str],
         y_graph_scalars: Optional[List[str]],
@@ -174,14 +178,19 @@
 
         # columns
         self.atomic_numbers_col = atomic_numbers_col
         self.node_attrs_col = node_attrs_col
         self.edge_attrs_col = edge_attrs_col
         self.node_idxs_col = node_idxs_col
         self.edge_idxs_col = edge_idxs_col
+        self.graph_attrs_cols = graph_attrs_cols
+        # sort alphabetically
+        if self.graph_attrs_cols is not None:
+            self.graph_attrs_cols = sorted(self.graph_attrs_cols)
+
         self.coordinates_col = coordinates_col
         self.total_atomic_energy_col = total_atomic_energy_col
 
         # num elements
         self.num_elements = num_elements
 
         # neighbourhood setup
@@ -244,14 +253,30 @@
         raw_atomic_numbers = datapoint.get(self.atomic_numbers_col, None)
         node_attrs = datapoint.get(self.node_attrs_col, None)
         initial_edge_attrs = datapoint.get(self.edge_attrs_col, None)
         initial_edge_indices = datapoint.get(self.edge_idxs_col, None)
         coordinates = datapoint[self.coordinates_col]
         total_atomic_energy = datapoint.get(self.total_atomic_energy_col, None)
 
+        if self.graph_attrs_cols is not None:
+            graph_attrs_list = []
+            for graph_attrs_col in self.graph_attrs_cols:
+                feat = datapoint[graph_attrs_col]
+                if isinstance(feat, list):
+                    graph_attrs_list += feat
+                elif isinstance(feat, float):
+                    graph_attrs_list.append(feat)
+                else:
+                    raise RuntimeError(
+                        f"Unsupported type {type(feat)} for graph attributes.",
+                    )
+            graph_attrs = torch.tensor(graph_attrs_list).unsqueeze(0) * 1.0
+        else:
+            graph_attrs = None
+
         if raw_atomic_numbers is not None:
             raw_atomic_numbers = torch.tensor(raw_atomic_numbers)
             atomic_numbers: Optional[torch.Tensor] = (
                 torch.nn.functional.one_hot(
                     raw_atomic_numbers,
                     num_classes=self.num_elements,
                 )
@@ -348,14 +373,15 @@
             atomic_numbers=atomic_numbers,
             total_atomic_energy=total_atomic_energy,
             coordinates=coordinates,
             edge_index=edge_indices,
             cell_shift_vector=cell_shift_vector,
             node_attrs=node_attrs,
             edge_attrs=edge_attrs,
+            graph_attrs=graph_attrs,
             y_node_scalars=y_node_scalars,
             y_node_vector=y_node_vector,
             y_edge_scalars=y_edge_scalars,
             y_edge_vector=y_edge_vector,
             y_graph_scalars=y_graph_scalars,
             y_graph_vector=y_graph_vector,
             cell=self.cell_ten,
```

### Comparing `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py` & `physicsml-0.3.0/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py` & `physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py` & `physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py` & `physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py` & `physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py` & `physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py` & `physicsml-0.3.0/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/losses/barlow_twins_loss.py` & `physicsml-0.3.0/src/physicsml/lightning/losses/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/losses/loss_base.py` & `physicsml-0.3.0/src/physicsml/lightning/losses/loss_base.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/losses/masked_mse_loss.py` & `physicsml-0.3.0/src/physicsml/lightning/losses/masked_mse_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/losses/multitask_losses.py` & `physicsml-0.3.0/src/physicsml/lightning/losses/multitask_losses.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py` & `physicsml-0.3.0/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/losses/stock_losses.py` & `physicsml-0.3.0/src/physicsml/lightning/losses/stock_losses.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/losses/weighted_mse_loss.py` & `physicsml-0.3.0/src/physicsml/lightning/losses/weighted_mse_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/model.py` & `physicsml-0.3.0/src/physicsml/lightning/model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/model_uncertainty.py` & `physicsml-0.3.0/src/physicsml/lightning/model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/module.py` & `physicsml-0.3.0/src/physicsml/lightning/module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/pre_batching_in_memory.py` & `physicsml-0.3.0/src/physicsml/lightning/pre_batching_in_memory.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/lightning/pre_batching_on_disk.py` & `physicsml-0.3.0/src/physicsml/lightning/pre_batching_on_disk.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/allegro_prism.py` & `physicsml-0.3.0/src/physicsml/models/allegro/allegro_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/mean_var/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/allegro/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py` & `physicsml-0.3.0/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py` & `physicsml-0.3.0/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/modules/allegro.py` & `physicsml-0.3.0/src/physicsml/models/allegro/modules/allegro.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/modules/channels.py` & `physicsml-0.3.0/src/physicsml/models/allegro/modules/channels.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/modules/contract.py` & `physicsml-0.3.0/src/physicsml/models/allegro/modules/contract.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/modules/cutoffs.py` & `physicsml-0.3.0/src/physicsml/models/allegro/modules/cutoffs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/modules/fc.py` & `physicsml-0.3.0/src/physicsml/models/allegro/modules/fc.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/modules/layout.py` & `physicsml-0.3.0/src/physicsml/models/allegro/modules/layout.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/modules/linear.py` & `physicsml-0.3.0/src/physicsml/models/allegro/modules/linear.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/modules/radial.py` & `physicsml-0.3.0/src/physicsml/models/allegro/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/modules/spmm.py` & `physicsml-0.3.0/src/physicsml/models/allegro/modules/spmm.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/supervised/allegro_model.py` & `physicsml-0.3.0/src/physicsml/models/allegro/supervised/allegro_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/supervised/allegro_module.py` & `physicsml-0.3.0/src/physicsml/models/allegro/supervised/allegro_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/allegro/supervised/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/allegro/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/ani_1_2_defaults.py` & `physicsml-0.3.0/src/physicsml/models/ani/ani_1_2_defaults.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/ani_datamodule.py` & `physicsml-0.3.0/src/physicsml/models/ani/ani_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/ani_dataset.py` & `physicsml-0.3.0/src/physicsml/models/ani/ani_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/ani_prism.py` & `physicsml-0.3.0/src/physicsml/models/ani/ani_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/config.py` & `physicsml-0.3.0/src/physicsml/models/ani/config.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/ensemble/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/ani/ensemble/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/ensemble/ensemble_ani_model.py` & `physicsml-0.3.0/src/physicsml/models/ani/ensemble/ensemble_ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/ensemble/ensemble_ani_module.py` & `physicsml-0.3.0/src/physicsml/models/ani/ensemble/ensemble_ani_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/mean_var/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/ani/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/mean_var/mean_var_ani_model.py` & `physicsml-0.3.0/src/physicsml/models/ani/mean_var/mean_var_ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/mean_var/mean_var_ani_module.py` & `physicsml-0.3.0/src/physicsml/models/ani/mean_var/mean_var_ani_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/modules/aev.py` & `physicsml-0.3.0/src/physicsml/models/ani/modules/aev.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/supervised/ani_model.py` & `physicsml-0.3.0/src/physicsml/models/ani/supervised/ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/supervised/ani_module.py` & `physicsml-0.3.0/src/physicsml/models/ani/supervised/ani_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/ani/supervised/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/ani/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_model.py` & `physicsml-0.3.0/src/physicsml/models/egnn/adapter/adapter_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_module.py` & `physicsml-0.3.0/src/physicsml/models/egnn/adapter/adapter_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py` & `physicsml-0.3.0/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/adapter/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/egnn/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/egnn_prism.py` & `physicsml-0.3.0/src/physicsml/models/egnn/egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/egnn_utils.py` & `physicsml-0.3.0/src/physicsml/models/egnn/egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/mean_var/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/egnn/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py` & `physicsml-0.3.0/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py` & `physicsml-0.3.0/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/ssf/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/egnn/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_model.py` & `physicsml-0.3.0/src/physicsml/models/egnn/ssf/ssf_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_module.py` & `physicsml-0.3.0/src/physicsml/models/egnn/ssf/ssf_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py` & `physicsml-0.3.0/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/supervised/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/egnn/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/supervised/egnn_model.py` & `physicsml-0.3.0/src/physicsml/models/egnn/supervised/egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/egnn/supervised/egnn_module.py` & `physicsml-0.3.0/src/physicsml/models/egnn/supervised/egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_model.py` & `physicsml-0.3.0/src/physicsml/models/mace/adapter/adapter_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_module.py` & `physicsml-0.3.0/src/physicsml/models/mace/adapter/adapter_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_utils.py` & `physicsml-0.3.0/src/physicsml/models/mace/adapter/adapter_mace_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/adapter/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/mace/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/mace_prism.py` & `physicsml-0.3.0/src/physicsml/models/mace/mace_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/mean_var/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/mace/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/mean_var/mean_var_mace_model.py` & `physicsml-0.3.0/src/physicsml/models/mace/mean_var/mean_var_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/mean_var/mean_var_mace_module.py` & `physicsml-0.3.0/src/physicsml/models/mace/mean_var/mean_var_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/modules/_activation.py` & `physicsml-0.3.0/src/physicsml/models/mace/modules/_activation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/modules/blocks.py` & `physicsml-0.3.0/src/physicsml/models/mace/modules/blocks.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/modules/cg.py` & `physicsml-0.3.0/src/physicsml/models/mace/modules/cg.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/modules/irreps_tools.py` & `physicsml-0.3.0/src/physicsml/models/mace/modules/irreps_tools.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/modules/mace.py` & `physicsml-0.3.0/src/physicsml/models/mace/modules/mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/modules/radial.py` & `physicsml-0.3.0/src/physicsml/models/mace/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/modules/symmetric_contraction.py` & `physicsml-0.3.0/src/physicsml/models/mace/modules/symmetric_contraction.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/ssf/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/mace/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_model.py` & `physicsml-0.3.0/src/physicsml/models/mace/ssf/ssf_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_module.py` & `physicsml-0.3.0/src/physicsml/models/mace/ssf/ssf_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_utils.py` & `physicsml-0.3.0/src/physicsml/models/mace/ssf/ssf_mace_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/supervised/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/mace/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/supervised/mace_model.py` & `physicsml-0.3.0/src/physicsml/models/mace/supervised/mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/mace/supervised/mace_module.py` & `physicsml-0.3.0/src/physicsml/models/mace/supervised/mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_model.py` & `physicsml-0.3.0/src/physicsml/models/nequip/adapter/adapter_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_module.py` & `physicsml-0.3.0/src/physicsml/models/nequip/adapter/adapter_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py` & `physicsml-0.3.0/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/adapter/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/nequip/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/mean_var/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/nequip/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py` & `physicsml-0.3.0/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py` & `physicsml-0.3.0/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/modules/_activation.py` & `physicsml-0.3.0/src/physicsml/models/nequip/modules/_activation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/modules/_gate.py` & `physicsml-0.3.0/src/physicsml/models/nequip/modules/_gate.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/modules/convnet_layer.py` & `physicsml-0.3.0/src/physicsml/models/nequip/modules/convnet_layer.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/modules/interaction_block.py` & `physicsml-0.3.0/src/physicsml/models/nequip/modules/interaction_block.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/modules/nequip.py` & `physicsml-0.3.0/src/physicsml/models/nequip/modules/nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/modules/radial.py` & `physicsml-0.3.0/src/physicsml/models/nequip/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/modules/scale_shift.py` & `physicsml-0.3.0/src/physicsml/models/nequip/modules/scale_shift.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/nequip_prism.py` & `physicsml-0.3.0/src/physicsml/models/nequip/nequip_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/ssf/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/nequip/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_model.py` & `physicsml-0.3.0/src/physicsml/models/nequip/ssf/ssf_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_module.py` & `physicsml-0.3.0/src/physicsml/models/nequip/ssf/ssf_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py` & `physicsml-0.3.0/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/supervised/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/nequip/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/supervised/nequip_model.py` & `physicsml-0.3.0/src/physicsml/models/nequip/supervised/nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/nequip/supervised/nequip_module.py` & `physicsml-0.3.0/src/physicsml/models/nequip/supervised/nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/prism.py` & `physicsml-0.3.0/src/physicsml/models/prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/tensor_net/modules/embedding.py` & `physicsml-0.3.0/src/physicsml/models/tensor_net/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/tensor_net/modules/interaction.py` & `physicsml-0.3.0/src/physicsml/models/tensor_net/modules/interaction.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/tensor_net/modules/output.py` & `physicsml-0.3.0/src/physicsml/models/tensor_net/modules/output.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/tensor_net/modules/utils.py` & `physicsml-0.3.0/src/physicsml/models/tensor_net/modules/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/default_configs.py` & `physicsml-0.3.0/src/physicsml/models/tensor_net/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/tensor_net_model.py` & `physicsml-0.3.0/src/physicsml/models/tensor_net/supervised/tensor_net_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/tensor_net_module.py` & `physicsml-0.3.0/src/physicsml/models/tensor_net/supervised/tensor_net_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/models/utils.py` & `physicsml-0.3.0/src/physicsml/models/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/plugins/ase/ase_ani.py` & `physicsml-0.3.0/src/physicsml/plugins/ase/ase_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/plugins/ase/ase_graph.py` & `physicsml-0.3.0/src/physicsml/plugins/ase/ase_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/plugins/ase/calculator.py` & `physicsml-0.3.0/src/physicsml/plugins/ase/calculator.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/plugins/ase/load.py` & `physicsml-0.3.0/src/physicsml/plugins/ase/load.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/plugins/openmm/load.py` & `physicsml-0.3.0/src/physicsml/plugins/openmm/load.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_ani.py` & `physicsml-0.3.0/src/physicsml/plugins/openmm/openmm_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_base.py` & `physicsml-0.3.0/src/physicsml/plugins/openmm/openmm_base.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_graph.py` & `physicsml-0.3.0/src/physicsml/plugins/openmm/openmm_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/plugins/openmm/physicsml_potential.py` & `physicsml-0.3.0/src/physicsml/plugins/openmm/physicsml_potential.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml/utils.py` & `physicsml-0.3.0/src/physicsml/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml.egg-info/PKG-INFO` & `physicsml-0.3.0/src/physicsml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsml
-Version: 0.2.4
+Version: 0.3.0
 Summary: A package for all physics based/related models
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/physicsml/issues
 Project-URL: repository, https://github.com/exscientia/physicsml.git
 Project-URL: issue-tracker, https://github.com/exscientia/physicsml/issues
 Project-URL: changelog, https://github.com/exscientia/physicsml/src/main/CHANGELOG.md
```

### Comparing `physicsml-0.2.4/src/physicsml.egg-info/SOURCES.txt` & `physicsml-0.3.0/src/physicsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml.egg-info/entry_points.txt` & `physicsml-0.3.0/src/physicsml.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/src/physicsml.egg-info/requires.txt` & `physicsml-0.3.0/src/physicsml.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/ase/conftest.py` & `physicsml-0.3.0/tests/ase/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/ase/test_ase_ani.py` & `physicsml-0.3.0/tests/ase/test_ase_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/ase/test_ase_graph.py` & `physicsml-0.3.0/tests/ase/test_ase_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/alanine-dipeptide-truncated.pdb` & `physicsml-0.3.0/tests/data/alanine-dipeptide-truncated.pdb`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/ani1x.h5` & `physicsml-0.3.0/tests/data/ani1x.h5`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/ani_model/featurisation_metadata.json` & `physicsml-0.3.0/tests/data/ani_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.3.0/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/ani_model/model_config.json` & `physicsml-0.3.0/tests/data/ani_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/egnn_model/featurisation_metadata.json` & `physicsml-0.3.0/tests/data/egnn_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.3.0/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/egnn_model/model_config.json` & `physicsml-0.3.0/tests/data/egnn_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/gdb9.csv` & `physicsml-0.3.0/tests/data/gdb9.csv`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/gdb9.sdf` & `physicsml-0.3.0/tests/data/gdb9.sdf`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/mace_model/featurisation_metadata.json` & `physicsml-0.3.0/tests/data/mace_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.3.0/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/mace_model/model_config.json` & `physicsml-0.3.0/tests/data/mace_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/nequip_model/featurisation_metadata.json` & `physicsml-0.3.0/tests/data/nequip_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.3.0/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/data/nequip_model/model_config.json` & `physicsml-0.3.0/tests/data/nequip_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openeye/conftest.py` & `physicsml-0.3.0/tests/openeye/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openeye/core/data/test_datamodule.py` & `physicsml-0.3.0/tests/openeye/core/data/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openeye/core/data/test_graph_dataset.py` & `physicsml-0.3.0/tests/openeye/core/data/test_graph_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         y_features=None,
         with_y_features=False,
         atomic_numbers_col="physicsml_atom_numbers",
         node_attrs_col="physicsml_atom_features",
         edge_attrs_col="physicsml_bond_features",
         node_idxs_col="physicsml_atom_idxs",
         edge_idxs_col="physicsml_bond_idxs",
+        graph_attrs_cols=None,
         coordinates_col="physicsml_coordinates",
         total_atomic_energy_col="physicsml_total_atomic_energy_col",
         num_elements=4,
         cut_off=5.0,
         y_node_scalars=None,
         y_node_vector=None,
         y_edge_scalars=None,
@@ -66,14 +67,15 @@
         y_features=None,
         with_y_features=False,
         atomic_numbers_col="physicsml_atom_numbers",
         node_attrs_col="physicsml_atom_features",
         edge_attrs_col="physicsml_bond_features",
         node_idxs_col="physicsml_atom_idxs",
         edge_idxs_col="physicsml_bond_idxs",
+        graph_attrs_cols=None,
         coordinates_col="physicsml_coordinates",
         total_atomic_energy_col="physicsml_total_atomic_energy_col",
         num_elements=4,
         cut_off=5.0,
         y_node_scalars=None,
         y_node_vector=None,
         y_edge_scalars=None,
@@ -119,14 +121,15 @@
         y_features=None,
         with_y_features=False,
         atomic_numbers_col="physicsml_atom_numbers",
         node_attrs_col="physicsml_atom_features",
         edge_attrs_col="physicsml_bond_features",
         node_idxs_col="physicsml_atom_idxs",
         edge_idxs_col="physicsml_bond_idxs",
+        graph_attrs_cols=None,
         coordinates_col="physicsml_coordinates",
         total_atomic_energy_col="physicsml_total_atomic_energy_col",
         num_elements=4,
         cut_off=5.0,
         y_node_scalars=None,
         y_node_vector=None,
         y_edge_scalars=None,
```

### Comparing `physicsml-0.2.4/tests/openeye/core/featurisation/test_physicsml_featurisation.py` & `physicsml-0.3.0/tests/openeye/core/featurisation/test_physicsml_featurisation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openeye/integration/prism/test_egnn_prism.py` & `physicsml-0.3.0/tests/openeye/integration/prism/test_egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openeye/integration/training/egnn/test_egnn.py` & `physicsml-0.3.0/tests/openeye/integration/training/egnn/test_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openmm/conftest.py` & `physicsml-0.3.0/tests/openmm/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openmm/test_openmm_ani.py` & `physicsml-0.3.0/tests/openmm/test_openmm_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openmm/test_openmm_egnn.py` & `physicsml-0.3.0/tests/openmm/test_openmm_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openmm/test_openmm_mace.py` & `physicsml-0.3.0/tests/openmm/test_openmm_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openmm/test_openmm_nequip.py` & `physicsml-0.3.0/tests/openmm/test_openmm_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/openmm/test_openmm_nnp_potential.py` & `physicsml-0.3.0/tests/openmm/test_openmm_nnp_potential.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/conftest.py` & `physicsml-0.3.0/tests/rdkit/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/core/data/test_datamodule.py` & `physicsml-0.3.0/tests/rdkit/core/data/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/core/data/test_graph_dataset.py` & `physicsml-0.3.0/tests/rdkit/core/data/test_graph_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         y_features=None,
         with_y_features=False,
         atomic_numbers_col="physicsml_atom_numbers",
         node_attrs_col="physicsml_atom_features",
         edge_attrs_col="physicsml_bond_features",
         node_idxs_col="physicsml_atom_idxs",
         edge_idxs_col="physicsml_bond_idxs",
+        graph_attrs_cols=None,
         coordinates_col="physicsml_coordinates",
         total_atomic_energy_col="physicsml_total_atomic_energy_col",
         num_elements=4,
         cut_off=5.0,
         y_node_scalars=None,
         y_node_vector=None,
         y_edge_scalars=None,
@@ -66,14 +67,15 @@
         y_features=None,
         with_y_features=False,
         atomic_numbers_col="physicsml_atom_numbers",
         node_attrs_col="physicsml_atom_features",
         edge_attrs_col="physicsml_bond_features",
         node_idxs_col="physicsml_atom_idxs",
         edge_idxs_col="physicsml_bond_idxs",
+        graph_attrs_cols=None,
         coordinates_col="physicsml_coordinates",
         total_atomic_energy_col="physicsml_total_atomic_energy_col",
         num_elements=4,
         cut_off=5.0,
         y_node_scalars=None,
         y_node_vector=None,
         y_edge_scalars=None,
@@ -119,14 +121,15 @@
         y_features=None,
         with_y_features=False,
         atomic_numbers_col="physicsml_atom_numbers",
         node_attrs_col="physicsml_atom_features",
         edge_attrs_col="physicsml_bond_features",
         node_idxs_col="physicsml_atom_idxs",
         edge_idxs_col="physicsml_bond_idxs",
+        graph_attrs_cols=None,
         coordinates_col="physicsml_coordinates",
         total_atomic_energy_col="physicsml_total_atomic_energy_col",
         num_elements=4,
         cut_off=5.0,
         y_node_scalars=None,
         y_node_vector=None,
         y_edge_scalars=None,
```

### Comparing `physicsml-0.2.4/tests/rdkit/core/featurisation/test_physicsml_featurisation.py` & `physicsml-0.3.0/tests/rdkit/core/featurisation/test_physicsml_featurisation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/prism/test_allegro_prism.py` & `physicsml-0.3.0/tests/rdkit/integration/prism/test_allegro_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/prism/test_ani_prism.py` & `physicsml-0.3.0/tests/rdkit/integration/prism/test_ani_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/prism/test_egnn_prism.py` & `physicsml-0.3.0/tests/rdkit/integration/prism/test_egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/prism/test_mace_prism.py` & `physicsml-0.3.0/tests/rdkit/integration/prism/test_mace_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/prism/test_nequip_prism.py` & `physicsml-0.3.0/tests/rdkit/integration/prism/test_nequip_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py` & `physicsml-0.3.0/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_forces.py` & `physicsml-0.3.0/tests/rdkit/integration/training/allegro/test_allegro_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py` & `physicsml-0.3.0/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allergo.py` & `physicsml-0.3.0/tests/rdkit/integration/training/allegro/test_allergo.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani.py` & `physicsml-0.3.0/tests/rdkit/integration/training/ani/test_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_ensemble.py` & `physicsml-0.3.0/tests/rdkit/integration/training/ani/test_ani_ensemble.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_forces.py` & `physicsml-0.3.0/tests/rdkit/integration/training/ani/test_ani_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_mean_var.py` & `physicsml-0.3.0/tests/rdkit/integration/training/ani/test_ani_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_adapter_egnn.py` & `physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_adapter_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn.py` & `physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py` & `physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_forces.py` & `physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_egnn_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py` & `physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_ssf_egnn.py` & `physicsml-0.3.0/tests/rdkit/integration/training/egnn/test_ssf_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_adapter_mace.py` & `physicsml-0.3.0/tests/rdkit/integration/training/mace/test_adapter_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace.py` & `physicsml-0.3.0/tests/rdkit/integration/training/mace/test_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_energy_charges.py` & `physicsml-0.3.0/tests/rdkit/integration/training/mace/test_mace_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_forces.py` & `physicsml-0.3.0/tests/rdkit/integration/training/mace/test_mace_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_mean_var.py` & `physicsml-0.3.0/tests/rdkit/integration/training/mace/test_mace_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_ssf_mace.py` & `physicsml-0.3.0/tests/rdkit/integration/training/mace/test_ssf_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_adapter_nequip.py` & `physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_adapter_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip.py` & `physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py` & `physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_forces.py` & `physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_nequip_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py` & `physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_ssf_nequip.py` & `physicsml-0.3.0/tests/rdkit/integration/training/nequip/test_ssf_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net.py` & `physicsml-0.3.0/tests/rdkit/integration/training/tensor_net/test_tensor_net.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py` & `physicsml-0.3.0/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py` & `physicsml-0.3.0/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py`

 * *Files identical despite different names*

