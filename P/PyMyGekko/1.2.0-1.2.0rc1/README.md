# Comparing `tmp/pymygekko-1.2.0.tar.gz` & `tmp/pymygekko-1.2.0rc1.tar.gz`

## Comparing `pymygekko-1.2.0.tar` & `pymygekko-1.2.0rc1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymygekko-1.2.0/.DS_Store
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pymygekko-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pymygekko-1.2.0/setup.cfg
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pymygekko-1.2.0/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 pymygekko-1.2.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/__about__.py
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/__init__.py
--rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/api_var_demo_data.json
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/api_var_status_demo_data.json
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/data_provider.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/Actions.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/AlarmsLogics.py
--rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/Blinds.py
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/EnergyCosts.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/HotWaterSystems.py
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/Lights.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/Loads.py
--rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/RoomTemps.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/__init__.py
--rw-r--r--   0        0        0    14574 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PyMyGekko/resources/vents.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/api_var_status_response_slidejson
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/test_pymygekko.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/actions/test_pymygekko_actions_596610.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/actions/test_pymygekko_actions_680016.py
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/actions/data/api_var_response_596610.json
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/actions/data/api_var_response_680016.json
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/actions/data/api_var_status_response_596610.json
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/actions/data/api_var_status_response_680016.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/alarms_logics/test_pymygekko_alarms_logics_596610.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/alarms_logics/test_pymygekko_alarms_logics_680016.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/alarms_logics/data/api_var_response_596610.json
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/alarms_logics/data/api_var_response_680016.json
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/alarms_logics/data/api_var_status_response_596610.json
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/alarms_logics/data/api_var_status_response_680016.json
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/blinds/test_pymygekko_blinds_596610.py
--rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/blinds/test_pymygekko_blinds_680016.py
--rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/blinds/data/api_var_response_596610.json
--rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/blinds/data/api_var_response_680016.json
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/blinds/data/api_var_status_response_596610.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/blinds/data/api_var_status_response_680016.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/energy_costs/test_pymygekko_energy_costs_596610.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/energy_costs/test_pymygekko_energy_costs_643612.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/energy_costs/test_pymygekko_energy_costs_slide.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/energy_costs/data/api_var_response_596610.json
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/energy_costs/data/api_var_response_643612.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/energy_costs/data/api_var_response_slide.json
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/energy_costs/data/api_var_status_response_596610.json
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/energy_costs/data/api_var_status_response_643612.json
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/energy_costs/data/api_var_status_response_slide.json
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/global_networks/api_var_response.json
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/global_networks/api_var_status_response.json
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/global_networks/test_pymygekko_global_networks.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/hotwater_systems/test_pymygekko_hotwater_systems_596610.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/hotwater_systems/test_pymygekko_hotwater_systems_680016.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/hotwater_systems/data/api_var_response_596610.json
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/hotwater_systems/data/api_var_response_680016.json
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/hotwater_systems/data/api_var_status_response_596610.json
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/hotwater_systems/data/api_var_status_response_680016.json
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/lights/test_pymygekko_lights_596610.py
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/lights/test_pymygekko_lights_680016.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/lights/data/api_var_response_596610.json
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/lights/data/api_var_response_680016.json
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/lights/data/api_var_status_response_596610.json
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/lights/data/api_var_status_response_680016.json
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/loads/test_pymygekko_loads_680016.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/loads/data/api_var_response_680016.json
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/loads/data/api_var_status_response_680016.json
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/test_pymygekko_room_temps_596610.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/test_pymygekko_room_temps_680016.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/test_pymygekko_room_temps_713511.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/test_pymygekko_room_temps_slide.py
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/data/api_var_response_596610.json
--rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/data/api_var_response_680016.json
--rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/data/api_var_response_713511.json
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/data/api_var_response_slide.json
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/data/api_var_status_response_596610.json
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/data/api_var_status_response_680016.json
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/data/api_var_status_response_713511.json
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/room_temps/data/api_var_status_response_slide.json
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/vents/test_pymygekko_vents_596610.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/vents/test_pymygekko_vents_680016.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/vents/test_pymygekko_vents_slide.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/vents/data/api_var_response_596610.json
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/vents/data/api_var_response_680016.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/vents/data/api_var_response_slide.json
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/vents/data/api_var_status_response_596610.json
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/vents/data/api_var_status_response_680016.json
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pymygekko-1.2.0/tests/vents/data/api_var_status_response_slide.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 pymygekko-1.2.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pymygekko-1.2.0/LICENSE
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pymygekko-1.2.0/README.md
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pymygekko-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pymygekko-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/.DS_Store
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/setup.cfg
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/__about__.py
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/__init__.py
+-rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/api_var_demo_data.json
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/api_var_status_demo_data.json
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/data_provider.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/Actions.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/AlarmsLogics.py
+-rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/Blinds.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/EnergyCosts.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/HotWaterSystems.py
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/Lights.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/Loads.py
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/RoomTemps.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/__init__.py
+-rw-r--r--   0        0        0    14574 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PyMyGekko/resources/vents.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/api_var_status_response_slidejson
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/test_pymygekko.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/actions/test_pymygekko_actions_596610.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/actions/test_pymygekko_actions_680016.py
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/actions/data/api_var_response_596610.json
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/actions/data/api_var_response_680016.json
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/actions/data/api_var_status_response_596610.json
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/actions/data/api_var_status_response_680016.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/alarms_logics/test_pymygekko_alarms_logics_596610.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/alarms_logics/test_pymygekko_alarms_logics_680016.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/alarms_logics/data/api_var_response_596610.json
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/alarms_logics/data/api_var_response_680016.json
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/alarms_logics/data/api_var_status_response_596610.json
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/alarms_logics/data/api_var_status_response_680016.json
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/blinds/test_pymygekko_blinds_596610.py
+-rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/blinds/test_pymygekko_blinds_680016.py
+-rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/blinds/data/api_var_response_596610.json
+-rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/blinds/data/api_var_response_680016.json
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/blinds/data/api_var_status_response_596610.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/blinds/data/api_var_status_response_680016.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/energy_costs/test_pymygekko_energy_costs_596610.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/energy_costs/test_pymygekko_energy_costs_643612.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/energy_costs/test_pymygekko_energy_costs_slide.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_response_596610.json
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_response_643612.json
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_response_slide.json
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_status_response_596610.json
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_status_response_643612.json
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_status_response_slide.json
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/global_networks/api_var_response.json
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/global_networks/api_var_status_response.json
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/global_networks/test_pymygekko_global_networks.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/hotwater_systems/test_pymygekko_hotwater_systems_596610.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/hotwater_systems/test_pymygekko_hotwater_systems_680016.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/hotwater_systems/data/api_var_response_596610.json
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/hotwater_systems/data/api_var_response_680016.json
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/hotwater_systems/data/api_var_status_response_596610.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/hotwater_systems/data/api_var_status_response_680016.json
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/lights/test_pymygekko_lights_596610.py
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/lights/test_pymygekko_lights_680016.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/lights/data/api_var_response_596610.json
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/lights/data/api_var_response_680016.json
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/lights/data/api_var_status_response_596610.json
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/lights/data/api_var_status_response_680016.json
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/loads/test_pymygekko_loads_680016.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/loads/data/api_var_response_680016.json
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/loads/data/api_var_status_response_680016.json
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/test_pymygekko_room_temps_596610.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/test_pymygekko_room_temps_680016.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/test_pymygekko_room_temps_713511.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/test_pymygekko_room_temps_slide.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/data/api_var_response_596610.json
+-rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/data/api_var_response_680016.json
+-rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/data/api_var_response_713511.json
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/data/api_var_response_slide.json
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/data/api_var_status_response_596610.json
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/data/api_var_status_response_680016.json
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/data/api_var_status_response_713511.json
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/room_temps/data/api_var_status_response_slide.json
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/vents/test_pymygekko_vents_596610.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/vents/test_pymygekko_vents_680016.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/vents/test_pymygekko_vents_slide.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/vents/data/api_var_response_596610.json
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/vents/data/api_var_response_680016.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/vents/data/api_var_response_slide.json
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/vents/data/api_var_status_response_596610.json
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/vents/data/api_var_status_response_680016.json
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/tests/vents/data/api_var_status_response_slide.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/LICENSE
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/README.md
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 pymygekko-1.2.0rc1/PKG-INFO
```

### Comparing `pymygekko-1.2.0/.DS_Store` & `pymygekko-1.2.0rc1/.DS_Store`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/.pre-commit-config.yaml` & `pymygekko-1.2.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/.github/workflows/python-package.yml` & `pymygekko-1.2.0rc1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/__init__.py` & `pymygekko-1.2.0rc1/PyMyGekko/__init__.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/api_var_demo_data.json` & `pymygekko-1.2.0rc1/PyMyGekko/api_var_demo_data.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/api_var_status_demo_data.json` & `pymygekko-1.2.0rc1/PyMyGekko/api_var_status_demo_data.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/data_provider.py` & `pymygekko-1.2.0rc1/PyMyGekko/data_provider.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/Actions.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/Actions.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/AlarmsLogics.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/AlarmsLogics.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/Blinds.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/Blinds.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/EnergyCosts.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/EnergyCosts.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/HotWaterSystems.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/HotWaterSystems.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/Lights.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/Lights.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/Loads.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/Loads.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/RoomTemps.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/RoomTemps.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/__init__.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/PyMyGekko/resources/vents.py` & `pymygekko-1.2.0rc1/PyMyGekko/resources/vents.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/api_var_status_response_slidejson` & `pymygekko-1.2.0rc1/tests/api_var_status_response_slidejson`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/test_pymygekko.py` & `pymygekko-1.2.0rc1/tests/test_pymygekko.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/actions/test_pymygekko_actions_596610.py` & `pymygekko-1.2.0rc1/tests/actions/test_pymygekko_actions_596610.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/actions/test_pymygekko_actions_680016.py` & `pymygekko-1.2.0rc1/tests/actions/test_pymygekko_actions_680016.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/actions/data/api_var_response_596610.json` & `pymygekko-1.2.0rc1/tests/actions/data/api_var_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/actions/data/api_var_response_680016.json` & `pymygekko-1.2.0rc1/tests/actions/data/api_var_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/actions/data/api_var_status_response_596610.json` & `pymygekko-1.2.0rc1/tests/actions/data/api_var_status_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/actions/data/api_var_status_response_680016.json` & `pymygekko-1.2.0rc1/tests/actions/data/api_var_status_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/alarms_logics/test_pymygekko_alarms_logics_596610.py` & `pymygekko-1.2.0rc1/tests/alarms_logics/test_pymygekko_alarms_logics_596610.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/alarms_logics/test_pymygekko_alarms_logics_680016.py` & `pymygekko-1.2.0rc1/tests/alarms_logics/test_pymygekko_alarms_logics_680016.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/alarms_logics/data/api_var_response_596610.json` & `pymygekko-1.2.0rc1/tests/alarms_logics/data/api_var_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/alarms_logics/data/api_var_response_680016.json` & `pymygekko-1.2.0rc1/tests/alarms_logics/data/api_var_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/alarms_logics/data/api_var_status_response_596610.json` & `pymygekko-1.2.0rc1/tests/alarms_logics/data/api_var_status_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/alarms_logics/data/api_var_status_response_680016.json` & `pymygekko-1.2.0rc1/tests/alarms_logics/data/api_var_status_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/blinds/test_pymygekko_blinds_596610.py` & `pymygekko-1.2.0rc1/tests/blinds/test_pymygekko_blinds_596610.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/blinds/test_pymygekko_blinds_680016.py` & `pymygekko-1.2.0rc1/tests/blinds/test_pymygekko_blinds_680016.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/blinds/data/api_var_response_596610.json` & `pymygekko-1.2.0rc1/tests/blinds/data/api_var_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/blinds/data/api_var_response_680016.json` & `pymygekko-1.2.0rc1/tests/blinds/data/api_var_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/blinds/data/api_var_status_response_596610.json` & `pymygekko-1.2.0rc1/tests/blinds/data/api_var_status_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/blinds/data/api_var_status_response_680016.json` & `pymygekko-1.2.0rc1/tests/blinds/data/api_var_status_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/energy_costs/test_pymygekko_energy_costs_596610.py` & `pymygekko-1.2.0rc1/tests/energy_costs/test_pymygekko_energy_costs_596610.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/energy_costs/test_pymygekko_energy_costs_643612.py` & `pymygekko-1.2.0rc1/tests/energy_costs/test_pymygekko_energy_costs_643612.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/energy_costs/test_pymygekko_energy_costs_slide.py` & `pymygekko-1.2.0rc1/tests/energy_costs/test_pymygekko_energy_costs_slide.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/energy_costs/data/api_var_response_596610.json` & `pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/energy_costs/data/api_var_response_643612.json` & `pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_response_643612.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/energy_costs/data/api_var_response_slide.json` & `pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_response_slide.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/energy_costs/data/api_var_status_response_596610.json` & `pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_status_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/energy_costs/data/api_var_status_response_643612.json` & `pymygekko-1.2.0rc1/tests/energy_costs/data/api_var_status_response_643612.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/global_networks/api_var_response.json` & `pymygekko-1.2.0rc1/tests/global_networks/api_var_response.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/global_networks/test_pymygekko_global_networks.py` & `pymygekko-1.2.0rc1/tests/global_networks/test_pymygekko_global_networks.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/hotwater_systems/test_pymygekko_hotwater_systems_596610.py` & `pymygekko-1.2.0rc1/tests/hotwater_systems/test_pymygekko_hotwater_systems_596610.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/hotwater_systems/test_pymygekko_hotwater_systems_680016.py` & `pymygekko-1.2.0rc1/tests/hotwater_systems/test_pymygekko_hotwater_systems_680016.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/hotwater_systems/data/api_var_response_596610.json` & `pymygekko-1.2.0rc1/tests/hotwater_systems/data/api_var_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/hotwater_systems/data/api_var_response_680016.json` & `pymygekko-1.2.0rc1/tests/hotwater_systems/data/api_var_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/lights/test_pymygekko_lights_596610.py` & `pymygekko-1.2.0rc1/tests/lights/test_pymygekko_lights_596610.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/lights/test_pymygekko_lights_680016.py` & `pymygekko-1.2.0rc1/tests/lights/test_pymygekko_lights_680016.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/lights/data/api_var_response_596610.json` & `pymygekko-1.2.0rc1/tests/lights/data/api_var_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/lights/data/api_var_response_680016.json` & `pymygekko-1.2.0rc1/tests/lights/data/api_var_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/lights/data/api_var_status_response_596610.json` & `pymygekko-1.2.0rc1/tests/lights/data/api_var_status_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/lights/data/api_var_status_response_680016.json` & `pymygekko-1.2.0rc1/tests/lights/data/api_var_status_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/loads/test_pymygekko_loads_680016.py` & `pymygekko-1.2.0rc1/tests/loads/test_pymygekko_loads_680016.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/loads/data/api_var_response_680016.json` & `pymygekko-1.2.0rc1/tests/loads/data/api_var_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/loads/data/api_var_status_response_680016.json` & `pymygekko-1.2.0rc1/tests/loads/data/api_var_status_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/test_pymygekko_room_temps_596610.py` & `pymygekko-1.2.0rc1/tests/room_temps/test_pymygekko_room_temps_596610.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/test_pymygekko_room_temps_680016.py` & `pymygekko-1.2.0rc1/tests/room_temps/test_pymygekko_room_temps_680016.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/test_pymygekko_room_temps_713511.py` & `pymygekko-1.2.0rc1/tests/room_temps/test_pymygekko_room_temps_713511.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/test_pymygekko_room_temps_slide.py` & `pymygekko-1.2.0rc1/tests/room_temps/test_pymygekko_room_temps_slide.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/data/api_var_response_596610.json` & `pymygekko-1.2.0rc1/tests/room_temps/data/api_var_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/data/api_var_response_680016.json` & `pymygekko-1.2.0rc1/tests/room_temps/data/api_var_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/data/api_var_response_713511.json` & `pymygekko-1.2.0rc1/tests/room_temps/data/api_var_response_713511.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/data/api_var_response_slide.json` & `pymygekko-1.2.0rc1/tests/room_temps/data/api_var_response_slide.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/data/api_var_status_response_596610.json` & `pymygekko-1.2.0rc1/tests/room_temps/data/api_var_status_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/data/api_var_status_response_680016.json` & `pymygekko-1.2.0rc1/tests/room_temps/data/api_var_status_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/data/api_var_status_response_713511.json` & `pymygekko-1.2.0rc1/tests/room_temps/data/api_var_status_response_713511.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/room_temps/data/api_var_status_response_slide.json` & `pymygekko-1.2.0rc1/tests/room_temps/data/api_var_status_response_slide.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/vents/test_pymygekko_vents_596610.py` & `pymygekko-1.2.0rc1/tests/vents/test_pymygekko_vents_596610.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/vents/test_pymygekko_vents_680016.py` & `pymygekko-1.2.0rc1/tests/vents/test_pymygekko_vents_680016.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/vents/test_pymygekko_vents_slide.py` & `pymygekko-1.2.0rc1/tests/vents/test_pymygekko_vents_slide.py`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/vents/data/api_var_response_596610.json` & `pymygekko-1.2.0rc1/tests/vents/data/api_var_response_596610.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/vents/data/api_var_response_680016.json` & `pymygekko-1.2.0rc1/tests/vents/data/api_var_response_680016.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/tests/vents/data/api_var_response_slide.json` & `pymygekko-1.2.0rc1/tests/vents/data/api_var_response_slide.json`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/.gitignore` & `pymygekko-1.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/LICENSE` & `pymygekko-1.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymygekko-1.2.0/README.md` & `pymygekko-1.2.0rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 ```
 
 ## Usage
 
 ```python
 from aiohttp import ClientSession
 
-from PyMyGekko import MyGekkoQueryApiClient
+from PyMyGekko import MyGekkoApiClient
 from PyMyGekko.resources.Lights import LightState
 
 async with ClientSession() as session:
-    api = MyGekkoQueryApiClient(
+    api = MyGekkoApiClient(
         "USERNAME",
         "APIKEY",
         "GEKKOID",
         session,
     )
 
     await api.read_data()
```

### Comparing `pymygekko-1.2.0/pyproject.toml` & `pymygekko-1.2.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 requires-python = ">=3.10"
 license = "MIT"
 keywords = ['mygekko']
 authors = [
   { name = "Stephan Uhle", email = "stephanu@gmx.net" },
 ]
 classifiers = [
-  "Development Status :: 5 - Production/Stable",
-  "Intended Audience :: Developers",
+  "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
  "aiohttp >= 3.8"
  ]
 dynamic = ["version"]
```

### Comparing `pymygekko-1.2.0/PKG-INFO` & `pymygekko-1.2.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: PyMyGekko
-Version: 1.2.0
+Version: 1.2.0rc1
 Summary: Python Library to access the myGEKKO Query API.
 Project-URL: Documentation, https://github.com/StephanU/#readme
 Project-URL: Issues, https://github.com/StephanU/PyMyGekko/issues
 Project-URL: Source, https://github.com/StephanU/PyMyGekko
 Author-email: Stephan Uhle <stephanu@gmx.net>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: mygekko
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: aiohttp>=3.8
 Description-Content-Type: text/markdown
 
 # PyMyGekko
@@ -43,19 +41,19 @@
 ```
 
 ## Usage
 
 ```python
 from aiohttp import ClientSession
 
-from PyMyGekko import MyGekkoQueryApiClient
+from PyMyGekko import MyGekkoApiClient
 from PyMyGekko.resources.Lights import LightState
 
 async with ClientSession() as session:
-    api = MyGekkoQueryApiClient(
+    api = MyGekkoApiClient(
         "USERNAME",
         "APIKEY",
         "GEKKOID",
         session,
     )
 
     await api.read_data()
```

