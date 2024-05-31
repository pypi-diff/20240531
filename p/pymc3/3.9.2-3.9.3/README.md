# Comparing `tmp/pymc3-3.9.2.tar.gz` & `tmp/pymc3-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc3-3.9.2.tar", last modified: Wed Jun 24 12:08:39 2020, max compression
+gzip compressed data, was "dist/pymc3-3.9.3.tar", last modified: Tue Aug 11 03:30:55 2020, max compression
```

## Comparing `pymc3-3.9.2.tar` & `pymc3-3.9.3.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/
--rw-r--r--   0 runner    (1001) docker     (116)     3508 2020-06-24 12:08:31.000000 pymc3-3.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     7945 2020-06-24 12:08:31.000000 pymc3-3.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (116)    16956 2020-06-24 12:08:31.000000 pymc3-3.9.2/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (116)    11720 2020-06-24 12:08:31.000000 pymc3-3.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      266 2020-06-24 12:08:31.000000 pymc3-3.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    11226 2020-06-24 12:08:39.000000 pymc3-3.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8634 2020-06-24 12:08:31.000000 pymc3-3.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)    46662 2020-06-24 12:08:31.000000 pymc3-3.9.2/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/
--rw-r--r--   0 runner    (1001) docker     (116)     2236 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/backends/
--rw-r--r--   0 runner    (1001) docker     (116)     5254 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    20319 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     8025 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/backends/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (116)    14116 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (116)     7528 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (116)    13203 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/backends/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (116)     7959 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/backends/text.py
--rw-r--r--   0 runner    (1001) docker     (116)     3014 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/backends/tracetab.py
--rw-r--r--   0 runner    (1001) docker     (116)     6961 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/blocking.py
--rw-r--r--   0 runner    (1001) docker     (116)    20763 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/distributions/
--rw-r--r--   0 runner    (1001) docker     (116)     5261 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10904 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (116)   147600 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (116)    53088 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (116)    17562 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (116)    42018 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (116)    27211 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/mixture.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    73906 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (116)    28796 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/posterior_predictive.py
--rw-r--r--   0 runner    (1001) docker     (116)    14022 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2293 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (116)     1898 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/special.py
--rw-r--r--   0 runner    (1001) docker     (116)    16798 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (116)    15362 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/distributions/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     1821 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/GHME_2013.py
--rw-r--r--   0 runner    (1001) docker     (116)     1638 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/LKJ_correlation.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      714 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/arbitrary_stochastic.py
--rw-r--r--   0 runner    (1001) docker     (116)     2112 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/arma_example.py
--rw-r--r--   0 runner    (1001) docker     (116)     1016 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/baseball.py
--rw-r--r--   0 runner    (1001) docker     (116)     3375 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/custom_dists.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/examples/data/
--rw-r--r--   0 runner    (1001) docker     (116)     2333 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/Guber1999data.txt
--rw-r--r--   0 runner    (1001) docker     (116)      927 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/HtWt.csv
--rw-r--r--   0 runner    (1001) docker     (116)   131016 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/SP500.csv
--rw-r--r--   0 runner    (1001) docker     (116)     6040 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/babies.csv
--rw-r--r--   0 runner    (1001) docker     (116)   140076 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/cty.dat
--rw-r--r--   0 runner    (1001) docker     (116)     1008 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/efron-morris-75-data.tsv
--rw-r--r--   0 runner    (1001) docker     (116)    80080 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/extrahard_MC_500_5_4.npz.npy
--rw-r--r--   0 runner    (1001) docker     (116)     4080 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/extrahard_MC_500_5_4_reference_classes.npy
--rw-r--r--   0 runner    (1001) docker     (116)      575 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/mastectomy.csv
--rw-r--r--   0 runner    (1001) docker     (116)     5181 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/merged_ice_core_yearly.csv
--rw-r--r--   0 runner    (1001) docker     (116)      340 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/milk.csv
--rw-r--r--   0 runner    (1001) docker     (116)  1979173 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/ml_100k_u.data
--rw-r--r--   0 runner    (1001) docker     (116)   236356 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/ml_100k_u.item
--rw-r--r--   0 runner    (1001) docker     (116)    72328 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/monthly_in_situ_co2_mlo.csv
--rw-r--r--   0 runner    (1001) docker     (116)     2271 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/old_faithful.csv
--rw-r--r--   0 runner    (1001) docker     (116)    79411 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/pancreatitis.csv
--rw-r--r--   0 runner    (1001) docker     (116)   157833 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/radon.csv
--rw-r--r--   0 runner    (1001) docker     (116)     1740 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/rugby.csv
--rw-r--r--   0 runner    (1001) docker     (116)  1637302 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/srrs2.dat
--rw-r--r--   0 runner    (1001) docker     (116)    26978 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/stock_prices.csv
--rw-r--r--   0 runner    (1001) docker     (116)     9222 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/sunspot.csv
--rw-r--r--   0 runner    (1001) docker     (116)     9819 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/test_scores.csv
--rw-r--r--   0 runner    (1001) docker     (116)    98295 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/data/wells.dat
--rw-r--r--   0 runner    (1001) docker     (116)     1623 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/disaster_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     2213 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/disaster_model_theano_op.py
--rw-r--r--   0 runner    (1001) docker     (116)      553 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/factor_potential.py
--rw-r--r--   0 runner    (1001) docker     (116)     1430 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/garch_example.py
--rw-r--r--   0 runner    (1001) docker     (116)      660 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/gelman_bioassay.py
--rw-r--r--   0 runner    (1001) docker     (116)      943 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/gelman_schools.py
--rw-r--r--   0 runner    (1001) docker     (116)     2005 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/lasso_missing.py
--rw-r--r--   0 runner    (1001) docker     (116)     1121 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/lightspeed_example.py
--rw-r--r--   0 runner    (1001) docker     (116)     1779 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/rankdata_ordered.py
--rw-r--r--   0 runner    (1001) docker     (116)     3301 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/samplers_mvnormal.py
--rw-r--r--   0 runner    (1001) docker     (116)      509 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/examples/simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)     2314 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/glm/
--rw-r--r--   0 runner    (1001) docker     (116)      668 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/glm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3830 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/glm/families.py
--rw-r--r--   0 runner    (1001) docker     (116)     7696 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/glm/linear.py
--rw-r--r--   0 runner    (1001) docker     (116)     4584 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/glm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/gp/
--rw-r--r--   0 runner    (1001) docker     (116)      739 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    23454 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (116)    44809 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2502 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (116)     5095 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (116)    12344 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/math.py
--rw-r--r--   0 runner    (1001) docker     (116)     2675 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/memoize.py
--rw-r--r--   0 runner    (1001) docker     (116)    66676 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     8615 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/ode/
--rw-r--r--   0 runner    (1001) docker     (116)      662 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9037 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (116)     4488 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/ode/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    14892 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/parallel_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/plots/
--rw-r--r--   0 runner    (1001) docker     (116)     3691 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2002 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/plots/posteriorplot.py
--rw-r--r--   0 runner    (1001) docker     (116)    76088 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/smc/
--rw-r--r--   0 runner    (1001) docker     (116)      639 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6981 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/smc/sample_smc.py
--rw-r--r--   0 runner    (1001) docker     (116)    16218 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/smc/smc.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/stats/
--rw-r--r--   0 runner    (1001) docker     (116)     1879 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/step_methods/
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9387 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (116)     2689 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/compound.py
--rw-r--r--   0 runner    (1001) docker     (116)     4430 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/elliptical_slice.py
--rw-r--r--   0 runner    (1001) docker     (116)     2943 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/gibbs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (116)      658 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8264 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (116)     6283 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (116)     3723 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (116)    17291 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (116)    23094 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (116)    28126 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (116)     7106 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/sgmcmc.py
--rw-r--r--   0 runner    (1001) docker     (116)     4208 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (116)     3021 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/step_methods/step_sizes.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      659 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22927 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/backend_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/checks.py
--rw-r--r--   0 runner    (1001) docker     (116)     1452 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     3254 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     5380 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     6150 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/sampler_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (116)      490 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_coords.py
--rw-r--r--   0 runner    (1001) docker     (116)    10531 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_data_container.py
--rw-r--r--   0 runner    (1001) docker     (116)     7628 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_dist_math.py
--rw-r--r--   0 runner    (1001) docker     (116)     2433 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_distribution_defaults.py
--rw-r--r--   0 runner    (1001) docker     (116)    61738 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (116)    51538 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_distributions_random.py
--rw-r--r--   0 runner    (1001) docker     (116)     5476 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_distributions_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (116)    12421 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (116)     6129 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_glm.py
--rw-r--r--   0 runner    (1001) docker     (116)    46863 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_gp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2754 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_hdf5_backend.py
--rw-r--r--   0 runner    (1001) docker     (116)     2507 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_hmc.py
--rw-r--r--   0 runner    (1001) docker     (116)     6823 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (116)      914 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_memo.py
--rw-r--r--   0 runner    (1001) docker     (116)    11952 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_minibatches.py
--rw-r--r--   0 runner    (1001) docker     (116)     3479 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_missing.py
--rw-r--r--   0 runner    (1001) docker     (116)    21969 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (116)    13783 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     1949 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_model_func.py
--rw-r--r--   0 runner    (1001) docker     (116)     3219 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_model_graph.py
--rw-r--r--   0 runner    (1001) docker     (116)     6381 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_model_helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     3973 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_modelcontext.py
--rw-r--r--   0 runner    (1001) docker     (116)     5121 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_models_linear.py
--rw-r--r--   0 runner    (1001) docker     (116)     3507 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_models_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     8335 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_ndarray_backend.py
--rw-r--r--   0 runner    (1001) docker     (116)    14276 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_ode.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_parallel_sampling.py
--rw-r--r--   0 runner    (1001) docker     (116)     1197 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (116)     1355 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_posdef_sym.py
--rw-r--r--   0 runner    (1001) docker     (116)     1357 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_posterior_predictive.py
--rw-r--r--   0 runner    (1001) docker     (116)     2395 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_posteriors.py
--rw-r--r--   0 runner    (1001) docker     (116)     1089 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (116)     9261 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (116)     6530 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (116)    36352 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (116)     8032 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_shape_handling.py
--rw-r--r--   0 runner    (1001) docker     (116)     2426 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (116)     4012 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_smc.py
--rw-r--r--   0 runner    (1001) docker     (116)     1964 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_special_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2657 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_sqlite_backend.py
--rw-r--r--   0 runner    (1001) docker     (116)     2689 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_starting.py
--rw-r--r--   0 runner    (1001) docker     (116)    33808 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (116)     3010 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_text_backend.py
--rw-r--r--   0 runner    (1001) docker     (116)     8967 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_theanof.py
--rw-r--r--   0 runner    (1001) docker     (116)     3169 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_tracetab.py
--rw-r--r--   0 runner    (1001) docker     (116)    15133 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (116)     1978 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_tuning.py
--rw-r--r--   0 runner    (1001) docker     (116)     2079 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     2961 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_updates.py
--rw-r--r--   0 runner    (1001) docker     (116)     5340 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (116)    35927 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tests/test_variational_inference.py
--rw-r--r--   0 runner    (1001) docker     (116)    15487 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/theanof.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/tuning/
--rw-r--r--   0 runner    (1001) docker     (116)      695 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3827 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (116)     9142 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (116)     5691 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3/variational/
--rw-r--r--   0 runner    (1001) docker     (116)     1405 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    20530 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (116)     4510 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (116)    17918 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/flows.py
--rw-r--r--   0 runner    (1001) docker     (116)    31502 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (116)     4192 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (116)    61467 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (116)     3050 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (116)     1739 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/test_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    38659 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-06-24 12:08:31.000000 pymc3-3.9.2/pymc3/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/pymc3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    11226 2020-06-24 12:08:38.000000 pymc3-3.9.2/pymc3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5727 2020-06-24 12:08:38.000000 pymc3-3.9.2/pymc3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-24 12:08:38.000000 pymc3-3.9.2/pymc3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      179 2020-06-24 12:08:38.000000 pymc3-3.9.2/pymc3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-06-24 12:08:38.000000 pymc3-3.9.2/pymc3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      176 2020-06-24 12:08:31.000000 pymc3-3.9.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 12:08:39.000000 pymc3-3.9.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)     1269 2020-06-24 12:08:31.000000 pymc3-3.9.2/scripts/create_testenv.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)     1555 2020-06-24 12:08:31.000000 pymc3-3.9.2/scripts/install_miniconda.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)       53 2020-06-24 12:08:31.000000 pymc3-3.9.2/scripts/lint.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      980 2020-06-24 12:08:31.000000 pymc3-3.9.2/scripts/start_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      246 2020-06-24 12:08:31.000000 pymc3-3.9.2/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (116)      167 2020-06-24 12:08:39.000000 pymc3-3.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     3048 2020-06-24 12:08:31.000000 pymc3-3.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/
+-rw-r--r--   0 runner    (1001) docker     (116)     3508 2020-08-11 03:30:43.000000 pymc3-3.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)     7945 2020-08-11 03:30:43.000000 pymc3-3.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (116)    16956 2020-08-11 03:30:43.000000 pymc3-3.9.3/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (116)    11720 2020-08-11 03:30:43.000000 pymc3-3.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      266 2020-08-11 03:30:43.000000 pymc3-3.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    16079 2020-08-11 03:30:55.000000 pymc3-3.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    13335 2020-08-11 03:30:43.000000 pymc3-3.9.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)    48737 2020-08-11 03:30:43.000000 pymc3-3.9.3/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/
+-rw-r--r--   0 runner    (1001) docker     (116)     1928 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/backends/
+-rw-r--r--   0 runner    (1001) docker     (116)     5254 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20319 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8025 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/backends/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14116 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7963 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13203 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/backends/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7959 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/backends/text.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3014 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/backends/tracetab.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6961 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20763 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/data.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/distributions/
+-rw-r--r--   0 runner    (1001) docker     (116)     5261 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10833 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (116)   147600 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (116)    53088 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17562 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (116)    42018 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27402 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/mixture.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    73874 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30314 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/posterior_predictive.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14022 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5718 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1898 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/special.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17204 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15362 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/distributions/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)     1821 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/GHME_2013.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1638 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/LKJ_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      714 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/arbitrary_stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2112 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/arma_example.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1016 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/baseball.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3375 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/custom_dists.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (116)     2333 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/Guber1999data.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      927 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/HtWt.csv
+-rw-r--r--   0 runner    (1001) docker     (116)   131016 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/SP500.csv
+-rw-r--r--   0 runner    (1001) docker     (116)     6040 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/babies.csv
+-rw-r--r--   0 runner    (1001) docker     (116)   140076 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/cty.dat
+-rw-r--r--   0 runner    (1001) docker     (116)     1008 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/efron-morris-75-data.tsv
+-rw-r--r--   0 runner    (1001) docker     (116)    80080 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/extrahard_MC_500_5_4.npz.npy
+-rw-r--r--   0 runner    (1001) docker     (116)     4080 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/extrahard_MC_500_5_4_reference_classes.npy
+-rw-r--r--   0 runner    (1001) docker     (116)      575 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/mastectomy.csv
+-rw-r--r--   0 runner    (1001) docker     (116)     5181 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/merged_ice_core_yearly.csv
+-rw-r--r--   0 runner    (1001) docker     (116)      340 2020-08-11 03:30:43.000000 pymc3-3.9.3/pymc3/examples/data/milk.csv
+-rw-r--r--   0 runner    (1001) docker     (116)  1979173 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/ml_100k_u.data
+-rw-r--r--   0 runner    (1001) docker     (116)   236356 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/ml_100k_u.item
+-rw-r--r--   0 runner    (1001) docker     (116)    72328 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/monthly_in_situ_co2_mlo.csv
+-rw-r--r--   0 runner    (1001) docker     (116)     2271 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/old_faithful.csv
+-rw-r--r--   0 runner    (1001) docker     (116)    79411 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/pancreatitis.csv
+-rw-r--r--   0 runner    (1001) docker     (116)   157833 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/radon.csv
+-rw-r--r--   0 runner    (1001) docker     (116)     1740 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/rugby.csv
+-rw-r--r--   0 runner    (1001) docker     (116)  1637302 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/srrs2.dat
+-rw-r--r--   0 runner    (1001) docker     (116)    26978 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/stock_prices.csv
+-rw-r--r--   0 runner    (1001) docker     (116)     9222 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/sunspot.csv
+-rw-r--r--   0 runner    (1001) docker     (116)     9819 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/test_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (116)    98295 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/data/wells.dat
+-rw-r--r--   0 runner    (1001) docker     (116)     1623 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/disaster_model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2213 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/disaster_model_theano_op.py
+-rw-r--r--   0 runner    (1001) docker     (116)      553 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/factor_potential.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1430 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/garch_example.py
+-rw-r--r--   0 runner    (1001) docker     (116)      660 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/gelman_bioassay.py
+-rw-r--r--   0 runner    (1001) docker     (116)      943 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/gelman_schools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2005 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/lasso_missing.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1121 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/lightspeed_example.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1779 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/rankdata_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3301 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/samplers_mvnormal.py
+-rw-r--r--   0 runner    (1001) docker     (116)      509 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/examples/simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2314 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/glm/
+-rw-r--r--   0 runner    (1001) docker     (116)      668 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/glm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3830 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/glm/families.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7696 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/glm/linear.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4584 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/glm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/gp/
+-rw-r--r--   0 runner    (1001) docker     (116)      739 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23890 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (116)    44809 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2502 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5095 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12404 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/math.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2675 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (116)    66676 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8615 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/ode/
+-rw-r--r--   0 runner    (1001) docker     (116)      662 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9037 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4488 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/ode/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16815 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/parallel_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/plots/
+-rw-r--r--   0 runner    (1001) docker     (116)     3691 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2002 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/plots/posteriorplot.py
+-rw-r--r--   0 runner    (1001) docker     (116)    78689 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/smc/
+-rw-r--r--   0 runner    (1001) docker     (116)      639 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9556 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/smc/sample_smc.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13305 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/smc/smc.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/stats/
+-rw-r--r--   0 runner    (1001) docker     (116)     1879 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9387 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2689 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/compound.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4430 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/elliptical_slice.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2943 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/gibbs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (116)      658 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9124 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6470 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3723 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17918 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23094 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28126 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7106 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/sgmcmc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4208 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3015 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/step_methods/step_sizes.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      659 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22927 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/backend_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/checks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1458 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3254 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5380 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6150 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/sampler_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (116)      490 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_coords.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10531 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_data_container.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7652 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2433 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_distribution_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (116)    61596 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    51586 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_distributions_random.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5476 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_distributions_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12552 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6129 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_glm.py
+-rw-r--r--   0 runner    (1001) docker     (116)    46863 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_gp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2754 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_hdf5_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2507 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6823 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (116)      914 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_memo.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11958 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_minibatches.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3479 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_missing.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22514 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13783 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1949 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_model_func.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3219 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_model_graph.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6381 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_model_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3973 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_modelcontext.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5121 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_models_linear.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3507 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_models_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8335 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_ndarray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14276 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_ode.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4167 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_parallel_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1197 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1355 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_posdef_sym.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1357 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_posterior_predictive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2395 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1089 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9261 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6530 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37882 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8032 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_shape_handling.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2426 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7494 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_smc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1964 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_special_functions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2657 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_sqlite_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2689 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_starting.py
+-rw-r--r--   0 runner    (1001) docker     (116)    33916 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3010 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_text_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8967 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_theanof.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3169 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_tracetab.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15133 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1978 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2079 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2961 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_updates.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5340 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35997 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tests/test_variational_inference.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15487 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/theanof.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/tuning/
+-rw-r--r--   0 runner    (1001) docker     (116)      695 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3827 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9142 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6481 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3/variational/
+-rw-r--r--   0 runner    (1001) docker     (116)     1405 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20530 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4510 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17918 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/flows.py
+-rw-r--r--   0 runner    (1001) docker     (116)    31502 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4192 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (116)    61467 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3050 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1739 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/test_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    38659 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-08-11 03:30:44.000000 pymc3-3.9.3/pymc3/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    16079 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5727 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      191 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-08-11 03:30:55.000000 pymc3-3.9.3/pymc3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      213 2020-08-11 03:30:44.000000 pymc3-3.9.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-11 03:30:55.000000 pymc3-3.9.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (116)      882 2020-08-11 03:30:44.000000 pymc3-3.9.3/scripts/create_testenv.sh
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1442 2020-08-11 03:30:44.000000 pymc3-3.9.3/scripts/install_miniconda.sh
+-rwxr-xr-x   0 runner    (1001) docker     (116)       53 2020-08-11 03:30:44.000000 pymc3-3.9.3/scripts/lint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (116)      980 2020-08-11 03:30:44.000000 pymc3-3.9.3/scripts/start_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (116)      246 2020-08-11 03:30:44.000000 pymc3-3.9.3/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (116)      167 2020-08-11 03:30:55.000000 pymc3-3.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3048 2020-08-11 03:30:44.000000 pymc3-3.9.3/setup.py
```

### Comparing `pymc3-3.9.2/CODE_OF_CONDUCT.md` & `pymc3-3.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/CONTRIBUTING.md` & `pymc3-3.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/GOVERNANCE.md` & `pymc3-3.9.3/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/LICENSE` & `pymc3-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/RELEASE-NOTES.md` & `pymc3-3.9.3/RELEASE-NOTES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 # Release Notes
 
 ## PyMC3 3.9.x (on deck)
-*waiting for contributions*
+
+### Maintenance
+- Fix an error on Windows and Mac where error message from unpickling models did not show up in the notebook, or where sampling froze when a worker process crashed (see [#3991](https://github.com/pymc-devs/pymc3/pull/3991)).
+
+### Documentation
+- Notebook on [multilevel modeling](https://docs.pymc.io/notebooks/multilevel_modeling.html) has been rewritten to showcase ArviZ and xarray usage for inference result analysis (see [#3963](https://github.com/pymc-devs/pymc3/pull/3963))
+
+### New features
+- Introduce optional arguments to `pm.sample`: `mp_ctx` to control how the processes for parallel sampling are started, and `pickle_backend` to specify which library is used to pickle models in parallel sampling when the multiprocessing cnotext is not of type `fork`. (see [#3991](https://github.com/pymc-devs/pymc3/pull/3991))
+- Add sampler stats `process_time_diff`, `perf_counter_diff` and `perf_counter_start`, that record wall and CPU times for each NUTS and HMC sample (see [ #3986](https://github.com/pymc-devs/pymc3/pull/3986)).
+- Extend `keep_size` argument handling for `sample_posterior_predictive` and `fast_sample_posterior_predictive`, to work on arviz InferenceData and xarray Dataset input values. (see [PR #4006](https://github.com/pymc-devs/pymc3/pull/4006) and [Issue #4004](https://github.com/pymc-devs/pymc3/issues/4004).
+- SMC-ABC: add the wasserstein and energy distance functions. Refactor API, the distance, sum_stats and epsilon arguments are now passed `pm.Simulator` instead of `pm.sample_smc`. Add random method to `pm.Simulator`. Add option to save the simulated data. Improves LaTeX representation [#3996](https://github.com/pymc-devs/pymc3/pull/3996)
+- SMC-ABC: Allow use of potentials by adding them to the prior term. [#4016](https://github.com/pymc-devs/pymc3/pull/4016)
 
 ## PyMC3 3.9.2 (24 June 2020)
 ### Maintenance
 - Warning added in GP module when `input_dim` is lower than the number of columns in `X` to compute the covariance function (see [#3974](https://github.com/pymc-devs/pymc3/pull/3974)).
 - Pass the `tune` argument from `sample` when using `advi+adapt_diag_grad` (see issue [#3965](https://github.com/pymc-devs/pymc3/issues/3965), fixed by [#3979](https://github.com/pymc-devs/pymc3/pull/3979)).
-- Add simple test case for new coords and dims feature in `pm.Model` (see [#3977](https://github.com/pymc-devs/pymc3/pull/3977)). 
+- Add simple test case for new coords and dims feature in `pm.Model` (see [#3977](https://github.com/pymc-devs/pymc3/pull/3977)).
 - Require ArviZ >= 0.9.0 (see [#3977](https://github.com/pymc-devs/pymc3/pull/3977)).
+- Fixed issue [#3962](https://github.com/pymc-devs/pymc3/issues/3962) by making change in the `_random()` method of `GaussianRandomWalk` class, refer to PR [#3985]. Further testing revealed a new issue which is being tracked [#4010](https://github.com/pymc-devs/pymc3/issues/4010) 
 
 _NB: The `docs/*` folder is still removed from the tarball due to an upload size limit on PyPi._
 
 ## PyMC3 3.9.1 (16 June 2020)
 The `v3.9.0` upload to PyPI didn't include a tarball, which is fixed in this release.
 Though we had to temporarily remove the `docs/*` folder from the tarball due to a size limit.
```

### Comparing `pymc3-3.9.2/pymc3/__init__.py` & `pymc3-3.9.3/pymc3/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,44 +9,34 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 # pylint: disable=wildcard-import
-__version__ = "3.9.2"
+__version__ = "3.9.3"
 
 import logging
 import multiprocessing as mp
 import platform
 
 _log = logging.getLogger("pymc3")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
         _log.addHandler(handler)
 
-# Set start method to forkserver for MacOS to enable multiprocessing
-# Closes issue https://github.com/pymc-devs/pymc3/issues/3849
-sys = platform.system()
-if sys == "Darwin":
-    new_context = mp.get_context("forkserver")
-
 
 def __set_compiler_flags():
     # Workarounds for Theano compiler problems on various platforms
     import theano
-
-    system = platform.system()
-    if system == "Windows":
-        theano.config.mode = "FAST_COMPILE"
-    elif system == "Darwin":
-        theano.config.gcc.cxxflags = "-Wno-c++11-narrowing"
+    current = theano.config.gcc.cxxflags
+    theano.config.gcc.cxxflags = f"{current} -Wno-c++11-narrowing"
 
 
 __set_compiler_flags()
 
 from .blocking import *
 from .distributions import *
 from .distributions import transforms
```

### Comparing `pymc3-3.9.2/pymc3/backends/__init__.py` & `pymc3-3.9.3/pymc3/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/backends/base.py` & `pymc3-3.9.3/pymc3/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/backends/hdf5.py` & `pymc3-3.9.3/pymc3/backends/hdf5.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/backends/ndarray.py` & `pymc3-3.9.3/pymc3/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/backends/report.py` & `pymc3-3.9.3/pymc3/backends/report.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
-from collections import namedtuple
 import logging
 import enum
-import typing
+from typing import Any, Optional
+import dataclasses
+
 from ..util import is_transformed_name, get_untransformed_name
 
 import arviz
 
 logger = logging.getLogger('pymc3')
 
 
@@ -34,30 +35,39 @@
     BAD_PARAMS = 5
     # Indications that chains did not converge, eg Rhat
     CONVERGENCE = 6
     BAD_ACCEPTANCE = 7
     BAD_ENERGY = 8
 
 
-SamplerWarning = namedtuple(
-    'SamplerWarning',
-    "kind, message, level, step, exec_info, extra")
+@dataclasses.dataclass
+class SamplerWarning:
+    kind: WarningType
+    message: str
+    level: str
+    step: Optional[int] = None
+    exec_info: Optional[Any] = None
+    extra: Optional[Any] = None
+    divergence_point_source: Optional[dict] = None
+    divergence_point_dest: Optional[dict] = None
+    divergence_info: Optional[Any] = None
 
 
 _LEVELS = {
     'info': logging.INFO,
     'error': logging.ERROR,
     'warn': logging.WARN,
     'debug': logging.DEBUG,
     'critical': logging.CRITICAL,
 }
 
 
 class SamplerReport:
-    """This object bundles warnings, convergence statistics and metadata of a sampling run."""
+    """Bundle warnings, convergence stats and metadata of a sampling run."""
+
     def __init__(self):
         self._chain_warnings = {}
         self._global_warnings = []
         self._ess = None
         self._rhat = None
         self._n_tune = None
         self._n_draws = None
@@ -71,44 +81,50 @@
     @property
     def ok(self):
         """Whether the automatic convergence checks found serious problems."""
         return all(_LEVELS[warn.level] < _LEVELS['warn']
                    for warn in self._warnings)
 
     @property
-    def n_tune(self) -> typing.Optional[int]:
+    def n_tune(self) -> Optional[int]:
         """Number of tune iterations - not necessarily kept in trace!"""
         return self._n_tune
 
     @property
-    def n_draws(self) -> typing.Optional[int]:
+    def n_draws(self) -> Optional[int]:
         """Number of draw iterations."""
         return self._n_draws
 
     @property
-    def t_sampling(self) -> typing.Optional[float]:
+    def t_sampling(self) -> Optional[float]:
         """
         Number of seconds that the sampling procedure took.
 
         (Includes parallelization overhead.)
         """
         return self._t_sampling
 
     def raise_ok(self, level='error'):
         errors = [warn for warn in self._warnings
                   if _LEVELS[warn.level] >= _LEVELS[level]]
         if errors:
             raise ValueError('Serious convergence issues during sampling.')
 
-    def _run_convergence_checks(self, idata:arviz.InferenceData, model):
+    def _run_convergence_checks(self, idata: arviz.InferenceData, model):
+        if not hasattr(idata, 'posterior'):
+            msg = "No posterior samples. Unable to run convergence checks"
+            warn = SamplerWarning(WarningType.BAD_PARAMS, msg, 'info',
+                                  None, None, None)
+            self._add_warnings([warn])
+            return
+
         if idata.posterior.sizes['chain'] == 1:
             msg = ("Only one chain was sampled, this makes it impossible to "
                    "run some convergence checks")
-            warn = SamplerWarning(WarningType.BAD_PARAMS, msg, 'info',
-                                  None, None, None)
+            warn = SamplerWarning(WarningType.BAD_PARAMS, msg, 'info')
             self._add_warnings([warn])
             return
 
         valid_name = [rv.name for rv in model.free_RVs + model.deterministics]
         varnames = []
         for rv in model.free_RVs:
             rv_name = rv.name
@@ -123,49 +139,50 @@
 
         warnings = []
         rhat_max = max(val.max() for val in rhat.values())
         if rhat_max > 1.4:
             msg = ("The rhat statistic is larger than 1.4 for some "
                    "parameters. The sampler did not converge.")
             warn = SamplerWarning(
-                WarningType.CONVERGENCE, msg, 'error', None, None, rhat)
+                WarningType.CONVERGENCE, msg, 'error', extra=rhat)
             warnings.append(warn)
         elif rhat_max > 1.2:
             msg = ("The rhat statistic is larger than 1.2 for some "
                    "parameters.")
             warn = SamplerWarning(
-                WarningType.CONVERGENCE, msg, 'warn', None, None, rhat)
+                WarningType.CONVERGENCE, msg, 'warn', extra=rhat)
             warnings.append(warn)
         elif rhat_max > 1.05:
             msg = ("The rhat statistic is larger than 1.05 for some "
                    "parameters. This indicates slight problems during "
                    "sampling.")
             warn = SamplerWarning(
-                WarningType.CONVERGENCE, msg, 'info', None, None, rhat)
+                WarningType.CONVERGENCE, msg, 'info', extra=rhat)
             warnings.append(warn)
 
         eff_min = min(val.min() for val in ess.values())
-        n_samples = idata.posterior.sizes['chain'] * idata.posterior.sizes['draw']
+        sizes = idata.posterior.sizes
+        n_samples = sizes['chain'] * sizes['draw']
         if eff_min < 200 and n_samples >= 500:
             msg = ("The estimated number of effective samples is smaller than "
                    "200 for some parameters.")
             warn = SamplerWarning(
-                WarningType.CONVERGENCE, msg, 'error', None, None, ess)
+                WarningType.CONVERGENCE, msg, 'error', extra=ess)
             warnings.append(warn)
         elif eff_min / n_samples < 0.1:
             msg = ("The number of effective samples is smaller than "
                    "10% for some parameters.")
             warn = SamplerWarning(
-                WarningType.CONVERGENCE, msg, 'warn', None, None, ess)
+                WarningType.CONVERGENCE, msg, 'warn', extra=ess)
             warnings.append(warn)
         elif eff_min / n_samples < 0.25:
             msg = ("The number of effective samples is smaller than "
                    "25% for some parameters.")
             warn = SamplerWarning(
-                WarningType.CONVERGENCE, msg, 'info', None, None, ess)
+                WarningType.CONVERGENCE, msg, 'info', extra=ess)
             warnings.append(warn)
 
         self._add_warnings(warnings)
 
     def _add_warnings(self, warnings, chain=None):
         if chain is None:
             warn_list = self._global_warnings
@@ -190,15 +207,15 @@
         def filter_warns(warnings):
             filtered = []
             for warn in warnings:
                 if warn.step is None:
                     filtered.append(warn)
                 elif (start <= warn.step < stop and
                         (warn.step - start) % step == 0):
-                    warn = warn._replace(step=warn.step - start)
+                    warn = dataclasses.replace(warn, step=warn.step - start)
                     filtered.append(warn)
             return filtered
 
         report._add_warnings(filter_warns(self._global_warnings))
         for chain in self._chain_warnings:
             report._add_warnings(
                 filter_warns(self._chain_warnings[chain]),
```

### Comparing `pymc3-3.9.2/pymc3/backends/sqlite.py` & `pymc3-3.9.3/pymc3/backends/sqlite.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/backends/text.py` & `pymc3-3.9.3/pymc3/backends/text.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/backends/tracetab.py` & `pymc3-3.9.3/pymc3/backends/tracetab.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/blocking.py` & `pymc3-3.9.3/pymc3/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/data.py` & `pymc3-3.9.3/pymc3/data.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/distributions/__init__.py` & `pymc3-3.9.3/pymc3/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/distributions/bound.py` & `pymc3-3.9.3/pymc3/distributions/bound.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,16 +273,15 @@
 
     def __call__(self, name, *args, **kwargs):
         if "observed" in kwargs:
             raise ValueError(
                 "Observed Bound distributions are not supported. "
                 "If you want to model truncated data "
                 "you can use a pm.Potential in combination "
-                "with the cumulative probability function. See "
-                "pymc3/examples/censored_data.py for an example."
+                "with the cumulative probability function."
             )
 
         transform = kwargs.pop("transform", "infer")
         if issubclass(self.distribution, Continuous):
             return _ContinuousBounded(
                 name,
                 self.distribution,
```

### Comparing `pymc3-3.9.2/pymc3/distributions/continuous.py` & `pymc3-3.9.3/pymc3/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/distributions/discrete.py` & `pymc3-3.9.3/pymc3/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/distributions/dist_math.py` & `pymc3-3.9.3/pymc3/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/distributions/distribution.py` & `pymc3-3.9.3/pymc3/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/distributions/mixture.py` & `pymc3-3.9.3/pymc3/distributions/mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,21 @@
                 if 'mean' not in defaults:
                     defaults.append('mean')
             except AttributeError:
                 pass
         dtype = kwargs.pop('dtype', default_dtype)
 
         try:
-            comp_modes = self._comp_modes()
-            comp_mode_logps = self.logp(comp_modes)
-            self.mode = comp_modes[tt.argmax(w * comp_mode_logps, axis=-1)]
+            if isinstance(comp_dists, Distribution):
+                comp_mode_logps = comp_dists.logp(comp_dists.mode)
+            else:
+                comp_mode_logps = tt.stack([cd.logp(cd.mode) for cd in comp_dists])
+
+            mode_idx = tt.argmax(tt.log(w) + comp_mode_logps, axis=-1)
+            self.mode = self._comp_modes()[mode_idx]
 
             if 'mode' not in defaults:
                 defaults.append('mode')
         except (AttributeError, ValueError, IndexError):
             pass
 
         super().__init__(shape, dtype, defaults=defaults, *args, **kwargs)
@@ -423,15 +427,15 @@
 
         Returns
         -------
         TensorVariable
         """
         w = self.w
 
-        return bound(logsumexp(tt.log(w) + self._comp_logp(value), axis=-1),
+        return bound(logsumexp(tt.log(w) + self._comp_logp(value), axis=-1, keepdims=False),
                      w >= 0, w <= 1, tt.allclose(w.sum(axis=-1), 1),
                      broadcast_conditions=False)
 
     def random(self, point=None, size=None):
         """
         Draw random values from defined Mixture distribution.
```

### Comparing `pymc3-3.9.2/pymc3/distributions/multivariate.py` & `pymc3-3.9.3/pymc3/distributions/multivariate.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import numpy as np
 import scipy
 import theano
 import theano.tensor as tt
 
 from scipy import stats, linalg
 
+from theano.gof.op import get_test_value
 from theano.tensor.nlinalg import det, matrix_inverse, trace, eigh
 from theano.tensor.slinalg import Cholesky
 import pymc3 as pm
 
 from pymc3.theanof import floatX
 from . import transforms
 from pymc3.util import get_variable_name
@@ -483,30 +484,31 @@
     a: array
         Concentration parameters (a > 0).
     """
 
     def __init__(self, a, transform=transforms.stick_breaking,
                  *args, **kwargs):
 
-        if not isinstance(a, pm.model.TensorVariable):
-            if not isinstance(a, list) and not isinstance(a, np.ndarray):
-                raise TypeError(
-                    'The vector of concentration parameters (a) must be a python list '
-                    'or numpy array.')
-            a = np.array(a)
-            if (a <= 0).any():
-               raise ValueError("All concentration parameters (a) must be > 0.")
-
-        shape = np.atleast_1d(a.shape)[-1]
+        if kwargs.get('shape') is None:
+            warnings.warn(
+                (
+                    "Shape not explicitly set. "
+                    "Please, set the value using the `shape` keyword argument. "
+                    "Using the test value to infer the shape."
+                ),
+                DeprecationWarning
+            )
+            try:
+                kwargs['shape'] = get_test_value(tt.shape(a))
+            except AttributeError:
+                pass
 
-        kwargs.setdefault("shape", shape)
         super().__init__(transform=transform, *args, **kwargs)
 
         self.size_prefix = tuple(self.shape[:-1])
-        self.k = tt.as_tensor_variable(shape)
         self.a = a = tt.as_tensor_variable(a)
         self.mean = a / tt.sum(a)
 
         self.mode = tt.switch(tt.all(a > 1),
                               (a - 1) / tt.sum(a - 1),
                               np.nan)
 
@@ -565,22 +567,21 @@
         value: numeric
             Value for which log-probability is calculated.
 
         Returns
         -------
         TensorVariable
         """
-        k = self.k
         a = self.a
 
         # only defined for sum(value) == 1
         return bound(tt.sum(logpow(value, a - 1) - gammaln(a), axis=-1)
                      + gammaln(tt.sum(a, axis=-1)),
                      tt.all(value >= 0), tt.all(value <= 1),
-                     k > 1, tt.all(a > 0),
+                     np.logical_not(a.broadcastable), tt.all(a > 0),
                      broadcast_conditions=False)
 
     def _repr_latex_(self, name=None, dist=None):
         if dist is None:
             dist = self
         a = dist.a
         return r'${} \sim \text{{Dirichlet}}(\mathit{{a}}={})$'.format(name,
```

### Comparing `pymc3-3.9.2/pymc3/distributions/posterior_predictive.py` & `pymc3-3.9.3/pymc3/distributions/posterior_predictive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,147 +1,194 @@
 import numbers
-from typing import List, Dict, Any, Optional, Tuple, Union, cast, TYPE_CHECKING, Callable, overload
+from typing import (
+    List,
+    Dict,
+    Any,
+    Optional,
+    Tuple,
+    Union,
+    cast,
+    TYPE_CHECKING,
+    Callable,
+    overload,
+    Set,
+)
 import warnings
 import logging
 from collections import UserDict
 from contextlib import AbstractContextManager
-if TYPE_CHECKING:
-    import contextvars          # noqa: F401
-    from typing import Set
-from typing_extensions import Protocol
+import contextvars
+from typing_extensions import Protocol, Literal
 
 import numpy as np
 import theano
 import theano.tensor as tt
 from xarray import Dataset
+from arviz import InferenceData
 
-from ..backends.base import MultiTrace #, TraceLike, TraceDict
-from .distribution import _DrawValuesContext, _DrawValuesContextBlocker, is_fast_drawable, _compile_theano_function, vectorized_ppc
-from ..model import Model, get_named_nodes_and_relations, ObservedRV, MultiObservedRV, modelcontext
+from ..backends.base import MultiTrace
+from .distribution import (
+    _DrawValuesContext,
+    _DrawValuesContextBlocker,
+    is_fast_drawable,
+    _compile_theano_function,
+    vectorized_ppc,
+)
+from ..model import (
+    Model,
+    get_named_nodes_and_relations,
+    ObservedRV,
+    MultiObservedRV,
+    modelcontext,
+)
 from ..exceptions import IncorrectArgumentsError
 from ..vartypes import theano_constant
-from ..util import dataset_to_point_dict
+from ..util import dataset_to_point_dict, chains_and_samples
+
 # Failing tests:
 #    test_mixture_random_shape::test_mixture_random_shape
 #
 
 PosteriorPredictiveTrace = Dict[str, np.ndarray]
 Point = Dict[str, np.ndarray]
 
+
 class HasName(Protocol):
-    name = None                 # type: str
+    name: str
+
 
 if TYPE_CHECKING:
     _TraceDictParent = UserDict[str, np.ndarray]
 else:
     _TraceDictParent = UserDict
 
+
 class _TraceDict(_TraceDictParent):
     """This class extends the standard trace-based representation
     of traces by adding some helpful attributes used in posterior predictive
     sampling.
 
     Attributes
     ~~~~~~~~~~
         varnames: list of strings"""
 
-    varnames = None             # type: List[str]
-    _len = None                 # type: int
-    data = None                 # type: Dict[str, np.ndarray]
-    
-
-    def __init__(self, point_list: Optional[List[Dict[str, np.ndarray]]] = None, \
-                 multi_trace: Optional[MultiTrace] = None,
-                 dict: Optional[Dict[str, np.ndarray]] = None):
+    varnames: List[str]
+    _len: int
+    data: Dict[str, np.ndarray]
+
+    def __init__(
+        self,
+        point_list: Optional[List[Dict[str, np.ndarray]]] = None,
+        multi_trace: Optional[MultiTrace] = None,
+        dict: Optional[Dict[str, np.ndarray]] = None,
+    ):
         """
 
         """
         if multi_trace:
             assert point_list is None and dict is None
-            self.data = {}      # Dict[str, np.ndarray]
-            self._len = sum((len(multi_trace._straces[chain]) for chain in multi_trace.chains))
+            self.data = {}  # Dict[str, np.ndarray]
+            self._len = sum(
+                (len(multi_trace._straces[chain]) for chain in multi_trace.chains)
+            )
             self.varnames = multi_trace.varnames
             for vn in multi_trace.varnames:
                 self.data[vn] = multi_trace.get_values(vn)
         if point_list is not None:
             assert multi_trace is None and dict is None
             self.varnames = varnames = list(point_list[0].keys())
-            rep_values = [point_list[0][varname ]for varname in varnames]
+            rep_values = [point_list[0][varname] for varname in varnames]
             # translate the point list.
             self._len = num_points = len(point_list)
+
             def arr_for(val):
                 if np.isscalar(val):
                     return np.ndarray(shape=(num_points,))
                 elif isinstance(val, np.ndarray):
                     shp = (num_points,) + val.shape
                     return np.ndarray(shape=shp)
                 else:
-                    raise TypeError("Illegal object %s of type %s as value of variable in point list."%(val, type(val)))
+                    raise TypeError(
+                        "Illegal object %s of type %s as value of variable in point list."
+                        % (val, type(val))
+                    )
+
             self.data = {name: arr_for(val) for name, val in zip(varnames, rep_values)}
             for i, point in enumerate(point_list):
                 for var, value in point.items():
                     self.data[var][i] = value
         if dict is not None:
             assert point_list is None and multi_trace is None
             self.data = dict
             self.varnames = list(dict.keys())
             self._len = dict[self.varnames[0]].shape[0]
-        assert self.varnames is not None and self._len is not None and self.data is not None
+        assert (
+            self.varnames is not None
+            and self._len is not None
+            and self.data is not None
+        )
 
     def __len__(self) -> int:
         return self._len
 
-    def _extract_slice(self, slc: slice) -> '_TraceDict':
-        sliced_dict = {}        # type: Dict[str, np.ndarray]
+    def _extract_slice(self, slc: slice) -> "_TraceDict":
+        sliced_dict: Dict[str, np.ndarray] = {}
+
         def apply_slice(arr: np.ndarray) -> np.ndarray:
             if len(arr.shape) == 1:
                 return arr[slc]
             else:
-                return arr[slc,:]
+                return arr[slc, :]
+
         for vn, arr in self.data.items():
             sliced_dict[vn] = apply_slice(arr)
         return _TraceDict(dict=sliced_dict)
 
     @overload
-    def __getitem__(self, item: Union[str, HasName]) -> np.ndarray: ...
+    def __getitem__(self, item: Union[str, HasName]) -> np.ndarray:
+        ...
 
     @overload
-    def __getitem__(self, item: Union[slice, int]) -> '_TraceDict': ...
+    def __getitem__(self, item: Union[slice, int]) -> "_TraceDict":
+        ...
 
     def __getitem__(self, item):
         if isinstance(item, str):
             return super(_TraceDict, self).__getitem__(item)
         elif isinstance(item, slice):
             return self._extract_slice(item)
         elif isinstance(item, int):
-            return _TraceDict(dict={k: np.atleast_1d(v[item]) for k, v in self.data.items()})
-        elif hasattr(item, 'name'):
+            return _TraceDict(
+                dict={k: np.atleast_1d(v[item]) for k, v in self.data.items()}
+            )
+        elif hasattr(item, "name"):
             return super(_TraceDict, self).__getitem__(item.name)
         else:
-            raise IndexError("Illegal index %s for _TraceDict"%str(item))
-
+            raise IndexError("Illegal index %s for _TraceDict" % str(item))
 
 
-def fast_sample_posterior_predictive(trace: Union[MultiTrace, Dataset, List[Dict[str, np.ndarray]]],
-                                samples: Optional[int]=None,
-                                model: Optional[Model]=None,
-                                var_names: Optional[List[str]]=None,
-                                keep_size: bool=False,
-                                random_seed=None) -> Dict[str, np.ndarray]:
+def fast_sample_posterior_predictive(
+    trace: Union[MultiTrace, Dataset, InferenceData, List[Dict[str, np.ndarray]]],
+    samples: Optional[int] = None,
+    model: Optional[Model] = None,
+    var_names: Optional[List[str]] = None,
+    keep_size: bool = False,
+    random_seed=None,
+) -> Dict[str, np.ndarray]:
     """Generate posterior predictive samples from a model given a trace.
 
     This is a vectorized alternative to the standard ``sample_posterior_predictive`` function.
     It aims to be as compatible as possible with the original API, and is significantly
     faster.  Both posterior predictive sampling functions have some remaining issues, and
     we encourage users to verify agreement across the results of both functions for the time
     being.
 
     Parameters
     ----------
-    trace: MultiTrace, xarray.Dataset, or List of points (dictionary)
+    trace: MultiTrace, xarray.Dataset, InferenceData, or List of points (dictionary)
         Trace generated from MCMC sampling.
     samples: int, optional
         Number of posterior predictive samples to generate. Defaults to one posterior predictive
         sample per posterior sample, that is, the number of draws times the number of chains. It
         is not recommended to modify this value; when modified, some chains may not be represented
         in the posterior predictive sample.
     model: Model (optional if in `with` context)
@@ -166,291 +213,339 @@
     ### Canonicalizing the trace argument into a _TraceDict object and fitting it
     ### to the requested number of samples.  Then it invokes posterior_predictive_draw_values
     ### *repeatedly*.  It does this repeatedly, because the trace argument is set up to be
     ### the same as the number of samples. So if the number of samples requested is
     ### greater than the number of samples in the trace parameter, we sample repeatedly.  This
     ### makes the shape issues just a little easier to deal with.
 
-    if isinstance(trace, Dataset):
+    if isinstance(trace, InferenceData):
+        nchains, ndraws = chains_and_samples(trace)
+        trace = dataset_to_point_dict(trace.posterior)
+    elif isinstance(trace, Dataset):
+        nchains, ndraws = chains_and_samples(trace)
         trace = dataset_to_point_dict(trace)
+    elif isinstance(trace, MultiTrace):
+        nchains = trace.nchains
+        ndraws = len(trace)
+    else:
+        if keep_size:
+            # arguably this should be just a warning.
+            raise IncorrectArgumentsError(
+                "For keep_size, cannot identify chains and length from %s.", trace
+            )
 
     model = modelcontext(model)
     assert model is not None
     with model:
 
         if keep_size and samples is not None:
-            raise IncorrectArgumentsError("Should not specify both keep_size and samples arguments")
-        if keep_size and not isinstance(trace, MultiTrace):
-            # arguably this should be just a warning.
-            raise IncorrectArgumentsError("keep_size argument only applies when sampling from MultiTrace.")
+            raise IncorrectArgumentsError(
+                "Should not specify both keep_size and samples arguments"
+            )
 
         if isinstance(trace, list) and all((isinstance(x, dict) for x in trace)):
-           _trace = _TraceDict(point_list=trace)
+            _trace = _TraceDict(point_list=trace)
         elif isinstance(trace, MultiTrace):
             _trace = _TraceDict(multi_trace=trace)
         else:
-            raise TypeError("Unable to generate posterior predictive samples from argument of type %s"%type(trace))
+            raise TypeError(
+                "Unable to generate posterior predictive samples from argument of type %s"
+                % type(trace)
+            )
 
         len_trace = len(_trace)
 
         assert isinstance(_trace, _TraceDict)
 
-        _samples = [] # type: List[int]
+        _samples: List[int] = []
         # temporary replacement for more complicated logic.
         max_samples: int = len_trace
         if samples is None or samples == max_samples:
             _samples = [max_samples]
         elif samples < max_samples:
-            warnings.warn("samples parameter is smaller than nchains times ndraws, some draws "
-                          "and/or chains may not be represented in the returned posterior "
-                          "predictive sample")
+            warnings.warn(
+                "samples parameter is smaller than nchains times ndraws, some draws "
+                "and/or chains may not be represented in the returned posterior "
+                "predictive sample"
+            )
             # if this is less than the number of samples in the trace, take a slice and
             # work with that.
             _trace = _trace[slice(samples)]
             _samples = [samples]
         elif samples > max_samples:
             full, rem = divmod(samples, max_samples)
             _samples = (full * [max_samples]) + ([rem] if rem != 0 else [])
         else:
-            raise IncorrectArgumentsError("Unexpected combination of samples (%s) and max_samples (%d)"%(samples, max_samples))
+            raise IncorrectArgumentsError(
+                "Unexpected combination of samples (%s) and max_samples (%d)"
+                % (samples, max_samples)
+            )
 
         if var_names is None:
             vars = model.observed_RVs
         else:
             vars = [model[x] for x in var_names]
 
         if random_seed is not None:
             np.random.seed(random_seed)
 
         if TYPE_CHECKING:
             _ETPParent = UserDict[str, np.ndarray]  # this is only processed by mypy
         else:
-            _ETPParent = UserDict  # this is not seen by mypy but will be executed at runtime.
+            # this is not seen by mypy but will be executed at runtime.
+            _ETPParent = UserDict
 
         class _ExtendableTrace(_ETPParent):
             def extend_trace(self, trace: Dict[str, np.ndarray]) -> None:
                 for k, v in trace.items():
                     if k in self.data:
                         self.data[k] = np.concatenate((self.data[k], v))
                     else:
                         self.data[k] = v
 
-
         ppc_trace = _ExtendableTrace()
         for s in _samples:
             strace = _trace if s == len_trace else _trace[slice(0, s)]
             try:
-                values = posterior_predictive_draw_values(cast(List[Any], vars), strace, s)
-                new_trace = {k.name: v for (k, v) in zip(vars, values)}  # type: Dict[str, np.ndarray]
+                values = posterior_predictive_draw_values(
+                    cast(List[Any], vars), strace, s
+                )
+                new_trace: Dict[str, np.ndarray] = {
+                    k.name: v for (k, v) in zip(vars, values)
+                }
                 ppc_trace.extend_trace(new_trace)
             except KeyboardInterrupt:
                 pass
 
         if keep_size:
-            assert isinstance(trace, MultiTrace)
-            return {k: ary.reshape((trace.nchains, len(trace), *ary.shape[1:])) for k, ary in ppc_trace.items() }
-        else:
-            return ppc_trace.data # this gets us a Dict[str, np.ndarray] instead of my wrapped equiv.
+            return {
+                k: ary.reshape((nchains, ndraws, *ary.shape[1:]))
+                for k, ary in ppc_trace.items()
+            }
+        # this gets us a Dict[str, np.ndarray] instead of my wrapped equiv.
+        return ppc_trace.data
 
 
-def posterior_predictive_draw_values(vars: List[Any], trace: _TraceDict, samples: int) -> List[np.ndarray]:
+def posterior_predictive_draw_values(
+    vars: List[Any], trace: _TraceDict, samples: int
+) -> List[np.ndarray]:
     with _PosteriorPredictiveSampler(vars, trace, samples, None) as sampler:
         return sampler.draw_values()
 
+
 class _PosteriorPredictiveSampler(AbstractContextManager):
-    '''The process of posterior predictive sampling is quite complicated so this provides a central data store.'''
+    """The process of posterior predictive sampling is quite complicated so this provides a central data store."""
 
     # inputs
     vars: List[Any]
     trace: _TraceDict
     samples: int
-    size: Optional[int] # not supported!
+    size: Optional[int]  # not supported!
 
     # other slots
     logger: logging.Logger
 
     # for the search
     evaluated: Dict[int, np.ndarray]
     symbolic_params: List[Tuple[int, Any]]
 
     # set by make_graph...
     leaf_nodes: Dict[str, Any]
     named_nodes_parents: Dict[str, Any]
     named_nodes_children: Dict[str, Any]
-    _tok = None                  # type: contextvars.Token
-    
-    def __init__(self, vars, trace: _TraceDict, samples, model: Optional[Model], size=None):
+    _tok: contextvars.Token
+
+    def __init__(
+        self, vars, trace: _TraceDict, samples, model: Optional[Model], size=None
+    ):
         if size is not None:
-            raise NotImplementedError("sample_posterior_predictive does not support the size argument at this time.")
+            raise NotImplementedError(
+                "sample_posterior_predictive does not support the size argument at this time."
+            )
         assert vars is not None
         self.vars = vars
         self.trace = trace
         self.samples = samples
         self.size = size
-        self.logger = logging.getLogger('posterior_predictive')
+        self.logger = logging.getLogger("posterior_predictive")
 
-    def __enter__(self) -> '_PosteriorPredictiveSampler':
+    def __enter__(self) -> "_PosteriorPredictiveSampler":
         self._tok = vectorized_ppc.set(posterior_predictive_draw_values)
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> bool:
+    def __exit__(self, exc_type, exc_val, exc_tb) -> Literal[False]:
         vectorized_ppc.reset(self._tok)
         return False
-        
+
     def draw_values(self) -> List[np.ndarray]:
         vars = self.vars
         trace = self.trace
         samples = self.samples
         # size = self.size
         params = dict(enumerate(vars))
 
         with _DrawValuesContext() as context:
             self.init()
             self.make_graph()
 
             drawn = context.drawn_vars
 
             # Init givens and the stack of nodes to try to `_draw_value` from
-            givens = {p.name: (p, v) for (p, samples), v in drawn.items()
-                      if getattr(p, 'name', None) is not None}
+            givens = {
+                p.name: (p, v)
+                for (p, samples), v in drawn.items()
+                if getattr(p, "name", None) is not None
+            }
             stack = list(self.leaf_nodes.values())  # A queue would be more appropriate
 
             while stack:
                 next_ = stack.pop(0)
                 if (next_, samples) in drawn:
                     # If the node already has a givens value, skip it
                     continue
-                elif isinstance(next_, (theano_constant,
-                                        tt.sharedvar.SharedVariable)):
+                elif isinstance(next_, (theano_constant, tt.sharedvar.SharedVariable)):
                     # If the node is a theano.tensor.TensorConstant or a
                     # theano.tensor.sharedvar.SharedVariable, its value will be
                     # available automatically in _compile_theano_function so
                     # we can skip it. Furthermore, if this node was treated as a
                     # TensorVariable that should be compiled by theano in
                     # _compile_theano_function, it would raise a `TypeError:
                     # ('Constants not allowed in param list', ...)` for
                     # TensorConstant, and a `TypeError: Cannot use a shared
                     # variable (...) as explicit input` for SharedVariable.
                     # ObservedRV and MultiObservedRV instances are ViewOPs
                     # of TensorConstants or SharedVariables, we must add them
                     # to the stack or risk evaluating deterministics with the
                     # wrong values (issue #3354)
-                    stack.extend([node for node in self.named_nodes_parents[next_]
-                                  if isinstance(node, (ObservedRV,
-                                                       MultiObservedRV))
-                                  and (node, samples) not in drawn])
+                    stack.extend(
+                        [
+                            node
+                            for node in self.named_nodes_parents[next_]
+                            if isinstance(node, (ObservedRV, MultiObservedRV))
+                            and (node, samples) not in drawn
+                        ]
+                    )
                     continue
                 else:
                     # If the node does not have a givens value, try to draw it.
                     # The named node's children givens values must also be taken
                     # into account.
                     children = self.named_nodes_children[next_]
                     temp_givens = [givens[k] for k in givens if k in children]
                     try:
                         # This may fail for autotransformed RVs, which don't
                         # have the random method
-                        value = self.draw_value(next_,
-                                                trace=trace,
-                                                givens=temp_givens)
+                        value = self.draw_value(next_, trace=trace, givens=temp_givens)
                         assert isinstance(value, np.ndarray)
                         givens[next_.name] = (next_, value)
                         drawn[(next_, samples)] = value
                     except theano.gof.fg.MissingInputError:
                         # The node failed, so we must add the node's parents to
                         # the stack of nodes to try to draw from. We exclude the
                         # nodes in the `params` list.
-                        stack.extend([node for node in self.named_nodes_parents[next_]
-                                      if node is not None and
-                                      (node, samples) not in drawn])
-
+                        stack.extend(
+                            [
+                                node
+                                for node in self.named_nodes_parents[next_]
+                                if node is not None and (node, samples) not in drawn
+                            ]
+                        )
 
             # the below makes sure the graph is evaluated in order
             # test_distributions_random::TestDrawValues::test_draw_order fails without it
             # The remaining params that must be drawn are all hashable
-            to_eval = set() # type: Set[int]
-            missing_inputs = set([j for j, p in self.symbolic_params]) # type: Set[int]
+            to_eval: Set[int] = set()
+            missing_inputs: Set[int] = set([j for j, p in self.symbolic_params])
 
             while to_eval or missing_inputs:
                 if to_eval == missing_inputs:
-                    raise ValueError('Cannot resolve inputs for {}'.format([str(trace.varnames[j]) for j in to_eval]))
+                    raise ValueError(
+                        "Cannot resolve inputs for {}".format(
+                            [str(trace.varnames[j]) for j in to_eval]
+                        )
+                    )
                 to_eval = set(missing_inputs)
                 missing_inputs = set()
                 for param_idx in to_eval:
                     param = vars[param_idx]
                     drawn = context.drawn_vars
                     if (param, samples) in drawn:
                         self.evaluated[param_idx] = drawn[(param, samples)]
                     else:
                         try:
                             if param in self.named_nodes_children:
                                 for node in self.named_nodes_children[param]:
                                     if (
-                                        node.name not in givens and
-                                        (node, samples) in drawn
+                                        node.name not in givens
+                                        and (node, samples) in drawn
                                     ):
                                         givens[node.name] = (
                                             node,
-                                            drawn[(node, samples)]
+                                            drawn[(node, samples)],
                                         )
-                            value = self.draw_value(param,
-                                                    trace=self.trace,
-                                                    givens=givens.values())
+                            value = self.draw_value(
+                                param, trace=self.trace, givens=givens.values()
+                            )
                             assert isinstance(value, np.ndarray)
                             self.evaluated[param_idx] = drawn[(param, samples)] = value
                             givens[param.name] = (param, value)
                         except theano.gof.fg.MissingInputError:
                             missing_inputs.add(param_idx)
         return [self.evaluated[j] for j in params]
 
-
     def init(self) -> None:
-        '''This method carries out the initialization phase of sampling 
+        """This method carries out the initialization phase of sampling 
     from the posterior predictive distribution.  Notably it initializes the
     ``_DrawValuesContext`` bookkeeping object and evaluates the "fast drawable"
-    parts of the model.'''
+    parts of the model."""
         vars: List[Any] = self.vars
         trace: _TraceDict = self.trace
         samples: int = self.samples
+        leaf_nodes: Dict[str, Any]
+        named_nodes_parents: Dict[str, Any]
+        named_nodes_children: Dict[str, Any]
 
         # initialization phase
         context = _DrawValuesContext.get_context()
         assert isinstance(context, _DrawValuesContext)
         with context:
             drawn = context.drawn_vars
-            evaluated = {} # type: Dict[int, Any]
+            evaluated: Dict[int, Any] = {}
             symbolic_params = []
             for i, var in enumerate(vars):
                 if is_fast_drawable(var):
                     evaluated[i] = self.draw_value(var)
                     continue
-                name = getattr(var, 'name', None)
+                name = getattr(var, "name", None)
                 if (var, samples) in drawn:
                     evaluated[i] = drawn[(var, samples)]
-                                # We filter out Deterministics by checking for `model` attribute
-                elif name is not None and hasattr(var, 'model') and name in trace.varnames:
+                    # We filter out Deterministics by checking for `model` attribute
+                elif (
+                    name is not None
+                    and hasattr(var, "model")
+                    and name in trace.varnames
+                ):
                     # param.name is in the trace.  Record it as drawn and evaluated
                     drawn[(var, samples)] = evaluated[i] = trace[cast(str, name)]
                 else:
                     # param still needs to be drawn
                     symbolic_params.append((i, var))
         self.evaluated = evaluated
         self.symbolic_params = symbolic_params
 
-
-
     def make_graph(self) -> None:
         # Distribution parameters may be nodes which have named node-inputs
         # specified in the point. Need to find the node-inputs, their
         # parents and children to replace them.
         symbolic_params = self.symbolic_params
-        self.leaf_nodes = {} # type: Dict[str, Any]
-        self.named_nodes_parents = {} # type: Dict[str, Any]
-        self.named_nodes_children = {} # type: Dict[str, Any]
+        self.leaf_nodes = {}
+        self.named_nodes_parents = {}
+        self.named_nodes_children = {}
         for _, param in symbolic_params:
-            if hasattr(param, 'name'):
+            if hasattr(param, "name"):
                 # Get the named nodes under the `param` node
                 nn, nnp, nnc = get_named_nodes_and_relations(param)
                 self.leaf_nodes.update(nn)
                 # Update the discovered parental relationships
                 for k in nnp.keys():
                     if k not in self.named_nodes_parents.keys():
                         self.named_nodes_parents[k] = nnp[k]
@@ -459,15 +554,15 @@
                 # Update the discovered child relationships
                 for k in nnc.keys():
                     if k not in self.named_nodes_children.keys():
                         self.named_nodes_children[k] = nnc[k]
                     else:
                         self.named_nodes_children[k].update(nnc[k])
 
-    def draw_value(self, param, trace: Optional[_TraceDict]=None, givens=None):
+    def draw_value(self, param, trace: Optional[_TraceDict] = None, givens=None):
         """Draw a set of random values from a distribution or return a constant.
 
         Parameters
         ----------
         param: number, array like, theano variable or pymc3 random variable
             The value or distribution. Constants or shared variables
             will be converted to an array and returned. Theano variables
@@ -479,133 +574,173 @@
             used to provide context for evaluating ``param``.
         givens: dict, optional
             A dictionary from theano variables to their values. These values
             are used to evaluate ``param`` if it is a theano variable.
         """
         samples = self.samples
 
-        def random_sample(meth: Callable[..., np.ndarray], param, point: _TraceDict, size: int, shape: Tuple[int, ...]) -> np.ndarray:
+        def random_sample(
+            meth: Callable[..., np.ndarray],
+            param,
+            point: _TraceDict,
+            size: int,
+            shape: Tuple[int, ...],
+        ) -> np.ndarray:
             val = meth(point=point, size=size)
             if size == 1:
                 val = np.expand_dims(val, axis=0)
             try:
-                assert val.shape == (size, ) + shape, "Sampling from random of %s yields wrong shape"%param
+                assert val.shape == (size,) + shape, (
+                    "Sampling from random of %s yields wrong shape" % param
+                )
             # error-quashing here is *extremely* ugly, but it seems to be what the logic in DensityDist wants.
             except AssertionError as e:
-                if hasattr(param, 'distribution') and hasattr(param.distribution, 'wrap_random_with_dist_shape') \
-                   and not param.distribution.wrap_random_with_dist_shape:
+                if (
+                    hasattr(param, "distribution")
+                    and hasattr(param.distribution, "wrap_random_with_dist_shape")
+                    and not param.distribution.wrap_random_with_dist_shape
+                ):
                     pass
                 else:
                     raise e
-                
+
             return val
 
         if isinstance(param, (numbers.Number, np.ndarray)):
             return param
         elif isinstance(param, theano_constant):
             return param.value
         elif isinstance(param, tt.sharedvar.SharedVariable):
             return param.get_value()
         elif isinstance(param, (tt.TensorVariable, MultiObservedRV)):
-            if hasattr(param, 'model') and trace and param.name in trace.varnames:
+            if hasattr(param, "model") and trace and param.name in trace.varnames:
                 return trace[param.name]
-            elif hasattr(param, 'random') and param.random is not None:
+            elif hasattr(param, "random") and param.random is not None:
                 model = modelcontext(None)
                 assert isinstance(model, Model)
-                shape = tuple(_param_shape(param, model)) # type: Tuple[int, ...]
-                return random_sample(param.random, param, point=trace, size=samples, shape=shape)
-            elif (hasattr(param, 'distribution') and
-                    hasattr(param.distribution, 'random') and
-                    param.distribution.random is not None):
-                if hasattr(param, 'observations'):
+                shape: Tuple[int, ...] = tuple(_param_shape(param, model))
+                return random_sample(
+                    param.random, param, point=trace, size=samples, shape=shape
+                )
+            elif (
+                hasattr(param, "distribution")
+                and hasattr(param.distribution, "random")
+                and param.distribution.random is not None
+            ):
+                if hasattr(param, "observations"):
                     # shape inspection for ObservedRV
                     dist_tmp = param.distribution
                     try:
-                        distshape = tuple(param.observations.shape.eval()) # type: Tuple[int, ...]
+                        distshape: Tuple[int, ...] = tuple(
+                            param.observations.shape.eval()
+                        )
                     except AttributeError:
                         distshape = tuple(param.observations.shape)
 
                     dist_tmp.shape = distshape
                     try:
-                        return random_sample(dist_tmp.random, param, point=trace, size=samples, shape=distshape)
+                        return random_sample(
+                            dist_tmp.random,
+                            param,
+                            point=trace,
+                            size=samples,
+                            shape=distshape,
+                        )
                     except (ValueError, TypeError):
                         # reset shape to account for shape changes
                         # with theano.shared inputs
                         dist_tmp.shape = ()
                         # We want to draw values to infer the dist_shape,
                         # we don't want to store these drawn values to the context
                         with _DrawValuesContextBlocker():
                             point = trace[0] if trace else None
-                            temp_val = np.atleast_1d(dist_tmp.random(point=point, size=None))
+                            temp_val = np.atleast_1d(
+                                dist_tmp.random(point=point, size=None)
+                            )
                         # if hasattr(param, 'name') and param.name == 'obs':
                         #     import pdb; pdb.set_trace()
                         # Sometimes point may change the size of val but not the
                         # distribution's shape
                         if point and samples is not None:
                             temp_size = np.atleast_1d(samples)
-                            if all(temp_val.shape[:len(temp_size)] == temp_size):
-                                dist_tmp.shape = tuple(temp_val.shape[len(temp_size):])
+                            if all(temp_val.shape[: len(temp_size)] == temp_size):
+                                dist_tmp.shape = tuple(temp_val.shape[len(temp_size) :])
                             else:
                                 dist_tmp.shape = tuple(temp_val.shape)
                         # I am not sure why I need to do this, but I do in order to trim off a
                         # degenerate dimension [2019/09/05:rpg]
                         if dist_tmp.shape[0] == 1 and len(dist_tmp.shape) > 1:
                             dist_tmp.shape = dist_tmp.shape[1:]
-                        return random_sample(dist_tmp.random, point=trace, size=samples, param=param, shape=tuple(dist_tmp.shape))
-                else: # has a distribution, but no observations
+                        return random_sample(
+                            dist_tmp.random,
+                            point=trace,
+                            size=samples,
+                            param=param,
+                            shape=tuple(dist_tmp.shape),
+                        )
+                else:  # has a distribution, but no observations
                     distshape = tuple(param.distribution.shape)
-                    return random_sample(meth=param.distribution.random, param=param, point=trace, size=samples, shape=distshape)
+                    return random_sample(
+                        meth=param.distribution.random,
+                        param=param,
+                        point=trace,
+                        size=samples,
+                        shape=distshape,
+                    )
             # NOTE: I think the following is already vectorized.
-            else: 
+            else:
                 if givens:
                     variables, values = list(zip(*givens))
                 else:
                     variables = values = []
                 # We only truly care if the ancestors of param that were given
                 # value have the matching dshape and val.shape
-                param_ancestors = \
-                    set(theano.gof.graph.ancestors([param],
-                                                   blockers=list(variables))
-                        )
-                inputs = [(var, val) for var, val in
-                          zip(variables, values)
-                          if var in param_ancestors]
+                param_ancestors = set(
+                    theano.gof.graph.ancestors([param], blockers=list(variables))
+                )
+                inputs = [
+                    (var, val)
+                    for var, val in zip(variables, values)
+                    if var in param_ancestors
+                ]
                 if inputs:
                     input_vars, input_vals = list(zip(*inputs))
                 else:
                     input_vars = []
                     input_vals = []
                 func = _compile_theano_function(param, input_vars)
                 if not input_vars:
-                    assert input_vals == []  # AFAICT if there are now vars, there can't be vals
+                    assert (
+                        input_vals == []
+                    )  # AFAICT if there are now vars, there can't be vals
                     output = func(*input_vals)
-                    if hasattr(output, 'shape'):
+                    if hasattr(output, "shape"):
                         val = np.repeat(np.expand_dims(output, 0), samples, axis=0)
                     else:
                         val = np.full(samples, output)
 
                 else:
                     val = func(*input_vals)
                     # np.ndarray([func(*input_vals) for inp in zip(*input_vals)])
                 return val
-        raise ValueError('Unexpected type in draw_value: %s' % type(param))
+        raise ValueError("Unexpected type in draw_value: %s" % type(param))
 
 
 def _param_shape(var_desig, model: Model) -> Tuple[int, ...]:
     if isinstance(var_desig, str):
         v = model[var_desig]
     else:
-        v = var_desig                                                                          
-    if hasattr(v, 'observations'):
+        v = var_desig
+    if hasattr(v, "observations"):
         try:
             # To get shape of _observed_ data container `pm.Data`
             # (wrapper for theano.SharedVariable) we evaluate it.
             shape = tuple(v.observations.shape.eval())
         except AttributeError:
             shape = v.observations.shape
-    elif hasattr(v, 'dshape'):
+    elif hasattr(v, "dshape"):
         shape = v.dshape
     else:
         shape = v.tag.test_value.shape
     if shape == (1,):
         shape = tuple()
     return shape
```

### Comparing `pymc3-3.9.2/pymc3/distributions/shape_utils.py` & `pymc3-3.9.3/pymc3/distributions/shape_utils.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/distributions/special.py` & `pymc3-3.9.3/pymc3/distributions/special.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/distributions/timeseries.py` & `pymc3-3.9.3/pymc3/distributions/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #   limitations under the License.
 
 import warnings
 
 from scipy import stats
 import theano.tensor as tt
 from theano import scan
+import numpy as np
 
 from pymc3.util import get_variable_name
 from .continuous import get_tau_sigma, Normal, Flat
 from .shape_utils import to_tuple
 from . import multivariate
 from . import distribution
 
@@ -299,22 +300,31 @@
             mu=mu,
             size=size,
             dist_shape=self.shape,
             not_broadcast_kwargs={"sample_shape": to_tuple(size)},
         )
 
     def _random(self, sigma, mu, size, sample_shape):
-        """Implement a Gaussian random walk as a cumulative sum of normals."""
+        """Implement a Gaussian random walk as a cumulative sum of normals.
+        axis = len(size) - 1 denotes the axis along which cumulative sum would be calculated.
+        This might need to be corrected in future when issue #4010 is fixed.
+        Lines 318-322 ties the starting point of each instance of random walk to 0"
+        """
         if size[len(sample_shape)] == sample_shape:
             axis = len(sample_shape)
         else:
-            axis = 0
+            axis = len(size) - 1
         rv = stats.norm(mu, sigma)
         data = rv.rvs(size).cumsum(axis=axis)
-        data = data - data[0]  # TODO: this should be a draw from `init`, if available
+        data = np.array(data)
+        if len(data.shape)>1:
+            for i in range(data.shape[0]):
+                data[i] = data[i] - data[i][0]
+        else:
+            data = data - data[0]
         return data
 
     def _repr_latex_(self, name=None, dist=None):
         if dist is None:
             dist = self
         mu = dist.mu
         sigma = dist.sigma
```

### Comparing `pymc3-3.9.2/pymc3/distributions/transforms.py` & `pymc3-3.9.3/pymc3/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/GHME_2013.py` & `pymc3-3.9.3/pymc3/examples/GHME_2013.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/LKJ_correlation.py` & `pymc3-3.9.3/pymc3/examples/LKJ_correlation.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/arbitrary_stochastic.py` & `pymc3-3.9.3/pymc3/examples/arbitrary_stochastic.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/arma_example.py` & `pymc3-3.9.3/pymc3/examples/arma_example.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/baseball.py` & `pymc3-3.9.3/pymc3/examples/baseball.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/custom_dists.py` & `pymc3-3.9.3/pymc3/examples/custom_dists.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/Guber1999data.txt` & `pymc3-3.9.3/pymc3/examples/data/Guber1999data.txt`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/HtWt.csv` & `pymc3-3.9.3/pymc3/examples/data/HtWt.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/SP500.csv` & `pymc3-3.9.3/pymc3/examples/data/SP500.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/babies.csv` & `pymc3-3.9.3/pymc3/examples/data/babies.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/cty.dat` & `pymc3-3.9.3/pymc3/examples/data/cty.dat`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/efron-morris-75-data.tsv` & `pymc3-3.9.3/pymc3/examples/data/efron-morris-75-data.tsv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/extrahard_MC_500_5_4.npz.npy` & `pymc3-3.9.3/pymc3/examples/data/extrahard_MC_500_5_4.npz.npy`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/extrahard_MC_500_5_4_reference_classes.npy` & `pymc3-3.9.3/pymc3/examples/data/extrahard_MC_500_5_4_reference_classes.npy`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/mastectomy.csv` & `pymc3-3.9.3/pymc3/examples/data/mastectomy.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/merged_ice_core_yearly.csv` & `pymc3-3.9.3/pymc3/examples/data/merged_ice_core_yearly.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/ml_100k_u.data` & `pymc3-3.9.3/pymc3/examples/data/ml_100k_u.data`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/ml_100k_u.item` & `pymc3-3.9.3/pymc3/examples/data/ml_100k_u.item`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/monthly_in_situ_co2_mlo.csv` & `pymc3-3.9.3/pymc3/examples/data/monthly_in_situ_co2_mlo.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/old_faithful.csv` & `pymc3-3.9.3/pymc3/examples/data/old_faithful.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/pancreatitis.csv` & `pymc3-3.9.3/pymc3/examples/data/pancreatitis.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/radon.csv` & `pymc3-3.9.3/pymc3/examples/data/radon.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/rugby.csv` & `pymc3-3.9.3/pymc3/examples/data/rugby.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/srrs2.dat` & `pymc3-3.9.3/pymc3/examples/data/srrs2.dat`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/stock_prices.csv` & `pymc3-3.9.3/pymc3/examples/data/stock_prices.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/sunspot.csv` & `pymc3-3.9.3/pymc3/examples/data/sunspot.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/test_scores.csv` & `pymc3-3.9.3/pymc3/examples/data/test_scores.csv`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/data/wells.dat` & `pymc3-3.9.3/pymc3/examples/data/wells.dat`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/disaster_model.py` & `pymc3-3.9.3/pymc3/examples/disaster_model.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/disaster_model_theano_op.py` & `pymc3-3.9.3/pymc3/examples/disaster_model_theano_op.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/factor_potential.py` & `pymc3-3.9.3/pymc3/examples/factor_potential.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/garch_example.py` & `pymc3-3.9.3/pymc3/examples/garch_example.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/gelman_bioassay.py` & `pymc3-3.9.3/pymc3/examples/gelman_bioassay.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/gelman_schools.py` & `pymc3-3.9.3/pymc3/examples/gelman_schools.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/lasso_missing.py` & `pymc3-3.9.3/pymc3/examples/lasso_missing.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/lightspeed_example.py` & `pymc3-3.9.3/pymc3/examples/lightspeed_example.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/rankdata_ordered.py` & `pymc3-3.9.3/pymc3/examples/rankdata_ordered.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/examples/samplers_mvnormal.py` & `pymc3-3.9.3/pymc3/examples/samplers_mvnormal.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/exceptions.py` & `pymc3-3.9.3/pymc3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/glm/__init__.py` & `pymc3-3.9.3/pymc3/glm/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/glm/families.py` & `pymc3-3.9.3/pymc3/glm/families.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/glm/linear.py` & `pymc3-3.9.3/pymc3/glm/linear.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/glm/utils.py` & `pymc3-3.9.3/pymc3/glm/utils.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/gp/__init__.py` & `pymc3-3.9.3/pymc3/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/gp/cov.py` & `pymc3-3.9.3/pymc3/gp/cov.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,14 +349,25 @@
 
 class Periodic(Stationary):
     r"""
     The Periodic kernel.
 
     .. math::
        k(x, x') = \mathrm{exp}\left( -\frac{\mathrm{sin}^2(\pi |x-x'| \frac{1}{T})}{2\ell^2} \right)
+
+    Notes
+    -----
+    Note that the scaling factor for this kernel is different compared to the more common
+    definition (see [1]_). Here, 0.5 is in the exponent instead of the more common value, 2.
+    Divide the length-scale by 2 when initializing the kernel to recover the standard definition.
+
+    References
+    ----------
+    .. [1] David Duvenaud, "The Kernel Cookbook"
+       https://www.cs.toronto.edu/~duvenaud/cookbook/
     """
 
     def __init__(self, input_dim, period, ls=None, ls_inv=None, active_dims=None):
         super().__init__(input_dim, ls, ls_inv, active_dims)
         self.period = period
 
     def full(self, X, Xs=None):
```

### Comparing `pymc3-3.9.2/pymc3/gp/gp.py` & `pymc3-3.9.3/pymc3/gp/gp.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/gp/mean.py` & `pymc3-3.9.3/pymc3/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/gp/util.py` & `pymc3-3.9.3/pymc3/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/math.py` & `pymc3-3.9.3/pymc3/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,18 +164,19 @@
     Temporary function to silence round warning in Theano. Please remove
     when the warning disappears.
     """
     kwargs["mode"] = "half_to_even"
     return tt.round(*args, **kwargs)
 
 
-def logsumexp(x, axis=None):
+def logsumexp(x, axis=None, keepdims=True):
     # Adapted from https://github.com/Theano/Theano/issues/1563
     x_max = tt.max(x, axis=axis, keepdims=True)
-    return tt.log(tt.sum(tt.exp(x - x_max), axis=axis, keepdims=True)) + x_max
+    res = tt.log(tt.sum(tt.exp(x - x_max), axis=axis, keepdims=True)) + x_max
+    return res if keepdims else res.squeeze()
 
 
 def logaddexp(a, b):
     diff = b - a
     return tt.switch(diff > 0, b + tt.log1p(tt.exp(-diff)), a + tt.log1p(tt.exp(diff)))
```

### Comparing `pymc3-3.9.2/pymc3/memoize.py` & `pymc3-3.9.3/pymc3/memoize.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/model.py` & `pymc3-3.9.3/pymc3/model.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/model_graph.py` & `pymc3-3.9.3/pymc3/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/ode/__init__.py` & `pymc3-3.9.3/pymc3/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/ode/ode.py` & `pymc3-3.9.3/pymc3/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/ode/utils.py` & `pymc3-3.9.3/pymc3/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/parallel_sampling.py` & `pymc3-3.9.3/pymc3/parallel_sampling.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,58 +13,28 @@
 #   limitations under the License.
 
 import multiprocessing
 import multiprocessing.sharedctypes
 import ctypes
 import time
 import logging
+import pickle
 from collections import namedtuple
 import traceback
+import platform
 from pymc3.exceptions import SamplingError
-import errno
 
 import numpy as np
 from fastprogress.fastprogress import progress_bar
 
 from . import theanof
 
 logger = logging.getLogger("pymc3")
 
 
-def _get_broken_pipe_exception():
-    import sys
-
-    if sys.platform == "win32":
-        return RuntimeError(
-            "The communication pipe between the main process "
-            "and its spawned children is broken.\n"
-            "In Windows OS, this usually means that the child "
-            "process raised an exception while it was being "
-            "spawned, before it was setup to communicate to "
-            "the main process.\n"
-            "The exceptions raised by the child process while "
-            "spawning cannot be caught or handled from the "
-            "main process, and when running from an IPython or "
-            "jupyter notebook interactive kernel, the child's "
-            "exception and traceback appears to be lost.\n"
-            "A known way to see the child's error, and try to "
-            "fix or handle it, is to run the problematic code "
-            "as a batch script from a system's Command Prompt. "
-            "The child's exception will be printed to the "
-            "Command Promt's stderr, and it should be visible "
-            "above this error and traceback.\n"
-            "Note that if running a jupyter notebook that was "
-            "invoked from a Command Prompt, the child's "
-            "exception should have been printed to the Command "
-            "Prompt on which the notebook is running."
-        )
-    else:
-        return None
-
-
 class ParallelSamplingError(Exception):
     def __init__(self, message, chain, warnings=None):
         super().__init__(message)
         if warnings is None:
             warnings = []
         self._chain = chain
         self._warnings = warnings
@@ -100,34 +70,73 @@
 # ('error', warnings, *exception_info)
 
 # ('abort', reason)
 # ('write_next',)
 # ('start',)
 
 
-class _Process(multiprocessing.Process):
+class _Process:
     """Seperate process for each chain.
     We communicate with the main process using a pipe,
     and send finished samples using shared memory.
     """
 
-    def __init__(self, name:str, msg_pipe, step_method, shared_point, draws:int, tune:int, seed):
-        super().__init__(daemon=True, name=name)
+    def __init__(
+        self,
+        name: str,
+        msg_pipe,
+        step_method,
+        step_method_is_pickled,
+        shared_point,
+        draws: int,
+        tune: int,
+        seed,
+        pickle_backend,
+    ):
         self._msg_pipe = msg_pipe
         self._step_method = step_method
+        self._step_method_is_pickled = step_method_is_pickled
         self._shared_point = shared_point
         self._seed = seed
         self._tt_seed = seed + 1
         self._draws = draws
         self._tune = tune
+        self._pickle_backend = pickle_backend
+
+    def _unpickle_step_method(self):
+        unpickle_error = (
+            "The model could not be unpickled. This is required for sampling "
+            "with more than one core and multiprocessing context spawn "
+            "or forkserver."
+        )
+        if self._step_method_is_pickled:
+            if self._pickle_backend == 'pickle':
+                try:
+                    self._step_method = pickle.loads(self._step_method)
+                except Exception:
+                    raise ValueError(unpickle_error)
+            elif self._pickle_backend == 'dill':
+                try:
+                    import dill
+                except ImportError:
+                    raise ValueError(
+                        "dill must be installed for pickle_backend='dill'."
+                    )
+                try:
+                    self._step_method = dill.loads(self._step_method)
+                except Exception:
+                    raise ValueError(unpickle_error)
+            else:
+                raise ValueError("Unknown pickle backend")
 
     def run(self):
         try:
             # We do not create this in __init__, as pickling this
             # would destroy the shared memory.
+            self._unpickle_step_method()
             self._point = self._make_numpy_refs()
             self._start_loop()
         except KeyboardInterrupt:
             pass
         except BaseException as e:
             e = ExceptionWithTraceback(e, e.__traceback__)
             # Send is not blocking so we have to force a wait for the abort
@@ -215,81 +224,123 @@
     def _collect_warnings(self):
         if hasattr(self._step_method, "warnings"):
             return self._step_method.warnings()
         else:
             return []
 
 
+def _run_process(*args):
+    _Process(*args).run()
+
+
 class ProcessAdapter:
     """Control a Chain process from the main thread."""
 
-    def __init__(self, draws:int, tune:int, step_method, chain:int, seed, start):
+    def __init__(
+        self,
+        draws: int,
+        tune: int,
+        step_method,
+        step_method_pickled,
+        chain: int,
+        seed,
+        start,
+        mp_ctx,
+        pickle_backend,
+    ):
         self.chain = chain
         process_name = "worker_chain_%s" % chain
         self._msg_pipe, remote_conn = multiprocessing.Pipe()
 
         self._shared_point = {}
         self._point = {}
         for name, (shape, dtype) in step_method.vars_shape_dtype.items():
             size = 1
             for dim in shape:
                 size *= int(dim)
             size *= dtype.itemsize
             if size != ctypes.c_size_t(size).value:
                 raise ValueError("Variable %s is too large" % name)
 
-            array = multiprocessing.sharedctypes.RawArray("c", size)
+            array = mp_ctx.RawArray("c", size)
             self._shared_point[name] = array
             array_np = np.frombuffer(array, dtype).reshape(shape)
             array_np[...] = start[name]
             self._point[name] = array_np
 
         self._readable = True
         self._num_samples = 0
 
-        self._process = _Process(
-            process_name,
-            remote_conn,
-            step_method,
-            self._shared_point,
-            draws,
-            tune,
-            seed,
+        if step_method_pickled is not None:
+            step_method_send = step_method_pickled
+        else:
+            step_method_send = step_method
+
+        self._process = mp_ctx.Process(
+            daemon=True,
+            name=process_name,
+            target=_run_process,
+            args=(
+                process_name,
+                remote_conn,
+                step_method_send,
+                step_method_pickled is not None,
+                self._shared_point,
+                draws,
+                tune,
+                seed,
+                pickle_backend,
+            )
         )
-        try:
-            self._process.start()
-        except IOError as e:
-            # Something may have gone wrong during the fork / spawn
-            if e.errno == errno.EPIPE:
-                exc = _get_broken_pipe_exception()
-                if exc is not None:
-                    # Sleep a little to give the child process time to flush
-                    # all its error message
-                    time.sleep(0.2)
-                    raise exc
-            raise
+        self._process.start()
+        # Close the remote pipe, so that we get notified if the other
+        # end is closed.
+        remote_conn.close()
 
     @property
     def shared_point_view(self):
         """May only be written to or read between a `recv_draw`
         call from the process and a `write_next` or `abort` call.
         """
         if not self._readable:
             raise RuntimeError()
         return self._point
 
+    def _send(self, msg, *args):
+        try:
+            self._msg_pipe.send((msg, *args))
+        except Exception:
+            # try to recive an error message
+            message = None
+            try:
+                message = self._msg_pipe.recv()
+            except Exception:
+                pass
+            if message is not None and message[0] == "error":
+                warns, old_error = message[1:]
+                if warns is not None:
+                    error = ParallelSamplingError(
+                        str(old_error),
+                        self.chain,
+                        warns
+                    )
+                else:
+                    error = RuntimeError("Chain %s failed." % self.chain)
+                raise error from old_error
+            raise
+
     def start(self):
-        self._msg_pipe.send(("start",))
+        self._send("start")
 
     def write_next(self):
         self._readable = False
-        self._msg_pipe.send(("write_next",))
+        self._send("write_next")
 
     def abort(self):
-        self._msg_pipe.send(("abort",))
+        self._send("abort")
 
     def join(self, timeout=None):
         self._process.join(timeout)
 
     def terminate(self):
         self._process.terminate()
 
@@ -320,15 +371,15 @@
             raise ValueError("Sampler sent bad message.")
 
     @staticmethod
     def terminate_all(processes, patience=2):
         for process in processes:
             try:
                 process.abort()
-            except EOFError:
+            except Exception:
                 pass
 
         start_time = time.time()
         try:
             for process in processes:
                 timeout = time.time() + patience - start_time
                 if timeout < 0:
@@ -349,31 +400,60 @@
     "Draw", ["chain", "is_last", "draw_idx", "tuning", "stats", "point", "warnings"]
 )
 
 
 class ParallelSampler:
     def __init__(
         self,
-        draws:int,
-        tune:int,
-        chains:int,
-        cores:int,
-        seeds:list,
-        start_points:list,
+        draws: int,
+        tune: int,
+        chains: int,
+        cores: int,
+        seeds: list,
+        start_points: list,
         step_method,
-        start_chain_num:int=0,
-        progressbar:bool=True,
+        start_chain_num: int = 0,
+        progressbar: bool = True,
+        mp_ctx=None,
+        pickle_backend: str = 'pickle',
     ):
 
         if any(len(arg) != chains for arg in [seeds, start_points]):
             raise ValueError("Number of seeds and start_points must be %s." % chains)
 
+        if mp_ctx is None or isinstance(mp_ctx, str):
+            # Closes issue https://github.com/pymc-devs/pymc3/issues/3849
+            if platform.system() == 'Darwin':
+                mp_ctx = "forkserver"
+            mp_ctx = multiprocessing.get_context(mp_ctx)
+
+        step_method_pickled = None
+        if mp_ctx.get_start_method() != 'fork':
+            if pickle_backend == 'pickle':
+                step_method_pickled = pickle.dumps(step_method, protocol=-1)
+            elif pickle_backend == 'dill':
+                try:
+                    import dill
+                except ImportError:
+                    raise ValueError(
+                        "dill must be installed for pickle_backend='dill'."
+                    )
+                step_method_pickled = dill.dumps(step_method, protocol=-1)
+
         self._samplers = [
             ProcessAdapter(
-                draws, tune, step_method, chain + start_chain_num, seed, start
+                draws,
+                tune,
+                step_method,
+                step_method_pickled,
+                chain + start_chain_num,
+                seed,
+                start,
+                mp_ctx,
+                pickle_backend
             )
             for chain, seed, start in zip(range(chains), seeds, start_points)
         ]
 
         self._inactive = self._samplers.copy()
         self._finished = []
         self._active = []
```

### Comparing `pymc3-3.9.2/pymc3/plots/__init__.py` & `pymc3-3.9.3/pymc3/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/plots/posteriorplot.py` & `pymc3-3.9.3/pymc3/plots/posteriorplot.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/sampling.py` & `pymc3-3.9.3/pymc3/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import packaging
 import pickle
 import logging
 import time
 import warnings
 
 import arviz
+from arviz import InferenceData
 import numpy as np
 import theano.gradient as tg
 from theano.tensor import Tensor
 import xarray
 
 from .backends.base import BaseTrace, MultiTrace
 from .backends.ndarray import NDArray
@@ -53,14 +54,15 @@
 )
 from .util import (
     update_start_vals,
     get_untransformed_name,
     is_transformed_name,
     get_default_varnames,
     dataset_to_point_dict,
+    chains_and_samples,
 )
 from .vartypes import discrete_types
 from .exceptions import IncorrectArgumentsError
 from .parallel_sampling import _cpu_count, Draw
 from pymc3.step_methods.hmc import quadpotential
 import pymc3 as pm
 from fastprogress.fastprogress import progress_bar
@@ -87,28 +89,30 @@
     BinaryMetropolis,
     BinaryGibbsMetropolis,
     Slice,
     CategoricalGibbsMetropolis,
 )
 
 ArrayLike = Union[np.ndarray, List[float]]
+PointType = Dict[str, np.ndarray]
+PointList = List[PointType]
 
 _log = logging.getLogger("pymc3")
 
 
-def instantiate_steppers(model, steps, selected_steps, step_kwargs=None):
+def instantiate_steppers(_model, steps, selected_steps, step_kwargs=None):
     """Instantiate steppers assigned to the model variables.
 
     This function is intended to be called automatically from ``sample()``, but
     may be called manually.
 
     Parameters
     ----------
     model : Model object
-        A fully-specified model object
+        A fully-specified model object; legacy argument -- ignored
     steps : step function or vector of step functions
         One or more step functions that have been assigned to some subset of
         the model's parameters. Defaults to None (no assigned variables).
     selected_steps : dictionary of step methods and variables
         The step methods and the variables that have were assigned to them.
     step_kwargs : dict
         Parameters for the samplers. Keys are the lower case names of
@@ -218,15 +222,17 @@
     elif isinstance(s, CompoundStep):
         _log.info(">" * level + "CompoundStep")
         for i in s.methods:
             _print_step_hierarchy(i, level + 1)
     else:
         varnames = ", ".join(
             [
-                get_untransformed_name(v.name) if is_transformed_name(v.name) else v.name
+                get_untransformed_name(v.name)
+                if is_transformed_name(v.name)
+                else v.name
                 for v in s.vars
             ]
         )
         _log.info(">" * level + "{}: [{}]".format(s.__class__.__name__, varnames))
 
 
 def sample(
@@ -244,16 +250,18 @@
     model=None,
     random_seed=None,
     discard_tuned_samples=True,
     compute_convergence_checks=True,
     callback=None,
     *,
     return_inferencedata=None,
-    idata_kwargs:dict=None,
-    **kwargs
+    idata_kwargs: dict = None,
+    mp_ctx=None,
+    pickle_backend: str = "pickle",
+    **kwargs,
 ):
     """Draw samples from the posterior using the given step methods.
 
     Multiple step methods are supported via compound step methods.
 
     Parameters
     ----------
@@ -332,14 +340,21 @@
 
         Sampling can be interrupted by throwing a ``KeyboardInterrupt`` in the callback.
     return_inferencedata : bool, optional, default=False
         Whether to return the trace as an `arviz.InferenceData` (True) object or a `MultiTrace` (False)
         Defaults to `False`, but we'll switch to `True` in an upcoming release.
     idata_kwargs : dict, optional
         Keyword arguments for `arviz.from_pymc3`
+    mp_ctx : multiprocessing.context.BaseContent
+        A multiprocessing context for parallel sampling. See multiprocessing
+        documentation for details.
+    pickle_backend : str
+        One of `'pickle'` or `'dill'`. The library used to pickle models
+        in parallel sampling if the multiprocessing context is not of type
+        `fork`.
 
     Returns
     -------
     trace : pymc3.backends.base.MultiTrace or arviz.InferenceData
         A ``MultiTrace`` or ArviZ ``InferenceData`` object that contains the samples.
 
     Notes
@@ -424,24 +439,24 @@
         raise TypeError("Invalid value for `random_seed`. Must be tuple, list or int")
 
     if not discard_tuned_samples and not return_inferencedata:
         warnings.warn(
             "Tuning samples will be included in the returned `MultiTrace` object, which can lead to"
             " complications in your downstream analysis. Please consider to switch to `InferenceData`:\n"
             "`pm.sample(..., return_inferencedata=True)`",
-            UserWarning
+            UserWarning,
         )
 
     if return_inferencedata is None:
         v = packaging.version.parse(pm.__version__)
         if v.release[0] > 3 or v.release[1] >= 10:
             warnings.warn(
                 "In an upcoming release, pm.sample will return an `arviz.InferenceData` object instead of a `MultiTrace` by default. "
                 "You can pass return_inferencedata=True or return_inferencedata=False to be safe and silence this warning.",
-                FutureWarning
+                FutureWarning,
             )
         # set the default
         return_inferencedata = False
 
     if start is not None:
         for start_vals in start:
             _check_start_shape(model, start_vals)
@@ -466,21 +481,24 @@
             start_, step = init_nuts(
                 init=init,
                 chains=chains,
                 n_init=n_init,
                 model=model,
                 random_seed=random_seed,
                 progressbar=progressbar,
-                **kwargs
+                **kwargs,
             )
             if start is None:
                 start = start_
         except (AttributeError, NotImplementedError, tg.NullTypeGradError):
             # gradient computation failed
-            _log.info("Initializing NUTS failed. " "Falling back to elementwise auto-assignment.")
+            _log.info(
+                "Initializing NUTS failed. "
+                "Falling back to elementwise auto-assignment."
+            )
             _log.debug("Exception in init nuts", exec_info=True)
             step = assign_step_methods(model, step, step_kwargs=kwargs)
     else:
         step = assign_step_methods(model, step, step_kwargs=kwargs)
 
     if isinstance(step, list):
         step = CompoundStep(step)
@@ -498,14 +516,19 @@
         "chains": chains,
         "tune": tune,
         "progressbar": progressbar,
         "model": model,
         "random_seed": random_seed,
         "cores": cores,
         "callback": callback,
+        "discard_tuned_samples": discard_tuned_samples,
+    }
+    parallel_args = {
+        "pickle_backend": pickle_backend,
+        "mp_ctx": mp_ctx,
     }
 
     sample_args.update(kwargs)
 
     has_population_samplers = np.any(
         [
             isinstance(m, arraystep.PopulationArrayStepShared)
@@ -515,15 +538,15 @@
 
     parallel = cores > 1 and chains > 1 and not has_population_samplers
     t_start = time.time()
     if parallel:
         _log.info("Multiprocess sampling ({} chains in {} jobs)".format(chains, cores))
         _print_step_hierarchy(step)
         try:
-            trace = _mp_sample(**sample_args)
+            trace = _mp_sample(**sample_args, **parallel_args)
         except pickle.PickleError:
             _log.warning("Could not pickle model, sampling singlethreaded.")
             _log.debug("Pickling error:", exec_info=True)
             parallel = False
         except AttributeError as e:
             if str(e).startswith("AttributeError: Can't pickle"):
                 _log.warning("Could not pickle model, sampling singlethreaded.")
@@ -532,15 +555,17 @@
             else:
                 raise
     if not parallel:
         if has_population_samplers:
             has_demcmc = np.any(
                 [
                     isinstance(m, DEMetropolis)
-                    for m in (step.methods if isinstance(step, CompoundStep) else [step])
+                    for m in (
+                        step.methods if isinstance(step, CompoundStep) else [step]
+                    )
                 ]
             )
             _log.info("Population sampling ({} chains)".format(chains))
             if has_demcmc and chains < 3:
                 raise ValueError(
                     "DEMetropolis requires at least 3 chains. "
                     "For this {}-dimensional model you should use ≥{} chains".format(
@@ -559,19 +584,19 @@
             _log.info("Sequential sampling ({} chains in 1 job)".format(chains))
             _print_step_hierarchy(step)
             trace = _sample_many(**sample_args)
 
     t_sampling = time.time() - t_start
     # count the number of tune/draw iterations that happened
     # ideally via the "tune" statistic, but not all samplers record it!
-    if 'tune' in trace.stat_names:
-        stat = trace.get_sampler_stats('tune', chains=0)
+    if "tune" in trace.stat_names:
+        stat = trace.get_sampler_stats("tune", chains=0)
         # when CompoundStep is used, the stat is 2 dimensional!
         if len(stat.shape) == 2:
-            stat = stat[:,0]
+            stat = stat[:, 0]
         stat = tuple(stat)
         n_tune = stat.count(True)
         n_draws = stat.count(False)
     else:
         # these may be wrong when KeyboardInterrupt happened, but they're better than nothing
         n_tune = min(tune, len(trace))
         n_draws = max(0, len(trace) - n_tune)
@@ -583,28 +608,30 @@
     trace.report._n_tune = n_tune
     trace.report._n_draws = n_draws
     trace.report._t_sampling = t_sampling
 
     n_chains = len(trace.chains)
     _log.info(
         f'Sampling {n_chains} chain{"s" if n_chains > 1 else ""} for {n_tune:_d} tune and {n_draws:_d} draw iterations '
-        f'({n_tune*n_chains:_d} + {n_draws*n_chains:_d} draws total) '
-        f'took {trace.report.t_sampling:.0f} seconds.'
+        f"({n_tune*n_chains:_d} + {n_draws*n_chains:_d} draws total) "
+        f"took {trace.report.t_sampling:.0f} seconds."
     )
 
     idata = None
     if compute_convergence_checks or return_inferencedata:
         ikwargs = dict(model=model, save_warmup=not discard_tuned_samples)
         if idata_kwargs:
             ikwargs.update(idata_kwargs)
         idata = arviz.from_pymc3(trace, **ikwargs)
 
     if compute_convergence_checks:
         if draws - tune < 100:
-            warnings.warn("The number of samples is too small to check convergence reliably.")
+            warnings.warn(
+                "The number of samples is too small to check convergence reliably."
+            )
         else:
             trace.report._run_convergence_checks(idata, model)
     trace.report._log_summary()
 
     if return_inferencedata:
         return idata
     else:
@@ -632,15 +659,24 @@
                         tuple(var_shape), var.name, start[var.name]
                     )
 
     if e != "":
         raise ValueError("Bad shape for start argument:{}".format(e))
 
 
-def _sample_many(draws, chain:int, chains:int, start:list, random_seed:list, step, callback=None, **kwargs):
+def _sample_many(
+    draws,
+    chain: int,
+    chains: int,
+    start: list,
+    random_seed: list,
+    step,
+    callback=None,
+    **kwargs,
+):
     """Samples all chains sequentially.
 
     Parameters
     ----------
     draws: int
         The number of samples to draw
     chain: int
@@ -664,15 +700,15 @@
         trace = _sample(
             draws=draws,
             chain=chain + i,
             start=start[i],
             step=step,
             random_seed=random_seed[i],
             callback=callback,
-            **kwargs
+            **kwargs,
         )
         if trace is None:
             if len(traces) == 0:
                 raise ValueError("Sampling stopped before a sample was created.")
             else:
                 break
         elif len(trace) < draws:
@@ -681,25 +717,25 @@
             break
         else:
             traces.append(trace)
     return MultiTrace(traces)
 
 
 def _sample_population(
-    draws:int,
-    chain:int,
-    chains:int,
+    draws: int,
+    chain: int,
+    chains: int,
     start,
     random_seed,
     step,
     tune,
     model,
     progressbar: bool = True,
     parallelize=False,
-    **kwargs
+    **kwargs,
 ):
     """Performs sampling of a population of chains using the ``PopulationStepper``.
 
     Parameters
     ----------
     draws : int
         The number of samples to draw
@@ -756,15 +792,15 @@
     start,
     draws: int,
     step=None,
     trace=None,
     tune=None,
     model: Optional[Model] = None,
     callback=None,
-    **kwargs
+    **kwargs,
 ):
     """Main iteration for singleprocess sampling.
 
     Multiple step methods are supported via compound step methods.
 
     Parameters
     ----------
@@ -793,15 +829,17 @@
     Returns
     -------
     strace : pymc3.backends.base.BaseTrace
         A ``BaseTrace`` object that contains the samples for this chain.
     """
     skip_first = kwargs.get("skip_first", 0)
 
-    sampling = _iter_sample(draws, step, start, trace, chain, tune, model, random_seed, callback)
+    sampling = _iter_sample(
+        draws, step, start, trace, chain, tune, model, random_seed, callback
+    )
     _pbar_data = {"chain": chain, "divergences": 0}
     _desc = "Sampling chain {chain:d}, {divergences:,d} divergences"
     if progressbar:
         sampling = progress_bar(sampling, total=draws, display=progressbar)
         sampling.comment = _desc.format(**_pbar_data)
     try:
         strace = None
@@ -867,21 +905,31 @@
     Examples
     --------
     ::
 
         for trace in iter_sample(500, step):
             ...
     """
-    sampling = _iter_sample(draws, step, start, trace, chain, tune, model, random_seed, callback)
+    sampling = _iter_sample(
+        draws, step, start, trace, chain, tune, model, random_seed, callback
+    )
     for i, (strace, _) in enumerate(sampling):
         yield MultiTrace([strace[: i + 1]])
 
 
 def _iter_sample(
-    draws, step, start=None, trace=None, chain=0, tune=None, model=None, random_seed=None, callback=None
+    draws,
+    step,
+    start=None,
+    trace=None,
+    chain=0,
+    tune=None,
+    model=None,
+    random_seed=None,
+    callback=None,
 ):
     """Generator for sampling one chain. (Used in singleprocess sampling.)
 
     Parameters
     ----------
     draws : int
         The number of samples to draw
@@ -937,15 +985,15 @@
     if step.generates_stats and strace.supports_sampler_stats:
         strace.setup(draws, chain, step.stats_dtypes)
     else:
         strace.setup(draws, chain)
 
     try:
         step.tune = bool(tune)
-        if hasattr(step, 'reset_tuning'):
+        if hasattr(step, "reset_tuning"):
             step.reset_tuning()
         for i in range(draws):
             stats = None
             diverging = False
 
             if i == 0 and hasattr(step, "iter_count"):
                 step.iter_count = 0
@@ -959,15 +1007,18 @@
                 else:
                     strace.record(point)
             else:
                 point = step.step(point)
                 strace.record(point)
             if callback is not None:
                 warns = getattr(step, "warnings", None)
-                callback(trace=strace, draw=Draw(chain, i == draws, i, i < tune, stats, point, warns))
+                callback(
+                    trace=strace,
+                    draw=Draw(chain, i == draws, i, i < tune, stats, point, warns),
+                )
 
             yield strace, diverging
     except KeyboardInterrupt:
         strace.close()
         if hasattr(step, "warnings"):
             warns = step.warnings()
             strace._add_warnings(warns)
@@ -980,14 +1031,15 @@
         if hasattr(step, "warnings"):
             warns = step.warnings()
             strace._add_warnings(warns)
 
 
 class PopulationStepper:
     """Wraps population of step methods to step them in parallel with single or multiprocessing."""
+
     def __init__(self, steppers, parallelize, progressbar=True):
         """Use multiprocessing to parallelize chains.
 
         Falls back to sequential evaluation if multiprocessing fails.
 
         In the multiprocessing mode of operation, a new process is started for each
         chain/stepper and Pipes are used to communicate with the main process.
@@ -1011,15 +1063,17 @@
                 # configure a child process for each stepper
                 _log.info(
                     "Attempting to parallelize chains to all cores. You can turn this off with `pm.sample(cores=1)`."
                 )
                 import multiprocessing
 
                 for c, stepper in (
-                    enumerate(progress_bar(steppers)) if progressbar else enumerate(steppers)
+                    enumerate(progress_bar(steppers))
+                    if progressbar
+                    else enumerate(steppers)
                 ):
                     secondary_end, primary_end = multiprocessing.Pipe()
                     stepper_dumps = pickle.dumps(stepper, protocol=4)
                     process = multiprocessing.Process(
                         target=self.__class__._run_secondary,
                         args=(c, stepper_dumps, secondary_end),
                         name="ChainWalker{}".format(c),
@@ -1078,15 +1132,17 @@
         np.random.seed(None)
         try:
             stepper = pickle.loads(stepper_dumps)
             # the stepper is not necessarily a PopulationArraySharedStep itself,
             # but rather a CompoundStep. PopulationArrayStepShared.population
             # has to be updated, therefore we identify the substeppers first.
             population_steppers = []
-            for sm in stepper.methods if isinstance(stepper, CompoundStep) else [stepper]:
+            for sm in (
+                stepper.methods if isinstance(stepper, CompoundStep) else [stepper]
+            ):
                 if isinstance(sm, arraystep.PopulationArrayStepShared):
                     population_steppers.append(sm)
             while True:
                 incoming = secondary_end.recv()
                 # receiving a None is the signal to exit
                 if incoming is None:
                     break
@@ -1135,15 +1191,15 @@
 
 
 def _prepare_iter_population(
     draws: int,
     chains: list,
     step,
     start: list,
-    parallelize:bool,
+    parallelize: bool,
     tune=None,
     model=None,
     random_seed=None,
     progressbar=True,
 ):
     """Prepare a PopulationStepper and traces for population sampling.
 
@@ -1343,15 +1399,18 @@
     chain: int,
     random_seed: list,
     start: list,
     progressbar=True,
     trace=None,
     model=None,
     callback=None,
-    **kwargs
+    discard_tuned_samples=True,
+    mp_ctx=None,
+    pickle_backend="pickle",
+    **kwargs,
 ):
     """Main iteration for multiprocess sampling.
 
     Parameters
     ----------
     draws : int
         The number of samples to draw
@@ -1405,15 +1464,25 @@
         if step.generates_stats and strace.supports_sampler_stats:
             strace.setup(draws + tune, idx + chain, step.stats_dtypes)
         else:
             strace.setup(draws + tune, idx + chain)
         traces.append(strace)
 
     sampler = ps.ParallelSampler(
-        draws, tune, chains, cores, random_seed, start, step, chain, progressbar
+        draws,
+        tune,
+        chains,
+        cores,
+        random_seed,
+        start,
+        step,
+        chain,
+        progressbar,
+        mp_ctx=mp_ctx,
+        pickle_backend=pickle_backend,
     )
     try:
         try:
             with sampler:
                 for draw in sampler:
                     trace = traces[draw.chain - chain]
                     if trace.supports_sampler_stats and draw.stats is not None:
@@ -1435,15 +1504,18 @@
                 trace.close()
 
             multitrace = MultiTrace(traces)
             multitrace._report._log_summary()
             raise
         return MultiTrace(traces)
     except KeyboardInterrupt:
-        traces, length = _choose_chains(traces, tune)
+        if discard_tuned_samples:
+            traces, length = _choose_chains(traces, tune)
+        else:
+            traces, length = _choose_chains(traces, 0)
         return MultiTrace(traces)[:length]
     finally:
         for trace in traces:
             trace.close()
 
 
 def _choose_chains(traces, tune):
@@ -1550,30 +1622,29 @@
     random_seed=None,
     progressbar: bool = True,
 ) -> Dict[str, np.ndarray]:
     """Generate posterior predictive samples from a model given a trace.
 
     Parameters
     ----------
-    trace : backend, list, xarray.Dataset, or MultiTrace
+    trace : backend, list, xarray.Dataset, arviz.InferenceData, or MultiTrace
         Trace generated from MCMC sampling, or a list of dicts (eg. points or from find_MAP()),
         or xarray.Dataset (eg. InferenceData.posterior or InferenceData.prior)
     samples : int
         Number of posterior predictive samples to generate. Defaults to one posterior predictive
         sample per posterior sample, that is, the number of draws times the number of chains. It
         is not recommended to modify this value; when modified, some chains may not be represented
         in the posterior predictive sample.
     model : Model (optional if in ``with`` context)
         Model used to generate ``trace``
     vars : iterable
         Variables for which to compute the posterior predictive samples.
         Deprecated: please use ``var_names`` instead.
     var_names : Iterable[str]
-        Alternative way to specify vars to sample, to make this function orthogonal with
-        others.
+        Names of variables for which to compute the posterior predictive samples.
     size : int
         The number of random draws from the distribution specified by the parameters in each
         sample of the trace. Not recommended unless more than ndraws times nchains posterior
         predictive samples are needed.
     keep_size : bool, optional
         Force posterior predictive sample to have the same shape as posterior and sample stats
         data: ``(nchains, ndraws, ...)``. Overrides samples and size parameters.
@@ -1586,54 +1657,76 @@
 
     Returns
     -------
     samples : dict
         Dictionary with the variable names as keys, and values numpy arrays containing
         posterior predictive samples.
     """
-    if isinstance(trace, xarray.Dataset):
-        trace = dataset_to_point_dict(trace)
 
-    len_trace = len(trace)
-    try:
-        nchain = trace.nchains
-    except AttributeError:
-        nchain = 1
+    _trace: Union[MultiTrace, PointList]
+    if isinstance(trace, InferenceData):
+        _trace = dataset_to_point_dict(trace.posterior)
+    elif isinstance(trace, xarray.Dataset):
+        _trace = dataset_to_point_dict(trace)
+    else:
+        _trace = trace
+
+    nchain: int
+    len_trace: int
+    if isinstance(trace, (InferenceData, xarray.Dataset)):
+        nchain, len_trace = chains_and_samples(trace)
+    else:
+        len_trace = len(_trace)
+        try:
+            nchain = _trace.nchains
+        except AttributeError:
+            nchain = 1
 
     if keep_size and samples is not None:
-        raise IncorrectArgumentsError("Should not specify both keep_size and samples arguments")
+        raise IncorrectArgumentsError(
+            "Should not specify both keep_size and samples arguments"
+        )
     if keep_size and size is not None:
-        raise IncorrectArgumentsError("Should not specify both keep_size and size arguments")
+        raise IncorrectArgumentsError(
+            "Should not specify both keep_size and size arguments"
+        )
 
     if samples is None:
-        if isinstance(trace, MultiTrace):
-            samples = sum(len(v) for v in trace._straces.values())
-        elif isinstance(trace, list) and all((isinstance(x, dict) for x in trace)):
+        if isinstance(_trace, MultiTrace):
+            samples = sum(len(v) for v in _trace._straces.values())
+        elif isinstance(_trace, list) and all((isinstance(x, dict) for x in _trace)):
             # this is a list of points
-            samples = len(trace)
+            samples = len(_trace)
         else:
-            raise ValueError("Do not know how to compute number of samples for trace argument of type %s"%type(trace))
+            raise TypeError(
+                "Do not know how to compute number of samples for trace argument of type %s"
+                % type(_trace)
+            )
 
+    assert samples is not None
     if samples < len_trace * nchain:
         warnings.warn(
             "samples parameter is smaller than nchains times ndraws, some draws "
             "and/or chains may not be represented in the returned posterior "
             "predictive sample"
         )
 
     model = modelcontext(model)
 
     if var_names is not None:
         if vars is not None:
-            raise IncorrectArgumentsError("Should not specify both vars and var_names arguments.")
+            raise IncorrectArgumentsError(
+                "Should not specify both vars and var_names arguments."
+            )
         else:
             vars = [model[x] for x in var_names]
-    elif vars is not None: # var_names is None, and vars is not.
-        warnings.warn("vars argument is deprecated in favor of var_names.",
-                      DeprecationWarning)
+    elif vars is not None:  # var_names is None, and vars is not.
+        warnings.warn(
+            "vars argument is deprecated in favor of var_names.", DeprecationWarning
+        )
     if vars is None:
         vars = model.observed_RVs
 
     if random_seed is not None:
         np.random.seed(random_seed)
 
     indices = np.arange(samples)
@@ -1641,18 +1734,29 @@
     if progressbar:
         indices = progress_bar(indices, total=samples, display=progressbar)
 
     ppc_trace_t = _DefaultTrace(samples)
     try:
         for idx in indices:
             if nchain > 1:
-                chain_idx, point_idx = np.divmod(idx, len_trace)
-                param = trace._straces[chain_idx % nchain].point(point_idx)
+                # the trace object will either be a MultiTrace (and have _straces)...
+                if hasattr(_trace, "_straces"):
+                    chain_idx, point_idx = np.divmod(idx, len_trace)
+                    param = (
+                        cast(MultiTrace, _trace)
+                        ._straces[chain_idx % nchain]
+                        .point(point_idx)
+                    )
+                # ... or a PointList
+                else:
+                    param = cast(PointList, _trace)[idx % len_trace]
+            # there's only a single chain, but the index might hit it multiple times if
+            # the number of indices is greater than the length of the trace.
             else:
-                param = trace[idx % len_trace]
+                param = _trace[idx % len_trace]
 
             values = draw_values(vars, point=param, size=size)
             for k, v in zip(vars, values):
                 ppc_trace_t.insert(k.name, v, idx)
 
     except KeyboardInterrupt:
         pass
@@ -1825,23 +1929,26 @@
         samples.
     """
     model = modelcontext(model)
 
     if vars is None and var_names is None:
         prior_pred_vars = model.observed_RVs
         prior_vars = (
-            get_default_varnames(model.unobserved_RVs, include_transformed=True) + model.potentials
+            get_default_varnames(model.unobserved_RVs, include_transformed=True)
+            + model.potentials
         )
         vars_ = [var.name for var in prior_vars + prior_pred_vars]
         vars = set(vars_)
     elif vars is None:
         vars = var_names
         vars_ = vars
     elif vars is not None:
-        warnings.warn("vars argument is deprecated in favor of var_names.", DeprecationWarning)
+        warnings.warn(
+            "vars argument is deprecated in favor of var_names.", DeprecationWarning
+        )
         vars_ = vars
     else:
         raise ValueError("Cannot supply both vars and var_names arguments.")
     vars = cast(TIterable[str], vars)  # tell mypy that vars cannot be None here.
 
     if random_seed is not None:
         np.random.seed(random_seed)
@@ -1863,15 +1970,21 @@
                 prior[var_name] = model[untransformed].transformation.forward_val(
                     data[untransformed]
                 )
     return prior
 
 
 def init_nuts(
-    init="auto", chains=1, n_init=500000, model=None, random_seed=None, progressbar=True, **kwargs
+    init="auto",
+    chains=1,
+    n_init=500000,
+    model=None,
+    random_seed=None,
+    progressbar=True,
+    **kwargs,
 ):
     """Set up the mass matrix initialization for NUTS.
 
     NUTS convergence and sampling speed is extremely dependent on the
     choice of mass/scaling matrix. This function implements different
     methods for choosing or adapting the mass matrix.
 
@@ -1919,15 +2032,17 @@
     """
     model = modelcontext(model)
 
     vars = kwargs.get("vars", model.vars)
     if set(vars) != set(model.vars):
         raise ValueError("Must use init_nuts on all variables of a model.")
     if not all_continuous(vars):
-        raise ValueError("init_nuts can only be used for models with only " "continuous variables.")
+        raise ValueError(
+            "init_nuts can only be used for models with only " "continuous variables."
+        )
 
     if not isinstance(init, str):
         raise TypeError("init must be a string.")
 
     if init is not None:
         init = init.lower()
 
@@ -1973,15 +2088,17 @@
         start = approx.sample(draws=chains)
         start = list(start)
         stds = approx.bij.rmap(approx.std.eval())
         cov = model.dict_to_array(stds) ** 2
         mean = approx.bij.rmap(approx.mean.get_value())
         mean = model.dict_to_array(mean)
         weight = 50
-        potential = quadpotential.QuadPotentialDiagAdaptGrad(model.ndim, mean, cov, weight)
+        potential = quadpotential.QuadPotentialDiagAdaptGrad(
+            model.ndim, mean, cov, weight
+        )
     elif init == "advi+adapt_diag":
         approx = pm.fit(
             random_seed=random_seed,
             n=n_init,
             method="advi",
             model=model,
             callbacks=cb,
@@ -2033,15 +2150,15 @@
         start = [start] * chains
         potential = quadpotential.QuadPotentialFull(cov)
     elif init == "adapt_full":
         start = [model.test_point] * chains
         mean = np.mean([model.dict_to_array(vals) for vals in start], axis=0)
         cov = np.eye(model.ndim)
         potential = quadpotential.QuadPotentialFullAdapt(model.ndim, mean, cov, 10)
-    elif init == 'jitter+adapt_full':
+    elif init == "jitter+adapt_full":
         start = []
         for _ in range(chains):
             mean = {var: val.copy() for var, val in model.test_point.items()}
             for val in mean.values():
                 val[...] += 2 * np.random.rand(*val.shape) - 1
             start.append(mean)
         mean = np.mean([model.dict_to_array(vals) for vals in start], axis=0)
```

### Comparing `pymc3-3.9.2/pymc3/smc/__init__.py` & `pymc3-3.9.3/pymc3/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/smc/sample_smc.py` & `pymc3-3.9.3/pymc3/smc/sample_smc.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,33 +10,43 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import time
 import logging
+import warnings
+from collections.abc import Iterable
+import multiprocessing as mp
+import numpy as np
+
 from .smc import SMC
+from ..model import modelcontext
+from ..backends.base import MultiTrace
+from ..parallel_sampling import _cpu_count
+
+EXPERIMENTAL_WARNING = (
+    "Warning: SMC-ABC is an experimental step method and not yet recommended for use in PyMC3!"
+)
 
 
 def sample_smc(
-    draws=1000,
+    draws=2000,
     kernel="metropolis",
     n_steps=25,
-    parallel=False,
     start=None,
-    cores=None,
     tune_steps=True,
     p_acc_rate=0.99,
     threshold=0.5,
-    epsilon=1.0,
-    dist_func="gaussian_kernel",
-    sum_stat="identity",
-    progressbar=False,
+    save_sim_data=False,
     model=None,
     random_seed=-1,
+    parallel=False,
+    chains=None,
+    cores=None,
 ):
     r"""
     Sequential Monte Carlo based sampling
 
     Parameters
     ----------
     draws: int
@@ -45,45 +55,43 @@
     kernel: str
         Kernel method for the SMC sampler. Available option are ``metropolis`` (default) and `ABC`.
         Use `ABC` for likelihood free inference togheter with a ``pm.Simulator``.
     n_steps: int
         The number of steps of each Markov Chain. If ``tune_steps == True`` ``n_steps`` will be used
         for the first stage and for the others it will be determined automatically based on the
         acceptance rate and `p_acc_rate`, the max number of steps is ``n_steps``.
-    parallel: bool
-        Distribute computations across cores if the number of cores is larger than 1.
-        Defaults to False.
     start: dict, or array of dict
         Starting point in parameter space. It should be a list of dict with length `chains`.
         When None (default) the starting point is sampled from the prior distribution. 
-    cores: int
-        The number of chains to run in parallel. If ``None`` (default), it will be automatically
-        set to the number of CPUs in the system.
     tune_steps: bool
         Whether to compute the number of steps automatically or not. Defaults to True
     p_acc_rate: float
         Used to compute ``n_steps`` when ``tune_steps == True``. The higher the value of
         ``p_acc_rate`` the higher the number of steps computed automatically. Defaults to 0.99.
         It should be between 0 and 1.
     threshold: float
         Determines the change of beta from stage to stage, i.e.indirectly the number of stages,
         the higher the value of `threshold` the higher the number of stages. Defaults to 0.5.
         It should be between 0 and 1.
-    epsilon: float
-        Standard deviation of the gaussian pseudo likelihood. Only works with `kernel = ABC`
-    dist_func: str
-        Distance function. The only available option is ``gaussian_kernel``
-    sum_stat: str or callable
-        Summary statistics. Available options are ``indentity``, ``sorted``, ``mean``, ``median``.
-        If a callable is based it should return a number or a 1d numpy array.
-    progressbar: bool
-        Flag for displaying a progress bar. Defaults to False.
+    save_sim_data : bool
+        Whether or not to save the simulated data. This parameters only work with the ABC kernel.
+        The stored data corresponds to the posterior predictive distribution.
     model: Model (optional if in ``with`` context)).
     random_seed: int
         random seed
+    parallel: bool
+        Distribute computations across cores if the number of cores is larger than 1.
+        Defaults to False.
+    cores : int
+        The number of chains to run in parallel. If ``None``, set to the number of CPUs in the
+        system, but at most 4.
+    chains : int
+        The number of chains to sample. Running independent chains is important for some
+        convergence statistics. If ``None`` (default), then set to either ``cores`` or 2, whichever
+        is larger.
 
     Notes
     -----
     SMC works by moving through successive stages. At each stage the inverse temperature
     :math:`\beta` is increased a little bit (starting from 0 up to 1). When :math:`\beta` = 0
     we have the prior distribution and when :math:`\beta` =1 we have the posterior distribution.
     So in more general terms we are always computing samples from a tempered posterior that we can
@@ -122,56 +130,144 @@
     .. [Ching2007] Ching, J. and Chen, Y. (2007).
         Transitional Markov Chain Monte Carlo Method for Bayesian Model Updating, Model Class
         Selection, and Model Averaging. J. Eng. Mech., 10.1061/(ASCE)0733-9399(2007)133:7(816),
         816-832. `link <http://ascelibrary.org/doi/abs/10.1061/%28ASCE%290733-9399
         %282007%29133:7%28816%29>`__
     """
 
+    _log = logging.getLogger("pymc3")
+    _log.info("Initializing SMC sampler...")
+
+    model = modelcontext(model)
+    if cores is None:
+        cores = _cpu_count()
+
+    if chains is None:
+        chains = max(2, cores)
+    elif chains == 1:
+        cores = 1
+
+    _log.info(
+        (
+            f"Multiprocess sampling ({chains} chain{'s' if chains > 1 else ''} "
+            f"in {cores} job{'s' if cores > 1 else ''})"
+        )
+    )
+
+    if random_seed == -1:
+        random_seed = None
+    if chains == 1 and isinstance(random_seed, int):
+        random_seed = [random_seed]
+    if random_seed is None or isinstance(random_seed, int):
+        if random_seed is not None:
+            np.random.seed(random_seed)
+        random_seed = [np.random.randint(2 ** 30) for _ in range(chains)]
+    if not isinstance(random_seed, Iterable):
+        raise TypeError("Invalid value for `random_seed`. Must be tuple, list or int")
+
+    if kernel.lower() == "abc":
+        warnings.warn(EXPERIMENTAL_WARNING)
+        if len(model.observed_RVs) != 1:
+            warnings.warn("SMC-ABC only works properly with models with one observed variable")
+        if model.potentials:
+            _log.info("Potentials will be added to the prior term")
+
+    params = (
+        draws,
+        kernel,
+        n_steps,
+        start,
+        tune_steps,
+        p_acc_rate,
+        threshold,
+        save_sim_data,
+        model,
+    )
+
+    t1 = time.time()
+    if parallel and chains > 1:
+        loggers = [_log] + [None] * (chains - 1)
+        pool = mp.Pool(cores)
+        results = pool.starmap(
+            sample_smc_int, [(*params, random_seed[i], i, loggers[i]) for i in range(chains)]
+        )
+
+        pool.close()
+        pool.join()
+    else:
+        results = []
+        for i in range(chains):
+            results.append((sample_smc_int(*params, random_seed[i], i, _log)))
+
+    traces, sim_data, log_marginal_likelihoods, betas, accept_ratios, nsteps = zip(*results)
+    trace = MultiTrace(traces)
+    trace.report._n_draws = draws
+    trace.report._n_tune = 0
+    trace.report._t_sampling = time.time() - t1
+    trace.report.log_marginal_likelihood = np.array(log_marginal_likelihoods)
+    trace.report.betas = betas
+    trace.report.accept_ratios = accept_ratios
+    trace.report.nsteps = nsteps
+
+    if save_sim_data:
+        return trace, {modelcontext(model).observed_RVs[0].name: np.array(sim_data)}
+    else:
+        return trace
+
+
+def sample_smc_int(
+    draws,
+    kernel,
+    n_steps,
+    start,
+    tune_steps,
+    p_acc_rate,
+    threshold,
+    save_sim_data,
+    model,
+    random_seed,
+    chain,
+    _log,
+):
+
     smc = SMC(
         draws=draws,
         kernel=kernel,
         n_steps=n_steps,
-        parallel=parallel,
         start=start,
-        cores=cores,
         tune_steps=tune_steps,
         p_acc_rate=p_acc_rate,
         threshold=threshold,
-        epsilon=epsilon,
-        dist_func=dist_func,
-        sum_stat=sum_stat,
-        progressbar=progressbar,
+        save_sim_data=save_sim_data,
         model=model,
         random_seed=random_seed,
+        chain=chain,
     )
-
-    t1 = time.time()
-    _log = logging.getLogger("pymc3")
-    _log.info("Sample initial stage: ...")
     stage = 0
+    betas = []
+    accept_ratios = []
+    nsteps = []
     smc.initialize_population()
     smc.setup_kernel()
     smc.initialize_logp()
 
     while smc.beta < 1:
         smc.update_weights_beta()
-        _log.info(
-            "Stage: {:3d} Beta: {:.3f} Steps: {:3d} Acce: {:.3f}".format(
-                stage, smc.beta, smc.n_steps, smc.acc_rate
-            )
-        )
-        smc.resample()
+        if _log is not None:
+            _log.info(f"Stage: {stage:3d} Beta: {smc.beta:.3f}")
         smc.update_proposal()
-        if stage > 0:
-            smc.tune()
+        smc.resample()
         smc.mutate()
+        smc.tune()
         stage += 1
-
-    if smc.parallel and smc.cores > 1:
-        smc.pool.close()
-        smc.pool.join()
-
-    trace = smc.posterior_to_trace()
-    trace.report._n_draws = smc.draws
-    trace.report._n_tune = 0
-    trace.report._t_sampling = time.time() - t1
-    return trace
+        betas.append(smc.beta)
+        accept_ratios.append(smc.acc_rate)
+        nsteps.append(smc.n_steps)
+
+    return (
+        smc.posterior_to_trace(),
+        smc.sim_data,
+        smc.log_marginal_likelihood,
+        betas,
+        accept_ratios,
+        nsteps,
+    )
```

### Comparing `pymc3-3.9.2/pymc3/smc/smc.py` & `pymc3-3.9.3/pymc3/smc/smc.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,94 +12,67 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 from collections import OrderedDict
 
 import numpy as np
 from scipy.special import logsumexp
-from fastprogress.fastprogress import progress_bar
-import multiprocessing as mp
-import warnings
 from theano import function as theano_function
+import theano.tensor as tt
 
 from ..model import modelcontext, Point
-from ..parallel_sampling import _cpu_count
-from ..theanof import inputvars, make_shared_replacements
-from ..vartypes import discrete_types
+from ..theanof import floatX, inputvars, make_shared_replacements, join_nonshared_inputs
 from ..sampling import sample_prior_predictive
-from ..theanof import floatX, join_nonshared_inputs
-from ..step_methods.arraystep import metrop_select
-from ..step_methods.metropolis import MultivariateNormalProposal
 from ..backends.ndarray import NDArray
-from ..backends.base import MultiTrace
-
-EXPERIMENTAL_WARNING = (
-    "Warning: SMC-ABC methods are experimental step methods and not yet"
-    " recommended for use in PyMC3!"
-)
 
 
 class SMC:
     def __init__(
         self,
-        draws=1000,
+        draws=2000,
         kernel="metropolis",
         n_steps=25,
-        parallel=False,
         start=None,
-        cores=None,
         tune_steps=True,
         p_acc_rate=0.99,
         threshold=0.5,
-        epsilon=1.0,
-        dist_func="absolute_error",
-        sum_stat="Identity",
-        progressbar=False,
+        save_sim_data=False,
         model=None,
         random_seed=-1,
+        chain=0,
     ):
 
         self.draws = draws
         self.kernel = kernel
         self.n_steps = n_steps
-        self.parallel = parallel
         self.start = start
-        self.cores = cores
         self.tune_steps = tune_steps
         self.p_acc_rate = p_acc_rate
         self.threshold = threshold
-        self.epsilon = epsilon
-        self.dist_func = dist_func
-        self.sum_stat = sum_stat
-        self.progressbar = progressbar
+        self.save_sim_data = save_sim_data
         self.model = model
         self.random_seed = random_seed
+        self.chain = chain
 
         self.model = modelcontext(model)
 
         if self.random_seed != -1:
             np.random.seed(self.random_seed)
 
-        if self.cores is None:
-            self.cores = _cpu_count()
-
         self.beta = 0
         self.max_steps = n_steps
         self.proposed = draws * n_steps
         self.acc_rate = 1
         self.acc_per_chain = np.ones(self.draws)
-        self.model.marginal_log_likelihood = 0
         self.variables = inputvars(self.model.vars)
-        dimension = sum(v.dsize for v in self.variables)
-        self.scalings = np.ones(self.draws) * min(1, 2.38 ** 2 / dimension)
-        self.discrete = np.concatenate(
-            [[v.dtype in discrete_types] * (v.dsize or 1) for v in self.variables]
-        )
-        self.any_discrete = self.discrete.any()
-        self.all_discrete = self.discrete.all()
+        self.dimension = sum(v.dsize for v in self.variables)
+        self.scalings = np.ones(self.draws) * 2.38 / (self.dimension) ** 0.5
+        self.weights = np.ones(self.draws) / self.draws
+        self.log_marginal_likelihood = 0
+        self.sim_data = []
 
     def initialize_population(self):
         """
         Create an initial population from the prior distribution
         """
         population = []
         var_info = OrderedDict()
@@ -124,108 +97,108 @@
         self.var_info = var_info
 
     def setup_kernel(self):
         """
         Set up the likelihood logp function based on the chosen kernel
         """
         shared = make_shared_replacements(self.variables, self.model)
-        self.prior_logp = logp_forw([self.model.varlogpt], self.variables, shared)
 
         if self.kernel.lower() == "abc":
-            warnings.warn(EXPERIMENTAL_WARNING)
-            if len(self.model.observed_RVs) != 1:
-                warnings.warn("SMC-ABC only works properly with models with one observed variable")
+            factors = [var.logpt for var in self.model.free_RVs]
+            factors += [tt.sum(factor) for factor in self.model.potentials]
+            self.prior_logp_func = logp_forw([tt.sum(factors)], self.variables, shared)
             simulator = self.model.observed_RVs[0]
-            self.likelihood_logp = PseudoLikelihood(
-                self.epsilon,
+            distance = simulator.distribution.distance
+            sum_stat = simulator.distribution.sum_stat
+            self.likelihood_logp_func = PseudoLikelihood(
+                simulator.distribution.epsilon,
                 simulator.observations,
                 simulator.distribution.function,
                 [v.name for v in simulator.distribution.params],
                 self.model,
                 self.var_info,
                 self.variables,
-                self.dist_func,
-                self.sum_stat,
+                distance,
+                sum_stat,
+                self.draws,
+                self.save_sim_data,
             )
         elif self.kernel.lower() == "metropolis":
-            self.likelihood_logp = logp_forw([self.model.datalogpt], self.variables, shared)
+            self.prior_logp_func = logp_forw([self.model.varlogpt], self.variables, shared)
+            self.likelihood_logp_func = logp_forw([self.model.datalogpt], self.variables, shared)
 
     def initialize_logp(self):
         """
         initialize the prior and likelihood log probabilities
         """
-        if self.parallel and self.cores > 1:
-            self.pool = mp.Pool(processes=self.cores)
-            priors = self.pool.starmap(self.prior_logp, [(sample,) for sample in self.posterior])
-            likelihoods = self.pool.starmap(
-                self.likelihood_logp, [(sample,) for sample in self.posterior]
-            )
-        else:
-            priors = [self.prior_logp(sample) for sample in self.posterior]
-            likelihoods = [self.likelihood_logp(sample) for sample in self.posterior]
+        priors = [self.prior_logp_func(sample) for sample in self.posterior]
+        likelihoods = [self.likelihood_logp_func(sample) for sample in self.posterior]
 
-        self.priors = np.array(priors).squeeze()
-        self.likelihoods = np.array(likelihoods).squeeze()
+        self.prior_logp = np.array(priors).squeeze()
+        self.likelihood_logp = np.array(likelihoods).squeeze()
+
+        if self.save_sim_data:
+            self.sim_data = self.likelihood_logp_func.get_data()
 
     def update_weights_beta(self):
         """
         Calculate the next inverse temperature (beta), the importance weights based on current beta
         and tempered likelihood and updates the marginal likelihood estimation
         """
         low_beta = old_beta = self.beta
         up_beta = 2.0
-        rN = int(len(self.likelihoods) * self.threshold)
+        rN = int(len(self.likelihood_logp) * self.threshold)
 
         while up_beta - low_beta > 1e-6:
             new_beta = (low_beta + up_beta) / 2.0
-            log_weights_un = (new_beta - old_beta) * self.likelihoods
+            log_weights_un = (new_beta - old_beta) * self.likelihood_logp
             log_weights = log_weights_un - logsumexp(log_weights_un)
             ESS = int(np.exp(-logsumexp(log_weights * 2)))
             if ESS == rN:
                 break
             elif ESS < rN:
                 up_beta = new_beta
             else:
                 low_beta = new_beta
         if new_beta >= 1:
             new_beta = 1
-            log_weights_un = (new_beta - old_beta) * self.likelihoods
+            log_weights_un = (new_beta - old_beta) * self.likelihood_logp
             log_weights = log_weights_un - logsumexp(log_weights_un)
 
-        ll_max = np.max(log_weights_un)
-        self.model.marginal_log_likelihood += ll_max + np.log(
-            np.exp(log_weights_un - ll_max).mean()
-        )
+        self.log_marginal_likelihood += logsumexp(log_weights_un) - np.log(self.draws)
         self.beta = new_beta
         self.weights = np.exp(log_weights)
 
     def resample(self):
         """
         Resample particles based on importance weights
         """
         resampling_indexes = np.random.choice(
             np.arange(self.draws), size=self.draws, p=self.weights
         )
+
         self.posterior = self.posterior[resampling_indexes]
-        self.priors = self.priors[resampling_indexes]
-        self.likelihoods = self.likelihoods[resampling_indexes]
-        self.tempered_logp = self.priors + self.likelihoods * self.beta
+        self.prior_logp = self.prior_logp[resampling_indexes]
+        self.likelihood_logp = self.likelihood_logp[resampling_indexes]
+        self.posterior_logp = self.prior_logp + self.likelihood_logp * self.beta
         self.acc_per_chain = self.acc_per_chain[resampling_indexes]
         self.scalings = self.scalings[resampling_indexes]
+        if self.save_sim_data:
+            self.sim_data = self.sim_data[resampling_indexes]
 
     def update_proposal(self):
         """
         Update proposal based on the covariance matrix from tempered posterior
         """
-        cov = np.cov(self.posterior, bias=False, rowvar=0)
+        cov = np.cov(self.posterior, ddof=0, aweights=self.weights, rowvar=0)
         cov = np.atleast_2d(cov)
         cov += 1e-6 * np.eye(cov.shape[0])
         if np.isnan(cov).any() or np.isinf(cov).any():
             raise ValueError('Sample covariances not valid! Likely "draws" is too small!')
-        self.proposal = MultivariateNormalProposal(cov)
+        self.cov = cov
 
     def tune(self):
         """
         Tune scaling and n_steps based on the acceptance rate.
         """
         ave_scaling = np.exp(np.log(self.scalings.mean()) + (self.acc_per_chain.mean() - 0.234))
         self.scalings = 0.5 * (
@@ -237,136 +210,60 @@
             self.n_steps = min(
                 self.max_steps, max(2, int(np.log(1 - self.p_acc_rate) / np.log(1 - acc_rate))),
             )
 
         self.proposed = self.draws * self.n_steps
 
     def mutate(self):
-        """
-        Perform mutation step, i.e. apply selected kernel
-        """
-        parameters = (
-            self.proposal,
-            self.scalings,
-            self.any_discrete,
-            self.all_discrete,
-            self.discrete,
-            self.n_steps,
-            self.prior_logp,
-            self.likelihood_logp,
-            self.beta,
-        )
-        if self.parallel and self.cores > 1:
-            results = self.pool.starmap(
-                metrop_kernel,
-                [
-                    (
-                        self.posterior[draw],
-                        self.tempered_logp[draw],
-                        self.priors[draw],
-                        self.likelihoods[draw],
-                        draw,
-                        *parameters,
-                    )
-                    for draw in range(self.draws)
-                ],
+        ac_ = np.empty((self.n_steps, self.draws))
+
+        proposals = (
+            np.random.multivariate_normal(
+                np.zeros(self.dimension), self.cov, size=(self.n_steps, self.draws)
             )
-        else:
-            iterator = range(self.draws)
-            if self.progressbar:
-                iterator = progress_bar(iterator, display=self.progressbar)
-            results = [
-                metrop_kernel(
-                    self.posterior[draw],
-                    self.tempered_logp[draw],
-                    self.priors[draw],
-                    self.likelihoods[draw],
-                    draw,
-                    *parameters,
-                )
-                for draw in iterator
-            ]
-        posterior, acc_list, priors, likelihoods = zip(*results)
-        self.posterior = np.array(posterior)
-        self.priors = np.array(priors)
-        self.likelihoods = np.array(likelihoods)
-        self.acc_per_chain = np.array(acc_list)
-        self.acc_rate = np.mean(acc_list)
+            * self.scalings[:, None]
+        )
+        log_R = np.log(np.random.rand(self.n_steps, self.draws))
+
+        for n_step in range(self.n_steps):
+            proposal = floatX(self.posterior + proposals[n_step])
+            ll = np.array([self.likelihood_logp_func(prop) for prop in proposal])
+            pl = np.array([self.prior_logp_func(prop) for prop in proposal])
+            proposal_logp = pl + ll * self.beta
+            accepted = log_R[n_step] < (proposal_logp - self.posterior_logp)
+            ac_[n_step] = accepted
+            self.posterior[accepted] = proposal[accepted]
+            self.posterior_logp[accepted] = proposal_logp[accepted]
+            self.prior_logp[accepted] = pl[accepted]
+            self.likelihood_logp[accepted] = ll[accepted]
+            if self.save_sim_data:
+                self.sim_data[accepted] = self.likelihood_logp_func.get_data()[accepted]
+
+        self.acc_per_chain = np.mean(ac_, axis=0)
+        self.acc_rate = np.mean(ac_)
 
     def posterior_to_trace(self):
         """
         Save results into a PyMC3 trace
         """
         lenght_pos = len(self.posterior)
         varnames = [v.name for v in self.variables]
 
         with self.model:
             strace = NDArray(self.model)
-            strace.setup(lenght_pos, 0)
+            strace.setup(lenght_pos, self.chain)
         for i in range(lenght_pos):
             value = []
             size = 0
             for var in varnames:
                 shape, new_size = self.var_info[var]
                 value.append(self.posterior[i][size : size + new_size].reshape(shape))
                 size += new_size
-            strace.record({k: v for k, v in zip(varnames, value)})
-        return MultiTrace([strace])
-
-
-def metrop_kernel(
-    q_old,
-    old_tempered_logp,
-    old_prior,
-    old_likelihood,
-    draw,
-    proposal,
-    scalings,
-    any_discrete,
-    all_discrete,
-    discrete,
-    n_steps,
-    prior_logp,
-    likelihood_logp,
-    beta,
-):
-    """
-    Metropolis kernel
-    """
-    deltas = np.squeeze(proposal(n_steps) * scalings[draw])
-
-    accepted = 0
-    for n_step in range(n_steps):
-        delta = deltas[n_step]
-
-        if any_discrete:
-            if all_discrete:
-                delta = np.round(delta, 0).astype("int64")
-                q_old = q_old.astype("int64")
-                q_new = (q_old + delta).astype("int64")
-            else:
-                delta[discrete] = np.round(delta[discrete], 0)
-                q_new = floatX(q_old + delta)
-        else:
-            q_new = floatX(q_old + delta)
-
-        ll = likelihood_logp(q_new)
-        pl = prior_logp(q_new)
-
-        new_tempered_logp = pl + ll * beta
-
-        q_old, accept = metrop_select(new_tempered_logp - old_tempered_logp, q_new, q_old)
-
-        if accept:
-            accepted += 1
-            old_prior = pl
-            old_likelihood = ll
-            old_tempered_logp = new_tempered_logp
-
-    return q_old, accepted / n_steps, old_prior, old_likelihood
+            strace.record(point={k: v for k, v in zip(varnames, value)})
+        return strace
 
 
 def logp_forw(out_vars, vars, shared):
     """Compile Theano function of the model and the input and output variables.
 
     Parameters
     ----------
@@ -395,65 +292,58 @@
         function,
         params,
         model,
         var_info,
         variables,
         distance,
         sum_stat,
+        size,
+        save,
     ):
         """
         epsilon: float
             Standard deviation of the gaussian pseudo likelihood.
         observations: array-like
             observed data
         function: python function
             data simulator
         params: list
             names of the variables parameterizing the simulator.
         model: PyMC3 model
         var_info: dict
             generated by ``SMC.initialize_population``
+        variables: list
+            Model variables.
         distance : str or callable
-            Distance function. The only available option is ``gaussian_kernel``
+            Distance function.
         sum_stat: str or callable
-            Summary statistics. Available options are ``indentity``, ``sorted``, ``mean``,
-            ``median``. The user can pass any valid Python function
+            Summary statistics.
+        size : int
+            Number of simulated datasets to save. When this number is exceeded the counter will be
+            restored to zero and it will start saving again.
+        save : bool
+            whether to save or not the simulated data.
         """
         self.epsilon = epsilon
         self.function = function
         self.params = params
         self.model = model
         self.var_info = var_info
         self.variables = variables
         self.varnames = [v.name for v in self.variables]
+        self.distance = distance
+        self.sum_stat = sum_stat
         self.unobserved_RVs = [v.name for v in self.model.unobserved_RVs]
         self.get_unobserved_fn = self.model.fastfn(self.model.unobserved_RVs)
-
-        if sum_stat == "identity":
-            self.sum_stat = lambda x: x
-        elif sum_stat == "sorted":
-            self.sum_stat = np.sort
-        elif sum_stat == "mean":
-            self.sum_stat = np.mean
-        elif sum_stat == "median":
-            self.sum_stat = np.median
-        elif hasattr(sum_stat, "__call__"):
-            self.sum_stat = sum_stat
-        else:
-            raise ValueError(f"The summary statistics {sum_stat} is not implemented")
+        self.size = size
+        self.save = save
+        self.lista = []
 
         self.observations = self.sum_stat(observations)
 
-        if distance == "gaussian_kernel":
-            self.distance = self.gaussian_kernel
-        elif hasattr(distance, "__call__"):
-            self.distance = distance
-        else:
-            raise ValueError(f"The distance metric {distance} is not implemented")
-
     def posterior_to_function(self, posterior):
         model = self.model
         var_info = self.var_info
 
         varvalues = []
         samples = {}
         size = 0
@@ -463,14 +353,21 @@
             size += new_size
         point = {k: v for k, v in zip(self.varnames, varvalues)}
         for varname, value in zip(self.unobserved_RVs, self.get_unobserved_fn(point)):
             if varname in self.params:
                 samples[varname] = value
         return samples
 
-    def gaussian_kernel(self, obs_data, sim_data):
-        return np.sum(-0.5 * ((obs_data - sim_data) / self.epsilon) ** 2)
+    def save_data(self, sim_data):
+        if len(self.lista) == self.size:
+            self.lista = []
+        self.lista.append(sim_data)
+
+    def get_data(self):
+        return np.array(self.lista)
 
     def __call__(self, posterior):
         func_parameters = self.posterior_to_function(posterior)
-        sim_data = self.sum_stat(self.function(**func_parameters))
-        return self.distance(self.observations, sim_data)
+        sim_data = self.function(**func_parameters)
+        if self.save:
+            self.save_data(sim_data)
+        return self.distance(self.epsilon, self.observations, self.sum_stat(sim_data))
```

### Comparing `pymc3-3.9.2/pymc3/stats/__init__.py` & `pymc3-3.9.3/pymc3/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/__init__.py` & `pymc3-3.9.3/pymc3/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/arraystep.py` & `pymc3-3.9.3/pymc3/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/compound.py` & `pymc3-3.9.3/pymc3/step_methods/compound.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/elliptical_slice.py` & `pymc3-3.9.3/pymc3/step_methods/elliptical_slice.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/gibbs.py` & `pymc3-3.9.3/pymc3/step_methods/gibbs.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/hmc/__init__.py` & `pymc3-3.9.3/pymc3/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/hmc/base_hmc.py` & `pymc3-3.9.3/pymc3/step_methods/hmc/base_hmc.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 from collections import namedtuple
+import time
 
 import numpy as np
 import logging
 from pymc3.model import modelcontext, Point
 from pymc3.step_methods import arraystep
 from pymc3.step_methods.hmc import integration
 from pymc3.theanof import inputvars, floatX
@@ -24,19 +25,25 @@
 from .quadpotential import quad_potential, QuadPotentialDiagAdapt
 from pymc3.step_methods import step_sizes
 from pymc3.backends.report import SamplerWarning, WarningType
 from pymc3.exceptions import SamplingError
 
 logger = logging.getLogger("pymc3")
 
-HMCStepData = namedtuple("HMCStepData", "end, accept_stat, divergence_info, stats")
+HMCStepData = namedtuple(
+    "HMCStepData",
+    "end, accept_stat, divergence_info, stats"
+)
+
+DivergenceInfo = namedtuple(
+    "DivergenceInfo",
+    "message, exec_info, state, state_div"
+)
 
 
-DivergenceInfo = namedtuple("DivergenceInfo", "message, exec_info, state")
-
 class BaseHMC(arraystep.GradientSharedStep):
     """Superclass to implement Hamiltonian/hybrid monte carlo."""
 
     default_blocked = True
 
     def __init__(
         self,
@@ -128,74 +135,98 @@
 
         Subclasses must overwrite this method and return a `HMCStepData`.
         """
         raise NotImplementedError("Abstract method")
 
     def astep(self, q0):
         """Perform a single HMC iteration."""
+        perf_start = time.perf_counter()
+        process_start = time.process_time()
+
         p0 = self.potential.random()
         start = self.integrator.compute_state(q0, p0)
 
         if not np.isfinite(start.energy):
             model = self._model
             check_test_point = model.check_test_point()
             error_logp = check_test_point.loc[
                 (np.abs(check_test_point) >= 1e20) | np.isnan(check_test_point)
             ]
             self.potential.raise_ok(self._logp_dlogp_func._ordering.vmap)
             message_energy = (
                 "Bad initial energy, check any log probabilities that "
-                "are inf or -inf, nan or very small:\n{}".format(error_logp.to_string())
+                "are inf or -inf, nan or very small:\n{}"
+                .format(error_logp.to_string())
             )
             warning = SamplerWarning(
                 WarningType.BAD_ENERGY,
                 message_energy,
                 "critical",
                 self.iter_count,
-                None,
-                None,
             )
             self._warnings.append(warning)
             raise SamplingError("Bad initial energy")
 
         adapt_step = self.tune and self.adapt_step_size
         step_size = self.step_adapt.current(adapt_step)
         self.step_size = step_size
 
         if self._step_rand is not None:
             step_size = self._step_rand(step_size)
 
         hmc_step = self._hamiltonian_step(start, p0, step_size)
 
+        perf_end = time.perf_counter()
+        process_end = time.process_time()
+
         self.step_adapt.update(hmc_step.accept_stat, adapt_step)
         self.potential.update(hmc_step.end.q, hmc_step.end.q_grad, self.tune)
         if hmc_step.divergence_info:
             info = hmc_step.divergence_info
+            point = None
+            point_dest = None
+            info_store = None
             if self.tune:
                 kind = WarningType.TUNING_DIVERGENCE
-                point = None
             else:
                 kind = WarningType.DIVERGENCE
                 self._num_divs_sample += 1
                 # We don't want to fill up all memory with divergence info
-                if self._num_divs_sample < 100:
+                if self._num_divs_sample < 100 and info.state is not None:
                     point = self._logp_dlogp_func.array_to_dict(info.state.q)
-                else:
-                    point = None
+                if self._num_divs_sample < 100 and info.state_div is not None:
+                    point_dest = self._logp_dlogp_func.array_to_dict(
+                        info.state_div.q
+                    )
+                if self._num_divs_sample < 100:
+                    info_store = info
             warning = SamplerWarning(
-                kind, info.message, "debug", self.iter_count, info.exec_info, point
+                kind,
+                info.message,
+                "debug",
+                self.iter_count,
+                info.exec_info,
+                divergence_point_source=point,
+                divergence_point_dest=point_dest,
+                divergence_info=info_store,
             )
 
             self._warnings.append(warning)
 
         self.iter_count += 1
         if not self.tune:
             self._samples_after_tune += 1
 
-        stats = {"tune": self.tune, "diverging": bool(hmc_step.divergence_info)}
+        stats = {
+            "tune": self.tune,
+            "diverging": bool(hmc_step.divergence_info),
+            "perf_counter_diff": perf_end - perf_start,
+            "process_time_diff": process_end - process_start,
+            "perf_counter_start": perf_start,
+        }
 
         stats.update(hmc_step.stats)
         stats.update(self.step_adapt.stats())
 
         return hmc_step.end.q, [stats]
 
     def reset_tuning(self, start=None):
@@ -226,14 +257,12 @@
         elif n_divs > 1:
             message = (
                 "There were %s divergences after tuning. Increase "
                 "`target_accept` or reparameterize." % n_divs
             )
 
         if message:
-            warning = SamplerWarning(
-                WarningType.DIVERGENCES, message, "error", None, None, None
-            )
+            warning = SamplerWarning(WarningType.DIVERGENCES, message, "error")
             warnings.append(warning)
 
         warnings.extend(self.step_adapt.warnings())
         return warnings
```

### Comparing `pymc3-3.9.2/pymc3/step_methods/hmc/hmc.py` & `pymc3-3.9.3/pymc3/step_methods/hmc/hmc.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         'accept': np.float64,
         'diverging': np.bool,
         'energy_error': np.float64,
         'energy': np.float64,
         'path_length': np.float64,
         'accepted': np.bool,
         'model_logp': np.float64,
+        'process_time_diff': np.float64,
+        'perf_counter_diff': np.float64,
+        'perf_counter_start': np.float64,
     }]
 
     def __init__(self, vars=None, path_length=2., max_steps=1024, **kwargs):
         """Set up the Hamiltonian Monte Carlo sampler.
 
         Parameters
         ----------
@@ -109,31 +112,33 @@
 
     def _hamiltonian_step(self, start, p0, step_size):
         n_steps = max(1, int(self.path_length / step_size))
         n_steps = min(self.max_steps, n_steps)
 
         energy_change = -np.inf
         state = start
+        last = state
         div_info = None
         try:
             for _ in range(n_steps):
+                last = state
                 state = self.integrator.step(step_size, state)
         except IntegrationError as e:
-            div_info = DivergenceInfo('Divergence encountered.', e, state)
+            div_info = DivergenceInfo('Integration failed.', e, last, None)
         else:
             if not np.isfinite(state.energy):
                 div_info = DivergenceInfo(
-                    'Divergence encountered, bad energy.', None, state)
+                    'Divergence encountered, bad energy.', None, last, state)
             energy_change = start.energy - state.energy
             if np.isnan(energy_change):
                 energy_change = -np.inf
             if np.abs(energy_change) > self.Emax:
                 div_info = DivergenceInfo(
                     'Divergence encountered, large integration error.',
-                    None, state)
+                    None, last, state)
 
         accept_stat = min(1, np.exp(energy_change))
 
         if div_info is not None or np.random.rand() >= accept_stat:
             end = start
             accepted = False
         else:
```

### Comparing `pymc3-3.9.2/pymc3/step_methods/hmc/integration.py` & `pymc3-3.9.3/pymc3/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/hmc/nuts.py` & `pymc3-3.9.3/pymc3/step_methods/hmc/nuts.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,21 @@
     - `tune`: This is `True`, if step size adaptation was turned on when
       this sample was generated.
     - `step_size`: The step size used for this sample.
     - `step_size_bar`: The current best known step-size. After the tuning
       samples, the step size is set to this value. This should converge
       during tuning.
     - `model_logp`: The model log-likelihood for this sample.
+    - `process_time_diff`: The time it took to draw the sample, as defined
+      by the python standard library `time.process_time`. This counts all
+      the CPU time, including worker processes in BLAS and OpenMP.
+    - `perf_counter_diff`: The time it took to draw the sample, as defined
+      by the python standard library `time.perf_counter` (wall time).
+    - `perf_counter_start`: The value of `time.perf_counter` at the beginning
+      of the computation of the draw.
 
     References
     ----------
     .. [1] Hoffman, Matthew D., & Gelman, Andrew. (2011). The No-U-Turn
        Sampler: Adaptively Setting Path Lengths in Hamiltonian Monte Carlo.
     """
 
@@ -92,14 +99,17 @@
             "step_size_bar": np.float64,
             "tree_size": np.float64,
             "diverging": np.bool,
             "energy_error": np.float64,
             "energy": np.float64,
             "max_energy_error": np.float64,
             "model_logp": np.float64,
+            "process_time_diff": np.float64,
+            "perf_counter_diff": np.float64,
+            "perf_counter_start": np.float64,
         }
     ]
 
     def __init__(self, vars=None, max_treedepth=10, early_max_treedepth=8, **kwargs):
         r"""Set up the No-U-Turn sampler.
 
         Parameters
@@ -196,15 +206,15 @@
         n_treedepth = self._reached_max_treedepth
 
         if n_samples > 0 and n_treedepth / float(n_samples) > 0.05:
             msg = (
                 "The chain reached the maximum tree depth. Increase "
                 "max_treedepth, increase target_accept or reparameterize."
             )
-            warn = SamplerWarning(WarningType.TREEDEPTH, msg, "warn", None, None, None)
+            warn = SamplerWarning(WarningType.TREEDEPTH, msg, 'warn')
             warnings.append(warn)
         return warnings
 
 
 # A proposal for the next position
 Proposal = namedtuple("Proposal", "q, q_grad, energy, log_p_accept_weighted, logp")
 
@@ -317,14 +327,15 @@
     def _single_step(self, left, epsilon):
         """Perform a leapfrog step and handle error cases."""
         try:
             right = self.integrator.step(epsilon, left)
         except IntegrationError as err:
             error_msg = str(err)
             error = err
+            right = None
         else:
             # h - H0
             energy_change = right.energy - self.start_energy
             if np.isnan(energy_change):
                 energy_change = np.inf
 
             if np.abs(energy_change) > np.abs(self.max_energy_change):
@@ -349,15 +360,15 @@
                 return tree, None, False
             else:
                 error_msg = (
                     "Energy change in leapfrog step is too large: %s." % energy_change
                 )
                 error = None
         tree = Subtree(None, None, None, None, -np.inf, -np.inf, 1)
-        divergance_info = DivergenceInfo(error_msg, error, left)
+        divergance_info = DivergenceInfo(error_msg, error, left, right)
         return tree, divergance_info, False
 
     def _build_subtree(self, left, depth, epsilon):
         if depth == 0:
             return self._single_step(left, epsilon)
 
         tree1, diverging, turning = self._build_subtree(left, depth - 1, epsilon)
```

### Comparing `pymc3-3.9.2/pymc3/step_methods/hmc/quadpotential.py` & `pymc3-3.9.3/pymc3/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/metropolis.py` & `pymc3-3.9.3/pymc3/step_methods/metropolis.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/sgmcmc.py` & `pymc3-3.9.3/pymc3/step_methods/sgmcmc.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/slicer.py` & `pymc3-3.9.3/pymc3/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/step_methods/step_sizes.py` & `pymc3-3.9.3/pymc3/step_methods/step_sizes.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,11 +73,11 @@
         if target_accept < lower or target_accept > upper:
             msg = ('The acceptance probability does not match the target. It '
                    'is %s, but should be close to %s. Try to increase the '
                    'number of tuning steps.'
                    % (mean_accept, target_accept))
             info = {'target': target_accept, 'actual': mean_accept}
             warning = SamplerWarning(
-                WarningType.BAD_ACCEPTANCE, msg, 'warn', None, None, info)
+                WarningType.BAD_ACCEPTANCE, msg, 'warn', extra=info)
             return [warning]
         else:
             return []
```

### Comparing `pymc3-3.9.2/pymc3/tests/__init__.py` & `pymc3-3.9.3/pymc3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/backend_fixtures.py` & `pymc3-3.9.3/pymc3/tests/backend_fixtures.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/checks.py` & `pymc3-3.9.3/pymc3/tests/checks.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/conftest.py` & `pymc3-3.9.3/pymc3/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,12 +40,12 @@
             warn_float64='raise')
         with config:
             yield
     else:
         yield
 
 
-@pytest.fixture('function', autouse=False)
+@pytest.fixture(scope='function', autouse=False)
 def seeded_test():
     # TODO: use this instead of SeededTest
     np.random.seed(42)
     pm.set_tt_rng(42)
```

### Comparing `pymc3-3.9.2/pymc3/tests/helpers.py` & `pymc3-3.9.3/pymc3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/models.py` & `pymc3-3.9.3/pymc3/tests/models.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/sampler_fixtures.py` & `pymc3-3.9.3/pymc3/tests/sampler_fixtures.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_data_container.py` & `pymc3-3.9.3/pymc3/tests/test_data_container.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_dist_math.py` & `pymc3-3.9.3/pymc3/tests/test_dist_math.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,19 +122,19 @@
 
 def test_multinomial_bound():
 
     x = np.array([1, 5])
     n = x.sum()
 
     with pm.Model() as modelA:
-        p_a = pm.Dirichlet('p', floatX(np.ones(2)))
+        p_a = pm.Dirichlet('p', floatX(np.ones(2)), shape=(2,))
         MultinomialA('x', n, p_a, observed=x)
 
     with pm.Model() as modelB:
-        p_b = pm.Dirichlet('p', floatX(np.ones(2)))
+        p_b = pm.Dirichlet('p', floatX(np.ones(2)), shape=(2,))
         MultinomialB('x', n, p_b, observed=x)
 
     assert np.isclose(modelA.logp({'p_stickbreaking__': [0]}),
                       modelB.logp({'p_stickbreaking__': [0]}))
 
 
 class TestMvNormalLogp():
```

### Comparing `pymc3-3.9.2/pymc3/tests/test_distribution_defaults.py` & `pymc3-3.9.3/pymc3/tests/test_distribution_defaults.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_distributions.py` & `pymc3-3.9.3/pymc3/tests/test_distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1324,25 +1324,22 @@
 
     @pytest.mark.parametrize("n", [2, 3])
     def test_dirichlet(self, n):
         self.pymc3_matches_scipy(
             Dirichlet, Simplex(n), {"a": Vector(Rplus, n)}, dirichlet_logpdf
         )
 
-    @pytest.mark.parametrize("n", [3, 4])
-    def test_dirichlet_init_fail(self, n):
-        with Model():
-            with pytest.raises(
-                ValueError, match=r"All concentration parameters \(a\) must be > 0."
-            ):
-                _ = Dirichlet("x", a=np.zeros(n), shape=n)
-            with pytest.raises(
-                ValueError, match=r"All concentration parameters \(a\) must be > 0."
-            ):
-                _ = Dirichlet("x", a=np.array([-1.0] * n), shape=n)
+    def test_dirichlet_shape(self):
+        a = tt.as_tensor_variable(np.r_[1, 2])
+        with pytest.warns(DeprecationWarning):
+            dir_rv = Dirichlet.dist(a)
+            assert dir_rv.shape == (2,)
+
+        with pytest.warns(DeprecationWarning), theano.change_flags(compute_test_value="ignore"):
+            dir_rv = Dirichlet.dist(tt.vector())
 
     def test_dirichlet_2D(self):
         self.pymc3_matches_scipy(
             Dirichlet,
             MultiSimplex(2, 2),
             {"a": Vector(Vector(Rplus, 2), 2)},
             dirichlet_logpdf,
```

### Comparing `pymc3-3.9.2/pymc3/tests/test_distributions_random.py` & `pymc3-3.9.3/pymc3/tests/test_distributions_random.py`

 * *Files 0% similar despite different names*

```diff
@@ -908,23 +908,23 @@
 
 def test_mixture_random_shape():
     # test the shape broadcasting in mixture random
     y = np.concatenate([nr.poisson(5, size=10),
                         nr.poisson(9, size=10)])
     with pm.Model() as m:
         comp0 = pm.Poisson.dist(mu=np.ones(2))
-        w0 = pm.Dirichlet('w0', a=np.ones(2))
+        w0 = pm.Dirichlet('w0', a=np.ones(2), shape=(2,))
         like0 = pm.Mixture('like0',
                            w=w0,
                            comp_dists=comp0,
                            observed=y)
 
         comp1 = pm.Poisson.dist(mu=np.ones((20, 2)),
                                 shape=(20, 2))
-        w1 = pm.Dirichlet('w1', a=np.ones(2))
+        w1 = pm.Dirichlet('w1', a=np.ones(2), shape=(2,))
         like1 = pm.Mixture('like1',
                            w=w1,
                            comp_dists=comp1,
                            observed=y)
 
         comp2 = pm.Poisson.dist(mu=np.ones(2))
         w2 = pm.Dirichlet('w2',
@@ -963,23 +963,23 @@
 @pytest.mark.xfail
 def test_mixture_random_shape_fast():
     # test the shape broadcasting in mixture random
     y = np.concatenate([nr.poisson(5, size=10),
                         nr.poisson(9, size=10)])
     with pm.Model() as m:
         comp0 = pm.Poisson.dist(mu=np.ones(2))
-        w0 = pm.Dirichlet('w0', a=np.ones(2))
+        w0 = pm.Dirichlet('w0', a=np.ones(2), shape=(2,))
         like0 = pm.Mixture('like0',
                            w=w0,
                            comp_dists=comp0,
                            observed=y)
 
         comp1 = pm.Poisson.dist(mu=np.ones((20, 2)),
                                 shape=(20, 2))
-        w1 = pm.Dirichlet('w1', a=np.ones(2))
+        w1 = pm.Dirichlet('w1', a=np.ones(2), shape=(2,))
         like1 = pm.Mixture('like1',
                            w=w1,
                            comp_dists=comp1,
                            observed=y)
 
         comp2 = pm.Poisson.dist(mu=np.ones(2))
         w2 = pm.Dirichlet('w2',
```

### Comparing `pymc3-3.9.2/pymc3/tests/test_distributions_timeseries.py` & `pymc3-3.9.3/pymc3/tests/test_distributions_timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_examples.py` & `pymc3-3.9.3/pymc3/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,22 @@
 import numpy as np
 import pandas as pd
 import pymc3 as pm
 import theano.tensor as tt
 import pytest
 import theano
 from pymc3.theanof import floatX
+from packaging import version
 
 from .helpers import SeededTest
 
-matplotlib.use('Agg', warn=False)
+if version.parse(matplotlib.__version__) < version.parse('3.3'):
+    matplotlib.use('Agg', warn=False)
+else:
+    matplotlib.use('Agg')
 
 
 def get_city_data():
     """Helper to get city data"""
     data = pd.read_csv(pm.get_data('srrs2.dat'))
     cty_data = pd.read_csv(pm.get_data('cty.dat'))
```

### Comparing `pymc3-3.9.2/pymc3/tests/test_glm.py` & `pymc3-3.9.3/pymc3/tests/test_glm.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_gp.py` & `pymc3-3.9.3/pymc3/tests/test_gp.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_hdf5_backend.py` & `pymc3-3.9.3/pymc3/tests/test_hdf5_backend.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_hmc.py` & `pymc3-3.9.3/pymc3/tests/test_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_math.py` & `pymc3-3.9.3/pymc3/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_memo.py` & `pymc3-3.9.3/pymc3/tests/test_memo.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_minibatches.py` & `pymc3-3.9.3/pymc3/tests/test_minibatches.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                         high=self.data.shape[0] - 1e-16)
                .astype('int64'))
         return np.asarray(self.data[idx], self.dtype)
 
     next = __next__
 
 
-@pytest.fixture('module')
+@pytest.fixture(scope='module')
 def datagen():
     return _DataSampler(np.random.uniform(size=(1000, 10)))
 
 
 def integers():
     i = 0
     while True:
```

### Comparing `pymc3-3.9.2/pymc3/tests/test_missing.py` & `pymc3-3.9.3/pymc3/tests/test_missing.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_mixture.py` & `pymc3-3.9.3/pymc3/tests/test_mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,28 @@
         cls.norm_sd = np.ones_like(cls.norm_mu)
         cls.norm_x = generate_normal_mixture_data(cls.norm_w, cls.norm_mu, cls.norm_sd, size=1000)
 
         cls.pois_w = np.array([0.4, 0.6])
         cls.pois_mu = np.array([5., 20.])
         cls.pois_x = generate_poisson_mixture_data(cls.pois_w, cls.pois_mu, size=1000)
 
+    def test_dimensions(self):
+        a1 = Normal.dist(mu=0, sigma=1)
+        a2 = Normal.dist(mu=10, sigma=1)
+        mix = Mixture.dist(w=np.r_[0.5, 0.5], comp_dists=[a1, a2])
+
+        assert mix.mode.ndim == 0
+        assert mix.logp(0.0).ndim == 0
+
+        value = np.r_[0.0, 1.0, 2.0]
+        assert mix.logp(value).ndim == 1
+
     def test_mixture_list_of_normals(self):
         with Model() as model:
-            w = Dirichlet('w', floatX(np.ones_like(self.norm_w)))
+            w = Dirichlet('w', floatX(np.ones_like(self.norm_w)), shape=self.norm_w.size)
             mu = Normal('mu', 0., 10., shape=self.norm_w.size)
             tau = Gamma('tau', 1., 1., shape=self.norm_w.size)
             Mixture('x_obs', w,
                     [Normal.dist(mu[0], tau=tau[0]), Normal.dist(mu[1], tau=tau[1])],
                     observed=self.norm_x)
             step = Metropolis()
             trace = sample(5000, step, random_seed=self.random_seed,
@@ -83,15 +94,15 @@
                         rtol=0.1, atol=0.1)
         assert_allclose(np.sort(trace['mu'].mean(axis=0)),
                         np.sort(self.norm_mu),
                         rtol=0.1, atol=0.1)
 
     def test_normal_mixture(self):
         with Model() as model:
-            w = Dirichlet('w', floatX(np.ones_like(self.norm_w)))
+            w = Dirichlet('w', floatX(np.ones_like(self.norm_w)), shape=self.norm_w.size)
             mu = Normal('mu', 0., 10., shape=self.norm_w.size)
             tau = Gamma('tau', 1., 1., shape=self.norm_w.size)
             NormalMixture('x_obs', w, mu, tau=tau, observed=self.norm_x)
             step = Metropolis()
             trace = sample(5000, step, random_seed=self.random_seed,
                            progressbar=False, chains=1)
 
@@ -120,25 +131,25 @@
                                                 mu=test_mus,
                                                 sd=1/np.sqrt(test_taus),
                                                 size=10)
 
         with Model() as model0:
             mus = Normal('mus', shape=comp_shape)
             taus = Gamma('taus', alpha=1, beta=1, shape=comp_shape)
-            ws = Dirichlet('ws', np.ones(ncomp))
+            ws = Dirichlet('ws', np.ones(ncomp), shape=(ncomp,))
             mixture0 = NormalMixture('m', w=ws, mu=mus, tau=taus, shape=nd,
                                      comp_shape=comp_shape)
             obs0 = NormalMixture('obs', w=ws, mu=mus, tau=taus, shape=nd,
                                  comp_shape=comp_shape,
                                  observed=observed)
 
         with Model() as model1:
             mus = Normal('mus', shape=comp_shape)
             taus = Gamma('taus', alpha=1, beta=1, shape=comp_shape)
-            ws = Dirichlet('ws', np.ones(ncomp))
+            ws = Dirichlet('ws', np.ones(ncomp), shape=(ncomp,))
             comp_dist = [Normal.dist(mu=mus[..., i], tau=taus[..., i],
                                      shape=nd)
                          for i in range(ncomp)]
             mixture1 = Mixture('m', w=ws, comp_dists=comp_dist, shape=nd)
             obs1 = Mixture('obs', w=ws, comp_dists=comp_dist, shape=nd,
                            observed=observed)
 
@@ -148,15 +159,15 @@
             # it does broadcast, an error is raised if the mixture is given
             # observed data.
             # Furthermore, the Mixture will also raise errors when the observed
             # data is multidimensional but it does not broadcast well with
             # comp_dists.
             mus = Normal('mus', shape=comp_shape)
             taus = Gamma('taus', alpha=1, beta=1, shape=comp_shape)
-            ws = Dirichlet('ws', np.ones(ncomp))
+            ws = Dirichlet('ws', np.ones(ncomp), shape=(ncomp,))
             if len(nd) > 1:
                 if nd[-1] != ncomp:
                     with pytest.raises(ValueError):
                         NormalMixture('m', w=ws, mu=mus, tau=taus,
                                       shape=nd)
                     mixture2 = None
                 else:
@@ -193,15 +204,15 @@
         if mixture2 is not None:
             assert_allclose(mixture0.logp(testpoint), mixture2.logp(testpoint))
         if obs2 is not None:
             assert_allclose(obs0.logp(testpoint), obs2.logp(testpoint))
 
     def test_poisson_mixture(self):
         with Model() as model:
-            w = Dirichlet('w', floatX(np.ones_like(self.pois_w)))
+            w = Dirichlet('w', floatX(np.ones_like(self.pois_w)), shape=self.pois_w.shape)
             mu = Gamma('mu', 1., 1., shape=self.pois_w.size)
             Mixture('x_obs', w, Poisson.dist(mu), observed=self.pois_x)
             step = Metropolis()
             trace = sample(5000, step, random_seed=self.random_seed,
                            progressbar=False, chains=1)
 
         assert_allclose(np.sort(trace['w'].mean(axis=0)),
@@ -209,15 +220,15 @@
                         rtol=0.1, atol=0.1)
         assert_allclose(np.sort(trace['mu'].mean(axis=0)),
                         np.sort(self.pois_mu),
                         rtol=0.1, atol=0.1)
 
     def test_mixture_list_of_poissons(self):
         with Model() as model:
-            w = Dirichlet('w', floatX(np.ones_like(self.pois_w)))
+            w = Dirichlet('w', floatX(np.ones_like(self.pois_w)), shape=self.pois_w.shape)
             mu = Gamma('mu', 1., 1., shape=self.pois_w.size)
             Mixture('x_obs', w,
                     [Poisson.dist(mu[0]), Poisson.dist(mu[1])],
                     observed=self.pois_x)
             step = Metropolis()
             trace = sample(5000, step, random_seed=self.random_seed,
                            progressbar=False, chains=1)
@@ -232,15 +243,15 @@
     def test_mixture_of_mvn(self):
         mu1 = np.asarray([0., 1.])
         cov1 = np.diag([1.5, 2.5])
         mu2 = np.asarray([1., 0.])
         cov2 = np.diag([2.5, 3.5])
         obs = np.asarray([[.5, .5], mu1, mu2])
         with Model() as model:
-            w = Dirichlet('w', floatX(np.ones(2)), transform=None)
+            w = Dirichlet('w', floatX(np.ones(2)), transform=None, shape=(2,))
             mvncomp1 = MvNormal.dist(mu=mu1, cov=cov1)
             mvncomp2 = MvNormal.dist(mu=mu2, cov=cov2)
             y = Mixture('x_obs', w, [mvncomp1, mvncomp2],
                     observed=obs)
 
         # check logp of each component
         complogp_st = np.vstack((st.multivariate_normal.logpdf(obs, mu1, cov1),
@@ -248,15 +259,15 @@
                                 ).T
         complogp = y.distribution._comp_logp(theano.shared(obs)).eval()
         assert_allclose(complogp, complogp_st)
 
         # check logp of mixture
         testpoint = model.test_point
         mixlogp_st = logsumexp(np.log(testpoint['w']) + complogp_st,
-                               axis=-1, keepdims=True)
+                               axis=-1, keepdims=False)
         assert_allclose(y.logp_elemwise(testpoint),
                         mixlogp_st)
 
         # check logp of model
         priorlogp = st.dirichlet.logpdf(x=testpoint['w'],
                                         alpha=np.ones(2),
                                         )
@@ -276,21 +287,21 @@
                 sigma=1,
                 shape=nbr)
             l_comp = Lognormal.dist(
                 mu=Exponential('mu_l', lam=1.0, shape=nbr, transform=None),
                 sigma=1,
                 shape=nbr)
             # weight vector for the mixtures
-            g_w = Dirichlet('g_w', a=floatX(np.ones(nbr)*0.0000001), transform=None)
-            l_w = Dirichlet('l_w', a=floatX(np.ones(nbr)*0.0000001), transform=None)
+            g_w = Dirichlet('g_w', a=floatX(np.ones(nbr)*0.0000001), transform=None, shape=(nbr,))
+            l_w = Dirichlet('l_w', a=floatX(np.ones(nbr)*0.0000001), transform=None, shape=(nbr,))
             # mixture components
             g_mix = Mixture.dist(w=g_w, comp_dists=g_comp)
             l_mix = Mixture.dist(w=l_w, comp_dists=l_comp)
             # mixture of mixtures
-            mix_w = Dirichlet('mix_w', a=floatX(np.ones(2)), transform=None)
+            mix_w = Dirichlet('mix_w', a=floatX(np.ones(2)), transform=None, shape=(2,))
             mix = Mixture('mix', w=mix_w,
                           comp_dists=[g_mix, l_mix],
                           observed=np.exp(self.norm_x))
 
         test_point = model.test_point
 
         def mixmixlogp(value, point):
@@ -317,15 +328,15 @@
                                           np.exp(point['mu_l'])).astype(floatX)
             mixlogp2 = logsumexp(np.log(point['l_w']).astype(floatX) +
                                  complogp2,
                                  axis=-1, keepdims=True)
             complogp_mix = np.concatenate((mixlogp1, mixlogp2), axis=1)
             mixmixlogpg = logsumexp(np.log(point['mix_w']).astype(floatX) +
                                     complogp_mix,
-                                    axis=-1, keepdims=True)
+                                    axis=-1, keepdims=False)
             return priorlogp, mixmixlogpg
 
         value = np.exp(self.norm_x)[:, None]
         priorlogp, mixmixlogpg = mixmixlogp(value, test_point)
 
         # check logp of mixture
         assert_allclose(mixmixlogpg, mix.logp_elemwise(test_point),
@@ -363,15 +374,15 @@
         N = 100  # number of data points
         K = 3  # number of mixture components
         D = 3  # dimensionality of the data
 
         X, y = build_toy_dataset(N, K)
 
         with pm.Model() as model:
-            pi = pm.Dirichlet('pi', np.ones(K))
+            pi = pm.Dirichlet('pi', np.ones(K), shape=(K,))
 
             comp_dist = []
             mu = []
             packed_chol = []
             chol = []
             for i in range(K):
                 mu.append(pm.Normal('mu%i' % i, 0, 10, shape=D))
```

### Comparing `pymc3-3.9.2/pymc3/tests/test_model.py` & `pymc3-3.9.3/pymc3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_model_func.py` & `pymc3-3.9.3/pymc3/tests/test_model_func.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_model_graph.py` & `pymc3-3.9.3/pymc3/tests/test_model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_model_helpers.py` & `pymc3-3.9.3/pymc3/tests/test_model_helpers.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_modelcontext.py` & `pymc3-3.9.3/pymc3/tests/test_modelcontext.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_models_linear.py` & `pymc3-3.9.3/pymc3/tests/test_models_linear.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_models_utils.py` & `pymc3-3.9.3/pymc3/tests/test_models_utils.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_ndarray_backend.py` & `pymc3-3.9.3/pymc3/tests/test_ndarray_backend.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_ode.py` & `pymc3-3.9.3/pymc3/tests/test_ode.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_pickling.py` & `pymc3-3.9.3/pymc3/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_posdef_sym.py` & `pymc3-3.9.3/pymc3/tests/test_posdef_sym.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_posterior_predictive.py` & `pymc3-3.9.3/pymc3/tests/test_posterior_predictive.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_posteriors.py` & `pymc3-3.9.3/pymc3/tests/test_posteriors.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_profile.py` & `pymc3-3.9.3/pymc3/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_quadpotential.py` & `pymc3-3.9.3/pymc3/tests/test_quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_random.py` & `pymc3-3.9.3/pymc3/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_sampling.py` & `pymc3-3.9.3/pymc3/tests/test_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,14 +377,21 @@
 
             # test keep_size parameter
             ppc = pm.sample_posterior_predictive(trace, keep_size=True)
             assert ppc["a"].shape == (nchains, ndraws)
             ppc = pm.fast_sample_posterior_predictive(trace, keep_size=True)
             assert ppc["a"].shape == (nchains, ndraws)
 
+            # test keep_size parameter and idata input
+            idata = az.from_pymc3(trace)
+            ppc = pm.sample_posterior_predictive(idata, keep_size=True)
+            assert ppc["a"].shape == (nchains, ndraws)
+            ppc = pm.fast_sample_posterior_predictive(trace, keep_size=True)
+            assert ppc["a"].shape == (nchains, ndraws)
+
             # test default case
             ppc = pm.sample_posterior_predictive(trace, var_names=["a"])
             assert "a" in ppc
             assert ppc["a"].shape == (nchains * ndraws,)
             # mu's standard deviation may have changed thanks to a's observed
             _, pval = stats.kstest(ppc["a"] - trace["mu"], stats.norm(loc=0, scale=1).cdf)
             assert pval > 0.001
@@ -424,22 +431,39 @@
             ppc = pm.sample_posterior_predictive(trace, keep_size=True)
             assert ppc["a"].shape == (trace.nchains, len(trace), 2)
             with pytest.warns(UserWarning):
                 ppc = pm.sample_posterior_predictive(trace, samples=12, var_names=["a"])
             assert "a" in ppc
             assert ppc["a"].shape == (12, 2)
 
+            # test keep_size parameter with inference data as input...
+            idata = az.from_pymc3(trace)
+            ppc = pm.sample_posterior_predictive(idata, keep_size=True)
+            assert ppc["a"].shape == (trace.nchains, len(trace), 2)
+            with pytest.warns(UserWarning):
+                ppc = pm.sample_posterior_predictive(trace, samples=12, var_names=["a"])
+            assert "a" in ppc
+            assert ppc["a"].shape == (12, 2)
+
             # test keep_size parameter
             ppc = pm.fast_sample_posterior_predictive(trace, keep_size=True)
             assert ppc["a"].shape == (trace.nchains, len(trace), 2)
             with pytest.warns(UserWarning):
                 ppc = pm.fast_sample_posterior_predictive(trace, samples=12, var_names=["a"])
             assert "a" in ppc
             assert ppc["a"].shape == (12, 2)
 
+            # test keep_size parameter with inference data as input
+            ppc = pm.fast_sample_posterior_predictive(idata, keep_size=True)
+            assert ppc["a"].shape == (trace.nchains, len(trace), 2)
+            with pytest.warns(UserWarning):
+                ppc = pm.fast_sample_posterior_predictive(trace, samples=12, var_names=["a"])
+            assert "a" in ppc
+            assert ppc["a"].shape == (12, 2)
+
 
             # size unsupported by fast_ version  argument. [2019/08/19:rpg]
             ppc = pm.sample_posterior_predictive(trace, samples=10, var_names=["a"], size=4)
             assert "a" in ppc
             assert ppc["a"].shape == (10, 4, 2)
 
     def test_exceptions(self, caplog):
@@ -455,14 +479,20 @@
                 ppc = pm.fast_sample_posterior_predictive(trace, samples=10, keep_size=True)
 
             # Not for fast_sample_posterior_predictive
             with pytest.raises(IncorrectArgumentsError):
                 ppc = pm.sample_posterior_predictive(trace, size=4, keep_size=True)
             with pytest.raises(IncorrectArgumentsError):
                 ppc = pm.sample_posterior_predictive(trace, vars=[a], var_names=["a"])
+            # test wrong type argument
+            bad_trace = {'mu': stats.norm.rvs(size=1000)}
+            with pytest.raises(TypeError):
+                ppc = pm.sample_posterior_predictive(bad_trace)
+            with pytest.raises(TypeError):
+                ppc = pm.fast_sample_posterior_predictive(bad_trace)
 
     def test_vector_observed(self):
         with pm.Model() as model:
             mu = pm.Normal("mu", mu=0, sigma=1)
             a = pm.Normal("a", mu=mu, sigma=1, observed=np.array([0.0, 1.0]))
             trace = pm.sample()
 
@@ -550,17 +580,15 @@
             trace = pm.sample(100)
 
         x_shared.set_value([-1, 0, 1.0])
         y_shared.set_value([0, 0, 0])
 
         samples = 100
         with model:
-            post_pred = pm.sample_posterior_predictive(
-                trace, samples=samples, var_names=["p", "obs"]
-            )
+            post_pred = pm.sample_posterior_predictive(trace, samples=samples, var_names=["p", "obs"])
 
         expected_p = np.array(
             [logistic.eval({coeff: val}) for val in trace["x"][:samples]]
         )
         assert post_pred["obs"].shape == (samples, 3)
         assert np.allclose(post_pred["p"], expected_p)
```

### Comparing `pymc3-3.9.2/pymc3/tests/test_shape_handling.py` & `pymc3-3.9.3/pymc3/tests/test_shape_handling.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_shared.py` & `pymc3-3.9.3/pymc3/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_special_functions.py` & `pymc3-3.9.3/pymc3/tests/test_special_functions.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_sqlite_backend.py` & `pymc3-3.9.3/pymc3/tests/test_sqlite_backend.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_starting.py` & `pymc3-3.9.3/pymc3/tests/test_starting.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_step.py` & `pymc3-3.9.3/pymc3/tests/test_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -975,15 +975,15 @@
                 trace.report.raise_ok()
             error.match("issues during sampling")
 
             assert not trace.report.ok
 
     def test_sampler_stats(self):
         with Model() as model:
-            x = Normal("x", mu=0, sigma=1)
+            Normal("x", mu=0, sigma=1)
             trace = sample(draws=10, tune=1, chains=1)
 
         # Assert stats exist and have the correct shape.
         expected_stat_names = {
             "depth",
             "diverging",
             "energy",
@@ -991,18 +991,22 @@
             "model_logp",
             "max_energy_error",
             "mean_tree_accept",
             "step_size",
             "step_size_bar",
             "tree_size",
             "tune",
+            "perf_counter_diff",
+            "perf_counter_start",
+            "process_time_diff",
         }
         assert trace.stat_names == expected_stat_names
         for varname in trace.stat_names:
             assert trace.get_sampler_stats(varname).shape == (10,)
 
         # Assert model logp is computed correctly: computing post-sampling
         # and tracking while sampling should give same results.
-        model_logp_ = np.array(
-            [model.logp(trace.point(i, chain=c)) for c in trace.chains for i in range(len(trace))]
-        )
+        model_logp_ = np.array([
+            model.logp(trace.point(i, chain=c))
+            for c in trace.chains for i in range(len(trace))
+        ])
         assert (trace.model_logp == model_logp_).all()
```

### Comparing `pymc3-3.9.2/pymc3/tests/test_text_backend.py` & `pymc3-3.9.3/pymc3/tests/test_text_backend.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_theanof.py` & `pymc3-3.9.3/pymc3/tests/test_theanof.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_tracetab.py` & `pymc3-3.9.3/pymc3/tests/test_tracetab.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_transforms.py` & `pymc3-3.9.3/pymc3/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_tuning.py` & `pymc3-3.9.3/pymc3/tests/test_tuning.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_types.py` & `pymc3-3.9.3/pymc3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_updates.py` & `pymc3-3.9.3/pymc3/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_util.py` & `pymc3-3.9.3/pymc3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tests/test_variational_inference.py` & `pymc3-3.9.3/pymc3/tests/test_variational_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     tracker = pm.callbacks.Tracker(
         bad=lambda t: t  # bad signature
     )
     with pytest.raises(TypeError):
         tracker(None, None, 1)
 
 
-@pytest.fixture('module')
+@pytest.fixture(scope='module')
 def three_var_model():
     with pm.Model() as model:
         pm.HalfNormal('one', shape=(10, 2), total_size=100)
         pm.Normal('two', shape=(10, ))
         pm.Normal('three', shape=(10, 1, 2))
     return model
 
@@ -569,15 +569,15 @@
             with pm.theanof.change_flags(compute_test_value='off'):
                 elbo_via_beta_kl = -pm.operators.KL(mean_field_3, beta=beta)()(10000)
 
         np.testing.assert_allclose(elbo_via_total_size_scaled.eval(), elbo_via_beta_kl.eval(), rtol=0, atol=1e-1)
 
 
 @pytest.fixture(
-    'module',
+    scope='module',
     params=[True, False],
     ids=['mini', 'full']
 )
 def use_minibatch(request):
     return request.param
 
 
@@ -613,15 +613,15 @@
             sigma=simple_model_data['sigma0'], testval=0)
         pm.Normal('x', mu=mu_, sigma=simple_model_data['sigma'],
                   observed=simple_model_data['data'],
                   total_size=simple_model_data['n'])
     return model
 
 
-@pytest.fixture('module', params=[
+@pytest.fixture(scope='module', params=[
         dict(cls=NFVI, init=dict(flow='scale-loc')),
         dict(cls=ADVI, init=dict()),
         dict(cls=FullRankADVI, init=dict()),
         dict(cls=SVGD, init=dict(n_particles=500, jitter=1)),
         dict(cls=ASVGD, init=dict(temperature=1.)),
     ], ids=[
         'NFVI=scale-loc',
@@ -638,21 +638,21 @@
         k = init.copy()
         k.update(kw)
         return cls(**k)
     init_.cls = cls
     return init_
 
 
-@pytest.fixture('function')
+@pytest.fixture(scope='function')
 def inference(inference_spec, simple_model):
     with simple_model:
         return inference_spec()
 
 
-@pytest.fixture('function')
+@pytest.fixture(scope='function')
 def fit_kwargs(inference, use_minibatch):
     _select = {
         (ADVI, 'full'): dict(
             obj_optimizer=pm.adagrad_window(learning_rate=0.02, n_win=50),
             n=5000
         ),
         (ADVI, 'mini'): dict(
@@ -705,15 +705,15 @@
 def test_fit_oo(inference,
                 fit_kwargs,
                 simple_model_data):
     trace = inference.fit(**fit_kwargs).sample(10000)
     mu_post = simple_model_data['mu_post']
     d = simple_model_data['d']
     np.testing.assert_allclose(np.mean(trace['mu']), mu_post, rtol=0.05)
-    np.testing.assert_allclose(np.std(trace['mu']), np.sqrt(1. / d), rtol=0.1)
+    np.testing.assert_allclose(np.std(trace['mu']), np.sqrt(1. / d), rtol=0.2)
 
 
 def test_profile(inference):
     inference.run_profiling(n=100).summary()
 
 
 def test_remove_scan_op():
@@ -743,15 +743,15 @@
         inference_new = pm.KLqp(new_a)
         inference_new.fit(n=10)
         assert any(len(c) != 0 for c in inference_new.approx._cache.values())
         pymc3.memoize.clear_cache(inference_new.approx)
         assert all(len(c) == 0 for c in inference_new.approx._cache.values())
 
 
-@pytest.fixture('module')
+@pytest.fixture(scope='module')
 def another_simple_model():
     _model = models.simple_model()[1]
     with _model:
         pm.Potential('pot', tt.ones((10, 10)))
     return _model
 
 
@@ -794,15 +794,15 @@
         if error is not None:
             with pytest.raises(error):
                 fit(10, method=method, **kwargs)
         else:
             fit(10, method=method, **kwargs)
 
 
-@pytest.fixture('module')
+@pytest.fixture(scope='module')
 def aevb_model():
     with pm.Model() as model:
         pm.HalfNormal('x', shape=(2,), total_size=5)
         pm.Normal('y', shape=(2,))
     x = model.x
     y = model.y
     mu = theano.shared(x.init_value)
@@ -867,25 +867,25 @@
 def test_pickle_approx_aevb(three_var_aevb_approx):
     import pickle
     dump = pickle.dumps(three_var_aevb_approx)
     new = pickle.loads(dump)
     assert new.sample(1000)
 
 
-@pytest.fixture('module')
+@pytest.fixture(scope='module')
 def binomial_model():
     n_samples = 100
     xs = intX(np.random.binomial(n=1, p=0.2, size=n_samples))
     with pm.Model() as model:
         p = pm.Beta('p', alpha=1, beta=1)
         pm.Binomial('xs', n=1, p=p, observed=xs)
     return model
 
 
-@pytest.fixture('module')
+@pytest.fixture(scope='module')
 def binomial_model_inference(binomial_model, inference_spec):
     with binomial_model:
         return inference_spec()
 
 
 @pytest.mark.run(after='test_sample_replacements')
 def test_replacements(binomial_model_inference):
@@ -976,18 +976,18 @@
         x_new = pm.floatX(np.linspace(0, 10, 11))
         assert advi.sample_node(mean, more_replacements={inp: x_new}).eval().shape == (11, )
 
 
 def test_empirical_from_trace(another_simple_model):
     with another_simple_model:
         step = pm.Metropolis()
-        trace = pm.sample(100, step=step, chains=1)
+        trace = pm.sample(100, step=step, chains=1, tune=0)
         emp = Empirical(trace)
         assert emp.histogram.shape[0].eval() == 100
-        trace = pm.sample(100, step=step, chains=4)
+        trace = pm.sample(100, step=step, chains=4, tune=0)
         emp = Empirical(trace)
         assert emp.histogram.shape[0].eval() == 400
 
 
 @pytest.fixture(
     params=[
         dict(cls=flows.PlanarFlow, init=dict(jitter=.1)),
```

### Comparing `pymc3-3.9.2/pymc3/theanof.py` & `pymc3-3.9.3/pymc3/theanof.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tuning/__init__.py` & `pymc3-3.9.3/pymc3/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tuning/scaling.py` & `pymc3-3.9.3/pymc3/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/tuning/starting.py` & `pymc3-3.9.3/pymc3/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/util.py` & `pymc3-3.9.3/pymc3/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import re
 import functools
-from typing import List, Dict
+from typing import List, Dict, Tuple, Union
 
 import xarray
+import arviz
 from numpy import asscalar, ndarray
 
 
-LATEX_ESCAPE_RE = re.compile(r'(%|_|\$|#|&)', re.MULTILINE)
+LATEX_ESCAPE_RE = re.compile(r"(%|_|\$|#|&)", re.MULTILINE)
 
 
 def escape_latex(strng):
     r"""Consistently escape LaTeX special characters for _repr_latex_ in IPython
 
     Implementation taken from the IPython magic `format_latex`
 
@@ -39,16 +40,16 @@
 
     Returns
     -------
     str
         A string with LaTeX escaped
     """
     if strng is None:
-        return 'None'
-    return LATEX_ESCAPE_RE.sub(r'\\\1', strng)
+        return "None"
+    return LATEX_ESCAPE_RE.sub(r"\\\1", strng)
 
 
 def get_transformed_name(name, transform):
     r"""
     Consistent way of transforming names
 
     Parameters
@@ -76,15 +77,15 @@
         Name to check
 
     Returns
     -------
     bool
         Boolean, whether the string could have been produced by `get_transformed_name`
     """
-    return name.endswith('__') and name.count('_') >= 3
+    return name.endswith("__") and name.count("_") >= 3
 
 
 def get_untransformed_name(name):
     r"""
     Undo transformation in `get_transformed_name`. Throws ValueError if name wasn't transformed
 
     Parameters
@@ -94,16 +95,16 @@
 
     Returns
     -------
     str
         String with untransformed version of the name.
     """
     if not is_transformed_name(name):
-        raise ValueError('{} does not appear to be a transformed name'.format(name))
-    return '_'.join(name.split('_')[:-3])
+        raise ValueError("{} does not appear to be a transformed name".format(name))
+    return "_".join(name.split("_")[:-3])
 
 
 def get_default_varnames(var_iterator, include_transformed):
     r"""Helper to extract default varnames from a trace.
 
     Parameters
     ----------
@@ -125,49 +126,50 @@
 
 def get_variable_name(variable):
     r"""Returns the variable data type if it is a constant, otherwise
     returns the argument name.
     """
     name = variable.name
     if name is None:
-        if hasattr(variable, 'get_parents'):
+        if hasattr(variable, "get_parents"):
             try:
-                names = [get_variable_name(item)
-                         for item in variable.get_parents()[0].inputs]
+                names = [
+                    get_variable_name(item) for item in variable.get_parents()[0].inputs
+                ]
                 # do not escape_latex these, since it is not idempotent
-                return 'f(%s)' % ',~'.join([n for n in names if isinstance(n, str)])
+                return "f(%s)" % ",~".join([n for n in names if isinstance(n, str)])
             except IndexError:
                 pass
         value = variable.eval()
         if not value.shape:
             return asscalar(value)
-        return 'array'
-    return r'\text{%s}' % name
+        return "array"
+    return r"\text{%s}" % name
 
 
 def update_start_vals(a, b, model):
     r"""Update a with b, without overwriting existing keys. Values specified for
     transformed variables on the original scale are also transformed and inserted.
     """
     if model is not None:
         for free_RV in model.free_RVs:
             tname = free_RV.name
             for name in a:
                 if is_transformed_name(tname) and get_untransformed_name(tname) == name:
                     transform_func = [
-                        d.transformation for d in model.deterministics if d.name == name]
+                        d.transformation for d in model.deterministics if d.name == name
+                    ]
                     if transform_func:
-                        b[tname] = transform_func[0].forward_val(
-                            a[name], point=b)
+                        b[tname] = transform_func[0].forward_val(a[name], point=b)
 
     a.update({k: v for k, v in b.items() if k not in a})
 
 
 def get_transformed(z):
-    if hasattr(z, 'transformed'):
+    if hasattr(z, "transformed"):
         z = z.transformed
     return z
 
 
 def biwrap(wrapper):
     @functools.wraps(wrapper)
     def enhanced(*args, **kwargs):
@@ -178,26 +180,46 @@
             count = 0
         if len(args) > count:
             newfn = wrapper(*args, **kwargs)
             return newfn
         else:
             newwrapper = functools.partial(wrapper, *args, **kwargs)
             return newwrapper
+
     return enhanced
 
+
+# FIXME: this function is poorly named, because it returns a LIST of
+# points, not a dictionary of points.
 def dataset_to_point_dict(ds: xarray.Dataset) -> List[Dict[str, ndarray]]:
     # grab posterior samples for each variable
-    _samples = {
-        vn : ds[vn].values
-        for vn in ds.keys()
-    }
+    _samples: Dict[str, ndarray] = {vn: ds[vn].values for vn in ds.keys()}
     # make dicts
-    points = []
+    points: List[Dict[str, ndarray]] = []
+    vn: str
+    s: ndarray
     for c in ds.chain:
         for d in ds.draw:
-            points.append({
-                vn : s[c, d]
-                for vn, s in _samples.items()
-            })
+            points.append({vn: s[c, d] for vn, s in _samples.items()})
     # use the list of points
-    ds = points
-    return ds
+    return points
+
+
+def chains_and_samples(
+    data: Union[xarray.Dataset, arviz.InferenceData]
+) -> Tuple[int, int]:
+    """Extract and return number of chains and samples in xarray or arviz traces."""
+    dataset: xarray.Dataset
+    if isinstance(data, xarray.Dataset):
+        dataset = data
+    elif isinstance(data, arviz.InferenceData):
+        dataset = data.posterior
+    else:
+        raise ValueError(
+            "Argument must be xarray Dataset or arviz InferenceData. Got %s",
+            data.__class__,
+        )
+
+    coords = dataset.coords
+    nchains = coords["chain"].sizes["chain"]
+    nsamples = coords["draw"].sizes["draw"]
+    return nchains, nsamples
```

### Comparing `pymc3-3.9.2/pymc3/variational/__init__.py` & `pymc3-3.9.3/pymc3/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/variational/approximations.py` & `pymc3-3.9.3/pymc3/variational/approximations.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/variational/callbacks.py` & `pymc3-3.9.3/pymc3/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/variational/flows.py` & `pymc3-3.9.3/pymc3/variational/flows.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/variational/inference.py` & `pymc3-3.9.3/pymc3/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/variational/operators.py` & `pymc3-3.9.3/pymc3/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/variational/opvi.py` & `pymc3-3.9.3/pymc3/variational/opvi.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/variational/stein.py` & `pymc3-3.9.3/pymc3/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/variational/test_functions.py` & `pymc3-3.9.3/pymc3/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/variational/updates.py` & `pymc3-3.9.3/pymc3/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3/vartypes.py` & `pymc3-3.9.3/pymc3/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/pymc3.egg-info/SOURCES.txt` & `pymc3-3.9.3/pymc3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/scripts/install_miniconda.sh` & `pymc3-3.9.3/scripts/install_miniconda.sh`

 * *Files 20% similar despite different names*

```diff
@@ -42,9 +42,7 @@
 else
   echo "Miniconda already installed at ${INSTALL_FOLDER}.  Updating, adding to path and exiting"
 fi
 
 export PATH="$INSTALL_FOLDER/bin:$PATH"
 echo "Adding $INSTALL_FOLDER to PATH.  Consider adding it in your .rc file as well."
 conda update -q -y conda
-# Uninstalling miniconda's numpy to avoid conflicting versions when creating the test env
-pip uninstall -y numpy
```

### Comparing `pymc3-3.9.2/scripts/start_container.sh` & `pymc3-3.9.3/scripts/start_container.sh`

 * *Files identical despite different names*

### Comparing `pymc3-3.9.2/setup.py` & `pymc3-3.9.3/setup.py`

 * *Files identical despite different names*

