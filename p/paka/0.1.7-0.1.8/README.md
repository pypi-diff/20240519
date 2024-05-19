# Comparing `tmp/paka-0.1.7.tar.gz` & `tmp/paka-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paka-0.1.7.tar", max compression
+gzip compressed data, was "paka-0.1.8.tar", max compression
```

## Comparing `paka-0.1.7.tar` & `paka-0.1.8.tar`

### file list

```diff
@@ -1,69 +1,71 @@
--rw-r--r--   0        0        0     1072 2024-05-08 07:01:18.660155 paka-0.1.7/LICENSE
--rw-r--r--   0        0        0     4321 2024-05-08 07:01:18.660155 paka-0.1.7/README.md
--rw-r--r--   0        0        0      153 2024-05-08 07:01:18.664155 paka-0.1.7/paka/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/__init__.py
--rw-r--r--   0        0        0     1608 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/__main__.py
--rw-r--r--   0        0        0     1401 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/build.py
--rw-r--r--   0        0        0     4652 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/cluster.py
--rw-r--r--   0        0        0     7308 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/function.py
--rw-r--r--   0        0        0     6482 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/job.py
--rw-r--r--   0        0        0      903 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/kubeconfig.py
--rw-r--r--   0        0        0     2441 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/model_group.py
--rw-r--r--   0        0        0     3392 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/run.py
--rw-r--r--   0        0        0    11072 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/utils.py
--rw-r--r--   0        0        0        0 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/__init__.py
--rw-r--r--   0        0        0      968 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/cloudwatch.py
--rw-r--r--   0        0        0     3049 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/cluster_autoscaler.py
--rw-r--r--   0        0        0      542 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/container_registry.py
--rw-r--r--   0        0        0     2466 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/ebs_csi_driver.py
--rw-r--r--   0        0        0    12290 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/eks.py
--rw-r--r--   0        0        0     1468 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/aws/elb.py
--rw-r--r--   0        0        0      569 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/aws/object_store.py
--rw-r--r--   0        0        0     3969 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/aws/service_account.py
--rw-r--r--   0        0        0     1904 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/aws/utils.py
--rw-r--r--   0        0        0     3799 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/context.py
--rw-r--r--   0        0        0     4580 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/fluentbit.py
--rw-r--r--   0        0        0     1189 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/keda.py
--rw-r--r--   0        0        0     4981 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/knative.py
--rw-r--r--   0        0        0     2480 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/kubectl.py
--rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/manager/__init__.py
--rw-r--r--   0        0        0      928 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/manager/aws.py
--rw-r--r--   0        0        0     2863 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/manager/base.py
--rw-r--r--   0        0        0      914 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/namespace.py
--rw-r--r--   0        0        0     3484 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/nvidia_device_plugin.py
--rw-r--r--   0        0        0     4275 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/prometheus.py
--rw-r--r--   0        0        0     3600 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/pulumi.py
--rw-r--r--   0        0        0     3998 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/qdrant.py
--rw-r--r--   0        0        0     2286 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/redis.py
--rw-r--r--   0        0        0      284 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/utils.py
--rw-r--r--   0        0        0      908 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/zipkin.py
--rw-r--r--   0        0        0    18815 2024-05-08 07:01:18.668155 paka-0.1.7/paka/config.py
--rw-r--r--   0        0        0      467 2024-05-08 07:01:18.668155 paka-0.1.7/paka/constants.py
--rw-r--r--   0        0        0     3623 2024-05-08 07:01:18.668155 paka-0.1.7/paka/container/ecr.py
--rw-r--r--   0        0        0     2627 2024-05-08 07:01:18.668155 paka-0.1.7/paka/container/pack.py
--rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/function/__init__.py
--rw-r--r--   0        0        0     5677 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/function/service.py
--rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/job/__init__.py
--rw-r--r--   0        0        0     2365 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/job/autoscaler.py
--rw-r--r--   0        0        0     4093 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/job/worker.py
--rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/__init__.py
--rw-r--r--   0        0        0     1364 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/ingress.py
--rw-r--r--   0        0        0      131 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/manifest.py
--rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/runtime/__init__.py
--rw-r--r--   0        0        0     4820 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/runtime/llama_cpp.py
--rw-r--r--   0        0        0     1708 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/runtime/vllm.py
--rw-r--r--   0        0        0    21811 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/service.py
--rw-r--r--   0        0        0    19234 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/utils.py
--rw-r--r--   0        0        0      761 2024-05-08 07:01:18.668155 paka-0.1.7/paka/logger.py
--rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/__init__.py
--rw-r--r--   0        0        0     2705 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/base_model.py
--rw-r--r--   0        0        0     2462 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/hf_model.py
--rw-r--r--   0        0        0     1488 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/http_model.py
--rw-r--r--   0        0        0     1444 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/manifest.py
--rw-r--r--   0        0        0     2565 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/progress_bar.py
--rw-r--r--   0        0        0     2080 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/settings.py
--rw-r--r--   0        0        0    10006 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/store.py
--rw-r--r--   0        0        0    11138 2024-05-08 07:01:18.668155 paka-0.1.7/paka/utils.py
--rw-r--r--   0        0        0     1477 2024-05-08 07:01:18.668155 paka-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 paka-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-19 08:14:16.473163 paka-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4321 2024-05-19 08:14:16.473163 paka-0.1.8/README.md
+-rw-r--r--   0        0        0      153 2024-05-19 08:14:16.477163 paka-0.1.8/paka/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/__init__.py
+-rw-r--r--   0        0        0     1608 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/__main__.py
+-rw-r--r--   0        0        0     1402 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/build.py
+-rw-r--r--   0        0        0     4449 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/cluster.py
+-rw-r--r--   0        0        0    14006 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/function.py
+-rw-r--r--   0        0        0     5666 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/job.py
+-rw-r--r--   0        0        0      903 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/kubeconfig.py
+-rw-r--r--   0        0        0     2577 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/model_group.py
+-rw-r--r--   0        0        0     3443 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/run.py
+-rw-r--r--   0        0        0    11534 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/__init__.py
+-rw-r--r--   0        0        0      968 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/cloudwatch.py
+-rw-r--r--   0        0        0     3982 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/cluster_autoscaler.py
+-rw-r--r--   0        0        0      542 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/container_registry.py
+-rw-r--r--   0        0        0     2466 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/ebs_csi_driver.py
+-rw-r--r--   0        0        0    15960 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/eks.py
+-rw-r--r--   0        0        0     1732 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/elb.py
+-rw-r--r--   0        0        0      569 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/object_store.py
+-rw-r--r--   0        0        0     3969 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/service_account.py
+-rw-r--r--   0        0        0     1904 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/utils.py
+-rw-r--r--   0        0        0     4136 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/context.py
+-rw-r--r--   0        0        0     4580 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/fluentbit.py
+-rw-r--r--   0        0        0     1189 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/keda.py
+-rw-r--r--   0        0        0     4981 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/knative.py
+-rw-r--r--   0        0        0     2480 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/kubectl.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/manager/__init__.py
+-rw-r--r--   0        0        0      928 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/manager/aws.py
+-rw-r--r--   0        0        0     3485 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/manager/base.py
+-rw-r--r--   0        0        0      914 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/namespace.py
+-rw-r--r--   0        0        0     3484 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/nvidia_device_plugin.py
+-rw-r--r--   0        0        0     4275 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/prometheus.py
+-rw-r--r--   0        0        0     3600 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/pulumi.py
+-rw-r--r--   0        0        0     3998 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/qdrant.py
+-rw-r--r--   0        0        0     2286 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/redis.py
+-rw-r--r--   0        0        0      284 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/utils.py
+-rw-r--r--   0        0        0      908 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/zipkin.py
+-rw-r--r--   0        0        0    22175 2024-05-19 08:14:16.477163 paka-0.1.8/paka/config.py
+-rw-r--r--   0        0        0      467 2024-05-19 08:14:16.477163 paka-0.1.8/paka/constants.py
+-rw-r--r--   0        0        0     3623 2024-05-19 08:14:16.477163 paka-0.1.8/paka/container/ecr.py
+-rw-r--r--   0        0        0     2627 2024-05-19 08:14:16.477163 paka-0.1.8/paka/container/pack.py
+-rw-r--r--   0        0        0     6536 2024-05-19 08:14:16.477163 paka-0.1.8/paka/gguf.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/function/__init__.py
+-rw-r--r--   0        0        0    11603 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/function/service.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/job/__init__.py
+-rw-r--r--   0        0        0     2370 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/job/autoscaler.py
+-rw-r--r--   0        0        0     4093 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/job/worker.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/__init__.py
+-rw-r--r--   0        0        0     1364 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/ingress.py
+-rw-r--r--   0        0        0      131 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/manifest.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/runtime/__init__.py
+-rw-r--r--   0        0        0     4820 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/runtime/llama_cpp.py
+-rw-r--r--   0        0        0     1883 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/runtime/vllm.py
+-rw-r--r--   0        0        0    22683 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/service.py
+-rw-r--r--   0        0        0     9948 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/service_v1.py
+-rw-r--r--   0        0        0    21190 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/utils.py
+-rw-r--r--   0        0        0      761 2024-05-19 08:14:16.477163 paka-0.1.8/paka/logger.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/__init__.py
+-rw-r--r--   0        0        0     2705 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/base_model.py
+-rw-r--r--   0        0        0     2462 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/hf_model.py
+-rw-r--r--   0        0        0     1488 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/http_model.py
+-rw-r--r--   0        0        0     1444 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/manifest.py
+-rw-r--r--   0        0        0     2565 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/progress_bar.py
+-rw-r--r--   0        0        0     2080 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/settings.py
+-rw-r--r--   0        0        0    10006 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/store.py
+-rw-r--r--   0        0        0    12339 2024-05-19 08:14:16.477163 paka-0.1.8/paka/utils.py
+-rw-r--r--   0        0        0     1630 2024-05-19 08:14:16.481163 paka-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 paka-0.1.8/PKG-INFO
```

### Comparing `paka-0.1.7/LICENSE` & `paka-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/README.md` & `paka-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cli/__main__.py` & `paka-0.1.8/paka/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cli/build.py` & `paka-0.1.8/paka/cli/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 from paka.cli.utils import build_and_push
 
 build_app = typer.Typer()
 
 
 @build_app.callback(invoke_without_command=True)
 def build(
-    source_dir: str = typer.Argument(
-        ...,
-        help="Source directory of the application.",
-    ),
     cluster_name: Optional[str] = typer.Option(
         os.getenv("PAKA_CURRENT_CLUSTER"),
         "--cluster",
         "-c",
         help="The name of the cluster.",
     ),
+    source_dir: str = typer.Argument(
+        ...,
+        help="Source directory of the application.",
+    ),
     image_name: str = typer.Option(
         "",
         "--image-name",
         help="Provide a custom name for the Docker image. If omitted, "
         "the base name of the source code directory will be used as the image name.",
     ),
 ) -> None:
     """
     Build a Docker image from the application in the specified source directory.
+
     The source directory must contain a Procfile and a .cnignore file. The Procfile
     defines the commands to run for the application. The .cnignore file defines the
     files and directories to exclude from the image. Once the image is built,
     it will be pushed to the container repository of the current cluster.
 
     A Dockerfile is NOT required. The image will be built using Cloud Native Buildpacks.
     In cluster build is not supported yet. User machine must have Docker installed.
```

### Comparing `paka-0.1.7/paka/cli/cluster.py` & `paka-0.1.8/paka/cli/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from __future__ import annotations
 
-import json
 import threading
 import time
 from typing import List
 
-import click
 import typer
 
 from paka.cli.utils import load_cluster_manager, load_kubeconfig
-from paka.k8s.utils import remove_crd_finalizers, update_kubeconfig
-from paka.logger import logger
+from paka.k8s.utils import remove_crd_finalizers
 
 cluster_app = typer.Typer()
 
 
 @cluster_app.command()
 def up(
     cluster_config: str = typer.Option(
@@ -34,19 +31,16 @@
         "Use this option to prevent updating the kubeconfig file.",
     ),
 ) -> None:
     """
     Creates or updates a Kubernetes cluster based on the provided configuration.
     """
     cluster_manager = load_cluster_manager(cluster_config)
+    cluster_manager.ctx.set_should_save_kubeconfig(not no_kubeconfig)
     cluster_manager.create()
-    if not no_kubeconfig:
-        logger.info("Updating kubeconfig...")
-        update_kubeconfig(json.loads(cluster_manager.ctx.kubeconfig))
-        logger.info("Successfully updated kubeconfig.")
 
 
 @cluster_app.command()
 def down(
     cluster_config: str = typer.Option(
         "",
         "--file",
@@ -61,15 +55,15 @@
         help="Automatic yes to prompts. Use this option to bypass the confirmation "
         "prompt and directly proceed with the operation.",
     ),
 ) -> None:
     """
     Tears down the Kubernetes cluster, removing all associated resources and data.
     """
-    if yes or click.confirm(
+    if yes or typer.confirm(
         f"Are you sure you want to proceed with the operation? Please note that "
         "all resources and data will be permanently deleted.",
         default=False,
     ):
         cluster_manager = load_cluster_manager(cluster_config)
 
         # Sometime finalizers might block CRD deletion, so we need to force delete those.
```

### Comparing `paka-0.1.7/paka/cli/job.py` & `paka-0.1.8/paka/cli/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import os
 from typing import Optional
 
-import click
 import typer
 from kubernetes import client
 
 from paka.cli.utils import get_cluster_namespace, load_kubeconfig, resolve_image
 from paka.k8s.job.worker import create_workers, delete_workers
 from paka.logger import logger
 from paka.utils import kubify_name
@@ -80,22 +79,14 @@
         help="Determines whether the system should wait for existing tasks to "
         "complete before deploying the new job. If set to true, the deployment "
         "will wait until all current tasks have finished.",
     ),
 ) -> None:
     """
     Deploy a job.
-
-    A job leverages a Redis queue to distribute work to a pool of autoscaling workers.
-    The job can be specified by providing a Docker image or a source directory containing the application code.
-
-    If a Docker image is provided, the cluster will run the job using this image.
-    If a source directory is provided, the cluster will build a Docker image from the source code and then run the job.
-
-    If both an image and a source directory are provided, the Docker image is used and the source directory is ignored.
     """
     load_kubeconfig(cluster_name)
     resolved_image = resolve_image(cluster_name, image, source_dir)
 
     if image:
         job_name = image
     elif source_dir:
@@ -110,24 +101,24 @@
         max_replicas=max_workers,
         drain_existing_job=wait_existing_tasks,
     )
 
 
 @job_app.command()
 def delete(
-    name: str = typer.Argument(
-        ...,
-        help="The name of the job to delete.",
-    ),
     cluster_name: Optional[str] = typer.Option(
         os.getenv("PAKA_CURRENT_CLUSTER"),
         "--cluster",
         "-c",
         help="The name of the cluster.",
     ),
+    name: str = typer.Argument(
+        ...,
+        help="The name of the job to delete.",
+    ),
     wait_existing_tasks: bool = typer.Option(
         True,
         "--wait-existing-tasks",
         help="Determines whether the system should wait for existing tasks to "
         "complete before deploying the new job. If set to true, the deployment "
         "will wait until all current tasks have finished.",
     ),
@@ -136,25 +127,17 @@
         "--yes",
         "-y",
         help="Automatic yes to prompts. Use this option to bypass the confirmation "
         "prompt and directly proceed with the deletion.",
     ),
 ) -> None:
     """
-    Deletes a job.
-
-    Args:
-        name (str): The unique identifier of the job to be deleted.
-        wait_existing_tasks (bool): Determines whether the system should wait for existing tasks to complete before deleting the job.
-        yes (bool): If True, bypasses the confirmation prompt and directly proceeds with the deletion.
-
-    Returns:
-        None
+    Delete a job.
     """
-    if yes or click.confirm(
+    if yes or typer.confirm(
         f"Are you sure you want to delete the job {name}?", default=False
     ):
         load_kubeconfig(cluster_name)
         logger.info(f"Deleting job {name}")
         delete_workers(
             get_cluster_namespace(cluster_name),
             prefixed_job_name(name),
@@ -182,11 +165,12 @@
 
     # List the deployments in the specified namespace that match the field selector
     deployments = api_instance.list_namespaced_deployment(
         namespace=get_cluster_namespace(cluster_name), label_selector=label_selector
     )
 
     for deployment in deployments.items:
-        logger.info(deployment.metadata.name)
+        if deployment.metadata and deployment.metadata.name:
+            logger.info(deployment.metadata.name)
 
     if not deployments.items:
         logger.info("No jobs found.")
```

### Comparing `paka-0.1.7/paka/cli/kubeconfig.py` & `paka-0.1.8/paka/cli/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cli/model_group.py` & `paka-0.1.8/paka/cli/model_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,19 +64,24 @@
     ),
 ) -> None:
     """
     List all model groups.
     """
     load_kubeconfig(cluster_name)
     services = filter_services(get_cluster_namespace(cluster_name))
-    model_groups = [service.spec.selector.get("model") for service in services]
+    model_groups = [
+        service.spec.selector.get("model", "")
+        for service in services
+        if service.spec and service.spec.selector and "model" in service.spec.selector
+    ]
 
     v1 = client.CoreV1Api()
     cfg = v1.read_namespaced_config_map("config-domain", "knative-serving")
-    filtered_keys = [key for key in cfg.data.keys() if key.endswith("sslip.io")]
+    cfg_data = cfg.data or {}
+    filtered_keys = [key for key in cfg_data if key.endswith("sslip.io")]
     if not filtered_keys:
         if not model_groups:
             logger.info("No model groups found.")
         else:
             logger.info("\n".join(model_groups))
         return
     domain = filtered_keys[0]
```

### Comparing `paka-0.1.7/paka/cli/run.py` & `paka-0.1.8/paka/cli/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 CLEANUP_TIMEOUT = 600  # 10 minutes
 
 run_app = typer.Typer()
 
 
 @run_app.callback(invoke_without_command=True)
 def one_off_script(
-    entrypoint: str = typer.Option(
-        ...,
-        "--entrypoint",
-        help="The entrypoint of the application. This refers to the command "
-        "defined in the Procfile that will be executed.",
-    ),
     cluster_name: Optional[str] = typer.Option(
         os.getenv("PAKA_CURRENT_CLUSTER"),
         "--cluster",
         "-c",
         help="The name of the cluster.",
     ),
+    entrypoint: str = typer.Option(
+        ...,
+        "--entrypoint",
+        help="The entrypoint of the application. This refers to the command "
+        "defined in the Procfile that will be executed.",
+    ),
     source_dir: Optional[str] = typer.Option(
         None,
         "--source",
         help="The directory containing the source code of the application. If "
         "specified, a new Docker image will be built using the source code from "
         "this directory. A Dockerfile is not required because the build process "
         "uses Cloud Native's Buildpacks, which automatically detect and install "
@@ -91,8 +91,9 @@
 
     logger.info(f"Waiting for the task to complete...")
     api = client.CoreV1Api()
     pods = api.list_namespaced_pod(
         namespace=namespace, label_selector=f"job-name={job_name}"
     )
     for pod in pods.items:
-        tail_logs(namespace, pod.metadata.name, "one-off-script")
+        if pod.metadata and pod.metadata.name:
+            tail_logs(namespace, pod.metadata.name, "one-off-script")
```

### Comparing `paka-0.1.7/paka/cli/utils.py` & `paka-0.1.8/paka/cli/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import functools
 import os
 import platform
 import re
 import subprocess
+from datetime import timedelta
 from typing import Any, Optional
 
 import typer
 from kubernetes import config as k8s_config
 
 from paka.cluster.manager.aws import AWSClusterManager
 from paka.cluster.manager.base import ClusterManager
@@ -304,7 +305,23 @@
     return namespace
 
 
 def load_kubeconfig(cluster_name: Optional[str]) -> None:
     cluster_name = ensure_cluster_name(cluster_name)
     kubeconfig = read_pulumi_stack(cluster_name, "kubeconfig")
     k8s_config.load_kube_config_from_dict(kubeconfig)
+
+
+def format_timedelta(td: timedelta) -> str:
+    total_seconds = int(td.total_seconds())
+    hours, remainder = divmod(total_seconds, 3600)
+    minutes, seconds = divmod(remainder, 60)
+    days, hours = divmod(hours, 24)
+
+    if days > 0:
+        return f"{days}d{hours}h"
+    elif hours > 0:
+        return f"{hours}h{minutes}m"
+    elif minutes > 0:
+        return f"{minutes}m{seconds}s"
+    else:
+        return f"{seconds}s"
```

### Comparing `paka-0.1.7/paka/cluster/aws/cloudwatch.py` & `paka-0.1.8/paka/cluster/aws/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/aws/container_registry.py` & `paka-0.1.8/paka/cluster/aws/container_registry.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/aws/ebs_csi_driver.py` & `paka-0.1.8/paka/cluster/aws/ebs_csi_driver.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/aws/eks.py` & `paka-0.1.8/paka/cluster/aws/eks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import json
 from typing import List, Optional, cast
 
 import pulumi
 import pulumi_aws as aws
 import pulumi_awsx as awsx
 import pulumi_eks as eks
 import pulumi_kubernetes as k8s
@@ -18,15 +19,16 @@
 from paka.cluster.knative import create_knative_and_istio
 from paka.cluster.namespace import create_namespace
 from paka.cluster.nvidia_device_plugin import install_nvidia_device_plugin
 from paka.cluster.prometheus import create_prometheus
 from paka.cluster.qdrant import create_qdrant
 from paka.cluster.redis import create_redis
 from paka.cluster.zipkin import create_zipkin
-from paka.config import AwsModelGroup
+from paka.config import AwsMixedModelGroup, AwsModelGroup
+from paka.k8s.utils import update_kubeconfig
 from paka.utils import kubify_name
 
 
 def _ignore_tags_transformation(
     args: pulumi.ResourceTransformationArgs,
 ) -> Optional[pulumi.ResourceTransformationResult]:
     """
@@ -75,51 +77,146 @@
         return
 
     cluster_name = ctx.cluster_name
 
     model_groups = cast(List[AwsModelGroup], ctx.cloud_config.modelGroups)
 
     for model_group in model_groups:
+        taints = [
+            aws.eks.NodeGroupTaintArgs(
+                effect="NO_SCHEDULE", key="app", value="model-group"
+            ),
+            aws.eks.NodeGroupTaintArgs(
+                effect="NO_SCHEDULE", key="model", value=model_group.name
+            ),
+        ]
+
+        gpu_enabled = model_group.gpu and model_group.gpu.enabled
+
+        ami_type = "AL2_x86_64_GPU" if gpu_enabled else None
+
+        disk_size = (
+            model_group.gpu.diskSize
+            if gpu_enabled and model_group.gpu
+            else model_group.diskSize
+        )
+
         # Create a managed node group for our cluster
         eks.ManagedNodeGroup(
             f"{cluster_name}-{kubify_name(model_group.name)}-group",
-            node_group_name=f"{cluster_name}-{kubify_name(model_group.name)}-group",
+            node_group_name=f"{cluster_name}-{kubify_name(model_group.name)}-on-demand",
             cluster=cluster,
             instance_types=[model_group.nodeType],
             scaling_config=aws.eks.NodeGroupScalingConfigArgs(
                 desired_size=model_group.minInstances,
                 min_size=model_group.minInstances,
                 max_size=model_group.maxInstances,
             ),
             labels={
                 "size": model_group.nodeType,
                 "app": "model-group",
                 "model": model_group.name,
+                "lifecycle": "on-demand",
             },
             node_role_arn=worker_role.arn,
             subnet_ids=vpc.private_subnet_ids,
-            taints=[
-                aws.eks.NodeGroupTaintArgs(
-                    effect="NO_SCHEDULE", key="app", value="model-group"
-                ),
-                aws.eks.NodeGroupTaintArgs(
-                    effect="NO_SCHEDULE", key="model", value=model_group.name
-                ),
-            ],
+            taints=taints,
             # Supported AMI types https://docs.aws.amazon.com/eks/latest/APIReference/API_Nodegroup.html#AmazonEKS-Type-Nodegroup-amiType
-            ami_type=(
-                "AL2_x86_64_GPU"
-                if model_group.gpu and model_group.gpu.enabled
-                else None
+            ami_type=ami_type,
+            disk_size=disk_size,
+            capacity_type="ON_DEMAND",
+        )
+
+
+def create_node_group_for_mixed_model_group(
+    ctx: Context,
+    cluster: eks.Cluster,
+    vpc: awsx.ec2.Vpc,
+    worker_role: aws.iam.Role,
+) -> None:
+
+    if ctx.cloud_config.mixedModelGroups is None:
+        return
+
+    cluster_name = ctx.cluster_name
+
+    mixed_model_groups = cast(
+        List[AwsMixedModelGroup], ctx.cloud_config.mixedModelGroups
+    )
+
+    for mixed_model_group in mixed_model_groups:
+        taints = [
+            aws.eks.NodeGroupTaintArgs(
+                effect="NO_SCHEDULE", key="app", value="model-group"
             ),
-            disk_size=(
-                model_group.gpu.diskSize
-                if model_group.gpu and model_group.gpu.enabled
-                else model_group.diskSize
+            aws.eks.NodeGroupTaintArgs(
+                effect="NO_SCHEDULE", key="model", value=mixed_model_group.name
             ),
+        ]
+
+        gpu_enabled = mixed_model_group.gpu and mixed_model_group.gpu.enabled
+
+        ami_type = "AL2_x86_64_GPU" if gpu_enabled else None
+
+        disk_size = (
+            mixed_model_group.gpu.diskSize
+            if gpu_enabled and mixed_model_group.gpu
+            else mixed_model_group.diskSize
+        )
+
+        # Create a managed node group for our cluster
+        eks.ManagedNodeGroup(
+            f"{cluster_name}-{kubify_name(mixed_model_group.name)}-group",
+            node_group_name=f"{cluster_name}-{kubify_name(mixed_model_group.name)}-on-demand",
+            cluster=cluster,
+            instance_types=[mixed_model_group.nodeType],
+            scaling_config=aws.eks.NodeGroupScalingConfigArgs(
+                desired_size=mixed_model_group.baseInstances,
+                min_size=mixed_model_group.baseInstances,
+                max_size=mixed_model_group.maxOnDemandInstances,
+            ),
+            labels={
+                "size": mixed_model_group.nodeType,
+                "app": "model-group",
+                "model": mixed_model_group.name,
+                "lifecycle": "on-demand",
+            },
+            node_role_arn=worker_role.arn,
+            subnet_ids=vpc.private_subnet_ids,
+            taints=taints,
+            # Supported AMI types https://docs.aws.amazon.com/eks/latest/APIReference/API_Nodegroup.html#AmazonEKS-Type-Nodegroup-amiType
+            ami_type=ami_type,
+            disk_size=disk_size,
+            capacity_type="ON_DEMAND",
+        )
+
+        # Create a managed node group with spot instances
+        eks.ManagedNodeGroup(
+            f"{cluster_name}-{kubify_name(mixed_model_group.name)}-spot-group",
+            node_group_name=f"{cluster_name}-{kubify_name(mixed_model_group.name)}-spot",
+            cluster=cluster,
+            instance_types=[mixed_model_group.nodeType],
+            scaling_config=aws.eks.NodeGroupScalingConfigArgs(
+                desired_size=mixed_model_group.spot.minInstances,
+                min_size=mixed_model_group.spot.minInstances,
+                max_size=mixed_model_group.spot.maxInstances,
+            ),
+            labels={
+                "size": mixed_model_group.nodeType,
+                "app": "model-group",
+                "model": mixed_model_group.name,
+                "lifecycle": "spot",
+            },
+            node_role_arn=worker_role.arn,
+            subnet_ids=vpc.private_subnet_ids,
+            taints=taints,
+            # Supported AMI types https://docs.aws.amazon.com/eks/latest/APIReference/API_Nodegroup.html#AmazonEKS-Type-Nodegroup-amiType
+            ami_type=ami_type,
+            disk_size=disk_size,
+            capacity_type="SPOT",
         )
 
 
 def create_node_group_for_qdrant(
     ctx: Context,
     cluster: eks.Cluster,
     vpc: awsx.ec2.Vpc,
@@ -270,23 +367,26 @@
         node_role_arn=worker_role.arn,
         subnet_ids=vpc.private_subnet_ids,
     )
 
     # Create a managed node group for each model group
     create_node_group_for_model_group(ctx, cluster, vpc, worker_role)
 
+    create_node_group_for_mixed_model_group(ctx, cluster, vpc, worker_role)
+
     # Create a managed node group for Qdrant
     create_node_group_for_qdrant(ctx, cluster, vpc, worker_role)
 
     def create_eks_resources(kubeconfig_json: str) -> None:
         k8s_provider = k8s.Provider("k8s-provider", kubeconfig=cluster.kubeconfig)
         ctx.set_k8s_provider(k8s_provider)
         ctx.set_kubeconfig(kubeconfig_json)
 
-        # save_kubeconfig(ctx.cluster_name, kubeconfig_json)
+        if ctx.should_save_kubeconfig:
+            update_kubeconfig(json.loads(kubeconfig_json))
 
         # Deploy the metrics server. This is required for the Horizontal Pod Autoscaler to work.
         # HPA requires metrics to be available in order to scale the pods.
         k8s.yaml.ConfigFile(
             "metrics-server",
             file="https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml",
             opts=pulumi.ResourceOptions(provider=k8s_provider),
```

### Comparing `paka-0.1.7/paka/cluster/aws/elb.py` & `paka-0.1.8/paka/cluster/aws/elb.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,14 +36,21 @@
 def get_elb_name(kubeconfig_json: str) -> Optional[str]:
     config.load_kube_config_from_dict(json.loads(kubeconfig_json))
 
     v1 = client.CoreV1Api()
     services = v1.list_service_for_all_namespaces(watch=False)
 
     for service in services.items:
-        if service.spec.type == "LoadBalancer":
+        if service.spec and service.spec.type == "LoadBalancer":
             # The name of the ELB is the first part of the hostname of the load balancer
-            elb_hostname = service.status.load_balancer.ingress[0].hostname
-            elb_name = elb_hostname.split("-")[0]
-            return elb_name
+            if (
+                service.status
+                and service.status.load_balancer
+                and service.status.load_balancer.ingress
+            ):
+                elb_hostname = service.status.load_balancer.ingress[0].hostname
+                if not elb_hostname:
+                    continue
+                elb_name = elb_hostname.split("-")[0]
+                return elb_name
 
     return None
```

### Comparing `paka-0.1.7/paka/cluster/aws/object_store.py` & `paka-0.1.8/paka/cluster/aws/object_store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/aws/service_account.py` & `paka-0.1.8/paka/cluster/aws/service_account.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/aws/utils.py` & `paka-0.1.8/paka/cluster/aws/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/context.py` & `paka-0.1.8/paka/cluster/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     # Materialized bucket with a unique name
     _bucket: Optional[str]
     # Materialized container registry url
     _registry: Optional[str]
     # The kubeconfig str
     _kubeconfig: Optional[str]
 
+    # Need to lock the access to these fields
+    _should_save_kubeconfig: bool = False
+
     def __init__(self) -> None:
         # Ugly, ideally, we can create these locks dynamically in __getattr__.
         # However, __getattr__ is not thread safe either. We need another lock to protect the creation of locks.
         # This lock is going to be a bottleneck. Therefore, we pre-create the locks.
         # Multiple locks pose a risk of deadlock. We need to be careful when acquiring multiple locks.
         self._k8s_provider_lock = fasteners.ReaderWriterLock()
         self._config_lock = fasteners.ReaderWriterLock()
@@ -105,7 +108,14 @@
     def set_kubeconfig(self, kubeconfig: str) -> None:
         self._kubeconfig = kubeconfig
 
     @property
     @fasteners.read_locked(lock="_kubeconfig_lock")
     def kubeconfig(self) -> Optional[str]:
         return self._kubeconfig
+
+    def set_should_save_kubeconfig(self, should_save_kubeconfig: bool) -> None:
+        self._should_save_kubeconfig = should_save_kubeconfig
+
+    @property
+    def should_save_kubeconfig(self) -> bool:
+        return self._should_save_kubeconfig
```

### Comparing `paka-0.1.7/paka/cluster/fluentbit.py` & `paka-0.1.8/paka/cluster/fluentbit.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/keda.py` & `paka-0.1.8/paka/cluster/keda.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/knative.py` & `paka-0.1.8/paka/cluster/knative.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/kubectl.py` & `paka-0.1.8/paka/cluster/kubectl.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/manager/aws.py` & `paka-0.1.8/paka/cluster/manager/aws.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/manager/base.py` & `paka-0.1.8/paka/cluster/manager/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from paka.cluster.pulumi import ensure_pulumi
 from paka.config import CloudConfig, Config
 from paka.constants import PULUMI_STACK_NAME
 from paka.k8s.model_group.service import (
     cleanup_staled_model_group_services,
     create_model_group_service,
 )
+from paka.k8s.model_group.service_v1 import (
+    create_model_group_service as create_model_group_service_v1,
+)
 from paka.logger import logger
 
 STACK_NAME = "default"
 
 
 class ClusterManager(ABC):
     """
@@ -66,27 +69,38 @@
             self._stack.set_config(
                 "aws:region", auto.ConfigValue(value=self.cloud_config.cluster.region)
             )
 
         logger.info("Creating resources...")
         self._stack.up(on_output=logger.info)
 
-        if self.cloud_config.modelGroups is None:
+        if (
+            self.cloud_config.modelGroups is None
+            and self.cloud_config.mixedModelGroups is None
+        ):
             return
 
         namespace = self.cloud_config.cluster.namespace
 
         # Clean up staled model group resources before creating new ones
-        cleanup_staled_model_group_services(
-            namespace, [mg.name for mg in self.config.aws.modelGroups or []]
-        )
+        model_group_names = [mg.name for mg in self.config.aws.modelGroups or []]
+        mixed_model_group_names = [
+            mg.name for mg in self.config.aws.mixedModelGroups or []
+        ]
+        all_group_names = model_group_names + mixed_model_group_names
 
-        for model_group in self.cloud_config.modelGroups:
+        cleanup_staled_model_group_services(namespace, all_group_names)
+        # TODO: We should clean up deployment as well
+
+        for model_group in self.cloud_config.modelGroups or []:
             create_model_group_service(self.ctx, namespace, model_group)
 
+        for mixed_model_group in self.cloud_config.mixedModelGroups or []:
+            create_model_group_service_v1(self.ctx, namespace, mixed_model_group)
+
     def destroy(self) -> Any:
         logger.info("Destroying resources...")
         return self._stack.destroy(on_output=logger.info)
 
     def refresh(self) -> None:
         logger.info("Refreshing the stack...")
         self._stack.refresh(on_output=logger.info)
```

### Comparing `paka-0.1.7/paka/cluster/namespace.py` & `paka-0.1.8/paka/cluster/namespace.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/nvidia_device_plugin.py` & `paka-0.1.8/paka/cluster/nvidia_device_plugin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/prometheus.py` & `paka-0.1.8/paka/cluster/prometheus.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/pulumi.py` & `paka-0.1.8/paka/cluster/pulumi.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/qdrant.py` & `paka-0.1.8/paka/cluster/qdrant.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/redis.py` & `paka-0.1.8/paka/cluster/redis.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/cluster/zipkin.py` & `paka-0.1.8/paka/cluster/zipkin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/config.py` & `paka-0.1.8/paka/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Dict, Generic, List, Optional, TypeVar
 
 from pydantic import BaseModel, ConfigDict, Field, field_validator, model_validator
 from ruamel.yaml import YAML
 
 from paka.utils import to_yaml
 
-CONFIG_VERSION = "1.0"
+CONFIG_VERSION = "1.1"
 
 
 class PakaBaseModel(BaseModel):
     model_config = ConfigDict(extra="forbid")
 
 
 def validate_size(v: str, error_message: str = "Invalid size format") -> str:
@@ -139,16 +139,14 @@
 
 
 class AwsNode(CloudNode):
     """
     Represents an AWS cloud node configuration.
     """
 
-    model_config = ConfigDict(extra="forbid")
-
     gpu: Optional[AwsGpuNodeConfig] = Field(
         None, description="The AWS GPU node configuration, if applicable."
     )
 
 
 class Runtime(PakaBaseModel):
     """
@@ -173,31 +171,84 @@
         ["*"], description="The list of files to include from the repository."
     )
     useModelStore: bool = Field(
         True, description="Whether to save the model to a model store, such as s3."
     )
 
 
-class ModelGroup(PakaBaseModel):
+class Trigger(PakaBaseModel):
     """
-    Represents a group of VMs that serve the inference for a specific type of model.
+    Represents a trigger.
+    """
+
+    type: str = Field(..., description="The type of the trigger.")
+    metadata: Dict[str, str] = Field(
+        ..., description="The metadata associated with the trigger."
+    )
+
+
+class CloudModelGroup(CloudNode):
+    """
+    Represents a group of cloud models.
     """
 
     name: str = Field(..., description="The name of the model group.")
+    model: Optional[Model] = Field(
+        None,
+        description="The model to deploy in the model group. If None, runtime image is responsible for loading the model.",
+    )
+    runtime: Runtime = Field(..., description="The runtime for the model group.")
+
+    resourceRequest: Optional[ResourceRequest] = Field(
+        None,
+        description="The resource request for the model group, specifying the amount of CPU and memory to request.",
+    )
+
+    autoScaleTriggers: Optional[List[Trigger]] = Field(
+        None,
+        description="""The list of triggers for auto-scaling.
+    Triggers for autoscaling the model group. Trigger are not strongly typed, so we use a list of dictionaries to represent them.
+    For example:
+
+    autoScaleTriggers=[
+        # CPU trigger example
+        Trigger(
+            type="cpu",
+            metadata={
+                "type": "Utilization",
+                "value": "70"
+            }
+        ),
+        # Prometheus trigger example
+        Trigger(
+            type="prometheus",
+            metadata={
+                "serverAddress": "http://prometheus-operated.default.svc.cluster.local",
+                "metricName": "http_requests_total",
+                "threshold": "100",
+                "query": "sum(rate(http_requests_total{job=\"example-job\"}[2m]))"
+            }
+        )
+    ]
+    """,
+    )
+
+    isPublic: bool = Field(
+        False,
+        description="Whether the model group can be accessed through a public endpoint.",
+    )
+
+
+class ScalingConfig(PakaBaseModel):
     minInstances: int = Field(
         ..., description="The minimum number of instances to provision."
     )
     maxInstances: int = Field(
         ..., description="The maximum number of instances to provision."
     )
-    model: Optional[Model] = Field(
-        None,
-        description="The model to deploy in the model group. If None, runtime image is responsible for loading the model.",
-    )
-    runtime: Runtime = Field(..., description="The runtime for the model group.")
 
     @model_validator(mode="before")
     def check_instances_num(cls, values: Dict[str, int]) -> Dict[str, int]:
         min_instances, max_instances = values.get("minInstances"), values.get(
             "maxInstances"
         )
         if min_instances and max_instances and max_instances < min_instances:
@@ -222,66 +273,73 @@
             ValueError: If the value of the input value is invalid.
         """
         if v <= 0:
             raise ValueError("minInstances must be greater than 0")
         return v
 
 
-class Trigger(PakaBaseModel):
-    """
-    Represents a trigger.
-    """
-
-    type: str = Field(..., description="The type of the trigger.")
-    metadata: Dict[str, str] = Field(
-        ..., description="The metadata associated with the trigger."
-    )
-
+class OnDemandModelGroup(CloudModelGroup, ScalingConfig):
+    pass
 
-class CloudModelGroup(ModelGroup, CloudNode):
-    """
-    Represents a group of cloud models.
-    """
 
-    resourceRequest: ResourceRequest = Field(
+class MixedModelGroup(CloudModelGroup):
+    baseInstances: int = Field(
         ...,
-        description="The resource request for the model group, specifying the amount of CPU and memory to request.",
+        description=(
+            "Initial set of instances that are provisioned using on-demand "
+            "instances. These instances are always running. Their primary purpose is to guarantee the constant "
+            "availability of the model group service. If you don't require these base instances, you can set their number to 0."
+        ),
     )
-
-    autoScaleTriggers: Optional[List[Trigger]] = Field(
-        None,
-        description="""The list of triggers for auto-scaling.
-    Triggers for autoscaling the model group. Trigger are not strongly typed, so we use a list of dictionaries to represent them.
-    For example:
-
-    autoScaleTriggers=[
-        # CPU trigger example
-        Trigger(
-            type="cpu",
-            metadata={
-                "type": "Utilization",
-                "value": "70"
-            }
+    maxOnDemandInstances: int = Field(
+        ...,
+        description=(
+            "This sets the maximum limit for provisioning on-demand instances, including the base instances. "
+            "It should always be set to a value equal to or greater than 'baseInstances'. "
+            "These on-demand instances serve as a fallback when spot instances are unavailable. "
+            "The actual number of on-demand instances is dynamically adjusted by the autoscaler based on the workload requirements."
+        ),
+    )
+    spot: ScalingConfig = Field(
+        ...,
+        description=(
+            "This configuration sets the scaling parameters for spot instances within the node group. "
+            "It specifies the minimum and maximum number of spot instances that can be used. "
+            "Spot instances are cost-effective but may not always be available due to market conditions. "
+            "The autoscaler uses this configuration to dynamically adjust the number of spot instances based on workload demand."
         ),
-        # Prometheus trigger example
-        Trigger(
-            type="prometheus",
-            metadata={
-                "serverAddress": "http://prometheus-operated.default.svc.cluster.local",
-                "metricName": "http_requests_total",
-                "threshold": "100",
-                "query": "sum(rate(http_requests_total{job=\"example-job\"}[2m]))"
-            }
-        )
-    ]
-    """,
     )
 
+    @model_validator(mode="before")
+    def check_instances_num(cls, values: Dict[str, int]) -> Dict[str, int]:
+        base_instances, max_on_demand_instances = values.get(
+            "baseInstances"
+        ), values.get("maxOnDemandInstances")
+        if (
+            base_instances is not None
+            and max_on_demand_instances is not None
+            and max_on_demand_instances < base_instances
+        ):
+            raise ValueError(
+                "maxOnDemandInstances must be greater than or equal to baseInstances"
+            )
+        return values
+
+    @field_validator("baseInstances", mode="before")
+    def validate_base_instances(cls, v: int) -> int:
+        if v < 0:
+            raise ValueError("baseInstances must be greater than or equal to 0")
+        return v
+
 
-class AwsModelGroup(CloudModelGroup, AwsNode):
+class AwsModelGroup(OnDemandModelGroup, AwsNode):
+    pass
+
+
+class AwsMixedModelGroup(MixedModelGroup, AwsNode):
     pass
 
 
 class ClusterConfig(PakaBaseModel):
     """
     Represents the configuration for a cluster.
     """
@@ -445,29 +503,34 @@
     )
     zipkinHelmSettings: Optional[Dict[str, Any]] = Field(
         None,
         description="The settings for the Zipkin Helm chart. See https://github.com/openzipkin/zipkin-helm",
     )
 
 
-T_CloudModelGroup = TypeVar("T_CloudModelGroup", bound=CloudModelGroup)
+T_OnDemandModelGroup = TypeVar("T_OnDemandModelGroup", bound=OnDemandModelGroup)
+T_MixedModelGroup = TypeVar("T_MixedModelGroup", bound=MixedModelGroup)
 
 
-class CloudConfig(PakaBaseModel, Generic[T_CloudModelGroup]):
+class CloudConfig(PakaBaseModel, Generic[T_OnDemandModelGroup, T_MixedModelGroup]):
     """
     Represents the configuration for the cloud environment.
     """
 
     cluster: ClusterConfig = Field(
         ..., description="The configuration for the Kubernetes cluster."
     )
-    modelGroups: Optional[List[T_CloudModelGroup]] = Field(
+    modelGroups: Optional[List[T_OnDemandModelGroup]] = Field(
         None,
         description="The list of model groups to be deployed in the cloud. Default is None. If None, no model groups are deployed.",
     )
+    mixedModelGroups: Optional[List[T_MixedModelGroup]] = Field(
+        None,
+        description="The list of mixed model groups to be deployed in the cloud. Default is None. If None, no mixed model groups are deployed.",
+    )
     vectorStore: Optional[CloudVectorStore] = Field(
         None,
         description="The configuration for the vector store in the cloud. Default is None. If None, no vector store is deployed",
     )
     job: Optional[Job] = Field(
         None,
         description="The configuration for the job broker. Default is None. If None, no job broker is deployed.",
@@ -477,31 +540,45 @@
         description="The configuration for Prometheus. Default is None. If None, Prometheus is not deployed.",
     )
     tracing: Optional[Tracing] = Field(
         None,
         description="The configuration for tracing. Default is None. If None, tracing is not enabled.",
     )
 
-    @field_validator("modelGroups", mode="before")
-    def check_model_group(cls, v: List[Any]) -> List[Any]:
-        if v is None or len(v) == 0:
-            return v
-        # Check if there are duplicated model group names
-        model_group_names = [dict(group)["name"] for group in v]
-        if len(set(model_group_names)) != len(model_group_names):
-            raise ValueError("Duplicate model group names are not allowed")
-        return v
+    @model_validator(mode="before")
+    def check_model_group_names(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        # No model groups should have the same name
+        model_group_names = set()
+
+        for group in values.get("modelGroups", []):
+            group_name = dict(group)["name"]
+            if group_name in model_group_names:
+                raise ValueError(f"Duplicate model group names are not allowed")
+            model_group_names.add(group_name)
+
+        for mixed_group in values.get("mixedModelGroups", []):
+            mixed_group_name = dict(mixed_group)["name"]
+            if mixed_group_name in model_group_names:
+                raise ValueError(f"Duplicate model group names are not allowed")
+            model_group_names.add(mixed_group_name)
+
+        return values
 
 
-class AwsConfig(CloudConfig[AwsModelGroup]):
+class AwsConfig(CloudConfig[AwsModelGroup, AwsMixedModelGroup]):
     modelGroups: Optional[List[AwsModelGroup]] = Field(
         None,
         description="The list of model groups to be deployed in the cloud. Default is None. If None, no model groups are deployed.",
     )
 
+    mixedModelGroups: Optional[List[AwsMixedModelGroup]] = Field(
+        None,
+        description="The list of mixed model groups to be deployed in the cloud. Default is None. If None, no mixed model groups are deployed.",
+    )
+
 
 class Config(PakaBaseModel):
     """
     Configuration class for managing cloud cluster settings.
     """
 
     version: str = Field(..., description="The version of the configuration.")
```

### Comparing `paka-0.1.7/paka/container/ecr.py` & `paka-0.1.8/paka/container/ecr.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/container/pack.py` & `paka-0.1.8/paka/container/pack.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/k8s/job/autoscaler.py` & `paka-0.1.8/paka/k8s/job/autoscaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,11 +64,11 @@
 
 
 def delete_autoscaler(namespace: str, job_name: str) -> None:
     scaled_object = CustomResource(
         api_version="keda.sh/v1alpha1",
         kind="ScaledObject",
         plural="scaledobjects",
-        metadata=client.V1ObjectMeta(job_name, namespace=namespace),
+        metadata=client.V1ObjectMeta(name=job_name, namespace=namespace),
         spec={},
     )
     delete_namespaced_custom_object(job_name, namespace, scaled_object)
```

### Comparing `paka-0.1.7/paka/k8s/job/worker.py` & `paka-0.1.8/paka/k8s/job/worker.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/k8s/model_group/ingress.py` & `paka-0.1.8/paka/k8s/model_group/ingress.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/k8s/model_group/runtime/llama_cpp.py` & `paka-0.1.8/paka/k8s/model_group/runtime/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/k8s/model_group/runtime/vllm.py` & `paka-0.1.8/paka/k8s/model_group/runtime/vllm.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from huggingface_hub.utils import validate_repo_id
 
 from paka.cluster.context import Context
 from paka.cluster.utils import get_model_store
 from paka.config import CloudModelGroup
 from paka.constants import MODEL_MOUNT_PATH
+from paka.k8s.utils import get_gpu_count
 
 
 # Heuristic to determine if the image is a vLLM image
 def is_vllm_image(image: str) -> bool:
     return image.lower().startswith("vllm")
 
 
@@ -42,8 +43,13 @@
         return command + ["--model", model_to_load]
 
     if runtime.command:
         return attach_model_to_command(runtime.command)
 
     command = shlex.split("python3 -O -u -m vllm.entrypoints.api_server --host 0.0.0.0")
 
+    gpu_count = get_gpu_count(ctx, model_group)
+
+    if gpu_count > 1:
+        command += ["--tensor-parallel-size", str(gpu_count)]
+
     return attach_model_to_command(command)
```

### Comparing `paka-0.1.7/paka/k8s/model_group/service.py` & `paka-0.1.8/paka/k8s/model_group/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from typing import List, Optional, Tuple, cast
 
 from kubernetes import client
 from kubernetes import config as k8s_config
 
 from paka.cluster.context import Context
 from paka.cluster.utils import get_model_store
-from paka.config import T_CloudModelGroup
+from paka.config import CloudModelGroup, T_OnDemandModelGroup
 from paka.constants import ACCESS_ALL_SA, MODEL_MOUNT_PATH
 from paka.k8s.model_group.ingress import create_model_vservice
 from paka.k8s.model_group.runtime.llama_cpp import (
     get_runtime_command_llama_cpp,
     is_llama_cpp_image,
 )
 from paka.k8s.model_group.runtime.vllm import get_runtime_command_vllm, is_vllm_image
-from paka.k8s.utils import CustomResource, apply_resource
+from paka.k8s.utils import CustomResource, apply_resource, get_gpu_count
 from paka.logger import logger
 from paka.model.hf_model import HuggingFaceModel
 from paka.model.store import MODEL_PATH_PREFIX
-from paka.utils import kubify_name
+from paka.utils import get_instance_info, kubify_name
 
 
 def get_runtime_command(
-    ctx: Context, model_group: T_CloudModelGroup, port: int
+    ctx: Context, model_group: CloudModelGroup, port: int
 ) -> List[str]:
     """
     Gets the runtime command for a machine learning model group.
 
     Args:
         model_group (T_CloudModelGroup): The model group to get the runtime command for.
 
@@ -53,25 +53,25 @@
             break
     else:
         command.extend(["--port", str(port)])
 
     return command
 
 
-def get_health_check_paths(model_group: T_CloudModelGroup) -> Tuple[str, str]:
+def get_health_check_paths(model_group: CloudModelGroup) -> Tuple[str, str]:
     # Return a tuple for ready and live probes
     if is_llama_cpp_image(model_group.runtime.image):
         return ("/health", "/health")
     elif is_vllm_image(model_group.runtime.image):
         return ("/health", "/health")
 
     raise ValueError("Unsupported runtime image for health check paths.")
 
 
-def init_aws(ctx: Context, model_group: T_CloudModelGroup) -> client.V1Container:
+def init_aws(ctx: Context, model_group: CloudModelGroup) -> client.V1Container:
     """
     Initializes an AWS container for downloading a model from S3.
 
     Args:
         config (CloudConfig): The cloud configuration.
         model_group (T_CloudModelGroup): The cloud model group.
 
@@ -99,17 +99,17 @@
         ],
     )
 
 
 def create_pod(
     ctx: Context,
     namespace: str,
-    model_group: T_CloudModelGroup,
+    model_group: CloudModelGroup,
     port: int,
-) -> client.V1Pod:
+) -> client.V1PodTemplateSpec:
     """
     Creates a Kubernetes Pod for a machine learning model group.
 
     This function creates a Kubernetes Pod with the specified configuration. The Pod runs a container
     with the specified runtime image and exposes the specified port. The container runs a machine learning
     model from the model group.
 
@@ -166,33 +166,49 @@
             timeout_seconds=30,
             success_threshold=1,
             failure_threshold=5,
         ),
     }
 
     if model_group.resourceRequest:
-        container_args["resources"] = client.V1ResourceRequirements(
-            requests={
-                "cpu": model_group.resourceRequest.cpu,
-                "memory": model_group.resourceRequest.memory,
-            },
+        cpu_request = model_group.resourceRequest.cpu
+        memory_request = model_group.resourceRequest.memory
+    else:
+        instance_info = get_instance_info(
+            ctx.provider, ctx.region, model_group.nodeType
         )
+        if not instance_info:
+            raise ValueError(
+                f"No instance information found for instance type {model_group.nodeType} in {ctx.provider} {ctx.region}"
+            )
+        cpu_milli = cast(int, instance_info["cpu"]) * 1000
+        # Leave 400m for other processes
+        cpu_request = f"{cpu_milli - 400}m"
+        # Leave 2GB for other processes
+        memory_request = f"{cast(int, instance_info['memory']) - (2 * 1024)}Mi"
+
+    resources = client.V1ResourceRequirements(
+        requests={
+            "cpu": cpu_request,
+            "memory": memory_request,
+        },
+    )
+
+    container_args["resources"] = resources
 
     if hasattr(model_group, "gpu") and model_group.gpu and model_group.gpu.enabled:
-        if "resources" not in container_args:
-            container_args["resources"] = client.V1ResourceRequirements()
-        if container_args["resources"].limits is None:
-            container_args["resources"].limits = {}
-        gpu_count = 1
-        if model_group.resourceRequest and model_group.resourceRequest.gpu:
-            gpu_count = model_group.resourceRequest.gpu
+        if resources.limits is None:
+            resources.limits = {}
+
+        gpu_count = get_gpu_count(ctx=ctx, model_group=model_group)
+
         # Ah, we only support nvidia GPUs for now
-        container_args["resources"].limits["nvidia.com/gpu"] = gpu_count
+        resources.limits["nvidia.com/gpu"] = str(gpu_count)
 
-    return client.V1Pod(
+    return client.V1PodTemplateSpec(
         metadata=client.V1ObjectMeta(
             name=f"{kubify_name(model_group.name)}",
             namespace=namespace,
             labels={
                 "app": "model-group",
                 "model": model_group.name,
             },
@@ -207,15 +223,15 @@
             ],
             # Download models from s3 only when s3 is used as a model store
             init_containers=(
                 [init_aws(ctx, model_group)]
                 if model_group.model and model_group.model.useModelStore
                 else []
             ),
-            containers=[client.V1Container(**container_args)],
+            containers=[client.V1Container(**container_args)],  # type: ignore
             tolerations=[
                 client.V1Toleration(
                     key="app",
                     value="model-group",
                     effect="NoSchedule",
                 ),
                 client.V1Toleration(
@@ -258,15 +274,15 @@
                 ),
             ),
         ),
     )
 
 
 def create_deployment(
-    namespace: str, model_group: T_CloudModelGroup, pod: client.V1Pod
+    namespace: str, model_group: T_OnDemandModelGroup, pod: client.V1PodTemplateSpec
 ) -> client.V1Deployment:
     """
     Creates a Kubernetes Deployment for a machine learning model group.
 
     Args:
         namespace (str): The namespace to create the Deployment in.
         model_group (T_CloudModelGroup): The model group to run in the Deployment.
@@ -291,15 +307,15 @@
                 }
             ),
             template=pod,
         ),
     )
 
 
-def create_service_monitor(namespace: str, model_group: T_CloudModelGroup) -> None:
+def create_service_monitor(namespace: str, model_group: CloudModelGroup) -> None:
     monitor = CustomResource(
         api_version="monitoring.coreos.com/v1",
         kind="ServiceMonitor",
         plural="servicemonitors",
         metadata=client.V1ObjectMeta(
             name=kubify_name(model_group.name), namespace=namespace
         ),
@@ -331,15 +347,18 @@
                 "interval": "15s",
             }
         )
     apply_resource(monitor)
 
 
 def create_service(
-    namespace: str, model_group: T_CloudModelGroup, port: int, sidecar_port: int = 15090
+    namespace: str,
+    model_group: CloudModelGroup,
+    port: int,
+    sidecar_port: int = 15090,
 ) -> client.V1Service:
     """
     Creates a Kubernetes Service for a machine learning model group.
 
     Args:
         namespace (str): The namespace to create the Service in.
         model_group (T_CloudModelGroup): The model group to expose with the Service.
@@ -395,24 +414,25 @@
 
     v1 = client.CoreV1Api()
 
     services = v1.list_namespaced_service(namespace)
     filtered_services = [
         service
         for service in services.items
-        if service.spec.selector
+        if service.spec
+        and service.spec.selector
         and service.spec.selector.get("app") == "model-group"
         and service.spec.selector.get("model")
     ]
 
     return filtered_services
 
 
 def create_hpa(
-    namespace: str, model_group: T_CloudModelGroup, deployment: client.V1Deployment
+    namespace: str, model_group: T_OnDemandModelGroup, deployment: client.V1Deployment
 ) -> client.V2HorizontalPodAutoscaler:
     """
     Creates a Kubernetes Horizontal Pod Autoscaler (HPA) for a machine learning model group.
 
     This function creates a Kubernetes HPA with the specified namespace, model group, and deployment.
     The HPA automatically scales the number of Pods in the deployment based on the CPU utilization.
 
@@ -423,14 +443,15 @@
         namespace (str): The namespace to create the HPA in.
         model_group (T_CloudModelGroup): The model group to scale with the HPA.
         deployment (client.V1Deployment): The deployment to scale.
 
     Returns:
         client.V2HorizontalPodAutoscaler: The created HPA.
     """
+    assert deployment.metadata and deployment.metadata.name
     return client.V2HorizontalPodAutoscaler(
         api_version="autoscaling/v2",
         kind="HorizontalPodAutoscaler",
         metadata=client.V1ObjectMeta(
             name=f"{kubify_name(model_group.name)}",
             namespace=namespace,
         ),
@@ -455,15 +476,19 @@
                 )
             ],
         ),
     )
 
 
 def create_scaled_object(
-    namespace: str, model_group: T_CloudModelGroup, deployment: client.V1Deployment
+    namespace: str,
+    model_group: CloudModelGroup,
+    deployment: client.V1Deployment,
+    min_replicas: int,
+    max_replicas: int,
 ) -> Optional[CustomResource]:
     """
     Creates a KEDA ScaledObject for a given model group.
 
     This function creates a ScaledObject custom resource for Kubernetes Event-driven Autoscaling (KEDA).
     The ScaledObject is used to scale a Kubernetes Deployment based on the triggers defined in the model group.
 
@@ -475,28 +500,30 @@
 
     Returns:
         None
     """
     if not model_group.autoScaleTriggers:
         return None
 
+    assert deployment.metadata and deployment.metadata.name
+
     return CustomResource(
         api_version="keda.sh/v1alpha1",
         kind="ScaledObject",
         plural="scaledobjects",
         metadata=client.V1ObjectMeta(
             name=f"{kubify_name(model_group.name)}", namespace=namespace
         ),
         spec={
             "scaleTargetRef": {
                 "kind": "Deployment",
                 "name": deployment.metadata.name,
             },
-            "minReplicaCount": model_group.minInstances,
-            "maxReplicaCount": model_group.maxInstances,
+            "minReplicaCount": min_replicas,
+            "maxReplicaCount": max_replicas,
             "pollingInterval": 15,
             "triggers": list(
                 map(
                     lambda trigger: {
                         "type": trigger.type,
                         "metadata": trigger.metadata,
                     },
@@ -506,15 +533,15 @@
         },
     )
 
 
 def create_model_group_service(
     ctx: Context,
     namespace: str,
-    model_group: T_CloudModelGroup,
+    model_group: T_OnDemandModelGroup,
 ) -> None:
     """
     Creates a Kubernetes service for a machine learning model group.
 
     Args:
         namespace (str): The namespace to create the service in.
         config (Config): The configuration for the service.
@@ -562,20 +589,27 @@
 
     svc = create_service(namespace, model_group, port)
     apply_resource(svc)
 
     if config.prometheus and config.prometheus.enabled:
         create_service_monitor(namespace, model_group)
 
-    scaled_object = create_scaled_object(namespace, model_group, deployment)
+    scaled_object = create_scaled_object(
+        namespace,
+        model_group,
+        deployment,
+        model_group.minInstances,
+        model_group.maxInstances,
+    )
     if scaled_object:
         apply_resource(scaled_object)
 
     # Create a vservice to export the model group to the outside world
-    create_model_vservice(namespace, model_group.name)
+    if model_group.isPublic:
+        create_model_vservice(namespace, model_group.name)
 
 
 def cleanup_model_group_service_by_name(
     namespace: str,
     model_group_name: str,
 ) -> None:
     """
@@ -585,56 +619,56 @@
         namespace (str): The namespace to clean up the service in.
         model_group_name (str): The name of the model group to clean up the service for.
 
     Returns:
         None
     """
 
-    api_client = client.AppsV1Api()
+    apps_v1_api = client.AppsV1Api()
 
     # Delete the deployment
-    api_client.delete_namespaced_deployment(
+    apps_v1_api.delete_namespaced_deployment(
         name=kubify_name(model_group_name),
         namespace=namespace,
         body=client.V1DeleteOptions(
             propagation_policy="Foreground", grace_period_seconds=30
         ),
     )
 
     # Delete the service
-    api_client = client.CoreV1Api()
+    core_v1_api = client.CoreV1Api()
 
     # Delete the service
-    api_client.delete_namespaced_service(
+    core_v1_api.delete_namespaced_service(
         name=kubify_name(model_group_name),
         namespace=namespace,
         body=client.V1DeleteOptions(
             propagation_policy="Foreground", grace_period_seconds=30
         ),
     )
 
-    api_client = client.CustomObjectsApi()
+    custom_objects_api = client.CustomObjectsApi()
 
     # Best effort deletion
     try:
         # Delete the service monitor
-        api_client.delete_namespaced_custom_object(
+        custom_objects_api.delete_namespaced_custom_object(
             group="monitoring.coreos.com",
             version="v1",
             namespace=namespace,
             plural="servicemonitors",
             name=kubify_name(model_group_name),
             body=client.V1DeleteOptions(),
         )
     except:
         pass
 
     # Delete the scaled object
     try:
-        api_client.delete_namespaced_custom_object(
+        custom_objects_api.delete_namespaced_custom_object(
             group="keda.sh",
             version="v1alpha1",
             namespace=namespace,
             plural="scaledobjects",
             name=kubify_name(model_group_name),
             body=client.V1DeleteOptions(),
         )
@@ -642,18 +676,19 @@
         pass
 
 
 def cleanup_staled_model_group_services(
     namespace: str, source_of_truth_model_groups: List[str]
 ) -> None:
     services = filter_services(namespace)
-    model_groups: List[str] = [
+    model_groups = [
         # Get the model group name from the service selector
-        cast(client.V1ServiceSpec, service.spec).selector.get("model")
+        service.spec.selector.get("model", "")
         for service in services
+        if service.spec and service.spec.selector
     ]
 
     source_of_truth_model_groups_set = set(source_of_truth_model_groups)
 
     for model_group in model_groups:
         if model_group not in source_of_truth_model_groups_set:
             cleanup_model_group_service_by_name(namespace, model_group)
```

### Comparing `paka-0.1.7/paka/k8s/utils.py` & `paka-0.1.8/paka/k8s/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 import select
 import socket
 import threading
 import time
 from functools import partial
 from typing import Any, Callable, Dict, List, Literal, Optional, Protocol, Tuple
 
-from kubernetes import client, watch
-from kubernetes.client.rest import ApiException
+from kubernetes import watch  # type: ignore
+from kubernetes import client
+from kubernetes.client.exceptions import ApiException
 from kubernetes.stream import portforward
 from ruamel.yaml import YAML
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 from typing_extensions import TypeAlias
 
+from paka.cluster.context import Context
+from paka.config import CloudModelGroup
 from paka.logger import logger
-from paka.utils import read_yaml_file
+from paka.utils import get_instance_info, read_yaml_file
 
 KubernetesResourceKind: TypeAlias = Literal[
     "Deployment",
     "Service",
     "HorizontalPodAutoscaler",
     "ScaledObject",
     "TriggerAuthentication",
@@ -37,18 +40,21 @@
     "Gateway",
     "VirtualService",
     "ServiceMonitor",
 ]
 
 
 class CustomResource:
+    metadata: Optional[client.V1ObjectMeta]
+    kind: Optional[str]
+
     def __init__(
         self,
         api_version: str,
-        kind: KubernetesResourceKind,
+        kind: str,
         plural: str,
         spec: Dict[str, Any],
         metadata: client.V1ObjectMeta,
         status: Optional[Dict[str, Any]] = None,
     ):
         # Ensure api_version is in the format group/version
         if not re.match(r"^.+/v[\w]+$", api_version):
@@ -59,14 +65,15 @@
         self.plural = plural
         self.metadata = metadata
         self.spec = spec
         self.status = status
 
 
 def create_namespaced_custom_object(namespace: str, resource: CustomResource) -> Any:
+    assert resource.metadata
     body = {
         "apiVersion": resource.api_version,
         "kind": resource.kind,
         "metadata": {
             **resource.metadata.to_dict(),
             "name": resource.metadata.name,
             "namespace": namespace,
@@ -100,14 +107,15 @@
         name=name,
     )
 
 
 def replace_namespaced_custom_object(
     name: str, namespace: str, resource: CustomResource
 ) -> Any:
+    assert resource.metadata
     res = read_namespaced_custom_object(name, namespace, resource)
     body = {
         "apiVersion": resource.api_version,
         "kind": resource.kind,
         "metadata": {
             **resource.metadata.to_dict(),
             "name": resource.metadata.name,
@@ -148,16 +156,16 @@
         namespace=namespace,
         plural=resource.plural,
     )
     return custom_resources.get("items", [])
 
 
 class KubernetesResource(Protocol):
-    metadata: client.V1ObjectMeta
-    kind: KubernetesResourceKind
+    metadata: Optional[client.V1ObjectMeta]
+    kind: Optional[str]
 
 
 def apply_resource(
     resource: KubernetesResource,
 ) -> Any:
     """
     Applies a Kubernetes resource by creating or updating it.
@@ -169,72 +177,76 @@
         Any: The response from the API call.
 
     Raises:
         ValueError: If the resource kind is unsupported.
         ApiException: If an error occurs while creating or updating the resource.
     """
     # Determine the resource kind and prepare the appropriate API client
+    assert resource.metadata and resource.kind
+
     kind = resource.kind
     namespace = resource.metadata.namespace
     if not namespace:
         raise ValueError("Namespace is required")
 
     if kind == "Deployment":
-        api = client.AppsV1Api()
-        create_method = api.create_namespaced_deployment
-        replace_method = api.replace_namespaced_deployment
-        read_method = api.read_namespaced_deployment
+        apps_v1_api = client.AppsV1Api()
+        create_method: Callable[..., Any] = apps_v1_api.create_namespaced_deployment
+        replace_method: Callable[..., Any] = apps_v1_api.replace_namespaced_deployment
+        read_method: Callable[..., Any] = apps_v1_api.read_namespaced_deployment
     elif kind == "Service":
-        api = client.CoreV1Api()
-        create_method = api.create_namespaced_service
-        replace_method = api.replace_namespaced_service
-        read_method = api.read_namespaced_service
+        core_v1_api = client.CoreV1Api()
+        create_method = core_v1_api.create_namespaced_service
+        replace_method = core_v1_api.replace_namespaced_service
+        read_method = core_v1_api.read_namespaced_service
     elif kind == "HorizontalPodAutoscaler":
-        api = client.AutoscalingV2Api()
-        create_method = api.create_namespaced_horizontal_pod_autoscaler
-        replace_method = api.replace_namespaced_horizontal_pod_autoscaler
-        read_method = api.read_namespaced_horizontal_pod_autoscaler
+        auto_scaling_v2_api = client.AutoscalingV2Api()
+        create_method = auto_scaling_v2_api.create_namespaced_horizontal_pod_autoscaler
+        replace_method = (
+            auto_scaling_v2_api.replace_namespaced_horizontal_pod_autoscaler
+        )
+        read_method = auto_scaling_v2_api.read_namespaced_horizontal_pod_autoscaler
     elif kind in [
         "ScaledObject",
         "TriggerAuthentication",
         "Package",
         "Environment",
         "Function",
         "Gateway",
         "VirtualService",
         "ServiceMonitor",
     ]:
         create_method = create_namespaced_custom_object
         replace_method = replace_namespaced_custom_object
         read_method = partial(read_namespaced_custom_object, resource=resource)
     elif kind == "ServiceAccount":
-        api = client.CoreV1Api()
-        create_method = api.create_namespaced_service_account
-        replace_method = api.patch_namespaced_service_account
-        read_method = api.read_namespaced_service_account
+        core_v1_api = client.CoreV1Api()
+        create_method = core_v1_api.create_namespaced_service_account
+        replace_method = core_v1_api.patch_namespaced_service_account
+        read_method = core_v1_api.read_namespaced_service_account
     elif kind == "Secret":
-        api = client.CoreV1Api()
-        create_method = api.create_namespaced_secret
-        replace_method = api.patch_namespaced_secret
-        read_method = api.read_namespaced_secret
+        core_v1_api = client.CoreV1Api()
+        create_method = core_v1_api.create_namespaced_secret
+        replace_method = core_v1_api.patch_namespaced_secret
+        read_method = core_v1_api.read_namespaced_secret
     elif kind == "RoleBinding":
-        api = client.RbacAuthorizationV1Api()
-        create_method = api.create_namespaced_role_binding
-        replace_method = api.patch_namespaced_role_binding
-        read_method = api.read_namespaced_role_binding
+        rbac_authorization_v1_api = client.RbacAuthorizationV1Api()
+        create_method = rbac_authorization_v1_api.create_namespaced_role_binding
+        replace_method = rbac_authorization_v1_api.patch_namespaced_role_binding
+        read_method = rbac_authorization_v1_api.read_namespaced_role_binding
     elif kind == "Role":
-        api = client.RbacAuthorizationV1Api()
-        create_method = api.create_namespaced_role
-        replace_method = api.patch_namespaced_role
-        read_method = api.read_namespaced_role
+        rbac_authorization_v1_api = client.RbacAuthorizationV1Api()
+        create_method = rbac_authorization_v1_api.create_namespaced_role
+        replace_method = rbac_authorization_v1_api.patch_namespaced_role
+        read_method = rbac_authorization_v1_api.read_namespaced_role
     elif kind == "ConfigMap":
-        api = client.CoreV1Api()
-        create_method = api.create_namespaced_config_map
-        replace_method = api.patch_namespaced_config_map
-        read_method = api.read_namespaced_config_map
+        core_v1_api = client.CoreV1Api()
+        create_method = core_v1_api.create_namespaced_config_map
+        replace_method = core_v1_api.patch_namespaced_config_map
+        read_method = core_v1_api.read_namespaced_config_map
     else:
         raise ValueError(f"Unsupported kind: {kind}")
 
     # Try to read (get) the resource; if it exists, replace it, otherwise create it
     try:
         read_method(resource.metadata.name, namespace)
         response = replace_method(resource.metadata.name, namespace, resource)
@@ -287,15 +299,15 @@
     subject_namespace: str,
     service_account_name: str,
 ) -> None:
     role_binding = client.V1RoleBinding(
         kind="RoleBinding",
         metadata=client.V1ObjectMeta(name=binding_name, namespace=binding_namespace),
         subjects=[
-            client.V1Subject(
+            client.RbacV1Subject(
                 kind="ServiceAccount",
                 name=service_account_name,
                 namespace=subject_namespace,
             )
         ],
         role_ref=client.V1RoleRef(
             api_group="rbac.authorization.k8s.io", kind="Role", name=role_name
@@ -352,39 +364,44 @@
     pods = v1.list_namespaced_pod(namespace, label_selector=label_selector)
 
     if len(pods.items) == 0:
         raise Exception(
             f"No available pod for port-forwarding with label selector {label_selector}"
         )
 
-    namespaces: Dict[str, Any] = {}
+    namespaces: Dict[str, List[client.V1Pod]] = {}
     ns_list = []
 
     for pod in pods.items:
-        if pod.metadata.namespace not in namespaces:
-            namespaces[pod.metadata.namespace] = []
-            ns_list.append(pod.metadata.namespace)
-        namespaces[pod.metadata.namespace].append(pod)
+        pod_ns = (
+            pod.metadata.namespace if pod.metadata and pod.metadata.namespace else None
+        )
+        if pod_ns and pod_ns not in namespaces:
+            namespaces[pod_ns] = []
+            ns_list.append(pod_ns)
+        if pod_ns and pod:
+            namespaces[pod_ns].append(pod)
 
     if len(ns_list) > 1:
         raise Exception(
             f"Found pods in {len(namespaces)} namespaces, {', '.join(ns_list)}. Please specify a namespace."
         )
 
     ns = ns_list[0]
-    pods = namespaces.get(ns)
+    target_pods = namespaces.get(ns)
 
-    if pods is None:
+    if target_pods is None:
         raise Exception(f"Error finding pods within the given namespace {ns}")
 
     pod_name = None
     pod_namespace = None
 
-    for pod in pods:
+    for pod in target_pods:
         if is_ready_pod(pod):
+            assert pod.metadata
             pod_name = pod.metadata.name
             pod_namespace = pod.metadata.namespace
             break
 
     if pod_name is None or pod_namespace is None:
         raise Exception(
             f"No ready pod for port-forwarding with label selector {label_selector}"
@@ -422,15 +439,15 @@
 
         except Exception as e:
             pass
         finally:
             client_socket.close()
 
     def _run_forward() -> None:
-        pf = portforward(
+        pf: Any = portforward(
             v1.connect_get_namespaced_pod_portforward,
             pod_name,
             pod_namespace,
             ports=str(container_port),
         )
 
         while not pf.connected:
@@ -581,17 +598,17 @@
 
 def tail_logs(namespace: str, pod_name: str, container_name: str) -> None:
     v1 = client.CoreV1Api()
     w = watch.Watch()
 
     while True:
         pod = v1.read_namespaced_pod(name=pod_name, namespace=namespace)
-        if pod.status.phase == "Running":
+        if pod.status and pod.status.phase == "Running":
             break
-        elif pod.status.phase in ["Failed", "Succeeded"]:
+        elif pod.status and pod.status.phase in ["Failed", "Succeeded"]:
             logger.info(f"\nPod {pod_name} is in phase {pod.status.phase}")
             return
         else:
             # print dot on the same line
             print(".", end="", flush=True)
             time.sleep(1)
 
@@ -610,15 +627,37 @@
     wait=wait_fixed(1),
     retry=retry_if_exception_type(ApiException),
 )
 def remove_crd_finalizers(name: str) -> None:
     try:
         api = client.ApiextensionsV1Api()
         crd = api.read_custom_resource_definition(name)
-        if crd.metadata.finalizers:
+        if crd.metadata and crd.metadata.finalizers:
             body = [{"op": "remove", "path": "/metadata/finalizers"}]
             api.patch_custom_resource_definition(name, body)
     except ApiException as e:
         if e.status == 404:
             pass
         else:
             raise
+
+
+def get_gpu_count(ctx: Context, model_group: CloudModelGroup) -> int:
+    gpu_count = 0
+    if hasattr(model_group, "gpu") and model_group.gpu and model_group.gpu.enabled:
+        if model_group.resourceRequest and model_group.resourceRequest.gpu:
+            gpu_count = model_group.resourceRequest.gpu
+        else:
+            instance_info = get_instance_info(
+                ctx.provider, ctx.region, model_group.nodeType
+            )
+            if not instance_info:
+                raise ValueError(
+                    f"No instance information found for instance type {model_group.nodeType} in {ctx.provider} {ctx.region}"
+                )
+            elif "gpu_count" not in instance_info:
+                raise ValueError(
+                    f"Instance type {model_group.nodeType} in {ctx.provider} {ctx.region} does not have GPU information"
+                )
+            gpu_count = instance_info["gpu_count"]
+
+    return gpu_count
```

### Comparing `paka-0.1.7/paka/logger.py` & `paka-0.1.8/paka/logger.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/model/base_model.py` & `paka-0.1.8/paka/model/base_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/model/hf_model.py` & `paka-0.1.8/paka/model/hf_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/model/http_model.py` & `paka-0.1.8/paka/model/http_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/model/manifest.py` & `paka-0.1.8/paka/model/manifest.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/model/progress_bar.py` & `paka-0.1.8/paka/model/progress_bar.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/model/settings.py` & `paka-0.1.8/paka/model/settings.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/model/store.py` & `paka-0.1.8/paka/model/store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.7/paka/utils.py` & `paka-0.1.8/paka/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         if not has_been_called:
             has_been_called = True
             return func(*args, **kwargs)
 
     return cast(T, wrapper)
 
 
-def to_yaml(obj: Dict[str, Any]) -> str:
+def to_yaml(obj: Dict[Any, Any]) -> str:
     """
     Converts an dictionary to a YAML string.
 
     Args:
         obj (dict): The dictionary to be converted.
 
     Returns:
@@ -371,7 +371,35 @@
     elif k == PulumiStackKey.KUBECONFIG:
         for resource in resources:
             # Since we creating only one secret, there is no need to use the resource urn
             if resource["type"] == "eks:index:Cluster":
                 return resource["outputs"]["core"]["kubeconfig"]
 
     raise Exception(f"Unsupported PulumiStackKey: {k}")
+
+
+@lru_cache(maxsize=100)
+def get_instance_info(provider: str, region: str, instance_type: str) -> Dict[str, Any]:
+    if provider == "aws":
+        # Get the CPU, memory and GPU count for the instance type with boto3
+        ec2 = boto3.client("ec2", region_name=region)
+
+        response = ec2.describe_instance_types(InstanceTypes=[instance_type])  # type: ignore
+
+        instance_types = response.get("InstanceTypes", [])
+        if instance_types:
+            instance_type_info = instance_types[0]
+            gpu_info = instance_type_info.get("GpuInfo", {})
+            gpu, vram = gpu_info.get("Gpus", [{}])[0], gpu_info.get(
+                "TotalGpuMemoryInMiB"
+            )
+            return {
+                "cpu": instance_type_info.get("VCpuInfo", {}).get("DefaultVCpus"),
+                "memory": instance_type_info.get("MemoryInfo", {}).get("SizeInMiB"),
+                "gpu_count": gpu.get("Count"),
+                "vram": vram,
+                "gpu_manufacturer": gpu.get("Manufacturer"),
+                "gpu_name": gpu.get("Name"),
+            }
+    else:
+        raise Exception(f"Unsupported provider: {provider}")
+    raise Exception(f"Unsupported provider: {provider}")
```

### Comparing `paka-0.1.7/pyproject.toml` & `paka-0.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [tool.poetry]
 name = "paka"
-version = "0.1.7"
+version = "0.1.8"
 description = "LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications"
+homepage = "https://github.com/jjleng/paka"
+keywords = ["LLMOps", "RAG", "production", "Cloud"]
 authors = ["Jijun Leng"]
 readme = "README.md"
 
 [tool.codespell]
 check-filenames = true
 
 [tool.mypy]
@@ -52,14 +54,15 @@
 pytest = "^8.1.1"
 pytest-snapshot = "^0.9.0"
 types-requests = "2.31.0.6"
 isort = "^5.13.2"
 types-tabulate = "^0.9.0.20240106"
 pulumi-policy = "^1.11.0"
 moto = "^5.0.5"
-boto3-stubs = { extras = ["ecr", "s3"], version = "^1.34.93" }
+boto3-stubs = { extras = ["ec2", "ecr", "s3"], version = "^1.34.106" }
 types-tqdm = "^4.66.0.20240417"
 pytest-order = "^1.2.1"
+kubernetes-stubs-elephant-fork = "^29.0.0.post1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `paka-0.1.7/PKG-INFO` & `paka-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: paka
-Version: 0.1.7
+Version: 0.1.8
 Summary: LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications
+Home-page: https://github.com/jjleng/paka
+Keywords: LLMOps,RAG,production,Cloud
 Author: Jijun Leng
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

