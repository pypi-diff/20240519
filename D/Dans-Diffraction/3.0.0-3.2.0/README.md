# Comparing `tmp/Dans_Diffraction-3.0.0.tar.gz` & `tmp/Dans_Diffraction-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Dans_Diffraction-3.0.0.tar", last modified: Sun Jul  2 16:47:16 2023, max compression
+gzip compressed data, was "Dans_Diffraction-3.2.0.tar", last modified: Sun May 19 07:09:06 2024, max compression
```

## Comparing `Dans_Diffraction-3.0.0.tar` & `Dans_Diffraction-3.2.0.tar`

### file list

```diff
@@ -1,130 +1,133 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:16.000000 Dans_Diffraction-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:15.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:15.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/
--rw-rw-rw-   0        0        0     4217 2016-08-03 08:31:31.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Aluminium.cif
--rw-rw-rw-   0        0        0     2503 2017-07-31 08:37:44.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/BCC.cif
--rw-rw-rw-   0        0        0     1188 2015-08-03 13:46:33.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Beryllium.cif
--rw-rw-rw-   0        0        0     2250 2018-03-01 19:54:35.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Ca2RuO4.cif
--rw-rw-rw-   0        0        0     3878 2016-11-10 08:23:42.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Ca3CoMnO6.mcif
--rw-rw-rw-   0        0        0     1226 2017-07-31 09:00:59.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Cobalt.cif
--rw-rw-rw-   0        0        0     4214 2015-08-03 13:23:49.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Copper.cif
--rw-rw-rw-   0        0        0     1671 2016-09-15 10:40:04.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Cubic.cif
--rw-rw-rw-   0        0        0     4714 2016-12-06 14:03:28.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Diamond.cif
--rw-rw-rw-   0        0        0     4214 2015-08-03 13:23:49.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/FCC.cif
--rw-rw-rw-   0        0        0     4212 2018-02-14 08:14:18.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Gold.cif
--rw-rw-rw-   0        0        0     2243 2017-04-12 13:11:25.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Graphite.cif
--rw-rw-rw-   0        0        0     1226 2017-07-31 09:00:59.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/HCP.cif
--rw-rw-rw-   0        0        0     2503 2017-07-31 08:37:44.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Iron.cif
--rw-rw-rw-   0        0        0     4325 2017-07-09 15:12:00.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/KCl.cif
--rw-rw-rw-   0        0        0     3082 2020-04-17 07:58:01.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/LaMnO3.mcif
--rw-rw-rw-   0        0        0     1987 2016-05-31 12:37:29.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/LiCoO2.cif
--rw-rw-rw-   0        0        0     2067 2015-05-15 09:42:35.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Na0.8CoO2_P63mmc.cif
--rw-rw-rw-   0        0        0    17159 2023-05-08 11:29:37.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/NaCoO2_stripe_supercell.cif
--rw-rw-rw-   0        0        0     2507 2016-08-03 08:28:38.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Niobium.cif
--rw-rw-rw-   0        0        0     1901 2016-12-06 14:29:29.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Ruby.cif
--rw-rw-rw-   0        0        0     1191 2016-03-07 11:53:11.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Ruthenium.cif
--rw-rw-rw-   0        0        0     1927 2019-05-03 14:32:02.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Sapphire.cif
--rw-rw-rw-   0        0        0     4739 2015-08-04 14:43:40.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Silicon.cif
--rw-rw-rw-   0        0        0     4315 2017-09-05 12:52:37.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Silver.cif
--rw-rw-rw-   0        0        0    83448 2020-03-26 10:12:50.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Sr3LiRuO6.cif
--rw-rw-rw-   0        0        0     4568 2020-02-24 07:33:16.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Sr3LiRuO6_C2'c'.mcif
--rw-rw-rw-   0        0        0     2532 2019-04-03 13:35:10.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Vanadium.cif
--rw-rw-rw-   0        0        0     2468 2020-02-17 08:59:33.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/ZnO.cif
--rw-rw-rw-   0        0        0     7917 2023-07-02 13:33:07.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-04-26 10:54:53.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/__main__.py
--rw-rw-rw-   0        0        0    92544 2023-06-29 05:23:06.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/classes_crystal.py
--rw-rw-rw-   0        0        0    52076 2021-12-15 15:33:14.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/classes_fdmnes.py
--rw-rw-rw-   0        0        0     9899 2022-07-23 11:12:54.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/classes_multicrystal.py
--rw-rw-rw-   0        0        0    17089 2020-10-19 07:41:46.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/classes_orbitals.py
--rw-rw-rw-   0        0        0    10482 2023-01-06 13:55:56.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/classes_orientation.py
--rw-rw-rw-   0        0        0    84117 2023-07-02 14:53:03.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/classes_plotting.py
--rw-rw-rw-   0        0        0    26560 2023-05-18 07:40:06.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/classes_properties.py
--rw-rw-rw-   0        0        0   125734 2023-07-02 14:56:25.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/classes_scattering.py
--rw-rw-rw-   0        0        0     2203 2019-08-07 06:59:10.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/classes_structures.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:15.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/
--rw-rw-rw-   0        0        0    54010 2020-05-02 16:39:54.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/Dans Element Properties.txt
--rw-rw-rw-   0        0        0    43658 2019-12-13 07:38:09.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/Dans Element Properties_old.txt
--rw-rw-rw-   0        0        0     4719 2019-07-31 18:31:45.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/Element_OxidationStates.txt
--rw-rw-rw-   0        0        0    58645 2021-03-31 11:01:14.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/PointGroups.json
--rw-rw-rw-   0        0        0   997216 2020-04-22 21:04:44.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/SpaceGroups.json
--rw-rw-rw-   0        0        0  8319520 2020-05-26 14:42:44.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/SpaceGroupsMagnetic.json
--rw-rw-rw-   0        0        0    30113 2016-12-01 11:30:15.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/XRayEdges.dat
--rw-rw-rw-   0        0        0  2779670 2020-05-06 09:22:05.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/XRayMassAtten_muenp.dat
--rw-rw-rw-   0        0        0  2779670 2020-05-06 09:22:05.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/XRayMassAtten_mup.dat
--rw-rw-rw-   0        0        0  1317778 2021-01-21 09:28:34.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/atomic_scattering_factors.npy
--rw-rw-rw-   0        0        0    43385 2021-06-08 07:44:54.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/f0_WaasKirf.dat
--rw-rw-rw-   0        0        0    25892 2023-05-06 11:12:54.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/data/peng.dat
--rw-rw-rw-   0        0        0   137036 2023-07-02 13:21:23.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/functions_crystallography.py
--rw-rw-rw-   0        0        0    42603 2023-06-02 05:14:41.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/functions_general.py
--rw-rw-rw-   0        0        0    33113 2023-05-16 17:25:23.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/functions_plotting.py
--rw-rw-rw-   0        0        0    44417 2023-05-07 14:24:07.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/functions_scattering.py
--rw-rw-rw-   0        0        0    27095 2020-10-15 13:27:33.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/multiple_scattering.py
--rw-rw-rw-   0        0        0   192479 2023-01-06 14:04:42.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tensor_scattering.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:15.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/
--rw-rw-rw-   0        0        0     1256 2023-06-28 07:12:14.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/__init__.py
--rw-rw-rw-   0        0        0    12198 2023-05-24 05:32:43.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/basic_widgets.py
--rw-rw-rw-   0        0        0    15559 2023-06-28 10:25:11.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/converter.py
--rw-rw-rw-   0        0        0    49324 2023-06-28 07:31:38.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/crystal.py
--rw-rw-rw-   0        0        0    64567 2023-06-29 05:23:06.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/diffractometer.py
--rw-rw-rw-   0        0        0    22733 2023-05-16 05:57:15.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/fdmnes.py
--rw-rw-rw-   0        0        0    10161 2022-07-23 11:12:54.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/multi_crystal.py
--rw-rw-rw-   0        0        0     7170 2019-12-16 07:45:56.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/multiple_scattering.py
--rw-rw-rw-   0        0        0    10826 2023-05-16 16:30:28.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/periodic_table.py
--rw-rw-rw-   0        0        0    30256 2023-05-18 07:33:36.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/properties.py
--rw-rw-rw-   0        0        0    69222 2023-06-25 15:23:07.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/scattering.py
--rw-rw-rw-   0        0        0    14775 2023-05-22 06:11:38.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/spacegroups.py
--rw-rw-rw-   0        0        0    13686 2020-02-20 13:50:35.000000 Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/tensor_scattering.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:15.000000 Dans_Diffraction-3.0.0/Dans_Diffraction.egg-info/
--rw-rw-rw-   0        0        0    16912 2023-07-02 16:47:14.000000 Dans_Diffraction-3.0.0/Dans_Diffraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4313 2023-07-02 16:47:14.000000 Dans_Diffraction-3.0.0/Dans_Diffraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 16:47:14.000000 Dans_Diffraction-3.0.0/Dans_Diffraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-02 16:47:14.000000 Dans_Diffraction-3.0.0/Dans_Diffraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-02 16:47:14.000000 Dans_Diffraction-3.0.0/Dans_Diffraction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16912 2023-07-02 16:47:16.000000 Dans_Diffraction-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    13629 2023-07-02 13:42:25.000000 Dans_Diffraction-3.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-02 16:47:16.000000 Dans_Diffraction-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1254 2023-06-25 15:48:08.000000 Dans_Diffraction-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:16.000000 Dans_Diffraction-3.0.0/test/
--rw-rw-rw-   0        0        0     2282 2018-02-13 15:38:28.000000 Dans_Diffraction-3.0.0/test/test_LS_magnetic_components.py
--rw-rw-rw-   0        0        0     8939 2021-06-10 16:58:04.000000 Dans_Diffraction-3.0.0/test/test_WaasKirf_xray_factors.py
--rw-rw-rw-   0        0        0     2197 2020-04-30 13:31:49.000000 Dans_Diffraction-3.0.0/test/test_atom_properties.py
--rw-rw-rw-   0        0        0     1170 2020-05-06 08:27:47.000000 Dans_Diffraction-3.0.0/test/test_attenuation.py
--rw-rw-rw-   0        0        0     1910 2021-01-25 17:53:20.000000 Dans_Diffraction-3.0.0/test/test_attenuation_length.py
--rw-rw-rw-   0        0        0     2002 2020-11-12 13:20:39.000000 Dans_Diffraction-3.0.0/test/test_bmatrix.py
--rw-rw-rw-   0        0        0     1562 2020-10-19 07:41:46.000000 Dans_Diffraction-3.0.0/test/test_cif_files.py
--rw-rw-rw-   0        0        0     6312 2021-07-19 15:51:46.000000 Dans_Diffraction-3.0.0/test/test_coherent_diffraction.py
--rw-rw-rw-   0        0        0     3230 2021-07-17 05:26:09.000000 Dans_Diffraction-3.0.0/test/test_coherent_diffraction2.py
--rw-rw-rw-   0        0        0     1859 2019-12-12 20:20:59.000000 Dans_Diffraction-3.0.0/test/test_compare_intensity.py
--rw-rw-rw-   0        0        0     8480 2020-10-26 14:50:52.000000 Dans_Diffraction-3.0.0/test/test_compare_intensity_calculation.py
--rw-rw-rw-   0        0        0     4552 2020-05-12 07:18:31.000000 Dans_Diffraction-3.0.0/test/test_compound_name.py
--rw-rw-rw-   0        0        0     2740 2022-03-11 16:54:13.000000 Dans_Diffraction-3.0.0/test/test_convolve2d.py
--rw-rw-rw-   0        0        0      289 2020-10-20 19:46:18.000000 Dans_Diffraction-3.0.0/test/test_detector.py
--rw-rw-rw-   0        0        0     2902 2020-05-15 15:03:16.000000 Dans_Diffraction-3.0.0/test/test_electron_density.py
--rw-rw-rw-   0        0        0     5008 2020-10-19 07:41:46.000000 Dans_Diffraction-3.0.0/test/test_exchange_path.py
--rw-rw-rw-   0        0        0     4144 2020-10-19 07:41:46.000000 Dans_Diffraction-3.0.0/test/test_exchange_path2.py
--rw-rw-rw-   0        0        0      149 2018-06-08 14:18:49.000000 Dans_Diffraction-3.0.0/test/test_files.py
--rw-rw-rw-   0        0        0     5627 2021-07-15 05:41:12.000000 Dans_Diffraction-3.0.0/test/test_functions_scattering.py
--rw-rw-rw-   0        0        0     1152 2021-07-15 16:03:30.000000 Dans_Diffraction-3.0.0/test/test_functions_scattering_dispersion.py
--rw-rw-rw-   0        0        0     3320 2021-07-14 17:11:38.000000 Dans_Diffraction-3.0.0/test/test_functions_scattering_new.py
--rw-rw-rw-   0        0        0     4726 2021-07-13 13:13:30.000000 Dans_Diffraction-3.0.0/test/test_functions_scattering_pol.py
--rw-rw-rw-   0        0        0     3102 2021-07-13 14:17:38.000000 Dans_Diffraction-3.0.0/test/test_functions_scattering_xrm.py
--rw-rw-rw-   0        0        0     1691 2020-03-27 07:59:19.000000 Dans_Diffraction-3.0.0/test/test_gaussian.py
--rw-rw-rw-   0        0        0    17556 2020-06-09 08:44:11.000000 Dans_Diffraction-3.0.0/test/test_gen_sym_mat.py
--rw-rw-rw-   0        0        0      256 2020-03-31 13:19:32.000000 Dans_Diffraction-3.0.0/test/test_gui_multicrystal.py
--rw-rw-rw-   0        0        0     3193 2020-11-22 19:46:51.000000 Dans_Diffraction-3.0.0/test/test_i16_azimuth.py
--rw-rw-rw-   0        0        0      552 2020-03-27 16:10:17.000000 Dans_Diffraction-3.0.0/test/test_intensity_grid.py
--rw-rw-rw-   0        0        0     1196 2020-03-27 08:15:40.000000 Dans_Diffraction-3.0.0/test/test_isincell.py
--rw-rw-rw-   0        0        0     2536 2021-10-04 20:22:07.000000 Dans_Diffraction-3.0.0/test/test_laue_backscatter.py
--rw-rw-rw-   0        0        0     3864 2019-02-22 16:52:35.000000 Dans_Diffraction-3.0.0/test/test_nonresonant.py
--rw-rw-rw-   0        0        0     5702 2019-01-21 13:30:00.000000 Dans_Diffraction-3.0.0/test/test_nonresonant_plot.py
--rw-rw-rw-   0        0        0     3092 2019-01-21 13:25:46.000000 Dans_Diffraction-3.0.0/test/test_nonresonant_sergio.py
--rw-rw-rw-   0        0        0      453 2021-09-26 16:50:06.000000 Dans_Diffraction-3.0.0/test/test_orientation.py
--rw-rw-rw-   0        0        0     1044 2017-11-26 15:52:58.000000 Dans_Diffraction-3.0.0/test/test_parameter_plot.py
--rw-rw-rw-   0        0        0     4428 2020-11-22 20:40:03.000000 Dans_Diffraction-3.0.0/test/test_plot_orbitals.py
--rw-rw-rw-   0        0        0     1956 2017-08-22 12:09:50.000000 Dans_Diffraction-3.0.0/test/test_plotintensity.py
--rw-rw-rw-   0        0        0     2890 2017-08-22 15:29:48.000000 Dans_Diffraction-3.0.0/test/test_plotintensity2.py
--rw-rw-rw-   0        0        0     2593 2020-05-05 08:27:58.000000 Dans_Diffraction-3.0.0/test/test_readstfm.py
--rw-rw-rw-   0        0        0      988 2021-01-26 07:46:04.000000 Dans_Diffraction-3.0.0/test/test_refractive_index.py
--rw-rw-rw-   0        0        0     1843 2017-10-30 14:29:08.000000 Dans_Diffraction-3.0.0/test/test_scattering.py
--rw-rw-rw-   0        0        0     2649 2017-11-09 11:24:34.000000 Dans_Diffraction-3.0.0/test/test_supercell.py
--rw-rw-rw-   0        0        0     9400 2020-06-09 13:06:44.000000 Dans_Diffraction-3.0.0/test/test_symmetry_ops2magnetic.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.573392 Dans_Diffraction-3.2.0/
+drwxrwxrwx   0        0        0        0 2024-05-19 07:09:05.976489 Dans_Diffraction-3.2.0/Dans_Diffraction/
+drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.111949 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/
+-rw-rw-rw-   0        0        0     4217 2016-08-03 08:31:31.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Aluminium.cif
+-rw-rw-rw-   0        0        0     2503 2017-07-31 08:37:44.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/BCC.cif
+-rw-rw-rw-   0        0        0     1188 2015-08-03 13:46:33.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Beryllium.cif
+-rw-rw-rw-   0        0        0     2250 2018-03-01 19:54:35.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ca2RuO4.cif
+-rw-rw-rw-   0        0        0     3878 2016-11-10 08:23:42.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ca3CoMnO6.mcif
+-rw-rw-rw-   0        0        0     1226 2017-07-31 09:00:59.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Cobalt.cif
+-rw-rw-rw-   0        0        0     4214 2015-08-03 13:23:49.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Copper.cif
+-rw-rw-rw-   0        0        0     1671 2016-09-15 10:40:04.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Cubic.cif
+-rw-rw-rw-   0        0        0     4714 2016-12-06 14:03:28.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Diamond.cif
+-rw-rw-rw-   0        0        0     4214 2015-08-03 13:23:49.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/FCC.cif
+-rw-rw-rw-   0        0        0     4212 2018-02-14 08:14:18.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Gold.cif
+-rw-rw-rw-   0        0        0     2243 2017-04-12 13:11:25.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Graphite.cif
+-rw-rw-rw-   0        0        0     1226 2017-07-31 09:00:59.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/HCP.cif
+-rw-rw-rw-   0        0        0     2503 2017-07-31 08:37:44.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Iron.cif
+-rw-rw-rw-   0        0        0     4325 2017-07-09 15:12:00.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/KCl.cif
+-rw-rw-rw-   0        0        0     3082 2020-04-17 07:58:01.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/LaMnO3.mcif
+-rw-rw-rw-   0        0        0     1987 2016-05-31 12:37:29.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/LiCoO2.cif
+-rw-rw-rw-   0        0        0     2067 2015-05-15 09:42:35.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Na0.8CoO2_P63mmc.cif
+-rw-rw-rw-   0        0        0    17159 2023-05-08 11:29:37.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/NaCoO2_stripe_supercell.cif
+-rw-rw-rw-   0        0        0     2507 2016-08-03 08:28:38.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Niobium.cif
+-rw-rw-rw-   0        0        0     1901 2016-12-06 14:29:29.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ruby.cif
+-rw-rw-rw-   0        0        0     1191 2016-03-07 11:53:11.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ruthenium.cif
+-rw-rw-rw-   0        0        0     1927 2019-05-03 14:32:02.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sapphire.cif
+-rw-rw-rw-   0        0        0     4739 2015-08-04 14:43:40.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Silicon.cif
+-rw-rw-rw-   0        0        0     4315 2017-09-05 12:52:37.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Silver.cif
+-rw-rw-rw-   0        0        0    83448 2020-03-26 10:12:50.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sr3LiRuO6.cif
+-rw-rw-rw-   0        0        0     4568 2020-02-24 07:33:16.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sr3LiRuO6_C2'c'.mcif
+-rw-rw-rw-   0        0        0     2532 2019-04-03 13:35:10.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Vanadium.cif
+-rw-rw-rw-   0        0        0     2468 2020-02-17 08:59:33.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/ZnO.cif
+-rw-rw-rw-   0        0        0     9450 2024-05-19 06:53:14.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-04-26 10:54:53.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/__main__.py
+-rw-rw-rw-   0        0        0    92680 2024-05-02 07:03:04.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_crystal.py
+-rw-rw-rw-   0        0        0    51728 2024-05-02 07:03:04.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_fdmnes.py
+-rw-rw-rw-   0        0        0     9899 2022-07-23 11:12:54.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_multicrystal.py
+-rw-rw-rw-   0        0        0    19043 2023-07-16 14:24:15.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_orbitals.py
+-rw-rw-rw-   0        0        0    10482 2023-01-06 13:55:56.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_orientation.py
+-rw-rw-rw-   0        0        0    93613 2024-05-19 06:53:14.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_plotting.py
+-rw-rw-rw-   0        0        0    37527 2024-03-28 13:31:10.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_properties.py
+-rw-rw-rw-   0        0        0   139952 2024-05-19 06:32:45.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_scattering.py
+-rw-rw-rw-   0        0        0     2867 2023-08-18 10:11:48.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_structures.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.220819 Dans_Diffraction-3.2.0/Dans_Diffraction/data/
+-rw-rw-rw-   0        0        0    54010 2020-05-02 16:39:54.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/Dans Element Properties.txt
+-rw-rw-rw-   0        0        0    43658 2019-12-13 07:38:09.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/Dans Element Properties_old.txt
+-rw-rw-rw-   0        0        0     4719 2019-07-31 18:31:45.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/Element_OxidationStates.txt
+-rw-rw-rw-   0        0        0    58645 2021-03-31 11:01:14.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/PointGroups.json
+-rw-rw-rw-   0        0        0   997216 2020-04-22 21:04:44.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/SpaceGroups.json
+-rw-rw-rw-   0        0        0  8319520 2020-05-26 14:42:44.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/SpaceGroupsMagnetic.json
+-rw-rw-rw-   0        0        0    30113 2016-12-01 11:30:15.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayEdges.dat
+-rw-rw-rw-   0        0        0  2779670 2020-05-06 09:22:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayMassAtten_muenp.dat
+-rw-rw-rw-   0        0        0  2779670 2020-05-06 09:22:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayMassAtten_mup.dat
+-rw-rw-rw-   0        0        0  1317778 2021-01-21 09:28:34.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/atomic_scattering_factors.npy
+-rw-rw-rw-   0        0        0    43385 2021-06-08 07:44:54.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/f0_WaasKirf.dat
+-rw-rw-rw-   0        0        0    25892 2023-05-06 11:12:54.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/peng.dat
+-rw-rw-rw-   0        0        0   152719 2024-05-18 09:47:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/functions_crystallography.py
+-rw-rw-rw-   0        0        0    47409 2024-05-15 19:15:56.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/functions_general.py
+-rw-rw-rw-   0        0        0    34608 2024-05-19 06:39:03.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/functions_plotting.py
+-rw-rw-rw-   0        0        0    44417 2023-05-07 14:24:07.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/functions_scattering.py
+-rw-rw-rw-   0        0        0    27095 2020-10-15 13:27:33.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/multiple_scattering.py
+-rw-rw-rw-   0        0        0   192479 2023-01-06 14:04:42.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tensor_scattering.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.266292 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/
+-rw-rw-rw-   0        0        0     1570 2024-03-28 13:17:42.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/__init__.py
+-rw-rw-rw-   0        0        0    14834 2023-07-16 12:26:55.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/basic_widgets.py
+-rw-rw-rw-   0        0        0    16665 2023-10-19 11:03:24.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/converter.py
+-rw-rw-rw-   0        0        0    50929 2024-03-28 16:28:00.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/crystal.py
+-rw-rw-rw-   0        0        0    73139 2023-10-19 09:23:59.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/diffractometer.py
+-rw-rw-rw-   0        0        0    26672 2023-07-20 05:54:00.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/fdmnes.py
+-rw-rw-rw-   0        0        0     9934 2024-03-28 15:58:36.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/multi_crystal.py
+-rw-rw-rw-   0        0        0     7072 2023-07-14 09:21:27.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/multiple_scattering.py
+-rw-rw-rw-   0        0        0    10826 2023-05-16 16:30:28.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/periodic_table.py
+-rw-rw-rw-   0        0        0    30256 2023-08-14 07:29:38.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/properties.py
+-rw-rw-rw-   0        0        0    94783 2024-05-18 09:36:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/scattering.py
+-rw-rw-rw-   0        0        0    14775 2023-05-22 06:11:38.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/spacegroups.py
+-rw-rw-rw-   0        0        0    13686 2020-02-20 13:50:35.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/tensor_scattering.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:09:05.999499 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/
+-rw-rw-rw-   0        0        0    14849 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4390 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2020-04-19 15:46:17.000000 Dans_Diffraction-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0    14849 2024-05-19 07:09:06.570107 Dans_Diffraction-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14048 2024-05-17 08:01:40.000000 Dans_Diffraction-3.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 07:09:06.573892 Dans_Diffraction-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2024-05-19 06:53:14.000000 Dans_Diffraction-3.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.567029 Dans_Diffraction-3.2.0/test/
+-rw-rw-rw-   0        0        0     2282 2018-02-13 15:38:28.000000 Dans_Diffraction-3.2.0/test/test_LS_magnetic_components.py
+-rw-rw-rw-   0        0        0     8939 2021-06-10 16:58:04.000000 Dans_Diffraction-3.2.0/test/test_WaasKirf_xray_factors.py
+-rw-rw-rw-   0        0        0     2197 2020-04-30 13:31:49.000000 Dans_Diffraction-3.2.0/test/test_atom_properties.py
+-rw-rw-rw-   0        0        0     1170 2020-05-06 08:27:47.000000 Dans_Diffraction-3.2.0/test/test_attenuation.py
+-rw-rw-rw-   0        0        0     1910 2021-01-25 17:53:20.000000 Dans_Diffraction-3.2.0/test/test_attenuation_length.py
+-rw-rw-rw-   0        0        0     2002 2020-11-12 13:20:39.000000 Dans_Diffraction-3.2.0/test/test_bmatrix.py
+-rw-rw-rw-   0        0        0     1704 2023-08-16 11:18:50.000000 Dans_Diffraction-3.2.0/test/test_check_append_vs_unique.py
+-rw-rw-rw-   0        0        0     1562 2020-10-19 07:41:46.000000 Dans_Diffraction-3.2.0/test/test_cif_files.py
+-rw-rw-rw-   0        0        0     6312 2021-07-19 15:51:46.000000 Dans_Diffraction-3.2.0/test/test_coherent_diffraction.py
+-rw-rw-rw-   0        0        0     3230 2021-07-17 05:26:09.000000 Dans_Diffraction-3.2.0/test/test_coherent_diffraction2.py
+-rw-rw-rw-   0        0        0     1859 2019-12-12 20:20:59.000000 Dans_Diffraction-3.2.0/test/test_compare_intensity.py
+-rw-rw-rw-   0        0        0     8480 2020-10-26 14:50:52.000000 Dans_Diffraction-3.2.0/test/test_compare_intensity_calculation.py
+-rw-rw-rw-   0        0        0     4552 2020-05-12 07:18:31.000000 Dans_Diffraction-3.2.0/test/test_compound_name.py
+-rw-rw-rw-   0        0        0     2740 2022-03-11 16:54:13.000000 Dans_Diffraction-3.2.0/test/test_convolve2d.py
+-rw-rw-rw-   0        0        0      289 2020-10-20 19:46:18.000000 Dans_Diffraction-3.2.0/test/test_detector.py
+-rw-rw-rw-   0        0        0     2902 2020-05-15 15:03:16.000000 Dans_Diffraction-3.2.0/test/test_electron_density.py
+-rw-rw-rw-   0        0        0     5008 2020-10-19 07:41:46.000000 Dans_Diffraction-3.2.0/test/test_exchange_path.py
+-rw-rw-rw-   0        0        0     4144 2020-10-19 07:41:46.000000 Dans_Diffraction-3.2.0/test/test_exchange_path2.py
+-rw-rw-rw-   0        0        0      149 2018-06-08 14:18:49.000000 Dans_Diffraction-3.2.0/test/test_files.py
+-rw-rw-rw-   0        0        0     5627 2021-07-15 05:41:12.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering.py
+-rw-rw-rw-   0        0        0     1152 2021-07-15 16:03:30.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering_dispersion.py
+-rw-rw-rw-   0        0        0     3320 2021-07-14 17:11:38.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering_new.py
+-rw-rw-rw-   0        0        0     4726 2021-07-13 13:13:30.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering_pol.py
+-rw-rw-rw-   0        0        0     3102 2021-07-13 14:17:38.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering_xrm.py
+-rw-rw-rw-   0        0        0     1691 2020-03-27 07:59:19.000000 Dans_Diffraction-3.2.0/test/test_gaussian.py
+-rw-rw-rw-   0        0        0    17556 2020-06-09 08:44:11.000000 Dans_Diffraction-3.2.0/test/test_gen_sym_mat.py
+-rw-rw-rw-   0        0        0      256 2020-03-31 13:19:32.000000 Dans_Diffraction-3.2.0/test/test_gui_multicrystal.py
+-rw-rw-rw-   0        0        0     3193 2020-11-22 19:46:51.000000 Dans_Diffraction-3.2.0/test/test_i16_azimuth.py
+-rw-rw-rw-   0        0        0      552 2020-03-27 16:10:17.000000 Dans_Diffraction-3.2.0/test/test_intensity_grid.py
+-rw-rw-rw-   0        0        0     1196 2020-03-27 08:15:40.000000 Dans_Diffraction-3.2.0/test/test_isincell.py
+-rw-rw-rw-   0        0        0     2536 2021-10-04 20:22:07.000000 Dans_Diffraction-3.2.0/test/test_laue_backscatter.py
+-rw-rw-rw-   0        0        0     3864 2019-02-22 16:52:35.000000 Dans_Diffraction-3.2.0/test/test_nonresonant.py
+-rw-rw-rw-   0        0        0     5702 2019-01-21 13:30:00.000000 Dans_Diffraction-3.2.0/test/test_nonresonant_plot.py
+-rw-rw-rw-   0        0        0     3092 2019-01-21 13:25:46.000000 Dans_Diffraction-3.2.0/test/test_nonresonant_sergio.py
+-rw-rw-rw-   0        0        0      453 2021-09-26 16:50:06.000000 Dans_Diffraction-3.2.0/test/test_orientation.py
+-rw-rw-rw-   0        0        0     1044 2017-11-26 15:52:58.000000 Dans_Diffraction-3.2.0/test/test_parameter_plot.py
+-rw-rw-rw-   0        0        0     4428 2020-11-22 20:40:03.000000 Dans_Diffraction-3.2.0/test/test_plot_orbitals.py
+-rw-rw-rw-   0        0        0     1956 2017-08-22 12:09:50.000000 Dans_Diffraction-3.2.0/test/test_plotintensity.py
+-rw-rw-rw-   0        0        0     2890 2017-08-22 15:29:48.000000 Dans_Diffraction-3.2.0/test/test_plotintensity2.py
+-rw-rw-rw-   0        0        0     2593 2020-05-05 08:27:58.000000 Dans_Diffraction-3.2.0/test/test_readstfm.py
+-rw-rw-rw-   0        0        0      327 2023-07-19 15:10:57.000000 Dans_Diffraction-3.2.0/test/test_reflection_selector.py
+-rw-rw-rw-   0        0        0      988 2021-01-26 07:46:04.000000 Dans_Diffraction-3.2.0/test/test_refractive_index.py
+-rw-rw-rw-   0        0        0     1843 2017-10-30 14:29:08.000000 Dans_Diffraction-3.2.0/test/test_scattering.py
+-rw-rw-rw-   0        0        0     2649 2017-11-09 11:24:34.000000 Dans_Diffraction-3.2.0/test/test_supercell.py
+-rw-rw-rw-   0        0        0     9400 2020-06-09 13:06:44.000000 Dans_Diffraction-3.2.0/test/test_symmetry_ops2magnetic.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Aluminium.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Aluminium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/BCC.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/BCC.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Beryllium.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Beryllium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Ca2RuO4.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ca2RuO4.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Ca3CoMnO6.mcif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ca3CoMnO6.mcif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Cobalt.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Cobalt.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Copper.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Copper.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Cubic.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Cubic.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Diamond.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Diamond.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/FCC.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/FCC.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Gold.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Gold.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Graphite.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Graphite.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/HCP.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/HCP.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Iron.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Iron.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/KCl.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/KCl.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/LaMnO3.mcif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/LaMnO3.mcif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/LiCoO2.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/LiCoO2.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Na0.8CoO2_P63mmc.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Na0.8CoO2_P63mmc.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/NaCoO2_stripe_supercell.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/NaCoO2_stripe_supercell.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Niobium.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Niobium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Ruby.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ruby.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Ruthenium.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ruthenium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Sapphire.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sapphire.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Silicon.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Silicon.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Silver.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Silver.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Sr3LiRuO6.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sr3LiRuO6.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Sr3LiRuO6_C2'c'.mcif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sr3LiRuO6_C2'c'.mcif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/Vanadium.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Vanadium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/Structures/ZnO.cif` & `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/ZnO.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/__init__.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
 Dans_Diffraction
 Python package for loading crystal structures from cif files and calculating diffraction information.
 
 Installation:
-$ pip install Dans-Diffraction
+$ python -m pip install Dans-Diffraction
 or
 $ git clone https://github.com/DanPorter/Dans_Diffraction.git
 or
-$ pip install git+https://github.com/DanPorter/Dans_Diffraction.git
+$ python -m pip install git+https://github.com/DanPorter/Dans_Diffraction.git
 
 Requirements:
-Python 2.7+/3+ with packages: Numpy, Matplotlib, Tkinter
+Python 3.5+ with packages: Numpy, Matplotlib, Tkinter
 BuiltIn packages used: sys, os, re, glob, warnings, json, itertools
 
 Usage:
     ***In Python/ script***
     import Dans_Diffraction as dif
     f = '/location/of/file.cif'
     xtl = dif.Crystal(f)
     
 Usage:
     ***From Terminal***
     $ cd /location/of/file
     $ ipython -i -m -matplotlib tk Dans_Diffraction
 
 GitHub Repo: https://github.com/DanPorter/Dans_Diffraction
-Citation DOI: https://doi.org/10.5281/zenodo.3859501
+Citation DOI: https://doi.org/10.5281/zenodo.8106031
 
 By Dan Porter, PhD
 Diamond
 2017
 
-Version 3.0.0
-Last updated: 02/07/23
+Version 3.2.0
+Last updated: 19/05/24
 
 Version History:
 02/03/18 1.0    Version History started.
 30/05/18 1.1    Fdmnes added
 08/06/18 1.2    Python3 now fully supported
 23/02/19 1.3    Graphical user intrface and magnetic x-ray scattering now implemented
 13/07/19 1.4    FDMNES GUI functionality added
@@ -64,14 +64,22 @@
 07/02/22 2.1.2  Corrected error in classes_scattering.powder() of wrong tth values. Thanks Mirko!
 14/03/22 2.2.0  Scatter.powder() updated for new inputs and outputs for pVoight and custom peak shapes. Thanks yevgenyr!
 23/07/22 2.2.1  Fixed error in MultiCrystal.Scatter
 06/01/23 2.2.2  Removed redundent references to np.float
 14/01/23 2.2.3  Corrected background error in xtl.Scatter.powder
 08/05/23 2.3.0  Merged pull request for non-integer hkl option on SF and electron form factors. Thanks Prestipino!
 25/06/23 3.0.0  Added new GUI elements including new Scattering UI and diffractomter simulator, plus other updates
+11/07/23 3.0.1  Some fixes for plotting and additions to diffractometer orientation. Thanks asteppke!
+20/07/23 3.1.0  Refactored FDMNES wrapper with new methods and new defaults. Thanks YvesJoly!
+26/09/23 3.1.1  Minor changes and improvments. Added hkl1, hkl2 = xtl.scatter.orientation_reflections()
+19/10/23 3.1.2  xray_resonant() now works with non-cubic systems, fixed scaling issue in diffractometer.py
+25/10/23 3.1.3  Fixed error with powder plot for Neutrons. Thanks Cyril!
+28/03/24 3.1.4  Fixed error with site symmetries having spaces in AtomsGui, added Properties.relative_positions()
+10/05/24 3.1.5  Fixed SyntaxWarnings from Unrecognized escape sequences in Python 3.12, various fixes to scattering
+15/05/24 3.2.0  Added "save" and "load" methods to structure factor calculation, improved powder for large calculations
 
 Acknoledgements:
     2018        Thanks to Hepesu for help with Python3 support and ideas about breaking up calculations
     Dec 2019    Thanks to Gareth Nisbet for allowing me to inlude his multiple scattering siumulation
     April 2020  Thanks to ChunHai Wang for helpful suggestions in readcif!
     May 2020    Thanks to AndreEbel for helpful suggestions on citations
     Dec 2020    Thanks to Chris Drozdowski for suggestions about reflection families
@@ -79,17 +87,23 @@
     April 2021  Thanks to Trygve Ræder for suggestions about x-ray scattering factors
     Feb 2022    Thanks to Mirko for pointing out the error in two-theta values in Scatter.powder
     March 2022  Thanks to yevgenyr for suggesting new peak profiles in Scatter.powder
     Jan 2023    Thanks to Anuradha Vibhakar for pointing out the error in f0 + if'-if''
     Jan 2023    Thanks to Andreas Rosnes for testing the installation in jupyterlab
     May 2023    Thanks to Carmelo Prestipino for adding electron scattering factors
     June 2023   Thanks to Sergio I. Rincon for pointing out the rounding error in Scatter.powder
+    July 2023   Thanks to asteppke for suggested update to Arrow3D for matplotlib V>3.4
+    July 2023   Thanks to Yves Joly for helpful suggestions on FDMNES wrapper
+    Oct 2023    Thanks to asteppke for pointing out scaling issue in diffractometer gui
+    Oct 2023    Thanks to Cyril Cayron for pointing out the error with plotting neutron power spectra
+    May 2024    Thanks to Innbig for spotting some errors in large liquid crystal powder patterns
+    May 2024    Thanks to paul-cares pointing out a silly spelling error in the title!
 
 -----------------------------------------------------------------------------
-   Copyright 2023 Diamond Light Source Ltd.
+   Copyright 2024 Diamond Light Source Ltd.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
@@ -124,24 +138,20 @@
 # Dans Diffraction
 from . import functions_general as fg
 from . import functions_plotting as fp
 from . import functions_crystallography as fc
 from .classes_crystal import Crystal
 from .classes_multicrystal import MultiCrystal
 from .classes_structures import Structures
+from .classes_fdmnes import fdmnes_checker, Fdmnes, FdmnesAnalysis
 from .functions_crystallography import readcif
 
-# FDMNES
-from .classes_fdmnes import fdmnes_checker
-if fdmnes_checker():
-    from .classes_fdmnes import Fdmnes, FdmnesAnalysis
 
-
-__version__ = '3.0.0'
-__date__ = '02/07/23'
+__version__ = '3.2.0'
+__date__ = '19/05/24'
 
 
 # Build
 structure_list = Structures()
 
 
 def version_info():
@@ -183,12 +193,15 @@
         from .tkgui import CrystalGui
         CrystalGui(xtl)
     except ImportError:
         print('GUI functionality not available, you need to install tkinter.')
 
 
 # FDMNES Activation
-def activate_fdmnes():
-    """To activate FDMNES functionality"""
-    fdmnes_checker(activate=True)
-    if fdmnes_checker():
-        from .classes_fdmnes import Fdmnes, FdmnesAnalysis
+def activate_fdmnes(initial_dir=None, fdmnes_filename='fdmnes_win64.exe'):
+    """
+    Call to activate FDMNES functionality
+    :param fdmnes_filename: name of the executable to search for
+    :param initial_dir: None or str, if directory, look here for file
+    :return: None
+    """
+    fdmnes_checker(activate=True, fdmnes_filename=fdmnes_filename, initial_dir=initial_dir)
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/__main__.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/__main__.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/classes_crystal.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_crystal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1383,14 +1383,19 @@
             elif self.uiso[n] > 0.1:
                 good = False
                 print('Atom %d has uiso greater than 0.1!' % n)
 
         if good:
             print("Atoms look good.")
 
+    def fitincell(self):
+        """Adjust all atom positions to fit within unit cell"""
+        uvw = fc.fitincell(self.uvw())
+
+
     def uvw(self):
         """
         Returns a [nx3] array of current positions
         :return: np.array([nx3])
         """
         return np.asarray([self.u, self.v, self.w], dtype=float).T
 
@@ -2070,15 +2075,15 @@
         return out
 
     def symmetric_magnetic_vectors(self, MXMYMZ):
         """
         NOT COMPLETE
         """
 
-        """
+        r"""
         for n, (mx, my, mz) in enumerate(MXMYMZ):
             # Apply symmetry constraints
             if len(contraints) > 0:
                 C = constraints
                 C = C.replace('m','')
                 #print('Constraint: {:3s} {:s}'.format(label[n],C))
                 # convert '2x' to 'x'
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/classes_fdmnes.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_fdmnes.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,126 +3,158 @@
 FDMNES class "classes_fdmnes.py"
  functions for generating fdmnes files
 
 By Dan Porter, PhD
 Diamond
 2018
 
-Version 1.6
-Last updated: 22/04/20
+Version 2.0
+Last updated: 20/07/23
 
 Version History:
 17/04/18 0.9    Program created
 04/06/18 1.0    Program completed and tested
 11/06/18 1.1    Analysis updated to find density with _sd1 and _sd0
 13/07/19 1.2    Small updates for gui functionality
 07/08/19 1.3    Changed reflist in FdmnesAnalysis to list of hkl
 16/08/19 1.4    Added BavFile to read parts of .bav file
 18/03/20 1.5    Corrected density file for new headers
 22/04/20 1.6    Added FdmnesCompare and __add__ method for FdmnesAnalysis
+20/07/23 2.0    Refactored program and updated, added new methods and put indata writer in classes_properties
 
 @author: DGPorter
 """
 
 import os, re
 import numpy as np
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d import Axes3D  # 3D plotting
 
 from . import functions_general as fg
 from . import functions_crystallography as fc
+from . import Crystal
 
-__version__ = '1.6'
+
+__version__ = '2.0'
 
 
 class Fdmnes:
     """
-    FDMNES Create files and run program
+    FDMNES class: Create input files for the FDMNES software and run the program inside a python console
+
+    FDMNES (Finite Difference Method for Near Edge Structure) is an abinitio DFT program for
+    simulating x-ray absorption spectra and resonant diffraction.
+    FDMNES is developed by Yves Joly at CNRS and can be freely downloaded from here:
+      www.fdmnes.neel.cnrs.fr
+
+    In case of publication, please include the following citation:
+      O. Bunau and Y. Joly "Self-consistent aspects of x-ray absorption calculations"
+      J. Phys.: Condens. Matter 21, 345501 (2009)
+
+    This class creates a simple wrapper to automatically generate input files from Dans_Diffraction
+    Crystal structures. The output files from the calculation can also be automatically plotted.
 
     E.G.
+    xtl = Crystal('Co.cif')
     fdm = Fdmnes(xtl)
-    fdm.setup(comment='Test',
+    fdm.setup(folder_name='New_Calculation',
+              comment='Test',
               absorber='Co',
               edge='K'
               azi_ref=[0,0,1],
               hkl_reflections=[[1,0,0],[0,1,0],[1,1,0]]
-    fdm.create_files('New_Calculation')
+    fdm.create_files()
     fdm.write_fdmfile()
-    output = fdm.run_fdmnes()
+    fdm.run_fdmnes()
     ###Wait for program completion###
     analysis = fdm.analyse()
+    print(analysis)
+    analysis.xanes.plot()
+    analysis.density.plot()
+    for ref in analysis:
+        ref.plot3D()
     """
 
-    def __init__(self, xtl):
-        """
-        initialise
-        :param xtl: object
-        """
+    def __init__(self, xtl=Crystal()):
         self.xtl = xtl
 
         # Options
-        self.exe_path = find_fdmnes()
+        if fdmnes_checker():
+            self.exe_path = find_fdmnes()
+        else:
+            self.exe_path = ''
         self.output_name = 'out'
-        self.output_path = self.generate_output_path()
+        self.folder_name = fg.saveable(self.xtl.name)
         self.input_name = 'FDMNES_%s.txt' % fg.saveable(self.xtl.name)
+        self.output_path = self.generate_output_path()
         self.comment = ''
-        self.range = '-19 0.1 20'
+        self.range = '-19. 1. -5 0.1 -2. 0.05 5 0.1 10. 0.5 25 1 31. '
         self.radius = 4.0
         self.edge = 'K'
-        self.absorber = self.xtl.Atoms.type[0]
+        self.absorber = self.xtl.Properties.resonant_element()
         self.green = True
         self.scf = False
         self.quadrupole = False
+        self.magnetism = True if self.xtl.Structure.ismagnetic() else False
+        self.spinorbit = False
         self.azi_ref = [1, 0, 0]
         self.correct_azi = True
         self.hkl_reflections = [[1, 0, 0]]
 
+    def __repr__(self):
+        return "Fdmnes('%s')" % self.xtl.name
+
+    def __str__(self):
+        return self.info()
+
     def setup(self, exe_path=None, output_path=None, output_name=None, folder_name=None, input_name=None,
-              comment=None, range=None, radius=None, edge=None, absorber=None, green=None, scf=None,
+              comment=None, energy_range=None, radius=None, edge=None, absorber=None, green=None, scf=None,
               quadrupole=None, azi_ref=None, correct_azi=None, hkl_reflections=None):
-        """
+        r"""
         Set FDMNES Parameters
         :param exe_path: Location of FDMNES executable, e.g. 'c:\FDMNES\fdmnes_win64.exe'
         :param output_path: Specify the output path
         :param folder_name: Specify output folder name (replaces output_path)
         :param output_name: Name of FDMNES output files
         :param input_name: Name of FDMNES input file
         :param comment: A comment written in the input file
-        :param range: str energy range in eV relative to Fermi energy
+        :param energy_range: str energy range in eV relative to Fermi energy
         :param radius: calculation radius
         :param edge: absorptin edge, 'K', 'L3', 'L2'
         :param absorber: absorbing element, 'Co'
         :param green: Green's function (muffin-tin potential)
         :param scf: True/False, Self consistent solution
         :param quadrupole: False/True, E1E2 terms allowed
         :param azi_ref: azimuthal reference, [1,0,0]
         :param correct_azi: if True, correct azimuthal reference for real cell (use in hexagonal systems)
         :param hkl_reflections: list of hkl reflections [[1,0,0],[0,1,0]]
         :return: None
         """
         if exe_path is not None:
             self.exe_path = exe_path
+            self.output_path = self.generate_output_path()
 
         if output_path is not None:
             self.output_path = output_path
 
         if output_name is not None:
             self.output_name = output_name
 
         if folder_name is not None:
-            self.output_path = self.generate_output_path(folder_name)
+            self.folder_name = folder_name
+            self.output_path = self.generate_output_path()
 
         if input_name is not None:
             self.input_name = input_name
 
         if comment is not None:
             self.comment = comment
 
-        if range is not None:
-            self.range = range
+        if energy_range is not None:
+            self.range = energy_range
 
         if radius is not None:
             self.radius = radius
 
         if edge is not None:
             self.edge = edge
 
@@ -141,46 +173,49 @@
         if azi_ref is not None:
             self.azi_ref = azi_ref
 
         if correct_azi is not None:
             self.correct_azi = correct_azi
 
         if hkl_reflections is not None:
-            self.hkl_reflections = np.asarray(hkl_reflections).reshape(-1,3)
-
-        self.info()
+            self.hkl_reflections = np.asarray(hkl_reflections).reshape(-1, 3)
 
     def info(self):
         """
         Print setup info
-        :return: None
+        :return: str
         """
-
-        print('FDMNES Options')
-        print('exe_path : %s' % self.exe_path)
-        print('output_path : %s' % self.output_path)
-        print('output_name : %s' % self.output_name)
-        print('input_name : %s' % self.input_name)
-        print('comment : %s' % self.comment)
-        print('range : %s' % self.range)
-        print('radius : %s' % self.radius)
-        print('absorber : %s' % self.absorber)
-        print('edge : %s' % self.edge)
-        print('green : %s' % self.green)
-        print('scf : %s' % self.scf)
-        print('quadrupole : %s' % self.quadrupole)
+        s = 'FDMNES Options\n'
+        s += 'Crystal: %s\n' % self.xtl.name
+        s += 'exe_path : %s\n' % self.exe_path
+        s += 'output_path : %s\n' % self.output_path
+        s += 'output_name : %s\n' % self.output_name
+        s += 'input_name : %s\n' % self.input_name
+        s += 'comment : %s\n' % self.comment
+        s += 'range : %s\n' % self.range
+        s += 'radius : %s\n' % self.radius
+        s += 'absorber : %s\n' % self.absorber
+        s += 'edge : %s\n' % self.edge
+        s += 'green : %s\n' % self.green
+        s += 'scf : %s\n' % self.scf
+        s += 'quadrupole : %s\n' % self.quadrupole
         if self.correct_azi:
-            print('azi_ref : %s' % self.azimuthal_reference(self.azi_ref))
+            s += 'azi_ref : %s\n' % self.azimuthal_reference(self.azi_ref)
         else:
-            print('azi_ref : %s' % self.azi_ref)
-        print('hkl_reflections:')
+            s += 'azi_ref : %s\n' % self.azi_ref
+        s += 'hkl_reflections:\n'
         for ref in self.hkl_reflections:
-            print('  (%1.0f,%1.0f,%1.0f)' % (ref[0], ref[1], ref[2]))
+            s += '  (%1.0f,%1.0f,%1.0f)\n' % (ref[0], ref[1], ref[2])
+        return s
+
+    def find_fdmnes_exe(self, initial_dir=None, fdmnes_filename='fdmnes_win64.exe', reset=False):
+        """Find fdmnes executable"""
+        self.exe_path = find_fdmnes(reset=reset, fdmnes_filename=fdmnes_filename, initial_dir=initial_dir)
 
-    def azimuthal_reference(self, hkl=[1, 0, 0]):
+    def azimuthal_reference(self, hkl=(1, 0, 0)):
         """
         Generate the azimuthal reference
         :param hkl: (1*3) array [h,k,l]
         :return: None
         """
 
         UV = self.xtl.Cell.UV()
@@ -192,184 +227,99 @@
         return fdm_ar
 
     def generate_parameters_string(self):
         """
         Create the string of parameters and comments for the input file
         :return: str
         """
-
-        # Get crystal parameters
-        UV = self.xtl.Cell.UV()
-        avUV=self.xtl.Cell.UV()
-        uvw, type, label, occupancy, uiso, mxmymz = self.xtl.Structure.get()
-
-        noat = len(uvw)
-
-        # Lattice parameters
-        a,b,c,alpha,beta,gamma = self.xtl.Cell.lp()
-
-        # element types
-        types,typ_idx = np.unique(type, return_inverse=True)
-        Z = fc.atom_properties(types,'Z')
-
-        absorber_idx = np.where(type == self.absorber)[0]
-        nonabsorber_idx = np.where(type != self.absorber)[0]
-
-        if self.correct_azi:
-            fdm_ar = self.azimuthal_reference(self.azi_ref)
-        else:
-            fdm_ar = self.azi_ref
-
-        if self.scf:
-            SCF = ''
-        else:
-            SCF = '!'
-
-        if self.quadrupole:
-            quadrupole = ''
-        else:
-            quadrupole = '!'
-
-        if self.green:
-            green = ''
-        else:
-            green = '!'
-
-        param_string = ''
-
-        # Write top matter
-        param_string += '! FDMNES indata file\n'
-        param_string += '! {}\n'.format(self.xtl.name)
-        param_string += '! {}\n'.format(self.comment)
-        param_string += '! indata file generated by Dans_Diffraction.classes_fdmnes\n'
-        param_string += '! By Dan Porter, PhD\n'
-        param_string += '\n'
-        param_string += ' Filout\n'
-        param_string += '   {}\n\n'.format(os.path.join(self.output_path,self.output_name))
-        param_string += '  Range                       ! Energy range of calculation (eV). Energy of photoelectron relative to Fermi level.\n'
-        param_string += ' %s \n\n'%self.range
-        param_string += ' Radius                       ! Radius of the cluster where final state calculation is performed\n'
-        param_string += '   {:3.1f}                        ! For a good calculation, this radius must be increased up to 6 or 7 Angstroems\n\n'.format(self.radius)
-        param_string += ' Edge                         ! Threshold type\n'
-        param_string += '  {}\n\n'.format(self.edge)
-        param_string += '%s SCF                          ! Self consistent solution\n' % SCF
-        param_string += '%s Green                        ! Muffin tin potential - faster\n' % green
-        param_string += '%s Quadrupole                   ! Allows quadrupolar E1E2 terms\n' % quadrupole
-        param_string += '! magnetism                    ! performs magnetic calculations\n'
-        param_string += ' Density                      ! Outputs the density of states as _sd1.txt\n'
-        param_string += ' Sphere_all                   ! Outputs the spherical tensors as _sph_.txt\n'
-        param_string += ' Cartesian                    ! Outputs the cartesian tensors as _car_.txt\n'
-        param_string += ' energpho                     ! output the energies in real terms\n'
-        param_string += ' Convolution                  ! Performs the convolution\n\n'
-
-        param_string += ' Zero_azim                    ! Define basis vector for zero psi angle\n'
-        param_string += '  {:6.3f} {:6.3f} {:6.3f}     '.format(fdm_ar[0],fdm_ar[1],fdm_ar[2])
-        if self.correct_azi:
-            param_string += '! Same as I16, Reciprocal ({} {} {}) in units of real SL. \n'.format(self.azi_ref[0],self.azi_ref[1],self.azi_ref[2])
-        else:
-            param_string += '\n'
-
-        param_string += ' rxs                          ! Resonant x-ray scattering at various peaks, peak given by: h k l sigma pi azimuth.\n'
-        for hkl in self.hkl_reflections:
-            param_string += ' {} {} {}    1 1                 ! ({} {} {}) sigma-sigma\n'.format(hkl[0],hkl[1],hkl[2],hkl[0],hkl[1],hkl[2])
-            param_string += ' {} {} {}    1 2                 ! ({} {} {}) sigma-pi\n'.format(hkl[0],hkl[1],hkl[2],hkl[0],hkl[1],hkl[2])
-        param_string += ' \n'
-
-        param_string += ' Atom ! s=0,p=1,d=2,f=3, must be neutral, get d states right by moving e to 2s and 2p sites\n'
-        for n in range(len(types)):
-            param_string += ' {:3.0f} 0 ! {}\n'.format(Z[n],types[n])
-        param_string += ' \n'
-
-        param_string += ' Crystal                      ! Periodic material description (unit cell)\n'
-        param_string += ' {:9.5f} {:9.5f} {:9.5f} {:9.5f} {:9.5f} {:9.5f}\n'.format(a,b,c,alpha,beta,gamma)
-        param_string += '! Coordinates - 1st atom is the absorber\n'
-        # Write atomic coordinates
-        for nn in range(len(absorber_idx)):
-            n = absorber_idx[nn]
-            param_string += '{0:2.0f} {1:20.15f} {2:20.15f} {3:20.15f} ! {4:-3.0f} {5:2s}\n'.format(typ_idx[n]+1,uvw[n,0],uvw[n,1],uvw[n,2],n,type[n])
-        for nn in range(len(nonabsorber_idx)):
-            n = nonabsorber_idx[nn]
-            param_string += '{0:2.0f} {1:20.15f} {2:20.15f} {3:20.15f} ! {4:-3.0f} {5:2s}\n'.format(typ_idx[n]+1,uvw[n,0],uvw[n,1],uvw[n,2],n,type[n])
-        param_string += '\n'
-
-        # Write end matter
-        param_string += ' End\n'
-        return param_string
-
-    def write_runfile(self, param_string=None):
-        """
-        Write FDMNES input data to a file
-        :return: None
-        """
-
-        if param_string is None:
-            param_string = self.generate_parameters_string()
-
-        # Create cell file
-        fname = os.path.join(self.output_path, self.input_name)
-        fdfile = open(fname, 'w')
-        fdfile.write(param_string)
-        fdfile.close()
-        print("FDMNES file written to {}".format(os.path.join(self.output_path, self.input_name)))
+        outstr = self.xtl.Properties.fdmnes_runfile(
+            output_path=os.path.join(self.output_path, self.output_name),
+            comment=self.comment,
+            energy_range=self.range,
+            radius=self.radius,
+            edge=self.edge,
+            absorber=self.absorber,
+            green=self.green,
+            scf=self.scf,
+            quadrupole=self.quadrupole,
+            magnetism=self.magnetism,
+            spinorbit=self.spinorbit,
+            azi_ref=self.azi_ref,
+            correct_azi=self.correct_azi,
+            hkl_reflections=self.hkl_reflections
+        )
+        return outstr
 
     def generate_output_path(self, folder_name=None, overwrite=False):
-        """
-        Creates an automatic output path in the FDMNES/Sims directory
+        r"""
+        Creates an automatic output path in the FDMNES/Sim directory
          If overwrite is False and the directory already exists, a number will be appended to the name
         :param folder_name: str or None, if None xtl.name will be used
         :param overwrite: True/False
-        :return: str directory E.G. 'c:\FDMNES\sim\Fe2O3'
+        :return: str directory E.G. 'c:\FDMNES\Sim\Fe2O3'
         """
 
         if folder_name is None:
-            folder_name = fg.saveable(self.xtl.name)
+            folder_name = self.folder_name
 
-        newpath = os.path.join(os.path.dirname(self.exe_path), 'sim', folder_name)
+        newpath = os.path.join(os.path.dirname(self.exe_path), 'Sim', folder_name)
 
         if overwrite:
             return newpath
 
         n = 0
         while os.path.isdir(newpath):
             n += 1
-            newpath = os.path.join(os.path.dirname(self.exe_path), 'sim', folder_name+'_%d'%n)
+            newpath = os.path.join(os.path.dirname(self.exe_path), 'Sim', folder_name + '_%d' % n)
         return newpath
 
     def generate_input_path(self):
-        """
+        r"""
         Returns the input file pathname
-         E.G. 'c:\FDMNES\sim\Fe2O3\FDMNES_Fe2O3.txt'
+         E.G. 'c:\FDMNES\Sim\Fe2O3\FDMNES_Fe2O3.txt'
         :return: filepath
         """
         return os.path.join(self.output_path, self.input_name)
 
     def create_directory(self):
         """
         Create a directory in the FDMNES/Sim folder
         :return: None
         """
-
+        if not self.exe_path:
+            raise AttributeError('FDMNES executable path has not been specified')
         if not os.path.isdir(self.output_path):
             os.makedirs(self.output_path)
+            print("Created folder: '{}'".format(self.output_path))
+
+    def write_runfile(self, param_string=None):
+        """
+        Write FDMNES input data to a file
+        :param param_string: str text to add to indata file (None will generate)
+        :return: None
+        """
+
+        if param_string is None:
+            param_string = self.generate_parameters_string()
+
+        # Create cell file
+        fname = self.generate_input_path()
+        with open(fname, 'w') as fdfile:
+            fdfile.write(param_string)
+        print("FDMNES file written to '{}'".format(fname))
 
-    def create_files(self, folder_name=None, param_string=None):
+    def create_files(self, param_string=None):
         """
         Create FDMNES calculation directory and files
          - creates new directory
          - writes the input file to that directory
-        :param folder_name: Set a folder name with the 'sim' folder of fdmnes, or None for default
-        :param param_string: Pass a string of the parameter input file to write
+        :param param_string: str text to add to indata file (None will generate)
         :return: None
         """
-
-        if folder_name is not None:
-            self.output_path = self.generate_output_path(folder_name)
         self.create_directory()
-        if param_string is None:
-            param_string = self.generate_parameters_string()
         self.write_runfile(param_string)
         print('Ready for calculation!')
 
     def write_fdmfile(self, file_list=None):
         """
         Create fdmfile with list of calculations
         :param file_list: list of parameter file names for fdmfile, or None to only calculate current parameters
@@ -379,54 +329,60 @@
         if file_list is None:
             file_list = [os.path.join(self.output_path, self.input_name)]
 
         fdmstr = ''
         fdmstr += '! FDMNES Calculations\n'
         fdmstr += '! List of calculations here\n\n'
 
-        fdmstr += ' %1.0f\n'%len(file_list)
+        fdmstr += ' %1.0f\n' % len(file_list)
         fdmstr += '\n'.join(file_list)
 
         # Create/ overwrite file
+        if not self.exe_path:
+            raise AttributeError('FDMNES executable path has not been specified')
         fdmfile = os.path.join(os.path.dirname(self.exe_path), 'fdmfile.txt')
-        out = open(fdmfile, 'w')
-        out.write(fdmstr)
-        out.close()
+        with open(fdmfile, 'w') as out:
+            out.write(fdmstr)
         print('fdmfile created.')
 
     def run_fdmnes(self):
         """
         Run the fdmnes code, waits until the program completes
         Remember to use self.create_files and self.write_fdmfile first!
         :return: subprocess.call output
         """
+        if not self.exe_path:
+            raise AttributeError('FDMNES executable path has not been specified')
 
         import subprocess
         wd = os.getcwd()
         path, file = os.path.split(self.exe_path)
         os.chdir(path)
         print('Starting FDMNES...')
         output = subprocess.call(file, shell=True)
         os.chdir(wd)
         print('FDMNES Finished!')
         return output
 
-    def analyse(self,folder_name=None):
+    def analyse(self, folder_name=None):
         """
         Analyse the completed calculation
-        :param folder_name: if not None, loads data from here
+        :param folder_name: str name or directory of calculation (None to use current calculation)
         :return: FdmnesAnalysis Object
         """
 
         analysis_path = self.output_path
 
         if folder_name is not None:
-            analysis_path = self.generate_output_path(folder_name, overwrite=True)
-
-        return FdmnesAnalysis(analysis_path, self.output_name)
+            if os.path.isdir(folder_name):
+                analysis_path = folder_name
+            else:
+                analysis_path = self.generate_output_path(folder_name, overwrite=True)
+        calcname = '%s %s %s' % (self.xtl.name, self.absorber, self.edge)
+        return FdmnesAnalysis(analysis_path, self.output_name, calc_name=calcname)
 
 
 class FdmnesAnalysis:
     """
     Create fdmnes object from *_scan_conv.txt file
 
     Usage:
@@ -444,34 +400,37 @@
     energy = np.array([0])
     angle = np.array([0])
     reflections = {}
     reflist = []
     refkeys = []
     sphkeys = []
 
-    def __init__(self, output_path, output_name='out'):
-        """
+    def __init__(self, output_path, output_name='out', calc_name=None):
+        r"""
         Loads data from an FDMNES calculation, allowing plotting and data cuts
          E.G.
          fdm = FdmnesAnalysis('c:\FDMNES\Fe2O3','out')
          fdm.xanes.plot()
          plt.show()
 
         :param output_path: directory of the calculation to be loaded
         :param output_name: base output name for the calculation (default='out')
         """
         output_path = output_path.replace('\\', '/')  # convert windows directories
-        if output_path[-4:].lower() == '.txt':
+        if output_path.endswith('.txt'):
             output_path, filename = os.path.split(output_path)
             filename = filename.replace('_', '.')
             output_name = filename.split('.')[0]
-        calc_name = output_path.split('/')[-1]  # calculation name
-        bav_name = os.path.join(output_path,output_name+'_bav.txt')
-        scan_conv_name = os.path.join(output_path,output_name+'_scan_conv.txt')
-        convname = os.path.join(output_path,output_name+'_conv.txt')
+        elif not os.path.isdir(output_path):
+            output_path = sim_folder(output_path)
+        if calc_name is None:
+            calc_name = output_path.split('/')[-1]  # calculation name
+        bav_name = os.path.join(output_path, output_name + '_bav.txt')
+        scan_conv_name = os.path.join(output_path, output_name + '_scan_conv.txt')
+        convname = os.path.join(output_path, output_name + '_conv.txt')
         densityname = os.path.join(output_path, output_name + '_sd%d.txt')
         spherename = os.path.join(output_path, output_name + '_sph_signal_rxs%d.txt')
 
         self.output_name = output_name
         self.output_path = output_path
         self.calc_name = calc_name
 
@@ -488,14 +447,16 @@
 
         # Read density of states file
         # sometimes this is _sd0.txt and sometimes _sd1.txt
         if os.path.isfile(densityname % 0):
             self.density = Density(densityname % 0)
         elif os.path.isfile(densityname % 1):
             self.density = Density(densityname % 1)
+        else:
+            self.density = None
 
         if os.path.isfile(scan_conv_name):
             # Read reflection files (_scan_conv.txt)
             energy, angle, intensity = read_scan_conv(scan_conv_name)
             self.energy = energy
             self.angle = angle
             self.reflections = intensity
@@ -512,15 +473,15 @@
                 refobj = Reflection(self.energy, self.angle, self.reflections[ref], ref, calc_name)
                 setattr(self, refname, refobj)
                 self.refkeys += [refname]
 
                 # Read spherical contribution files
                 sphrefname = 'sph_' + refname
                 if os.path.isfile(spherename % (n + 1)):
-                    data = np.genfromtxt(spherename % (n + 1), skip_header=3, names=True)
+                    data = read_spherical(spherename % (n + 1))
                     sphobj = Spherical(data, ref, calc_name)
                     setattr(self, sphrefname, sphobj)
                     self.sphkeys += [sphrefname]
         else:
             self.reflist = []
             self.refkeys = []
             self.sphkeys = []
@@ -531,24 +492,37 @@
         :return: str
         """
         out = 'FDMNES Analysis: %s' % os.path.join(self.output_path, self.output_name+'.txt')
         out += self.bavfile.header()
         return out
 
     def __repr__(self):
+        return "FdmnesAnalysis('%s', '%s', calc_name='%s')" % (self.output_path, self.output_name, self.calc_name)
+
+    def __str__(self):
         name = '%s/%s' % (self.calc_name, self.output_name)
         filename = os.path.join(self.output_path, self.output_name+'.txt')
         cycles = self.bavfile.cycles()
         edge = self.bavfile.edge()
         radius = self.bavfile.radius()
-        return 'FDMNES Analysis: %30s, Edge: %20s, Radius: %10s, Cycles: %10s' % (name, edge, radius, cycles)
+        refs = ', '.join(self.refkeys)
+        sphs = ', '.join(self.sphkeys)
+        out = 'FDMNES Analysis: %30s\nEdge: %20s\nRadius: %10s\nCycles: %10s\n' % (name, edge, radius, cycles)
+        out += 'RXS Refs: %s\nSPH Refs: %s\n' % (refs, sphs)
+        return out
 
     def __add__(self, other):
         return FdmnesCompare([self, other])
 
+    def __getitem__(self, item):
+        """Return Reflection"""
+        if item in self.refkeys or item in self.sphkeys:
+            return getattr(self, item)
+        return getattr(self, self.refkeys[item])
+
 
 class FdmnesCompare:
     """
     Compare FDMNES Calculations
     Method of joining sevearl FdmnesAnalysis objects to plot spectra on the same plot for comparison.
     Usage:
         fd1 = FdmnesAnalysis('calc_dir/calc1')
@@ -565,17 +539,17 @@
         fdms.plot_reflection_azimuth('I003sp', 2838) # specify energy in eV
     """
 
     def __init__(self, fdm_objects):
         self.fdm_objects = fdm_objects
         self._gen_refkeys()
 
-    def load(self, bav_files=[]):
+    def load(self, bav_files=()):
         """Load a series of calculation files"""
-        bav_files = np.array(bav_files).reshape(-1)
+        bav_files = np.asarray(bav_files).reshape(-1)
         for file in bav_files:
             self.fdm_objects += [FdmnesAnalysis(file)]
             print(self.fdm_objects[-1])
         self._gen_refkeys()
 
     def _gen_refkeys(self):
         """Generate unique reflection keys"""
@@ -641,15 +615,15 @@
                 print('No %s in %s' % (refkey, fdm))
                 continue
             en = ref.energy
             inten = ref.eng_cut(psi)
             if normalise:
                 inten = inten/inten.max()
             plt.plot(en, inten, '-', lw=3, label=fdm.calc_name)
-        plt.title('%s $\Psi$ = %s Deg' % (refkey, psi), fontsize=32, fontname='Times New Roman')
+        plt.title(r'%s $\Psi$ = %s Deg' % (refkey, psi), fontsize=32, fontname='Times New Roman')
         plt.legend(loc=0, frameon=False, fontsize=20)
         plt.xlabel('Energy [eV]', fontsize=28, fontname='Times New Roman')
         plt.ylabel('Intensity [arb. units]', fontsize=28, fontname='Times New Roman')
         plt.xticks(fontsize=25, fontname='Times New Roman')
         plt.yticks(fontsize=25, fontname='Times New Roman')
 
     def plot_reflection_azimuth(self, refkey, energy=0, normalise=False, new_figure=True):
@@ -675,15 +649,15 @@
             psi = ref.angle
             inten = ref.azi_cut(energy)
             if normalise:
                 inten = inten/inten.max()
             plt.plot(psi, inten, '-', lw=3, label=fdm.calc_name)
         plt.title('%s E = %s eV' % (refkey, energy), fontsize=32, fontname='Times New Roman')
         plt.legend(loc=0, frameon=False, fontsize=20)
-        plt.xlabel('$\Psi$ [Deg]', fontsize=28, fontname='Times New Roman')
+        plt.xlabel(r'$\Psi$ [Deg]', fontsize=28, fontname='Times New Roman')
         plt.ylabel('Intensity [arb. units]', fontsize=28, fontname='Times New Roman')
         plt.xticks(fontsize=25, fontname='Times New Roman')
         plt.yticks(fontsize=25, fontname='Times New Roman')
 
     def plot_all_spectra(self, psi=0, normalise=False):
         """
         Plot all available spectra across calculations
@@ -792,14 +766,16 @@
 
     def potrmt_str(self):
         """
         Return final cycle "Potrmt" string
         :return: str
         """
         keys = list(self.potrmt.keys())
+        if len(keys) == 0:
+            return '"Potrmt" charge string not found'
         outstr = ' '.join(['%8s' % key for key in keys]) + '\n'
         for n in range(len(self.potrmt[keys[0]])):
             outstr += ' '.join(['%8s' % self.potrmt[key][n] for key in keys]) + '\n'
         return outstr
 
     def cycle_energy(self):
         """Return array of total energy per atom for each cycle"""
@@ -840,14 +816,17 @@
         """
         self.energy = energy
         self.angle = angle
         self.intensity = intensity
         self.refname = refname
         self.calc_name = calc_name
 
+    def __repr__(self):
+        return "Reflection('%s', '%s')" % (self.refname, self.calc_name)
+
     def azi_cut(self, cutenergy=None):
         """
         Returns the array of intensitiy values at a particular energy
         :param cutenergy: energy of cut (eV)
         :return: array of intensities
         """
         cutintensity = azi_cut(self.energy, self.intensity, cutenergy)
@@ -868,15 +847,16 @@
         :return: None
         """
         # 3D figure
         fig = plt.figure(figsize=[12, 10], dpi=80)
         ax = fig.add_subplot(111, projection='3d')
 
         XX, YY = np.meshgrid(self.angle, self.energy)
-        ax.plot_surface(XX, YY, self.intensity, rstride=3, cstride=3, cmap=plt.cm.coolwarm,
+        cm = plt.get_cmap('coolwarm')
+        ax.plot_surface(XX, YY, self.intensity, rstride=3, cstride=3, cmap=cm,
                         linewidth=0, antialiased=False)
 
         # Axis labels
         ax.set_xlabel('Angle (DEG)', fontsize=18)
         ax.set_ylabel('Energy (eV)', fontsize=18)
         ax.set_zlabel('Intensity', fontsize=18)
         plt.suptitle('{}\n{}'.format(self.calc_name, self.refname), fontsize=21, fontweight='bold')
@@ -918,14 +898,17 @@
         :param intensity: array of intensity values
         :param calc_name: calculation name for plot title
         """
         self.energy = energy
         self.intensity = intensity
         self.calc_name = calc_name
 
+    def __repr__(self):
+        return "Xanes('%s')" % self.calc_name
+
     def plot(self):
         """
         Plot the Xanes spectra
         :return: None
         """
         plt.figure(figsize=[12, 10], dpi=80)
         plt.plot(self.energy, self.intensity, lw=3)
@@ -941,63 +924,32 @@
         """
         Load Density of states file from FDMNES calculations '..._sd0.txt'
         :param file: filename
         """
 
         dirname, filetitle = os.path.split(file)  # calculation directory
         self.calc_name = dirname.split('/')[-1]  # calculation name
-        self.data = np.genfromtxt(file, skip_header=0, names=True)
+        self.data = read_density(file)
 
-        self.energy = self.data['Energy']
-        self.s = np.zeros(len(self.energy))
-        self.s_total = np.zeros(len(self.energy))
-        self.px = np.zeros(len(self.energy))
-        self.py = np.zeros(len(self.energy))
-        self.pz = np.zeros(len(self.energy))
-        self.p_total = np.zeros(len(self.energy))
-        self.dxy = np.zeros(len(self.energy))
-        self.dxz = np.zeros(len(self.energy))
-        self.dyz = np.zeros(len(self.energy))
-        self.dx2y2 = np.zeros(len(self.energy))
-        self.dz2r2 = np.zeros(len(self.energy))
-        self.d_total = np.zeros(len(self.energy))
-
-        # Calculate real harmonics - old field names
-        if 'n11' in self.data.dtype.fields.keys():
-            self.s = self.data['n00']
-            self.s_total = self.data['n_l0']
-        if 'n11' in self.data.dtype.fields.keys():
-            self.px = self.data['n11_1']
-            self.py = self.data['n11']
-            self.pz = self.data['n10']
-            self.p_total = self.data['n_l1']
-        if 'n22' in self.data.dtype.fields.keys():
-            self.dxy = self.data['n22_1']
-            self.dxz = self.data['n21_1']
-            self.dyz = self.data['n21']
-            self.dx2y2 = self.data['n22']
-            self.dz2r2 = self.data['n20']
-            self.d_total = self.data['n_l2']
-
-        # Calculate real harmonics - new field names fdmnes version 2020+
-        if 's' in self.data.dtype.fields.keys():
-            self.s = self.data['s']
-            self.s_total = self.data['Ints']
-        if 'px' in self.data.dtype.fields.keys():
-            self.px = self.data['px']
-            self.py = self.data['py']
-            self.pz = self.data['pz']
-            self.p_total = self.data['Intp']
-        if 'dxy' in self.data.dtype.fields.keys():
-            self.dxy = self.data['dxy']
-            self.dxz = self.data['dxz']
-            self.dyz = self.data['dyz']
-            self.dx2y2 = self.data['dx2y2']
-            self.dz2r2 = self.data['dz2']
-            self.d_total = self.data['Intd']
+        self.energy = self.data['energy']
+        self.s = self.data['s']
+        self.s_total = self.data['s_total']
+        self.px = self.data['px']
+        self.py = self.data['py']
+        self.pz = self.data['pz']
+        self.p_total = self.data['p_total']
+        self.dxy = self.data['dxy']
+        self.dxz = self.data['dxz']
+        self.dyz = self.data['dyz']
+        self.dx2y2 = self.data['dx2y2']
+        self.dz2r2 = self.data['dz2r2']
+        self.d_total = self.data['d_total']
+
+    def __repr__(self):
+        return "Density('%s')" % self.calc_name
 
     def plot(self):
         """
         Creates a plot of the DOS spectra, with all d states in one plot
         :return: None
         """
 
@@ -1019,39 +971,33 @@
         plt.ticklabel_format(style='sci', scilimits=(-3, 3))
 
 
 class Spherical:
     def __init__(self, data, refname, calc_name):
         """
         Load contribution from spherical harmonics from out_sph_signal_rxs1.txt
-        :param data: data array from genfromtext
+        :param data: data array from read_spherical()
         :param refname: reflection name for plot title
         :param calc_name: calculation name for plot title
         """
 
         self.data = data
         self.calc_name = calc_name
         self.refname = refname
 
-        self.energy = self.data['Energy']
+        self.energy = self.data['energy']
+        self.d_total = self.data['D00']
+        self.dxy = self.data['D_xy']
+        self.dxz = self.data['D_xz']
+        self.dyz = self.data['D_yz']
+        self.dx2y2 = self.data['D_x2y2']
+        self.dz2r2 = self.data['D_z2']
 
-        self.d_total = self.data['D00_r'] + 1j * self.data['D00_i']
-
-        self.dxy = self.data['D_xy_r'] + 1j * self.data['D_xy_i']
-        self.dxz = self.data['D_xz_r'] + 1j * self.data['D_xz_i']
-        self.dyz = self.data['D_yz_r'] + 1j * self.data['D_yz_i']
-        self.dx2y2 = self.data['D_x2y2_r'] + 1j * self.data['D_x2y2_i']
-        self.dz2r2 = self.data['D_z2_r'] + 1j * self.data['D_z2_i']
-
-        self.d_total = np.real(self.d_total * np.conj(self.d_total))
-        self.dxy = np.real(self.dxy * np.conj(self.dxy))
-        self.dxz = np.real(self.dxz * np.conj(self.dxz))
-        self.dyz = np.real(self.dyz * np.conj(self.dyz))
-        self.dx2y2 = np.real(self.dx2y2 * np.conj(self.dx2y2))
-        self.dz2r2 = np.real(self.dz2r2 * np.conj(self.dz2r2))
+    def __repr__(self):
+        return "Spherical('%s', '%s')" % (self.refname, self.calc_name)
 
     def plot(self):
         """
         Plot the spherical components
         :return: None
         """
 
@@ -1070,103 +1016,112 @@
         plt.ylabel('|d$_{ii}$|$^2$', fontsize=28, fontname='Times New Roman')
         plt.xticks(fontsize=20, fontname='Times New Roman')
         plt.yticks(fontsize=20, fontname='Times New Roman')
         plt.ticklabel_format(useOffset=False)
         plt.ticklabel_format(style='sci', scilimits=(-3, 3))
 
 
-############## FUNCTIONS ########################
+"--------------------------------------------------------"
+"------------------------ FUNCTIONS ---------------------"
+"--------------------------------------------------------"
 
 
-def fdmnes_checker(activate=False):
+def fdmnes_checker(activate=False, fdmnes_filename='fdmnes_win64.exe', initial_dir=None):
     """Returns True if fdmnes available and activated"""
 
-    datadir = os.path.abspath(os.path.dirname(__file__))  # same directory as this file
-    pointerfile = os.path.join(datadir, 'data', 'FDMNES_pointer.txt')
-
     if activate:
-        find_fdmnes(reset=True)
+        find_fdmnes(fdmnes_filename=fdmnes_filename, reset=True, initial_dir=initial_dir)
 
-    if os.path.isfile(pointerfile):
-        with open(pointerfile) as file:
-            for location in file:
-                loc = location.strip()
-                if os.path.isfile(loc):
-                    return True
-    return False
-
-
-def fdmnes_location():
-    """
-    Returns the current location of the FDMNES pointer, or None otherwise
-    :return: str
-    """
-
-    # Dans_Diffraction FDMNES pointer file
     datadir = os.path.abspath(os.path.dirname(__file__))  # same directory as this file
     pointerfile = os.path.join(datadir, 'data', 'FDMNES_pointer.txt')
 
     if os.path.isfile(pointerfile):
         with open(pointerfile) as file:
             for location in file:
                 loc = location.strip()
                 if os.path.isfile(loc):
-                    return loc
-    return find_fdmnes()
+                    return True
+    return False
 
 
-def find_fdmnes(fdmnes_filename='fdmnes_win64.exe', reset=False):
+def find_fdmnes(fdmnes_filename='fdmnes_win64.exe', reset=False, initial_dir=None):
     """
     Finds the path of the fdmnes_win64.exe file
      The name of the file is taken from the envrionment varialbe fdmnes_filename
      The first time this is run, it will take a while, searching through every folder for the file
      On completion, a file will be generated in the /data directory with the filepath
      Subsequent runs will quickly load from this file
     :param fdmnes_filename: name of the executable to search for
     :param reset: if True, pointerfile will be ignored.
+    :param initial_dir: None or str, if directory, look here for file
     :return: str : location of fdmnes executable file
     """
 
     # Dans_Diffraction FDMNES pointer file
     datadir = os.path.abspath(os.path.dirname(__file__))  # same directory as this file
     pointerfile = os.path.join(datadir, 'data', 'FDMNES_pointer.txt')
 
-    if os.path.isfile(pointerfile):
+    if not reset and os.path.isfile(pointerfile):
         with open(pointerfile) as file:
             for location in file:
                 loc = location.strip()
                 if os.path.isfile(loc):
                     return loc
 
+    if os.path.isfile(fdmnes_filename):
+        # Save location
+        with open(pointerfile, 'w') as file:
+            file.write(os.path.abspath(fdmnes_filename))
+        return os.path.abspath(fdmnes_filename)
+
+    initial_dir = os.path.abspath(os.sep) if initial_dir is None else initial_dir
+
     # Find FDMNES
     print('Hang on... just looking for %s...' % fdmnes_filename)
-    for dirName, subdirList, fileList in os.walk(os.path.abspath(os.sep)):
+    for dirName, subdirList, fileList in os.walk(initial_dir):
         if fdmnes_filename in fileList:
-            print('Found FDMNES at: %s'%dirName)
+            print('Found FDMNES at: %s' % dirName)
             location = os.path.join(dirName, fdmnes_filename)
             # Save location
-            file = open(pointerfile, 'w')
-            file.write(location)
-            file.close()
+            with open(pointerfile, 'w') as file:
+                file.write(location)
             return location
     print('%s not found, please enter location manually' % fdmnes_filename)
     return os.path.abspath(os.sep)
 
 
+def sim_folder(folder_name='', new_folder=False):
+    r"""
+    Generates a calculation path directory in the FDMNES/Sim directory
+      If new_folder is True and the directory already exists, a number will be appended to the name
+    :param folder_name: str folder name
+    :param new_folder: True/False*
+    :return: str directory E.G. 'c:\FDMNES\Sim\folder_name'
+    """
+    exe_path = find_fdmnes()
+    newpath = os.path.join(os.path.dirname(exe_path), 'Sim', folder_name)
+    if new_folder:
+        n = 0
+        while os.path.isdir(newpath):
+            n += 1
+            newpath = os.path.join(os.path.dirname(exe_path), 'Sim', folder_name + '_%d' % n)
+    return newpath
+
+
 def find_fdmnes_files(parent_directory=None, output_name='out'):
     """
     Finds all fdmnes calculations below a parent directory
     Assumes all files have the same output name
     :param parent_directory: top directory, searches lower directories recursivley
     :param output_name: e.g. 'out.txt'
     :return: list of filenames ['dir/out.txt']
     """
 
     if parent_directory is None:
-        parent_directory = fdmnes_location()
+        parent_directory = find_fdmnes()
 
     if '.txt' not in output_name:
         output_name = output_name + '_bav.txt'
 
     calc_dirs = []
     for dirpath, dirnames, filenames in os.walk(parent_directory):
         if output_name in filenames:
@@ -1191,15 +1146,15 @@
     fdms.load(calc_dirs)
     return fdms
 
 
 def read_conv(filename='out_conv.txt', plot=False):
     """
     Reads fdmnes output file out_conv.txt, that gives the XANES spectra
-      energy,intensity = read_conv(filename)
+      energy, intensity = read_conv(filename)
     """
 
     filename = filename.replace('\\', '/')  # convert windows directories
     dirname, filetitle = os.path.split(filename)  # calculation directory
     calc_name = dirname.split('/')[-1]  # calculation nam
 
     data = np.loadtxt(filename, skiprows=1)
@@ -1216,60 +1171,56 @@
         plt.yticks(fontsize=25, fontname='Times New Roman')
     return energy, xanes
 
 
 def read_scan_conv(filename='out_scan_conv.txt'):
     """
     Read FDMNES _scan_conv.txt files, return simulated azimuthal and energy values
-    energy,angle,intensity = read_scan_conv(filename)
-        filename = directory and name of _scan_conv.txt file
-        energy = [nx1] array of energy values
-        angle = [mx1] array on angle values
-        intensity = {'I(100)ss'}[nxm] dict of arrays of simulated intensities for each reflection
-
+       energy, angle, intensity = read_scan_conv('out_scan_conv.txt')
     You can see all the available reflections with intensity.keys()
+    :param filename: str name of '*_scan_conv.txt' file from FDMNED calculation
+    :return energy: [nx1] array of energy values
+    :return angle: [mx1] array on angle values
+    :return intensity:  {'I(100)ss'}[nxm] dict of arrays of simulated intensities for each reflection
     """
 
     # Open file
-    file = open(filename)
+    with open(filename) as file:
+        # Determine reflections in file
+        filetext = file.read()  # generate string
+        reftext = re.findall(r'I\(-?\d+-?\d+?-?\d+?\)\w+', filetext)  # find reflection strings
+
+        refs = np.unique(reftext)  # remove duplicates
+        Npeak = len(refs)
+        Nenergy = len(reftext) // Npeak
+        Nangle = 180
+
+        file.seek(0)  # return to start of file
+
+        # pre-define arrays
+        storevals = {}
+        for ref in refs:
+            storevals[ref] = np.zeros([Nenergy, Nangle])
+
+        storeeng = np.zeros(Nenergy)
+        storeang = np.zeros(Nangle)
+
+        # Read file, line by line
+        for E in range(Nenergy):
+            file.readline()  # blank line
+            storeeng[E] = float(file.readline().strip())  # energy
+            for P in range(Npeak):
+                peak = file.readline().strip()  # current reflection
+                # read angle,Intensity lines
+                vals = np.zeros([Nangle, 2])
+                for m in range(Nangle):
+                    vals[m, :] = [float(x) for x in file.readline().split()]
 
-    # Determine reflections in file
-    filetext = file.read()  # generate string
-    reftext = re.findall(r'I\(-?\d+-?\d+?-?\d+?\)\w+', filetext)  # find reflection strings
-
-    refs = np.unique(reftext)  # remove duplicates
-    Npeak = len(refs)
-    Nenergy = len(reftext) // Npeak
-    Nangle = 180
-
-    file.seek(0)  # return to start of file
-
-    # pre-define arrays
-    storevals = {}
-    for ref in refs:
-        storevals[ref] = np.zeros([Nenergy, Nangle])
-
-    storeeng = np.zeros(Nenergy)
-    storeang = np.zeros(Nangle)
-
-    # Read file, line by line
-    for E in range(Nenergy):
-        file.readline()  # blank line
-        storeeng[E] = float(file.readline().strip())  # energy
-        for P in range(Npeak):
-            peak = file.readline().strip()  # current reflection
-            # read angle,Intensity lines
-            vals = np.zeros([Nangle, 2])
-            for m in range(Nangle):
-                vals[m, :] = [float(x) for x in file.readline().split()]
-
-            storeang = vals[:, 0]  # store angle values
-            storevals[peak][E, :] = vals[:, 1]  # store intensity values
-
-    file.close()
+                storeang = vals[:, 0]  # store angle values
+                storevals[peak][E, :] = vals[:, 1]  # store intensity values
     return storeeng, storeang, storevals
 
 
 def azi_cut(storeeng, intensities, cutenergy=None):
     """
     Generate azimuthal cut at a particular energy
     cutintensity = azi_cut(storeeng,intensities,cutenergy)
@@ -1334,15 +1285,15 @@
     :return: dict with keys ['Z', 'charge', 'ch_ion', 'Vmft', 'Ionic radius']
     """
 
     # Header
     idx = bav_text.rfind('ch_ion')  # last occurance of ch_ion
     if idx == -1:
         return {}
-    hline = bav_text[ bav_text[:idx].rfind('\n') : bav_text[idx:].find('\n') + idx ].strip()
+    hline = bav_text[bav_text[:idx].rfind('\n'): bav_text[idx:].find('\n') + idx].strip()
     head = re.split(r'\s\s+', hline.strip())
 
     lines = bav_text[idx:].split('\n')
     values = []
     for line in lines[1:]:
         data = line.split()
         if len(data) != len(head): break
@@ -1350,7 +1301,70 @@
         values += [data]
 
     values = np.array(values)
     out = {}
     for n in range(len(head)):
         out[head[n]] = values[:, n]
     return out
+
+
+def read_density(filename):
+    """Load Density of states file from FDMNES calculations '..._sd0.txt'"""
+
+    data = np.genfromtxt(filename, skip_header=0, names=True)
+
+    # Old field names + new field names from fdmnes version 2020+
+    key_names = {
+        's': ['n00', 's'],
+        's_total': ['n_l0', 'Ints'],
+        'px': ['n11_1', 'px'],
+        'py': ['n11', 'py'],
+        'pz': ['n10', 'pz'],
+        'p_total': ['n_l1', 'Intp'],
+        'dxy': ['n22_1', 'dxy'],
+        'dxz': ['n21_1', 'dxz'],
+        'dyz': ['n21', 'dyz'],
+        'dx2y2': ['n22', 'dx2y2'],
+        'dz2r2': ['n20', 'dz2'],
+        'd_total': ['n_l2', 'Intd'],
+    }
+
+    def get_data(key):
+        values = np.zeros(len(data))
+        for name in key_names[key]:
+            if name in data.dtype.names:
+                values = data[name]
+        return values
+    out = {
+        key: get_data(key) for key in key_names
+    }
+    out['energy'] = data['Energy']
+    return out
+
+
+def read_spherical(filename):
+    """Load contribution from spherical harmonics to resonant reflection, from e.g. out_sph_signal_rxs1.txt"""
+    keys = ['D00', 'D_xy', 'D_xz', 'D_yz', 'D_x2y2', 'D_z2']
+    data = np.genfromtxt(filename, skip_header=3, names=True)
+    # Only load L3 part if "L23" is used
+    if 'D(00)_r_L3' in data.dtype.names or 'D(00)_r_1_L3' in data.dtype.names:
+        l3 = '_l3'
+    else:
+        l3 = ''
+
+    def modulus(key):
+        if key + '_r' + l3 in data.dtype.names:
+            value = data[key + '_r' + l3] + 1j * data[key + '_i' + l3]
+        elif key + '_r_1' + l3 in data.dtype.names:
+            n = 1
+            value = 0j
+            while key + ('_r_%d' % n) + l3 in data.dtype.names:
+                value += data[key + ('_r_%d' % n) + l3] + 1j * data[key + ('_i_%d' % n) + l3]
+                n += 1
+        else:
+            value = 0.0
+        return np.real(value * np.conj(value))
+    out = {
+        key: modulus(key) for key in keys
+    }
+    out['energy'] = data['Energy']
+    return out
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/classes_multicrystal.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_multicrystal.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/classes_orbitals.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_orbitals.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,24 +115,24 @@
     print(orb_3d7)
     >> 3d7
     """
     _level_max = [0, 1, 2, 3, 3, 2, 1]
     _state = ['s', 'p', 'd', 'f']
     _state_max = [2, 6, 10, 14]
 
-    def __init__(self, standard=None, n=1, l=0, fill=0):
-        if standard is not None:
-            self.standard = standard
-            self.n = int(standard[0])
-            self.l_name = standard[1].lower()
-            self.l = self._state.index(standard[1].lower())
-            if len(standard) == 2:
+    def __init__(self, orbital_string=None, n=1, l=0, fill=0):
+        if orbital_string is not None:
+            self.standard = orbital_string
+            self.n = int(orbital_string[0])
+            self.l_name = orbital_string[1].lower()
+            self.l = self._state.index(orbital_string[1].lower())
+            if len(orbital_string) == 2:
                 self.fill = 0.
             else:
-                self.fill = float(standard[2:])
+                self.fill = float(orbital_string[2:])
             self.max_fill = self._state_max[self.l]
             self.max_l = self._level_max[self.n - 1]
         else:
             self.n = int(n)
             self.l = int(l)
             self.fill = float(fill)
             self.l_name = self._state[l]
@@ -140,27 +140,34 @@
             self.max_l = self._level_max[self.n - 1]
             self.standard = self.generate_string_standard()
 
     def __call__(self):
         return self.generate_string_standard()
 
     def __repr__(self):
-        return 'Orbital: %s' % self.generate_string_standard()
+        return 'Orbital(%s)' % self.generate_string_standard()
+
+    def __str__(self):
+        return self.generate_string_standard()
 
     def __eq__(self, other):
         if isinstance(other, Orbital):
             if self.n == other.n and self.l == other.l:
                 return True
         return False
 
     def generate_string_standard(self):
         return '%d%s%1.3g' % (self.n, self.l_name, self.fill)
 
-    def generate_string_fdmnes(self):
-        return '%d %d %4.2f' % (self.n, self.l, self.fill)
+    def generate_string_fdmnes(self, spin=False):
+        if spin:
+            # split occupancy accross up and down states
+            return '%d %d %4.2f %4.2f' % (self.n, self.l, self.fill/2, self.fill/2)
+        else:
+            return '%d %d %4.2f' % (self.n, self.l, self.fill)
 
     def generate_string_latex(self):
         return '%d%s$^{%1.3g}$' % (self.n, self.l_name, self.fill)
 
     def add_electron(self, n=1.):
         new_fill = self.fill + n
         if new_fill > self.max_fill:
@@ -224,16 +231,23 @@
         self.z, self.name, config = fc.atom_properties(element, ['Z', 'Name', 'Config'])[0]
         self.orbitals = [Orbital(s) for s in config.split('.')]
         #self.oxidation_states = oxidation_states(element)
         self.charge = charge
         self.assign_charge(charge)
 
     def __repr__(self):
+        elestr = fc.element_charge_string(self.element_symbol, occupancy=self.occupancy, charge=self.charge)
+        return "Atom(%s)" % elestr
+
+    def __str__(self):
         return 'Atom: %s\n' % self.generate_string_standard()
 
+    def __getitem__(self, item):
+        return self.orbitals.__getitem__(item)
+
     def valence_orbitals(self):
         valence = []
         for orbital in self.orbitals[:-1]:
             if orbital.max_fill - orbital.fill > 0.01:
                 valence += [orbital]
         valence += [self.orbitals[-1]]
         return valence
@@ -377,49 +391,57 @@
             self.orbitals = self.orbitals[:-1]
 
     def generate_string_standard(self):
         elestr = fc.element_charge_string(self.element_symbol, occupancy=self.occupancy, charge=self.charge)
         orbstr = ' '.join([orb.generate_string_standard() for orb in self.orbitals])
         return '%3d %10s  %s' % (self.z, elestr, orbstr)
 
-    def generate_string_fdmnes(self):
+    def generate_string_fdmnes(self, spin=False):
         elestr = fc.element_charge_string(self.element_symbol, occupancy=self.occupancy, charge=self.charge)
         empty_orbital = self.orbitals[-1].next_orbital()
         valence = self.valence_orbitals()
         orbitals = valence + [empty_orbital]
-        fdm = '  '.join([orb.generate_string_fdmnes() for orb in orbitals])
+        # keep atom neutral by adding charge electrons to outer shell
+        unused = orbitals[-1].add_electron(self.charge)
+        fdm = '  '.join([orb.generate_string_fdmnes(spin) for orb in orbitals])
         std = ' '.join([orb.generate_string_standard() for orb in orbitals])
-        return '%d  %s ! %s %s' % (len(orbitals), fdm, elestr, std)
+        return '%3d %d  %s ! %s %s' % (self.z, len(orbitals), fdm, elestr, std)
 
     def generate_string_latex(self):
         orbstr = ' '.join([orb.generate_string_latex() for orb in self.orbitals])
         elestr = fc.element_charge_string(self.element_symbol, self.occupancy, self.charge, latex=True)
         return '%4s:  %s' % (elestr, orbstr)
 
 
 class Compound:
     """
     Compound - collection of atoms
-    LiCoO2 = Compound('Li0.7CoO2')
+    LiCoO2 = Compound([Atom, Atom, Atom])
     print(LiCoO2)
     >> Li0.7CoO2:
     >>   3 Li0.7+  1s2 2s0.3
     >>  27 Co3.3+  1s2 2s2 2p6 3s2 3p6 3d5 4s0.7
     >>   8  O2-  1s2 2s2 2p6
     >>   8  O2-  1s2 2s2 2p6
     """
 
     def __init__(self, atom_list):
-        self.atom_list = atom_list
+        self.atom_list = atom_list  # list of Atom objects
         self.balance_charge()
         self.compound_string = self.generate_charge_name()
 
     def __repr__(self):
+        return 'Compound(%s)' % self.compound_string
+
+    def __str__(self):
         return 'Compound: %s:\n%s' % (self.compound_string, self.generate_string_standard())
 
+    def __getitem__(self, item):
+        return self.atom_list.__getitem__(item)
+
     def charge_list(self):
         return [at.occupancy*at.check_charge() for at in self.atom_list]
 
     def balance_charge(self):
         """
         Add together known charges of elements (e.g. O, Na, Ca), use to estimate the charges of remaining ions
         :return:
@@ -452,20 +474,36 @@
             else:
                 newname = name
             if newname not in cnames:
                 cnames += [newname]
         return ' '.join(cnames)
 
     def generate_string_standard(self):
+        """Generate string showing atomic orbitals"""
         return '\n'.join([at.generate_string_standard() for at in self.atom_list])
 
-    def generate_string_fdmnes(self):
-        return '\n'.join([at.generate_string_fdmnes() for at in self.atom_list])
+    def generate_string_fdmnes(self, spin=False):
+        """Generate string showing atomic orbittals in FDMNES format"""
+        return '\n'.join([at.generate_string_fdmnes(spin) for at in self.atom_list])
+
+    def generate_string_fdmnes_absorber(self, absorber, spin=False):
+        """
+        Generate string showing atomic orbittals in FDMNES format
+        :param absorber: str element symbol of principal absorber
+        :param spin: Bool, if True element populations will be split by spin up/down
+        :return: str, element list
+        """
+        ele_list = [at.element_symbol for at in self.atom_list if at.element_symbol == absorber]
+        ele_list += [at.element_symbol for at in self.atom_list if at.element_symbol != absorber]
+        out = [at.generate_string_fdmnes(spin) for at in self.atom_list if at.element_symbol == absorber]
+        out += ['%3d 0 ! %s' % (at.z, at.element_symbol) for at in self.atom_list if at.element_symbol != absorber]
+        return '\n'.join(out), ele_list
 
     def generate_string_latex(self):
+        """Generate string showing atomic orbittals in Latex format"""
         return '\n'.join([at.generate_string_latex() for at in self.atom_list])
 
 
 class CompoundString(Compound):
     """
     Compound - collection of atoms
     LiCoO2 = Compound('Li0.7CoO2')
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/classes_orientation.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_orientation.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/classes_plotting.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
  functions to plot the crystal structure and simulated 
  diffraction patterns.
 
 By Dan Porter, PhD
 Diamond
 2017
 
-Version 1.9.5
-Last updated: 15/11/21
+Version 1.9.8
+Last updated: 19/05/24
 
 Version History:
 18/08/17 0.1    Program created
 30/10/17 1.0    Main functions finished.
 06/10/18 1.1    Program renamed
 05/03/18 1.2    Added plt.show() to functions
 17/04/18 1.3    Removed plt.show() from functions (allowing plot editing +stackig in non-interactive mode)
@@ -27,58 +27,60 @@
 16/06/20 1.8.2  Change to simulate_powder to make pixels int, remove linspace error in new numpy
 29/06/20 1.9.0  Removed scipy.convolve2d due to problems importing, new method more accurate but slower
 26/11/20 1.9.1  Added layers input to plot_layers
 21/01/21 1.9.2  Added plot_xray_resonance
 15/02/21 1.9.3  Added axis_reciprocal_lattice_points/lines/vectors
 11/10/21 1.9.4  Centered crystal in plot_crystal
 15/11/21 1.9.5  Added plot_diffractometer_reciprocal_space
+25/10/23 1.9.6  Corrected Plotting.simulate_powder to display radiation and wavelength
+03/05/24 1.9.7  Switched to using Scatter.generate_intensity_cut()
+19/05/24 1.9.8  Renamed to PlottingSuperstructure.parent_generate_inensity_cut
 
 @author: DGPorter
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d import Axes3D
 #from scipy.signal import convolve2d
 
 from . import functions_general as fg
 from . import functions_plotting as fp
 from . import functions_crystallography as fc
 
-__version__ = '1.9.5'
+__version__ = '1.9.8'
 
 
 class Plotting:
     """
     Plotting functions for the Crystal Object
     """
     # Plot options
     _figure_size = fp.FIGURE_SIZE
     _figure_dpi = fp.FIGURE_DPI
 
     def __init__(self, xtl):
-        "initialise"
         self.xtl = xtl
     
     def plot_crystal(self, show_labels=False):
         """
         Plot the atomic cell in 3D
             Click and drag to rotate the structure in 3D
             Atoms are coloured according to their label
             set show_labels=True to show the label of each sphere
         """
         
         # Generate lattice
         tol = 0.05
-        uvw, type, label, occ, uiso, mxmymz = self.xtl.Structure.generate_lattice(1, 1, 1)
+        uvw, element, label, occ, uiso, mxmymz = self.xtl.Structure.generate_lattice(1, 1, 1)
         #uvw,type,label,occ,uiso,mxmymz = self.xtl.Structure.get()
         
         # Split atom types, color & radii
         labels, idx, invidx = np.unique(label, return_index=True, return_inverse=True)
-        types = type[idx]
+        types = element[idx]
         colors = plt.cm.gist_rainbow(np.linspace(0, 1, len(types)))
         #sizes = 300*np.ones(len(types))
         #sizes[types=='O'] = 50.
         sizes = fc.atom_properties(types, 'Radii')
         
         # Get atomic positions
         R = self.xtl.Cell.calculateR(uvw)
@@ -274,15 +276,80 @@
         ax = plt.gca()
         for ex, dis in zip(exchange_paths, exchange_distances):
             x = [el[2][0] for el in ex]
             y = [el[2][1] for el in ex]
             z = [el[2][2] for el in ex]
             ax.plot3D(x, y, z, '-', lw=5)
 
-    def simulate_powder(self, energy_kev=None, peak_width=0.01, background=0, powder_average=True):
+    def simulate_powder(self, scattering_type=None, units=None, peak_width=None, background=None, pixels=None,
+                        powder_average=None, lorentz_fraction=None, custom_peak=None, min_overlap=None, **options):
+        """
+        Generates array of intensities along a spaced grid, equivalent to a powder pattern.
+          tth, inten, reflections = Scatter.powder('xray', units='tth', energy_kev=8)
+
+        Note: This function is the new replacement for generate_power and uses both _scattering_min_twotheta
+        and _scattering_max_twotheta.
+
+        :param scattering_type: str : one of ['xray','neutron','xray magnetic','neutron magnetic','xray resonant']
+        :param units: str : one of ['tth', 'dspace', 'q']
+        :param peak_width: float : Peak with in units of inverse wavevector (Q)
+        :param background: float : if >0, a normal background around this value will be added
+        :param pixels: int : number of pixels per inverse-anstrom to add to the resulting mesh
+        :param powder_average: Bool : if True, intensities will be reduced for the powder average
+        :param lorentz_fraction: float 0-1: sets the Lorentzian fraction of the psuedo-Voight peak functions
+        :param custom_peak: array: if not None, the array will be convolved with delta-functions at each reflection.
+        :param min_overlap: minimum overlap of neighboring reflections.
+        :param options: additional arguments to pass to intensity calculation
+        :return xval: arrray : x-axis of powder scan (units)
+        :return inten: array :  intensity values at each point in x-axis
+        :return reflections: (h, k, l, xval, intensity) array of reflection positions, grouped by min_overlap
+        """
+        xval, mesh, reflections = self.xtl.Scatter.powder(
+            scattering_type=scattering_type,
+            units=units,
+            peak_width=peak_width,
+            background=background,
+            pixels=pixels,
+            powder_average=powder_average,
+            lorentz_fraction=lorentz_fraction,
+            custom_peak=custom_peak,
+            min_overlap=min_overlap,
+            **options
+        )
+        energy_kev = self.xtl.Scatter.get_energy(**options)
+        wavelength_a = fc.energy2wave(energy_kev)
+        # Scattering type
+        if scattering_type is None:
+            scattering_type = self.xtl.Scatter._scattering_type
+        # X Label
+        if units is None:
+            units = self.xtl.Scatter._powder_units
+        if units.lower() in ['tth', 'angle', 'two-theta', 'twotheta', 'theta']:
+            xlab = u'Two-Theta [Deg]'
+        elif units.lower() in ['d', 'dspace', 'd-spacing', 'dspacing']:
+            xlab = u'd-spacing [\u00C5]'
+        else:
+            xlab = u'Q [\u00C5$^{-1}]$'
+
+        plt.figure(figsize=[2*self._figure_size[0], self._figure_size[1]], dpi=self._figure_dpi)
+        plt.plot(xval, mesh, label=self.xtl.name)
+        for h, k, l, x, y in reflections:
+            if x < xval.min() or x > xval.max():
+                continue
+            if y > mesh.min() + 1:
+                # reflection
+                plt.text(x, y, fc.hkl2str((h, k, l)), c='k')
+            else:
+                # extinction
+                plt.text(x, y + 1, fc.hkl2str((h, k, l)), c='r')
+        ylab = u'Intensity [a. u.]'
+        ttl = u'%s\n%s \u03BB = %1.3f \u00C5' % (self.xtl.name, scattering_type.capitalize(), wavelength_a)
+        fp.labels(ttl, xlab, ylab)
+
+    def simulate_powder_old(self, energy_kev=None, peak_width=0.01, background=0, powder_average=True):
         """
         Generates a powder pattern, plots in a new figure with labels
             see classes_scattering.generate_powder
         """
 
         if energy_kev is None:
             energy_kev = self.xtl.Scatter._energy_kev
@@ -384,16 +451,18 @@
         ext_y = background + 0.01 * plt.ylim()[1]
         for n in range(len(ext_n)):
             plt.text(mesh_x[ext_n[n]], ext_y, ext_txt[n],
                      fontname=fp.DEFAULT_FONT, fontsize=18, color='r',
                      rotation='vertical', ha='center', va='bottom')
         
         # Plot labels
+        wavelength_a = fc.energy2wave(energy_kev)
+        scattering = self.xtl.Scatter._scattering_type
         ylab = u'Intensity [a. u.]'
-        ttl = '%s\nE = %1.3f keV' % (self.xtl.name, energy_kev)
+        ttl = u'%s\n%s \u03BB = %1.3f \u00C5' % (self.xtl.name, scattering.capitalize(), wavelength_a)
         fp.labels(ttl, xlab, ylab)
 
     def axis_reciprocal_lattice_points(self, axes=None, x_axis=(1, 0, 0), y_axis=(0, 1, 0), centre=(0, 0, 0),
                                        q_max=4.0, cut_width=0.05, **kwargs):
         """
         Add lines to the current axis showing the reciprocal lattice
         :param axes: None for plt.gca() or axis of choice
@@ -506,79 +575,79 @@
         cen_lab = '(%1.3g,%1.3g,%1.3g)' % (centre[0], centre[1], centre[2])
         vec_a_lab = '(%1.3g,%1.3g,%1.3g)' % (vec_a[0] + centre[0], vec_a[1] + centre[1], vec_a[2] + centre[2])
         vec_b_lab = '(%1.3g,%1.3g,%1.3g)' % (vec_b[0] + centre[0], vec_b[1] + centre[1], vec_b[2] + centre[2])
 
         fp.plot_vector_arrows(mesh_vec_a, mesh_vec_b, vec_a_lab, vec_b_lab, axis=axes)
         plt.text(0 - (0.2 * q_max), 0 - (0.1 * q_max), cen_lab, fontname=fp.DEFAULT_FONT, weight='bold', size=18)
 
-    def generate_intensity_cut(self,x_axis=[1,0,0],y_axis=[0,1,0],centre=[0,0,0],
-                                    q_max=4.0,cut_width=0.05,background=0.0, peak_width=0.05):
-        """
-        Generate a cut through reciprocal space, returns an array with centred reflections
-        Inputs:
-          x_axis = direction along x, in units of the reciprocal lattice (hkl)
-          y_axis = direction along y, in units of the reciprocal lattice (hkl)
-          centre = centre of the plot, in units of the reciprocal lattice (hkl)
-          q_max = maximum distance to plot to - in A-1
-          cut_width = width in height that will be included, in A-1
-          background = average background value
-          peak_width = reflection width in A-1
-        Returns:
-          Qx/Qy = [1000x1000] array of coordinates
-          plane = [1000x1000] array of plane in reciprocal space 
-        
-        E.G. hk plane at L=3 for hexagonal system:
-            Qx,Qy,plane = xtl.generate_intensity_cut([1,0,0],[0,1,0],[0,0,3])
-            plt.figure()
-            plt.pcolormesh(Qx,Qy,plane)
-            plt.axis('image')
-        """
-
-        qx, qy, hkl = self.xtl.Cell.reciprocal_space_plane(x_axis, y_axis, centre, q_max, cut_width)
-        
-        # Calculate intensities
-        inten = self.xtl.Scatter.intensity(hkl)
-        
-        # create plotting mesh
-        pixels = 1001  # reduce this to make convolution faster
-        pixel_size = (2.0*q_max)/pixels
-        mesh = np.zeros([pixels, pixels])
-        mesh_x = np.linspace(-q_max, q_max, pixels)
-        xx, yy = np.meshgrid(mesh_x,mesh_x)
-
-        if peak_width is None or peak_width < pixel_size:
-            peak_width = pixel_size / 2
-
-        for n in range(len(inten)):
-            # Add each reflection as a gaussian
-            mesh += inten[n] * np.exp(-np.log(2) * (((xx - qx[n]) ** 2 + (yy - qy[n]) ** 2) / (peak_width / 2) ** 2))
+    # def generate_intensity_cut(self,x_axis=[1,0,0],y_axis=[0,1,0],centre=[0,0,0],
+    #                                 q_max=4.0,cut_width=0.05,background=0.0, peak_width=0.05):
+    #     """
+    #     Generate a cut through reciprocal space, returns an array with centred reflections
+    #     Inputs:
+    #       x_axis = direction along x, in units of the reciprocal lattice (hkl)
+    #       y_axis = direction along y, in units of the reciprocal lattice (hkl)
+    #       centre = centre of the plot, in units of the reciprocal lattice (hkl)
+    #       q_max = maximum distance to plot to - in A-1
+    #       cut_width = width in height that will be included, in A-1
+    #       background = average background value
+    #       peak_width = reflection width in A-1
+    #     Returns:
+    #       Qx/Qy = [1000x1000] array of coordinates
+    #       plane = [1000x1000] array of plane in reciprocal space
+    #
+    #     E.G. hk plane at L=3 for hexagonal system:
+    #         Qx,Qy,plane = xtl.generate_intensity_cut([1,0,0],[0,1,0],[0,0,3])
+    #         plt.figure()
+    #         plt.pcolormesh(Qx,Qy,plane)
+    #         plt.axis('image')
+    #     """
+    #
+    #     qx, qy, hkl = self.xtl.Cell.reciprocal_space_plane(x_axis, y_axis, centre, q_max, cut_width)
+    #
+    #     # Calculate intensities
+    #     inten = self.xtl.Scatter.intensity(hkl)
+    #
+    #     # create plotting mesh
+    #     pixels = 1001  # reduce this to make convolution faster
+    #     pixel_size = (2.0*q_max)/pixels
+    #     mesh = np.zeros([pixels, pixels])
+    #     mesh_x = np.linspace(-q_max, q_max, pixels)
+    #     xx, yy = np.meshgrid(mesh_x,mesh_x)
+    #
+    #     if peak_width is None or peak_width < pixel_size:
+    #         peak_width = pixel_size / 2
+    #
+    #     for n in range(len(inten)):
+    #         # Add each reflection as a gaussian
+    #         mesh += inten[n] * np.exp(-np.log(2) * (((xx - qx[n]) ** 2 + (yy - qy[n]) ** 2) / (peak_width / 2) ** 2))
+    #
+    #     """ old style using convolve2d, fast but occasional import problems, plus positions slightly inaccurate
+    #     # add reflections to background
+    #     pixel_i = ((Qx/(2*q_max) + 0.5)*pixels).astype(int)
+    #     pixel_j = ((Qy/(2*q_max) + 0.5)*pixels).astype(int)
+    #
+    #     mesh[pixel_j,pixel_i] = I
+    #
+    #     # Convolve with a gaussian (if not None or 0)
+    #     if peak_width:
+    #         peak_width_pixels = peak_width/pixel_size
+    #         gauss_x = np.arange(-2*peak_width_pixels,2*peak_width_pixels+1)
+    #         G = fg.gauss(gauss_x, gauss_x, height=1, cen=0, fwhm=peak_width_pixels, bkg=0)
+    #         mesh = convolve2d(mesh,G, mode='same') # this is the slowest part
+    #     """
+    #     # Add background (if not None or 0)
+    #     if background:
+    #         bkg = np.random.normal(background, np.sqrt(background), [pixels, pixels])
+    #         mesh = mesh+bkg
+    #
+    #     return xx, yy, mesh
 
-        """ old style using convolve2d, fast but occasional import problems, plus positions slightly inaccurate
-        # add reflections to background
-        pixel_i = ((Qx/(2*q_max) + 0.5)*pixels).astype(int)
-        pixel_j = ((Qy/(2*q_max) + 0.5)*pixels).astype(int)
-        
-        mesh[pixel_j,pixel_i] = I
-        
-        # Convolve with a gaussian (if not None or 0)
-        if peak_width:
-            peak_width_pixels = peak_width/pixel_size
-            gauss_x = np.arange(-2*peak_width_pixels,2*peak_width_pixels+1)
-            G = fg.gauss(gauss_x, gauss_x, height=1, cen=0, fwhm=peak_width_pixels, bkg=0)
-            mesh = convolve2d(mesh,G, mode='same') # this is the slowest part
-        """
-        # Add background (if not None or 0)
-        if background:
-            bkg = np.random.normal(background, np.sqrt(background), [pixels, pixels])
-            mesh = mesh+bkg
-        
-        return xx, yy, mesh
-    
-    def simulate_intensity_cut(self,x_axis=[1,0,0],y_axis=[0,1,0],centre=[0,0,0],
-                                    q_max=4.0,cut_width=0.05,background=0.0, peak_width=0.05):
+    def simulate_intensity_cut(self, x_axis=(1, 0, 0), y_axis=(0, 1, 0), centre=(0, 0, 0),
+                               q_max=4.0, cut_width=0.05, background=0.0, peak_width=0.05):
         """
         Plot a cut through reciprocal space, visualising the intensity
           x_axis = direction along x, in units of the reciprocal lattice (hkl)
           y_axis = direction along y, in units of the reciprocal lattice (hkl)
           centre = centre of the plot, in units of the reciprocal lattice (hkl)
           q_max = maximum distance to plot to - in A-1
           cut_width = width in height that will be included, in A-1
@@ -604,15 +673,17 @@
         
         # Determine orthogonal lattice vectors for plotting lines and labels
         vec_a = x_axis
         vec_c = np.cross(x_axis, y_axis)
         vec_b = fg.norm(np.cross(vec_c, vec_a))
         
         # Generate intensity cut
-        X, Y, mesh = self.generate_intensity_cut(x_axis, y_axis, centre, q_max, cut_width, background, peak_width)
+        X, Y, mesh = self.xtl.Scatter.generate_intensity_cut(
+            x_axis, y_axis, centre, q_max, cut_width, background, peak_width
+        )
         
         # create figure
         plt.figure(figsize=self._figure_size, dpi=self._figure_dpi)
         cmap = plt.get_cmap('hot_r')
         plt.pcolormesh(X, Y, mesh, cmap=cmap, shading='auto')
         plt.axis('image')
         plt.colorbar()
@@ -637,16 +708,16 @@
         fp.plot_vector_arrows(mesh_vec_a, mesh_vec_b, vec_a_lab, vec_b_lab)
         #fp.plot_vector_lines(Q_vec_a, Q_vec_b)
         #fp.plot_vector_arrows(Q_vec_a, Q_vec_b, vec_a_lab, vec_b_lab)
         plt.text(0 - (0.2*q_max), 0 - (0.1*q_max), cen_lab, fontname=fp.DEFAULT_FONT, weight='bold', size=18)
         
         # Plot labels
         scatter_type = self.xtl.Scatter._scattering_type.capitalize()
-        xlab = u'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (x_axis[0], x_axis[1], x_axis[2])
-        ylab = u'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (y_axis[0], y_axis[1], y_axis[2])
+        xlab = r'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (x_axis[0], x_axis[1], x_axis[2])
+        ylab = r'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (y_axis[0], y_axis[1], y_axis[2])
         ttl = '%s %s\n(%1.3g,%1.3g,%1.3g)' % (self.xtl.name, scatter_type, centre[0], centre[1], centre[2])
         fp.labels(ttl, xlab, ylab)
     
     def simulate_hk0(self, L=0, **kwargs):
         """
         Plots the hk(L) layer of reciprocal space
          for inputs, see help(xtl.simulate_intensity_cut)
@@ -669,15 +740,84 @@
     
     def simulate_hhl(self, HmH=0, **kwargs):
         """
         Plots the hhl layer of reciprocal space
          for inputs, see help(xtl.simulate_intensity_cut)
         """
         self.simulate_intensity_cut([1,1,0], [0,0,1], [HmH,-HmH,0],**kwargs)
-    
+
+    def simulate_envelope_cut(self, x_axis=(1, 0, 0), y_axis=(0, 1, 0), centre=(0, 0, 0),
+                              q_max=4.0, background=0.0, pixels=301):
+        """
+        *In Development*
+        Simulate enveloping function by calculating the structure factor on a discrete set of points on a grid
+
+        :param x_axis: direction along x, in units of the reciprocal lattice (hkl)
+        :param y_axis: direction along y, in units of the reciprocal lattice (hkl)
+        :param centre: centre of the plot, in units of the reciprocal lattice (hkl)
+        :param q_max: maximum distance to plot to - in A-1
+        :param background: width in height that will be included, in A-1
+        :param pixels: size of mesh, calculates structure factor at each pixel
+        :return:
+        """
+        # Determine the directions in cartesian space
+        x_cart = fg.norm(self.xtl.Cell.calculateQ(x_axis))
+        y_cart = fg.norm(self.xtl.Cell.calculateQ(y_axis))
+        z_cart = fg.norm(np.cross(x_cart, y_cart))  # z is perp. to x+y
+        y_cart = np.cross(x_cart, z_cart)  # make sure y is perp. to x
+        c_cart = self.xtl.Cell.calculateQ(centre)
+
+        # Correct y-axis for label - original may not have been perp. to x_axis (e.g. hexagonal)
+        y_axis = fg.norm(self.xtl.Cell.indexQ(y_cart))
+        y_axis = -y_axis / np.min(np.abs(y_axis[np.abs(y_axis) > 0])) + 0.0  # +0.0 to remove -0
+
+        # Determine orthogonal lattice vectors for plotting lines and labels
+        vec_a = x_axis
+        vec_c = np.cross(x_axis, y_axis)
+        vec_b = fg.norm(np.cross(vec_c, vec_a))
+
+        # Generate intensity cut
+        X, Y, mesh = self.xtl.Scatter.generate_envelope_cut(x_axis, y_axis, centre, q_max, background, pixels)
+
+        # create figure
+        plt.figure(figsize=self._figure_size, dpi=self._figure_dpi)
+        cmap = plt.get_cmap('hot_r')
+        plt.pcolormesh(X, Y, mesh, cmap=cmap, shading='auto')
+        plt.axis('image')
+        plt.colorbar()
+        plt.clim([background - (np.max(mesh) / 200), background + (np.max(mesh) / 5)])
+
+        # Lattice points and vectors within the plot
+        Q_vec_a = self.xtl.Cell.calculateQ(vec_a)
+        Q_vec_b = self.xtl.Cell.calculateQ(vec_b)
+
+        CELL = np.array([2 * q_max * x_cart, -2 * q_max * y_cart, z_cart])  # Plot/mesh unit cell
+
+        mesh_vec_a = fg.index_coordinates(Q_vec_a, CELL) * 2 * q_max  # coordinates wrt plot axes
+        mesh_vec_b = fg.index_coordinates(Q_vec_b, CELL) * 2 * q_max
+
+        # Vector arrows and lattice point labels
+        cen_lab = '(%1.3g,%1.3g,%1.3g)' % (centre[0], centre[1], centre[2])
+        vec_a_lab = '(%1.3g,%1.3g,%1.3g)' % (vec_a[0] + centre[0], vec_a[1] + centre[1], vec_a[2] + centre[2])
+        vec_b_lab = '(%1.3g,%1.3g,%1.3g)' % (vec_b[0] + centre[0], vec_b[1] + centre[1], vec_b[2] + centre[2])
+
+        lattQ = fp.axis_lattice_points(mesh_vec_a, mesh_vec_b, plt.axis())
+        fp.plot_lattice_lines(lattQ, mesh_vec_a, mesh_vec_b)
+        fp.plot_vector_arrows(mesh_vec_a, mesh_vec_b, vec_a_lab, vec_b_lab)
+        # fp.plot_vector_lines(Q_vec_a, Q_vec_b)
+        # fp.plot_vector_arrows(Q_vec_a, Q_vec_b, vec_a_lab, vec_b_lab)
+        plt.text(0 - (0.2 * q_max), 0 - (0.1 * q_max), cen_lab, fontname=fp.DEFAULT_FONT, weight='bold', size=18)
+
+        # Plot labels
+        scatter_type = self.xtl.Scatter._scattering_type.capitalize()
+        xlab = r'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (x_axis[0], x_axis[1], x_axis[2])
+        ylab = r'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (y_axis[0], y_axis[1], y_axis[2])
+        ttl = '%s %s\n(%1.3g,%1.3g,%1.3g)' % (self.xtl.name, scatter_type, centre[0], centre[1], centre[2])
+        fp.labels(ttl, xlab, ylab)
+
     def simulate_ewald_coverage(self,energy_kev=8.0,sample_normal=[0,0,1],sample_para=[1,0,0],phi=0,chi=0,**kwargs):
         """
         NOT FINISHED
         Plot ewald space coverage within a particular scattering plane
           energy_kev = energy of incident radiation in keV
           sample_normal = direction of scattering plane perp to beam direction
           sample_para = direction of scattering plane || to beam direction
@@ -862,16 +1002,16 @@
             plt.scatter(mesh_Q[n,0],mesh_Q[n,1],s=50*np.log10(I[n]+1))
         
         plt.axis('image')
         plt.axis([-q_max,q_max,-q_max,q_max])
         
         
         # Plot labels
-        xlab = u'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (x_axis[0],x_axis[1],x_axis[2])
-        ylab = u'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (y_axis[0],y_axis[1],y_axis[2])
+        xlab = r'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (x_axis[0],x_axis[1],x_axis[2])
+        ylab = r'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (y_axis[0],y_axis[1],y_axis[2])
         ttl = '%s\n(%1.3g,%1.3g,%1.3g)' % (self.xtl.name,centre[0],centre[1],centre[2])
         fp.labels(ttl,xlab,ylab)
 
     def plot_xray_resonance(self, hkl, energy_kev=None, width=1.0, npoints=200):
         """
         Plot energy scan using x-ray dispersion corrections
         :param hkl: list of [h,k,l] reflections
@@ -904,21 +1044,21 @@
         if energy_kev is None:
             energy_kev = self.xtl.Scatter._energy_kev
         
         psi = np.arange(-180,180,0.2)
         IXR=self.xtl.Scatter.xray_resonant(hkl, energy_kev, polarisation,F0=F0,F1=F1,F2=F2,azim_zero=azim_zero,PSI=psi)
         
         if polarisation == 'ss':
-            pol = '$\sigma$-$\sigma$'
+            pol = r'$\sigma$-$\sigma$'
         elif polarisation == 'sp':
-            pol = '$\sigma$-$\pi$'
+            pol = r'$\sigma$-$\pi$'
         elif polarisation == 'ps':
-            pol = '$\pi$-$\sigma$'
+            pol = r'$\pi$-$\sigma$'
         elif polarisation == 'pp':
-            pol = '$\pi$-$\pi$'
+            pol = r'$\pi$-$\pi$'
         
         ttl = '%s %5.3f keV %s\n(%1.0f,%1.0f,%1.0f) aziref=(%1.0f,%1.0f,%1.0f)'
         ttl = ttl % (self.xtl.name,energy_kev,pol,hkl[0],hkl[1],hkl[2],azim_zero[0],azim_zero[1],azim_zero[2])
         
         plt.figure(figsize=self._figure_size, dpi=self._figure_dpi)
         plt.plot(psi,IXR.T,'-',lw=2)
         plt.xlim([-180,180])
@@ -951,15 +1091,15 @@
         ttl = '%s %5.3f keV\n(%1.0f,%1.0f,%1.0f) aziref=(%1.0f,%1.0f,%1.0f) %s'
         ttl = ttl % (self.xtl.name, energy_kev, hkl[0], hkl[1], hkl[2], azim_zero[0], azim_zero[1], azim_zero[2], polarisation)
 
         plt.figure(figsize=self._figure_size, dpi=self._figure_dpi)
         plt.plot(azi, I, '-', lw=2)
         plt.xlim([-180, 180])
         plt.ylim([0, 1.1 * np.max(I)])
-        fp.labels(ttl, '$\Psi$ [Deg]', 'Resonant Magnetic Intensity')
+        fp.labels(ttl, r'$\Psi$ [Deg]', 'Resonant Magnetic Intensity')
 
     def simulate_azimuth_nonresonant(self, hkl, energy_kev=None, polarisation='sp', azim_zero=[1, 0, 0]):
         """
         Simulate azimuthal scan of resonant x-ray scattering
             energy_kev = x-ray energy in keV
             polarisation = x-ray polarisation: 'ss',{'sp'},'ps','pp'
             F0/1/2 = Resonance factor Flm
@@ -983,15 +1123,15 @@
         ttl = ttl % (
         self.xtl.name, energy_kev, hkl[0], hkl[1], hkl[2], azim_zero[0], azim_zero[1], azim_zero[2], polarisation)
 
         plt.figure(figsize=self._figure_size, dpi=self._figure_dpi)
         plt.plot(azi, I, '-', lw=2)
         plt.xlim([-180, 180])
         plt.ylim([0, 1.1 * np.max(I)])
-        fp.labels(ttl, '$\Psi$ [Deg]', 'Non-Resonant Magnetic Intensity')
+        fp.labels(ttl, r'$\Psi$ [Deg]', 'Non-Resonant Magnetic Intensity')
 
     def simulate_polarisation_resonant(self, hkl, energy_kev=None, F0=1, F1=1, F2=1, azim_zero=[1, 0, 0], psi=0):
         """
         Simulate azimuthal scan of resonant x-ray scattering
             energy_kev = x-ray energy in keV
             polarisation = x-ray polarisation: 'ss',{'sp'},'ps','pp'
             F0/1/2 = Resonance factor Flm
@@ -1196,15 +1336,15 @@
             plt.yscale('log')
         ttl = 'Multiple Scattering %s\n' % self.xtl.name
         ttl += 'Calculation: %s, E = %5.3f keV\n' % (calcstr, energy_kev)
         ttl += 'hkl = %s Incident polarisation vector = %s' % (hkl, str(pv))
         fp.labels(ttl, r'$\psi$ (deg)', 'Intensity')
         #plt.subplots_adjust(bottom=0.2)
 
-    ''' Remove tensor_scattering 26/05/20
+    r''' Remove tensor_scattering 26/05/20
     def tensor_scattering_azimuth(self, atom_label, hkl, energy_kev, azir=[0, 0, 1], process='E1E1',
                                   rank=2, time=+1, parity=+1, mk=None, lk=None, sk=None):
         """
         Plot tensor scattering intensities
           ss, sp, ps, pp = tensor_scattering('Ru1', [0,0,3], 2.838, [0,1,0], psideg=90)
         Uses TensorScatteringClass.py by Prof. Steve Collins, Dimaond Light Source Ltd.
         :param atom_label: str atom site label, e.g. Ru1
@@ -1284,33 +1424,39 @@
     generate_intensity_cut & simulate_intensity_cut
      - Refelctions are symmetrised by the parent symmetry, accounting for multiple superlattice domains
      - Generated plots have lines and vectors associated with parent structure
      - Effects functions such as xtl.Plot.simulate_hk0()
     """
 
     _intensity_cut_parent_symmetry = True  # if True, symmetrises the cuts using the parent symmetry
-    
-    def generate_intensity_cut(self,x_axis=[1,0,0], y_axis=[0,1,0], centre=[0,0,0],
-                                    q_max=4.0, cut_width=0.05, background=0.0, peak_width=0.05):
+
+    def use_parent_symmetry(self, val=None):
+        """Set the parent symmetry flag, if True, symmetrises intensity cuts using parent symmetry"""
+        if val is None:
+            return self._intensity_cut_parent_symmetry
+        self._intensity_cut_parent_symmetry = val
+
+    def parent_generate_intensity_cut(self, x_axis=(1, 0, 0), y_axis=(0, 1, 0), centre=(0, 0, 0),
+                                      q_max=4.0, cut_width=0.05, background=0.0, peak_width=0.05, pixels=1001):
         """
         Generate a cut through reciprocal space, returns an array with centred reflections
         Inputs:
           x_axis = direction along x, in units of the parent reciprocal lattice (hkl)
           y_axis = direction along y, in units of the parent reciprocal lattice (hkl)
           centre = centre of the plot, in units of the parent reciprocal lattice (hkl)
           q_max = maximum distance to plot to - in A-1
           cut_width = width in height that will be included, in A-1
           background = average background value
           peak_width = reflection width in A-1
         Returns:
-          qx/qy = [1000x1000] array of coordinates
-          plane = [1000x1000] array of plane in reciprocal space 
+          qx/qy = [pixels x pixels] array of coordinates
+          plane = [pixels x pixels] array of plane in reciprocal space
         
         E.G. hk plane at L=3 for hexagonal system:
-            qx,qy,plane = xtl.generate_intensity_cut([1,0,0],[0,1,0],[0,0,3])
+            qx,qy,plane = xtl.Plot.parent_generate_intensity_cut([1,0,0],[0,1,0],[0,0,3])
             plt.figure()
             plt.pcolormesh(qx,qy,plane)
             plt.axis('image')
         """
 
         # Check q_max
         c_cart = self.xtl.Parent.Cell.calculateQ(centre)
@@ -1337,15 +1483,15 @@
             phkl = self.xtl.superhkl2parent(hkl)
             symhkl = self.xtl.Parent.Symmetry.symmetric_reflections_unique(phkl)
             symQ = self.xtl.Parent.Cell.calculateQ(symhkl)
 
             box_coord = fg.index_coordinates(symQ - c_cart, CELL)
             if np.any(np.all(np.abs(box_coord) <= 0.5, axis=1)):
                 HKLinbox += [hkl]
-        print('Number of non-symmetric reflections in box: %1.0f'%len(HKLinbox))
+        print('Number of non-symmetric reflections in box: %1.0f' % len(HKLinbox))
 
         # Calculate intensity
         inten = self.xtl.Scatter.intensity(HKLinbox)
 
         # Apply Parent symmetry
         if self._intensity_cut_parent_symmetry:
             pHKL = self.xtl.superhkl2parent(HKLinbox)
@@ -1359,26 +1505,42 @@
         incell = np.all(np.abs(box_coord) <= 0.5, axis=1)
         plane_coord = 2 * q_max * box_coord[incell, :]
         qx = plane_coord[:, 0]
         qy = plane_coord[:, 1]
         inten = inten[incell]
 
         # create plotting mesh
-        pixels = 1001  # reduce this to make convolution faster
         pixel_size = (2.0 * q_max) / pixels
         mesh = np.zeros([pixels, pixels])
         mesh_x = np.linspace(-q_max, q_max, pixels)
         xx, yy = np.meshgrid(mesh_x, mesh_x)
 
         if peak_width is None or peak_width < pixel_size:
             peak_width = pixel_size / 2
 
+        # Add Gaussian profile to each peak
+        KS = 3  # kernel size in units of peak width
+        kernel_size = int(2 * KS * peak_width * pixels / (2 * q_max))
+        kernel_size = kernel_size + 1 if kernel_size % 2 == 1 else kernel_size  # kernel_size must be even
+        hks = kernel_size // 2
+        kernel_x = np.linspace(-KS * peak_width, KS * peak_width, kernel_size)
+        kxx, kyy = np.meshgrid(kernel_x, kernel_x)
+        kernel = np.exp(-np.log(2) * ((kxx ** 2 + kyy ** 2) / (peak_width / 2) ** 2))
         for n in range(len(inten)):
-            # Add each reflection as a gaussian
-            mesh += inten[n] * np.exp(-np.log(2) * (((xx - qx[n]) ** 2 + (yy - qy[n]) ** 2) / (peak_width / 2) ** 2))
+            ix = np.nanargmin(np.abs(mesh_x - qy[n]))  # I need to switch qx,qy here for some reason
+            iy = np.nanargmin(np.abs(mesh_x - qx[n]))  # must be a flip somewhere
+            ix_min = 0 if ix < hks else ix - hks
+            ix_max = pixels if ix > (pixels - hks) else ix + hks
+            iy_min = 0 if iy < hks else iy - hks
+            iy_max = pixels if iy > (pixels - hks) else iy + hks
+            ikx_min = -(ix - hks) if ix < hks else 0
+            ikx_max = hks + pixels - ix if ix > (pixels - hks) else kernel_size
+            iky_min = -(iy - hks) if iy < hks else 0
+            iky_max = hks + pixels - iy if iy > (pixels - hks) else kernel_size
+            mesh[ix_min:ix_max, iy_min:iy_max] += inten[n] * kernel[ikx_min:ikx_max, iky_min:iky_max]
 
         """ Old method using convolve2d
         # add reflections to background
         pixel_i = ((qx/(2*q_max) + 0.5)*pixels).astype(int)
         pixel_j = ((qy/(2*q_max) + 0.5)*pixels).astype(int)
         
         # Only take values within the mesh
@@ -1398,18 +1560,20 @@
         """
         # Add background (if not None or 0)
         if background:
             bkg = np.random.normal(background,np.sqrt(background), [pixels, pixels])
             mesh = mesh+bkg
         return xx, yy, mesh
     
-    def simulate_intensity_cut(self,x_axis=[1,0,0],y_axis=[0,1,0],centre=[0,0,0],
-                                    q_max=4.0,cut_width=0.05,background=0.0, peak_width=0.05):
+    def simulate_intensity_cut(self, x_axis=(1, 0, 0), y_axis=(0, 1, 0), centre=(0, 0, 0),
+                               q_max=4.0, cut_width=0.05, background=0.0, peak_width=0.05):
         """
         Plot a cut through reciprocal space, visualising the intensity
+        This method, as part of a superstructure, overloads simulate_intensity_cut,
+        providing orientation of parent and symmetrisation of parent.
           x_axis = direction along x, in units of the parent reciprocal lattice (hkl)
           y_axis = direction along y, in units of the parent reciprocal lattice (hkl)
           centre = centre of the plot, in units of the parent reciprocal lattice (hkl)
           q_max = maximum distance to plot to - in A-1
           cut_width = width in height that will be included, in A-1
           background = average background value
           peak_width = reflection width in A-1
@@ -1434,16 +1598,16 @@
         vec_b = fg.norm(np.cross(vec_c, vec_a))
 
         # Determine the supercell axes
         super_x_axis = self.xtl.parenthkl2super(x_axis)
         super_y_axis = self.xtl.parenthkl2super(y_axis)
 
         # Generate intensity cut
-        X, Y, mesh = self.generate_intensity_cut(super_x_axis, super_y_axis, centre, q_max, cut_width, background,
-                                                 peak_width)
+        X, Y, mesh = self.parent_generate_intensity_cut(super_x_axis, super_y_axis, centre, q_max, cut_width,
+                                                        background, peak_width)
 
         # create figure
         plt.figure(figsize=self._figure_size, dpi=self._figure_dpi)
         cmap = plt.get_cmap('hot_r')
         plt.pcolormesh(X, Y, mesh, cmap=cmap)
         plt.axis('image')
         plt.colorbar()
@@ -1465,16 +1629,16 @@
 
         lattQ = fp.axis_lattice_points(mesh_vec_a, mesh_vec_b, plt.axis())
         fp.plot_lattice_lines(lattQ, mesh_vec_a, mesh_vec_b, lw=0.5, c='grey')
         fp.plot_vector_arrows(mesh_vec_a, mesh_vec_b, vec_a_lab, vec_b_lab)
         plt.text(0 - (0.2 * q_max), 0 - (0.1 * q_max), cen_lab, fontname=fp.DEFAULT_FONT, weight='bold', size=18)
 
         # Plot labels
-        xlab = u'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (x_axis[0], x_axis[1], x_axis[2])
-        ylab = u'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (y_axis[0], y_axis[1], y_axis[2])
+        xlab = r'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (x_axis[0], x_axis[1], x_axis[2])
+        ylab = r'Q || (%1.3g,%1.3g,%1.3g) [$\AA^{-1}$]' % (y_axis[0], y_axis[1], y_axis[2])
         supercentre = self.xtl.parenthkl2super(centre)[0]
         ttl = '%s\n(%1.3g,%1.3g,%1.3g)$_{p}$ = (%1.3g,%1.3g,%1.3g)$_{s}$' \
               % (self.xtl.name, centre[0], centre[1], centre[2], supercentre[0], supercentre[1], supercentre[2])
         fp.labels(ttl, xlab, ylab)
 
 
 class MultiPlotting:
@@ -1483,15 +1647,15 @@
     """
     _figure_size = fp.FIGURE_SIZE
     _figure_dpi = fp.FIGURE_DPI
 
     def __init__(self, crystal_list):
         self.crystal_list = crystal_list
 
-    def simulate_powder(self, energy_kev=8.0, peak_width=0.05, background=0, powder_average=True):
+    def simulate_powder(self, energy_kev=8.0, peak_width=0.01, background=0, powder_average=True):
         """
         Generates a powder pattern for multiple phases
             see classes_scattering.generate_powder
         """
         
         plt.figure(figsize=[2*self._figure_size[0], self._figure_size[1]], dpi=self._figure_dpi)
         colours = iter(['b','g','r','c','m','y','k'])
@@ -1552,15 +1716,16 @@
             ref_n = fc.group_intensities(xvalues, I, min_overlap)
 
             grp_hkl = HKL[ref_n, :]
             grp_xval = xvalues[ref_n]
             grp_inten = mesh[pixel_coord[ref_n]]
 
             # create figure
-            plt.plot(xval, mesh, '-', lw=2, label=xtl.name, c=col)
+            lab = '%s: %s' % (xtl.Scatter._scattering_type.capitalize(), xtl.name)
+            plt.plot(xval, mesh, '-', lw=2, label=lab, c=col)
 
             # Reflection labels
             for n in range(len(grp_hkl)):
                 if grp_inten[n] > 1.01 * background:
                     plt.text(grp_xval[n], 1.01 * grp_inten[n], fc.hkl2str(grp_hkl[n]),
                              fontname=fp.DEFAULT_FONT, fontsize=12, color=col, fontweight='bold',
                              rotation='vertical', ha='center', va='bottom')
@@ -1568,17 +1733,17 @@
                     plt.text(grp_xval[n], (1.01 * background) + 1, fc.hkl2str(grp_hkl[n]),
                              fontname=fp.DEFAULT_FONT, fontsize=12, color=col, fontweight='bold',
                              rotation='vertical', ha='center', va='bottom')
 
         if xtl.Scatter._powder_units.lower() in ['tth', 'angle', 'two-theta', 'twotheta', 'theta']:
             xlab = u'Two-Theta [Deg]'
         elif xtl.Scatter._powder_units.lower() in ['d', 'dspace', 'd-spacing', 'dspacing']:
-            xlab = u'd-spacing [$\AA$]'
+            xlab = r'd-spacing [$\AA$]'
         else:
-            xlab = u'Q [$\AA^{-1}]$'
+            xlab = r'Q [$\AA^{-1}]$'
 
         ylab = u'Intensity [a. u.]'
         ttl = 'E = %1.3f keV' % energy_kev
         plt.legend(loc=0, fontsize=18, frameon=False)
         fp.labels(ttl, xlab, ylab)
     
     def simulate_intensity_cut(self,x_axis_crystal=[[1,0,0]],y_axis_crystal=[[0,1,0]],centre=[0,0,0],
@@ -1700,16 +1865,16 @@
         # Update plot
         # a very odd bug noted by lumbric:
         # https://stackoverflow.com/questions/18797175/animation-with-pcolormesh-routine-in-matplotlib-how-do-i-initialize-the-data
         mesh = mesh[:-1, :-1]
         pp.set_array(mesh.ravel())
 
         # Plot labels
-        xlab = u'Qx [$\AA^{-1}$]'
-        ylab = u'Qy [$\AA^{-1}$]'
+        xlab = r'Qx [$\AA^{-1}$]'
+        ylab = r'Qy [$\AA^{-1}$]'
         # ttl = '%s\n(%1.3g,%1.3g,%1.3g)' % (self.name,centre[0],centre[1],centre[2])
         fp.labels(None, xlab, ylab)
     
     def quick_intensity_cut(self,x_axis_crystal=[[1,0,0]],y_axis_crystal=[[0,1,0]],centre=[0,0,0], q_max=4.0,cut_width=0.05):
         """
         Plot a cut through reciprocal space, visualising the intensity as different sized markers
           x_axis = direction along x, in units of the reciprocal lattice (hkl)
@@ -1795,12 +1960,12 @@
             legend_entries += [pt]
             
             # Plot reflections as circles using logged intensity as the radius
             for n in range(len(I)):
                 plt.scatter(mesh_Q[n,0],mesh_Q[n,1],s=50*np.log10(I[n]+1),c=col)
         
         # Plot labels
-        xlab = u'Qx [$\AA^{-1}$]'
-        ylab = u'Qy [$\AA^{-1}$]'
+        xlab = r'Qx [$\AA^{-1}$]'
+        ylab = r'Qy [$\AA^{-1}$]'
         fp.labels(None,xlab,ylab)
         names = [xtl.name for xtl in self.crystal_list]
         plt.legend(legend_entries,names,frameon=True,fontsize=16)
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/classes_scattering.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_scattering.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Scattering Class "classes_scattering.py"
     Scattering functions for Crystal class.
 
 By Dan Porter, PhD
 Diamond
 2017
 
-Version 2.3.0
-Last updated: 02/07/23
+Version 2.3.4
+Last updated: 17/05/24
 
 Version History:
 10/09/17 0.1    Program created
 30/10/17 1.0    Main functions finshed, some testing done
 06/01/18 1.1    Renamed classes_scattering.py
 31/10/18 1.2    Added print_symmetric_contributions
 21/01/19 1.3    Added non-resonant diffraction, corrected resonant diffraction
@@ -29,29 +29,35 @@
 20/08/21 2.0    Switched over to new scattering module, added self.powder()
 28/09/21 2.0.1  Added __repr__
 08/02/22 2.0.3  Corrected error in powder of wrong tth values. Thanks Mirko!
 14/03/22 2.1.0   powder() updated for new inputs and outputs for pVoight and custom peak shapes. Thanks yevgenyr!
 14/01/23 2.1.1  Corrected background error in xtl.Scatter.powder
 06/05/23 2.0.0  Merged pull request for non-integer hkl option on SF and electron form factors. Thanks Prestipino!
 02/07/23 2.3.0  Fixed rounding error in Scatter.powder, thanks Sergio I. Rincon!
+26/09/23 2.3.1  Added Scattering.orientation_reflections for automatic orientation help
+19/20/23 2.3.2  Fixed scatteringbasis so xray_resonant() now works with non-cubic systems
+28/03/24 2.3.3  Fixed scattering type comparison to compare .lower() scattering types
+02/05/24 2.3.4  added min_twotheta to get_hkl, added generate_envelope_cut, fixed low tth error in powder()
+15/05/24 2.3.4  Added "save" and "load" methods to structure factor calculation, improved powder for large calculations
+16/05/24 2.3.4  Added printed progress bar to generate_intensity_cut during convolusion
+17/05/24 2.3.4  Changed generate_intensity_cut to make it much faster
 
 @author: DGPorter
 """
 
-import sys,os
 import numpy as np
 import datetime
 
 from . import functions_general as fg
 from . import functions_crystallography as fc
 from . import functions_scattering as fs
 from . import multiple_scattering as ms
 # from . import tensor_scattering as ts  # Removed V1.7
 
-__version__ = '2.3.0'
+__version__ = '2.3.4'
 __scattering_types__ = {'xray': ['xray', 'x', 'x-ray', 'thomson', 'charge'],
                         'neutron': ['neutron', 'n', 'nuclear'],
                         'xray magnetic': ['xray magnetic', 'magnetic xray', 'spin xray', 'xray spin'],
                         'neutron magnetic': ['neutron magnetic', 'magnetic neutron', 'magnetic'],
                         'xray resonant': ['xray resonant', 'resonant', 'resonant xray', 'rxs'],
                         'xray dispersion': ['dispersion', 'xray dispersion']}
 
@@ -69,26 +75,26 @@
             'xray','neutron','xray magnetic','neutron magnetic','xray resonant'
     """
     
     #------Options-------
     # Standard Options
     _hkl = None  # added so recalculation not required
     _scattering_type = 'xray'  # 'xray','neutron','xray magnetic','neutron magnetic','xray resonant'
-    _scattering_specular_direction = [0,0,1]  # reflection
-    _scattering_parallel_direction = [0,0,1]  # transmission
+    _scattering_specular_direction = [0, 0, 1]  # reflection
+    _scattering_parallel_direction = [0, 0, 1]  # transmission
     _scattering_theta_offset = 0.0
     _scattering_min_theta = -180.0
     _scattering_max_theta = 180.0
     _scattering_min_twotheta = -180.0
     _scattering_max_twotheta = 180.0
     _time_report = True
     _debug_mode = False
 
     # powder options
-    _powder_units = 'tth' # tth (two theta), Q, d
+    _powder_units = 'tth'  # tth (two theta), Q, d
     _powder_background = 0.0
     _powder_peak_width = 0.01  # in Deg
     _powder_lorentz_fraction = 0.5
     _powder_average = True
     _powder_pixels = 2000  # no. pixels per inverse angstrom (in q)
     _powder_min_overlap = 0.02
     
@@ -308,27 +314,31 @@
         max_tth = self._scattering_max_twotheta
 
         hkl = self.xtl.Cell.all_hkl(en, max_tth)
         if remove_symmetric:
             hkl = self.xtl.Symmetry.remove_symmetric_reflections(hkl)
         hkl = self.xtl.Cell.sort_hkl(hkl)[1:]  # remove (0, 0, 0)
 
+        tth = self.xtl.Cell.tth(hkl, en)
+        hkl = hkl[tth > self._scattering_min_twotheta, :]
+        tth = tth[tth > self._scattering_min_twotheta]
+
         if reflection:
-            tth = self.xtl.Cell.tth(hkl, en)
-            hkl = hkl[tth > self._scattering_min_twotheta, :]
-            tth = tth[tth > self._scattering_min_twotheta]
+            # tth = self.xtl.Cell.tth(hkl, en)
+            # hkl = hkl[tth > self._scattering_min_twotheta, :]
+            # tth = tth[tth > self._scattering_min_twotheta]
             theta = self.xtl.Cell.theta_reflection(hkl, en, self._scattering_specular_direction,
                                                    self._scattering_theta_offset)
             p1 = (theta > self._scattering_min_theta) * (theta < self._scattering_max_theta)
             p2 = (tth > (theta + self._scattering_min_theta)) * (tth < (theta + self._scattering_max_theta))
             hkl = hkl[p1 * p2]
         elif transmission:
-            tth = self.xtl.Cell.tth(hkl, en)
-            hkl = hkl[tth > self._scattering_min_twotheta, :]
-            tth = tth[tth > self._scattering_min_twotheta]
+            # tth = self.xtl.Cell.tth(hkl, en)
+            # hkl = hkl[tth > self._scattering_min_twotheta, :]
+            # tth = tth[tth > self._scattering_min_twotheta]
             theta = self.xtl.Cell.theta_transmission(hkl, en, self._scattering_parallel_direction)
 
             p1 = (theta > self._scattering_min_theta) * (theta < self._scattering_max_theta)
             p2 = (tth > (theta + self._scattering_min_theta)) * (tth < (theta + self._scattering_max_theta))
             hkl = hkl[p1 * p2]
         self._hkl = hkl
         return self._hkl
@@ -352,25 +362,31 @@
         - This may be a little slow for large numbers of reflections, as it is not currently
          possible to use accelerated calculation methods in Jython.
         - Debye-Waller factor (atomic displacement) is applied for isotropic ADPs
         - Crystal.scale is used to scale the complex structure factor, so the intensity is
          reduced by (Crystal.scale)^2
         - Testing against structure factors calculated by Vesta.exe is exactly the same when using Waasmaier structure factors.
 
+        Save/Load behaviour
+            structure_factor(..., save='sf.npy')  # saves structure factors after calculation in compressed file
+            structure_factor(..., load='sf.npy')  # loads structure factors if sf.npy, rather than calculating
+              - if the number of values in load doesn't match the number of hkl indices, an Exception is raised
+
         :param hkl: array[n,3] : reflection indexes (h, k, l)
         :param scattering_type: str : one of ['xray','neutron','xray magnetic','neutron magnetic','xray resonant']
         :param int_hkl: Bool : when True, hkl values are converted to integer.
         :param kwargs: additional options to pass to scattering function
         :return: complex array[n] : structure factors
         """
 
         if hkl is None:
             hkl = self.get_hkl()
         if scattering_type is None:
             scattering_type = self._scattering_type
+        # scattering_type = scattering_type.lower()
         if int_hkl:
             hkl = np.asarray(np.rint(hkl), dtype=float).reshape([-1, 3])
         else:
             hkl = np.asarray(hkl, dtype=float).reshape([-1, 3])
         uvw, atom_type, label, occ, uiso, mxmymz = self.xtl.Structure.get()
 
         q = self.xtl.Cell.calculateQ(hkl)
@@ -405,26 +421,44 @@
             f1=self._resonant_flm[1],
             f2=self._resonant_flm[2],
         )
         options.update(kwargs)
         scattering_fun = fs.get_scattering_function(scattering_type)
         # print('Scattering function: %s' % scattering_fun.__name__)
 
+        if 'load' in kwargs:
+            # Load SF from file
+            sf = np.load(kwargs['load'])
+            if sf.shape[0] != len(hkl):
+                raise Exception(
+                    "File '%s' with %d structure factors doesn't match %d reflections" % (
+                        kwargs['load'], sf.shape[0], len(hkl))
+                )
+            return sf
+
         # Break up long lists of HKLs
         nref, natom = len(q), len(r)
+        if nref == 0:
+            if nenergy == 1 and npsi == 1:
+                return np.empty([0], dtype=complex)  # shape(nref)
+            if nenergy == 1:
+                return np.empty([0, nenergy], dtype=complex)  # shape(nref)  # shape(nref, nenergy)
+            if npsi == 1:
+                return np.empty([0, npsi], dtype=complex)  # shape(nref)  # shape(nref, npsi)
+            return np.empty([0, nenergy, npsi], dtype=complex)
         n_arrays = np.ceil(nref * natom / fs.MAX_QR_ARRAY)
         if n_arrays > 1:
             print('Splitting %d reflections (%d atoms) into %1.0f parts' % (nref, natom, n_arrays))
         q_array = np.array_split(q, n_arrays)
         sf = np.zeros([nref, nenergy, npsi], dtype=complex)
         start_time = datetime.datetime.now()
-        for e, enval in enumerate(energy_kev): # for all the energy values
+        for e, enval in enumerate(energy_kev):  # for all the energy values
             for p, psival in enumerate(psi):   # for all azimutal angle
                 ls = 0
-                for n, _q in enumerate(q_array): # for all the reflections parts
+                for n, _q in enumerate(q_array):  # for all the reflections parts
                     if n_arrays > 1:
                         print(' Starting %2.0f/%2.0f: %d:%d' % (n + 1, n_arrays, ls, ls + len(_q)))
                     qmag = fg.mag(_q)      # q magnitude
                     # Scattering factors
                     if scattering_type in fs.SCATTERING_TYPES['neutron']:
                         ff = fc.atom_properties(atom_type, 'Coh_b')
                     elif scattering_type in fs.SCATTERING_TYPES['electron']:
@@ -463,19 +497,22 @@
 
         end_time = datetime.datetime.now()
         time_difference = end_time - start_time
         if self._time_report and time_difference.total_seconds() > 10:
             print('Calculated %d structure factors in %s' % (nref, time_difference))
         sf = sf / self.xtl.scale
         if nenergy == 1 and npsi == 1:
-            return sf[:, 0, 0]  # shape(nref)
-        if nenergy == 1:
-            return sf[:, 0, :]  # shape(nref, nenergy)
-        if npsi == 1:
-            return sf[:, :, 0]  # shape(nref, nspi)
+            sf = sf[:, 0, 0]  # shape(nref)
+        elif nenergy == 1:
+            sf = sf[:, 0, :]  # shape(nref, nenergy)
+        elif npsi == 1:
+            sf = sf[:, :, 0]  # shape(nref, npsi)
+        if 'save' in kwargs:
+            np.save(kwargs['save'], sf, allow_pickle=True)
+            print("Saved %d structure factors to '%s'" % (sf.size, kwargs['save']))
         return sf
     new_structure_factor = structure_factor
 
     def intensity(self, hkl=None, scattering_type=None, int_hkl=True, **options):
         """
         Return the structure factor squared
         :param hkl: array[n,3] : reflection indexes (h, k, l)
@@ -524,36 +561,43 @@
             powder_average = self._powder_average
         if lorentz_fraction is None:
             lorentz_fraction = self._powder_lorentz_fraction
         if min_overlap is None:
             min_overlap = self._powder_min_overlap
         energy_kev = self.get_energy(**options)
 
+        # Extend range to account for peak widths beyond range
+        ext = 3  # int, multiples of the peak_width used
+
         # Units
         min_twotheta = self._scattering_min_twotheta
-        if min_twotheta <= 0: min_twotheta = 1.0
+        if min_twotheta <= 1.0: min_twotheta = 1.0
         max_twotheta = self._scattering_max_twotheta
-        q_min = fc.calqmag(min_twotheta, energy_kev)
-        q_max = fc.calqmag(max_twotheta, energy_kev)
+        if max_twotheta >= 179: max_twotheta = 179
+        q_min = fc.calqmag(min_twotheta, energy_kev) - ext * peak_width
+        q_max = fc.calqmag(max_twotheta, energy_kev) + ext * peak_width
+        if q_min <= 0: q_min = 0.0
+        if q_max >= fc.calqmag(179, energy_kev): q_max = fc.calqmag(179, energy_kev)
         q_range = q_max - q_min
 
-        # Get reflections
-        HKL = self.xtl.Cell.all_hkl(maxq=q_max)
-        HKL = self.xtl.Cell.sort_hkl(HKL)  # required for labels
-        Qmag = self.xtl.Cell.Qmag(HKL)
-
         # create plotting mesh
         tot_pixels = int(pixels * q_range)  # reduce this to make convolution faster
-        pixel_size = q_range / float(tot_pixels)
-        peak_width_pixels = peak_width / pixel_size
+        pixel_size = q_range / float(tot_pixels)  # units of A-1
+        peak_width_pixels = int(np.round(peak_width / pixel_size))  # peak_width is in A-1
         mesh = np.zeros([tot_pixels])
         mesh_q = np.linspace(q_min, q_max, tot_pixels)
-        pixel_coord = np.round(tot_pixels * (Qmag - q_min) / q_range).astype(int)
 
-        select = (pixel_coord < tot_pixels) * (pixel_coord > 0)
+        # Get reflections
+        HKL = self.xtl.Cell.all_hkl(maxq=q_max + pixel_size)
+        HKL = self.xtl.Cell.sort_hkl(HKL)  # required for labels
+        Qmag = self.xtl.Cell.Qmag(HKL)
+
+        # remove reflections not within the calculation
+        pixel_coord = np.round(tot_pixels * (Qmag - q_min) / q_range).astype(int)
+        select = (pixel_coord < tot_pixels) * (pixel_coord >= 0)
         HKL = HKL[select, :]
         Qmag = Qmag[select]
         pixel_coord = pixel_coord[select]
 
         # Calculate intensities
         I = self.intensity(HKL, scattering_type, **options)
 
@@ -585,16 +629,188 @@
         xvalues = fc.q2units(Qmag, units, energy_kev)
         ref_n = fc.group_intensities(xvalues, I, min_overlap)
 
         grp_hkl = HKL[ref_n, :]
         grp_xval = xvalues[ref_n]
         grp_inten = mesh[pixel_coord[ref_n]]
         reflections = np.transpose([grp_hkl[:, 0], grp_hkl[:, 1], grp_hkl[:, 2], grp_xval, grp_inten])
+
+        # Remove extended part
+        ixmin = np.nanargmin(np.abs(xval - fc.q2units(fc.calqmag(min_twotheta, energy_kev), units, energy_kev)))
+        ixmax = np.nanargmin(np.abs(xval - fc.q2units(fc.calqmag(max_twotheta, energy_kev), units, energy_kev)))
+        # mesh = mesh[ext * peak_width_pixels:-ext * peak_width_pixels - 1]
+        # xval = xval[ext * peak_width_pixels:-ext * peak_width_pixels - 1]
+        mesh = mesh[ixmin:ixmax]
+        xval = xval[ixmin:ixmax]
         return xval, mesh, reflections
 
+    def generate_intensity_cut(self, x_axis=(1, 0, 0), y_axis=(0, 1, 0), centre=(0, 0, 0),
+                               q_max=4.0, cut_width=0.05, background=0.0, peak_width=0.05, pixels=1001):
+        """
+        Generate a cut through reciprocal space, returns an array with centred reflections
+        Inputs:
+          x_axis = direction along x, in units of the reciprocal lattice (hkl)
+          y_axis = direction along y, in units of the reciprocal lattice (hkl)
+          centre = centre of the plot, in units of the reciprocal lattice (hkl)
+          q_max = maximum distance to plot to - in A-1
+          cut_width = width in height that will be included, in A-1
+          background = average background value
+          peak_width = reflection width in A-1
+          pixels = size of the plotting mesh
+        Returns:
+          Qx/Qy = [pixels x pixels] array of coordinates
+          plane = [pixels x pixels] array of plane in reciprocal space
+
+        E.G. hk plane at L=3 for hexagonal system:
+            Qx,Qy,plane = xtl.Scatter.generate_intensity_cut([1,0,0],[0,1,0],[0,0,3])
+            plt.figure()
+            plt.pcolormesh(Qx,Qy,plane)
+            plt.axis('image')
+        """
+        qx, qy, hkl = self.xtl.Cell.reciprocal_space_plane(x_axis, y_axis, centre, q_max, cut_width)
+
+        # Calculate intensities
+        inten = self.xtl.Scatter.intensity(hkl)
+
+        # create plotting mesh
+        pixel_size = (2.0 * q_max) / pixels
+        mesh = np.zeros([pixels, pixels])
+        mesh_x = np.linspace(-q_max, q_max, pixels)
+        xx, yy = np.meshgrid(mesh_x, mesh_x)
+
+        if peak_width is None or peak_width < pixel_size:
+            peak_width = pixel_size / 2
+
+        # Add Gaussian profile to each peak
+        KS = 3  # kernel size in units of peak width
+        kernel_size = int(2 * KS * peak_width * pixels / (2 * q_max))
+        kernel_size = kernel_size + 1 if kernel_size % 2 == 1 else kernel_size  # kernel_size must be even
+        hks = kernel_size // 2
+        kernel_x = np.linspace(-KS * peak_width, KS * peak_width, kernel_size)
+        kxx, kyy = np.meshgrid(kernel_x, kernel_x)
+        kernel = np.exp(-np.log(2) * ((kxx ** 2 + kyy ** 2) / (peak_width / 2) ** 2))
+        for n in range(len(inten)):
+            ix = np.nanargmin(np.abs(mesh_x - qy[n]))  # I need to switch qx,qy here for some reason
+            iy = np.nanargmin(np.abs(mesh_x - qx[n]))  # must be a flip somewhere
+            ix_min = 0 if ix < hks else ix - hks
+            ix_max = pixels if ix > (pixels - hks) else ix + hks
+            iy_min = 0 if iy < hks else iy - hks
+            iy_max = pixels if iy > (pixels - hks) else iy + hks
+            ikx_min = -(ix - hks) if ix < hks else 0
+            ikx_max = hks + pixels - ix if ix > (pixels - hks) else kernel_size
+            iky_min = -(iy - hks) if iy < hks else 0
+            iky_max = hks + pixels - iy if iy > (pixels - hks) else kernel_size
+            mesh[ix_min:ix_max, iy_min:iy_max] += inten[n] * kernel[ikx_min:ikx_max, iky_min:iky_max]
+
+        # Add background (if not None or 0)
+        if background:
+            bkg = np.random.normal(background, np.sqrt(background), [pixels, pixels])
+            mesh = mesh + bkg
+        return xx, yy, mesh
+
+    def generate_intensity_cut_old(self, x_axis=(1, 0, 0), y_axis=(0, 1, 0), centre=(0, 0, 0),
+                                   q_max=4.0, cut_width=0.05, background=0.0, peak_width=0.05, pixels=1001):
+        """
+        Generate a cut through reciprocal space, returns an array with centred reflections
+          **Old version - creates full Gaussian for each peak, very slow**
+        Inputs:
+          x_axis = direction along x, in units of the reciprocal lattice (hkl)
+          y_axis = direction along y, in units of the reciprocal lattice (hkl)
+          centre = centre of the plot, in units of the reciprocal lattice (hkl)
+          q_max = maximum distance to plot to - in A-1
+          cut_width = width in height that will be included, in A-1
+          background = average background value
+          peak_width = reflection width in A-1
+        Returns:
+          Qx/Qy = [1000x1000] array of coordinates
+          plane = [1000x1000] array of plane in reciprocal space
+
+        E.G. hk plane at L=3 for hexagonal system:
+            Qx,Qy,plane = xtl.generate_intensity_cut([1,0,0],[0,1,0],[0,0,3])
+            plt.figure()
+            plt.pcolormesh(Qx,Qy,plane)
+            plt.axis('image')
+        """
+        qx, qy, hkl = self.xtl.Cell.reciprocal_space_plane(x_axis, y_axis, centre, q_max, cut_width)
+
+        # Calculate intensities
+        inten = self.xtl.Scatter.intensity(hkl)
+
+        # create plotting mesh
+        pixel_size = (2.0 * q_max) / pixels
+        mesh = np.zeros([pixels, pixels])
+        mesh_x = np.linspace(-q_max, q_max, pixels)
+        xx, yy = np.meshgrid(mesh_x, mesh_x)
+
+        if peak_width is None or peak_width < pixel_size:
+            peak_width = pixel_size / 2
+
+        start_time = datetime.datetime.now()
+        print('Convolving with 2D Gaussian: |' + 50 * '-' + '|', end='\r', flush=True)
+        for n in range(len(inten)):
+            # Add each reflection as a gaussian - this is very slow!
+            mesh += inten[n] * np.exp(-np.log(2) * (((xx - qx[n]) ** 2 + (yy - qy[n]) ** 2) / (peak_width / 2) ** 2))
+            if n % (len(inten)/50) < 1:
+                _done = int(n // (len(inten)/50))
+                print('Convolving with 2D Gaussian: |' + (_done * '█') + (50-_done) * '-' + '|', end='\r', flush=True)
+        print('Convolving with 2D Gaussian: |' + 50 * '█' + '|', end='\n', flush=True)
+        end_time = datetime.datetime.now()
+        time_difference = end_time - start_time
+        print('Time taken for %d reflections: %s' % (len(inten), time_difference))
+
+        # Add background (if not None or 0)
+        if background:
+            bkg = np.random.normal(background, np.sqrt(background), [pixels, pixels])
+            mesh = mesh + bkg
+        return xx, yy, mesh
+
+    def generate_envelope_cut(self, x_axis=(1, 0, 0), y_axis=(0, 1, 0), centre=(0, 0, 0),
+                              q_max=4.0, background=0.0, pixels=301):
+        """
+        *In Development*
+        Generate the envelope function, calculating the structure factor at discrete points
+        Inputs:
+          x_axis = direction along x, in units of the reciprocal lattice (hkl)
+          y_axis = direction along y, in units of the reciprocal lattice (hkl)
+          centre = centre of the plot, in units of the reciprocal lattice (hkl)
+          q_max = maximum distance to plot to - in A-1
+          background = average background value
+          pixels = size of mesh, calculates structure factor at each pixel
+        Returns:
+          Qx/Qy = [pixels x pixels] array of coordinates
+          plane = [pixels x pixels] array of plane in reciprocal space
+
+        E.G. hk plane at L=3 for hexagonal system:
+            Qx, Qy, plane = xtl.generate_envelope_cut([1,0,0],[0,1,0],[0,0,3])
+            plt.figure()
+            plt.pcolormesh(Qx, Qy, plane)
+            plt.axis('image')
+        """
+        x_cart = self.xtl.Cell.calculateQ(x_axis)
+        y_cart = self.xtl.Cell.calculateQ(y_axis)
+        x_cart, y_cart, z_cart = fc.orthogonal_axes(x_cart, y_cart)
+        c_cart = self.xtl.Cell.calculateQ(centre)
+
+        xx, yy = np.meshgrid(range(pixels), range(pixels))
+        q_range = np.linspace(-q_max, q_max, pixels)
+        qx, qy = q_range[xx], q_range[yy]  # [pixels, pixels]
+        qxqy = np.transpose([qx.reshape(-1), qy.reshape(-1)])  # returns [qx, qy]
+        qxqyz = np.dot(qxqy, [x_cart, y_cart])  # returns [qx,qy,qz]
+        hkl = self.xtl.Cell.indexQ(qxqyz + c_cart)
+
+        # Calculate intensities
+        inten = self.intensity(hkl, int_hkl=False)
+        mesh = inten.reshape([pixels, pixels])
+
+        # Add background (if not None or 0)
+        if background:
+            bkg = np.random.normal(background, np.sqrt(background), [pixels, pixels])
+            mesh = mesh + bkg
+        return qx, qy, mesh
+
     def x_ray(self, HKL):
         """
         Calculate the squared structure factor for the given HKL, using x-ray scattering factors
           Scattering.x_ray([1,0,0])
           Scattering.x_ray([[1,0,0],[2,0,0],[3,0,0])
         Returns an array with the same length as HKL, giving the real intensity at each reflection.
         """
@@ -1278,22 +1494,31 @@
             out_eout[n, :] = eout
 
         return out_kin, out_kout, out_ein, out_eout
 
     def scatteringcomponents(self, mxmymz, hkl, azim_zero=[1,0,0], psi=0):
         """
         Transform magnetic vector into components within the scattering plane
-            ***warning - may not be correct for non-cubic systems***
+        First transforms the moments into a cartesian reference frame.
+           U1 = direction || ki - kf = Q
+           U2 = direction || kf + ki (within scattering plane, pi)
+           U3 = direction perp. to U1, U2 (normal to scattering plane, sigma)
         """
 
         # Define coordinate system I,J,Q (U1,U2,U3)
         U = self.scatteringbasis(hkl, azim_zero, psi)
+
+        # Calculate moment
+        momentmag = fg.mag(mxmymz).reshape([-1, 1])
+        momentxyz = self.xtl.Cell.calculateR(mxmymz)  # moment direction in cartesian reference frame
+        moment = momentmag * fg.norm(momentxyz)  # broadcast n*1 x n*3 = n*3
+        moment[np.isnan(moment)] = 0.
         
         # Determine components of the magnetic vector
-        z1z2z3 = np.dot(mxmymz, U.T) # [mxmymz.I, mxmymz.J, mxmymz.Q]
+        z1z2z3 = np.dot(moment, U.T)  # [mxmymz.I, mxmymz.J, mxmymz.Q]
         return fg.norm(z1z2z3)
 
     def scatteringbasis(self, hkl, azim_zero=[1, 0, 0], psi=0):
         """
         Determine the scattering and polarisation vectors of a reflection based on energy, azimuth and polarisation.
         :param hkl: [n,3] array of reflections
         :param azim_zero: [1,3] direction along which the azimuthal zero angle is determind
@@ -1849,15 +2074,15 @@
             # if not print_symmetric and np.abs(tth[n]-tth[n-1]) < 0.01: continue # only works if sorted
             count += 1
             outstr += fmt % (HKL[n, 0], HKL[n, 1], HKL[n, 2], tth[n], theta[n], inten[n])
         outstr += 'Reflections: %1.0f\n' % count
         return outstr
     
     def print_tran_reflections(self, energy_kev=None, min_intensity=0.01, max_intensity=None):
-        """
+        r"""
         Prints a list of all allowed reflections at this energy in the transmission geometry
             energy = energy in keV
             min_intensity = None/ 0.01 : omits reflections less than this (remove extinctions)
             max_intensity = None/ 0.01 : omits reflections greater than this (show extinctions only)
                    \ /      
              --<-- || --<-- 
                   / \       
@@ -2091,15 +2316,59 @@
                     tot_sf += sf[n, a]
                 ss += '%74sTotal:  %s  %s\n' % (' ', fg.complex2str(tot_phase), fg.complex2str(tot_sf))
                 all_phase += tot_phase
                 all_sf += tot_sf
             ss += '%62s Reflection Total:  %s  %s\n' % (' ', fg.complex2str(all_phase), fg.complex2str(all_sf))
             outstr += '(%2.0f,%2.0f,%2.0f) I = %9.2f    %s\n' % (HKL[n, 0], HKL[n, 1], HKL[n, 2], I[n], ss)
         return outstr
-    
+
+    def orientation_reflections(self, energy_kev, hkl_1=None):
+        """
+        Return 2 reflections to use to orient a crystal
+         1. a strong reflection that is easy to discriminate in 2-theta
+         2. another strong reflection non-parallel and non-normal to (1)
+
+        hkl_1, hkl_2, alternatives = xtl.Scatter.orientation_reflections(8)
+
+        :param energy_kev: photon energy in keV
+        :param hkl_1: None or [h,k,l], allows to specify the first reflection
+        :returns hkl_1: [h,k,l] indices of reflection 1
+        :returns hkl_2: [h,k,l] indices of reflection 2
+        :returns hkl_2_alternatives: [[h,k,l],...] list of alternative reflections with same angles
+        """
+        # Reflection 1 seletor
+        if hkl_1 is None:
+            refs = self.get_hkl(energy_kev=energy_kev, remove_symmetric=True)
+            ref_tth = self.xtl.Cell.tth(refs, energy_kev=energy_kev)
+            ref_multiplicity = self.xtl.Symmetry.reflection_multiplyer(refs)
+            ref_intensity = self.intensity(refs)
+            ref_cluster = np.array([np.sum(1 / (np.abs(th - ref_tth) + 1)) - 1 for th in ref_tth])
+            ref_select = ref_intensity * ref_multiplicity / ref_cluster  # ** 2
+            hkl_1 = refs[np.argmax(ref_select), :]
+
+        # Reflection 2 selector
+        next_refs = self.get_hkl(energy_kev=energy_kev, remove_symmetric=False)
+        # tth_1 = self.xtl.Cell.tth(hkl_1, energy_kev=energy_kev)
+        # tth_2 = self.xtl.Cell.tth(refs, energy_kev=energy_kev)
+        q_1 = self.xtl.Cell.calculateQ(hkl_1)
+        q_2 = self.xtl.Cell.calculateQ(next_refs)
+        angles = abs(fg.vectors_angle_degrees(q_1, q_2))
+        ref_select = (angles > 1.) * (angles < 40.)
+        if sum(ref_select) < 1:
+            ref_select = angles > 1.
+        next_refs = next_refs[ref_select]
+        angles = angles[ref_select]
+        tth_1 = self.xtl.Cell.tth(hkl_1, energy_kev=energy_kev)
+        tth_2 = self.xtl.Cell.tth(next_refs, energy_kev=energy_kev)
+        next_select = self.intensity(next_refs) / angles
+        idx = np.argmax(next_select)
+        hkl_2 = next_refs[idx]
+        hkl_2_options = (abs(angles - angles[idx]) < 1.) * (abs(tth_2 - tth_2[idx]) < 1.)
+        return hkl_1, hkl_2, next_refs[hkl_2_options]
+
     def find_close_reflections(self,HKL,energy_kev=None,max_twotheta=2,max_angle=10):
         """
         Find and print list of reflections close to the given one
         """
         
         if energy_kev is None:
             energy_kev = self._energy_kev
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/classes_structures.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_structures.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,85 +2,105 @@
 CIF Directory
 Various standard structures to load into Dans_Diffraction.
 
 Usage:
     from classes_structures import Structures
     structure_list = Structures() # builds database of all cif files in Structures Directory
     xtl = structure_list.Silicon() # builds Crystal class of selected structure
+    all_xts = [xtl for xtl in structure_list]
 
 By Dan Porter, PhD
 Diamond
 2018
 
-Version 1.1
-Last updated: 07/08/19
+Version 1.2
+Last updated: 18/08/23
 
 Version History:
 02/03/18 1.0    Program created
-07/08/19 1.1    Added _call__ and __repr__ methods
+07/08/19 1.1    Added __call__ and __repr__ methods
+18/08/23 1.2    Added __getitem__ to Structures class
 
 @author: DGPorter
 """
 
 import sys, os, glob
 import numpy as np
 from . import Crystal
 
-__version__ = '1.1'
+__version__ = '1.2'
 
 
 def cif_list():
     """"Returns a list of cif files in the current directory"""
     current_dir = os.path.dirname(__file__)
-    structure_dir = os.path.join(current_dir,'Structures','*cif')
+    structure_dir = os.path.join(current_dir, 'Structures', '*cif')
     cif_files = glob.glob(structure_dir)
     cif_files = np.sort(cif_files)
     return cif_files
 
 
 class Structures:
     """
     Provides a database of cif files
         S = Structures() # builds database
         xtl = S.Diamond.build()
         
         Use S.list to see the available structures
+        Use S.cif_files to see filenames of structures
+
+        Iterating over all structures:
+        for xtl in S:
+            print(xtl)
     """
     def __init__(self):
         # Read cif files in current directory
-        cif_files = cif_list()
+        self.cif_files = cif_list()
         
-        self.list=[]
-        for filename in cif_files:
+        self.list = []
+        self.builder_list = []
+        for filename in self.cif_files:
             # Generate structure name
-            (dirName,filetitle)=os.path.split(filename)
-            (fname, Ext)=os.path.splitext(filetitle)
+            (dirName, filetitle) = os.path.split(filename)
+            (fname, Ext) = os.path.splitext(filetitle)
             
             # Replace illegal characters
             for chars in '\'!$,.()[]{}':
-                fname = fname.replace(chars,'')
+                fname = fname.replace(chars, '')
             self.list += [fname]
-            
-            setattr(self, fname, BuildCrystal(filename))
+            builder = BuildCrystal(filename)
+            self.builder_list += [builder]
+            setattr(self, fname, builder)
+
+    def __str__(self):
+        out = ''
+        for s, f in zip(self.list, self.cif_files):
+            out += "%12s: %s\n" % (s, f)
+        return out
     
     def info(self):
         """"Print Available Structures"""
-        for s in self.list:
-            print(s)
+        print(self.__str__())
+
+    def __getitem__(self, item):
+        return self.builder_list[item].build()
 
 
 class BuildCrystal:
     """
     Storage Class for filename and build command
     Builds a Crystal class.
     """
-    def __init__(self,filename):
+    def __init__(self, filename):
         self.filename = filename
 
     def __repr__(self):
+        return "BuildCrystal('%s')" % self.filename
+
+    def __str__(self):
         return self.filename
 
     def __call__(self):
         return Crystal(self.filename)
     
     def build(self):
         return Crystal(self.filename)
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/Dans Element Properties.txt` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/Dans Element Properties.txt`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/Dans Element Properties_old.txt` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/Dans Element Properties_old.txt`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/Element_OxidationStates.txt` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/Element_OxidationStates.txt`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/PointGroups.json` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/PointGroups.json`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/SpaceGroups.json` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/SpaceGroups.json`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/SpaceGroupsMagnetic.json` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/SpaceGroupsMagnetic.json`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/XRayEdges.dat` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayEdges.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/XRayMassAtten_muenp.dat` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayMassAtten_muenp.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/XRayMassAtten_mup.dat` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayMassAtten_mup.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/atomic_scattering_factors.npy` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/atomic_scattering_factors.npy`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/f0_WaasKirf.dat` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/f0_WaasKirf.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/data/peng.dat` & `Dans_Diffraction-3.2.0/Dans_Diffraction/data/peng.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/functions_crystallography.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/functions_crystallography.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 2018
 
 Usage: 
     - Run this file in an interactive console
     OR
     - from Dans_Diffraction import functions_crystallography as fc
 
-Version 3.8.1
-Last updated: 22/05/23
+Version 3.8.2
+Last updated: 02/07/23
 
 Version History:
 09/07/15 0.1    Version History started.
 30/10/17 1.0    Many updates
 06/01/18 2.0    Renamed functions_crystallography.py
 02/03/18 2.1    Removed call to tkinter
 05/04/18 2.2    Added invert_sym
@@ -54,15 +54,15 @@
 import sys, os, re
 import json
 import numpy as np
 from warnings import warn
 
 from . import functions_general as fg
 
-__version__ = '3.8.1'
+__version__ = '3.8.2'
 
 # File directory - location of "Dans Element Properties.txt"
 datadir = os.path.abspath(os.path.dirname(__file__))  # same directory as this file
 datadir = os.path.join(datadir, 'data')
 ATOMFILE = os.path.join(datadir, 'Dans Element Properties.txt')
 PENGFILE = os.path.join(datadir, 'peng.dat')
 
@@ -459,15 +459,15 @@
         if label[n] in const_labels:
             # Assumes single constraint per atom
             idx = const_labels.index(label[n])
             C = constraints[idx]
             C = C.replace('m', '')
             # print('Constraint: {:3s} {:s}'.format(label[n],C))
             # convert '2x' to 'x'
-            old = re.findall('\d[xyz]', C)
+            old = re.findall(r'\d[xyz]', C)
             new = [s.replace('x', '*x').replace('y', '*y').replace('z', '*z') for s in old]
             for s in range(len(old)):
                 C = C.replace(old[s], new[s])
             C = C.split(',')
             # Apply constraint to symmetry arguments
             S = [s.replace('x', 'a').replace('y', 'b').replace('z', 'c') for s in symmag]
             S = [s.replace('a', C[0]).replace('b', C[1]).replace('c', C[2]) for s in S]
@@ -1031,15 +1031,15 @@
     :return: [m*n] array of scattering factors
     """
 
     filename = os.path.join(datadir, 'f0_WaasKirf.dat')
     data = np.loadtxt(filename)
     # get names
     with open(filename) as f:
-        lines = re.findall('#S\s+\d+\s+[A-Z].*?\n', f.read())
+        lines = re.findall(r'#S\s+\d+\s+[A-Z].*?\n', f.read())
         table_names = [line[7:].strip() for line in lines]
 
     # Qmag should be a 1D array
     Qmag = np.asarray(Qmag).reshape(-1)
     element = np.asarray(element, dtype=str).reshape(-1)
 
     # data table: a1  a2  a3  a4  a5  c  b1  b2  b3  b4  b5
@@ -1621,26 +1621,26 @@
     :return: symbol: str
     :return: occupancy: float
     :return: charge: float
     """
     # Find element
     symbol = element_regex.findall(element)[0]
     # Find charge
-    find_charge = re.findall('[\d\.]+[\+-]', element)
+    find_charge = re.findall(r'[\d\.]+[\+-]', element)
     if len(find_charge) > 0:
         chargestr = find_charge[0]
         element = element.replace(chargestr, '')
         if '-' in chargestr:
             charge = -float(chargestr[:-1])
         else:
             charge = float(chargestr[:-1])
     else:
         charge = 0.
     # Find occupancy
-    find_occ = re.findall('[\d\.]+', element)
+    find_occ = re.findall(r'[\d\.]+', element)
     if len(find_occ) > 0:
         occupancy = float(find_occ[0])
     else:
         occupancy = 1.
     return symbol, occupancy, charge
 
 
@@ -1681,15 +1681,15 @@
     Values in brackets are multiplied out.
     E.g.
         split_compound('Mn0.3(Fe3.6(Co1.2)2)4(Mo0.7Pr44)3')
         >> ['Mn0.3', 'Fe14.4', 'Co9.6', 'Mo2.1', 'Pr132']
     :param compound_name: str
     :return: list of str
     """
-    regex_element_num = re.compile('|'.join(['%s[\d\.]*' % el for el in ELEMENT_LIST]))
+    regex_element_num = re.compile('|'.join([r'%s[\d\.]*' % el for el in ELEMENT_LIST]))
     # Multiply out brackets
     compound_name = fg.replace_bracket_multiple(compound_name)
     return regex_element_num.findall(compound_name)
 
 
 def orbital_configuration(element, charge=None):
     """
@@ -2051,16 +2051,17 @@
       Elastic scattering:            |kf| = |ki|
       Therefore:          |Q + ki| - |ki| = 0
       Expanding & simplifing: Q.Q + 2Q.ki = 0
     :param Q: [[nx3]] array of reciprocal lattice coordinates, in A-1
     :param ki: [x,y,z] incident wavevector, in A-1
     :return: [nx1] array of difference, in A-1
     """
-    Q = np.reshape(Q, [-1, 3])
-    return np.array([np.dot(q, q) + 2 * np.dot(q, ki) for q in Q])
+    return np.abs(fg.mag(Q + ki) - fg.mag(ki))
+    # Q = np.reshape(Q, [-1, 3])
+    # return np.array([np.dot(q, q) + 2 * np.dot(q, ki) for q in Q])
 
 
 def latparvolume(a, b=None, c=None, alpha=90., beta=90., gamma=90.):
     """
     Calcualte the unit cell volume in A^3
     :param a, b, c: float lattice parameters
     :param alpha, beta, gamma: float lattice angles
@@ -3179,15 +3180,15 @@
 
 
 def q2units(qmag, units='tth', energy_kev=None):
     """
     Convert |Q| in A^-1 to choice of units
     :param qmag: float or array in inverse-Angstrom
     :param units: str: 'tth', 'dspace', 'q' (raises ValueError if wrong)
-    :param energy_kev: float
+    :param energy_kev: float or None
     :return: float or array
     """
     units = units.lower().replace(' ', '').replace('-', '')
     if 'q' in units:
         return qmag
     if units in ['d', 'dspace', 'dspacing', 'angstrom', 'A']:
         return q2dspace(qmag)
@@ -3206,30 +3207,32 @@
     theta = twotheta * np.pi / 360  # theta in radians
     return (fg.h * fg.c * 1e10) / (res * np.sin(theta) * fg.e * 2 * 1000.)
 
 
 def wave2energy(wavelength):
     """
     Converts wavelength in A to energy in keV
-     Energy = wave2energy(wavelength)
+     energy_kev = wave2energy(wavelength_a)
+     Energy [keV] = h*c/L = 12.3984 / lambda [A]
     """
 
     # SI: E = hc/lambda
     lam = wavelength * fg.A
     E = fg.h * fg.c / lam
 
     # Electron Volts:
     Energy = E / fg.e
     return Energy / 1000.0
 
 
 def energy2wave(energy_kev):
     """
     Converts energy in keV to wavelength in A
-     wavelength = energy2wave(energy)
+     wavelength_a = energy2wave(energy_kev)
+     lambda [A] = h*c/E = 12.3984 / E [keV]
     """
 
     # Electron Volts:
     E = 1000 * energy_kev * fg.e
 
     # SI: E = hc/lambda
     lam = fg.h * fg.c / E
@@ -3339,14 +3342,31 @@
     """
     if wavelength_a is None:
         wavelength_a = energy2wave(energy_kev)
     costheta = np.cos(np.deg2rad(twotheta / 2.))
     return np.rad2deg(shape_factor * wavelength_a / (size * costheta))
 
 
+def peakwidth_deg(domain_size_a, twotheta, wavelength_a=None, energy_kev=None, instrument_resolution=0):
+    """
+    Return the peak width in degrees for a given two-theta based on the
+    crystallite domain size and instrument resolution.
+      Equivalent to the Scherrer equation with shape factor 1.0
+    :param domain_size_a: crystallite domain size in Anstroms
+    :param twotheta: scattering angle in degrees
+    :param wavelength_a: incident beam wavelength, in Angstroms
+    :param energy_kev: or, incident beam energy, in keV
+    :param instrument_resolution: instrument resolution in inverse Anstroms
+    :return:
+    """
+    peak_width = np.sqrt(dspace2q(domain_size_a)**2 + instrument_resolution**2)
+    q = calqmag(twotheta, energy_kev, wavelength_a)
+    return cal2theta(q + peak_width, energy_kev, wavelength_a) - twotheta
+
+
 def biso2uiso(biso):
     """
     Convert B isotropic thermal parameters to U isotropic thermal parameters
     :param biso: Biso value or array
     :return: Uiso value or array
     """
     biso = np.asarray(biso, dtype=float)
@@ -3585,15 +3605,15 @@
     extra = ', '.join(extra)
 
     # Create table str
     out = '%% %s\n' % cif['Filename']
     out += '\\begin{table}[htp]\n'
     out += '    \\centering\n'
     out += '       \\begin{tabular}{c|c|ccccc}\n'
-    out += '             & Site & x & y & z & Occ. & %s \\\\ \hline\n' % u_or_b
+    out += r'             & Site & x & y & z & Occ. & %s \\\\ \hline\n' % u_or_b
     fmt = '        %4s & %5s & %s & %s & %s & %s & %s \\\\\n'
     for n in range(len(label)):
         out += fmt % (label[n], mult[n], u[n], v[n], w[n], occ[n], uiso[n])
     out += '        \\end{tabular}\n'
     out += '    \\caption{%s with %s. %s}\n' % (name, lp, extra)
     out += '    \\label{tab:}\n'
     out += '\\end{table}\n'
@@ -3720,7 +3740,272 @@
     :param intensity: intensity value
     :param wavevector_diff: distance from centre in inverse angstroms
     :param resolution: resolution in inverse angstroms
     :return:
     """
     return intensity * np.exp(-np.log(2) * (wavevector_diff / (0.5 * resolution)) ** 2)
 
+
+def wavevector_resolution(energy_range_ev=200, wavelength_range_a=None, domain_size_a=1000):
+    """
+    Calculate the combined wavevector resolutuion in inverse Angstroms
+    Combines instrument incident beam resolution and the mosaic of the crystal
+    :param energy_range_ev: Incident x-ray beam resolution in eV
+    :param wavelength_range_a: Incident beam resolution in Angstroms
+    :param domain_size_a: crysallite size in Angstroms (provides mosic using Scherrer equation)
+    :return: float, resolutuion in inverse Angstroms
+    """
+    if wavelength_range_a is None:
+        beam_resolution = wavevector(energy_kev=energy_range_ev / 1000)
+    else:
+        beam_resolution = dspace2q(wavelength_range_a)
+    sample_resolution = dspace2q(domain_size_a)
+    return np.sqrt(sample_resolution**2 + beam_resolution**2)
+
+
+def reciprocal_volume(twotheta, twotheta_min=0, energy_kev=None, wavelength_a=1.5):
+    """
+    Calculate the volume of reciprocal space covered between two scattering angles
+    :param twotheta: larger scattering angle (Bragg angle, 2theta)
+    :param twotheta_min: smaller scattering angle
+    :param energy_kev: photon energy, in keV
+    :param wavelength_a: wavelength in Angstroms
+    :return: float, volume, in Angstroms^-3
+    """
+    q1 = calqmag(twotheta_min, energy_kev, wavelength_a)
+    q2 = calqmag(twotheta, energy_kev, wavelength_a)
+    vol1 = 4 * fg.pi * q1 ** 3 / 3
+    vol2 = 4 * fg.pi * q2 ** 3 / 3
+    return vol2 - vol1
+
+
+def detector_angle_size(detector_distance_mm=565, height_mm=67, width_mm=34, pixel_size_um=172):
+    """
+    Return the angular spread of the detector
+      delta_width, gamma_width, pixel_width = detector_angle_size(distance, height, widht, pixel)
+    :param detector_distance_mm: Detector distance from sample in mm
+    :param height_mm: Detector size in the vertical direction, in mm
+    :param width_mm: Detector size in the horizontal direction, in mm
+    :param pixel_size_um: Pixel size in microns
+    :return x_angle: total angular spread in the diffractometer x-axis, in degrees
+    :return z_angle: total angular spread in the diffractometer z-axis, in degrees
+    :return pixel_angle: angular spread per pixel, in degrees
+    """
+    gam_width = 2 * np.rad2deg(np.arctan2(width_mm / 2, detector_distance_mm))
+    del_height = 2 * np.rad2deg(np.arctan2(height_mm / 2, detector_distance_mm))
+    pix_width = 2 * np.rad2deg(np.arctan2(pixel_size_um / 2, 1000 * detector_distance_mm))
+    return gam_width, del_height, pix_width
+
+
+def detector_coverage(wavelength_a=1.5, resolution=0.1, delta=0, gamma=0,
+                      detector_distance_mm=565, height_mm=67, width_mm=34):
+    """
+    Determine volume of reciprocal space covered by the detector based on angular spread
+    :param wavelength_a: Incicent beam wavelength, in Angstroms
+    :param resolution: Incident beam resolution, in inverse-Angstroms
+    :param delta: float or array, detector vertical rotation
+    :param gamma: float or array, detector horizontal rotation
+    :param detector_distance_mm: Detector distance from sample in mm
+    :param height_mm: Detector size in the vertical direction, in mm
+    :param width_mm: Detector size in the horizontal direction, in mm
+    :return: volume in inverse-Angstroms
+    """
+    gam_width = np.rad2deg(np.arctan2(width_mm / 2, detector_distance_mm))
+    del_height = np.rad2deg(np.arctan2(height_mm / 2, detector_distance_mm))
+    gam_wid_a = 2 * dspace2q(scherrer_size(gam_width, gamma, wavelength_a=wavelength_a, shape_factor=1.0))
+    del_wid_a = 2 * dspace2q(scherrer_size(del_height, delta, wavelength_a=wavelength_a, shape_factor=1.0))
+    det_wid = 2 * resolution
+    return gam_wid_a * del_wid_a * det_wid
+
+
+def detector_volume(wavelength_a=1.5, resolution=0.1,
+                    phi=0, chi=0, eta=0, mu=0, delta=0, gamma=0,
+                    detector_distance_mm=565, height_mm=67, width_mm=34, lab=np.eye(3)):
+    """
+    Determine volume of reciprocal space covered by the detector, return list of voxels covered by detector
+      total_volume, hkl = detector_volume(1.5, 0.1, chi=90, eta=30, delta=60)
+    The returned list of coordinates (hkl) is defined in the sample frame, where each coordinate specifies a voxel
+    in reciprocal space with size resolution(inverse-Anstroms) ** 3
+    As such, the total volume of reciprocal space measured is:
+        total_volume = len(hkl) * fc.wavevector(energy_kev=energy_range_ev / 1000.) ** 3
+
+    :param wavelength_a: Incicent beam wavelength, in Angstroms
+    :param resolution: Incident beam resolution, in inverse-Angstroms (determines segmentation of calculation)
+    :param phi: float, phi-axis rotation about sample-z axis
+    :param chi: float, chi-axis rotation about sample-y' axis
+    :param eta: float, eta-axis rotation about sample-z'' axis
+    :param mu: float, mu-axis rotation about sample-x''' axis
+    :param delta: float, detector rotation vertical rotation
+    :param gamma: float, detector rotation horizontal rotation
+    :param detector_distance_mm: Detector distance from sample in mm
+    :param height_mm: Detector size in the vertical direction, in mm
+    :param width_mm: Detector size in the horizontal direction, in mm
+    :param lab: [3x3] Transformation matrix to change the lab coordinate system
+    :return total_volume: float, total volume of reciprocal space in inverse Angstroms
+    :return hkl: [nx3] array of voxels covered by detector, integer coordinates in the sample frame
+    """
+    # Rotate detector
+    D = rotmatrixz(-delta)  # left handed
+    G = rotmatrixx(gamma)
+    Rdet = np.dot(G, D)
+    position_mm = detector_distance_mm * labvector([0, 1., 0], R=Rdet, LAB=lab)
+    normal_dir = labvector([0, -1, 0], R=Rdet, LAB=lab)
+    x_axis = width_mm * fg.norm(np.cross(normal_dir, (0, 0, 1.)))
+    z_axis = height_mm * fg.norm(np.cross(x_axis, normal_dir))
+    corners = np.array([
+        position_mm + x_axis / 2 + z_axis / 2,
+        position_mm + x_axis / 2 - z_axis / 2,
+        position_mm - x_axis / 2 - z_axis / 2,
+        position_mm - x_axis / 2 + z_axis / 2,
+    ])
+
+    # Create a reciprocal lattice with basis size = resolution
+    ub = resolution * np.eye(3)
+    k = wavevector(wavelength=wavelength_a)
+    ki = k * labvector([0, 1, 0], LAB=lab)  # incident beam
+
+    # Determine the lattice position at each of the detector corners to determine a rough lattice
+    gam_width = np.rad2deg(np.arctan2(width_mm / 2, detector_distance_mm))
+    del_height = np.rad2deg(np.arctan2(height_mm / 2, detector_distance_mm))
+    hkl_corners = np.array([
+        diff6circle2hkl(ub, phi, chi, eta, mu, delta=delta + del_height, gamma=gamma + gam_width,
+                        wavelength=wavelength_a, lab=lab),
+        diff6circle2hkl(ub, phi, chi, eta, mu, delta=delta - del_height, gamma=gamma + gam_width,
+                        wavelength=wavelength_a, lab=lab),
+        diff6circle2hkl(ub, phi, chi, eta, mu, delta=delta - del_height, gamma=gamma - gam_width,
+                        wavelength=wavelength_a, lab=lab),
+        diff6circle2hkl(ub, phi, chi, eta, mu, delta=delta + del_height, gamma=gamma - gam_width,
+                        wavelength=wavelength_a, lab=lab),
+    ])
+    h_range = range(int(min(hkl_corners[:, 0])) - 2, int(max(hkl_corners[:, 0])) + 2)
+    k_range = range(int(min(hkl_corners[:, 1])) - 2, int(max(hkl_corners[:, 1])) + 2)
+    l_range = range(int(min(hkl_corners[:, 2])) - 2, int(max(hkl_corners[:, 2])) + 2)
+    HH, KK, LL = np.meshgrid(h_range, k_range, l_range)
+    hkl = np.asarray([HH.ravel(), KK.ravel(), LL.ravel()]).T
+
+    # Rotate lattice
+    R = diffractometer_rotation(phi=phi, chi=chi, eta=eta, mu=mu)
+    q = labvector(resolution * hkl, R=R, LAB=lab)
+
+    # Find lattice points incident on detector
+    kf = q + ki
+    directions = fg.norm(kf)
+    # Check magnitude of kf matches ki
+    scatters = np.flatnonzero(np.abs(fg.mag(kf) - k) < resolution)
+    # check which lattice directions are in the quadrent of detector
+    corner_angle = min(np.dot(fg.norm(corners), fg.norm(position_mm)))
+    vec_angles = np.dot(directions[scatters], fg.norm(position_mm))
+    # Check with lattice point directions intercept the detector plane
+    # Only loop over lattice points with correct magnitude and in the right direction
+    check = vec_angles > corner_angle
+    iuvw = np.nan * np.zeros([len(hkl), 3])
+    for n in scatters[check]:
+        ixyz = fg.plane_intersection((0, 0, 0), directions[n], position_mm, normal_dir)
+        # incident positions on detector
+        iuvw[n] = fg.index_coordinates(np.subtract(ixyz, position_mm), [x_axis, z_axis, normal_dir])
+    iuvw[np.any(abs(iuvw) > 0.5, axis=1)] = [np.nan, np.nan, np.nan]
+
+    # Remove non-incident reflections
+    idx = ~np.isnan(iuvw[:, 0])  # iuvw same size as Q
+    tot_space = np.sum(idx)
+    tot_recspace = tot_space * resolution ** 3  # A-3
+    # print(f"Measured Reciprocal space: {tot_space:.0f} voxels, {tot_recspace: .4g} A-3")
+    return tot_recspace, hkl[idx, :]
+
+
+def detector_volume_scan(wavelength_a=1.5, resolution=0.1,
+                         phi=0, chi=0, eta=0, mu=0, delta=0, gamma=0,
+                         detector_distance_mm=565, height_mm=67, width_mm=34, lab=np.eye(3)):
+    """
+    Return total reciprocal space volume covered by scanning an axis with a detector
+      total, hkl, overlaps = detector_volume_scan(1.5, 0.1, phi=np.arange(-180,180))
+    Rotation axes can be specified as either floats or arrays, where all arrays must have the same length.
+
+    :param wavelength_a: Incicent beam wavelength, in Angstroms
+    :param resolution: Incident beam resolution, in inverse-Angstroms (determines segmentation of calculation)
+    :param phi: float or array, phi-axis about sample-z axis
+    :param chi: float or array, chi-axis about sample-y' axis
+    :param eta: float or array, eta-axis about sample-z'' axis
+    :param mu: float or array, mu-axis about sample-x''' axis
+    :param delta: float or array, detector vertical rotation
+    :param gamma: float or array, detector horizontal rotation
+    :param detector_distance_mm: Detector distance from sample in mm
+    :param height_mm: Detector size in the vertical direction, in mm
+    :param width_mm: Detector size in the horizontal direction, in mm
+    :param lab: [3x3] Transformation matrix to change the lab coordinate system
+    :return total: float, total volume covered, in cubic inverse Angstroms
+    :return hkl: [nx3] array of voxels covered by detector, integer coordinates in the sample frame
+    :return overlaps: [n] array of the number of times each voxel has been repeatedly measured (0 = only measurred once)
+    """
+    # pad the scan axes
+    scan_angles = [phi, chi, eta, mu, delta, gamma]
+    axes = np.zeros([min([np.size(s) for s in scan_angles if np.size(s) > 1]), len(scan_angles)])
+    for n in range(len(scan_angles)):
+        axes[:, n] = scan_angles[n]
+    # loop over the scan
+    hkl_list = np.empty([0, 3], dtype=int)
+    for phi, chi, eta, mu, delta, gamma in axes:
+        vol, hkl = detector_volume(wavelength_a, resolution, phi, chi, eta, mu, delta, gamma,
+                                   detector_distance_mm, height_mm, width_mm, lab)
+        hkl_list = np.vstack([hkl_list, hkl])
+    # Find the overlapping points
+    hkl, counts = np.unique(hkl_list, return_counts=True, axis=0)
+    overlaps = counts - 1
+    total = len(hkl) * resolution ** 3
+    return total, hkl, overlaps
+
+
+def diffractometer_step(wavelength_a=1.5, resolution=0.1,
+                        phi=0, chi=0, eta=0, mu=0, delta=0, gamma=0, lab=np.eye(3)):
+    """
+    Determine the euler angle steps required to scan through reciprocal space at the required resolutuion
+        phi_step, chi_step, eta_step, mu_step = diffractometer_step(1.5, 0.1, chi=90, eta=20, delta=40)
+    The returned step size will provide a rotation that moves the wavevector transfer by approximately the resolutuion.
+    Any steps returning 0 are unsensitive to the rotation in this position
+    :param wavelength_a: Incicent beam wavelength, in Angstroms
+    :param resolution: float, combined resolution required, in inverse Angstroms
+    :param phi: float, phi-axis about sample-z axis
+    :param chi: float, chi-axis about sample-y' axis
+    :param eta: float, eta-axis about sample-z'' axis
+    :param mu: float, mu-axis about sample-x''' axis
+    :param delta: float, detector vertical rotation
+    :param gamma: float, detector horizontal rotation
+    :param lab: [3x3] Transformation matrix to change the lab coordinate system
+    :returns: phi_step, chi_step, eta_step, mu_step
+    """
+    ub = resolution * np.eye(3)
+    # Determine current location of diffractometer in orthogonal basis coordinates
+    hkl = diff6circle2hkl(ub, phi=phi, chi=chi, eta=eta, mu=mu, delta=delta, gamma=gamma,
+                          wavelength=wavelength_a, lab=lab)
+    # Convert hkl back to wavevector units
+    q0 = np.dot(ub, hkl)
+    q = labvector(q0, R=diffractometer_rotation(phi=phi, chi=chi, eta=eta, mu=mu), LAB=lab)
+    # Add the resolution in various directions and determine the max angular difference
+    q2 = q + [
+        [resolution, 0, 0],
+        [0, resolution, 0],
+        [0, 0, resolution],
+        resolution * fg.norm([1, 1, 0]),
+        resolution * fg.norm([1, 0, 1]),
+        resolution * fg.norm([0, 1, 1]),
+        resolution * fg.norm([1, 1, 1]),
+    ]
+    ang = max(np.abs(fg.vectors_angle_degrees(q, q2)))
+
+    # Add this angle in each axis and check how much is moved
+    q_phi = fg.mag(q - labvector(q0, R=diffractometer_rotation(phi=phi + ang, chi=chi, eta=eta, mu=mu), LAB=lab))
+    q_chi = fg.mag(q - labvector(q0, R=diffractometer_rotation(phi=phi, chi=chi + ang, eta=eta, mu=mu), LAB=lab))
+    q_eta = fg.mag(q - labvector(q0, R=diffractometer_rotation(phi=phi, chi=chi, eta=eta + ang, mu=mu), LAB=lab))
+    q_mu = fg.mag(q - labvector(q0, R=diffractometer_rotation(phi=phi, chi=chi, eta=eta, mu=mu + ang), LAB=lab))
+
+    # Scale this movement back to the resolution
+    phi_ang = ang * resolution / q_phi
+    chi_ang = ang * resolution / q_chi
+    eta_ang = ang * resolution / q_eta
+    mu_ang = ang * resolution / q_mu
+    # if the movement is unrealistically large, the axis is unsensitive
+    if phi_ang > 20: phi_ang = 0
+    if chi_ang > 20: chi_ang = 0
+    if eta_ang > 20: eta_ang = 0
+    if mu_ang > 20: mu_ang = 0
+    return phi_ang, chi_ang, eta_ang, mu_ang
+
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/functions_general.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/functions_general.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1293 +1,1393 @@
-# -*- coding: utf-8 -*-
-"""
-Module: Generally useful functions "functions_general.py"
-
-Contains various useful shortcuts for manipulating strings and arrays,
-making use of numpy and re.
-
-By Dan Porter, PhD
-Diamond
-2021
-
-Version 2.2.0
-Last updated: 11/03/22
-
-Version History:
-06/01/18 1.0    Program created from DansGeneralProgs.py V2.3
-02/05/18 1.1    Added find_vector
-24/05/18 1.2    Corrected 'quad' for the case (1,-2,1)=1
-31/10/18 1.3    Added complex2str
-20/08/19 1.4    Added search_dict_lists
-27/03/20 1.5    Corrected error in gauss for 1d case when centre /= 0
-05/05/20 1.6    New version of readstfm, allows E powers and handles non-numbers.
-12/05/20 1.7    Added sph2cart, replace_bracket_multiple
-20/07/20 1.8    Added vector_inersection and plane_intersection, updated findranges, added whererun
-01/12/20 1.8.1  Added get_methods function
-26/01/21 1.8.2  Added shortstr and squaredata
-02/02/21 2.0.0  Merged changes in other versions, added vector_intersection and you_normal_vector
-15/11/21 2.1.0  Added normal_basis
-11/03/22 2.2.0  Added Lorentzian, pVoight, peak_function functions
-
-@author: DGPorter
-"""
-
-import sys, os, re
-import numpy as np
-import inspect
-
-__version__ = '2.2.1'
-__date__ = '01/June/2023'
-
-# File directory
-directory = os.path.abspath(os.path.dirname(__file__))
-
-# Constants
-pi = np.pi  # mmmm tasty Pi
-e = 1.6021733E-19  # C  electron charge
-h = 6.62606868E-34  # Js  Plank consant
-c = 299792458  # m/s   Speed of light
-u0 = 4 * pi * 1e-7  # H m-1 Magnetic permeability of free space
-me = 9.109e-31  # kg Electron rest mass
-mn = 1.6749e-27 # kg Neutron rest mass
-Na = 6.022e23  # Avagadro's No
-A = 1e-10  # m Angstrom
-r0 = 2.8179403227e-15  # m classical electron radius = e^2/(4pi*e0*me*c^2)
-Cu = 8.048  # Cu-Ka emission energy, keV
-Mo = 17.4808  # Mo-Ka emission energy, keV
-# Mo = 17.4447 # Mo emission energy, keV
-
-'--------------------------Misc General Programs------------------------'
-
-'---------------------------Vector manipulation-------------------------'
-
-
-def mag(A):
-    """
-    Returns the magnitude of vector A
-    If A has 2 dimensions, returns an array of magnitudes
-
-    E.G.
-     mag([1,1,1]) = 1.732
-     mag(array([[1,1,1],[2,2,2]]) = [1.732, 3.464]
-    """
-    A = np.asarray(A, dtype=float)
-    return np.sqrt(np.sum(A ** 2, axis=len(A.shape) - 1))
-
-
-def norm(A):
-    """
-    Returns normalised vector A
-    If A has 2 dimensions, returns an array of normalised vectors
-    The returned array will be the same shape as the given array.
-
-    E.G.
-     norm([1,1,1]) = [1,1,1]/1.732 = [ 0.57735,  0.57735,  0.57735]
-     norm(array([[1,1,1],[2,2,2]]) = [ [ 0.57735,  0.57735,  0.57735] , [ 0.57735,  0.57735,  0.57735] ]
-     """
-
-    A = np.asarray(A, dtype=float).reshape((-1, np.shape(A)[-1]))
-    mag = np.sqrt(np.sum(A ** 2, axis=A.ndim - 1)).reshape((-1, 1))
-    mag[mag == 0] = 1  # stop warning errors
-    N = A / mag
-    if A.shape[0] == 1:
-        N = N.reshape(-1)
-    return N
-
-
-def quad(A):
-    """
-    Returns +/-1 depending on quadrant of 3D vector A
-    i.e.:    A      Returns
-        [ 1, 1, 1]    1
-        [-1, 1, 1]    1
-        [ 1,-1, 1]    1
-        [ 1, 1,-1]    1
-        [-1,-1, 1]   -1
-        [-1, 1,-1]   -1
-        [ 1,-1,-1]   -1
-        [-1,-1,-1]   -1
-    """
-
-    A = np.asarray(A, dtype=float).reshape((-1, 3))
-    if A.size == 1:
-        # return (np.sum(A,axis=1)>0)[0]*2 - 1
-        return (np.sum(A >= 0, axis=1) > 1)[0] * 2 - 1
-    else:
-        # return (np.sum(A,axis=1)>0)*2 - 1
-        return (np.sum(A >= 0, axis=1) > 1) * 2 - 1
-
-
-def quadmag(A):
-    """
-    Returns +/- mag depending on quadrant of a 3D vector A
-    i.e.:    A      Returns
-        [ 1, 1, 1]    1.732
-        [-1, 1, 1]    1.732
-        [ 1,-1, 1]    1.732
-        [ 1, 1,-1]    1.732
-        [-1,-1, 1]   -1.732
-        [-1, 1,-1]   -1.732
-        [ 1,-1,-1]   -1.732
-        [-1,-1,-1]   -1.732
-    """
-
-    A = np.asarray(A, dtype=float).reshape((-1, 3))
-    mag = np.sqrt(np.sum(A ** 2, axis=len(A.shape) - 1)).reshape(-1)
-    quad = (np.sum(A, len(A.shape) - 1) > 0) * 2 - 1
-    if len(A) == 1:
-        return quad[0] * mag[0]
-    else:
-        return quad * mag
-
-
-def ang(a, b, deg=False):
-    """
-    Returns the angle, in Radians between vectors a and b
-    E.G.
-    ang([1,0,0],[0,1,0]) >> 1.571
-    ang([1,0,0],[0,1,0],'deg') >> 90
-    """
-    a = np.asarray(a, dtype=float).reshape([-1])
-    b = np.asarray(b, dtype=float).reshape([-1])
-
-    cosang = np.dot(a, b)
-    sinang = quadmag(np.cross(a, b))
-    angle = np.arctan2(sinang, cosang)
-    if deg:
-        return np.rad2deg(angle)
-    return angle
-
-
-def vectors_angle_degrees(a, b):
-    """
-    Returns the angle, in degrees between vectors a and b.
-    Gives the absolute angle, negatives are not given for sectors.
-        angle = acos(a.b / |a|.|b|)
-    :param a: [nx3] array of vectors [x,y,z]
-    :param b: [mx3] array of vectors [x,y,z]
-    :return: float angle in degrees is n==m==1
-    :return: [max(n, m)] array of angles in degrees if n or m == 1
-    :return: [n, m] array of angles in degrees if n and m > 1
-    """
-    a = np.asarray(a, dtype=float).reshape([-1, 3])
-    b = np.asarray(b, dtype=float).reshape([-1, 3])
-
-    cosang = np.squeeze(np.dot(a, b.T))
-    sinang = np.squeeze([quadmag(np.cross(a, bb)) for bb in b]).T  # more efficient with larger len(a) and len(b)
-    return np.rad2deg(np.arctan2(sinang, cosang))
-
-
-def cart2sph(xyz, deg=False):
-    """
-    Convert coordinates in cartesian to coordinates in spherical
-    https://en.wikipedia.org/wiki/Spherical_coordinate_system
-    ISO convention used.
-        theta = angle from Z-axis to X-axis
-          phi = angle from X-axis to component in XY plane
-    :param xyz: [n*3] array of [x,y,z] coordinates
-    :param deg: if True, returns angles in degrees
-    :return: [r, theta, phi]
-    """
-    xyz = np.asarray(xyz).reshape(-1, 3)
-    xy = xyz[:, 0] ** 2 + xyz[:, 1] ** 2
-    r = mag(xyz)
-    theta = np.arctan2(np.sqrt(xy), xyz[:, 2])  # for elevation angle defined from Z-axis down
-    # theta = np.arctan2(xyz[:,2], np.sqrt(xy))  # for elevation angle defined from XY-plane up
-    phi = np.arctan2(xyz[:, 1], xyz[:, 0])
-    if deg:
-        theta = np.rad2deg(theta)
-        phi = np.rad2deg(phi)
-    return np.vstack((r, theta, phi)).T
-
-
-def rot3D(A, alpha=0., beta=0., gamma=0.):
-    """Rotate 3D vector A by euler angles
-        A = rot3D(A,alpha=0.,beta=0.,gamma=0.)
-       where alpha = angle from X axis to Y axis (Yaw)
-             beta  = angle from Z axis to X axis (Pitch)
-             gamma = angle from Y axis to Z axis (Roll)
-       angles in degrees
-       In a right handed coordinate system.
-           Z
-          /|\
-           |
-           |________\Y
-           \        /
-            \
-            _\/X
-    """
-
-    A = np.asarray(A, dtype=float).reshape((-1, 3))
-
-    # Convert to radians
-    alpha = alpha * np.pi / 180.
-    beta = beta * np.pi / 180.
-    gamma = gamma * np.pi / 180.
-
-    # Define 3D rotation matrix
-    Rx = np.array([[1, 0, 0], [0, np.cos(gamma), -np.sin(gamma)], [0., np.sin(gamma), np.cos(gamma)]])
-    Ry = np.array([[np.cos(beta), 0., np.sin(beta)], [0., 1., 0.], [-np.sin(beta), 0., np.cos(beta)]])
-    Rz = np.array([[np.cos(alpha), -np.sin(alpha), 0.], [np.sin(alpha), np.cos(alpha), 0.], [0., 0., 1.]])
-    R = np.dot(np.dot(Rx, Ry), Rz)
-
-    # Rotate coordinates
-    return np.dot(R, A.T).T
-
-
-def rotmat(a, b):
-    """
-    Determine rotation matrix from a to b
-    From Kuba Ober's answer on stackexchange:
-    http://math.stackexchange.com/questions/180418/calculate-rotation-matrix-to-align-vector-a-to-vector-b-in-3d/476311#476311
-    Usage:
-     a = [1,0,0]
-     b = [0,1,0]
-     U = rotmat(a,b)
-     np.dot(U,a)
-     >> [0,1,0]
-    """
-
-    a = norm(a)
-    b = norm(b)
-
-    d = np.dot(a, b)
-    c = mag(np.cross(a, b))
-    G = np.array([[d, -c, 0], [c, d, 0], [0, 0, 1]])
-
-    u = a
-    v = norm(b - np.dot(a, b) * a)
-    w = np.cross(b, a)
-
-    Fm1 = np.array([u, v, w]).T
-    F = np.linalg.inv(Fm1)
-    U = np.dot(np.dot(Fm1, G), F)
-
-    # print('a = {}\nb = {}'.format(str(a),str(b)))
-    # print('G = {}\nFm1 = {}\nF = {}\nU = {}'.format(str(G),str(Fm1),str(F),str(U)))
-    return U
-
-
-def rotate_about_axis(point, axis, angle):
-    """
-    Rotate vector A about vector Axis by angle
-    Using Rodrigues' rotation formula: https://en.wikipedia.org/wiki/Rodrigues%27_rotation_formula
-    :param point: [x,y,z] coordinate to rotate
-    :param axis: [dx,dy,dz] vector about which to rotate
-    :param angle: angle to rotate in deg
-    :return: [x,y,z] rotated point
-    """
-    point = np.asarray(point, dtype=float)
-    axis = np.asarray(axis, dtype=float) / np.sqrt(np.sum(np.square(axis)))
-    rad = np.deg2rad(angle)
-    cs = np.cos(rad)
-    sn = np.sin(rad)
-    return point * cs + np.cross(axis, point) * sn + axis * np.dot(axis, point) * (1 - cs)
-
-
-def you_normal_vector(eta=0, chi=90, mu=0):
-    """
-    Determine the normal vector using the You diffractometer angles
-      you_normal_vector(0, 0, 0) = [1, 0, 0]
-      you_normal_vector(0, 90, 0) = [0, 1, 0]
-      you_normal_vector(90, 90, 0) = [0, 0, -1]
-      you_normal_vector(0, 0, 90) = [0, 0, -1]
-    :param eta: angle (deg) along the x-axis
-    :param mu: angle (deg) about the z-axis
-    :param chi: angle deg) a
-    :return: array
-    """
-    eta = np.deg2rad(eta)
-    chi = np.deg2rad(chi)
-    mu = np.deg2rad(mu)
-    normal = np.array([np.sin(mu) * np.sin(eta) * np.sin(chi) + np.cos(mu) * np.cos(chi),
-                       np.cos(eta) * np.sin(chi),
-                       -np.cos(mu) * np.sin(eta) * np.sin(chi) - np.sin(mu) * np.cos(chi)])
-    return normal
-
-
-def normal_basis(vec, normal=(1, 0, 0), azi=0):
-    """
-    Return a vector basis with 3 normal vectors such that:
-        [|normal x vec|, |vec x (normal x vec)|, |vec|]
-    if azi is given, the resulting vectors [0,1] will be rotated about [2]
-    :param vec: [3*1] array of vector
-    :param normal: [3*1] array of normal vector
-    :param azi: float azimuthal rotation about vec in degrees
-    :return: array [3*3] as unit vectors [vec1, vec2, vec3]
-    """
-    # U1 || projection of normal vector
-    # U2 _|_ U1,U3
-    # U3 || vec
-    vec = norm(vec)  # || vec
-    AxQ = norm(np.cross(normal, vec))
-    Ihat = norm(np.cross(vec, AxQ))  # || to normal
-    Jhat = norm(np.cross(vec, Ihat))  # -| to I and vec
-
-    # Rotate psi about Qhat
-    razi = np.deg2rad(azi)
-    # -ve sin makes clockwise rotation
-    Ihat_psi = norm(np.cos(razi) * Ihat - np.sin(razi) * Jhat)
-    Jhat_psi = norm(np.cross(vec, Ihat_psi))
-    return np.vstack([Ihat_psi, Jhat_psi, vec])
-
-
-def group(A, tolerance=0.0001):
-    """
-    Group similear values in an array, returning the group and indexes
-    array will be sorted so lowest numbers are grouped first
-      group_index, group_values, group_counts = group([2.1, 3.0, 3.1, 1.00], 0.1)
-    group_values = [1., 2., 3.] array of grouped numbers (rounded)
-    array_index = [1, 2, 2, 0] array matching A values to groups, such that A ~ group_values[group_index]
-    group_index = [3, 0, 1] array matching group values to A, such that group_values ~ A[group_index]
-    group_counts = [1, 1, 2] number of iterations of each item in group_values
-    :param A: list or numpy array of numbers
-    :param tolerance: values within this number will be grouped
-    :return: group_values, array_index, group_index, group_counts
-    """
-    A = np.asarray(A, dtype=float).reshape(-1)
-    idx = np.argsort(A)
-    rtn_idx = np.argsort(idx)
-    A2 = np.round(A / tolerance) * tolerance
-    groups, indices, inverse, counts = np.unique(A2[idx], return_index=True, return_inverse=True, return_counts=True)
-    # groups = A[idx][indices]  # return original, not rounded values
-    array_index = inverse[rtn_idx]
-    group_index = idx[indices]
-    return groups, array_index, group_index, counts
-
-
-def unique_vector(vecarray, tol=0.05):
-    """
-    Find unique vectors in an array within a certain tolerance
-
-    newarray,uniqueidx,matchidx = unique_vector(vecarray,tol=0.05)
-       vecarray = np.array([[:]])
-       newarray = vecarray with duplicate vectors removed
-       uniqueidx= index vectors of newarray such that vecarray[uniqueidx]=newarray
-       matchidx = index vectors of vecarray such that newarray[matchidx]=vecarray
-       tol = tolerance of vector difference to define unique vectors
-
-    E.G.
-    vecarray = [[1,1,1],[2,2,2],[3,3,3],[1,1,1],[4,4,4],[2,2,2]]
-    newarray,uniqueidx,matchidx = unique_vector(vecarray,tol=0.05)
-      newarray:        uniqueidx:
-     [[1, 1, 1],           [0,
-      [2, 2, 2],            1,
-      [3, 3, 3],            2,
-      [4, 4, 4]]            4]
-
-    matchidx: [0, 1, 2, 0, 3, 1]
-
-    E.G.
-    newarray,uniqueidx,matchidx = unique_vector([[1,0,0],[1,0,0],[0,1,0]],tol=0.05)
-    >> newarray = [[1,0,0],[0,1,0]]
-    >> uniqueidx= [0,2]
-    >> matchidx = [0,0,1]
-    """
-
-    vecarray = np.asarray(vecarray).reshape([len(vecarray), -1])
-    matchidx = -np.ones(len(vecarray), dtype=int)
-    Nunique = 0
-    for n in range(len(vecarray)):
-        if matchidx[n] > -1: continue
-        diff = mag(vecarray - vecarray[n])
-        matchidx[diff < tol] = Nunique
-        Nunique += 1
-    matchidx = matchidx.tolist()
-    uniqueidx = [matchidx.index(n) for n in range(np.max(matchidx) + 1)]
-    newarray = vecarray[uniqueidx, :]
-    return newarray, uniqueidx, matchidx
-
-
-def distance2line(line_start, line_end, point):
-    """
-    Calculate distance from a line between the start and end to an arbitary point in space
-    :param line_start: array, position of the start of the line
-    :param line_end:  array, position of the end of the line
-    :param point: array, arbitary position in space
-    :return: float
-    """
-    line_start = np.asarray(line_start)
-    line_end = np.asarray(line_end)
-    point = np.asarray(point)
-
-    line_diff = line_end - line_start
-    unit_line = line_diff / np.sqrt(np.sum(line_diff ** 2))
-
-    vec_arb = (line_start - point) - np.dot((line_start - point), unit_line) * unit_line
-    return np.sqrt(np.sum(vec_arb ** 2))
-
-
-def vector_intersection(point1, direction1, point2, direction2):
-    """
-    Calculate the point in 2D where two lines cross.
-    If lines are parallel, return nan
-    For derivation, see: http://paulbourke.net/geometry/pointlineplane/
-    :param point1: [x,y] some coordinate on line 1
-    :param direction1: [dx, dy] the direction of line 1
-    :param point2: [x,y] some coordinate on line 2
-    :param direction2: [dx, dy] the direction of line 2
-    :return: [x, y]
-    """
-
-    point1 = np.asarray(point1)
-    point2 = np.asarray(point2)
-    direction1 = np.asarray(direction1) / np.sqrt(np.sum(np.square(direction1)))
-    direction2 = np.asarray(direction2) / np.sqrt(np.sum(np.square(direction2)))
-
-    mat = np.array([direction1, -direction2])
-    try:
-        inv = np.linalg.inv(mat)
-    except np.linalg.LinAlgError:
-        print('Vectors are parallel')
-        return np.array([np.nan, np.nan])
-    ua, ub = np.dot(point2 - point1, inv)
-    intersect = point1 + ua*direction1
-    return intersect
-
-
-def vector_intersection3d(point1, direction1, point2, direction2):
-    """
-    Calculate the point in 3D where two lines cross.
-    If lines are parallel, return nan
-    For derivation, see: https://math.stackexchange.com/questions/270767/find-intersection-of-two-3d-lines/271366
-    :param point1: [x,y,z] some coordinate on line 1
-    :param direction1: [dx, dy, dz] the direction of line 1
-    :param point2: [x,y,z] some coordinate on line 2
-    :param direction2: [dx, dy, dz] the direction of line 2
-    :return: [x, y, z]
-    """
-
-    point1 = np.asarray(point1)
-    point2 = np.asarray(point2)
-    direction1 = np.asarray(direction1)/np.sqrt(np.sum(np.square(direction1)))
-    direction2 = np.asarray(direction2)/np.sqrt(np.sum(np.square(direction2)))
-
-    line = point2 - point1
-    c1 = np.cross(direction2, line)
-    c2 = np.cross(direction2, direction1)
-    h = mag(c1)
-    k = mag(c2)
-    a = ang(c1, c2)
-    if h == 0 or k == 0:
-        print('Lines parallel')
-        return np.array([np.nan, np.nan, np.nan])
-    v = (h/k) * direction1
-    if np.abs(a) < np.pi/2:
-        return point1 + v
-    return point1 - v
-
-
-def plane_intersection(line_point, line_direction, plane_point, plane_normal):
-    """
-    Calculate the point at which a line intersects a plane
-    :param line_point: [x,y],z] some coordinate on line
-    :param line_direction: [dx,dy],dz] the direction of line
-    :param plane_point:  [x,y],z] some coordinate on the plane
-    :param plane_normal: [dx,dy],dz] the normal vector of the plane
-    :return: [x,y],z]
-    """
-
-    line_point = np.asarray(line_point)
-    plane_point = np.asarray(plane_point)
-    line_direction = np.asarray(line_direction) / np.sqrt(np.sum(np.square(line_direction)))
-    plane_normal = np.asarray(plane_normal) / np.sqrt(np.sum(np.square(plane_normal)))
-
-    u1 = np.dot(plane_normal, plane_point - line_point)
-    u2 = np.dot(plane_normal, line_direction)
-
-    if u2 == 0:
-        print('Plane is parallel to line')
-        return None
-    u = u1 / u2
-    intersect = line_point + u*line_direction
-    return intersect
-
-
-def find_index(A, value):
-    """
-    Return the index of the closest number in array A to value
-
-    E.G.
-    A = [1,2,3,4,5]
-    find_index(A,3.5)
-     >> 2
-    A = [[1,2],[3,4]]
-    find_index(A,3.2)
-     >> (1,0)
-
-     For multiple values, use:
-     B = [find_index(A,x) for x in values]
-    """
-    A = np.asarray(A, dtype=float)
-    idx = np.argmin(np.abs(A - value))
-    if len(A.shape) < 2:
-        return idx
-    else:
-        return np.unravel_index(idx, A.shape)
-
-
-def find_vector(A, V, difference=0.01):
-    """
-    Return the index(s) of vectors in array A within difference of vector V
-    Comparison is based on vector difference A[n,:]-V
-
-    Returns None if no matching vector is present.
-
-    E.G.
-    A = [[1,2,3],
-         [4,5,6],
-         [7,8,9]]
-    find_index(A,[4,5,6])
-     >> 1
-
-    A = [[0, 2.5, 0],
-         [1, 0.1, 0],
-         [1,-0.1, 0],
-         [0, 0.5, ]]
-    find_vector(A, [1,0,0], difference=0.1)
-     >> [1, 2]
-    """
-    A = np.asarray(A).reshape((-1, np.shape(A)[-1]))
-    V = np.asarray(V).reshape(-1)
-    M = mag(A - V)
-    idx = np.where(M < difference)[0]
-    if len(idx) == 1:
-        return idx[0]
-    elif len(idx) == 0:
-        return None
-    else:
-        return idx
-
-
-def search_dict_lists(d, **kwargs):
-    """
-    Search equal length lists in a dictionary for specific values
-    e.g.
-        idx = search_dict_lists(cif, _geom_bond_atom_site_label_1='Ru1',
-                                     _geom_bond_atom_site_label_2='O1',
-                                     _geom_bond_site_symmetry_2='.')
-    :param d: dict
-    :param kwargs: keyword=item
-    :return: boolean array index
-    """
-    search = [np.array(d[key]) == value for key, value in kwargs.items()]
-    bool = np.product(search, axis=0)
-    return np.argwhere(bool).reshape(-1)
-
-
-def detail(A):
-    """
-    Prints details about the given vector,
-    including length, min, max, number of elements
-    """
-    tp = type(A)
-    print('Type: {}'.format(tp))
-    A = np.asarray(A, dtype=float)
-    size = ' x '.join([str(x) for x in A.shape])
-    mem = '%1.3g MB' % (A.nbytes * 1e-6)
-    print('Size: {} (elements={}, {})'.format(size, A.size, mem))
-    print('Min: {}, Max: {}, Mean: {}, NaNs: {}'.format(np.nanmin(A), np.nanmax(A), np.nanmean(A), np.sum(np.isnan(A))))
-
-
-def inline_help(func):
-    """Return function spec and first line of help in line"""
-    fun_name = '%s%s' % (func.__name__, inspect.signature(func))
-    fun_doc = func.__doc__.strip().split('\n')[0] if func.__doc__ else ""
-    return "%s\n\t%s" % (fun_name, fun_doc)
-
-
-def array_str(A):
-    """
-    Returns a short string with array information
-    :param A: np array
-    :return: str
-    """
-    shape = np.shape(A)
-    try:
-        amax = np.max(A)
-        amin = np.min(A)
-        amean = np.mean(A)
-        out_str = "%s max: %4.5g, min: %4.5g, mean: %4.5g"
-        return out_str % (shape, amax, amin, amean)
-    except TypeError:
-        # list of str
-        array = np.asarray(A).reshape(-1)
-        array_start = array[0]
-        array_end = array[-1]
-        out_str = "%s [%s, ..., %s]"
-        return out_str % (shape, array_start, array_end)
-
-
-def print_arrays(arrays=[]):
-    """
-    Prints values from several arrays with nice formatting
-    e.g. dgp.print_arrays(1e6*np.random.rand(5,5))
-         0   6.04e+03   2.29e+05   7.19e+05   4.74e+05   9.59e+05
-         1   9.16e+05   6.33e+05    1.6e+05   3.75e+05   3.01e+05
-         2   4.21e+04   1.78e+05   4.78e+05   7.56e+05   2.47e+05
-         3   9.26e+05   6.39e+05   3.96e+05   4.42e+05   4.52e+04
-         4   3.38e+05   4.54e+05   4.29e+05   6.34e+04   6.06e+04
-    """
-
-    # Combine all arrays into BigArray
-    BigArray = np.arange(len(arrays[0])).reshape([len(arrays[0]), -1])
-    for A in arrays:
-        BigArray = np.hstack((BigArray, np.asarray(A).reshape([len(A), -1])))
-
-    # Print BigArray
-    fmt = '{:10.3g} ' * BigArray.shape[1]
-    for n in range(len(BigArray)):
-        print(fmt.format(*BigArray[n, :]))
-
-
-def cell(lengths=[1, 1, 1], rotation=[0, 0, 0]):
-    """
-    Returns a unit CELL with vectors defined by length and rotation (Deg)
-    :param lengths:
-    :param rotation:
-    :return:
-    """
-    CELL = np.eye(3) * lengths
-    CELL = rot3D(CELL, *rotation)
-    return CELL
-
-
-def index_coordinates(A, CELL):
-    """
-    Index A(x1,y1,1) on new coordinate system B(x2,y2,z2), defined by unit vectors CELL = [A,B,C]
-      A = [[nx3]] array of vectors
-      CELL = [[3x3]] matrix of vectors [a,b,c]
-    """
-
-    A = np.asarray(A, dtype=float).reshape((-1, 3))
-    B = np.dot(A, np.linalg.inv(CELL))
-    return B
-
-
-def isincell(A, cell_centre=[0, 0, 0], CELL=cell()):
-    """
-     Return boolean of whether vector xyx is inside a cell defined by position, size and rotation
-       A = [x,y,z] or [[x1,y1,z1]] array of positions
-       cell_centre = [x,y,z] cell centre
-       CELL = [[3x3]] matrix of vectors [a,b,c]
-
-    E.G.
-       xyz = [[1,1,0],[0,0,0.5],[0.1,0,5]]
-       centre = [0,0,0]
-       CELL = cell([1,1,10],[0,0,0])
-       isinbox(xyz,centre,CELL)
-       >>> [False,True,True]
-    """
-
-    A = np.asarray(A, dtype=float).reshape((-1, 3))
-    A = A - cell_centre
-    idx = index_coordinates(A, CELL)
-    return np.all(np.abs(idx) <= 0.5, axis=1)
-
-
-def sphere_array(A, max_angle1=90, max_angle2=90, step1=1, step2=1):
-    """
-    Rotate points in array A by multiple angles
-     B = sphere_array(A, max_angle1, max_angle2, step1, step2)
-
-      A = [nx3] array of 3D coordinates
-      max_angle1 = max rotation angle
-      max_angle1 = max rotation angle
-      step1 = angular step size
-      step2 = angular step size
-
-    Each coordinate in A will be rotated by angles:
-        angles = np.arange(0, max_angle+step, step)
-    The output B will have size:
-        [len(A) * len(angles1) * len(angles2), 3]
-    """
-
-    A = np.asarray(A, dtype=float).reshape((-1, 3))
-
-    angles1 = np.arange(0, max_angle1 + step1, step1)
-    angles2 = np.arange(0, max_angle2 + step2, step2)
-    len1 = len(angles1)
-    len2 = len(angles2)
-    len3 = len(A)
-    tot_size = len1 * len2 * len3
-    OUT = np.zeros([tot_size, 3])
-    for n in range(len(angles1)):
-        for m in range(len(angles2)):
-            B = rot3D(A, 0, angles1[n], angles2[m])
-            st = n * len2 + m * len3
-            nd = n * len2 + (m + 1) * len3
-            OUT[st:nd, :] = B
-    return OUT
-
-
-'---------------------------String manipulation-------------------------'
-
-
-def stfm(val, err):
-    """
-    Create standard form string from value and uncertainty"
-     str = stfm(val,err)
-     Examples:
-          '35.25 (1)' = stfm(35.25,0.01)
-          '110 (5)' = stfm(110.25,5)
-          '0.0015300 (5)' = stfm(0.00153,0.0000005)
-          '1.56(2)E+6' = stfm(1.5632e6,1.53e4)
-
-    Notes:
-     - Errors less than 0.01% of values will be given as 0
-     - The maximum length of string is 13 characters
-     - Errors greater then 10x the value will cause the value to be rounded to zero
-    """
-
-    # Determine the number of significant figures from the error
-    if err == 0. or val / float(err) >= 1E5:
-        # Zero error - give value to 4 sig. fig.
-        out = '{:1.5G}'.format(val)
-        if 'E' in out:
-            out = '{}(0)E{}'.format(*out.split('E'))
-        else:
-            out = out + ' (0)'
-        return out
-    elif np.log10(np.abs(err)) > 0.:
-        # Error > 0
-        sigfig = np.ceil(np.log10(np.abs(err))) - 1
-        dec = 0.
-    elif np.isnan(err):
-        # nan error
-        return '{} (-)'.format(val)
-    else:
-        # error < 0
-        sigfig = np.floor(np.log10(np.abs(err)) + 0.025)
-        dec = -sigfig
-
-    # Round value and error to the number of significant figures
-    rval = round(val / (10. ** sigfig)) * (10. ** sigfig)
-    rerr = round(err / (10. ** sigfig)) * (10. ** sigfig)
-    # size of value and error
-    pw = np.floor(np.log10(np.abs(rval)))
-    pwr = np.floor(np.log10(np.abs(rerr)))
-
-    max_pw = max(pw, pwr)
-    ln = max_pw - sigfig  # power difference
-
-    if np.log10(np.abs(err)) < 0:
-        rerr = err / (10. ** sigfig)
-
-    # Small numbers - exponential notation
-    if max_pw < -3.:
-        rval = rval / (10. ** max_pw)
-        fmt = '{' + '0:1.{:1.0f}f'.format(ln) + '}({1:1.0f})E{2:1.0f}'
-        return fmt.format(rval, rerr, max_pw)
-
-    # Large numbers - exponential notation
-    if max_pw >= 4.:
-        rval = rval / (10. ** max_pw)
-        rerr = rerr / (10. ** sigfig)
-        fmt = '{' + '0:1.{:1.0f}f'.format(ln) + '}({1:1.0f})E+{2:1.0f}'
-        return fmt.format(rval, rerr, max_pw)
-
-    fmt = '{' + '0:0.{:1.0f}f'.format(dec + 0) + '} ({1:1.0f})'
-    return fmt.format(rval, rerr)
-
-
-def readstfm(string):
-    """
-    Read numbers written in standard form: 0.01(2), return value and error
-    Read numbers from string with form 0.01(2), returns floats 0.01 and 0.02
-    Errors and values will return 0 if not given.
-
-    E.G.
-    readstfm('0.01(2)') = (0.01, 0.02)
-    readstfm('1000(300)') = (1000.,300.)
-    readstfm('1.23(3)E4') = (12300.0, 300.0)
-    """
-
-    values = re.findall('[-0-9.]+|\([-0-9.]+\)', string)
-    if len(values) > 0 and '(' not in values[0] and values[0] != '.':
-        value = values[0]
-    else:
-        value = '0'
-
-    # Determine number of decimal places for error
-    idx = value.find('.')  # returns -1 if . not found
-    if idx > -1:
-        pp = idx - len(value) + 1
-    else:
-        pp = 0
-    value = float(value)
-
-    error = re.findall('\([-0-9.]+\)', string)
-    if len(error) > 0:
-        error = abs(float(error[0].strip('()')))
-        error = error * 10 ** pp
-    else:
-        error = 0.
-
-    power = re.findall('(?:[eE]|x10\^|\*10\^|\*10\*\*)([+-]?\d*\.?\d+)', string)
-    if len(power) > 0:
-        power = float(power[0])
-        value = value * 10 ** power
-        error = error * 10 ** power
-    return value, error
-
-
-def saveable(string):
-    """
-    Returns a string without special charaters.
-    Removes bad characters from a string, so it can be used as a filename
-    E.G.
-    saveable('Test#1<froot@5!') = 'TestS1_froot_5'
-    """
-    # Special - replace # with S for scans
-    string = string.replace('#', 'S')
-    # Replace some characters with underscores
-    for char in '#%{}\/<>@|':
-        string = string.replace(char, '_')
-        # Replace other characters with nothing
-    for char in '*$&^?!':
-        string = string.replace(char, '')
-    # Remove non-ascii characters
-    string = ''.join(i for i in string if ord(i) < 128)
-    # string = string.decode('unicode_escape').encode('ascii','ignore')
-    return string
-
-
-def findranges(scannos, sep=':'):
-    """
-    Convert a list of numbers to a simple string
-    E.G.
-    findranges([1,2,3,4,5]) = '1:5'
-    findranges([1,2,3,4,5,10,12,14,16]) = '1:5,10:2:16'
-    """
-
-    scannos = np.sort(scannos).astype(int)
-
-    dif = np.diff(scannos)
-
-    stt, stp, rng = [scannos[0]], [dif[0]], [1]
-    for n in range(1, len(dif)):
-        if scannos[n + 1] != scannos[n] + dif[n - 1]:
-            stt += [scannos[n]]
-            stp += [dif[n]]
-            rng += [1]
-        else:
-            rng[-1] += 1
-    stt += [scannos[-1]]
-    rng += [1]
-
-    out = []
-    x = 0
-    while x < len(stt):
-        if rng[x] == 1:
-            out += ['{}'.format(stt[x])]
-            x += 1
-        elif stp[x] == 1:
-            out += ['{}{}{}'.format(stt[x], sep, stt[x + 1])]
-            x += 2
-        else:
-            out += ['{}{}{}{}{}'.format(stt[x], sep, stp[x], sep, stt[x + 1])]
-            x += 2
-    return ','.join(out)
-
-
-def str2array(string):
-    """Convert string to array"""
-    string = string.replace(',', ' ')  # remove commas
-    string = string.replace('(', '').replace(')', '')  # remove brackets
-    string = string.replace('[', '').replace(']', '')  # remove brackets
-    return np.fromstring(string, sep=' ')
-
-
-def numbers2string(scannos, sep=':'):
-    """
-    Convert a list of numbers to a simple string
-    E.G.
-    numbers2string([50001,50002,50003]) = '5000[1:3]'
-    numbers2string([51020,51030,51040]) = '510[20:10:40]'
-    """
-
-    if type(scannos) is str or type(scannos) is int or len(scannos) == 1:
-        return str(scannos)
-
-    scannos = np.sort(scannos).astype(str)
-
-    n = len(scannos[0])
-    while np.all([scannos[0][:-n] == x[:-n] for x in scannos]):
-        n -= 1
-
-    if n == len(scannos[0]):
-        return '{}-{}'.format(scannos[0], scannos[-1])
-
-    inistr = scannos[0][:-(n + 1)]
-    strc = [i[-(n + 1):] for i in scannos]
-    liststr = findranges(strc, sep=sep)
-    return '{}[{}]'.format(inistr, liststr)
-
-
-def complex2str(val, fmt='6.1f'):
-    """
-    Convert complex number to string
-    """
-
-    rl = np.real(val)
-    im = np.imag(val)
-    fmt1 = '%' + fmt
-    fmt2 = '%-' + fmt
-    if im >= 0:
-        return (fmt1 + ' + i' + fmt2) % (rl, im)
-    elif im < 0:
-        return (fmt1 + ' - i' + fmt2) % (rl, np.abs(im))
-
-
-def multi_replace(string, old=[], new=[]):
-    """
-    Replace multiple strings at once
-    :param string:
-    :param old:
-    :param new:
-    :return:
-    """
-
-    if type(new) is str:
-        new = [new]
-    if type(old) is str:
-        old = [old]
-    if len(new) == 1:
-        new = new * len(old)
-    for i, j in zip(old, new):
-        string = string.replace(i, j)
-    return string
-
-
-def replace_bracket_multiple(name):
-    """
-    Replace any numbers in brackets with numbers multipled by bracket multiplyer
-    Assumes bracket multiplier is on the left side
-    e.g.
-        replace_bracket_multiple('Mn0.3(Fe3.6(Co1.2)2)4(Mo0.7Pr44)3')
-        >> 'Mn0.3Fe14.4Co9.6Mo2.1Pr132'
-    :param name: str
-    :return: str
-    """
-    """
-    To do:
-     - Multiply by fraction (regex for '/number')
-     - Multiple on right hand side
-    """
-    # Regex:
-    regex_num = re.compile('[\d\.]+')
-    regex_bracket_n = re.compile('\)[\d\.]+')
-
-    # Find outside brackets
-    bracket = []
-    start_idx = []
-    level = 0
-    for n, s in enumerate(name):
-        if s in ['(', '[', '{']:
-            start_idx += [n]
-            level += 1
-        elif s in [')', ']', '}']:
-            level -= 1
-            if level == 0:
-                num = regex_bracket_n.findall(name[n:])
-                if len(num) > 0:
-                    bracket_end = n + len(num[0])
-                    num = float(num[0][1:])
-                else:
-                    bracket_end = n + 1
-                    num = 1.0
-                bracket += [(
-                    name[start_idx[0] + 1:n],  # insde brackets
-                    name[start_idx[0]:bracket_end],  # str to replace
-                    num  # multiplication appending bracket
-                )]
-                start_idx = []
-
-    for numstr, repstr, num in bracket:
-        # Run recursivley to get inner brackets
-        numstr = replace_bracket_multiple(numstr)
-        # Replace each number by it's multiple
-        for oldnum in regex_num.findall(numstr):
-            numstr = numstr.replace(oldnum, '%0.3g' % (float(oldnum) * num))
-        # Replace in original string
-        name = name.replace(repstr, numstr)
-    return name
-
-
-def shortstr(string):
-    """
-    Shorten string by removing long floats
-    :param string: string, e.g. '#810002 scan eta 74.89533603616637 76.49533603616636 0.02 pil3_100k 1 roi2'
-    :return: shorter string, e.g. '#810002 scan eta 74.895 76.495 0.02 pil3_100k 1 roi2'
-    """
-    #return re.sub(r'(\d\d\d)\d{4,}', r'\1', string)
-    def subfun(m):
-        return str(round(float(m.group()), 3))
-    return re.sub(r'\d+\.\d{5,}', subfun, string)
-
-
-def nice_print(precision=4, linewidth=300):
-    """
-    Sets default printing of arrays to a nicer format
-    """
-    np.set_printoptions(precision=precision, suppress=True, linewidth=linewidth)
-
-
-'----------------------------------Others-------------------------------'
-
-
-def gauss(x, y=None, height=1, centre=0, fwhm=0.5, bkg=0, centre_y=None, fwhm_y=None):
-    """
-    Define a Gaussian distribution in 1 or 2 dimensions
-
-        g = height * exp( -ln2 (x-centre)^2 / (fwhm/2)^2 ) + bkg
-    From http://fityk.nieto.pl/model.html
-
-        x = [1xn] array of values, defines size of gaussian in dimension 1
-        y = None* or [1xm] array of values, defines size of gaussian in dimension 2
-        height = peak height
-        centre = peak centre
-        fwhm = peak full width at half-max
-        bkg = background
-        centre_y = if 2D, centre along the y-axis (defaults to centre)
-        fwhm_y = if 2D, fwhm along the y-axis (defaults to fwhm)
-    """
-
-    if centre_y is None:
-        centre_y = centre
-    if fwhm_y is None:
-        fwhm_y = fwhm
-    if y is None:
-        y = centre_y
-
-    x = np.asarray(x, dtype=float).reshape([-1])
-    y = np.asarray(y, dtype=float).reshape([-1])
-    X, Y = np.meshgrid(x, y)
-    Px = (X - centre) ** 2 / (fwhm / 2) ** 2
-    Py = (Y - centre_y) ** 2 / (fwhm_y / 2) ** 2
-    g = height * np.exp(-np.log(2) * (Px + Py)) + bkg
-
-    if len(y) == 1:
-        g = g.reshape([-1])
-    return g
-
-
-def lorentz(x, y=None, height=1, centre=0, fwhm=0.5, bkg=0, centre_y=None, fwhm_y=None):
-    """
-    Define a Lorentzian distribution in 1 or 2 dimensions
-
-        l = height / ( 1 + (x - centre)^2 / (fwhm/2)^2 + bkg
-
-        x = [1xn] array of values, defines size of gaussian in dimension 1
-        y = None* or [1xm] array of values, defines size of gaussian in dimension 2
-        height = peak height
-        centre = peak centre
-        fwhm = peak full width at half-max
-        bkg = background
-        centre_y = if 2D, centre along the y-axis (defaults to centre)
-        fwhm_y = if 2D, fwhm along the y-axis (defaults to fwhm)
-    """
-
-    if centre_y is None:
-        centre_y = centre
-    if fwhm_y is None:
-        fwhm_y = fwhm
-    if y is None:
-        y = centre_y
-
-    sigma_x = fwhm / 2.
-    sigma_y = fwhm_y / 2.
-
-    x = np.asarray(x, dtype=float).reshape([-1])
-    y = np.asarray(y, dtype=float).reshape([-1])
-    X, Y = np.meshgrid(x, y)
-    Px = (X - centre) ** 2 / sigma_x ** 2
-    Py = (Y - centre_y) ** 2 / sigma_y ** 2
-    lz = height / (1 + Px + Py) + bkg
-
-    if len(y) == 1:
-        lz = lz.reshape([-1])
-    return lz
-
-
-def pvoight(x, y=None, height=1, centre=0, fwhm=0.5, bkg=0, l_fraction=0.5, centre_y=None, fwhm_y=None):
-    """
-    Define psuedo-voight distribution in 1 or 2 dimensions
-
-        v = fraction * lorentz() + (1 - fraction) * gauss()
-
-        x = [1xn] array of values, defines size of gaussian in dimension 1
-        y = None* or [1xm] array of values, defines size of gaussian in dimension 2
-        height = peak height
-        centre = peak centre
-        fwhm = peak full width at half-max
-        bkg = background
-        l_fraction = Lorentzian fraction (0-1)
-        centre_y = if 2D, centre along the y-axis (defaults to centre)
-        fwhm_y = if 2D, fwhm along the y-axis (defaults to fwhm)
-    """
-    g = gauss(x, y, height=height, centre=centre, fwhm=fwhm, bkg=bkg, centre_y=centre_y, fwhm_y=fwhm_y)
-    l = lorentz(x, y, height=height, centre=centre, fwhm=fwhm, bkg=bkg, centre_y=centre_y, fwhm_y=fwhm_y)
-    return (1 - l_fraction) * g + l_fraction * l
-
-
-def peak_function(func_name, *args, **kwargs):
-    """
-    Choose & create peak function, using either gaussian, lorentzian or pseudo-voight
-    :param func_name: 'gaussian', 'lorentzian', 'psudovoight' (raise ValueError if wrong)
-    :param args: x, y, height, centre, fwhm, bkg, (fraction), centre_y, fwhm_y
-    :param kwargs:
-    :return: array()
-    """
-    func_name = func_name.lower().replace(' ', '').replace('-', '')
-    if 'gauss' in func_name:
-        return gauss(*args, **kwargs)
-    if 'lorentz' in func_name:
-        return lorentz(*args, **kwargs)
-    if 'voight' in func_name:
-        return pvoight(*args, **kwargs)
-    raise ValueError('%s not available as peak function.' % func_name)
-
-
-def frange(start, stop=None, step=1):
-    """
-    Returns a list of floats from start to stop in step increments
-    Like np.arange but ends at stop, rather than at stop-step
-    E.G.
-    A = frange(0,5,1) = [0.,1.,2.,3.,4.,5.]
-    """
-    if stop is None:
-        stop = start
-        start = 0
-
-    return list(np.arange(start, stop + 0.00001, step, dtype=float))
-
-
-def squaredata(xdata, ydata, data, repeat=None):
-    """
-    Generate square arrays from 1D data, automatically determinging the repeat value
-    :param xdata: [n] array
-    :param ydata: [n] array
-    :param data: [n] array
-    :param repeat: int m or None to deteremine m from differences in xdata and y data
-    :return: X, Y, D [n//m, m] arrays
-    """
-
-    if repeat is None:
-        # Determine the repeat length of the scans
-        delta_x = np.abs(np.diff(xdata))
-        ch_idx_x = np.where(delta_x > delta_x.max() * 0.9)  # find biggest changes
-        ch_delta_x = np.diff(ch_idx_x)
-        rep_len_x = np.round(np.mean(ch_delta_x))
-        delta_y = np.abs(np.diff(ydata))
-        ch_idx_y = np.where(delta_y > delta_y.max() * 0.9)  # find biggest changes
-        ch_delta_y = np.diff(ch_idx_y)
-        rep_len_y = np.round(np.mean(ch_delta_y))
-        repeat = int(max(rep_len_x, rep_len_y))
-    xsquare = xdata[:repeat * (len(xdata) // repeat)].reshape(-1, repeat)
-    ysquare = ydata[:repeat * (len(ydata) // repeat)].reshape(-1, repeat)
-    dsquare = data[:repeat * (len(data) // repeat)].reshape(-1, repeat)
-    return xsquare, ysquare, dsquare
-
-
-def grid_intensity(points, values, resolution=0.01, peak_width=0.1, background=0):
-    """
-    Generates array of intensities along a spaced grid, equivalent to a powder pattern.
-      grid, values = generate_powder(points, values, resolution=0.01, peak_width=0.1, background=0)
-    :param points: [nx1] position of values to place on grid
-    :param values: [nx1] values to place at points
-    :param resolution: grid spacing size, with same units as points
-    :param peak_width: width of convolved gaussian, with same units as points
-    :param background: add a normal (random) background with width sqrt(background)
-    :return: points, values
-    """
-
-    points = np.asarray(points, dtype=float)
-    values = np.asarray(values, dtype=float)
-
-    # create plotting mesh
-    grid_points = np.arange(np.min(points) - 50 * resolution, np.max(points) + 50 * resolution, resolution)
-    pixels = len(grid_points)
-    grid_values = np.zeros([pixels])
-
-    # add reflections to background
-    pixel_size = (grid_points.max() - grid_points.min()) / pixels
-    peak_width_pixels = peak_width / (1.0 * pixel_size)
-
-    pixel_coord = (points - grid_points.min()) / (grid_points - grid_points.min()).max()
-    pixel_coord = (pixel_coord * (pixels - 1)).astype(int)
-    pixel_coord = pixel_coord.astype(int)
-
-    for n in range(0, len(values)):
-        grid_values[pixel_coord[n]] = grid_values[pixel_coord[n]] + values[n]
-
-    # Convolve with a gaussian (if >0 or not None)
-    if peak_width:
-        gauss_x = np.arange(-3 * peak_width_pixels, 3 * peak_width_pixels + 1)  # gaussian width = 2*FWHM
-        g = gauss(gauss_x, None, height=1, centre=0, fwhm=peak_width_pixels, bkg=0)
-        grid_values = np.convolve(grid_values, g, mode='same')
-
-    # Add background (if >0 or not None)
-    if background:
-        bkg = np.random.normal(background, np.sqrt(background), [pixels])
-        grid_values = grid_values + bkg
-    return grid_points, grid_values
-
-
-def map2grid(grid, points, values, widths=None, background=0):
-    """
-    Generates array of intensities along a spaced grid, equivalent to a powder pattern.
-      grid, values = generate_powder(points, values, resolution=0.01, peak_width=0.1, background=0)
-    :param grid: [mx1] grid of positions
-    :param points: [nx1] position of values to place on grid
-    :param values: [nx1] values to place at points
-    :param widths: width of convolved gaussian, with same units as points
-    :param background: add a normal (random) background with width sqrt(background)
-    :return: points, values
-    """
-    grid = np.asarray(grid, dtype=float)
-    points = np.asarray(points, dtype=float)
-    values = np.asarray(values, dtype=float)
-    widths = np.asarray(widths, dtype=float)
-
-    if widths.size == 1:
-        widths = widths * np.ones(len(points))
-
-    pixels = len(grid)
-    grid_values = np.zeros([pixels])
-
-    for point, value, width in zip(points, values, widths):
-        g = gauss(grid, None, height=value, centre=point, fwhm=width, bkg=0)
-        grid_values += g
-
-    # Add background (if >0 or not None)
-    if background:
-        bkg = np.random.normal(background, np.sqrt(background), [pixels])
-        grid_values = grid_values + bkg
-    return grid_values
-
-
-def whererun():
-    """Returns the location where python was run"""
-    return os.path.abspath('.')
-
-
-def lastlines(filename, lines=1, max_line_length=255):
-    """Returns the last n lines of a text file"""
-    with open(filename, 'rb') as f:
-        f.seek(-(lines+1)*max_line_length, os.SEEK_END)
-        endlines = f.read().decode().split('\n')
-    return endlines[-lines:]
-
-
-def get_methods(object, include_special=True):
-    """Returns a list of methods (functions) within object"""
-    if include_special:
-        return [method_name for method_name in dir(object) if callable(getattr(object, method_name))]
-    return [method_name for method_name in dir(object) if callable(getattr(object, method_name)) and '__' not in method_name]
-
-
-def list_methods(object, include_special=False):
-    """Return list of methods (functions) in class object"""
-    methods = get_methods(object, include_special)
-    return '\n'.join([inline_help(getattr(object, fun)) for fun in methods])
+# -*- coding: utf-8 -*-
+"""
+Module: Generally useful functions "functions_general.py"
+
+Contains various useful shortcuts for manipulating strings and arrays,
+making use of numpy and re.
+
+By Dan Porter, PhD
+Diamond
+2021
+
+Version 2.2.0
+Last updated: 11/03/22
+
+Version History:
+06/01/18 1.0    Program created from DansGeneralProgs.py V2.3
+02/05/18 1.1    Added find_vector
+24/05/18 1.2    Corrected 'quad' for the case (1,-2,1)=1
+31/10/18 1.3    Added complex2str
+20/08/19 1.4    Added search_dict_lists
+27/03/20 1.5    Corrected error in gauss for 1d case when centre /= 0
+05/05/20 1.6    New version of readstfm, allows E powers and handles non-numbers.
+12/05/20 1.7    Added sph2cart, replace_bracket_multiple
+20/07/20 1.8    Added vector_inersection and plane_intersection, updated findranges, added whererun
+01/12/20 1.8.1  Added get_methods function
+26/01/21 1.8.2  Added shortstr and squaredata
+02/02/21 2.0.0  Merged changes in other versions, added vector_intersection and you_normal_vector
+15/11/21 2.1.0  Added normal_basis
+11/03/22 2.2.0  Added Lorentzian, pVoight, peak_function functions
+15/05/24 2.2.2  Added sph2cart, meshgrid_sphere
+
+@author: DGPorter
+"""
+
+import sys, os, re
+import numpy as np
+import inspect
+
+__version__ = '2.2.2'
+__date__ = '15/May/2024'
+
+# File directory
+directory = os.path.abspath(os.path.dirname(__file__))
+
+# Constants
+pi = np.pi  # mmmm tasty Pi
+e = 1.6021733E-19  # C  electron charge
+h = 6.62606868E-34  # Js  Plank consant
+c = 299792458  # m/s   Speed of light
+u0 = 4 * pi * 1e-7  # H m-1 Magnetic permeability of free space
+me = 9.109e-31  # kg Electron rest mass
+mn = 1.6749e-27 # kg Neutron rest mass
+Na = 6.022e23  # Avagadro's No
+A = 1e-10  # m Angstrom
+r0 = 2.8179403227e-15  # m classical electron radius = e^2/(4pi*e0*me*c^2)
+Cu = 8.048  # Cu-Ka emission energy, keV
+Mo = 17.4808  # Mo-Ka emission energy, keV
+# Mo = 17.4447 # Mo emission energy, keV
+
+# Characters
+AA = u'\u212B'
+Am1 = u'\u212B\u207B\u00B9'
+THETA = u'\u03B8'
+DELTA = u'\u0394'
+SIGMA = u'\u03c3'
+PI = u'\u03c0'
+
+
+'--------------------------Misc General Programs------------------------'
+
+'---------------------------Vector manipulation-------------------------'
+
+
+def mag(A):
+    """
+    Returns the magnitude of vector A
+    If A has 2 dimensions, returns an array of magnitudes
+
+    E.G.
+     mag([1,1,1]) = 1.732
+     mag(array([[1,1,1],[2,2,2]]) = [1.732, 3.464]
+    """
+    A = np.asarray(A, dtype=float)
+    return np.sqrt(np.sum(A ** 2, axis=len(A.shape) - 1))
+
+
+def norm(A):
+    """
+    Returns normalised vector A
+    If A has 2 dimensions, returns an array of normalised vectors
+    The returned array will be the same shape as the given array.
+
+    E.G.
+     norm([1,1,1]) = [1,1,1]/1.732 = [ 0.57735,  0.57735,  0.57735]
+     norm(array([[1,1,1],[2,2,2]]) = [ [ 0.57735,  0.57735,  0.57735] , [ 0.57735,  0.57735,  0.57735] ]
+     """
+
+    A = np.asarray(A, dtype=float).reshape((-1, np.shape(A)[-1]))
+    mag = np.sqrt(np.sum(A ** 2, axis=A.ndim - 1)).reshape((-1, 1))
+    mag[mag == 0] = 1  # stop warning errors
+    N = A / mag
+    if A.shape[0] == 1:
+        N = N.reshape(-1)
+    return N
+
+
+def quad(A):
+    """
+    Returns +/-1 depending on quadrant of 3D vector A
+    i.e.:    A      Returns
+        [ 1, 1, 1]    1
+        [-1, 1, 1]    1
+        [ 1,-1, 1]    1
+        [ 1, 1,-1]    1
+        [-1,-1, 1]   -1
+        [-1, 1,-1]   -1
+        [ 1,-1,-1]   -1
+        [-1,-1,-1]   -1
+    """
+
+    A = np.asarray(A, dtype=float).reshape((-1, 3))
+    if A.size == 1:
+        # return (np.sum(A,axis=1)>0)[0]*2 - 1
+        return (np.sum(A >= 0, axis=1) > 1)[0] * 2 - 1
+    else:
+        # return (np.sum(A,axis=1)>0)*2 - 1
+        return (np.sum(A >= 0, axis=1) > 1) * 2 - 1
+
+
+def quadmag(A):
+    """
+    Returns +/- mag depending on quadrant of a 3D vector A
+    i.e.:    A      Returns
+        [ 1, 1, 1]    1.732
+        [-1, 1, 1]    1.732
+        [ 1,-1, 1]    1.732
+        [ 1, 1,-1]    1.732
+        [-1,-1, 1]   -1.732
+        [-1, 1,-1]   -1.732
+        [ 1,-1,-1]   -1.732
+        [-1,-1,-1]   -1.732
+    """
+
+    A = np.asarray(A, dtype=float).reshape((-1, 3))
+    mag = np.sqrt(np.sum(A ** 2, axis=len(A.shape) - 1)).reshape(-1)
+    quad = (np.sum(A, len(A.shape) - 1) > 0) * 2 - 1
+    if len(A) == 1:
+        return quad[0] * mag[0]
+    else:
+        return quad * mag
+
+
+def ang(a, b, deg=False):
+    """
+    Returns the angle, in Radians between vectors a and b
+    E.G.
+    ang([1,0,0],[0,1,0]) >> 1.571
+    ang([1,0,0],[0,1,0],'deg') >> 90
+    """
+    a = np.asarray(a, dtype=float).reshape([-1])
+    b = np.asarray(b, dtype=float).reshape([-1])
+
+    cosang = np.dot(a, b)
+    sinang = quadmag(np.cross(a, b))
+    angle = np.arctan2(sinang, cosang)
+    if deg:
+        return np.rad2deg(angle)
+    return angle
+
+
+def vectors_angle_degrees(a, b):
+    """
+    Returns the angle, in degrees between vectors a and b.
+    Gives the absolute angle, negatives are not given for sectors.
+        angle = acos(a.b / |a|.|b|)
+    :param a: [nx3] array of vectors [x,y,z]
+    :param b: [mx3] array of vectors [x,y,z]
+    :return: float angle in degrees is n==m==1
+    :return: [max(n, m)] array of angles in degrees if n or m == 1
+    :return: [n, m] array of angles in degrees if n and m > 1
+    """
+    a = np.asarray(a, dtype=float).reshape([-1, 3])
+    b = np.asarray(b, dtype=float).reshape([-1, 3])
+
+    cosang = np.squeeze(np.dot(a, b.T))
+    sinang = np.squeeze([quadmag(np.cross(a, bb)) for bb in b]).T  # more efficient with larger len(a) and len(b)
+    return np.rad2deg(np.arctan2(sinang, cosang))
+
+
+def cart2sph(xyz, deg=False):
+    """
+    Convert coordinates in cartesian to coordinates in spherical
+    https://en.wikipedia.org/wiki/Spherical_coordinate_system
+    ISO convention used.
+        theta = angle from Z-axis to X-axis
+          phi = angle from X-axis to component in XY plane
+    :param xyz: [n*3] array of [x,y,z] coordinates
+    :param deg: if True, returns angles in degrees
+    :return: [r, theta, phi]
+    """
+    xyz = np.asarray(xyz).reshape(-1, 3)
+    xy = xyz[:, 0] ** 2 + xyz[:, 1] ** 2
+    r = mag(xyz)
+    theta = np.arctan2(np.sqrt(xy), xyz[:, 2])  # for elevation angle defined from Z-axis down
+    # theta = np.arctan2(xyz[:,2], np.sqrt(xy))  # for elevation angle defined from XY-plane up
+    phi = np.arctan2(xyz[:, 1], xyz[:, 0])
+    if deg:
+        theta = np.rad2deg(theta)
+        phi = np.rad2deg(phi)
+    return np.vstack((r, theta, phi)).T
+
+
+def sph2cart(r_th_ph, deg=False):
+    """
+    Convert coordinates in spherical to coordinates in cartesian
+    https://en.wikipedia.org/wiki/Spherical_coordinate_system
+        radius = sphere radius
+        theta = angle from Z-axis to X-axis
+          phi = angle from X-axis to component in XY plane
+    :param r_th_ph: [[radius, theta, phi], ]
+    :param deg: if True, converts theta, phi from degrees
+    :return: [x,y,z]
+    """
+    r, theta, phi = np.transpose(r_th_ph)
+    if deg:
+        theta = np.deg2rad(theta)
+        phi = np.deg2rad(phi)
+    x = r * np.sin(theta) * np.cos(phi)
+    y = r * np.sin(theta) * np.sin(phi)
+    z = r * np.cos(theta)
+    return np.vstack((x, y, z)).T
+
+
+def meshgrid_sphere(sep, r_max, r_min=0):
+    """
+    Return a cartesian grid of points within a spherical shell
+    :param sep: average separation between lattice points
+    :param r_max: outer shell radiuc
+    :param r_min: inner shell radius
+    :return: array([u, v, w]) of lattice points
+    """
+    r_range = np.arange(r_min, r_max, sep)
+    # use cosine rule to determine average angular separation between points
+    angle_sep = np.arccos(1 - (sep ** 2 / (0.5 * (r_max - r_min) ** 2)))
+    th_range = np.arange(-np.pi, np.pi, angle_sep)
+    ph_range = np.arange(0, np.pi/2, angle_sep)
+    rr, tt, pp = np.meshgrid(r_range, th_range, ph_range)
+    # convert to Cartesian coodinates
+    xx = rr * np.sin(tt) * np.cos(pp)
+    yy = rr * np.sin(tt) * np.sin(pp)
+    zz = rr * np.cos(tt)
+    return np.transpose([xx.reshape(-1), yy.reshape(-1), zz.reshape(-1)])
+
+
+def rot3D(A, alpha=0., beta=0., gamma=0.):
+    r"""Rotate 3D vector A by euler angles
+        A = rot3D(A,alpha=0.,beta=0.,gamma=0.)
+       where alpha = angle from X axis to Y axis (Yaw)
+             beta  = angle from Z axis to X axis (Pitch)
+             gamma = angle from Y axis to Z axis (Roll)
+       angles in degrees
+       In a right-handed coordinate system.
+           Z
+          /|\
+           |
+           |________\Y
+           \        /
+            \
+            _\/X
+    """
+
+    A = np.asarray(A, dtype=float).reshape((-1, 3))
+
+    # Convert to radians
+    alpha = alpha * np.pi / 180.
+    beta = beta * np.pi / 180.
+    gamma = gamma * np.pi / 180.
+
+    # Define 3D rotation matrix
+    Rx = np.array([[1, 0, 0], [0, np.cos(gamma), -np.sin(gamma)], [0., np.sin(gamma), np.cos(gamma)]])
+    Ry = np.array([[np.cos(beta), 0., np.sin(beta)], [0., 1., 0.], [-np.sin(beta), 0., np.cos(beta)]])
+    Rz = np.array([[np.cos(alpha), -np.sin(alpha), 0.], [np.sin(alpha), np.cos(alpha), 0.], [0., 0., 1.]])
+    R = np.dot(np.dot(Rx, Ry), Rz)
+
+    # Rotate coordinates
+    return np.dot(R, A.T).T
+
+
+def rotmat(a, b):
+    """
+    Determine rotation matrix from a to b
+    From Kuba Ober's answer on stackexchange:
+    http://math.stackexchange.com/questions/180418/calculate-rotation-matrix-to-align-vector-a-to-vector-b-in-3d/476311#476311
+    Usage:
+     a = [1,0,0]
+     b = [0,1,0]
+     U = rotmat(a,b)
+     np.dot(U,a)
+     >> [0,1,0]
+    """
+
+    a = norm(a)
+    b = norm(b)
+
+    d = np.dot(a, b)
+    c = mag(np.cross(a, b))
+    G = np.array([[d, -c, 0], [c, d, 0], [0, 0, 1]])
+
+    u = a
+    v = norm(b - np.dot(a, b) * a)
+    w = np.cross(b, a)
+
+    Fm1 = np.array([u, v, w]).T
+    F = np.linalg.inv(Fm1)
+    U = np.dot(np.dot(Fm1, G), F)
+
+    # print('a = {}\nb = {}'.format(str(a),str(b)))
+    # print('G = {}\nFm1 = {}\nF = {}\nU = {}'.format(str(G),str(Fm1),str(F),str(U)))
+    return U
+
+
+def rotate_about_axis(point, axis, angle):
+    """
+    Rotate vector A about vector Axis by angle
+    Using Rodrigues' rotation formula: https://en.wikipedia.org/wiki/Rodrigues%27_rotation_formula
+    :param point: [x,y,z] coordinate to rotate
+    :param axis: [dx,dy,dz] vector about which to rotate
+    :param angle: angle to rotate in deg
+    :return: [x,y,z] rotated point
+    """
+    point = np.asarray(point, dtype=float)
+    axis = np.asarray(axis, dtype=float) / np.sqrt(np.sum(np.square(axis)))
+    rad = np.deg2rad(angle)
+    cs = np.cos(rad)
+    sn = np.sin(rad)
+    return point * cs + np.cross(axis, point) * sn + axis * np.dot(axis, point) * (1 - cs)
+
+
+def you_normal_vector(eta=0, chi=90, mu=0):
+    """
+    Determine the normal vector using the You diffractometer angles
+      you_normal_vector(0, 0, 0) = [1, 0, 0]
+      you_normal_vector(0, 90, 0) = [0, 1, 0]
+      you_normal_vector(90, 90, 0) = [0, 0, -1]
+      you_normal_vector(0, 0, 90) = [0, 0, -1]
+    :param eta: angle (deg) along the x-axis
+    :param mu: angle (deg) about the z-axis
+    :param chi: angle deg) a
+    :return: array
+    """
+    eta = np.deg2rad(eta)
+    chi = np.deg2rad(chi)
+    mu = np.deg2rad(mu)
+    normal = np.array([np.sin(mu) * np.sin(eta) * np.sin(chi) + np.cos(mu) * np.cos(chi),
+                       np.cos(eta) * np.sin(chi),
+                       -np.cos(mu) * np.sin(eta) * np.sin(chi) - np.sin(mu) * np.cos(chi)])
+    return normal
+
+
+def normal_basis(vec, normal=(1, 0, 0), azi=0):
+    """
+    Return a vector basis with 3 normal vectors such that:
+        [|normal x vec|, |vec x (normal x vec)|, |vec|]
+    if azi is given, the resulting vectors [0,1] will be rotated about [2]
+    :param vec: [3*1] array of vector
+    :param normal: [3*1] array of normal vector
+    :param azi: float azimuthal rotation about vec in degrees
+    :return: array [3*3] as unit vectors [vec1, vec2, vec3]
+    """
+    # U1 || projection of normal vector
+    # U2 _|_ U1,U3
+    # U3 || vec
+    vec = norm(vec)  # || vec
+    AxQ = norm(np.cross(normal, vec))
+    Ihat = norm(np.cross(vec, AxQ))  # || to normal
+    Jhat = norm(np.cross(vec, Ihat))  # -| to I and vec
+
+    # Rotate psi about Qhat
+    razi = np.deg2rad(azi)
+    # -ve sin makes clockwise rotation
+    Ihat_psi = norm(np.cos(razi) * Ihat - np.sin(razi) * Jhat)
+    Jhat_psi = norm(np.cross(vec, Ihat_psi))
+    return np.vstack([Ihat_psi, Jhat_psi, vec])
+
+
+def group(A, tolerance=0.0001):
+    """
+    Group similear values in an array, returning the group and indexes
+    array will be sorted so lowest numbers are grouped first
+      group_index, group_values, group_counts = group([2.1, 3.0, 3.1, 1.00], 0.1)
+    group_values = [1., 2., 3.] array of grouped numbers (rounded)
+    array_index = [1, 2, 2, 0] array matching A values to groups, such that A ~ group_values[group_index]
+    group_index = [3, 0, 1] array matching group values to A, such that group_values ~ A[group_index]
+    group_counts = [1, 1, 2] number of iterations of each item in group_values
+    :param A: list or numpy array of numbers
+    :param tolerance: values within this number will be grouped
+    :return: group_values, array_index, group_index, group_counts
+    """
+    A = np.asarray(A, dtype=float).reshape(-1)
+    idx = np.argsort(A)
+    rtn_idx = np.argsort(idx)
+    A2 = np.round(A / tolerance) * tolerance
+    groups, indices, inverse, counts = np.unique(A2[idx], return_index=True, return_inverse=True, return_counts=True)
+    # groups = A[idx][indices]  # return original, not rounded values
+    array_index = inverse[rtn_idx]
+    group_index = idx[indices]
+    return groups, array_index, group_index, counts
+
+
+def unique_vector(vecarray, tol=0.05):
+    """
+    Find unique vectors in an array within a certain tolerance
+
+    newarray,uniqueidx,matchidx = unique_vector(vecarray,tol=0.05)
+       vecarray = np.array([[:]])
+       newarray = vecarray with duplicate vectors removed
+       uniqueidx= index vectors of newarray such that vecarray[uniqueidx]=newarray
+       matchidx = index vectors of vecarray such that newarray[matchidx]=vecarray
+       tol = tolerance of vector difference to define unique vectors
+
+    E.G.
+    vecarray = [[1,1,1],[2,2,2],[3,3,3],[1,1,1],[4,4,4],[2,2,2]]
+    newarray,uniqueidx,matchidx = unique_vector(vecarray,tol=0.05)
+      newarray:        uniqueidx:
+     [[1, 1, 1],           [0,
+      [2, 2, 2],            1,
+      [3, 3, 3],            2,
+      [4, 4, 4]]            4]
+
+    matchidx: [0, 1, 2, 0, 3, 1]
+
+    E.G.
+    newarray,uniqueidx,matchidx = unique_vector([[1,0,0],[1,0,0],[0,1,0]],tol=0.05)
+    >> newarray = [[1,0,0],[0,1,0]]
+    >> uniqueidx= [0,2]
+    >> matchidx = [0,0,1]
+    """
+
+    vecarray = np.asarray(vecarray).reshape([len(vecarray), -1])
+    matchidx = -np.ones(len(vecarray), dtype=int)
+    Nunique = 0
+    for n in range(len(vecarray)):
+        if matchidx[n] > -1: continue
+        diff = mag(vecarray - vecarray[n])
+        matchidx[diff < tol] = Nunique
+        Nunique += 1
+    matchidx = matchidx.tolist()
+    uniqueidx = [matchidx.index(n) for n in range(np.max(matchidx) + 1)]
+    newarray = vecarray[uniqueidx, :]
+    return newarray, uniqueidx, matchidx
+
+
+def unique_vectors_fast(vecarray, tol):
+    """
+
+    :param vecarray:
+    :param tol:
+    :return:
+    """
+    vecarray = np.asarray(vecarray).reshape([len(vecarray), -1])
+    vecarray_int = ((1/tol) * vecarray).astype(int)  # convert to int
+    _, uniqueidx, matchidx = np.unique(vecarray_int, return_index=True, return_inverse=True, axis=0)
+    return vecarray[uniqueidx], uniqueidx, matchidx
+
+
+def vectorinvector(vecarray1, vecarray2, tol=0.05):
+    """
+    Return True if vecarray1 is replicated in vecarray2
+    :param vecarray1: [1xn] list or array
+    :param vecarray2: [mxn] list or array
+    :param tol: float
+    :return: Bool
+    """
+    vecarray1 = np.asarray(vecarray1)
+    vecarray2 = np.asarray(vecarray2)
+    if len(vecarray2) == 0: return False
+    diff = mag(vecarray1 - vecarray2)
+    return True if np.any(diff < tol) else False
+
+
+def distance2line(line_start, line_end, point):
+    """
+    Calculate distance from a line between the start and end to an arbitary point in space
+    :param line_start: array, position of the start of the line
+    :param line_end:  array, position of the end of the line
+    :param point: array, arbitary position in space
+    :return: float
+    """
+    line_start = np.asarray(line_start)
+    line_end = np.asarray(line_end)
+    point = np.asarray(point)
+
+    line_diff = line_end - line_start
+    unit_line = line_diff / np.sqrt(np.sum(line_diff ** 2))
+
+    vec_arb = (line_start - point) - np.dot((line_start - point), unit_line) * unit_line
+    return np.sqrt(np.sum(vec_arb ** 2))
+
+
+def vector_intersection(point1, direction1, point2, direction2):
+    """
+    Calculate the point in 2D where two lines cross.
+    If lines are parallel, return nan
+    For derivation, see: http://paulbourke.net/geometry/pointlineplane/
+    :param point1: [x,y] some coordinate on line 1
+    :param direction1: [dx, dy] the direction of line 1
+    :param point2: [x,y] some coordinate on line 2
+    :param direction2: [dx, dy] the direction of line 2
+    :return: [x, y]
+    """
+
+    point1 = np.asarray(point1)
+    point2 = np.asarray(point2)
+    direction1 = np.asarray(direction1) / np.sqrt(np.sum(np.square(direction1)))
+    direction2 = np.asarray(direction2) / np.sqrt(np.sum(np.square(direction2)))
+
+    mat = np.array([direction1, -direction2])
+    try:
+        inv = np.linalg.inv(mat)
+    except np.linalg.LinAlgError:
+        print('Vectors are parallel')
+        return np.array([np.nan, np.nan])
+    ua, ub = np.dot(point2 - point1, inv)
+    intersect = point1 + ua*direction1
+    return intersect
+
+
+def vector_intersection3d(point1, direction1, point2, direction2):
+    """
+    Calculate the point in 3D where two lines cross.
+    If lines are parallel, return nan
+    For derivation, see: https://math.stackexchange.com/questions/270767/find-intersection-of-two-3d-lines/271366
+    :param point1: [x,y,z] some coordinate on line 1
+    :param direction1: [dx, dy, dz] the direction of line 1
+    :param point2: [x,y,z] some coordinate on line 2
+    :param direction2: [dx, dy, dz] the direction of line 2
+    :return: [x, y, z]
+    """
+
+    point1 = np.asarray(point1)
+    point2 = np.asarray(point2)
+    direction1 = np.asarray(direction1)/np.sqrt(np.sum(np.square(direction1)))
+    direction2 = np.asarray(direction2)/np.sqrt(np.sum(np.square(direction2)))
+
+    line = point2 - point1
+    c1 = np.cross(direction2, line)
+    c2 = np.cross(direction2, direction1)
+    h = mag(c1)
+    k = mag(c2)
+    a = ang(c1, c2)
+    if h == 0 or k == 0:
+        print('Lines parallel')
+        return np.array([np.nan, np.nan, np.nan])
+    v = (h/k) * direction1
+    if np.abs(a) < np.pi/2:
+        return point1 + v
+    return point1 - v
+
+
+def plane_intersection(line_point, line_direction, plane_point, plane_normal):
+    """
+    Calculate the point at which a line intersects a plane
+    :param line_point: [x,y],z] some coordinate on line
+    :param line_direction: [dx,dy],dz] the direction of line
+    :param plane_point:  [x,y],z] some coordinate on the plane
+    :param plane_normal: [dx,dy],dz] the normal vector of the plane
+    :return: [x,y],z]
+    """
+
+    line_point = np.asarray(line_point)
+    plane_point = np.asarray(plane_point)
+    line_direction = np.asarray(line_direction) / np.sqrt(np.sum(np.square(line_direction)))
+    plane_normal = np.asarray(plane_normal) / np.sqrt(np.sum(np.square(plane_normal)))
+
+    u1 = np.dot(plane_normal, plane_point - line_point)
+    u2 = np.dot(plane_normal, line_direction)
+
+    if u2 == 0:
+        print('Plane is parallel to line')
+        return None
+    u = u1 / u2
+    intersect = line_point + u*line_direction
+    return intersect
+
+
+def find_index(A, value):
+    """
+    Return the index of the closest number in array A to value
+
+    E.G.
+    A = [1,2,3,4,5]
+    find_index(A,3.5)
+     >> 2
+    A = [[1,2],[3,4]]
+    find_index(A,3.2)
+     >> (1,0)
+
+     For multiple values, use:
+     B = [find_index(A,x) for x in values]
+    """
+    A = np.asarray(A, dtype=float)
+    idx = np.argmin(np.abs(A - value))
+    if len(A.shape) < 2:
+        return idx
+    else:
+        return np.unravel_index(idx, A.shape)
+
+
+def find_vector(A, V, difference=0.01):
+    """
+    Return the index(s) of vectors in array A within difference of vector V
+    Comparison is based on vector difference A[n,:]-V
+
+    Returns [] if no matching vector is present.
+
+    E.G.
+    A = [[1,2,3],
+         [4,5,6],
+         [7,8,9]]
+    find_index(A,[4,5,6])
+     >> [1]
+
+    A = [[0, 2.5, 0],
+         [1, 0.1, 0],
+         [1,-0.1, 0],
+         [0, 0.5, ]]
+    find_vector(A, [1,0,0], difference=0.1)
+     >> [1, 2]
+    """
+    A = np.asarray(A).reshape((-1, np.shape(A)[-1]))
+    V = np.asarray(V).reshape(-1)
+    return np.flatnonzero(mag(A - V) < difference)
+
+
+def search_dict_lists(d, **kwargs):
+    """
+    Search equal length lists in a dictionary for specific values
+    e.g.
+        idx = search_dict_lists(cif, _geom_bond_atom_site_label_1='Ru1',
+                                     _geom_bond_atom_site_label_2='O1',
+                                     _geom_bond_site_symmetry_2='.')
+    :param d: dict
+    :param kwargs: keyword=item
+    :return: boolean array index
+    """
+    search = [np.array(d[key]) == value for key, value in kwargs.items()]
+    bool = np.product(search, axis=0)
+    return np.argwhere(bool).reshape(-1)
+
+
+def detail(A):
+    """
+    Prints details about the given vector,
+    including length, min, max, number of elements
+    """
+    tp = type(A)
+    print('Type: {}'.format(tp))
+    A = np.asarray(A, dtype=float)
+    size = ' x '.join([str(x) for x in A.shape])
+    mem = '%1.3g MB' % (A.nbytes * 1e-6)
+    print('Size: {} (elements={}, {})'.format(size, A.size, mem))
+    print('Min: {}, Max: {}, Mean: {}, NaNs: {}'.format(np.nanmin(A), np.nanmax(A), np.nanmean(A), np.sum(np.isnan(A))))
+
+
+def inline_help(func):
+    """Return function spec and first line of help in line"""
+    fun_name = '%s%s' % (func.__name__, inspect.signature(func))
+    fun_doc = func.__doc__.strip().split('\n')[0] if func.__doc__ else ""
+    return "%s\n\t%s" % (fun_name, fun_doc)
+
+
+def array_str(A):
+    """
+    Returns a short string with array information
+    :param A: np array
+    :return: str
+    """
+    shape = np.shape(A)
+    try:
+        amax = np.max(A)
+        amin = np.min(A)
+        amean = np.mean(A)
+        out_str = "%s max: %4.5g, min: %4.5g, mean: %4.5g"
+        return out_str % (shape, amax, amin, amean)
+    except TypeError:
+        # list of str
+        array = np.asarray(A).reshape(-1)
+        array_start = array[0]
+        array_end = array[-1]
+        out_str = "%s [%s, ..., %s]"
+        return out_str % (shape, array_start, array_end)
+
+
+def print_arrays(arrays=[]):
+    """
+    Prints values from several arrays with nice formatting
+    e.g. dgp.print_arrays(1e6*np.random.rand(5,5))
+         0   6.04e+03   2.29e+05   7.19e+05   4.74e+05   9.59e+05
+         1   9.16e+05   6.33e+05    1.6e+05   3.75e+05   3.01e+05
+         2   4.21e+04   1.78e+05   4.78e+05   7.56e+05   2.47e+05
+         3   9.26e+05   6.39e+05   3.96e+05   4.42e+05   4.52e+04
+         4   3.38e+05   4.54e+05   4.29e+05   6.34e+04   6.06e+04
+    """
+
+    # Combine all arrays into BigArray
+    BigArray = np.arange(len(arrays[0])).reshape([len(arrays[0]), -1])
+    for A in arrays:
+        BigArray = np.hstack((BigArray, np.asarray(A).reshape([len(A), -1])))
+
+    # Print BigArray
+    fmt = '{:10.3g} ' * BigArray.shape[1]
+    for n in range(len(BigArray)):
+        print(fmt.format(*BigArray[n, :]))
+
+
+def cell(lengths=[1, 1, 1], rotation=[0, 0, 0]):
+    """
+    Returns a unit CELL with vectors defined by length and rotation (Deg)
+    :param lengths:
+    :param rotation:
+    :return:
+    """
+    CELL = np.eye(3) * lengths
+    CELL = rot3D(CELL, *rotation)
+    return CELL
+
+
+def index_coordinates(A, CELL):
+    """
+    Index A(x1,y1,1) on new coordinate system B(x2,y2,z2), defined by unit vectors CELL = [A,B,C]
+      A = [[nx3]] array of vectors
+      CELL = [[3x3]] matrix of vectors [a,b,c]
+    """
+
+    A = np.asarray(A, dtype=float).reshape((-1, 3))
+    B = np.dot(A, np.linalg.inv(CELL))
+    return B
+
+
+def isincell(A, cell_centre=[0, 0, 0], CELL=cell()):
+    """
+     Return boolean of whether vector xyx is inside a cell defined by position, size and rotation
+       A = [x,y,z] or [[x1,y1,z1]] array of positions
+       cell_centre = [x,y,z] cell centre
+       CELL = [[3x3]] matrix of vectors [a,b,c]
+
+    E.G.
+       xyz = [[1,1,0],[0,0,0.5],[0.1,0,5]]
+       centre = [0,0,0]
+       CELL = cell([1,1,10],[0,0,0])
+       isinbox(xyz,centre,CELL)
+       >>> [False,True,True]
+    """
+
+    A = np.asarray(A, dtype=float).reshape((-1, 3))
+    A = A - cell_centre
+    idx = index_coordinates(A, CELL)
+    return np.all(np.abs(idx) <= 0.5, axis=1)
+
+
+def sphere_array(A, max_angle1=90, max_angle2=90, step1=1, step2=1):
+    """
+    Rotate points in array A by multiple angles
+     B = sphere_array(A, max_angle1, max_angle2, step1, step2)
+
+      A = [nx3] array of 3D coordinates
+      max_angle1 = max rotation angle
+      max_angle1 = max rotation angle
+      step1 = angular step size
+      step2 = angular step size
+
+    Each coordinate in A will be rotated by angles:
+        angles = np.arange(0, max_angle+step, step)
+    The output B will have size:
+        [len(A) * len(angles1) * len(angles2), 3]
+    """
+
+    A = np.asarray(A, dtype=float).reshape((-1, 3))
+
+    angles1 = np.arange(0, max_angle1 + step1, step1)
+    angles2 = np.arange(0, max_angle2 + step2, step2)
+    len1 = len(angles1)
+    len2 = len(angles2)
+    len3 = len(A)
+    tot_size = len1 * len2 * len3
+    OUT = np.zeros([tot_size, 3])
+    for n in range(len(angles1)):
+        for m in range(len(angles2)):
+            B = rot3D(A, 0, angles1[n], angles2[m])
+            st = n * len2 + m * len3
+            nd = n * len2 + (m + 1) * len3
+            OUT[st:nd, :] = B
+    return OUT
+
+
+def rebin_volume(volume, step=(1, 1, 1), average_points=True):
+    """
+    Rebins the array volume along 3 dimensions, taking the average of elements within each step
+    :param volume: Volume object or numpy.array with ndim==3
+    :param step: [i', j', k'] step size along each dimension
+    :param average_points: Bool, if True, averages the points along each step, otherwise just sum
+    :return: volume[i//i',j//j',k//k']
+    """
+
+    i, j, k = volume.shape
+
+    # remove trailing elements
+    vol2 = volume[:i - i % step[0], :j - j % step[1], :k - k % step[2]]
+
+    # sum pixels
+    count = 0.0
+    volsum = np.zeros(np.floor_divide(vol2.shape, step))
+    for n in range(step[0]):
+        for m in range(step[1]):
+            for o in range(step[2]):
+                count += 1.0
+                volsum += vol2[n::step[0],m::step[1],o::step[2]]
+    if average_points:
+        return volsum / count  # Take the average
+    return volsum
+
+
+'---------------------------String manipulation-------------------------'
+
+
+def stfm(val, err):
+    """
+    Create standard form string from value and uncertainty"
+     str = stfm(val,err)
+     Examples:
+          '35.25 (1)' = stfm(35.25,0.01)
+          '110 (5)' = stfm(110.25,5)
+          '0.0015300 (5)' = stfm(0.00153,0.0000005)
+          '1.56(2)E+6' = stfm(1.5632e6,1.53e4)
+
+    Notes:
+     - Errors less than 0.01% of values will be given as 0
+     - The maximum length of string is 13 characters
+     - Errors greater then 10x the value will cause the value to be rounded to zero
+    """
+
+    # Determine the number of significant figures from the error
+    if err == 0. or val / float(err) >= 1E5:
+        # Zero error - give value to 4 sig. fig.
+        out = '{:1.5G}'.format(val)
+        if 'E' in out:
+            out = '{}(0)E{}'.format(*out.split('E'))
+        else:
+            out = out + ' (0)'
+        return out
+    elif np.log10(np.abs(err)) > 0.:
+        # Error > 0
+        sigfig = np.ceil(np.log10(np.abs(err))) - 1
+        dec = 0.
+    elif np.isnan(err):
+        # nan error
+        return '{} (-)'.format(val)
+    else:
+        # error < 0
+        sigfig = np.floor(np.log10(np.abs(err)) + 0.025)
+        dec = -sigfig
+
+    # Round value and error to the number of significant figures
+    rval = round(val / (10. ** sigfig)) * (10. ** sigfig)
+    rerr = round(err / (10. ** sigfig)) * (10. ** sigfig)
+    # size of value and error
+    pw = np.floor(np.log10(np.abs(rval)))
+    pwr = np.floor(np.log10(np.abs(rerr)))
+
+    max_pw = max(pw, pwr)
+    ln = max_pw - sigfig  # power difference
+
+    if np.log10(np.abs(err)) < 0:
+        rerr = err / (10. ** sigfig)
+
+    # Small numbers - exponential notation
+    if max_pw < -3.:
+        rval = rval / (10. ** max_pw)
+        fmt = '{' + '0:1.{:1.0f}f'.format(ln) + '}({1:1.0f})E{2:1.0f}'
+        return fmt.format(rval, rerr, max_pw)
+
+    # Large numbers - exponential notation
+    if max_pw >= 4.:
+        rval = rval / (10. ** max_pw)
+        rerr = rerr / (10. ** sigfig)
+        fmt = '{' + '0:1.{:1.0f}f'.format(ln) + '}({1:1.0f})E+{2:1.0f}'
+        return fmt.format(rval, rerr, max_pw)
+
+    fmt = '{' + '0:0.{:1.0f}f'.format(dec + 0) + '} ({1:1.0f})'
+    return fmt.format(rval, rerr)
+
+
+def readstfm(string):
+    """
+    Read numbers written in standard form: 0.01(2), return value and error
+    Read numbers from string with form 0.01(2), returns floats 0.01 and 0.02
+    Errors and values will return 0 if not given.
+
+    E.G.
+    readstfm('0.01(2)') = (0.01, 0.02)
+    readstfm('1000(300)') = (1000.,300.)
+    readstfm('1.23(3)E4') = (12300.0, 300.0)
+    """
+
+    values = re.findall(r'[-0-9.]+|\([-0-9.]+\)', string)
+    if len(values) > 0 and '(' not in values[0] and values[0] != '.':
+        value = values[0]
+    else:
+        value = '0'
+
+    # Determine number of decimal places for error
+    idx = value.find('.')  # returns -1 if . not found
+    if idx > -1:
+        pp = idx - len(value) + 1
+    else:
+        pp = 0
+    value = float(value)
+
+    error = re.findall(r'\([-0-9.]+\)', string)
+    if len(error) > 0:
+        error = abs(float(error[0].strip('()')))
+        error = error * 10 ** pp
+    else:
+        error = 0.
+
+    power = re.findall(r'(?:[eE]|x10\^|\*10\^|\*10\*\*)([+-]?\d*\.?\d+)', string)
+    if len(power) > 0:
+        power = float(power[0])
+        value = value * 10 ** power
+        error = error * 10 ** power
+    return value, error
+
+
+def saveable(string):
+    """
+    Returns a string without special charaters.
+    Removes bad characters from a string, so it can be used as a filename
+    E.G.
+    saveable('Test#1<froot@5!') = 'TestS1_froot_5'
+    """
+    # Special - replace # with S for scans
+    string = string.replace('#', 'S')
+    # Replace some characters with underscores
+    for char in r'#%{}\/<>@|':
+        string = string.replace(char, '_')
+        # Replace other characters with nothing
+    for char in '*$&^?!':
+        string = string.replace(char, '')
+    # Remove non-ascii characters
+    string = ''.join(i for i in string if ord(i) < 128)
+    # string = string.decode('unicode_escape').encode('ascii','ignore')
+    return string
+
+
+def findranges(scannos, sep=':'):
+    """
+    Convert a list of numbers to a simple string
+    E.G.
+    findranges([1,2,3,4,5]) = '1:5'
+    findranges([1,2,3,4,5,10,12,14,16]) = '1:5,10:2:16'
+    """
+
+    scannos = np.sort(scannos).astype(int)
+
+    dif = np.diff(scannos)
+
+    stt, stp, rng = [scannos[0]], [dif[0]], [1]
+    for n in range(1, len(dif)):
+        if scannos[n + 1] != scannos[n] + dif[n - 1]:
+            stt += [scannos[n]]
+            stp += [dif[n]]
+            rng += [1]
+        else:
+            rng[-1] += 1
+    stt += [scannos[-1]]
+    rng += [1]
+
+    out = []
+    x = 0
+    while x < len(stt):
+        if rng[x] == 1:
+            out += ['{}'.format(stt[x])]
+            x += 1
+        elif stp[x] == 1:
+            out += ['{}{}{}'.format(stt[x], sep, stt[x + 1])]
+            x += 2
+        else:
+            out += ['{}{}{}{}{}'.format(stt[x], sep, stp[x], sep, stt[x + 1])]
+            x += 2
+    return ','.join(out)
+
+
+def str2array(string):
+    """Convert string to array"""
+    string = string.replace(',', ' ')  # remove commas
+    string = string.replace('(', '').replace(')', '')  # remove brackets
+    string = string.replace('[', '').replace(']', '')  # remove brackets
+    return np.fromstring(string, sep=' ')
+
+
+def numbers2string(scannos, sep=':'):
+    """
+    Convert a list of numbers to a simple string
+    E.G.
+    numbers2string([50001,50002,50003]) = '5000[1:3]'
+    numbers2string([51020,51030,51040]) = '510[20:10:40]'
+    """
+
+    if type(scannos) is str or type(scannos) is int or len(scannos) == 1:
+        return str(scannos)
+
+    scannos = np.sort(scannos).astype(str)
+
+    n = len(scannos[0])
+    while np.all([scannos[0][:-n] == x[:-n] for x in scannos]):
+        n -= 1
+
+    if n == len(scannos[0]):
+        return '{}-{}'.format(scannos[0], scannos[-1])
+
+    inistr = scannos[0][:-(n + 1)]
+    strc = [i[-(n + 1):] for i in scannos]
+    liststr = findranges(strc, sep=sep)
+    return '{}[{}]'.format(inistr, liststr)
+
+
+def complex2str(val, fmt='6.1f'):
+    """
+    Convert complex number to string
+    """
+
+    rl = np.real(val)
+    im = np.imag(val)
+    fmt1 = '%' + fmt
+    fmt2 = '%-' + fmt
+    if im >= 0:
+        return (fmt1 + ' + i' + fmt2) % (rl, im)
+    elif im < 0:
+        return (fmt1 + ' - i' + fmt2) % (rl, np.abs(im))
+
+
+def multi_replace(string, old=[], new=[]):
+    """
+    Replace multiple strings at once
+    :param string:
+    :param old:
+    :param new:
+    :return:
+    """
+
+    if type(new) is str:
+        new = [new]
+    if type(old) is str:
+        old = [old]
+    if len(new) == 1:
+        new = new * len(old)
+    for i, j in zip(old, new):
+        string = string.replace(i, j)
+    return string
+
+
+def replace_bracket_multiple(name):
+    """
+    Replace any numbers in brackets with numbers multipled by bracket multiplyer
+    Assumes bracket multiplier is on the left side
+    e.g.
+        replace_bracket_multiple('Mn0.3(Fe3.6(Co1.2)2)4(Mo0.7Pr44)3')
+        >> 'Mn0.3Fe14.4Co9.6Mo2.1Pr132'
+    :param name: str
+    :return: str
+    """
+    """
+    To do:
+     - Multiply by fraction (regex for '/number')
+     - Multiple on right hand side
+    """
+    # Regex:
+    regex_num = re.compile(r'[\d\.]+')
+    regex_bracket_n = re.compile(r'\)[\d\.]+')
+
+    # Find outside brackets
+    bracket = []
+    start_idx = []
+    level = 0
+    for n, s in enumerate(name):
+        if s in ['(', '[', '{']:
+            start_idx += [n]
+            level += 1
+        elif s in [')', ']', '}']:
+            level -= 1
+            if level == 0:
+                num = regex_bracket_n.findall(name[n:])
+                if len(num) > 0:
+                    bracket_end = n + len(num[0])
+                    num = float(num[0][1:])
+                else:
+                    bracket_end = n + 1
+                    num = 1.0
+                bracket += [(
+                    name[start_idx[0] + 1:n],  # insde brackets
+                    name[start_idx[0]:bracket_end],  # str to replace
+                    num  # multiplication appending bracket
+                )]
+                start_idx = []
+
+    for numstr, repstr, num in bracket:
+        # Run recursivley to get inner brackets
+        numstr = replace_bracket_multiple(numstr)
+        # Replace each number by it's multiple
+        for oldnum in regex_num.findall(numstr):
+            numstr = numstr.replace(oldnum, '%0.3g' % (float(oldnum) * num))
+        # Replace in original string
+        name = name.replace(repstr, numstr)
+    return name
+
+
+def shortstr(string):
+    """
+    Shorten string by removing long floats
+    :param string: string, e.g. '#810002 scan eta 74.89533603616637 76.49533603616636 0.02 pil3_100k 1 roi2'
+    :return: shorter string, e.g. '#810002 scan eta 74.895 76.495 0.02 pil3_100k 1 roi2'
+    """
+    #return re.sub(r'(\d\d\d)\d{4,}', r'\1', string)
+    def subfun(m):
+        return str(round(float(m.group()), 3))
+    return re.sub(r'\d+\.\d{5,}', subfun, string)
+
+
+def nice_print(precision=4, linewidth=300):
+    """
+    Sets default printing of arrays to a nicer format
+    """
+    np.set_printoptions(precision=precision, suppress=True, linewidth=linewidth)
+
+
+'----------------------------------Others-------------------------------'
+
+
+def gauss(x, y=None, height=1, centre=0, fwhm=0.5, bkg=0, centre_y=None, fwhm_y=None):
+    """
+    Define a Gaussian distribution in 1 or 2 dimensions
+
+        g = height * exp( -ln2 (x-centre)^2 / (fwhm/2)^2 ) + bkg
+    From http://fityk.nieto.pl/model.html
+
+        x = [1xn] array of values, defines size of gaussian in dimension 1
+        y = None* or [1xm] array of values, defines size of gaussian in dimension 2
+        height = peak height
+        centre = peak centre
+        fwhm = peak full width at half-max
+        bkg = background
+        centre_y = if 2D, centre along the y-axis (defaults to centre)
+        fwhm_y = if 2D, fwhm along the y-axis (defaults to fwhm)
+    """
+
+    if centre_y is None:
+        centre_y = centre
+    if fwhm_y is None:
+        fwhm_y = fwhm
+    if y is None:
+        y = centre_y
+
+    x = np.asarray(x, dtype=float).reshape([-1])
+    y = np.asarray(y, dtype=float).reshape([-1])
+    X, Y = np.meshgrid(x, y)
+    Px = (X - centre) ** 2 / (fwhm / 2) ** 2
+    Py = (Y - centre_y) ** 2 / (fwhm_y / 2) ** 2
+    g = height * np.exp(-np.log(2) * (Px + Py)) + bkg
+
+    if len(y) == 1:
+        g = g.reshape([-1])
+    return g
+
+
+def lorentz(x, y=None, height=1, centre=0, fwhm=0.5, bkg=0, centre_y=None, fwhm_y=None):
+    """
+    Define a Lorentzian distribution in 1 or 2 dimensions
+
+        l = height / ( 1 + (x - centre)^2 / (fwhm/2)^2 + bkg
+
+        x = [1xn] array of values, defines size of gaussian in dimension 1
+        y = None* or [1xm] array of values, defines size of gaussian in dimension 2
+        height = peak height
+        centre = peak centre
+        fwhm = peak full width at half-max
+        bkg = background
+        centre_y = if 2D, centre along the y-axis (defaults to centre)
+        fwhm_y = if 2D, fwhm along the y-axis (defaults to fwhm)
+    """
+
+    if centre_y is None:
+        centre_y = centre
+    if fwhm_y is None:
+        fwhm_y = fwhm
+    if y is None:
+        y = centre_y
+
+    sigma_x = fwhm / 2.
+    sigma_y = fwhm_y / 2.
+
+    x = np.asarray(x, dtype=float).reshape([-1])
+    y = np.asarray(y, dtype=float).reshape([-1])
+    X, Y = np.meshgrid(x, y)
+    Px = (X - centre) ** 2 / sigma_x ** 2
+    Py = (Y - centre_y) ** 2 / sigma_y ** 2
+    lz = height / (1 + Px + Py) + bkg
+
+    if len(y) == 1:
+        lz = lz.reshape([-1])
+    return lz
+
+
+def pvoight(x, y=None, height=1, centre=0, fwhm=0.5, bkg=0, l_fraction=0.5, centre_y=None, fwhm_y=None):
+    """
+    Define psuedo-voight distribution in 1 or 2 dimensions
+
+        v = fraction * lorentz() + (1 - fraction) * gauss()
+
+        x = [1xn] array of values, defines size of gaussian in dimension 1
+        y = None* or [1xm] array of values, defines size of gaussian in dimension 2
+        height = peak height
+        centre = peak centre
+        fwhm = peak full width at half-max
+        bkg = background
+        l_fraction = Lorentzian fraction (0-1)
+        centre_y = if 2D, centre along the y-axis (defaults to centre)
+        fwhm_y = if 2D, fwhm along the y-axis (defaults to fwhm)
+    """
+    g = gauss(x, y, height=height, centre=centre, fwhm=fwhm, bkg=bkg, centre_y=centre_y, fwhm_y=fwhm_y)
+    l = lorentz(x, y, height=height, centre=centre, fwhm=fwhm, bkg=bkg, centre_y=centre_y, fwhm_y=fwhm_y)
+    return (1 - l_fraction) * g + l_fraction * l
+
+
+def peak_function(func_name, *args, **kwargs):
+    """
+    Choose & create peak function, using either gaussian, lorentzian or pseudo-voight
+    :param func_name: 'gaussian', 'lorentzian', 'psudovoight' (raise ValueError if wrong)
+    :param args: x, y, height, centre, fwhm, bkg, (fraction), centre_y, fwhm_y
+    :param kwargs:
+    :return: array()
+    """
+    func_name = func_name.lower().replace(' ', '').replace('-', '')
+    if 'gauss' in func_name:
+        return gauss(*args, **kwargs)
+    if 'lorentz' in func_name:
+        return lorentz(*args, **kwargs)
+    if 'voight' in func_name:
+        return pvoight(*args, **kwargs)
+    raise ValueError('%s not available as peak function.' % func_name)
+
+
+def frange(start, stop=None, step=1):
+    """
+    Returns a list of floats from start to stop in step increments
+    Like np.arange but ends at stop, rather than at stop-step
+    E.G.
+    A = frange(0,5,1) = [0.,1.,2.,3.,4.,5.]
+    """
+    if stop is None:
+        stop = start
+        start = 0
+
+    return list(np.arange(start, stop + 0.00001, step, dtype=float))
+
+
+def squaredata(xdata, ydata, data, repeat=None):
+    """
+    Generate square arrays from 1D data, automatically determinging the repeat value
+    :param xdata: [n] array
+    :param ydata: [n] array
+    :param data: [n] array
+    :param repeat: int m or None to deteremine m from differences in xdata and y data
+    :return: X, Y, D [n//m, m] arrays
+    """
+
+    if repeat is None:
+        # Determine the repeat length of the scans
+        delta_x = np.abs(np.diff(xdata))
+        ch_idx_x = np.where(delta_x > delta_x.max() * 0.9)  # find biggest changes
+        ch_delta_x = np.diff(ch_idx_x)
+        rep_len_x = np.round(np.mean(ch_delta_x))
+        delta_y = np.abs(np.diff(ydata))
+        ch_idx_y = np.where(delta_y > delta_y.max() * 0.9)  # find biggest changes
+        ch_delta_y = np.diff(ch_idx_y)
+        rep_len_y = np.round(np.mean(ch_delta_y))
+        repeat = int(max(rep_len_x, rep_len_y))
+    xsquare = xdata[:repeat * (len(xdata) // repeat)].reshape(-1, repeat)
+    ysquare = ydata[:repeat * (len(ydata) // repeat)].reshape(-1, repeat)
+    dsquare = data[:repeat * (len(data) // repeat)].reshape(-1, repeat)
+    return xsquare, ysquare, dsquare
+
+
+def grid_intensity(points, values, resolution=0.01, peak_width=0.1, background=0):
+    """
+    Generates array of intensities along a spaced grid, equivalent to a powder pattern.
+      grid, values = generate_powder(points, values, resolution=0.01, peak_width=0.1, background=0)
+    :param points: [nx1] position of values to place on grid
+    :param values: [nx1] values to place at points
+    :param resolution: grid spacing size, with same units as points
+    :param peak_width: width of convolved gaussian, with same units as points
+    :param background: add a normal (random) background with width sqrt(background)
+    :return: points, values
+    """
+
+    points = np.asarray(points, dtype=float)
+    values = np.asarray(values, dtype=float)
+
+    # create plotting mesh
+    grid_points = np.arange(np.min(points) - 50 * resolution, np.max(points) + 50 * resolution, resolution)
+    pixels = len(grid_points)
+    grid_values = np.zeros([pixels])
+
+    # add reflections to background
+    pixel_size = (grid_points.max() - grid_points.min()) / pixels
+    peak_width_pixels = peak_width / (1.0 * pixel_size)
+
+    pixel_coord = (points - grid_points.min()) / (grid_points - grid_points.min()).max()
+    pixel_coord = (pixel_coord * (pixels - 1)).astype(int)
+    pixel_coord = pixel_coord.astype(int)
+
+    for n in range(0, len(values)):
+        grid_values[pixel_coord[n]] = grid_values[pixel_coord[n]] + values[n]
+
+    # Convolve with a gaussian (if >0 or not None)
+    if peak_width:
+        gauss_x = np.arange(-3 * peak_width_pixels, 3 * peak_width_pixels + 1)  # gaussian width = 2*FWHM
+        g = gauss(gauss_x, None, height=1, centre=0, fwhm=peak_width_pixels, bkg=0)
+        grid_values = np.convolve(grid_values, g, mode='same')
+
+    # Add background (if >0 or not None)
+    if background:
+        bkg = np.random.normal(background, np.sqrt(background), [pixels])
+        grid_values = grid_values + bkg
+    return grid_points, grid_values
+
+
+def map2grid(grid, points, values, widths=None, background=0):
+    """
+    Generates array of intensities along a spaced grid, equivalent to a powder pattern.
+      grid, values = generate_powder(points, values, resolution=0.01, peak_width=0.1, background=0)
+    :param grid: [mx1] grid of positions
+    :param points: [nx1] position of values to place on grid
+    :param values: [nx1] values to place at points
+    :param widths: width of convolved gaussian, with same units as points
+    :param background: add a normal (random) background with width sqrt(background)
+    :return: points, values
+    """
+    grid = np.asarray(grid, dtype=float)
+    points = np.asarray(points, dtype=float)
+    values = np.asarray(values, dtype=float)
+    widths = np.asarray(widths, dtype=float)
+
+    if widths.size == 1:
+        widths = widths * np.ones(len(points))
+
+    pixels = len(grid)
+    grid_values = np.zeros([pixels])
+
+    for point, value, width in zip(points, values, widths):
+        g = gauss(grid, None, height=value, centre=point, fwhm=width, bkg=0)
+        grid_values += g
+
+    # Add background (if >0 or not None)
+    if background:
+        bkg = np.random.normal(background, np.sqrt(background), [pixels])
+        grid_values = grid_values + bkg
+    return grid_values
+
+
+def whererun():
+    """Returns the location where python was run"""
+    return os.path.abspath('.')
+
+
+def lastlines(filename, lines=1, max_line_length=255):
+    """Returns the last n lines of a text file"""
+    with open(filename, 'rb') as f:
+        f.seek(-(lines+1)*max_line_length, os.SEEK_END)
+        endlines = f.read().decode().split('\n')
+    return endlines[-lines:]
+
+
+def get_methods(object, include_special=True):
+    """Returns a list of methods (functions) within object"""
+    if include_special:
+        return [method_name for method_name in dir(object) if callable(getattr(object, method_name))]
+    return [method_name for method_name in dir(object) if callable(getattr(object, method_name)) and '__' not in method_name]
+
+
+def list_methods(object, include_special=False):
+    """Return list of methods (functions) in class object"""
+    methods = get_methods(object, include_special)
+    return '\n'.join([inline_help(getattr(object, fun)) for fun in methods])
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/functions_plotting.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/functions_plotting.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,959 +1,971 @@
-# -*- coding: utf-8 -*-
-"""
-Module: Handy plotting functions "functions_plotting.py"
-
-Contains various plotting shortcuts using matplotlib.pyplot
-
-By Dan Porter, PhD
-Diamond
-2018
-
-Usage: 
-    - Run this file in an interactive console
-    OR
-    - from Dans_Diffraction import functions_plotting as fp
-
-All plots generated require plt.show() call, unless using interactive mode
-
-
-Version 2.1
-Last updated: 10/08/22
-
-Version History:
-06/01/18 1.0    Program created from DansGeneralProgs.py V2.3
-05/03/18 1.1    Removed plt.show from arrow functions
-17/04/18 1.2    Removed plt.show from other functions
-03/05/18 1.3    Removed plot_vector_lines(vec_a,vec_b), replaced with plot_lattice_lines(Q, vec_a, vec_b)
-30/05/18 1.4    Added multiplot
-07/03/19 1.5    Added plot_attenuation and others
-22/03/19 1.6    Added plot_circle, updated vecplot and plot_lattice_lines
-03/05/19 1.7    Added legend to labels function
-09/03/20 1.8    Added default figure size
-22/11/20 1.9    Update to labels to fix 3D plotting
-15/02/21 1.9.1  Update to vecplot for plotting on axis
-27/09/21 2.0    Added plot3darray, plot_diffractometer_reciprocal_space
-10/08/22 2.1    Added plot_lattice_points3D, set_plot_defaults, changed default fig size
-
-@author: DGPorter
-"""
-
-import sys, os
-import numpy as np
-import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib.patches import FancyArrowPatch
-from mpl_toolkits.mplot3d import proj3d
-
-from . import functions_general as fg
-from . import functions_crystallography as fc
-
-__version__ = '2.1'
-
-DEFAULT_FONT = 'Times New Roman'
-DEFAULT_FONTSIZE = 14
-FIGURE_SIZE = [12, 8]
-FIGURE_DPI = 80
-
-
-'----------------------------Plot manipulation--------------------------'
-
-
-def set_plot_defaults(rcdefaults=False):
-    """
-    Set custom matplotlib rcparams, or revert to matplotlib defaults
-    These handle the default look of matplotlib plots
-    See: https://matplotlib.org/stable/tutorials/introductory/customizing.html#the-default-matplotlibrc-file
-    :param rcdefaults: False*/ True, if True, revert to matplotlib defaults
-    :return: None
-    """
-    if rcdefaults:
-        print('Return matplotlib rcparams to default settings.')
-        plt.rcdefaults()
-        return
-
-    plt.rc('figure', figsize=FIGURE_SIZE, dpi=FIGURE_DPI, autolayout=False)
-    plt.rc('lines', marker='o', color='r', linewidth=2, markersize=6)
-    plt.rc('errorbar', capsize=2)
-    plt.rc('legend', loc='best', frameon=False, fontsize=DEFAULT_FONTSIZE)
-    plt.rc('axes', linewidth=2, titleweight='bold', labelsize='large')
-    plt.rc('xtick', labelsize='large')
-    plt.rc('ytick', labelsize='large')
-    plt.rc('axes.formatter', limits=(-3, 3), offset_threshold=6)
-    plt.rc('image', cmap='viridis')  # default colourmap, see https://matplotlib.org/stable/gallery/color/colormap_reference.html
-    # Note font values appear to only be set when plt.show is called
-    plt.rc(
-        'font',
-        family='serif',
-        style='normal',
-        weight='bold',
-        size=DEFAULT_FONTSIZE,
-        serif=['Times New Roman', 'Times', 'DejaVu Serif']
-    )
-    # plt.rcParams["savefig.directory"] = os.path.dirname(__file__) # Default save directory for figures
-
-
-def labels(ttl=None, xvar=None, yvar=None, zvar=None, legend=False, size='Normal', font='Times New Roman'):
-    """
-    Add formatted labels to current plot, also increases the tick size
-    :param ttl: title
-    :param xvar: x label
-    :param yvar: y label
-    :param zvar: z label (3D plots only)
-    :param legend: False/ True, adds default legend to plot 
-    :param size: 'Normal' or 'Big'
-    :param font: str font name, 'Times New Roman'
-    :return: None
-    """
-
-    if size.lower() in ['big', 'large', 'xxl', 'xl']:
-        tik = 30
-        tit = 32
-        lab = 35
-        leg = 25
-    else:
-        # Normal
-        tik = 18
-        tit = 20
-        lab = 22
-        leg = 18
-
-    plt.xticks(fontsize=tik, fontname=font)
-    plt.yticks(fontsize=tik, fontname=font)
-    plt.setp(plt.gca().spines.values(), linewidth=2)
-    if plt.gca().get_yaxis().get_scale() != 'log' and 'linear' in plt.gca().name:
-        plt.ticklabel_format(useOffset=False)
-        plt.ticklabel_format(style='sci', scilimits=(-3,3))
-
-    if ttl is not None:
-        plt.gca().set_title(ttl, fontsize=tit, fontweight='bold', fontname=font)
-
-    if xvar is not None:
-        plt.gca().set_xlabel(xvar, fontsize=lab, fontname=font)
-
-    if yvar is not None:
-        plt.gca().set_ylabel(yvar, fontsize=lab, fontname=font)
-
-    if zvar is not None:
-        # Don't think this works, use ax.set_zaxis
-        plt.gca().set_zlabel(zvar, fontsize=lab, fontname=font)
-        for t in plt.gca().zaxis.get_major_ticks():
-            t.label.set_fontsize(tik)
-            t.label.set_fontname(font)
-
-    if legend:
-        plt.legend(loc=0, frameon=False, prop={'size': leg, 'family': 'serif'})
-
-
-def saveplot(name, dpi=None, figure=None):
-    """
-    Saves current figure as a png in the home directory
-    :param name: filename, including or expluding directory and or extension
-    :param dpi: image resolution, higher means larger image size, default=matplotlib default
-    :param figure: figure number, default = plt.gcf()
-    :return: None
-
-    E.G.
-    ---select figure to save by clicking on it---
-    saveplot('test')
-    E.G.
-    saveplot('c:\somedir\apicture.jpg', dpi=600, figure=3)
-    """
-
-    if type(name) is int:
-        name = str(name)
-
-    if figure is None:
-        gcf = plt.gcf()
-    else:
-        gcf = plt.figure(figure)
-
-    dir = os.path.dirname(name)
-    file, ext = os.path.basename(name)
-
-    if len(dir) == 0:
-        dir = os.path.expanduser('~')
-
-    if len(ext) == 0:
-        ext = '.png'
-
-    savefile = os.path.join(dir, file+ext)
-    gcf.savefig(savefile, dpi=dpi)
-    print('Saved Figure {} as {}'.format(gcf.number, savefile))
-
-
-def newplot(*args, **kwargs):
-    """
-    Shortcut to creating a simple plot
-    E.G.
-      x = np.arange(-5,5,0.1)
-      y = x**2
-      newplot(x,y,'r-',lw=2,label='Line')
-    """
-
-    if 'linewidth' and 'lw' not in kwargs.keys():
-        kwargs['linewidth'] = 2
-
-    plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
-    plt.plot(*args, **kwargs)
-
-    plt.setp(plt.gca().spines.values(), linewidth=2)
-    plt.xticks(fontsize=25, fontname='Times New Roman')
-    plt.yticks(fontsize=25, fontname='Times New Roman')
-    plt.ticklabel_format(useOffset=False)
-    plt.ticklabel_format(style='sci', scilimits=(-3, 3))
-
-
-def multiplot(xvals, yvals=None, datarange=None, cmap='jet', labels=None, marker=None):
-    """
-    Shortcut to creating a simple multiplot with either colorbar or legend
-    E.G.
-      x = np.arange(-5,5,0.1)
-      ys = [x**2, 1+x**2, 2+x**2, 3+x**2, 4+x**2]
-      datarange = [0,1,2,3,4]
-      multiplot(x, ys, datarange, cmap='winter')
-    OR:
-      x = np.arange(-5,5,0.1)
-      ys = [x**2, 1+x**2, 2+x**2, 3+x**2, 4+x**2]
-      labels = ['x*x','2+x*x','3+x*x','4+x*x']
-      multiplot(x, ys, labels=labels)
-    """
-
-    if yvals is None:
-        yvals = xvals
-        xvals = []
-    yvals = np.asarray(yvals)
-    xvals = np.asarray(xvals)
-
-    if datarange is None:
-        datarange = range(len(yvals))
-    datarange = np.asarray(datarange,dtype=float)
-
-    cm = plt.get_cmap(cmap)
-    colrange = (datarange - datarange.min()) / (datarange.max() - datarange.min())
-    
-    if marker is None:
-        marker = ''
-    linearg = '-' + marker
-
-    plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
-    for n in range(len(datarange)):
-        col = cm(colrange[n])
-        if len(xvals) == 0:
-            plt.plot(yvals[n], linearg, lw=2, color=col)
-        elif len(xvals.shape) == 1:
-            plt.plot(xvals, yvals[n], linearg, lw=2, color=col)
-        else:
-            plt.plot(xvals[n], yvals[n], linearg, lw=2, color=col)
-
-    plt.setp(plt.gca().spines.values(), linewidth=2)
-    plt.xticks(fontsize=25, fontname='Times New Roman')
-    plt.yticks(fontsize=25, fontname='Times New Roman')
-    plt.ticklabel_format(useOffset=False)
-    plt.ticklabel_format(style='sci', scilimits=(-3, 3))
-
-    if labels is None:
-        # Add Colorbar
-        sm = plt.cm.ScalarMappable(cmap=cm)
-        sm.set_array(datarange)
-        cbar = plt.colorbar(sm)
-        #cbar.set_label('variation [unit]', fontsize=24, fontweight='bold', fontname='Times New Roman')
-    else:
-        # Add legend
-        plt.legend(labels, loc=0, frameon=False, prop={'size':20,'family':'serif'})
-
-
-def newplot3(*args, **kwargs):
-    """
-    Shortcut to creating a simple 3D plot
-    Automatically tiles 1 dimensional x and y arrays to match 2D z array,
-    assuming z.shape = (len(x),len(y))
-      newplot3(x, y, z, ...)
-
-    E.G.
-      newplot3([1,2,3,4],[9,8,7],[[2,4,6],[8,10,12],[14,16,18],[20,22,24]],'-o')
-    """
-
-    if 'linewidth' and 'lw' not in kwargs.keys():
-        kwargs['linewidth'] = 2
-
-    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
-    ax = fig.add_subplot(111, projection='3d')
-
-    x = np.asarray(args[0], dtype=float)
-    y = np.asarray(args[1], dtype=float)
-    z = np.asarray(args[2], dtype=float)
-
-    if z.ndim == 2:
-        if x.ndim < 2:
-            x = np.tile(x, z.shape[1]).reshape(z.T.shape).T
-        if y.ndim < 2:
-            y = np.tile(y, z.shape[0]).reshape(z.shape)
-
-        # Plot each array independently
-        for n in range(len(z)):
-            ax.plot(x[n], y[n], z[n], *args[3:], **kwargs)
-    else:
-        ax.plot(*args, **kwargs)
-
-
-def plot3darray(vec, *args, **kwargs):
-    """
-    Plot 3D vectors in 3D
-        plt.plot(vec[:, 0], vec[:, 1], vec[:, 3], *args, **kwargs)
-    :param vec: [n*3] array
-    :param args: args to pass to plt.plot
-    :param kwargs: kwargs to pass to plt.plot
-    :return: matplotlib plot object
-    """
-    vec = np.reshape(vec, (-1, 3))
-    return plt.plot(vec[:, 0], vec[:, 1], vec[:, 2], *args, **kwargs)
-
-
-def sliderplot(YY, X=None, slidervals=None, *args, **kwargs):
-    """
-    Shortcut to creating a simple 2D plot with a slider to go through a third dimension
-    YY = [nxm]: y axis data (initially plots Y[0,:])
-     X = [n] or [nxm]:  x axis data (can be 1D or 2D, either same length or shape as Y)
-     slidervals = None or [m]: Values to give in the slider
-
-    E.G.
-      sliderplot([1,2,3],[[2,4,6],[8,10,12],[14,16,18],[20,22,24]],slidervals=[3,6,9,12])
-    """
-
-    if 'linewidth' and 'lw' not in kwargs.keys():
-        kwargs['linewidth'] = 2
-
-    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
-
-    X = np.asarray(X, dtype=float)
-    Y = np.asarray(YY, dtype=float)
-    if slidervals is None:
-        slidervals = range(Y.shape[0])
-    slidervals = np.asarray(slidervals, dtype=float)
-
-    if X.ndim < 2:
-        X = np.tile(X, Y.shape[0]).reshape(Y.shape)
-
-    plotline, = plt.plot(X[0, :], Y[0, :], *args, **kwargs)
-    plt.axis([X.min(), X.max(), Y.min(), Y.max()])
-    plt.subplots_adjust(bottom=0.2)
-    ax = plt.gca()
-
-    " Create slider on plot"
-    axsldr = plt.axes([0.15, 0.05, 0.65, 0.03], axisbg='lightgoldenrodyellow')
-
-    sldr = plt.Slider(axsldr, '', 0, len(slidervals) - 1)
-    txt = axsldr.set_xlabel('{} [{}]'.format(slidervals[0], 0), fontsize=18)
-
-    plt.sca(ax)
-
-    " Slider update function"
-
-    def update(val):
-        "Update function for pilatus image"
-        pno = int(np.floor(sldr.val))
-        plotline.set_xdata(X[pno, :])
-        plotline.set_ydata(Y[pno, :])
-        txt.set_text('{} [{}]'.format(slidervals[pno], pno))
-        plt.draw()
-        plt.gcf().canvas.draw()
-        # fig1.canvas.draw()
-
-    sldr.on_changed(update)
-
-
-def sliderplot2D(ZZZ, XX=None, YY=None, slidervals=None, *args, **kwargs):
-    """
-    Shortcut to creating an image plot with a slider to go through a third dimension
-    ZZZ = [nxmxo]: z axis data
-     XX = [nxm] or [n]:  x axis data
-     YY = [nxm] or [m]: y axis data
-     slidervals = None or [o]: Values to give in the slider
-
-    if XX and/or YY have a single dimension, the 2D values are generated via meshgrid
-
-    E.G.
-      sliderplot([1,2,3],[[2,4,6],[8,10,12],[14,16,18],[20,22,24]],slidervals=[3,6,9,12])
-    """
-
-    if 'linewidth' and 'lw' not in kwargs.keys():
-        kwargs['linewidth'] = 2
-
-    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
-
-    ZZZ = np.asarray(ZZZ, dtype=float)
-
-    if slidervals is None:
-        slidervals = range(ZZZ.shape[2])
-    slidervals = np.asarray(slidervals, dtype=float)
-
-    if XX is None:
-        XX = range(ZZZ.shape[1])
-    if YY is None:
-        YY = range(ZZZ.shape[0])
-    XX = np.asarray(XX, dtype=float)
-    YY = np.asarray(YY, dtype=float)
-    if XX.ndim < 2:
-        XX, YY = np.meshgrid(XX, YY)
-
-    p = plt.pcolormesh(XX, YY, ZZZ[:, :, 0])
-    # p.set_clim(cax)
-
-    plt.subplots_adjust(bottom=0.2)
-    ax = plt.gca()
-    ax.set_aspect('equal')
-    ax.autoscale(tight=True)
-
-    " Create slider on plot"
-    axsldr = plt.axes([0.15, 0.05, 0.65, 0.03], axisbg='lightgoldenrodyellow')
-
-    sldr = plt.Slider(axsldr, '', 0, len(slidervals) - 1)
-    txt = axsldr.set_xlabel('{} [{}]'.format(slidervals[0], 0), fontsize=18)
-
-    plt.sca(ax)
-
-    " Slider update function"
-
-    def update(val):
-        "Update function for pilatus image"
-        pno = int(np.round(sldr.val))
-        p.set_array(ZZZ[:-1, :-1, pno].ravel())
-        txt.set_text('{} [{}]'.format(slidervals[pno], pno))
-        plt.draw()
-        plt.gcf().canvas.draw()
-        # fig1.canvas.draw()
-    sldr.on_changed(update)
-
-
-def plot_cell(cell_centre=[0, 0, 0], CELL=np.eye(3), color='k'):
-    """
-    Plot a box defined by a unit cell on the current plot
-    :param cell_centre: [1x3] array : centre of cell, default [0,0,0]
-    :param CELL: [3x3] array : unit cell vectors [A,B,C]
-    :return: None
-    """
-
-    uvw = np.array([[0., 0, 0], [1, 0, 0], [1, 0, 1], [1, 1, 1], [1, 1, 0], [0, 1, 0], [0, 1, 1],
-                    [0, 0, 1], [1, 0, 1], [1, 0, 0], [1, 1, 0], [1, 1, 1], [0, 1, 1], [0, 1, 0], [0, 0, 0], [0, 0, 1]])
-    uvw = uvw - 0.5  # plot around box centre
-    bpos = np.dot(uvw, CELL)
-    bpos = bpos + cell_centre
-    plt.plot(bpos[:, 0], bpos[:, 1], bpos[:, 2], c=color)  # cell box
-
-
-def plot_circle(radius=1.0, centre=[0,0], height=0, *args, **kwargs):
-    """
-    Generate circle on current plot
-    :param radius: radius of the circle
-    :param centre: [x,y] centre of the circle
-    :param height: reduce the radius by increasing the height from a surface
-    :param args: plot commands
-    :param kwargs: plot commands
-    :return: none
-    """
-
-    deg = np.linspace(0, 360, 361)
-    rad = np.deg2rad(deg)
-    x = centre[0] + np.sqrt((radius**2-height**2))*np.cos(rad)
-    y = centre[1] + np.sqrt((radius**2-height**2))*np.sin(rad)
-    plt.plot(x, y, *args, **kwargs)
-
-
-def plot_arrow(x, y, z=None, col='r', width=2, arrow_size=40):
-    """
-    Plot arrow in 2D or 3D on current axes
-    Usage 2D:
-      plot_arrow([xi,xf],[yi,yf])
-    Usage 3D:
-      plot_arrow([xi,xf],[yi,yf],[zi,zf])
-
-    Options:
-      width = line width (Def. = 2)
-      arrow_size = size of arrow head (Def. = 40)
-      col = arrow color (Deg. = red)
-    """
-
-    # 2D Arrow
-    if z is None or not hasattr(plt.gca(), 'get_zlim'):
-        x0 = x[0]
-        y0 = y[0]
-        dx = x[1] - x[0]
-        dy = y[1] - y[0]
-
-        plt.arrow(x0, y0, dx, dy, width=arrow_size / 4000.0, color=col, length_includes_head=True)
-        # V = FancyArrowPatch(x,y, mutation_scale=arrow_size, lw=width, arrowstyle="-|>", color=col)
-        # plt.gca().add_artist(V)
-        return
-
-    # 3D Arrow
-    V = Arrow3D(x, y, z, mutation_scale=arrow_size, lw=width, arrowstyle="-|>", color=col)
-    plt.gca().add_artist(V)
-
-
-class Arrow3D(FancyArrowPatch):
-    """
-    FancyArrow3D patch for 3D arrows, by CT Zhu
-     http://stackoverflow.com/questions/22867620/putting-arrowheads-on-vectors-in-matplotlibs-3d-plot
-    Useage:
-      fig = plt.figure()
-      ax = fig.add_subplot(111, projection='3d')
-      ax.plot([0,1],[0,0],[0,0],'k-')
-      ax.plot([0,0],[0,1],[0,0],'k-')
-      ax.plot([0,0],[0,0],[0,1],'k-')
-      v = Arrow3D([0,1],[0,1],[0,1], mutation_scale=20, lw=3, arrowstyle="-|>", color="r")
-      ax.add_artist(v)
-
-    """
-
-    def __init__(self, xs, ys, zs, *args, **kwargs):
-        if 'arrowstyle' not in kwargs.keys():
-            kwargs['arrowstyle'] = "-|>"
-        if 'mutation_scale' not in kwargs.keys():
-            kwargs['mutation_scale'] = 20
-        FancyArrowPatch.__init__(self, (0, 0), (0, 0), *args, **kwargs)
-        self._verts3d = xs, ys, zs
-
-    def draw(self, renderer):
-        xs3d, ys3d, zs3d = self._verts3d
-        xs, ys, zs = proj3d.proj_transform(xs3d, ys3d, zs3d, renderer.M)
-        self.set_positions((xs[0], ys[0]), (xs[1], ys[1]))
-        FancyArrowPatch.draw(self, renderer)
-
-
-'----------------------- Crystal Plotting Programs----------------------'
-
-
-def vecplot(UV, mode='hk0', axis=None, *args, **kwargs):
-    """
-    Plot grid of a,b vectors on current axis
-    :param UV: [a;b;c] array of unit vectors
-    :param mode: definition of axis plane, 'hk0', 'h0l', '0kl', 'hhl'
-    :param axis: axis to create lines on, if None, plt.gca is used
-    :param args: arguments to pass to plot command, e.g. linewidth, alpha, color
-    :return: None
-    """
-
-    if mode == 'h0l':
-        # h0l
-        UV = np.dot(np.array([[1, 0, 0], [0, 0, 1], [0, 1, 0]]), fg.rot3D(UV, gamma=-90))
-    elif mode == '0kl':
-        # 0kl
-        UV = np.dot(np.array([[0, 1, 0], [0, 0, 1], [1, 0, 0]]), UV)
-    elif mode == 'hhl':
-        # hhl ***untested
-        UV = np.dot(np.array([[1, 1, 0], [0, 0, 1], [0, 1, 0]]), UV)
-
-    if axis is None:
-        axis = plt.gca()
-    axsize = axis.axis()
-    latt = axis_lattice_points(UV[0], UV[1], axis=axsize)
-    plot_lattice_lines(latt, UV[0], UV[1], axis=axis, *args, **kwargs)
-
-
-def UV_arrows(UV, alabel='a', blabel='b', clabel='c'):
-    """
-    Plot arrows with a*,b* on current figure
-    """
-    # Get current axis size
-    ax = plt.gca()
-    if ax.name.lower() == '3d':
-        # 3D plot
-        ax_xlim = ax.get_xlim()
-        ax_ylim = ax.get_ylim()
-        ax_zlim = ax.get_zlim()
-        arrow_size = 40
-        color = 'k'
-        fontsize = 18
-        plot_arrow([0, UV[0, 0]], [0, UV[0, 1]], [0, UV[0, 2]], arrow_size=arrow_size, col=color)
-        ax.text(UV[0, 0], UV[0, 1], UV[0, 2], alabel, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
-        plot_arrow([0, UV[1, 0]], [0, UV[1, 1]], [0, UV[1, 2]], arrow_size=arrow_size, col=color)
-        ax.text(UV[1, 0], UV[1, 1], UV[1, 2], blabel, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
-        plot_arrow([0, UV[2, 0]], [0, UV[2, 1]], [0, UV[2, 2]], arrow_size=arrow_size, col=color)
-        ax.text(UV[2, 0], UV[2, 1], UV[2, 2], clabel, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
-        ax.set_xlim(ax_xlim)
-        ax.set_ylim(ax_ylim)
-        ax.set_zlim(ax_zlim)
-        return
-    # 2D plot
-    axsize = ax.axis()
-    asty = dict(arrowstyle="->")
-    plt.annotate("", xy=(UV[0, 0], UV[0, 1]), xytext=(0.0, 0.0), arrowprops=asty)
-    plt.annotate("", xy=(UV[1, 0], UV[1, 1]), xytext=(0.0, 0.0), arrowprops=asty)
-    plt.annotate(alabel, (0.1 + UV[0, 0], UV[0, 1] - 0.2))
-    plt.annotate(blabel, (UV[1, 0] - 0.2, 0.1 + UV[1, 1]))
-    ax.axis(axsize)
-
-
-def axis_lattice_points(vec_a=[1, 0, 0], vec_b=[0, 1, 0], axis=[-4, 4, -4, 4]):
-    """
-    Generate a 2D lattice of points generated by 2 vectors within a 2D axis
-    :param vec_a: [1x3] array : a* vector
-    :param vec_b: [1x3] array : b* vector
-    :param axis: [1x4] axis array, plt.axis()
-    :return: [nx3] array of lattice points
-    """
-
-    # Vectors
-    A = np.asarray(vec_a, dtype=float).reshape([3])
-    B = np.asarray(vec_b, dtype=float).reshape([3])
-    # Generate a 3D cell to make use of indx function
-    U = np.array([A, B, np.cross(A, B)])
-    corners = [[axis[1], axis[2], 0],
-               [axis[1], axis[3], 0],
-               [axis[0], axis[2], 0],
-               [axis[0], axis[3], 0]]
-    # Determine the coefficients required to generate lattice points of the 2 vectors at
-    # all 4 corners of the axis
-    idx = fc.indx(corners, U)
-    min_x = np.floor(np.min(idx[:, 0]))
-    max_x = np.ceil(np.max(idx[:, 0]))
-    min_y = np.floor(np.min(idx[:, 1]))
-    max_y = np.ceil(np.max(idx[:, 1]))
-    hkl = fc.genHKL([min_x, max_x], [min_y, max_y], 0)
-    latt = np.dot(hkl, U)
-    return latt
-
-
-def plot_lattice_points2D(Q, markersize=12, color='b', marker='o'):
-    """
-    Add points to the current axis
-    :param Q: [nx2/3] array : lattice points to plot
-    :param markersize: default 12
-    :param color: default 'b'
-    :param marker: default 'o'
-    :return: None
-    """
-
-    ax = plt.gca()
-    axsize = ax.axis()
-
-    ax.plot(Q[:, 0], Q[:, 1], markersize=markersize, color=color, marker=marker)
-    ax.axis(axsize)
-
-
-def plot_lattice_points3D(Q, point_size=None, color=None, cmap=None):
-    """
-    Plot lattice points is 3D reciprocal space
-    :param Q: [nx3] array of wavevector transfer positions in reciprocal space, units A^-1
-    :param point_size: scalar or array of length n, determines each point size (for intensity), in pixels
-    :param color: colour specifier, can be a list of values length n
-    :param cmap: str name of colormap to use if color is a list of values
-    :return:
-    """
-
-    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
-    ax = fig.add_subplot(111, projection='3d')
-
-    ax.scatter(Q[:, 0], Q[:, 1], Q[:, 2], s=point_size, c=color, cmap=cmap)
-    labels(None, 'Q$_x$', 'Q$_y$', 'Q$_z$')
-    ax.set_xlim([4, -4])
-    ax.set_ylim([4, -4])
-    ax.set_zlim([-4, 4])
-
-
-def plot_lattice_lines(latt, vec_a=(1, 0, 0), vec_b=(0, 1, 0), axis=None, *args, **kwargs):
-    """
-    Add lines defining the reciprocal lattice to the current plot
-        Generates square or hexagonal lines where vertices are the lattice points within the image.
-    :param latt: [nx2/3] array : points at which to generate lattice
-    :param vec_a: [1x2/3] array : a* vector
-    :param vec_b: [1x2/3] array : b* vector
-    :param axis: axis to plot on (None for plt.gca)
-    :param args: argments to pass to plot function, e.g. linewidth, alpha, color
-    :return: None
-    """
-
-    if axis is None:
-        axis = plt.gca()
-    axsize = axis.axis()
-
-    # vectors
-    A = np.asarray(vec_a, dtype=float).reshape([3])
-    B = np.asarray(vec_b, dtype=float).reshape([3])
-
-    # Angle between vectors
-    angle = fg.ang(A, B)
-
-    # At each lattice point, draw the unit vectors
-    for n in range(len(latt)):
-        lp = latt[n, :]
-        uv1_1 = lp - A
-        uv1_2 = lp + A
-        uv2_1 = lp - B
-        uv2_2 = lp + B
-
-        axis.plot([uv1_1[0], uv1_2[0]], [uv1_1[1], uv1_2[1]], 'k-', *args, **kwargs)
-        axis.plot([uv2_1[0], uv2_2[0]], [uv2_1[1], uv2_2[1]], 'k-', *args, **kwargs)
-        if abs(angle - np.pi / 3) < 0.01:  # 60Deg
-            uv3_1 = lp + A - B
-            uv3_2 = lp - A + B
-            axis.plot([uv3_1[0], uv3_2[0]], [uv3_1[1], uv3_2[1]], 'k-', *args, **kwargs)
-        elif abs(angle - 2 * np.pi / 3) < 0.01:  # 120 Deg
-            uv3_1 = lp + A + B
-            uv3_2 = lp - A - B
-            axis.plot([uv3_1[0], uv3_2[0]], [uv3_1[1], uv3_2[1]], 'k-', *args, **kwargs)
-    axis.axis(axsize)
-
-
-def plot_vector_arrows(vec_a=[1, 0, 0], vec_b=[1, 0, 0], vec_a_lab=None, vec_b_lab=None,
-                       arrow_size=40, color='b', fontsize=18, axis=None):
-    """
-    Plot vector arrows for Cell on current axis
-        Will generate two arrows on the current axis, pointing from the origin to vec_a and vec_b, respectivley.
-    :param vec_a: [1x2/3] array : a* vector
-    :param vec_b: [1x2/3] array : b* vector
-    :param vec_a_lab: str : e.g. 'a*'
-    :param vec_b_lab: str : e.g. 'b*'
-    :param arrow_size: size of arrow, default 40
-    :param color:  arror colour, default 'b'
-    :param fontsize: text size, default 18
-    :return: None
-    """
-
-    vec_a = np.asarray(vec_a).reshape([-1, np.shape(vec_a)[-1]])
-    vec_b = np.asarray(vec_b).reshape((-1, np.shape(vec_b)[-1]))
-
-    if axis is None:
-        axis = plt.gca()
-    axsize = axis.axis()
-
-    # Vector arrows and lattice point labels
-    if vec_a_lab is None:
-        vec_a_lab = 'a*'
-    if vec_b_lab is None:
-        vec_b_lab = 'b*'
-
-    plt.sca(axis)
-    plot_arrow([0, vec_a[0, 0]], [0, vec_a[0, 1]], arrow_size=arrow_size, col=color)
-    plt.text(vec_a[0, 0], vec_a[0, 1], vec_a_lab, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
-    plot_arrow([0, vec_b[0, 0]], [0, vec_b[0, 1]], arrow_size=arrow_size, col=color)
-    plt.text(vec_b[0, 0], vec_b[0, 1], vec_b_lab, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
-    axis.axis(axsize)
-
-
-def plot_ewald_coverage(energy_kev, color='k', linewidth=2):
-    """
-    Plot Ewald coverage of a single axis diffractometer on current plot in 2D
-    Includes boundaries for theta=0, twotheta=180 and theta=twotheta
-
-    :param energy_kev: float
-    :param color: str
-    :param linewidth: float
-    :return: None
-    """
-
-    q_max = fc.calqmag(180, energy_kev)
-
-    # calculate diffractometer angles
-    angles = np.arange(0, 180, 0.1)
-    Q1x, Q1y = fc.diffractometer_Q(angles, 180, energy_kev)  # delta=180
-    Q2x, Q2y = fc.diffractometer_Q(angles, angles, energy_kev)  # eta=delta
-    Q3x, Q3y = fc.diffractometer_Q(0, angles, energy_kev)  # eta=0
-
-    # Add diffractometer angles
-    plt.plot(Q1x, Q1y, color, linewidth, label=r'2$\theta$=180')
-    plt.plot(Q2x, Q2y, color, linewidth, label=r'2$\theta$=$\theta$')
-    plt.plot(Q3x, Q3y, color, linewidth, label=r'$\theta$=0')
-    plt.axis([-q_max, q_max, 0, q_max])
-
-
-def plot_diffractometer_reciprocal_space(phi, chi, eta, mu, delta, gamma, uv, u, lab, energy_kev):
-    """
-    Plot crystal axes in lab frame of 6-circle diffractometer
-    :param phi:
-    :param chi:
-    :param eta:
-    :param mu:
-    :param delta:
-    :param gamma:
-    :param uv:
-    :param u:
-    :param lab:
-    :param energy_kev:
-    :return:
-    """
-
-    uvstar = fc.RcSp(uv)
-    maxhkl = fc.maxHKL(2, uvstar)
-    hkl = fc.genHKL(*maxhkl)
-    r = fc.diffractometer_rotation(phi, chi, eta, mu)
-    qdet = fc.diff6circleq(delta, gamma, energy_kev, lab=lab)
-    ki, kf = fc.diff6circlek(delta, gamma, energy_kev, lab=lab)
-    qlab = fc.labwavevector(hkl, uv, u, r, lab)
-    astar = fc.labwavevector([1, 0, 0], uv, u, r, lab)
-    bstar = fc.labwavevector([0, 1, 0], uv, u, r, lab)
-    cstar = fc.labwavevector([0, 0, 1], uv, u, r, lab)
-
-    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
-    ax = fig.add_subplot(111, projection='3d')
-
-    def pltvec(vec, *args, **kwargs):
-        vec = np.reshape(vec, (-1, 3))
-        return plt.plot(vec[:, 1], vec[:, 2], vec[:, 0], *args, **kwargs)
-
-    pltvec(qlab, 'r+', ms=12, label='hkl')
-    pltvec([-ki, [0, 0, 0], kf, [0, 0, 0], qdet], 'k-', lw=5, label='q = kf - ki')
-    pltvec([[0, 0, 0], qdet], 'm-', lw=5, label='q = kf - ki')
-    pltvec([[0, 0, 0], astar], 'b-', lw=5, label='astar')
-    pltvec([[0, 0, 0], bstar], 'g-', lw=5, label='bstar')
-    pltvec([[0, 0, 0], cstar], 'y-', lw=5, label='cstar')
-    labels(None, 'Y', 'Z', 'X', legend=True)
-    ax.set_xlim([2, -2])
-    ax.set_ylim([2, -2])
-    ax.set_zlim([-2, 2])
-    #ax.invert_xaxis()
-    #ax.invert_yaxis()
-    plt.show()
-
-
-def plot_xray_scattering_factor(elements, maxq=10):
-    """
-    Plot x-ray scattering factor for 1 or more elements
-    :param elements:
-    :return: None
-    """
-
-    q = np.linspace(0, maxq, 200)
-    xrf = fc.xray_scattering_factor(elements, q)
-
-    newplot(q, xrf)
-    plt.legend(np.asarray(elements).reshape(-1), loc=0, frameon=False, fontsize=18)
-    labels('X-Ray Scattering Factor', 'Q [$\AA^{-1}$]')
-
-
-def plot_magnetic_form_factor(elements, maxq=10):
-    """
-    Plot magnetic form factor for 1 or more elements
-    :param elements:
-    :return: None
-    """
-
-    q = np.linspace(0, maxq, 200)
-    mff = fc.magnetic_form_factor(elements, q)
-
-    newplot(q, mff)
-    plt.legend(np.asarray(elements).reshape(-1), loc=0, frameon=False, fontsize=18)
-    labels('Magnetic Form Factor', 'Q [$\AA^{-1}$]')
-
-
-def plot_xray_attenuation(elements, min_energy=0, max_energy=20):
-    """
-    Plot x-ray scattering factor for 1 or more elements
-    :param elements:
-    :return: None
-    """
-
-    Zarray = fc.atom_properties(elements, 'Z')
-    ene = np.arange(min_energy, max_energy+0.01, 0.01)
-
-    Aarray = fc.attenuation(Zarray, ene)
-    newplot(ene, Aarray)
-    plt.yscale('log')
-    plt.xlim([min_energy, max_energy])
-    plt.legend(np.asarray(elements).reshape(-1), loc=0, frameon=False, fontsize=18)
-    labels('X-Ray Attenuation', 'Energy [keV]', r'$\mu/\rho$ [cm$^2$/g]')
-
-
-def plot_atomic_scattering_factor(element, min_energy=0.5, max_energy=20):
-    """
-    Plot atomic scattering factor for 1 or more elements
-    :param element: str name of element to plot
-    :param min_energy: float min energy in keV
-    :param max_energy: float max energy in keV
-    :return: None
-    """
-
-    ene = np.arange(min_energy, max_energy+0.01, 0.01)
-    f1, f2 = fc.atomic_scattering_factor(element, ene)
-
-    newplot(ene, f1, '-', lw=2, label='f1')
-    plt.plot(ene, f2, '-', lw=2, label='f2')
-    plt.xlim([min_energy, max_energy])
-    labels('X-Ray Scattering Factor\n%s' % element, 'Energy [keV]', None, legend=True)
-
-
-def plot_xray_transmission(chemical_formula, density=8.9, energy_range=None, thickness_um=100):
-    """
-    Plot transmission of x-ray through a slab of material at range of energies
-    Equivalent to https://henke.lbl.gov/optical_constants/filter2.html
-    Based on formulas from: Henke, Gullikson, and Davis, Atomic Data and Nuclear Data Tables 54 no.2, 181-342 (July 1993)
-    :param chemical_formula: str molecular formula
-    :param density: float density in g/cm^3
-    :param energy_range: array x-ray energy in keV, None for default range
-    :param thickness_um: slab thickness in microns
-    :return: float or array
-    """
-    if energy_range is None:
-        energy_range = np.arange(0.03, 20, 0.01)
-
-    transmission = fc.filter_transmission(chemical_formula, energy_range, density, thickness_um)
-    ttl = '%s Density=%5.3f, thickness=%3.3g μm' % (chemical_formula, density, thickness_um)
-
-    newplot(energy_range, transmission)
-    labels(ttl, 'Energy [keV]', 'Transmission')
-
-
-def plot_xray_attenuation_length(chemical_formula, density=8.9, energy_range=None, grazing_angle=90):
-    """
-    Plot the X-Ray Attenuation Length of a compound
-    Equivalent to: https://henke.lbl.gov/optical_constants/atten2.html
-    Based on formulas from: Henke, Gullikson, and Davis, Atomic Data and Nuclear Data Tables 54 no.2, 181-342 (July 1993)
-    :param chemical_formula: str molecular formula
-    :param density: float density in g/cm^3
-    :param energy_range: array x-ray energy in keV, None for default range
-    :param grazing_angle: incidence angle relative to the surface, in degrees
-    :return: float or array, in microns
-    """
-    if energy_range is None:
-        energy_range = np.arange(0.03, 20, 0.01)
-
-    transmission = fc.molecular_attenuation_length(chemical_formula, energy_range, density, grazing_angle)
-    ttl = '%s Density=%5.3f, Angle=%3.3g deg' % (chemical_formula, density, grazing_angle)
-
-    newplot(energy_range, transmission)
-    labels(ttl, 'Energy [keV]', 'Atten Length [μm]')
-
-
-def plot_xray_reflectivity(chemical_formula, density=8.9, energy_range=None, grazing_angle=2):
-    """
-    Plot the specular reflectivity of a material
-    From: https://xdb.lbl.gov/Section4/Sec_4-2.html
-    :param chemical_formula: str molecular formula
-    :param density: float, density in g/cm^3
-    :param energy_range: float or array, x-ray energy in keV
-    :param grazing_angle: float, incidence angle relative to the surface, in degrees
-    :return: float or array
-    """
-    if energy_range is None:
-        energy_range = np.arange(0.03, 20, 0.01)
-
-    reflectivity = fc.molecular_reflectivity(chemical_formula, energy_range, density, grazing_angle)
-    ttl = '%s Density=%5.3f, Angle=%3.3g deg' % (chemical_formula, density, grazing_angle)
-
-    newplot(energy_range, reflectivity)
-    labels(ttl, 'Energy [keV]', 'Atten Length [μm]')
-
-
-def plot_xray_refractive_index(chemical_formula, density=8.9, energy_range=None):
-    """
-    Plot the Complex Index of Refraction of a compound
-        n = 1 - (1/2pi)N*r0*lambda^2*(f1+if2) = 1 - Delta - iBeta
-    Equivalent to: https://henke.lbl.gov/optical_constants/getdb2.html
-    Based on formulas from: Henke, Gullikson, and Davis, Atomic Data and Nuclear Data Tables 54 no.2, 181-342 (July 1993)
-    :param chemical_formula: str molecular formula
-    :param density: float density in g/cm^3
-    :param energy_range: array x-ray energy in keV, None for default range
-    :return: float or array, in microns
-    """
-    if energy_range is None:
-        energy_range = np.arange(0.03, 20, 0.01)
-
-    n, delta, beta = fc.molecular_refractive_index(chemical_formula, energy_range, density)
-    ttl = '%s Density=%5.3f\nIndex of Refraction = 1 - δ - iβ' % (chemical_formula, density)
-
-    newplot(energy_range, delta, 'r-', lw=2, label='δ')
-    plt.plot(energy_range, beta, 'b-', lw=2, label='β')
-    labels(ttl, 'Energy [keV]', None, legend=True)
-    plt.xscale('log')
-    plt.yscale('log')
-
+# -*- coding: utf-8 -*-
+"""
+Module: Handy plotting functions "functions_plotting.py"
+
+Contains various plotting shortcuts using matplotlib.pyplot
+
+By Dan Porter, PhD
+Diamond
+2018
+
+Usage: 
+    - Run this file in an interactive console
+    OR
+    - from Dans_Diffraction import functions_plotting as fp
+
+All plots generated require plt.show() call, unless using interactive mode
+
+
+Version 2.2
+Last updated: 09/07/23
+
+Version History:
+06/01/18 1.0    Program created from DansGeneralProgs.py V2.3
+05/03/18 1.1    Removed plt.show from arrow functions
+17/04/18 1.2    Removed plt.show from other functions
+03/05/18 1.3    Removed plot_vector_lines(vec_a,vec_b), replaced with plot_lattice_lines(Q, vec_a, vec_b)
+30/05/18 1.4    Added multiplot
+07/03/19 1.5    Added plot_attenuation and others
+22/03/19 1.6    Added plot_circle, updated vecplot and plot_lattice_lines
+03/05/19 1.7    Added legend to labels function
+09/03/20 1.8    Added default figure size
+22/11/20 1.9    Update to labels to fix 3D plotting
+15/02/21 1.9.1  Update to vecplot for plotting on axis
+27/09/21 2.0    Added plot3darray, plot_diffractometer_reciprocal_space
+10/08/22 2.1    Added plot_lattice_points3D, set_plot_defaults, changed default fig size
+09/07/23 2.2    Thanks to asteppke for suggested update to Arrow3D for matplotlib V>3.4
+
+@author: DGPorter
+"""
+
+import sys, os
+import numpy as np
+import matplotlib.pyplot as plt
+from mpl_toolkits.mplot3d import Axes3D
+from matplotlib.patches import FancyArrowPatch
+from mpl_toolkits.mplot3d import proj3d
+
+from . import functions_general as fg
+from . import functions_crystallography as fc
+
+__version__ = '2.2'
+
+DEFAULT_FONT = 'Times New Roman'
+DEFAULT_FONTSIZE = 14
+FIGURE_SIZE = [12, 8]
+FIGURE_DPI = 80
+
+
+'----------------------------Plot manipulation--------------------------'
+
+
+def set_plot_defaults(rcdefaults=False):
+    """
+    Set custom matplotlib rcparams, or revert to matplotlib defaults
+    These handle the default look of matplotlib plots
+    See: https://matplotlib.org/stable/tutorials/introductory/customizing.html#the-default-matplotlibrc-file
+    :param rcdefaults: False*/ True, if True, revert to matplotlib defaults
+    :return: None
+    """
+    if rcdefaults:
+        print('Return matplotlib rcparams to default settings.')
+        plt.rcdefaults()
+        return
+
+    plt.rc('figure', figsize=FIGURE_SIZE, dpi=FIGURE_DPI, autolayout=False)
+    plt.rc('lines', marker='o', color='r', linewidth=2, markersize=6)
+    plt.rc('errorbar', capsize=2)
+    plt.rc('legend', loc='best', frameon=False, fontsize=DEFAULT_FONTSIZE)
+    plt.rc('axes', linewidth=2, titleweight='bold', labelsize='large')
+    plt.rc('xtick', labelsize='large')
+    plt.rc('ytick', labelsize='large')
+    plt.rc('axes.formatter', limits=(-3, 3), offset_threshold=6)
+    plt.rc('image', cmap='viridis')  # default colourmap, see https://matplotlib.org/stable/gallery/color/colormap_reference.html
+    # Note font values appear to only be set when plt.show is called
+    plt.rc(
+        'font',
+        family='serif',
+        style='normal',
+        weight='bold',
+        size=DEFAULT_FONTSIZE,
+        serif=['Times New Roman', 'Times', 'DejaVu Serif']
+    )
+    # plt.rcParams["savefig.directory"] = os.path.dirname(__file__) # Default save directory for figures
+
+
+def labels(ttl=None, xvar=None, yvar=None, zvar=None, legend=False, size='Normal', font='Times New Roman'):
+    """
+    Add formatted labels to current plot, also increases the tick size
+    :param ttl: title
+    :param xvar: x label
+    :param yvar: y label
+    :param zvar: z label (3D plots only)
+    :param legend: False/ True, adds default legend to plot 
+    :param size: 'Normal' or 'Big'
+    :param font: str font name, 'Times New Roman'
+    :return: None
+    """
+
+    if size.lower() in ['big', 'large', 'xxl', 'xl']:
+        tik = 30
+        tit = 32
+        lab = 35
+        leg = 25
+    else:
+        # Normal
+        tik = 18
+        tit = 20
+        lab = 22
+        leg = 18
+
+    plt.xticks(fontsize=tik, fontname=font)
+    plt.yticks(fontsize=tik, fontname=font)
+    plt.setp(plt.gca().spines.values(), linewidth=2)
+    if plt.gca().get_yaxis().get_scale() != 'log' and 'linear' in plt.gca().name:
+        plt.ticklabel_format(useOffset=False)
+        plt.ticklabel_format(style='sci', scilimits=(-3,3))
+
+    if ttl is not None:
+        plt.gca().set_title(ttl, fontsize=tit, fontweight='bold', fontname=font)
+
+    if xvar is not None:
+        plt.gca().set_xlabel(xvar, fontsize=lab, fontname=font)
+
+    if yvar is not None:
+        plt.gca().set_ylabel(yvar, fontsize=lab, fontname=font)
+
+    if zvar is not None:
+        # Don't think this works, use ax.set_zaxis
+        plt.gca().set_zlabel(zvar, fontsize=lab, fontname=font)
+        for t in plt.gca().zaxis.get_major_ticks():
+            t.label.set_fontsize(tik)
+            t.label.set_fontname(font)
+
+    if legend:
+        plt.legend(loc=0, frameon=False, prop={'size': leg, 'family': 'serif'})
+
+
+def saveplot(name, dpi=None, figure=None):
+    r"""
+    Saves current figure as a png in the home directory
+    :param name: filename, including or expluding directory and or extension
+    :param dpi: image resolution, higher means larger image size, default=matplotlib default
+    :param figure: figure number, default = plt.gcf()
+    :return: None
+
+    E.G.
+    ---select figure to save by clicking on it---
+    saveplot('test')
+    E.G.
+    saveplot('c:\somedir\apicture.jpg', dpi=600, figure=3)
+    """
+
+    if type(name) is int:
+        name = str(name)
+
+    if figure is None:
+        gcf = plt.gcf()
+    else:
+        gcf = plt.figure(figure)
+
+    dir = os.path.dirname(name)
+    file, ext = os.path.basename(name)
+
+    if len(dir) == 0:
+        dir = os.path.expanduser('~')
+
+    if len(ext) == 0:
+        ext = '.png'
+
+    savefile = os.path.join(dir, file+ext)
+    gcf.savefig(savefile, dpi=dpi)
+    print('Saved Figure {} as {}'.format(gcf.number, savefile))
+
+
+def newplot(*args, **kwargs):
+    """
+    Shortcut to creating a simple plot
+    E.G.
+      x = np.arange(-5,5,0.1)
+      y = x**2
+      newplot(x,y,'r-',lw=2,label='Line')
+    """
+
+    if 'linewidth' and 'lw' not in kwargs.keys():
+        kwargs['linewidth'] = 2
+
+    plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
+    plt.plot(*args, **kwargs)
+
+    plt.setp(plt.gca().spines.values(), linewidth=2)
+    plt.xticks(fontsize=25, fontname='Times New Roman')
+    plt.yticks(fontsize=25, fontname='Times New Roman')
+    plt.ticklabel_format(useOffset=False)
+    plt.ticklabel_format(style='sci', scilimits=(-3, 3))
+
+
+def multiplot(xvals, yvals=None, datarange=None, cmap='jet', labels=None, marker=None):
+    """
+    Shortcut to creating a simple multiplot with either colorbar or legend
+    E.G.
+      x = np.arange(-5,5,0.1)
+      ys = [x**2, 1+x**2, 2+x**2, 3+x**2, 4+x**2]
+      datarange = [0,1,2,3,4]
+      multiplot(x, ys, datarange, cmap='winter')
+    OR:
+      x = np.arange(-5,5,0.1)
+      ys = [x**2, 1+x**2, 2+x**2, 3+x**2, 4+x**2]
+      labels = ['x*x','2+x*x','3+x*x','4+x*x']
+      multiplot(x, ys, labels=labels)
+    """
+
+    if yvals is None:
+        yvals = xvals
+        xvals = []
+    yvals = np.asarray(yvals)
+    xvals = np.asarray(xvals)
+
+    if datarange is None:
+        datarange = range(len(yvals))
+    datarange = np.asarray(datarange,dtype=float)
+
+    cm = plt.get_cmap(cmap)
+    colrange = (datarange - datarange.min()) / (datarange.max() - datarange.min())
+    
+    if marker is None:
+        marker = ''
+    linearg = '-' + marker
+
+    plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
+    for n in range(len(datarange)):
+        col = cm(colrange[n])
+        if len(xvals) == 0:
+            plt.plot(yvals[n], linearg, lw=2, color=col)
+        elif len(xvals.shape) == 1:
+            plt.plot(xvals, yvals[n], linearg, lw=2, color=col)
+        else:
+            plt.plot(xvals[n], yvals[n], linearg, lw=2, color=col)
+
+    plt.setp(plt.gca().spines.values(), linewidth=2)
+    plt.xticks(fontsize=25, fontname='Times New Roman')
+    plt.yticks(fontsize=25, fontname='Times New Roman')
+    plt.ticklabel_format(useOffset=False)
+    plt.ticklabel_format(style='sci', scilimits=(-3, 3))
+
+    if labels is None:
+        # Add Colorbar
+        sm = plt.cm.ScalarMappable(cmap=cm)
+        sm.set_array(datarange)
+        cbar = plt.colorbar(sm)
+        #cbar.set_label('variation [unit]', fontsize=24, fontweight='bold', fontname='Times New Roman')
+    else:
+        # Add legend
+        plt.legend(labels, loc=0, frameon=False, prop={'size':20,'family':'serif'})
+
+
+def newplot3(*args, **kwargs):
+    """
+    Shortcut to creating a simple 3D plot
+    Automatically tiles 1 dimensional x and y arrays to match 2D z array,
+    assuming z.shape = (len(x),len(y))
+      newplot3(x, y, z, ...)
+
+    E.G.
+      newplot3([1,2,3,4],[9,8,7],[[2,4,6],[8,10,12],[14,16,18],[20,22,24]],'-o')
+    """
+
+    if 'linewidth' and 'lw' not in kwargs.keys():
+        kwargs['linewidth'] = 2
+
+    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
+    ax = fig.add_subplot(111, projection='3d')
+
+    x = np.asarray(args[0], dtype=float)
+    y = np.asarray(args[1], dtype=float)
+    z = np.asarray(args[2], dtype=float)
+
+    if z.ndim == 2:
+        if x.ndim < 2:
+            x = np.tile(x, z.shape[1]).reshape(z.T.shape).T
+        if y.ndim < 2:
+            y = np.tile(y, z.shape[0]).reshape(z.shape)
+
+        # Plot each array independently
+        for n in range(len(z)):
+            ax.plot(x[n], y[n], z[n], *args[3:], **kwargs)
+    else:
+        ax.plot(*args, **kwargs)
+
+
+def plot3darray(vec, *args, **kwargs):
+    """
+    Plot 3D vectors in 3D
+        plt.plot(vec[:, 0], vec[:, 1], vec[:, 3], *args, **kwargs)
+    :param vec: [n*3] array
+    :param args: args to pass to plt.plot
+    :param kwargs: kwargs to pass to plt.plot
+    :return: matplotlib plot object
+    """
+    vec = np.reshape(vec, (-1, 3))
+    return plt.plot(vec[:, 0], vec[:, 1], vec[:, 2], *args, **kwargs)
+
+
+def sliderplot(YY, X=None, slidervals=None, *args, **kwargs):
+    """
+    Shortcut to creating a simple 2D plot with a slider to go through a third dimension
+    YY = [nxm]: y axis data (initially plots Y[0,:])
+     X = [n] or [nxm]:  x axis data (can be 1D or 2D, either same length or shape as Y)
+     slidervals = None or [m]: Values to give in the slider
+
+    E.G.
+      sliderplot([1,2,3],[[2,4,6],[8,10,12],[14,16,18],[20,22,24]],slidervals=[3,6,9,12])
+    """
+
+    if 'linewidth' and 'lw' not in kwargs.keys():
+        kwargs['linewidth'] = 2
+
+    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
+
+    X = np.asarray(X, dtype=float)
+    Y = np.asarray(YY, dtype=float)
+    if slidervals is None:
+        slidervals = range(Y.shape[0])
+    slidervals = np.asarray(slidervals, dtype=float)
+
+    if X.ndim < 2:
+        X = np.tile(X, Y.shape[0]).reshape(Y.shape)
+
+    plotline, = plt.plot(X[0, :], Y[0, :], *args, **kwargs)
+    plt.axis([X.min(), X.max(), Y.min(), Y.max()])
+    plt.subplots_adjust(bottom=0.2)
+    ax = plt.gca()
+
+    " Create slider on plot"
+    axsldr = plt.axes([0.15, 0.05, 0.65, 0.03], axisbg='lightgoldenrodyellow')
+
+    sldr = plt.Slider(axsldr, '', 0, len(slidervals) - 1)
+    txt = axsldr.set_xlabel('{} [{}]'.format(slidervals[0], 0), fontsize=18)
+
+    plt.sca(ax)
+
+    " Slider update function"
+
+    def update(val):
+        "Update function for pilatus image"
+        pno = int(np.floor(sldr.val))
+        plotline.set_xdata(X[pno, :])
+        plotline.set_ydata(Y[pno, :])
+        txt.set_text('{} [{}]'.format(slidervals[pno], pno))
+        plt.draw()
+        plt.gcf().canvas.draw()
+        # fig1.canvas.draw()
+
+    sldr.on_changed(update)
+
+
+def sliderplot2D(ZZZ, XX=None, YY=None, slidervals=None, *args, **kwargs):
+    """
+    Shortcut to creating an image plot with a slider to go through a third dimension
+    ZZZ = [nxmxo]: z axis data
+     XX = [nxm] or [n]:  x axis data
+     YY = [nxm] or [m]: y axis data
+     slidervals = None or [o]: Values to give in the slider
+
+    if XX and/or YY have a single dimension, the 2D values are generated via meshgrid
+
+    E.G.
+      sliderplot([1,2,3],[[2,4,6],[8,10,12],[14,16,18],[20,22,24]],slidervals=[3,6,9,12])
+    """
+
+    if 'linewidth' and 'lw' not in kwargs.keys():
+        kwargs['linewidth'] = 2
+
+    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
+
+    ZZZ = np.asarray(ZZZ, dtype=float)
+
+    if slidervals is None:
+        slidervals = range(ZZZ.shape[2])
+    slidervals = np.asarray(slidervals, dtype=float)
+
+    if XX is None:
+        XX = range(ZZZ.shape[1])
+    if YY is None:
+        YY = range(ZZZ.shape[0])
+    XX = np.asarray(XX, dtype=float)
+    YY = np.asarray(YY, dtype=float)
+    if XX.ndim < 2:
+        XX, YY = np.meshgrid(XX, YY)
+
+    p = plt.pcolormesh(XX, YY, ZZZ[:, :, 0])
+    # p.set_clim(cax)
+
+    plt.subplots_adjust(bottom=0.2)
+    ax = plt.gca()
+    ax.set_aspect('equal')
+    ax.autoscale(tight=True)
+
+    " Create slider on plot"
+    axsldr = plt.axes([0.15, 0.05, 0.65, 0.03], axisbg='lightgoldenrodyellow')
+
+    sldr = plt.Slider(axsldr, '', 0, len(slidervals) - 1)
+    txt = axsldr.set_xlabel('{} [{}]'.format(slidervals[0], 0), fontsize=18)
+
+    plt.sca(ax)
+
+    " Slider update function"
+
+    def update(val):
+        "Update function for pilatus image"
+        pno = int(np.round(sldr.val))
+        p.set_array(ZZZ[:-1, :-1, pno].ravel())
+        txt.set_text('{} [{}]'.format(slidervals[pno], pno))
+        plt.draw()
+        plt.gcf().canvas.draw()
+        # fig1.canvas.draw()
+    sldr.on_changed(update)
+
+
+def plot_cell(cell_centre=[0, 0, 0], CELL=np.eye(3), color='k'):
+    """
+    Plot a box defined by a unit cell on the current plot
+    :param cell_centre: [1x3] array : centre of cell, default [0,0,0]
+    :param CELL: [3x3] array : unit cell vectors [A,B,C]
+    :return: None
+    """
+
+    uvw = np.array([[0., 0, 0], [1, 0, 0], [1, 0, 1], [1, 1, 1], [1, 1, 0], [0, 1, 0], [0, 1, 1],
+                    [0, 0, 1], [1, 0, 1], [1, 0, 0], [1, 1, 0], [1, 1, 1], [0, 1, 1], [0, 1, 0], [0, 0, 0], [0, 0, 1]])
+    uvw = uvw - 0.5  # plot around box centre
+    bpos = np.dot(uvw, CELL)
+    bpos = bpos + cell_centre
+    plt.plot(bpos[:, 0], bpos[:, 1], bpos[:, 2], c=color)  # cell box
+
+
+def plot_circle(radius=1.0, centre=[0,0], height=0, *args, **kwargs):
+    """
+    Generate circle on current plot
+    :param radius: radius of the circle
+    :param centre: [x,y] centre of the circle
+    :param height: reduce the radius by increasing the height from a surface
+    :param args: plot commands
+    :param kwargs: plot commands
+    :return: none
+    """
+
+    deg = np.linspace(0, 360, 361)
+    rad = np.deg2rad(deg)
+    x = centre[0] + np.sqrt((radius**2-height**2))*np.cos(rad)
+    y = centre[1] + np.sqrt((radius**2-height**2))*np.sin(rad)
+    plt.plot(x, y, *args, **kwargs)
+
+
+def plot_arrow(x, y, z=None, col='r', width=2, arrow_size=40):
+    """
+    Plot arrow in 2D or 3D on current axes
+    Usage 2D:
+      plot_arrow([xi,xf],[yi,yf])
+    Usage 3D:
+      plot_arrow([xi,xf],[yi,yf],[zi,zf])
+
+    Options:
+      width = line width (Def. = 2)
+      arrow_size = size of arrow head (Def. = 40)
+      col = arrow color (Deg. = red)
+    """
+
+    # 2D Arrow
+    if z is None or not hasattr(plt.gca(), 'get_zlim'):
+        x0 = x[0]
+        y0 = y[0]
+        dx = x[1] - x[0]
+        dy = y[1] - y[0]
+
+        plt.arrow(x0, y0, dx, dy, width=arrow_size / 4000.0, color=col, length_includes_head=True)
+        # V = FancyArrowPatch(x,y, mutation_scale=arrow_size, lw=width, arrowstyle="-|>", color=col)
+        # plt.gca().add_artist(V)
+        return
+
+    # 3D Arrow
+    V = Arrow3D(x, y, z, mutation_scale=arrow_size, lw=width, arrowstyle="-|>", color=col)
+    plt.gca().add_artist(V)
+
+
+class Arrow3D(FancyArrowPatch):
+    """
+    FancyArrow3D patch for 3D arrows, by CT Zhu
+     http://stackoverflow.com/questions/22867620/putting-arrowheads-on-vectors-in-matplotlibs-3d-plot
+    Useage:
+      fig = plt.figure()
+      ax = fig.add_subplot(111, projection='3d')
+      ax.plot([0,1],[0,0],[0,0],'k-')
+      ax.plot([0,0],[0,1],[0,0],'k-')
+      ax.plot([0,0],[0,0],[0,1],'k-')
+      v = Arrow3D([0,1],[0,1],[0,1], mutation_scale=20, lw=3, arrowstyle="-|>", color="r")
+      ax.add_artist(v)
+
+    """
+
+    def __init__(self, xs, ys, zs, *args, **kwargs):
+        if 'arrowstyle' not in kwargs.keys():
+            kwargs['arrowstyle'] = "-|>"
+        if 'mutation_scale' not in kwargs.keys():
+            kwargs['mutation_scale'] = 20
+        super().__init__((0,0), (0,0), *args, **kwargs)
+        self._verts3d = xs, ys, zs
+
+    # Fix for change in matplotlib 3.5.0 (https://github.com/matplotlib/matplotlib/issues/21688)
+    def do_3d_projection(self, renderer=None):
+        xs3d, ys3d, zs3d = self._verts3d
+        xs, ys, zs = proj3d.proj_transform(xs3d, ys3d, zs3d, self.axes.M)
+        self.set_positions((xs[0], ys[0]), (xs[1], ys[1]))
+        return np.min(zs)
+
+    # keep this part for older versions of matplotlib
+    def draw(self, renderer):
+        xs3d, ys3d, zs3d = self._verts3d
+        xs, ys, zs = proj3d.proj_transform(xs3d, ys3d, zs3d, self.axes.M)
+        self.set_positions((xs[0], ys[0]), (xs[1], ys[1]))
+        super().draw(renderer)
+
+
+'----------------------- Crystal Plotting Programs----------------------'
+
+
+def vecplot(UV, mode='hk0', axis=None, *args, **kwargs):
+    """
+    Plot grid of a,b vectors on current axis
+    :param UV: [a;b;c] array of unit vectors
+    :param mode: definition of axis plane, 'hk0', 'h0l', '0kl', 'hhl'
+    :param axis: axis to create lines on, if None, plt.gca is used
+    :param args: arguments to pass to plot command, e.g. linewidth, alpha, color
+    :return: None
+    """
+
+    if mode == 'h0l':
+        # h0l
+        UV = np.dot(np.array([[1, 0, 0], [0, 0, 1], [0, 1, 0]]), fg.rot3D(UV, gamma=-90))
+    elif mode == '0kl':
+        # 0kl
+        UV = np.dot(np.array([[0, 1, 0], [0, 0, 1], [1, 0, 0]]), UV)
+    elif mode == 'hhl':
+        # hhl ***untested
+        UV = np.dot(np.array([[1, 1, 0], [0, 0, 1], [0, 1, 0]]), UV)
+
+    if axis is None:
+        axis = plt.gca()
+    axsize = axis.axis()
+    latt = axis_lattice_points(UV[0], UV[1], axis=axsize)
+    plot_lattice_lines(latt, UV[0], UV[1], axis=axis, *args, **kwargs)
+
+
+def UV_arrows(UV, alabel='a', blabel='b', clabel='c'):
+    """
+    Plot arrows with a*,b* on current figure
+    """
+    # Get current axis size
+    ax = plt.gca()
+    if ax.name.lower() == '3d':
+        # 3D plot
+        ax_xlim = ax.get_xlim()
+        ax_ylim = ax.get_ylim()
+        ax_zlim = ax.get_zlim()
+        arrow_size = 40
+        color = 'k'
+        fontsize = 18
+        plot_arrow([0, UV[0, 0]], [0, UV[0, 1]], [0, UV[0, 2]], arrow_size=arrow_size, col=color)
+        ax.text(UV[0, 0], UV[0, 1], UV[0, 2], alabel, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
+        plot_arrow([0, UV[1, 0]], [0, UV[1, 1]], [0, UV[1, 2]], arrow_size=arrow_size, col=color)
+        ax.text(UV[1, 0], UV[1, 1], UV[1, 2], blabel, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
+        plot_arrow([0, UV[2, 0]], [0, UV[2, 1]], [0, UV[2, 2]], arrow_size=arrow_size, col=color)
+        ax.text(UV[2, 0], UV[2, 1], UV[2, 2], clabel, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
+        ax.set_xlim(ax_xlim)
+        ax.set_ylim(ax_ylim)
+        ax.set_zlim(ax_zlim)
+        return
+    # 2D plot
+    axsize = ax.axis()
+    asty = dict(arrowstyle="->")
+    plt.annotate("", xy=(UV[0, 0], UV[0, 1]), xytext=(0.0, 0.0), arrowprops=asty)
+    plt.annotate("", xy=(UV[1, 0], UV[1, 1]), xytext=(0.0, 0.0), arrowprops=asty)
+    plt.annotate(alabel, (0.1 + UV[0, 0], UV[0, 1] - 0.2))
+    plt.annotate(blabel, (UV[1, 0] - 0.2, 0.1 + UV[1, 1]))
+    ax.axis(axsize)
+
+
+def axis_lattice_points(vec_a=[1, 0, 0], vec_b=[0, 1, 0], axis=[-4, 4, -4, 4]):
+    """
+    Generate a 2D lattice of points generated by 2 vectors within a 2D axis
+    :param vec_a: [1x3] array : a* vector
+    :param vec_b: [1x3] array : b* vector
+    :param axis: [1x4] axis array, plt.axis()
+    :return: [nx3] array of lattice points
+    """
+
+    # Vectors
+    A = np.asarray(vec_a, dtype=float).reshape([3])
+    B = np.asarray(vec_b, dtype=float).reshape([3])
+    # Generate a 3D cell to make use of indx function
+    U = np.array([A, B, np.cross(A, B)])
+    corners = [[axis[1], axis[2], 0],
+               [axis[1], axis[3], 0],
+               [axis[0], axis[2], 0],
+               [axis[0], axis[3], 0]]
+    # Determine the coefficients required to generate lattice points of the 2 vectors at
+    # all 4 corners of the axis
+    idx = fc.indx(corners, U)
+    min_x = np.floor(np.min(idx[:, 0]))
+    max_x = np.ceil(np.max(idx[:, 0]))
+    min_y = np.floor(np.min(idx[:, 1]))
+    max_y = np.ceil(np.max(idx[:, 1]))
+    hkl = fc.genHKL([min_x, max_x], [min_y, max_y], 0)
+    latt = np.dot(hkl, U)
+    return latt
+
+
+def plot_lattice_points2D(Q, markersize=12, color='b', marker='o'):
+    """
+    Add points to the current axis
+    :param Q: [nx2/3] array : lattice points to plot
+    :param markersize: default 12
+    :param color: default 'b'
+    :param marker: default 'o'
+    :return: None
+    """
+
+    ax = plt.gca()
+    axsize = ax.axis()
+
+    ax.plot(Q[:, 0], Q[:, 1], markersize=markersize, color=color, marker=marker)
+    ax.axis(axsize)
+
+
+def plot_lattice_points3D(Q, point_size=None, color=None, cmap=None):
+    """
+    Plot lattice points is 3D reciprocal space
+    :param Q: [nx3] array of wavevector transfer positions in reciprocal space, units A^-1
+    :param point_size: scalar or array of length n, determines each point size (for intensity), in pixels
+    :param color: colour specifier, can be a list of values length n
+    :param cmap: str name of colormap to use if color is a list of values
+    :return:
+    """
+
+    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
+    ax = fig.add_subplot(111, projection='3d')
+
+    ax.scatter(Q[:, 0], Q[:, 1], Q[:, 2], s=point_size, c=color, cmap=cmap)
+    labels(None, 'Q$_x$', 'Q$_y$', 'Q$_z$')
+    ax.set_xlim([4, -4])
+    ax.set_ylim([4, -4])
+    ax.set_zlim([-4, 4])
+
+
+def plot_lattice_lines(latt, vec_a=(1, 0, 0), vec_b=(0, 1, 0), axis=None, *args, **kwargs):
+    """
+    Add lines defining the reciprocal lattice to the current plot
+        Generates square or hexagonal lines where vertices are the lattice points within the image.
+    :param latt: [nx2/3] array : points at which to generate lattice
+    :param vec_a: [1x2/3] array : a* vector
+    :param vec_b: [1x2/3] array : b* vector
+    :param axis: axis to plot on (None for plt.gca)
+    :param args: argments to pass to plot function, e.g. linewidth, alpha, color
+    :return: None
+    """
+
+    if axis is None:
+        axis = plt.gca()
+    axsize = axis.axis()
+
+    if 'c' not in kwargs and 'color' not in kwargs:
+        kwargs['color'] = 'k'
+
+    # vectors
+    A = np.asarray(vec_a, dtype=float).reshape([3])
+    B = np.asarray(vec_b, dtype=float).reshape([3])
+
+    # Angle between vectors
+    angle = fg.ang(A, B)
+
+    # At each lattice point, draw the unit vectors
+    for n in range(len(latt)):
+        lp = latt[n, :]
+        uv1_1 = lp - A
+        uv1_2 = lp + A
+        uv2_1 = lp - B
+        uv2_2 = lp + B
+
+        axis.plot([uv1_1[0], uv1_2[0]], [uv1_1[1], uv1_2[1]], '-', *args, **kwargs)
+        axis.plot([uv2_1[0], uv2_2[0]], [uv2_1[1], uv2_2[1]], '-', *args, **kwargs)
+        if abs(angle - np.pi / 3) < 0.01:  # 60Deg
+            uv3_1 = lp + A - B
+            uv3_2 = lp - A + B
+            axis.plot([uv3_1[0], uv3_2[0]], [uv3_1[1], uv3_2[1]], '-', *args, **kwargs)
+        elif abs(angle - 2 * np.pi / 3) < 0.01:  # 120 Deg
+            uv3_1 = lp + A + B
+            uv3_2 = lp - A - B
+            axis.plot([uv3_1[0], uv3_2[0]], [uv3_1[1], uv3_2[1]], '-', *args, **kwargs)
+    axis.axis(axsize)
+
+
+def plot_vector_arrows(vec_a=[1, 0, 0], vec_b=[1, 0, 0], vec_a_lab=None, vec_b_lab=None,
+                       arrow_size=40, color='b', fontsize=18, axis=None):
+    """
+    Plot vector arrows for Cell on current axis
+        Will generate two arrows on the current axis, pointing from the origin to vec_a and vec_b, respectivley.
+    :param vec_a: [1x2/3] array : a* vector
+    :param vec_b: [1x2/3] array : b* vector
+    :param vec_a_lab: str : e.g. 'a*'
+    :param vec_b_lab: str : e.g. 'b*'
+    :param arrow_size: size of arrow, default 40
+    :param color:  arror colour, default 'b'
+    :param fontsize: text size, default 18
+    :return: None
+    """
+
+    vec_a = np.asarray(vec_a).reshape([-1, np.shape(vec_a)[-1]])
+    vec_b = np.asarray(vec_b).reshape((-1, np.shape(vec_b)[-1]))
+
+    if axis is None:
+        axis = plt.gca()
+    axsize = axis.axis()
+
+    # Vector arrows and lattice point labels
+    if vec_a_lab is None:
+        vec_a_lab = 'a*'
+    if vec_b_lab is None:
+        vec_b_lab = 'b*'
+
+    plt.sca(axis)
+    plot_arrow([0, vec_a[0, 0]], [0, vec_a[0, 1]], arrow_size=arrow_size, col=color)
+    plt.text(vec_a[0, 0], vec_a[0, 1], vec_a_lab, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
+    plot_arrow([0, vec_b[0, 0]], [0, vec_b[0, 1]], arrow_size=arrow_size, col=color)
+    plt.text(vec_b[0, 0], vec_b[0, 1], vec_b_lab, fontname=DEFAULT_FONT, weight='bold', size=fontsize)
+    axis.axis(axsize)
+
+
+def plot_ewald_coverage(energy_kev, color='k', linewidth=2):
+    """
+    Plot Ewald coverage of a single axis diffractometer on current plot in 2D
+    Includes boundaries for theta=0, twotheta=180 and theta=twotheta
+
+    :param energy_kev: float
+    :param color: str
+    :param linewidth: float
+    :return: None
+    """
+
+    q_max = fc.calqmag(180, energy_kev)
+
+    # calculate diffractometer angles
+    angles = np.arange(0, 180, 0.1)
+    Q1x, Q1y = fc.diffractometer_Q(angles, 180, energy_kev)  # delta=180
+    Q2x, Q2y = fc.diffractometer_Q(angles, angles, energy_kev)  # eta=delta
+    Q3x, Q3y = fc.diffractometer_Q(0, angles, energy_kev)  # eta=0
+
+    # Add diffractometer angles
+    plt.plot(Q1x, Q1y, color, linewidth, label=r'2$\theta$=180')
+    plt.plot(Q2x, Q2y, color, linewidth, label=r'2$\theta$=$\theta$')
+    plt.plot(Q3x, Q3y, color, linewidth, label=r'$\theta$=0')
+    plt.axis([-q_max, q_max, 0, q_max])
+
+
+def plot_diffractometer_reciprocal_space(phi, chi, eta, mu, delta, gamma, uv, u, lab, energy_kev):
+    """
+    Plot crystal axes in lab frame of 6-circle diffractometer
+    :param phi:
+    :param chi:
+    :param eta:
+    :param mu:
+    :param delta:
+    :param gamma:
+    :param uv:
+    :param u:
+    :param lab:
+    :param energy_kev:
+    :return:
+    """
+
+    uvstar = fc.RcSp(uv)
+    maxhkl = fc.maxHKL(2, uvstar)
+    hkl = fc.genHKL(*maxhkl)
+    r = fc.diffractometer_rotation(phi, chi, eta, mu)
+    qdet = fc.diff6circleq(delta, gamma, energy_kev, lab=lab)
+    ki, kf = fc.diff6circlek(delta, gamma, energy_kev, lab=lab)
+    qlab = fc.labwavevector(hkl, uv, u, r, lab)
+    astar = fc.labwavevector([1, 0, 0], uv, u, r, lab)
+    bstar = fc.labwavevector([0, 1, 0], uv, u, r, lab)
+    cstar = fc.labwavevector([0, 0, 1], uv, u, r, lab)
+
+    fig = plt.figure(figsize=FIGURE_SIZE, dpi=FIGURE_DPI)
+    ax = fig.add_subplot(111, projection='3d')
+
+    def pltvec(vec, *args, **kwargs):
+        vec = np.reshape(vec, (-1, 3))
+        return plt.plot(vec[:, 1], vec[:, 2], vec[:, 0], *args, **kwargs)
+
+    pltvec(qlab, 'r+', ms=12, label='hkl')
+    pltvec([-ki, [0, 0, 0], kf, [0, 0, 0], qdet], 'k-', lw=5, label='q = kf - ki')
+    pltvec([[0, 0, 0], qdet], 'm-', lw=5, label='q = kf - ki')
+    pltvec([[0, 0, 0], astar], 'b-', lw=5, label='astar')
+    pltvec([[0, 0, 0], bstar], 'g-', lw=5, label='bstar')
+    pltvec([[0, 0, 0], cstar], 'y-', lw=5, label='cstar')
+    labels(None, 'Y', 'Z', 'X', legend=True)
+    ax.set_xlim([2, -2])
+    ax.set_ylim([2, -2])
+    ax.set_zlim([-2, 2])
+    #ax.invert_xaxis()
+    #ax.invert_yaxis()
+    plt.show()
+
+
+def plot_xray_scattering_factor(elements, maxq=10):
+    """
+    Plot x-ray scattering factor for 1 or more elements
+    :param elements:
+    :return: None
+    """
+
+    q = np.linspace(0, maxq, 200)
+    xrf = fc.xray_scattering_factor(elements, q)
+
+    newplot(q, xrf)
+    plt.legend(np.asarray(elements).reshape(-1), loc=0, frameon=False, fontsize=18)
+    labels('X-Ray Scattering Factor', r'Q [$\AA^{-1}$]')
+
+
+def plot_magnetic_form_factor(elements, maxq=10):
+    """
+    Plot magnetic form factor for 1 or more elements
+    :param elements:
+    :return: None
+    """
+
+    q = np.linspace(0, maxq, 200)
+    mff = fc.magnetic_form_factor(elements, q)
+
+    newplot(q, mff)
+    plt.legend(np.asarray(elements).reshape(-1), loc=0, frameon=False, fontsize=18)
+    labels('Magnetic Form Factor', r'Q [$\AA^{-1}$]')
+
+
+def plot_xray_attenuation(elements, min_energy=0, max_energy=20):
+    """
+    Plot x-ray scattering factor for 1 or more elements
+    :param elements:
+    :return: None
+    """
+
+    Zarray = fc.atom_properties(elements, 'Z')
+    ene = np.arange(min_energy, max_energy+0.01, 0.01)
+
+    Aarray = fc.attenuation(Zarray, ene)
+    newplot(ene, Aarray)
+    plt.yscale('log')
+    plt.xlim([min_energy, max_energy])
+    plt.legend(np.asarray(elements).reshape(-1), loc=0, frameon=False, fontsize=18)
+    labels('X-Ray Attenuation', 'Energy [keV]', r'$\mu/\rho$ [cm$^2$/g]')
+
+
+def plot_atomic_scattering_factor(element, min_energy=0.5, max_energy=20):
+    """
+    Plot atomic scattering factor for 1 or more elements
+    :param element: str name of element to plot
+    :param min_energy: float min energy in keV
+    :param max_energy: float max energy in keV
+    :return: None
+    """
+
+    ene = np.arange(min_energy, max_energy+0.01, 0.01)
+    f1, f2 = fc.atomic_scattering_factor(element, ene)
+
+    newplot(ene, f1, '-', lw=2, label='f1')
+    plt.plot(ene, f2, '-', lw=2, label='f2')
+    plt.xlim([min_energy, max_energy])
+    labels('X-Ray Scattering Factor\n%s' % element, 'Energy [keV]', None, legend=True)
+
+
+def plot_xray_transmission(chemical_formula, density=8.9, energy_range=None, thickness_um=100):
+    """
+    Plot transmission of x-ray through a slab of material at range of energies
+    Equivalent to https://henke.lbl.gov/optical_constants/filter2.html
+    Based on formulas from: Henke, Gullikson, and Davis, Atomic Data and Nuclear Data Tables 54 no.2, 181-342 (July 1993)
+    :param chemical_formula: str molecular formula
+    :param density: float density in g/cm^3
+    :param energy_range: array x-ray energy in keV, None for default range
+    :param thickness_um: slab thickness in microns
+    :return: float or array
+    """
+    if energy_range is None:
+        energy_range = np.arange(0.03, 20, 0.01)
+
+    transmission = fc.filter_transmission(chemical_formula, energy_range, density, thickness_um)
+    ttl = '%s Density=%5.3f, thickness=%3.3g μm' % (chemical_formula, density, thickness_um)
+
+    newplot(energy_range, transmission)
+    labels(ttl, 'Energy [keV]', 'Transmission')
+
+
+def plot_xray_attenuation_length(chemical_formula, density=8.9, energy_range=None, grazing_angle=90):
+    """
+    Plot the X-Ray Attenuation Length of a compound
+    Equivalent to: https://henke.lbl.gov/optical_constants/atten2.html
+    Based on formulas from: Henke, Gullikson, and Davis, Atomic Data and Nuclear Data Tables 54 no.2, 181-342 (July 1993)
+    :param chemical_formula: str molecular formula
+    :param density: float density in g/cm^3
+    :param energy_range: array x-ray energy in keV, None for default range
+    :param grazing_angle: incidence angle relative to the surface, in degrees
+    :return: float or array, in microns
+    """
+    if energy_range is None:
+        energy_range = np.arange(0.03, 20, 0.01)
+
+    transmission = fc.molecular_attenuation_length(chemical_formula, energy_range, density, grazing_angle)
+    ttl = '%s Density=%5.3f, Angle=%3.3g deg' % (chemical_formula, density, grazing_angle)
+
+    newplot(energy_range, transmission)
+    labels(ttl, 'Energy [keV]', 'Atten Length [μm]')
+
+
+def plot_xray_reflectivity(chemical_formula, density=8.9, energy_range=None, grazing_angle=2):
+    """
+    Plot the specular reflectivity of a material
+    From: https://xdb.lbl.gov/Section4/Sec_4-2.html
+    :param chemical_formula: str molecular formula
+    :param density: float, density in g/cm^3
+    :param energy_range: float or array, x-ray energy in keV
+    :param grazing_angle: float, incidence angle relative to the surface, in degrees
+    :return: None
+    """
+    if energy_range is None:
+        energy_range = np.arange(0.03, 20, 0.01)
+
+    reflectivity = fc.molecular_reflectivity(chemical_formula, energy_range, density, grazing_angle)
+    ttl = '%s Density=%5.3f, Angle=%3.3g deg' % (chemical_formula, density, grazing_angle)
+
+    newplot(energy_range, reflectivity)
+    labels(ttl, 'Energy [keV]', 'Reflectivity')
+
+
+def plot_xray_refractive_index(chemical_formula, density=8.9, energy_range=None):
+    """
+    Plot the Complex Index of Refraction of a compound
+        n = 1 - (1/2pi)N*r0*lambda^2*(f1+if2) = 1 - Delta - iBeta
+    Equivalent to: https://henke.lbl.gov/optical_constants/getdb2.html
+    Based on formulas from: Henke, Gullikson, and Davis, Atomic Data and Nuclear Data Tables 54 no.2, 181-342 (July 1993)
+    :param chemical_formula: str molecular formula
+    :param density: float density in g/cm^3
+    :param energy_range: array x-ray energy in keV, None for default range
+    :return: float or array, in microns
+    """
+    if energy_range is None:
+        energy_range = np.arange(0.03, 20, 0.01)
+
+    n, delta, beta = fc.molecular_refractive_index(chemical_formula, energy_range, density)
+    ttl = '%s Density=%5.3f\nIndex of Refraction = 1 - δ - iβ' % (chemical_formula, density)
+
+    newplot(energy_range, delta, 'r-', lw=2, label='δ')
+    plt.plot(energy_range, beta, 'b-', lw=2, label='β')
+    labels(ttl, 'Energy [keV]', None, legend=True)
+    plt.xscale('log')
+    plt.yscale('log')
+
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/functions_scattering.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/functions_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/multiple_scattering.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/multiple_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tensor_scattering.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tensor_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/__init__.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,31 +6,35 @@
   Requires:
       numpy, matplotlib, tkinter
 
 By Dan Porter, PhD
 Diamond
 2019
 
-Version 3.0.0
-Last updated: 25/06/23
+Version 3.1.3
+Last updated: 28/03/24
 
 Version History:
 10/11/17 0.1    Program created
 23/02/19 1.0    Finished the basic program and gave it colours
 09/03/19 1.1    Added properties, superstructure, other improvements
 13/07/19 1.2    Added FDMNES windows
 13/12/19 2.0    Changed to internal tkgui package
 19/04/20 2.1    Added multi-crystal, write-cif buttons, changed layout of scattering gui
 27/04/20 2.2    Added SelectionBox to basic_widgets and spacegroup entry to SymmetryGui
 15/10/20 2.2.1  Slight correction to SymmetryGui - no longer adds 'm' to labels
 21/01/21 2.2.2  Added 'xray dispersion' scattering option
 26/01/21 2.3.0  Refactored properites into new file, added x-ray interactions GUI
 16/05/23 2.4.0  Added periodic_table.py and added menu items to CrystalGUI. Changed default fonts and colours
 25/06/23 3.0.0  Added new GUI elements including new Scattering UI, diffractomter simulator, unit converter
+20/07/23 3.1.0  Added new FDMNES GUI elements including in the Menu
+19/10/23 3.1.1  Fixed scaling issue in diffractometer.py. Thanks asteppke!
+25/10/23 3.1.2  Fixed error with powder plot for Neutrons. Thanks Cyril!
+28/03/24 3.1.3  Fixed error with site symmetries having spaces in AtomsGui, use RegEx instead
 
 @author: DGPorter
 """
 
 from .crystal import CrystalGui
 
-__version__ = '3.0.0'
-__date__ = '25/06/23'
+__version__ = '3.1.3'
+__date__ = '28/03/24'
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/basic_widgets.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/basic_widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 """
 
 import sys
 import re
 
 if sys.version_info[0] < 3:
     import Tkinter as tk
+    import tkFileDialog as filedialog
     import tkMessageBox as messagebox
 else:
     import tkinter as tk
+    from tkinter import filedialog
     from tkinter import messagebox
 
 # Fonts
 TF = ['Palatino', 12]  # ["Times", 12]
 BF = ['Palatino', 14]  # ["Times", 14]
 SF = ['Palatino', 14]  # ["Times New Roman", 14]
 LF = ['Palatino', 14]  # ["Times", 14]
 MF = ["Courier", 8]  # fixed distance format
-HF = ['Courier',12]
+HF = ['Courier', 12]
 TTF = ("Helvetica", 10, "bold italic")
 # Colours - background
 bkg = 'snow'  # background colour
 ety = 'white'  # entry box
 btn = 'azure'  # buttons 'light slate blue'
 opt = 'azure'  # option background  'light slate blue'
 btn2 = 'gold'  # main button
@@ -66,17 +68,17 @@
     btn2 = 'gold'
 
 
 def popup_message(parent, title, message):
     """Create a message box"""
     root = tk.Toplevel(parent)
     root.title(title)
-    #frame = tk.Frame(root)
+    # frame = tk.Frame(root)
     tk.Label(root, text=message, padx=20, pady=20).pack()
-    #root.after(2000, root.destroy)
+    # root.after(2000, root.destroy)
     return root
 
 
 def popup_about():
     """Create about message"""
     from Dans_Diffraction import version_info, module_info
     msg = "%s\n\n" \
@@ -122,23 +124,60 @@
 
 def menu_github():
     """Open GitHub page"""
     import webbrowser
     webbrowser.open_new_tab("https://github.com/DanPorter/Dans_Diffraction#dans_diffaction")
 
 
+def search_re(pattern, text):
+    matches = []
+    text = text.splitlines()
+    for i, line in enumerate(text):
+        for match in re.finditer(pattern, line):
+            if match.groups():
+                matches.append((f"{i + 1}.{match.span(1)[0]}", f"{i + 1}.{match.span(1)[1]}"))
+            else:
+                matches.append((f"{i + 1}.{match.start()}", f"{i + 1}.{match.end()}"))
+    return matches
+
+
+def text_search(text: tk.Text, search_pattern: str, highlight_colour='yellow'):
+    """
+    Find string patterns in tk Text object and highlight them
+    :param text: tk.Text object
+    :param search_pattern: str text to search for or Regular expression
+    :param highlight_colour: str color spec
+    :return: None
+    """
+    # Remove all tags so they can be redrawn
+    for tag in text.tag_names():
+        text.tag_remove(tag, "1.0", tk.END)
+
+    if not search_pattern: return
+
+    # Add tags where the search_re function found the pattern
+    for i, (start, end) in enumerate(search_re(search_pattern, text.get('1.0', tk.END))):
+        text.tag_add(f'{i}', start, end)
+        text.tag_config(f'{i}', background=highlight_colour)
+    # Scroll to first instance
+    index = text.search(search_pattern, '1.0')
+    if index:
+        text.see(index)
+
+
 class StringViewer:
     """
     Simple GUI that displays strings
         StringViewer(string, title, width)
     """
 
     def __init__(self, string, title='', width=40):
         """Initialise"""
         # Create Tk inter instance
+        self.title = title
         self.root = tk.Tk()
         self.root.wm_title(title)
         # self.root.minsize(width=640, height=480)
         self.root.maxsize(width=self.root.winfo_screenwidth(), height=self.root.winfo_screenheight())
         self.root.tk_setPalette(
             background=bkg,
             foreground=txtcol,
@@ -160,14 +199,27 @@
 
         # --- Button ---
         frm1 = tk.Frame(frame)
         frm1.pack(side=tk.BOTTOM, fill=tk.X)
         var = tk.Button(frm1, text='Close', font=BF, command=self.fun_close, bg=btn, activebackground=btn_active)
         var.pack(fill=tk.X)
 
+        # --- Search ---
+        self.search_str = tk.StringVar(self.root, '')
+        frm1 = tk.Frame(frame)
+        frm1.pack(side=tk.BOTTOM, fill=tk.X)
+        var = tk.Entry(frm1, textvariable=self.search_str)
+        var.pack(side=tk.LEFT)
+        var.bind('<Return>', self.fun_search)
+        var.bind('<KP_Enter>', self.fun_search)
+        var = tk.Button(frm1, text='Search', font=BF, command=self.fun_search, bg=btn, activebackground=btn_active)
+        var.pack(side=tk.LEFT)
+        var = tk.Button(frm1, text='SaveAs', font=BF, command=self.fun_saveas, bg=btn, activebackground=btn_active)
+        var.pack(side=tk.RIGHT)
+
         # --- Text box ---
         frame_box = tk.Frame(frame)
         frame_box.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
 
         # Scrollbars
         scanx = tk.Scrollbar(frame_box, orient=tk.HORIZONTAL)
         scanx.pack(side=tk.BOTTOM, fill=tk.X)
@@ -180,14 +232,31 @@
         self.text.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
         self.text.insert(tk.END, string)
 
         self.text.config(xscrollcommand=scanx.set, yscrollcommand=scany.set)
         scanx.config(command=self.text.xview)
         scany.config(command=self.text.yview)
 
+    def fun_search(self, event=None):
+        """Search"""
+        text_search(self.text, self.search_str.get())
+
+    def fun_saveas(self):
+        """Save as text file"""
+        filename = filedialog.asksaveasfilename(
+            parent=self.root,
+            title='Save as text file',
+            initialfile='%s.txt' % self.title,
+            filetypes=[('Text file', '*.txt')],
+        )
+        if filename:
+            with open(filename, 'wt') as f:
+                f.write(self.text.get('1.0', tk.END))
+            print('File written: %s' % filename)
+
     def fun_close(self):
         """close window"""
         self.root.destroy()
 
 
 "------------------------------------------------------------------------"
 "----------------------------Selection Box-------------------------------"
@@ -333,8 +402,7 @@
         self.output = [self.data_fields[n] for n in selection]
         self.root.destroy()
 
     def f_exit(self, event=None):
         """Closes the current data window"""
         self.output = self.initial_selection
         self.root.destroy()
-
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/converter.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         self.fwhm_deg = tk.StringVar(self.root, '0.1')
         self.fwhm_q = tk.StringVar(self.root, '0.008')
 
         self.dom_size = tk.StringVar(self.root, '807.44')
         self.dom_size_unit = tk.StringVar(self.root, u'\u212B')
         self._dom_size_unit = tk.StringVar(self.root, u'\u212B')
 
+        self.refine_hkl = False  # used in self.update_hkl, altered in self.but_hkl_switch
 
         # --- Mass / Wavelength / Energy ---
         frame = tk.Frame(self.root)
         frame.pack(side=tk.TOP, fill=tk.X, expand=tk.YES, padx=6, pady=2)
         var = tk.Label(frame, text='Mass: ', font=TTF, width=10)
         var.pack(side=tk.LEFT)
         var = tk.Entry(frame, textvariable=self.mass, font=TF, width=12, bg=ety, fg=ety_txt)
@@ -138,22 +139,26 @@
 
         # --- Reflection / Angle ---
         frame = tk.Frame(self.root, relief=tk.RIDGE)  # horizontal line
         frame.pack(side=tk.TOP, fill=tk.X, expand=tk.YES, padx=2, pady=4)
 
         frame = tk.Frame(self.root)
         frame.pack(side=tk.TOP, fill=tk.X, expand=tk.YES, padx=6, pady=6)
-        var = tk.Label(frame, text='hkl: ', font=TTF, width=4)
+        var = tk.Label(frame, text='hkl: ', font=TTF, width=4, borderwidth=0, relief="ridge")
         var.pack(side=tk.LEFT)
+        var.bind("<Button-1>", self.but_hkl_switch)
+        self.hkl_label = var
         var = tk.Entry(frame, textvariable=self.hkl, font=TF, width=20, bg=ety, fg=ety_txt)
         var.pack(side=tk.LEFT)
         var.bind('<Return>', self.fun_hkl)
         var.bind('<KP_Enter>', self.fun_hkl)
-        var = tk.Label(frame, text='Lattice: ', font=TTF)
+        var = tk.Label(frame, text='Lattice: ', font=TTF, borderwidth=2, relief="ridge")
         var.pack(side=tk.LEFT, padx=6)
+        var.bind("<Button-1>", self.but_latt_switch)
+        self.lattice_label = var
         var = tk.Entry(frame, textvariable=self.latt, font=TF, width=8, bg=ety, fg=ety_txt)
         var.pack(side=tk.LEFT)
         var.bind('<Return>', self.fun_setlat)
         var.bind('<KP_Enter>', self.fun_setlat)
         var = tk.Label(frame, text=u'\u212B', font=TF)
         var.pack(side=tk.LEFT)
         var = tk.Button(frame, text='Latt', command=self.fun_latt, font=BF, bg=btn,
@@ -307,14 +312,24 @@
         LatparGui(self.xtl)
 
     def fun_setlat(self, event=None):
         latt = float(self.latt.get())
         self.xtl.Cell.latt(latt)  # set cubic lattice
         self.fun_hkl()
 
+    def but_hkl_switch(self, event=None):
+        self.lattice_label.config(borderwidth=0)
+        self.hkl_label.config(borderwidth=2)
+        self.refine_hkl = True
+
+    def but_latt_switch(self, event=None):
+        self.lattice_label.config(borderwidth=2)
+        self.hkl_label.config(borderwidth=0)
+        self.refine_hkl = False
+
     def fun_hkl(self, event=None):
         hkl = fg.str2array(self.hkl.get())
         wavelength_a = self.get_wavelength_a()
         tth = self.xtl.Cell.tth(hkl, wavelength_a=wavelength_a)[0]
         dspace = self.xtl.Cell.dspace(hkl)[0]
         qmag = self.xtl.Cell.Qmag(hkl)[0]
         self.tth.set(FMT % tth)
@@ -324,17 +339,28 @@
 
     def update_hkl(self, qmag):
         old_hkl = fg.str2array(self.hkl.get())
         oldq = self.xtl.Cell.calculateQ(old_hkl)[0]
         oldqmag = fg.mag(oldq)
         newq = oldq * qmag / oldqmag
         new_hkl = self.xtl.Cell.indexQ(newq)[0]
-        hkl_str = ' '.join([FMT % h for h in new_hkl])
-        self.hkl.set(hkl_str)
-        self.fun_hkl()
+
+        if self.refine_hkl:
+            # Update hkl
+            hkl_str = ' '.join([FMT % h for h in new_hkl])
+            self.hkl.set(hkl_str)
+            self.fun_hkl()
+        else:
+            # update lattice
+            old_lat = self.xtl.Cell.lp()
+            new_lat = [old_lat[n] * old_hkl[n] / new_hkl[n] if abs(old_hkl[n]) > 0 else old_lat[n] for n in range(3)]
+            new_lat.extend(old_lat[3:])
+            self.xtl.Cell.latt(new_lat)
+            self.latt.set('%.3f' % new_lat[0])
+            self.fun_hkl()
 
     def fun_tth(self, event=None):
         wavelength_a = self.get_wavelength_a()
         tth = float(self.tth.get())
         qmag = fc.calqmag(tth, wavelength_a=wavelength_a)
         self.update_hkl(qmag)
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/crystal.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/crystal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 """
 Main crystal gui windows
 """
 
 import sys, os
+import re
 import matplotlib.pyplot as plt  # Plotting
 import numpy as np
 
-
-if sys.version_info[0] < 3:
-    import Tkinter as tk
-    import tkFileDialog as filedialog
-    import tkMessageBox as messagebox
-else:
-    import tkinter as tk
-    from tkinter import filedialog
-    from tkinter import messagebox
-
 # Internal functions
 from ..classes_crystal import Crystal
 from ..classes_structures import Structures
 from ..classes_fdmnes import fdmnes_checker
 from .. import functions_crystallography as fc
+from .basic_widgets import tk, filedialog, messagebox
 from .basic_widgets import StringViewer, SelectionBox, popup_help, popup_about, topmenu, menu_github, menu_docs
 from .basic_widgets import (TF, BF, SF, HF, TTF,
                             bkg, ety, btn, opt, btn_active, opt_active, txtcol,
                             ety_txt)
 from .properties import PropertiesGui
 from .scattering import ScatteringGui
 from .multi_crystal import MultiCrystalGui
@@ -45,14 +37,17 @@
             self.xtl = xtl
 
         # start matplotlib interactive mode
         plt.ion()
 
         # Create Tk inter instance
         self.root = tk.Tk()
+        #icon = tk.PhotoImage(file=os.path.dirname(__file__) + '/../../DD_icon.png')
+        #self.root.iconphoto(True, icon)
+        # self.root.iconbitmap(default=os.path.dirname(__file__) + '/../../DD_icon.ico')  # test this on linux first!
         self.root.wm_title('Crystal  by D G Porter [dan.porter@diamond.ac.uk]')
         # self.root.minsize(width=640, height=480)
         self.root.maxsize(width=self.root.winfo_screenwidth(), height=self.root.winfo_screenheight())
         self.root.tk_setPalette(
             background=bkg,
             foreground=txtcol,
             activeBackground=opt_active,
@@ -60,35 +55,39 @@
 
         self.structure_list = Structures()
 
         # ---Menu---
         menu = {
             'File': {
                 'New Window': self.menu_new,
+                'Copy filename to clipboard': self.menu_file_clipboard,
                 'Exit': self.on_closing,
             },
             'Crystal Info': {
                 'Crystal': self.menu_info_crystal,
                 'Symmetric Atom Sites': self.menu_info_atoms,
                 'Symmetry': self.menu_info_symmetry,
                 'All Atom Sites': self.menu_info_structure,
+                'Reflection list': self.menu_ref_list,
                 'Properties': self.menu_info_properties,
                 'Show CIF': self.menu_info_cif,
                 'Latex table': self.menu_latex,
+                'FDMNES indata': self.menu_fdmnes_indata,
             },
             'Databases': {
                 'Element Info': self.menu_info_elements,
                 'Periodic Table': self.menu_info_table,
                 'X-Ray Interactions': self.menu_xray_interactions,
                 'Spacegroup Viewer': self.menu_spacegroups,
                 'Unit Converter': self.menu_converter,
             },
             'Help': {
                 'Help': popup_help,
                 # 'Dark mode': self.menu_darkmode,
+                'Set scale': self.menu_scale,
                 'Examples': self.menu_examples,
                 'Activate FDMNES option': self.menu_start_fdmnes,
                 'Analyse FDMNES data': self.menu_analyse_fdmnes,
                 'Documentation': menu_docs,
                 'GitHub Page': menu_github,
                 'About': popup_about,
             }
@@ -181,18 +180,17 @@
         var = tk.Button(f_but, text='Diffractometer\nSimulator', bg=btn, activebackground=btn_active, font=BF,
                         command=self.fun_diffractometer)
         var.pack(side=tk.LEFT)
         # Remove Tensor-Scattering 26/05/20
         #var = tk.Button(f_but, text='Tensor\nScattering', bg=btn, activebackground=btn_active, font=BF,
         #                command=self.fun_tensor_scattering)
         #var.pack(side=tk.LEFT)
-        if fdmnes_checker():
-            var = tk.Button(f_but, text='Run\nFDMNES', bg=btn, activebackground=btn_active, font=BF,
-                            command=self.fun_fdmnes)
-            var.pack(side=tk.LEFT)
+        var = tk.Button(f_but, text='FDMNES', bg=btn, activebackground=btn_active, font=BF, height=2,
+                        command=self.fun_fdmnes)
+        var.pack(side=tk.LEFT)
 
         # start mainloop
         # In interactive mode, this freezes the terminal
         # To stop this, need a way of checking if interactive or not ('-i' in sys.argv)
         # However sys in this file is not the same as sys in the operating script
         self.root.protocol("WM_DELETE_WINDOW", self.on_closing)
         self.root.mainloop()
@@ -200,14 +198,19 @@
     ###################################################################################
     ################################# MENU ############################################
     ###################################################################################
     def menu_new(self):
         """Create a new instance"""
         CrystalGui()
 
+    def menu_file_clipboard(self):
+        """Add filename to clipboard"""
+        self.root.clipboard_clear()
+        self.root.clipboard_append(self.xtl.filename)
+
     def menu_info_crystal(self):
         """Crystal info"""
         string = '%s\n%s' % (self.xtl.filename, self.xtl.info())
         StringViewer(string, self.xtl.name, width=60)
 
     def menu_info_atoms(self):
         """Atoms info"""
@@ -220,14 +223,20 @@
         StringViewer(string, self.xtl.name, width=60)
 
     def menu_info_symmetry(self):
         """Symmetry info"""
         string = '%s\n%s' % (self.xtl.name, self.xtl.Symmetry.info())
         StringViewer(string, self.xtl.name, width=60)
 
+    def menu_ref_list(self):
+        """Reflection list"""
+        from .scattering import ReflectionSelectionBox
+        out = ReflectionSelectionBox(self.xtl, self.root).show()
+        print(out)
+
     def menu_info_properties(self):
         """Properties info"""
         string = '%s\n%s' % (self.xtl.name, self.xtl.Properties.info())
         StringViewer(string, self.xtl.name, width=60)
 
     def menu_info_cif(self):
         """Print cif"""
@@ -267,14 +276,19 @@
         XrayInteractionsGui(self.xtl)
 
     def menu_spacegroups(self):
         """Open Spacegroup viewer gui"""
         from .spacegroups import SpaceGroupGui
         SpaceGroupGui(self.xtl.Symmetry)
 
+    def menu_scale(self):
+        """Change the scale of the tkinter instance"""
+        print('pixels in 1 inch: %s' % self.root.winfo_fpixels('1i'))
+        self.root.tk.call('tk', 'scaling', self.root.winfo_fpixels('1i')/72)
+
     def menu_examples(self):
         """List example files, open in system viewer"""
         import subprocess, platform, ast
 
         example_dir = os.path.join(os.path.split(__file__)[0], '../../Examples')
         if not os.path.isdir(example_dir):
             messagebox.showwarning(
@@ -324,23 +338,33 @@
         except KeyError:
             messagebox.showwarning(
                 parent=self.root,
                 title='CIF Table',
                 message='No .cif file associated with this crystal'
             )
 
+    def menu_fdmnes_indata(self):
+        """Display FDMNES indata file"""
+        if self.xtl.Structure.ismagnetic():
+            fdm = self.xtl.Properties.fdmnes_runfile(magnetism=True)
+        else:
+            fdm = self.xtl.Properties.fdmnes_runfile()
+        StringViewer(fdm, self.xtl.name, width=120)
+
     def menu_start_fdmnes(self):
         """Search for FDMNES, restart GUI"""
-        from Dans_Diffraction import activate_fdmnes, fdmnes_checker, start_gui
-        activate_fdmnes()
-        if fdmnes_checker():
-            self.on_closing()
-            start_gui(self.xtl)
-        else:
-            messagebox.showinfo('FDMNES Checker', 'FDMNES could not be found')
+        from Dans_Diffraction import activate_fdmnes
+        filename = filedialog.askopenfilename(
+            parent=self.root,
+            title='Select FDMNES Executable',
+            filetypes=[('EXE File', '*.exe'), ('All Files', '*.*')],
+            initialfile='fdmnes_win64.exe',
+        )
+        if filename:
+            activate_fdmnes(fdmnes_filename=filename)
 
     def menu_analyse_fdmnes(self):
         """Open FDMNS analysis GUI"""
         from .fdmnes import AnaFDMNESgui
         AnaFDMNESgui()
 
     def menu_darkmode(self):
@@ -696,18 +720,24 @@
 
         # Close window
         self.root.destroy()
 
         AtomsGui(self.xtl, self.symmetric_only, not self.magnetic_moments)
 
     def fun_update(self):
-        "Update atomic properties, close window"
+        """Update atomic properties, close window"""
         # Get string from text box
         s = self.text.get('1.0', tk.END)
 
+        # regular expression matching text string
+        rex = r'\s*?(\d+)\s+(\w+?)\s+(\w+?)\s+\w+?\s\(.+?\)' + r'\s+(\d+?.\d+)'*5
+        if self.magnetic_moments:
+            rex += r'\s+(\d+?.\d+)'*3
+        reg_match = re.compile(rex)
+
         # Analyse string
         """
         values = np.genfromtxt(str)
         n = values[:,0]
         type = values[:,1]
         label = values[:,2]
         u = values[:,3]
@@ -725,28 +755,30 @@
         w = []
         occ = []
         uiso = []
         mx = []
         my = []
         mz = []
         for ln in lines:
-            items = ln.split()
+            m = reg_match.match(ln)
+            if m is None: continue
+            items = m.groups()
             if len(items) < 8: continue
             n += [int(items[0])]
             scattering_type += [items[1]]
             label += [items[2]]
-            u += [float(items[5])]
-            v += [float(items[6])]
-            w += [float(items[7])]
-            occ += [float(items[8])]
-            uiso += [float(items[9])]
+            u += [float(items[3])]
+            v += [float(items[4])]
+            w += [float(items[5])]
+            occ += [float(items[6])]
+            uiso += [float(items[7])]
             if self.magnetic_moments:
-                mx += [float(items[10])]
-                my += [float(items[11])]
-                mz += [float(items[12])]
+                mx += [float(items[8])]
+                my += [float(items[9])]
+                mz += [float(items[10])]
 
         self.Atoms.type = scattering_type
         self.Atoms.label = label
         self.Atoms.u = np.array(u)
         self.Atoms.v = np.array(v)
         self.Atoms.w = np.array(w)
         self.Atoms.occupancy = np.array(occ)
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/diffractometer.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/diffractometer.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,32 +19,35 @@
 the sum of the detector at each step
 
  Dr Daniel G Porter, dan.porter@diamond.ac.uk
  www.diamond.ac.uk
  Diamond Light Source, Chilton, Didcot, Oxon, OX11 0DE, U.K.
 """
 
-import matplotlib.pyplot as plt
 import numpy as np
+from itertools import cycle
 from matplotlib.figure import Figure
+from matplotlib.colors import TABLEAU_COLORS
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.backends.backend_tkagg import NavigationToolbar2Tk as NavigationToolbar2TkAgg
 
 from .. import functions_general as fg
 from .. import functions_crystallography as fc
 from .. import functions_plotting as fp
 from .. import Crystal
 from .basic_widgets import tk, StringViewer, messagebox, topmenu, popup_about
 from .basic_widgets import (TF, BF, SF, LF, HF, TTF,
                             bkg, ety, btn, opt, btn2,
                             btn_active, opt_active, txtcol,
                             btn_txt, ety_txt, opt_txt)
 
 # Figure DPI
-FIGURE_DPI = 60
+FIGURE_DPI = 80
+FIGURE_3D_SIZE = [8, 4]
+FIGURE_DET_SIZE = [7, 4]
 
 # Help messages
 MSG_PHI = "1st rotation, left handed roation about z'''-axis (crystal axis)"
 MSG_CHI = "2nd rotation, right handed rotation about y''-axis."
 MSG_ETA = "3rd rotation, left handed rotation about z'-axis"
 MSG_MU = "4th rotation, right handed rotation about diffractometer x-axis"
 MSG_DEL = "Detector rotation, left handed rotation about diffractometer z-axis"
@@ -59,32 +62,38 @@
 DEFAULT_DET_WIDTH = 200  # mm
 DEFAULT_DET_HEIGHT = 200  # mm
 DEFAULT_DET_PIXEL = 0.2  # mm
 # Plot options
 OPTIONS = {
     '3d_lattice': True,
     '3d_basis': False,
+    '3d_detector_corners': False,
+    '3d_ref_arrows': False,
     'det_labels': True,
     'det_log': False,
     'det_clim': [0.0, 1.0],
     'det_cmap': 'viridis',
-    'fig_dpi': 60,
+    'fig_dpi': FIGURE_DPI,
     'maxq': 4.0,
+    'min_intensity': 0.01
 }
 # Detector Reflection list
 REFLIST = {
     'hkl': np.zeros([0, 3], dtype=int),
     'qxqyqz': np.zeros([0, 3], dtype=float),
     'intensity': np.zeros([0], dtype=float),
     'scaled': np.zeros([0], dtype=float),
     'detx': np.zeros([0], dtype=float),
     'dety': np.zeros([0], dtype=float),
     'hkl_str': [],
     'fwhm': np.zeros([0], dtype=float),
+    'color': [],
 }
+# Colours
+col_cycle = cycle([TABLEAU_COLORS[c] for c in TABLEAU_COLORS])
 
 
 def default_fun(*args, **kwargs):
     return None
 
 
 def reflist_str():
@@ -121,14 +130,16 @@
 
         self.wavelength_a = 1  # A
         self.resolution = 0.5  # A-1
         self.domain_size = 1000  # A
         self.hkl = np.zeros([0, 3], dtype=float)
         self.initial_qxqyqz = np.zeros([0, 3], dtype=float)
         self.rotated_qxqyqz = np.zeros([0, 3], dtype=float)
+        self.initial_vectors = np.eye(3, dtype=float)
+        self.vectors = np.eye(3, dtype=float)
         self.qmag = np.zeros([0], dtype=float)
         self.tth = np.zeros([0], dtype=float)
         self.fwhm = np.zeros([0], dtype=float)
         self.hkl_str = []
         self.intensity = np.zeros([0], dtype=float)
         self._calculated = np.zeros([0], dtype=bool)
         self.rotate_to(0, 0, 0, 0)
@@ -158,25 +169,27 @@
     def rotate_to(self, phi=0., chi=0., eta=0., mu=0.):
         self._current_phi = phi
         self._current_chi = chi
         self._current_eta = eta
         self._current_mu = mu
         R = fc.diffractometer_rotation(phi, chi, eta, mu)
         self.rotated_qxqyqz = fc.labvector(self.initial_qxqyqz, self._u, R, self._lab)
+        self.vectors = fc.labvector(self.initial_vectors, self._u, R, self._lab)
 
     def generate_hkl(self, wavelength_a, max_q=4):
         """Generate reflection list"""
         self.wavelength_a = wavelength_a
         self.hkl = self.xtl.Cell.all_hkl(maxq=max_q)
         self.initial_qxqyqz = self.xtl.Cell.calculateQ(self.hkl)
+        self.initial_vectors = self.xtl.Cell.calculateQ([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
         self.qmag = fg.mag(self.initial_qxqyqz)
         self.tth = fc.cal2theta(self.qmag, wavelength_a=wavelength_a)
         tth = 1.0 * self.tth
         tth[tth > 175] = 175.  # stop peaks becoming too broad at high angle
-        self.fwhm = fc.scherrer_fwhm(self.domain_size, tth, wavelength_a=wavelength_a)
+        self.fwhm = fc.scherrer_fwhm(self.domain_size, tth, wavelength_a=wavelength_a, shape_factor=1.0)
         self.hkl_str = np.array(fc.hkl2str(self.hkl).split('\n'))
         self.intensity = np.zeros_like(self.qmag)
         self._calculated = np.zeros_like(self.qmag, dtype=bool)
         self.rotate_to(self._current_phi, self._current_chi, self._current_eta, self._current_mu)
 
     def generate_intensities(self, calculate_index=()):
         """Generate list of structure factors"""
@@ -231,24 +244,14 @@
         self._z_size = z_size
         self._initial_x_axis = x_size * fg.norm(np.cross(self.normal_dir, (0, 0, 1.)))
         self._initial_z_axis = z_size * fg.norm(np.cross(self.x_axis, self.normal_dir))
         self._pixel_size = pixel_size
         self._lab = labmatrix
         self.rotate_to(0, 0)
 
-        # Plot
-        self.fig2 = Figure(figsize=[6, 4], dpi=FIGURE_DPI)
-        self.fig2.patch.set_facecolor('w')
-        self.axd = self.fig2.add_subplot(111)
-        self.axd_image = self.axd.pcolormesh(np.zeros([10, 10]))
-        self.axd_center = self.axd.plot([0], [0], 'k+', ms=6, label='Centre')
-        self.axd_lattice = self.axd.plot([], [], 'k+', ms=6, label='Nearby reflections')
-        self.axd_allowed = self.axd.plot([], [], 'ro', ms=6, label='Reflections')
-        self.toolbar2 = None
-
     def __repr__(self):
         s = "Detector(delta=%.5g, gamma=%.5g)"
         return s % (self._current_delta, self._current_gamma)
 
     def set_detector(self, distance=1., normal_dir=(0, -1., 0), x_size=1., z_size=1.,
                      pixel_size=0.01):
         self._distance = distance
@@ -309,23 +312,42 @@
         c += [self.position - self.x_axis / 2 - self.z_axis / 2 + n * 0.01 * self.z_axis for n in range(100)]
         c += [self.position - self.x_axis / 2 + n * 0.01 * self.x_axis + self.z_axis / 2 for n in range(100)]
         c += [self.position + self.x_axis / 2 + self.z_axis / 2]
         wv = fc.wavevector(wavelength=wavelength_a)
         kf = wv * fg.norm(c)
         return kf - wv * fc.labvector([0, 1, 0], LAB=self._lab)
 
+    def ki(self, wavelength_a):
+        wv = fc.wavevector(wavelength=wavelength_a)
+        return wv * fc.labvector([0, 1, 0], LAB=self._lab)
+
     def kfkiq(self, wavelength_a):
         """Return lines traving kf, ki and Q"""
         wv = fc.wavevector(wavelength=wavelength_a)
         ki = wv * fc.labvector([0, 1, 0], LAB=self._lab)
         kf = wv * fg.norm(self.position)
         kikf = np.array([-ki, [0, 0, 0], kf])
         qq = np.array([[0, 0, 0], kf - ki])
         return kikf, qq
 
+    def kfkiq_corners(self, wavelength_a):
+        """Return lines to corners of kif, ki and Q"""
+        wv = fc.wavevector(wavelength=wavelength_a)
+        ki = wv * fc.labvector([0, 1, 0], LAB=self._lab)
+        kf = wv * fg.norm(self.corners())
+        z = [0, 0, 0]
+        kikf = np.vstack([-ki, z, kf[0], kf[1], z, kf[1],  kf[2], z, kf[2], kf[3], z, kf[3], kf[0]])
+        qq = np.array([
+            z, kf[0] - ki,
+            z, kf[1] - ki,
+            z, kf[2] - ki,
+            z, kf[3] - ki,
+        ])
+        return kikf, qq
+
     def twotheta(self):
         """Return detector angle in degrees"""
         incident = fc.labvector(self._initial_position, LAB=self._lab)
         return fg.vectors_angle_degrees(incident, self.position)
 
     def width_lim(self):
         return [-1000 * self._x_size / 2, 1000 * self._x_size / 2]
@@ -603,15 +625,15 @@
         new_unit = res_unit.get()
         if old_unit == 'eV':
             res = fc.wavevector(val / 1000.)
         elif old_unit == 'meV':  # neutron
             res = fc.wavevector(wavelength=fc.neutron_wavelength(val))
         elif old_unit == 'Deg':
             wavelength = get_wavelength()
-            res = fc.calqmag(val, fc.wave2energy(wavelength))
+            res = fc.calqmag(val, wavelength_a=wavelength)
         elif old_unit == u'\u212B':  # Angstroms
             res = fc.dspace2q(val)
         else:  # inverse angstroms
             res = val
         # Convert if changed
         if old_unit != new_unit:
             dspace = fc.q2dspace(res)
@@ -717,15 +739,15 @@
             peak_width.set(peakwidth_deg)
             peak_width_type.set(peak_width_types[0])
             _prev_peak_width_type.set(peak_width_types[0])
 
     # TK widgets
     OPT_WIDTH = 14
     frm = tk.LabelFrame(parent, text='Beam', relief=tk.RIDGE)
-    frm.pack(fill=tk.X, padx=2, pady=2)
+    frm.pack(fill=tk.BOTH, expand=tk.YES, padx=2, pady=2)
 
     # Radiation
     ln = tk.Frame(frm)
     ln.pack(side=tk.TOP, fill=tk.X)
     var = tk.Label(ln, text='Radiation:', font=SF)
     var.pack(side=tk.LEFT)
     var = tk.OptionMenu(ln, radiation_type, *radiations, command=fun_radiation)
@@ -852,15 +874,15 @@
         if pixel_size is not None:
             det_pixel_size.set(pixel_size)
 
     frm = tk.LabelFrame(parent, text='Detector', relief=tk.RIDGE)
     frm.pack(fill=tk.X, padx=2, pady=2)
 
     ln = tk.Frame(frm)
-    ln.pack(side=tk.TOP, fill=tk.X)
+    ln.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
     var = tk.Label(ln, text='Distance:', font=SF)
     var.pack(side=tk.LEFT)
     var = tk.Entry(ln, textvariable=det_distance, font=TF, width=8, bg=ety, fg=ety_txt)
     var.pack(side=tk.LEFT)
     var.bind('<Return>', fun_update_det)
     var.bind('<KP_Enter>', fun_update_det)
     var = tk.Label(ln, text='mm', font=SF)
@@ -1057,18 +1079,28 @@
             xx, yy, mesh = generate_reflections(
                 latt=latt,
                 det=det,
                 minimum_gaussian_intensity=0.01
             )
             scan_sum[n] = np.sum(mesh)
 
+        # Create new frame
+        newframe = tk.Toplevel(parent)
+        newframe.title('%s Scan' % angle_name)
+        fig = Figure(figsize=FIGURE_3D_SIZE, dpi=OPTIONS['fig_dpi'])
+        canvas = FigureCanvasTkAgg(fig, newframe)
+        canvas.get_tk_widget().configure(bg='black')
+        canvas.draw()
+
         # Plot data
-        fp.newplot(scan_range, scan_sum)
-        fp.labels(None, '%s [Deg]' % angle_name, 'Detector Sum')
-        plt.show()
+        ax = fig.add_subplot(111)
+        ax.plot(scan_range, scan_sum)
+        ax.set_xlabel('%s [Deg]' % angle_name)
+        ax.set_ylabel('Detector Sum')
+        canvas.get_tk_widget().pack(fill=tk.BOTH, expand=tk.YES)
 
     frm = tk.LabelFrame(parent, text='Scan', relief=tk.RIDGE)
     frm.pack(fill=tk.X, padx=2, pady=2)
 
     var = tk.OptionMenu(frm, scan_angle, *angle_dict.keys())
     var.config(font=SF, width=10, bg=opt, activebackground=opt_active)
     var["menu"].config(bg=opt, bd=0, activebackground=opt_active)
@@ -1121,21 +1153,24 @@
                      'hot', 'hot_r', 'hsv', 'rainbow', 'jet']
 
     root = tk.Toplevel(parent)
     root.title('Plot Options')
 
     pl_lattice = tk.BooleanVar(root, OPTIONS['3d_lattice'])
     pl_basis = tk.BooleanVar(root, OPTIONS['3d_basis'])
+    pl_det_corners = tk.BooleanVar(root, OPTIONS['3d_detector_corners'])
+    pl_ref_arrows = tk.BooleanVar(root, OPTIONS['3d_ref_arrows'])
     pl_labels = tk.BooleanVar(root, OPTIONS['det_labels'])
     pl_log = tk.BooleanVar(root, OPTIONS['det_log'])
     clim_min = tk.DoubleVar(root, OPTIONS['det_clim'][0])
     clim_max = tk.DoubleVar(root, OPTIONS['det_clim'][1])
     cmap = tk.StringVar(root, OPTIONS['det_cmap'])
     dpi = tk.IntVar(root, OPTIONS['fig_dpi'])
     maxq = tk.DoubleVar(root, OPTIONS['maxq'])
+    mininten = tk.DoubleVar(root, OPTIONS['min_intensity'])
 
     def fun_log(event=None):
         log = pl_log.get()
         cmin = clim_min.get()
         cmax = clim_max.get()
         if log:
             clim_min.set(round(np.log10(cmin+1), 3))
@@ -1143,34 +1178,41 @@
         else:
             clim_min.set(round(10 ** cmin - 1, 3))
             clim_max.set(round(10 ** cmax, 3))
 
     def fun_update():
         OPTIONS['3d_lattice'] = pl_lattice.get()
         OPTIONS['3d_basis'] = pl_basis.get()
+        OPTIONS['3d_detector_corners'] = pl_det_corners.get()
+        OPTIONS['3d_ref_arrows'] = pl_ref_arrows.get()
         OPTIONS['det_labels'] = pl_labels.get()
         OPTIONS['det_log'] = pl_log.get()
         OPTIONS['det_clim'] = [clim_min.get(), clim_max.get()]
         OPTIONS['det_cmap'] = cmap.get()
         OPTIONS['fig_dpi'] = dpi.get()
         OPTIONS['maxq'] = maxq.get()
+        OPTIONS['min_intensity'] = mininten.get()
         callback()
         root.destroy()
 
     ln = tk.Frame(root)
     ln.pack(side=tk.TOP, fill=tk.X)
     var = tk.Checkbutton(ln, text='Plot 3D Lattice', variable=pl_lattice, font=SF)
     var.pack(side=tk.LEFT, padx=3)
     var = tk.Checkbutton(ln, text='Plot 3D Basis', variable=pl_basis, font=SF)
     var.pack(side=tk.LEFT, padx=3)
+    var = tk.Checkbutton(ln, text='Plot 3D corners', variable=pl_det_corners, font=SF)
+    var.pack(side=tk.LEFT, padx=3)
 
     ln = tk.Frame(root)
     ln.pack(side=tk.TOP, fill=tk.X)
     var = tk.Checkbutton(ln, text='Detector HKL labels', variable=pl_labels, font=SF)
     var.pack(side=tk.LEFT, padx=3)
+    var = tk.Checkbutton(ln, text='Plot ref arrows', variable=pl_ref_arrows, font=SF)
+    var.pack(side=tk.LEFT, padx=3)
 
     ln = tk.Frame(root)
     ln.pack(side=tk.TOP, fill=tk.X)
     var = tk.Label(ln, text='Detector Clim:', font=SF)
     var.pack(side=tk.LEFT)
     var = tk.Entry(ln, textvariable=clim_min, font=TF, width=8, bg=ety, fg=ety_txt)
     var.pack(side=tk.LEFT)
@@ -1192,14 +1234,18 @@
     var.pack(side=tk.LEFT)
     var = tk.Entry(ln, textvariable=dpi, font=TF, width=8, bg=ety, fg=ety_txt)
     var.pack(side=tk.LEFT)
     var = tk.Label(ln, text='3D Plot Max:', font=SF)
     var.pack(side=tk.LEFT)
     var = tk.Entry(ln, textvariable=maxq, font=TF, width=8, bg=ety, fg=ety_txt)
     var.pack(side=tk.LEFT)
+    var = tk.Label(ln, text='Min Intensity:', font=SF)
+    var.pack(side=tk.LEFT)
+    var = tk.Entry(ln, textvariable=mininten, font=TF, width=8, bg=ety, fg=ety_txt)
+    var.pack(side=tk.LEFT)
 
     ln = tk.Frame(root)
     ln.pack(side=tk.TOP, fill=tk.X)
     var = tk.Button(ln, text='Update', font=TF, command=fun_update, bg=btn,
                     activebackground=btn_active)
     var.pack(pady=2)
 
@@ -1208,41 +1254,148 @@
     """Orientation options window"""
     root = tk.Toplevel(parent)
     root.title('Orientation Options')
 
     ustr = str(latt._u.tolist()).replace('], [', '\n').replace('[', '').replace(']', '')
     lstr = str(latt._lab.tolist()).replace('], [', '\n').replace('[', '').replace(']', '')
 
-    ln = tk.Frame(root)
+    right = tk.Frame(root, relief=tk.RAISED)
+    right.pack(side=tk.RIGHT, fill=tk.Y, expand=tk.YES, padx=6)
+
+    # Tranformation
+    def fun_transform(event=None):
+        mat = transform_optoins[transform.get()]
+        for m in range(3):
+            for n in range(3):
+                matrix_vars[m][n].set(mat[m, n])
+
+    transform_optoins = {
+        'c || z, b || y': np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]]),
+        'c || z, b || x': np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]]),
+        'a || z, b || x': np.array([[0, 0, 1], [1, 0, 0], [0, 1, 0]]),
+        'a || z, z || x': np.array([[0, 0, 1], [0, 1, 0], [1, 0, 0]]),
+        'b || z, z || x': np.array([[0, 1, 0], [0, 0, 1], [1, 0, 0]]),
+        'b || z, a || x': np.array([[1, 0, 0], [0, 0, 1], [0, 1, 0]]),
+    }
+    transform = tk.StringVar(root, 'c || z, b || y')
+    var = tk.OptionMenu(right, transform, *transform_optoins, command=fun_transform)
+    var.config(font=SF, bg=opt, activebackground=opt_active)
+    var["menu"].config(bg=opt, bd=0, activebackground=opt_active)
+    var.pack(side=tk.TOP)
+
+    # Rotation
+    ln = tk.Frame(right)
+    ln.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES, pady=4)
+    var = tk.Label(ln, text='Rotate ', font=SF)
+    var.pack(side=tk.LEFT)
+    angle_deg = tk.DoubleVar(root, 0)
+    var = tk.Entry(ln, textvariable=angle_deg, font=TF, width=3, bg=ety, fg=ety_txt)
+    var.pack(side=tk.LEFT)
+    var = tk.Label(ln, text='Deg, about ', font=SF)
+    var.pack(side=tk.LEFT)
+
+    def fun_rotate():
+        angle = angle_deg.get()
+        rmat = rotate_options[rotate_about.get()](angle)
+        cmat = np.array([[matrix_vars[m][n].get() for n in range(3)] for m in range(3)])
+        nmat = np.dot(rmat, cmat.T).T
+        for m in range(3):
+            for n in range(3):
+                matrix_vars[m][n].set(nmat[m, n])
+
+    rotate_options = {
+        'X': fc.rotmatrixx,
+        'Y': fc.rotmatrixy,
+        'Z': fc.rotmatrixz,
+    }
+    rotate_about = tk.StringVar(root, 'Z')
+    var = tk.OptionMenu(ln, rotate_about, *rotate_options)
+    var.config(font=SF, bg=opt, activebackground=opt_active)
+    var["menu"].config(bg=opt, bd=0, activebackground=opt_active)
+    var.pack(side=tk.LEFT)
+    var = tk.Button(ln, text='Go', font=TF, command=fun_rotate, bg=btn, activebackground=btn_active)
+    var.pack(side=tk.LEFT)
+
+    # Matrix
+    matrix_vars = [[tk.DoubleVar(root, latt._u[m, n]) for n in range(3)] for m in range(3)]
+    ln = tk.Frame(right, relief=tk.RIDGE)
+    ln.pack(side=tk.TOP, fill=tk.Y, expand=tk.YES, pady=4)
+    for m in range(3):
+        mat_ln = tk.Frame(ln)
+        mat_ln.pack(side=tk.TOP, fill=tk.X)
+        for n in range(3):
+            var = tk.Entry(mat_ln, textvariable=matrix_vars[m][n], font=TF, width=3, bg=ety, fg=ety_txt)
+            var.pack(side=tk.LEFT)
+
+    def fun_gen_u():
+        nstr = '\n'.join([' '.join(['%6.4f' % matrix_vars[m][n].get() for n in range(3)]) for m in range(3)])
+        utext.delete('1.0', tk.END)
+        utext.insert(tk.END, nstr)
+
+    def fun_load_u():
+        s = utext.get('1.0', tk.END)
+        uary = fg.str2array(s).reshape(3, 3)
+        for m in range(3):
+            for n in range(3):
+                matrix_vars[m][n].set(uary[m, n])
+
+    def fun_gen_l():
+        nstr = '\n'.join([' '.join(['%6.4f' % matrix_vars[m][n].get() for n in range(3)]) for m in range(3)])
+        ltext.delete('1.0', tk.END)
+        ltext.insert(tk.END, nstr)
+
+    def fun_load_l():
+        s = ltext.get('1.0', tk.END)
+        lary = fg.str2array(s).reshape(3, 3)
+        for m in range(3):
+            for n in range(3):
+                matrix_vars[m][n].set(lary[m, n])
+
+    left = tk.Frame(root)
+    left.pack(side=tk.LEFT, fill=tk.Y, expand=tk.YES)
+
+    ln = tk.Frame(left)
     ln.pack(side=tk.TOP, fill=tk.X)
     var = tk.Label(ln, text='U:', width=10, font=SF)
     var.pack(side=tk.LEFT)
     utext = tk.Text(ln, width=20, height=3, font=HF, wrap=tk.NONE, background=ety)
     utext.pack(side=tk.LEFT, fill=tk.BOTH, expand=tk.YES)
     utext.insert(tk.END, ustr)
+    var = tk.Button(ln, text=u'\u25B6', font=TF, command=fun_load_u, bg=btn,
+                    activebackground=btn_active)
+    var.pack(side=tk.LEFT, fill=tk.Y, expand=tk.YES)
+    var = tk.Button(ln, text=u'\u25C0', font=TF, command=fun_gen_u, bg=btn,
+                    activebackground=btn_active)
+    var.pack(side=tk.LEFT, fill=tk.Y, expand=tk.YES)
 
-    ln = tk.Frame(root)
+    ln = tk.Frame(left)
     ln.pack(side=tk.TOP, fill=tk.X)
     var = tk.Label(ln, text='LabFrame:', width=10, font=SF)
     var.pack(side=tk.LEFT)
     ltext = tk.Text(ln, width=20, height=3, font=HF, wrap=tk.NONE, background=ety)
     ltext.pack(side=tk.LEFT, fill=tk.BOTH, expand=tk.YES)
     ltext.insert(tk.END, lstr)
+    var = tk.Button(ln, text=u'\u25B6', font=TF, command=fun_load_l, bg=btn,
+                    activebackground=btn_active)
+    var.pack(side=tk.LEFT, fill=tk.Y, expand=tk.YES)
+    var = tk.Button(ln, text=u'\u25C0', font=TF, command=fun_gen_l, bg=btn,
+                    activebackground=btn_active)
+    var.pack(side=tk.LEFT, fill=tk.Y, expand=tk.YES)
 
     def fun_update(event=None):
         s = utext.get('1.0', tk.END)
         uary = fg.str2array(s).reshape(3, 3)
         s = ltext.get('1.0', tk.END)
         lary = fg.str2array(s).reshape(3, 3)
         latt.set_orientation(uary, lary)
         det.set_labframe(lary)
         callback()
         root.destroy()
 
-    ln = tk.Frame(root)
+    ln = tk.Frame(left)
     ln.pack(side=tk.TOP, fill=tk.X)
     var = tk.Button(ln, text='Update', font=TF, command=fun_update, bg=btn,
                     activebackground=btn_active)
     var.pack(pady=2)
 
 
 def tk_help():
@@ -1276,14 +1429,15 @@
     REFLIST['hkl_str'] = latt.hkl_str[idx][good]
     REFLIST['qxqyqz'] = latt.rotated_qxqyqz[idx, :][good, :]
     REFLIST['fwhm'] = latt.fwhm[idx][good]
     REFLIST['intensity'] = latt.intensity[idx][good]
     REFLIST['scaled'] = scaled_inten[good]
     REFLIST['detx'] = det_x * 1000.  # mm
     REFLIST['dety'] = det_y * 1000.  # mm
+    REFLIST['color'] = [next(col_cycle) for n in range(len(det_x))]
     return xx, yy, mesh
 
 
 def update_3d(array, line_obj):
     """Update 3D line object"""
     line_obj.set_xdata(array[:, 0])
     line_obj.set_ydata(array[:, 1])
@@ -1291,18 +1445,16 @@
 
 
 class DiffractometerGui:
     """
     View and edit the symmetry operations
     """
 
-    _figure_dpi = FIGURE_DPI
-    _figure_3d_size = [8, 4]
-    _figure_det_size = [7, 4]
-    _minimum_gaussian_intensity = 0.01
+    _figure_3d_size = FIGURE_3D_SIZE
+    _figure_det_size = FIGURE_DET_SIZE
 
     def __init__(self, xtl: Crystal):
         """"Initialise"""
         self.xtl = xtl
         self.scatter = self.xtl.Scatter
 
         # Create Tk inter instance
@@ -1336,39 +1488,43 @@
                 'Docs': tk_help,
                 'About': popup_about,
             }
         }
         topmenu(self.root, menu)
 
         # XXXXXXX GUI ELEMENTS XXXXXXX
+        grid = tk.Frame(self.root)
+        grid.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
+        grid.columnconfigure((0, 1), weight=1)
+        grid.rowconfigure((0, 1), weight=1)
+        border = {}  # {'highlightbackground': "black", 'highlightthickness': 1}
+
         # ***--- TOP ---***
         # --- Reciprocal Space Plot ---
-        #line = tk.Frame(self.root)
-        #line.grid(row=1, column=1, sticky=tk.EW, columnspan=2, rowspan=2)
-        # line.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
-        top_left = tk.LabelFrame(self.root, text='Diffractometer')
-        #sec.pack(side=tk.LEFT, expand=tk.YES, padx=4, pady=4)
-        top_left.grid(row=1, column=1, sticky=tk.N+tk.E+tk.S+tk.W)
+        top_left = tk.LabelFrame(grid, text='Diffractometer', **border)
+        top_left.grid(row=0, column=0, sticky='nsew')
         frm = tk.Frame(top_left)
         frm.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
 
-        self.fig1 = Figure(figsize=self._figure_3d_size, dpi=self._figure_dpi)
+        self.fig1 = Figure(figsize=self._figure_3d_size, dpi=OPTIONS['fig_dpi'])
         self.fig1.patch.set_facecolor('w')
 
         canvas = FigureCanvasTkAgg(self.fig1, frm)
         canvas.get_tk_widget().configure(bg='black')
         canvas.draw()  # this must go above 3d axes or the mouse movement doesn't work
 
         self.ax3d = self.fig1.add_subplot(111, projection='3d')
         self.ax3d_reciprocal_lattice, = self.ax3d.plot([], [], [], 'bo', ms=6, alpha=0.3, label='Lattice')
         self.ax3d_lattice_detector, = self.ax3d.plot([], [], [], 'bo', ms=8, label='Reflections')
         self.ax3d_beam_lines, = self.ax3d.plot([], [], [], 'k-', lw=3, label='Beam')
         self.ax3d_wavevector, = self.ax3d.plot([], [], [], 'r-', lw=3, label='Q')
         self.ax3d_detector, = self.ax3d.plot([], [], [], 'k-', lw=2, label='Beam')
         self.ax3d_qdetector, = self.ax3d.plot([], [], [], 'r-', lw=2, label='Beam')
+        self.ax3d_basis_arrows = []
+        self.ax3d_ref_arrows = []
         self.ax3d.set_xlabel(u'Qx [\u212B\u207B\u00B9]')
         self.ax3d.set_ylabel(u'Qy [\u212B\u207B\u00B9]')
         self.ax3d.set_zlabel(u'Qz [\u212B\u207B\u00B9]')
         self.ax3d.set_xlim([-1, 1])
         self.ax3d.set_ylim([-1, 1])
         self.ax3d.set_zlim([-1, 1])
         canvas.get_tk_widget().pack(fill=tk.BOTH, expand=tk.YES)
@@ -1377,21 +1533,21 @@
         # frm = tk.Frame(sec)
         # frm.pack(expand=tk.YES)
         # self.toolbar1 = NavigationToolbar2TkAgg(canvas, frm)
         # self.toolbar1.update()
         # self.toolbar1.pack(fill=tk.X, expand=tk.YES)
 
         # --- Detector Plot ---
-        top_right = tk.LabelFrame(self.root, text='Detector')
+        top_right = tk.LabelFrame(grid, text='Detector', **border)
         # sec.pack(side=tk.LEFT, expand=tk.YES, padx=4, pady=4)
-        top_right.grid(row=1, column=2, sticky=tk.N+tk.E+tk.S+tk.W)
+        top_right.grid(row=0, column=1, sticky='nsew')
         frm = tk.Frame(top_right)
         frm.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
 
-        self.fig2 = Figure(figsize=self._figure_det_size, dpi=self._figure_dpi)
+        self.fig2 = Figure(figsize=self._figure_det_size, dpi=OPTIONS['fig_dpi'])
         self.fig2.patch.set_facecolor('w')
         self.axd = self.fig2.add_subplot(111)
         self.axd_image = self.axd.pcolormesh(np.zeros([10, 10]), shading='auto')
         self.axd_center, = self.axd.plot([0], [0], 'w+', ms=6, label='Centre')
         self.axd_lattice, = self.axd.plot([], [], 'r+', ms=6, label='Nearby reflections')
         self.axd_allowed, = self.axd.plot([], [], 'ko', ms=6, label='Reflections')
         self.axd_ref_str = []
@@ -1410,20 +1566,20 @@
         frm.pack(expand=tk.YES)
         self.toolbar2 = NavigationToolbar2TkAgg(canvas, frm)
         self.toolbar2.update()
         self.toolbar2.pack(fill=tk.X, expand=tk.YES)
 
         # ***--- BOTTOM ---***
         # --- Diffractometer axes ---
-        bottom_left = tk.Frame(self.root)
+        bottom_left = tk.Frame(grid, **border)
         # sec.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
-        bottom_left.grid(row=2, column=1, sticky=tk.N+tk.E+tk.S+tk.W)
+        bottom_left.grid(row=1, column=0, sticky='nsew')
 
         sec = tk.LabelFrame(bottom_left, text='Angles (Deg)')
-        sec.pack(side=tk.TOP, fill=tk.X, expand=tk.YES, padx=4, pady=4)
+        sec.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES, padx=4, pady=4)
 
         # Default scattering angle
         tth = self.xtl.Cell.tth([0, 0, 2], 8)[0]
 
         self.phi = tk_angle_element('Phi', sec, self.update, MSG_PHI, (-180, 180), 0)
         self.chi = tk_angle_element('Chi', sec, self.update, MSG_CHI, (-90, 100), 0)
         self.eta = tk_angle_element('Eta', sec, self.update, MSG_ETA, (-180, 180), 0)
@@ -1436,28 +1592,34 @@
             'Eta': self.eta,
             'Mu': self.mu,
             'Delta': self.delta,
             'Gamma': self.gamma
         }
 
         # --- Beam ---
-        bottom_right = tk.Frame(self.root)
+        bottom_right = tk.Frame(grid, **border)
         # sec.pack(side=tk.LEFT, expand=tk.YES, padx=4, pady=4)
-        bottom_right.grid(row=2, column=2, sticky=tk.N+tk.E+tk.S+tk.W)
+        bottom_right.grid(row=1, column=1, sticky='nsew')
         self.latt = tk_beam(bottom_right, self.xtl, self.update)
 
         # --- Detector ---
         self.det = tk_detector(bottom_right, self.update)
 
         # --- HKL ---
         tk_hkl(bottom_left, self.latt, self.gamma, self.mu, self.update)
 
         # --- Scan ---
         tk_scan(bottom_left, angle_dict, self.latt, self.det)
 
+        # Configure expansion of Tk frame
+        self.root.columnconfigure(0, weight=1)
+        self.root.columnconfigure(1, weight=1)
+        self.root.rowconfigure(0, weight=1)
+        self.root.rowconfigure(1, weight=1)
+
         self.latt.generate_refs()
         self.det.generate_detector()
 
     ###################################################################################
     ################################# MENU ############################################
     ###################################################################################
 
@@ -1493,28 +1655,59 @@
             gamma=self.gamma.get()
         )
 
         # Generate reflections on detector (update REFLIST)
         xx, yy, mesh = generate_reflections(
             latt=self.latt,
             det=self.det,
-            minimum_gaussian_intensity=self._minimum_gaussian_intensity
+            minimum_gaussian_intensity=OPTIONS['min_intensity']
         )
 
         # --- Update 3D Plot ---
         if OPTIONS['3d_lattice']:
             update_3d(self.latt.rotated_qxqyqz, self.ax3d_reciprocal_lattice)
         else:
             update_3d(np.zeros([1, 3]), self.ax3d_reciprocal_lattice)
+
+        [artist.remove() for artist in self.ax3d_basis_arrows]
+        if OPTIONS['3d_basis']:
+            astar, bstar, cstar = self.latt.vectors
+            self.ax3d_basis_arrows = [
+                fp.Arrow3D([0, astar[0]], [0, astar[1]], [0, astar[2]], lw=3, arrowstyle="-|>", color="r"),
+                fp.Arrow3D([0, bstar[0]], [0, bstar[1]], [0, bstar[2]], lw=3, arrowstyle="-|>", color="b"),
+                fp.Arrow3D([0, cstar[0]], [0, cstar[1]], [0, cstar[2]], lw=3, arrowstyle="-|>", color="g"),
+            ]
+            [self.ax3d.add_artist(artist) for artist in self.ax3d_basis_arrows]
+        else:
+            self.ax3d_basis_arrows = []
+
         update_3d(REFLIST['qxqyqz'], self.ax3d_lattice_detector)
+        [artist.remove() for artist in self.ax3d_ref_arrows]
+        if OPTIONS['3d_ref_arrows']:
+            ki = self.det.ki(self.latt.wavelength_a)
+            self.ax3d_ref_arrows = [
+                fp.Arrow3D([0, q[0] + ki[0]], [0, q[1] + ki[1]], [0, q[2] + ki[2]], lw=1, arrowstyle="-|>", color=c)
+                for q, c in zip(REFLIST['qxqyqz'], REFLIST['color'])  # kf arrows
+            ] + [
+                fp.Arrow3D([0, q[0]], [0, q[1]], [0, q[2]], lw=1, arrowstyle="-|>", color=c)
+                for q, c in zip(REFLIST['qxqyqz'], REFLIST['color'])  # q arrows
+            ]
+            [self.ax3d.add_artist(artist) for artist in self.ax3d_ref_arrows]
+        else:
+            self.ax3d_ref_arrows = []
         # update_3d(self.det.corners(), self.ax3d_detector)
         update_3d(self.det.q_shape(self.latt.wavelength_a), self.ax3d_qdetector)
-        kikf, qq = self.det.kfkiq(self.latt.wavelength_a)
-        update_3d(kikf, self.ax3d_beam_lines)
-        update_3d(qq, self.ax3d_wavevector)
+        if OPTIONS['3d_detector_corners']:
+            kikf, qq = self.det.kfkiq_corners(self.latt.wavelength_a)
+            update_3d(kikf, self.ax3d_beam_lines)
+            update_3d(qq, self.ax3d_wavevector)
+        else:
+            kikf, qq = self.det.kfkiq(self.latt.wavelength_a)
+            update_3d(kikf, self.ax3d_beam_lines)
+            update_3d(qq, self.ax3d_wavevector)
 
         self.ax3d.set_xlim([-OPTIONS['maxq'], OPTIONS['maxq']])
         self.ax3d.set_ylim([-OPTIONS['maxq'], OPTIONS['maxq']])
         self.ax3d.set_zlim([-OPTIONS['maxq'], OPTIONS['maxq']])
 
         self.fig1.set_dpi(OPTIONS['fig_dpi'])
         # self.toolbar2.update()
@@ -1561,16 +1754,16 @@
             wavelength_a=fc.energy2wave(8),
             max_q=4,
             resolution=0.0005,
             peakwidth_deg=0.1
         )
         self.det.update_widgets(
             distance=565,
-            width=34,
-            height=84,
+            width=487 * 0.172 * np.cos(np.deg2rad(35)),
+            height=195 * 0.172,
             pixel_size=0.172,
         )
         self.update()
 
     def fun_wish(self):
         """"Add Wish parameters"""
         self.latt.update_widgets(
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/fdmnes.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/fdmnes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 """
 FDMNES tkinter GUI windows
 """
 
-import sys, os
-import matplotlib.pyplot as plt # Plotting
-if sys.version_info[0] < 3:
-    import Tkinter as tk
-    import tkFileDialog as filedialog
-else:
-    import tkinter as tk
-    from tkinter import filedialog
-from ..classes_fdmnes import Fdmnes, FdmnesAnalysis, find_fdmnes
+import os
+import matplotlib.pyplot as plt  # Plotting
+from ..classes_fdmnes import Fdmnes, FdmnesAnalysis, find_fdmnes, fdmnes_checker
+from .basic_widgets import tk, filedialog, messagebox
+from .basic_widgets import StringViewer, text_search
+from .basic_widgets import popup_help, popup_about, topmenu, menu_github, menu_docs
 from .basic_widgets import (TF, BF, SF, LF, HF, TTF, TTFG, TTBG,
                             bkg, ety, btn, opt, btn2,
                             btn_active, opt_active, txtcol,
                             btn_txt, ety_txt, opt_txt)
 
 
+def menu_help():
+    """Display help"""
+    StringViewer(Fdmnes.__doc__, title='Dans_Diffraction diffractometer', width=121)
+
+
+def menu_fdmnes():
+    """Open GitHub page"""
+    import webbrowser
+    webbrowser.open_new_tab("https://fdmnes.neel.cnrs.fr/")
+
+
 class RunFDMNESgui:
     """
     Create FDMNES indata files and run them
     """
 
     def __init__(self, xtl):
         """Initialise"""
@@ -35,54 +43,84 @@
             background=bkg,
             foreground=txtcol,
             activeBackground=opt_active,
             activeForeground=txtcol)
         default_width = 60
         default_height = 30
 
+        # ---Menu---
+        menu = {
+            'File': {
+                'New Window': self.menu_new,
+                'Analyse Output': self.menu_fdmnes_ana,
+                'Exit': self.on_closing,
+            },
+            'Help': {
+                'Help': menu_help,
+                'FDMNES Homepage': menu_fdmnes,
+                'Select FDMNES executable': self.fun_loadfdmnespath,
+                'About': popup_about,
+            }
+        }
+        topmenu(self.root, menu)
+
         frame = tk.Frame(self.root)
         frame.pack(side=tk.LEFT, anchor=tk.N, fill=tk.BOTH, expand=tk.YES)
 
         # Available x-ray edges
         self.xr_edges, self.xr_energies = self.xtl.Properties.xray_edges()
+        absorber = '%s K' % self.xtl.Properties.resonant_element()
         # Polarisations
         poltypes = [u'\u03c3-\u03c3', u'\u03c3-\u03c0', u'\u03c0-\u03c3', u'\u03c0-\u03c0']
 
         # Variables
         if hasattr(xtl, 'P'):
             # Superstructure with parent
             pass
         else:
             # Not superstructure
             pass
+        self.fdmnes_path = tk.StringVar(frame, self.fdm.exe_path)
         self.calculation_name = tk.StringVar(frame, self.fdm.output_name)
         self.calculation_path = tk.StringVar(frame, self.fdm.generate_input_path())
         self.calc_comment = tk.StringVar(frame, self.fdm.comment)
         self.calc_range = tk.StringVar(frame, self.fdm.range)
         self.calc_radius = tk.DoubleVar(frame, self.fdm.radius)
-        self.calc_edge = tk.StringVar(frame, self.xr_edges[0])
+        self.calc_edge = tk.StringVar(frame, absorber)
         self.calc_green = tk.BooleanVar(frame, self.fdm.green)
         self.calc_scf = tk.BooleanVar(frame, self.fdm.scf)
         self.calc_quad = tk.BooleanVar(frame, self.fdm.quadrupole)
+        self.calc_mag = tk.BooleanVar(frame, self.fdm.magnetism)
+        self.calc_spo = tk.BooleanVar(frame, self.fdm.spinorbit)
+        self.calc_ss = tk.BooleanVar(frame, True)
+        self.calc_sp = tk.BooleanVar(frame, True)
         self.calc_aziref = tk.StringVar(frame, str(self.fdm.azi_ref).strip('[]'))
         self.calc_reflist = tk.StringVar(frame, str(self.fdm.hkl_reflections))
-        self.calc_addref = tk.StringVar(frame, '1, 0, 0')
-        self.calc_addpol = tk.StringVar(frame,  poltypes[1])
+        # self.calc_addref = tk.StringVar(frame, '1, 0, 0')
+        # self.calc_addpol = tk.StringVar(frame,  poltypes[1])
 
         # ---Line 0---
         line = tk.Frame(frame, bg=TTBG)
         line.pack(expand=tk.YES, fill=tk.X)
         var = tk.Label(line, text='FDMNES Code, by Y. Joly and O. Bunau', font=TTF, fg=TTFG, bg=TTBG)
         var.pack(fill=tk.X, expand=tk.YES)
 
         # ---Line 0---
         line = tk.Frame(frame)
         line.pack(expand=tk.YES, fill=tk.X)
-        var = tk.Label(line, text='FDMNES Path: %s' % self.fdm.exe_path, font=SF)
-        var.pack(side=tk.LEFT, fill=tk.X, expand=tk.YES)
+        var = tk.Label(line, text='FDMNES Path:', font=SF)
+        var.pack(side=tk.LEFT)
+        var = tk.Entry(line, textvariable=self.fdmnes_path, font=HF, bg=ety, fg=ety_txt)
+        var.pack(side=tk.LEFT, expand=tk.YES, fill=tk.X)
+        var = tk.Button(line, text='Select', font=BF, bg=btn, activebackground=btn_active,
+                        command=self.fun_loadfdmnespath)
+        var.pack(side=tk.LEFT, padx=5)
+        var = tk.Button(line, text='Search', font=BF, bg=btn, activebackground=btn_active,
+                        command=self.fun_findfdmnespath)
+        var.pack(side=tk.LEFT, padx=5)
 
         # ---Line 1---
         line = tk.Frame(frame)
         line.pack(expand=tk.YES, fill=tk.X)
         var = tk.Label(line, text='Path:', font=SF)
         var.pack(side=tk.LEFT)
         var = tk.Entry(line, textvariable=self.calculation_path, font=HF, bg=ety, fg=ety_txt)
@@ -151,50 +189,50 @@
 
         # ---Line B5---
         bline = tk.Frame(box)
         bline.pack(side=tk.TOP, fill=tk.X, pady=5)
         var = tk.Checkbutton(bline, text='Quadrupole', variable=self.calc_quad, font=SF)
         var.pack(side=tk.LEFT, padx=6)
 
+        # ---Line B5---
+        bline = tk.Frame(box)
+        bline.pack(side=tk.TOP, fill=tk.X, pady=5)
+        var = tk.Checkbutton(bline, text='Magnetic', variable=self.calc_mag, font=SF, command=self.fun_mag)
+        var.pack(side=tk.LEFT, padx=6)
+        var = tk.Checkbutton(bline, text='Spin-Orbit', variable=self.calc_spo, font=SF, command=self.fun_mag)
+        var.pack(side=tk.LEFT, padx=6)
+
         # ---Line B6---
         bline = tk.Frame(box)
         bline.pack(side=tk.TOP, fill=tk.X, pady=5)
         var = tk.Label(bline, text='Azimuthal Reference:', font=SF)
         var.pack(side=tk.LEFT)
         var = tk.Entry(bline, textvariable=self.calc_aziref, font=SF, width=6, bg=ety, fg=ety_txt)
         var.pack(side=tk.LEFT, expand=tk.YES, padx=6)
 
         # ---Line B7---
         bline = tk.Frame(box)
         bline.pack(side=tk.TOP, fill=tk.X, pady=5)
-        var = tk.Label(bline, text='h,k,l:', font=SF)
-        var.pack(side=tk.LEFT)
-        var = tk.Entry(bline, textvariable=self.calc_addref, font=SF, width=6, bg=ety, fg=ety_txt)
-        var.pack(side=tk.LEFT, expand=tk.YES, padx=6)
-        """
-        var = tk.OptionMenu(bline, self.calc_addpol, *poltypes)
-        var.config(font=SF, width=5, bg=opt, activebackground=opt_active)
-        var["menu"].config(bg=opt, bd=0, activebackground=opt_active)
-        var.pack(side=tk.LEFT)
-        """
-        var = tk.Button(bline, text='Add Ref', font=BF, bg=btn, activebackground=btn_active,
-                        command=self.fun_addref)
-        var.pack(side=tk.LEFT)
-
-        # ---Line B8---
-        bline = tk.Frame(box)
-        bline.pack(side=tk.TOP, fill=tk.X, pady=5)
         var = tk.Label(bline, text='Reflections:', font=SF)
         var.pack(side=tk.LEFT)
         var = tk.Label(bline, textvariable=self.calc_reflist, font=SF)
         var.pack(side=tk.LEFT)
-        var = tk.Button(bline, text='Clear', font=BF, bg=btn, activebackground=btn_active,
-                        command=self.fun_clearref)
+        iline = tk.Frame(bline)
+        iline.pack(side=tk.LEFT)
+        var = tk.Checkbutton(iline, text=u'\u03c3-\u03c3', variable=self.calc_ss, font=SF)
+        var.pack(side=tk.TOP, padx=3)
+        var = tk.Checkbutton(iline, text=u'\u03c3-\u03c0', variable=self.calc_sp, font=SF)
+        var.pack(side=tk.TOP, padx=3)
+        var = tk.Button(bline, text='Add Refs', font=BF, bg=btn, activebackground=btn_active, command=self.fun_addref)
         var.pack(side=tk.LEFT)
 
+        # ---Line B8---
+        # bline = tk.Frame(box)
+        # bline.pack(side=tk.TOP, fill=tk.X, pady=5)
+
         # ---Line  B9---
         bline = tk.Frame(box)
         bline.pack(fill=tk.X)
         var = tk.Button(bline, text='Update input text', font=BF, bg=btn, activebackground=btn_active,
                         command=self.fun_update)
         var.pack(side=tk.RIGHT)
 
@@ -230,14 +268,20 @@
         self.text.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
         self.gentxt()
 
         self.text.config(xscrollcommand=scanx.set, yscrollcommand=scany.set)
         scanx.config(command=self.text.xview)
         scany.config(command=self.text.yview)
 
+    def menu_new(self):
+        RunFDMNESgui()
+
+    def menu_fdmnes_ana(self):
+        AnaFDMNESgui()
+
     def update(self):
         """Updates the internal fdm object"""
 
         filepath, filename = os.path.split(self.calculation_path.get())
         self.fdm.output_path = filepath
         self.fdm.input_name = filename
         self.fdm.output_name = self.calculation_name.get()
@@ -245,45 +289,87 @@
         self.fdm.range = self.calc_range.get()
         self.fdm.radius = self.calc_radius.get()
         absedge = self.calc_edge.get()
         self.fdm.absorber, self.fdm.edge = absedge.split()
         self.fdm.green = self.calc_green.get()
         self.fdm.scf = self.calc_scf.get()
         self.fdm.quadrupole = self.calc_quad.get()
+        self.fdm.magnetism = self.calc_mag.get()
+        self.fdm.spinorbit = self.calc_spo.get()
         self.fdm.azi_ref = [float(n) for n in self.calc_aziref.get().replace(',', ' ').split()]
 
     def gentxt(self):
         """Generate input file text"""
         parstr = self.fdm.generate_parameters_string()
         self.text.delete('1.0', tk.END)
         self.text.insert(tk.END, parstr)
 
-    def write_reflections(self):
-        """ Write reflections string"""
-        self.calc_reflist.set('%s'%self.fdm.hkl_reflections)
+    def fun_loadfdmnespath(self):
+        """Select fdmnes executable"""
+        filename = filedialog.askopenfilename(
+            parent=self.root,
+            title='Select FDMNES Executable',
+            filetypes=[('EXE File', '*.exe'), ('All Files', '*.*')],
+            initialfile='fdmnes_win64.exe',
+        )
+        if filename:
+            self.fdm.setup(exe_path=filename)
+            self.fdmnes_path.set(filename)
+            self.calculation_path.set(self.fdm.generate_input_path())
+
+    def fun_findfdmnespath(self):
+        """Find fdmnes executable"""
+        filename = find_fdmnes()
+        self.fdm.setup(exe_path=filename)
+        self.fdmnes_path.set(filename)
+        self.calculation_path.set(self.fdm.generate_input_path())
 
     def fun_loadpath(self, event=None):
         """Select folder"""
         filepath, filename = os.path.split(self.calculation_path.get())
-        filepath = filedialog.askdirectory(initialdir=filepath)
-        self.fdm.input_name = filename
-        self.fdm.output_path = filepath
-        self.calculation_path.set(self.fdm.generate_input_path())
+        filepath = filedialog.askdirectory(parent=self.root, initialdir=filepath)
+        if filepath:
+            self.fdm.input_name = filename
+            self.fdm.output_path = filepath
+            self.calculation_path.set(self.fdm.generate_input_path())
+
+    def fun_mag(self, event=None):
+        """Toggle magnetic / spin-orbit"""
+        magnetic = self.calc_mag.get()
+        spinorbit = self.calc_spo.get()
+        if spinorbit:
+            self.calc_mag.set(False)
+        if magnetic:
+            self.calc_spo.set(False)
 
     def fun_addref(self, event=None):
         """Add reflection to list"""
-        newhkl = [int(n) for n in self.calc_addref.get().replace(',', ' ').split()]
-        newpol = self.calc_addpol.get()
-        self.fdm.hkl_reflections += [newhkl]
-        self.write_reflections()
-
-    def fun_clearref(self, event=None):
-        """Clear reflection list"""
-        self.fdm.hkl_reflections = []
-        self.write_reflections()
+        from ..functions_crystallography import energy2wave
+        from .scattering import ReflectionSelectionBox
+
+        edge = self.calc_edge.get()
+        idx = self.xr_edges.index(edge)
+        energy_kev = self.xr_energies[idx]
+        wavelength_a = energy2wave(energy_kev)
+
+        refs = ReflectionSelectionBox(
+            xtl=self.xtl,
+            parent=self.root,
+            title='Select Resonant Reflections',
+            radiation='X-Ray',
+            wavelength_a=wavelength_a,
+        ).show()
+        if len(refs['hkl']) == 0:
+            return
+
+        ss = self.calc_ss.get()
+        sp = self.calc_sp.get()
+
+        self.fdm.hkl_reflections = refs['hkl']
+        self.calc_reflist.set('%d' % len(refs['hkl']))
 
     def fun_update(self, event=None):
         """Update values and generate text"""
         self.update()
         self.gentxt()
 
     def fun_writefiles(self, event=None):
@@ -307,14 +393,18 @@
         #self.fdm.info()
 
     def fun_analyse(self, event=None):
         """Start Analysis GUI"""
         self.update()
         AnaFDMNESgui(self.fdm.output_path, self.fdm.output_name)
 
+    def on_closing(self):
+        """End mainloop on close window"""
+        self.root.destroy()
+
 
 class AnaFDMNESgui:
     """
     Read files from a completed FDMNES calculation folder
     """
 
     def __init__(self, output_path=None, output_name='out'):
@@ -464,18 +554,20 @@
         scany.config(command=self.text.yview)
 
         # Set cursor
         self.text.mark_set(tk.INSERT, "1.0")
 
     def fun_loadpath(self, event=None):
         """Button Select - Open new folder"""
-        ini_dir = find_fdmnes()
-        title = 'Select FDMNES output file, e.g. name_bav.txt'
-        filetypes = [('FDMNES output file', '.txt'), ('All files', '.*')]
-        filename = filedialog.askopenfilename(initialdir=ini_dir, title=title, filetypes=filetypes)
+        filename = filedialog.askopenfilename(
+            parent=self.root,
+            initialdir=find_fdmnes() if fdmnes_checker() else os.path.expanduser('~'),
+            title='Select FDMNES output file, e.g. name_bav.txt',
+            filetypes=[('FDMNES output file', '.txt'), ('All files', '.*')]
+        )
         if filename:
             filepath, filename = os.path.split(filename)
             filename = filename.replace('_', '.')
             calc_name = filename.split('.')[0]
             self.root.destroy()
             AnaFDMNESgui(filepath, calc_name)
         else:
@@ -484,16 +576,23 @@
     def fun_xanes(self, event=None):
         """Button XANES"""
         self.fdm.xanes.plot()
         plt.show()
 
     def fun_dos(self, event=None):
         """Button DOS"""
-        self.fdm.density.plot()
-        plt.show()
+        if self.fdm.density is not None:
+            self.fdm.density.plot()
+            plt.show()
+        else:
+            messagebox.showinfo(
+                parent=self.root,
+                title='FDMNES DOS',
+                message="Density of States file ('%s_sd0.txt') not available." % self.fdm.output_name
+            )
 
     def fun_ref3d(self, event=None):
         """Button Plot all Azim/energy"""
         refn = self.reflection.get()
         refob = self.fdm.__getattribute__(refn)
         refob.plot3D()
         plt.show()
@@ -503,15 +602,19 @@
         refn = self.reflection.get()
         sphrefname = 'sph_' + refn
         if sphrefname in self.fdm.__dict__.keys():
             refob = self.fdm.__getattribute__(sphrefname)
             refob.plot()
             plt.show()
         else:
-            print('Spherical tensor file not available')
+            messagebox.showinfo(
+                parent=self.root,
+                title='FDMNES',
+                message="Spherical tensor file not available"
+            )
 
     def fun_refenergy(self, event=None):
         """Button Plot Energy"""
         refn = self.reflection.get()
         azim = self.cutangle.get()
         try:
             azim = float(azim)
@@ -532,28 +635,30 @@
         refob = self.fdm.__getattribute__(refn)
         refob.plot_azi(energy)
         plt.show()
 
     def fun_search_next(self, event=None):
         """Button Next"""
         search_text = self.bavsearch.get()
-        if search_text == '': return
+        text_search(self.text, search_text)  # Add tags
+        if not search_text: return
 
         searchpos = self.text.index(tk.INSERT) + "+1c"
 
         res = self.text.search(search_text, searchpos, stopindex=tk.END)
         if res == '': return
         self.text.focus_set()
         self.text.mark_set(tk.INSERT, res)
         self.text.see(tk.INSERT)
 
     def fun_search_prev(self, event=None):
         """Button Prev"""
         search_text = self.bavsearch.get()
-        if search_text == '': return
+        text_search(self.text, search_text)  # Add tags
+        if not search_text: return
 
         searchpos = self.text.index(tk.INSERT) + "-1c"
 
         res = self.text.search(search_text, searchpos, stopindex=None, backwards=True)
         if res == '': return
         self.text.focus_set()
         self.text.mark_set(tk.INSERT, res)
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/multi_crystal.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/multi_crystal.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,21 @@
 GUI for MultiCrystal code
 """
 
 import sys, os
 
 import matplotlib.pyplot as plt
 import numpy as np
-if sys.version_info[0] < 3:
-    import Tkinter as tk
-    import tkFileDialog as filedialog
-    import tkMessageBox as messagebox
-else:
-    import tkinter as tk
-    from tkinter import filedialog
-    #from tkinter import messagebox
 
 from .. import functions_general as fg
 from .. import functions_crystallography as fc
 from ..classes_crystal import Crystal
 from ..classes_structures import Structures
 from ..classes_multicrystal import MultiCrystal
-from .basic_widgets import StringViewer
+from .basic_widgets import StringViewer, tk, filedialog
 from .basic_widgets import (TF, BF, SF, LF, HF, TTF, TTFG, TTBG,
                             bkg, ety, btn, opt, btn2,
                             btn_active, opt_active, txtcol,
                             btn_txt, ety_txt, opt_txt)
 
 
 class MultiCrystalGui:
@@ -53,16 +45,16 @@
 
         # Variatbles
         self.struct_list = tk.StringVar(frame, 'Add Structure')
         self.scale = tk.DoubleVar(frame, 1.0)
         self.energy_kev = tk.DoubleVar(frame, 8.0)
         self.edge = tk.StringVar(frame, 'Edge')
         self.type = tk.StringVar(frame, 'X-Ray')
-        self.twotheta_min = tk.DoubleVar(frame, -180.0)
-        self.twotheta_max = tk.DoubleVar(frame, 180.0)
+        self.twotheta_min = tk.DoubleVar(frame, 5.0)
+        self.twotheta_max = tk.DoubleVar(frame, 60.0)
         self.powder_units = tk.StringVar(frame, 'Two-Theta')
 
         # X-ray edges:
         self.xr_edges = []
         self.xr_energies = []
         for xtl in self.xtls.crystal_list:
             edges, energies = xtl.Properties.xray_edges()
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/multiple_scattering.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/multiple_scattering.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,18 @@
 GUI for MultipleScattering code
 """
 
 import sys, os
 
 import matplotlib.pyplot as plt
 import numpy as np
-if sys.version_info[0] < 3:
-    import Tkinter as tk
-else:
-    import tkinter as tk
 
 from .. import functions_general as fg
 from .. import functions_crystallography as fc
-from .basic_widgets import StringViewer
+from .basic_widgets import tk
 from .basic_widgets import (TF, BF, SF, LF, HF, TTF, TTFG, TTBG,
                             bkg, ety, btn, opt, btn2,
                             btn_active, opt_active, txtcol,
                             btn_txt, ety_txt, opt_txt)
 
 
 class MultipleScatteringGui:
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/periodic_table.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/periodic_table.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/properties.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,15 +676,15 @@
                         activebackground=btn_active)
         var.pack(side=tk.LEFT)
 
     def _atom_str(self, atom):
         s = '%4s [%2s] (%5.2f,%5.2f,%5.2f)'
         return s % (atom.label, atom.type, atom.u, atom.v, atom.w)
 
-    def atom_update(self, event=True):
+    def atom_update(self, event=None):
         idx = self.structure_index.get()
         self.atom_str.set(self.atom_list[idx])
 
     def button_select_atom(self):
         choose = SelectionBox(self.root, self.atom_list, multiselect=False, title='Select atom site').show()
         if choose:
             idx = self.atom_list.index(choose[0])
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/scattering.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/scattering.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,26 @@
 """
 Scattering GUI
 """
 
 import sys, os
+import re
 
-import matplotlib.pyplot as plt # Plotting
+import matplotlib.pyplot as plt
 import numpy as np
-if sys.version_info[0] < 3:
-    import Tkinter as tk
-else:
-    import tkinter as tk
 
 from .. import functions_general as fg
 from .. import functions_crystallography as fc
-from .basic_widgets import StringViewer, topmenu
-from .basic_widgets import (TF, BF, SF, LF, HF,
+from .. import fdmnes_checker
+from .basic_widgets import tk, StringViewer, topmenu, messagebox
+from .basic_widgets import (TF, BF, SF, LF, HF, MF,
                             bkg, ety, btn, opt, btn2,
                             btn_active, opt_active, txtcol,
                             btn_txt, ety_txt, opt_txt)
 
-# Scattering functions
-"""
-
-
-
-
-plot_xray_resonance(self, hkl, energy_kev=None, width=1.0, npoints=200)
-plot_3Dpolarisation(self, hkl, energy_kev=None, polarisation='sp', azim_zero=[1,0,0], psi=0)
-
-
-
-ms_azimuth(self, hkl, energy_kev, azir=[0, 0, 1], pv=[1, 0], numsteps=3, peak_width=0.1,
-                   full=False, pv1=False, pv2=False, sfonly=True, pv1xsf1=False)
-diff6circle_intensity(self, phi=0, chi=0, eta=0, mu=0, delta=0, gamma=0,
-                              energy_kev=None, wavelength=1.0, fwhm=0.5)
-multiple_scattering(self, hkl, azir=[0, 0, 1], pv=[1, 0], energy_range=[7.8, 8.2], numsteps=60,
-                            full=False, pv1=False, pv2=False, sfonly=True, pv1xsf1=False)
-"""
-
 
 class ScatteringGuiOLD:
     """
     Simulate scattering of various forms
     """
 
     def __init__(self, xtl):
@@ -485,18 +464,18 @@
         tth = self.xtl.Cell.tth(hkl, energy)
 
         if unit.lower() in ['tth', 'angle', 'twotheta', 'theta', 'two-theta']:
             self.hkl_result.set('I:%10.0f TTH:%8.2f' % (I, tth))
         elif unit.lower() in ['d', 'dspace', 'd-spacing', 'dspacing']:
             q = fc.calqmag(tth, energy)
             d = fc.q2dspace(q)
-            self.hkl_result.set(u'I:%10.0f   d:%8.2f \u00c5' % (I, d))
+            self.hkl_result.set(u'I:%10.0f   d:%8.2f \u212B' % (I, d))
         else:
             q = fc.calqmag(tth, energy)
-            self.hkl_result.set(u'I:%8.0f   Q:%8.2f \u00c5\u207B\u00B9' % (I, q))
+            self.hkl_result.set(u'I:%8.0f   Q:%8.2f \u212B\u207B\u00B9' % (I, q))
 
     def fun_hklsym(self):
         """Print symmetric reflections"""
         hkl = self.fun_get_hkl()
         out = self.xtl.Scatter.print_symmetric_reflections(hkl)
         StringViewer(out, 'Symmetric Reflections %s' % hkl)
 
@@ -538,15 +517,15 @@
         energy = self.energy_kev.get()
         min_q = fc.calqmag(self.twotheta_min.get(), energy)
         max_q = fc.calqmag(self.twotheta_max.get(), energy)
         pow_avg = self.powderaverage.get()
         pow_wid = self.powder_width.get()
         #if min_q < 0: min_q = 0.0
 
-        self.xtl.Plot.simulate_powder(energy, peak_width=pow_wid, powder_average=pow_avg)
+        self.xtl.Plot.simulate_powder(energy_kev=energy, peak_width=pow_wid, powder_average=pow_avg)
         plt.show()
 
     def fun_hki(self):
         """Plot hki plane"""
         self.fun_get()
         i = self.val_i.get()
         self.xtl.Plot.simulate_hk0(i, peak_width=0.2)
@@ -639,14 +618,16 @@
         self.powderaverage = tk.BooleanVar(frame, True)
         self.powder_width = tk.DoubleVar(frame, 0.01)
         self.hkl_check = tk.StringVar(frame, '0 0 1')
         self.hkl_result = tk.StringVar(frame, 'I:%10.0f TTH:%8.2f' % (0, 0))
         self.close_twotheta = tk.DoubleVar(frame, 2)
         self.close_angle = tk.DoubleVar(frame, 10)
         self.val_i = tk.IntVar(frame, 0)
+        self.cmin = tk.StringVar(frame, '')
+        self.cmax = tk.StringVar(frame, '')
 
         # radiation
         radiations = ['X-Ray', 'Neutron', 'Electron']
         energy_units = ['keV', 'eV', 'meV']
         wavelength_units = [u'\u212B', 'nm']
 
         # X-ray edges:
@@ -881,14 +862,32 @@
         var.pack()
 
         side = tk.Frame(box)
         side.pack(side=tk.LEFT, padx=5, pady=5)
         var = tk.Button(side, text='Arbitary Cut', font=BF, command=self.fun_cut, bg=btn,
                         activebackground=btn_active)
         var.pack()
+        # clim
+        frm = tk.Frame(side, relief=tk.RIDGE)
+        frm.pack(side=tk.TOP, pady=10)
+        line = tk.Frame(frm)
+        line.pack(side=tk.TOP)
+        var = tk.Label(line, text='Clim:', font=SF)
+        var.pack(side=tk.LEFT)
+        var = tk.Entry(line, textvariable=self.cmin, font=TF, width=6, bg=ety, fg=ety_txt)
+        var.pack(side=tk.LEFT)
+        var.bind('<Return>', self.fun_clim)
+        var.bind('<KP_Enter>', self.fun_clim)
+        var = tk.Entry(line, textvariable=self.cmax, font=TF, width=6, bg=ety, fg=ety_txt)
+        var.pack(side=tk.LEFT)
+        var.bind('<Return>', self.fun_clim)
+        var.bind('<KP_Enter>', self.fun_clim)
+        var = tk.Button(line, text='Update', font=TF, command=self.fun_clim, bg=btn,
+                        activebackground=btn_active)
+        var.pack(side=tk.LEFT, pady=2)
 
         # ---X-ray Magnetic scattering---
         box = tk.Frame(right)
         box.pack(side=tk.TOP, fill=tk.BOTH, padx=5, pady=5)
         var = tk.Button(box, text='X-Ray Magnetic Scattering', font=BF, command=self.fun_rxs, bg=btn,
                         activebackground=btn_active)
         var.pack(fill=tk.X)
@@ -1121,18 +1120,18 @@
         tth = self.xtl.Cell.tth(hkl, energy)
 
         if unit.lower() in ['tth', 'angle', 'twotheta', 'theta', 'two-theta']:
             self.hkl_result.set('I:%10.0f TTH:%8.2f' % (I, tth))
         elif unit.lower() in ['d', 'dspace', 'd-spacing', 'dspacing']:
             q = fc.calqmag(tth, energy)
             d = fc.q2dspace(q)
-            self.hkl_result.set(u'I:%10.0f   d:%8.2f \u00c5' % (I, d))
+            self.hkl_result.set(u'I:%10.0f   d:%8.2f \u212B' % (I, d))
         else:
             q = fc.calqmag(tth, energy)
-            self.hkl_result.set(u'I:%8.0f   Q:%8.2f \u00c5\u207B\u00B9' % (I, q))
+            self.hkl_result.set(u'I:%8.0f   Q:%8.2f \u212B\u207B\u00B9' % (I, q))
 
     def fun_hklsym(self):
         """Print symmetric reflections"""
         hkl = self.fun_get_hkl()
         out = self.xtl.Scatter.print_symmetric_reflections(hkl)
         StringViewer(out, 'Symmetric Reflections %s' % hkl)
 
@@ -1167,56 +1166,71 @@
             units = self.powder_units.get()
             string = self.xtl.Scatter.print_all_reflections(min_intensity=-1, max_intensity=None, units=units)
         StringViewer(string, 'Intensities %s' % self.xtl.name)
 
     def fun_powder(self):
         """Plot Powder"""
         self.fun_get()
-        energy = self.get_energy()
-        min_q = fc.calqmag(self.twotheta_min.get(), energy)
-        max_q = fc.calqmag(self.twotheta_max.get(), energy)
+        wavelength_a = self.get_wavelength()
+        energy_kev = fc.wave2energy(wavelength_a)
         pow_avg = self.powderaverage.get()
         pow_wid = self.powder_width.get()
-        #if min_q < 0: min_q = 0.0
 
-        self.xtl.Plot.simulate_powder(energy, peak_width=pow_wid, powder_average=pow_avg)
+        self.xtl.Plot.simulate_powder(energy_kev=energy_kev, peak_width=pow_wid, powder_average=pow_avg)
         plt.show()
 
     def fun_hki(self):
         """Plot hki plane"""
         self.fun_get()
         i = self.val_i.get()
         self.xtl.Plot.simulate_hk0(i, peak_width=0.2)
+        self.fun_clim()
         plt.show()
 
     def fun_hil(self):
         """Plot hil plane"""
         self.fun_get()
         i = self.val_i.get()
         self.xtl.Plot.simulate_h0l(i, peak_width=0.2)
+        self.fun_clim()
         plt.show()
 
     def fun_ikl(self):
         """Plot ikl plane"""
         self.fun_get()
         i = self.val_i.get()
         self.xtl.Plot.simulate_0kl(i, peak_width=0.2)
+        self.fun_clim()
         plt.show()
 
     def fun_hhi(self):
         """Plot hhl plane"""
         self.fun_get()
         i = self.val_i.get()
         self.xtl.Plot.simulate_hhl(i, peak_width=0.2)
+        self.fun_clim()
         plt.show()
 
     def fun_cut(self):
         self.fun_get()
         ArbitaryCutGui(self.xtl)
 
+    def fun_clim(self, event=None):
+        """Update clim"""
+        try:
+            cmin = float(self.cmin.get())
+        except ValueError:
+            cmin = None
+        try:
+            cmax = float(self.cmax.get())
+        except ValueError:
+            cmax = None
+        plt.gca()
+        plt.clim(cmin, cmax)
+
     def fun_rxs(self):
         ResonantXrayGui(self)
 
 
 class ArbitaryCutGui:
     """
     Simulate scattering of various forms
@@ -1249,15 +1263,15 @@
         self.lattice_points = tk.BooleanVar(frame, False)
         self.cmin = tk.StringVar(frame, '')
         self.cmax = tk.StringVar(frame, '')
 
         # --- Title ---
         line = tk.Frame(frame)
         line.pack(side=tk.TOP, fill=tk.X, pady=5)
-        var = tk.Label(line, text='Arbitary HKl Cut', font=LF)
+        var = tk.Label(line, text='Arbitary HKL Cut', font=LF)
         var.pack(side=tk.LEFT)
 
         # --- Entry ---
         frm = tk.Frame(frame)
         frm.pack(side=tk.TOP, fill=tk.BOTH, pady=5)
 
         line = tk.Frame(frm)
@@ -1331,14 +1345,18 @@
 
         line = tk.Frame(frm)
         line.pack(side=tk.TOP)
         var = tk.Button(line, text='Generate\nCut', font=TF, command=self.fun_generate, bg=btn,
                         activebackground=btn_active)
         var.pack(side=tk.LEFT, pady=2)
 
+        var = tk.Button(line, text='Generate\nEnvelope', font=TF, command=self.fun_envelope, bg=btn,
+                        activebackground=btn_active)
+        var.pack(side=tk.LEFT, pady=2)
+
         var = tk.Button(line, text='Generate\n3D Lattice', font=TF, command=self.fun_3dlattice, bg=btn,
                         activebackground=btn_active)
         var.pack(side=tk.LEFT, pady=2)
 
         var = tk.Button(line, text='Show\nCoverage', font=TF, command=self.fun_ewald, bg=btn,
                         activebackground=btn_active)
         var.pack(side=tk.LEFT, pady=2)
@@ -1375,14 +1393,36 @@
                 y_axis=fg.str2array(self.hkl_plane_y.get()),
                 centre=fg.str2array(self.hkl_plane_c.get()),
                 q_max=self.hkl_plane_q.get(),
                 cut_width=self.hkl_plane_width.get()
             )
         plt.show()
 
+    def fun_envelope(self):
+        """Run code"""
+        self.xtl.Plot.simulate_envelope_cut(
+            x_axis=fg.str2array(self.hkl_plane_x.get()),
+            y_axis=fg.str2array(self.hkl_plane_y.get()),
+            centre=fg.str2array(self.hkl_plane_c.get()),
+            q_max=self.hkl_plane_q.get(),
+            background=self.hkl_plane_bkg.get(),
+            pixels=301,
+        )
+        self.fun_clim()
+        if self.lattice_points.get():
+            self.xtl.Plot.axis_reciprocal_lattice_points(
+                axes=None,
+                x_axis=fg.str2array(self.hkl_plane_x.get()),
+                y_axis=fg.str2array(self.hkl_plane_y.get()),
+                centre=fg.str2array(self.hkl_plane_c.get()),
+                q_max=self.hkl_plane_q.get(),
+                cut_width=self.hkl_plane_width.get()
+            )
+        plt.show()
+
     def fun_ewald(self):
         """Button plot ewald coverage"""
         self.xtl.Plot.simulate_ewald_coverage(
             energy_kev=self.xtl.Scatter.get_energy(),
             sample_normal=fg.str2array(self.hkl_plane_y.get()),
             sample_para=fg.str2array(self.hkl_plane_x.get()),
             cut_width=self.hkl_plane_width.get(),
@@ -1567,14 +1607,19 @@
         var = tk.Button(line, text='Simulate\n Azimuth', font=BF, command=self.fun_azimuth, width=7, bg=btn,
                         activebackground=btn_active)
         var.pack(side=tk.RIGHT)
         # Energy Button
         var = tk.Button(line, text='Simulate\n Resonance', font=BF, command=self.fun_dispersion, width=10, bg=btn,
                         activebackground=btn_active)
         var.pack(side=tk.RIGHT)
+        # FDMNES Button
+        if fdmnes_checker():
+            var = tk.Button(line, text='FDMNES', font=BF, command=self.fun_fdmnes_ref, height=2, width=10, bg=btn,
+                            activebackground=btn_active)
+            var.pack(side=tk.RIGHT)
 
     def fun_energy(self, event=None):
         """Set wavelength"""
         energy_kev = self.energy_kev.get()
         self.wavelenth_a.set(round(fc.energy2wave(energy_kev), 4))
 
     def fun_wavelength(self, event=None):
@@ -1618,14 +1663,62 @@
                 hkl,
                 energy_kev=energy_kev,
                 azim_zero=azi, psi=psi,
                 polarisation=pol)
 
         self.magresult.set('I = %9.4g' % maginten)
 
+    def fun_fdmnes_ref(self):
+        """Run FDMNES calculation"""
+        from ..classes_fdmnes import Fdmnes, sim_folder
+        edge = self.edge.get()
+        if edge == 'Edge':
+            messagebox.showinfo(
+                parent=self.root,
+                title='FDMNES Calculation',
+                message='Please choose an absorption edge'
+            )
+            return
+        absorber, edge = edge.split()
+        hkl = fg.str2array(self.hkl_magnetic.get())
+        azi = fg.str2array(self.azim_zero.get())
+        pol = self.polval.get().replace('\u03c3', 's').replace('\u03c0', 'p')
+
+        # Create FDMNES calculation
+        fdm = Fdmnes(self.xtl)
+        fdm.setup(
+            output_path=sim_folder('.Dans_Diffraction'),
+            comment='Scattering GUI calculation',
+            energy_range='-10. 1. -5 0.1 -2. 0.05 5 0.1 10. 0.5 25 1 31.',
+            radius=4.0,
+            edge=edge,
+            absorber=absorber,
+            scf=False,
+            quadrupole=True,
+            azi_ref=azi,
+            hkl_reflections=[hkl]
+        )
+        answer = messagebox.askyesnocancel(
+            parent=self.root,
+            title='FDMNES Calculation',
+            message='Run FDMNES calculation?\nThis will take a few minutes.\nClick No to reload a previous calcualtion'
+        )
+        if answer is None:
+            return
+        elif answer:
+            # Create files and run FDMNES
+            fdm.create_files()
+            fdm.write_fdmfile()
+            fdm.run_fdmnes()
+        # Analyse data
+        ana = fdm.analyse()
+        for ref in ana:
+            ref.plot3D()
+        plt.show()
+
     def fun_hklmag_list(self, event=None):
         """"Magnetic scattering"""
 
         energy_kev = self.energy_kev.get()
         azi = fg.str2array(self.azim_zero.get())
         psi = self.psival.get()
         F0 = self.resF0.get()
@@ -1693,7 +1786,521 @@
         """Simulate energy resonance"""
 
         energy_kev = self.energy_kev.get()
         hkl = fg.str2array(self.hkl_magnetic.get())
         hkl = np.array([hkl, -hkl])
         self.xtl.Plot.plot_xray_resonance(hkl, energy_kev=energy_kev, width=1.0, npoints=200)
         plt.show()
+
+
+class ReflectionSelectionBox:
+    """
+    Displays all data fields and returns a selection
+    Making a selection returns a list of field strings
+
+    out = ReflectionSelectionBox(['field1','field2','field3'], current_selection=['field2'], title='', multiselect=False).show()
+    # Make selection and press "Select" > box disappears
+    out = ['list','of','strings']
+    """
+
+    REF_FMT = '%14s %8.2f  %12.4g'
+
+    def __init__(self, xtl, parent, title='Reflections', multiselect=True,
+                 radiation=None, wavelength_a=None):
+        self.xtl = xtl
+        self.hkl_list = []
+        self.tth_list = []
+        self.sf_list = []
+        self.str_list = []
+        self.current_selection = []
+        self.output = []
+
+        # Create Tk inter instance
+        self.root = tk.Toplevel(parent)
+        self.root.wm_title(title)
+        self.root.minsize(width=100, height=300)
+        self.root.maxsize(width=1200, height=1200)
+        self.root.tk_setPalette(
+            background=bkg,
+            foreground=txtcol,
+            activeBackground=opt_active,
+            activeForeground=txtcol
+        )
+
+        # tk variables
+        radiations = ['X-Ray', 'Neutron', 'Electron']
+        wavelength_types = ['Energy [keV]', 'Energy [eV]', 'Energy [meV]', u'Wavelength [\u212B]', 'Wavelength [nm]']
+        max_types = [u'Max Q [\u212B\u207B\u00B9]', u'Max 2\u03B8 [Deg]', u'min d [\u212B]']
+        self.radiation_type = tk.StringVar(self.root, radiations[0] if radiation is None else radiation)
+        self.check_magnetic = tk.BooleanVar(self.root, False)
+        self.wavelength_type = tk.StringVar(self.root, 'Energy [keV]')
+        self._prev_wavelength_type = tk.StringVar(self.root, 'Energy [keV]')
+        self.wavelength_val = tk.DoubleVar(self.root, 8)
+        self.edge = tk.StringVar(self.root, 'Edge')
+        self.max_gen_type = tk.StringVar(self.root, u'Max Q [\u212B\u207B\u00B9]')
+        self._prev_max_gen_type = tk.StringVar(self.root, u'Max Q [\u212B\u207B\u00B9]')
+        self.max_val = tk.DoubleVar(self.root, 4)
+        self.min_sf = tk.DoubleVar(self.root, 0)
+        self.max_sf = tk.DoubleVar(self.root, np.inf)
+        self.add_hkl = tk.StringVar(self.root, '')
+
+        self.fun_radiation()
+        self.set_wavelength(1.5 if wavelength_a is None else wavelength_a)
+
+        # X-ray edges:
+        self.xr_edges, self.xr_energies = self.xtl.Properties.xray_edges()
+        self.xr_edges.insert(0, 'Cu Ka')
+        self.xr_edges.insert(1, 'Mo Ka')
+        self.xr_energies.insert(0, fg.Cu)
+        self.xr_energies.insert(1, fg.Mo)
+
+        # tk Frames
+        frame = tk.Frame(self.root)
+        frame.pack(side=tk.LEFT, fill=tk.BOTH, expand=tk.YES, anchor=tk.N)
+
+        "---------------------------Scattering------------------------"
+        OPT_WIDTH = 14
+        frm = tk.LabelFrame(frame, text='Radiation', relief=tk.RIDGE)
+        frm.pack(fill=tk.X, padx=4, pady=4)
+
+        # Radiation
+        if radiation is None:
+            ln = tk.Frame(frm)
+            ln.pack(side=tk.TOP, fill=tk.X)
+            var = tk.Label(ln, text='Radiation:', font=SF)
+            var.pack(side=tk.LEFT)
+            var = tk.OptionMenu(ln, self.radiation_type, *radiations, command=self.fun_radiation)
+            var.config(font=SF, width=OPT_WIDTH, bg=opt, activebackground=opt_active)
+            var["menu"].config(bg=opt, bd=0, activebackground=opt_active)
+            var.pack(side=tk.LEFT)
+            var = tk.Checkbutton(ln, text='Magnetic', variable=self.check_magnetic, font=SF)
+            var.pack(side=tk.LEFT, padx=6)
+
+        # Wavelength / Energy
+        ln = tk.Frame(frm)
+        ln.pack(side=tk.TOP, fill=tk.X)
+        if wavelength_a is None:
+            var = tk.OptionMenu(ln, self.wavelength_type, *wavelength_types, command=self.fun_wavelength)
+            var.config(font=SF, width=OPT_WIDTH, bg=opt, activebackground=opt_active)
+            var["menu"].config(bg=opt, bd=0, activebackground=opt_active)
+            var.pack(side=tk.LEFT)
+            var = tk.OptionMenu(ln, self.edge, *self.xr_edges, command=self.fun_edge)
+            var.config(font=SF, width=5, bg=opt, activebackground=opt_active)
+            var["menu"].config(bg=opt, bd=0, activebackground=opt_active)
+            var.pack(side=tk.LEFT)
+            var = tk.Entry(ln, textvariable=self.wavelength_val, font=TF, width=8, bg=ety, fg=ety_txt)
+            var.pack(side=tk.LEFT)
+            var.bind('<Return>', self.fun_wavelength)
+            var.bind('<KP_Enter>', self.fun_wavelength)
+        else:
+            var = tk.Label(ln, textvariable=self.wavelength_type, font=SF)
+            var.pack(side=tk.LEFT)
+            var = tk.Label(ln, textvariable=self.wavelength_val, font=SF)
+            var.pack(side=tk.LEFT)
+
+        # Max Q
+        ln = tk.Frame(frm)
+        ln.pack(side=tk.TOP, fill=tk.X)
+        var = tk.OptionMenu(ln, self.max_gen_type, *max_types, command=self.get_max_q)
+        var.config(font=SF, width=OPT_WIDTH, bg=opt, activebackground=opt_active)
+        var["menu"].config(bg=opt, bd=0, activebackground=opt_active)
+        var.pack(side=tk.LEFT)
+        var = tk.Entry(ln, textvariable=self.max_val, font=TF, width=8, bg=ety, fg=ety_txt)
+        var.pack(side=tk.LEFT)
+        var.bind('<Return>', self.fun_gen_refs)
+        var.bind('<KP_Enter>', self.fun_gen_refs)
+        var = tk.Button(ln, text='?', font=TF, command=self.help_max_q, bg=btn, activebackground=btn_active)
+        var.pack(side=tk.LEFT, pady=2)
+
+        # Intensities
+        ln = tk.Frame(frm)
+        ln.pack(side=tk.TOP, fill=tk.X)
+        var = tk.Label(ln, text=u'Min |SF|\u00B2:', font=SF)
+        var.pack(side=tk.LEFT)
+        var = tk.Entry(ln, textvariable=self.min_sf, font=TF, width=8, bg=ety, fg=ety_txt)
+        var.pack(side=tk.LEFT)
+        var = tk.Label(ln, text=u'    Max |SF|\u00B2:', font=SF)
+        var.pack(side=tk.LEFT)
+        var = tk.Entry(ln, textvariable=self.max_sf, font=TF, width=8, bg=ety, fg=ety_txt)
+        var.pack(side=tk.LEFT)
+
+        # Add hkl
+        ln = tk.Frame(frm)
+        ln.pack(side=tk.TOP, fill=tk.X)
+        var = tk.Label(ln, text=u'hkl', font=SF)
+        var.pack(side=tk.LEFT)
+        var = tk.Entry(ln, textvariable=self.add_hkl, font=TF, width=8, bg=ety, fg=ety_txt)
+        var.pack(side=tk.LEFT)
+        var.bind('<Return>', self.fun_add_hkl)
+        var.bind('<KP_Enter>', self.fun_add_hkl)
+        var = tk.Button(ln, text='Add ref', font=TF, command=self.fun_add_hkl, bg=btn,
+                        activebackground=btn_active)
+        var.pack(side=tk.LEFT, pady=2)
+
+        # Generate Buttons
+        ln = tk.Frame(frm)
+        ln.pack(side=tk.TOP, fill=tk.X)
+        var = tk.Button(ln, text='Gen Sym', font=TF, command=self.fun_gen_sym_refs, bg=btn,
+                        activebackground=btn_active)
+        var.pack(side=tk.LEFT, pady=2)
+        var = tk.Button(ln, text='Rem Sym', font=TF, command=self.fun_rem_sym_refs, bg=btn,
+                        activebackground=btn_active)
+        var.pack(side=tk.LEFT, pady=2)
+        var = tk.Button(ln, text='Gen Refs', font=TF, command=self.fun_gen_refs, bg=btn,
+                        activebackground=btn_active)
+        var.pack(side=tk.RIGHT, pady=2)
+        var = tk.Button(ln, text='Clear', font=TF, command=self.clear_reflections, bg=btn,
+                        activebackground=btn_active)
+        var.pack(side=tk.RIGHT, pady=2)
+
+        "---------------------------ListBox---------------------------"
+        ln = tk.Frame(frame)
+        ln.pack(side=tk.TOP)
+        var = tk.Label(ln, text='hkl    Two-Theta    Intensity', font=SF)
+        var.pack(side=tk.LEFT)
+
+        # Eval box with scroll bar
+        frm = tk.Frame(frame)
+        frm.pack(side=tk.TOP, fill=tk.BOTH, expand=tk.YES)
+
+        sclx = tk.Scrollbar(frm, orient=tk.HORIZONTAL)
+        sclx.pack(side=tk.BOTTOM, fill=tk.BOTH)
+
+        scly = tk.Scrollbar(frm)
+        scly.pack(side=tk.RIGHT, fill=tk.BOTH)
+
+        self.lst_data = tk.Listbox(frm, font=MF, selectmode=tk.SINGLE, width=40, height=20, bg=ety,
+                                   xscrollcommand=sclx.set, yscrollcommand=scly.set)
+        self.lst_data.configure(exportselection=True)
+        if multiselect:
+            self.lst_data.configure(selectmode=tk.EXTENDED)
+        self.lst_data.bind('<<ListboxSelect>>', self.fun_listboxselect)
+        self.lst_data.bind('<Double-Button-1>', self.fun_exitbutton)
+        self.lst_data.pack(side=tk.LEFT, fill=tk.BOTH, expand=tk.YES)
+
+        sclx.config(command=self.lst_data.xview)
+        scly.config(command=self.lst_data.yview)
+
+        # self.txt_data.config(xscrollcommand=scl_datax.set,yscrollcommand=scl_datay.set)
+
+        "----------------------------Search Field-----------------------------"
+        frm = tk.LabelFrame(frame, text='Search', relief=tk.RIDGE)
+        frm.pack(fill=tk.X, expand=tk.YES, padx=2, pady=2)
+
+        self.searchbox = tk.StringVar(self.root, '')
+        var = tk.Entry(frm, textvariable=self.searchbox, font=TF, bg=ety, fg=ety_txt)
+        var.bind('<Key>', self.fun_search)
+        var.pack(fill=tk.X, expand=tk.YES, padx=2, pady=2)
+
+        "----------------------------Exit Button------------------------------"
+        frm_btn = tk.Frame(frame)
+        frm_btn.pack(fill=tk.X, expand=tk.YES)
+
+        self.numberoffields = tk.StringVar(self.root, '%3d Selected Fields' % 0)
+        var = tk.Label(frm_btn, textvariable=self.numberoffields, width=20)
+        var.pack(side=tk.LEFT)
+        btn_exit = tk.Button(frm_btn, text='Select', font=BF, command=self.fun_exitbutton, bg=btn,
+                             activebackground=btn_active)
+        btn_exit.pack(side=tk.RIGHT)
+
+        "-------------------------Start Mainloop------------------------------"
+        self.root.protocol("WM_DELETE_WINDOW", self.f_exit)
+        # self.root.mainloop()
+
+    "------------------------------------------------------------------------"
+    "------------------------Scattering Functions----------------------------"
+    "------------------------------------------------------------------------"
+
+    def get_scattering_type(self):
+        """Get scattering type"""
+        radiation = self.radiation_type.get()
+        magnetic = self.check_magnetic.get()
+        if radiation == 'X-Ray':
+            if magnetic:
+                scattering_type = 'xray magnetic'
+            else:
+                scattering_type = 'xray'
+        elif radiation == 'Neutron':
+            if magnetic:
+                scattering_type = 'neutron magnetic'
+            else:
+                scattering_type = 'neutron'
+        elif radiation == 'Electron':
+            scattering_type = 'electron'
+        else:
+            scattering_type = radiation
+        return scattering_type
+
+    def get_wavelength(self):
+        """Return wavelength in A according to unit"""
+        val = self.wavelength_val.get()
+        rad = self.radiation_type.get()
+        unit = self._prev_wavelength_type.get()
+
+        if unit == 'Energy [keV]':
+            if 'Electron' in rad:
+                wavelength_a = fc.electron_wavelength(val * 1000)
+            elif 'Neutron' in rad:
+                wavelength_a = fc.neutron_wavelength(val * 1e6)
+            else:
+                wavelength_a = fc.energy2wave(val)
+        elif unit == 'Energy [meV]':
+            if 'Electron' in rad:
+                wavelength_a = fc.electron_wavelength(val / 1000.)
+            elif 'Neutron' in rad:
+                wavelength_a = fc.neutron_wavelength(val)
+            else:
+                wavelength_a = fc.energy2wave(val / 1.0e6)
+        elif unit == 'Energy [eV]':
+            if 'Electron' in rad:
+                wavelength_a = fc.electron_wavelength(val)
+            elif 'Neutron' in rad:
+                wavelength_a = fc.neutron_wavelength(val * 1000)
+            else:
+                wavelength_a = fc.energy2wave(val / 1000.)
+        elif unit == 'Wavelength [nm]':
+            wavelength_a = val / 10.
+        else:
+            wavelength_a = val
+        return wavelength_a
+
+    def set_wavelength(self, wavelength_a):
+        """set wavelength according to unit"""
+        rad = self.radiation_type.get()
+        unit = self.wavelength_type.get()
+
+        if unit == 'Energy [keV]':
+            if 'Electron' in rad:
+                val = fc.electron_energy(wavelength_a) / 1000.
+            elif 'Neutron' in rad:
+                val = fc.neutron_energy(wavelength_a) / 1.0e6
+            else:
+                val = fc.wave2energy(wavelength_a)
+        elif unit == 'Energy [meV]':
+            if 'Electron' in rad:
+                val = fc.electron_energy(wavelength_a) * 1000
+            elif 'Neutron' in rad:
+                val = fc.neutron_energy(wavelength_a)
+            else:
+                val = fc.wave2energy(wavelength_a) / 1.0e6
+        elif unit == 'Energy [eV]':
+            if 'Electron' in rad:
+                val = fc.electron_energy(wavelength_a)
+            elif 'Neutron' in rad:
+                val = fc.neutron_energy(wavelength_a) * 1000
+            else:
+                val = fc.wave2energy(wavelength_a) / 1000.
+        elif unit == 'Wavelength [nm]':
+            val = wavelength_a * 10.,
+        else:
+            val = wavelength_a
+        self.wavelength_val.set(round(val, 4))
+        self._prev_wavelength_type.set(unit)
+        # Set max Q
+        max_q = fc.calqmag(180, wavelength_a=wavelength_a)
+        max_gen = self.max_gen_type.get()
+        if max_gen == u'Max Q [\u212B\u207B\u00B9]':
+            self.max_val.set(round(max_q, 4))
+        # elif max_gen == u'Max 2\u03B8 [Deg]':
+        #     energy_kev = fc.wave2energy(wavelength_a)
+        #     max_val.set(round(fc.cal2theta(max_q, energy_kev), 4))
+        elif max_gen == u'min d [\u212B]':
+            self.max_val.set(round(fc.q2dspace(max_q), 4))
+
+    def fun_radiation(self, event=None):
+        """Set radiation"""
+        rad = self.radiation_type.get()
+        wavelength_a = self.get_wavelength()
+        if 'Neutron' in rad:
+            self.wavelength_type.set('Energy [meV]')
+        elif 'Electron' in rad:
+            self.wavelength_type.set('Energy [eV]')
+            self.check_magnetic.set(False)
+        else:
+            self.wavelength_type.set('Energy [keV]')
+        self.set_wavelength(wavelength_a)
+
+    def fun_wavelength(self, event=None):
+        """Convert previous unit"""
+        wavelength_a = self.get_wavelength()
+        self.set_wavelength(wavelength_a)
+
+    def fun_edge(self, event=None):
+        """X-ray edge option menu"""
+        edge_name = self.edge.get()
+        if edge_name in self.xr_edges:
+            idx = self.xr_edges.index(edge_name)
+            self.set_wavelength(fc.energy2wave(self.xr_energies[idx]))
+
+    def get_max_q(self, event=None):
+        """Return max val in inverse angstroms, convert if changed"""
+        val = self.max_val.get()
+        old_max_gen = self._prev_max_gen_type.get()
+        max_gen = self.max_gen_type.get()
+        if old_max_gen == u'Max Q [\u212B\u207B\u00B9]':
+            max_q = val
+        elif old_max_gen == u'Max 2\u03B8 [Deg]':
+            wavelength_a = self.get_wavelength()
+            max_q = fc.calqmag(twotheta=val, wavelength_a=wavelength_a)
+        else:  # max_gen == u'min d [\u212B]'
+            max_q = fc.dspace2q(val)
+        # Convert if changed
+        if max_gen != old_max_gen:
+            if max_gen == u'Max Q [\u212B\u207B\u00B9]':
+                self.max_val.set(round(max_q, 4))
+            elif max_gen == u'Max 2\u03B8 [Deg]':
+                wavelength_a = self.get_wavelength()
+                tth = fc.cal2theta(max_q, wavelength_a=wavelength_a)
+                tth = 180. if np.isnan(tth) else tth
+                self.max_val.set(round(tth, 4))
+            else:  # max_gen == u'min d [\u212B]'
+                self.max_val.set(round(fc.q2dspace(max_q), 4))
+            self._prev_max_gen_type.set(max_gen)
+        return max_q
+
+    def help_max_q(self):
+        msg = "Calculate reflection list upto this value\n  (lower angle is less reflections)."
+        messagebox.showinfo(
+            parent=self.root,
+            title='max-Q',
+            message=msg
+        )
+
+    def fun_add_hkl(self, event=None):
+        """Add additional hkl"""
+        hkl = fg.str2array(self.add_hkl.get())
+        if len(hkl) > 0:
+            self.add_reflection(hkl)
+
+    def fun_gen_sym_refs(self):
+        new_list = []
+        for hkl in self.hkl_list:
+            if not fg.vectorinvector(hkl, new_list):
+                new_list += [hkl]
+            sym_list = self.xtl.Symmetry.symmetric_reflections_unique(hkl)
+            for sym_hkl in sym_list:
+                if not fg.vectorinvector(sym_hkl, new_list):
+                    new_list += [sym_hkl]
+        self.add_reflection_list(new_list)
+
+    def fun_rem_sym_refs(self):
+        new_list = self.xtl.Symmetry.remove_symmetric_reflections(self.hkl_list)
+        self.add_reflection_list(new_list)
+
+    def fun_gen_refs(self):
+        """Generate reflections"""
+        maxq = self.get_max_q()
+        hkl = self.xtl.Cell.all_hkl(maxq=maxq)
+        hkl = self.xtl.Cell.sort_hkl(hkl)[1:]  # remove [0,0,0]
+        self.add_reflection_list(hkl)
+
+    def clear_reflections(self):
+        """Clear reflection list"""
+        self.hkl_list = []
+        self.tth_list = []
+        self.sf_list = []
+        self.str_list = []
+        self.lst_data.delete(0, tk.END)
+
+    def add_reflection(self, hkl):
+        """Add reflection to list"""
+        if not fg.vectorinvector(hkl, self.hkl_list):
+            wavelength_a = self.get_wavelength()
+            scattering_type = self.get_scattering_type()
+            tth = self.xtl.Cell.tth(hkl, wavelength_a=wavelength_a)[0]
+            intensity = self.xtl.Scatter.intensity(
+                hkl=hkl,
+                scattering_type=scattering_type,
+                wavelength_a=wavelength_a
+            )[0]
+            intensity = round(intensity, 2)
+            hkl_str = fc.hkl2str(hkl)
+            ref_str = self.REF_FMT % (hkl_str, tth, intensity)
+            self.hkl_list += [hkl]
+            self.tth_list += [tth]
+            self.sf_list += [intensity]
+            self.str_list += [ref_str]
+            self.lst_data.insert(tk.END, ref_str)
+
+    def add_reflection_list(self, hkl_list):
+        """Replace reflection list"""
+        min_sf = self.min_sf.get()
+        max_sf = self.max_sf.get()
+        self.clear_reflections()
+        wavelength_a = self.get_wavelength()
+        scattering_type = self.get_scattering_type()
+        tth = self.xtl.Cell.tth(hkl_list, wavelength_a=wavelength_a)
+        intensity = self.xtl.Scatter.intensity(
+            hkl=hkl_list,
+            scattering_type=scattering_type,
+            wavelength_a=wavelength_a
+        )
+        for n in range(len(hkl_list)):
+            if min_sf < intensity[n] < max_sf:
+                ii = round(intensity[n], 2)
+                hkl_str = fc.hkl2str(hkl_list[n])
+                ref_str = self.REF_FMT % (hkl_str, tth[n], ii)
+                self.hkl_list += [hkl_list[n]]
+                self.tth_list += [tth[n]]
+                self.sf_list += [ii]
+                self.str_list += [ref_str]
+                self.lst_data.insert(tk.END, ref_str)
+
+    "------------------------------------------------------------------------"
+    "--------------------------ListBox Functions-----------------------------"
+    "------------------------------------------------------------------------"
+
+    def show(self):
+        """Run the selection box, wait for response"""
+
+        # self.root.deiconify()  # show window
+        self.root.wait_window()  # wait for window
+        return self.output
+
+    def fun_search(self, event=None):
+        """Search the selection for string"""
+        search_str = self.searchbox.get()
+        search_str = search_str + event.char
+        search_str = search_str.strip().lower()
+        if not search_str: return
+
+        # Clear current selection
+        self.lst_data.select_clear(0, tk.END)
+        view_idx = None
+        # Search for whole words first
+        for n, item in enumerate(self.str_list):
+            if re.search(r'\b%s\b' % search_str, item.lower()):  # whole word search
+                self.lst_data.select_set(n)
+                view_idx = n
+        # if nothing found, search anywhere
+        if view_idx is None:
+            for n, item in enumerate(self.str_list):
+                if search_str in item.lower():
+                    self.lst_data.select_set(n)
+                    view_idx = n
+        if view_idx is not None:
+            self.lst_data.see(view_idx)
+        self.fun_listboxselect()
+
+    def fun_listboxselect(self, event=None):
+        """Update label on listbox selection"""
+        self.numberoffields.set('%3d Selected Fields' % len(self.lst_data.curselection()))
+
+    def fun_exitbutton(self, event=None):
+        """Closes the current data window and generates output"""
+        selection = self.lst_data.curselection()
+        self.output = {
+            'hkl': np.array([self.hkl_list[n] for n in selection], dtype=int),
+            'tth': np.array([self.tth_list[n] for n in selection]),
+            'sf2': np.array([self.sf_list[n] for n in selection]),
+        }
+        self.root.destroy()
+
+    def f_exit(self, event=None):
+        """Closes the current data window"""
+        self.output = {
+            'hkl': np.array([]),
+            'tth': np.array([]),
+            'sf2': np.array([])
+        }
+        self.root.destroy()
+
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/spacegroups.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/spacegroups.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction/tkgui/tensor_scattering.py` & `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/tensor_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction.egg-info/PKG-INFO` & `Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,330 +1,334 @@
 Metadata-Version: 2.1
 Name: Dans-Diffraction
-Version: 3.0.0
+Version: 3.2.0
 Summary: Generate diffracted intensities from crystals
 Home-page: https://github.com/DanPorter/Dans_Diffraction
 Author: Dan Porter
 Author-email: d.g.porter@outlook.com
-License: UNKNOWN
-Description: # Dans_Diffaction
-        Reads crystallographic cif files, calculates crystal properties and simulates diffraction.
-        
-        **Version 3.0**
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7725644.svg)](https://doi.org/10.5281/zenodo.7725644)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb) 
-        [![](https://img.shields.io/github/forks/DanPorter/Dans_Diffraction?label=GitHub%20Repo&style=social)](https://github.com/DanPorter/Dans_Diffraction)
-        
-        
-        By Dan Porter, Diamond Light Source
-        2023
-        
-        #### TL;DR:
-        ```text
-        $ ipython -i -m Dans_Diffraction
-        OR
-        $ ipython -m Dans_Diffraction gui
-        ```
-        
-        ```python
-        """Python Sctipt"""
-        import Dans_Diffraction as dif
-        xtl = dif.Crystal('some_file.cif')
-        print(xtl) # print Crystal structure parameters
-        
-        # Print reflection list:
-        print(xtl.Scatter.print_all_reflections(energy_kev=5)) 
-        
-        # Plot Powder pattern:
-        xtl.Plot.simulate_powder(energy_kev=8)
-        plt.show()
-        
-        # Start graphical user interface:
-        xtl.start_gui()
-        ```
-        
-        Full code documentation available [here](https://danporter.github.io/Dans_Diffraction/).
-        
-        Try it out on [mybinder!](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb)
-        
-        For comments, queries or bugs - email [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk)
-        
-        **Citation:** If you use this code (great!), please cite the published DOI: [10.5281/zenodo.3859501](https://doi.org/10.5281/zenodo.3859501)
-        
-        # Installation
-        **Requirements:** 
-        Python 3+ with packages: *Numpy*, *Matplotlib*, *Tkinter*.
-        BuiltIn packages used: *sys*, *os*, *re*, *glob*, *warnings*, *json*, *itertools*
-        
-        Install stable version from PyPI:
-        ```text
-        $ python -m pip install Dans-Diffraction
-        ```
-        
-        Or, install the latest version direct from GitHub:
-        ```text
-        $ python -m pip install git+https://github.com/DanPorter/Dans_Diffraction.git
-        ```
-        
-        Or, Download the latest version from GitHub (with examples!):
-        ```text
-        $ git clone https://github.com/DanPorter/Dans_Diffraction.git
-        ```
-        
-        
-        
-        # Operation
-        Dans_Diffraction is best run within an interactive python environment:
-        ```text
-        $ ipython -i -m Dans_Diffraction
-        ```
-        
-        Dans_Diffraction can also be run in scripts as an import, example scripts are provided in the [Examples](https://github.com/DanPorter/Dans_Diffraction/blob/master/Examples) folder.
-        ### Read CIF file
-        ```python
-        import Dans_Diffraction as dif
-        xtl = dif.Crystal('some_file.cif')
-        xtl.info() # print Crystal structure parameters
-        help(xtl)  # all functions (nearly!) are documented
-        ```
-        
-        ### Alter atomic positions
-        ```python
-        xtl.Cell.latt([2.85,2.85,10.8,90,90,120]) #  set lattice parameters
-        xtl.Atoms.info() # Print Symmetric positions
-        xtl.Structure.info() # Print All positions in P1 symmetry (same structure and functions as xtl.Atoms)
-        # Symmetric positions
-        xtl.Atoms.changeatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
-        xtl.Atoms.addatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
-        # After adding or changing an atom in the Atoms class, re-generate the full structure using symmetry arguments:
-        xtl.generate_lattice()
-        # Full atomic structure in P1 symmetry
-        xtl.Structure.changeatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
-        xtl.Structure.addatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
-        # Plot crystal Structure
-        xtl.Plot.plot_crystal() # 3D plot
-        xtl.Plot.plot_layers() # 2D plot for layered materials
-        ```
-        ![3D Plot](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/3Dstructrue_Ca3CoMnO6.png?raw=true)
-        
-        
-        ### Alter crystal symmetry
-        ```python
-        xtl.Symmetry.info() # print symmetry arguments
-        xtl.Symmetry.addsym('x,y,z+1/2') # adds single symmetry operation
-        xtl.Symmetry.changesym(0, 'x,y,z+1/4')
-        xtl.Symmetry.load_spacegroup(194) # replaces current symmetry operations
-        # After adding or changing symmetry operations, regengerate the symmetry matrices
-        xtl.Symmetry.generate_matrices()
-        ```
-        
-        ### Save structure as CIF
-        Lattice parameters, crystal structure and symmetry operations will be saved to the CIF.
-        If magnetic moments are defined, magnetic symmetry operations and moments will also be saved
-        and format changed to "*.mcif".
-        ```python
-        xtl.write_cif('edited file.cif')
-        ```
-        
-        ### Calculate Structure Factors
-        X-ray or neutron structure factors/ intensities are calculated based on the full unit cell structure, including atomic 
-        form-factors (x-rays) or coherent scattering lengths (neutrons).
-        ```python
-        # Choose scattering options (see help(xtl.Scatter.setup_scatter))
-        xtl.Scatter.setup_scatter(type='x-ray', energy_keV=8.0)
-        # Allowed radiation types:
-        #    'xray','neutron','xray magnetic','neutron magnetic','xray resonant'
-        xtl.Scatter.print_all_refelctions() # Returns formated string of all allowed reflections
-        inten = xtl.Scatter.intensity([h,k,l]) # Returns intensity
-        twotheta, iten, reflections = xtl.Scatter.powder(units='twotheta')
-        # Plot Experimental Intensities
-        xtl.Plot.simulate_powder() # Powder pattern
-        xtl.Plot.simulate_hk0() # Reciprocal space plane
-        ```
-        ![Powder Pattern](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/powder_diamond.png?raw=true)
-        ![HK0 Simulation](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/supercell_diffraction.png?raw=true)
-        
-        
-        ### Magnetic Structrues
-        *Magnetic structures and scattering are currently in development and shouldn't be treated as accurate!*
-        
-        Simple magnetic structures can be loaded from magnetic cif (*.mcif) files. Magnetic moments are stored for each atomic 
-        position as a vector. The crystal object has a seperate set of magnetic symmetry operations. Symmetry operations from the 
-        tables of magnetic spacegroups can also be loaded. Only simple magnetic structures are allowed. There must be the same
-        number of magnetic symmetry operations as crystal symmetry operations and atomic positions can only have single moments
-        assigned.
-        ```python
-        xtl = dif.Crystal('some_file.mcif')
-        xtl.Atoms.mxmymz() # return magnetic moment vectors on each ion
-        xtl.Symmetry.symmetry_operations_magnetic # magnetic symmetry operations (list of strings)
-        xtl.Symmetry.print_magnetic_spacegroups() # return str of available magnetic spacegroups, given crystal's spacegroup
-        xtl.Symmetry.load_magnetic_spacegroup(mag_spg_number) # loads mag. operations given mag. spacegroup number
-        ```
-        Magnetic scattering is also available for neutrons and x-rays (both resonant and non-resonant), using the appropriate magnetic form-factors.
-        ```python
-        Imag = xtl.Scatter.magnetic_neutron(HKL=[0,0,3])
-        Ires = xtl.Scatter.xray_resonant_magnetic(HKL=[0,0,3], energy_kev=2.838, azim_zero=[1, 0, 0], psi=0, polarisation='s-p', F0=0, F1=1, F2=0)
-        ```
-        
-        ### Superstructures
-        Superstructures can be built using the Superstructure class, requring only a matrix to define the new phase:
-        ```python
-        su = xtl.generate_superstructure([[2,0,0],[0,2,0],[0,0,1]])
-        ```
-        
-        Superstucture classes behave like Crystal classes, but have an additional 'Parent' property that references the original 
-        crystal structure and additional behaviours partiular to superstructures. Superstructures loose their parent crystal and
-        magnetic symmetry, always being defined in P1 symmetry. So su.Atoms == su.Structure.
-        
-        ```python
-        print(su.parent.info())  # Parent structure
-        su.P # superstructure matrix 
-        su.superhkl2parent([h, k, l])  # index superstructure hkl with parent cell
-        su.parenthkl2super([h, k, l])  # index parent hkl with supercell
-        ```
-        
-        ### Multi-phase
-        Scattering from different crystal structures can be compared using the MultiCrystal class:
-        ```python
-        xtls = xtl1 + xtl2
-        xtls.simulate_powder()
-        ```
-        
-        
-        ### Properties
-        The Crystal class contains a lot of atomic properties that can be exposed in the Properties class:
-        ```python
-        xtl.Properties.info()
-        ```
-        
-        Calculated properties include:
-         - Molecular weight
-         - Density
-         - Diamagnetic suscpetibility 
-         - x-ray absorption coefficient, attenuation length, transmission and refractive index
-         - Molecular charge balance
-         - Molecular mass fraction
-         - Atomic orbitals
-         - Magnetic exchange paths (in progress...)
-        
-        Properties are calulated using the atomic structure along with atomic data stored in the folder [Dans_Diffraction/data](data).
-        
-        
-        ### Multiple Scattering
-        Simulations of multiple scattering at different azimuths for a particular energy can be simulated. Based on [code by Dr Gareth Nisbet](https://journals.iucr.org/a/issues/2015/01/00/td5022/).
-         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.12866.svg)](https://doi.org/10.5281/zenodo.12866).
-        
-        ```python
-        azimuth, intensity = xtl.Scatter.ms_azimuth([h,k,l], energy_kev=8)
-        ```
-        
-        ![Multiple Scattering](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/ms_azimuth_silicon.png?raw=true)
-        
-        
-        ### Graphical Front End
-        ![All GUI elements](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_all.png?raw=true)
-        
-        Start a new GUI, then select a cif file:
-        ```text
-        $ ipython -i -m Dans_Diffraction gui
-        ```
-        Or start the GUI from within the interactive console:
-        ```python
-        dif.start_gui()
-        ```
-        Using an already generated crystal:
-        ```python
-        xtl.start_gui()
-        ```
-        
-        ### Diffractometer Simulator
-        ![Diffractometer](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/diffractometer.png?raw=true)
-        
-        New in version 3.0.0. Simulate a generic detector situated around the crystal sample, with the ability to 
-        control detector location shape and size and lattice orientation.
-        
-        
-        ### FDMNES functionality
-        FDMNES is a powerful tool for simulating resonant x-ray diffraction, created by [Y. Joly and O. Bunau.](http://neel.cnrs.fr/spip.php?rubrique1007&lang=en)
-        
-        The Dans_Diffraction FDMNES class allows for the automatic creation of input files and simple analysis of results.
-        The following command should be used to activate these features (only needs to be issued once). 
-        ```python
-        dif.activate_fdmnes()
-        ```
-        Once activated, the FDMNES classes become available.
-        ```python
-        fdm = dif.Fdmnes(xtl) # Create input files and run FDMNES
-        fdma = dif.FdmnesAnalysis(output_path, output_name) # Load output files and plot results
-        ```
-        See class documentation for more information.
-        
-        
-        Once activated, FDMNES GUI elements become available from the main window, emulating functionality of the classes.
-        
-        ![FDMNES Run](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_08.png?raw=true)
-        ![FDMNES Analyse](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_09.png?raw=true)
-        
-        
-        # Acknoledgements
-        | Date       | Thanks to...                                                                            |
-        |------------|-----------------------------------------------------------------------------------------|
-        | 2018       | Thanks to Hepesu for help with Python3 support and ideas about breaking up calculations |
-        | Dec 2019   | Thanks to Gareth Nisbet for allowing me to inlude his multiple scattering siumulation   |
-        | April 2020 | Thanks to ChunHai Wang for helpful suggestions in readcif!                              |
-        | May 2020   | Thanks to AndreEbel for helpful suggestions on citations                                |
-        | Dec 2020   | Thanks to Chris Drozdowski for suggestions about reflection families                    |
-        | Jan 2021   | Thanks to aslarsen for suggestions about outputting the structure factor                |
-        | April 2021 | Thanks to Trygve RÃ¦der for suggestions about x-ray scattering factors                   |
-        | Feb 2022   | Thanks to Mirko for pointing out the error in two-theta values in Scatter.powder        |
-        | March 2022 | Thanks to yevgenyr for suggesting new peak profiles in Scatter.powder                   |
-        | Jan 2023  | Thanks to Anuradha Vibhakar for pointing out the error in f0 + if'-if'' |
-        | Jan 2023   | Thanks to Andreas Rosnes for testing the installation in jupyterlab                     |
-        | May 2023   | Thanks to Carmelo Prestipino for adding electron scattering factors                     |
-        | June 2023  | Thanks to Sergio I. Rincon for pointing out the rounding error in Scatter.powder        |
-        
-        
-        Copyright
-        -----------------------------------------------------------------------------
-           Copyright 2023 Diamond Light Source Ltd.
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-        Files in this package covered by this licence:
-        * classes_crystal.py
-        * classes_scattering.py
-        * classes_plotting.py
-        * classes_properties.py
-        * classes_multicrystal.py
-        * classes_orientation.py
-        * classes_orbitals.py
-        * functions_general.py
-        * functions_plotting.py
-        * functions_scattering.py
-        * functions_crystallography.py
-        * tkgui/*.py
-        
-        Other files are either covered by their own licence or not licenced for other use.
-        
-        | Dr Daniel G Porter | [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk) |
-        | ---- | ---- |
-        | [www.diamond.ac.uk](www.diamond.ac.uk) | Diamond Light Source, Chilton, Didcot, Oxon, OX11 0DE, U.K. |
-        
 Keywords: crystal,cif,diffraction,crystallography,science,x-ray,neutron,resonant,magnetic,magnetism,multiple scattering,fdmnes,super structure,spacegroup,space group,diffractometer
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+
+# Dans_Diffraction
+Reads crystallographic cif files, calculates crystal properties and simulates diffraction.
+
+**Version 3.2**
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106031.svg)](https://doi.org/10.5281/zenodo.8106031)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb) 
+[![](https://img.shields.io/github/forks/DanPorter/Dans_Diffraction?label=GitHub%20Repo&style=social)](https://github.com/DanPorter/Dans_Diffraction)
+
+
+By Dan Porter, Diamond Light Source
+2024
+
+#### TL;DR:
+```text
+$ ipython -i -m Dans_Diffraction
+OR
+$ ipython -m Dans_Diffraction gui
+```
+
+```python
+"""Python Sctipt"""
+import Dans_Diffraction as dif
+xtl = dif.Crystal('some_file.cif')
+print(xtl) # print Crystal structure parameters
+
+# Print reflection list:
+print(xtl.Scatter.print_all_reflections(energy_kev=5)) 
+
+# Plot Powder pattern:
+xtl.Plot.simulate_powder(energy_kev=8)
+plt.show()
+
+# Start graphical user interface:
+xtl.start_gui()
+```
+
+Full code documentation available [here](https://danporter.github.io/Dans_Diffraction/).
+
+Try it out on [mybinder!](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb)
+
+For comments, queries or bugs - email [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk)
+
+**Citation:** If you use this code (great!), please cite the published DOI: [10.5281/zenodo.8106031](https://doi.org/10.5281/zenodo.8106031)
+
+# Installation
+**Requirements:** 
+Python 3+ with packages: *Numpy*, *Matplotlib*, *Tkinter*.
+BuiltIn packages used: *sys*, *os*, *re*, *glob*, *warnings*, *json*, *itertools*
+
+Install stable version from PyPI:
+```text
+$ python -m pip install Dans-Diffraction
+```
+
+Or, install the latest version direct from GitHub:
+```text
+$ python -m pip install git+https://github.com/DanPorter/Dans_Diffraction.git
+```
+
+Or, Download the latest version from GitHub (with examples!):
+```text
+$ git clone https://github.com/DanPorter/Dans_Diffraction.git
+```
+
+
+
+# Operation
+Dans_Diffraction is best run within an interactive python environment:
+```text
+$ ipython -i -m Dans_Diffraction
+```
+
+Dans_Diffraction can also be run in scripts as an import, example scripts are provided in the [Examples](https://github.com/DanPorter/Dans_Diffraction/blob/master/Examples) folder.
+### Read CIF file
+```python
+import Dans_Diffraction as dif
+xtl = dif.Crystal('some_file.cif')
+xtl.info() # print Crystal structure parameters
+help(xtl)  # all functions (nearly!) are documented
+```
+
+### Alter atomic positions
+```python
+xtl.Cell.latt([2.85,2.85,10.8,90,90,120]) #  set lattice parameters
+xtl.Atoms.info() # Print Symmetric positions
+xtl.Structure.info() # Print All positions in P1 symmetry (same structure and functions as xtl.Atoms)
+# Symmetric positions
+xtl.Atoms.changeatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
+xtl.Atoms.addatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
+# After adding or changing an atom in the Atoms class, re-generate the full structure using symmetry arguments:
+xtl.generate_lattice()
+# Full atomic structure in P1 symmetry
+xtl.Structure.changeatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
+xtl.Structure.addatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
+# Plot crystal Structure
+xtl.Plot.plot_crystal() # 3D plot
+xtl.Plot.plot_layers() # 2D plot for layered materials
+```
+![3D Plot](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/3Dstructrue_Ca3CoMnO6.png?raw=true)
+
+
+### Alter crystal symmetry
+```python
+xtl.Symmetry.info() # print symmetry arguments
+xtl.Symmetry.addsym('x,y,z+1/2') # adds single symmetry operation
+xtl.Symmetry.changesym(0, 'x,y,z+1/4')
+xtl.Symmetry.load_spacegroup(194) # replaces current symmetry operations
+# After adding or changing symmetry operations, regengerate the symmetry matrices
+xtl.Symmetry.generate_matrices()
+```
+
+### Save structure as CIF
+Lattice parameters, crystal structure and symmetry operations will be saved to the CIF.
+If magnetic moments are defined, magnetic symmetry operations and moments will also be saved
+and format changed to "*.mcif".
+```python
+xtl.write_cif('edited file.cif')
+```
+
+### Calculate Structure Factors
+X-ray or neutron structure factors/ intensities are calculated based on the full unit cell structure, including atomic 
+form-factors (x-rays) or coherent scattering lengths (neutrons).
+```python
+# Choose scattering options (see help(xtl.Scatter.setup_scatter))
+xtl.Scatter.setup_scatter(type='x-ray', energy_keV=8.0)
+# Allowed radiation types:
+#    'xray','neutron','xray magnetic','neutron magnetic','xray resonant'
+xtl.Scatter.print_all_refelctions() # Returns formated string of all allowed reflections
+inten = xtl.Scatter.intensity([h,k,l]) # Returns intensity
+twotheta, iten, reflections = xtl.Scatter.powder(units='twotheta')
+# Plot Experimental Intensities
+xtl.Plot.simulate_powder() # Powder pattern
+xtl.Plot.simulate_hk0() # Reciprocal space plane
+```
+![Powder Pattern](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/powder_diamond.png?raw=true)
+![HK0 Simulation](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/supercell_diffraction.png?raw=true)
+
+
+### Magnetic Structrues
+*Magnetic structures and scattering are currently in development and shouldn't be treated as accurate!*
+
+Simple magnetic structures can be loaded from magnetic cif (*.mcif) files. Magnetic moments are stored for each atomic 
+position as a vector. The crystal object has a seperate set of magnetic symmetry operations. Symmetry operations from the 
+tables of magnetic spacegroups can also be loaded. Only simple magnetic structures are allowed. There must be the same
+number of magnetic symmetry operations as crystal symmetry operations and atomic positions can only have single moments
+assigned.
+```python
+xtl = dif.Crystal('some_file.mcif')
+xtl.Atoms.mxmymz() # return magnetic moment vectors on each ion
+xtl.Symmetry.symmetry_operations_magnetic # magnetic symmetry operations (list of strings)
+xtl.Symmetry.print_magnetic_spacegroups() # return str of available magnetic spacegroups, given crystal's spacegroup
+xtl.Symmetry.load_magnetic_spacegroup(mag_spg_number) # loads mag. operations given mag. spacegroup number
+```
+Magnetic scattering is also available for neutrons and x-rays (both resonant and non-resonant), using the appropriate magnetic form-factors.
+```python
+Imag = xtl.Scatter.magnetic_neutron(HKL=[0,0,3])
+Ires = xtl.Scatter.xray_resonant_magnetic(HKL=[0,0,3], energy_kev=2.838, azim_zero=[1, 0, 0], psi=0, polarisation='s-p', F0=0, F1=1, F2=0)
+```
+
+### Superstructures
+Superstructures can be built using the Superstructure class, requring only a matrix to define the new phase:
+```python
+su = xtl.generate_superstructure([[2,0,0],[0,2,0],[0,0,1]])
+```
+
+Superstucture classes behave like Crystal classes, but have an additional 'Parent' property that references the original 
+crystal structure and additional behaviours partiular to superstructures. Superstructures loose their parent crystal and
+magnetic symmetry, always being defined in P1 symmetry. So su.Atoms == su.Structure.
+
+```python
+print(su.parent.info())  # Parent structure
+su.P # superstructure matrix 
+su.superhkl2parent([h, k, l])  # index superstructure hkl with parent cell
+su.parenthkl2super([h, k, l])  # index parent hkl with supercell
+```
+
+### Multi-phase
+Scattering from different crystal structures can be compared using the MultiCrystal class:
+```python
+xtls = xtl1 + xtl2
+xtls.simulate_powder()
+```
+
+
+### Properties
+The Crystal class contains a lot of atomic properties that can be exposed in the Properties class:
+```python
+xtl.Properties.info()
+```
+
+Calculated properties include:
+ - Molecular weight
+ - Density
+ - Diamagnetic suscpetibility 
+ - x-ray absorption coefficient, attenuation length, transmission and refractive index
+ - Molecular charge balance
+ - Molecular mass fraction
+ - Atomic orbitals
+ - Magnetic exchange paths (in progress...)
+
+Properties are calulated using the atomic structure along with atomic data stored in the folder [Dans_Diffraction/data](data).
+
+
+### Multiple Scattering
+Simulations of multiple scattering at different azimuths for a particular energy can be simulated. Based on [code by Dr Gareth Nisbet](https://journals.iucr.org/a/issues/2015/01/00/td5022/).
+ [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.12866.svg)](https://doi.org/10.5281/zenodo.12866).
+
+```python
+azimuth, intensity = xtl.Scatter.ms_azimuth([h,k,l], energy_kev=8)
+```
+
+![Multiple Scattering](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/ms_azimuth_silicon.png?raw=true)
+
+
+### Graphical Front End
+![All GUI elements](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_all.png?raw=true)
+
+Start a new GUI, then select a cif file:
+```text
+$ ipython -i -m Dans_Diffraction gui
+```
+Or start the GUI from within the interactive console:
+```python
+dif.start_gui()
+```
+Using an already generated crystal:
+```python
+xtl.start_gui()
+```
+
+### Diffractometer Simulator
+![Diffractometer](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/diffractometer.png?raw=true)
+
+New in version 3.0.0. Simulate a generic detector situated around the crystal sample, with the ability to 
+control detector location shape and size and lattice orientation.
+
+
+### FDMNES functionality
+FDMNES is a powerful tool for simulating resonant x-ray diffraction, created by [Y. Joly and O. Bunau.](https://fdmnes.neel.cnrs.fr/)
+
+The Dans_Diffraction FDMNES class allows for the automatic creation of input files and simple analysis of results.
+The following command should be used to activate these features (only needs to be issued once). 
+```python
+dif.activate_fdmnes()
+```
+Once activated, the FDMNES classes become available.
+```python
+fdm = dif.Fdmnes(xtl) # Create input files and run FDMNES
+fdma = dif.FdmnesAnalysis(output_path, output_name) # Load output files and plot results
+```
+See class documentation for more information.
+
+
+Once activated, FDMNES GUI elements become available from the main window, emulating functionality of the classes.
+
+![FDMNES Run](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_08.png?raw=true)
+![FDMNES Analyse](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_09.png?raw=true)
+
+
+# Acknoledgements
+| Date       | Thanks to...                                                                            |
+|------------|-----------------------------------------------------------------------------------------|
+| 2018       | Thanks to Hepesu for help with Python3 support and ideas about breaking up calculations |
+| Dec 2019   | Thanks to Gareth Nisbet for allowing me to inlude his multiple scattering siumulation   |
+| April 2020 | Thanks to ChunHai Wang for helpful suggestions in readcif!                              |
+| May 2020   | Thanks to AndreEbel for helpful suggestions on citations                                |
+| Dec 2020   | Thanks to Chris Drozdowski for suggestions about reflection families                    |
+| Jan 2021   | Thanks to aslarsen for suggestions about outputting the structure factor                |
+| April 2021 | Thanks to Trygve RÃ¦der for suggestions about x-ray scattering factors                   |
+| Feb 2022   | Thanks to Mirko for pointing out the error in two-theta values in Scatter.powder        |
+| March 2022 | Thanks to yevgenyr for suggesting new peak profiles in Scatter.powder                   |
+| Jan 2023   | Thanks to Anuradha Vibhakar for pointing out the error in f0 + if'-if''                 |
+| Jan 2023   | Thanks to Andreas Rosnes for testing the installation in jupyterlab                     |
+| May 2023   | Thanks to Carmelo Prestipino for adding electron scattering factors                     |
+| June 2023  | Thanks to Sergio I. Rincon for pointing out the rounding error in Scatter.powder        |
+| July 2023  | Thanks to asteppke for suggested update to Arrow3D for matplotlib V>3.4                 |
+| July 2023  | Thanks to Yves Joly for helpful suggestions on FDMNES wrapper                           |
+| April 2024 | Thanks to Innbig for pointing out an issue with liquid crystal simulations              |
+| May 2024   | Thanks to paul-cares pointing out a silly spelling error in the title!                  |
+
+Copyright
+-----------------------------------------------------------------------------
+   Copyright 2024 Diamond Light Source Ltd.
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+Files in this package covered by this licence:
+* classes_crystal.py
+* classes_scattering.py
+* classes_plotting.py
+* classes_properties.py
+* classes_multicrystal.py
+* classes_orientation.py
+* classes_orbitals.py
+* functions_general.py
+* functions_plotting.py
+* functions_scattering.py
+* functions_crystallography.py
+* tkgui/*.py
+
+Other files are either covered by their own licence or not licenced for other use.
+
+| Dr Daniel G Porter | [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk) |
+| ---- | ---- |
+| [www.diamond.ac.uk](www.diamond.ac.uk) | Diamond Light Source, Chilton, Didcot, Oxon, OX11 0DE, U.K. |
```

### Comparing `Dans_Diffraction-3.0.0/Dans_Diffraction.egg-info/SOURCES.txt` & `Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 Dans_Diffraction/__init__.py
 Dans_Diffraction/__main__.py
 Dans_Diffraction/classes_crystal.py
 Dans_Diffraction/classes_fdmnes.py
 Dans_Diffraction/classes_multicrystal.py
@@ -78,14 +79,15 @@
 Dans_Diffraction/tkgui/tensor_scattering.py
 test/test_LS_magnetic_components.py
 test/test_WaasKirf_xray_factors.py
 test/test_atom_properties.py
 test/test_attenuation.py
 test/test_attenuation_length.py
 test/test_bmatrix.py
+test/test_check_append_vs_unique.py
 test/test_cif_files.py
 test/test_coherent_diffraction.py
 test/test_coherent_diffraction2.py
 test/test_compare_intensity.py
 test/test_compare_intensity_calculation.py
 test/test_compound_name.py
 test/test_convolve2d.py
@@ -111,11 +113,12 @@
 test/test_nonresonant_sergio.py
 test/test_orientation.py
 test/test_parameter_plot.py
 test/test_plot_orbitals.py
 test/test_plotintensity.py
 test/test_plotintensity2.py
 test/test_readstfm.py
+test/test_reflection_selector.py
 test/test_refractive_index.py
 test/test_scattering.py
 test/test_supercell.py
 test/test_symmetry_ops2magnetic.py
```

### Comparing `Dans_Diffraction-3.0.0/PKG-INFO` & `Dans_Diffraction-3.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,330 +1,334 @@
 Metadata-Version: 2.1
 Name: Dans_Diffraction
-Version: 3.0.0
+Version: 3.2.0
 Summary: Generate diffracted intensities from crystals
 Home-page: https://github.com/DanPorter/Dans_Diffraction
 Author: Dan Porter
 Author-email: d.g.porter@outlook.com
-License: UNKNOWN
-Description: # Dans_Diffaction
-        Reads crystallographic cif files, calculates crystal properties and simulates diffraction.
-        
-        **Version 3.0**
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7725644.svg)](https://doi.org/10.5281/zenodo.7725644)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb) 
-        [![](https://img.shields.io/github/forks/DanPorter/Dans_Diffraction?label=GitHub%20Repo&style=social)](https://github.com/DanPorter/Dans_Diffraction)
-        
-        
-        By Dan Porter, Diamond Light Source
-        2023
-        
-        #### TL;DR:
-        ```text
-        $ ipython -i -m Dans_Diffraction
-        OR
-        $ ipython -m Dans_Diffraction gui
-        ```
-        
-        ```python
-        """Python Sctipt"""
-        import Dans_Diffraction as dif
-        xtl = dif.Crystal('some_file.cif')
-        print(xtl) # print Crystal structure parameters
-        
-        # Print reflection list:
-        print(xtl.Scatter.print_all_reflections(energy_kev=5)) 
-        
-        # Plot Powder pattern:
-        xtl.Plot.simulate_powder(energy_kev=8)
-        plt.show()
-        
-        # Start graphical user interface:
-        xtl.start_gui()
-        ```
-        
-        Full code documentation available [here](https://danporter.github.io/Dans_Diffraction/).
-        
-        Try it out on [mybinder!](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb)
-        
-        For comments, queries or bugs - email [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk)
-        
-        **Citation:** If you use this code (great!), please cite the published DOI: [10.5281/zenodo.3859501](https://doi.org/10.5281/zenodo.3859501)
-        
-        # Installation
-        **Requirements:** 
-        Python 3+ with packages: *Numpy*, *Matplotlib*, *Tkinter*.
-        BuiltIn packages used: *sys*, *os*, *re*, *glob*, *warnings*, *json*, *itertools*
-        
-        Install stable version from PyPI:
-        ```text
-        $ python -m pip install Dans-Diffraction
-        ```
-        
-        Or, install the latest version direct from GitHub:
-        ```text
-        $ python -m pip install git+https://github.com/DanPorter/Dans_Diffraction.git
-        ```
-        
-        Or, Download the latest version from GitHub (with examples!):
-        ```text
-        $ git clone https://github.com/DanPorter/Dans_Diffraction.git
-        ```
-        
-        
-        
-        # Operation
-        Dans_Diffraction is best run within an interactive python environment:
-        ```text
-        $ ipython -i -m Dans_Diffraction
-        ```
-        
-        Dans_Diffraction can also be run in scripts as an import, example scripts are provided in the [Examples](https://github.com/DanPorter/Dans_Diffraction/blob/master/Examples) folder.
-        ### Read CIF file
-        ```python
-        import Dans_Diffraction as dif
-        xtl = dif.Crystal('some_file.cif')
-        xtl.info() # print Crystal structure parameters
-        help(xtl)  # all functions (nearly!) are documented
-        ```
-        
-        ### Alter atomic positions
-        ```python
-        xtl.Cell.latt([2.85,2.85,10.8,90,90,120]) #  set lattice parameters
-        xtl.Atoms.info() # Print Symmetric positions
-        xtl.Structure.info() # Print All positions in P1 symmetry (same structure and functions as xtl.Atoms)
-        # Symmetric positions
-        xtl.Atoms.changeatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
-        xtl.Atoms.addatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
-        # After adding or changing an atom in the Atoms class, re-generate the full structure using symmetry arguments:
-        xtl.generate_lattice()
-        # Full atomic structure in P1 symmetry
-        xtl.Structure.changeatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
-        xtl.Structure.addatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
-        # Plot crystal Structure
-        xtl.Plot.plot_crystal() # 3D plot
-        xtl.Plot.plot_layers() # 2D plot for layered materials
-        ```
-        ![3D Plot](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/3Dstructrue_Ca3CoMnO6.png?raw=true)
-        
-        
-        ### Alter crystal symmetry
-        ```python
-        xtl.Symmetry.info() # print symmetry arguments
-        xtl.Symmetry.addsym('x,y,z+1/2') # adds single symmetry operation
-        xtl.Symmetry.changesym(0, 'x,y,z+1/4')
-        xtl.Symmetry.load_spacegroup(194) # replaces current symmetry operations
-        # After adding or changing symmetry operations, regengerate the symmetry matrices
-        xtl.Symmetry.generate_matrices()
-        ```
-        
-        ### Save structure as CIF
-        Lattice parameters, crystal structure and symmetry operations will be saved to the CIF.
-        If magnetic moments are defined, magnetic symmetry operations and moments will also be saved
-        and format changed to "*.mcif".
-        ```python
-        xtl.write_cif('edited file.cif')
-        ```
-        
-        ### Calculate Structure Factors
-        X-ray or neutron structure factors/ intensities are calculated based on the full unit cell structure, including atomic 
-        form-factors (x-rays) or coherent scattering lengths (neutrons).
-        ```python
-        # Choose scattering options (see help(xtl.Scatter.setup_scatter))
-        xtl.Scatter.setup_scatter(type='x-ray', energy_keV=8.0)
-        # Allowed radiation types:
-        #    'xray','neutron','xray magnetic','neutron magnetic','xray resonant'
-        xtl.Scatter.print_all_refelctions() # Returns formated string of all allowed reflections
-        inten = xtl.Scatter.intensity([h,k,l]) # Returns intensity
-        twotheta, iten, reflections = xtl.Scatter.powder(units='twotheta')
-        # Plot Experimental Intensities
-        xtl.Plot.simulate_powder() # Powder pattern
-        xtl.Plot.simulate_hk0() # Reciprocal space plane
-        ```
-        ![Powder Pattern](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/powder_diamond.png?raw=true)
-        ![HK0 Simulation](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/supercell_diffraction.png?raw=true)
-        
-        
-        ### Magnetic Structrues
-        *Magnetic structures and scattering are currently in development and shouldn't be treated as accurate!*
-        
-        Simple magnetic structures can be loaded from magnetic cif (*.mcif) files. Magnetic moments are stored for each atomic 
-        position as a vector. The crystal object has a seperate set of magnetic symmetry operations. Symmetry operations from the 
-        tables of magnetic spacegroups can also be loaded. Only simple magnetic structures are allowed. There must be the same
-        number of magnetic symmetry operations as crystal symmetry operations and atomic positions can only have single moments
-        assigned.
-        ```python
-        xtl = dif.Crystal('some_file.mcif')
-        xtl.Atoms.mxmymz() # return magnetic moment vectors on each ion
-        xtl.Symmetry.symmetry_operations_magnetic # magnetic symmetry operations (list of strings)
-        xtl.Symmetry.print_magnetic_spacegroups() # return str of available magnetic spacegroups, given crystal's spacegroup
-        xtl.Symmetry.load_magnetic_spacegroup(mag_spg_number) # loads mag. operations given mag. spacegroup number
-        ```
-        Magnetic scattering is also available for neutrons and x-rays (both resonant and non-resonant), using the appropriate magnetic form-factors.
-        ```python
-        Imag = xtl.Scatter.magnetic_neutron(HKL=[0,0,3])
-        Ires = xtl.Scatter.xray_resonant_magnetic(HKL=[0,0,3], energy_kev=2.838, azim_zero=[1, 0, 0], psi=0, polarisation='s-p', F0=0, F1=1, F2=0)
-        ```
-        
-        ### Superstructures
-        Superstructures can be built using the Superstructure class, requring only a matrix to define the new phase:
-        ```python
-        su = xtl.generate_superstructure([[2,0,0],[0,2,0],[0,0,1]])
-        ```
-        
-        Superstucture classes behave like Crystal classes, but have an additional 'Parent' property that references the original 
-        crystal structure and additional behaviours partiular to superstructures. Superstructures loose their parent crystal and
-        magnetic symmetry, always being defined in P1 symmetry. So su.Atoms == su.Structure.
-        
-        ```python
-        print(su.parent.info())  # Parent structure
-        su.P # superstructure matrix 
-        su.superhkl2parent([h, k, l])  # index superstructure hkl with parent cell
-        su.parenthkl2super([h, k, l])  # index parent hkl with supercell
-        ```
-        
-        ### Multi-phase
-        Scattering from different crystal structures can be compared using the MultiCrystal class:
-        ```python
-        xtls = xtl1 + xtl2
-        xtls.simulate_powder()
-        ```
-        
-        
-        ### Properties
-        The Crystal class contains a lot of atomic properties that can be exposed in the Properties class:
-        ```python
-        xtl.Properties.info()
-        ```
-        
-        Calculated properties include:
-         - Molecular weight
-         - Density
-         - Diamagnetic suscpetibility 
-         - x-ray absorption coefficient, attenuation length, transmission and refractive index
-         - Molecular charge balance
-         - Molecular mass fraction
-         - Atomic orbitals
-         - Magnetic exchange paths (in progress...)
-        
-        Properties are calulated using the atomic structure along with atomic data stored in the folder [Dans_Diffraction/data](data).
-        
-        
-        ### Multiple Scattering
-        Simulations of multiple scattering at different azimuths for a particular energy can be simulated. Based on [code by Dr Gareth Nisbet](https://journals.iucr.org/a/issues/2015/01/00/td5022/).
-         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.12866.svg)](https://doi.org/10.5281/zenodo.12866).
-        
-        ```python
-        azimuth, intensity = xtl.Scatter.ms_azimuth([h,k,l], energy_kev=8)
-        ```
-        
-        ![Multiple Scattering](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/ms_azimuth_silicon.png?raw=true)
-        
-        
-        ### Graphical Front End
-        ![All GUI elements](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_all.png?raw=true)
-        
-        Start a new GUI, then select a cif file:
-        ```text
-        $ ipython -i -m Dans_Diffraction gui
-        ```
-        Or start the GUI from within the interactive console:
-        ```python
-        dif.start_gui()
-        ```
-        Using an already generated crystal:
-        ```python
-        xtl.start_gui()
-        ```
-        
-        ### Diffractometer Simulator
-        ![Diffractometer](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/diffractometer.png?raw=true)
-        
-        New in version 3.0.0. Simulate a generic detector situated around the crystal sample, with the ability to 
-        control detector location shape and size and lattice orientation.
-        
-        
-        ### FDMNES functionality
-        FDMNES is a powerful tool for simulating resonant x-ray diffraction, created by [Y. Joly and O. Bunau.](http://neel.cnrs.fr/spip.php?rubrique1007&lang=en)
-        
-        The Dans_Diffraction FDMNES class allows for the automatic creation of input files and simple analysis of results.
-        The following command should be used to activate these features (only needs to be issued once). 
-        ```python
-        dif.activate_fdmnes()
-        ```
-        Once activated, the FDMNES classes become available.
-        ```python
-        fdm = dif.Fdmnes(xtl) # Create input files and run FDMNES
-        fdma = dif.FdmnesAnalysis(output_path, output_name) # Load output files and plot results
-        ```
-        See class documentation for more information.
-        
-        
-        Once activated, FDMNES GUI elements become available from the main window, emulating functionality of the classes.
-        
-        ![FDMNES Run](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_08.png?raw=true)
-        ![FDMNES Analyse](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_09.png?raw=true)
-        
-        
-        # Acknoledgements
-        | Date       | Thanks to...                                                                            |
-        |------------|-----------------------------------------------------------------------------------------|
-        | 2018       | Thanks to Hepesu for help with Python3 support and ideas about breaking up calculations |
-        | Dec 2019   | Thanks to Gareth Nisbet for allowing me to inlude his multiple scattering siumulation   |
-        | April 2020 | Thanks to ChunHai Wang for helpful suggestions in readcif!                              |
-        | May 2020   | Thanks to AndreEbel for helpful suggestions on citations                                |
-        | Dec 2020   | Thanks to Chris Drozdowski for suggestions about reflection families                    |
-        | Jan 2021   | Thanks to aslarsen for suggestions about outputting the structure factor                |
-        | April 2021 | Thanks to Trygve RÃ¦der for suggestions about x-ray scattering factors                   |
-        | Feb 2022   | Thanks to Mirko for pointing out the error in two-theta values in Scatter.powder        |
-        | March 2022 | Thanks to yevgenyr for suggesting new peak profiles in Scatter.powder                   |
-        | Jan 2023  | Thanks to Anuradha Vibhakar for pointing out the error in f0 + if'-if'' |
-        | Jan 2023   | Thanks to Andreas Rosnes for testing the installation in jupyterlab                     |
-        | May 2023   | Thanks to Carmelo Prestipino for adding electron scattering factors                     |
-        | June 2023  | Thanks to Sergio I. Rincon for pointing out the rounding error in Scatter.powder        |
-        
-        
-        Copyright
-        -----------------------------------------------------------------------------
-           Copyright 2023 Diamond Light Source Ltd.
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-        Files in this package covered by this licence:
-        * classes_crystal.py
-        * classes_scattering.py
-        * classes_plotting.py
-        * classes_properties.py
-        * classes_multicrystal.py
-        * classes_orientation.py
-        * classes_orbitals.py
-        * functions_general.py
-        * functions_plotting.py
-        * functions_scattering.py
-        * functions_crystallography.py
-        * tkgui/*.py
-        
-        Other files are either covered by their own licence or not licenced for other use.
-        
-        | Dr Daniel G Porter | [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk) |
-        | ---- | ---- |
-        | [www.diamond.ac.uk](www.diamond.ac.uk) | Diamond Light Source, Chilton, Didcot, Oxon, OX11 0DE, U.K. |
-        
 Keywords: crystal,cif,diffraction,crystallography,science,x-ray,neutron,resonant,magnetic,magnetism,multiple scattering,fdmnes,super structure,spacegroup,space group,diffractometer
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+
+# Dans_Diffraction
+Reads crystallographic cif files, calculates crystal properties and simulates diffraction.
+
+**Version 3.2**
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106031.svg)](https://doi.org/10.5281/zenodo.8106031)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb) 
+[![](https://img.shields.io/github/forks/DanPorter/Dans_Diffraction?label=GitHub%20Repo&style=social)](https://github.com/DanPorter/Dans_Diffraction)
+
+
+By Dan Porter, Diamond Light Source
+2024
+
+#### TL;DR:
+```text
+$ ipython -i -m Dans_Diffraction
+OR
+$ ipython -m Dans_Diffraction gui
+```
+
+```python
+"""Python Sctipt"""
+import Dans_Diffraction as dif
+xtl = dif.Crystal('some_file.cif')
+print(xtl) # print Crystal structure parameters
+
+# Print reflection list:
+print(xtl.Scatter.print_all_reflections(energy_kev=5)) 
+
+# Plot Powder pattern:
+xtl.Plot.simulate_powder(energy_kev=8)
+plt.show()
+
+# Start graphical user interface:
+xtl.start_gui()
+```
+
+Full code documentation available [here](https://danporter.github.io/Dans_Diffraction/).
+
+Try it out on [mybinder!](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb)
+
+For comments, queries or bugs - email [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk)
+
+**Citation:** If you use this code (great!), please cite the published DOI: [10.5281/zenodo.8106031](https://doi.org/10.5281/zenodo.8106031)
+
+# Installation
+**Requirements:** 
+Python 3+ with packages: *Numpy*, *Matplotlib*, *Tkinter*.
+BuiltIn packages used: *sys*, *os*, *re*, *glob*, *warnings*, *json*, *itertools*
+
+Install stable version from PyPI:
+```text
+$ python -m pip install Dans-Diffraction
+```
+
+Or, install the latest version direct from GitHub:
+```text
+$ python -m pip install git+https://github.com/DanPorter/Dans_Diffraction.git
+```
+
+Or, Download the latest version from GitHub (with examples!):
+```text
+$ git clone https://github.com/DanPorter/Dans_Diffraction.git
+```
+
+
+
+# Operation
+Dans_Diffraction is best run within an interactive python environment:
+```text
+$ ipython -i -m Dans_Diffraction
+```
+
+Dans_Diffraction can also be run in scripts as an import, example scripts are provided in the [Examples](https://github.com/DanPorter/Dans_Diffraction/blob/master/Examples) folder.
+### Read CIF file
+```python
+import Dans_Diffraction as dif
+xtl = dif.Crystal('some_file.cif')
+xtl.info() # print Crystal structure parameters
+help(xtl)  # all functions (nearly!) are documented
+```
+
+### Alter atomic positions
+```python
+xtl.Cell.latt([2.85,2.85,10.8,90,90,120]) #  set lattice parameters
+xtl.Atoms.info() # Print Symmetric positions
+xtl.Structure.info() # Print All positions in P1 symmetry (same structure and functions as xtl.Atoms)
+# Symmetric positions
+xtl.Atoms.changeatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
+xtl.Atoms.addatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
+# After adding or changing an atom in the Atoms class, re-generate the full structure using symmetry arguments:
+xtl.generate_lattice()
+# Full atomic structure in P1 symmetry
+xtl.Structure.changeatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
+xtl.Structure.addatom(idx=0, u=0, v=0, w=0, type='Co', label='Co1')
+# Plot crystal Structure
+xtl.Plot.plot_crystal() # 3D plot
+xtl.Plot.plot_layers() # 2D plot for layered materials
+```
+![3D Plot](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/3Dstructrue_Ca3CoMnO6.png?raw=true)
+
+
+### Alter crystal symmetry
+```python
+xtl.Symmetry.info() # print symmetry arguments
+xtl.Symmetry.addsym('x,y,z+1/2') # adds single symmetry operation
+xtl.Symmetry.changesym(0, 'x,y,z+1/4')
+xtl.Symmetry.load_spacegroup(194) # replaces current symmetry operations
+# After adding or changing symmetry operations, regengerate the symmetry matrices
+xtl.Symmetry.generate_matrices()
+```
+
+### Save structure as CIF
+Lattice parameters, crystal structure and symmetry operations will be saved to the CIF.
+If magnetic moments are defined, magnetic symmetry operations and moments will also be saved
+and format changed to "*.mcif".
+```python
+xtl.write_cif('edited file.cif')
+```
+
+### Calculate Structure Factors
+X-ray or neutron structure factors/ intensities are calculated based on the full unit cell structure, including atomic 
+form-factors (x-rays) or coherent scattering lengths (neutrons).
+```python
+# Choose scattering options (see help(xtl.Scatter.setup_scatter))
+xtl.Scatter.setup_scatter(type='x-ray', energy_keV=8.0)
+# Allowed radiation types:
+#    'xray','neutron','xray magnetic','neutron magnetic','xray resonant'
+xtl.Scatter.print_all_refelctions() # Returns formated string of all allowed reflections
+inten = xtl.Scatter.intensity([h,k,l]) # Returns intensity
+twotheta, iten, reflections = xtl.Scatter.powder(units='twotheta')
+# Plot Experimental Intensities
+xtl.Plot.simulate_powder() # Powder pattern
+xtl.Plot.simulate_hk0() # Reciprocal space plane
+```
+![Powder Pattern](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/powder_diamond.png?raw=true)
+![HK0 Simulation](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/supercell_diffraction.png?raw=true)
+
+
+### Magnetic Structrues
+*Magnetic structures and scattering are currently in development and shouldn't be treated as accurate!*
+
+Simple magnetic structures can be loaded from magnetic cif (*.mcif) files. Magnetic moments are stored for each atomic 
+position as a vector. The crystal object has a seperate set of magnetic symmetry operations. Symmetry operations from the 
+tables of magnetic spacegroups can also be loaded. Only simple magnetic structures are allowed. There must be the same
+number of magnetic symmetry operations as crystal symmetry operations and atomic positions can only have single moments
+assigned.
+```python
+xtl = dif.Crystal('some_file.mcif')
+xtl.Atoms.mxmymz() # return magnetic moment vectors on each ion
+xtl.Symmetry.symmetry_operations_magnetic # magnetic symmetry operations (list of strings)
+xtl.Symmetry.print_magnetic_spacegroups() # return str of available magnetic spacegroups, given crystal's spacegroup
+xtl.Symmetry.load_magnetic_spacegroup(mag_spg_number) # loads mag. operations given mag. spacegroup number
+```
+Magnetic scattering is also available for neutrons and x-rays (both resonant and non-resonant), using the appropriate magnetic form-factors.
+```python
+Imag = xtl.Scatter.magnetic_neutron(HKL=[0,0,3])
+Ires = xtl.Scatter.xray_resonant_magnetic(HKL=[0,0,3], energy_kev=2.838, azim_zero=[1, 0, 0], psi=0, polarisation='s-p', F0=0, F1=1, F2=0)
+```
+
+### Superstructures
+Superstructures can be built using the Superstructure class, requring only a matrix to define the new phase:
+```python
+su = xtl.generate_superstructure([[2,0,0],[0,2,0],[0,0,1]])
+```
+
+Superstucture classes behave like Crystal classes, but have an additional 'Parent' property that references the original 
+crystal structure and additional behaviours partiular to superstructures. Superstructures loose their parent crystal and
+magnetic symmetry, always being defined in P1 symmetry. So su.Atoms == su.Structure.
+
+```python
+print(su.parent.info())  # Parent structure
+su.P # superstructure matrix 
+su.superhkl2parent([h, k, l])  # index superstructure hkl with parent cell
+su.parenthkl2super([h, k, l])  # index parent hkl with supercell
+```
+
+### Multi-phase
+Scattering from different crystal structures can be compared using the MultiCrystal class:
+```python
+xtls = xtl1 + xtl2
+xtls.simulate_powder()
+```
+
+
+### Properties
+The Crystal class contains a lot of atomic properties that can be exposed in the Properties class:
+```python
+xtl.Properties.info()
+```
+
+Calculated properties include:
+ - Molecular weight
+ - Density
+ - Diamagnetic suscpetibility 
+ - x-ray absorption coefficient, attenuation length, transmission and refractive index
+ - Molecular charge balance
+ - Molecular mass fraction
+ - Atomic orbitals
+ - Magnetic exchange paths (in progress...)
+
+Properties are calulated using the atomic structure along with atomic data stored in the folder [Dans_Diffraction/data](data).
+
+
+### Multiple Scattering
+Simulations of multiple scattering at different azimuths for a particular energy can be simulated. Based on [code by Dr Gareth Nisbet](https://journals.iucr.org/a/issues/2015/01/00/td5022/).
+ [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.12866.svg)](https://doi.org/10.5281/zenodo.12866).
+
+```python
+azimuth, intensity = xtl.Scatter.ms_azimuth([h,k,l], energy_kev=8)
+```
+
+![Multiple Scattering](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/ms_azimuth_silicon.png?raw=true)
+
+
+### Graphical Front End
+![All GUI elements](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_all.png?raw=true)
+
+Start a new GUI, then select a cif file:
+```text
+$ ipython -i -m Dans_Diffraction gui
+```
+Or start the GUI from within the interactive console:
+```python
+dif.start_gui()
+```
+Using an already generated crystal:
+```python
+xtl.start_gui()
+```
+
+### Diffractometer Simulator
+![Diffractometer](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/diffractometer.png?raw=true)
+
+New in version 3.0.0. Simulate a generic detector situated around the crystal sample, with the ability to 
+control detector location shape and size and lattice orientation.
+
+
+### FDMNES functionality
+FDMNES is a powerful tool for simulating resonant x-ray diffraction, created by [Y. Joly and O. Bunau.](https://fdmnes.neel.cnrs.fr/)
+
+The Dans_Diffraction FDMNES class allows for the automatic creation of input files and simple analysis of results.
+The following command should be used to activate these features (only needs to be issued once). 
+```python
+dif.activate_fdmnes()
+```
+Once activated, the FDMNES classes become available.
+```python
+fdm = dif.Fdmnes(xtl) # Create input files and run FDMNES
+fdma = dif.FdmnesAnalysis(output_path, output_name) # Load output files and plot results
+```
+See class documentation for more information.
+
+
+Once activated, FDMNES GUI elements become available from the main window, emulating functionality of the classes.
+
+![FDMNES Run](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_08.png?raw=true)
+![FDMNES Analyse](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_09.png?raw=true)
+
+
+# Acknoledgements
+| Date       | Thanks to...                                                                            |
+|------------|-----------------------------------------------------------------------------------------|
+| 2018       | Thanks to Hepesu for help with Python3 support and ideas about breaking up calculations |
+| Dec 2019   | Thanks to Gareth Nisbet for allowing me to inlude his multiple scattering siumulation   |
+| April 2020 | Thanks to ChunHai Wang for helpful suggestions in readcif!                              |
+| May 2020   | Thanks to AndreEbel for helpful suggestions on citations                                |
+| Dec 2020   | Thanks to Chris Drozdowski for suggestions about reflection families                    |
+| Jan 2021   | Thanks to aslarsen for suggestions about outputting the structure factor                |
+| April 2021 | Thanks to Trygve RÃ¦der for suggestions about x-ray scattering factors                   |
+| Feb 2022   | Thanks to Mirko for pointing out the error in two-theta values in Scatter.powder        |
+| March 2022 | Thanks to yevgenyr for suggesting new peak profiles in Scatter.powder                   |
+| Jan 2023   | Thanks to Anuradha Vibhakar for pointing out the error in f0 + if'-if''                 |
+| Jan 2023   | Thanks to Andreas Rosnes for testing the installation in jupyterlab                     |
+| May 2023   | Thanks to Carmelo Prestipino for adding electron scattering factors                     |
+| June 2023  | Thanks to Sergio I. Rincon for pointing out the rounding error in Scatter.powder        |
+| July 2023  | Thanks to asteppke for suggested update to Arrow3D for matplotlib V>3.4                 |
+| July 2023  | Thanks to Yves Joly for helpful suggestions on FDMNES wrapper                           |
+| April 2024 | Thanks to Innbig for pointing out an issue with liquid crystal simulations              |
+| May 2024   | Thanks to paul-cares pointing out a silly spelling error in the title!                  |
+
+Copyright
+-----------------------------------------------------------------------------
+   Copyright 2024 Diamond Light Source Ltd.
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+Files in this package covered by this licence:
+* classes_crystal.py
+* classes_scattering.py
+* classes_plotting.py
+* classes_properties.py
+* classes_multicrystal.py
+* classes_orientation.py
+* classes_orbitals.py
+* functions_general.py
+* functions_plotting.py
+* functions_scattering.py
+* functions_crystallography.py
+* tkgui/*.py
+
+Other files are either covered by their own licence or not licenced for other use.
+
+| Dr Daniel G Porter | [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk) |
+| ---- | ---- |
+| [www.diamond.ac.uk](www.diamond.ac.uk) | Diamond Light Source, Chilton, Didcot, Oxon, OX11 0DE, U.K. |
```

### Comparing `Dans_Diffraction-3.0.0/README.md` & `Dans_Diffraction-3.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Dans_Diffaction
+# Dans_Diffraction
 Reads crystallographic cif files, calculates crystal properties and simulates diffraction.
 
-**Version 3.0**
+**Version 3.2**
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7725644.svg)](https://doi.org/10.5281/zenodo.7725644)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106031.svg)](https://doi.org/10.5281/zenodo.8106031)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb) 
 [![](https://img.shields.io/github/forks/DanPorter/Dans_Diffraction?label=GitHub%20Repo&style=social)](https://github.com/DanPorter/Dans_Diffraction)
 
 
 By Dan Porter, Diamond Light Source
-2023
+2024
 
 #### TL;DR:
 ```text
 $ ipython -i -m Dans_Diffraction
 OR
 $ ipython -m Dans_Diffraction gui
 ```
@@ -37,15 +37,15 @@
 
 Full code documentation available [here](https://danporter.github.io/Dans_Diffraction/).
 
 Try it out on [mybinder!](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb)
 
 For comments, queries or bugs - email [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk)
 
-**Citation:** If you use this code (great!), please cite the published DOI: [10.5281/zenodo.3859501](https://doi.org/10.5281/zenodo.3859501)
+**Citation:** If you use this code (great!), please cite the published DOI: [10.5281/zenodo.8106031](https://doi.org/10.5281/zenodo.8106031)
 
 # Installation
 **Requirements:** 
 Python 3+ with packages: *Numpy*, *Matplotlib*, *Tkinter*.
 BuiltIn packages used: *sys*, *os*, *re*, *glob*, *warnings*, *json*, *itertools*
 
 Install stable version from PyPI:
@@ -233,15 +233,15 @@
 ![Diffractometer](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/diffractometer.png?raw=true)
 
 New in version 3.0.0. Simulate a generic detector situated around the crystal sample, with the ability to 
 control detector location shape and size and lattice orientation.
 
 
 ### FDMNES functionality
-FDMNES is a powerful tool for simulating resonant x-ray diffraction, created by [Y. Joly and O. Bunau.](http://neel.cnrs.fr/spip.php?rubrique1007&lang=en)
+FDMNES is a powerful tool for simulating resonant x-ray diffraction, created by [Y. Joly and O. Bunau.](https://fdmnes.neel.cnrs.fr/)
 
 The Dans_Diffraction FDMNES class allows for the automatic creation of input files and simple analysis of results.
 The following command should be used to activate these features (only needs to be issued once). 
 ```python
 dif.activate_fdmnes()
 ```
 Once activated, the FDMNES classes become available.
@@ -266,23 +266,26 @@
 | April 2020 | Thanks to ChunHai Wang for helpful suggestions in readcif!                              |
 | May 2020   | Thanks to AndreEbel for helpful suggestions on citations                                |
 | Dec 2020   | Thanks to Chris Drozdowski for suggestions about reflection families                    |
 | Jan 2021   | Thanks to aslarsen for suggestions about outputting the structure factor                |
 | April 2021 | Thanks to Trygve Ræder for suggestions about x-ray scattering factors                   |
 | Feb 2022   | Thanks to Mirko for pointing out the error in two-theta values in Scatter.powder        |
 | March 2022 | Thanks to yevgenyr for suggesting new peak profiles in Scatter.powder                   |
-| Jan 2023  | Thanks to Anuradha Vibhakar for pointing out the error in f0 + if'-if'' |
+| Jan 2023   | Thanks to Anuradha Vibhakar for pointing out the error in f0 + if'-if''                 |
 | Jan 2023   | Thanks to Andreas Rosnes for testing the installation in jupyterlab                     |
 | May 2023   | Thanks to Carmelo Prestipino for adding electron scattering factors                     |
 | June 2023  | Thanks to Sergio I. Rincon for pointing out the rounding error in Scatter.powder        |
-
+| July 2023  | Thanks to asteppke for suggested update to Arrow3D for matplotlib V>3.4                 |
+| July 2023  | Thanks to Yves Joly for helpful suggestions on FDMNES wrapper                           |
+| April 2024 | Thanks to Innbig for pointing out an issue with liquid crystal simulations              |
+| May 2024   | Thanks to paul-cares pointing out a silly spelling error in the title!                  |
 
 Copyright
 -----------------------------------------------------------------------------
-   Copyright 2023 Diamond Light Source Ltd.
+   Copyright 2024 Diamond Light Source Ltd.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `Dans_Diffraction-3.0.0/setup.py` & `Dans_Diffraction-3.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,24 @@
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='Dans_Diffraction',
     packages=['Dans_Diffraction', 'Dans_Diffraction.tkgui'],
-    version='3.0.0',
+    version='3.2.0',
     description='Generate diffracted intensities from crystals',
     long_description_content_type='text/markdown',
     long_description=readme(),
     author='Dan Porter',
     author_email='d.g.porter@outlook.com',
     url='https://github.com/DanPorter/Dans_Diffraction',
     keywords=[
         'crystal', 'cif', 'diffraction', 'crystallography', 'science',
-        'x-ray','neutron','resonant', 'magnetic', 'magnetism', 'multiple scattering', 
+        'x-ray', 'neutron', 'resonant', 'magnetic', 'magnetism', 'multiple scattering',
         'fdmnes', 'super structure', 'spacegroup', 'space group', 'diffractometer'
         ],
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Physics',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `Dans_Diffraction-3.0.0/test/test_LS_magnetic_components.py` & `Dans_Diffraction-3.2.0/test/test_LS_magnetic_components.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_WaasKirf_xray_factors.py` & `Dans_Diffraction-3.2.0/test/test_WaasKirf_xray_factors.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_atom_properties.py` & `Dans_Diffraction-3.2.0/test/test_atom_properties.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_attenuation.py` & `Dans_Diffraction-3.2.0/test/test_attenuation.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_attenuation_length.py` & `Dans_Diffraction-3.2.0/test/test_attenuation_length.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_bmatrix.py` & `Dans_Diffraction-3.2.0/test/test_bmatrix.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_cif_files.py` & `Dans_Diffraction-3.2.0/test/test_cif_files.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_coherent_diffraction.py` & `Dans_Diffraction-3.2.0/test/test_coherent_diffraction.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_coherent_diffraction2.py` & `Dans_Diffraction-3.2.0/test/test_coherent_diffraction2.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_compare_intensity.py` & `Dans_Diffraction-3.2.0/test/test_compare_intensity.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_compare_intensity_calculation.py` & `Dans_Diffraction-3.2.0/test/test_compare_intensity_calculation.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_compound_name.py` & `Dans_Diffraction-3.2.0/test/test_compound_name.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_convolve2d.py` & `Dans_Diffraction-3.2.0/test/test_convolve2d.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_electron_density.py` & `Dans_Diffraction-3.2.0/test/test_electron_density.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_exchange_path.py` & `Dans_Diffraction-3.2.0/test/test_exchange_path.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_exchange_path2.py` & `Dans_Diffraction-3.2.0/test/test_exchange_path2.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_functions_scattering.py` & `Dans_Diffraction-3.2.0/test/test_functions_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_functions_scattering_dispersion.py` & `Dans_Diffraction-3.2.0/test/test_functions_scattering_dispersion.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_functions_scattering_new.py` & `Dans_Diffraction-3.2.0/test/test_functions_scattering_new.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_functions_scattering_pol.py` & `Dans_Diffraction-3.2.0/test/test_functions_scattering_pol.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_functions_scattering_xrm.py` & `Dans_Diffraction-3.2.0/test/test_functions_scattering_xrm.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_gaussian.py` & `Dans_Diffraction-3.2.0/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_gen_sym_mat.py` & `Dans_Diffraction-3.2.0/test/test_gen_sym_mat.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_i16_azimuth.py` & `Dans_Diffraction-3.2.0/test/test_i16_azimuth.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_intensity_grid.py` & `Dans_Diffraction-3.2.0/test/test_intensity_grid.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_isincell.py` & `Dans_Diffraction-3.2.0/test/test_isincell.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_laue_backscatter.py` & `Dans_Diffraction-3.2.0/test/test_laue_backscatter.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_nonresonant.py` & `Dans_Diffraction-3.2.0/test/test_nonresonant.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_nonresonant_plot.py` & `Dans_Diffraction-3.2.0/test/test_nonresonant_plot.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_nonresonant_sergio.py` & `Dans_Diffraction-3.2.0/test/test_nonresonant_sergio.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_parameter_plot.py` & `Dans_Diffraction-3.2.0/test/test_parameter_plot.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_plot_orbitals.py` & `Dans_Diffraction-3.2.0/test/test_plot_orbitals.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_plotintensity.py` & `Dans_Diffraction-3.2.0/test/test_plotintensity.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_plotintensity2.py` & `Dans_Diffraction-3.2.0/test/test_plotintensity2.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_readstfm.py` & `Dans_Diffraction-3.2.0/test/test_readstfm.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_refractive_index.py` & `Dans_Diffraction-3.2.0/test/test_refractive_index.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_scattering.py` & `Dans_Diffraction-3.2.0/test/test_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_supercell.py` & `Dans_Diffraction-3.2.0/test/test_supercell.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.0.0/test/test_symmetry_ops2magnetic.py` & `Dans_Diffraction-3.2.0/test/test_symmetry_ops2magnetic.py`

 * *Files identical despite different names*

