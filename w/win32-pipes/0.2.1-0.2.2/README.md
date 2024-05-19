# Comparing `tmp/win32_pipes-0.2.1.tar.gz` & `tmp/win32_pipes-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win32_pipes-0.2.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "win32_pipes-0.2.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `win32_pipes-0.2.1.tar` & `win32_pipes-0.2.2.tar`

### file list

```diff
@@ -1,212 +1,212 @@
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/.clang-format
--rw-r--r--   0        0        0     1962 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     3085 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/.gitignore
--rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/.gitmodules
--rw-r--r--   0        0        0     1141 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1166 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/CMakeLists.txt
--rw-r--r--   0        0        0     1103 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/LICENSE
--rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/README.md
--rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/.git
--rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/.github/ISSUE_TEMPLATE/all-other.yml
--rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1710 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/.github/workflows/ci.yml
--rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/.gitignore
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/.gitmodules
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/.readthedocs.yaml
--rw-r--r--   0        0        0     5223 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/CMakeLists.txt
--rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/LICENSE
--rw-r--r--   0        0        0     2972 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/README.md
--rw-r--r--   0        0        0      825 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/cmake/collect-symbols-pypy.py
--rw-r--r--   0        0        0     1374 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/cmake/collect-symbols.py
--rw-r--r--   0        0        0    21604 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/cmake/darwin-ld-cpython.sym
--rw-r--r--   0        0        0    24687 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/cmake/darwin-ld-pypy.sym
--rw-r--r--   0        0        0    12296 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/cmake/nanobind-config.cmake
--rw-r--r--   0        0        0    14454 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/api_cmake.rst
--rw-r--r--   0        0        0    98247 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/api_core.rst
--rw-r--r--   0        0        0    42426 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/api_extra.rst
--rw-r--r--   0        0        0    14772 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/basics.rst
--rw-r--r--   0        0        0     7853 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/benchmark.rst
--rw-r--r--   0        0        0     4421 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/building.rst
--rw-r--r--   0        0        0    44820 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/changelog.rst
--rw-r--r--   0        0        0    28295 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/classes.rst
--rw-r--r--   0        0        0     8130 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/conf.py
--rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/cppyy.h
--rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/eigen.rst
--rw-r--r--   0        0        0    10941 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/exceptions.rst
--rw-r--r--   0        0        0    13951 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/exchanging.rst
--rw-r--r--   0        0        0    16804 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/faq.rst
--rw-r--r--   0        0        0    15052 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/functions.rst
--rw-r--r--   0        0        0    20461 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/binding-dark.svg
--rw-r--r--   0        0        0    20183 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/binding-light.svg
--rw-r--r--   0        0        0    18165 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/caster-dark.svg
--rw-r--r--   0        0        0    17829 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/caster-light.svg
--rw-r--r--   0        0        0   426666 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/logo.jpg
--rw-r--r--   0        0        0    56614 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/perf.svg
--rw-r--r--   0        0        0    53541 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/sizes.svg
--rw-r--r--   0        0        0    52665 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/times.svg
--rw-r--r--   0        0        0    14221 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/wrapper-dark.svg
--rw-r--r--   0        0        0    13943 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/images/wrapper-light.svg
--rw-r--r--   0        0        0     3435 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/index.rst
--rw-r--r--   0        0        0     1565 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/installing.rst
--rw-r--r--   0        0        0    11256 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/lowlevel.rst
--rw-r--r--   0        0        0    17077 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/microbenchmark.ipynb
--rw-r--r--   0        0        0    20006 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/ndarray.rst
--rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/ndarray_index.rst
--rw-r--r--   0        0        0    15752 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/ownership.rst
--rw-r--r--   0        0        0    17447 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/ownership_adv.rst
--rw-r--r--   0        0        0    12130 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/packaging.rst
--rw-r--r--   0        0        0    14298 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/porting.rst
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/pypy.rst
--rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/release.rst
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/requirements.txt
--rw-r--r--   0        0        0     7114 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/typeslots.rst
--rw-r--r--   0        0        0     1671 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/utilities.rst
--rw-r--r--   0        0        0    10852 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/docs/why.rst
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/.codecov.yml
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/.git
--rw-r--r--   0        0        0     4748 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3484 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/CMakeLists.txt
--rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/LICENSE
--rw-r--r--   0        0        0    21210 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/README.md
--rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/cmake/tsl-robin-mapConfig.cmake.in
--rw-r--r--   0        0        0   108206 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/doxygen.conf
--rw-r--r--   0        0        0    11776 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/include/tsl/robin_growth_policy.h
--rw-r--r--   0        0        0    54550 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/include/tsl/robin_hash.h
--rw-r--r--   0        0        0    28414 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/include/tsl/robin_map.h
--rw-r--r--   0        0        0    23593 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/include/tsl/robin_set.h
--rw-r--r--   0        0        0     1141 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/CMakeLists.txt
--rw-r--r--   0        0        0     3875 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/custom_allocator_tests.cpp
--rw-r--r--   0        0        0     1247 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/main.cpp
--rw-r--r--   0        0        0     3351 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/policy_tests.cpp
--rw-r--r--   0        0        0    45919 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/robin_map_tests.cpp
--rw-r--r--   0        0        0     5762 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/robin_set_tests.cpp
--rw-r--r--   0        0        0    12624 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/utils.h
--rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tsl-robin-map.natvis
--rw-r--r--   0        0        0    17889 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/eigen/dense.h
--rw-r--r--   0        0        0     6505 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/eigen/sparse.h
--rw-r--r--   0        0        0     1939 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/eval.h
--rw-r--r--   0        0        0     8884 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/intrusive/counter.h
--rw-r--r--   0        0        0     4874 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/intrusive/counter.inl
--rw-r--r--   0        0        0     4860 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/intrusive/ref.h
--rw-r--r--   0        0        0     5601 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/make_iterator.h
--rw-r--r--   0        0        0     1628 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nanobind.h
--rw-r--r--   0        0        0     6228 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_accessor.h
--rw-r--r--   0        0        0     9513 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_attr.h
--rw-r--r--   0        0        0     5471 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_call.h
--rw-r--r--   0        0        0    17851 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_cast.h
--rw-r--r--   0        0        0    25113 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_class.h
--rw-r--r--   0        0        0     6232 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_defs.h
--rw-r--r--   0        0        0     4129 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_descr.h
--rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_enums.h
--rw-r--r--   0        0        0     5207 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_error.h
--rw-r--r--   0        0        0    10802 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_func.h
--rw-r--r--   0        0        0    21272 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_lib.h
--rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_misc.h
--rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_python.h
--rw-r--r--   0        0        0     7314 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_traits.h
--rw-r--r--   0        0        0     2468 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_tuple.h
--rw-r--r--   0        0        0    28452 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_types.h
--rw-r--r--   0        0        0    20322 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/ndarray.h
--rw-r--r--   0        0        0     7449 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/operators.h
--rw-r--r--   0        0        0      535 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/array.h
--rw-r--r--   0        0        0     5939 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/bind_map.h
--rw-r--r--   0        0        0     7420 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/bind_vector.h
--rw-r--r--   0        0        0     8673 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/chrono.h
--rw-r--r--   0        0        0     2154 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/complex.h
--rw-r--r--   0        0        0    10571 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/chrono.h
--rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/nb_array.h
--rw-r--r--   0        0        0     2904 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/nb_dict.h
--rw-r--r--   0        0        0     2247 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/nb_list.h
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/nb_set.h
--rw-r--r--   0        0        0     3219 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/traits.h
--rw-r--r--   0        0        0     2719 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/filesystem.h
--rw-r--r--   0        0        0     2477 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/function.h
--rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/list.h
--rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/map.h
--rw-r--r--   0        0        0     2202 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/optional.h
--rw-r--r--   0        0        0     2770 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/pair.h
--rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/set.h
--rw-r--r--   0        0        0     4820 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/shared_ptr.h
--rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/string.h
--rw-r--r--   0        0        0     1062 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/string_view.h
--rw-r--r--   0        0        0     3307 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/tuple.h
--rw-r--r--   0        0        0     4389 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/unique_ptr.h
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/unordered_map.h
--rw-r--r--   0        0        0      652 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/unordered_set.h
--rw-r--r--   0        0        0     2776 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/variant.h
--rw-r--r--   0        0        0      537 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/vector.h
--rw-r--r--   0        0        0     2975 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/include/nanobind/trampoline.h
--rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/pyproject.toml
--rw-r--r--   0        0        0     3211 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/setup.py
--rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/__init__.py
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/__main__.py
--rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/buffer.h
--rw-r--r--   0        0        0    30688 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/common.cpp
--rw-r--r--   0        0        0     8851 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/error.cpp
--rw-r--r--   0        0        0     1009 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/hash.h
--rw-r--r--   0        0        0     2318 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/implicit.cpp
--rw-r--r--   0        0        0    14686 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/nb_enum.cpp
--rw-r--r--   0        0        0    40196 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/nb_func.cpp
--rw-r--r--   0        0        0    15914 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/nb_internals.cpp
--rw-r--r--   0        0        0    10614 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/nb_internals.h
--rw-r--r--   0        0        0    24024 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/nb_ndarray.cpp
--rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/nb_static_property.cpp
--rw-r--r--   0        0        0    59202 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/nb_type.cpp
--rw-r--r--   0        0        0     5144 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/src/trampoline.cpp
--rw-r--r--   0        0        0     3562 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/CMakeLists.txt
--rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/common.py
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/inter_module.cpp
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/inter_module.h
--rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/object_py.h
--rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_chrono.cpp
--rw-r--r--   0        0        0    10852 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_chrono.py
--rw-r--r--   0        0        0    18240 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_classes.cpp
--rw-r--r--   0        0        0    20465 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_classes.py
--rw-r--r--   0        0        0     9586 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_eigen.cpp
--rw-r--r--   0        0        0    12097 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_eigen.py
--rw-r--r--   0        0        0     2391 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_enum.cpp
--rw-r--r--   0        0        0     5680 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_enum.py
--rw-r--r--   0        0        0     2342 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_eval.cpp
--rw-r--r--   0        0        0      893 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_eval.py
--rw-r--r--   0        0        0     2579 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_exception.cpp
--rw-r--r--   0        0        0     3301 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_exception.py
--rw-r--r--   0        0        0     7965 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_functions.cpp
--rw-r--r--   0        0        0     9820 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_functions.py
--rw-r--r--   0        0        0     9373 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_holders.cpp
--rw-r--r--   0        0        0    11149 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_holders.py
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_inter_module.py
--rw-r--r--   0        0        0      170 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_inter_module_1.cpp
--rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_inter_module_2.cpp
--rw-r--r--   0        0        0     1884 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_intrusive.cpp
--rw-r--r--   0        0        0     1281 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_intrusive.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_intrusive_impl.cpp
--rw-r--r--   0        0        0     1845 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_issue.cpp
--rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_issue.py
--rw-r--r--   0        0        0     1741 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_make_iterator.cpp
--rw-r--r--   0        0        0      816 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_make_iterator.py
--rw-r--r--   0        0        0    11559 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_ndarray.cpp
--rw-r--r--   0        0        0    18521 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_ndarray.py
--rw-r--r--   0        0        0    15922 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_stl.cpp
--rw-r--r--   0        0        0    24433 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_stl.py
--rw-r--r--   0        0        0     2478 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_stl_bind_map.cpp
--rw-r--r--   0        0        0     5597 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_stl_bind_map.py
--rw-r--r--   0        0        0     1279 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_stl_bind_vector.cpp
--rw-r--r--   0        0        0     4034 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/ext/nanobind/tests/test_stl_bind_vector.py
--rw-r--r--   0        0        0     2107 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2268 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/Pipe.cpp
--rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/Pipe.h
--rw-r--r--   0        0        0      878 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/PipeClient.cpp
--rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/PipeClient.h
--rw-r--r--   0        0        0    10256 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/PipeConnection.cpp
--rw-r--r--   0        0        0     2475 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/PipeConnection.h
--rw-r--r--   0        0        0     3083 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/PipeListener.cpp
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/PipeListener.h
--rw-r--r--   0        0        0     2802 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/module.cpp
--rw-r--r--   0        0        0      719 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/util.cpp
--rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/cpp/util.h
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/win32_pipes/__init__.py
--rw-r--r--   0        0        0     1698 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/win32_pipes/_ext.pyi
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/src/win32_pipes/py.typed
--rw-r--r--   0        0        0     5290 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/tests/test_pipes.py
--rw-r--r--   0        0        0      138 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/tox.ini
--rw-r--r--   0        0        0     1463 2022-11-09 12:37:21.000000 win32_pipes-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/.clang-format
+-rw-r--r--   0        0        0     1962 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     3085 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/.gitignore
+-rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/.gitmodules
+-rw-r--r--   0        0        0     1141 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1166 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/CMakeLists.txt
+-rw-r--r--   0        0        0     1103 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1491 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/README.md
+-rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/.git
+-rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/.github/ISSUE_TEMPLATE/all-other.yml
+-rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1710 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/.gitignore
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/.gitmodules
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/.readthedocs.yaml
+-rw-r--r--   0        0        0     5223 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/CMakeLists.txt
+-rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/LICENSE
+-rw-r--r--   0        0        0     2972 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/README.md
+-rw-r--r--   0        0        0      825 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/cmake/collect-symbols-pypy.py
+-rw-r--r--   0        0        0     1374 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/cmake/collect-symbols.py
+-rw-r--r--   0        0        0    21604 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/cmake/darwin-ld-cpython.sym
+-rw-r--r--   0        0        0    24687 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/cmake/darwin-ld-pypy.sym
+-rw-r--r--   0        0        0    12296 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/cmake/nanobind-config.cmake
+-rw-r--r--   0        0        0    14454 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/api_cmake.rst
+-rw-r--r--   0        0        0    98247 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/api_core.rst
+-rw-r--r--   0        0        0    42426 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/api_extra.rst
+-rw-r--r--   0        0        0    14772 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/basics.rst
+-rw-r--r--   0        0        0     7853 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/benchmark.rst
+-rw-r--r--   0        0        0     4421 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/building.rst
+-rw-r--r--   0        0        0    44820 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/changelog.rst
+-rw-r--r--   0        0        0    28295 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/classes.rst
+-rw-r--r--   0        0        0     8130 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/conf.py
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/cppyy.h
+-rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/eigen.rst
+-rw-r--r--   0        0        0    10941 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/exceptions.rst
+-rw-r--r--   0        0        0    13951 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/exchanging.rst
+-rw-r--r--   0        0        0    16804 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/faq.rst
+-rw-r--r--   0        0        0    15052 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/functions.rst
+-rw-r--r--   0        0        0    20461 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/binding-dark.svg
+-rw-r--r--   0        0        0    20183 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/binding-light.svg
+-rw-r--r--   0        0        0    18165 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/caster-dark.svg
+-rw-r--r--   0        0        0    17829 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/caster-light.svg
+-rw-r--r--   0        0        0   426666 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/logo.jpg
+-rw-r--r--   0        0        0    56614 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/perf.svg
+-rw-r--r--   0        0        0    53541 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/sizes.svg
+-rw-r--r--   0        0        0    52665 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/times.svg
+-rw-r--r--   0        0        0    14221 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/wrapper-dark.svg
+-rw-r--r--   0        0        0    13943 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/images/wrapper-light.svg
+-rw-r--r--   0        0        0     3435 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/index.rst
+-rw-r--r--   0        0        0     1565 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/installing.rst
+-rw-r--r--   0        0        0    11256 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/lowlevel.rst
+-rw-r--r--   0        0        0    17077 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/microbenchmark.ipynb
+-rw-r--r--   0        0        0    20006 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/ndarray.rst
+-rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/ndarray_index.rst
+-rw-r--r--   0        0        0    15752 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/ownership.rst
+-rw-r--r--   0        0        0    17447 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/ownership_adv.rst
+-rw-r--r--   0        0        0    12130 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/packaging.rst
+-rw-r--r--   0        0        0    14298 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/porting.rst
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/pypy.rst
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/release.rst
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/requirements.txt
+-rw-r--r--   0        0        0     7114 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/typeslots.rst
+-rw-r--r--   0        0        0     1671 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/utilities.rst
+-rw-r--r--   0        0        0    10852 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/docs/why.rst
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/.codecov.yml
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/.git
+-rw-r--r--   0        0        0     4748 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3484 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/CMakeLists.txt
+-rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/LICENSE
+-rw-r--r--   0        0        0    21210 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/README.md
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/cmake/tsl-robin-mapConfig.cmake.in
+-rw-r--r--   0        0        0   108206 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/doxygen.conf
+-rw-r--r--   0        0        0    11776 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/include/tsl/robin_growth_policy.h
+-rw-r--r--   0        0        0    54550 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/include/tsl/robin_hash.h
+-rw-r--r--   0        0        0    28414 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/include/tsl/robin_map.h
+-rw-r--r--   0        0        0    23593 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/include/tsl/robin_set.h
+-rw-r--r--   0        0        0     1141 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     3875 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/custom_allocator_tests.cpp
+-rw-r--r--   0        0        0     1247 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/main.cpp
+-rw-r--r--   0        0        0     3351 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/policy_tests.cpp
+-rw-r--r--   0        0        0    45919 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/robin_map_tests.cpp
+-rw-r--r--   0        0        0     5762 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/robin_set_tests.cpp
+-rw-r--r--   0        0        0    12624 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/utils.h
+-rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tsl-robin-map.natvis
+-rw-r--r--   0        0        0    17889 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/eigen/dense.h
+-rw-r--r--   0        0        0     6505 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/eigen/sparse.h
+-rw-r--r--   0        0        0     1939 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/eval.h
+-rw-r--r--   0        0        0     8884 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/intrusive/counter.h
+-rw-r--r--   0        0        0     4874 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/intrusive/counter.inl
+-rw-r--r--   0        0        0     4860 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/intrusive/ref.h
+-rw-r--r--   0        0        0     5601 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/make_iterator.h
+-rw-r--r--   0        0        0     1628 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nanobind.h
+-rw-r--r--   0        0        0     6228 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_accessor.h
+-rw-r--r--   0        0        0     9513 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_attr.h
+-rw-r--r--   0        0        0     5471 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_call.h
+-rw-r--r--   0        0        0    17851 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_cast.h
+-rw-r--r--   0        0        0    25113 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_class.h
+-rw-r--r--   0        0        0     6232 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_defs.h
+-rw-r--r--   0        0        0     4129 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_descr.h
+-rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_enums.h
+-rw-r--r--   0        0        0     5207 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_error.h
+-rw-r--r--   0        0        0    10802 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_func.h
+-rw-r--r--   0        0        0    21272 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_lib.h
+-rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_misc.h
+-rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_python.h
+-rw-r--r--   0        0        0     7314 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_traits.h
+-rw-r--r--   0        0        0     2468 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_tuple.h
+-rw-r--r--   0        0        0    28452 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_types.h
+-rw-r--r--   0        0        0    20322 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/ndarray.h
+-rw-r--r--   0        0        0     7449 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/operators.h
+-rw-r--r--   0        0        0      535 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/array.h
+-rw-r--r--   0        0        0     5939 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/bind_map.h
+-rw-r--r--   0        0        0     7420 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/bind_vector.h
+-rw-r--r--   0        0        0     8673 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/chrono.h
+-rw-r--r--   0        0        0     2154 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/complex.h
+-rw-r--r--   0        0        0    10571 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/chrono.h
+-rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/nb_array.h
+-rw-r--r--   0        0        0     2904 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/nb_dict.h
+-rw-r--r--   0        0        0     2247 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/nb_list.h
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/nb_set.h
+-rw-r--r--   0        0        0     3219 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/traits.h
+-rw-r--r--   0        0        0     2719 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/filesystem.h
+-rw-r--r--   0        0        0     2477 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/function.h
+-rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/list.h
+-rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/map.h
+-rw-r--r--   0        0        0     2202 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/optional.h
+-rw-r--r--   0        0        0     2770 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/pair.h
+-rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/set.h
+-rw-r--r--   0        0        0     4820 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/shared_ptr.h
+-rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/string.h
+-rw-r--r--   0        0        0     1062 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/string_view.h
+-rw-r--r--   0        0        0     3307 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/tuple.h
+-rw-r--r--   0        0        0     4389 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/unique_ptr.h
+-rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/unordered_map.h
+-rw-r--r--   0        0        0      652 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/unordered_set.h
+-rw-r--r--   0        0        0     2776 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/variant.h
+-rw-r--r--   0        0        0      537 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/vector.h
+-rw-r--r--   0        0        0     2975 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/include/nanobind/trampoline.h
+-rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/pyproject.toml
+-rw-r--r--   0        0        0     3211 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/setup.py
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/__init__.py
+-rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/__main__.py
+-rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/buffer.h
+-rw-r--r--   0        0        0    30688 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/common.cpp
+-rw-r--r--   0        0        0     8851 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/error.cpp
+-rw-r--r--   0        0        0     1009 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/hash.h
+-rw-r--r--   0        0        0     2318 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/implicit.cpp
+-rw-r--r--   0        0        0    14686 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/nb_enum.cpp
+-rw-r--r--   0        0        0    40196 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/nb_func.cpp
+-rw-r--r--   0        0        0    15914 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/nb_internals.cpp
+-rw-r--r--   0        0        0    10614 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/nb_internals.h
+-rw-r--r--   0        0        0    24024 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/nb_ndarray.cpp
+-rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/nb_static_property.cpp
+-rw-r--r--   0        0        0    59202 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/nb_type.cpp
+-rw-r--r--   0        0        0     5144 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/src/trampoline.cpp
+-rw-r--r--   0        0        0     3562 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/common.py
+-rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/inter_module.cpp
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/inter_module.h
+-rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/object_py.h
+-rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_chrono.cpp
+-rw-r--r--   0        0        0    10852 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_chrono.py
+-rw-r--r--   0        0        0    18240 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_classes.cpp
+-rw-r--r--   0        0        0    20465 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_classes.py
+-rw-r--r--   0        0        0     9586 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_eigen.cpp
+-rw-r--r--   0        0        0    12097 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_eigen.py
+-rw-r--r--   0        0        0     2391 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_enum.cpp
+-rw-r--r--   0        0        0     5680 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_enum.py
+-rw-r--r--   0        0        0     2342 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_eval.cpp
+-rw-r--r--   0        0        0      893 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_eval.py
+-rw-r--r--   0        0        0     2579 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_exception.cpp
+-rw-r--r--   0        0        0     3301 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_exception.py
+-rw-r--r--   0        0        0     7965 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_functions.cpp
+-rw-r--r--   0        0        0     9820 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_functions.py
+-rw-r--r--   0        0        0     9373 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_holders.cpp
+-rw-r--r--   0        0        0    11149 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_holders.py
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_inter_module.py
+-rw-r--r--   0        0        0      170 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_inter_module_1.cpp
+-rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_inter_module_2.cpp
+-rw-r--r--   0        0        0     1884 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_intrusive.cpp
+-rw-r--r--   0        0        0     1281 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_intrusive.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_intrusive_impl.cpp
+-rw-r--r--   0        0        0     1845 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_issue.cpp
+-rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_issue.py
+-rw-r--r--   0        0        0     1741 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_make_iterator.cpp
+-rw-r--r--   0        0        0      816 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_make_iterator.py
+-rw-r--r--   0        0        0    11559 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_ndarray.cpp
+-rw-r--r--   0        0        0    18521 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_ndarray.py
+-rw-r--r--   0        0        0    15922 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_stl.cpp
+-rw-r--r--   0        0        0    24433 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_stl.py
+-rw-r--r--   0        0        0     2478 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_stl_bind_map.cpp
+-rw-r--r--   0        0        0     5597 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_stl_bind_map.py
+-rw-r--r--   0        0        0     1279 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_stl_bind_vector.cpp
+-rw-r--r--   0        0        0     4034 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/ext/nanobind/tests/test_stl_bind_vector.py
+-rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2268 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/Pipe.cpp
+-rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/Pipe.h
+-rw-r--r--   0        0        0      878 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/PipeClient.cpp
+-rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/PipeClient.h
+-rw-r--r--   0        0        0    10256 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/PipeConnection.cpp
+-rw-r--r--   0        0        0     2475 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/PipeConnection.h
+-rw-r--r--   0        0        0     3083 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/PipeListener.cpp
+-rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/PipeListener.h
+-rw-r--r--   0        0        0     2802 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/module.cpp
+-rw-r--r--   0        0        0      719 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/util.cpp
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/cpp/util.h
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/win32_pipes/__init__.py
+-rw-r--r--   0        0        0     1810 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/win32_pipes/_ext.pyi
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/src/win32_pipes/py.typed
+-rw-r--r--   0        0        0     5290 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/tests/test_pipes.py
+-rw-r--r--   0        0        0      138 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/tox.ini
+-rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 win32_pipes-0.2.2/PKG-INFO
```

### Comparing `win32_pipes-0.2.1/.github/workflows/wheels.yml` & `win32_pipes-0.2.2/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/.gitignore` & `win32_pipes-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/.pre-commit-config.yaml` & `win32_pipes-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/CMakeLists.txt` & `win32_pipes-0.2.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/LICENSE` & `win32_pipes-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/.github/ISSUE_TEMPLATE/all-other.yml` & `win32_pipes-0.2.2/ext/nanobind/.github/ISSUE_TEMPLATE/all-other.yml`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/.github/ISSUE_TEMPLATE/bug-report.yml` & `win32_pipes-0.2.2/ext/nanobind/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/.github/workflows/ci.yml` & `win32_pipes-0.2.2/ext/nanobind/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/CMakeLists.txt` & `win32_pipes-0.2.2/ext/nanobind/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/LICENSE` & `win32_pipes-0.2.2/ext/nanobind/LICENSE`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/README.md` & `win32_pipes-0.2.2/ext/nanobind/README.md`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/cmake/collect-symbols-pypy.py` & `win32_pipes-0.2.2/ext/nanobind/cmake/collect-symbols-pypy.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/cmake/collect-symbols.py` & `win32_pipes-0.2.2/ext/nanobind/cmake/collect-symbols.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/cmake/darwin-ld-cpython.sym` & `win32_pipes-0.2.2/ext/nanobind/cmake/darwin-ld-cpython.sym`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/cmake/darwin-ld-pypy.sym` & `win32_pipes-0.2.2/ext/nanobind/cmake/darwin-ld-pypy.sym`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/cmake/nanobind-config.cmake` & `win32_pipes-0.2.2/ext/nanobind/cmake/nanobind-config.cmake`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/api_cmake.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/api_cmake.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/api_core.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/api_core.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/api_extra.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/api_extra.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/basics.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/benchmark.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/building.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/building.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/changelog.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/classes.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/conf.py` & `win32_pipes-0.2.2/ext/nanobind/docs/conf.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/eigen.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/eigen.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/exceptions.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/exchanging.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/exchanging.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/faq.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/functions.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/functions.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/binding-dark.svg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/binding-dark.svg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/binding-light.svg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/binding-light.svg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/caster-dark.svg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/caster-dark.svg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/caster-light.svg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/caster-light.svg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/logo.jpg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/perf.svg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/perf.svg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/sizes.svg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/sizes.svg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/times.svg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/times.svg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/wrapper-dark.svg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/wrapper-dark.svg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/images/wrapper-light.svg` & `win32_pipes-0.2.2/ext/nanobind/docs/images/wrapper-light.svg`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/index.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/index.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/installing.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/lowlevel.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/lowlevel.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/microbenchmark.ipynb` & `win32_pipes-0.2.2/ext/nanobind/docs/microbenchmark.ipynb`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/ndarray.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/ndarray.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/ownership.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/ownership.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/ownership_adv.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/ownership_adv.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/packaging.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/packaging.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/porting.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/porting.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/pypy.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/pypy.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/release.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/release.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/typeslots.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/typeslots.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/utilities.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/docs/why.rst` & `win32_pipes-0.2.2/ext/nanobind/docs/why.rst`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/.github/workflows/ci.yml` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/CMakeLists.txt` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/LICENSE` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/LICENSE`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/README.md` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/README.md`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/doxygen.conf` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/doxygen.conf`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/include/tsl/robin_growth_policy.h` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/include/tsl/robin_growth_policy.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/include/tsl/robin_hash.h` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/include/tsl/robin_hash.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/include/tsl/robin_map.h` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/include/tsl/robin_map.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/include/tsl/robin_set.h` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/include/tsl/robin_set.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/CMakeLists.txt` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/custom_allocator_tests.cpp` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/custom_allocator_tests.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/main.cpp` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/main.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/policy_tests.cpp` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/policy_tests.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/robin_map_tests.cpp` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/robin_map_tests.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/robin_set_tests.cpp` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/robin_set_tests.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tests/utils.h` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tests/utils.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/ext/robin_map/tsl-robin-map.natvis` & `win32_pipes-0.2.2/ext/nanobind/ext/robin_map/tsl-robin-map.natvis`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/eigen/dense.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/eigen/dense.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/eigen/sparse.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/eigen/sparse.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/eval.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/eval.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/intrusive/counter.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/intrusive/counter.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/intrusive/counter.inl` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/intrusive/counter.inl`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/intrusive/ref.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/intrusive/ref.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/make_iterator.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/make_iterator.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nanobind.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nanobind.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_accessor.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_accessor.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_attr.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_attr.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_call.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_call.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_cast.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_cast.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_class.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_class.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_defs.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_defs.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_descr.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_descr.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_enums.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_enums.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_error.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_error.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_func.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_func.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_lib.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_lib.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_misc.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_misc.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_python.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_python.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_traits.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_traits.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_tuple.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_tuple.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/nb_types.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/nb_types.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/ndarray.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/ndarray.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/operators.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/operators.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/array.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/array.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/bind_map.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/bind_map.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/bind_vector.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/bind_vector.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/chrono.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/chrono.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/complex.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/complex.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/chrono.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/chrono.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/nb_array.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/nb_array.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/nb_dict.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/nb_dict.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/nb_list.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/nb_list.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/nb_set.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/nb_set.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/detail/traits.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/detail/traits.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/filesystem.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/function.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/function.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/list.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/list.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/map.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/map.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/optional.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/optional.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/pair.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/pair.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/set.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/set.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/shared_ptr.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/shared_ptr.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/string.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/string.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/string_view.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/string_view.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/tuple.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/tuple.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/unique_ptr.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/unique_ptr.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/unordered_map.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/unordered_map.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/unordered_set.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/unordered_set.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/variant.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/variant.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/stl/vector.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/stl/vector.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/include/nanobind/trampoline.h` & `win32_pipes-0.2.2/ext/nanobind/include/nanobind/trampoline.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/setup.py` & `win32_pipes-0.2.2/ext/nanobind/setup.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/__init__.py` & `win32_pipes-0.2.2/ext/nanobind/src/__init__.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/__main__.py` & `win32_pipes-0.2.2/ext/nanobind/src/__main__.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/buffer.h` & `win32_pipes-0.2.2/ext/nanobind/src/buffer.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/common.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/common.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/error.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/error.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/hash.h` & `win32_pipes-0.2.2/ext/nanobind/src/hash.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/implicit.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/implicit.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/nb_enum.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/nb_enum.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/nb_func.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/nb_func.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/nb_internals.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/nb_internals.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/nb_internals.h` & `win32_pipes-0.2.2/ext/nanobind/src/nb_internals.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/nb_ndarray.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/nb_ndarray.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/nb_static_property.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/nb_static_property.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/nb_type.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/nb_type.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/src/trampoline.cpp` & `win32_pipes-0.2.2/ext/nanobind/src/trampoline.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/CMakeLists.txt` & `win32_pipes-0.2.2/ext/nanobind/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/object_py.h` & `win32_pipes-0.2.2/ext/nanobind/tests/object_py.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_chrono.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_chrono.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_classes.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_classes.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_classes.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_eigen.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_eigen.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_enum.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_enum.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_eval.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_eval.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_exception.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_exception.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_exception.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_functions.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_functions.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_functions.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_holders.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_holders.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_holders.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_holders.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_intrusive.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_intrusive.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_intrusive.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_intrusive.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_issue.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_issue.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_issue.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_make_iterator.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_make_iterator.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_make_iterator.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_make_iterator.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_ndarray.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_ndarray.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_ndarray.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_ndarray.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_stl.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_stl.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_stl_bind_map.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_stl_bind_map.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_stl_bind_map.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_stl_bind_map.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_stl_bind_vector.cpp` & `win32_pipes-0.2.2/ext/nanobind/tests/test_stl_bind_vector.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/ext/nanobind/tests/test_stl_bind_vector.py` & `win32_pipes-0.2.2/ext/nanobind/tests/test_stl_bind_vector.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/pyproject.toml` & `win32_pipes-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core>=0.8.2"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "win32_pipes"
-version = "0.2.1"
+version = "0.2.2"
 description="A non-blocking C++ NamedPipe implementation for Windows."
 readme = "README.md"
 authors = [
   { name = "Artur Drogunow", email = "Artur.Drogunow@zf.com" },
 ]
 requires-python = ">=3.8"
 license = { text = "MIT" }
@@ -37,14 +37,19 @@
 dev = [
   "tox",
   "pre-commit",
   "pipx",
   "ruff",
 ]
 
+[tool.scikit-build]
+wheel.packages = ["src/win32_pipes"]
+wheel.py-api = "cp312"
+cmake.version = ">=3.26.1"
+
 [tool.cibuildwheel]
 test-requires = "pytest"
 test-command = "pytest --no-header -vv {project}/tests"
 build-frontend = "build"
 skip = "pp*"
 
 [tool.pytest.ini_options]
```

### Comparing `win32_pipes-0.2.1/src/cpp/Pipe.cpp` & `win32_pipes-0.2.2/src/cpp/Pipe.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/src/cpp/PipeClient.cpp` & `win32_pipes-0.2.2/src/cpp/PipeClient.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/src/cpp/PipeConnection.cpp` & `win32_pipes-0.2.2/src/cpp/PipeConnection.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/src/cpp/PipeConnection.h` & `win32_pipes-0.2.2/src/cpp/PipeConnection.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/src/cpp/PipeListener.cpp` & `win32_pipes-0.2.2/src/cpp/PipeListener.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/src/cpp/PipeListener.h` & `win32_pipes-0.2.2/src/cpp/PipeListener.h`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/src/cpp/module.cpp` & `win32_pipes-0.2.2/src/cpp/module.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/src/cpp/util.cpp` & `win32_pipes-0.2.2/src/cpp/util.cpp`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/src/win32_pipes/__init__.py` & `win32_pipes-0.2.2/src/win32_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `win32_pipes-0.2.1/src/win32_pipes/_ext.pyi` & `win32_pipes-0.2.2/src/win32_pipes/_ext.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2024-present Artur Drogunow <artur.drogunow@zf.com>
+#
+# SPDX-License-Identifier: MIT
+
 from contextlib import AbstractContextManager
 from types import TracebackType
 from typing import Self
 
 __version__: str
 
 class PipeConnection(AbstractContextManager[PipeConnection]):
```

### Comparing `win32_pipes-0.2.1/tests/test_pipes.py` & `win32_pipes-0.2.2/tests/test_pipes.py`

 * *Files identical despite different names*

