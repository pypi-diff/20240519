# Comparing `tmp/wfl-0.2.5.tar.gz` & `tmp/wfl-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfl-0.2.5.tar", last modified: Fri May 17 17:02:53 2024, max compression
+gzip compressed data, was "wfl-0.2.6.tar", last modified: Sun May 19 00:19:51 2024, max compression
```

## Comparing `wfl-0.2.5.tar` & `wfl-0.2.6.tar`

### file list

```diff
@@ -1,151 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.212019 wfl-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-17 17:02:53.212019 wfl-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 17:02:49.000000 wfl-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 17:02:53.212019 wfl-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-17 17:02:49.000000 wfl-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.196019 wfl-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_ace_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_atoms_and_dimers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_autoparallelize.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_batch_gap_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_buildcell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_calc_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_cli_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_configset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_descriptor_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_doc_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_flat_histo_to_nearby.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_gap_fitting_multistage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_gap_fitting_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_kspacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_mace_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_minimahopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_ndim_neigh_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_neb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_normal_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_outputspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_point_defects.py
--rw-r--r--   0 runner    (1001) docker     (127)    17757 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_remote_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_rng_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_select_greedy_fps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_select_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-17 17:02:49.000000 wfl-0.2.5/tests/test_version_str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.196019 wfl-0.2.5/wfl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.196019 wfl-0.2.5/wfl/autoparallelize/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/autoparallelize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/autoparallelize/autoparainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/autoparallelize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/autoparallelize/mpipool_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/autoparallelize/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/autoparallelize/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/autoparallelize/remoteinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/autoparallelize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.200019 wfl-0.2.5/wfl/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/aims.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/castep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/committee.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/espresso.py
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/mopac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.200019 wfl-0.2.5/wfl/calculators/orca/
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/orca/basinhopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/calculators/wfl_fileio_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.200019 wfl-0.2.5/wfl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/cli_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.200019 wfl-0.2.5/wfl/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/commands/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/commands/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/commands/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/commands/select.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5598 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/dft_convergence_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    60870 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/cli/gap_rss_iter_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    31413 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/configset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/descriptor_heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.204018 wfl-0.2.5/wfl/descriptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/descriptors/quippy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.204018 wfl-0.2.5/wfl/fit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20665 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/ace.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21419 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.204018 wfl-0.2.5/wfl/fit/gap/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/gap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/gap/glue_2b.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22213 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/gap/multistage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/gap/relocate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/gap/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/mace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.204018 wfl-0.2.5/wfl/fit/modify_database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/modify_database/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7599 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/modify_database/gap_rss_set_config_sigmas_from_convex_hull.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      777 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/modify_database/scale_orig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/modify_database/simple_factor_nonperiodic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5832 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/fit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.208019 wfl-0.2.5/wfl/generate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/atoms_and_dimers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/buildcell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.208019 wfl-0.2.5/wfl/generate/md/
--rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/md/abort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/md/abort_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/minimahopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/neb.py
--rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/normal_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/smiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21142 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/generate/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.208019 wfl-0.2.5/wfl/select/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/select/by_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/select/convex_hull.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/select/flat_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/select/selection_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/select/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.212019 wfl-0.2.5/wfl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/at_copy_save_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/convex_hull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/find_voids.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/gap_xml_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/julia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/ndim_neighbor_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/quip_cli_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/replace_eval_in_strs.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/round_sig_figs.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-17 17:02:49.000000 wfl-0.2.5/wfl/utils/vol_composition_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:02:53.212019 wfl-0.2.5/wfl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-17 17:02:53.000000 wfl-0.2.5/wfl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-17 17:02:53.000000 wfl-0.2.5/wfl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:02:53.000000 wfl-0.2.5/wfl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-17 17:02:53.000000 wfl-0.2.5/wfl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-17 17:02:53.000000 wfl-0.2.5/wfl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 17:02:53.000000 wfl-0.2.5/wfl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.513652 wfl-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-19 00:19:47.000000 wfl-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23585 2024-05-19 00:19:51.513652 wfl-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-19 00:19:47.000000 wfl-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.481653 wfl-0.2.6/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/cli_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.477652 wfl-0.2.6/deprecated/devtools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.481653 wfl-0.2.6/deprecated/devtools/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8092 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/devtools/scripts/pretty_pca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.477652 wfl-0.2.6/deprecated/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.481653 wfl-0.2.6/deprecated/examples/DFT-calculations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/examples/DFT-calculations/castep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/examples/DFT-calculations/quantum_espresso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/examples/DFT-calculations/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.485653 wfl-0.2.6/deprecated/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/plotting/maxveit_plottools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/plotting/normal_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/plotting/plot_2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/plotting/plot_ef_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/plotting/reactions_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.477652 wfl-0.2.6/deprecated/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.485653 wfl-0.2.6/deprecated/user/reactions/
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/cli_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/cli_reactions_iter_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.485653 wfl-0.2.6/deprecated/user/reactions/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/generate/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/generate/irc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/generate/neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/generate/radicals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/generate/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.485653 wfl-0.2.6/deprecated/user/reactions/reactions_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/reactions_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/reactions_processing/trajectory_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.485653 wfl-0.2.6/deprecated/user/reactions/select/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/select/simple_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/select/weighted_cur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.485653 wfl-0.2.6/deprecated/user/reactions/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-19 00:19:47.000000 wfl-0.2.6/deprecated/user/reactions/tests/test_molecules_radicals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.481653 wfl-0.2.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.485653 wfl-0.2.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-19 00:19:47.000000 wfl-0.2.6/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.481653 wfl-0.2.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.485653 wfl-0.2.6/examples/iterative_gap_fit/
+-rw-r--r--   0 runner    (1001) docker     (127)    14955 2024-05-19 00:19:47.000000 wfl-0.2.6/examples/iterative_gap_fit/batch_gap_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-19 00:19:47.000000 wfl-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 00:19:51.513652 wfl-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.493652 wfl-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_ace_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_atoms_and_dimers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_autoparallelize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_batch_gap_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_buildcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_calc_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_cli_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_configset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_descriptor_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_doc_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_flat_histo_to_nearby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_gap_fitting_multistage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_gap_fitting_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_kspacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_mace_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_minimahopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_ndim_neigh_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_normal_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_outputspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_point_defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17757 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_remote_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_rng_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_select_greedy_fps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_select_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-19 00:19:47.000000 wfl-0.2.6/tests/test_version_str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.493652 wfl-0.2.6/wfl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.497652 wfl-0.2.6/wfl/autoparallelize/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/autoparallelize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/autoparallelize/autoparainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/autoparallelize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/autoparallelize/mpipool_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/autoparallelize/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/autoparallelize/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/autoparallelize/remoteinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/autoparallelize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.501653 wfl-0.2.6/wfl/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/aims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/castep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/committee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/espresso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/mopac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.501653 wfl-0.2.6/wfl/calculators/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/orca/basinhopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/calculators/wfl_fileio_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.501653 wfl-0.2.6/wfl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/cli_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.501653 wfl-0.2.6/wfl/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/commands/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/commands/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/commands/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/commands/select.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5598 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/dft_convergence_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60870 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/cli/gap_rss_iter_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31413 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/configset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/descriptor_heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.501653 wfl-0.2.6/wfl/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/descriptors/quippy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.505653 wfl-0.2.6/wfl/fit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20665 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/ace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21419 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.505653 wfl-0.2.6/wfl/fit/gap/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/gap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/gap/glue_2b.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22213 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/gap/multistage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/gap/relocate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/gap/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/mace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.505653 wfl-0.2.6/wfl/fit/modify_database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/modify_database/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7599 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/modify_database/gap_rss_set_config_sigmas_from_convex_hull.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      777 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/modify_database/scale_orig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/modify_database/simple_factor_nonperiodic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5832 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/fit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.505653 wfl-0.2.6/wfl/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/atoms_and_dimers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/buildcell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.509652 wfl-0.2.6/wfl/generate/md/
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/md/abort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/md/abort_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/minimahopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/normal_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21142 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/generate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.509652 wfl-0.2.6/wfl/select/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/select/by_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/select/convex_hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/select/flat_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/select/selection_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/select/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.513652 wfl-0.2.6/wfl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/at_copy_save_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/convex_hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/find_voids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/gap_xml_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/julia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/ndim_neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/quip_cli_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/replace_eval_in_strs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/round_sig_figs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-19 00:19:47.000000 wfl-0.2.6/wfl/utils/vol_composition_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:19:51.513652 wfl-0.2.6/wfl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23585 2024-05-19 00:19:51.000000 wfl-0.2.6/wfl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-19 00:19:51.000000 wfl-0.2.6/wfl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 00:19:51.000000 wfl-0.2.6/wfl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-19 00:19:51.000000 wfl-0.2.6/wfl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-19 00:19:51.000000 wfl-0.2.6/wfl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 00:19:51.000000 wfl-0.2.6/wfl.egg-info/top_level.txt
```

### Comparing `wfl-0.2.5/PKG-INFO` & `wfl-0.2.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: wfl
-Version: 0.2.5
-Description-Content-Type: text/markdown
-Requires-Dist: click>=7.0
-Requires-Dist: numpy
-Requires-Dist: ase>=3.22.1
-Requires-Dist: pyyaml
-Requires-Dist: spglib
-Requires-Dist: docstring_parser
-Requires-Dist: expyre-wfl
-Requires-Dist: universalSOAP
-
 <img src="docs/wf_logo_final.png" width=200>
 
 # Overview
 
 Workflow is a Python toolkit for building interatomic potential creation and atomistic simulation workflows. 
 
 The main functions of Workflow is to efficiently parallelise operations over a set of atomic configurations (Atomic Simulation Environment's "Atoms" objects). Given an operation that is defined to act on a single configuration (e.g. evaluate energy of a structure with CASTEP ASE calculator), Workflow may apply the operation to multiple configurations in parallel. Workflow also interfaces with [ExPyRe](https://github.com/libAtoms/ExPyRe/tree/main/expyre) to manage evaluation of (autoparallelized) Python functions via a queueing system on a (remote) cluster.
```

### Comparing `wfl-0.2.5/tests/test_ace_fitting.py` & `wfl-0.2.6/tests/test_ace_fitting.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_atoms_and_dimers.py` & `wfl-0.2.6/tests/test_atoms_and_dimers.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_autoparallelize.py` & `wfl-0.2.6/tests/test_autoparallelize.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_batch_gap_fit.py` & `wfl-0.2.6/tests/test_batch_gap_fit.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_buildcell.py` & `wfl-0.2.6/tests/test_buildcell.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_calc_descriptor.py` & `wfl-0.2.6/tests/test_calc_descriptor.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_cli_rss.py` & `wfl-0.2.6/tests/test_cli_rss.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_configset.py` & `wfl-0.2.6/tests/test_configset.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_descriptor_heuristics.py` & `wfl-0.2.6/tests/test_descriptor_heuristics.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_doc_examples.py` & `wfl-0.2.6/tests/test_doc_examples.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_error.py` & `wfl-0.2.6/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_flat_histo_to_nearby.py` & `wfl-0.2.6/tests/test_flat_histo_to_nearby.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_gap_fitting_multistage.py` & `wfl-0.2.6/tests/test_gap_fitting_multistage.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_gap_fitting_simple.py` & `wfl-0.2.6/tests/test_gap_fitting_simple.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_kspacing.py` & `wfl-0.2.6/tests/test_kspacing.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_mace_fitting.py` & `wfl-0.2.6/tests/test_mace_fitting.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_map.py` & `wfl-0.2.6/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_md.py` & `wfl-0.2.6/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_minimahopping.py` & `wfl-0.2.6/tests/test_minimahopping.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_molecules.py` & `wfl-0.2.6/tests/test_molecules.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_ndim_neigh_list.py` & `wfl-0.2.6/tests/test_ndim_neigh_list.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_neb.py` & `wfl-0.2.6/tests/test_neb.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_normal_modes.py` & `wfl-0.2.6/tests/test_normal_modes.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_optimize.py` & `wfl-0.2.6/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_outputspec.py` & `wfl-0.2.6/tests/test_outputspec.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_phonopy.py` & `wfl-0.2.6/tests/test_phonopy.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_point_defects.py` & `wfl-0.2.6/tests/test_point_defects.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_remote_run.py` & `wfl-0.2.6/tests/test_remote_run.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_rng_determinism.py` & `wfl-0.2.6/tests/test_rng_determinism.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_select_greedy_fps.py` & `wfl-0.2.6/tests/test_select_greedy_fps.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/tests/test_select_simple.py` & `wfl-0.2.6/tests/test_select_simple.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/autoparallelize/autoparainfo.py` & `wfl-0.2.6/wfl/autoparallelize/autoparainfo.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/autoparallelize/base.py` & `wfl-0.2.6/wfl/autoparallelize/base.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/autoparallelize/mpipool_support.py` & `wfl-0.2.6/wfl/autoparallelize/mpipool_support.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/autoparallelize/pool.py` & `wfl-0.2.6/wfl/autoparallelize/pool.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/autoparallelize/remote.py` & `wfl-0.2.6/wfl/autoparallelize/remote.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/autoparallelize/remoteinfo.py` & `wfl-0.2.6/wfl/autoparallelize/remoteinfo.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/autoparallelize/utils.py` & `wfl-0.2.6/wfl/autoparallelize/utils.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/aims.py` & `wfl-0.2.6/wfl/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/castep.py` & `wfl-0.2.6/wfl/calculators/castep.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/committee.py` & `wfl-0.2.6/wfl/calculators/committee.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/espresso.py` & `wfl-0.2.6/wfl/calculators/espresso.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/generic.py` & `wfl-0.2.6/wfl/calculators/generic.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/kpts.py` & `wfl-0.2.6/wfl/calculators/kpts.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/mopac.py` & `wfl-0.2.6/wfl/calculators/mopac.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/orca/__init__.py` & `wfl-0.2.6/wfl/calculators/orca/__init__.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/orca/basinhopping.py` & `wfl-0.2.6/wfl/calculators/orca/basinhopping.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/utils.py` & `wfl-0.2.6/wfl/calculators/utils.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/vasp.py` & `wfl-0.2.6/wfl/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/calculators/wfl_fileio_calculator.py` & `wfl-0.2.6/wfl/calculators/wfl_fileio_calculator.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/cli/cli.py` & `wfl-0.2.6/wfl/cli/cli.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/cli/cli_options.py` & `wfl-0.2.6/wfl/cli/cli_options.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/cli/commands/descriptor.py` & `wfl-0.2.6/wfl/cli/commands/descriptor.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/cli/commands/error.py` & `wfl-0.2.6/wfl/cli/commands/error.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/cli/commands/eval.py` & `wfl-0.2.6/wfl/cli/commands/eval.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/cli/commands/generate.py` & `wfl-0.2.6/wfl/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/cli/commands/select.py` & `wfl-0.2.6/wfl/cli/commands/select.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/cli/dft_convergence_test.py` & `wfl-0.2.6/wfl/cli/dft_convergence_test.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/cli/gap_rss_iter_fit.py` & `wfl-0.2.6/wfl/cli/gap_rss_iter_fit.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/configset.py` & `wfl-0.2.6/wfl/configset.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/descriptor_heuristics.py` & `wfl-0.2.6/wfl/descriptor_heuristics.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/descriptors/quippy.py` & `wfl-0.2.6/wfl/descriptors/quippy.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/ace.py` & `wfl-0.2.6/wfl/fit/ace.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/error.py` & `wfl-0.2.6/wfl/fit/error.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/gap/glue_2b.py` & `wfl-0.2.6/wfl/fit/gap/glue_2b.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/gap/multistage.py` & `wfl-0.2.6/wfl/fit/gap/multistage.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/gap/relocate.py` & `wfl-0.2.6/wfl/fit/gap/relocate.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/gap/simple.py` & `wfl-0.2.6/wfl/fit/gap/simple.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/mace.py` & `wfl-0.2.6/wfl/fit/mace.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/modify_database/gap_rss_set_config_sigmas_from_convex_hull.py` & `wfl-0.2.6/wfl/fit/modify_database/gap_rss_set_config_sigmas_from_convex_hull.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/modify_database/scale_orig.py` & `wfl-0.2.6/wfl/fit/modify_database/scale_orig.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/modify_database/simple_factor_nonperiodic.py` & `wfl-0.2.6/wfl/fit/modify_database/simple_factor_nonperiodic.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/fit/utils.py` & `wfl-0.2.6/wfl/fit/utils.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/atoms_and_dimers.py` & `wfl-0.2.6/wfl/generate/atoms_and_dimers.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/buildcell.py` & `wfl-0.2.6/wfl/generate/buildcell.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/md/__init__.py` & `wfl-0.2.6/wfl/generate/md/__init__.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/md/abort.py` & `wfl-0.2.6/wfl/generate/md/abort.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/md/abort_base.py` & `wfl-0.2.6/wfl/generate/md/abort_base.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/minimahopping.py` & `wfl-0.2.6/wfl/generate/minimahopping.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/neb.py` & `wfl-0.2.6/wfl/generate/neb.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/normal_modes.py` & `wfl-0.2.6/wfl/generate/normal_modes.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/optimize.py` & `wfl-0.2.6/wfl/generate/optimize.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/phonopy.py` & `wfl-0.2.6/wfl/generate/phonopy.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/smiles.py` & `wfl-0.2.6/wfl/generate/smiles.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/generate/supercells.py` & `wfl-0.2.6/wfl/generate/supercells.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/map.py` & `wfl-0.2.6/wfl/map.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/select/by_descriptor.py` & `wfl-0.2.6/wfl/select/by_descriptor.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/select/convex_hull.py` & `wfl-0.2.6/wfl/select/convex_hull.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/select/flat_histogram.py` & `wfl-0.2.6/wfl/select/flat_histogram.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/select/selection_space.py` & `wfl-0.2.6/wfl/select/selection_space.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/select/simple.py` & `wfl-0.2.6/wfl/select/simple.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/configs.py` & `wfl-0.2.6/wfl/utils/configs.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/convex_hull.py` & `wfl-0.2.6/wfl/utils/convex_hull.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/file_utils.py` & `wfl-0.2.6/wfl/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/find_voids.py` & `wfl-0.2.6/wfl/utils/find_voids.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/gap_xml_tools.py` & `wfl-0.2.6/wfl/utils/gap_xml_tools.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/logging.py` & `wfl-0.2.6/wfl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/misc.py` & `wfl-0.2.6/wfl/utils/misc.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/ndim_neighbor_list.py` & `wfl-0.2.6/wfl/utils/ndim_neighbor_list.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/parallel.py` & `wfl-0.2.6/wfl/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/params.py` & `wfl-0.2.6/wfl/utils/params.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/pressure.py` & `wfl-0.2.6/wfl/utils/pressure.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/quip_cli_strings.py` & `wfl-0.2.6/wfl/utils/quip_cli_strings.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/replace_eval_in_strs.py` & `wfl-0.2.6/wfl/utils/replace_eval_in_strs.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/round_sig_figs.py` & `wfl-0.2.6/wfl/utils/round_sig_figs.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/version.py` & `wfl-0.2.6/wfl/utils/version.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.5/wfl/utils/vol_composition_space.py` & `wfl-0.2.6/wfl/utils/vol_composition_space.py`

 * *Files identical despite different names*

