# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1716094984.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1716139671.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1716094984.tar", last modified: Sun May 19 05:05:26 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1716139671.tar", last modified: Sun May 19 17:30:02 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984.tar` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:05:26.365526 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 05:05:26.365526 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:05:26.349526 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4454 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:05:26.353526 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21648 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29690 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:05:26.357526 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1116 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    24968 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    13340 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8612 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     7575 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)     6879 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    25169 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:05:26.357526 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:05:26.361526 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      590 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108491 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14976 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    91820 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:05:26.361526 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 05:05:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-19 05:05:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 05:05:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 05:05:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 05:05:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-05-19 05:05:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 05:05:26.365526 pulumi_kubernetes_the_hard_way-0.0.21a1716094984/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.643216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4536 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.647216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      496 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21648 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)     4775 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    12667 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    38474 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.651216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1116 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    24968 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    13340 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8612 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     7575 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)     6879 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    25169 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.655216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108491 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14976 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91820 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716094984
+Version: 0.0.21a1716139671
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/README.md` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     resource_modules="""
 [
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "config",
   "fqn": "pulumi_kubernetes_the_hard_way.config",
   "classes": {
-   "kubernetes-the-hard-way:config:KubeVipManifest": "KubeVipManifest"
+   "kubernetes-the-hard-way:config:KubeVipManifest": "KubeVipManifest",
+   "kubernetes-the-hard-way:config:KubeletConfiguration": "KubeletConfiguration"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 from ._enums import *
 import pulumi_kubernetes
 
 __all__ = [
     'Cluster',
     'Context',
     'Kubeconfig',
+    'KubeletConfiguration',
+    'KubeletConfigurationAuthentication',
+    'KubeletConfigurationAuthenticationAnonymous',
+    'KubeletConfigurationAuthenticationWebhook',
+    'KubeletConfigurationAuthenticationx509',
+    'KubeletConfigurationAuthorization',
     'PodManifest',
     'User',
 ]
 
 @pulumi.output_type
 class Cluster(dict):
     def __init__(__self__, *,
@@ -101,14 +107,292 @@
     @property
     @pulumi.getter
     def users(self) -> Sequence['outputs.User']:
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
+class KubeletConfiguration(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "apiVersion":
+            suggest = "api_version"
+        elif key == "cgroupDriver":
+            suggest = "cgroup_driver"
+        elif key == "clusterDNS":
+            suggest = "cluster_dns"
+        elif key == "clusterDomain":
+            suggest = "cluster_domain"
+        elif key == "containerRuntimeEndpoint":
+            suggest = "container_runtime_endpoint"
+        elif key == "podCIDR":
+            suggest = "pod_cidr"
+        elif key == "resolvConf":
+            suggest = "resolv_conf"
+        elif key == "runtimeRequestTimeout":
+            suggest = "runtime_request_timeout"
+        elif key == "tlsCertFile":
+            suggest = "tls_cert_file"
+        elif key == "tlsPrivateKeyFile":
+            suggest = "tls_private_key_file"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in KubeletConfiguration. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        KubeletConfiguration.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        KubeletConfiguration.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 api_version: str,
+                 authentication: 'outputs.KubeletConfigurationAuthentication',
+                 authorization: 'outputs.KubeletConfigurationAuthorization',
+                 cgroup_driver: str,
+                 cluster_dns: Sequence[str],
+                 cluster_domain: str,
+                 container_runtime_endpoint: str,
+                 kind: str,
+                 pod_cidr: str,
+                 resolv_conf: str,
+                 runtime_request_timeout: str,
+                 tls_cert_file: str,
+                 tls_private_key_file: str):
+        """
+        :param str cgroup_driver: TODO
+        :param Sequence[str] cluster_dns: TODO
+        :param str cluster_domain: TODO
+        :param str container_runtime_endpoint: TODO
+        :param str pod_cidr: TODO
+        :param str resolv_conf: TODO
+        :param str runtime_request_timeout: TODO
+        :param str tls_cert_file: TODO
+        :param str tls_private_key_file: TODO
+        """
+        pulumi.set(__self__, "api_version", 'kubelet.config.k8s.io/v1beta1')
+        pulumi.set(__self__, "authentication", authentication)
+        pulumi.set(__self__, "authorization", authorization)
+        pulumi.set(__self__, "cgroup_driver", cgroup_driver)
+        pulumi.set(__self__, "cluster_dns", cluster_dns)
+        pulumi.set(__self__, "cluster_domain", cluster_domain)
+        pulumi.set(__self__, "container_runtime_endpoint", container_runtime_endpoint)
+        pulumi.set(__self__, "kind", 'KubeletConfiguration')
+        pulumi.set(__self__, "pod_cidr", pod_cidr)
+        pulumi.set(__self__, "resolv_conf", resolv_conf)
+        pulumi.set(__self__, "runtime_request_timeout", runtime_request_timeout)
+        pulumi.set(__self__, "tls_cert_file", tls_cert_file)
+        pulumi.set(__self__, "tls_private_key_file", tls_private_key_file)
+
+    @property
+    @pulumi.getter(name="apiVersion")
+    def api_version(self) -> str:
+        return pulumi.get(self, "api_version")
+
+    @property
+    @pulumi.getter
+    def authentication(self) -> 'outputs.KubeletConfigurationAuthentication':
+        return pulumi.get(self, "authentication")
+
+    @property
+    @pulumi.getter
+    def authorization(self) -> 'outputs.KubeletConfigurationAuthorization':
+        return pulumi.get(self, "authorization")
+
+    @property
+    @pulumi.getter(name="cgroupDriver")
+    def cgroup_driver(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "cgroup_driver")
+
+    @property
+    @pulumi.getter(name="clusterDNS")
+    def cluster_dns(self) -> Sequence[str]:
+        """
+        TODO
+        """
+        return pulumi.get(self, "cluster_dns")
+
+    @property
+    @pulumi.getter(name="clusterDomain")
+    def cluster_domain(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "cluster_domain")
+
+    @property
+    @pulumi.getter(name="containerRuntimeEndpoint")
+    def container_runtime_endpoint(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "container_runtime_endpoint")
+
+    @property
+    @pulumi.getter
+    def kind(self) -> str:
+        return pulumi.get(self, "kind")
+
+    @property
+    @pulumi.getter(name="podCIDR")
+    def pod_cidr(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "pod_cidr")
+
+    @property
+    @pulumi.getter(name="resolvConf")
+    def resolv_conf(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "resolv_conf")
+
+    @property
+    @pulumi.getter(name="runtimeRequestTimeout")
+    def runtime_request_timeout(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "runtime_request_timeout")
+
+    @property
+    @pulumi.getter(name="tlsCertFile")
+    def tls_cert_file(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "tls_cert_file")
+
+    @property
+    @pulumi.getter(name="tlsPrivateKeyFile")
+    def tls_private_key_file(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "tls_private_key_file")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthentication(dict):
+    def __init__(__self__, *,
+                 anonymous: 'outputs.KubeletConfigurationAuthenticationAnonymous',
+                 webhook: 'outputs.KubeletConfigurationAuthenticationWebhook',
+                 x509: 'outputs.KubeletConfigurationAuthenticationx509'):
+        pulumi.set(__self__, "anonymous", anonymous)
+        pulumi.set(__self__, "webhook", webhook)
+        pulumi.set(__self__, "x509", x509)
+
+    @property
+    @pulumi.getter
+    def anonymous(self) -> 'outputs.KubeletConfigurationAuthenticationAnonymous':
+        return pulumi.get(self, "anonymous")
+
+    @property
+    @pulumi.getter
+    def webhook(self) -> 'outputs.KubeletConfigurationAuthenticationWebhook':
+        return pulumi.get(self, "webhook")
+
+    @property
+    @pulumi.getter
+    def x509(self) -> 'outputs.KubeletConfigurationAuthenticationx509':
+        return pulumi.get(self, "x509")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthenticationAnonymous(dict):
+    def __init__(__self__, *,
+                 enabled: bool):
+        """
+        :param bool enabled: TODO
+        """
+        pulumi.set(__self__, "enabled", enabled)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> bool:
+        """
+        TODO
+        """
+        return pulumi.get(self, "enabled")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthenticationWebhook(dict):
+    def __init__(__self__, *,
+                 enabled: bool):
+        """
+        :param bool enabled: TODO
+        """
+        pulumi.set(__self__, "enabled", enabled)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> bool:
+        """
+        TODO
+        """
+        return pulumi.get(self, "enabled")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthenticationx509(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clientCAFile":
+            suggest = "client_ca_file"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in KubeletConfigurationAuthenticationx509. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        KubeletConfigurationAuthenticationx509.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        KubeletConfigurationAuthenticationx509.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 client_ca_file: str):
+        """
+        :param str client_ca_file: TODO
+        """
+        pulumi.set(__self__, "client_ca_file", client_ca_file)
+
+    @property
+    @pulumi.getter(name="clientCAFile")
+    def client_ca_file(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "client_ca_file")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthorization(dict):
+    def __init__(__self__, *,
+                 mode: str):
+        pulumi.set(__self__, "mode", mode)
+
+    @property
+    @pulumi.getter
+    def mode(self) -> str:
+        return pulumi.get(self, "mode")
+
+
+@pulumi.output_type
 class PodManifest(dict):
     """
     Pod is a collection of containers that can run on a host. This resource is created by clients and scheduled onto hosts.
 
     This resource waits until its status is ready before registering success
     for create/update, and populating output properties from the current state of the resource.
     The following conditions are used to determine whether the resource creation has
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716094984
+Version: 0.0.21a1716139671
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 pulumi_kubernetes_the_hard_way.egg-info/requires.txt
 pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
 pulumi_kubernetes_the_hard_way/config/__init__.py
 pulumi_kubernetes_the_hard_way/config/_enums.py
 pulumi_kubernetes_the_hard_way/config/_inputs.py
 pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
 pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
 pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
 pulumi_kubernetes_the_hard_way/config/outputs.py
 pulumi_kubernetes_the_hard_way/remote/__init__.py
 pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
 pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716094984/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.21a1716094984"
+  version = "0.0.21a1716139671"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

