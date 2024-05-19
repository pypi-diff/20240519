# Comparing `tmp/nuvla_job_engine-4.0.8.tar.gz` & `tmp/nuvla_job_engine-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvla_job_engine-4.0.8.tar", max compression
+gzip compressed data, was "nuvla_job_engine-4.0.9.tar", max compression
```

## Comparing `nuvla_job_engine-4.0.8.tar` & `nuvla_job_engine-4.0.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0    11357 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/LICENSE
--rw-r--r--   0        0        0     4586 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/README.md
--rw-r--r--   0        0        0       74 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/__init__.py
--rw-r--r--   0        0        0       24 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/__init__.py
--rw-r--r--   0        0        0     1340 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/connector.py
--rw-r--r--   0        0        0    11757 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/docker_compose.py
--rw-r--r--   0        0        0    33689 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/docker_machine.py
--rw-r--r--   0        0        0    15017 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/docker_service.py
--rw-r--r--   0        0        0     8401 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/docker_stack.py
--rwxr-xr-x   0        0        0     1412 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/extra/install-rancher.sh
--rw-r--r--   0        0        0     1713 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/extra/k8s-install.sh
--rw-r--r--   0        0        0     1432 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/extra/portainer-k8s.yaml
--rw-r--r--   0        0        0      774 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/extra/portainer-swarm.yaml
--rw-r--r--   0        0        0       68 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/extra/ssh-add-keys.sh
--rw-r--r--   0        0        0     2868 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/helm_driver.py
--rw-r--r--   0        0        0    28925 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/k8s_driver.py
--rw-r--r--   0        0        0    24927 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/kubernetes.py
--rw-r--r--   0        0        0      322 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/machine/__init__.py
--rw-r--r--   0        0        0      641 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/machine/helper.py
--rw-r--r--   0        0        0    11681 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/machine/machine.py
--rw-r--r--   0        0        0    29845 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/nuvlabox.py
--rw-r--r--   0        0        0     5380 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/registry.py
--rw-r--r--   0        0        0     3668 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/connector/utils.py
--rw-r--r--   0        0        0       95 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/__init__.py
--rw-r--r--   0        0        0     1989 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/__init__.py
--rwxr-xr-x   0        0        0     2999 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/application_docker_compose_validate.py
--rwxr-xr-x   0        0        0      320 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_deployment_set_start.py
--rwxr-xr-x   0        0        0     1686 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py
--rwxr-xr-x   0        0        0      322 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_deployment_set_update.py
--rwxr-xr-x   0        0        0      711 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py
--rwxr-xr-x   0        0        0      692 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_stop_deployment.py
--rwxr-xr-x   0        0        0      908 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_update_deployment.py
--rwxr-xr-x   0        0        0     1298 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/cancel_children_jobs.py
--rwxr-xr-x   0        0        0     4269 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/coe_provision.py
--rwxr-xr-x   0        0        0     1719 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/coe_start.py
--rwxr-xr-x   0        0        0     1644 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/coe_stop.py
--rwxr-xr-x   0        0        0     2601 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/coe_terminate.py
--rwxr-xr-x   0        0        0     2982 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/component_image_state.py
--rwxr-xr-x   0        0        0     8667 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/credential_check.py
--rw-r--r--   0        0        0     3129 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/dct_check.py
--rw-r--r--   0        0        0     2831 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_log_fetch.py
--rwxr-xr-x   0        0        0      345 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_set_delete.py
--rwxr-xr-x   0        0        0      421 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_set_force_delete.py
--rwxr-xr-x   0        0        0     5402 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_start.py
--rwxr-xr-x   0        0        0     7341 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_state.py
--rw-r--r--   0        0        0     3207 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_stop.py
--rw-r--r--   0        0        0     4010 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_update.py
--rwxr-xr-x   0        0        0      366 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/dummy_test_action.py
--rw-r--r--   0        0        0      729 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/handle_trial_end.py
--rwxr-xr-x   0        0        0     1051 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/jobs_cleanup.py
--rw-r--r--   0        0        0     3553 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/monitor_bulk_job.py
--rw-r--r--   0        0        0      697 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/notify_coupon_end.py
--rwxr-xr-x   0        0        0     2803 2024-05-14 21:17:54.289621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py
--rwxr-xr-x   0        0        0      692 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_check_api.py
--rwxr-xr-x   0        0        0      867 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_cluster.py
--rwxr-xr-x   0        0        0     2100 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py
--rwxr-xr-x   0        0        0     4570 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_decommission.py
--rwxr-xr-x   0        0        0     1856 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py
--rwxr-xr-x   0        0        0     1273 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py
--rw-r--r--   0        0        0     1287 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py
--rwxr-xr-x   0        0        0     1247 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_reboot.py
--rwxr-xr-x   0        0        0     4513 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_releases.py
--rwxr-xr-x   0        0        0     1280 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py
--rwxr-xr-x   0        0        0     2515 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py
--rwxr-xr-x   0        0        0     2429 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py
--rwxr-xr-x   0        0        0     1633 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_update.py
--rw-r--r--   0        0        0      849 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/register_usage_record.py
--rwxr-xr-x   0        0        0     3059 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/service_image_state.py
--rw-r--r--   0        0        0        0 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/__init__.py
--rw-r--r--   0        0        0     1574 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/bulk_action.py
--rwxr-xr-x   0        0        0      854 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/bulk_deployment.py
--rwxr-xr-x   0        0        0     8840 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py
--rwxr-xr-x   0        0        0     1289 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/deployment_set_remove.py
--rw-r--r--   0        0        0    11037 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/deployment_utils.py
--rw-r--r--   0        0        0     4008 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/resource_log_fetch.py
--rwxr-xr-x   0        0        0     9633 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/vulnerabilities_database.py
--rw-r--r--   0        0        0     7838 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/base.py
--rw-r--r--   0        0        0     2107 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distribution.py
--rw-r--r--   0        0        0     1989 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/__init__.py
--rwxr-xr-x   0        0        0     1500 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/component_image_state.py
--rwxr-xr-x   0        0        0     2296 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/deployment_state.py
--rwxr-xr-x   0        0        0     1214 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/deployment_state_new.py
--rwxr-xr-x   0        0        0     2479 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/deployment_state_old.py
--rwxr-xr-x   0        0        0      408 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/dummy_action.py
--rwxr-xr-x   0        0        0     2907 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/handle_trial_end.py
--rwxr-xr-x   0        0        0      440 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/jobs_cleanup.py
--rwxr-xr-x   0        0        0     1803 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py
--rwxr-xr-x   0        0        0     1754 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/notify_coupon_end.py
--rwxr-xr-x   0        0        0      487 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/nuvlabox_cluster_cleanup.py
--rwxr-xr-x   0        0        0     1435 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/nuvlabox_offline.py
--rwxr-xr-x   0        0        0      475 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/nuvlabox_releases.py
--rwxr-xr-x   0        0        0     1210 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py
--rwxr-xr-x   0        0        0     2464 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/register_usage_record.py
--rwxr-xr-x   0        0        0     3119 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py
--rwxr-xr-x   0        0        0     1556 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/service_image_state.py
--rwxr-xr-x   0        0        0      503 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/vulnerabilities_database.py
--rw-r--r--   0        0        0        0 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributor/__init__.py
--rw-r--r--   0        0        0     1400 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributor/distributor.py
--rw-r--r--   0        0        0        0 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/executor/__init__.py
--rw-r--r--   0        0        0     4391 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/executor/executor.py
--rw-r--r--   0        0        0    10902 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/job.py
--rw-r--r--   0        0        0     1975 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/util.py
--rw-r--r--   0        0        0      186 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/job_engine/job/version.py
--rwxr-xr-x   0        0        0     2708 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/scripts/job_deployment_state_push.py
--rwxr-xr-x   0        0        0      208 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/scripts/job_distributor.py
--rwxr-xr-x   0        0        0      197 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/scripts/job_executor.py
--rwxr-xr-x   0        0        0     1967 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/scripts/job_restore.py
--rwxr-xr-x   0        0        0      186 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/nuvla/scripts/pause.py
--rw-r--r--   0        0        0     1204 2024-05-14 21:17:54.293621 nuvla_job_engine-4.0.8/pyproject.toml
--rw-r--r--   0        0        0     5630 1970-01-01 00:00:00.000000 nuvla_job_engine-4.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/LICENSE
+-rw-r--r--   0        0        0     4586 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/README.md
+-rw-r--r--   0        0        0       74 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/__init__.py
+-rw-r--r--   0        0        0     1340 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/connector.py
+-rw-r--r--   0        0        0    11891 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/docker_compose.py
+-rw-r--r--   0        0        0    33689 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/docker_machine.py
+-rw-r--r--   0        0        0    15017 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/docker_service.py
+-rw-r--r--   0        0        0     8423 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/docker_stack.py
+-rwxr-xr-x   0        0        0     1412 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/extra/install-rancher.sh
+-rw-r--r--   0        0        0     1713 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/extra/k8s-install.sh
+-rw-r--r--   0        0        0     1432 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/extra/portainer-k8s.yaml
+-rw-r--r--   0        0        0      774 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/extra/portainer-swarm.yaml
+-rw-r--r--   0        0        0       68 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/extra/ssh-add-keys.sh
+-rw-r--r--   0        0        0     2868 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/helm_driver.py
+-rw-r--r--   0        0        0    28925 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/k8s_driver.py
+-rw-r--r--   0        0        0    24927 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/kubernetes.py
+-rw-r--r--   0        0        0      322 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/machine/__init__.py
+-rw-r--r--   0        0        0      641 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/machine/helper.py
+-rw-r--r--   0        0        0    11681 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/machine/machine.py
+-rw-r--r--   0        0        0    29971 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/nuvlabox.py
+-rw-r--r--   0        0        0     5380 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/registry.py
+-rw-r--r--   0        0        0     3668 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/connector/utils.py
+-rw-r--r--   0        0        0       95 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/__init__.py
+-rw-r--r--   0        0        0     1989 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/__init__.py
+-rwxr-xr-x   0        0        0     2999 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/application_docker_compose_validate.py
+-rwxr-xr-x   0        0        0      320 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_deployment_set_start.py
+-rwxr-xr-x   0        0        0     1686 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py
+-rwxr-xr-x   0        0        0      322 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_deployment_set_update.py
+-rwxr-xr-x   0        0        0      711 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py
+-rwxr-xr-x   0        0        0      692 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_stop_deployment.py
+-rwxr-xr-x   0        0        0      908 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_update_deployment.py
+-rwxr-xr-x   0        0        0     1298 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/cancel_children_jobs.py
+-rwxr-xr-x   0        0        0     4269 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/coe_provision.py
+-rwxr-xr-x   0        0        0     1719 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/coe_start.py
+-rwxr-xr-x   0        0        0     1644 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/coe_stop.py
+-rwxr-xr-x   0        0        0     2601 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/coe_terminate.py
+-rwxr-xr-x   0        0        0     2982 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/component_image_state.py
+-rwxr-xr-x   0        0        0     8667 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/credential_check.py
+-rw-r--r--   0        0        0     3129 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/dct_check.py
+-rw-r--r--   0        0        0     2831 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_log_fetch.py
+-rwxr-xr-x   0        0        0      345 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_set_delete.py
+-rwxr-xr-x   0        0        0      421 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_set_force_delete.py
+-rwxr-xr-x   0        0        0     5402 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_start.py
+-rwxr-xr-x   0        0        0     7341 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_state.py
+-rw-r--r--   0        0        0     3207 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_stop.py
+-rw-r--r--   0        0        0     4010 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_update.py
+-rwxr-xr-x   0        0        0      366 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/dummy_test_action.py
+-rw-r--r--   0        0        0      729 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/handle_trial_end.py
+-rwxr-xr-x   0        0        0     1051 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/jobs_cleanup.py
+-rw-r--r--   0        0        0     3553 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/monitor_bulk_job.py
+-rw-r--r--   0        0        0      697 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/notify_coupon_end.py
+-rwxr-xr-x   0        0        0     2803 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py
+-rwxr-xr-x   0        0        0      692 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_check_api.py
+-rwxr-xr-x   0        0        0      867 2024-05-19 18:22:59.218153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_cluster.py
+-rwxr-xr-x   0        0        0     2100 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py
+-rwxr-xr-x   0        0        0     4570 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_decommission.py
+-rwxr-xr-x   0        0        0     1856 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py
+-rwxr-xr-x   0        0        0     1273 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py
+-rw-r--r--   0        0        0     1287 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py
+-rwxr-xr-x   0        0        0     1247 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_reboot.py
+-rwxr-xr-x   0        0        0     4513 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_releases.py
+-rwxr-xr-x   0        0        0     1280 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py
+-rwxr-xr-x   0        0        0     2515 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py
+-rwxr-xr-x   0        0        0     2429 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py
+-rwxr-xr-x   0        0        0     1633 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_update.py
+-rw-r--r--   0        0        0      849 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/register_usage_record.py
+-rwxr-xr-x   0        0        0     3059 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/service_image_state.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/__init__.py
+-rw-r--r--   0        0        0     1574 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/bulk_action.py
+-rwxr-xr-x   0        0        0      854 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/bulk_deployment.py
+-rwxr-xr-x   0        0        0     8840 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py
+-rwxr-xr-x   0        0        0     1289 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/deployment_set_remove.py
+-rw-r--r--   0        0        0    11037 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/deployment_utils.py
+-rw-r--r--   0        0        0     4008 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/resource_log_fetch.py
+-rwxr-xr-x   0        0        0     9633 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/vulnerabilities_database.py
+-rw-r--r--   0        0        0     7838 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/base.py
+-rw-r--r--   0        0        0     2107 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distribution.py
+-rw-r--r--   0        0        0     1989 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/__init__.py
+-rwxr-xr-x   0        0        0     1500 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/component_image_state.py
+-rwxr-xr-x   0        0        0     2296 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/deployment_state.py
+-rwxr-xr-x   0        0        0     1214 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/deployment_state_new.py
+-rwxr-xr-x   0        0        0     2479 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/deployment_state_old.py
+-rwxr-xr-x   0        0        0      408 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/dummy_action.py
+-rwxr-xr-x   0        0        0     2907 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/handle_trial_end.py
+-rwxr-xr-x   0        0        0      440 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/jobs_cleanup.py
+-rwxr-xr-x   0        0        0     1803 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py
+-rwxr-xr-x   0        0        0     1754 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/notify_coupon_end.py
+-rwxr-xr-x   0        0        0      487 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/nuvlabox_cluster_cleanup.py
+-rwxr-xr-x   0        0        0     1435 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/nuvlabox_offline.py
+-rwxr-xr-x   0        0        0      475 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/nuvlabox_releases.py
+-rwxr-xr-x   0        0        0     1210 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py
+-rwxr-xr-x   0        0        0     2464 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/register_usage_record.py
+-rwxr-xr-x   0        0        0     3119 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py
+-rwxr-xr-x   0        0        0     1556 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/service_image_state.py
+-rwxr-xr-x   0        0        0      503 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/vulnerabilities_database.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributor/__init__.py
+-rw-r--r--   0        0        0     1400 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributor/distributor.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/executor/__init__.py
+-rw-r--r--   0        0        0     4391 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/executor/executor.py
+-rw-r--r--   0        0        0    10902 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/job.py
+-rw-r--r--   0        0        0     1975 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/util.py
+-rw-r--r--   0        0        0      186 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/job_engine/job/version.py
+-rwxr-xr-x   0        0        0     2708 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/scripts/job_deployment_state_push.py
+-rwxr-xr-x   0        0        0      208 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/scripts/job_distributor.py
+-rwxr-xr-x   0        0        0      197 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/scripts/job_executor.py
+-rwxr-xr-x   0        0        0     1967 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/scripts/job_restore.py
+-rwxr-xr-x   0        0        0      186 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/nuvla/scripts/pause.py
+-rw-r--r--   0        0        0     1204 2024-05-19 18:22:59.222153 nuvla_job_engine-4.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5630 1970-01-01 00:00:00.000000 nuvla_job_engine-4.0.9/PKG-INFO
```

### Comparing `nuvla_job_engine-4.0.8/LICENSE` & `nuvla_job_engine-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/README.md` & `nuvla_job_engine-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/connector.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/connector.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/docker_compose.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/docker_compose.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,29 +178,29 @@
             compose_file.close()
             service_id = self._get_service_id(deployment_uuid, component,
                                               compose_file_path, env)
         if service_id:
             since_opt = ['--since', since.isoformat()] if since else []
             list_opts = ['-t', '--tail', str(lines)] + since_opt + [service_id]
             cmd = self.build_cmd_line(list_opts, docker_command='logs')
-            return execute_cmd(cmd).stdout
+            return execute_cmd(cmd, sterr_in_stdout=True).stdout
         else:
-            return ''
+            return f'{datetime.utcnow().isoformat()} [Failed to find container "{component}" for deployment {deployment_uuid}]'
 
     @staticmethod
     def _get_image(container_info):
         try:
             return container_info[0]['Config']['Image']
         except KeyError:
             return ''
 
     def _get_service_id(self, project_name, service, docker_compose_path, env):
         cmd = self.build_cmd_line(['-p', project_name,
                                    '-f', docker_compose_path,
-                                   'ps', '-q', service])
+                                   'ps', '-q', '-a', service])
         stdout = self._execute_clean_command(cmd, env=env).stdout
 
         return yaml.load(stdout, Loader=yaml.FullLoader)
 
     @staticmethod
     def _get_service_ports(container_info):
         try:
```

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/docker_machine.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/docker_machine.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/docker_service.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/docker_service.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/docker_stack.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/docker_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     @should_connect
     def log(self, component: str, since: datetime, lines: int,
             **_kwargs) -> str:
         since_opt = ['--since', since.isoformat()] if since else []
         list_opts = ['-t', '--no-trunc', '--tail', str(lines)] + since_opt + [
             component]
         cmd = self.build_cmd_line(['service', 'logs'] + list_opts)
-        return execute_cmd(cmd).stdout
+        return execute_cmd(cmd, sterr_in_stdout=True).stdout
 
     @staticmethod
     def ports_info(port):
         external_port_info, internal_port_info = port.split('->')
         external_port = external_port_info.split(':')[1]
         internal_port, protocol = internal_port_info.split('/')
         return protocol, internal_port, external_port
```

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/extra/install-rancher.sh` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/extra/install-rancher.sh`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/extra/k8s-install.sh` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/extra/k8s-install.sh`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/extra/portainer-k8s.yaml` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/extra/portainer-k8s.yaml`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/extra/portainer-swarm.yaml` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/extra/portainer-swarm.yaml`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/helm_driver.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/helm_driver.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/k8s_driver.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/k8s_driver.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/kubernetes.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/kubernetes.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/machine/helper.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/machine/helper.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/machine/machine.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/machine/machine.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/nuvlabox.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/nuvlabox.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,26 +630,28 @@
             command += [f'--current-environment={repr(",".join(current_env))}']
 
         if new_env:
             command += [f'--new-environment={repr(",".join(new_env))}']
 
         target_release = kwargs.get('target_release')
         command.append(f'--target-version={target_release}')
-
+        
+        updater_env = {
+            'NUVLA_ENDPOINT': self.api.endpoint,
+            'NUVLA_ENDPOINT_INSECURE': str(not self.api.session.verify)
+        }
         if all(k in self.api.session.login_params for k in ['key', 'secret']):
             key = self.api.session.login_params['key']
             secret = self.api.session.login_params['secret']
-            updater_env = {
+            updater_env.update({
                 'NUVLABOX_API_KEY': key,
                 'NUVLABOX_API_SECRET': secret,
                 'NUVLAEDGE_API_KEY': key,
                 'NUVLAEDGE_API_SECRET': secret
-            }
-        else:
-            updater_env = {}
+            })
 
         current_version = self.nuvlabox_status.get('nuvlabox-engine-version',
                                                    install_params_from_payload.get(
                                                        'current-version'))
 
         if current_version:
             command.append(f'--current-version={current_version}')
```

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/registry.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/registry.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/connector/utils.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/connector/utils.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/__init__.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/application_docker_compose_validate.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/application_docker_compose_validate.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_stop_deployment.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_stop_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/bulk_update_deployment.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/bulk_update_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/cancel_children_jobs.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/cancel_children_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/coe_provision.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/coe_provision.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/coe_start.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/coe_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/coe_stop.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/coe_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/coe_terminate.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/coe_terminate.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/component_image_state.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/component_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/credential_check.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/credential_check.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/dct_check.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/dct_check.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_log_fetch.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_log_fetch.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_start.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_state.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_stop.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/deployment_update.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/deployment_update.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/handle_trial_end.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/handle_trial_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/jobs_cleanup.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/jobs_cleanup.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/monitor_bulk_job.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/monitor_bulk_job.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/notify_coupon_end.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/notify_coupon_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_check_api.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_check_api.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_cluster.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_cluster.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_decommission.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_decommission.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_reboot.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_reboot.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_releases.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_releases.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/nuvlabox_update.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/nuvlabox_update.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/register_usage_record.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/register_usage_record.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/service_image_state.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/service_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/bulk_action.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/bulk_action.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/bulk_deployment.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/bulk_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/deployment_set_remove.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/deployment_set_remove.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/deployment_utils.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/utils/resource_log_fetch.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/utils/resource_log_fetch.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/actions/vulnerabilities_database.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/actions/vulnerabilities_database.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/base.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/base.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distribution.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distribution.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/__init__.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/component_image_state.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/component_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/deployment_state.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/deployment_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/deployment_state_new.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/deployment_state_new.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/deployment_state_old.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/deployment_state_old.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/handle_trial_end.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/handle_trial_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/notify_coupon_end.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/notify_coupon_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/nuvlabox_offline.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/nuvlabox_offline.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/register_usage_record.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/register_usage_record.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributions/service_image_state.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributions/service_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/distributor/distributor.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/distributor/distributor.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/executor/executor.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/executor/executor.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/job.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/job.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/job_engine/job/util.py` & `nuvla_job_engine-4.0.9/nuvla/job_engine/job/util.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/scripts/job_deployment_state_push.py` & `nuvla_job_engine-4.0.9/nuvla/scripts/job_deployment_state_push.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/nuvla/scripts/job_restore.py` & `nuvla_job_engine-4.0.9/nuvla/scripts/job_restore.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.8/pyproject.toml` & `nuvla_job_engine-4.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuvla-job-engine"
-version = "4.0.8"
+version = "4.0.9"
 description = "Nuvla Job Engine."
 license = "Apache-2.0"
 authors = ["SixSq SA <support@sixsq.com>"]
 maintainers = ["Ignacio Penas <nacho@sixsq.com>"]
 readme = "README.md"
 repository = "https://github.com/nuvla/job-engine"
 classifiers = [
```

### Comparing `nuvla_job_engine-4.0.8/PKG-INFO` & `nuvla_job_engine-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvla-job-engine
-Version: 4.0.8
+Version: 4.0.9
 Summary: Nuvla Job Engine.
 Home-page: https://github.com/nuvla/job-engine
 License: Apache-2.0
 Author: SixSq SA
 Author-email: support@sixsq.com
 Maintainer: Ignacio Penas
 Maintainer-email: nacho@sixsq.com
```

