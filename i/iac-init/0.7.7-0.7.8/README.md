# Comparing `tmp/iac_init-0.7.7.tar.gz` & `tmp/iac_init-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.7.7.tar", max compression
+gzip compressed data, was "iac_init-0.7.8.tar", max compression
```

## Comparing `iac_init-0.7.7.tar` & `iac_init-0.7.8.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    16295 2024-05-19 10:12:06.580417 iac_init-0.7.7/LICENSE
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.580417 iac_init-0.7.7/README.md
--rw-r--r--   0        0        0      392 2024-05-19 10:12:06.580417 iac_init-0.7.7/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-19 10:12:06.580417 iac_init-0.7.7/iac_init/__main__.py
--rwxr-xr-x   0        0        0   727800 2024-05-19 10:12:21.944455 iac_init-0.7.7/iac_init/cli/main.so
--rwxr-xr-x   0        0        0    69824 2024-05-19 10:12:22.164456 iac_init-0.7.7/iac_init/cli/options.so
--rw-r--r--   0        0        0     1827 2024-05-19 10:12:06.580417 iac_init-0.7.7/iac_init/conf/__init__.py
--rwxr-xr-x   0        0        0   176224 2024-05-19 10:12:22.724457 iac_init-0.7.7/iac_init/conf/global_settings.so
--rwxr-xr-x   0        0        0   246168 2024-05-19 10:12:26.488464 iac_init-0.7.7/iac_init/scripts/ansible_tool.so
--rwxr-xr-x   0        0        0   294536 2024-05-19 10:12:27.900467 iac_init-0.7.7/iac_init/scripts/apic_connecton_tool.so
--rwxr-xr-x   0        0        0   675792 2024-05-19 10:12:25.212462 iac_init-0.7.7/iac_init/scripts/cimc_precheck_tool.so
--rwxr-xr-x   0        0        0   168632 2024-05-19 10:12:28.436469 iac_init-0.7.7/iac_init/scripts/ssh_tool.so
--rwxr-xr-x   0        0        0   137000 2024-05-19 10:12:26.904465 iac_init-0.7.7/iac_init/scripts/telnet_tool.so
--rwxr-xr-x   0        0        0   156336 2024-05-19 10:12:25.696463 iac_init-0.7.7/iac_init/scripts/thread_tool.so
--rw-r--r--   0        0        0     3778 2024-05-19 10:12:06.580417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-19 10:12:06.580417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-19 10:12:06.580417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-19 10:12:06.580417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-19 10:12:06.580417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.584417 iac_init-0.7.7/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 10:12:06.588417 iac_init-0.7.7/iac_init/templates/12-config_backup/inventory.yaml.j2
--rwxr-xr-x   0        0        0    62360 2024-05-19 10:12:13.748434 iac_init-0.7.7/iac_init/utils/exceptions.so
--rwxr-xr-x   0        0        0   333200 2024-05-19 10:12:13.560433 iac_init-0.7.7/iac_init/utils/functional.so
--rwxr-xr-x   0        0        0   932744 2024-05-19 10:12:12.504430 iac_init-0.7.7/iac_init/validator.so
--rwxr-xr-x   0        0        0   503352 2024-05-19 10:12:15.512440 iac_init-0.7.7/iac_init/yaml_conf/yaml.so
--rwxr-xr-x   0        0        0   600936 2024-05-19 10:12:17.924447 iac_init-0.7.7/iac_init/yaml_conf/yaml_writer.so
--rw-r--r--   0        0        0     1636 2024-05-19 10:12:06.592417 iac_init-0.7.7/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-19 11:13:18.242629 iac_init-0.7.8/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.242629 iac_init-0.7.8/README.md
+-rw-r--r--   0        0        0      392 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/__main__.py
+-rwxr-xr-x   0        0        0   727800 2024-05-19 11:13:36.934588 iac_init-0.7.8/iac_init/cli/main.so
+-rwxr-xr-x   0        0        0    69824 2024-05-19 11:13:37.166587 iac_init-0.7.8/iac_init/cli/options.so
+-rw-r--r--   0        0        0     1827 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/conf/__init__.py
+-rwxr-xr-x   0        0        0   176224 2024-05-19 11:13:37.738586 iac_init-0.7.8/iac_init/conf/global_settings.so
+-rwxr-xr-x   0        0        0   246168 2024-05-19 11:13:41.526575 iac_init-0.7.8/iac_init/scripts/ansible_tool.so
+-rwxr-xr-x   0        0        0   294536 2024-05-19 11:13:42.974572 iac_init-0.7.8/iac_init/scripts/apic_connecton_tool.so
+-rwxr-xr-x   0        0        0   675792 2024-05-19 11:13:40.234579 iac_init-0.7.8/iac_init/scripts/cimc_precheck_tool.so
+-rwxr-xr-x   0        0        0   168632 2024-05-19 11:13:43.518570 iac_init-0.7.8/iac_init/scripts/ssh_tool.so
+-rwxr-xr-x   0        0        0   137000 2024-05-19 11:13:41.958574 iac_init-0.7.8/iac_init/scripts/telnet_tool.so
+-rwxr-xr-x   0        0        0   156336 2024-05-19 11:13:40.722578 iac_init-0.7.8/iac_init/scripts/thread_tool.so
+-rw-r--r--   0        0        0     3778 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-19 11:13:18.242629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.246629 iac_init-0.7.8/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 11:13:18.250630 iac_init-0.7.8/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rwxr-xr-x   0        0        0    62360 2024-05-19 11:13:28.286607 iac_init-0.7.8/iac_init/utils/exceptions.so
+-rwxr-xr-x   0        0        0   333200 2024-05-19 11:13:28.094607 iac_init-0.7.8/iac_init/utils/functional.so
+-rwxr-xr-x   0        0        0   932744 2024-05-19 11:13:27.002606 iac_init-0.7.8/iac_init/validator.so
+-rwxr-xr-x   0        0        0   503352 2024-05-19 11:13:30.074608 iac_init-0.7.8/iac_init/yaml_conf/yaml.so
+-rwxr-xr-x   0        0        0   600936 2024-05-19 11:13:32.614600 iac_init-0.7.8/iac_init/yaml_conf/yaml_writer.so
+-rw-r--r--   0        0        0     1636 2024-05-19 11:13:18.250630 iac_init-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.7.8/PKG-INFO
```

### Comparing `iac_init-0.7.7/LICENSE` & `iac_init-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/cli/main.so` & `iac_init-0.7.8/iac_init/cli/main.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/cli/options.so` & `iac_init-0.7.8/iac_init/cli/options.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/conf/__init__.py` & `iac_init-0.7.8/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/conf/global_settings.so` & `iac_init-0.7.8/iac_init/conf/global_settings.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/scripts/ansible_tool.so` & `iac_init-0.7.8/iac_init/scripts/ansible_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/scripts/apic_connecton_tool.so` & `iac_init-0.7.8/iac_init/scripts/apic_connecton_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/scripts/cimc_precheck_tool.so` & `iac_init-0.7.8/iac_init/scripts/cimc_precheck_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/scripts/ssh_tool.so` & `iac_init-0.7.8/iac_init/scripts/ssh_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/scripts/telnet_tool.so` & `iac_init-0.7.8/iac_init/scripts/telnet_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/scripts/thread_tool.so` & `iac_init-0.7.8/iac_init/scripts/thread_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.7.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.7.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/utils/exceptions.so` & `iac_init-0.7.8/iac_init/utils/exceptions.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/utils/functional.so` & `iac_init-0.7.8/iac_init/utils/functional.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/validator.so` & `iac_init-0.7.8/iac_init/validator.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/yaml_conf/yaml.so` & `iac_init-0.7.8/iac_init/yaml_conf/yaml.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/iac_init/yaml_conf/yaml_writer.so` & `iac_init-0.7.8/iac_init/yaml_conf/yaml_writer.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.7/pyproject.toml` & `iac_init-0.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.7.7"
+version = "0.7.8"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.7.7/PKG-INFO` & `iac_init-0.7.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.7.7
+Version: 0.7.8
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

