# Comparing `tmp/janus_core-0.4.0b0.tar.gz` & `tmp/janus_core-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_core-0.4.0b0.tar", max compression
+gzip compressed data, was "janus_core-0.5.0b0.tar", max compression
```

## Comparing `janus_core-0.4.0b0.tar` & `janus_core-0.5.0b0.tar`

### file list

```diff
@@ -1,21 +1,27 @@
--rw-r--r--   0        0        0     1533 2024-05-13 13:13:50.085032 janus_core-0.4.0b0/LICENSE
--rw-r--r--   0        0        0     9907 2024-05-13 13:13:50.085032 janus_core-0.4.0b0/README.md
--rw-r--r--   0        0        0      132 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/__init__.py
--rw-r--r--   0        0        0     4814 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/calculations/geom_opt.py
--rw-r--r--   0        0        0    36040 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/calculations/md.py
--rw-r--r--   0        0        0    12143 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/calculations/single_point.py
--rw-r--r--   0        0        0     6958 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/geomopt.py
--rw-r--r--   0        0        0     1000 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/janus.py
--rw-r--r--   0        0        0    13636 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/md.py
--rw-r--r--   0        0        0     5203 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/singlepoint.py
--rw-r--r--   0        0        0     1701 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/train.py
--rw-r--r--   0        0        0     3481 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/types.py
--rw-r--r--   0        0        0     3274 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/utils.py
--rw-r--r--   0        0        0     1686 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/janus_types.py
--rw-r--r--   0        0        0     4053 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/log.py
--rw-r--r--   0        0        0     3532 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/mlip_calculators.py
--rw-r--r--   0        0        0     5838 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/stats.py
--rw-r--r--   0        0        0     2272 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/train.py
--rw-r--r--   0        0        0     1544 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/utils.py
--rw-r--r--   0        0        0     2558 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/pyproject.toml
--rw-r--r--   0        0        0    10966 1970-01-01 00:00:00.000000 janus_core-0.4.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/LICENSE
+-rw-r--r--   0        0        0    14066 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/README.md
+-rw-r--r--   0        0        0      132 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/__init__.py
+-rw-r--r--   0        0        0     6913 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/calculations/eos.py
+-rw-r--r--   0        0        0     7339 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/calculations/geom_opt.py
+-rw-r--r--   0        0        0    35666 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/calculations/md.py
+-rw-r--r--   0        0        0    18631 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/calculations/phonons.py
+-rw-r--r--   0        0        0    12424 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/calculations/single_point.py
+-rw-r--r--   0        0        0     5030 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/descriptors.py
+-rw-r--r--   0        0        0     6289 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/eos.py
+-rw-r--r--   0        0        0     7107 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/geomopt.py
+-rw-r--r--   0        0        0     1199 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/janus.py
+-rw-r--r--   0        0        0    13468 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/md.py
+-rw-r--r--   0        0        0     9223 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/phonons.py
+-rw-r--r--   0        0        0     4583 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/singlepoint.py
+-rw-r--r--   0        0        0     1701 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/train.py
+-rw-r--r--   0        0        0     3481 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/types.py
+-rw-r--r--   0        0        0     5035 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/cli/utils.py
+-rw-r--r--   0        0        0     4647 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/helpers/descriptors.py
+-rw-r--r--   0        0        0     2079 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/helpers/janus_types.py
+-rw-r--r--   0        0        0     4081 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/helpers/log.py
+-rw-r--r--   0        0        0     3740 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/helpers/mlip_calculators.py
+-rw-r--r--   0        0        0     5838 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/helpers/stats.py
+-rw-r--r--   0        0        0     2272 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/helpers/train.py
+-rw-r--r--   0        0        0     6576 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/janus_core/helpers/utils.py
+-rw-r--r--   0        0        0     2620 2024-05-31 05:07:12.222686 janus_core-0.5.0b0/pyproject.toml
+-rw-r--r--   0        0        0    15246 1970-01-01 00:00:00.000000 janus_core-0.5.0b0/PKG-INFO
```

### Comparing `janus_core-0.4.0b0/LICENSE` & `janus_core-0.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_core-0.4.0b0/README.md` & `janus_core-0.5.0b0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: janus-core
+Version: 0.5.0b0
+Summary: Tools for machine learnt interatomic potentials
+Home-page: https://github.com/stfc/janus-core/
+Author: Elliott Kasoar
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ase (>=3.22.1,<4.0.0)
+Requires-Dist: mace-torch (>=0.3.4,<0.4.0)
+Requires-Dist: phonopy (>=2.23.1,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: seekpath (>=2.1.0,<3.0.0)
+Requires-Dist: spglib (>=2.3.0,<3.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer-config (>=1.4.0,<2.0.0)
+Project-URL: Documentation, https://stfc.github.io/janus-core/
+Project-URL: Repository, https://github.com/stfc/janus-core/
+Description-Content-Type: text/markdown
+
 [![Build Status][ci-badge]][ci-link]
 [![Coverage Status][cov-badge]][cov-link]
 [![Docs status][docs-badge]][docs-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![License][license-badge]][license-link]
 [![DOI][doi-badge]][doi-link]
 
@@ -20,16 +49,17 @@
 - [x] Single point calculations
 - [x] Geometry optimisation
 - [x] Molecular Dynamics
   - NVE
   - NVT (Langevin(Eijnden/Ciccotti flavour) and Nosé-Hoover (Melchionna flavour))
   - NPT (Nosé-Hoover (Melchiona flavour))
 - [ ] Nudge Elastic Band
-- [ ] Phonons
-  - vibroscopy
+- [x] Phonons
+  - Phonopy
+- [x] Equation of State
 - [x] Training ML potentials
   - MACE
 - [x] Fine tunning MLIPs
   - MACE
 - [ ] Rare events simulations
   - PLUMED
 
@@ -77,15 +107,22 @@
 
 ```shell
 janus singlepoint --struct tests/data/NaCl.cif --arch mace --calc-kwargs "{'model' : '/path/to/your/ml.model'}" --properties energy --properties forces --log ./example.log --out ./example.xyz
 ```
 
 This calculates both forces and energies, defines the MLIP architecture and path to your locally saved model, and changes where the log and results files are saved.
 
-Note: the MACE calculator currently returns energy, forces and stress together, so in this case the choice of property will not change the output.
+> [!NOTE]
+> The MACE calculator currently returns energy, forces and stress together, so in this case the choice of property will not change the output.
+
+By default, all structures in a trajectory file will be read, but specific structures can be selected using --read-kwargs:
+
+```shell
+janus singlepoint --struct tests/data/benzene-traj.xyz --read-kwargs "{'index': 0}"
+```
 
 For all options, run `janus singlepoint --help`.
 
 
 ### Geometry optimization
 
 Perform geometry optimization (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
@@ -166,14 +203,67 @@
 janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10 --steps 1000 --temp 300
 ```
 
 This performs the same initial heating, before running a further 1000 steps (1 ps) at 300K.
 
 When MD is run with heating the trajectory ```NaCl-nvt-T20.0-T300.0-T300.0-traj.xyz``` and statistics ```NaCl-nvt-T20.0-T300.0-T300.0-stats.dat``` files will indicate the heating range and MD temperature (which may be different). With heating and MD trajectories/statistics within the same files.
 
+Additional settings for geometry optimization, such as enabling optimization of cell vectors by setting `hydrostatic_strain = True` for the ASE filter, can be set using the `--minimize-kwargs` option:
+
+```shell
+janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 0 --temp-end 300 --temp-step 10 --temp-time 10 --minimize --minimize-kwargs "{'filter_kwargs': {'hydrostatic_strain' : True}}"
+```
+
+### Equation of State
+
+Fit the equation of state for a structure (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
+
+```shell
+janus eos --struct tests/data/NaCl.cif --no-minimize --min-volume 0.9 --max-volume 1.1 --n-volumes 9 --arch mace_mp --calc-kwargs "{'model' : 'small'}"
+```
+
+This will save the energies and volumes for nine lattice constants in `NaCl-eos-raw.dat`, and the fitted minimum energy, volume, and bulk modulus in `NaCl-eos-fit.dat`, in addition to generating a log file, `eos.log`, and summary of inputs, `eos_summary.yml`.
+
+By default, geometry optimization will be performed on the initial structure, before calculations are performed for the range of lattice constants consistent with minimum and maximum volumes supplied. Optimization at constant volume for all generated structures can also be performed (sharing the same maximum force convergence):
+
+```shell
+janus eos --struct tests/data/NaCl.cif --minimize-all --fmax 0.0001
+```
+
+For all options, run `janus eos --help`.
+
+
+### Phonons
+
+Calculate phonons with a 2x2x2 supercell, after geometry optimization (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
+
+```shell
+janus phonons --struct tests/data/NaCl.cif --supercell 2x2x2 --minimize --arch mace_mp --calc-kwargs "{'model' : 'small'}"
+```
+
+This will save the Phonopy parameters, including displacements and force constants, to `NaCl-phonopy.yml` and `NaCl-force_constants.hdf5`, in addition to generating a log file, `phonons.log`, and summary of inputs, `phonons_summary.yml`.
+
+Additionally, the `--band` option can be added to calculate the band structure and save the results to `NaCl-auto_bands.yml`:
+
+```shell
+janus phonons --struct tests/data/NaCl.cif --supercell 2x2x2 --minimize --arch mace_mp --calc-kwargs "{'model' : 'small'}" --band
+```
+
+If you need eigenvectors and group velocities written, add the `--write-full` option. This will generate a much larger file, but can be used to visualise phonon modes.
+
+Further calculations, including thermal properties, DOS, and PDOS, can also be calculated (using a 2x3x4 supercell):
+
+```shell
+janus phonons --struct tests/data/NaCl.cif --supercell 2x3x4 --dos --pdos --thermal --temp-start 0 --temp-end 300 --temp-step 50
+```
+
+This will create additional output files: `NaCl-thermal.dat` for the thermal properties (heat capacity, entropy, and free energy) between 0K and 300K, `NaCl-dos.dat` for the DOS, and `NaCl-pdos.dat` for the PDOS.
+
+For all options, run `janus phonons --help`.
+
 
 ### Using configuration files
 
 Default values for all command line options may be specifed through a Yaml 1.1 formatted configuration file by adding the `--config` option. If an option is present in both the command line and configuration file, the command line value takes precedence.
 
 For example, with the following configuration file and command:
 
@@ -214,14 +304,35 @@
 
 Foundational models can also be fine-tuned, by including the `foundation_model` option in your configuration file, and using `--fine-tune` option:
 
 ```shell
 janus train --mlip-config /path/to/fine/tuning/config.yml --fine-tune
 ```
 
+
+### Calculate MACE descriptors
+
+MACE descriptors can be calculated for structures (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
+
+```shell
+janus descriptors --struct tests/data/NaCl.cif --arch mace_mp --calc-kwargs "{'model' : 'small'}"
+```
+
+This will calculate the mean descriptor for this structure and save this as attached information (`descriptors`) in `NaCl-descriptors.xyz`, in addition to generating a log file, `descriptors.log`, and summary of inputs, `descriptors_summary.yml`.
+
+The mean descriptor per element can also be calculated, and all descriptors, rather than only the invariant part, can be used when calculating the means:
+
+```shell
+janus descriptors --struct tests/data/NaCl.cif --no-invariants-only --calc-per-element
+```
+
+This will generate the same output files, but additional labels (`Cl_descriptor` and `Na_descriptor`) will be saved in `NaCl-descriptors.xyz`.
+
+For all options, run `janus descriptors --help`.
+
 ## License
 
 [BSD 3-Clause License](LICENSE)
 
 ## Funding
 
 Contributors to this project were funded by
@@ -240,7 +351,8 @@
 [pypi-badge]: https://badge.fury.io/py/janus-core.svg
 [pypi-link]: https://badge.fury.io/py/janus-core
 [license-badge]: https://img.shields.io/badge/License-BSD_3--Clause-blue.svg
 [license-link]: https://opensource.org/licenses/BSD-3-Clause
 [doi-link]: https://zenodo.org/badge/latestdoi/754081470
 [doi-badge]: https://zenodo.org/badge/754081470.svg
 [logo]: https://raw.githubusercontent.com/stfc/janus-core/main/docs/source/images/janus-core-100.png
+
```

### Comparing `janus_core-0.4.0b0/janus_core/calculations/md.py` & `janus_core-0.5.0b0/janus_core/calculations/md.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 )
 from ase.md.verlet import VelocityVerlet
 import numpy as np
 
 from janus_core.calculations.geom_opt import optimize
 from janus_core.helpers.janus_types import Ensembles, PathLike
 from janus_core.helpers.log import config_logger
+from janus_core.helpers.utils import FileNameMixin
 
 DENS_FACT = (units.m / 1.0e2) ** 3 / units.mol
 
 
-class MolecularDynamics:  # pylint: disable=too-many-instance-attributes
+class MolecularDynamics(FileNameMixin):  # pylint: disable=too-many-instance-attributes
     """
     Configure shared molecular dynamics simulation options.
 
     Parameters
     ----------
     struct : Atoms
         Structure to simulate.
@@ -162,15 +163,15 @@
         """
         Initialise molecular dynamics simulation configuration.
 
         Parameters
         ----------
         struct : Atoms
             Structure to simulate.
-        struct_name : str
+        struct_name : Optional[str]
             Name of structure to simulate. Default is inferred from filepath or
             chemical formula.
         ensemble : Ensembles
             Name for thermodynamic ensemble. Default is None.
         steps : int
             Number of steps in simulation. Default is 0.
         timestep : float
@@ -233,25 +234,23 @@
         log_kwargs : Optional[dict[str, Any]]
             Keyword arguments to pass to log config. Default is None.
         seed : Optional[int]
             Random seed used by numpy.random and random functions, such as in Langevin.
             Default is None.
         """
         self.struct = struct
-        self.struct_name = struct_name
         self.timestep = timestep * units.fs
         self.steps = steps
         self.temp = temp
         self.equil_steps = equil_steps
         self.minimize = minimize
         self.minimize_every = minimize_every
         self.rescale_velocities = rescale_velocities
         self.remove_rot = remove_rot
         self.rescale_every = rescale_every
-        self.file_prefix = file_prefix
         self.restart = restart
         self.restart_stem = restart_stem
         self.restart_every = restart_every
         self.rotate_restart = rotate_restart
         self.restarts_to_keep = restarts_to_keep
         self.stats_file = stats_file
         self.stats_every = stats_every
@@ -263,14 +262,16 @@
         self.temp_end = temp_end
         self.temp_step = temp_step
         self.temp_time = temp_time * units.fs if temp_time else None
         self.log_kwargs = log_kwargs
         self.ensemble = ensemble
         self.seed = seed
 
+        FileNameMixin.__init__(self, struct, struct_name, file_prefix, ensemble)
+
         self.log_kwargs = (
             log_kwargs if log_kwargs else {}
         )  # pylint: disable=duplicate-code
         if self.log_kwargs and "filename" not in self.log_kwargs:
             raise ValueError("'filename' must be included in `log_kwargs`")
 
         self.log_kwargs.setdefault("name", __name__)
@@ -313,19 +314,24 @@
             raise ValueError("Start and end temperatures must be positive")
 
         self.minimize_kwargs = minimize_kwargs if minimize_kwargs else {}
         self.restart_files = []
         self.dyn = None
         self.n_atoms = len(self.struct)
 
-        # Infer names for structure and if not specified
-        if not self.struct_name:
-            self.struct_name = self.struct.get_chemical_formula()
-
-        self.configure_filenames()
+        self.stats_file = self._build_filename(
+            "stats.dat",
+            self._parameter_prefix if file_prefix is None else "",
+            filename=self.stats_file,
+        )
+        self.traj_file = self._build_filename(
+            "traj.xyz",
+            self._parameter_prefix if file_prefix is None else "",
+            filename=self.traj_file,
+        )
 
         self.offset = 0
 
         if "masses" not in self.struct.arrays.keys():
             self.struct.set_masses()
 
         if self.seed:
@@ -384,68 +390,50 @@
         -------
         str
            Formatted temperature range if heating and target temp if running md.
         """
 
         temperature_prefix = ""
         if self.temp_start is not None and self.temp_end is not None:
-            temperature_prefix = f"-T{self.temp_start}-T{self.temp_end}"
+            temperature_prefix += f"-T{self.temp_start}-T{self.temp_end}"
 
         if self.steps > 0:
             temperature_prefix += f"-T{self.temp}"
 
-        return temperature_prefix
+        return temperature_prefix.lstrip("-")
 
     @property
     def _final_file(self) -> str:
         """
         Final state file name.
 
         Returns
         -------
         str
            File name for final state.
         """
 
-        if not self.restart_stem:
-            return f"{self.file_prefix}-T{self.temp}-final.xyz"
-        # respect the users choice
-        return f"{self.restart_stem}-T{self.temp}-final.xyz"
+        return self._build_filename(
+            "final.xyz", f"T{self.temp}", prefix_override=self.restart_stem
+        )
 
     @property
     def _restart_file(self) -> str:
         """
         Restart file name.
 
         Returns
         -------
         str
            File name for restart files.
         """
         step = self.offset + self.dyn.nsteps
-        if not self.restart_stem:
-            return f"{self.file_prefix}-T{self.temp}-res-{step}.xyz"
-        return f"{self.restart_stem}-T{self.temp}-res-{step}.xyz"
-
-    def configure_filenames(self) -> None:
-        """Setup filenames for output files."""
-
-        if not self.file_prefix:
-            self.file_prefix = f"{self.struct_name}-{self.ensemble}"
-            data_prefix = f"{self.file_prefix}{self._parameter_prefix}"
-        else:
-            data_prefix = f"{self.file_prefix}"
-            if not self.restart_stem:
-                self.restart_stem = f"{self.file_prefix}"
-
-        if not self.stats_file:
-            self.stats_file = f"{data_prefix}-stats.dat"
-
-        if not self.traj_file:
-            self.traj_file = f"{data_prefix}-traj.xyz"
+        return self._build_filename(
+            f"res-{step}.xyz", f"T{self.temp}", prefix_override=self.restart_stem
+        )
 
     @staticmethod
     def get_log_header() -> str:
         """
         Get header string for molecular dynamics log.
 
         Returns
@@ -470,15 +458,15 @@
         str
             Thermodynamical statistics to be written out.
         """
         e_pot = self.dyn.atoms.get_potential_energy() / self.n_atoms
         e_kin = self.dyn.atoms.get_kinetic_energy() / self.n_atoms
         current_temp = e_kin / (1.5 * units.kB)
 
-        time = self.offset * self.timestep + self.dyn.get_time() / units.fs
+        time = (self.offset * self.timestep + self.dyn.get_time()) / units.fs
         step = self.offset + self.dyn.nsteps
         self.dyn.atoms.info["time_fs"] = time
         self.dyn.atoms.info["step"] = step
 
         time_now = datetime.datetime.now()
         real_time = time_now - self.dyn.atoms.info["real_time"]
         self.dyn.atoms.info["real_time"] = time_now
@@ -518,14 +506,19 @@
         )
 
         return log_stats
 
     def _write_stats_file(self) -> None:
         """Write molecular dynamics log."""
         log_stats = self.get_log_stats()
+
+        # we do not want to print step 0 in restarts
+        if self.restart and self.dyn.nsteps == 0:
+            return
+
         with open(self.stats_file, "a", encoding="utf8") as stats_file:
             print(log_stats, file=stats_file)
 
     def _write_traj(self) -> None:
         """Write current structure to trajectory file."""
         if self.dyn.nsteps >= self.traj_start:
             # Append if restarting or already started writing
@@ -764,34 +757,37 @@
 
         Returns
         -------
         str
            File name for final state, includes pressure.
         """
 
-        pressure = f"-p{self.pressure}" if not isinstance(self, NVT_NH) else ""
-        if not self.restart_stem:
-            return f"{self.file_prefix}-T{self.temp}{pressure}-final.xyz"
-        return f"{self.restart_stem}-T{self.temp}{pressure}-final.xyz"
+        pressure = f"p{self.pressure}" if not isinstance(self, NVT_NH) else ""
+        return self._build_filename(
+            "final.xyz", f"T{self.temp}", pressure, prefix_override=self.restart_stem
+        )
 
     @property
     def _restart_file(self) -> str:
         """
         Restart file name.
 
         Returns
         -------
         str
            File name for restart file, includes pressure.
         """
         step = self.offset + self.dyn.nsteps
-        pressure = f"-p{self.pressure}" if not isinstance(self, NVT_NH) else ""
-        if not self.restart_stem:
-            return f"{self.file_prefix}-T{self.temp}{pressure}-res-{step}.xyz"
-        return f"{self.restart_stem}-T{self.temp}{pressure}-res-{step}.xyz"
+        pressure = f"p{self.pressure}" if not isinstance(self, NVT_NH) else ""
+        return self._build_filename(
+            f"res-{step}.xyz",
+            f"T{self.temp}",
+            pressure,
+            prefix_override=self.restart_stem,
+        )
 
     def get_log_stats(self) -> str:
         """
         Get thermodynamical statistics to be written to molecular dynamics log.
 
         Returns
         -------
```

### Comparing `janus_core-0.4.0b0/janus_core/calculations/single_point.py` & `janus_core-0.5.0b0/janus_core/calculations/single_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     CalcResults,
     Devices,
     MaybeList,
     MaybeSequence,
 )
 from janus_core.helpers.log import config_logger
 from janus_core.helpers.mlip_calculators import choose_calculator
-from janus_core.helpers.utils import none_to_dict
+from janus_core.helpers.utils import FileNameMixin, none_to_dict
 
 
-class SinglePoint:
+class SinglePoint(FileNameMixin):
     """
     Prepare and perform single point calculations.
 
     Parameters
     ----------
     struct : Optional[MaybeSequence[Atoms]]
         ASE Atoms structure(s) to simulate. Required if `struct_path` is None.
@@ -39,15 +39,16 @@
         is specified, else inferred from `struct_path`.
     architecture : Literal[architectures]
         MLIP architecture to use for single point calculations.
         Default is "mace_mp".
     device : Devices
         Device to run model on. Default is "cpu".
     read_kwargs : ASEReadArgs
-        Keyword arguments to pass to ase.io.read. Default is {}.
+        Keyword arguments to pass to ase.io.read. By default,
+        read_kwargs["index"] is ":".
     calc_kwargs : Optional[dict[str, Any]]
         Keyword arguments to pass to the selected calculator. Default is {}.
     log_kwargs : Optional[dict[str, Any]]
             Keyword arguments to pass to `config_logger`. Default is {}.
 
     Attributes
     ----------
@@ -101,15 +102,16 @@
             is specified, else inferred from `struct_path`.
         architecture : Architectures
             MLIP architecture to use for single point calculations.
             Default is "mace_mp".
         device : Devices
             Device to run MLIP model on. Default is "cpu".
         read_kwargs : Optional[ASEReadArgs]
-            Keyword arguments to pass to ase.io.read. Default is {}.
+            Keyword arguments to pass to ase.io.read. By default,
+            read_kwargs["index"] is ":".
         calc_kwargs : Optional[dict[str, Any]]
             Keyword arguments to pass to the selected calculator. Default is {}.
         log_kwargs : Optional[dict[str, Any]]
             Keyword arguments to pass to `config_logger`. Default is {}.
         """
         if struct and struct_path:
             raise ValueError(
@@ -134,21 +136,24 @@
         self.logger = config_logger(**log_kwargs)
 
         self.architecture = architecture
         self.device = device
         self.struct_path = struct_path
         self.struct_name = struct_name
 
+        # Read full trajectory by default
+        read_kwargs.setdefault("index", ":")
+
         # Read structure if given as path
         if self.struct_path:
             self.read_structure(**read_kwargs)
         else:
             self.struct = struct
-            if not self.struct_name:
-                self.struct_name = self.struct.get_chemical_formula()
+
+        FileNameMixin.__init__(self, self.struct, self.struct_name, None)
 
         # Configure calculator
         self.set_calculator(**calc_kwargs)
 
         if self.logger:
             self.logger.info("Single point calculator configured")
 
@@ -160,21 +165,21 @@
         will be read by default.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments passed to ase.io.read.
         """
-        if self.struct_path:
-            self.struct = read(self.struct_path, **kwargs)
-            if not self.struct_name:
-                self.struct_name = Path(self.struct_path).stem
-        else:
+        if not self.struct_path:
             raise ValueError("`struct_path` must be defined")
 
+        self.struct = read(self.struct_path, **kwargs)
+        if not self.struct_name:
+            self.struct_name = Path(self.struct_path).stem
+
     def set_calculator(
         self, read_kwargs: Optional[ASEReadArgs] = None, **kwargs
     ) -> None:
         """
         Configure calculator and attach to structure.
 
         Parameters
@@ -192,14 +197,17 @@
         if self.struct is None:
             read_kwargs = read_kwargs if read_kwargs else {}
             self.read_structure(**read_kwargs)
 
         if isinstance(self.struct, list):
             for struct in self.struct:
                 struct.calc = calculator
+            # Return single Atoms object if only one image in list
+            if len(self.struct) == 1:
+                self.struct = self.struct[0]
         else:
             self.struct.calc = calculator
 
     def _get_potential_energy(self) -> MaybeList[float]:
         """
         Calculate potential energy using MLIP.
 
@@ -334,15 +342,15 @@
                     f"Property '{prop}' cannot currently be calculated."
                 )
 
         write_kwargs = write_kwargs if write_kwargs else {}
 
         write_kwargs.setdefault(
             "filename",
-            Path(f"./{self.struct_name}-results.xyz").absolute(),
+            self._build_filename("results.xyz").absolute(),
         )
 
         if self.logger:
             self.logger.info("Starting single point calculation")
 
         if "energy" in properties or len(properties) == 0:
             results["energy"] = self._get_potential_energy()
```

### Comparing `janus_core-0.4.0b0/janus_core/cli/geomopt.py` & `janus_core-0.5.0b0/janus_core/cli/geomopt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Set up geomopt commandline interface."""
 
 from pathlib import Path
 from typing import Annotated
 
+from ase import units
 from typer import Context, Option, Typer
 from typer_config import use_config
 
 from janus_core.calculations.geom_opt import optimize
 from janus_core.calculations.single_point import SinglePoint
 from janus_core.cli.types import (
     Architecture,
@@ -19,14 +20,15 @@
     Summary,
     WriteKwargs,
 )
 from janus_core.cli.utils import (
     check_config,
     end_summary,
     parse_typer_dicts,
+    save_struct_calc,
     start_summary,
     yaml_converter_callback,
 )
 from janus_core.helpers.utils import dict_paths_to_strs
 
 app = Typer()
 
@@ -36,28 +38,33 @@
 )
 @use_config(yaml_converter_callback)
 def geomopt(
     # pylint: disable=too-many-arguments,too-many-locals,duplicate-code
     # numpydoc ignore=PR02
     ctx: Context,
     struct: StructPath,
-    fmax: Annotated[float, Option(help="Maximum force for convergence.")] = 0.1,
+    fmax: Annotated[
+        float, Option(help="Maximum force for convergence, in eV/Å.")
+    ] = 0.1,
     steps: Annotated[int, Option(help="Maximum number of optimization steps.")] = 1000,
     arch: Architecture = "mace_mp",
     device: Device = "cpu",
     vectors_only: Annotated[
         bool,
         Option(help="Optimize cell vectors, as well as atomic positions."),
     ] = False,
     fully_opt: Annotated[
         bool,
         Option(
             help="Fully optimize the cell vectors, angles, and atomic positions.",
         ),
     ] = False,
+    pressure: Annotated[
+        float, Option(help="Scalar pressure when optimizing cell geometry, in bar.")
+    ] = 0.0,
     out: Annotated[
         Path,
         Option(
             help=(
                 "Path to save optimized structure. Default is inferred from name "
                 "of structure file."
             ),
@@ -80,29 +87,31 @@
     Parameters
     ----------
     ctx : Context
         Typer (Click) Context. Automatically set.
     struct : Path
         Path of structure to simulate.
     fmax : float
-        Set force convergence criteria for optimizer in units eV/Å.
-        Default is 0.1.
+        Set force convergence criteria for optimizer, in eV/Å. Default is 0.1.
     steps : int
         Set maximum number of optimization steps to run. Default is 1000.
     arch : Optional[str]
         MLIP architecture to use for geometry optimization.
         Default is "mace_mp".
     device : Optional[str]
         Device to run model on. Default is "cpu".
     vectors_only : bool
         Whether to optimize cell vectors, as well as atomic positions, by setting
         `hydrostatic_strain` in the filter function. Default is False.
     fully_opt : bool
         Whether to fully optimize the cell vectors, angles, and atomic positions.
         Default is False.
+    pressure : float
+        Scalar pressure when optimizing cell geometry, in bar. Passed to the filter
+        function if either `vectors_only` or `fully_opt` is True. Default is 0.0.
     out : Optional[Path]
         Path to save optimized structure, or last structure if optimization did not
         converge. Default is inferred from name of structure file.
     traj : Optional[str]
         Path if saving optimization frames. Default is None.
     read_kwargs : Optional[dict[str, Any]]
         Keyword arguments to pass to ase.io.read. Default is {}.
@@ -155,14 +164,15 @@
     # Set same trajectory filenames to overwrite saved binary with xyz
     opt_kwargs["trajectory"] = traj if traj else None
     traj_kwargs = {"filename": traj} if traj else None
 
     # Set hydrostatic_strain
     # If not passed --fully-opt or --vectors-only, will be unused
     filter_kwargs = {"hydrostatic_strain": vectors_only}
+    filter_kwargs["scalar_pressure"] = pressure * units.bar
 
     # Use default filter if passed --fully-opt or --vectors-only
     # Otherwise override with None
     fully_opt_dict = {} if (fully_opt or vectors_only) else {"filter_func": None}
 
     # Dictionary of inputs for optimize function
     optimize_kwargs = {
@@ -181,27 +191,15 @@
     # Store inputs for yaml summary
     inputs = optimize_kwargs.copy()
 
     # Store only filename as filemode is not set by user
     del inputs["log_kwargs"]
     inputs["log"] = log
 
-    inputs["struct"] = {
-        "n_atoms": len(s_point.struct),
-        "struct_path": struct,
-        "struct_name": s_point.struct_name,
-        "formula": s_point.struct.get_chemical_formula(),
-    }
-
-    inputs["calc"] = {
-        "arch": arch,
-        "device": device,
-        "read_kwargs": read_kwargs,
-        "calc_kwargs": calc_kwargs,
-    }
+    save_struct_calc(inputs, s_point, arch, device, read_kwargs, calc_kwargs)
 
     # Convert all paths to strings in inputs nested dictionary
     dict_paths_to_strs(inputs)
 
     # Save summary information before optimization begins
     start_summary(command="geomopt", summary=summary, inputs=inputs)
```

### Comparing `janus_core-0.4.0b0/janus_core/cli/janus.py` & `janus_core-0.5.0b0/janus_core/cli/janus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """Set up commandline interface."""
 
 from typing import Annotated
 
 from typer import Exit, Option, Typer
 
 from janus_core import __version__
+from janus_core.cli.descriptors import descriptors
+from janus_core.cli.eos import eos
 from janus_core.cli.geomopt import geomopt
 from janus_core.cli.md import md
+from janus_core.cli.phonons import phonons
 from janus_core.cli.singlepoint import singlepoint
 
 app = Typer(name="janus", no_args_is_help=True)
 app.command()(singlepoint)
 app.command()(geomopt)
 app.command()(md)
+app.command()(phonons)
+app.command()(eos)
+app.command()(descriptors)
+
 # Train not imlpemented in older versions of MACE
 try:
     from janus_core.cli.train import train
 
     app.command()(train)
 except NotImplementedError:
     pass
```

### Comparing `janus_core-0.4.0b0/janus_core/cli/md.py` & `janus_core-0.5.0b0/janus_core/cli/md.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     StructPath,
     Summary,
 )
 from janus_core.cli.utils import (
     check_config,
     end_summary,
     parse_typer_dicts,
+    save_struct_calc,
     start_summary,
     yaml_converter_callback,
 )
 from janus_core.helpers.janus_types import Ensembles
 from janus_core.helpers.utils import dict_paths_to_strs
 
 app = Typer()
@@ -181,15 +182,15 @@
     ----------
     ctx : Context
         Typer (Click) Context. Automatically set.
     ensemble : str
         Name of thermodynamic ensemble.
     struct : Path
         Path of structure to simulate.
-    struct_name : str
+    struct_name : Optional[str]
         Name of structure to simulate. Default is inferred from filepath or chemical
         formula.
     steps : int
         Number of steps in simulation. Default is 0.
     timestep : float
         Timestep for integrator, in fs. Default is 1.0.
     temp : float
@@ -338,60 +339,45 @@
     }
 
     # Instantiate MD ensemble
     if ensemble == "nvt":
         for key in ["thermostat_time", "barostat_time", "bulk_modulus", "pressure"]:
             del dyn_kwargs[key]
         dyn = NVT(**dyn_kwargs)
-
-    if ensemble == "npt":
+    elif ensemble == "npt":
         del dyn_kwargs["friction"]
         dyn = NPT(**dyn_kwargs)
-
-    if ensemble == "nph":
+    elif ensemble == "nph":
         for key in ["friction", "barostat_time"]:
             del dyn_kwargs[key]
         dyn = NPH(**dyn_kwargs)
-
-    if ensemble == "nve":
+    elif ensemble == "nve":
         for key in [
             "thermostat_time",
             "barostat_time",
             "bulk_modulus",
             "pressure",
             "friction",
         ]:
             del dyn_kwargs[key]
         dyn = NVE(**dyn_kwargs)
-
-    if ensemble == "nvt-nh":
+    elif ensemble == "nvt-nh":
         for key in ["barostat_time", "bulk_modulus", "pressure", "friction"]:
             del dyn_kwargs[key]
         dyn = NVT_NH(**dyn_kwargs)
-
+    else:
+        raise ValueError(f"Unsupported Ensemble ({ensemble})")
     # Store inputs for yaml summary
     inputs = dyn_kwargs | {"ensemble": ensemble}
 
     # Store only filename as filemode is not set by user
     del inputs["log_kwargs"]
     inputs["log"] = log
 
-    inputs["struct"] = {
-        "n_atoms": len(s_point.struct),
-        "struct_path": struct,
-        "struct_name": s_point.struct_name,
-        "formula": s_point.struct.get_chemical_formula(),
-    }
-
-    inputs["calc"] = {
-        "arch": arch,
-        "device": device,
-        "read_kwargs": read_kwargs,
-        "calc_kwargs": calc_kwargs,
-    }
+    save_struct_calc(inputs, s_point, arch, device, read_kwargs, calc_kwargs)
 
     # Convert all paths to strings in inputs nested dictionary
     dict_paths_to_strs(inputs)
 
     # Save summary information before simulation begins
     start_summary(command="md", summary=summary, inputs=inputs)
```

### Comparing `janus_core-0.4.0b0/janus_core/cli/singlepoint.py` & `janus_core-0.5.0b0/janus_core/cli/singlepoint.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Set up singlepoint commandline interface."""
 
 from pathlib import Path
 from typing import Annotated
 
-from ase import Atoms
 from typer import Context, Option, Typer
 from typer_config import use_config
 
 from janus_core.calculations.single_point import SinglePoint
 from janus_core.cli.types import (
     Architecture,
     CalcKwargs,
@@ -18,14 +17,15 @@
     Summary,
     WriteKwargs,
 )
 from janus_core.cli.utils import (
     check_config,
     end_summary,
     parse_typer_dicts,
+    save_struct_calc,
     start_summary,
     yaml_converter_callback,
 )
 from janus_core.helpers.utils import dict_paths_to_strs
 
 app = Typer()
 
@@ -120,38 +120,19 @@
         "log_kwargs": {"filename": log, "filemode": "w"},
     }
 
     # Initialise singlepoint structure and calculator
     s_point = SinglePoint(**singlepoint_kwargs)
 
     # Store inputs for yaml summary
-    inputs = singlepoint_kwargs.copy()
 
     # Store only filename as filemode is not set by user
-    del inputs["log_kwargs"]
-    del inputs["struct_path"]
-    inputs["log"] = log
-
-    if isinstance(s_point.struct, Atoms):
-        inputs["struct"] = {
-            "n_atoms": len(s_point.struct),
-            "struct_path": struct,
-            "struct_name": s_point.struct_name,
-            "formula": s_point.struct.get_chemical_formula(),
-        }
-    else:
-        inputs["traj"] = {
-            "length": len(s_point.struct),
-            "struct_path": struct,
-            "struct_name": s_point.struct_name,
-            "struct": {
-                "n_atoms": len(s_point.struct[0]),
-                "formula": s_point.struct[0].get_chemical_formula(),
-            },
-        }
+    inputs = {"log": log}
+
+    save_struct_calc(inputs, s_point, arch, device, read_kwargs, calc_kwargs)
 
     inputs["run"] = {
         "properties": properties,
         "write_kwargs": write_kwargs,
     }
 
     # Convert all paths to strings in inputs nested dictionary
```

### Comparing `janus_core-0.4.0b0/janus_core/cli/train.py` & `janus_core-0.5.0b0/janus_core/cli/train.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.4.0b0/janus_core/cli/types.py` & `janus_core-0.5.0b0/janus_core/cli/types.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.4.0b0/janus_core/cli/utils.py` & `janus_core-0.5.0b0/janus_core/cli/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Utility functions for CLI."""
 
+from collections.abc import Sequence
 import datetime
 import logging
 from pathlib import Path
 from typing import Any
 
+from ase import Atoms
 from typer import Context
 from typer_config import conf_callback_factory, yaml_loader
 import yaml
 
+from janus_core.calculations.single_point import SinglePoint
 from janus_core.cli.types import TyperDict
+from janus_core.helpers.janus_types import Architectures, ASEReadArgs, Devices
 from janus_core.helpers.utils import dict_remove_hyphens
 
 
 def parse_typer_dicts(typer_dicts: list[TyperDict]) -> list[dict]:
     """
     Convert list of TyperDict objects to list of dictionaries.
 
@@ -103,14 +107,67 @@
             {"end_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")},
             outfile,
             default_flow_style=False,
         )
     logging.shutdown()
 
 
+def save_struct_calc(
+    inputs: dict,
+    s_point: SinglePoint,
+    arch: Architectures,
+    device: Devices,
+    read_kwargs: ASEReadArgs,
+    calc_kwargs: dict[str, Any],
+) -> None:
+    """
+    Add structure and calculator input information to a dictionary.
+
+    Parameters
+    ----------
+
+    inputs : dict
+        Inputs dictionary to add information to.
+    s_point : SinglePoint
+        SinglePoint object storing structure with attached calculator.
+    arch : Architectures
+        MLIP architecture.
+    device : Devices
+        Device to run calculations on.
+    read_kwargs : ASEReadArgs
+        Keyword arguments to pass to ase.io.read.
+    calc_kwargs : dict[str, Any]]
+        Keyword arguments to pass to the calculator.
+    """
+    if isinstance(s_point.struct, Atoms):
+        inputs["struct"] = {
+            "n_atoms": len(s_point.struct),
+            "struct_path": s_point.struct_path,
+            "struct_name": s_point.struct_name,
+            "formula": s_point.struct.get_chemical_formula(),
+        }
+    elif isinstance(s_point.struct, Sequence):
+        inputs["traj"] = {
+            "length": len(s_point.struct),
+            "struct_path": s_point.struct_path,
+            "struct_name": s_point.struct_name,
+            "struct": {
+                "n_atoms": len(s_point.struct[0]),
+                "formula": s_point.struct[0].get_chemical_formula(),
+            },
+        }
+
+    inputs["calc"] = {
+        "arch": arch,
+        "device": device,
+        "read_kwargs": read_kwargs,
+        "calc_kwargs": calc_kwargs,
+    }
+
+
 def check_config(ctx: Context) -> None:
     """
     Check options in configuration file are valid options for CLI command.
 
     Parameters
     ----------
     ctx : Context
```

### Comparing `janus_core-0.4.0b0/janus_core/helpers/janus_types.py` & `janus_core-0.5.0b0/janus_core/helpers/janus_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections.abc import Sequence
 from enum import Enum
 import logging
 from pathlib import Path, PurePath
 from typing import IO, Literal, Optional, TypedDict, TypeVar, Union
 
 from ase import Atoms
+from ase.eos import EquationOfState
 import numpy as np
 from numpy.typing import NDArray
 
 # General
 
 T = TypeVar("T")
 MaybeList = Union[T, list[T]]
@@ -45,28 +46,51 @@
     """Main arugments for ase optimisers."""
 
     restart: Optional[bool]
     logfile: Optional[PathLike]
     trajectory: Optional[str]
 
 
+# eos_names from ase.eos
+EoSNames = Literal[
+    "sj",
+    "taylor",
+    "murnaghan",
+    "birch",
+    "birchmurnaghan",
+    "pouriertarantola",
+    "vinet",
+    "antonschmidt",
+    "p3",
+]
+
+
+# Janus specific
+Architectures = Literal["mace", "mace_mp", "mace_off", "m3gnet", "chgnet"]
+Devices = Literal["cpu", "cuda", "mps"]
+Ensembles = Literal["nph", "npt", "nve", "nvt", "nvt-nh"]
+
+
 class LogLevel(Enum):  # numpydoc ignore=PR01
     """Supported options for logger levels."""
 
     DEBUG = logging.DEBUG
     INFO = logging.INFO
     WARNING = logging.WARNING
     ERROR = logging.ERROR
 
 
-# Janus specific
-Architectures = Literal["mace", "mace_mp", "mace_off", "m3gnet", "chgnet"]
-Devices = Literal["cpu", "cuda", "mps"]
-Ensembles = Literal["nph", "npt", "nve", "nvt", "nvt-nh"]
-
-
 class CalcResults(TypedDict, total=False):
     """Return type from calculations."""
 
     energy: MaybeList[float]
     forces: MaybeList[NDArray[np.float64]]
     stress: MaybeList[NDArray[np.float64]]
+
+
+class EoSResults(TypedDict, total=False):
+    """Return type from calculations."""
+
+    eos: EquationOfState
+    bulk_modulus: float
+    v_0: float
+    e_0: float
```

### Comparing `janus_core-0.4.0b0/janus_core/helpers/log.py` & `janus_core-0.5.0b0/janus_core/helpers/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 def config_logger(
     name: str,
     filename: Optional[str] = None,
     level: LogLevel = logging.INFO,
     capture_warnings: bool = True,
     filemode: Literal["r", "w", "a", "x", "r+", "w+", "a+", "x+"] = "w",
     force: bool = True,
-):
+) -> Optional[logging.Logger]:
     """
     Configure logger with yaml-styled format.
 
     Parameters
     ----------
     name : str
         Name of logger. Default is None.
```

### Comparing `janus_core-0.4.0b0/janus_core/helpers/mlip_calculators.py` & `janus_core-0.5.0b0/janus_core/helpers/mlip_calculators.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Similar in spirit to matcalc and quacc approaches
 - https://github.com/materialsvirtuallab/matcalc
 - https://github.com/Quantum-Accelerators/quacc.git
 """
 
 from ase.calculators.calculator import Calculator
+import torch
 
 from janus_core.helpers.janus_types import Architectures, Devices
 
 
 def choose_calculator(
     architecture: Architectures = "mace",
     device: Devices = "cpu",
@@ -77,22 +78,28 @@
         kwargs.setdefault("default_dtype", "float64")
         calculator = mace_off(**kwargs)
 
     elif architecture == "m3gnet":
         from matgl import __version__, load_model
         from matgl.ext.ase import M3GNetCalculator
 
+        # Set before loading model to avoid type mismatches
+        torch.set_default_dtype(torch.float32)
+
         model = kwargs.setdefault("model", load_model("M3GNet-MP-2021.2.8-DIRECT-PES"))
         kwargs.setdefault("stress_weight", 1.0 / 160.21766208)
+
         calculator = M3GNetCalculator(potential=model, **kwargs)
 
     elif architecture == "chgnet":
         from chgnet import __version__
         from chgnet.model.dynamics import CHGNetCalculator
 
+        # Set to avoid type mismatches
+        torch.set_default_dtype(torch.float32)
         calculator = CHGNetCalculator(use_device=device, **kwargs)
 
     else:
         raise ValueError(
             f"Unrecognized {architecture=}. Suported architectures "
             f"are {', '.join(Architectures.__args__)}"
         )
```

### Comparing `janus_core-0.4.0b0/janus_core/helpers/stats.py` & `janus_core-0.5.0b0/janus_core/helpers/stats.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.4.0b0/janus_core/helpers/train.py` & `janus_core-0.5.0b0/janus_core/helpers/train.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.4.0b0/pyproject.toml` & `janus_core-0.5.0b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "janus-core"
-version = "0.4.0b0"
+version = "0.5.0b0"
 description = "Tools for machine learnt interatomic potentials"
 authors = [
     "Elliott Kasoar",
     "Federica Zanca",
     "Patrick Austin",
     "David Mason",
     "Jacob Wilkins",
@@ -28,14 +28,17 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 ase = "^3.22.1"
 mace-torch = "^0.3.4"
 pyyaml = "^6.0.1"
 typer = "^0.9.0"
 typer-config = "^1.4.0"
+phonopy = "^2.23.1"
+seekpath = "^2.1.0"
+spglib = "^2.3.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = "^7.4.1"}
 pgtest = "^1.3.2"
 pytest = "^8.0"
 pytest-cov = "^4.1.0"
 tox = "^4.12.1"
@@ -61,28 +64,28 @@
 
 [tool.poetry.group.extra-mlips]
 optional = true
 [tool.poetry.group.extra-mlips.dependencies]
 dgl = "^1.1.3"
 chgnet = "^0.3.4"
 matgl = "^1.0.0"
-spglib = "<=2.2.0"
 torch-dftd = "^0.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 
 [tool.pylint.format]
 max-line-length = 88
 max-args = 10
 good-names = ["e", "i", "j", "k"]
+min-similarity-lines=9
 
 [tool.pytest.ini_options]
 # Configuration for [pytest](https://docs.pytest.org)
 python_files = "test_*.py"
 addopts = '--cov-report xml'
 pythonpath = ["."]
```

### Comparing `janus_core-0.4.0b0/PKG-INFO` & `janus_core-0.5.0b0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: janus-core
-Version: 0.4.0b0
-Summary: Tools for machine learnt interatomic potentials
-Home-page: https://github.com/stfc/janus-core/
-Author: Elliott Kasoar
-Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ase (>=3.22.1,<4.0.0)
-Requires-Dist: mace-torch (>=0.3.4,<0.4.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
-Requires-Dist: typer-config (>=1.4.0,<2.0.0)
-Project-URL: Documentation, https://stfc.github.io/janus-core/
-Project-URL: Repository, https://github.com/stfc/janus-core/
-Description-Content-Type: text/markdown
-
 [![Build Status][ci-badge]][ci-link]
 [![Coverage Status][cov-badge]][cov-link]
 [![Docs status][docs-badge]][docs-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![License][license-badge]][license-link]
 [![DOI][doi-badge]][doi-link]
 
@@ -46,16 +20,17 @@
 - [x] Single point calculations
 - [x] Geometry optimisation
 - [x] Molecular Dynamics
   - NVE
   - NVT (Langevin(Eijnden/Ciccotti flavour) and Nosé-Hoover (Melchionna flavour))
   - NPT (Nosé-Hoover (Melchiona flavour))
 - [ ] Nudge Elastic Band
-- [ ] Phonons
-  - vibroscopy
+- [x] Phonons
+  - Phonopy
+- [x] Equation of State
 - [x] Training ML potentials
   - MACE
 - [x] Fine tunning MLIPs
   - MACE
 - [ ] Rare events simulations
   - PLUMED
 
@@ -103,15 +78,22 @@
 
 ```shell
 janus singlepoint --struct tests/data/NaCl.cif --arch mace --calc-kwargs "{'model' : '/path/to/your/ml.model'}" --properties energy --properties forces --log ./example.log --out ./example.xyz
 ```
 
 This calculates both forces and energies, defines the MLIP architecture and path to your locally saved model, and changes where the log and results files are saved.
 
-Note: the MACE calculator currently returns energy, forces and stress together, so in this case the choice of property will not change the output.
+> [!NOTE]
+> The MACE calculator currently returns energy, forces and stress together, so in this case the choice of property will not change the output.
+
+By default, all structures in a trajectory file will be read, but specific structures can be selected using --read-kwargs:
+
+```shell
+janus singlepoint --struct tests/data/benzene-traj.xyz --read-kwargs "{'index': 0}"
+```
 
 For all options, run `janus singlepoint --help`.
 
 
 ### Geometry optimization
 
 Perform geometry optimization (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
@@ -192,14 +174,67 @@
 janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10 --steps 1000 --temp 300
 ```
 
 This performs the same initial heating, before running a further 1000 steps (1 ps) at 300K.
 
 When MD is run with heating the trajectory ```NaCl-nvt-T20.0-T300.0-T300.0-traj.xyz``` and statistics ```NaCl-nvt-T20.0-T300.0-T300.0-stats.dat``` files will indicate the heating range and MD temperature (which may be different). With heating and MD trajectories/statistics within the same files.
 
+Additional settings for geometry optimization, such as enabling optimization of cell vectors by setting `hydrostatic_strain = True` for the ASE filter, can be set using the `--minimize-kwargs` option:
+
+```shell
+janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 0 --temp-end 300 --temp-step 10 --temp-time 10 --minimize --minimize-kwargs "{'filter_kwargs': {'hydrostatic_strain' : True}}"
+```
+
+### Equation of State
+
+Fit the equation of state for a structure (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
+
+```shell
+janus eos --struct tests/data/NaCl.cif --no-minimize --min-volume 0.9 --max-volume 1.1 --n-volumes 9 --arch mace_mp --calc-kwargs "{'model' : 'small'}"
+```
+
+This will save the energies and volumes for nine lattice constants in `NaCl-eos-raw.dat`, and the fitted minimum energy, volume, and bulk modulus in `NaCl-eos-fit.dat`, in addition to generating a log file, `eos.log`, and summary of inputs, `eos_summary.yml`.
+
+By default, geometry optimization will be performed on the initial structure, before calculations are performed for the range of lattice constants consistent with minimum and maximum volumes supplied. Optimization at constant volume for all generated structures can also be performed (sharing the same maximum force convergence):
+
+```shell
+janus eos --struct tests/data/NaCl.cif --minimize-all --fmax 0.0001
+```
+
+For all options, run `janus eos --help`.
+
+
+### Phonons
+
+Calculate phonons with a 2x2x2 supercell, after geometry optimization (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
+
+```shell
+janus phonons --struct tests/data/NaCl.cif --supercell 2x2x2 --minimize --arch mace_mp --calc-kwargs "{'model' : 'small'}"
+```
+
+This will save the Phonopy parameters, including displacements and force constants, to `NaCl-phonopy.yml` and `NaCl-force_constants.hdf5`, in addition to generating a log file, `phonons.log`, and summary of inputs, `phonons_summary.yml`.
+
+Additionally, the `--band` option can be added to calculate the band structure and save the results to `NaCl-auto_bands.yml`:
+
+```shell
+janus phonons --struct tests/data/NaCl.cif --supercell 2x2x2 --minimize --arch mace_mp --calc-kwargs "{'model' : 'small'}" --band
+```
+
+If you need eigenvectors and group velocities written, add the `--write-full` option. This will generate a much larger file, but can be used to visualise phonon modes.
+
+Further calculations, including thermal properties, DOS, and PDOS, can also be calculated (using a 2x3x4 supercell):
+
+```shell
+janus phonons --struct tests/data/NaCl.cif --supercell 2x3x4 --dos --pdos --thermal --temp-start 0 --temp-end 300 --temp-step 50
+```
+
+This will create additional output files: `NaCl-thermal.dat` for the thermal properties (heat capacity, entropy, and free energy) between 0K and 300K, `NaCl-dos.dat` for the DOS, and `NaCl-pdos.dat` for the PDOS.
+
+For all options, run `janus phonons --help`.
+
 
 ### Using configuration files
 
 Default values for all command line options may be specifed through a Yaml 1.1 formatted configuration file by adding the `--config` option. If an option is present in both the command line and configuration file, the command line value takes precedence.
 
 For example, with the following configuration file and command:
 
@@ -240,14 +275,35 @@
 
 Foundational models can also be fine-tuned, by including the `foundation_model` option in your configuration file, and using `--fine-tune` option:
 
 ```shell
 janus train --mlip-config /path/to/fine/tuning/config.yml --fine-tune
 ```
 
+
+### Calculate MACE descriptors
+
+MACE descriptors can be calculated for structures (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
+
+```shell
+janus descriptors --struct tests/data/NaCl.cif --arch mace_mp --calc-kwargs "{'model' : 'small'}"
+```
+
+This will calculate the mean descriptor for this structure and save this as attached information (`descriptors`) in `NaCl-descriptors.xyz`, in addition to generating a log file, `descriptors.log`, and summary of inputs, `descriptors_summary.yml`.
+
+The mean descriptor per element can also be calculated, and all descriptors, rather than only the invariant part, can be used when calculating the means:
+
+```shell
+janus descriptors --struct tests/data/NaCl.cif --no-invariants-only --calc-per-element
+```
+
+This will generate the same output files, but additional labels (`Cl_descriptor` and `Na_descriptor`) will be saved in `NaCl-descriptors.xyz`.
+
+For all options, run `janus descriptors --help`.
+
 ## License
 
 [BSD 3-Clause License](LICENSE)
 
 ## Funding
 
 Contributors to this project were funded by
@@ -266,8 +322,7 @@
 [pypi-badge]: https://badge.fury.io/py/janus-core.svg
 [pypi-link]: https://badge.fury.io/py/janus-core
 [license-badge]: https://img.shields.io/badge/License-BSD_3--Clause-blue.svg
 [license-link]: https://opensource.org/licenses/BSD-3-Clause
 [doi-link]: https://zenodo.org/badge/latestdoi/754081470
 [doi-badge]: https://zenodo.org/badge/754081470.svg
 [logo]: https://raw.githubusercontent.com/stfc/janus-core/main/docs/source/images/janus-core-100.png
-
```

