# Comparing `tmp/iac_init-0.7.4.tar.gz` & `tmp/iac_init-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.7.4.tar", max compression
+gzip compressed data, was "iac_init-0.7.5.tar", max compression
```

## Comparing `iac_init-0.7.4.tar` & `iac_init-0.7.5.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    16295 2024-05-19 07:49:30.575019 iac_init-0.7.4/LICENSE
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.575019 iac_init-0.7.4/README.md
--rw-r--r--   0        0        0      392 2024-05-19 07:49:30.575019 iac_init-0.7.4/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-19 07:49:30.575019 iac_init-0.7.4/iac_init/__main__.py
--rwxr-xr-x   0        0        0   727800 2024-05-19 07:49:45.935159 iac_init-0.7.4/iac_init/cli/main.so
--rwxr-xr-x   0        0        0    69824 2024-05-19 07:49:46.159161 iac_init-0.7.4/iac_init/cli/options.so
--rw-r--r--   0        0        0     1820 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/conf/__init__.py
--rwxr-xr-x   0        0        0   176224 2024-05-19 07:49:46.723165 iac_init-0.7.4/iac_init/conf/global_settings.so
--rwxr-xr-x   0        0        0   246168 2024-05-19 07:49:50.475196 iac_init-0.7.4/iac_init/scripts/ansible_tool.so
--rwxr-xr-x   0        0        0   294536 2024-05-19 07:49:51.895208 iac_init-0.7.4/iac_init/scripts/apic_connecton_tool.so
--rwxr-xr-x   0        0        0   675792 2024-05-19 07:49:49.203186 iac_init-0.7.4/iac_init/scripts/cimc_precheck_tool.so
--rwxr-xr-x   0        0        0   168632 2024-05-19 07:49:52.431213 iac_init-0.7.4/iac_init/scripts/ssh_tool.so
--rwxr-xr-x   0        0        0   137000 2024-05-19 07:49:50.899200 iac_init-0.7.4/iac_init/scripts/telnet_tool.so
--rwxr-xr-x   0        0        0   156336 2024-05-19 07:49:49.683190 iac_init-0.7.4/iac_init/scripts/thread_tool.so
--rw-r--r--   0        0        0     3778 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.579019 iac_init-0.7.4/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-19 07:49:30.583019 iac_init-0.7.4/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-19 07:49:30.587019 iac_init-0.7.4/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-19 07:49:30.587019 iac_init-0.7.4/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-19 07:49:30.587019 iac_init-0.7.4/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-19 07:49:30.587019 iac_init-0.7.4/iac_init/templates/12-config_backup/inventory.yaml.j2
--rwxr-xr-x   0        0        0    62360 2024-05-19 07:49:37.679081 iac_init-0.7.4/iac_init/utils/exceptions.so
--rwxr-xr-x   0        0        0   333200 2024-05-19 07:49:37.491079 iac_init-0.7.4/iac_init/utils/functional.so
--rwxr-xr-x   0        0        0   935456 2024-05-19 07:49:36.411069 iac_init-0.7.4/iac_init/validator.so
--rwxr-xr-x   0        0        0   503352 2024-05-19 07:49:39.435097 iac_init-0.7.4/iac_init/yaml_conf/yaml.so
--rwxr-xr-x   0        0        0   600936 2024-05-19 07:49:41.863117 iac_init-0.7.4/iac_init/yaml_conf/yaml_writer.so
--rw-r--r--   0        0        0     1636 2024-05-19 07:49:30.587019 iac_init-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-19 07:54:39.497074 iac_init-0.7.5/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.497074 iac_init-0.7.5/README.md
+-rw-r--r--   0        0        0      392 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/__main__.py
+-rwxr-xr-x   0        0        0   727800 2024-05-19 07:54:54.685128 iac_init-0.7.5/iac_init/cli/main.so
+-rwxr-xr-x   0        0        0    69824 2024-05-19 07:54:54.901129 iac_init-0.7.5/iac_init/cli/options.so
+-rw-r--r--   0        0        0     1827 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/conf/__init__.py
+-rwxr-xr-x   0        0        0   176224 2024-05-19 07:54:55.461131 iac_init-0.7.5/iac_init/conf/global_settings.so
+-rwxr-xr-x   0        0        0   246168 2024-05-19 07:54:59.169142 iac_init-0.7.5/iac_init/scripts/ansible_tool.so
+-rwxr-xr-x   0        0        0   294536 2024-05-19 07:55:00.573147 iac_init-0.7.5/iac_init/scripts/apic_connecton_tool.so
+-rwxr-xr-x   0        0        0   675792 2024-05-19 07:54:57.901138 iac_init-0.7.5/iac_init/scripts/cimc_precheck_tool.so
+-rwxr-xr-x   0        0        0   168632 2024-05-19 07:55:01.105148 iac_init-0.7.5/iac_init/scripts/ssh_tool.so
+-rwxr-xr-x   0        0        0   137000 2024-05-19 07:54:59.585144 iac_init-0.7.5/iac_init/scripts/telnet_tool.so
+-rwxr-xr-x   0        0        0   156336 2024-05-19 07:54:58.377140 iac_init-0.7.5/iac_init/scripts/thread_tool.so
+-rw-r--r--   0        0        0     3778 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-19 07:54:39.497074 iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.501074 iac_init-0.7.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-19 07:54:39.505074 iac_init-0.7.5/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rwxr-xr-x   0        0        0    62360 2024-05-19 07:54:46.533102 iac_init-0.7.5/iac_init/utils/exceptions.so
+-rwxr-xr-x   0        0        0   333200 2024-05-19 07:54:46.349101 iac_init-0.7.5/iac_init/utils/functional.so
+-rwxr-xr-x   0        0        0   935456 2024-05-19 07:54:45.285098 iac_init-0.7.5/iac_init/validator.so
+-rwxr-xr-x   0        0        0   503352 2024-05-19 07:54:48.285107 iac_init-0.7.5/iac_init/yaml_conf/yaml.so
+-rwxr-xr-x   0        0        0   600936 2024-05-19 07:54:50.677115 iac_init-0.7.5/iac_init/yaml_conf/yaml_writer.so
+-rw-r--r--   0        0        0     1636 2024-05-19 07:54:39.505074 iac_init-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.7.5/PKG-INFO
```

### Comparing `iac_init-0.7.4/LICENSE` & `iac_init-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/cli/main.so` & `iac_init-0.7.5/iac_init/cli/main.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/cli/options.so` & `iac_init-0.7.5/iac_init/cli/options.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/conf/__init__.py` & `iac_init-0.7.5/iac_init/conf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
 
 from iac_init.conf import global_settings
-from iac_init.utils.functional import LazyObject
+from iac_init.utils.functional import LazyObject, empty
 
 ENVIRONMENT_VARIABLE = "IAC_INIT_SETTINGS_MODULE"
 
 
 class SettingsReference(str):
     """
     String subclass which references a current settings value. It's treated as
```

### Comparing `iac_init-0.7.4/iac_init/conf/global_settings.so` & `iac_init-0.7.5/iac_init/conf/global_settings.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/scripts/ansible_tool.so` & `iac_init-0.7.5/iac_init/scripts/ansible_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/scripts/apic_connecton_tool.so` & `iac_init-0.7.5/iac_init/scripts/apic_connecton_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/scripts/cimc_precheck_tool.so` & `iac_init-0.7.5/iac_init/scripts/cimc_precheck_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/scripts/ssh_tool.so` & `iac_init-0.7.5/iac_init/scripts/ssh_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/scripts/telnet_tool.so` & `iac_init-0.7.5/iac_init/scripts/telnet_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/scripts/thread_tool.so` & `iac_init-0.7.5/iac_init/scripts/thread_tool.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.7.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.7.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/utils/exceptions.so` & `iac_init-0.7.5/iac_init/utils/exceptions.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/utils/functional.so` & `iac_init-0.7.5/iac_init/utils/functional.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/validator.so` & `iac_init-0.7.5/iac_init/validator.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/yaml_conf/yaml.so` & `iac_init-0.7.5/iac_init/yaml_conf/yaml.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/iac_init/yaml_conf/yaml_writer.so` & `iac_init-0.7.5/iac_init/yaml_conf/yaml_writer.so`

 * *Files identical despite different names*

### Comparing `iac_init-0.7.4/pyproject.toml` & `iac_init-0.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.7.4"
+version = "0.7.5"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.7.4/PKG-INFO` & `iac_init-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.7.4
+Version: 0.7.5
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

