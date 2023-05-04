# Comparing `tmp/eksupgrade-0.8.3.tar.gz` & `tmp/eksupgrade-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eksupgrade-0.8.3.tar", max compression
+gzip compressed data, was "eksupgrade-0.9.0.tar", max compression
```

## Comparing `eksupgrade-0.8.3.tar` & `eksupgrade-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,24 @@
--rw-r--r--   0        0        0      927 2023-04-01 17:56:17.465851 eksupgrade-0.8.3/LICENSE
--rw-r--r--   0        0        0    12491 2023-04-01 17:56:17.465851 eksupgrade-0.8.3/README.md
--rw-r--r--   0        0        0      138 2023-04-01 17:56:17.465851 eksupgrade-0.8.3/eksupgrade/__init__.py
--rw-r--r--   0        0        0       85 2023-04-01 17:56:17.465851 eksupgrade-0.8.3/eksupgrade/__main__.py
--rw-r--r--   0        0        0     8334 2023-04-01 17:56:17.465851 eksupgrade-0.8.3/eksupgrade/cli.py
--rw-r--r--   0        0        0      804 2023-04-01 17:56:17.465851 eksupgrade-0.8.3/eksupgrade/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-01 17:56:17.465851 eksupgrade-0.8.3/eksupgrade/models/__init__.py
--rw-r--r--   0        0        0     3038 2023-04-01 17:56:17.465851 eksupgrade-0.8.3/eksupgrade/models/base.py
--rw-r--r--   0        0        0    42054 2023-04-01 17:56:17.465851 eksupgrade-0.8.3/eksupgrade/models/eks.py
--rw-r--r--   0        0        0     7750 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/S3Files/coredns.json
--rw-r--r--   0        0        0      626 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/S3Files/kube-proxy-configmap.json
--rw-r--r--   0        0        0     5733 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/S3Files/kube-proxy.json
--rw-r--r--   0        0        0      363 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/S3Files/version_dict.json
--rw-r--r--   0        0        0     3699 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/S3Files/vpc-cni.json
--rw-r--r--   0        0        0        0 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/__init__.py
--rw-r--r--   0        0        0    14242 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/boto_aws.py
--rw-r--r--   0        0        0     3113 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/eks_get_image_type.py
--rw-r--r--   0        0        0    13679 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/k8s_client.py
--rw-r--r--   0        0        0     1717 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/latest_ami.py
--rw-r--r--   0        0        0    48644 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/preflight_module.py
--rw-r--r--   0        0        0     5600 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/src/self_managed.py
--rw-r--r--   0        0        0     5578 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/starter.py
--rw-r--r--   0        0        0     2325 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/eksupgrade/utils.py
--rw-r--r--   0        0        0     2715 2023-04-01 17:56:17.469851 eksupgrade-0.8.3/pyproject.toml
--rw-r--r--   0        0        0    13569 1970-01-01 00:00:00.000000 eksupgrade-0.8.3/setup.py
--rw-r--r--   0        0        0    13660 1970-01-01 00:00:00.000000 eksupgrade-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      927 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/LICENSE
+-rw-r--r--   0        0        0    11018 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/README.md
+-rw-r--r--   0        0        0      138 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/__main__.py
+-rw-r--r--   0        0        0     7445 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/cli.py
+-rw-r--r--   0        0        0      804 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/models/__init__.py
+-rw-r--r--   0        0        0     3038 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/models/base.py
+-rw-r--r--   0        0        0    42054 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/models/eks.py
+-rw-r--r--   0        0        0     7750 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/S3Files/coredns.json
+-rw-r--r--   0        0        0      626 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/S3Files/kube-proxy-configmap.json
+-rw-r--r--   0        0        0     5733 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/S3Files/kube-proxy.json
+-rw-r--r--   0        0        0      363 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/S3Files/version_dict.json
+-rw-r--r--   0        0        0     3699 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/S3Files/vpc-cni.json
+-rw-r--r--   0        0        0        0 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/__init__.py
+-rw-r--r--   0        0        0    14226 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/boto_aws.py
+-rw-r--r--   0        0        0     3113 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/eks_get_image_type.py
+-rw-r--r--   0        0        0    13679 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/k8s_client.py
+-rw-r--r--   0        0        0     1717 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/latest_ami.py
+-rw-r--r--   0        0        0     5600 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/src/self_managed.py
+-rw-r--r--   0        0        0     5578 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/starter.py
+-rw-r--r--   0        0        0     2325 2023-05-04 14:15:17.140774 eksupgrade-0.9.0/eksupgrade/utils.py
+-rw-r--r--   0        0        0     2648 2023-05-04 14:15:17.144774 eksupgrade-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    12187 1970-01-01 00:00:00.000000 eksupgrade-0.9.0/PKG-INFO
```

### Comparing `eksupgrade-0.8.3/LICENSE` & `eksupgrade-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/README.md` & `eksupgrade-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,36 +6,18 @@
 <a href="https://codecov.io/github/aws-samples/eks-cluster-upgrade?branch=main"><img alt="Coverage Status" src="https://codecov.io/github/aws-samples/eks-cluster-upgrade/coverage.svg?branch=main"></a>
 <a href="https://pypi.org/project/eksupgrade/"><img alt="PyPI" src="https://img.shields.io/pypi/v/eksupgrade"></a>
 <a href="https://pepy.tech/project/eksupgrade"><img alt="Downloads" src="https://pepy.tech/badge/eksupgrade"></a>
 </p>
 
 Amazon EKS cluster upgrade is a utility that automates the upgrade process for Amazon EKS clusters.
 
-## Process
 
-The process for upgrading an Amazon EKS cluster using `eksupgrade` consists of primarily of three parts:
+## Checks post v0.9.0
 
-1. Perform pre-flight checks prior to upgrading the cluster
-2. Upgrade the cluster
-3. Evaluate the cluster after upgrade
-
-### Pre-Flight Checks
-
-There are a number of version compatibility constraints, health checks, etc., before a cluster can successfully be upgraded. `eksupgrade` performs the following pre-flight checks:
-
-1. Target Version Compatibility Check - Since any cluster in EKS is always allowed to upgrade to one version above and not beyond, a check for the target version is done as with each upgrade there are a lot of configuration changes and upgrading directly to a higher version can lead to breakdown of the services being provided by it.
-2. Customer Management Key - A cluster might have a CMK Key associated with it, so it is essential to verify if the same exists in user's account before carrying out the upgrade.
-3. Security Group - Every cluster has a security group associated with it to restrict and allow the flow of traffic across it, and therefore it has to be verified whether it exists in the user's VPC or not.
-4. Node group and worker node detail - EKS cluster supports multiple types of node groups. So for the purpose of upgrade, their kubelet version compatibility has to be checked to proceed with the upgrade step.
-5. Subnets - A minimum of 4-5 free IPs are required when doing a cluster upgrade to launch new nodes and node groups with the old ones to keep the services of the cluster running while the upgrade is going on. So check on the existence of the free IPs is performed.
-6. Cluster Roles - There are a lot of important cluster roles required during the upgrade related to addons, nodes, and other components of the cluster without which the cluster upgrade cannot be executed successfully.
-7. Pod Security Policy - EKS privileged role has to be checked to be present with the current pod security policy. (deprecated in Kubernetes v1.21, and removed from Kubernetes in v1.25)
-8. Cluster addons - The cluster addons like kube-proxy, VPC CNI and CoreDNS are essential for running various services across the cluster. The parameters available on these addons which are customized by the users on the target cluster have to be captured while upgrading so that they are to added back to maintain service availability.
-9. Pod Disruption Budget - The existence of PDB has to be checked in the cluster, and minimum and maximum available with it has to be taken into account while upgrading.
-10. Horizontal Pod and Cluster Autoscaler - As the other components are upgraded to the compatible image version, a check is performed to see if Cluster or Horizontal Pod Autoscaler are present. They are reviewed to upgrade to a compatible version with respect to the control plane.
+The pre/post-flight checks are removed in favor of guiding the user to evaluate their clusters with existing tools which handle this better such as **[eksup](https://github.com/clowdhaus/eksup)**. The existing pre/post checks will be replaced with relevant checks specific to the upgrade (based on previous understanding the cluster is eligible for such an upgrade).
 
 ### Cluster Upgrade
 
 1. Control plane upgrade - This is handled entirely by AWS once the version upgrade has been requested.
 2. Identification of Managed and Self-managed node - The worker nodes are identified as EKS managed and Self-managed to perform upgrade.
 3. Managed Node group update - Updates managed node group to the specified version.
 4. Self-managed Node group update
@@ -46,15 +28,15 @@
 ## Pre-Requisites
 
 Before running `eksupgrade`, you will need to have permission for both AWS and the Kubernetes cluster itself.
 
 1. Install `eksupgrade` locally:
 
 ```sh
-pip install eksupgrade
+python -m pip install eksupgrade
 ```
 
 2. Ensure you have the necessary AWS permissions; an example policy of required permissions is listed below:
 
 ```json
 {
   "Version": "2012-10-17",
@@ -115,32 +97,32 @@
 ```
 
 ```sh
  Usage: eksupgrade [OPTIONS] CLUSTER_NAME CLUSTER_VERSION REGION
 
  Run eksupgrade against a target cluster.
 
-╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ *    cluster_name         TEXT  The name of the cluster to be upgraded [default: None] [required]                                                                                                                   │
-│ *    cluster_version      TEXT  The target Kubernetes version to upgrade the cluster to [default: None] [required]                                                                                                  │
-│ *    region               TEXT  The AWS region where the target cluster resides [default: None] [required]                                                                                                          │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --max-retry                                    INTEGER  The most number of times to retry an upgrade [default: 2]                                                                                                   │
-│ --force                 --no-force                      Force the upgrade (e.g. pod eviction with PDB) [default: no-force]                                                                                          │
-│ --preflight             --no-preflight                  Run pre-flight check without upgrade [default: no-preflight]                                                                                                │
-│ --parallel              --no-parallel                   Upgrade all nodegroups in parallel [default: no-parallel]                                                                                                   │
-│ --latest-addons         --no-latest-addons              Upgrade addons to the latest eligible version instead of default [default: no-latest-addons]                                                                │
-│ --disable-checks        --no-disable-checks             Disable the pre-flight and post-flight checks during upgrade scenarios [default: no-disable-checks]                                                         │
-│ --interactive           --no-interactive                If enabled, prompt the user for confirmations [default: interactive]                                                                                        │
-│ --version                                               Display the current eksupgrade version                                                                                                                      │
-│ --install-completion                                    Install completion for the current shell.                                                                                                                   │
-│ --show-completion                                       Show completion for the current shell, to copy it or customize the installation.                                                                            │
-│ --help                                                  Show this message and exit.                                                                                                                                 │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *    cluster_name         TEXT  The name of the cluster to be upgraded [default: None] [required]                                                                                                                                                        │
+│ *    cluster_version      TEXT  The target Kubernetes version to upgrade the cluster to [default: None] [required]                                                                                                                                       │
+│ *    region               TEXT  The AWS region where the target cluster resides [default: None] [required]                                                                                                                                               │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --max-retry                                    INTEGER  The most number of times to retry an upgrade [default: 2]                                                                                                                                        │
+│ --force                 --no-force                      Force the upgrade (e.g. pod eviction with PDB) [default: no-force]                                                                                                                               │
+│ --preflight             --no-preflight                  Run pre-upgrade checks without upgrade [default: no-preflight]                                                                                                                                   │
+│ --parallel              --no-parallel                   Upgrade all nodegroups in parallel [default: no-parallel]                                                                                                                                        │
+│ --latest-addons         --no-latest-addons              Upgrade addons to the latest eligible version instead of default [default: no-latest-addons]                                                                                                     │
+│ --disable-checks        --no-disable-checks             Disable the pre-upgrade and post-upgrade checks during upgrade scenarios [default: no-disable-checks]                                                                                            │
+│ --interactive           --no-interactive                If enabled, prompt the user for confirmations [default: interactive]                                                                                                                             │
+│ --version                                               Display the current eksupgrade version                                                                                                                                                           │
+│ --install-completion                                    Install completion for the current shell.                                                                                                                                                        │
+│ --show-completion                                       Show completion for the current shell, to copy it or customize the installation.                                                                                                                 │
+│ --help                                                  Show this message and exit.                                                                                                                                                                      │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ## Support & Feedback
 
 This project is maintained by AWS Solution Architects and Consultants. It is not part of an AWS service and support is provided best-effort by the maintainers. To post feedback, submit feature ideas, or report bugs, please use the [Issues section](https://github.com/aws-samples/eks-cluster-upgrade/issues) of this repo. If you are interested in contributing, please see the [Contribution guide](https://github.com/aws-samples/eks-cluster-upgrade/blob/main/CONTRIBUTING.md).
 
 ## Security
```

#### html2text {}

```diff
@@ -1,97 +1,66 @@
 # Amazon EKS Upgrade Utility
 [Validation_Status] [E2E_Cluster_Upgrade] [Coverage_Status] [PyPI] [Downloads]
 Amazon EKS cluster upgrade is a utility that automates the upgrade process for
-Amazon EKS clusters. ## Process The process for upgrading an Amazon EKS cluster
-using `eksupgrade` consists of primarily of three parts: 1. Perform pre-flight
-checks prior to upgrading the cluster 2. Upgrade the cluster 3. Evaluate the
-cluster after upgrade ### Pre-Flight Checks There are a number of version
-compatibility constraints, health checks, etc., before a cluster can
-successfully be upgraded. `eksupgrade` performs the following pre-flight
-checks: 1. Target Version Compatibility Check - Since any cluster in EKS is
-always allowed to upgrade to one version above and not beyond, a check for the
-target version is done as with each upgrade there are a lot of configuration
-changes and upgrading directly to a higher version can lead to breakdown of the
-services being provided by it. 2. Customer Management Key - A cluster might
-have a CMK Key associated with it, so it is essential to verify if the same
-exists in user's account before carrying out the upgrade. 3. Security Group -
-Every cluster has a security group associated with it to restrict and allow the
-flow of traffic across it, and therefore it has to be verified whether it
-exists in the user's VPC or not. 4. Node group and worker node detail - EKS
-cluster supports multiple types of node groups. So for the purpose of upgrade,
-their kubelet version compatibility has to be checked to proceed with the
-upgrade step. 5. Subnets - A minimum of 4-5 free IPs are required when doing a
-cluster upgrade to launch new nodes and node groups with the old ones to keep
-the services of the cluster running while the upgrade is going on. So check on
-the existence of the free IPs is performed. 6. Cluster Roles - There are a lot
-of important cluster roles required during the upgrade related to addons,
-nodes, and other components of the cluster without which the cluster upgrade
-cannot be executed successfully. 7. Pod Security Policy - EKS privileged role
-has to be checked to be present with the current pod security policy.
-(deprecated in Kubernetes v1.21, and removed from Kubernetes in v1.25) 8.
-Cluster addons - The cluster addons like kube-proxy, VPC CNI and CoreDNS are
-essential for running various services across the cluster. The parameters
-available on these addons which are customized by the users on the target
-cluster have to be captured while upgrading so that they are to added back to
-maintain service availability. 9. Pod Disruption Budget - The existence of PDB
-has to be checked in the cluster, and minimum and maximum available with it has
-to be taken into account while upgrading. 10. Horizontal Pod and Cluster
-Autoscaler - As the other components are upgraded to the compatible image
-version, a check is performed to see if Cluster or Horizontal Pod Autoscaler
-are present. They are reviewed to upgrade to a compatible version with respect
-to the control plane. ### Cluster Upgrade 1. Control plane upgrade - This is
-handled entirely by AWS once the version upgrade has been requested. 2.
+Amazon EKS clusters. ## Checks post v0.9.0 The pre/post-flight checks are
+removed in favor of guiding the user to evaluate their clusters with existing
+tools which handle this better such as **[eksup](https://github.com/clowdhaus/
+eksup)**. The existing pre/post checks will be replaced with relevant checks
+specific to the upgrade (based on previous understanding the cluster is
+eligible for such an upgrade). ### Cluster Upgrade 1. Control plane upgrade -
+This is handled entirely by AWS once the version upgrade has been requested. 2.
 Identification of Managed and Self-managed node - The worker nodes are
 identified as EKS managed and Self-managed to perform upgrade. 3. Managed Node
 group update - Updates managed node group to the specified version. 4. Self-
 managed Node group update - Launch new nodes with upgraded version and wait
 until they require ready status for next step. - Mark existing nodes as
 unschedulable. - If pod disruption budget (PDB) is present then check for force
 eviction flag (--force) which is given by user, only then evict the pods or
 continue with the flow. ## Pre-Requisites Before running `eksupgrade`, you will
 need to have permission for both AWS and the Kubernetes cluster itself. 1.
-Install `eksupgrade` locally: ```sh pip install eksupgrade ``` 2. Ensure you
-have the necessary AWS permissions; an example policy of required permissions
-is listed below: ```json { "Version": "2012-10-17", "Statement": [ { "Sid":
-"iam", "Effect": "Allow", "Action": [ "iam:GetRole", "sts:GetAccessKeyInfo",
-"sts:GetCallerIdentity", "sts:GetSessionToken" ], "Resource": "*" }, { "Sid":
-"ec2", "Effect": "Allow", "Action": [ "autoscaling:CreateLaunchConfiguration",
-"autoscaling:Describe*", "autoscaling:SetDesiredCapacity", "autoscaling:
-TerminateInstanceInAutoScalingGroup", "autoscaling:UpdateAutoScalingGroup",
-"ec2:Describe*", "ssm:*" ], "Resource": "*" }, { "Sid": "eks", "Effect":
-"Allow", "Action": [ "eks:Describe*", "eks:List*", "eks:UpdateAddon", "eks:
-UpdateClusterVersion", "eks:UpdateNodegroupVersion" ], "Resource": "*" } ] }
-``` 3. Update your local kubeconfig to authenticate to the cluster: ```sh aws
-eks update-kubeconfig --name  --region  ``` ## Usage To view the arguments and
-options, run: ```sh eksupgrade --help ``` ```sh Usage: eksupgrade [OPTIONS]
-CLUSTER_NAME CLUSTER_VERSION REGION Run eksupgrade against a target cluster.
-â­â Arguments
-ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+Install `eksupgrade` locally: ```sh python -m pip install eksupgrade ``` 2.
+Ensure you have the necessary AWS permissions; an example policy of required
+permissions is listed below: ```json { "Version": "2012-10-17", "Statement": [
+{ "Sid": "iam", "Effect": "Allow", "Action": [ "iam:GetRole", "sts:
+GetAccessKeyInfo", "sts:GetCallerIdentity", "sts:GetSessionToken" ],
+"Resource": "*" }, { "Sid": "ec2", "Effect": "Allow", "Action": [ "autoscaling:
+CreateLaunchConfiguration", "autoscaling:Describe*", "autoscaling:
+SetDesiredCapacity", "autoscaling:TerminateInstanceInAutoScalingGroup",
+"autoscaling:UpdateAutoScalingGroup", "ec2:Describe*", "ssm:*" ], "Resource":
+"*" }, { "Sid": "eks", "Effect": "Allow", "Action": [ "eks:Describe*", "eks:
+List*", "eks:UpdateAddon", "eks:UpdateClusterVersion", "eks:
+UpdateNodegroupVersion" ], "Resource": "*" } ] } ``` 3. Update your local
+kubeconfig to authenticate to the cluster: ```sh aws eks update-kubeconfig --
+name  --region  ``` ## Usage To view the arguments and options, run: ```sh
+eksupgrade --help ``` ```sh Usage: eksupgrade [OPTIONS] CLUSTER_NAME
+CLUSTER_VERSION REGION Run eksupgrade against a target cluster. â­â
+Arguments
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â * cluster_name TEXT The name of the cluster to be upgraded [default: None]
 [required] â â * cluster_version TEXT The target Kubernetes version to
 upgrade the cluster to [default: None] [required] â â * region TEXT The AWS
 region where the target cluster resides [default: None] [required] â
-â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 â­â Options
-ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â --max-retry INTEGER The most number of times to retry an upgrade [default:
 2] â â --force --no-force Force the upgrade (e.g. pod eviction with PDB)
-[default: no-force] â â --preflight --no-preflight Run pre-flight check
+[default: no-force] â â --preflight --no-preflight Run pre-upgrade checks
 without upgrade [default: no-preflight] â â --parallel --no-parallel
 Upgrade all nodegroups in parallel [default: no-parallel] â â --latest-
 addons --no-latest-addons Upgrade addons to the latest eligible version instead
 of default [default: no-latest-addons] â â --disable-checks --no-disable-
-checks Disable the pre-flight and post-flight checks during upgrade scenarios
+checks Disable the pre-upgrade and post-upgrade checks during upgrade scenarios
 [default: no-disable-checks] â â --interactive --no-interactive If enabled,
 prompt the user for confirmations [default: interactive] â â --version
 Display the current eksupgrade version â â --install-completion Install
 completion for the current shell. â â --show-completion Show completion for
 the current shell, to copy it or customize the installation. â â --help
 Show this message and exit. â
-â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 ``` ## Support & Feedback This project is maintained by AWS Solution Architects
 and Consultants. It is not part of an AWS service and support is provided best-
 effort by the maintainers. To post feedback, submit feature ideas, or report
 bugs, please use the [Issues section](https://github.com/aws-samples/eks-
 cluster-upgrade/issues) of this repo. If you are interested in contributing,
 please see the [Contribution guide](https://github.com/aws-samples/eks-cluster-
 upgrade/blob/main/CONTRIBUTING.md). ## Security See [CONTRIBUTING]
```

### Comparing `eksupgrade-0.8.3/eksupgrade/cli.py` & `eksupgrade-0.9.0/eksupgrade/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Handle CLI specific logic and module definitions."""
 from __future__ import annotations
 
-import sys
 from queue import Queue
 from typing import Optional
 
 import typer
+import urllib3
 from rich.console import Console
 from rich.table import Table
 
 from eksupgrade import __version__
-from eksupgrade.utils import confirm, echo_error, echo_info, echo_success, echo_warning, get_logger
+from eksupgrade.utils import confirm, echo_error, echo_info, echo_warning, get_logger
 
 from .exceptions import ClusterInactiveException
 from .models.eks import Cluster
 from .src.k8s_client import cluster_auto_enable_disable, is_cluster_auto_scaler_present
-from .src.preflight_module import pre_flight_checks
 from .starter import StatsWorker, actual_update
 
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
 logger = get_logger(__name__)
 app = typer.Typer(help="Automated Amazon EKS cluster upgrade CLI utility")
 console = Console()
 
 
 def version_callback(value: bool) -> None:
     """Handle the version callback."""
@@ -33,55 +34,42 @@
 @app.command()
 def main(
     cluster_name: str = typer.Argument(..., help="The name of the cluster to be upgraded"),
     cluster_version: str = typer.Argument(..., help="The target Kubernetes version to upgrade the cluster to"),
     region: str = typer.Argument(..., help="The AWS region where the target cluster resides"),
     max_retry: int = typer.Option(default=2, help="The most number of times to retry an upgrade"),
     force: bool = typer.Option(default=False, help="Force the upgrade (e.g. pod eviction with PDB)"),
-    preflight: bool = typer.Option(default=False, help="Run pre-flight check without upgrade"),
+    preflight: bool = typer.Option(default=False, help="Run pre-upgrade checks without upgrade"),
     parallel: bool = typer.Option(default=False, help="Upgrade all nodegroups in parallel"),
     latest_addons: bool = typer.Option(
         default=False, help="Upgrade addons to the latest eligible version instead of default"
     ),
     disable_checks: bool = typer.Option(
-        default=False, help="Disable the pre-flight and post-flight checks during upgrade scenarios"
+        default=False, help="Disable the pre-upgrade and post-upgrade checks during upgrade scenarios"
     ),
     interactive: bool = typer.Option(default=True, help="If enabled, prompt the user for confirmations"),
     version: Optional[bool] = typer.Option(
         None, "--version", callback=version_callback, is_eager=True, help="Display the current eksupgrade version"
     ),
 ) -> None:
     """Run eksupgrade against a target cluster."""
     queue = Queue()
     is_present: bool = False
     replicas_value: int = 0
 
-    try:
-        # Preflight Logic
-        if not disable_checks:
-            if not pre_flight_checks(
-                preflight=True,
-                cluster_name=cluster_name,
-                region=region,
-                update_version=cluster_version,
-                force_upgrade=force,
-            ):
-                echo_error(
-                    f"Pre-flight check for cluster {cluster_name} targeting version: {cluster_version} failed!",
-                )
-                sys.exit()
-            else:
-                echo_success(
-                    f"Pre-flight check for the cluster {cluster_name} succeeded!",
-                )
-            if preflight:
-                sys.exit()
-        else:
-            echo_warning("Checks disabled! Pre/post-flight checks not executing!")
+    if disable_checks:
+        echo_warning("--disable-checks is currently unused until the new validation workflows are implemented")
+
+    if preflight:
+        echo_warning(
+            "--preflight is unused and will be removed in an upcoming release. "
+            "Please use an EKS upgrade readiness assessment tool such as: github.com/clowdhaus/eksup"
+        )
 
+    try:
         # Pull cluster details, populating the object for subsequent use throughout the upgrade.
         target_cluster: Cluster = Cluster.get(
             cluster_name=cluster_name, region=region, target_version=cluster_version, latest_addons=latest_addons
         )
         echo_info(
             f"Upgrading cluster: {cluster_name} from version: {target_cluster.version} to {target_cluster.target_version}...",
         )
@@ -165,24 +153,14 @@
 
         if is_present:
             cluster_auto_enable_disable(
                 cluster_name=cluster_name, operation="start", mx_val=replicas_value, region=region
             )
             echo_info("Cluster Autoscaler is Enabled Again")
         echo_info(f"EKS Cluster {cluster_name} UPDATED TO {cluster_version}")
-
-        if not disable_checks:
-            if not pre_flight_checks(preflight=False, cluster_name=cluster_name, region=region, force_upgrade=force):
-                echo_error(
-                    f"Post flight check for cluster {cluster_name} failed after it upgraded",
-                )
-            else:
-                echo_success("After update check for cluster completed successfully")
-        else:
-            echo_warning("Post-flight check was disabled and didn't run.")
     except typer.Abort:
         echo_warning("Cluster upgrade aborted!")
     except Exception as error:
         if is_present:
             try:
                 cluster_auto_enable_disable(
                     cluster_name=cluster_name, operation="start", mx_val=replicas_value, region=region
```

### Comparing `eksupgrade-0.8.3/eksupgrade/exceptions.py` & `eksupgrade-0.9.0/eksupgrade/exceptions.py`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/models/base.py` & `eksupgrade-0.9.0/eksupgrade/models/base.py`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/models/eks.py` & `eksupgrade-0.9.0/eksupgrade/models/eks.py`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/src/S3Files/coredns.json` & `eksupgrade-0.9.0/eksupgrade/src/S3Files/coredns.json`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/src/S3Files/kube-proxy-configmap.json` & `eksupgrade-0.9.0/eksupgrade/src/S3Files/kube-proxy-configmap.json`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/src/S3Files/kube-proxy.json` & `eksupgrade-0.9.0/eksupgrade/src/S3Files/kube-proxy.json`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/src/S3Files/vpc-cni.json` & `eksupgrade-0.9.0/eksupgrade/src/S3Files/vpc-cni.json`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/src/boto_aws.py` & `eksupgrade-0.9.0/eksupgrade/src/boto_aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,20 +216,20 @@
     old_lt_instance_ids = []
     instances = []
 
     response = asg_client.describe_auto_scaling_groups(AutoScalingGroupNames=[asg_name])
     asg_lt_name = ""
     # finding the launch type
     if "LaunchTemplate" in response["AutoScalingGroups"][0]:
-        lt_id = response["AutoScalingGroups"][0]["LaunchTemplate"]["LaunchTemplateId"]
+        response["AutoScalingGroups"][0]["LaunchTemplate"]["LaunchTemplateId"]
         asg_lt_name = response["AutoScalingGroups"][0]["LaunchTemplate"]["LaunchTemplateName"]
     elif "MixedInstancesPolicy" in response["AutoScalingGroups"][0]:
-        lt_id = response["AutoScalingGroups"][0]["MixedInstancesPolicy"]["LaunchTemplate"][
-            "LaunchTemplateSpecification"
-        ]["LaunchTemplateId"]
+        response["AutoScalingGroups"][0]["MixedInstancesPolicy"]["LaunchTemplate"]["LaunchTemplateSpecification"][
+            "LaunchTemplateId"
+        ]
         asg_lt_name = response["AutoScalingGroups"][0]["MixedInstancesPolicy"]["LaunchTemplate"][
             "LaunchTemplateSpecification"
         ]["LaunchTemplateName"]
     else:
         echo_error(f"Old Launch Template not found! ASG: {asg_name} - Region: {region}")
         return []
```

### Comparing `eksupgrade-0.8.3/eksupgrade/src/eks_get_image_type.py` & `eksupgrade-0.9.0/eksupgrade/src/eks_get_image_type.py`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/src/k8s_client.py` & `eksupgrade-0.9.0/eksupgrade/src/k8s_client.py`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/src/latest_ami.py` & `eksupgrade-0.9.0/eksupgrade/src/latest_ami.py`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/src/self_managed.py` & `eksupgrade-0.9.0/eksupgrade/src/self_managed.py`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/starter.py` & `eksupgrade-0.9.0/eksupgrade/starter.py`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/eksupgrade/utils.py` & `eksupgrade-0.9.0/eksupgrade/utils.py`

 * *Files identical despite different names*

### Comparing `eksupgrade-0.8.3/pyproject.toml` & `eksupgrade-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eksupgrade"
-version = "0.8.3"
+version = "0.9.0"
 description = "The Amazon EKS cluster upgrade utility"
 authors = ["EKS Upgrade Maintainers <eks-upgrade-maintainers@amazon.com>"]
 readme = "README.md"
 packages = [{include = "eksupgrade"}]
 license = "MIT-0"
 keywords = ["amazon", "aws", "aws-samples", "eks", "kubernetes", "upgrade", "eksupgrade"]
 classifiers = [
@@ -32,35 +32,30 @@
 profile = "black"
 line_length = 120
 
 [tool.black]
 line-length = 120
 target-version = ["py310"]
 
-[tool.pylint]
-max-line-length = 120
-
-[tool.pylint.messages_control]
-max-line-length = 120
-
-[tool.pylint.format]
-max-line-length = 120
-max-module-lines = 1000
+[tool.ruff]
+line-length = 120
+target-version = "py310"
 
 [tool.poe.tasks]
 isort = "isort --profile=black ."
 black = "black ."
 check-black = {cmd = "black . --check --diff", help = "Check code for black styling"}
 check-isort = {cmd = "isort --check --profile=black .", help = "Check code for import styling"}
 check-docstrings = "pydocstyle -e ."
-check-pylint = "pylint eksupgrade"
+check-ruff = "ruff check eksupgrade"
 check = ["check-isort", "check-black"]
-lint = ["check-docstrings", "check-pylint"]
+lint = ["check-docstrings", "check-ruff"]
 fix = ["isort", "black"]
 test = "pytest --cov=eksupgrade --cov-report=xml --cov-report=term"
+ruff = "ruff check --fix eksupgrade"
 safety = "safety check"
 bandit = "bandit -r eksupgrade"
 security = ["safety", "bandit"]
 # requires poethepoet outside of poetry.
 install = "poetry install"
 build = "poetry build"
 
@@ -79,17 +74,17 @@
 moto = {extras = ["autoscaling", "ec2", "eks", "ssm", "sts"], version = "^4.1.5"}
 
 
 [tool.poetry.group.dev.dependencies]
 isort = {extras = ["toml"], version = "^5.12.0"}
 black = "^22.12.0"
 pydocstyle = "^6.3.0"
-pylint = "^2.17.0"
 mypy = "^1.1.1"
 debugpy = "^1.6.6"
+ruff = "^0.0.264"
 
 
 [tool.poetry.group.security.dependencies]
 safety = "^2.3.5"
 bandit = {extras = ["toml"], version = "^1.7.5"}
```

### Comparing `eksupgrade-0.8.3/setup.py` & `eksupgrade-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,162 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: eksupgrade
+Version: 0.9.0
+Summary: The Amazon EKS cluster upgrade utility
+License: MIT-0
+Keywords: amazon,aws,aws-samples,eks,kubernetes,upgrade,eksupgrade
+Author: EKS Upgrade Maintainers
+Author-email: eks-upgrade-maintainers@amazon.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: boto3 (>=1.26.94,<2.0.0)
+Requires-Dist: kubernetes (>=21.0.0,<25.0.0)
+Requires-Dist: packaging (>=21.0,<22.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
+
+# Amazon EKS Upgrade Utility
+
+<p align="center">
+<a href="https://github.com/aws-samples/eks-cluster-upgrade/actions/workflows/validate.yaml"><img alt="Validation Status" src="https://github.com/aws-samples/eks-cluster-upgrade/actions/workflows/validate.yaml/badge.svg?branch=main&event=push"></a>
+<a href="https://github.com/aws-samples/eks-cluster-upgrade/actions/workflows/e2e-test.yaml"><img alt="E2E Cluster Upgrade" src="https://github.com/aws-samples/eks-cluster-upgrade/actions/workflows/e2e-test.yaml/badge.svg?branch=main"></a>
+<a href="https://codecov.io/github/aws-samples/eks-cluster-upgrade?branch=main"><img alt="Coverage Status" src="https://codecov.io/github/aws-samples/eks-cluster-upgrade/coverage.svg?branch=main"></a>
+<a href="https://pypi.org/project/eksupgrade/"><img alt="PyPI" src="https://img.shields.io/pypi/v/eksupgrade"></a>
+<a href="https://pepy.tech/project/eksupgrade"><img alt="Downloads" src="https://pepy.tech/badge/eksupgrade"></a>
+</p>
+
+Amazon EKS cluster upgrade is a utility that automates the upgrade process for Amazon EKS clusters.
+
+
+## Checks post v0.9.0
+
+The pre/post-flight checks are removed in favor of guiding the user to evaluate their clusters with existing tools which handle this better such as **[eksup](https://github.com/clowdhaus/eksup)**. The existing pre/post checks will be replaced with relevant checks specific to the upgrade (based on previous understanding the cluster is eligible for such an upgrade).
+
+### Cluster Upgrade
+
+1. Control plane upgrade - This is handled entirely by AWS once the version upgrade has been requested.
+2. Identification of Managed and Self-managed node - The worker nodes are identified as EKS managed and Self-managed to perform upgrade.
+3. Managed Node group update - Updates managed node group to the specified version.
+4. Self-managed Node group update
+   - Launch new nodes with upgraded version and wait until they require ready status for next step.
+   - Mark existing nodes as unschedulable.
+   - If pod disruption budget (PDB) is present then check for force eviction flag (--force) which is given by user, only then evict the pods or continue with the flow.
+
+## Pre-Requisites
+
+Before running `eksupgrade`, you will need to have permission for both AWS and the Kubernetes cluster itself.
+
+1. Install `eksupgrade` locally:
+
+```sh
+python -m pip install eksupgrade
+```
+
+2. Ensure you have the necessary AWS permissions; an example policy of required permissions is listed below:
+
+```json
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Sid": "iam",
+      "Effect": "Allow",
+      "Action": [
+        "iam:GetRole",
+        "sts:GetAccessKeyInfo",
+        "sts:GetCallerIdentity",
+        "sts:GetSessionToken"
+      ],
+      "Resource": "*"
+    },
+    {
+      "Sid": "ec2",
+      "Effect": "Allow",
+      "Action": [
+        "autoscaling:CreateLaunchConfiguration",
+        "autoscaling:Describe*",
+        "autoscaling:SetDesiredCapacity",
+        "autoscaling:TerminateInstanceInAutoScalingGroup",
+        "autoscaling:UpdateAutoScalingGroup",
+        "ec2:Describe*",
+        "ssm:*"
+      ],
+      "Resource": "*"
+    },
+    {
+      "Sid": "eks",
+      "Effect": "Allow",
+      "Action": [
+        "eks:Describe*",
+        "eks:List*",
+        "eks:UpdateAddon",
+        "eks:UpdateClusterVersion",
+        "eks:UpdateNodegroupVersion"
+      ],
+      "Resource": "*"
+    }
+  ]
+}
+```
 
-packages = \
-['eksupgrade', 'eksupgrade.models', 'eksupgrade.src']
+3. Update your local kubeconfig to authenticate to the cluster:
 
-package_data = \
-{'': ['*'], 'eksupgrade.src': ['S3Files/*']}
+```sh
+aws eks update-kubeconfig --name <CLUSTER-NAME> --region <REGION>
+```
 
-install_requires = \
-['boto3>=1.26.94,<2.0.0',
- 'kubernetes>=21.0.0,<25.0.0',
- 'packaging>=21.0,<22.0',
- 'typer[all]>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['eksupgrade = eksupgrade.cli:app']}
-
-setup_kwargs = {
-    'name': 'eksupgrade',
-    'version': '0.8.3',
-    'description': 'The Amazon EKS cluster upgrade utility',
-    'long_description': '# Amazon EKS Upgrade Utility\n\n<p align="center">\n<a href="https://github.com/aws-samples/eks-cluster-upgrade/actions/workflows/validate.yaml"><img alt="Validation Status" src="https://github.com/aws-samples/eks-cluster-upgrade/actions/workflows/validate.yaml/badge.svg?branch=main&event=push"></a>\n<a href="https://github.com/aws-samples/eks-cluster-upgrade/actions/workflows/e2e-test.yaml"><img alt="E2E Cluster Upgrade" src="https://github.com/aws-samples/eks-cluster-upgrade/actions/workflows/e2e-test.yaml/badge.svg?branch=main"></a>\n<a href="https://codecov.io/github/aws-samples/eks-cluster-upgrade?branch=main"><img alt="Coverage Status" src="https://codecov.io/github/aws-samples/eks-cluster-upgrade/coverage.svg?branch=main"></a>\n<a href="https://pypi.org/project/eksupgrade/"><img alt="PyPI" src="https://img.shields.io/pypi/v/eksupgrade"></a>\n<a href="https://pepy.tech/project/eksupgrade"><img alt="Downloads" src="https://pepy.tech/badge/eksupgrade"></a>\n</p>\n\nAmazon EKS cluster upgrade is a utility that automates the upgrade process for Amazon EKS clusters.\n\n## Process\n\nThe process for upgrading an Amazon EKS cluster using `eksupgrade` consists of primarily of three parts:\n\n1. Perform pre-flight checks prior to upgrading the cluster\n2. Upgrade the cluster\n3. Evaluate the cluster after upgrade\n\n### Pre-Flight Checks\n\nThere are a number of version compatibility constraints, health checks, etc., before a cluster can successfully be upgraded. `eksupgrade` performs the following pre-flight checks:\n\n1. Target Version Compatibility Check - Since any cluster in EKS is always allowed to upgrade to one version above and not beyond, a check for the target version is done as with each upgrade there are a lot of configuration changes and upgrading directly to a higher version can lead to breakdown of the services being provided by it.\n2. Customer Management Key - A cluster might have a CMK Key associated with it, so it is essential to verify if the same exists in user\'s account before carrying out the upgrade.\n3. Security Group - Every cluster has a security group associated with it to restrict and allow the flow of traffic across it, and therefore it has to be verified whether it exists in the user\'s VPC or not.\n4. Node group and worker node detail - EKS cluster supports multiple types of node groups. So for the purpose of upgrade, their kubelet version compatibility has to be checked to proceed with the upgrade step.\n5. Subnets - A minimum of 4-5 free IPs are required when doing a cluster upgrade to launch new nodes and node groups with the old ones to keep the services of the cluster running while the upgrade is going on. So check on the existence of the free IPs is performed.\n6. Cluster Roles - There are a lot of important cluster roles required during the upgrade related to addons, nodes, and other components of the cluster without which the cluster upgrade cannot be executed successfully.\n7. Pod Security Policy - EKS privileged role has to be checked to be present with the current pod security policy. (deprecated in Kubernetes v1.21, and removed from Kubernetes in v1.25)\n8. Cluster addons - The cluster addons like kube-proxy, VPC CNI and CoreDNS are essential for running various services across the cluster. The parameters available on these addons which are customized by the users on the target cluster have to be captured while upgrading so that they are to added back to maintain service availability.\n9. Pod Disruption Budget - The existence of PDB has to be checked in the cluster, and minimum and maximum available with it has to be taken into account while upgrading.\n10. Horizontal Pod and Cluster Autoscaler - As the other components are upgraded to the compatible image version, a check is performed to see if Cluster or Horizontal Pod Autoscaler are present. They are reviewed to upgrade to a compatible version with respect to the control plane.\n\n### Cluster Upgrade\n\n1. Control plane upgrade - This is handled entirely by AWS once the version upgrade has been requested.\n2. Identification of Managed and Self-managed node - The worker nodes are identified as EKS managed and Self-managed to perform upgrade.\n3. Managed Node group update - Updates managed node group to the specified version.\n4. Self-managed Node group update\n   - Launch new nodes with upgraded version and wait until they require ready status for next step.\n   - Mark existing nodes as unschedulable.\n   - If pod disruption budget (PDB) is present then check for force eviction flag (--force) which is given by user, only then evict the pods or continue with the flow.\n\n## Pre-Requisites\n\nBefore running `eksupgrade`, you will need to have permission for both AWS and the Kubernetes cluster itself.\n\n1. Install `eksupgrade` locally:\n\n```sh\npip install eksupgrade\n```\n\n2. Ensure you have the necessary AWS permissions; an example policy of required permissions is listed below:\n\n```json\n{\n  "Version": "2012-10-17",\n  "Statement": [\n    {\n      "Sid": "iam",\n      "Effect": "Allow",\n      "Action": [\n        "iam:GetRole",\n        "sts:GetAccessKeyInfo",\n        "sts:GetCallerIdentity",\n        "sts:GetSessionToken"\n      ],\n      "Resource": "*"\n    },\n    {\n      "Sid": "ec2",\n      "Effect": "Allow",\n      "Action": [\n        "autoscaling:CreateLaunchConfiguration",\n        "autoscaling:Describe*",\n        "autoscaling:SetDesiredCapacity",\n        "autoscaling:TerminateInstanceInAutoScalingGroup",\n        "autoscaling:UpdateAutoScalingGroup",\n        "ec2:Describe*",\n        "ssm:*"\n      ],\n      "Resource": "*"\n    },\n    {\n      "Sid": "eks",\n      "Effect": "Allow",\n      "Action": [\n        "eks:Describe*",\n        "eks:List*",\n        "eks:UpdateAddon",\n        "eks:UpdateClusterVersion",\n        "eks:UpdateNodegroupVersion"\n      ],\n      "Resource": "*"\n    }\n  ]\n}\n```\n\n3. Update your local kubeconfig to authenticate to the cluster:\n\n```sh\naws eks update-kubeconfig --name <CLUSTER-NAME> --region <REGION>\n```\n\n## Usage\n\nTo view the arguments and options, run:\n\n```sh\neksupgrade --help\n```\n\n```sh\n Usage: eksupgrade [OPTIONS] CLUSTER_NAME CLUSTER_VERSION REGION\n\n Run eksupgrade against a target cluster.\n\n╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ *    cluster_name         TEXT  The name of the cluster to be upgraded [default: None] [required]                                                                                                                   │\n│ *    cluster_version      TEXT  The target Kubernetes version to upgrade the cluster to [default: None] [required]                                                                                                  │\n│ *    region               TEXT  The AWS region where the target cluster resides [default: None] [required]                                                                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --max-retry                                    INTEGER  The most number of times to retry an upgrade [default: 2]                                                                                                   │\n│ --force                 --no-force                      Force the upgrade (e.g. pod eviction with PDB) [default: no-force]                                                                                          │\n│ --preflight             --no-preflight                  Run pre-flight check without upgrade [default: no-preflight]                                                                                                │\n│ --parallel              --no-parallel                   Upgrade all nodegroups in parallel [default: no-parallel]                                                                                                   │\n│ --latest-addons         --no-latest-addons              Upgrade addons to the latest eligible version instead of default [default: no-latest-addons]                                                                │\n│ --disable-checks        --no-disable-checks             Disable the pre-flight and post-flight checks during upgrade scenarios [default: no-disable-checks]                                                         │\n│ --interactive           --no-interactive                If enabled, prompt the user for confirmations [default: interactive]                                                                                        │\n│ --version                                               Display the current eksupgrade version                                                                                                                      │\n│ --install-completion                                    Install completion for the current shell.                                                                                                                   │\n│ --show-completion                                       Show completion for the current shell, to copy it or customize the installation.                                                                            │\n│ --help                                                  Show this message and exit.                                                                                                                                 │\n╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n## Support & Feedback\n\nThis project is maintained by AWS Solution Architects and Consultants. It is not part of an AWS service and support is provided best-effort by the maintainers. To post feedback, submit feature ideas, or report bugs, please use the [Issues section](https://github.com/aws-samples/eks-cluster-upgrade/issues) of this repo. If you are interested in contributing, please see the [Contribution guide](https://github.com/aws-samples/eks-cluster-upgrade/blob/main/CONTRIBUTING.md).\n\n## Security\n\nSee [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.\n\n## License\n\nThis library is licensed under the MIT-0 License. See the [LICENSE](LICENSE) file.\n',
-    'author': 'EKS Upgrade Maintainers',
-    'author_email': 'eks-upgrade-maintainers@amazon.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## Usage
+
+To view the arguments and options, run:
+
+```sh
+eksupgrade --help
+```
+
+```sh
+ Usage: eksupgrade [OPTIONS] CLUSTER_NAME CLUSTER_VERSION REGION
+
+ Run eksupgrade against a target cluster.
+
+╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *    cluster_name         TEXT  The name of the cluster to be upgraded [default: None] [required]                                                                                                                                                        │
+│ *    cluster_version      TEXT  The target Kubernetes version to upgrade the cluster to [default: None] [required]                                                                                                                                       │
+│ *    region               TEXT  The AWS region where the target cluster resides [default: None] [required]                                                                                                                                               │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --max-retry                                    INTEGER  The most number of times to retry an upgrade [default: 2]                                                                                                                                        │
+│ --force                 --no-force                      Force the upgrade (e.g. pod eviction with PDB) [default: no-force]                                                                                                                               │
+│ --preflight             --no-preflight                  Run pre-upgrade checks without upgrade [default: no-preflight]                                                                                                                                   │
+│ --parallel              --no-parallel                   Upgrade all nodegroups in parallel [default: no-parallel]                                                                                                                                        │
+│ --latest-addons         --no-latest-addons              Upgrade addons to the latest eligible version instead of default [default: no-latest-addons]                                                                                                     │
+│ --disable-checks        --no-disable-checks             Disable the pre-upgrade and post-upgrade checks during upgrade scenarios [default: no-disable-checks]                                                                                            │
+│ --interactive           --no-interactive                If enabled, prompt the user for confirmations [default: interactive]                                                                                                                             │
+│ --version                                               Display the current eksupgrade version                                                                                                                                                           │
+│ --install-completion                                    Install completion for the current shell.                                                                                                                                                        │
+│ --show-completion                                       Show completion for the current shell, to copy it or customize the installation.                                                                                                                 │
+│ --help                                                  Show this message and exit.                                                                                                                                                                      │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+## Support & Feedback
+
+This project is maintained by AWS Solution Architects and Consultants. It is not part of an AWS service and support is provided best-effort by the maintainers. To post feedback, submit feature ideas, or report bugs, please use the [Issues section](https://github.com/aws-samples/eks-cluster-upgrade/issues) of this repo. If you are interested in contributing, please see the [Contribution guide](https://github.com/aws-samples/eks-cluster-upgrade/blob/main/CONTRIBUTING.md).
+
+## Security
+
+See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
+
+## License
 
+This library is licensed under the MIT-0 License. See the [LICENSE](LICENSE) file.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,115 +1,84 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['eksupgrade', 'eksupgrade.models', 'eksupgrade.src'] package_data = \ {'':
-['*'], 'eksupgrade.src': ['S3Files/*']} install_requires = \
-['boto3>=1.26.94,<2.0.0', 'kubernetes>=21.0.0,<25.0.0',
-'packaging>=21.0,<22.0', 'typer[all]>=0.7.0,<0.8.0'] entry_points = \
-{'console_scripts': ['eksupgrade = eksupgrade.cli:app']} setup_kwargs =
-{ 'name': 'eksupgrade', 'version': '0.8.3', 'description': 'The Amazon EKS
-cluster upgrade utility', 'long_description': '# Amazon EKS Upgrade Utility\n\n
-   \n[Validation_Status]\n[E2E_Cluster_Upgrade]\n[Coverage_Status]\n[PyPI]\n
-                                 [Downloads]\n
-\n\nAmazon EKS cluster upgrade is a utility that automates the upgrade process
-for Amazon EKS clusters.\n\n## Process\n\nThe process for upgrading an Amazon
-EKS cluster using `eksupgrade` consists of primarily of three parts:\n\n1.
-Perform pre-flight checks prior to upgrading the cluster\n2. Upgrade the
-cluster\n3. Evaluate the cluster after upgrade\n\n### Pre-Flight
-Checks\n\nThere are a number of version compatibility constraints, health
-checks, etc., before a cluster can successfully be upgraded. `eksupgrade`
-performs the following pre-flight checks:\n\n1. Target Version Compatibility
-Check - Since any cluster in EKS is always allowed to upgrade to one version
-above and not beyond, a check for the target version is done as with each
-upgrade there are a lot of configuration changes and upgrading directly to a
-higher version can lead to breakdown of the services being provided by it.\n2.
-Customer Management Key - A cluster might have a CMK Key associated with it, so
-it is essential to verify if the same exists in user\'s account before carrying
-out the upgrade.\n3. Security Group - Every cluster has a security group
-associated with it to restrict and allow the flow of traffic across it, and
-therefore it has to be verified whether it exists in the user\'s VPC or
-not.\n4. Node group and worker node detail - EKS cluster supports multiple
-types of node groups. So for the purpose of upgrade, their kubelet version
-compatibility has to be checked to proceed with the upgrade step.\n5. Subnets -
-A minimum of 4-5 free IPs are required when doing a cluster upgrade to launch
-new nodes and node groups with the old ones to keep the services of the cluster
-running while the upgrade is going on. So check on the existence of the free
-IPs is performed.\n6. Cluster Roles - There are a lot of important cluster
-roles required during the upgrade related to addons, nodes, and other
-components of the cluster without which the cluster upgrade cannot be executed
-successfully.\n7. Pod Security Policy - EKS privileged role has to be checked
-to be present with the current pod security policy. (deprecated in Kubernetes
-v1.21, and removed from Kubernetes in v1.25)\n8. Cluster addons - The cluster
-addons like kube-proxy, VPC CNI and CoreDNS are essential for running various
-services across the cluster. The parameters available on these addons which are
-customized by the users on the target cluster have to be captured while
-upgrading so that they are to added back to maintain service availability.\n9.
-Pod Disruption Budget - The existence of PDB has to be checked in the cluster,
-and minimum and maximum available with it has to be taken into account while
-upgrading.\n10. Horizontal Pod and Cluster Autoscaler - As the other components
-are upgraded to the compatible image version, a check is performed to see if
-Cluster or Horizontal Pod Autoscaler are present. They are reviewed to upgrade
-to a compatible version with respect to the control plane.\n\n### Cluster
-Upgrade\n\n1. Control plane upgrade - This is handled entirely by AWS once the
-version upgrade has been requested.\n2. Identification of Managed and Self-
-managed node - The worker nodes are identified as EKS managed and Self-managed
-to perform upgrade.\n3. Managed Node group update - Updates managed node group
-to the specified version.\n4. Self-managed Node group update\n - Launch new
-nodes with upgraded version and wait until they require ready status for next
-step.\n - Mark existing nodes as unschedulable.\n - If pod disruption budget
-(PDB) is present then check for force eviction flag (--force) which is given by
-user, only then evict the pods or continue with the flow.\n\n## Pre-
-Requisites\n\nBefore running `eksupgrade`, you will need to have permission for
-both AWS and the Kubernetes cluster itself.\n\n1. Install `eksupgrade` locally:
-\n\n```sh\npip install eksupgrade\n```\n\n2. Ensure you have the necessary AWS
-permissions; an example policy of required permissions is listed below:
-\n\n```json\n{\n "Version": "2012-10-17",\n "Statement": [\n {\n "Sid":
-"iam",\n "Effect": "Allow",\n "Action": [\n "iam:GetRole",\n "sts:
-GetAccessKeyInfo",\n "sts:GetCallerIdentity",\n "sts:GetSessionToken"\n ],\n
-"Resource": "*"\n },\n {\n "Sid": "ec2",\n "Effect": "Allow",\n "Action": [\n
-"autoscaling:CreateLaunchConfiguration",\n "autoscaling:Describe*",\n
-"autoscaling:SetDesiredCapacity",\n "autoscaling:
-TerminateInstanceInAutoScalingGroup",\n "autoscaling:UpdateAutoScalingGroup",\n
-"ec2:Describe*",\n "ssm:*"\n ],\n "Resource": "*"\n },\n {\n "Sid": "eks",\n
-"Effect": "Allow",\n "Action": [\n "eks:Describe*",\n "eks:List*",\n "eks:
-UpdateAddon",\n "eks:UpdateClusterVersion",\n "eks:UpdateNodegroupVersion"\n
-],\n "Resource": "*"\n }\n ]\n}\n```\n\n3. Update your local kubeconfig to
-authenticate to the cluster:\n\n```sh\naws eks update-kubeconfig --name  --
-region \n```\n\n## Usage\n\nTo view the arguments and options, run:
-\n\n```sh\neksupgrade --help\n```\n\n```sh\n Usage: eksupgrade [OPTIONS]
-CLUSTER_NAME CLUSTER_VERSION REGION\n\n Run eksupgrade against a target
-cluster.\n\nâ­â Arguments
-ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®\nâ
-* cluster_name TEXT The name of the cluster to be upgraded [default: None]
-[required] â\nâ * cluster_version TEXT The target Kubernetes version to
-upgrade the cluster to [default: None] [required] â\nâ * region TEXT The
-AWS region where the target cluster resides [default: None] [required]
-â\nâ°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯\nâ­â
-Options
-ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®\nâ
---max-retry INTEGER The most number of times to retry an upgrade [default: 2]
-â\nâ --force --no-force Force the upgrade (e.g. pod eviction with PDB)
-[default: no-force] â\nâ --preflight --no-preflight Run pre-flight check
-without upgrade [default: no-preflight] â\nâ --parallel --no-parallel
-Upgrade all nodegroups in parallel [default: no-parallel] â\nâ --latest-
+Metadata-Version: 2.1 Name: eksupgrade Version: 0.9.0 Summary: The Amazon EKS
+cluster upgrade utility License: MIT-0 Keywords: amazon,aws,aws-
+samples,eks,kubernetes,upgrade,eksupgrade Author: EKS Upgrade Maintainers
+Author-email: eks-upgrade-maintainers@amazon.com Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
+Classifier: License :: Other/Proprietary License Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist:
+boto3 (>=1.26.94,<2.0.0) Requires-Dist: kubernetes (>=21.0.0,<25.0.0) Requires-
+Dist: packaging (>=21.0,<22.0) Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown # Amazon EKS Upgrade Utility
+[Validation_Status] [E2E_Cluster_Upgrade] [Coverage_Status] [PyPI] [Downloads]
+Amazon EKS cluster upgrade is a utility that automates the upgrade process for
+Amazon EKS clusters. ## Checks post v0.9.0 The pre/post-flight checks are
+removed in favor of guiding the user to evaluate their clusters with existing
+tools which handle this better such as **[eksup](https://github.com/clowdhaus/
+eksup)**. The existing pre/post checks will be replaced with relevant checks
+specific to the upgrade (based on previous understanding the cluster is
+eligible for such an upgrade). ### Cluster Upgrade 1. Control plane upgrade -
+This is handled entirely by AWS once the version upgrade has been requested. 2.
+Identification of Managed and Self-managed node - The worker nodes are
+identified as EKS managed and Self-managed to perform upgrade. 3. Managed Node
+group update - Updates managed node group to the specified version. 4. Self-
+managed Node group update - Launch new nodes with upgraded version and wait
+until they require ready status for next step. - Mark existing nodes as
+unschedulable. - If pod disruption budget (PDB) is present then check for force
+eviction flag (--force) which is given by user, only then evict the pods or
+continue with the flow. ## Pre-Requisites Before running `eksupgrade`, you will
+need to have permission for both AWS and the Kubernetes cluster itself. 1.
+Install `eksupgrade` locally: ```sh python -m pip install eksupgrade ``` 2.
+Ensure you have the necessary AWS permissions; an example policy of required
+permissions is listed below: ```json { "Version": "2012-10-17", "Statement": [
+{ "Sid": "iam", "Effect": "Allow", "Action": [ "iam:GetRole", "sts:
+GetAccessKeyInfo", "sts:GetCallerIdentity", "sts:GetSessionToken" ],
+"Resource": "*" }, { "Sid": "ec2", "Effect": "Allow", "Action": [ "autoscaling:
+CreateLaunchConfiguration", "autoscaling:Describe*", "autoscaling:
+SetDesiredCapacity", "autoscaling:TerminateInstanceInAutoScalingGroup",
+"autoscaling:UpdateAutoScalingGroup", "ec2:Describe*", "ssm:*" ], "Resource":
+"*" }, { "Sid": "eks", "Effect": "Allow", "Action": [ "eks:Describe*", "eks:
+List*", "eks:UpdateAddon", "eks:UpdateClusterVersion", "eks:
+UpdateNodegroupVersion" ], "Resource": "*" } ] } ``` 3. Update your local
+kubeconfig to authenticate to the cluster: ```sh aws eks update-kubeconfig --
+name  --region  ``` ## Usage To view the arguments and options, run: ```sh
+eksupgrade --help ``` ```sh Usage: eksupgrade [OPTIONS] CLUSTER_NAME
+CLUSTER_VERSION REGION Run eksupgrade against a target cluster. â­â
+Arguments
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * cluster_name TEXT The name of the cluster to be upgraded [default: None]
+[required] â â * cluster_version TEXT The target Kubernetes version to
+upgrade the cluster to [default: None] [required] â â * region TEXT The AWS
+region where the target cluster resides [default: None] [required] â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --max-retry INTEGER The most number of times to retry an upgrade [default:
+2] â â --force --no-force Force the upgrade (e.g. pod eviction with PDB)
+[default: no-force] â â --preflight --no-preflight Run pre-upgrade checks
+without upgrade [default: no-preflight] â â --parallel --no-parallel
+Upgrade all nodegroups in parallel [default: no-parallel] â â --latest-
 addons --no-latest-addons Upgrade addons to the latest eligible version instead
-of default [default: no-latest-addons] â\nâ --disable-checks --no-disable-
-checks Disable the pre-flight and post-flight checks during upgrade scenarios
-[default: no-disable-checks] â\nâ --interactive --no-interactive If
-enabled, prompt the user for confirmations [default: interactive] â\nâ --
-version Display the current eksupgrade version â\nâ --install-completion
-Install completion for the current shell. â\nâ --show-completion Show
-completion for the current shell, to copy it or customize the installation.
-â\nâ --help Show this message and exit.
-â\nâ°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯\n```\n##
-Support & Feedback\n\nThis project is maintained by AWS Solution Architects and
-Consultants. It is not part of an AWS service and support is provided best-
+of default [default: no-latest-addons] â â --disable-checks --no-disable-
+checks Disable the pre-upgrade and post-upgrade checks during upgrade scenarios
+[default: no-disable-checks] â â --interactive --no-interactive If enabled,
+prompt the user for confirmations [default: interactive] â â --version
+Display the current eksupgrade version â â --install-completion Install
+completion for the current shell. â â --show-completion Show completion for
+the current shell, to copy it or customize the installation. â â --help
+Show this message and exit. â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ## Support & Feedback This project is maintained by AWS Solution Architects
+and Consultants. It is not part of an AWS service and support is provided best-
 effort by the maintainers. To post feedback, submit feature ideas, or report
 bugs, please use the [Issues section](https://github.com/aws-samples/eks-
 cluster-upgrade/issues) of this repo. If you are interested in contributing,
 please see the [Contribution guide](https://github.com/aws-samples/eks-cluster-
-upgrade/blob/main/CONTRIBUTING.md).\n\n## Security\n\nSee [CONTRIBUTING]
-(CONTRIBUTING.md#security-issue-notifications) for more information.\n\n##
-License\n\nThis library is licensed under the MIT-0 License. See the [LICENSE]
-(LICENSE) file.\n', 'author': 'EKS Upgrade Maintainers', 'author_email': 'eks-
-upgrade-maintainers@amazon.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+upgrade/blob/main/CONTRIBUTING.md). ## Security See [CONTRIBUTING]
+(CONTRIBUTING.md#security-issue-notifications) for more information. ## License
+This library is licensed under the MIT-0 License. See the [LICENSE](LICENSE)
+file.
```

