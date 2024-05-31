# Comparing `tmp/sunray-0.4.0-py3-none-any.whl.zip` & `tmp/sunray-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 21972 bytes, number of entries: 16
+Zip file size: 21974 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     2272 b- defN 80-Jan-01 00:00 sunray/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunray/_internal/__init__.py
 -rw-r--r--  2.0 unx    25396 b- defN 80-Jan-01 00:00 sunray/_internal/actor_mixin.py
 -rw-r--r--  2.0 unx    65315 b- defN 80-Jan-01 00:00 sunray/_internal/callable.py
--rw-r--r--  2.0 unx    15470 b- defN 80-Jan-01 00:00 sunray/_internal/core.py
+-rw-r--r--  2.0 unx    15545 b- defN 80-Jan-01 00:00 sunray/_internal/core.py
 -rw-r--r--  2.0 unx    10468 b- defN 80-Jan-01 00:00 sunray/_internal/dag.py
 -rw-r--r--  2.0 unx      658 b- defN 80-Jan-01 00:00 sunray/_internal/io.py
 -rw-r--r--  2.0 unx    11074 b- defN 80-Jan-01 00:00 sunray/_internal/remote.py
--rw-r--r--  2.0 unx    11288 b- defN 80-Jan-01 00:00 sunray/_internal/typing.py
+-rw-r--r--  2.0 unx    10715 b- defN 80-Jan-01 00:00 sunray/_internal/typing.py
 -rw-r--r--  2.0 unx      807 b- defN 80-Jan-01 00:00 sunray/_internal/util.py
 -rw-r--r--  2.0 unx      430 b- defN 80-Jan-01 00:00 sunray/dag.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunray/py.typed
--rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 sunray-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     8848 b- defN 80-Jan-01 00:00 sunray-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunray-0.4.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1249 b- defN 16-Jan-01 00:00 sunray-0.4.0.dist-info/RECORD
-16 files, 154431 bytes uncompressed, 19942 bytes compressed:  87.1%
+-rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 sunray-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8848 b- defN 80-Jan-01 00:00 sunray-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunray-0.4.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1249 b- defN 16-Jan-01 00:00 sunray-0.4.1.dist-info/RECORD
+16 files, 153933 bytes uncompressed, 19944 bytes compressed:  87.0%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sunray/dag.py
 Comment: 
 
 Filename: sunray/py.typed
 Comment: 
 
-Filename: sunray-0.4.0.dist-info/LICENSE
+Filename: sunray-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: sunray-0.4.0.dist-info/METADATA
+Filename: sunray-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: sunray-0.4.0.dist-info/WHEEL
+Filename: sunray-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: sunray-0.4.0.dist-info/RECORD
+Filename: sunray-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sunray/__init__.py

```diff
@@ -1,12 +1,12 @@
 # ruff: noqa: E402, F401
 from __future__ import annotations
 
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __authors__ = [
     "ZhengYu, Xu <zen-xu@outlook.com>",
 ]
 
 # re-exports from ray
 from ray._private.worker import LOCAL_MODE as LOCAL_MODE
 from ray._private.worker import RESTORE_WORKER_MODE as RESTORE_WORKER_MODE
```

## sunray/_internal/core.py

```diff
@@ -31,15 +31,15 @@
     from typing_extensions import Self
     from typing_extensions import TypedDict
     from typing_extensions import deprecated
 
     from .typing import RuntimeEnv
 
     _T = TypeVar("_T")
-    _R = TypeVar("_R")
+    _R_co = TypeVar("_R_co", covariant=True)
     _R0 = TypeVar("_R0")
     _R1 = TypeVar("_R1")
     _R2 = TypeVar("_R2")
     _R3 = TypeVar("_R3")
     _R4 = TypeVar("_R4")
     _R5 = TypeVar("_R5")
     _R6 = TypeVar("_R6")
@@ -109,33 +109,33 @@
 
     class NodeID(UniqueID): ...
 
     class WorkerID(UniqueID): ...
 
     class FunctionID(UniqueID): ...
 
-    class ObjectRef(_BaseID, ray.ObjectRef[_R]):
-        def as_future(self, _internal: bool = False) -> asyncio.Future[_R]: ...
-        def future(self) -> concurrent.futures.Future[_R]: ...
+    class ObjectRef(_BaseID, ray.ObjectRef[_R_co]):  # type: ignore[type-var]
+        def as_future(self, _internal: bool = False) -> asyncio.Future[_R_co]: ...
+        def future(self) -> concurrent.futures.Future[_R_co]: ...
         def job_id(self) -> JobID: ...
         def task_id(self) -> TaskID: ...
         def owner_address(self) -> bytes: ...
         def call_site(self) -> str: ...
         @classmethod
         def from_random(cls) -> Self: ...
         @classmethod
         def nil(cls) -> Self: ...
-        def __await__(self) -> Generator[None, None, _R]: ...
+        def __await__(self) -> Generator[None, None, _R_co]: ...
 
-    class ObjectRefGenerator(Generator[ObjectRef[_R], None, None]):
+    class ObjectRefGenerator(Generator[ObjectRef[_R_co], None, None]):
         def __aiter__(self) -> Self: ...
 
-        async def __anext__(self) -> ObjectRef[_R]: ...
+        async def __anext__(self) -> ObjectRef[_R_co]: ...
 
-        def completed(self) -> ObjectRef[_R]: ...
+        def completed(self) -> ObjectRef[_R_co]: ...
 
         def next_ready(self) -> bool: ...
 
         def is_finished(self) -> bool: ...
 
     def method(
         *,
@@ -424,15 +424,15 @@
 
     @overload
     def timeline(filename: None = None) -> list[ProfileEvent]: ...
 
     def timeline(filename=None) -> Any: ...
 
     def cancel(
-        ray_waitable: ObjectRef[_R] | ObjectRefGenerator[_R],
+        ray_waitable: ObjectRef[_R_co] | ObjectRefGenerator[_R_co],
         *,
         force: bool = False,
         recursive: bool = True,
     ) -> None: ...
 
     def get_gpu_ids() -> list[int] | list[str]: ...
```

## sunray/_internal/typing.py

```diff
@@ -1,206 +1,213 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
+from typing import Any
+from typing import Union
+
+from ray.util import scheduling_strategies
+from typing_extensions import Literal
+from typing_extensions import NotRequired
+from typing_extensions import Required
+from typing_extensions import TypedDict
 
 
 if TYPE_CHECKING:
     import types
 
-    from typing import Any
-    from typing import Union
-
     from ray import runtime_env
-    from ray.util import scheduling_strategies
-    from typing_extensions import Literal
-    from typing_extensions import NotRequired
-    from typing_extensions import Required
-    from typing_extensions import TypedDict
 
-    SchedulingStrategy = Union[
-        Literal["DEFAULT", "SPREAD"],
-        scheduling_strategies.PlacementGroupSchedulingStrategy,
-        scheduling_strategies.NodeAffinitySchedulingStrategy,
-        scheduling_strategies.NodeLabelSchedulingStrategy,
-        None,
-    ]
 
-    class ActorRemoteOptions(TypedDict, total=False):
-        num_cpus: float
-        num_gpus: float
-        resources: dict[str, float]
-        accelerator_type: str
-        memory: float
-        object_store_memory: float
-        max_restarts: int
-        max_task_retries: int
-        max_pending_calls: int
-        max_concurrency: int
-        name: str
-        namespace: str
-        lifetime: Literal["detached"] | None
-        runtime_env: RuntimeEnv | dict[str, Any]
-        concurrency_groups: dict[str, int]
-        scheduling_strategy: SchedulingStrategy
+SchedulingStrategy = Union[
+    Literal["DEFAULT", "SPREAD"],
+    scheduling_strategies.PlacementGroupSchedulingStrategy,
+    scheduling_strategies.NodeAffinitySchedulingStrategy,
+    scheduling_strategies.NodeLabelSchedulingStrategy,
+    None,
+]
+
+
+class ActorRemoteOptions(TypedDict, total=False):
+    num_cpus: float
+    num_gpus: float
+    resources: dict[str, float]
+    accelerator_type: str
+    memory: float
+    object_store_memory: float
+    max_restarts: int
+    max_task_retries: int
+    max_pending_calls: int
+    max_concurrency: int
+    name: str
+    namespace: str
+    lifetime: Literal["detached"] | None
+    runtime_env: RuntimeEnv | dict[str, Any]
+    concurrency_groups: dict[str, int]
+    scheduling_strategy: SchedulingStrategy
+
+
+class FunctionRemoteOptions(TypedDict, total=False):
+    num_cpus: float
+    num_gpus: float
+    resources: dict[str, float]
+    accelerator_type: str
+    memory: float
+    object_store_memory: float
+    max_calls: int
+    max_retries: int
+    runtime_env: RuntimeEnv | dict[str, Any]
+    retry_exceptions: list[type[Exception]]
+    scheduling_strategy: SchedulingStrategy
+
+
+class RayInitOpts(TypedDict, total=False):
+    labels: dict[str, str]
+    namespace: str
+    runtime_env: RuntimeEnv | dict[str, Any]
+
 
-    class FunctionRemoteOptions(TypedDict, total=False):
-        num_cpus: float
-        num_gpus: float
-        resources: dict[str, float]
-        accelerator_type: str
-        memory: float
-        object_store_memory: float
-        max_calls: int
-        max_retries: int
-        runtime_env: RuntimeEnv | dict[str, Any]
-        retry_exceptions: list[type[Exception]]
-        scheduling_strategy: SchedulingStrategy
+class RuntimeEnv(TypedDict, total=False):
+    working_dir: str
+    """
+    Specifies the working directory for the Ray workers. This must either be (1) an local existing directory with total size at most 100 MiB, (2) a local existing zipped file with total unzipped size at most 100 MiB (Note: ``excludes`` has no effect), or (3) a URI to a remotely-stored zip file containing the working directory for your job (no file size limit is enforced by Ray). See :ref:`remote-uris` for details.
+    The specified directory will be downloaded to each node on the cluster, and Ray workers will be started in their node's copy of this directory.
 
-    class RayInitOpts(TypedDict, total=False):
-        labels: dict[str, str]
-        namespace: str
-        runtime_env: RuntimeEnv | dict[str, Any]
+    - Examples
 
-    class RuntimeEnv(TypedDict, total=False):
-        working_dir: str
-        """
-        Specifies the working directory for the Ray workers. This must either be (1) an local existing directory with total size at most 100 MiB, (2) a local existing zipped file with total unzipped size at most 100 MiB (Note: ``excludes`` has no effect), or (3) a URI to a remotely-stored zip file containing the working directory for your job (no file size limit is enforced by Ray). See :ref:`remote-uris` for details.
-        The specified directory will be downloaded to each node on the cluster, and Ray workers will be started in their node's copy of this directory.
+        - ``"."  # cwd``
 
-        - Examples
+        - ``"/src/my_project"``
 
-            - ``"."  # cwd``
+        - ``"/src/my_project.zip"``
 
-            - ``"/src/my_project"``
+        - ``"s3://path/to/my_dir.zip"``
 
-            - ``"/src/my_project.zip"``
+    Note: Setting a local directory per-task or per-actor is currently unsupported; it can only be set per-job (i.e., in ``ray.init()``).
 
-            - ``"s3://path/to/my_dir.zip"``
+    Note: If the local directory contains a ``.gitignore`` file, the files and paths specified there are not uploaded to the cluster.  You can disable this by setting the environment variable `RAY_RUNTIME_ENV_IGNORE_GITIGNORE=1` on the machine doing the uploading.
+    """
 
-        Note: Setting a local directory per-task or per-actor is currently unsupported; it can only be set per-job (i.e., in ``ray.init()``).
+    py_modules: list[str | types.ModuleType]
+    """
+    Specifies Python modules to be available for import in the Ray workers.  (For more ways to specify packages, see also the ``pip`` and ``conda`` fields below.)
+    Each entry must be either (1) a path to a local directory, (2) a URI to a remote zip or wheel file (see :ref:`remote-uris` for details), (3) a Python module object, or (4) a path to a local `.whl` file.
 
-        Note: If the local directory contains a ``.gitignore`` file, the files and paths specified there are not uploaded to the cluster.  You can disable this by setting the environment variable `RAY_RUNTIME_ENV_IGNORE_GITIGNORE=1` on the machine doing the uploading.
-        """
+    - Examples of entries in the list:
 
-        py_modules: list[str | types.ModuleType]
-        """
-        Specifies Python modules to be available for import in the Ray workers.  (For more ways to specify packages, see also the ``pip`` and ``conda`` fields below.)
-        Each entry must be either (1) a path to a local directory, (2) a URI to a remote zip or wheel file (see :ref:`remote-uris` for details), (3) a Python module object, or (4) a path to a local `.whl` file.
+        - ``"."``
 
-        - Examples of entries in the list:
+        - ``"/local_dependency/my_module"``
 
-            - ``"."``
+        - ``"s3://bucket/my_module.zip"``
 
-            - ``"/local_dependency/my_module"``
+        - ``my_module # Assumes my_module has already been imported, e.g. via 'import my_module'``
 
-            - ``"s3://bucket/my_module.zip"``
+        - ``my_module.whl``
 
-            - ``my_module # Assumes my_module has already been imported, e.g. via 'import my_module'``
+        - ``"s3://bucket/my_module.whl"``
 
-            - ``my_module.whl``
+    The modules will be downloaded to each node on the cluster.
 
-            - ``"s3://bucket/my_module.whl"``
+    Note: Setting options (1), (3) and (4) per-task or per-actor is currently unsupported, it can only be set per-job (i.e., in ``ray.init()``).
 
-        The modules will be downloaded to each node on the cluster.
+    Note: For option (1), if the local directory contains a ``.gitignore`` file, the files and paths specified there are not uploaded to the cluster.  You can disable this by setting the environment variable `RAY_RUNTIME_ENV_IGNORE_GITIGNORE=1` on the machine doing the uploading.
 
-        Note: Setting options (1), (3) and (4) per-task or per-actor is currently unsupported, it can only be set per-job (i.e., in ``ray.init()``).
+    Note: This feature is currently limited to modules that are packages with a single directory containing an ``__init__.py`` file.  For single-file modules, you may use ``working_dir``.
+    """
 
-        Note: For option (1), if the local directory contains a ``.gitignore`` file, the files and paths specified there are not uploaded to the cluster.  You can disable this by setting the environment variable `RAY_RUNTIME_ENV_IGNORE_GITIGNORE=1` on the machine doing the uploading.
+    excludes: list[str]
+    """
+    When used with ``working_dir`` or ``py_modules``, specifies a list of files or paths to exclude from being uploaded to the cluster.
 
-        Note: This feature is currently limited to modules that are packages with a single directory containing an ``__init__.py`` file.  For single-file modules, you may use ``working_dir``.
-        """
+    This field uses the pattern-matching syntax used by ``.gitignore`` files: see `<https://git-scm.com/docs/gitignore>`_ for details.
 
-        excludes: list[str]
-        """
-        When used with ``working_dir`` or ``py_modules``, specifies a list of files or paths to exclude from being uploaded to the cluster.
+    Note: In accordance with ``.gitignore`` syntax, if there is a separator (``/``) at the beginning or middle (or both) of the pattern, then the pattern is interpreted relative to the level of the ``working_dir``.
 
-        This field uses the pattern-matching syntax used by ``.gitignore`` files: see `<https://git-scm.com/docs/gitignore>`_ for details.
+    In particular, you shouldn't use absolute paths (e.g. `/Users/my_working_dir/subdir/`) with `excludes`; rather, you should use the relative path `/subdir/` (written here with a leading `/` to match only the top-level `subdir` directory, rather than all directories named `subdir` at all levels.)
 
-        Note: In accordance with ``.gitignore`` syntax, if there is a separator (``/``) at the beginning or middle (or both) of the pattern, then the pattern is interpreted relative to the level of the ``working_dir``.
+    - Example: ``{"working_dir": "/Users/my_working_dir/", "excludes": ["my_file.txt", "/subdir/, "path/to/dir", "*.log"]}``
+    """
 
-        In particular, you shouldn't use absolute paths (e.g. `/Users/my_working_dir/subdir/`) with `excludes`; rather, you should use the relative path `/subdir/` (written here with a leading `/` to match only the top-level `subdir` directory, rather than all directories named `subdir` at all levels.)
+    pip: list[str] | str | PipConf
+    """
+    Either (1) a list of pip `requirements specifiers <https://pip.pypa.io/en/stable/cli/pip_install/#requirement-specifiers>`_, (2) a string containing the path to a local pip
+    `“requirements.txt” <https://pip.pypa.io/en/stable/user_guide/#requirements-files>`_ file, or (3) a python dictionary that has three fields: (a) ``packages`` (required, List[str]): a list of pip packages,
+    (b) ``pip_check`` (optional, bool): whether to enable `pip check <https://pip.pypa.io/en/stable/cli/pip_check/>`_ at the end of pip install, defaults to ``False``.
+    (c) ``pip_version`` (optional, str): the version of pip; Ray will spell the package name "pip" in front of the ``pip_version`` to form the final requirement string.
+    The syntax of a requirement specifier is defined in full in `PEP 508 <https://www.python.org/dev/peps/pep-0508/>`_.
+    This will be installed in the Ray workers at runtime.  Packages in the preinstalled cluster environment will still be available.
+    To use a library like Ray Serve or Ray Tune, you will need to include ``"ray[serve]"`` or ``"ray[tune]"`` here.
+    The Ray version must match that of the cluster.
 
-        - Example: ``{"working_dir": "/Users/my_working_dir/", "excludes": ["my_file.txt", "/subdir/, "path/to/dir", "*.log"]}``
-        """
+    - Example: ``["requests==1.0.0", "aiohttp", "ray[serve]"]``
 
-        pip: list[str] | str | PipConf
-        """
-        Either (1) a list of pip `requirements specifiers <https://pip.pypa.io/en/stable/cli/pip_install/#requirement-specifiers>`_, (2) a string containing the path to a local pip
-        `“requirements.txt” <https://pip.pypa.io/en/stable/user_guide/#requirements-files>`_ file, or (3) a python dictionary that has three fields: (a) ``packages`` (required, List[str]): a list of pip packages,
-        (b) ``pip_check`` (optional, bool): whether to enable `pip check <https://pip.pypa.io/en/stable/cli/pip_check/>`_ at the end of pip install, defaults to ``False``.
-        (c) ``pip_version`` (optional, str): the version of pip; Ray will spell the package name "pip" in front of the ``pip_version`` to form the final requirement string.
-        The syntax of a requirement specifier is defined in full in `PEP 508 <https://www.python.org/dev/peps/pep-0508/>`_.
-        This will be installed in the Ray workers at runtime.  Packages in the preinstalled cluster environment will still be available.
-        To use a library like Ray Serve or Ray Tune, you will need to include ``"ray[serve]"`` or ``"ray[tune]"`` here.
-        The Ray version must match that of the cluster.
+    - Example: ``"./requirements.txt"``
 
-        - Example: ``["requests==1.0.0", "aiohttp", "ray[serve]"]``
+    - Example: ``{"packages":["tensorflow", "requests"], "pip_check": False, "pip_version": "==22.0.2;python_version=='3.8.11'"}``
 
-        - Example: ``"./requirements.txt"``
+    When specifying a path to a ``requirements.txt`` file, the file must be present on your local machine and it must be a valid absolute path or relative filepath relative to your local current working directory, *not* relative to the `working_dir` specified in the `runtime_env`.
+    Furthermore, referencing local files `within` a `requirements.txt` file is not supported (e.g., ``-r ./my-laptop/more-requirements.txt``, ``./my-pkg.whl``).
+    """
 
-        - Example: ``{"packages":["tensorflow", "requests"], "pip_check": False, "pip_version": "==22.0.2;python_version=='3.8.11'"}``
+    conda: str | dict
+    """
+    Either (1) a dict representing the conda environment YAML, (2) a string containing the path to a local
+    `conda “environment.yml” <https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#create-env-file-manually>`_ file,
+    or (3) the name of a local conda environment already installed on each node in your cluster (e.g., ``"pytorch_p36"``).
+    In the first two cases, the Ray and Python dependencies will be automatically injected into the environment to ensure compatibility, so there is no need to manually include them.
+    The Python and Ray version must match that of the cluster, so you likely should not specify them manually.
+    Note that the ``conda`` and ``pip`` keys of ``runtime_env`` cannot both be specified at the same time---to use them together, please use ``conda`` and add your pip dependencies in the ``"pip"`` field in your conda ``environment.yaml``.
 
-        When specifying a path to a ``requirements.txt`` file, the file must be present on your local machine and it must be a valid absolute path or relative filepath relative to your local current working directory, *not* relative to the `working_dir` specified in the `runtime_env`.
-        Furthermore, referencing local files `within` a `requirements.txt` file is not supported (e.g., ``-r ./my-laptop/more-requirements.txt``, ``./my-pkg.whl``).
-        """
+    - Example: ``{"dependencies": ["pytorch", "torchvision", "pip", {"pip": ["pendulum"]}]}``
 
-        conda: str | dict
-        """
-        Either (1) a dict representing the conda environment YAML, (2) a string containing the path to a local
-        `conda “environment.yml” <https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#create-env-file-manually>`_ file,
-        or (3) the name of a local conda environment already installed on each node in your cluster (e.g., ``"pytorch_p36"``).
-        In the first two cases, the Ray and Python dependencies will be automatically injected into the environment to ensure compatibility, so there is no need to manually include them.
-        The Python and Ray version must match that of the cluster, so you likely should not specify them manually.
-        Note that the ``conda`` and ``pip`` keys of ``runtime_env`` cannot both be specified at the same time---to use them together, please use ``conda`` and add your pip dependencies in the ``"pip"`` field in your conda ``environment.yaml``.
+    - Example: ``"./environment.yml"``
 
-        - Example: ``{"dependencies": ["pytorch", "torchvision", "pip", {"pip": ["pendulum"]}]}``
+    - Example: ``"pytorch_p36"``
 
-        - Example: ``"./environment.yml"``
+    When specifying a path to a ``environment.yml`` file, the file must be present on your local machine and it must be a valid absolute path or a relative filepath relative to your local current working directory, *not* relative to the `working_dir` specified in the `runtime_env`.
+    Furthermore, referencing local files `within` a `environment.yml` file is not supported.
+    """
 
-        - Example: ``"pytorch_p36"``
+    env_vars: dict[str, str]
+    """
+    Environment variables to set.  Environment variables already set on the cluster will still be visible to the Ray workers; so there is
+    no need to include ``os.environ`` or similar in the ``env_vars`` field.
+    By default, these environment variables override the same name environment variables on the cluster.
+    You can also reference existing environment variables using ${ENV_VAR} to achieve the appending behavior.
+    If the environment variable doesn't exist, it becomes an empty string `""`.
 
-        When specifying a path to a ``environment.yml`` file, the file must be present on your local machine and it must be a valid absolute path or a relative filepath relative to your local current working directory, *not* relative to the `working_dir` specified in the `runtime_env`.
-        Furthermore, referencing local files `within` a `environment.yml` file is not supported.
-        """
+    - Example: ``{"OMP_NUM_THREADS": "32", "TF_WARNINGS": "none"}``
 
-        env_vars: dict[str, str]
-        """
-        Environment variables to set.  Environment variables already set on the cluster will still be visible to the Ray workers; so there is
-        no need to include ``os.environ`` or similar in the ``env_vars`` field.
-        By default, these environment variables override the same name environment variables on the cluster.
-        You can also reference existing environment variables using ${ENV_VAR} to achieve the appending behavior.
-        If the environment variable doesn't exist, it becomes an empty string `""`.
+    - Example: ``{"LD_LIBRARY_PATH": "${LD_LIBRARY_PATH}:/home/admin/my_lib"}``
 
-        - Example: ``{"OMP_NUM_THREADS": "32", "TF_WARNINGS": "none"}``
+    - Non-existent variable example: ``{"ENV_VAR_NOT_EXIST": "${ENV_VAR_NOT_EXIST}:/home/admin/my_lib"}`` -> ``ENV_VAR_NOT_EXIST=":/home/admin/my_lib"``.
+    """
 
-        - Example: ``{"LD_LIBRARY_PATH": "${LD_LIBRARY_PATH}:/home/admin/my_lib"}``
+    config: RuntimeEnvConfig | runtime_env.RuntimeEnvConfig
+    """
+    - ``config`` (dict | :class:`ray.runtime_env.RuntimeEnvConfig <ray.runtime_env.RuntimeEnvConfig>`): config for runtime environment. Either a dict or a RuntimeEnvConfig.
+    Fields:
+    (1) setup_timeout_seconds, the timeout of runtime environment creation, timeout is in seconds.
 
-        - Non-existent variable example: ``{"ENV_VAR_NOT_EXIST": "${ENV_VAR_NOT_EXIST}:/home/admin/my_lib"}`` -> ``ENV_VAR_NOT_EXIST=":/home/admin/my_lib"``.
-        """
+    - Example: ``{"setup_timeout_seconds": 10}``
 
-        config: RuntimeEnvConfig | runtime_env.RuntimeEnvConfig
-        """
-        - ``config`` (dict | :class:`ray.runtime_env.RuntimeEnvConfig <ray.runtime_env.RuntimeEnvConfig>`): config for runtime environment. Either a dict or a RuntimeEnvConfig.
-        Fields:
-        (1) setup_timeout_seconds, the timeout of runtime environment creation, timeout is in seconds.
+    - Example: ``RuntimeEnvConfig(setup_timeout_seconds=10)``
 
-        - Example: ``{"setup_timeout_seconds": 10}``
+    (2) ``eager_install`` (bool): Indicates whether to install the runtime environment on the cluster at ``ray.init()`` time, before the workers are leased. This flag is set to ``True`` by default.
+    If set to ``False``, the runtime environment will be only installed when the first task is invoked or when the first actor is created.
+    Currently, specifying this option per-actor or per-task is not supported.
 
-        - Example: ``RuntimeEnvConfig(setup_timeout_seconds=10)``
+    - Example: ``{"eager_install": False}``
 
-        (2) ``eager_install`` (bool): Indicates whether to install the runtime environment on the cluster at ``ray.init()`` time, before the workers are leased. This flag is set to ``True`` by default.
-        If set to ``False``, the runtime environment will be only installed when the first task is invoked or when the first actor is created.
-        Currently, specifying this option per-actor or per-task is not supported.
+    - Example: ``RuntimeEnvConfig(eager_install=False)``
+    """
 
-        - Example: ``{"eager_install": False}``
 
-        - Example: ``RuntimeEnvConfig(eager_install=False)``
-        """
+class PipConf(TypedDict):
+    packages: Required[list[str]]
+    pip_check: NotRequired[bool]
+    pip_version: NotRequired[str]
 
-    class PipConf(TypedDict):
-        packages: Required[list[str]]
-        pip_check: NotRequired[bool]
-        pip_version: NotRequired[str]
 
-    class RuntimeEnvConfig(TypedDict, total=False):
-        setup_timeout_seconds: int
-        eager_install: bool
+class RuntimeEnvConfig(TypedDict, total=False):
+    setup_timeout_seconds: int
+    eager_install: bool
```

## Comparing `sunray-0.4.0.dist-info/LICENSE` & `sunray-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sunray-0.4.0.dist-info/METADATA` & `sunray-0.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunray
-Version: 0.4.0
+Version: 0.4.1
 Summary: More robust ray
 Author: ZhengYu, Xu
 Author-email: zen-xu@outlook.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `sunray-0.4.0.dist-info/RECORD` & `sunray-0.4.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-sunray/__init__.py,sha256=x7mVNvepo-qKpPv_yIU3Rt0akRC46f1xiEESdGvO_Gc,2272
+sunray/__init__.py,sha256=vuzcuAn-lXkmjcOr2o420KioET254LUri5DqiG_X25E,2272
 sunray/_internal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sunray/_internal/actor_mixin.py,sha256=zhtKOKSdrMURT2cTf3Bq-WqVyrpiemSVt5uAToZxNBI,25396
 sunray/_internal/callable.py,sha256=eVi_mmJjOsZzVwqaP1DTfWBDF3nRMXhacBC6yT_fPpM,65315
-sunray/_internal/core.py,sha256=fNLDsu8wuTrPx94ZP5ezdF8Ocf13Q4BSBjIegSNyI5E,15470
+sunray/_internal/core.py,sha256=2TJWaa9ubLuczOEp8eaaBGKwCVYv8Osi0rrN2EsH-5k,15545
 sunray/_internal/dag.py,sha256=B3g-Z0zVGfv7zWj2jO7eTrYsHdvzdxSel54UF_IeKU0,10468
 sunray/_internal/io.py,sha256=44YKqLW-oeKI8ehhGtc8ZhJ2yk4jx2Zrfh4pa3trNPs,658
 sunray/_internal/remote.py,sha256=Qsrql1NiiW26E_O6euuZ3U-E_RY_vz-6uqY6KdObsok,11074
-sunray/_internal/typing.py,sha256=brz_CAx45m8-28JTTqpT-5OKT3OU0N53KwF8-CyoS44,11288
+sunray/_internal/typing.py,sha256=3CU0vOuIsY3iOsdiEfPQ2aFcM1Gla2FidDHGO7aPy94,10715
 sunray/_internal/util.py,sha256=WQ6WLD_b2uY1d_6nyf24R7SbP1nqZ1CmUnzS5NMaiLA,807
 sunray/dag.py,sha256=ydCtgNVf_E2K0AFABzRhPkvlLPPUq6HQLR7QXswODJM,430
 sunray/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sunray-0.4.0.dist-info/LICENSE,sha256=4ix-bYe2BfMr6RchyTiQ2g18h5fXPTdVrjB6LLsxoaQ,1068
-sunray-0.4.0.dist-info/METADATA,sha256=AfkHFc_A9sD3mQoAuSec2tGKIhAqMgVulRPSADZr07M,8848
-sunray-0.4.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-sunray-0.4.0.dist-info/RECORD,,
+sunray-0.4.1.dist-info/LICENSE,sha256=4ix-bYe2BfMr6RchyTiQ2g18h5fXPTdVrjB6LLsxoaQ,1068
+sunray-0.4.1.dist-info/METADATA,sha256=T3srQIxm1wpApqgixek5si00jJm9Jx7a2RuInlVL8II,8848
+sunray-0.4.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+sunray-0.4.1.dist-info/RECORD,,
```

