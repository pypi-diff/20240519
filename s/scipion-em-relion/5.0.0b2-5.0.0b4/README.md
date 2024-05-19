# Comparing `tmp/scipion-em-relion-5.0.0b2.tar.gz` & `tmp/scipion-em-relion-5.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-relion-5.0.0b2.tar", last modified: Tue Apr 23 11:50:25 2024, max compression
+gzip compressed data, was "scipion-em-relion-5.0.0b4.tar", last modified: Sun May 19 13:28:45 2024, max compression
```

## Comparing `scipion-em-relion-5.0.0b2.tar` & `scipion-em-relion-5.0.0b4.tar`

### file list

```diff
@@ -1,103 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:50:25.637566 scipion-em-relion-5.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-23 11:50:00.000000 scipion-em-relion-5.0.0b2/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-23 11:50:00.000000 scipion-em-relion-5.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 11:50:00.000000 scipion-em-relion-5.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-23 11:50:25.637566 scipion-em-relion-5.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-23 11:50:00.000000 scipion-em-relion-5.0.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:50:25.625566 scipion-em-relion-5.0.0b2/relion/
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-23 11:50:00.000000 scipion-em-relion-5.0.0b2/relion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-23 11:50:00.000000 scipion-em-relion-5.0.0b2/relion/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-04-23 11:50:00.000000 scipion-em-relion-5.0.0b2/relion/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:50:25.625566 scipion-em-relion-5.0.0b2/relion/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/convert30.py
--rw-r--r--   0 runner    (1001) docker     (127)    27420 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/convert31.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/convert_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/convert_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    21454 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/convert_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17428 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/dataimport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:50:25.625566 scipion-em-relion-5.0.0b2/relion/convert/mtfs/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_apollo_300_ec_stdres.star
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_apollo_300_ec_superres.star
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_de20_300.star
--rw-r--r--   0 runner    (1001) docker     (127)    19051 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_eigerX500K_100.star
--rw-r--r--   0 runner    (1001) docker     (127)    15525 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f1_300.star
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f2_300.star
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f3_200_ec.star
--rw-r--r--   0 runner    (1001) docker     (127)    45351 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f3_200_linear.star
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f3_300_ec.star
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f4_200_ec.star
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f4_300_ec.star
--rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_k2_200_ec.star
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_k2_300_ec.star
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:50:25.633566 scipion-em-relion-5.0.0b2/relion/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_assign_optic_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_autopick.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_autopick_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    23860 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_autopick_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    72076 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_bayesian_polishing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_calculate_fsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_center_averages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_classify2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_classify3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_compress_movies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_create_mask3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_crop_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)    15811 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_dynamight.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_estimate_gain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_expand_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_export_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_export_ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_export_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20875 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_extract_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_gentle_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_import_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)    18508 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_localres.py
--rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_motioncor.py
--rw-r--r--   0 runner    (1001) docker     (127)    24114 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_multibody.py
--rw-r--r--   0 runner    (1001) docker     (127)    16883 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_refine3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_remove_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_select_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_subtract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols/protocol_symmetrize_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/protocols.conf
--rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/relion_logo.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:50:25.633566 scipion-em-relion-5.0.0b2/relion/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    31770 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/templates/betagal-turorial.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:50:25.633566 scipion-em-relion-5.0.0b2/relion/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36724 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/tests/test_projection_subtraction_no_relion.py
--rw-r--r--   0 runner    (1001) docker     (127)    39097 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/tests/test_protocols_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    29462 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/tests/test_protocols_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/tests/test_protocols_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7491 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/tests/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:50:25.633566 scipion-em-relion-5.0.0b2/relion/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38984 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/viewers/viewer_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16060 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/viewers/viewer_ctfrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/viewers/viewer_locres.py
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/viewers/viewer_motioncor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/viewers/viewer_multibody.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/viewers/viewer_polishing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/viewers/viewer_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/viewers/viewer_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/relion/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:50:25.637566 scipion-em-relion-5.0.0b2/scipion_em_relion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-23 11:50:25.000000 scipion-em-relion-5.0.0b2/scipion_em_relion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-23 11:50:25.000000 scipion-em-relion-5.0.0b2/scipion_em_relion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:50:25.000000 scipion-em-relion-5.0.0b2/scipion_em_relion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 11:50:25.000000 scipion-em-relion-5.0.0b2/scipion_em_relion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 11:50:25.000000 scipion-em-relion-5.0.0b2/scipion_em_relion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 11:50:25.000000 scipion-em-relion-5.0.0b2/scipion_em_relion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:50:25.637566 scipion-em-relion-5.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-04-23 11:50:01.000000 scipion-em-relion-5.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:45.902613 scipion-em-relion-5.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-19 13:28:45.902613 scipion-em-relion-5.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:45.886613 scipion-em-relion-5.0.0b4/relion/
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:45.890612 scipion-em-relion-5.0.0b4/relion/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/convert30.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27420 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/convert31.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/convert_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/convert_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21454 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/convert_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/dataimport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:45.890612 scipion-em-relion-5.0.0b4/relion/convert/mtfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_apollo_300_ec_stdres.star
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_apollo_300_ec_superres.star
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_de20_300.star
+-rw-r--r--   0 runner    (1001) docker     (127)    19051 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_eigerX500K_100.star
+-rw-r--r--   0 runner    (1001) docker     (127)    15525 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f1_300.star
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f2_300.star
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f3_200_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)    45351 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f3_200_linear.star
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f3_300_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f4_200_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f4_300_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_k2_200_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_k2_300_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:45.898613 scipion-em-relion-5.0.0b4/relion/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_assign_optic_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_autopick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_autopick_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23860 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_autopick_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72430 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_bayesian_polishing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_calculate_fsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_center_averages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_classify2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_classify3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_compress_movies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_create_mask3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_crop_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15811 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16037 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_dynamight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_estimate_gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_expand_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_export_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_export_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_export_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20875 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_extract_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_gentle_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18508 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_localres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_motioncor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24029 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_multibody.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16883 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_refine3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_remove_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_select_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols/protocol_symmetrize_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/relion_logo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:45.898613 scipion-em-relion-5.0.0b4/relion/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    32481 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/templates/betagal-turorial.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:45.898613 scipion-em-relion-5.0.0b4/relion/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36724 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/tests/test_projection_subtraction_no_relion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40368 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/tests/test_protocols_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29462 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/tests/test_protocols_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/tests/test_protocols_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7622 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:45.902613 scipion-em-relion-5.0.0b4/relion/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38984 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/viewers/viewer_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16060 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/viewers/viewer_ctfrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/viewers/viewer_locres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/viewers/viewer_motioncor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/viewers/viewer_multibody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/viewers/viewer_polishing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/viewers/viewer_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/viewers/viewer_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/relion/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:45.902613 scipion-em-relion-5.0.0b4/scipion_em_relion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-19 13:28:45.000000 scipion-em-relion-5.0.0b4/scipion_em_relion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-19 13:28:45.000000 scipion-em-relion-5.0.0b4/scipion_em_relion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:28:45.000000 scipion-em-relion-5.0.0b4/scipion_em_relion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 13:28:45.000000 scipion-em-relion-5.0.0b4/scipion_em_relion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 13:28:45.000000 scipion-em-relion-5.0.0b4/scipion_em_relion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 13:28:45.000000 scipion-em-relion-5.0.0b4/scipion_em_relion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:28:45.902613 scipion-em-relion-5.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-19 13:28:21.000000 scipion-em-relion-5.0.0b4/setup.py
```

### Comparing `scipion-em-relion-5.0.0b2/CHANGES.txt` & `scipion-em-relion-5.0.0b4/CHANGES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 5.0.0:
     - add Relion 5.0 support, removed 3.x support
     - fix gpu param value
     - float16=True by default
     - several fixes in the viewers
+    - import coordinates protocol moved to the pwem core pligin
+    - bugfix for finding optimiser file after gentle project cleaning
+    - mew protocol: DynaMight flexibility
 4.0.20: fix FSC viewer: Do not show empty figure when closing.
 4.0.19: fix adding more coords to the output of import coords protocol
 4.0.18: add ewald params to the reconstruct protocol
 4.0.17: add missing CUDA_BIN env var
 4.0.16: Remove direct pointer from class3d protocol
 4.0.15: Extending the conversion of incompatibles formats (Yunior)
 4.0.14: 2D class ranker improvements (JMRT)
```

### Comparing `scipion-em-relion-5.0.0b2/LICENSE` & `scipion-em-relion-5.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/PKG-INFO` & `scipion-em-relion-5.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-relion
-Version: 5.0.0b2
+Version: 5.0.0b4
 Summary: Plugin to use Relion programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-relion
 Author: Grigory Sharov, J.M. De la Rosa Trevin, Josue Gomez Blanco
 Author-email: gsharov@mrc-lmb.cam.ac.uk, delarosatrevin@scilifelab.se, josue.gomez-blanco@mcgill.ca
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-relion/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-relion/
@@ -102,16 +102,15 @@
         * ctf refinement
         * DynaMight flexibility
         * estimate gain to compress
         * expand symmetry
         * export coordinates
         * export ctf                
         * export particles
-        * import coordinates
-        * local resolution          
+        * local resolution
         * motion correction
         * particles extraction
         * post-processing           
         * preprocess particles      
         * reconstruct
         * remove preferential views
         * subtract projection
```

### Comparing `scipion-em-relion-5.0.0b2/README.rst` & `scipion-em-relion-5.0.0b4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,15 @@
 * ctf refinement
 * DynaMight flexibility
 * estimate gain to compress
 * expand symmetry
 * export coordinates
 * export ctf                
 * export particles
-* import coordinates
-* local resolution          
+* local resolution
 * motion correction
 * particles extraction
 * post-processing           
 * preprocess particles      
 * reconstruct
 * remove preferential views
 * subtract projection
```

### Comparing `scipion-em-relion-5.0.0b2/relion/__init__.py` & `scipion-em-relion-5.0.0b4/relion/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import pyworkflow.utils as pwutils
 from pyworkflow import Config
 import pwem
 
 from .constants import *
 
 
-__version__ = '5.0.0b2'
+__version__ = '5.0.0b4'
 _logo = "relion_logo.jpg"
 _references = ['Scheres2012a', 'Scheres2012b', 'Kimanius2016',
                'Zivanov2018', 'Kimanius2021']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = RELION_HOME
```

### Comparing `scipion-em-relion-5.0.0b2/relion/bibtex.py` & `scipion-em-relion-5.0.0b4/relion/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/constants.py` & `scipion-em-relion-5.0.0b4/relion/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/__init__.py` & `scipion-em-relion-5.0.0b4/relion/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/convert30.py` & `scipion-em-relion-5.0.0b4/relion/convert/convert30.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/convert31.py` & `scipion-em-relion-5.0.0b4/relion/convert/convert31.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/convert_base.py` & `scipion-em-relion-5.0.0b4/relion/convert/convert_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/convert_coordinates.py` & `scipion-em-relion-5.0.0b4/relion/convert/convert_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/convert_deprecated.py` & `scipion-em-relion-5.0.0b4/relion/convert/convert_deprecated.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/convert_utils.py` & `scipion-em-relion-5.0.0b4/relion/convert/convert_utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/dataimport.py` & `scipion-em-relion-5.0.0b4/relion/convert/dataimport.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,16 +32,17 @@
 
 from pyworkflow.object import Float
 from pwem.constants import ALIGN_PROJ, ALIGN_2D, ALIGN_NONE
 from pwem.objects import Micrograph
 import pwem.emlib.metadata as md
 import pyworkflow.utils as pwutils
 
-from .convert31 import OpticsGroups
-from .convert_utils import relionToLocation
+from relion import convert
+from relion.convert.convert31 import OpticsGroups
+from relion.convert.convert_utils import relionToLocation
 
 
 class FileTransform:
     """ Simple classes to handle input files.
     This classes will create a destination folder from which the input files
     will be accessible. The destination folder can be a symlink if the files
     are not required to be copied.
@@ -413,12 +414,37 @@
                 acquisitionDict['samplingRate'] = acqRow.rlnImagePixelSize
 
         except Exception as ex:
             logger.error(f"Error loading acquisition: {str(ex)}")
 
         return acquisitionDict
 
-    def importCoordinates(self, fileName, addCoordinate):
-        from .convert_deprecated import rowToCoordinate
-        for row in md.iterRows(fileName):
-            coord = rowToCoordinate(row)
-            addCoordinate(coord)
+    def importCoordinates(self):
+        prot = self.protocol  # shortcut
+        inputMics = prot.inputMicrographs
+        micList = [pwutils.removeExt(mic.getMicName()) for mic in inputMics.get()]
+        coordsSet = prot._createSetOfCoordinates(inputMics)
+
+        if len(prot.getMatchFiles()) == 1:  # particles.star file
+            for coordFile, _ in prot.iterFiles():
+                reader = convert.createReader()
+                reader.readSetOfCoordinates(
+                    coordFile, coordsSet, micList,
+                    postprocessCoordRow=self._postprocessCoordRow)
+                break
+        else:  # multiple star files with coords
+            from .convert_deprecated import rowToCoordinate
+            for coordFile, fileId in prot.iterFiles():
+                mic = prot.getMatchingMic(coordFile, fileId)
+                if mic is not None:
+                    # Parse the coordinates in the given format for this micrograph
+                    for row in md.iterRows(coordFile):
+                        coord = rowToCoordinate(row)
+                        coord.setMicrograph(mic)
+                        self._postprocessCoordRow(coord, row)
+                        coordsSet.append(coord)
+
+        return coordsSet
+
+    # -------------------------- UTILS functions ------------------------------
+    def _postprocessCoordRow(self, coord, row):
+        self.protocol.correctCoordinatePosition(coord)
```

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_apollo_300_ec_stdres.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_apollo_300_ec_stdres.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_apollo_300_ec_superres.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_apollo_300_ec_superres.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_de20_300.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_de20_300.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_eigerX500K_100.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_eigerX500K_100.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f1_300.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f1_300.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f2_300.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f2_300.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f3_200_ec.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f3_200_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f3_200_linear.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f3_200_linear.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f3_300_ec.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f3_300_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f4_200_ec.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f4_200_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_f4_300_ec.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_f4_300_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_k2_200_ec.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_k2_200_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/convert/mtfs/mtf_k2_300_ec.star` & `scipion-em-relion-5.0.0b4/relion/convert/mtfs/mtf_k2_300_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/objects.py` & `scipion-em-relion-5.0.0b4/relion/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/__init__.py` & `scipion-em-relion-5.0.0b4/relion/protocols/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,22 @@
 from .protocol_ctf_refinement import ProtRelionCtfRefinement
 from .protocol_expand_symmetry import ProtRelionExpandSymmetry
 from .protocol_export_coords import ProtRelionExportCoordinates
 from .protocol_export_ctf import ProtRelionExportCtf
 from .protocol_export_particles import ProtRelionExportParticles
 from .protocol_extract_particles import ProtRelionExtractParticles
 from .protocol_gentle_clean import ProtRelionCleanJobs
-from .protocol_import_coords import ProtRelionImportCoords
 from .protocol_initialmodel import ProtRelionInitialModel
 from .protocol_localres import ProtRelionLocalRes
 from .protocol_motioncor import ProtRelionMotioncor
 from .protocol_multibody import ProtRelionMultiBody
 from .protocol_postprocess import ProtRelionPostprocess
 from .protocol_preprocess import ProtRelionPreprocessParticles
 from .protocol_reconstruct import ProtRelionReconstruct
 from .protocol_refine3d import ProtRelionRefine3D
 from .protocol_remove_views import ProtRelionRemovePrefViews
 from .protocol_select_classes import ProtRelionSelectClasses2D
 from .protocol_subtract import ProtRelionSubtract
 from .protocol_symmetrize_volume import ProtRelionSymmetrizeVolume
 
-#if Plugin.IS_GT50():
-#    from .protocol_dynamight import ProtRelionDynaMight
+if Plugin.IS_GT50():
+    from .protocol_dynamight import ProtRelionDynaMight
```

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_assign_optic_groups.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_assign_optic_groups.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_autopick.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_autopick.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_autopick_log.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_autopick_log.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_autopick_ref.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_autopick_ref.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_base.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
             'optimiser': self.extraIter + 'optimiser.star',
             'angularDist_xmipp': self.extraIter + 'angularDist_xmipp.xmd',
             'all_avgPmax': self._getPath('iterations_avgPmax.star'),
             'all_changes': self._getPath('iterations_changes.star'),
             'selected_volumes': self._getPath('selected_volumes_xmipp.xmd'),
             'dataFinal': self._getExtraPath("relion_data.star"),
             'modelFinal': self._getExtraPath("relion_model.star"),
+            'optimiserFinal': self._getExtraPath("relion_optimiser.star"),
             'finalvolume': self._getExtraPath("relion_class%(ref3d)03d.mrc"),
             'final_half1_volume': self._getExtraPath("relion_half1_class%(ref3d)03d_unfil.mrc"),
             'final_half2_volume': self._getExtraPath("relion_half2_class%(ref3d)03d_unfil.mrc"),
             'finalSGDvolume': self._getExtraPath("relion_it%(iter)03d_class%(ref3d)03d.mrc"),
             'preprocess_particles': self._getPath("preprocess_particles.mrcs"),
             'preprocess_particles_star': self._getPath("preprocess_particles.star"),
             'preprocess_particles_prefix': "preprocess_particles",
@@ -1246,14 +1247,23 @@
 
     def _getnumberOfIters(self):
         if self.IS_2D and self.useGradientAlg:
             return self._getContinueIter() + self.numberOfVDAMBatches.get()
         else:
             return self._getContinueIter() + self.numberOfIterations.get()
 
+    def _getOptimiserFile(self):
+        lastIter = self._lastIter()
+        if lastIter is not None:
+            fnOptimiser = self._getFileName('optimiser', iter=lastIter)
+        else:
+            fnOptimiser = self._getFileName('optimiserFinal')
+
+        return fnOptimiser
+
     def _getReferenceVolumes(self):
         """ Return a list with all input references.
         (Could be one or more volumes).
         """
         inputObj = self.referenceVolume.get()
 
         if isinstance(inputObj, Volume):
```

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_bayesian_polishing.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_bayesian_polishing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_calculate_fsc.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_calculate_fsc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_center_averages.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_center_averages.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_classify2d.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_classify2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_classify3d.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_classify3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_compress_movies.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_compress_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_create_mask3d.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_create_mask3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_crop_resize.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_crop_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_ctf_refinement.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_dynamight.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_dynamight.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,23 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 import os.path
+from glob import glob
 from typing import List
 
 import pyworkflow.protocol.params as params
 from pyworkflow.constants import NEW
+import pyworkflow.utils as pwutils
 from pwem.protocols import ProtAnalysis3D
 from pwem.constants import ALIGN_PROJ
+from pwem.objects import SetOfVolumes, Volume
 
 from relion import Plugin
 import relion.convert as convert
 from relion.protocols.protocol_base import ProtRelionBase
 
 
 class ProtRelionDynaMight(ProtAnalysis3D, ProtRelionBase):
@@ -47,15 +50,15 @@
     It also implements functionality to calculate a pseudo-inverse 3D deformation
     field that can then be used in a deformed weighted backprojection algorithm
     to obtain an improved 3D reconstruction of the consensus structure.
 
     """
     _label = 'DynaMight flexibility'
     _devStatus = NEW
-    _possibleOutputs = {}
+    _possibleOutputs = {"Volumes": SetOfVolumes}
     IS_CLASSIFY = False
 
     @classmethod
     def isDisabled(cls):
         return not Plugin.IS_GT50()
 
     def _initialize(self):
@@ -130,15 +133,16 @@
                            "and for deformed backprojection. This will speed up "
                            "the calculations, but you need to make sure you have "
                            "enough RAM to do so.")
 
         form.addSection(label='Tasks', condition='doContinue')
         form.addParam('continueMsg', params.LabelParam,
                       condition='not doContinue',
-                      label='Tasks are not available outside of continue mode')
+                      label='Tasks are not available outside of continue mode. '
+                            'Choose a previous run to analyze.')
 
         group = form.addGroup('Visualize')
         group.addParam('doVisualize', params.BooleanParam, default=False,
                        condition='doContinue',
                        label="Do visualization?",
                        help="If set to Yes, dynamight will be run to visualize "
                             "the latent space and deformed models. One can also "
@@ -149,39 +153,31 @@
                        label="Half-set to visualize",
                        help="Select halfset 1 or 2 to explore the latent space "
                             "of that halfset. If you select halfset 0, then the "
                             "validation set is being visualised, which will give "
                             "you an estimate of the errors in the deformations.")
 
         group = form.addGroup('Deformations')
-        group.addParam('doDeformEstimate', params.BooleanParam, default=False,
+        group.addParam('doDeform', params.BooleanParam, default=False,
                        condition='doContinue',
-                       label="Do inverse-deformation estimation?",
+                       label="Estimate inverse deformation and backproject?",
                        help="If set to Yes, dynamight will be run to estimate "
-                            "inverse-deformations. These are necessary if one "
-                            "want to perform deformed backprojection to calculate "
+                            "inverse-deformations first. These are necessary "
+                            "to perform deformed backprojection to calculate "
                             "an improved consensus model.")
         group.addParam('numEpochs', params.IntParam, default=200,
-                       condition='doContinue and doDeformEstimate',
+                       condition='doContinue and doDeform',
                        label="Number of epochs to perform",
                        help="Number of epochs to perform inverse deformations. "
                             "You can monitor the convergence of the loss "
                             "function to assess how many are necessary. "
-                            "Often 200 are enough")
+                            "Often 200 are enough.")
 
-        group = form.addGroup('Backprojection')
-        group.addParam('doDeformBackProj', params.BooleanParam, default=False,
-                       condition='doContinue',
-                       label="Do deformed backprojection?",
-                       help="If set to Yes, dynamight will be run to perform "
-                            "a deformed backprojection, using "
-                            "inverse-deformations from a previous task, to "
-                            "get an improved consensus reconstruction.")
         group.addParam('batchSize', params.IntParam, default=10,
-                       condition='doContinue and doDeformBackProj',
+                       condition='doContinue and doDeform',
                        label="Backprojection batchsize",
                        help="Number of images to process in parallel. "
                             "This will speed up the calculation, but will "
                             "cost GPU memory. Try how high you can go on "
                             "your GPU, given your box size and size of the "
                             "neural network.")
 
@@ -191,28 +187,27 @@
     def _insertAllSteps(self):
         self._createFilenameTemplates()
 
         if not self.doContinue:
             self._insertFunctionStep(self.convertInputStep)
             self._insertFunctionStep(self.runDynamightStep)
         else:
-            self._insertFunctionStep(self.runTasksStep)
-
-        #self._insertFunctionStep(self.createOutputStep)
+            self.runTasks()
+            self._insertFunctionStep(self.createOutputStep)
 
     # -------------------------- STEPS functions ------------------------------
     def _createFilenameTemplates(self):
         """ Centralize how files are called for iterations and references. """
         deform_path = "forward_deformations/checkpoints"
         myDict = {
             'input_particles': self._getExtraPath('input_particles.star'),
             'checkpoint_iter': self._getExtraPath(deform_path,
                                                   '%(iter)03d.pth'),
             'checkpoint_final': self._getExtraPath(deform_path,
-                                                   'checkpoint_final.pth'),
+                                                   'checkpoint_final.pth')
             }
         self._updateFilenamesDict(myDict)
 
     def convertInputStep(self, *args):
         """ Create the input file in STAR format as expected by Relion.
         If the input particles comes from Relion, just link the file.
         """
@@ -237,60 +232,93 @@
             f"--n-threads {self.numberOfThreads}",
             f"--gpu-id {self.gpuList.get()}",
             "--preload-images" if self.allParticlesRam else ""
         ]
 
         self.runProgram(params)
 
-    def runTasksStep(self):
+    def runTasks(self):
         inputProt = self.continueRun.get()
-        inputProt._createFilenameTemplates()
-        checkpoint_file = inputProt._getFileName('checkpoint_final')
+        pwutils.createLink(inputProt._getExtraPath("forward_deformations"),
+                           self._getExtraPath("forward_deformations"))
+        checkpoint_file = self._getFileName('checkpoint_final')
 
         if self.doVisualize:
             params = [
                 "explore-latent-space",
                 self._getExtraPath(),
                 f"--half-set {self.halfSet.get()}",
                 f"--checkpoint-file {checkpoint_file}",
                 f"--gpu-id {self.gpuList.get()}"
             ]
-        elif self.doDeformEstimate:
+            self._insertFunctionStep(self.runTaskStep, params)
+
+        elif self.doDeform:
+            # Estimate inverse deformations
             params = [
                 "optimize-inverse-deformations",
                 self._getExtraPath(),
                 f"--n-epochs {self.numEpochs.get()}",
                 f"--checkpoint-file {checkpoint_file}",
                 f"--gpu-id {self.gpuList.get()}",
                 "--preload-images" if self.allParticlesRam else ""
             ]
+            self._insertFunctionStep(self.runTaskStep, params)
 
-        elif self.doDeformBackProj:
+            # Backproject
             params = [
                 "deformable-backprojection",
                 self._getExtraPath(),
                 f"--batch-size {self.batchSize.get()}",
                 f"--checkpoint-file {checkpoint_file}",
                 f"--gpu-id {self.gpuList.get()}",
                 "--preload-images"
             ]
-        else:
-            raise ValueError("Unrecognized task")
+            self._insertFunctionStep(self.runTaskStep, params)
 
+    def runTaskStep(self, params: List[str]):
+        """ Run the actual job. """
         self.runProgram(params)
 
+    def createOutputStep(self):
+        parts = self._getInputParticles()
+        if self.doVisualize:
+            output = self._getExtraPath("maps", "map???_half?.mrc")
+        elif self.doDeform:
+            output = self._getExtraPath("backprojection", "map_half?.mrc")
+
+        files = sorted(glob(output))
+        if files:
+            volumes = self._createSetOfVolumes()
+            volumes.setSamplingRate(parts.getSamplingRate())
+
+            for i, volFn in enumerate(files):
+                vol = Volume()
+                vol.setFileName(volFn)
+                if self.doDeform:
+                    vol.setObjLabel(f"half-map {i+1}")
+                volumes.append(vol)
+
+            self._defineOutputs(Volumes=volumes)
+            self._defineSourceRelation(parts, volumes)
+
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
-        return []
+        summary = []
+        if self.isFinished() and hasattr(self, "Volumes"):
+            if self.doVisualize:
+                summary.append("Movies/maps generated along the deformation trajectory")
+            else:
+                summary.append("Half-maps generated by inverse deformation")
+
+        return summary
 
     def _validate(self):
         errors = []
-        tasks = [self.doVisualize.get(),
-                 self.doDeformEstimate.get(),
-                 self.doDeformBackProj.get()]
+        tasks = [self.doVisualize.get(), self.doDeform.get()]
 
         if tasks.count(True) > 1:
             errors.append("You cannot select multiple tasks")
 
         if self.doContinue:
             inputProt = self.continueRun.get()
             inputProt._createFilenameTemplates()
```

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_estimate_gain.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_estimate_gain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_expand_symmetry.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_expand_symmetry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_export_coords.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_export_coords.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_export_ctf.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_export_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_export_particles.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_export_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_extract_particles.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_extract_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_gentle_clean.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_gentle_clean.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,17 @@
                       label="Gentle clean procedure will move all "
                             "intermediate files from finished Relion "
                             "protocols to Trash folder. For iteration-based "
                             "jobs, only the last iteration files are kept.")
 
     # --------------------------- INSERT steps functions ----------------------
     def _insertAllSteps(self):
-        self._insertFunctionStep("findRelionProtsStep")
-        self._insertFunctionStep("runCleanStep")
-        self._insertFunctionStep('createOutputStep')
+        self._insertFunctionStep(self.findRelionProtsStep)
+        self._insertFunctionStep(self.runCleanStep)
+        self._insertFunctionStep(self.createOutputStep)
 
     # --------------------------- STEPS functions -----------------------------
     def findRelionProtsStep(self):
         project = self.getProject()
         runs = project.getRuns()
         prjPath = os.path.abspath(project.getPath())
 
@@ -86,26 +86,28 @@
             self.info("Found the following folders:\n")
             for k, v in protDict.items():
                 self.info("%s: %s" % (k, v))
         else:
             return
 
         fnsTemplate = {
-            'ProtRelionExtractParticles': ['../micrographs_*.star'],
-            'ProtRelionPostProcess': ['*masked.mrc'],
-            'ProtRelionMotionCor': ['*corrected_micrographs.star',
+            'ProtRelionExtractParticles': ['micrographs_*.star'],
+            'ProtRelionPostprocess': ['*.eps'],
+            'ProtRelionMotioncor': ['*corrected_micrographs.star',
                                     '*.log',
                                     '*.TXT'],
             'ProtRelionBayesianPolishing': ['*_FCC_cc.mrc',
                                             '*_FCC_w0.mrc',
-                                            '*_FCC_w1.mrc'],
+                                            '*_FCC_w1.mrc',
+                                            '*.eps',
+                                            '*_shiny.star',
+                                            '*_tracks.star'],
             'ProtRelionCtfRefinement': ['*_wAcc_optics-group*.mrc',
                                         '*_xyAcc_optics-group*.mrc',
                                         '*_aberr-Axx_optics-group_*.mrc',
-                                        '*_aberr-Axx_optics-group_*.mrc',
                                         '*_aberr-Axy_optics-group_*.mrc',
                                         '*_aberr-Ayy_optics-group_*.mrc',
                                         '*_aberr-bx_optics-group_*.mrc',
                                         '*_aberr-by_optics-group_*.mrc',
                                         '*_mag_optics-group_*.mrc',
                                         '*_fit.star', '*_fit.eps'],
         }
@@ -126,15 +128,15 @@
                     self.debug(files)
                     result = None
                     if files:
                         s = re.search(r"_?t(\d{3})_", files[-1])
                         if s:
                             # group 1 is 3 digits iteration number
                             result = "relion_[ic]t%03d_" % int(s.group(1))
-                            self.info("I'll keep files: %s from %s" % (result, protDir))
+                            self.info(f"I'll keep files: {os.path.join(protDir, result)}*")
                     if result:
                         for f in files:
                             match = re.search(result, f)
                             if not match:
                                 self.moveDict[os.path.join(prjPath, protDir, f)] = os.path.join(prjPath, "Trash", protDir)
 
     def runCleanStep(self):
```

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_initialmodel.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_initialmodel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_localres.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_localres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_motioncor.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_motioncor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_multibody.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_multibody.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,16 +419,15 @@
             fnOptimiser = protRefine._getFileName('optimiser',
                                                   iter=continueIter)
 
             if protRefine.recSubtractedBodies:
                 args['--reconstruct_subtracted_bodies'] = ''
 
         else:
-            fnOptimiser = protRefine._getFileName('optimiser',
-                                                  iter=protRefine._lastIter())
+            fnOptimiser = protRefine._getOptimiserFile()
             args.update({
                 '--multibody_masks': self._getExtraPath('input_body.star'),
                 '--solvent_correct_fsc': '',
                 '--oversampling': 1,
                 '--pad': 1 if self.skipPadding else 2,
                 '--healpix_order': self.initialAngularSampling.get(),
                 '--auto_local_healpix_order': self.initialAngularSampling.get(),
```

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_postprocess.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_postprocess.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_preprocess.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_preprocess.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_reconstruct.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_reconstruct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_refine3d.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_refine3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_remove_views.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_remove_views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_select_classes.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_select_classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,16 +78,15 @@
         self._insertFunctionStep('runSelectStep')
         self._insertFunctionStep('createOutputStep')
 
     # --------------------------- STEPS functions -----------------------------
     def runSelectStep(self):
         inputProt = self.inputProtocol.get()
         inputProt._initialize()
-        fnOptimiser = inputProt._getFileName('optimiser',
-                                             iter=inputProt._lastIter())
+        fnOptimiser = inputProt._getOptimiserFile()
         params = " --opt %s --o %s --min_score %s" % (fnOptimiser,
                                                       self._getExtraPath(),
                                                       self.minThreshold.get())
         params += " --fn_sel_parts particles.star"
         params += " --fn_sel_classavgs class_averages.star"
         params += " --fn_root rank --do_granularity_features"
         params += " --auto_select"
```

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_subtract.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_subtract.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
                            'of each CTF onward. This can be useful if the CTF '
                            'model is inadequate at the lowest resolution. '
                            'Still, in general using higher amplitude contrast '
                            'on the CTFs (e.g. 10-20%) often yields better '
                            'results. Therefore, this option is not generally '
                            'recommended.')
 
-        form.addParallelSection(threads=0, mpi=1)
+        form.addParallelSection(threads=0, mpi=2)
     
     # -------------------------- INSERT steps functions -----------------------
     def _insertAllSteps(self):
         self.isRelionInput = self.relionInput.get()
         self._initialize()
 
         if not self.useAll or not self.isRelionInput:
@@ -241,16 +241,16 @@
             self._getFileName('output_star').replace(".star", ""))
 
         self.runJob('relion_project', params)
 
     def subtractStepRelion(self):
         inputProt = self.inputProtocol.get()
         inputProt._initialize()
-        fnOptimiser = inputProt._getFileName('optimiser',
-                                             iter=inputProt._lastIter())
+
+        fnOptimiser = inputProt._getOptimiserFile()
         params = " --i %s --o %s --new_box %s" % (fnOptimiser,
                                                   self._getExtraPath(),
                                                   self.newBoxSize.get())
 
         if not self.useAll:
             params += " --data %s" % self._getFileName('input_star')
         if self.centerOnMask:
```

### Comparing `scipion-em-relion-5.0.0b2/relion/protocols/protocol_symmetrize_volume.py` & `scipion-em-relion-5.0.0b4/relion/protocols/protocol_symmetrize_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/relion_logo.jpg` & `scipion-em-relion-5.0.0b4/relion/relion_logo.jpg`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/templates/betagal-turorial.json.template` & `scipion-em-relion-5.0.0b4/relion/templates/betagal-turorial.json.template`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-A complete tutorial using Relion 4 within Scipion. The workflow follows betagal Relion tutorial.
+A complete tutorial using Relion 5 within Scipion. The workflow follows betagal Relion tutorial.
 [
     {
         "object.className": "ProtImportMovies",
         "object.id": "2",
         "object.label": "pwem - import movies",
         "object.comment": "",
         "_useQueue": false,
@@ -47,35 +47,37 @@
         "object.label": "motioncorr - movie alignment",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
-        "gpuList": "0 1",
+        "inputMovies": "2.outputMovies",
         "doSaveAveMic": true,
         "useAlignToSum": true,
         "alignFrame0": 1,
         "alignFrameN": 24,
         "binFactor": 1.0,
         "cropOffsetX": 0,
         "cropOffsetY": 0,
         "cropDimX": 0,
         "cropDimY": 0,
         "splitEvenOdd": false,
         "doSaveMovie": false,
         "doComputePSD": false,
         "doComputeMicThumbnail": false,
         "extraProtocolParams": "",
+        "gpuList": "0 1",
         "doApplyDoseFilter": true,
         "patchX": 5,
         "patchY": 5,
         "patchOverlap": 0,
         "group": 1,
-        "tol": 0.5,
+        "groupLocal": 4,
+        "tol": 0.2,
         "doSaveUnweightedMic": false,
         "extraParams2": "",
         "gainRot": 0,
         "gainFlip": 0,
         "defectFile": null,
         "defectMap": null,
         "EERtext": null,
@@ -83,30 +85,30 @@
         "eerSampling": 0,
         "doMagCor": false,
         "scaleMaj": 1.0,
         "scaleMin": 1.0,
         "angDist": 0.0,
         "hostName": "localhost",
         "numberOfThreads": 3,
-        "numberOfMpi": 1,
-        "inputMovies": "2.outputMovies"
+        "numberOfMpi": 1
     },
     {
         "object.className": "CistemProtCTFFind",
-        "object.id": "195",
-        "object.label": "cistem - ctffind4",
+        "object.id": "196",
+        "object.label": "cistem - ctffind",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "recalculate": false,
         "sqliteFile": null,
         "inputType": 1,
+        "inputMicrographs": "88.outputMicrographsDoseWeighted",
         "avgFrames": 3,
         "usePowerSpectra": false,
         "windowSize": 512,
         "lowRes": 30.0,
         "highRes": 5.0,
         "minDefocus": 5000.0,
         "maxDefocus": 50000.0,
@@ -119,83 +121,83 @@
         "maxPhaseShift": 180.0,
         "stepPhaseShift": 10.0,
         "hostName": "localhost",
         "numberOfThreads": 8,
         "numberOfMpi": 1,
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
-        "streamingBatchSize": 8,
-        "inputMicrographs": "88.outputMicrographsDoseWeighted"
+        "streamingBatchSize": 8
     },
     {
         "object.className": "ProtRelionAutopickLoG",
-        "object.id": "259",
+        "object.id": "260",
         "object.label": "relion - auto-picking LoG",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputMicrographs": "88.outputMicrographsDoseWeighted",
         "boxSize": 100,
         "minDiameter": 150,
         "maxDiameter": 180,
         "areParticlesWhite": false,
         "maxResolution": 20.0,
         "threshold": 0.0,
         "threshold2": 5.0,
         "extraParams": "",
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
-        "streamingBatchSize": 8,
+        "streamingBatchSize": 0,
         "hostName": "localhost",
-        "numberOfMpi": 4,
-        "inputMicrographs": "88.outputMicrographsDoseWeighted"
+        "numberOfMpi": 4
     },
     {
         "object.className": "ProtRelionExtractParticles",
-        "object.id": "322",
-        "object.label": "relion - particles extraction 64",
+        "object.id": "310",
+        "object.label": "relion - particles extraction 64px",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputCoordinates": "260.outputCoordinates",
         "downsampleType": 0,
+        "ctfRelations": "196.outputCTF",
         "boxSize": 256,
         "doRescale": true,
         "rescaledSize": 64,
-        "saveFloat16": false,
+        "saveFloat16": true,
         "doInvert": true,
         "doNormalize": true,
         "backDiameter": 200,
         "stddevWhiteDust": -1.0,
         "stddevBlackDust": -1.0,
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
         "streamingBatchSize": 0,
         "hostName": "localhost",
-        "numberOfMpi": 4,
-        "ctfRelations": "195.outputCTF",
-        "inputCoordinates": "259.outputCoordinates"
+        "numberOfMpi": 4
     },
     {
         "object.className": "ProtRelionClassify2D",
-        "object.id": "391",
+        "object.id": "380",
         "object.label": "relion - 2D classification",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "isClassify": true,
         "is2D": true,
         "doContinue": false,
+        "inputParticles": "310.outputParticles",
         "copyAlignment": false,
         "alignmentAsPriors": false,
         "fillRandomSubset": true,
         "maskDiameterA": 200,
         "maskZero": 0,
         "continueIter": "last",
         "continueMsg": "True",
@@ -214,53 +216,55 @@
         "limitResolEStep": -1.0,
         "doImageAlignment": true,
         "inplaneAngularSamplingDeg": 6.0,
         "offsetSearchRangePix": 5.0,
         "offsetSearchStepPix": 1.0,
         "allowCoarserSampling": false,
         "useParallelDisk": true,
-        "pooledParticles": 3,
-        "allParticlesRam": false,
+        "pooledParticles": 30,
+        "allParticlesRam": true,
         "scratchDir": null,
         "combineItersDisc": false,
         "doGpu": true,
         "gpusToUse": "",
         "oversampling": 1,
         "extraParams": "",
         "hostName": "localhost",
         "numberOfThreads": 4,
-        "numberOfMpi": 5,
-        "inputParticles": "322.outputParticles"
+        "numberOfMpi": 5
     },
     {
         "object.className": "ProtUserSubSet",
-        "object.id": "473",
-        "object.label": "create subset for picking",
+        "object.id": "462",
+        "object.label": "create subset",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
-        "other": "371",
-        "sqliteFile": "Runs/000391_ProtRelionClassify2D/classes2D_state.sqlite,",
-        "outputClassName": "SetOfAverages,Representatives",
-        "inputObject": "391."
+        "inputObject": "380.",
+        "other": "359",
+        "sqliteFile": "Runs/000380_ProtRelionClassify2D/classes2D_state.sqlite,",
+        "outputClassName": "SetOfAverages,Representatives"
     },
     {
         "object.className": "ProtRelion2Autopick",
-        "object.id": "528",
-        "object.label": "relion - auto-picking ref-based",
+        "object.id": "518",
+        "object.label": "relion - auto-picking reference-based",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputMicrographs": "88.outputMicrographsDoseWeighted",
+        "ctfRelations": "196.outputCTF",
         "referencesType": 0,
+        "inputReferences": "462.outputRepresentatives",
         "symmetryGroup": "c1",
         "angularSamplingDeg": 0,
         "lowpassFilterRefs": 20,
         "highpassFilterMics": -1,
         "angularSampling": 5,
         "refsHaveInvertedContrast": true,
         "refsCtfCorrected": true,
@@ -273,60 +277,58 @@
         "doGpu": true,
         "gpusToUse": "",
         "extraParams": "",
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
         "streamingBatchSize": 0,
         "hostName": "localhost",
-        "numberOfMpi": 1,
-        "inputMicrographs": "88.outputMicrographsDoseWeighted",
-        "ctfRelations": "195.outputCTF",
-        "inputReferences": "473.outputRepresentatives"
+        "numberOfMpi": 1
     },
     {
         "object.className": "ProtRelionExtractParticles",
-        "object.id": "593",
-        "object.label": "relion - particles extraction 64",
+        "object.id": "583",
+        "object.label": "relion - particles extraction 64px #2",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputCoordinates": "518.outputCoordinates",
         "downsampleType": 0,
+        "ctfRelations": "196.outputCTF",
         "boxSize": 256,
         "doRescale": true,
         "rescaledSize": 64,
-        "saveFloat16": false,
+        "saveFloat16": true,
         "doInvert": true,
         "doNormalize": true,
         "backDiameter": 200,
         "stddevWhiteDust": -1.0,
         "stddevBlackDust": -1.0,
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
         "streamingBatchSize": 0,
         "hostName": "localhost",
-        "numberOfMpi": 4,
-        "ctfRelations": "195.outputCTF",
-        "inputCoordinates": "528.outputCoordinates"
+        "numberOfMpi": 4
     },
     {
         "object.className": "ProtRelionClassify2D",
-        "object.id": "662",
+        "object.id": "653",
         "object.label": "relion - 2D classification #2",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "isClassify": true,
         "is2D": true,
         "doContinue": false,
+        "inputParticles": "583.outputParticles",
         "copyAlignment": false,
         "alignmentAsPriors": false,
         "fillRandomSubset": true,
         "maskDiameterA": 200,
         "maskZero": 0,
         "continueIter": "last",
         "continueMsg": "True",
@@ -345,38 +347,53 @@
         "limitResolEStep": -1.0,
         "doImageAlignment": true,
         "inplaneAngularSamplingDeg": 6.0,
         "offsetSearchRangePix": 5.0,
         "offsetSearchStepPix": 1.0,
         "allowCoarserSampling": false,
         "useParallelDisk": true,
-        "pooledParticles": 3,
-        "allParticlesRam": false,
+        "pooledParticles": 30,
+        "allParticlesRam": true,
         "scratchDir": null,
         "combineItersDisc": false,
         "doGpu": true,
         "gpusToUse": "",
         "oversampling": 1,
         "extraParams": "",
         "hostName": "localhost",
         "numberOfThreads": 8,
-        "numberOfMpi": 1,
-        "inputParticles": "593.outputParticles"
+        "numberOfMpi": 1
+    },
+    {
+        "object.className": "ProtRelionSelectClasses2D",
+        "object.id": "728",
+        "object.label": "relion - 2D class ranker",
+        "object.comment": "",
+        "_useQueue": false,
+        "_prerequisites": "",
+        "_queueParams": null,
+        "runName": null,
+        "runMode": 0,
+        "inputProtocol": "653.",
+        "minThreshold": 0.35,
+        "minParts": -1,
+        "minCls": -1
     },
     {
         "object.className": "ProtRelionInitialModel",
-        "object.id": "737",
-        "object.label": "relion - 3D initial model D2",
+        "object.id": "798",
+        "object.label": "relion - 3D initial model",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "doContinue": false,
+        "inputParticles": "728.outputParticles",
         "maskDiameterA": 200,
         "continueIter": "last",
         "continueMsg": "True",
         "doCTF": true,
         "haveDataBeenPhaseFlipped": null,
         "ignoreCTFUntilFirstPeak": false,
         "doCtfManualGroups": false,
@@ -386,74 +403,44 @@
         "regularisationParamT": 4.0,
         "numberOfClasses": 1,
         "doFlattenSolvent": true,
         "symmetryGroup": "D2",
         "runInC1": true,
         "useParallelDisk": true,
         "pooledParticles": 30,
-        "skipGridding": true,
-        "allParticlesRam": false,
+        "allParticlesRam": true,
         "scratchDir": null,
         "combineItersDisc": false,
         "doGpu": true,
         "gpusToUse": "",
         "extraParams": "",
         "hostName": "localhost",
-        "numberOfThreads": 4,
-        "inputParticles": "845.outputParticles"
-    },
-    {
-        "object.className": "ProtRelionSelectClasses2D",
-        "object.id": "803",
-        "object.label": "relion - 2D class ranker",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "minThreshold": 0.05,
-        "minParts": -1,
-        "minCls": -1,
-        "inputProtocol": "662."
-    },
-    {
-        "object.className": "ProtUserSubSet",
-        "object.id": "845",
-        "object.label": "create subset",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "other": null,
-        "sqliteFile": "Runs/000803_ProtRelionSelectClasses2D/extra/classes2d_state.sqlite,",
-        "outputClassName": "SetOfParticles",
-        "inputObject": "803.outputClasses"
+        "numberOfThreads": 8
     },
     {
         "object.className": "ProtRelionClassify3D",
-        "object.id": "934",
+        "object.id": "856",
         "object.label": "relion - 3D classification",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "isClassify": true,
         "is2D": false,
         "doContinue": false,
+        "inputParticles": "798.outputParticles",
         "copyAlignment": false,
         "alignmentAsPriors": false,
         "fillRandomSubset": true,
         "maskDiameterA": 200,
         "maskZero": 0,
         "continueIter": "last",
+        "referenceVolume": "798.outputVolumeSymmetrized",
         "solventFscMask": false,
         "isMapAbsoluteGreyScale": true,
         "symmetryGroup": "c1",
         "initialLowPassFilterA": 50.0,
         "continueMsg": "True",
         "doCTF": true,
         "haveDataBeenPhaseFlipped": null,
@@ -461,152 +448,152 @@
         "doCtfManualGroups": false,
         "defocusRange": 1000.0,
         "numParticles": 10.0,
         "numberOfClasses": 4,
         "regularisationParamT": 4.0,
         "numberOfIterations": 25,
         "useFastSubsets": false,
+        "useBlush": false,
         "limitResolEStep": -1.0,
         "doImageAlignment": true,
         "angularSamplingDeg": 2,
         "offsetSearchRangePix": 5.0,
         "offsetSearchStepPix": 1.0,
         "localAngularSearch": false,
         "localAngularSearchRange": 5.0,
         "relaxSymm": "",
         "allowCoarserSampling": false,
         "useParallelDisk": true,
         "pooledParticles": 30,
         "skipPadding": false,
-        "skipGridding": true,
-        "allParticlesRam": false,
+        "allParticlesRam": true,
         "scratchDir": null,
         "combineItersDisc": false,
         "doGpu": true,
         "gpusToUse": "",
         "oversampling": 1,
         "extraParams": "",
         "hostName": "localhost",
         "numberOfThreads": 4,
-        "numberOfMpi": 3,
-        "inputParticles": "737.outputParticles",
-        "referenceVolume": "737.outputVolumeSymmetrized"
+        "numberOfMpi": 3
     },
     {
-        "object.className": "ProtUserSubSet",
-        "object.id": "1045",
-        "object.label": "create subset particles",
+        "object.className": "ProtExtractCoords",
+        "object.id": "1004",
+        "object.label": "pwem - extract coordinates",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
-        "other": "908",
-        "sqliteFile": "Runs/000934_ProtRelionClassify3D/classes3D_state.sqlite,",
-        "outputClassName": "SetOfParticles",
-        "inputObject": "934."
+        "inputParticles": "1046.outputParticles",
+        "inputMicrographs": "88.outputMicrographsDoseWeighted",
+        "applyShifts": true,
+        "hostName": "localhost"
     },
     {
         "object.className": "ProtUserSubSet",
-        "object.id": "1080",
-        "object.label": "create subset volume",
+        "object.id": "1046",
+        "object.label": "create subset particles",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
-        "other": "908",
-        "sqliteFile": "Runs/000934_ProtRelionClassify3D/classes3D_state.sqlite,",
-        "outputClassName": "SetOfVolumes,Representatives",
-        "inputObject": "934."
+        "inputObject": "856.",
+        "other": "948",
+        "sqliteFile": "Runs/000856_ProtRelionClassify3D/classes3D_state.sqlite,",
+        "outputClassName": "SetOfParticles"
     },
     {
-        "object.className": "ProtExtractCoords",
-        "object.id": "1153",
-        "object.label": "pwem - extract coordinates",
+        "object.className": "ProtUserSubSet",
+        "object.id": "1081",
+        "object.label": "create subset volume",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
-        "applyShifts": true,
-        "hostName": "localhost",
-        "inputMicrographs": "88.outputMicrographsDoseWeighted",
-        "inputParticles": "1045.outputParticles"
+        "inputObject": "856.",
+        "other": "948",
+        "sqliteFile": "Runs/000856_ProtRelionClassify3D/classes3D_state.sqlite,",
+        "outputClassName": "SetOfVolumes,Representatives"
     },
     {
         "object.className": "ProtRelionExtractParticles",
-        "object.id": "1195",
-        "object.label": "relion - particles extraction 256",
+        "object.id": "1164",
+        "object.label": "relion - particles extraction 256px",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputCoordinates": "1004.outputCoordinates",
         "downsampleType": 0,
+        "ctfRelations": "196.outputCTF",
         "boxSize": 360,
         "doRescale": true,
         "rescaledSize": 256,
-        "saveFloat16": false,
+        "saveFloat16": true,
         "doInvert": true,
         "doNormalize": true,
         "backDiameter": 200,
         "stddevWhiteDust": -1.0,
         "stddevBlackDust": -1.0,
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
         "streamingBatchSize": 0,
         "hostName": "localhost",
-        "numberOfMpi": 4,
-        "ctfRelations": "195.outputCTF",
-        "inputCoordinates": "1153.outputCoordinates"
+        "numberOfMpi": 4
     },
     {
         "object.className": "ProtRelionResizeVolume",
-        "object.id": "1264",
-        "object.label": "relion - crop/resize volumes 256",
+        "object.id": "1234",
+        "object.label": "relion - crop/resize volumes",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputVolumes": "1081.outputRepresentatives",
         "doRescale": true,
         "rescaleSamplingRate": 1.244,
         "doResize": true,
         "resizeSize": 256,
-        "hostName": "localhost",
-        "inputVolumes": "1080.outputRepresentatives"
+        "hostName": "localhost"
     },
     {
         "object.className": "ProtRelionRefine3D",
-        "object.id": "1336",
+        "object.id": "1288",
         "object.label": "relion - 3D auto-refine",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "isClassify": false,
         "is2D": false,
         "doContinue": false,
+        "inputParticles": "1164.outputParticles",
         "copyAlignment": false,
         "alignmentAsPriors": false,
         "fillRandomSubset": true,
         "maskDiameterA": 200,
         "maskZero": 0,
         "continueIter": "last",
+        "referenceVolume": "1234.outputVol.4",
         "solventFscMask": false,
         "isMapAbsoluteGreyScale": false,
-        "symmetryGroup": "d2",
+        "symmetryGroup": "D2",
         "initialLowPassFilterA": 50.0,
         "continueMsg": "True",
         "doCTF": true,
         "haveDataBeenPhaseFlipped": null,
         "ignoreCTFUntilFirstPeak": false,
         "doCtfManualGroups": false,
         "defocusRange": 1000.0,
@@ -614,183 +601,184 @@
         "doImageAlignment": true,
         "angularSamplingDeg": 2,
         "offsetSearchRangePix": 5.0,
         "offsetSearchStepPix": 1.0,
         "localSearchAutoSamplingDeg": 4,
         "relaxSymm": "",
         "useFinerSamplingFaster": false,
+        "useBlush": false,
         "useParallelDisk": true,
         "pooledParticles": 30,
         "skipPadding": false,
-        "skipGridding": true,
-        "allParticlesRam": false,
+        "allParticlesRam": true,
         "scratchDir": null,
         "combineItersDisc": false,
         "doGpu": true,
         "gpusToUse": "",
         "oversampling": 1,
         "extraParams": "",
         "hostName": "localhost",
         "numberOfThreads": 4,
-        "numberOfMpi": 3,
-        "inputParticles": "1195.outputParticles",
-        "referenceVolume": "1264.outputVol.2"
+        "numberOfMpi": 3
     },
     {
         "object.className": "ProtRelionCreateMask3D",
-        "object.id": "1445",
+        "object.id": "1368",
         "object.label": "relion - create 3d mask",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputVolume": "1288.outputVolume",
         "initialLowPassFilterA": 15.0,
         "threshold": 0.005,
         "doCompare": false,
         "operation": 0,
         "extend": 3,
         "edge": 6,
         "doInvert": false,
         "hostName": "localhost",
-        "numberOfThreads": 4,
-        "inputVolume": "1336.outputVolume"
+        "numberOfThreads": 4
     },
     {
         "object.className": "ProtRelionPostprocess",
-        "object.id": "1492",
+        "object.id": "1409",
         "object.label": "relion - post-processing",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "relionInput": true,
+        "protRefine": "1288.",
         "bodyNum": 1,
+        "solventMask": "1368.outputMask",
         "calibratedPixelSize": 0.0,
         "mtf": "/home/gsharov/soft/scipion-em-plugins/scipion-em-relion/relion/convert/mtfs/mtf_k2_200_ec.star",
         "origPixelSize": 0.885,
         "doAutoBfactor": true,
         "bfactorLowRes": 10.0,
         "bfactorHighRes": 0.0,
         "bfactor": -350.0,
         "skipFscWeighting": false,
         "lowRes": 5.0,
         "filterEdgeWidth": 2,
         "randomizeAtFsc": 0.8,
         "forceMask": false,
-        "hostName": "localhost",
-        "protRefine": "1336.",
-        "solventMask": "1445.outputMask"
+        "hostName": "localhost"
     },
     {
         "object.className": "ProtRelionCtfRefinement",
-        "object.id": "1556",
-        "object.label": "relion - ctf refinement aberr",
+        "object.id": "1497",
+        "object.label": "relion - ctf refinement aberrations",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputParticles": "1288.outputParticles",
+        "inputPostprocess": "1409.",
         "estimateAnisoMag": false,
         "doCtfFitting": false,
         "fitDefocus": 0,
         "fitAstig": 0,
         "fitBfactor": 0,
         "fitPhaseShift": 0,
         "doBeamtiltEstimation": true,
         "doEstimateTrefoil": true,
         "doEstimate4thOrder": true,
         "minResolution": 30.0,
         "extraParams": "",
         "hostName": "localhost",
         "numberOfThreads": 8,
-        "numberOfMpi": 1,
-        "inputParticles": "1336.outputParticles",
-        "inputPostprocess": "1492."
+        "numberOfMpi": 1
     },
     {
         "object.className": "ProtRelionCtfRefinement",
-        "object.id": "1621",
-        "object.label": "relion - ctf refinement aniso",
+        "object.id": "1569",
+        "object.label": "relion - ctf refinement magnification",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputParticles": "1497.outputParticles",
+        "inputPostprocess": "1409.",
         "estimateAnisoMag": true,
         "doCtfFitting": false,
         "fitDefocus": 0,
         "fitAstig": 0,
         "fitBfactor": 0,
         "fitPhaseShift": 0,
-        "doBeamtiltEstimation": true,
-        "doEstimateTrefoil": true,
-        "doEstimate4thOrder": true,
+        "doBeamtiltEstimation": false,
+        "doEstimateTrefoil": false,
+        "doEstimate4thOrder": false,
         "minResolution": 30.0,
         "extraParams": "",
         "hostName": "localhost",
         "numberOfThreads": 8,
-        "numberOfMpi": 1,
-        "inputPostprocess": "1492.",
-        "inputParticles": "1556.outputParticles"
+        "numberOfMpi": 1
     },
     {
         "object.className": "ProtRelionCtfRefinement",
-        "object.id": "1686",
-        "object.label": "relion - ctf refinement def",
+        "object.id": "1635",
+        "object.label": "relion - ctf refinement defocus",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputParticles": "1569.outputParticles",
+        "inputPostprocess": "1409.",
         "estimateAnisoMag": false,
         "doCtfFitting": true,
         "fitDefocus": 2,
         "fitAstig": 1,
         "fitBfactor": 0,
         "fitPhaseShift": 0,
         "doBeamtiltEstimation": false,
-        "doEstimateTrefoil": true,
+        "doEstimateTrefoil": false,
         "doEstimate4thOrder": false,
         "minResolution": 30.0,
         "extraParams": "",
         "hostName": "localhost",
         "numberOfThreads": 8,
-        "numberOfMpi": 1,
-        "inputPostprocess": "1492.",
-        "inputParticles": "1621.outputParticles"
+        "numberOfMpi": 1
     },
     {
         "object.className": "ProtRelionRefine3D",
-        "object.id": "1751",
+        "object.id": "1680",
         "object.label": "relion - 3D auto-refine #2",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "isClassify": false,
         "is2D": false,
         "doContinue": false,
+        "inputParticles": "1635.outputParticles",
         "copyAlignment": false,
         "alignmentAsPriors": false,
         "fillRandomSubset": true,
         "maskDiameterA": 200,
         "maskZero": 0,
         "continueIter": "last",
-        "solventFscMask": true,
+        "referenceVolume": "1288.outputVolume",
+        "referenceMask": "1368.outputMask",
+        "solventFscMask": false,
         "isMapAbsoluteGreyScale": true,
-        "symmetryGroup": "d2",
+        "symmetryGroup": "D2",
         "initialLowPassFilterA": 50.0,
         "continueMsg": "True",
         "doCTF": true,
         "haveDataBeenPhaseFlipped": null,
         "ignoreCTFUntilFirstPeak": false,
         "doCtfManualGroups": false,
         "defocusRange": 1000.0,
@@ -798,134 +786,155 @@
         "doImageAlignment": true,
         "angularSamplingDeg": 2,
         "offsetSearchRangePix": 5.0,
         "offsetSearchStepPix": 1.0,
         "localSearchAutoSamplingDeg": 4,
         "relaxSymm": "",
         "useFinerSamplingFaster": false,
+        "useBlush": false,
         "useParallelDisk": true,
         "pooledParticles": 30,
         "skipPadding": false,
-        "skipGridding": true,
-        "allParticlesRam": false,
+        "allParticlesRam": true,
         "scratchDir": null,
         "combineItersDisc": false,
         "doGpu": true,
         "gpusToUse": "",
         "oversampling": 1,
         "extraParams": "",
         "hostName": "localhost",
         "numberOfThreads": 4,
-        "numberOfMpi": 3,
-        "referenceVolume": "1336.outputVolume",
-        "referenceMask": "1445.outputMask",
-        "inputParticles": "1686.outputParticles"
+        "numberOfMpi": 3
     },
     {
         "object.className": "ProtRelionAssignOpticsGroup",
-        "object.id": "1831",
+        "object.id": "1781",
         "object.label": "relion - assign optics groups",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputSet": "88.outputMovies",
         "inputType": 0,
         "opticsGroupName": "opticsGroup1",
         "mtfFile": "/home/gsharov/soft/scipion-em-plugins/scipion-em-relion/relion/convert/mtfs/mtf_k2_200_ec.star",
         "beamTiltX": 0.0,
         "beamTiltY": 0.0,
         "gainFile": "/data/tutorials/relion30_tutorial/Movies/gain.mrc",
         "gainRot": 0,
         "gainFlip": 0,
         "defectFile": null,
-        "inputStar": null,
-        "inputSet": "88.outputMovies"
+        "inputStar": null
+    },
+    {
+        "object.className": "ProtRelionCreateMask3D",
+        "object.id": "1875",
+        "object.label": "relion - create 3d mask #2",
+        "object.comment": "",
+        "_useQueue": false,
+        "_prerequisites": "",
+        "_queueParams": null,
+        "runName": null,
+        "runMode": 0,
+        "inputVolume": "1680.outputVolume",
+        "initialLowPassFilterA": 15.0,
+        "threshold": 0.005,
+        "doCompare": false,
+        "operation": 0,
+        "extend": 3,
+        "edge": 6,
+        "doInvert": false,
+        "hostName": "localhost",
+        "numberOfThreads": 4
     },
     {
         "object.className": "ProtRelionPostprocess",
-        "object.id": "1924",
+        "object.id": "1916",
         "object.label": "relion - post-processing #2",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "relionInput": true,
+        "protRefine": "1680.",
         "bodyNum": 1,
+        "solventMask": "1875.outputMask",
         "calibratedPixelSize": 0.0,
         "mtf": "/home/gsharov/soft/scipion-em-plugins/scipion-em-relion/relion/convert/mtfs/mtf_k2_200_ec.star",
         "origPixelSize": 0.885,
         "doAutoBfactor": true,
         "bfactorLowRes": 10.0,
         "bfactorHighRes": 0.0,
         "bfactor": -350.0,
         "skipFscWeighting": false,
         "lowRes": 5.0,
         "filterEdgeWidth": 2,
         "randomizeAtFsc": 0.8,
         "forceMask": false,
-        "hostName": "localhost",
-        "solventMask": "1445.outputMask",
-        "protRefine": "1751."
+        "hostName": "localhost"
     },
     {
         "object.className": "ProtRelionBayesianPolishing",
-        "object.id": "1982",
+        "object.id": "2015",
         "object.label": "relion - bayesian polishing",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "inputMovies": "1781.outputMovies",
+        "inputParticles": "1680.outputParticles",
+        "inputPostprocess": "1916.",
         "frame0": 1,
         "frameN": 0,
         "extrSize": -1,
         "rescaledSize": -1,
-        "saveFloat16": false,
+        "saveFloat16": true,
         "operation": 1,
         "fractionFourierPx": 0.5,
         "numberOfParticles": 10000,
         "sigmaVel": 0.42,
         "sigmaDiv": 1600.0,
         "sigmaAcc": 2.61,
         "minResBfactor": 20.0,
         "maxResBfactor": -1.0,
         "hostName": "localhost",
         "numberOfThreads": 24,
-        "numberOfMpi": 1,
-        "inputParticles": "1751.outputParticles",
-        "inputMovies": "1831.outputMovies",
-        "inputPostprocess": "1924."
+        "numberOfMpi": 1
     },
     {
         "object.className": "ProtRelionRefine3D",
-        "object.id": "2051",
+        "object.id": "2070",
         "object.label": "relion - 3D auto-refine #3",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "isClassify": false,
         "is2D": false,
         "doContinue": false,
+        "inputParticles": "2015.outputParticles",
         "copyAlignment": false,
         "alignmentAsPriors": false,
         "fillRandomSubset": true,
         "maskDiameterA": 200,
         "maskZero": 0,
         "continueIter": "last",
+        "referenceVolume": "1680.outputVolume",
+        "referenceMask": "1875.outputMask",
         "solventFscMask": true,
         "isMapAbsoluteGreyScale": true,
-        "symmetryGroup": "d2",
+        "symmetryGroup": "D2",
         "initialLowPassFilterA": 50.0,
         "continueMsg": "True",
         "doCTF": true,
         "haveDataBeenPhaseFlipped": null,
         "ignoreCTFUntilFirstPeak": false,
         "doCtfManualGroups": false,
         "defocusRange": 1000.0,
@@ -933,79 +942,97 @@
         "doImageAlignment": true,
         "angularSamplingDeg": 2,
         "offsetSearchRangePix": 5.0,
         "offsetSearchStepPix": 1.0,
         "localSearchAutoSamplingDeg": 4,
         "relaxSymm": "",
         "useFinerSamplingFaster": false,
+        "useBlush": false,
         "useParallelDisk": true,
         "pooledParticles": 30,
         "skipPadding": false,
-        "skipGridding": true,
         "allParticlesRam": false,
         "scratchDir": null,
         "combineItersDisc": false,
         "doGpu": true,
         "gpusToUse": "",
         "oversampling": 1,
         "extraParams": "",
         "hostName": "localhost",
-        "numberOfThreads": 4,
-        "numberOfMpi": 3,
-        "referenceMask": "1445.outputMask",
-        "referenceVolume": "1751.outputVolume",
-        "inputParticles": "1982.outputParticles"
+        "numberOfThreads": 3,
+        "numberOfMpi": 3
+    },
+    {
+        "object.className": "ProtRelionCreateMask3D",
+        "object.id": "2150",
+        "object.label": "relion - create 3d mask #3",
+        "object.comment": "",
+        "_useQueue": false,
+        "_prerequisites": "",
+        "_queueParams": null,
+        "runName": null,
+        "runMode": 0,
+        "inputVolume": "2070.outputVolume",
+        "initialLowPassFilterA": 15.0,
+        "threshold": 0.005,
+        "doCompare": false,
+        "operation": 0,
+        "extend": 3,
+        "edge": 6,
+        "doInvert": false,
+        "hostName": "localhost",
+        "numberOfThreads": 4
     },
     {
         "object.className": "ProtRelionPostprocess",
-        "object.id": "2160",
+        "object.id": "2191",
         "object.label": "relion - post-processing #3",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "relionInput": true,
+        "protRefine": "2070.",
         "bodyNum": 1,
+        "solventMask": "2150.outputMask",
         "calibratedPixelSize": 0.0,
         "mtf": "/home/gsharov/soft/scipion-em-plugins/scipion-em-relion/relion/convert/mtfs/mtf_k2_200_ec.star",
         "origPixelSize": 0.885,
         "doAutoBfactor": true,
         "bfactorLowRes": 10.0,
         "bfactorHighRes": 0.0,
         "bfactor": -350.0,
         "skipFscWeighting": false,
         "lowRes": 5.0,
         "filterEdgeWidth": 2,
         "randomizeAtFsc": 0.8,
         "forceMask": false,
-        "hostName": "localhost",
-        "solventMask": "1445.outputMask",
-        "protRefine": "2051."
+        "hostName": "localhost"
     },
     {
         "object.className": "ProtRelionLocalRes",
-        "object.id": "2218",
+        "object.id": "2268",
         "object.label": "relion - local resolution",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
+        "protRefine": "2070.",
+        "solventMask": "2150.outputMask",
         "calibratedPixelSize": 1.244,
-        "bfactor": -8.0,
+        "bfactor": -7.64,
         "mtf": "/home/gsharov/soft/scipion-em-plugins/scipion-em-relion/relion/convert/mtfs/mtf_k2_200_ec.star",
         "origPixelSize": 0.885,
         "Msg": null,
         "locResSamp": 25,
         "locResMaskRad": -1,
         "locResEdgeWidth": -1,
         "locResRand": 25.0,
         "locResMin": 50,
         "hostName": "localhost",
-        "numberOfMpi": 8,
-        "solventMask": "1445.outputMask",
-        "protRefine": "2051."
+        "numberOfMpi": 8
     }
 ]
```

### Comparing `scipion-em-relion-5.0.0b2/relion/tests/__init__.py` & `scipion-em-relion-5.0.0b4/relion/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/tests/test_convert.py` & `scipion-em-relion-5.0.0b4/relion/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/tests/test_projection_subtraction_no_relion.py` & `scipion-em-relion-5.0.0b4/relion/tests/test_projection_subtraction_no_relion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/tests/test_protocols_2d.py` & `scipion-em-relion-5.0.0b4/relion/tests/test_protocols_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 from glob import glob
 
 from pyworkflow.tests import setupTestProject, DataSet
 from pyworkflow.plugin import Domain
 from pyworkflow.utils import magentaStr
 from pwem.objects import SetOfMovies
-from pwem.protocols import ProtImportAverages, ProtImportCTF, ProtImportParticles
+from pwem.protocols import (ProtImportAverages, ProtImportCTF,
+                            ProtImportParticles, ProtImportCoordinates)
 
 from ..protocols import *
 from ..convert import *
 from ..constants import *
 from relion.convert.convert31 import OpticsGroups
 from .test_protocols_base import TestRelionBase, USE_GPU, RUN_CPU, CPUS, MTF_FILE
 
@@ -589,29 +590,48 @@
 class TestRelionImportCoords(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.ds = DataSet.getDataSet('relion31_tutorial_precalculated')
         cls.mics = cls.ds.getFile('MotionCorr/job002/Movies/*frameImage.mrc')
         cls.parts = cls.ds.getFile('Refine3D/job029/run_it018_data.star')
+        cls.coords = cls.ds.getFile('AutoPick/job006/Movies')
         cls.protImportMics = cls.runImportMics(cls.mics, 0.885)
 
     def testImportCoords(self):
-        """ Run an Import coords protocol. """
-        print(magentaStr("\n==> Importing coordinates (from star file):"))
-        self.protImport = self.newProtocol(ProtRelionImportCoords,
-                                           filePath=self.parts,
+        """ Run an Import coords protocol from a particle star file. """
+        print(magentaStr("\n==> Importing coordinates (from particles star file):"))
+        self.protImport = self.newProtocol(ProtImportCoordinates,
+                                           objLabel="from particles star file",
+                                           importFrom=2,  # RELION
+                                           filesPath=self.parts,
                                            boxSize=128)
         self.protImport.inputMicrographs.set(self.protImportMics.outputMicrographs)
         self.launchProtocol(self.protImport)
         self.assertIsNotNone(self.protImport.outputCoordinates,
                              "SetOfCoordinates has not been produced.")
         self.assertEqual(self.protImport.outputCoordinates.getSize(),
                          4501, "Output size is not 4501!")
 
+    def testImportCoords2(self):
+        """ Run an Import coords protocol. """
+        print(magentaStr("\n==> Importing coordinates (from coordinates star file):"))
+        self.protImport = self.newProtocol(ProtImportCoordinates,
+                                           objLabel="from coordinates star file",
+                                           importFrom=2,  # RELION
+                                           filesPath=self.coords,
+                                           filesPattern="*autopick.star",
+                                           boxSize=128)
+        self.protImport.inputMicrographs.set(self.protImportMics.outputMicrographs)
+        self.launchProtocol(self.protImport)
+        self.assertIsNotNone(self.protImport.outputCoordinates,
+                             "SetOfCoordinates has not been produced.")
+        self.assertEqual(self.protImport.outputCoordinates.getSize(),
+                         1158, "Output size is not 1158!")
+
 
 class TestRelionImportParticles(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.ds = DataSet.getDataSet('relion31_tutorial_precalculated')
```

### Comparing `scipion-em-relion-5.0.0b2/relion/tests/test_protocols_3d.py` & `scipion-em-relion-5.0.0b4/relion/tests/test_protocols_3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/tests/test_protocols_base.py` & `scipion-em-relion-5.0.0b4/relion/tests/test_protocols_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/tests/test_workflow.py` & `scipion-em-relion-5.0.0b4/relion/tests/test_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,63 +84,66 @@
 
     def _runRelionMc(self, protImport):
         print(magentaStr("\n==> Testing relion - motioncor:"))
         protRelionMc = self.newProtocol(
             ProtRelionMotioncor,
             objLabel='relion - motioncor',
             patchX=1, patchY=1,
-            numberOfMpi=CPUS//2)
+            numberOfThreads=CPUS)
 
         protRelionMc.inputMovies.set(protImport.outputMovies)
         protRelionMc = self.launchProtocol(protRelionMc)
 
         return protRelionMc
 
     def _runRelionLog(self, protRelionMc):
         print(magentaStr("\n==> Testing relion - autopick LoG:"))
         protRelionLog = self.newProtocol(
             ProtRelionAutopickLoG,
             objLabel='relion - autopick log',
             boxSize=100,
             minDiameter=150, maxDiameter=180,
             threshold2=5.0,
-            numberOfMpi=CPUS//2)
+            streamingBatchSize=0,
+            numberOfMpi=1)
 
         protRelionLog.inputMicrographs.set(protRelionMc.outputMicrographsDoseWeighted)
         protRelionLog = self.launchProtocol(protRelionLog)
 
         return protRelionLog
 
-    def _runGctf(self, protMc):
-        print(magentaStr("\n==> Testing gctf - estimate ctf:"))
-        ProtGctf = Domain.importFromPlugin('gctf.protocols', 'ProtGctf')
-
-        protGctf = self.newProtocol(
-            ProtGctf,
-            objLabel='gctf',
-            lowRes=0.04, highRes=0.21,
+    def _runCtffind(self, protMc):
+        print(magentaStr("\n==> Testing ctffind - estimate ctf:"))
+        ProtCtfFind = Domain.importFromPlugin('cistem.protocols', 'CistemProtCTFFind')
+
+        protCtf = self.newProtocol(
+            ProtCtfFind,
+            objLabel='ctffind',
+            lowRes=20, highRes=3,
             astigmatism=100,
             windowSize=512,
-            gpuList="0"
+            usePowerSpectra=True,
+            streamingBatchSize=0
         )
 
-        protGctf.inputMicrographs.set(protMc.outputMicrographsDoseWeighted)
-        protGctf = self.launchProtocol(protGctf)
+        protCtf.inputMicrographs.set(protMc.outputMicrographsDoseWeighted)
+        protCtf = self.launchProtocol(protCtf)
 
-        return protGctf
+        return protCtf
 
     def _runRelionExtract(self, protPicking, protCtf):
         print(magentaStr("\n==> Testing relion - extract particles:"))
         protRelionExtract = self.newProtocol(
             ProtRelionExtractParticles,
             objLabel='relion - extract',
             boxSize=256, doRescale=True, rescaledSize=64,
             doInvert=True, doNormalize=True,
             backDiameter=200,
             numberOfMpi=CPUS,
+            streamingBatchSize=0,
             downsamplingType=0  # Micrographs same as picking
         )
 
         protRelionExtract.ctfRelations.set(protCtf.outputCTF)
         protRelionExtract.inputCoordinates.set(protPicking.outputCoordinates)
         protRelionExtract = self.launchProtocol(protRelionExtract)
 
@@ -177,14 +180,14 @@
         relionIniModel.inputParticles.set(protExtract.outputParticles)
         protInitModel = self.launchProtocol(relionIniModel)
         return protInitModel
 
     def test_workflow(self):
         protImport = self._importMovies()
         protRelionMc = self._runRelionMc(protImport)
-        protGctf = self._runGctf(protRelionMc)
+        protCtfFind = self._runCtffind(protRelionMc)
         protRelionLog = self._runRelionLog(protRelionMc)
-        protRelionExtract = self._runRelionExtract(protRelionLog, protGctf)
+        protRelionExtract = self._runRelionExtract(protRelionLog, protCtfFind)
         protRelion2D = self._runRelion2D(protRelionExtract)
         protInitModel = self._runInitModel(protRelionExtract)
         self.assertIsNotNone(protRelion2D.outputClasses, protRelion2D.getErrorMessage())
         self.assertIsNotNone(protInitModel.outputVolume, protInitModel.getErrorMessage())
```

### Comparing `scipion-em-relion-5.0.0b2/relion/viewers/__init__.py` & `scipion-em-relion-5.0.0b4/relion/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/viewers/viewer_base.py` & `scipion-em-relion-5.0.0b4/relion/viewers/viewer_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/viewers/viewer_ctfrefine.py` & `scipion-em-relion-5.0.0b4/relion/viewers/viewer_ctfrefine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/viewers/viewer_locres.py` & `scipion-em-relion-5.0.0b4/relion/viewers/viewer_locres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/viewers/viewer_motioncor.py` & `scipion-em-relion-5.0.0b4/relion/viewers/viewer_motioncor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/viewers/viewer_multibody.py` & `scipion-em-relion-5.0.0b4/relion/viewers/viewer_multibody.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/viewers/viewer_polishing.py` & `scipion-em-relion-5.0.0b4/relion/viewers/viewer_polishing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/viewers/viewer_postprocess.py` & `scipion-em-relion-5.0.0b4/relion/viewers/viewer_postprocess.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/viewers/viewer_reconstruct.py` & `scipion-em-relion-5.0.0b4/relion/viewers/viewer_reconstruct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/relion/wizards.py` & `scipion-em-relion-5.0.0b4/relion/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-5.0.0b2/scipion_em_relion.egg-info/PKG-INFO` & `scipion-em-relion-5.0.0b4/scipion_em_relion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-relion
-Version: 5.0.0b2
+Version: 5.0.0b4
 Summary: Plugin to use Relion programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-relion
 Author: Grigory Sharov, J.M. De la Rosa Trevin, Josue Gomez Blanco
 Author-email: gsharov@mrc-lmb.cam.ac.uk, delarosatrevin@scilifelab.se, josue.gomez-blanco@mcgill.ca
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-relion/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-relion/
@@ -102,16 +102,15 @@
         * ctf refinement
         * DynaMight flexibility
         * estimate gain to compress
         * expand symmetry
         * export coordinates
         * export ctf                
         * export particles
-        * import coordinates
-        * local resolution          
+        * local resolution
         * motion correction
         * particles extraction
         * post-processing           
         * preprocess particles      
         * reconstruct
         * remove preferential views
         * subtract projection
```

### Comparing `scipion-em-relion-5.0.0b2/scipion_em_relion.egg-info/SOURCES.txt` & `scipion-em-relion-5.0.0b4/scipion_em_relion.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 relion/protocols/protocol_estimate_gain.py
 relion/protocols/protocol_expand_symmetry.py
 relion/protocols/protocol_export_coords.py
 relion/protocols/protocol_export_ctf.py
 relion/protocols/protocol_export_particles.py
 relion/protocols/protocol_extract_particles.py
 relion/protocols/protocol_gentle_clean.py
-relion/protocols/protocol_import_coords.py
 relion/protocols/protocol_initialmodel.py
 relion/protocols/protocol_localres.py
 relion/protocols/protocol_motioncor.py
 relion/protocols/protocol_multibody.py
 relion/protocols/protocol_postprocess.py
 relion/protocols/protocol_preprocess.py
 relion/protocols/protocol_reconstruct.py
```

### Comparing `scipion-em-relion-5.0.0b2/setup.py` & `scipion-em-relion-5.0.0b4/setup.py`

 * *Files identical despite different names*

