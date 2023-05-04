# Comparing `tmp/backend.ai-manager-23.3.0a4.tar.gz` & `tmp/backend.ai-manager-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-manager-23.3.0a4.tar", last modified: Thu Mar 16 02:53:06 2023, max compression
+gzip compressed data, was "backend.ai-manager-23.3.1.tar", last modified: Thu May  4 05:10:19 2023, max compression
```

## Comparing `backend.ai-manager-23.3.0a4.tar` & `backend.ai-manager-23.3.1.tar`

### file list

```diff
@@ -1,237 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.036398 backend.ai-manager-23.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-03-16 02:53:06.036398 backend.ai-manager-23.3.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:05.996396 backend.ai-manager-23.3.0a4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:05.996396 backend.ai-manager-23.3.0a4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.000397 backend.ai-manager-23.3.0a4/ai/backend/manager/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.004397 backend.ai-manager-23.3.0a4/ai/backend/manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    37092 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15547 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/domainconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/groupconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)    35535 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)   107799 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    32708 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/userconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   111054 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/api/wsproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.008397 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/cli/image_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24884 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.008397 backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/harbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/idle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.012397 backend.ai-manager-23.3.0a4/ai/backend/manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.012397 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.032398 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
--rw-r--r--   0 runner    (1001) docker     (123)    23603 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d643752544de_.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/error_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48265 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    24502 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31774 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    48385 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20617 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.032398 backend.ai-manager-23.3.0a4/ai/backend/manager/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/minilang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/minilang/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/minilang/queryfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/resource_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    49485 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    41869 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    44934 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/models/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/pglock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.032398 backend.ai-manager-23.3.0a4/ai/backend/manager/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/plugin/error_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/plugin/webapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   122903 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.032398 backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51411 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/drf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/mof.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/ai/backend/manager/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:06.036398 backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:53:06.036398 backend.ai-manager-23.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-03-16 02:53:05.000000 backend.ai-manager-23.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.222647 backend.ai-manager-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-04 05:10:19.222647 backend.ai-manager-23.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.202647 backend.ai-manager-23.3.1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.202647 backend.ai-manager-23.3.1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.202647 backend.ai-manager-23.3.1/ai/backend/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.206647 backend.ai-manager-23.3.1/ai/backend/manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37001 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/domainconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/groupconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112264 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/userconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117914 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/api/wsproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.206647 backend.ai-manager-23.3.1/ai/backend/manager/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/cli/dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/cli/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/cli/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/cli/image_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25517 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.206647 backend.ai-manager-23.3.1/ai/backend/manager/container_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/container_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/container_registry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/container_registry/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/container_registry/harbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/container_registry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39619 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/idle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.210647 backend.ai-manager-23.3.1/ai/backend/manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.210647 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.222647 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23603 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d643752544de_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33845 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/error_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48343 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31774 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.222647 backend.ai-manager-23.3.1/ai/backend/manager/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/minilang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/minilang/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/minilang/queryfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/resource_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41915 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/models/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/pglock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.222647 backend.ai-manager-23.3.1/ai/backend/manager/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/plugin/error_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/plugin/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   113474 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.222647 backend.ai-manager-23.3.1/ai/backend/manager/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52451 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/scheduler/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/scheduler/drf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/scheduler/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/scheduler/mof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/scheduler/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/scheduler/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29977 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/ai/backend/manager/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:19.222647 backend.ai-manager-23.3.1/backend.ai_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-04 05:10:19.000000 backend.ai-manager-23.3.1/backend.ai_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-05-04 05:10:19.000000 backend.ai-manager-23.3.1/backend.ai_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:19.000000 backend.ai-manager-23.3.1/backend.ai_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-04 05:10:19.000000 backend.ai-manager-23.3.1/backend.ai_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:19.000000 backend.ai-manager-23.3.1/backend.ai_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:19.000000 backend.ai-manager-23.3.1/backend.ai_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-04 05:10:19.000000 backend.ai-manager-23.3.1/backend.ai_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:19.000000 backend.ai-manager-23.3.1/backend.ai_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:19.226647 backend.ai-manager-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-05-04 05:10:18.000000 backend.ai-manager-23.3.1/setup.py
```

### Comparing `backend.ai-manager-23.3.0a4/PKG-INFO` & `backend.ai-manager-23.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 Backend.AI Manager with API Gateway
 ===================================
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/acl.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/admin.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         redis_image=root_ctx.redis_image,
         redis_live=root_ctx.redis_live,
         manager_status=manager_status,
         known_slot_types=known_slot_types,
         background_task_manager=root_ctx.background_task_manager,
         storage_manager=root_ctx.storage_manager,
         registry=root_ctx.registry,
+        idle_checker_host=root_ctx.idle_checker_host,
     )
     result = app_ctx.gql_schema.execute(
         params["query"],
         app_ctx.gql_executor,
         variable_values=params["variables"],
         operation_name=params["operation_name"],
         context_value=gql_ctx,
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/auth.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,28 +349,24 @@
         body = b""
         if api_version < "v4.20181215":
             if request.can_read_body and request.content_type != "multipart/form-data":
                 # read the whole body if neither streaming nor bodyless
                 body = await request.read()
         body_hash = hashlib.new(hash_type, body).hexdigest()
 
-        sign_bytes = (
-            ("{0}\n{1}\n{2}\nhost:{3}\ncontent-type:{4}\n" "x-{name}-version:{5}\n{6}")
-            .format(
-                request.method,
-                str(request.raw_path),
-                request["raw_date"],
-                request.host,
-                request.content_type,
-                api_version,
-                body_hash,
-                name="backendai" if new_api_version is not None else "sorna",
-            )
-            .encode()
-        )
+        sign_bytes = "{0}\n{1}\n{2}\nhost:{3}\ncontent-type:{4}\nx-{name}-version:{5}\n{6}".format(
+            request.method,
+            str(request.raw_path),
+            request["raw_date"],
+            request.host,
+            request.content_type,
+            api_version,
+            body_hash,
+            name="backendai" if new_api_version is not None else "sorna",
+        ).encode()
         sign_key = hmac.new(
             secret_key.encode(), request["date"].strftime("%Y%m%d").encode(), hash_type
         ).digest()
         sign_key = hmac.new(sign_key, request.host.encode(), hash_type).digest()
         return hmac.new(sign_key, sign_bytes, hash_type).hexdigest()
     except ValueError:
         raise AuthorizationFailed("Invalid signature")
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/cluster_template.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/cluster_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 import trafaret as t
 import yaml
 from aiohttp import web
 
 from ai.backend.common import validators as tx
 from ai.backend.common.logging import BraceStyleAdapter
 
-from ..models import TemplateType, UserRole
+from ..models import (
+    TemplateType,
+    UserRole,
+)
 from ..models import association_groups_users as agus
 from ..models import (
     domains,
     groups,
     keypairs,
     query_accessible_session_templates,
     session_templates,
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/context.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/domainconfig.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/domainconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/etcd.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/etcd.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,16 @@
 
 
 @superadmin_required
 @check_api_params(
     t.Dict(
         {
             t.Key("key"): t.String,
-            t.Key("value"): (
-                t.String(allow_blank=True) | t.Mapping(t.String(allow_blank=True), t.Any)
+            t.Key("value"): t.String(allow_blank=True) | t.Mapping(
+                t.String(allow_blank=True), t.Any
             ),
         }
     )
 )
 async def set_config(request: web.Request, params: Any) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
     log.info(
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/events.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/exceptions.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,18 +60,18 @@
             lines.append(" -> extra_data: " + repr(self.extra_data))
         return "\n".join(lines)
 
     def __repr__(self):
         lines = []
         if self.extra_msg:
             lines.append(
-                f"<{type(self).__name__}({self.status}): " f"{self.error_title} ({self.extra_msg})>"
+                f"<{type(self).__name__}({self.status}): {self.error_title} ({self.extra_msg})>"
             )
         else:
-            lines.append(f"<{type(self).__name__}({self.status}): " f"{self.error_title}>")
+            lines.append(f"<{type(self).__name__}({self.status}): {self.error_title}>")
         if self.extra_data:
             lines.append(" -> extra_data: " + repr(self.extra_data))
         return "\n".join(lines)
 
     def __reduce__(self):
         return (
             type(self),
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/groupconfig.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/groupconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/image.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,32 +122,38 @@
                     "name": "Import options",
                     "fields": [
                         {
                             "name": "src",
                             "type": "string",
                             "label": "Source Docker image",
                             "placeholder": "index.docker.io/lablup/tensorflow:2.0-source",
-                            "help": "The full Docker image name to import from. "
-                            "The registry must be accessible by the client.",
+                            "help": (
+                                "The full Docker image name to import from. "
+                                "The registry must be accessible by the client."
+                            ),
                         },
                         {
                             "name": "target",
                             "type": "string",
                             "label": "Target Docker image",
                             "placeholder": "index.docker.io/lablup/tensorflow:2.0-target",
-                            "help": "The full Docker image name of the imported image."
-                            "The registry must be accessible by the client.",
+                            "help": (
+                                "The full Docker image name of the imported image."
+                                "The registry must be accessible by the client."
+                            ),
                         },
                         {
                             "name": "brand",
                             "type": "string",
                             "label": "Name of Jupyter kernel",
                             "placeholder": "TensorFlow 2.0",
-                            "help": "The name of kernel to be shown in the Jupyter's kernel menu. "
-                            'This will be suffixed with "on Backend.AI".',
+                            "help": (
+                                "The name of kernel to be shown in the Jupyter's kernel menu. "
+                                'This will be suffixed with "on Backend.AI".'
+                            ),
                         },
                         {
                             "name": "baseDistro",
                             "type": "choice",
                             "choices": ["ubuntu", "centos"],
                             "default": "ubuntu",
                             "label": "Base LINUX distribution",
@@ -187,58 +193,65 @@
                         },
                         {
                             "name": "runtimeType",
                             "type": "choice",
                             "choices": ["python"],
                             "default": "python",
                             "label": "Runtime type of the image",
-                            "help": "The runtime type of the image. "
-                            "Currently, the source image must have installed Python 2.7, 3.5, 3.6, "
-                            "or 3.7 at least to import. "
-                            "This will be used as the kernel of Jupyter service in this image.",
+                            "help": (
+                                "The runtime type of the image. Currently, the source image must"
+                                " have installed Python 2.7, 3.5, 3.6, or 3.7 at least to import."
+                                " This will be used as the kernel of Jupyter service in this image."
+                            ),
                         },
                         {
                             "name": "runtimePath",
                             "type": "string",
                             "default": "/usr/local/bin/python",
                             "label": "Path of the runtime",
                             "placeholder": "/usr/local/bin/python",
-                            "help": "The path to the main executalbe of runtime language of the image. "
-                            'Even for the same "python"-based images, this may differ significantly '
-                            "image by image. (e.g., /usr/bin/python, /usr/local/bin/python, "
-                            "/opt/something/bin/python, ...) "
-                            "Please check this carefully not to get confused with OS-default ones "
-                            "and custom-installed ones.",
+                            "help": (
+                                "The path to the main executalbe of runtime language of the image."
+                                ' Even for the same "python"-based images, this may differ'
+                                " significantly image by image. (e.g., /usr/bin/python,"
+                                " /usr/local/bin/python, /opt/something/bin/python, ...) Please"
+                                " check this carefully not to get confused with OS-default ones and"
+                                " custom-installed ones."
+                            ),
                         },
                         {
                             "name": "CPUCountEnvs",
                             "type": "list[string]",
                             "default": ["NPROC", "OMP_NUM_THREADS", "OPENBLAS_NUM_THREADS"],
                             "label": "CPU count environment variables",
-                            "help": "The name of environment variables to be overriden to the number of CPU "
-                            "cores actually allocated to the container. Required for legacy "
-                            "computation libraries.",
+                            "help": (
+                                "The name of environment variables to be overriden to the number of"
+                                " CPU cores actually allocated to the container. Required for"
+                                " legacy computation libraries."
+                            ),
                         },
                         {
                             "name": "servicePorts",
                             "type": "multichoice[template]",
                             "templates": [
                                 {"name": "jupyter", "protocol": "http", "ports": [8080]},
                                 {"name": "jupyterlab", "protocol": "http", "ports": [8090]},
                                 {"name": "tensorboard", "protocol": "http", "ports": [6006]},
                                 {"name": "digits", "protocol": "http", "ports": [5000]},
                                 {"name": "vscode", "protocol": "http", "ports": [8180]},
                                 {"name": "h2o-dai", "protocol": "http", "ports": [12345]},
                             ],
                             "label": "Supported service ports",
-                            "help": "The list of service ports supported by this image. "
-                            "Note that sshd (port 2200) and ttyd (port 7681) are intrinsic; "
-                            "they are always included regardless of the source image. "
-                            "The port number 2000-2003 are reserved by Backend.AI, and "
-                            "all port numbers must be larger than 1024 and smaller than 65535.",
+                            "help": (
+                                "The list of service ports supported by this image. "
+                                "Note that sshd (port 2200) and ttyd (port 7681) are intrinsic; "
+                                "they are always included regardless of the source image. "
+                                "The port number 2000-2003 are reserved by Backend.AI, and "
+                                "all port numbers must be larger than 1024 and smaller than 65535."
+                            ),
                         },
                     ],
                 },
                 {
                     "name": "Import Task Options",
                     "help": "The import task uses 1 CPU core and 2 GiB of memory.",
                     "fields": [
@@ -250,15 +263,17 @@
                             "help": "The user group where the import task will be executed.",
                         },
                         {
                             "name": "scalingGroup",
                             "type": "choice",
                             "choices": accessible_scaling_groups,
                             "label": "Scaling group to build image",
-                            "help": "The scaling group where the import task will take resources from.",
+                            "help": (
+                                "The scaling group where the import task will take resources from."
+                            ),
                         },
                     ],
                 },
             ],
         }
     )
 
@@ -346,15 +361,17 @@
             "service_ports": params["servicePorts"],
             "min_cpu": params["minCPU"],
             "min_mem": params["minMemory"],
             "pref_shmem": params["preferredSharedMemory"],
             "accelerators": params["supportedAccelerators"],
             "src": params["src"],
             "brand": params["brand"],
-            "has_ipykernel": True,  # TODO: in the future, we may allow import of service-port only kernels.
+            "has_ipykernel": (
+                True
+            ),  # TODO: in the future, we may allow import of service-port only kernels.
         }
     )
 
     session_creation_id = secrets.token_urlsafe(32)
     session_id = f"image-import-{secrets.token_urlsafe(8)}"
     access_key = request["keypair"]["access_key"]
     resource_policy = request["keypair"]["resource_policy"]
@@ -416,16 +433,16 @@
         {
             "creation_config": {
                 "scaling_group": params["launchOptions"]["scalingGroup"],
                 "environ": {
                     "SRC_IMAGE": source_image.canonical,
                     "TARGET_IMAGE": target_image.canonical,
                     "RUNTIME_PATH": params["runtimePath"],
-                    "BUILD_SCRIPT": (
-                        base64.b64encode(dockerfile_content.encode("utf8")).decode("ascii")
+                    "BUILD_SCRIPT": base64.b64encode(dockerfile_content.encode("utf8")).decode(
+                        "ascii"
                     ),
                 },
             },
             "kernel_configs": [
                 {
                     "image_ref": importer_image,
                     "cluster_role": DEFAULT_ROLE,
@@ -435,17 +452,17 @@
                     "creation_config": {
                         "resources": {"cpu": "1", "mem": "2g"},
                         "scaling_group": params["launchOptions"]["scalingGroup"],
                         "environ": {
                             "SRC_IMAGE": source_image.canonical,
                             "TARGET_IMAGE": target_image.canonical,
                             "RUNTIME_PATH": params["runtimePath"],
-                            "BUILD_SCRIPT": (
-                                base64.b64encode(dockerfile_content.encode("utf8")).decode("ascii")
-                            ),
+                            "BUILD_SCRIPT": base64.b64encode(
+                                dockerfile_content.encode("utf8")
+                            ).decode("ascii"),
                         },
                     },
                     "startup_command": "/root/build-image.sh",
                     "bootstrap_script": "",
                 },
             ],
         },
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/logs.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,16 +220,18 @@
     if raw_lifetime is None:
         raw_lifetime = "90d"
     try:
         lifetime = tx.TimeDuration().check(raw_lifetime)
     except ValueError:
         lifetime = dt.timedelta(days=90)
         log.warning(
-            "Failed to parse the error log retention period ({}) read from etcd; "
-            "falling back to 90 days",
+            (
+                "Failed to parse the error log retention period ({}) read from etcd; "
+                "falling back to 90 days"
+            ),
             raw_lifetime,
         )
     boundary = datetime.now() - lifetime
     async with root_ctx.db.begin() as conn:
         query = sa.delete(error_logs).where(error_logs.c.created_at < boundary)
         result = await conn.execute(query)
         if result.rowcount > 0:
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/manager.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/ratelimit.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/ratelimit.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/resource.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import copy
 import functools
 import json
 import logging
 import re
 from datetime import datetime, timedelta
 from decimal import Decimal
-from typing import TYPE_CHECKING, Any, Iterable, MutableMapping, Tuple
+from typing import TYPE_CHECKING, Any, Iterable, Mapping, MutableMapping, Tuple
 
 import aiohttp
 import aiohttp_cors
 import msgpack
 import sqlalchemy as sa
 import trafaret as t
 import yarl
@@ -72,15 +72,15 @@
     async with root_ctx.db.begin_readonly() as conn:
         query = sa.select([resource_presets]).select_from(resource_presets)
         # TODO: uncomment when we implement scaling group.
         # scaling_group = request.query.get('scaling_group')
         # if scaling_group is not None:
         #     query = query.where(resource_presets.c.scaling_group == scaling_group)
         resp: MutableMapping[str, Any] = {"presets": []}
-        async for row in (await conn.stream(query)):
+        async for row in await conn.stream(query):
             preset_slots = row["resource_slots"].normalize_slots(ignore_unknown=True)
             resp["presets"].append(
                 {
                     "name": row["name"],
                     "shared_memory": str(row["shared_memory"]) if row["shared_memory"] else None,
                     "resource_slots": preset_slots.to_json(),
                 }
@@ -213,28 +213,28 @@
             .select_from(j)
             .where(
                 (KernelRow.user_uuid == request["user"]["uuid"])
                 & (KernelRow.status.in_(AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES))
                 & (SessionRow.scaling_group_name.in_(sgroup_names)),
             )
         )
-        async for row in (await conn.stream(query)):
+        async for row in await conn.stream(query):
             per_sgroup[row["scaling_group_name"]]["using"] += row["occupied_slots"]
 
         # Per scaling group resource remaining from agents stats.
         sgroup_remaining = ResourceSlot({k: Decimal(0) for k in known_slot_types.keys()})
         query = (
             sa.select([agents.c.available_slots, agents.c.occupied_slots, agents.c.scaling_group])
             .select_from(agents)
             .where(
                 (agents.c.status == AgentStatus.ALIVE) & (agents.c.scaling_group.in_(sgroup_names)),
             )
         )
         agent_slots = []
-        async for row in (await conn.stream(query)):
+        async for row in await conn.stream(query):
             remaining = row["available_slots"] - row["occupied_slots"]
             remaining += ResourceSlot({k: Decimal(0) for k in known_slot_types.keys()})
             sgroup_remaining += remaining
             agent_slots.append(remaining)
             per_sgroup[row["scaling_group"]]["remaining"] += remaining
 
         # Take maximum allocatable resources per sgroup.
@@ -246,29 +246,29 @@
                             slots[slot] = min(keypair_remaining[slot], slots[slot])
                 per_sgroup[sgname][rtype] = slots.to_json()  # type: ignore  # it's serialization
         for slot in known_slot_types.keys():
             sgroup_remaining[slot] = min(keypair_remaining[slot], sgroup_remaining[slot])
 
         # Fetch all resource presets in the current scaling group.
         query = sa.select([resource_presets]).select_from(resource_presets)
-        async for row in (await conn.stream(query)):
+        async for row in await conn.stream(query):
             # Check if there are any agent that can allocate each preset.
             allocatable = False
             preset_slots = row["resource_slots"].normalize_slots(ignore_unknown=True)
             for agent_slot in agent_slots:
                 if agent_slot >= preset_slots and keypair_remaining >= preset_slots:
                     allocatable = True
                     break
             resp["presets"].append(
                 {
                     "name": row["name"],
                     "resource_slots": preset_slots.to_json(),
-                    "shared_memory": str(row["shared_memory"])
-                    if row["shared_memory"] is not None
-                    else None,
+                    "shared_memory": (
+                        str(row["shared_memory"]) if row["shared_memory"] is not None else None
+                    ),
                     "allocatable": allocatable,
                 }
             )
 
         # Return group resource status as NaN if not allowed.
         group_resource_visibility = await root_ctx.shared_config.get_raw(
             "config/api/resources/group_resource_visibility"
@@ -327,14 +327,15 @@
                     kernels.c.attached_devices,
                     kernels.c.occupied_slots,
                     kernels.c.resource_opts,
                     kernels.c.vfolder_mounts,
                     kernels.c.mounts,
                     kernels.c.image,
                     kernels.c.status,
+                    kernels.c.status_info,
                     kernels.c.status_changed,
                     kernels.c.last_stat,
                     kernels.c.status_history,
                     kernels.c.created_at,
                     kernels.c.terminated_at,
                     kernels.c.cluster_mode,
                     groups.c.name,
@@ -424,29 +425,30 @@
             "agent": row["agent"],
             "cpu_allocated": float(row.occupied_slots.get("cpu", 0)),
             "cpu_used": float(nmget(last_stat, "cpu_used.current", 0)),
             "mem_allocated": int(row.occupied_slots.get("mem", 0)),
             "mem_used": int(nmget(last_stat, "mem.capacity", 0)),
             "shared_memory": int(nmget(row.resource_opts, "shmem", 0)),
             "disk_allocated": 0,  # TODO: disk quota limit
-            "disk_used": (int(nmget(last_stat, "io_scratch_size/stats.max", 0, "/"))),
+            "disk_used": int(nmget(last_stat, "io_scratch_size/stats.max", 0, "/")),
             "io_read": int(nmget(last_stat, "io_read.current", 0)),
             "io_write": int(nmget(last_stat, "io_write.current", 0)),
             "used_time": used_time,
             "used_days": used_days,
             "device_type": list(device_type),
             "smp": float(smp),
             "gpu_mem_allocated": float(gpu_mem_allocated),
             "gpu_allocated": float(gpu_allocated),  # devices or shares
             "nfs": nfs,
             "image_id": row["image"],  # TODO: image id
             "image_name": row["image"],
             "created_at": str(row["created_at"]),
             "terminated_at": str(row["terminated_at"]),
             "status": row["status"].name,
+            "status_info": row["status_info"],
             "status_changed": str(row["status_changed"]),
             "status_history": row["status_history"] or {},
             "cluster_mode": row["cluster_mode"],
         }
         if group_id not in objs_per_group:
             objs_per_group[group_id] = {
                 "domain_name": row["domain_name"],
@@ -578,103 +580,122 @@
             [1562084708.657106, 2, 4.0, 1073741824, ...],
         ]
 
     Note that the timestamp is in UNIX-timestamp.
     """
     # Get all or user kernels for the last month from DB.
     time_window = 900  # 15 min
+    stat_length = 2880  # 15 * 4 * 24 * 30
     now = datetime.now(tzutc())
     start_date = now - timedelta(days=30)
     root_ctx: RootContext = request.app["_root.context"]
     async with root_ctx.db.begin_readonly() as conn:
         query = (
-            sa.select([kernels])
+            sa.select(
+                [
+                    kernels.c.id,
+                    kernels.c.created_at,
+                    kernels.c.terminated_at,
+                    kernels.c.occupied_slots,
+                ]
+            )
             .select_from(kernels)
             .where(
                 (kernels.c.terminated_at >= start_date)
                 & (kernels.c.status.in_(RESOURCE_USAGE_KERNEL_STATUSES)),
             )
             .order_by(sa.asc(kernels.c.created_at))
         )
         if user_uuid is not None:
             query = query.where(kernels.c.user_uuid == user_uuid)
         result = await conn.execute(query)
         rows = result.fetchall()
 
     # Build time-series of time-binned stats.
-    now_ts = now.timestamp()
     start_date_ts = start_date.timestamp()
-    ts = start_date_ts
-    tseries = []
-    # Iterate over each time window.
-    while ts < now_ts:
-        # Initialize the time-binned stats.
-        num_sessions = 0
-        cpu_allocated = 0
-        mem_allocated = 0
-        gpu_allocated = Decimal(0)
-        io_read_bytes = 0
-        io_write_bytes = 0
-        disk_used = 0
-        # Accumulate stats for containers overlapping with this time window.
-        for row in rows:
-            if (
-                ts + time_window <= row.created_at.timestamp()
-                or ts >= row.terminated_at.timestamp()
-            ):
-                continue
-            num_sessions += 1
-            cpu_allocated += int(row.occupied_slots.get("cpu", 0))
-            mem_allocated += int(row.occupied_slots.get("mem", 0))
-            if "cuda.devices" in row.occupied_slots:
-                gpu_allocated += int(row.occupied_slots["cuda.devices"])
-            if "cuda.shares" in row.occupied_slots:
-                gpu_allocated += Decimal(row.occupied_slots["cuda.shares"])
-            raw_stat = await redis_helper.execute(
-                root_ctx.redis_stat, lambda r: r.get(str(row["id"]))
-            )
-            if raw_stat:
-                last_stat = msgpack.unpackb(raw_stat)
-                io_read_bytes += int(nmget(last_stat, "io_read.current", 0))
-                io_write_bytes += int(nmget(last_stat, "io_write.current", 0))
-                disk_used += int(nmget(last_stat, "io_scratch_size/stats.max", 0, "/"))
-        stat = {
-            "date": ts,
+    time_series_list: list[dict[str, Any]] = [
+        {
+            "date": start_date_ts + (idx * time_window),
             "num_sessions": {
-                "value": num_sessions,
+                "value": 0,
                 "unit_hint": "count",
             },
             "cpu_allocated": {
-                "value": cpu_allocated,
+                "value": 0,
                 "unit_hint": "count",
             },
             "mem_allocated": {
-                "value": mem_allocated,
+                "value": 0,
                 "unit_hint": "bytes",
             },
             "gpu_allocated": {
-                "value": float(gpu_allocated),
+                "value": 0,
                 "unit_hint": "count",
             },
             "io_read_bytes": {
-                "value": io_read_bytes,
+                "value": 0,
                 "unit_hint": "bytes",
             },
             "io_write_bytes": {
-                "value": io_write_bytes,
+                "value": 0,
                 "unit_hint": "bytes",
             },
             "disk_used": {
-                "value ": disk_used,
+                "value": 0,
                 "unit_hint": "bytes",
             },
         }
-        tseries.append(stat)
-        ts += time_window
-    return tseries
+        for idx in range(stat_length)
+    ]
+
+    async def _pipe_builder(r: Redis) -> RedisPipeline:
+        pipe = r.pipeline()
+        for row in rows:
+            await pipe.get(str(row["id"]))
+        return pipe
+
+    raw_stats = await redis_helper.execute(root_ctx.redis_stat, _pipe_builder)
+
+    for row, raw_stat in zip(rows, raw_stats):
+        if raw_stat is not None:
+            last_stat = msgpack.unpackb(raw_stat)
+            io_read_byte = int(nmget(last_stat, "io_read.current", 0))
+            io_write_byte = int(nmget(last_stat, "io_write.current", 0))
+            disk_used = int(nmget(last_stat, "io_scratch_size.stats.max", 0, "/"))
+        else:
+            io_read_byte = 0
+            io_write_byte = 0
+            disk_used = 0
+
+        occupied_slots: Mapping[str, Any] = row.occupied_slots
+        kernel_created_at: float = row.created_at.timestamp()
+        kernel_terminated_at: float = row.terminated_at.timestamp()
+        cpu_value = int(occupied_slots.get("cpu", 0))
+        mem_value = int(occupied_slots.get("mem", 0))
+        cuda_device_value = int(occupied_slots.get("cuda.devices", 0))
+        cuda_share_value = Decimal(occupied_slots.get("cuda.shares", 0))
+
+        start_index = int((kernel_created_at - start_date_ts) // time_window)
+        end_index = int((kernel_terminated_at - start_date_ts) // time_window) + 1
+        if start_index < 0:
+            start_index = 0
+        for time_series in time_series_list[start_index:end_index]:
+            time_series["num_sessions"]["value"] += 1
+            time_series["cpu_allocated"]["value"] += cpu_value
+            time_series["mem_allocated"]["value"] += mem_value
+            time_series["gpu_allocated"]["value"] += cuda_device_value
+            time_series["gpu_allocated"]["value"] += cuda_share_value
+            time_series["io_read_bytes"]["value"] += io_read_byte
+            time_series["io_write_bytes"]["value"] += io_write_byte
+            time_series["disk_used"]["value"] += disk_used
+
+    # Change Decimal type to float to serialize to JSON
+    for time_series in time_series_list:
+        time_series["gpu_allocated"]["value"] = float(time_series["gpu_allocated"]["value"])
+    return time_series_list
 
 
 @server_status_required(READ_ALLOWED)
 @auth_required
 async def user_month_stats(request: web.Request) -> web.Response:
     """
     Return time-binned (15 min) stats for terminated user sessions
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/scaling_group.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/scaling_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,34 +48,37 @@
         }
     ),
 )
 async def list_available_sgroups(request: web.Request, params: Any) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
     domain_name = request["user"]["domain_name"]
+    is_admin = request["is_admin"]
     group_id_or_name = params["group"]
     log.info("SGROUPS.LIST(ak:{}, g:{}, d:{})", access_key, group_id_or_name, domain_name)
     async with root_ctx.db.begin() as conn:
         sgroups = await query_allowed_sgroups(conn, domain_name, group_id_or_name, access_key)
+        if not is_admin:
+            sgroups = [sgroup for sgroup in sgroups if sgroup["is_public"]]
         return web.json_response(
             {
                 "scaling_groups": [{"name": sgroup["name"]} for sgroup in sgroups],
             },
             status=200,
         )
 
 
 @auth_required
 @server_status_required(READ_ALLOWED)
 @check_api_params(
     t.Dict(
         {
-            tx.AliasedKey(["group", "group_id", "group_name"], default=None): t.Null
-            | tx.UUID
-            | t.String,
+            tx.AliasedKey(["group", "group_id", "group_name"], default=None): (
+                t.Null | tx.UUID | t.String
+            ),
         }
     )
 )
 async def get_wsproxy_version(request: web.Request, params: Any) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
     scaling_group_name = request.match_info["scaling_group"]
     access_key = request["keypair"]["access_key"]
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/service.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/session.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,25 +47,24 @@
 from dateutil.tz import tzutc
 from redis.asyncio import Redis
 from sqlalchemy.sql.expression import null, true
 
 from ai.backend.manager.models.image import ImageRow
 
 if TYPE_CHECKING:
-    from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
+    from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection, AsyncSession as SASession
 
 from ai.backend.common import redis_helper
 from ai.backend.common import validators as tx
 from ai.backend.common.docker import ImageRef
 from ai.backend.common.events import (
     AgentHeartbeatEvent,
     AgentStartedEvent,
     AgentTerminatedEvent,
     DoSyncKernelLogsEvent,
-    DoSyncKernelStatsEvent,
     DoTerminateSessionEvent,
     KernelCancelledEvent,
     KernelCreatingEvent,
     KernelLifecycleEventReason,
     KernelPreparingEvent,
     KernelPullingEvent,
     KernelStartedEvent,
@@ -79,32 +78,37 @@
     SessionStartedEvent,
     SessionSuccessEvent,
     SessionTerminatedEvent,
     SessionTerminatingEvent,
 )
 from ai.backend.common.exception import AliasResolutionFailed, UnknownImageReference
 from ai.backend.common.logging import BraceStyleAdapter
+from ai.backend.common.plugin.hook import HookResults
 from ai.backend.common.plugin.monitor import GAUGE
 from ai.backend.common.types import (
     AccessKey,
     AgentId,
     ClusterMode,
+    EtcdRedisConfig,
     KernelEnqueueingConfig,
     KernelId,
     SessionTypes,
     check_typed_dict,
 )
 from ai.backend.common.utils import cancel_tasks, str_to_timedelta
+from ai.backend.manager.defs import PluginDatabaseID
 
 from ..config import DEFAULT_CHUNK_SIZE
 from ..defs import DEFAULT_IMAGE_ARCH, DEFAULT_ROLE, REDIS_STREAM_DB
 from ..models import (
     AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES,
     DEAD_SESSION_STATUSES,
+    PRIVATE_KERNEL_ROLES,
     AgentStatus,
+    KernelRole,
     KernelRow,
     KernelStatus,
     RoutingRow,
     SessionRow,
     SessionStatus,
     UserRole,
 )
@@ -119,25 +123,28 @@
     query_bootstrap_script,
     scaling_groups,
     session_templates,
     users,
     verify_vfolder_name,
     vfolders,
 )
+from ..models.session import SessionDependencyRow
 from ..models.utils import execute_with_retry
 from ..types import UserScope
 from .auth import auth_required
 from .exceptions import (
     AppNotFound,
     BackendError,
+    GenericForbidden,
     ImageNotFound,
     InsufficientPrivilege,
     InternalServerError,
     InvalidAPIParameters,
     ObjectNotFound,
+    RejectedByHook,
     ServiceUnavailable,
     SessionAlreadyExists,
     SessionNotFound,
     StorageProxyError,
     TaskTemplateNotFound,
     TooManySessionsMatched,
     UnknownImageReferenceError,
@@ -185,99 +192,106 @@
 creation_config_v3 = t.Dict(
     {
         t.Key("mounts", default=None): t.Null | t.List(t.String),
         t.Key("environ", default=None): t.Null | t.Mapping(t.String, t.String),
         tx.AliasedKey(["cluster_size", "clusterSize"], default=None): t.Null | t.Int[1:],
         tx.AliasedKey(["scaling_group", "scalingGroup"], default=None): t.Null | t.String,
         t.Key("resources", default=None): t.Null | t.Mapping(t.String, t.Any),
-        tx.AliasedKey(["resource_opts", "resourceOpts"], default=None): t.Null
-        | t.Mapping(t.String, t.Any),
+        tx.AliasedKey(["resource_opts", "resourceOpts"], default=None): t.Null | t.Mapping(
+            t.String, t.Any
+        ),
     }
 )
 creation_config_v3_template = t.Dict(
     {
         t.Key("mounts", default=undefined): UndefChecker | t.Null | t.List(t.String),
         t.Key("environ", default=undefined): UndefChecker | t.Null | t.Mapping(t.String, t.String),
-        tx.AliasedKey(["cluster_size", "clusterSize"], default=undefined): UndefChecker
-        | t.Null
-        | t.Int[1:],
-        tx.AliasedKey(["scaling_group", "scalingGroup"], default=undefined): UndefChecker
-        | t.Null
-        | t.String,
+        tx.AliasedKey(["cluster_size", "clusterSize"], default=undefined): (
+            UndefChecker | t.Null | t.Int[1:]
+        ),
+        tx.AliasedKey(["scaling_group", "scalingGroup"], default=undefined): (
+            UndefChecker | t.Null | t.String
+        ),
         t.Key("resources", default=undefined): UndefChecker | t.Null | t.Mapping(t.String, t.Any),
-        tx.AliasedKey(["resource_opts", "resourceOpts"], default=undefined): UndefChecker
-        | t.Null
-        | t.Mapping(t.String, t.Any),
+        tx.AliasedKey(["resource_opts", "resourceOpts"], default=undefined): (
+            UndefChecker | t.Null | t.Mapping(t.String, t.Any)
+        ),
     }
 )
 creation_config_v4 = t.Dict(
     {
         t.Key("mounts", default=None): t.Null | t.List(t.String),
-        tx.AliasedKey(["mount_map", "mountMap"], default=None): t.Null
-        | t.Mapping(t.String, t.String),
+        tx.AliasedKey(["mount_map", "mountMap"], default=None): t.Null | t.Mapping(
+            t.String, t.String
+        ),
         t.Key("environ", default=None): t.Null | t.Mapping(t.String, t.String),
         tx.AliasedKey(["cluster_size", "clusterSize"], default=None): t.Null | t.Int[1:],
         tx.AliasedKey(["scaling_group", "scalingGroup"], default=None): t.Null | t.String,
         t.Key("resources", default=None): t.Null | t.Mapping(t.String, t.Any),
-        tx.AliasedKey(["resource_opts", "resourceOpts"], default=None): t.Null
-        | t.Mapping(t.String, t.Any),
-        tx.AliasedKey(["preopen_ports", "preopenPorts"], default=None): t.Null
-        | t.List(t.Int[1024:65535]),
+        tx.AliasedKey(["resource_opts", "resourceOpts"], default=None): t.Null | t.Mapping(
+            t.String, t.Any
+        ),
+        tx.AliasedKey(["preopen_ports", "preopenPorts"], default=None): t.Null | t.List(
+            t.Int[1024:65535]
+        ),
     }
 )
 creation_config_v4_template = t.Dict(
     {
         t.Key("mounts", default=undefined): UndefChecker | t.Null | t.List(t.String),
-        tx.AliasedKey(["mount_map", "mountMap"], default=undefined): UndefChecker
-        | t.Null
-        | t.Mapping(t.String, t.String),
+        tx.AliasedKey(["mount_map", "mountMap"], default=undefined): (
+            UndefChecker | t.Null | t.Mapping(t.String, t.String)
+        ),
         t.Key("environ", default=undefined): UndefChecker | t.Null | t.Mapping(t.String, t.String),
-        tx.AliasedKey(["cluster_size", "clusterSize"], default=undefined): UndefChecker
-        | t.Null
-        | t.Int[1:],
-        tx.AliasedKey(["scaling_group", "scalingGroup"], default=undefined): UndefChecker
-        | t.Null
-        | t.String,
+        tx.AliasedKey(["cluster_size", "clusterSize"], default=undefined): (
+            UndefChecker | t.Null | t.Int[1:]
+        ),
+        tx.AliasedKey(["scaling_group", "scalingGroup"], default=undefined): (
+            UndefChecker | t.Null | t.String
+        ),
         t.Key("resources", default=undefined): UndefChecker | t.Null | t.Mapping(t.String, t.Any),
-        tx.AliasedKey(["resource_opts", "resourceOpts"], default=undefined): UndefChecker
-        | t.Null
-        | t.Mapping(t.String, t.Any),
+        tx.AliasedKey(["resource_opts", "resourceOpts"], default=undefined): (
+            UndefChecker | t.Null | t.Mapping(t.String, t.Any)
+        ),
     }
 )
 creation_config_v5 = t.Dict(
     {
         t.Key("mounts", default=None): t.Null | t.List(t.String),
-        tx.AliasedKey(["mount_map", "mountMap"], default=None): t.Null
-        | t.Mapping(t.String, t.String),
+        tx.AliasedKey(["mount_map", "mountMap"], default=None): t.Null | t.Mapping(
+            t.String, t.String
+        ),
         t.Key("environ", default=None): t.Null | t.Mapping(t.String, t.String),
         # cluster_size is moved to the root-level parameters
         tx.AliasedKey(["scaling_group", "scalingGroup"], default=None): t.Null | t.String,
         t.Key("resources", default=None): t.Null | t.Mapping(t.String, t.Any),
-        tx.AliasedKey(["resource_opts", "resourceOpts"], default=None): t.Null
-        | t.Mapping(t.String, t.Any),
-        tx.AliasedKey(["preopen_ports", "preopenPorts"], default=None): t.Null
-        | t.List(t.Int[1024:65535]),
+        tx.AliasedKey(["resource_opts", "resourceOpts"], default=None): t.Null | t.Mapping(
+            t.String, t.Any
+        ),
+        tx.AliasedKey(["preopen_ports", "preopenPorts"], default=None): t.Null | t.List(
+            t.Int[1024:65535]
+        ),
         tx.AliasedKey(["agent_list", "agentList"], default=None): t.Null | t.List(t.String),
     }
 )
 creation_config_v5_template = t.Dict(
     {
         t.Key("mounts", default=undefined): UndefChecker | t.Null | t.List(t.String),
-        tx.AliasedKey(["mount_map", "mountMap"], default=undefined): UndefChecker
-        | t.Null
-        | t.Mapping(t.String, t.String),
+        tx.AliasedKey(["mount_map", "mountMap"], default=undefined): (
+            UndefChecker | t.Null | t.Mapping(t.String, t.String)
+        ),
         t.Key("environ", default=undefined): UndefChecker | t.Null | t.Mapping(t.String, t.String),
         # cluster_size is moved to the root-level parameters
-        tx.AliasedKey(["scaling_group", "scalingGroup"], default=undefined): UndefChecker
-        | t.Null
-        | t.String,
+        tx.AliasedKey(["scaling_group", "scalingGroup"], default=undefined): (
+            UndefChecker | t.Null | t.String
+        ),
         t.Key("resources", default=undefined): UndefChecker | t.Null | t.Mapping(t.String, t.Any),
-        tx.AliasedKey(["resource_opts", "resourceOpts"], default=undefined): UndefChecker
-        | t.Null
-        | t.Mapping(t.String, t.Any),
+        tx.AliasedKey(["resource_opts", "resourceOpts"], default=undefined): (
+            UndefChecker | t.Null | t.Mapping(t.String, t.Any)
+        ),
     }
 )
 
 
 overwritten_param_check = t.Dict(
     {
         t.Key("template_id"): tx.UUID,
@@ -568,14 +582,17 @@
         owner_uuid, group_id, resource_policy = await query_userinfo(request, params, conn)
 
         # Use keypair bootstrap_script if it is not delivered as a parameter
         if not params["bootstrap_script"]:
             script, _ = await query_bootstrap_script(conn, owner_access_key)
             params["bootstrap_script"] = script
 
+    public_sgroup_only = True
+    if _role_str := image_row.labels.get("ai.backend.role"):
+        public_sgroup_only = KernelRole(_role_str) not in PRIVATE_KERNEL_ROLES
     try:
         session_id = await asyncio.shield(
             app_ctx.database_ptask_group.create_task(
                 root_ctx.registry.enqueue_session(
                     session_creation_id,
                     params["session_name"],
                     owner_access_key,
@@ -606,14 +623,15 @@
                     cluster_mode=params["cluster_mode"],
                     cluster_size=params["cluster_size"],
                     session_tag=params["tag"],
                     starts_at=starts_at,
                     agent_list=params["config"]["agent_list"],
                     dependency_sessions=params["dependencies"],
                     callback_url=params["callback_url"],
+                    public_sgroup_only=public_sgroup_only,
                 )
             ),
         )
         resp["sessionId"] = str(session_id)  # changed since API v5
         resp["sessionName"] = str(params["session_name"])
         resp["status"] = "PENDING"
         resp["servicePorts"] = []
@@ -676,52 +694,47 @@
 @server_status_required(ALL_ALLOWED)
 @auth_required
 @check_api_params(
     t.Dict(
         {
             tx.AliasedKey(["template_id", "templateId"]): t.Null | tx.UUID,
             tx.AliasedKey(["name", "clientSessionToken"], default=undefined)
-            >> "session_name": UndefChecker
-            | t.Regexp(r"^(?=.{4,64}$)\w[\w.-]*\w$", re.ASCII),
+            >> "session_name": UndefChecker | t.Regexp(r"^(?=.{4,64}$)\w[\w.-]*\w$", re.ASCII),
             tx.AliasedKey(["image", "lang"], default=undefined): UndefChecker | t.Null | t.String,
             tx.AliasedKey(["arch", "architecture"], default=DEFAULT_IMAGE_ARCH)
             >> "architecture": t.String,
             tx.AliasedKey(["type", "sessionType"], default="interactive")
             >> "session_type": tx.Enum(SessionTypes),
-            tx.AliasedKey(["group", "groupName", "group_name"], default=undefined): UndefChecker
-            | t.Null
-            | t.String,
-            tx.AliasedKey(["domain", "domainName", "domain_name"], default=undefined): UndefChecker
-            | t.Null
-            | t.String,
+            tx.AliasedKey(["group", "groupName", "group_name"], default=undefined): (
+                UndefChecker | t.Null | t.String
+            ),
+            tx.AliasedKey(["domain", "domainName", "domain_name"], default=undefined): (
+                UndefChecker | t.Null | t.String
+            ),
             tx.AliasedKey(["cluster_size", "clusterSize"], default=1): t.ToInt[1:],  # new in APIv6
             tx.AliasedKey(["cluster_mode", "clusterMode"], default="single-node"): tx.Enum(
                 ClusterMode
             ),  # new in APIv6
             t.Key("config", default=dict): t.Mapping(t.String, t.Any),
             t.Key("tag", default=undefined): UndefChecker | t.Null | t.String,
             t.Key("enqueueOnly", default=False) >> "enqueue_only": t.ToBool,
             t.Key("maxWaitSeconds", default=0) >> "max_wait_seconds": t.Int[0:],
             tx.AliasedKey(["starts_at", "startsAt"], default=None): t.Null | t.String,
             t.Key("reuseIfExists", default=True) >> "reuse": t.ToBool,
-            t.Key("startupCommand", default=None) >> "startup_command": UndefChecker
-            | t.Null
-            | t.String,
-            tx.AliasedKey(["bootstrap_script", "bootstrapScript"], default=undefined): UndefChecker
-            | t.Null
-            | t.String,
-            t.Key("dependencies", default=None): UndefChecker
-            | t.Null
-            | t.List(tx.UUID)
-            | t.List(t.String),
-            tx.AliasedKey(
-                ["callback_url", "callbackUrl", "callbackURL"], default=None
-            ): UndefChecker
-            | t.Null
-            | tx.URL,
+            t.Key("startupCommand", default=None)
+            >> "startup_command": UndefChecker | t.Null | t.String,
+            tx.AliasedKey(["bootstrap_script", "bootstrapScript"], default=undefined): (
+                UndefChecker | t.Null | t.String
+            ),
+            t.Key("dependencies", default=None): (
+                UndefChecker | t.Null | t.List(tx.UUID) | t.List(t.String)
+            ),
+            tx.AliasedKey(["callback_url", "callbackUrl", "callbackURL"], default=None): (
+                UndefChecker | t.Null | tx.URL
+            ),
             t.Key("owner_access_key", default=undefined): UndefChecker | t.Null | t.String,
         },
     ),
     loads=_json_loads,
 )
 async def create_from_template(request: web.Request, params: dict[str, Any]) -> web.Response:
     # TODO: we need to refactor session_template model to load the template configs
@@ -888,16 +901,17 @@
             t.Key("enqueueOnly", default=False) >> "enqueue_only": t.ToBool,
             t.Key("maxWaitSeconds", default=0) >> "max_wait_seconds": t.ToInt[0:],
             tx.AliasedKey(["starts_at", "startsAt"], default=None): t.Null | t.String,
             t.Key("reuseIfExists", default=True) >> "reuse": t.ToBool,
             t.Key("startupCommand", default=None) >> "startup_command": t.Null | t.String,
             tx.AliasedKey(["bootstrap_script", "bootstrapScript"], default=None): t.Null | t.String,
             t.Key("dependencies", default=None): t.Null | t.List(tx.UUID) | t.List(t.String),
-            tx.AliasedKey(["callback_url", "callbackUrl", "callbackURL"], default=None): t.Null
-            | tx.URL,
+            tx.AliasedKey(["callback_url", "callbackUrl", "callbackURL"], default=None): (
+                t.Null | tx.URL
+            ),
             t.Key("owner_access_key", default=None): t.Null | t.String,
         }
     ),
     loads=_json_loads,
 )
 async def create_from_params(request: web.Request, params: dict[str, Any]) -> web.Response:
     if params["session_name"] in ["from-template"]:
@@ -928,23 +942,27 @@
         if not params["config"]["agent_list"]:
             pass
         else:
             agent_count = len(params["config"]["agent_list"])
             if params["cluster_mode"] == "multi-node":
                 if agent_count != params["cluster_size"]:
                     raise InvalidAPIParameters(
-                        "For multi-node cluster sessions, the number of manually assigned agents "
-                        "must be same to the clsuter size. "
-                        "Note that you may specify duplicate agents in the list.",
+                        (
+                            "For multi-node cluster sessions, the number of manually assigned"
+                            " agents must be same to the clsuter size. Note that you may specify"
+                            " duplicate agents in the list."
+                        ),
                     )
             else:
                 if agent_count != 1:
                     raise InvalidAPIParameters(
-                        "For non-cluster sessions and single-node cluster sessions, "
-                        "you may specify only one manually assigned agent.",
+                        (
+                            "For non-cluster sessions and single-node cluster sessions, "
+                            "you may specify only one manually assigned agent."
+                        ),
                     )
     return await _create(request, params)
 
 
 @server_status_required(ALL_ALLOWED)
 @auth_required
 @check_api_params(
@@ -1472,45 +1490,37 @@
 
     To avoid race condition between consumer and subscriber event handlers,
     we only have this handler to subscribe all kernel creation events,
     but distinguish which one to process using a unique creation_id
     generated when initiating the create_kernels() agent RPC call.
     """
     root_ctx: RootContext = app["_root.context"]
-    # ck_id = (event.creation_id, event.kernel_id)
-    ck_id = event.kernel_id
-    if ck_id in root_ctx.registry.kernel_creation_tracker:
-        log.debug(
-            "handle_kernel_creation_lifecycle: ev:{} k:{}",
-            event.name,
-            event.kernel_id,
-        )
+    log.debug(
+        "handle_kernel_creation_lifecycle: ev:{} k:{}",
+        event.name,
+        event.kernel_id,
+    )
     if isinstance(event, KernelPreparingEvent):
         # State transition is done by the DoPrepareEvent handler inside the scheduler-distpacher object.
         pass
     elif isinstance(event, KernelPullingEvent):
         await KernelRow.set_kernel_status(
             root_ctx.db, event.kernel_id, KernelStatus.PULLING, reason=event.reason
         )
     elif isinstance(event, KernelCreatingEvent):
         await KernelRow.set_kernel_status(
             root_ctx.db, event.kernel_id, KernelStatus.PREPARING, reason=event.reason
         )
     elif isinstance(event, KernelStartedEvent):
-        await root_ctx.registry.finalize_running(event.creation_info)
-        # post_create_kernel() coroutines are waiting for the creation tracker events to be set.
-        if (tracker := root_ctx.registry.kernel_creation_tracker.get(ck_id)) and not tracker.done():
-            tracker.set_result(None)
+        session_id = event.session_id
+        await root_ctx.registry.finalize_running(event.kernel_id, session_id, event.creation_info)
         if (endpoint_id := event.creation_info.get("endpoint_id")) is not None:
-            session_id = event.creation_info.get("session_id")
-            await RoutingRow.create(root_ctx.db, uuid.UUID(endpoint_id), uuid.UUID(session_id))
+            await RoutingRow.create(root_ctx.db, uuid.UUID(endpoint_id), uuid.UUID(str(session_id)))
     elif isinstance(event, KernelCancelledEvent):
-        if (tracker := root_ctx.registry.kernel_creation_tracker.get(ck_id)) and not tracker.done():
-            log.warning(f"Kernel cancelled, {event.reason = }")
-            tracker.cancel()
+        log.warning(f"Kernel cancelled, {event.reason = }")
 
 
 async def handle_kernel_termination_lifecycle(
     app: web.Application,
     source: AgentId,
     event: KernelTerminatingEvent | KernelTerminatedEvent,
 ) -> None:
@@ -1518,15 +1528,16 @@
     if isinstance(event, KernelTerminatingEvent):
         # The destroy_kernel() API handler will set the "TERMINATING" status.
         pass
     elif isinstance(event, KernelTerminatedEvent):
         await root_ctx.registry.mark_kernel_terminated(
             event.kernel_id, event.reason, event.exit_code
         )
-        await root_ctx.registry.check_session_terminated(event.kernel_id, event.reason)
+        session_id = event.session_id
+        await root_ctx.registry.check_session_terminated(session_id, event.reason)
 
 
 async def handle_session_creation_lifecycle(
     app: web.Application,
     source: AgentId,
     event: SessionStartedEvent | SessionCancelledEvent,
 ) -> None:
@@ -1573,24 +1584,14 @@
     await root_ctx.registry.destroy_session(
         session,
         forced=False,
         reason=event.reason or KernelLifecycleEventReason.KILLED_BY_EVENT,
     )
 
 
-async def handle_kernel_stat_sync(
-    app: web.Application,
-    agent_id: AgentId,
-    event: DoSyncKernelStatsEvent,
-) -> None:
-    root_ctx: RootContext = app["_root.context"]
-    if root_ctx.local_config["debug"]["periodic-sync-stats"]:
-        await root_ctx.registry.sync_kernel_stats(event.kernel_ids)
-
-
 async def _make_session_callback(data: dict[str, Any], url: yarl.URL) -> None:
     log_func = log.info
     log_msg: str = ""
     log_fmt: str = ""
     log_arg: Any = None
     begin = time.monotonic()
     try:
@@ -1639,35 +1640,47 @@
     | SessionStartedEvent
     | SessionCancelledEvent
     | SessionTerminatingEvent
     | SessionTerminatedEvent
     | SessionSuccessEvent
     | SessionFailureEvent,
 ) -> None:
-    app_ctx: PrivateContext = app["session.context"]
+    log.info("INVOKE_SESSION_CALLBACK (source:{}, event:{})", source, event)
     root_ctx: RootContext = app["_root.context"]
-    data = {
-        "type": "session_lifecycle",
-        "event": event.name.removeprefix("session_"),
-        "session_id": str(event.session_id),
-        "when": datetime.now(tzutc()).isoformat(),
-    }
     try:
+        allow_stale = isinstance(event, (SessionCancelledEvent, SessionTerminatedEvent))
         async with root_ctx.db.begin_readonly_session() as db_sess:
             session = await SessionRow.get_session_with_main_kernel(
-                event.session_id, db_session=db_sess
+                event.session_id, db_session=db_sess, allow_stale=allow_stale
             )
     except SessionNotFound:
         return
     url = session.callback_url
     if url is None:
         return
-    app_ctx.webhook_ptask_group.create_task(
-        _make_session_callback(data, url),
-    )
+    if (addr := root_ctx.local_config.get("pipeline", {}).get("event-queue")) is None:
+        return
+    etcd_redis_config: EtcdRedisConfig = {
+        "addr": addr,
+        "sentinel": None,
+        "service_name": None,
+        "password": None,
+    }
+    stream_key = "events"
+    token = url.query.get("token")
+
+    async def _dispatch() -> None:
+        hook_result = await root_ctx.hook_plugin_ctx.dispatch(
+            "PUBLISH_EVENT",
+            (event, etcd_redis_config, PluginDatabaseID.SESSION_EVENT, stream_key, token),
+        )
+        if hook_result.status != HookResults.PASSED:
+            raise RejectedByHook.from_hook_result(hook_result)
+
+    await execute_with_retry(_dispatch)
 
 
 async def handle_batch_result(
     app: web.Application,
     source: AgentId,
     event: SessionSuccessEvent | SessionFailureEvent,
 ) -> None:
@@ -1676,15 +1689,20 @@
     """
     root_ctx: RootContext = app["_root.context"]
     if isinstance(event, SessionSuccessEvent):
         await SessionRow.set_session_result(root_ctx.db, event.session_id, True, event.exit_code)
     elif isinstance(event, SessionFailureEvent):
         await SessionRow.set_session_result(root_ctx.db, event.session_id, False, event.exit_code)
     async with root_ctx.db.begin_session() as db_sess:
-        session = await SessionRow.get_session_with_kernels(event.session_id, db_session=db_sess)
+        try:
+            session = await SessionRow.get_session_with_kernels(
+                event.session_id, db_session=db_sess
+            )
+        except SessionNotFound:
+            return
     await root_ctx.registry.destroy_session(
         session,
         reason=KernelLifecycleEventReason.TASK_FINISHED,
     )
 
 
 async def handle_agent_lifecycle(
@@ -1891,14 +1909,15 @@
 
 @server_status_required(READ_ALLOWED)
 @auth_required
 @check_api_params(
     t.Dict(
         {
             t.Key("forced", default="false"): t.ToBool(),
+            t.Key("recursive", default="false"): t.ToBool(),
             t.Key("owner_access_key", default=None): t.Null | t.String,
         }
     )
 )
 async def destroy(request: web.Request, params: Any) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
     session_name = request.match_info["session_name"]
@@ -1909,32 +1928,69 @@
     ):
         raise InsufficientPrivilege("You are not allowed to force-terminate others's sessions")
     # domain_name = None
     # if requester_access_key != owner_access_key and \
     #         not request['is_superadmin'] and request['is_admin']:
     #     domain_name = request['user']['domain_name']
     log.info(
-        "DESTROY (ak:{0}/{1}, s:{2}, forced:{3})",
+        "DESTROY (ak:{0}/{1}, s:{2}, forced:{3}, recursive: {4})",
         requester_access_key,
         owner_access_key,
         session_name,
         params["forced"],
+        params["recursive"],
     )
-    async with root_ctx.db.begin_session() as db_sess:
-        session = await SessionRow.get_session_with_kernels(
-            session_name, owner_access_key, db_session=db_sess
+
+    requester_access_key, owner_access_key = await get_access_key_scopes(request, params)
+
+    if params["recursive"]:
+        async with root_ctx.db.begin_readonly_session() as db_sess:
+            dependent_session_ids = await find_dependent_sessions(
+                session_name, db_sess, owner_access_key
+            )
+
+            target_session_references: List[str | uuid.UUID] = [
+                *dependent_session_ids,
+                session_name,
+            ]
+            sessions = [
+                await SessionRow.get_session_with_kernels(
+                    name_or_id, owner_access_key, db_session=db_sess
+                )
+                for name_or_id in target_session_references
+            ]
+
+        last_stats = await asyncio.gather(
+            *[
+                root_ctx.registry.destroy_session(sess, forced=params["forced"])
+                for sess in sessions
+            ],
+            return_exceptions=True,
+        )
+
+        # Consider not found sessions already terminated.
+        # Consider GenericForbidden error occurs with scheduled/preparing/terminating/error status session, and leave them not to be quitted.
+        last_stats = [
+            *filter(lambda x: not isinstance(x, SessionNotFound | GenericForbidden), last_stats)
+        ]
+
+        return web.json_response(last_stats, status=200)
+    else:
+        async with root_ctx.db.begin_readonly_session() as db_sess:
+            session = await SessionRow.get_session_with_kernels(
+                session_name, owner_access_key, db_session=db_sess
+            )
+        last_stat = await root_ctx.registry.destroy_session(
+            session,
+            forced=params["forced"],
         )
-    last_stat = await root_ctx.registry.destroy_session(
-        session,
-        forced=params["forced"],
-    )
-    resp = {
-        "stats": last_stat,
-    }
-    return web.json_response(resp, status=200)
+        resp = {
+            "stats": last_stat,
+        }
+        return web.json_response(resp, status=200)
 
 
 @server_status_required(READ_ALLOWED)
 @auth_required
 @check_api_params(
     t.Dict(
         {
@@ -1977,14 +2033,43 @@
         },
         status=200,
     )
 
 
 @server_status_required(READ_ALLOWED)
 @auth_required
+async def get_direct_access_info(request: web.Request) -> web.Response:
+    root_ctx: RootContext = request.app["_root.context"]
+    session_name = request.match_info["session_name"]
+    _, owner_access_key = await get_access_key_scopes(request)
+
+    async with root_ctx.db.begin_session() as db_sess:
+        sess = await SessionRow.get_session_with_main_kernel(
+            session_name, owner_access_key, db_session=db_sess
+        )
+    kernel_role: KernelRole = sess.main_kernel.role
+    resp = {}
+    if kernel_role == KernelRole.SYSTEM:
+        public_host = sess.main_kernel.agent_row.public_host
+        found_ports: dict[str, list[str]] = {}
+        for sport in sess.main_kernel.service_ports:
+            if sport["name"] == "sshd":
+                found_ports["sshd"] = sport["host_ports"]
+            elif sport["name"] == "sftpd":
+                found_ports["sftpd"] = sport["host_ports"]
+        resp = {
+            "kernel_role": kernel_role.name,
+            "public_host": public_host,
+            "sshd_ports": found_ports.get("sftpd") or found_ports["sshd"],
+        }
+    return web.json_response(resp)
+
+
+@server_status_required(READ_ALLOWED)
+@auth_required
 async def get_info(request: web.Request) -> web.Response:
     # NOTE: This API should be replaced with GraphQL version.
     resp = {}
     root_ctx: RootContext = request.app["_root.context"]
     session_name = request.match_info["session_name"]
     requester_access_key, owner_access_key = await get_access_key_scopes(request)
     log.info("GET_INFO (ak:{0}/{1}, s:{2})", requester_access_key, owner_access_key, session_name)
@@ -2020,14 +2105,15 @@
         age = datetime.now(tzutc()) - sess.created_at
         resp["age"] = int(age.total_seconds() * 1000)  # age in milliseconds
         resp["creationTime"] = str(sess.created_at)
         resp["terminationTime"] = str(sess.terminated_at) if sess.terminated_at else None
 
         resp["numQueriesExecuted"] = sess.num_queries
         resp["lastStat"] = sess.last_stat
+        resp["idleChecks"] = await root_ctx.idle_checker_host.get_idle_check_report(sess.id)
 
         # Resource limits collected from agent heartbeats were erased, as they were deprecated
         # TODO: factor out policy/image info as a common repository
 
         log.info("information retrieved: {0!r}", resp)
     except BackendError:
         log.exception("GET_INFO: exception")
@@ -2241,14 +2327,41 @@
         await root_ctx.registry.shutdown_service(session, service_name)
     except BackendError:
         log.exception("SHUTDOWN_SERVICE: exception")
         raise
     return web.Response(status=204)
 
 
+async def find_dependent_sessions(
+    root_session_name_or_id: str | uuid.UUID,
+    db_session: SASession,
+    access_key: AccessKey,
+) -> Set[uuid.UUID]:
+    async def _find_dependent_sessions(session_id: uuid.UUID) -> Set[uuid.UUID]:
+        result = await db_session.execute(
+            sa.select(SessionDependencyRow).where(SessionDependencyRow.depends_on == session_id)
+        )
+        dependent_sessions: set[uuid.UUID] = {x.session_id for x in result.scalars()}
+
+        recursive_dependent_sessions: List[Set[uuid.UUID]] = [
+            await _find_dependent_sessions(dependent_session)
+            for dependent_session in dependent_sessions
+        ]
+
+        for recursive_dependent_session in recursive_dependent_sessions:
+            dependent_sessions |= recursive_dependent_session
+
+        return dependent_sessions
+
+    root_session = await SessionRow.get_session(
+        root_session_name_or_id, access_key=access_key, db_session=db_session
+    )
+    return await _find_dependent_sessions(cast(uuid.UUID, root_session.id))
+
+
 @server_status_required(READ_ALLOWED)
 @auth_required
 async def upload_files(request: web.Request) -> web.Response:
     loop = asyncio.get_event_loop()
     reader = await request.multipart()
     root_ctx: RootContext = request.app["_root.context"]
     session_name = request.match_info["session_name"]
@@ -2566,27 +2679,25 @@
     app_ctx.session_creation_tracker = {}
     app_ctx.database_ptask_group = aiotools.PersistentTaskGroup()
     app_ctx.rpc_ptask_group = aiotools.PersistentTaskGroup()
     app_ctx.webhook_ptask_group = aiotools.PersistentTaskGroup()
 
     # passive events
     evd = root_ctx.event_dispatcher
-    evd.subscribe(
+    evd.consume(
         KernelPreparingEvent, app, handle_kernel_creation_lifecycle, name="api.session.kprep"
     )
-    evd.subscribe(
-        KernelPullingEvent, app, handle_kernel_creation_lifecycle, name="api.session.kpull"
-    )
-    evd.subscribe(
+    evd.consume(KernelPullingEvent, app, handle_kernel_creation_lifecycle, name="api.session.kpull")
+    evd.consume(
         KernelCreatingEvent, app, handle_kernel_creation_lifecycle, name="api.session.kcreat"
     )
-    evd.subscribe(
+    evd.consume(
         KernelStartedEvent, app, handle_kernel_creation_lifecycle, name="api.session.kstart"
     )
-    evd.subscribe(
+    evd.consume(
         KernelCancelledEvent, app, handle_kernel_creation_lifecycle, name="api.session.kstart"
     )
     evd.subscribe(
         SessionStartedEvent,
         app,
         handle_session_creation_lifecycle,
         name="api.session.sstart",
@@ -2633,15 +2744,14 @@
     evd.consume(SessionSuccessEvent, app, handle_batch_result)
     evd.consume(SessionFailureEvent, app, handle_batch_result)
     evd.consume(AgentStartedEvent, app, handle_agent_lifecycle)
     evd.consume(AgentTerminatedEvent, app, handle_agent_lifecycle)
     evd.consume(AgentHeartbeatEvent, app, handle_agent_heartbeat)
 
     # action-trigerring events
-    evd.consume(DoSyncKernelStatsEvent, app, handle_kernel_stat_sync, name="api.session.synckstat")
     evd.consume(DoSyncKernelLogsEvent, app, handle_kernel_log, name="api.session.syncklog")
     evd.consume(DoTerminateSessionEvent, app, handle_destroy_session, name="api.session.doterm")
 
     app_ctx.pending_waits = set()
 
     # Scan ALIVE agents
     app_ctx.agent_lost_checker = aiotools.create_timer(
@@ -2687,14 +2797,17 @@
     cors.add(session_resource.add_route("GET", get_info))
     cors.add(session_resource.add_route("PATCH", restart))
     cors.add(session_resource.add_route("DELETE", destroy))
     cors.add(session_resource.add_route("POST", execute))
     task_log_resource = cors.add(app.router.add_resource(r"/_/logs"))
     cors.add(task_log_resource.add_route("HEAD", get_task_logs))
     cors.add(task_log_resource.add_route("GET", get_task_logs))
+    cors.add(
+        app.router.add_route("GET", "/{session_name}/direct-access-info", get_direct_access_info)
+    )
     cors.add(app.router.add_route("GET", "/{session_name}/logs", get_container_logs))
     cors.add(app.router.add_route("POST", "/{session_name}/rename", rename_session))
     cors.add(app.router.add_route("POST", "/{session_name}/interrupt", interrupt))
     cors.add(app.router.add_route("POST", "/{session_name}/complete", complete))
     cors.add(app.router.add_route("POST", "/{session_name}/shutdown-service", shutdown_service))
     cors.add(app.router.add_route("POST", "/{session_name}/upload", upload_files))
     cors.add(app.router.add_route("GET", "/{session_name}/download", download_files))
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/session_template.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/stream.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,17 +199,19 @@
                                             session,
                                         ),
                                     ),
                                 )
                                 socks[0].close()
                             else:
                                 log.warning(
-                                    "stream_stdin({0}): "
-                                    "duplicate kernel restart request; "
-                                    "ignoring it.",
+                                    (
+                                        "stream_stdin({0}): "
+                                        "duplicate kernel restart request; "
+                                        "ignoring it."
+                                    ),
                                     stream_key,
                                 )
                 elif msg.type == aiohttp.WSMsgType.ERROR:
                     log.warning(
                         "stream_stdin({0}): connection closed ({1})", stream_key, ws.exception()
                     )
         except asyncio.CancelledError:
@@ -394,16 +396,18 @@
             )
         raise
     except asyncio.CancelledError:
         if not ws.closed:
             await ws.send_json(
                 {
                     "status": "server-restarting",
-                    "msg": "The API server is going to restart for maintenance. "
-                    "Please connect again with the same run ID.",
+                    "msg": (
+                        "The API server is going to restart for maintenance. "
+                        "Please connect again with the same run ID."
+                    ),
                 }
             )
         raise
     finally:
         return ws
 
 
@@ -501,21 +505,19 @@
     else:
         raise InvalidAPIParameters(f"Unsupported service protocol: {sport['protocol']}")
 
     redis_live = root_ctx.redis_live
     conn_tracker_key = f"session.{kernel_id}.active_app_connections"
     conn_tracker_val = f"{kernel_id}:{service}:{stream_id}"
 
-    _conn_tracker_script = textwrap.dedent(
-        """
+    _conn_tracker_script = textwrap.dedent("""
         local now = redis.call('TIME')
         now = now[1] + (now[2] / (10^6))
         redis.call('ZADD', KEYS[1], now, ARGV[1])
-    """
-    )
+    """)
 
     async def refresh_cb(kernel_id: str, data: bytes) -> None:
         await asyncio.shield(
             rpc_ptask_group.create_task(
                 call_non_bursty(
                     conn_tracker_key,
                     apartial(
@@ -695,15 +697,16 @@
                 no_packet_timeout: timedelta = tx.TimeDuration().check(
                     await shared_config.etcd.get("config/idle/app-streaming-packet-timeout")
                     or "5m",
                 )
             except grpc.aio.AioRpcError as e:
                 if e.code() == grpc.StatusCode.UNAVAILABLE:
                     log.warn(
-                        "stream_conn_tracker_gc(): error while connecting to Etcd server, retrying..."
+                        "stream_conn_tracker_gc(): error while connecting to Etcd server,"
+                        " retrying..."
                     )
                 else:
                     raise e
             async with app_ctx.conn_tracker_lock:
                 now = await redis_helper.execute(redis_live, lambda r: r.time())
                 now = now[0] + (now[1] / (10**6))
                 for session_id in app_ctx.active_session_ids.keys():
@@ -721,16 +724,18 @@
                         ),
                     )
                     remaining_count = await redis_helper.execute(
                         redis_live,
                         lambda r: r.zcount(conn_tracker_key, float("-inf"), float("+inf")),
                     )
                     log.debug(
-                        f"conn_tracker: gc {session_id} "
-                        f"removed/remaining = {removed_count}/{remaining_count}",
+                        (
+                            f"conn_tracker: gc {session_id} "
+                            f"removed/remaining = {removed_count}/{remaining_count}"
+                        ),
                     )
                     if prev_remaining_count > 0 and remaining_count == 0:
                         await root_ctx.idle_checker_host.update_app_streaming_status(
                             session_id,
                             AppStreamingStatus.NO_ACTIVE_CONNECTIONS,
                         )
             await asyncio.sleep(10)
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/types.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/userconfig.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/userconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/utils.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,18 @@
             owner_domain = row["domain_name"]
             owner_role = row["role"]
         if request["is_superadmin"]:
             pass
         elif request["is_admin"]:
             if request["user"]["domain_name"] != owner_domain:
                 raise GenericForbidden(
-                    "Domain-admins can perform operations on behalf of "
-                    "other users in the same domain only.",
+                    (
+                        "Domain-admins can perform operations on behalf of "
+                        "other users in the same domain only."
+                    ),
                 )
             if owner_role == UserRole.SUPERADMIN:
                 raise GenericForbidden(
                     "Domain-admins cannot perform operations on behalf of super-admins.",
                 )
             pass
         else:
@@ -121,16 +123,18 @@
             owner_user_role = row["role"]
             owner_user_domain = row["domain_name"]
         if request["is_superadmin"]:
             pass
         elif request["is_admin"]:
             if request["user"]["domain_name"] != owner_user_domain:
                 raise GenericForbidden(
-                    "Domain-admins can perform operations on behalf of "
-                    "other users in the same domain only.",
+                    (
+                        "Domain-admins can perform operations on behalf of "
+                        "other users in the same domain only."
+                    ),
                 )
             if owner_user_role == UserRole.SUPERADMIN:
                 raise GenericForbidden(
                     "Domain-admins cannot perform operations on behalf of super-admins.",
                 )
             pass
         else:
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/vfolder.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/vfolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import functools
 import json
 import logging
 import math
 import stat
 import uuid
 from datetime import datetime
+from enum import StrEnum
 from pathlib import Path
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
@@ -29,22 +30,29 @@
 import aiohttp_cors
 import aiotools
 import attrs
 import sqlalchemy as sa
 import trafaret as t
 from aiohttp import web
 
+from ai.backend.common import msgpack, redis_helper
 from ai.backend.common import validators as tx
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import VFolderHostPermission, VFolderHostPermissionMap
+from ai.backend.common.types import (
+    RedisConnectionInfo,
+    VFolderHostPermission,
+    VFolderHostPermissionMap,
+)
+from ai.backend.manager.models.storage import StorageSessionManager
 
 from ..models import (
     AgentStatus,
     KernelStatus,
     UserRole,
+    UserStatus,
     VFolderAccessStatus,
     VFolderCloneInfo,
     VFolderDeletionInfo,
     VFolderInvitationState,
     VFolderOperationStatus,
     VFolderOwnershipType,
     VFolderPermission,
@@ -55,23 +63,25 @@
     filter_host_allowed_permission,
     get_allowed_vfolder_hosts_by_group,
     get_allowed_vfolder_hosts_by_user,
     groups,
     initiate_vfolder_clone,
     initiate_vfolder_removal,
     kernels,
+    keypair_resource_policies,
     keypairs,
     query_accessible_vfolders,
     query_owned_dotfiles,
     users,
     verify_vfolder_name,
     vfolder_invitations,
     vfolder_permissions,
     vfolders,
 )
+from ..models.utils import execute_with_retry
 from .auth import admin_required, auth_required, superadmin_required
 from .exceptions import (
     BackendAgentError,
     GenericForbidden,
     GroupNotFound,
     InsufficientPrivilege,
     InternalServerError,
@@ -80,14 +90,15 @@
     ServerMisconfiguredError,
     TooManyVFoldersFound,
     VFolderAlreadyExists,
     VFolderCreationFailed,
     VFolderFilterStatusFailed,
     VFolderFilterStatusNotAvailable,
     VFolderNotFound,
+    VFolderOperationFailed,
 )
 from .manager import ALL_ALLOWED, READ_ALLOWED, server_status_required
 from .resource import get_watcher_info
 from .utils import check_api_params, get_user_scopes
 
 if TYPE_CHECKING:
     from .context import RootContext
@@ -297,17 +308,17 @@
     t.Dict(
         {
             t.Key("name"): tx.Slug(allow_dot=True),
             t.Key("host", default=None) >> "folder_host": t.String | t.Null,
             t.Key("usage_mode", default="general"): tx.Enum(VFolderUsageMode) | t.Null,
             t.Key("permission", default="rw"): tx.Enum(VFolderPermission) | t.Null,
             tx.AliasedKey(["unmanaged_path", "unmanagedPath"], default=None): t.String | t.Null,
-            tx.AliasedKey(["group", "groupId", "group_id"], default=None): tx.UUID
-            | t.String
-            | t.Null,
+            tx.AliasedKey(["group", "groupId", "group_id"], default=None): (
+                tx.UUID | t.String | t.Null
+            ),
             t.Key("quota", default=None): tx.BinarySize | t.Null,
             t.Key("cloneable", default=False): t.Bool,
         }
     ),
 )
 async def create(request: web.Request, params: Any) -> web.Response:
     resp: Dict[str, Any] = {}
@@ -336,16 +347,15 @@
             raise GenericForbidden("Insufficient permission")
     else:
         # Resolve host for the new virtual folder.
         if not folder_host:
             folder_host = await root_ctx.shared_config.etcd.get("volumes/default_host")
             if not folder_host:
                 raise InvalidAPIParameters(
-                    "You must specify the vfolder host "
-                    "because the default host is not configured."
+                    "You must specify the vfolder host because the default host is not configured."
                 )
     allowed_vfolder_types = await root_ctx.shared_config.get_vfolder_types()
     for vf_type in allowed_vfolder_types:
         if vf_type not in ("user", "group"):
             raise ServerMisconfiguredError(
                 f"Invalid vfolder type(s): {str(allowed_vfolder_types)}."
                 ' Only "user" or "group" is allowed.'
@@ -608,14 +618,75 @@
         [VFolderDeletionInfo(folder_id, folder_host)],
         root_ctx.storage_manager,
         app_ctx.storage_ptask_group,
     )
     return web.Response(status=204)
 
 
+class ExposedVolumeInfoField(StrEnum):
+    percentage = "percentage"
+    used_bytes = "used_bytes"
+    capacity_bytes = "capacity_bytes"
+
+
+async def fetch_exposed_volume_fields(
+    storage_manager: StorageSessionManager,
+    redis_connection: RedisConnectionInfo,
+    proxy_name: str,
+    volume_name: str,
+) -> Dict[str, int | float]:
+    volume_usage = {}
+
+    show_percentage = ExposedVolumeInfoField.percentage in storage_manager._exposed_volume_info
+    show_used = ExposedVolumeInfoField.used_bytes in storage_manager._exposed_volume_info
+    show_total = ExposedVolumeInfoField.capacity_bytes in storage_manager._exposed_volume_info
+
+    if show_percentage or show_used or show_total:
+        volume_usage_cache = await redis_helper.execute(
+            redis_connection,
+            lambda r: r.get(f"volume.usage.{proxy_name}.{volume_name}"),
+        )
+
+        if volume_usage_cache:
+            volume_usage = msgpack.unpackb(volume_usage_cache)
+        else:
+            async with storage_manager.request(
+                proxy_name,
+                "GET",
+                "folder/fs-usage",
+                json={
+                    "volume": volume_name,
+                },
+            ) as (_, storage_resp):
+                storage_reply = await storage_resp.json()
+
+                if show_used:
+                    volume_usage["used"] = storage_reply[ExposedVolumeInfoField.used_bytes]
+
+                if show_total:
+                    volume_usage["total"] = storage_reply[ExposedVolumeInfoField.capacity_bytes]
+
+                if show_percentage:
+                    volume_usage["percentage"] = (
+                        storage_reply[ExposedVolumeInfoField.used_bytes]
+                        / storage_reply[ExposedVolumeInfoField.capacity_bytes]
+                    ) * 100
+
+            await redis_helper.execute(
+                redis_connection,
+                lambda r: r.set(
+                    f"volume.usage.{proxy_name}.{volume_name}",
+                    msgpack.packb(volume_usage),
+                    ex=60,
+                ),
+            )
+
+    return volume_usage
+
+
 @auth_required
 @server_status_required(READ_ALLOWED)
 @check_api_params(
     t.Dict(
         {
             tx.AliasedKey(["group_id", "groupId"], default=None): tx.UUID | t.String | t.Null,
         }
@@ -650,22 +721,33 @@
     all_hosts = {f"{proxy_name}:{volume_data['name']}" for proxy_name, volume_data in all_volumes}
     allowed_hosts = VFolderHostPermissionMap(
         {host: perms for host, perms in allowed_hosts.items() if host in all_hosts}
     )
     default_host = await root_ctx.shared_config.get_raw("volumes/default_host")
     if default_host not in allowed_hosts:
         default_host = None
+
     volume_info = {
         f"{proxy_name}:{volume_data['name']}": {
             "backend": volume_data["backend"],
             "capabilities": volume_data["capabilities"],
+            "usage": await fetch_exposed_volume_fields(
+                storage_manager=root_ctx.storage_manager,
+                redis_connection=root_ctx.redis_stat,
+                proxy_name=proxy_name,
+                volume_name=volume_data["name"],
+            ),
+            "sftp_scaling_groups": await root_ctx.storage_manager.get_sftp_scaling_groups(
+                proxy_name
+            ),
         }
         for proxy_name, volume_data in all_volumes
         if f"{proxy_name}:{volume_data['name']}" in allowed_hosts
     }
+
     resp = {
         "default": default_host,
         "allowed": sorted(allowed_hosts),
         "volume_info": volume_info,
     }
     return web.json_response(resp, status=200)
 
@@ -1034,21 +1116,21 @@
             user_role=user_role,
             domain_name=domain_name,
             allowed_vfolder_types=allowed_vfolder_types,
         )
         for entry in entries:
             if entry["name"] == new_name:
                 raise InvalidAPIParameters(
-                    "One of your accessible vfolders already has " "the name you requested."
+                    "One of your accessible vfolders already has the name you requested."
                 )
         for entry in entries:
             if entry["name"] == old_name:
                 if not entry["is_owner"]:
                     raise InvalidAPIParameters(
-                        "Cannot change the name of a vfolder " "that is not owned by myself."
+                        "Cannot change the name of a vfolder that is not owned by myself."
                     )
                 await ensure_host_permission_allowed(
                     conn,
                     entry["host"],
                     allowed_vfolder_types=allowed_vfolder_types,
                     user_uuid=user_uuid,
                     resource_policy=resource_policy,
@@ -1101,15 +1183,15 @@
     updated_fields = {}
     if params["cloneable"] is not None and params["cloneable"] != row["cloneable"]:
         updated_fields["cloneable"] = params["cloneable"]
     if params["permission"] is not None and params["permission"] != row["permission"]:
         updated_fields["permission"] = params["permission"]
     if not row["is_owner"]:
         raise InvalidAPIParameters(
-            "Cannot change the options of a vfolder " "that is not owned by myself."
+            "Cannot change the options of a vfolder that is not owned by myself."
         )
 
     if len(updated_fields) > 0:
         async with root_ctx.db.begin() as conn:
             query = sa.update(vfolders).values(**updated_fields).where(vfolders.c.id == row["id"])
             await conn.execute(query)
     return web.Response(status=201)
@@ -1971,16 +2053,15 @@
         users_to_share = [u["uuid"] for u in user_info]
         emails_to_share = [u["email"] for u in user_info]
         if len(user_info) < 1:
             raise ObjectNotFound(object_name="user")
         if len(user_info) < len(params["emails"]):
             users_not_in_vfolder_group = list(set(params["emails"]) - set(emails_to_share))
             raise ObjectNotFound(
-                "Some user does not belong to folder's group: "
-                ",".join(users_not_in_vfolder_group),
+                "Some user does not belong to folder's group: ,".join(users_not_in_vfolder_group),
                 object_name="user",
             )
 
         # Do not share to users who have already been shared the folder.
         query = (
             sa.select([vfolder_permissions.c.user])
             .select_from(vfolder_permissions)
@@ -2278,15 +2359,15 @@
     if not row["cloneable"]:
         raise GenericForbidden("The source vfolder is not permitted to be cloned.")
 
     if not target_folder_host:
         target_folder_host = await root_ctx.shared_config.etcd.get("volumes/default_host")
         if not target_folder_host:
             raise InvalidAPIParameters(
-                "You must specify the vfolder host " "because the default host is not configured."
+                "You must specify the vfolder host because the default host is not configured."
             )
 
     allowed_vfolder_types = await root_ctx.shared_config.get_vfolder_types()
     for vf_type in allowed_vfolder_types:
         if vf_type not in ("user", "group"):
             raise ServerMisconfiguredError(
                 f"Invalid vfolder type(s): {str(allowed_vfolder_types)}."
@@ -2308,15 +2389,16 @@
             domain_name=domain_name,
         )
         if (
             target_folder_host not in allowed_hosts
             or VFolderHostPermission.CREATE not in allowed_hosts[target_folder_host]
         ):
             raise InvalidAPIParameters(
-                f"`{VFolderHostPermission.CREATE}` Not allowed in vfolder host(`{target_folder_host}`)"
+                f"`{VFolderHostPermission.CREATE}` Not allowed in vfolder"
+                f" host(`{target_folder_host}`)"
             )
         # TODO: handle legacy host lists assuming that volume names don't overlap?
         if target_folder_host not in allowed_hosts:
             raise InvalidAPIParameters("You are not allowed to use this vfolder host.")
 
         # Check resource policy's max_vfolder_count
         if resource_policy["max_vfolder_count"] > 0:
@@ -2546,23 +2628,27 @@
                 "VFOLDER.GET_FSTAB_CONTENTS(u:{}): timeout from watcher (agent:{})",
                 access_key,
                 params["agent_id"],
             )
             raise BackendAgentError("TIMEOUT", "Could not fetch fstab data from agent")
         except Exception:
             log.exception(
-                "VFOLDER.GET_FSTAB_CONTENTS(u:{}): "
-                "unexpected error while reading from watcher (agent:{})",
+                (
+                    "VFOLDER.GET_FSTAB_CONTENTS(u:{}): "
+                    "unexpected error while reading from watcher (agent:{})"
+                ),
                 access_key,
                 params["agent_id"],
             )
             raise InternalServerError
     else:
         resp = {
-            "content": "# Since Backend.AI 20.09, reading the manager fstab is no longer supported.",
+            "content": (
+                "# Since Backend.AI 20.09, reading the manager fstab is no longer supported."
+            ),
             "node": "manager",
             "node_id": "manager",
         }
         return web.json_response(resp)
 
 
 @superadmin_required
@@ -2634,16 +2720,18 @@
                     "VFOLDER.LIST_MOUNTS(u:{}): timeout from watcher (agent:{})",
                     access_key,
                     agent_id,
                 )
                 raise
             except Exception:
                 log.exception(
-                    "VFOLDER.LIST_MOUNTS(u:{}): "
-                    "unexpected error while reading from watcher (agent:{})",
+                    (
+                        "VFOLDER.LIST_MOUNTS(u:{}): "
+                        "unexpected error while reading from watcher (agent:{})"
+                    ),
                     access_key,
                     agent_id,
                 )
                 raise
 
     async with root_ctx.db.begin() as conn:
         query = (
@@ -2905,14 +2993,113 @@
     exc_type: Type[Exception],
     exc_obj: Exception,
     tb: TracebackType,
 ):
     log.exception("Error while removing vFolder", exc_info=exc_obj)
 
 
+@superadmin_required
+@server_status_required(ALL_ALLOWED)
+@check_api_params(
+    t.Dict(
+        {
+            t.Key("vfolder"): tx.UUID,
+            t.Key("user_email"): t.String,
+        }
+    ),
+)
+async def change_vfolder_ownership(request: web.Request, params: Any) -> web.Response:
+    """
+    Change the ownership of vfolder
+    For now, we only provide changing the ownership of user-folder
+    """
+    vfolder_id = params["vfolder"]
+    user_email = params["user_email"]
+    root_ctx: RootContext = request.app["_root.context"]
+
+    allowed_hosts_by_user = VFolderHostPermissionMap()
+    async with root_ctx.db.begin_readonly() as conn:
+        j = sa.join(users, keypairs, users.c.email == keypairs.c.user_id)
+        query = (
+            sa.select([users.c.uuid, users.c.domain_name, keypairs.c.resource_policy])
+            .select_from(j)
+            .where((users.c.email == user_email) & (users.c.status == UserStatus.ACTIVE))
+        )
+        try:
+            result = await conn.execute(query)
+        except sa.exc.DataError:
+            raise InvalidAPIParameters
+        user_info = result.first()
+        if user_info is None:
+            raise ObjectNotFound(object_name="user")
+        resource_policy_name = user_info.resource_policy
+        result = await conn.execute(
+            sa.select([keypair_resource_policies.c.allowed_vfolder_hosts]).where(
+                keypair_resource_policies.c.name == resource_policy_name
+            )
+        )
+        resource_policy = result.first()
+        allowed_hosts_by_user = await get_allowed_vfolder_hosts_by_user(
+            conn=conn,
+            resource_policy=resource_policy,
+            domain_name=user_info.domain_name,
+            user_uuid=user_info.uuid,
+        )
+    log.info(
+        "VFOLDER.CHANGE_VFOLDER_OWNERSHIP(email:{}, ak:{}, vfid:{}, uid:{})",
+        request["user"]["email"],
+        request["keypair"]["access_key"],
+        vfolder_id,
+        user_info.uuid,
+    )
+    async with root_ctx.db.begin_readonly() as conn:
+        query = (
+            sa.select([vfolders.c.host]).select_from(vfolders).where(vfolders.c.id == vfolder_id)
+        )
+        folder_host = await conn.scalar(query)
+    if folder_host not in allowed_hosts_by_user:
+        raise VFolderOperationFailed("User to migrate vfolder needs an access to the storage host.")
+
+    async def _update() -> None:
+        async with root_ctx.db.begin() as conn:
+            # TODO: we need to implement migration from project to other project
+            #       for now we only support migration btw user folder only
+            #
+            query = (
+                sa.update(vfolders)
+                .values(user=user_info.uuid)
+                .where(
+                    (vfolders.c.id == vfolder_id)
+                    & (vfolders.c.ownership_type == VFolderOwnershipType.USER)
+                )
+            )
+            await conn.execute(query)
+
+    await execute_with_retry(_update)
+
+    async def _delete_vfolder_related_rows() -> None:
+        async with root_ctx.db.begin() as conn:
+            # delete vfolder_invitation if the new owner user has already been shared with the vfolder
+            query = sa.delete(vfolder_invitations).where(
+                (vfolder_invitations.c.invitee == user_email)
+                & (vfolder_invitations.c.vfolder == vfolder_id)
+            )
+            await conn.execute(query)
+            # delete vfolder_permission if the new owner user has already been shared with the vfolder
+            query = sa.delete(vfolder_permissions).where(
+                (vfolder_permissions.c.vfolder == vfolder_id)
+                & (vfolder_permissions.c.user == user_info.uuid)
+            )
+            await conn.execute(query)
+
+    await execute_with_retry(_delete_vfolder_related_rows)
+
+    return web.json_response({}, status=200)
+
+
 @attrs.define(slots=True, auto_attribs=True, init=False)
 class PrivateContext:
     database_ptask_group: aiotools.PersistentTaskGroup
     storage_ptask_group: aiotools.PersistentTaskGroup
 
 
 async def init(app: web.Application) -> None:
@@ -2975,12 +3162,13 @@
     cors.add(add_route("DELETE", r"/invitations/delete", delete_invitation))
     cors.add(add_route("GET", r"/_/shared", list_shared_vfolders))
     cors.add(add_route("POST", r"/_/shared", update_shared_vfolder))
     cors.add(add_route("GET", r"/_/fstab", get_fstab_contents))
     cors.add(add_route("GET", r"/_/mounts", list_mounts))
     cors.add(add_route("POST", r"/_/mounts", mount_host))
     cors.add(add_route("DELETE", r"/_/mounts", umount_host))
+    cors.add(add_route("POST", r"/_/change-ownership", change_vfolder_ownership))
     cors.add(add_route("GET", r"/_/quota", get_quota))
     cors.add(add_route("POST", r"/_/quota", update_quota))
     cors.add(add_route("GET", r"/_/usage", get_usage))
     cors.add(add_route("GET", r"/_/used-bytes", get_used_bytes))
     return app, []
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/api/wsproxy.py` & `backend.ai-manager-23.3.1/ai/backend/manager/api/wsproxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/cli/__main__.py` & `backend.ai-manager-23.3.1/ai/backend/manager/cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,26 +65,28 @@
 )
 @click.option(
     "--psql-container",
     "container_name",
     type=str,
     default=None,
     metavar="ID_OR_NAME",
-    help="Open a postgres client shell using the psql executable "
-    "shipped with the given postgres container. "
-    'If not set or set as an empty string "", it will auto-detect '
-    "the psql container from the halfstack. "
-    'If set "-", it will use the host-provided psql executable. '
-    "You may append additional arguments passed to the psql cli command. "
-    "[default: auto-detect from halfstack]",
+    help=(
+        "Open a postgres client shell using the psql executable "
+        "shipped with the given postgres container. "
+        'If not set or set as an empty string "", it will auto-detect '
+        "the psql container from the halfstack. "
+        'If set "-", it will use the host-provided psql executable. '
+        "You may append additional arguments passed to the psql cli command. "
+        "[default: auto-detect from halfstack]"
+    ),
 )
 @click.option(
     "--psql-help",
     is_flag=True,
-    help="Show the help text of the psql command instead of " "this dbshell command.",
+    help="Show the help text of the psql command instead of this dbshell command.",
 )
 @click.argument("psql_args", nargs=-1, type=click.UNPROCESSED)
 @click.pass_obj
 def dbshell(cli_ctx: CLIContext, container_name, psql_help, psql_args):
     """
     Run the database shell.
 
@@ -100,16 +102,18 @@
     if not container_name:
         # Try to get the database container name of the halfstack
         candidate_container_names = subprocess.check_output(
             ["docker", "ps", "--format", "{{.Names}}", "--filter", "name=half-db"],
         )
         if not candidate_container_names:
             click.echo(
-                "Could not find the halfstack postgres container. "
-                "Please set the container name explicitly.",
+                (
+                    "Could not find the halfstack postgres container. "
+                    "Please set the container name explicitly."
+                ),
                 err=True,
             )
             sys.exit(ExitCode.FAILURE)
         container_name = candidate_container_names.decode().splitlines()[0].strip()
     elif container_name == "-":
         # Use the host-provided psql command
         cmd = [
@@ -163,19 +167,21 @@
     help="The retention limit. e.g., 20d, 1mo, 6mo, 1yr",
 )
 @click.option(
     "-v",
     "--vacuum-full",
     type=bool,
     default=False,
-    help="Reclaim storage occupied by dead tuples."
-    "If not set or set False, it will run VACUUM without FULL. "
-    "If set True, it will run VACUUM FULL. "
-    "When VACUUM FULL is being processed, the database is locked. "
-    "[default: False]",
+    help=(
+        "Reclaim storage occupied by dead tuples."
+        "If not set or set False, it will run VACUUM without FULL. "
+        "If set True, it will run VACUUM FULL. "
+        "When VACUUM FULL is being processed, the database is locked. "
+        "[default: False]"
+    ),
 )
 @click.pass_obj
 def clear_history(cli_ctx: CLIContext, retention, vacuum_full) -> None:
     """
     Delete old records from the kernels table and
     invoke the PostgreSQL's vaccuum operation to clear up the actual disk space.
     """
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/cli/context.py` & `backend.ai-manager-23.3.1/ai/backend/manager/cli/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/cli/dbschema.py` & `backend.ai-manager-23.3.1/ai/backend/manager/cli/dbschema.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 @cli.command()
 @click.option(
     "-f",
     "--alembic-config",
     default="alembic.ini",
     metavar="PATH",
-    help="The path to Alembic config file. " "[default: alembic.ini]",
+    help="The path to Alembic config file. [default: alembic.ini]",
 )
 @click.pass_obj
 def show(cli_ctx: CLIContext, alembic_config) -> None:
     """Show the current schema information."""
 
     def _get_current_rev_sync(connection: Connection) -> str | None:
         context = MigrationContext.configure(connection)
@@ -65,15 +65,15 @@
 
 @cli.command()
 @click.option(
     "-f",
     "--alembic-config",
     default="alembic.ini",
     metavar="PATH",
-    help="The path to Alembic config file. " "[default: alembic.ini]",
+    help="The path to Alembic config file. [default: alembic.ini]",
 )
 @click.pass_obj
 def oneshot(cli_ctx: CLIContext, alembic_config) -> None:
     """
     Set up your database with one-shot schema migration instead of
     iterating over multiple revisions if there is no existing database.
     It uses alembic.ini to configure database connection.
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/cli/etcd.py` & `backend.ai-manager-23.3.1/ai/backend/manager/cli/etcd.py`

 * *Files 11% similar despite different names*

```diff
@@ -139,17 +139,19 @@
 @click.argument("src_prefix", type=str)
 @click.argument("dst_prefix", type=str)
 @click.option(
     "-s",
     "--scope",
     type=EnumChoice(ConfigScopes),
     default=ConfigScopes.GLOBAL,
-    help="The configuration scope to get/put the subtree. "
-    "To move between different scopes, use the global scope "
-    "and specify the per-scope prefixes manually.",
+    help=(
+        "The configuration scope to get/put the subtree. "
+        "To move between different scopes, use the global scope "
+        "and specify the per-scope prefixes manually."
+    ),
 )
 @click.pass_obj
 def move_subtree(cli_ctx: CLIContext, src_prefix, dst_prefix, scope) -> None:
     """
     Move a subtree to another key prefix.
     """
 
@@ -167,15 +169,15 @@
 
 
 @cli.command()
 @click.argument("key")
 @click.option(
     "--prefix",
     is_flag=True,
-    help="Get all key-value pairs prefixed with the given key " "as a JSON form.",
+    help="Get all key-value pairs prefixed with the given key as a JSON form.",
 )
 @click.option(
     "-s",
     "--scope",
     type=EnumChoice(ConfigScopes),
     default=ConfigScopes.GLOBAL,
     help="The configuration scope to put the value.",
@@ -346,7 +348,66 @@
 @click.argument("value")
 @click.pass_obj
 def unquote(cli_ctx: CLIContext, value) -> None:
     """
     Unquote the given string used as a URL piece in etcd keys.
     """
     print(etcd_unquote(value))
+
+
+@cli.command()
+@click.argument("proxy")
+@click.argument("scaling_groups")
+@click.option(
+    "-s",
+    "--scope",
+    type=EnumChoice(ConfigScopes),
+    default=ConfigScopes.GLOBAL,
+    help="The configuration scope to put the value.",
+)
+@click.pass_obj
+def set_storage_sftp_scaling_group(cli_ctx: CLIContext, proxy, scaling_groups, scope) -> None:
+    """
+    Updates storage proxy node config's SFTP desginated scaling groups.
+    To enter multiple scaling groups concatenate names with comma(,).
+    """
+
+    async def _impl():
+        async with etcd_ctx(cli_ctx) as etcd:
+            data = await etcd.get_prefix(f"volumes/proxies/{proxy}", scope=scope)
+            if len(data) == 0:
+                log.error("proxy {} does not exist", proxy)
+                sys.exit(ExitCode.FAILURE)
+            await etcd.put(
+                f"volumes/proxies/{proxy}/sftp_scaling_groups",
+                ",".join([x.strip() for x in scaling_groups.split(",")]),
+            )
+
+    with cli_ctx.logger:
+        asyncio.run(_impl())
+
+
+@cli.command()
+@click.argument("proxy")
+@click.option(
+    "-s",
+    "--scope",
+    type=EnumChoice(ConfigScopes),
+    default=ConfigScopes.GLOBAL,
+    help="The configuration scope to put the value.",
+)
+@click.pass_obj
+def remove_storage_sftp_scaling_group(cli_ctx: CLIContext, proxy, scope) -> None:
+    """
+    Removes storage proxy node config's SFTP desginated scaling groups.
+    """
+
+    async def _impl():
+        async with etcd_ctx(cli_ctx) as etcd:
+            data = await etcd.get_prefix(f"volumes/proxies/{proxy}", scope=scope)
+            if len(data) == 0:
+                log.error("proxy {} does not exist", proxy)
+                sys.exit(ExitCode.FAILURE)
+            await etcd.delete(f"volumes/proxies/{proxy}/sftp_scaling_groups")
+
+    with cli_ctx.logger:
+        asyncio.run(_impl())
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/cli/fixture.py` & `backend.ai-manager-23.3.1/ai/backend/manager/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/cli/gql.py` & `backend.ai-manager-23.3.1/ai/backend/manager/cli/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/cli/image.py` & `backend.ai-manager-23.3.1/ai/backend/manager/cli/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/cli/image_impl.py` & `backend.ai-manager-23.3.1/ai/backend/manager/cli/image_impl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/config.py` & `backend.ai-manager-23.3.1/ai/backend/manager/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,19 +130,23 @@
      - default_host: "{default-proxy}:{default-volume}"
      + proxies:   # each proxy may provide multiple volumes
        + "local"  # proxy name
          - client_api: "http://localhost:6021"
          - manager_api: "http://localhost:6022"
          - secret: "xxxxxx..."       # for manager API
          - ssl_verify: true | false  # for manager API
+         - sftp_scaling_groups: "group-1,group-2,..."
        + "mynas1"
          - client_api: "https://proxy1.example.com:6021"
          - manager_api: "https://proxy1.example.com:6022"
          - secret: "xxxxxx..."       # for manager API
          - ssl_verify: true | false  # for manager API
+         - sftp_scaling_groups: "group-3,group-4,..."
+     # 23.03 and later
+       + exposed_volume_info: "percentage"
        ...
      ...
    ...
  + nodes
    + manager
      - {instance-id}: "up"
      ...
@@ -244,15 +248,15 @@
                     ),
                     t.Key("num-proc", default=_max_cpu_count): t.Int[1:_max_cpu_count],
                     t.Key("id", default=f"i-{socket.gethostname()}"): t.String,
                     t.Key("user", default=None): tx.UserID(default_uid=_file_perm.st_uid),
                     t.Key("user", default=None): tx.UserID(default_uid=_file_perm.st_uid),
                     t.Key("group", default=None): tx.GroupID(default_gid=_file_perm.st_gid),
                     t.Key("service-addr", default=("0.0.0.0", 8080)): tx.HostPortPair,
-                    t.Key("heartbeat-timeout", default=5.0): t.Float[1.0:],  # type: ignore
+                    t.Key("heartbeat-timeout", default=40.0): t.Float[1.0:],  # type: ignore
                     t.Key("secret", default=None): t.Null | t.String,
                     t.Key("ssl-enabled", default=False): t.ToBool,
                     t.Key("ssl-cert", default=None): t.Null | tx.Path(type="file"),
                     t.Key("ssl-privkey", default=None): t.Null | tx.Path(type="file"),
                     t.Key("event-loop", default="asyncio"): t.Enum("asyncio", "uvloop"),
                     t.Key("distributed-lock", default="pg_advisory"): t.Enum(
                         "filelock", "pg_advisory", "redlock", "etcd"
@@ -266,14 +270,19 @@
                     t.Key("disabled-plugins", default=None): t.Null | tx.ToSet,
                     t.Key("hide-agents", default=False): t.Bool,
                     t.Key("importer-image", default="lablup/importer:manylinux2010"): t.String,
                     t.Key("max-wsmsg-size", default=16 * (2**20)): t.ToInt,  # default: 16 MiB
                     t.Key("aiomonitor-port", default=48100): t.Int[1:65535],
                 }
             ).allow_extra("*"),
+            t.Key("pipeline", default=None): t.Null | t.Dict(
+                {
+                    t.Key("event-queue", default=None): t.Null | tx.HostPortPair,
+                },
+            ).allow_extra("*"),
             t.Key("docker-registry"): t.Dict(
                 {  # deprecated in v20.09
                     t.Key("ssl-verify", default=True): t.ToBool,
                 }
             ).allow_extra("*"),
             t.Key("logging"): t.Any,  # checked in ai.backend.common.logging
             t.Key("debug"): t.Dict(
@@ -343,16 +352,17 @@
             {
                 t.Key("allow-origins", default=_shdefs["api"]["allow-origins"]): t.String,
             }
         ).allow_extra("*"),
         t.Key("redis", default=_shdefs["redis"]): t.Dict(
             {
                 t.Key("addr", default=_shdefs["redis"]["addr"]): t.Null | tx.HostPortPair,
-                t.Key("sentinel", default=None): t.Null
-                | tx.DelimiterSeperatedList(tx.HostPortPair),
+                t.Key("sentinel", default=None): t.Null | tx.DelimiterSeperatedList(
+                    tx.HostPortPair
+                ),
                 t.Key("service_name", default=None): t.Null | t.String,
                 t.Key("password", default=_shdefs["redis"]["password"]): t.Null | t.String,
             }
         ).allow_extra("*"),
         t.Key("docker", default=_shdefs["docker"]): t.Dict(
             {
                 t.Key("registry"): t.Mapping(t.String, container_registry_iv),
@@ -374,16 +384,15 @@
                     {
                         t.Key("agent", default=_shdefs["network"]["subnet"]["agent"]): tx.IPNetwork,
                         t.Key(
                             "container", default=_shdefs["network"]["subnet"]["container"]
                         ): tx.IPNetwork,
                     }
                 ).allow_extra("*"),
-                t.Key("overlay", default=None): t.Null
-                | t.Dict(
+                t.Key("overlay", default=None): t.Null | t.Dict(
                     {
                         t.Key("mtu", default=1500): t.Int[1:],
                     }
                 ).allow_extra("*"),
             }
         ).allow_extra("*"),
         t.Key("watcher", default=_shdefs["watcher"]): t.Dict(
@@ -401,17 +410,21 @@
             tx.Slug,
             t.Dict(
                 {
                     t.Key("client_api"): t.String,
                     t.Key("manager_api"): t.String,
                     t.Key("secret"): t.String,
                     t.Key("ssl_verify"): t.ToBool,
+                    t.Key("sftp_scaling_groups", default=None): t.Null | tx.StringList(
+                        delimiter=","
+                    ),
                 }
             ),
         ),
+        t.Key("exposed_volume_info", default="percentage"): tx.StringList(delimiter=","),
     }
 ).allow_extra("*")
 
 
 ConfigWatchCallback = Callable[[Sequence[str]], Awaitable[None]]
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/__init__.py` & `backend.ai-manager-23.3.1/ai/backend/manager/container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/base.py` & `backend.ai-manager-23.3.1/ai/backend/manager/container_registry/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -184,72 +184,61 @@
                 tg.create_task(self._scan_tag(sess, rqst_args, image, tag))
 
     async def _scan_tag(
         self,
         sess: aiohttp.ClientSession,
         rqst_args: dict[str, Any],
         image: str,
-        tag: str,
+        digest: str,
+        tag: Optional[str] = None,
     ) -> None:
-        async def _load_manifest(_tag: str):
+        async with self.sema.get():
             async with sess.get(
-                self.registry_url / f"v2/{image}/manifests/{_tag}", **rqst_args
+                self.registry_url / f"v2/{image}/manifests/{digest}", **rqst_args
             ) as resp:
                 if resp.status == 404:
                     # ignore missing tags
                     # (may occur after deleting an image from the docker hub)
-                    return {}
+                    return
                 resp.raise_for_status()
                 data = await resp.json()
 
-                if data["mediaType"] == "application/vnd.docker.distribution.manifest.list.v2+json":
-                    # recursively call _load_manifests with detected arch and corresponding image digest
-                    ret = {}
-                    for m in data["manifests"]:
-                        ret.update(
-                            await _load_manifest(
-                                m["digest"],
-                            ),
-                        )
-                    if (reporter := self.reporter.get()) is not None:
-                        reporter.total_progress += len(ret) - 1
-                    return ret
-
                 config_digest = data["config"]["digest"]
                 size_bytes = sum(layer["size"] for layer in data["layers"]) + data["config"]["size"]
                 async with sess.get(
                     self.registry_url / f"v2/{image}/blobs/{config_digest}", **rqst_args
                 ) as resp:
                     resp.raise_for_status()
                     data = json.loads(await resp.read())
                     architecture = arch_name_aliases.get(data["architecture"], data["architecture"])
                     labels = {}
                     if "container_config" in data:
                         raw_labels = data["container_config"].get("Labels")
                         if raw_labels:
                             labels.update(raw_labels)
                         else:
-                            log.warn("label not found on image {}:{}/{}", image, _tag, architecture)
+                            log.warn(
+                                "label not found on image {}:{}/{}", image, digest, architecture
+                            )
                     else:
                         raw_labels = data["config"].get("Labels")
                         if raw_labels:
                             labels.update(raw_labels)
                         else:
-                            log.warn("label not found on image {}:{}/{}", image, _tag, architecture)
-                    return {
+                            log.warn(
+                                "label not found on image {}:{}/{}", image, digest, architecture
+                            )
+                    manifest = {
                         architecture: {
                             "size": size_bytes,
                             "labels": labels,
                             "digest": config_digest,
                         },
                     }
-
-        async with self.sema.get():
-            manifests = await _load_manifest(tag)
-        await self._read_manifest(image, tag, manifests)
+        await self._read_manifest(image, tag or digest, manifest)
 
     async def _read_manifest(
         self,
         image: str,
         tag: str,
         manifests: dict[str, dict],
         skip_reason: Optional[str] = None,
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/docker.py` & `backend.ai-manager-23.3.1/ai/backend/manager/container_registry/docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                     for item in data["results"]:
                         # skip legacy images
                         if item["name"].startswith("kernel-"):
                             continue
                         yield f"{username}/{item['name']}"
                 else:
                     log.error(
-                        "Failed to fetch repository list from {0} " "(status={1})",
+                        "Failed to fetch repository list from {0} (status={1})",
                         repo_list_url,
                         resp.status,
                     )
                     break
             repo_list_url = None
             next_page_link = data.get("next", None)
             if next_page_link:
@@ -70,16 +70,15 @@
                 if resp.status == 200:
                     data = json.loads(await resp.read())
                     for item in data["repositories"]:
                         yield item
                     log.debug("found {} repositories", len(data["repositories"]))
                 else:
                     log.warning(
-                        "Docker registry {0} does not allow/support "
-                        "catalog search. (status={1})",
+                        "Docker registry {0} does not allow/support catalog search. (status={1})",
                         self.registry_url,
                         resp.status,
                     )
                     break
                 catalog_url = None
                 next_page_link = resp.links.get("next")
                 if next_page_link:
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/container_registry/local.py` & `backend.ai-manager-23.3.1/ai/backend/manager/container_registry/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import logging
-from typing import AsyncIterator
+from typing import AsyncIterator, Optional
 
 import aiohttp
 import sqlalchemy as sa
 import yarl
 
 from ai.backend.common.docker import get_docker_connector
 from ai.backend.common.logging import BraceStyleAdapter
@@ -49,33 +49,34 @@
         await self._scan_tag(sess, {}, repo, tag)
 
     async def _scan_tag(
         self,
         sess: aiohttp.ClientSession,
         rqst_args: dict[str, str],
         image: str,
-        tag: str,
+        digest: str,
+        tag: Optional[str] = None,
     ) -> None:
         async def _read_image_info(
             _tag: str,
         ) -> tuple[dict[str, dict], str | None]:
             async with sess.get(
-                self.registry_url / "images" / f"{image}:{tag}" / "json"
+                self.registry_url / "images" / f"{image}:{digest}" / "json"
             ) as response:
                 data = await response.json()
                 architecture = data["Architecture"]
                 summary = {
                     "Id": data["Id"],
                     "RepoDigests": data.get("RepoDigests", []),
                     "Config.Image": data["Config"]["Image"],
                     "ContainerConfig.Image": data["ContainerConfig"]["Image"],
                     "Architecture": data["Architecture"],
                 }
                 log.debug(
-                    "scanned image info: {}:{}\n{}", image, tag, json.dumps(summary, indent=2)
+                    "scanned image info: {}:{}\n{}", image, digest, json.dumps(summary, indent=2)
                 )
                 already_exists = 0
                 config_digest = data["Id"]
                 async with self.db.begin_readonly_session() as db_session:
                     already_exists = await db_session.scalar(
                         sa.select([sa.func.count(ImageRow.id)]).where(
                             ImageRow.config_digest == config_digest,
@@ -89,9 +90,9 @@
                         "size": data["Size"],
                         "labels": data["Config"]["Labels"],
                         "digest": config_digest,
                     },
                 }, None
 
         async with self.sema.get():
-            manifests, skip_reason = await _read_image_info(tag)
-            await self._read_manifest(image, tag, manifests, skip_reason)
+            manifests, skip_reason = await _read_image_info(digest)
+            await self._read_manifest(image, digest, manifests, skip_reason)
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/defs.py` & `backend.ai-manager-23.3.1/ai/backend/manager/defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,23 +48,33 @@
     "/tmp",
     "/usr",
     "/var",
     "/home",
 ]
 RESERVED_VFOLDER_PATTERNS = [re.compile(x) for x in _RESERVED_VFOLDER_PATTERNS]
 
+# Mapping between vfolder names and their in-container paths.
+VFOLDER_DSTPATHS_MAP = {
+    ".linuxbrew": "/home/linuxbrew/.linuxbrew",
+}
+
 # Redis database IDs depending on purposes
 REDIS_STAT_DB: Final = 0
 REDIS_RLIM_DB: Final = 1
 REDIS_LIVE_DB: Final = 2
 REDIS_IMAGE_DB: Final = 3
 REDIS_STREAM_DB: Final = 4
 REDIS_STREAM_LOCK: Final = 5
 
 
+# Redis database IDs used for plugins
+class PluginDatabaseID(enum.IntEnum):
+    SESSION_EVENT = 1
+
+
 # The unique identifiers for distributed locks.
 # To be used with PostgreSQL advisory locks, the values are defined as integers.
 class LockID(enum.IntEnum):
     LOCKID_TEST = 42
     LOCKID_SCHEDULE = 91
     LOCKID_PREPARE = 92
     LOCKID_SCHEDULE_TIMER = 191
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/exceptions.py` & `backend.ai-manager-23.3.1/ai/backend/manager/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Tuple, TypedDict
+import traceback
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    List,
+    NotRequired,
+    Tuple,
+    TypedDict,
+)
 
 from aiotools import TaskGroupError
 
 if TYPE_CHECKING:
     from ai.backend.common.types import AgentId
 
 
@@ -51,53 +59,63 @@
 
 class MultiAgentError(TaskGroupError):
     """
     An exception that is a collection of multiple errors from multiple agents.
     """
 
 
-class ErrorDetail(TypedDict, total=False):
+class ErrorDetail(TypedDict):
     src: str
     name: str
     repr: str
-    agent_id: str  # optional
-    collection: List[Any]  # optional; currently mypy cannot handle recursive types
+    agent_id: NotRequired[str]
+    collection: NotRequired[List[ErrorDetail]]
+    traceback: NotRequired[str]
 
 
 class ErrorStatusInfo(TypedDict):
     error: ErrorDetail
 
 
-def convert_to_status_data(e: Exception, is_debug: bool = False) -> ErrorStatusInfo:
+def convert_to_status_data(
+    e: Exception,
+    is_debug: bool = False,
+    *,
+    src: str | None = None,
+) -> ErrorStatusInfo:
     data: ErrorStatusInfo
     match e:
         case MultiAgentError():
             return {
                 "error": {
                     "src": "agent",
                     "name": "MultiAgentError",
                     "repr": f"MultiAgentError({len(e.__errors__)})",
                     "collection": [
-                        convert_to_status_data(sub_error, is_debug)["error"]
+                        convert_to_status_data(sub_error, is_debug, src="agent")["error"]
                         for sub_error in e.__errors__
                     ],
                 },
             }
         case AgentError():
             data = {
                 "error": {
                     "src": "agent",
                     "name": e.exc_name,
                     "repr": e.exc_repr,
                 },
             }
             if is_debug:
                 data["error"]["agent_id"] = e.agent_id
+                data["error"]["traceback"] = e.exc_tb or ""
             return data
         case _:
-            return {
+            data = {
                 "error": {
-                    "src": "other",
+                    "src": "other" if src is None else src,
                     "name": e.__class__.__name__,
                     "repr": repr(e),
                 },
             }
+            if is_debug:
+                data["error"]["traceback"] = "\n".join(traceback.format_tb(e.__traceback__))
+            return data
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/idle.py` & `backend.ai-manager-23.3.1/ai/backend/manager/idle.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 from __future__ import annotations
 
+import asyncio
 import enum
 import logging
 import math
 from abc import ABCMeta, abstractmethod
-from collections import defaultdict
+from collections import UserDict, defaultdict
 from datetime import datetime, timedelta
 from decimal import Decimal
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     DefaultDict,
+    Final,
     List,
     Mapping,
     MutableMapping,
+    NamedTuple,
+    Optional,
     Sequence,
     Set,
     Type,
     Union,
+    cast,
 )
 
+import aiotools
 import sqlalchemy as sa
 import trafaret as t
-from dateutil.tz import tzutc
+from aiotools import TaskGroupError
 from sqlalchemy.engine import Row
 
 import ai.backend.common.validators as tx
-from ai.backend.common import msgpack
-from ai.backend.common import redis_helper as redis_helper
+from ai.backend.common import msgpack, redis_helper
 from ai.backend.common.distributed import GlobalTimer
 from ai.backend.common.events import (
     AbstractEvent,
     DoIdleCheckEvent,
     DoTerminateSessionEvent,
     EventDispatcher,
     EventHandler,
@@ -41,45 +46,119 @@
     ExecutionFinishedEvent,
     ExecutionStartedEvent,
     ExecutionTimeoutEvent,
     KernelLifecycleEventReason,
     SessionStartedEvent,
 )
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import AccessKey, RedisConnectionInfo, SessionTypes
+from ai.backend.common.types import AccessKey, BinarySize, RedisConnectionInfo, SessionTypes
 from ai.backend.common.utils import nmget
 
 from .defs import DEFAULT_ROLE, REDIS_LIVE_DB, REDIS_STAT_DB, LockID
-from .models import kernels, keypair_resource_policies, keypairs
-from .models.kernel import LIVE_STATUS
+from .models.kernel import LIVE_STATUS, kernels
+from .models.keypair import keypairs
+from .models.resource_policy import keypair_resource_policies
+from .models.user import users
 from .types import DistributedLockFactory
 
 if TYPE_CHECKING:
     from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
 
     from ai.backend.common.types import AgentId, KernelId, SessionId
 
     from .config import SharedConfig
     from .models.utils import ExtendedAsyncSAEngine as SAEngine
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
+DEFAULT_CHECK_INTERVAL: Final = 15.0
+# idle checker's remaining time should be -1 when the remaining time is negative
+IDLE_TIMEOUT_VALUE: Final = -1
+
+
+class IdleCheckerError(TaskGroupError):
+    """
+    An exception that is a collection of multiple idle checkers.
+    """
+
+
+def parse_unit(resource_name: str, value: float | int) -> float | int:
+    if resource_name.find("mem") == -1:
+        return value
+    return BinarySize(int(value))
+
+
+def calculate_remaining_time(
+    now: datetime,
+    idle_baseline: datetime,
+    timeout_period: timedelta,
+    grace_period_end: Optional[datetime] = None,
+) -> float:
+    if grace_period_end is None:
+        baseline = idle_baseline
+    else:
+        baseline = max(idle_baseline, grace_period_end)
+    remaining = baseline - now + timeout_period
+    return remaining.total_seconds()
+
+
+class UtilizationExtraInfo(NamedTuple):
+    avg_util: float
+    threshold: float
+
+
+class UtilizationResourceReport(UserDict):
+    __slots__ = ("data",)
+
+    data: dict[str, UtilizationExtraInfo]
+
+    @classmethod
+    def from_avg_threshold(
+        cls,
+        avg_utils: Mapping[str, float],
+        thresholds: Mapping[str, Union[int, float, Decimal, None]],
+        exclusions: set[str],
+    ) -> UtilizationResourceReport:
+        data: dict[str, UtilizationExtraInfo] = {
+            k: UtilizationExtraInfo(float(avg_utils[k]), float(threshold))
+            for k, threshold in thresholds.items()
+            if (threshold is not None) and (k not in exclusions)
+        }
+        return cls(data)
+
+    def to_dict(self, apply_unit: bool = True) -> dict[str, UtilizationExtraInfo]:
+        if apply_unit:
+            return {
+                k: UtilizationExtraInfo(parse_unit(k, v[0]), parse_unit(k, v[1]))
+                for k, v in self.data.items()
+            }
+        return {**self.data}
+
+    @property
+    def utilization_result(self) -> dict[str, bool]:
+        return {k: v.avg_util >= v.threshold for k, v in self.data.items()}
+
 
 class AppStreamingStatus(enum.Enum):
     NO_ACTIVE_CONNECTIONS = 0
     HAS_ACTIVE_CONNECTIONS = 1
 
 
 class ThresholdOperator(enum.Enum):
     AND = "and"
     OR = "or"
 
 
+class RemainingTimeType(str, enum.Enum):
+    GRACE_PERIOD = "grace_period"
+    EXPIRE_AFTER = "expire_after"
+
+
 class IdleCheckerHost:
-    check_interval: ClassVar[float] = 15.0
+    check_interval: ClassVar[float] = DEFAULT_CHECK_INTERVAL
 
     def __init__(
         self,
         db: SAEngine,
         shared_config: SharedConfig,
         event_dispatcher: EventDispatcher,
         event_producer: EventProducer,
@@ -96,29 +175,36 @@
             self._shared_config.data["redis"],
             db=REDIS_LIVE_DB,
         )
         self._redis_stat = redis_helper.get_redis_object(
             self._shared_config.data["redis"],
             db=REDIS_STAT_DB,
         )
+        self._grace_period_checker: NewUserGracePeriodChecker = NewUserGracePeriodChecker(
+            event_dispatcher, self._redis_live, self._redis_stat
+        )
 
     def add_checker(self, checker: BaseIdleChecker):
         if self._frozen:
             raise RuntimeError(
                 "Cannot add a new idle checker after the idle checker host is frozen."
             )
         self._checkers.append(checker)
 
     async def start(self) -> None:
         self._frozen = True
+        raw_config = await self._shared_config.etcd.get_prefix_dict(
+            "config/idle/checkers",
+        )
+        raw_config = cast(Mapping[str, Mapping[str, Any]], raw_config)
+        await self._grace_period_checker.populate_config(
+            raw_config.get(self._grace_period_checker.name) or {}
+        )
         for checker in self._checkers:
-            raw_config = await self._shared_config.etcd.get_prefix_dict(
-                f"config/idle/checkers/{checker.name}",
-            )
-            await checker.populate_config(raw_config or {})
+            await checker.populate_config(raw_config.get(checker.name) or {})
         self.timer = GlobalTimer(
             self._lock_factory(LockID.LOCKID_IDLE_CHECK_TIMER, self.check_interval),
             self._event_producer,
             lambda: DoIdleCheckEvent(),
             self.check_interval,
         )
         self._evh_idle_check = self._event_dispatcher.consume(
@@ -149,67 +235,113 @@
         context: None,
         source: AgentId,
         event: DoIdleCheckEvent,
     ) -> None:
         log.debug("do_idle_check(): triggered")
         policy_cache: dict[AccessKey, Row] = {}
         async with self._db.begin_readonly() as conn:
+            j = sa.join(kernels, users, kernels.c.user_uuid == users.c.uuid)
             query = (
-                sa.select([kernels])
-                .select_from(kernels)
+                sa.select(
+                    [
+                        kernels.c.id,
+                        kernels.c.access_key,
+                        kernels.c.session_id,
+                        kernels.c.session_type,
+                        kernels.c.created_at,
+                        kernels.c.occupied_slots,
+                        kernels.c.cluster_size,
+                        users.c.created_at.label("user_created_at"),
+                    ]
+                )
+                .select_from(j)
                 .where(
                     (kernels.c.status.in_(LIVE_STATUS)) & (kernels.c.cluster_role == DEFAULT_ROLE),
                 )
             )
             result = await conn.execute(query)
             rows = result.fetchall()
-            for session in rows:
-                policy = policy_cache.get(session["access_key"], None)
+            for kernel in rows:
+                grace_period_end = await self._grace_period_checker.get_grace_period_end(kernel)
+                policy = policy_cache.get(kernel["access_key"], None)
                 if policy is None:
                     query = (
-                        sa.select([keypair_resource_policies])
+                        sa.select(
+                            [
+                                keypair_resource_policies.c.max_session_lifetime,
+                                keypair_resource_policies.c.idle_timeout,
+                            ]
+                        )
                         .select_from(
                             sa.join(
                                 keypairs,
                                 keypair_resource_policies,
                                 keypair_resource_policies.c.name == keypairs.c.resource_policy,
                             ),
                         )
-                        .where(keypairs.c.access_key == session["access_key"])
+                        .where(keypairs.c.access_key == kernel["access_key"])
                     )
                     result = await conn.execute(query)
                     policy = result.first()
                     assert policy is not None
-                    policy_cache[session["access_key"]] = policy
-                for checker in self._checkers:
-                    if not (await checker.check_session(session, conn, policy)):
+                    policy_cache[kernel["access_key"]] = policy
+
+                check_task = [
+                    checker.check_idleness(
+                        kernel, conn, policy, self._redis_live, grace_period_end=grace_period_end
+                    )
+                    for checker in self._checkers
+                ]
+                check_results = await asyncio.gather(*check_task, return_exceptions=True)
+                terminated = False
+                errors = []
+                for checker, result in zip(self._checkers, check_results):
+                    if isinstance(result, aiotools.TaskGroupError):
+                        errors.extend(result.__errors__)
+                        continue
+                    elif isinstance(result, Exception):
+                        # mark to be destroyed afterwards
+                        errors.append(result)
+                        continue
+                    if not result:
                         log.info(
                             "The {} idle checker triggered termination of s:{}",
                             checker.name,
-                            session["id"],
-                        )
-                        if isinstance(checker, TimeoutIdleChecker):
-                            terminate_reason = KernelLifecycleEventReason.IDLE_TIMEOUT
-                        elif isinstance(checker, SessionLifetimeChecker):
-                            terminate_reason = KernelLifecycleEventReason.IDLE_SESSION_LIFETIME
-                        elif isinstance(checker, UtilizationIdleChecker):
-                            terminate_reason = KernelLifecycleEventReason.IDLE_UTILIZATION
-                        await self._event_producer.produce_event(
-                            DoTerminateSessionEvent(
-                                session["id"],
-                                terminate_reason,
-                            ),
+                            kernel["session_id"],
                         )
-                        # If any one of checkers decided to terminate the session,
-                        # we can skip over remaining checkers.
-                        break
+                        if not terminated:
+                            terminated = True
+                            await self._event_producer.produce_event(
+                                DoTerminateSessionEvent(
+                                    kernel["session_id"],
+                                    checker.terminate_reason,
+                                ),
+                            )
+                if errors:
+                    raise IdleCheckerError("idle checker(s) raise errors", errors)
+
+    async def get_idle_check_report(
+        self,
+        session_id: SessionId,
+    ) -> dict[str, Any]:
+        return {
+            checker.name: {
+                "remaining": await checker.get_checker_result(self._redis_live, session_id),
+                "remaining_time_type": checker.remaining_time_type.value,
+                "extra": await checker.get_extra_info(session_id),
+            }
+            for checker in self._checkers
+        }
 
 
-class BaseIdleChecker(metaclass=ABCMeta):
+class AbstractIdleCheckReporter(metaclass=ABCMeta):
+    remaining_time_type: RemainingTimeType
     name: ClassVar[str] = "base"
+    report_key: ClassVar[str] = "base"
+    extra_info_key: ClassVar[str] = "base_extra"
 
     def __init__(
         self,
         event_dispatcher: EventDispatcher,
         redis_live: RedisConnectionInfo,
         redis_stat: RedisConnectionInfo,
     ) -> None:
@@ -227,31 +359,152 @@
     async def update_app_streaming_status(
         self,
         session_id: SessionId,
         status: AppStreamingStatus,
     ) -> None:
         pass
 
+    @classmethod
+    def get_report_key(cls, session_id: SessionId) -> str:
+        return f"session.{session_id}.{cls.name}.report"
+
+    @abstractmethod
+    async def get_extra_info(self, session_id: SessionId) -> Optional[dict[str, Any]]:
+        return None
+
+    @abstractmethod
+    async def get_checker_result(
+        self,
+        redis_obj: RedisConnectionInfo,
+        session_id: SessionId,
+    ) -> Optional[float]:
+        """
+        Get check result of the given session.
+        """
+        pass
+
+    async def set_remaining_time_report(
+        self, redis_obj: RedisConnectionInfo, session_id: SessionId, remaining: float
+    ) -> None:
+        await redis_helper.execute(
+            redis_obj,
+            lambda r: r.set(
+                self.get_report_key(session_id),
+                msgpack.packb(remaining),
+                ex=int(DEFAULT_CHECK_INTERVAL) * 10,
+            ),
+        )
+
+
+class AbstractIdleChecker(metaclass=ABCMeta):
+    terminate_reason: KernelLifecycleEventReason
+
     @abstractmethod
-    async def check_session(self, session: Row, dbconn: SAConnection, policy: Row) -> bool:
+    async def check_idleness(
+        self,
+        kernel: Row,
+        dbconn: SAConnection,
+        policy: Row,
+        redis_obj: RedisConnectionInfo,
+        *,
+        grace_period_end: Optional[datetime] = None,
+    ) -> bool:
         """
-        Return True if the session should be kept alive or
-        return False if the session should be terminated.
+        Check the kernel is whether idle or not.
+        And report the result to Redis.
         """
         return True
 
 
-class TimeoutIdleChecker(BaseIdleChecker):
+class NewUserGracePeriodChecker(AbstractIdleCheckReporter):
+    remaining_time_type: RemainingTimeType = RemainingTimeType.GRACE_PERIOD
+    name: ClassVar[str] = "user_grace_period"
+    report_key: ClassVar[str] = "user_grace_period"
+    user_initial_grace_period: Optional[timedelta] = None
+
+    _config_iv = t.Dict(
+        {
+            t.Key("user_initial_grace_period", default=None): t.Null | tx.TimeDuration(),
+        },
+    ).allow_extra("*")
+
+    async def populate_config(self, raw_config: Mapping[str, Any]) -> None:
+        config = self._config_iv.check(raw_config)
+        self.user_initial_grace_period = config["user_initial_grace_period"]
+        _grace_period = (
+            self.user_initial_grace_period.total_seconds()
+            if self.user_initial_grace_period is not None
+            else None
+        )
+
+        log.info(
+            f"NewUserGracePeriodChecker: default period = {_grace_period} seconds",
+        )
+
+    async def get_extra_info(self, session_id: SessionId) -> Optional[dict[str, Any]]:
+        return None
+
+    async def del_remaining_time_report(
+        self, redis_obj: RedisConnectionInfo, session_id: SessionId
+    ) -> None:
+        await redis_helper.execute(
+            redis_obj,
+            lambda r: r.delete(
+                self.get_report_key(session_id),
+            ),
+        )
+
+    async def get_grace_period_end(
+        self,
+        kernel: Row,
+    ) -> Optional[datetime]:
+        """
+        Calculate the user's initial grace period for idle checkers.
+        During the user's initial grace period, the checker does not calculate the time remaining until expiration
+        and does not yield any extra information such as average utilization.
+        """
+        if self.user_initial_grace_period is None:
+            return None
+        user_created_at: datetime = kernel["user_created_at"]
+        return user_created_at + self.user_initial_grace_period
+
+    @property
+    def grace_period_const(self) -> float:
+        return (
+            self.user_initial_grace_period.total_seconds()
+            if self.user_initial_grace_period is not None
+            else 0
+        )
+
+    async def get_checker_result(
+        self,
+        redis_obj: RedisConnectionInfo,
+        session_id: SessionId,
+    ) -> Optional[float]:
+        key = self.get_report_key(session_id)
+        data = await redis_helper.execute(redis_obj, lambda r: r.get(key))
+        return msgpack.unpackb(data) if data is not None else None
+
+
+class BaseIdleChecker(AbstractIdleChecker, AbstractIdleCheckReporter):
+    pass
+
+
+class NetworkTimeoutIdleChecker(BaseIdleChecker):
     """
     Checks the idleness of a session by the elapsed time since last used.
     The usage means processing of any computation requests, such as
     query/batch-mode code execution and having active service-port connections.
     """
 
-    name: ClassVar[str] = "timeout"
+    terminate_reason: KernelLifecycleEventReason = KernelLifecycleEventReason.IDLE_TIMEOUT
+    remaining_time_type: RemainingTimeType = RemainingTimeType.EXPIRE_AFTER
+    name: ClassVar[str] = "network_timeout"
+    report_key: ClassVar[str] = "network_timeout"
+    extra_info_key: ClassVar[str] = "network_timeout_timeout_extra"
 
     _config_iv = t.Dict(
         {
             t.Key("threshold", default="10m"): tx.TimeDuration(),
         },
     ).allow_extra("*")
 
@@ -278,41 +531,41 @@
         for _evh in self._evhandlers:
             self._event_dispatcher.unconsume(_evh)
 
     async def populate_config(self, raw_config: Mapping[str, Any]) -> None:
         config = self._config_iv.check(raw_config)
         self.idle_timeout = config["threshold"]
         log.info(
-            "TimeoutIdleChecker: default idle_timeout = {0:,} seconds",
+            "NetworkTimeoutIdleChecker: default idle_timeout = {0:,} seconds",
             self.idle_timeout.total_seconds(),
         )
 
     async def update_app_streaming_status(
         self,
         session_id: SessionId,
         status: AppStreamingStatus,
     ) -> None:
         if status == AppStreamingStatus.HAS_ACTIVE_CONNECTIONS:
             await self._disable_timeout(session_id)
         elif status == AppStreamingStatus.NO_ACTIVE_CONNECTIONS:
             await self._update_timeout(session_id)
 
     async def _disable_timeout(self, session_id: SessionId) -> None:
-        log.debug(f"TimeoutIdleChecker._disable_timeout({session_id})")
+        log.debug(f"NetworkTimeoutIdleChecker._disable_timeout({session_id})")
         await redis_helper.execute(
             self._redis_live,
             lambda r: r.set(
                 f"session.{session_id}.last_access",
                 "0",
                 xx=True,
             ),
         )
 
     async def _update_timeout(self, session_id: SessionId) -> None:
-        log.debug(f"TimeoutIdleChecker._update_timeout({session_id})")
+        log.debug(f"NetworkTimeoutIdleChecker._update_timeout({session_id})")
         t = await redis_helper.execute(self._redis_live, lambda r: r.time())
         t = t[0] + (t[1] / (10**6))
         await redis_helper.execute(
             self._redis_live,
             lambda r: r.set(
                 f"session.{session_id}.last_access",
                 f"{t:.06f}",
@@ -340,147 +593,285 @@
         self,
         context: None,
         source: AgentId,
         event: ExecutionFinishedEvent | ExecutionTimeoutEvent | ExecutionCancelledEvent,
     ) -> None:
         await self._update_timeout(event.session_id)
 
-    async def check_session(self, session: Row, dbconn: SAConnection, policy: Row) -> bool:
-        session_id = session["id"]
-        if session["session_type"] == SessionTypes.BATCH:
+    async def get_extra_info(self, session_id: SessionId) -> Optional[dict[str, Any]]:
+        return None
+
+    async def check_idleness(
+        self,
+        kernel: Row,
+        dbconn: SAConnection,
+        policy: Row,
+        redis_obj: RedisConnectionInfo,
+        *,
+        grace_period_end: Optional[datetime] = None,
+    ) -> bool:
+        """
+        Check the kernel is timeout or not.
+        And save remaining time until timeout of kernel to Redis.
+        """
+        session_id = kernel["session_id"]
+
+        if kernel["session_type"] == SessionTypes.BATCH:
             return True
+
         active_streams = await redis_helper.execute(
             self._redis_live,
             lambda r: r.zcount(
                 f"session.{session_id}.active_app_connections",
                 float("-inf"),
                 float("+inf"),
             ),
         )
         if active_streams is not None and active_streams > 0:
             return True
         t = await redis_helper.execute(self._redis_live, lambda r: r.time())
-        t = t[0] + (t[1] / (10**6))
+        now: float = t[0] + (t[1] / (10**6))
         raw_last_access = await redis_helper.execute(
             self._redis_live,
             lambda r: r.get(f"session.{session_id}.last_access"),
         )
         if raw_last_access is None or raw_last_access == "0":
             return True
         last_access = float(raw_last_access)
         # serves as the default fallback if keypair resource policy's idle_timeout is "undefined"
-        idle_timeout = self.idle_timeout.total_seconds()
+        idle_timeout: float = self.idle_timeout.total_seconds()
         # setting idle_timeout:
         # - zero/inf means "infinite"
         # - negative means "undefined"
         if policy["idle_timeout"] >= 0:
             idle_timeout = float(policy["idle_timeout"])
-        if (
-            (idle_timeout <= 0)
-            or (math.isinf(idle_timeout) and idle_timeout > 0)
-            or (t - last_access <= idle_timeout)
-        ):
+        if (idle_timeout <= 0) or (math.isinf(idle_timeout) and idle_timeout > 0):
             return True
-        return False
+        tz = grace_period_end.tzinfo if grace_period_end is not None else None
+        remaining = calculate_remaining_time(
+            datetime.fromtimestamp(now, tz=tz),
+            datetime.fromtimestamp(last_access, tz=tz),
+            timedelta(seconds=idle_timeout),
+            grace_period_end,
+        )
+        await self.set_remaining_time_report(
+            redis_obj, session_id, remaining if remaining > 0 else IDLE_TIMEOUT_VALUE
+        )
+        return remaining >= 0
+
+    async def get_checker_result(
+        self,
+        redis_obj: RedisConnectionInfo,
+        session_id: SessionId,
+    ) -> Optional[float]:
+        key = self.get_report_key(session_id)
+        data = await redis_helper.execute(redis_obj, lambda r: r.get(key))
+        return msgpack.unpackb(data) if data is not None else None
 
 
 class SessionLifetimeChecker(BaseIdleChecker):
+    terminate_reason: KernelLifecycleEventReason = KernelLifecycleEventReason.IDLE_SESSION_LIFETIME
+    remaining_time_type: RemainingTimeType = RemainingTimeType.EXPIRE_AFTER
     name: ClassVar[str] = "session_lifetime"
+    report_key: ClassVar[str] = "session_lifetime"
+    extra_info_key: ClassVar[str] = "session_lifetime_extra"
 
-    async def populate_config(self, config: Mapping[str, Any]) -> None:
+    async def populate_config(self, raw_config: Mapping[str, Any]) -> None:
         pass
 
-    async def check_session(self, session: Row, dbconn: SAConnection, policy: Row) -> bool:
-        now = await dbconn.scalar(sa.select(sa.func.now()))
-        if policy["max_session_lifetime"] > 0:
+    async def get_extra_info(self, session_id: SessionId) -> Optional[dict[str, Any]]:
+        return None
+
+    async def check_idleness(
+        self,
+        kernel: Row,
+        dbconn: SAConnection,
+        policy: Row,
+        redis_obj: RedisConnectionInfo,
+        *,
+        grace_period_end: Optional[datetime] = None,
+    ) -> bool:
+        """
+        Check the kernel has been living longer than resource policy's `max_session_lifetime`.
+        And save remaining time until `max_session_lifetime` of kernel to Redis.
+        """
+
+        session_id = kernel["session_id"]
+        if (max_session_lifetime := policy["max_session_lifetime"]) > 0:
             # TODO: once per-status time tracking is implemented, let's change created_at
             #       to the timestamp when the session entered PREPARING status.
-            if now - session["created_at"] >= timedelta(seconds=policy["max_session_lifetime"]):
-                return False
+            idle_timeout = timedelta(seconds=max_session_lifetime)
+            now: datetime = await dbconn.scalar(sa.select(sa.func.now()))
+            kernel_created_at: datetime = kernel["created_at"]
+            remaining = calculate_remaining_time(
+                now, kernel_created_at, idle_timeout, grace_period_end
+            )
+            await self.set_remaining_time_report(
+                redis_obj, session_id, remaining if remaining > 0 else IDLE_TIMEOUT_VALUE
+            )
+            return remaining > 0
         return True
 
+    async def get_checker_result(
+        self,
+        redis_obj: RedisConnectionInfo,
+        session_id: SessionId,
+    ) -> Optional[float]:
+        key = self.get_report_key(session_id)
+        data = await redis_helper.execute(redis_obj, lambda r: r.get(key))
+        return msgpack.unpackb(data) if data is not None else None
+
 
 class UtilizationIdleChecker(BaseIdleChecker):
     """
     Checks the idleness of a session by the average utilization of compute devices.
     """
 
+    terminate_reason: KernelLifecycleEventReason = KernelLifecycleEventReason.IDLE_UTILIZATION
+    remaining_time_type: RemainingTimeType = RemainingTimeType.GRACE_PERIOD
     name: ClassVar[str] = "utilization"
+    report_key: ClassVar[str] = "utilization"
+    extra_info_key: ClassVar[str] = "utilization_extra"
 
     _config_iv = t.Dict(
         {
             t.Key("time-window", default="10m"): tx.TimeDuration(),
             t.Key("initial-grace-period", default="5m"): tx.TimeDuration(),
             t.Key("thresholds-check-operator", default=ThresholdOperator.AND): tx.Enum(
                 ThresholdOperator
             ),
-            t.Key("resource-thresholds"): t.Dict(
+            t.Key("resource-thresholds", default=None): t.Null | t.Dict(
                 {
                     t.Key("cpu_util", default=None): t.Null | t.Dict({t.Key("average"): t.Float}),
                     t.Key("mem", default=None): t.Null | t.Dict({t.Key("average"): t.Float}),
                     t.Key("cuda_util", default=None): t.Null | t.Dict({t.Key("average"): t.Float}),
                     t.Key("cuda_mem", default=None): t.Null | t.Dict({t.Key("average"): t.Float}),
+                    t.Key("atom_mem", default=None): t.Null | t.Dict({t.Key("average"): t.Float}),
                 },
             ),
         },
     ).allow_extra("*")
 
-    resource_thresholds: MutableMapping[str, Union[int, float, Decimal]]
-    thresholds_check_operator: str
+    resource_thresholds: MutableMapping[str, Union[int, float, Decimal, None]]
+    thresholds_check_operator: ThresholdOperator
     time_window: timedelta
     initial_grace_period: timedelta
     _evhandlers: List[EventHandler[None, AbstractEvent]]
     slot_resource_map: Mapping[str, Set[str]] = {
         "cpu": {"cpu_util"},
         "mem": {"mem"},
         "cuda": {"cuda_util", "cuda_mem"},
+        "atom": {"atom_mem"},
     }
 
     async def populate_config(self, raw_config: Mapping[str, Any]) -> None:
         config = self._config_iv.check(raw_config)
-        self.resource_thresholds = {
-            k: nmget(v, "average") for k, v in config.get("resource-thresholds").items()
-        }
-        self.thresholds_check_operator = config.get("thresholds-check-operator")
+        raw_resource_thresholds = config.get("resource-thresholds")
+        if raw_resource_thresholds is not None:
+            self.resource_thresholds = {
+                k: nmget(v, "average") for k, v in raw_resource_thresholds.items()
+            }
+        else:
+            resources: list[str] = []
+            for r in self.slot_resource_map.values():
+                resources = [*resources, *r]
+            self.resource_thresholds = {r: None for r in resources}
+        self.thresholds_check_operator: ThresholdOperator = config.get("thresholds-check-operator")
         self.time_window = config.get("time-window")
         self.initial_grace_period = config.get("initial-grace-period")
 
         thresholds_log = " ".join(
             [f"{k}({threshold})," for k, threshold in self.resource_thresholds.items()]
         )
         log.info(
             f"UtilizationIdleChecker(%): {thresholds_log} "
             f'thresholds-check-operator("{self.thresholds_check_operator}"), '
-            f"time-window({self.time_window.total_seconds()}s)",
+            f"time-window({self.time_window.total_seconds()}s)"
         )
 
-    async def check_session(self, session: Row, dbconn: SAConnection, policy: Row) -> bool:
-        session_id = session["id"]
+    def get_extra_info_key(self, session_id: SessionId) -> str:
+        return f"session.{session_id}.{self.extra_info_key}"
+
+    async def get_extra_info(self, session_id: SessionId) -> Optional[dict[str, Any]]:
+        data = await redis_helper.execute(
+            self._redis_live,
+            lambda r: r.get(
+                self.get_extra_info_key(session_id),
+            ),
+        )
+        return msgpack.unpackb(data) if data is not None else None
+
+    def get_time_window(self, policy: Row) -> timedelta:
+        # Respect idle_timeout, from keypair resource policy, over time_window.
+        if (idle_timeout := policy["idle_timeout"]) >= 0:
+            return timedelta(seconds=idle_timeout)
+        return self.time_window
+
+    def get_last_collected_key(self, session_id: SessionId) -> str:
+        return f"session.{session_id}.util_last_collected"
+
+    async def check_idleness(
+        self,
+        kernel: Row,
+        dbconn: SAConnection,
+        policy: Row,
+        redis_obj: RedisConnectionInfo,
+        *,
+        grace_period_end: Optional[datetime] = None,
+    ) -> bool:
+        """
+        Check the the average utilization of kernel and whether it exceeds the threshold or not.
+        And save the average utilization of kernel to Redis.
+        """
+        session_id = kernel["session_id"]
+
         interval = IdleCheckerHost.check_interval
-        window_size = int(self.time_window.total_seconds() / interval)
-        occupied_slots = session["occupied_slots"]
+        # time_window: Utilization is calculated within this window.
+        time_window: timedelta = self.get_time_window(policy)
+        occupied_slots = kernel["occupied_slots"]
         unavailable_resources: Set[str] = set()
 
         util_series_key = f"session.{session_id}.util_series"
-        util_last_collected_key = f"session.{session_id}.util_last_collected"
+        util_last_collected_key = self.get_last_collected_key(session_id)
+
+        # window_size: the length of utilization reports.
+        window_size = int(time_window.total_seconds() / interval)
+        if (window_size <= 0) or (math.isinf(window_size) and window_size > 0):
+            return True
 
         # Wait until the time "interval" is passed after the last udpated time.
         t = await redis_helper.execute(self._redis_live, lambda r: r.time())
-        t = t[0] + (t[1] / (10**6))
+        util_now: float = t[0] + (t[1] / (10**6))
         raw_util_last_collected = await redis_helper.execute(
             self._redis_live,
             lambda r: r.get(util_last_collected_key),
         )
-        util_last_collected = float(raw_util_last_collected) if raw_util_last_collected else 0
-        if t - util_last_collected < interval:
+        util_last_collected: float = (
+            float(raw_util_last_collected) if raw_util_last_collected else 0.0
+        )
+        if util_now - util_last_collected < interval:
             return True
 
-        # Respect initial grace period (no termination of the session)
-        now = datetime.now(tzutc())
-        if now - session["created_at"] <= self.initial_grace_period:
+        # Report time remaining until the first time window is full as expire time
+        db_now: datetime = await dbconn.scalar(sa.select(sa.func.now()))
+        kernel_created_at: datetime = kernel["created_at"]
+        if grace_period_end is not None:
+            start_from = max(grace_period_end, kernel_created_at)
+        else:
+            start_from = kernel_created_at
+        total_initial_grace_period_end = start_from + self.initial_grace_period
+        remaining = calculate_remaining_time(
+            db_now, kernel_created_at, time_window, total_initial_grace_period_end
+        )
+        await self.set_remaining_time_report(
+            redis_obj, session_id, remaining if remaining > 0 else IDLE_TIMEOUT_VALUE
+        )
+
+        # Respect initial grace period (no calculation of utilization and no termination of the session)
+        if db_now <= total_initial_grace_period_end:
             return True
 
         # Merge same type of (exclusive) resources as a unique resource with the values added.
         # Example: {cuda.device: 0, cuda.shares: 0.5} -> {cuda: 0.5}.
         unique_res_map: DefaultDict[str, Any] = defaultdict(Decimal)
         for k, v in occupied_slots.items():
             unique_key = k.split(".")[0]
@@ -488,49 +879,39 @@
 
         # Do not take into account unallocated resources. For example, do not garbage collect
         # a session without GPU even if cuda_util is configured in resource-thresholds.
         for slot in unique_res_map:
             if unique_res_map[slot] == 0:
                 unavailable_resources.update(self.slot_resource_map[slot])
 
-        # Respect idle_timeout, from keypair resource policy, over time_window.
-        if policy["idle_timeout"] >= 0:
-            window_size = int(float(policy["idle_timeout"]) / interval)
-        if (window_size <= 0) or (math.isinf(window_size) and window_size > 0):
-            return True
-
         # Get current utilization data from all containers of the session.
-        if session["cluster_size"] > 1:
-            query = (
-                sa.select([kernels.c.id])
-                .select_from(kernels)
-                .where(
-                    (kernels.c.session_id == session_id) & (kernels.c.status.in_(LIVE_STATUS)),
-                )
+        if kernel["cluster_size"] > 1:
+            query = sa.select([kernels.c.id]).where(
+                (kernels.c.session_id == session_id) & (kernels.c.status.in_(LIVE_STATUS)),
             )
-            result = await dbconn.execute(query)
-            rows = result.fetchall()
+            rows = (await dbconn.execute(query)).fetchall()
             kernel_ids = [k["id"] for k in rows]
         else:
-            kernel_ids = [session_id]
+            kernel_ids = [kernel["id"]]
         current_utilizations = await self.get_current_utilization(kernel_ids, occupied_slots)
         if current_utilizations is None:
             return True
 
         # Update utilization time-series data.
-        not_enough_data = False
         raw_util_series = await redis_helper.execute(
             self._redis_live, lambda r: r.get(util_series_key)
         )
 
         try:
-            util_series = msgpack.unpackb(raw_util_series, use_list=True)
+            util_series: dict[str, list[float]] = msgpack.unpackb(raw_util_series, use_list=True)
         except TypeError:
             util_series = {k: [] for k in self.resource_thresholds.keys()}
 
+        not_enough_data = False
+
         for k in util_series:
             util_series[k].append(current_utilizations[k])
             if len(util_series[k]) > window_size:
                 util_series[k].pop(0)
             else:
                 not_enough_data = True
         await redis_helper.execute(
@@ -541,30 +922,49 @@
                 ex=max(86400, int(self.time_window.total_seconds() * 2)),
             ),
         )
         await redis_helper.execute(
             self._redis_live,
             lambda r: r.set(
                 util_last_collected_key,
-                f"{t:.06f}",
+                f"{util_now:.06f}",
                 ex=max(86400, int(self.time_window.total_seconds() * 2)),
             ),
         )
 
+        def _avg(util_list: list[float]) -> float:
+            try:
+                return sum(util_list) / len(util_list)
+            except ZeroDivisionError:
+                return 0.0
+
+        avg_utils: Mapping[str, float] = {k: _avg(v) for k, v in util_series.items()}
+
+        util_avg_thresholds = UtilizationResourceReport.from_avg_threshold(
+            avg_utils, self.resource_thresholds, unavailable_resources
+        )
+        report = {
+            "thresholds_check_operator": self.thresholds_check_operator.value,
+            "resources": util_avg_thresholds.to_dict(),
+        }
+        await redis_helper.execute(
+            self._redis_live,
+            lambda r: r.set(
+                self.get_extra_info_key(session_id),
+                msgpack.packb(report),
+                ex=int(DEFAULT_CHECK_INTERVAL) * 10,
+            ),
+        )
+
         if not_enough_data:
             return True
 
         # Check over-utilized (not to be collected) resources.
-        avg_utils = {k: sum(v) / len(v) for k, v in util_series.items()}
-        sufficiently_utilized = {
-            k: (float(avg_utils[k]) >= float(threshold))
-            for k, threshold in self.resource_thresholds.items()
-            if (threshold is not None) and (k not in unavailable_resources)
-        }
-
+        sufficiently_utilized = util_avg_thresholds.utilization_result
+        check_result = True
         if len(sufficiently_utilized) < 1:
             check_result = True
         elif self.thresholds_check_operator == ThresholdOperator.OR:
             check_result = all(sufficiently_utilized.values())
         else:  # "and" operation is the default
             check_result = any(sufficiently_utilized.values())
         if not check_result:
@@ -615,17 +1015,26 @@
             mem_current = float(nmget(live_stat, "mem.current", 0.0))
             utilizations["mem"] = mem_current / mem_slots * 100 if mem_slots > 0 else 0
             return utilizations
         except Exception as e:
             log.warning("Unable to collect utilization for idleness check", exc_info=e)
             return None
 
+    async def get_checker_result(
+        self,
+        redis_obj: RedisConnectionInfo,
+        session_id: SessionId,
+    ) -> Optional[float]:
+        key = self.get_report_key(session_id)
+        data = await redis_helper.execute(redis_obj, lambda r: r.get(key))
+        return msgpack.unpackb(data) if data is not None else None
+
 
 checker_registry: Mapping[str, Type[BaseIdleChecker]] = {
-    TimeoutIdleChecker.name: TimeoutIdleChecker,
+    NetworkTimeoutIdleChecker.name: NetworkTimeoutIdleChecker,
     UtilizationIdleChecker.name: UtilizationIdleChecker,
 }
 
 
 async def init_idle_checkers(
     db: SAEngine,
     shared_config: SharedConfig,
@@ -634,22 +1043,27 @@
     lock_factory: DistributedLockFactory,
 ) -> IdleCheckerHost:
     """
     Create an instance of session idleness checker
     from the given configuration and using the given event dispatcher.
     """
     checker_host = IdleCheckerHost(
-        db, shared_config, event_dispatcher, event_producer, lock_factory
+        db,
+        shared_config,
+        event_dispatcher,
+        event_producer,
+        lock_factory,
     )
     checker_init_args = (event_dispatcher, checker_host._redis_live, checker_host._redis_stat)
-    log.info("Initializing idle checker: session_lifetime")
+    log.info("Initializing idle checker: user_initial_grace_period, session_lifetime")
     checker_host.add_checker(SessionLifetimeChecker(*checker_init_args))  # enabled by default
     enabled_checkers = await shared_config.etcd.get("config/idle/enabled")
     if enabled_checkers:
         for checker_name in enabled_checkers.split(","):
+            checker_name = checker_name.strip()
             checker_cls = checker_registry.get(checker_name, None)
             if checker_cls is None:
                 log.warning("ignoring an unknown idle checker name: {}", checker_name)
                 continue
             log.info("Initializing idle checker: {}", checker_name)
             checker_instance = checker_cls(*checker_init_args)
             checker_host.add_checker(checker_instance)
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/__init__.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/acl.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/agent.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         server_default="default",
         default="default",
     ),
     sa.Column("schedulable", sa.Boolean(), nullable=False, server_default=true(), default=True),
     sa.Column("available_slots", ResourceSlotColumn(), nullable=False),
     sa.Column("occupied_slots", ResourceSlotColumn(), nullable=False),
     sa.Column("addr", sa.String(length=128), nullable=False),
+    sa.Column("public_host", sa.String(length=256), nullable=True),
     sa.Column("first_contact", sa.DateTime(timezone=True), server_default=sa.func.now()),
     sa.Column("lost_at", sa.DateTime(timezone=True), nullable=True),
     sa.Column("version", sa.String(length=64), nullable=False),
     sa.Column("architecture", sa.String(length=32), nullable=False),
     sa.Column("compute_plugins", pgsql.JSONB(), nullable=False, default={}),
 )
 
@@ -257,22 +258,26 @@
 
     @classmethod
     async def load_count(
         cls,
         graph_ctx: GraphQueryContext,
         *,
         scaling_group: str = None,
-        raw_status: str = None,
+        raw_status: Optional[str | AgentStatus] = None,
         filter: str = None,
     ) -> int:
+        if isinstance(raw_status, str):
+            status_list = [AgentStatus[s] for s in raw_status.split(",")]
+        elif isinstance(raw_status, AgentStatus):
+            status_list = [raw_status]
         query = sa.select([sa.func.count()]).select_from(agents)
         if scaling_group is not None:
             query = query.where(agents.c.scaling_group == scaling_group)
         if raw_status is not None:
-            query = query.where(agents.c.status == AgentStatus[raw_status])
+            query = query.where(agents.c.status.in_(status_list))
         if filter is not None:
             qfparser = QueryFilterParser(cls._queryfilter_fieldspec)
             query = qfparser.append_filter(query, filter)
         async with graph_ctx.db.begin_readonly() as conn:
             result = await conn.execute(query)
             return result.scalar()
 
@@ -284,19 +289,23 @@
         offset: int,
         *,
         scaling_group: str = None,
         raw_status: str = None,
         filter: str = None,
         order: str = None,
     ) -> Sequence[Agent]:
+        if isinstance(raw_status, str):
+            status_list = [AgentStatus[s] for s in raw_status.split(",")]
+        elif isinstance(raw_status, AgentStatus):
+            status_list = [raw_status]
         query = sa.select([agents]).select_from(agents).limit(limit).offset(offset)
         if scaling_group is not None:
             query = query.where(agents.c.scaling_group == scaling_group)
         if raw_status is not None:
-            query = query.where(agents.c.status == AgentStatus[raw_status])
+            query = query.where(agents.c.status.in_(status_list))
         if filter is not None:
             qfparser = QueryFilterParser(cls._queryfilter_fieldspec)
             query = qfparser.append_filter(query, filter)
         if order is not None:
             qoparser = QueryOrderParser(cls._queryorder_colmap)
             query = qoparser.append_ordering(query, order)
         else:
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/env.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,19 +33,17 @@
         "groups",
         sa.Column("total_resource_slots", postgresql.JSONB(astext_type=sa.Text()), nullable=True),
     )
     op.add_column("users", sa.Column("integration_id", sa.String(length=512), nullable=True))
     # ### end Alembic commandk ###
 
     print("\nSet group's total_resource_slots with empty dictionary.")
-    query = textwrap.dedent(
-        """\
+    query = textwrap.dedent("""\
         UPDATE groups SET total_resource_slots = '{}'::jsonb;
-    """
-    )
+    """)
     connection = op.get_bind()
     connection.execute(text(query))
 
 
 def downgrade():
     # ### commands auto generated by Alembic - please adjust! ###
     op.drop_column("users", "integration_id")
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,15 @@
         new_enum_val kernelstatus, old_enum_val kernelstatus_old
     )
         RETURNS boolean AS $$
             SELECT new_enum_val::text <> old_enum_val::text;
         $$ LANGUAGE SQL IMMUTABLE;
     """
     conn.execute(text(query))
-    queries = textwrap.dedent(
-        """
+    queries = textwrap.dedent("""
     CREATE OPERATOR <> (
         leftarg = kernelstatus,
         rightarg = kernelstatus_old,
         procedure = kernelstatus_new_old_compare
     );
 
     ALTER TABLE kernels
@@ -84,16 +83,15 @@
         ALTER COLUMN "status" SET DEFAULT 'PENDING'::kernelstatus;
 
     DROP FUNCTION kernelstatus_new_old_compare(
         new_enum_val kernelstatus, old_enum_val kernelstatus_old
     ) CASCADE;
 
     DROP TYPE kernelstatus_old;
-    """
-    )
+    """)
     for query in queries.split(";"):
         if len(query.strip()) == 0:
             continue
         conn.execute(text(query))
 
     op.add_column("agents", sa.Column("status_changed", sa.DateTime(timezone=True), nullable=True))
 
@@ -144,27 +142,24 @@
     op.create_index(op.f("ix_kernels_type"), "kernels", ["type"], unique=False)
 
 
 def downgrade():
     conn = op.get_bind()
     conn.execute(text("ALTER TYPE kernelstatus RENAME TO kernelstatus_new;"))
     kernelstatus_old.create(conn)
-    query = textwrap.dedent(
-        """
+    query = textwrap.dedent("""
         CREATE FUNCTION kernelstatus_new_old_compare(
             old_enum_val kernelstatus, new_enum_val kernelstatus_new
         )
             RETURNS boolean AS $$
                 SELECT old_enum_val::text <> new_enum_val::text;
             $$ LANGUAGE SQL IMMUTABLE;
-    """
-    )
+    """)
     conn.execute(text(query))
-    queries = textwrap.dedent(
-        """\
+    queries = textwrap.dedent("""\
         CREATE OPERATOR <> (
             leftarg = kernelstatus,
             rightarg = kernelstatus_new,
             procedure = kernelstatus_new_old_compare
         );
 
         ALTER TABLE kernels
@@ -179,16 +174,15 @@
             ALTER COLUMN "status" SET DEFAULT 'PREPARING'::kernelstatus;
 
         DROP FUNCTION kernelstatus_new_old_compare(
             old_enum_val kernelstatus, new_enum_val kernelstatus_new
         ) CASCADE;
 
         DROP TYPE kernelstatus_new;
-    """
-    )
+    """)
     for query in queries.split(";"):
         if len(query.strip()) == 0:
             continue
         conn.execute(text(query))
 
     # op.drop_index(op.f("ix_kernels_type"), table_name="kernels")
     op.drop_index(op.f("ix_kernels_result"), table_name="kernels")
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,22 +51,20 @@
 
 
 def upgrade():
     conn = op.get_bind()
     conn.execute(text("DROP INDEX IF EXISTS ix_kernels_unique_sess_token;"))
     conn.execute(text("ALTER TYPE kernelstatus RENAME TO kernelstatus_old;"))
     kernelstatus_new.create(conn)
-    query = textwrap.dedent(
-        """
+    query = textwrap.dedent("""
     ALTER TABLE kernels
         ALTER COLUMN "status" DROP DEFAULT,
         ALTER COLUMN "status" TYPE kernelstatus USING "status"::text::kernelstatus,
         ALTER COLUMN "status" SET DEFAULT 'PENDING'::kernelstatus;
-    """
-    )
+    """)
     conn.execute(text(query))
     query = "DROP TYPE kernelstatus_old;"
     conn.execute(text(query))
     op.create_index(
         "ix_kernels_unique_sess_token",
         "kernels",
         ["access_key", "sess_id"],
@@ -76,31 +74,25 @@
 
 
 def downgrade():
     op.drop_index("ix_kernels_unique_sess_token", table_name="kernels")
     conn = op.get_bind()
     conn.execute(text("ALTER TYPE kernelstatus RENAME TO kernelstatus_new;"))
     kernelstatus_old.create(conn)
-    conn.execute(
-        text(
-            textwrap.dedent(
-                """\
+    conn.execute(text(textwrap.dedent("""\
             ALTER TABLE kernels
                 ALTER COLUMN "status" DROP DEFAULT,
                 ALTER COLUMN "status" TYPE kernelstatus USING (
                     CASE "status"::text
                         WHEN 'CANCELLED' THEN 'TERMINATED'
                         ELSE "status"::text
                     END
                 )::kernelstatus,
                 ALTER COLUMN "status" SET DEFAULT 'PREPARING'::kernelstatus;
-            """
-            )
-        )
-    )
+            """)))
     conn.execute(text("DROP TYPE kernelstatus_new;"))
     op.create_index(
         "ix_kernels_unique_sess_token",
         "kernels",
         ["access_key", "sess_id"],
         unique=True,
         postgresql_where=sa.text("status != 'TERMINATED' and role = 'master'"),
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,16 +109,18 @@
     # Create indexes for name.
     op.create_index(op.f("ix_vfolders_name"), "vfolders", ["name"], unique=False)
 
     # Constraints
     op.create_check_constraint(
         "ownership_type_match_with_user_or_group",
         "vfolders",
-        "(ownership_type = 'user' AND \"user\" IS NOT NULL) OR "
-        "(ownership_type = 'group' AND \"group\" IS NOT NULL)",
+        (
+            "(ownership_type = 'user' AND \"user\" IS NOT NULL) OR "
+            "(ownership_type = 'group' AND \"group\" IS NOT NULL)"
+        ),
     )
     op.create_check_constraint(
         "either_one_of_user_or_group",
         "vfolders",
         '("user" IS NULL AND "group" IS NOT NULL) OR ("user" IS NOT NULL AND "group" IS NULL)',
     )
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     )
     op.create_index(
         "ix_kernels_unique_sess_token",
         "kernels",
         ["access_key", "session_id"],
         unique=True,
         postgresql_where=sa.text(
-            "status NOT IN ('TERMINATED', 'CANCELLED') " "and cluster_role = 'main'"
+            "status NOT IN ('TERMINATED', 'CANCELLED') and cluster_role = 'main'"
         ),
     )
 
 
 def downgrade():
     op.drop_index("ix_kernels_unique_sess_token", table_name="kernels")
     op.drop_index("ix_kernels_sess_id_role", table_name="kernels")
@@ -64,10 +64,10 @@
     op.drop_column("kernels", "cluster_hostname")
 
     op.create_index(
         "ix_kernels_unique_sess_token",
         "kernels",
         ["access_key", "session_name"],
         unique=True,
-        postgresql_where=sa.text("status NOT IN ('TERMINATED', 'CANCELLED') " "and role = 'main'"),
+        postgresql_where=sa.text("status NOT IN ('TERMINATED', 'CANCELLED') and role = 'main'"),
     )
     op.create_index("ix_kernels_sess_id_role", "kernels", ["session_name", "role"], unique=False)
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,26 +53,20 @@
 
 
 def upgrade():
     conn = op.get_bind()
     conn.execute(text("DROP INDEX IF EXISTS ix_kernels_unique_sess_token;"))
     conn.execute(text("ALTER TYPE kernelstatus RENAME TO kernelstatus_old;"))
     kernelstatus_new.create(conn)
-    conn.execute(
-        text(
-            textwrap.dedent(
-                """\
+    conn.execute(text(textwrap.dedent("""\
             ALTER TABLE kernels
                 ALTER COLUMN "status" DROP DEFAULT,
                 ALTER COLUMN "status" TYPE kernelstatus USING "status"::text::kernelstatus,
                 ALTER COLUMN "status" SET DEFAULT 'PENDING'::kernelstatus;
-            """
-            )
-        )
-    )
+            """)))
     conn.execute(text("DROP TYPE kernelstatus_old;"))
     # This also fixes the unique constraint columns:
     #   (access_key, session_id) -> (access_key, session_name)
     op.create_index(
         "ix_kernels_unique_sess_token",
         "kernels",
         ["access_key", "session_name"],
@@ -84,31 +78,25 @@
 
 
 def downgrade():
     op.drop_index("ix_kernels_unique_sess_token", table_name="kernels")
     conn = op.get_bind()
     conn.execute(text("ALTER TYPE kernelstatus RENAME TO kernelstatus_new;"))
     kernelstatus_old.create(conn)
-    conn.execute(
-        text(
-            textwrap.dedent(
-                """\
+    conn.execute(text(textwrap.dedent("""\
             ALTER TABLE kernels
                 ALTER COLUMN "status" DROP DEFAULT,
                 ALTER COLUMN "status" TYPE kernelstatus USING (
                     CASE "status"::text
                         WHEN 'SCHEDULED' THEN 'PREPARING'
                         ELSE "status"::text
                     END
                 )::kernelstatus,
                 ALTER COLUMN "status" SET DEFAULT 'PENDING'::kernelstatus;
-            """
-            )
-        )
-    )
+            """)))
     conn.execute(text("DROP TYPE kernelstatus_new;"))
     op.create_index(
         "ix_kernels_unique_sess_token",
         "kernels",
         ["access_key", "session_id"],
         unique=True,
         postgresql_where=sa.text("status != 'TERMINATED' and cluster_role = 'main'"),
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,63 +22,40 @@
 
 # select enum_range(null::sessiontypes);
 typename = SessionTypes.__name__.lower()
 
 
 def upgrade():
     op.execute(text("ALTER TYPE {} ADD VALUE IF NOT EXISTS 'INFERENCE';".format(typename)))
-    op.execute(
-        text(
-            textwrap.dedent(
-                """\
+    op.execute(text(textwrap.dedent("""\
                 ALTER TABLE sessions ALTER COLUMN session_type TYPE {} USING session_type::text::sessiontypes;
-            """.format(
-                    typename
-                )
-            )
-        )
-    )
+            """.format(typename))))
 
 
 def downgrade():
     conn = op.get_bind()
     conn.execute(
         text(
-            "UPDATE sessions SET session_type = 'INTERACTIVE'::{x} WHERE session_type = 'INFERENCE'::{x};".format(
-                x=typename
-            )
+            "UPDATE sessions SET session_type = 'INTERACTIVE'::{x} WHERE session_type ="
+            " 'INFERENCE'::{x};".format(x=typename)
         )
     )
 
-    cursor = conn.execute(
-        text(
-            textwrap.dedent(
-                """\
+    cursor = conn.execute(text(textwrap.dedent("""\
                 SELECT t.typname, e.enumlabel, e.enumsortorder, e.enumtypid
                 FROM pg_type t
                 JOIN pg_enum e ON e.enumtypid = t.oid
                 WHERE t.typtype = 'e'
                 AND e.enumlabel = 'INFERENCE'
                 ORDER BY 1, enumsortorder;
-            """
-            )
-        )
-    )
+            """)))
 
     if (row := next(cursor, None)) is None:
         return
 
     typname, enumlabel, enumsortorder, enumtypid = row
 
-    conn.execute(
-        text(
-            textwrap.dedent(
-                """\
+    conn.execute(text(textwrap.dedent("""\
                 DELETE FROM pg_enum
                 WHERE enumtypid = {enumtypid}
                 AND enumlabel = 'INFERENCE';
-            """.format(
-                    enumtypid=enumtypid
-                )
-            )
-        )
-    )
+            """.format(enumtypid=enumtypid))))
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 
 def upgrade():
     op.create_index(
         op.f("ix_kernels_unique_sess_token"),
         "kernels",
         ["access_key", "sess_id"],
         unique=True,
-        postgresql_where=sa.text("kernels.status != 'TERMINATED' and " "kernels.role = 'master'"),
+        postgresql_where=sa.text("kernels.status != 'TERMINATED' and kernels.role = 'master'"),
     )
 
 
 def downgrade():
     # op.drop_index(op.f("ix_kernels_unique_sess_token"), table_name="kernels")
     pass
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,19 +62,17 @@
     connection = op.get_bind()
     query = sa.select([domains]).select_from(domains).where(domains.c.name == "default")
     results = connection.execute(query).first()
     if results is None:
         query = sa.insert(domains).values(
             name="default", description="Default domain", is_active=True, total_resource_slots="{}"
         )
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             INSERT INTO domains (name, description, is_active, total_resource_slots)
-            VALUES ('default', 'Default domain', True, '{}'::jsonb);"""
-        )
+            VALUES ('default', 'Default domain', True, '{}'::jsonb);""")
         connection.execute(text(query))
 
     # Fill in users' domain_name field.
     query = "UPDATE users SET domain_name = 'default' WHERE email != 'admin@lablup.com';"
     connection.execute(text(query))
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,30 +72,26 @@
 
     # Create default group in the default domain.
     # Assumption: "default" domain must exist
     connection = op.get_bind()
     query = sa.insert(groups).values(
         name="default", description="Default group", is_active=True, domain_name="default"
     )
-    query = textwrap.dedent(
-        """\
+    query = textwrap.dedent("""\
         INSERT INTO groups (name, description, is_active, domain_name)
         VALUES ('default', 'Default group', True, 'default')
         ON CONFLICT (name, domain_name) DO NOTHING
         RETURNING id;
-    """
-    )
+    """)
     result = connection.execute(text(query)).first()
     gid = result.id if hasattr(result, "id") else None
     if gid is None:  # group already exists
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             SELECT id FROM groups where name = 'default' and domain_name = 'default';
-        """
-        )
+        """)
         gid = connection.execute(text(query)).first().id
 
     # Fill in kernels' domain_name, group_id, and user_uuid.
     query = sa.select([kernels.c.id, kernels.c.access_key]).select_from(kernels)
     all_kernels = connection.execute(query).fetchall()
     for kernel in all_kernels:
         # Get kernel's keypair (access_key).
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,43 +29,35 @@
     assert "superadmin" in userrole_choices, "superadmin in UserRole is required!"
 
     conn = op.get_bind()
     conn.execute(text("ALTER TYPE userrole RENAME TO userrole__;"))
     conn.execute(
         text("CREATE TYPE userrole as enum (%s)" % ("'" + "','".join(userrole_choices) + "'"))
     )
-    conn.execute(
-        text(
-            textwrap.dedent(
-                """\
+    conn.execute(text(textwrap.dedent("""\
         ALTER TABLE users
             ALTER COLUMN role TYPE userrole USING role::text::userrole;
-    """
-            )
-        )
-    )
+    """)))
     conn.execute(text("DROP TYPE userrole__;"))
 
     # Set admin@lablup.com's role as superadmin.
     # Also, set admin@lablup.com's domain to default.
     #
     # We have judged superadmin as an admin user not associated with any domain.
     # This results in broken code execution for superadmin since doamain_name should not be null.
     # So, this policy is changed to simply adopt superadmin role, and superadmin can also have
     # domain and groups as well.
     query = "SELECT uuid FROM users where email = 'admin@lablup.com';"
     result = conn.execute(text(query)).first()
     uuid = result.uuid if hasattr(result, "uuid") else None
     if uuid is not None:  # update only when admin@lablup.com user exist
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             UPDATE users SET domain_name = 'default', role = 'superadmin'
             WHERE email = 'admin@lablup.com';
-        """
-        )
+        """)
         conn.execute(text(query))
 
 
 def downgrade():
     # ### commands auto generated by Alembic - please adjust! ###
     pass
     # ### end Alembic commands ###
@@ -80,18 +72,12 @@
         conn.execute(text(query))
 
         # Remove superadmin from user role choices.
         conn.execute(text("ALTER TYPE userrole RENAME TO userrole___;"))
         conn.execute(
             text("CREATE TYPE userrole as enum (%s)" % ("'" + "','".join(userrole_choices) + "'"))
         )
-        conn.execute(
-            text(
-                textwrap.dedent(
-                    """\
+        conn.execute(text(textwrap.dedent("""\
             ALTER TABLE users
                 ALTER COLUMN role TYPE userrole USING role::text::userrole;
-        """
-                )
-            )
-        )
+        """)))
         conn.execute(text("DROP TYPE userrole___;"))
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def upgrade():
     op.drop_constraint("fk_kernel_dependencies_depends_on_kernels", "kernel_dependencies")
     op.drop_constraint("fk_kernel_dependencies_kernel_id_kernels", "kernel_dependencies")
     op.rename_table("kernel_dependencies", "session_dependencies")
     op.alter_column("session_dependencies", "kernel_id", new_column_name="session_id")
-    op.execute(text("ALTER INDEX pk_kernel_dependencies " "RENAME TO pk_session_dependencies"))
+    op.execute(text("ALTER INDEX pk_kernel_dependencies RENAME TO pk_session_dependencies"))
     op.execute(
         text(
             "ALTER INDEX ix_kernel_dependencies_depends_on "
             "RENAME TO ix_session_dependencies_depends_on"
         )
     )
     op.execute(
@@ -57,15 +57,15 @@
 
 
 def downgrade():
     op.drop_constraint("fk_session_dependencies_depends_on_kernels", "session_dependencies")
     op.drop_constraint("fk_session_dependencies_session_id_kernels", "session_dependencies")
     op.rename_table("session_dependencies", "kernel_dependencies")
     op.alter_column("kernel_dependencies", "session_id", new_column_name="kernel_id")
-    op.execute(text("ALTER INDEX pk_session_dependencies " "RENAME TO pk_kernel_dependencies"))
+    op.execute(text("ALTER INDEX pk_session_dependencies RENAME TO pk_kernel_dependencies"))
     op.execute(
         text(
             "ALTER INDEX ix_session_dependencies_depends_on "
             "RENAME TO ix_kernel_dependencies_depends_on"
         )
     )
     op.execute(
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/base.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -627,15 +627,15 @@
     """
     A batched query adaptor for (key -> item) resolving patterns.
     """
     objs_per_key: Dict[_Key, Optional[_GenericSQLBasedGQLObject]]
     objs_per_key = collections.OrderedDict()
     for key in key_list:
         objs_per_key[key] = None
-    async for row in (await db_conn.stream(query)):
+    async for row in await db_conn.stream(query):
         objs_per_key[key_getter(row)] = obj_type.from_row(graph_ctx, row)
     return [*objs_per_key.values()]
 
 
 async def batch_multiresult(
     graph_ctx: GraphQueryContext,
     db_conn: SAConnection,
@@ -647,15 +647,15 @@
     """
     A batched query adaptor for (key -> [item]) resolving patterns.
     """
     objs_per_key: Dict[_Key, List[_GenericSQLBasedGQLObject]]
     objs_per_key = collections.OrderedDict()
     for key in key_list:
         objs_per_key[key] = list()
-    async for row in (await db_conn.stream(query)):
+    async for row in await db_conn.stream(query):
         objs_per_key[key_getter(row)].append(
             obj_type.from_row(graph_ctx, row),
         )
     return [*objs_per_key.values()]
 
 
 async def batch_result_in_session(
@@ -670,15 +670,15 @@
     A batched query adaptor for (key -> item) resolving patterns.
     stream the result in async session.
     """
     objs_per_key: Dict[_Key, Optional[_GenericSQLBasedGQLObject]]
     objs_per_key = collections.OrderedDict()
     for key in key_list:
         objs_per_key[key] = None
-    async for row in (await db_sess.stream(query)):
+    async for row in await db_sess.stream(query):
         objs_per_key[key_getter(row)] = obj_type.from_row(graph_ctx, row)
     return [*objs_per_key.values()]
 
 
 async def batch_multiresult_in_session(
     graph_ctx: GraphQueryContext,
     db_sess: SASession,
@@ -691,15 +691,15 @@
     A batched query adaptor for (key -> [item]) resolving patterns.
     stream the result in async session.
     """
     objs_per_key: Dict[_Key, List[_GenericSQLBasedGQLObject]]
     objs_per_key = collections.OrderedDict()
     for key in key_list:
         objs_per_key[key] = list()
-    async for row in (await db_sess.stream(query)):
+    async for row in await db_sess.stream(query):
         objs_per_key[key_getter(row)].append(
             obj_type.from_row(graph_ctx, row),
         )
     return [*objs_per_key.values()]
 
 
 def privileged_query(required_role: UserRole):
@@ -813,16 +813,18 @@
                 else:
                     if target_func is None:
                         return cls(False, "misconfigured privileged mutation: no target_func", None)
                     target_domain, target_group = target_func(*args, **kwargs)
                     if target_domain is None and target_group is None:
                         return cls(
                             False,
-                            "misconfigured privileged mutation: "
-                            "both target_domain and target_group missing",
+                            (
+                                "misconfigured privileged mutation: "
+                                "both target_domain and target_group missing"
+                            ),
                             None,
                         )
                     permit_chains = []
                     if target_domain is not None:
                         if ctx.user["domain_name"] == target_domain:
                             permit_chains.append(True)
                     if target_group is not None:
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/domain.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/dotfile.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/dotfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,12 +74,14 @@
     vfolder_kernel_paths = {m.kernel_path for m in vfolder_mounts}
     for dotfile in internal_data.get("dotfiles", []):
         dotfile_path = PurePosixPath(dotfile["path"])
         if not dotfile_path.is_absolute():
             dotfile_path = PurePosixPath("/home/work", dotfile["path"])
         if dotfile_path in vfolder_kernel_paths:
             raise BackendError(
-                f"There is a kernel-side path from vfolders that conflicts with "
-                f"a dotfile '{dotfile['path']}'.",
+                (
+                    "There is a kernel-side path from vfolders that conflicts with "
+                    f"a dotfile '{dotfile['path']}'."
+                ),
             )
 
     return internal_data
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/endpoint.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/error_logs.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/error_logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/gql.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/gql.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     )
 
     from ..api.manager import ManagerStatus
     from ..config import LocalConfig, SharedConfig
     from ..registry import AgentRegistry
     from ..models.utils import ExtendedAsyncSAEngine
     from .storage import StorageSessionManager
+    from ..idle import IdleCheckerHost
 
 from ..api.exceptions import (
     ImageNotFound,
     InsufficientPrivilege,
     InvalidAPIParameters,
     ObjectNotFound,
     TooManyKernelsFound,
@@ -120,14 +121,15 @@
     redis_live: RedisConnectionInfo
     redis_image: RedisConnectionInfo
     manager_status: ManagerStatus
     known_slot_types: Mapping[SlotName, SlotTypes]
     background_task_manager: BackgroundTaskManager
     storage_manager: StorageSessionManager
     registry: AgentRegistry
+    idle_checker_host: IdleCheckerHost
 
 
 class Mutations(graphene.ObjectType):
     """
     All available GraphQL mutations.
     """
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/group.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,21 +568,23 @@
     )
     async def mutate(cls, root, info: graphene.ResolveInfo, gid: uuid.UUID) -> PurgeGroup:
         graph_ctx: GraphQueryContext = info.context
 
         async def _pre_func(conn: SAConnection) -> None:
             if await cls.group_vfolder_mounted_to_active_kernels(conn, gid):
                 raise RuntimeError(
-                    "Some of virtual folders that belong to this group "
-                    "are currently mounted to active sessions. "
-                    "Terminate them first to proceed removal.",
+                    (
+                        "Some of virtual folders that belong to this group "
+                        "are currently mounted to active sessions. "
+                        "Terminate them first to proceed removal."
+                    ),
                 )
             if await cls.group_has_active_kernels(conn, gid):
                 raise RuntimeError(
-                    "Group has some active session. " "Terminate them first to proceed removal.",
+                    "Group has some active session. Terminate them first to proceed removal.",
                 )
             await cls.delete_vfolders(graph_ctx.db, gid, graph_ctx.storage_manager)
             await cls.delete_kernels(conn, gid)
 
         delete_query = sa.delete(groups).where(groups.c.id == gid)
         return await simple_db_mutate(cls, graph_ctx, delete_query, pre_func=_pre_func)
 
@@ -675,15 +677,15 @@
             sa.select([kernels.c.mounts])
             .select_from(kernels)
             .where(
                 (kernels.c.group_id == group_id)
                 & (kernels.c.status.in_(AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES)),
             )
         )
-        async for row in (await db_conn.stream(query)):
+        async for row in await db_conn.stream(query):
             for _mount in row["mounts"]:
                 try:
                     vfolder_id = uuid.UUID(_mount[2])
                     if vfolder_id in group_vfolder_ids:
                         return True
                 except Exception:
                     pass
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/image.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/kernel.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from dateutil.tz import tzutc
 from graphene.types.datetime import DateTime as GQLDateTime
 from redis.asyncio import Redis
 from redis.asyncio.client import Pipeline
 from sqlalchemy.dialects import postgresql as pgsql
 from sqlalchemy.engine.row import Row
 from sqlalchemy.ext.asyncio import AsyncSession as SASession
-from sqlalchemy.orm import noload, relationship, selectinload
+from sqlalchemy.orm import load_only, noload, relationship, selectinload
 
 from ai.backend.common import msgpack, redis_helper
 from ai.backend.common.docker import ImageRef
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import (
     AccessKey,
     BinarySize,
@@ -84,23 +84,25 @@
     "get_user_email",
     "handle_kernel_exception",
     "kernels",
     "KernelRow",
     "KERNEL_STATUS_TRANSITION_MAP",
     "KernelStatistics",
     "KernelStatus",
+    "KernelRole",
     "ComputeContainer",
     "ComputeContainerList",
     "LegacyComputeSession",
     "LegacyComputeSessionList",
     "AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES",
     "USER_RESOURCE_OCCUPYING_KERNEL_STATUSES",
     "RESOURCE_USAGE_KERNEL_STATUSES",
     "DEAD_KERNEL_STATUSES",
     "LIVE_STATUS",
+    "PRIVATE_KERNEL_ROLES",
     "recalc_concurrency_used",
 )
 
 log = BraceStyleAdapter(logging.getLogger("ai.backend.manager.models.kernel"))
 
 
 class KernelStatus(enum.Enum):
@@ -121,14 +123,23 @@
     # ---
     TERMINATING = 40
     TERMINATED = 41
     ERROR = 42
     CANCELLED = 43
 
 
+class KernelRole(enum.Enum):
+    INFERENCE = "INFERENCE"
+    COMPUTE = "COMPUTE"
+    SYSTEM = "SYSTEM"
+
+
+PRIVATE_KERNEL_ROLES = (KernelRole.SYSTEM,)
+
+
 # statuses to consider when calculating current resource usage
 AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES = tuple(
     e
     for e in KernelStatus
     if e
     not in (
         KernelStatus.TERMINATED,
@@ -446,14 +457,22 @@
         "status",
         EnumType(KernelStatus),
         default=KernelStatus.PENDING,
         server_default=KernelStatus.PENDING.name,
         nullable=False,
         index=True,
     ),
+    sa.Column(
+        "role",
+        EnumType(KernelRole),
+        default=KernelRole.COMPUTE,
+        server_default=KernelRole.COMPUTE.name,
+        nullable=False,
+        index=True,
+    ),
     sa.Column("status_changed", sa.DateTime(timezone=True), nullable=True, index=True),
     sa.Column("status_info", sa.Unicode(), nullable=True, default=sa.null()),
     # status_info contains a kebab-cased string that expresses a summary of the last status change.
     # Examples: "user-requested", "self-terminated", "predicate-checks-failed", "no-available-instances"
     sa.Column("status_data", pgsql.JSONB(), nullable=True, default=sa.null()),
     # status_data contains a JSON object that contains detailed data for the last status change.
     # During scheduling (as PENDING + ("no-available-instances" | "predicate-checks-failed")):
@@ -515,15 +534,15 @@
     ),
     sa.Index(
         "ix_kernels_unique_sess_token",
         "access_key",
         "session_name",
         unique=True,
         postgresql_where=sa.text(
-            "status NOT IN ('TERMINATED', 'CANCELLED') and " "cluster_role = 'main'"
+            "status NOT IN ('TERMINATED', 'CANCELLED') and cluster_role = 'main'"
         ),
     ),
 )
 
 
 class KernelRow(Base):
     __table__ = kernels
@@ -566,27 +585,32 @@
                     if (k.status not in DEAD_KERNEL_STATUSES)
                     and (k.agent_row.status == AgentStatus.ALIVE)
                 ]
             if not cand:
                 raise SessionNotFound
             return cand[0]
 
-    @staticmethod
+    @classmethod
     async def set_kernel_status(
+        cls,
         db: ExtendedAsyncSAEngine,
         kernel_id: KernelId,
         status: KernelStatus,
         *,
         status_data: Optional[Mapping[str, Any]] = None,
         reason: Optional[str] = None,
+        status_changed_at: Optional[datetime] = None,
     ) -> None:
-        assert status != KernelStatus.TERMINATED, (
-            "TERMINATED status update must be handled in " "mark_kernel_terminated()"
-        )
-        now = datetime.now(tzutc())
+        assert (
+            status != KernelStatus.TERMINATED
+        ), "TERMINATED status update must be handled in mark_kernel_terminated()"
+        if status_changed_at is None:
+            now = datetime.now(tzutc())
+        else:
+            now = status_changed_at
         data = {
             "status": status,
             "status_changed": now,
             "status_history": sql_json_merge(
                 kernels.c.status_history,
                 (),
                 {
@@ -597,23 +621,71 @@
         if status_data is not None:
             data["status_data"] = status_data
         if reason is not None:
             data["status_info"] = reason
         if status in (KernelStatus.CANCELLED, KernelStatus.TERMINATED):
             data["terminated_at"] = now
 
-        async def _transit() -> None:
-            async with db.begin_session() as db_sess:
-                kernel_query = sa.select(KernelRow.status).where(KernelRow.id == kernel_id)
-                current_status = (await db_sess.execute(kernel_query)).scalar()
-                if status in KERNEL_STATUS_TRANSITION_MAP[current_status]:
-                    query = sa.update(KernelRow).values(**data).where(KernelRow.id == kernel_id)
-                    await db_sess.execute(query)
+        await cls.update_kernel(db, kernel_id, status, update_data=data)
 
-        await execute_with_retry(_transit)
+    @classmethod
+    async def update_kernel(
+        cls,
+        db: ExtendedAsyncSAEngine,
+        kernel_id: KernelId,
+        new_status: KernelStatus,
+        update_data: Optional[Mapping[str, Any]] = None,
+    ) -> bool:
+        """
+        Update kernel by given id and data.
+        Return True if the kernel is updated, else return False.
+        """
+
+        now = datetime.now(tzutc())
+
+        async def _update() -> bool:
+            async with db.begin_session() as db_session:
+                kernel_query = (
+                    sa.select(KernelRow)
+                    .where(KernelRow.id == kernel_id)
+                    .with_for_update()
+                    .options(
+                        noload("*"),
+                        load_only(KernelRow.status, KernelRow.session_id),
+                    )
+                )
+                kernel_row = (await db_session.scalars(kernel_query)).first()
+
+                if new_status not in KERNEL_STATUS_TRANSITION_MAP[kernel_row.status]:
+                    # TODO: log or raise error
+                    return False
+                if update_data is None:
+                    update_values = {
+                        "status": new_status,
+                        "status_history": sql_json_merge(
+                            KernelRow.status_history,
+                            (),
+                            {
+                                new_status.name: now.isoformat(),
+                            },
+                        ),
+                    }
+                else:
+                    update_values = {
+                        **update_data,
+                        "status": new_status,
+                    }
+
+                update_query = (
+                    sa.update(KernelRow).where(KernelRow.id == kernel_id).values(**update_values)
+                )
+                await db_session.execute(update_query)
+            return True
+
+        return await execute_with_retry(_update)
 
 
 DEFAULT_KERNEL_ORDERING = [
     sa.desc(
         sa.func.greatest(
             KernelRow.created_at,
             KernelRow.terminated_at,
@@ -657,26 +729,21 @@
         cls,
         ctx: GraphQueryContext,
         session_ids: Sequence[SessionId],
     ) -> Sequence[Optional[Mapping[str, Any]]]:
         async def _build_pipeline(redis: Redis) -> Pipeline:
             pipe = redis.pipeline()
             for sess_id in session_ids:
-                log.debug(
-                    "Getting {}",
-                    [f"session.{sess_id}.requests", f"session.{sess_id}.last_response_time"],
-                )
                 await pipe.mget(
                     [f"session.{sess_id}.requests", f"session.{sess_id}.last_response_time"]
                 )
             return pipe
 
         stats = []
         results = await redis_helper.execute(ctx.redis_live, _build_pipeline)
-        log.debug("results {}", results)
         for result in results:
             if result[0] is not None and result[1] is not None:
                 requests = int(result[0])
                 last_response_ms = int(result[1])
             else:
                 requests = 0
                 last_response_ms = 0
@@ -1366,15 +1433,16 @@
     concurrency_used: int
     async with db_sess.begin_nested():
         result = await db_sess.execute(
             sa.select(sa.func.count())
             .select_from(KernelRow)
             .where(
                 (KernelRow.access_key == access_key)
-                & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES)),
+                & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES))
+                & (KernelRow.role.not_in(PRIVATE_KERNEL_ROLES)),
             ),
         )
         concurrency_used = result.scalar()
         assert isinstance(concurrency_used, int)
 
     await redis_helper.execute(
         redis_stat,
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/keypair.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/keypair.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,16 +174,17 @@
     )
     concurrency_used = graphene.Int()
 
     user_info = graphene.Field(lambda: UserInfo)
 
     # Deprecated
     concurrency_limit = graphene.Int(
-        deprecation_reason="Moved to KeyPairResourcePolicy object as "
-        "the max_concurrent_sessions field."
+        deprecation_reason=(
+            "Moved to KeyPairResourcePolicy object as the max_concurrent_sessions field."
+        )
     )
 
     async def resolve_user_info(
         self,
         info: graphene.ResolveInfo,
     ) -> UserInfo:
         ctx: GraphQueryContext = info.context
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/minilang/ordering.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/minilang/ordering.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/minilang/queryfilter.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/minilang/queryfilter.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/resource_policy.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/resource_preset.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/resource_preset.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,17 +126,17 @@
         info: graphene.ResolveInfo,
         name: str,
         props: CreateResourcePresetInput,
     ) -> CreateResourcePreset:
         data = {
             "name": name,
             "resource_slots": ResourceSlot.from_user_input(props.resource_slots, None),
-            "shared_memory": BinarySize.from_str(props.shared_memory)
-            if props.shared_memory
-            else None,
+            "shared_memory": (
+                BinarySize.from_str(props.shared_memory) if props.shared_memory else None
+            ),
         }
         insert_query = sa.insert(resource_presets).values(data)
         return await simple_db_mutate_returning_item(
             cls,
             info.context,
             insert_query,
             item_cls=ResourcePreset,
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/routing.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/routing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/scaling_group.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/scaling_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import sqlalchemy as sa
 import trafaret as t
 from graphene.types.datetime import DateTime as GQLDateTime
 from sqlalchemy.dialects import postgresql as pgsql
 from sqlalchemy.engine.row import Row
 from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
 from sqlalchemy.orm import relationship
+from sqlalchemy.sql.expression import true
 
 from ai.backend.common import validators as tx
 from ai.backend.common.types import JSONSerializableMixin, SessionTypes
 
 from .base import (
     Base,
     StructuredJSONObjectColumn,
@@ -54,15 +55,19 @@
     "DisassociateScalingGroupWithKeyPair",
 )
 
 
 @attr.define(slots=True)
 class ScalingGroupOpts(JSONSerializableMixin):
     allowed_session_types: list[SessionTypes] = attr.Factory(
-        lambda: [SessionTypes.INTERACTIVE, SessionTypes.BATCH, SessionTypes.INFERENCE],
+        lambda: [
+            SessionTypes.INTERACTIVE,
+            SessionTypes.BATCH,
+            SessionTypes.INFERENCE,
+        ],
     )
     pending_timeout: timedelta = timedelta(seconds=0)
     config: Mapping[str, Any] = attr.Factory(dict)
 
     def to_json(self) -> dict[str, Any]:
         return {
             "allowed_session_types": [item.value for item in self.allowed_session_types],
@@ -90,14 +95,17 @@
 
 scaling_groups = sa.Table(
     "scaling_groups",
     mapper_registry.metadata,
     sa.Column("name", sa.String(length=64), primary_key=True),
     sa.Column("description", sa.String(length=512)),
     sa.Column("is_active", sa.Boolean, index=True, default=True),
+    sa.Column(
+        "is_public", sa.Boolean, index=True, default=True, server_default=true(), nullable=False
+    ),
     sa.Column("created_at", sa.DateTime(timezone=True), server_default=sa.func.now()),
     sa.Column("wsproxy_addr", sa.String(length=1024), nullable=True),
     sa.Column("driver", sa.String(length=64), nullable=False),
     sa.Column("driver_opts", pgsql.JSONB(), nullable=False, default={}),
     sa.Column("scheduler", sa.String(length=64), nullable=False),
     sa.Column("use_host_network", sa.Boolean, nullable=False, default=False),
     sa.Column(
@@ -278,14 +286,15 @@
     return [row for row in result]
 
 
 class ScalingGroup(graphene.ObjectType):
     name = graphene.String()
     description = graphene.String()
     is_active = graphene.Boolean()
+    is_public = graphene.Boolean()
     created_at = GQLDateTime()
     wsproxy_addr = graphene.String()
     driver = graphene.String()
     driver_opts = graphene.JSONString()
     scheduler = graphene.String()
     scheduler_opts = graphene.JSONString()
     use_host_network = graphene.Boolean()
@@ -298,14 +307,15 @@
     ) -> ScalingGroup | None:
         if row is None:
             return None
         return cls(
             name=row["name"],
             description=row["description"],
             is_active=row["is_active"],
+            is_public=row["is_public"],
             created_at=row["created_at"],
             wsproxy_addr=row["wsproxy_addr"],
             driver=row["driver"],
             driver_opts=row["driver_opts"],
             scheduler=row["scheduler"],
             scheduler_opts=row["scheduler_opts"].to_json(),
             use_host_network=row["use_host_network"],
@@ -452,25 +462,27 @@
                 lambda row: row["name"],
             )
 
 
 class CreateScalingGroupInput(graphene.InputObjectType):
     description = graphene.String(required=False, default="")
     is_active = graphene.Boolean(required=False, default=True)
+    is_public = graphene.Boolean(required=False, default=True)
     wsproxy_addr = graphene.String(required=False)
     driver = graphene.String(required=True)
     driver_opts = graphene.JSONString(required=False, default={})
     scheduler = graphene.String(required=True)
     scheduler_opts = graphene.JSONString(required=False, default={})
     use_host_network = graphene.Boolean(required=False, default=False)
 
 
 class ModifyScalingGroupInput(graphene.InputObjectType):
     description = graphene.String(required=False)
     is_active = graphene.Boolean(required=False)
+    is_public = graphene.Boolean(required=False)
     wsproxy_addr = graphene.String(required=False)
     driver = graphene.String(required=False)
     driver_opts = graphene.JSONString(required=False)
     scheduler = graphene.String(required=False)
     scheduler_opts = graphene.JSONString(required=False)
     use_host_network = graphene.Boolean(required=False)
 
@@ -494,14 +506,15 @@
         name: str,
         props: CreateScalingGroupInput,
     ) -> CreateScalingGroup:
         data = {
             "name": name,
             "description": props.description,
             "is_active": bool(props.is_active),
+            "is_public": bool(props.is_public),
             "wsproxy_addr": props.wsproxy_addr,
             "driver": props.driver,
             "driver_opts": props.driver_opts,
             "scheduler": props.scheduler,
             "scheduler_opts": ScalingGroupOpts.from_json(props.scheduler_opts),
             "use_host_network": bool(props.use_host_network),
         }
@@ -531,14 +544,15 @@
         info: graphene.ResolveInfo,
         name: str,
         props: ModifyScalingGroupInput,
     ) -> ModifyScalingGroup:
         data: Dict[str, Any] = {}
         set_if_set(props, data, "description")
         set_if_set(props, data, "is_active")
+        set_if_set(props, data, "is_public")
         set_if_set(props, data, "driver")
         set_if_set(props, data, "wsproxy_addr")
         set_if_set(props, data, "driver_opts")
         set_if_set(props, data, "scheduler")
         set_if_set(
             props, data, "scheduler_opts", clean_func=lambda v: ScalingGroupOpts.from_json(v)
         )
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/session.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,20 @@
 import graphene
 import sqlalchemy as sa
 from dateutil.parser import parse as dtparse
 from dateutil.tz import tzutc
 from graphene.types.datetime import DateTime as GQLDateTime
 from sqlalchemy.dialects import postgresql as pgsql
 from sqlalchemy.ext.asyncio import AsyncSession as SASession
-from sqlalchemy.orm import noload, relationship, selectinload
+from sqlalchemy.orm import load_only, noload, relationship, selectinload
 
 from ai.backend.common.types import (
     AccessKey,
     ClusterMode,
+    KernelId,
     ResourceSlot,
     SessionId,
     SessionResult,
     SessionTypes,
     SlotName,
     VFolderMount,
 )
@@ -608,17 +609,14 @@
         "status",
         EnumType(SessionStatus),
         default=SessionStatus.PENDING,
         server_default=SessionStatus.PENDING.name,
         nullable=False,
         index=True,
     )
-    # status_changed = sa.Column(
-    #     "status_changed", sa.DateTime(timezone=True), nullable=True, index=True
-    # )
     status_info = sa.Column("status_info", sa.Unicode(), nullable=True, default=sa.null())
 
     status_data = sa.Column("status_data", pgsql.JSONB(), nullable=True, default=sa.null())
     # status_data contains a JSON object that contains detailed data for the last status change.
     # During scheduling (as PENDING + ("no-available-instances" | "predicate-checks-failed")):
     # {
     #   "scheduler": {
@@ -707,24 +705,92 @@
             )
         if len(kerns) == 0:
             raise MainKernelNotFound(
                 f"Session (id: {self.id}) has no kernel with {cluster_name = }.",
             )
         return kerns[0]
 
+    @classmethod
+    async def get_session_id_by_kernel(
+        cls, db: ExtendedAsyncSAEngine, kernel_id: KernelId
+    ) -> SessionId:
+        query = sa.select(KernelRow.session_id).where(KernelRow.id == kernel_id)
+        async with db.begin_readonly_session() as db_session:
+            return await db_session.scalar(query)
+
+    @classmethod
+    async def transit_session_status(
+        cls,
+        db: ExtendedAsyncSAEngine,
+        session_id: SessionId,
+        *,
+        status_info: str | None = None,
+    ) -> SessionStatus | None:
+        """
+        Check status of session's sibling kernels and transit the status of session.
+        Return the new status of session.
+        """
+        now = datetime.now(tzutc())
+
+        async def _check_and_update() -> SessionStatus | None:
+            async with db.begin_session() as db_session:
+                session_query = (
+                    sa.select(SessionRow)
+                    .where(SessionRow.id == session_id)
+                    .with_for_update()
+                    .options(
+                        noload("*"),
+                        load_only(SessionRow.status),
+                        selectinload(SessionRow.kernels).options(
+                            noload("*"), load_only(KernelRow.status, KernelRow.cluster_role)
+                        ),
+                    )
+                )
+                session_row: SessionRow = (await db_session.scalars(session_query)).first()
+                determined_status = determine_session_status(session_row.kernels)
+                if determined_status not in SESSION_STATUS_TRANSITION_MAP[session_row.status]:
+                    # TODO: log or raise error
+                    return None
+
+                update_values = {
+                    "status": determined_status,
+                    "status_history": sql_json_merge(
+                        SessionRow.status_history,
+                        (),
+                        {
+                            determined_status.name: now.isoformat(),
+                        },
+                    ),
+                }
+                if determined_status in (SessionStatus.CANCELLED, SessionStatus.TERMINATED):
+                    update_values["terminated_at"] = now
+                if status_info is not None:
+                    update_values["status_info"] = status_info
+                update_query = (
+                    sa.update(SessionRow).where(SessionRow.id == session_id).values(**update_values)
+                )
+                await db_session.execute(update_query)
+            return determined_status
+
+        return await execute_with_retry(_check_and_update)
+
     @staticmethod
     async def set_session_status(
         db: ExtendedAsyncSAEngine,
         session_id: SessionId,
         status: SessionStatus,
         *,
         status_data: Optional[Mapping[str, Any]] = None,
         reason: Optional[str] = None,
+        status_changed_at: Optional[datetime] = None,
     ) -> None:
-        now = datetime.now(tzutc())
+        if status_changed_at is None:
+            now = datetime.now(tzutc())
+        else:
+            now = status_changed_at
         data = {
             "status": status,
             "status_history": sql_json_merge(
                 SessionRow.status_history,
                 (),
                 {
                     status.name: datetime.now(tzutc()).isoformat(),
@@ -734,20 +800,20 @@
         if status_data is not None:
             data["status_data"] = status_data
         if reason is not None:
             data["status_info"] = reason
         if status in (SessionStatus.CANCELLED, SessionStatus.TERMINATED):
             data["terminated_at"] = now
 
-        async def _transit() -> None:
+        async def _update() -> None:
             async with db.begin_session() as db_sess:
                 query = sa.update(SessionRow).values(**data).where(SessionRow.id == session_id)
                 await db_sess.execute(query)
 
-        await execute_with_retry(_transit)
+        await execute_with_retry(_update)
 
     async def set_session_result(
         db: ExtendedAsyncSAEngine,
         session_id: SessionId,
         success: bool,
         exit_code: int,
     ) -> None:
@@ -970,14 +1036,59 @@
                 selectinload(SessionRow.access_key_row).options(noload("*")),
                 selectinload(SessionRow.kernels).options(noload("*")),
             )
         )
         result = await db_sess.execute(query)
         return result.scalars().all()
 
+    @classmethod
+    async def get_session_to_destroy(
+        cls, db: ExtendedAsyncSAEngine, session_id: SessionId
+    ) -> SessionRow:
+        query = (
+            sa.select(SessionRow)
+            .where(SessionRow.id == session_id)
+            .options(
+                noload("*"),
+                load_only(SessionRow.creation_id, SessionRow.status),
+                selectinload(SessionRow.kernels).options(
+                    noload("*"),
+                    load_only(
+                        KernelRow.id,
+                        KernelRow.role,
+                        KernelRow.access_key,
+                        KernelRow.status,
+                        KernelRow.container_id,
+                        KernelRow.cluster_role,
+                        KernelRow.agent,
+                        KernelRow.agent_addr,
+                    ),
+                ),
+            )
+        )
+        async with db.begin_readonly_session() as db_session:
+            return (await db_session.scalars(query)).first()
+
+    @classmethod
+    async def get_session_to_produce_event(
+        cls, db: ExtendedAsyncSAEngine, session_id: SessionId
+    ) -> SessionRow:
+        query = (
+            sa.select(SessionRow)
+            .where(SessionRow.id == session_id)
+            .options(
+                noload("*"),
+                load_only(
+                    SessionRow.id, SessionRow.name, SessionRow.creation_id, SessionRow.access_key
+                ),
+            )
+        )
+        async with db.begin_readonly_session() as db_session:
+            return (await db_session.scalars(query)).first()
+
 
 class SessionDependencyRow(Base):
     __tablename__ = "session_dependencies"
     session_id = sa.Column(
         "session_id",
         GUID,
         sa.ForeignKey("sessions.id", onupdate="CASCADE", ondelete="CASCADE"),
@@ -1070,14 +1181,15 @@
     created_at = GQLDateTime()
     terminated_at = GQLDateTime()
     starts_at = GQLDateTime()
     startup_command = graphene.String()
     result = graphene.String()
     commit_status = graphene.String()
     abusing_reports = graphene.List(lambda: graphene.JSONString)
+    idle_checks = graphene.JSONString()
 
     # resources
     resource_opts = graphene.JSONString()
     scaling_group = graphene.String()
     service_ports = graphene.JSONString()
     mounts = graphene.List(lambda: graphene.String)
     vfolder_mounts = graphene.List(lambda: graphene.String)
@@ -1227,14 +1339,18 @@
         containers = self.containers
         if containers is None:
             containers = await self.resolve_containers(info)
         if containers is None:
             return []
         return [(await con.resolve_abusing_report(info, self.access_key)) for con in containers]
 
+    async def resolve_idle_checks(self, info: graphene.ResolveInfo) -> Mapping[str, Any]:
+        graph_ctx: GraphQueryContext = info.context
+        return await graph_ctx.idle_checker_host.get_idle_check_report(self.session_id)
+
     _queryfilter_fieldspec = {
         "id": ("sessions_id", None),
         "type": ("sessions_session_type", lambda s: SessionTypes[s]),
         "name": ("sessions_name", None),
         "domain_name": ("sessions_domain_name", None),
         "group_name": ("groups_name", None),
         "user_email": ("users_email", None),
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/session_template.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/session_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,50 +60,45 @@
                 tx.AliasedKey(["type", "session_type", "sessionType"], default="interactive")
                 >> "session_type": tx.Enum(SessionTypes),
                 t.Key("kernel"): t.Dict(
                     {
                         t.Key("image"): t.String,
                         t.Key("architecture", default="x86_64"): t.Null | t.String,
                         t.Key("environ", default={}): t.Null | t.Mapping(t.String, t.String),
-                        t.Key("run", default=None): t.Null
-                        | t.Dict(
+                        t.Key("run", default=None): t.Null | t.Dict(
                             {
                                 t.Key("bootstrap", default=None): t.Null | t.String,
                                 tx.AliasedKey(
                                     ["startup", "startup_command", "startupCommand"], default=None
                                 )
-                                >> "startup_command": t.Null
-                                | t.String,
+                                >> "startup_command": t.Null | t.String,
                             }
                         ),
-                        t.Key("git", default=None): t.Null
-                        | t.Dict(
+                        t.Key("git", default=None): t.Null | t.Dict(
                             {
                                 t.Key("repository"): t.String,
                                 t.Key("commit", default=None): t.Null | t.String,
                                 t.Key("branch", default=None): t.Null | t.String,
-                                t.Key("credential", default=None): t.Null
-                                | t.Dict(
+                                t.Key("credential", default=None): t.Null | t.Dict(
                                     {
                                         t.Key("username"): t.String,
                                         t.Key("password"): t.String,
                                     }
                                 ),
                                 tx.AliasedKey(["destination_dir", "destinationDir"], default=None)
-                                >> "dest_dir": t.Null
-                                | t.String,
+                                >> "dest_dir": t.Null | t.String,
                             }
                         ),
                     }
                 ),
                 t.Key("scaling_group", default=None): t.Null | t.String,
                 t.Key("mounts", default={}): t.Null | t.Mapping(t.String, t.Any),
                 t.Key("resources", default=None): t.Null | t.Mapping(t.String, t.Any),
-                tx.AliasedKey(["agent_list", "agentList"], default=None) >> "agent_list": t.Null
-                | t.List(t.String),
+                tx.AliasedKey(["agent_list", "agentList"], default=None)
+                >> "agent_list": t.Null | t.List(t.String),
             }
         ),
     }
 ).allow_extra("*")
 
 
 def check_task_template(raw_data: Mapping[str, Any]) -> Mapping[str, Any]:
@@ -269,15 +264,17 @@
                     "created_at": row.session_templates_created_at,
                     "is_owner": is_owner,
                     "user": (
                         str(row.session_templates_user_uuid)
                         if row.session_templates_user_uuid
                         else None
                     ),
-                    "group": str(row.session_templates_group_id)
-                    if row.session_templates_group_id
-                    else None,
+                    "group": (
+                        str(row.session_templates_group_id)
+                        if row.session_templates_group_id
+                        else None
+                    ),
                     "user_email": None,
                     "group_name": row.groups_name,
                 }
             )
     return entries
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/storage.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 @attrs.define(auto_attribs=True, slots=True, frozen=True)
 class StorageProxyInfo:
     session: aiohttp.ClientSession
     secret: str
     client_api_url: yarl.URL
     manager_api_url: yarl.URL
+    sftp_scaling_groups: list[str]
 
 
 AUTH_TOKEN_HDR: Final = "X-BackendAI-Storage-Auth-Token"
 
 _ctx_volumes_cache: ContextVar[List[Tuple[str, VolumeInfo]]] = ContextVar("_ctx_volumes")
 
 
@@ -64,26 +65,29 @@
     path: str
     fsprefix: str
     capabilities: List[str]
 
 
 class StorageSessionManager:
     _proxies: Mapping[str, StorageProxyInfo]
+    _exposed_volume_info: List[str]
 
     def __init__(self, storage_config: Mapping[str, Any]) -> None:
         self.config = storage_config
+        self._exposed_volume_info = self.config["exposed_volume_info"]
         self._proxies = {}
         for proxy_name, proxy_config in self.config["proxies"].items():
             connector = aiohttp.TCPConnector(ssl=proxy_config["ssl_verify"])
             session = aiohttp.ClientSession(connector=connector)
             self._proxies[proxy_name] = StorageProxyInfo(
                 session=session,
                 secret=proxy_config["secret"],
                 client_api_url=yarl.URL(proxy_config["client_api"]),
                 manager_api_url=yarl.URL(proxy_config["manager_api"]),
+                sftp_scaling_groups=proxy_config["sftp_scaling_groups"],
             )
 
     async def aclose(self) -> None:
         close_aws = []
         for proxy_info in self._proxies.values():
             close_aws.append(proxy_info.session.close())
         await asyncio.gather(*close_aws, return_exceptions=True)
@@ -116,14 +120,19 @@
 
         for proxy_name, proxy_info in self._proxies.items():
             fetch_aws.append(_fetch(proxy_name, proxy_info))
         results = [*itertools.chain(*await asyncio.gather(*fetch_aws))]
         _ctx_volumes_cache.set(results)
         return results
 
+    async def get_sftp_scaling_groups(self, proxy_name: str) -> List[str]:
+        if proxy_name not in self._proxies:
+            raise IndexError(f"proxy {proxy_name} does not exist")
+        return self._proxies[proxy_name].sftp_scaling_groups or []
+
     async def get_mount_path(
         self,
         vfolder_host: str,
         vfolder_id: UUID,
         subpath: PurePosixPath = PurePosixPath("."),
     ) -> str:
         async with self.request(
@@ -168,16 +177,18 @@
                     raise VFolderOperationFailed(
                         extra_msg=error_data.pop("msg", None),
                         extra_data=error_data,
                     )
                 except aiohttp.ClientResponseError:
                     # when the response body is not JSON, just raise with status info.
                     raise VFolderOperationFailed(
-                        extra_msg=f"Storage proxy responded with "
-                        f"{client_resp.status} {client_resp.reason}",
+                        extra_msg=(
+                            "Storage proxy responded with "
+                            f"{client_resp.status} {client_resp.reason}"
+                        ),
                         extra_data=None,
                     )
                 except VFolderOperationFailed as e:
                     raise InvalidAPIParameters(e.extra_msg, e.extra_data)
             yield proxy_info.client_api_url, client_resp
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/user.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -555,16 +555,16 @@
             # Create a default keypair for the user.
             from .keypair import CreateKeyPair, keypairs
 
             kp_data = CreateKeyPair.prepare_new_keypair(
                 email,
                 graph_ctx.schema.get_type("KeyPairInput").create_container(
                     {
-                        "is_active": (_status == UserStatus.ACTIVE),
-                        "is_admin": (user_data["role"] in [UserRole.SUPERADMIN, UserRole.ADMIN]),
+                        "is_active": _status == UserStatus.ACTIVE,
+                        "is_admin": user_data["role"] in [UserRole.SUPERADMIN, UserRole.ADMIN],
                         "resource_policy": "default",
                         "rate_limit": 10000,
                     }
                 ),
             )
             kp_insert_query = sa.insert(keypairs).values(
                 **kp_data,
@@ -649,17 +649,17 @@
                 .where(users.c.email == email),
             )
             row = result.first()
             prev_domain_name = row.domain_name
             prev_role = row.role
             user_update_data = data.copy()
             if "status" in data and row.status != data["status"]:
-                user_update_data[
-                    "status_info"
-                ] = "admin-requested"  # user mutation is only for admin
+                user_update_data["status_info"] = (
+                    "admin-requested"  # user mutation is only for admin
+                )
 
         update_query = lambda: (  # uses lambda because user_update_data is modified in _pre_func()
             sa.update(users).values(user_update_data).where(users.c.email == email)
         )
 
         async def _post_func(conn: SAConnection, result: Result) -> Row:
             nonlocal prev_domain_name, prev_role
@@ -853,16 +853,18 @@
             user_uuid = await conn.scalar(
                 sa.select([users.c.uuid]).select_from(users).where(users.c.email == email),
             )
             log.info("Purging all records of the user {0}...", email)
 
             if await cls.user_vfolder_mounted_to_active_kernels(conn, user_uuid):
                 raise RuntimeError(
-                    "Some of user's virtual folders are mounted to active kernels. "
-                    "Terminate those kernels first.",
+                    (
+                        "Some of user's virtual folders are mounted to active kernels. "
+                        "Terminate those kernels first."
+                    ),
                 )
             if await cls.user_has_active_kernels(conn, user_uuid):
                 raise RuntimeError("User has some active kernels. Terminate them first.")
 
             if not props.purge_shared_vfolders:
                 await cls.migrate_shared_vfolders(
                     conn,
@@ -916,15 +918,15 @@
         )
         query = (
             sa.select([vfolders.c.id, vfolders.c.name])
             .select_from(j)
             .where(vfolders.c.user == deleted_user_uuid)
         )
         migrate_updates = []
-        async for row in (await conn.stream(query)):
+        async for row in await conn.stream(query):
             name = row.name
             if name in existing_vfolder_names:
                 name += f"-{uuid4().hex[:10]}"
             migrate_updates.append({"vid": row.id, "vname": name})
         if migrate_updates:
             # Remove invitations and vfolder_permissions from target user.
             # Target user will be the new owner, and it does not make sense to have
@@ -1028,15 +1030,15 @@
         rows = result.fetchall()
         user_vfolder_ids = [row.id for row in rows]
         query = (
             sa.select([kernels.c.mounts])
             .select_from(kernels)
             .where(kernels.c.status.in_(AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES))
         )
-        async for row in (await conn.stream(query)):
+        async for row in await conn.stream(query):
             for _mount in row["mounts"]:
                 try:
                     vfolder_id = UUID(_mount[2])
                     if vfolder_id in user_vfolder_ids:
                         return True
                 except Exception:
                     pass
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/utils.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,18 @@
 
     @actxmgr
     async def begin_readonly(self, deferrable: bool = False) -> AsyncIterator[SAConnection]:
         async with self.connect() as conn:
             self._readonly_txn_count += 1
             if self._readonly_txn_count >= self._txn_concurrency_threshold:
                 log.warning(
-                    "The number of concurrent read-only transaction ({}) exceeded the threshold {}.",
+                    (
+                        "The number of concurrent read-only transaction ({}) exceeded the"
+                        " threshold {}."
+                    ),
                     self._readonly_txn_count,
                     self._txn_concurrency_threshold,
                     stack_info=False,
                 )
             conn_with_exec_opts = await conn.execution_options(
                 postgresql_readonly=True,
                 postgresql_deferrable=deferrable,
@@ -256,26 +259,28 @@
 
     Note that the existing value must be also an object, not a primitive value.
     """
     expr = sa.func.coalesce(
         col if _depth == 0 else col[key[:_depth]],
         sa.text("'{}'::jsonb"),
     ).concat(
-        sa.func.jsonb_build_object(
-            key[_depth],
-            (
-                sa.func.coalesce(col[key], sa.text("'{}'::jsonb")).concat(
-                    sa.func.cast(obj, psql.JSONB)
-                )
-                if _depth == len(key) - 1
-                else sql_json_merge(col, key, obj=obj, _depth=_depth + 1)
-            ),
-        )
-        if key
-        else sa.func.cast(obj, psql.JSONB),
+        (
+            sa.func.jsonb_build_object(
+                key[_depth],
+                (
+                    sa.func.coalesce(col[key], sa.text("'{}'::jsonb")).concat(
+                        sa.func.cast(obj, psql.JSONB)
+                    )
+                    if _depth == len(key) - 1
+                    else sql_json_merge(col, key, obj=obj, _depth=_depth + 1)
+                ),
+            )
+            if key
+            else sa.func.cast(obj, psql.JSONB)
+        ),
     )
     return expr
 
 
 def sql_json_increment(
     col,
     key: Tuple[str, ...],
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/models/vfolder.py` & `backend.ai-manager-23.3.1/ai/backend/manager/models/vfolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
 
 from ai.backend.common.bgtask import ProgressReporter
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import VFolderHostPermission, VFolderHostPermissionMap, VFolderMount
 
 from ..api.exceptions import InvalidAPIParameters, VFolderNotFound, VFolderOperationFailed
-from ..defs import RESERVED_VFOLDER_PATTERNS, RESERVED_VFOLDERS
+from ..defs import RESERVED_VFOLDER_PATTERNS, RESERVED_VFOLDERS, VFOLDER_DSTPATHS_MAP
 from ..types import UserScope
 from .base import (
     GUID,
     BigInt,
     EnumValueType,
     IDColumn,
     Item,
@@ -205,16 +205,18 @@
         "status",
         EnumValueType(VFolderOperationStatus),
         default=VFolderOperationStatus.READY,
         server_default=VFolderOperationStatus.READY.value,
         nullable=False,
     ),
     sa.CheckConstraint(
-        "(ownership_type = 'user' AND \"user\" IS NOT NULL) OR "
-        "(ownership_type = 'group' AND \"group\" IS NOT NULL)",
+        (
+            "(ownership_type = 'user' AND \"user\" IS NOT NULL) OR "
+            "(ownership_type = 'group' AND \"group\" IS NOT NULL)"
+        ),
         name="ownership_type_match_with_user_or_group",
     ),
     sa.CheckConstraint(
         '("user" IS NULL AND "group" IS NOT NULL) OR ("user" IS NOT NULL AND "group" IS NULL)',
         name="either_one_of_user_or_group",
     ),
 )
@@ -582,16 +584,15 @@
     matched_vfolder_mounts: list[VFolderMount] = []
 
     # Split the vfolder name and subpaths
     for key in requested_mounts:
         name, _, subpath = key.partition("/")
         if not PurePosixPath(os.path.normpath(key)).is_relative_to(name):
             raise InvalidAPIParameters(
-                f"The subpath '{subpath}' should designate "
-                f"a subdirectory of the vfolder '{name}'.",
+                f"The subpath '{subpath}' should designate a subdirectory of the vfolder '{name}'.",
             )
         requested_vfolder_names[key] = name
         requested_vfolder_subpaths[key] = os.path.normpath(subpath)
     for key, value in requested_mount_map.items():
         requested_vfolder_dstpaths[key] = value
 
     # Check if there are overlapping mount sources
@@ -661,14 +662,16 @@
                     vfolder["host"],
                     vfolder["id"],
                     PurePosixPath(requested_vfolder_subpaths[key]),
                 ),
             )
         except VFolderOperationFailed as e:
             raise InvalidAPIParameters(e.extra_msg, e.extra_data) from None
+        if (_vfname := vfolder["name"]) in VFOLDER_DSTPATHS_MAP:
+            requested_vfolder_dstpaths[_vfname] = VFOLDER_DSTPATHS_MAP[_vfname]
         if vfolder["name"] == ".local" and vfolder["group"] is not None:
             # Auto-create per-user subdirectory inside the group-owned ".local" vfolder.
             async with storage_manager.request(
                 vfolder["host"],
                 "POST",
                 "folder/file/mkdir",
                 params={
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/pglock.py` & `backend.ai-manager-23.3.1/ai/backend/manager/pglock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/plugin/error_monitor.py` & `backend.ai-manager-23.3.1/ai/backend/manager/plugin/error_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
 class ErrorMonitor(AbstractErrorReporterPlugin):
     async def init(self, context: Any = None) -> None:
         if context is None:
             log.warning(
-                "manager.plugin.error_monitor is initialized without the root context. "
-                "The plugin is disabled.",
+                (
+                    "manager.plugin.error_monitor is initialized without the root context. "
+                    "The plugin is disabled."
+                ),
             )
             self.enabled = False
             return
         else:
             self.enabled = True
         root_ctx: RootContext = context["_root.context"]  # type: ignore
         self.event_dispatcher = root_ctx.event_dispatcher
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/plugin/webapp.py` & `backend.ai-manager-23.3.1/ai/backend/manager/plugin/webapp.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/registry.py` & `backend.ai-manager-23.3.1/ai/backend/manager/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import copy
 import itertools
 import logging
 import re
 import time
 import typing
 import uuid
-import weakref
 import zlib
 from collections import defaultdict
 from contextlib import asynccontextmanager as actxmgr
 from contextvars import ContextVar
 from datetime import datetime
 from decimal import Decimal
 from typing import (
@@ -41,15 +40,14 @@
 from callosum.rpc import Peer, RPCUserError
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from dateutil.tz import tzutc
 from redis.asyncio import Redis
 from sqlalchemy.exc import DBAPIError
-from sqlalchemy.orm import selectinload
 from yarl import URL
 
 from ai.backend.common import msgpack, redis_helper
 from ai.backend.common.docker import ImageRef, get_known_registries, get_registry_info
 from ai.backend.common.events import (
     AgentStartedEvent,
     KernelCancelledEvent,
@@ -97,33 +95,32 @@
     QuotaExceeded,
     RejectedByHook,
     ScalingGroupNotFound,
     SessionNotFound,
 )
 from .config import SharedConfig
 from .defs import DEFAULT_ROLE, INTRINSIC_SLOTS
-from .exceptions import MultiAgentError
+from .exceptions import MultiAgentError, convert_to_status_data
 from .models import (
     AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES,
-    KERNEL_STATUS_TRANSITION_MAP,
-    SESSION_STATUS_TRANSITION_MAP,
+    PRIVATE_KERNEL_ROLES,
     USER_RESOURCE_OCCUPYING_KERNEL_STATUSES,
     AgentRow,
     AgentStatus,
     ImageRow,
+    KernelRole,
     KernelRow,
     KernelStatus,
     KeyPairResourcePolicyRow,
     KeyPairRow,
     SessionDependencyRow,
     SessionRow,
     SessionStatus,
     UserRow,
     agents,
-    determine_session_status,
     handle_session_exception,
     kernels,
     prepare_dotfiles,
     prepare_vfolder_mounts,
     query_allowed_sgroups,
     recalc_agent_resource_occupancy,
     recalc_concurrency_used,
@@ -223,15 +220,15 @@
                 zmq.TCP_KEEPALIVE_CNT: keepalive_retry_count,
             },
         },
         serializer=msgpack.packb,
         deserializer=msgpack.unpackb,
     )
     try:
-        async with (_timeout(invoke_timeout), peer):
+        async with _timeout(invoke_timeout), peer:
             okey_token = peer.call.order_key.set("")
             try:
                 yield peer
             finally:
                 peer.call.order_key.reset(okey_token)
     except RPCUserError as orig_exc:
         raise AgentError(agent_id, orig_exc.name, orig_exc.repr, orig_exc.args)
@@ -244,45 +241,42 @@
     Provide a high-level API to create, destroy, and query the computation
     kernels.
 
     The registry is also responsible to implement our resource management
     policy, such as the limitation of maximum number of kernels per instance.
     """
 
-    kernel_creation_tracker: Dict[KernelId, asyncio.Future]
-    _post_kernel_creation_tasks: weakref.WeakValueDictionary[KernelId, asyncio.Task]
-    _post_kernel_creation_infos: dict[KernelId, asyncio.Future]
     _kernel_actual_allocated_resources: dict[KernelId, ResourceSlot]
 
     def __init__(
         self,
         shared_config: SharedConfig,
         db: ExtendedAsyncSAEngine,
         redis_stat: RedisConnectionInfo,
         redis_live: RedisConnectionInfo,
         redis_image: RedisConnectionInfo,
         event_dispatcher: EventDispatcher,
         event_producer: EventProducer,
         storage_manager: StorageSessionManager,
         hook_plugin_ctx: HookPluginContext,
+        *,
+        debug: bool = False,
     ) -> None:
         self.shared_config = shared_config
         self.docker = aiodocker.Docker()
         self.db = db
         self.redis_stat = redis_stat
         self.redis_live = redis_live
         self.redis_image = redis_image
         self.event_dispatcher = event_dispatcher
         self.event_producer = event_producer
         self.storage_manager = storage_manager
         self.hook_plugin_ctx = hook_plugin_ctx
-        self.kernel_creation_tracker = {}
-        self._post_kernel_creation_tasks = weakref.WeakValueDictionary()
-        self._post_kernel_creation_infos = {}
         self._kernel_actual_allocated_resources = {}
+        self.debug = debug
         self.rpc_keepalive_timeout = int(
             shared_config.get("config/network/rpc/keepalive-timeout", "60")
         )
 
     async def init(self) -> None:
         self.heartbeat_lock = asyncio.Lock()
 
@@ -302,15 +296,15 @@
             return row
 
     async def enumerate_instances(self, check_shadow=True):
         async with self.db.begin_readonly() as conn:
             query = sa.select("*").select_from(agents)
             if check_shadow:
                 query = query.where(agents.c.status == AgentStatus.ALIVE)
-            async for row in (await conn.stream(query)):
+            async for row in await conn.stream(query):
                 yield row
 
     async def update_instance(self, inst_id, updated_fields):
         async def _update() -> None:
             async with self.db.begin() as conn:
                 query = sa.update(agents).values(**updated_fields).where(agents.c.id == inst_id)
                 await conn.execute(query)
@@ -352,14 +346,15 @@
         access_key: AccessKey,
         session_enqueue_configs: SessionEnqueueingConfig,
         scaling_group: Optional[str],
         session_type: SessionTypes,
         resource_policy: dict,
         *,
         user_scope: UserScope,
+        public_sgroup_only: bool = True,
         cluster_mode: ClusterMode = ClusterMode.SINGLE_NODE,
         cluster_size: int = 1,
         session_tag: str = None,
         internal_data: dict = None,
         starts_at: datetime = None,
         agent_list: Sequence[str] = None,
         dependency_sessions: Sequence[SessionId] = None,
@@ -374,32 +369,37 @@
         main_kernel_config = kernel_enqueue_configs[0]
         assert main_kernel_config["cluster_role"] == DEFAULT_ROLE
         session_creation_config: Mapping = session_enqueue_configs["creation_config"]
 
         # Check keypair resource limit
         if cluster_size > int(resource_policy["max_containers_per_session"]):
             raise QuotaExceeded(
-                f"You cannot create session with more than "
-                f"{resource_policy['max_containers_per_session']} containers.",
+                (
+                    "You cannot create session with more than "
+                    f"{resource_policy['max_containers_per_session']} containers."
+                ),
             )
 
         async with self.db.begin_readonly() as conn:
             checked_scaling_group = await check_scaling_group(
                 conn,
                 scaling_group,
                 session_type,
                 access_key,
                 user_scope.domain_name,
                 user_scope.group_id,
+                public_sgroup_only,
             )
             if scaling_group is None:
                 log.warning(
-                    f"enqueue_session(s:{session_name}, ak:{access_key}): "
-                    f"The client did not specify the scaling group for session; "
-                    f"falling back to {checked_scaling_group}",
+                    (
+                        f"enqueue_session(s:{session_name}, ak:{access_key}): "
+                        "The client did not specify the scaling group for session; "
+                        f"falling back to {checked_scaling_group}"
+                    ),
                 )
 
             use_host_network_query = (
                 sa.select([scaling_groups.c.use_host_network])
                 .select_from(scaling_groups)
                 .where(scaling_groups.c.name == checked_scaling_group)
             )
@@ -577,15 +577,15 @@
                 except ValueError:
                     log.exception("request_slots & image_slots calculation error")
                     # happens when requested_slots have more keys
                     # than the image-defined slots
                     # (e.g., image does not support accelerators
                     #  requested by the client)
                     raise InvalidAPIParameters(
-                        "Your resource request has resource type(s) " "not supported by the image."
+                        "Your resource request has resource type(s) not supported by the image."
                     )
 
                 # If intrinsic resources are not specified,
                 # fill them with image minimums.
                 for k, v in requested_slots.items():
                     if (v is None or v == 0) and k in INTRINSIC_SLOTS:
                         requested_slots[k] = image_min_slots[k]
@@ -608,18 +608,18 @@
                         "cpu": cpu,
                         "mem": mem,
                     },
                     known_slot_types,
                 )
                 gpu = creation_config.get("instanceGPUs")
                 if gpu is not None:
-                    raise InvalidAPIParameters("Client upgrade required " "to use GPUs (v19.03+).")
+                    raise InvalidAPIParameters("Client upgrade required to use GPUs (v19.03+).")
                 tpu = creation_config.get("instanceTPUs")
                 if tpu is not None:
-                    raise InvalidAPIParameters("Client upgrade required " "to use TPUs (v19.03+).")
+                    raise InvalidAPIParameters("Client upgrade required to use TPUs (v19.03+).")
 
             # Check the image resource slots.
             log_fmt = "s:{} k:{} r:{}-{}"
             log_args = (session_id, kernel_id, kernel["cluster_role"], kernel["cluster_idx"])
             log.debug(log_fmt + " -> requested_slots: {}", *log_args, requested_slots)
             log.debug(log_fmt + " -> resource_opts: {}", *log_args, resource_opts)
             log.debug(log_fmt + " -> image_min_slots: {}", *log_args, image_min_slots)
@@ -673,21 +673,24 @@
                 {
                     **kernel_shared_data,
                     "id": kernel_id,
                     "agent": mapped_agent,
                     "cluster_role": kernel["cluster_role"],
                     "cluster_idx": kernel["cluster_idx"],
                     "local_rank": kernel["local_rank"],
-                    "cluster_hostname": f"{kernel['cluster_role']}{kernel['cluster_idx']}"
-                    if not kernel["cluster_hostname"]
-                    else kernel["cluster_hostname"],
+                    "cluster_hostname": (
+                        f"{kernel['cluster_role']}{kernel['cluster_idx']}"
+                        if not kernel["cluster_hostname"]
+                        else kernel["cluster_hostname"]
+                    ),
                     "image": image_ref.canonical,
                     # "image_id": image_row.id,
                     "architecture": image_ref.architecture,
                     "registry": image_ref.registry,
+                    "role": KernelRole(image_row.labels.get("ai.backend.role", KernelRole.COMPUTE)),
                     "startup_command": kernel.get("startup_command"),
                     "occupied_slots": requested_slots,
                     "requested_slots": requested_slots,
                     "resource_opts": resource_opts,
                     "environ": [f"{k}={v}" for k, v in environ.items()],
                     "bootstrap_script": kernel.get("bootstrap_script"),
                     "preopen_ports": creation_config.get("preopen_ports", []),
@@ -764,15 +767,14 @@
                     agent_addr=k.agent_addr,
                     scaling_group=scheduled_session.scaling_group,
                 ),
                 allocated_host_ports=set(),
             )
             for k in scheduled_session.kernels
         ]
-        session_creation_id = scheduled_session.creation_id
 
         hook_result = await self.hook_plugin_ctx.dispatch(
             "PRE_START_SESSION",
             (
                 scheduled_session.id,
                 scheduled_session.name,
                 scheduled_session.access_key,
@@ -931,19 +933,19 @@
                 "BACKENDAI_CLUSTER_REPLICAS": ",".join(f"{k}:{v}" for k, v in replicas.items()),
                 "BACKENDAI_CLUSTER_HOSTS": ",".join(
                     binding.kernel.cluster_hostname for binding in kernel_agent_bindings
                 ),
                 "BACKENDAI_ACCESS_KEY": scheduled_session.access_key,
                 # BACKENDAI_SERVICE_PORTS are set as per-kernel env-vars.
                 # (In the future, each kernel in a cluster session may use different images)
-                "BACKENDAI_PREOPEN_PORTS": ",".join(
-                    str(port) for port in scheduled_session.main_kernel.preopen_ports
-                )
-                if scheduled_session.main_kernel.preopen_ports is not None
-                else "",
+                "BACKENDAI_PREOPEN_PORTS": (
+                    ",".join(str(port) for port in scheduled_session.main_kernel.preopen_ports)
+                    if scheduled_session.main_kernel.preopen_ports is not None
+                    else ""
+                ),
             }
         )
 
         # Aggregate by agents to minimize RPC calls
         per_agent_tasks = []
         keyfunc = lambda item: item.agent_alloc_ctx.agent_id
         for agent_id, group_iterator in itertools.groupby(
@@ -976,29 +978,17 @@
                     agent_errors.extend(result.__errors__)
                 elif isinstance(result, Exception):
                     # mark to be destroyed afterwards
                     agent_errors.append(result)
             if agent_errors:
                 raise MultiAgentError(
                     "agent(s) raise errors during kernel creation",
-                    errors=agent_errors,
+                    agent_errors,
                 )
             await self.settle_agent_alloc(kernel_agent_bindings)
-        # If all is well, let's say the session is ready.
-        await self.event_producer.produce_event(
-            SessionStartedEvent(scheduled_session.id, session_creation_id),
-        )
-        await self.hook_plugin_ctx.notify(
-            "POST_START_SESSION",
-            (
-                scheduled_session.id,
-                scheduled_session.name,
-                scheduled_session.access_key,
-            ),
-        )
 
     def convert_resource_spec_to_resource_slot(
         self,
         allocations: Mapping[str, Mapping[SlotName, Mapping[DeviceId, str]]],
     ) -> ResourceSlot:
         """
         Convert per-device resource spec allocations (agent-side format)
@@ -1015,180 +1005,117 @@
                     ):
                         total_allocs.append(Decimal(BinarySize.from_str(allocation)))
                     else:  # maybe Decimal("Infinity"), etc.
                         total_allocs.append(Decimal(allocation))
                 slots[slot_name] = str(sum(total_allocs))
         return slots
 
-    async def finalize_running(self, created_info: Mapping[str, Any]) -> None:
-        async def _finalize_running() -> Optional[SessionId]:
-            # Record kernel access information
-            try:
-                async with self.db.begin() as conn:
-                    kernel_query = (
-                        sa.select(kernels.c.status)
-                        .where(kernels.c.id == created_info["id"])
-                        .with_for_update(skip_locked=True)
-                    )
-                    current_status = (await conn.execute(kernel_query)).scalar()
-                    # current_status is None when kernel_query is locked by concurrent query.
-                    if (
-                        current_status is None
-                        or KernelStatus.RUNNING not in KERNEL_STATUS_TRANSITION_MAP[current_status]
-                    ):
-                        return None
-                    agent_host = URL(created_info["agent_addr"]).host
-                    kernel_host = created_info.get("kernel_host", agent_host)
-                    service_ports = created_info.get("service_ports", [])
-                    # NOTE: created_info contains resource_spec
-                    values = {
-                        "scaling_group": created_info["scaling_group"],
-                        "status": KernelStatus.RUNNING,
-                        "container_id": created_info["container_id"],
-                        "occupied_shares": {},
-                        "attached_devices": created_info.get("attached_devices", {}),
-                        "kernel_host": kernel_host,
-                        "repl_in_port": created_info["repl_in_port"],
-                        "repl_out_port": created_info["repl_out_port"],
-                        "stdin_port": created_info["stdin_port"],
-                        "stdout_port": created_info["stdout_port"],
-                        "service_ports": service_ports,
-                        "status_history": sql_json_merge(
-                            kernels.c.status_history,
-                            (),
-                            {
-                                KernelStatus.RUNNING.name: datetime.now(tzutc()).isoformat(),
-                            },
-                        ),
-                    }
-                    actual_allocs = self.convert_resource_spec_to_resource_slot(
-                        created_info["resource_spec"]["allocations"]
-                    )
-                    values["occupied_slots"] = actual_allocs
-                    self._kernel_actual_allocated_resources[created_info["id"]] = actual_allocs
-                    update_query = (
-                        sa.update(kernels)
-                        .values(values)
-                        .where(kernels.c.id == created_info["id"])
-                        .returning(kernels.c.session_id)
-                    )
-                    return (await conn.execute(update_query)).first()["session_id"]
-            except Exception:
-                log.exception("error while executing _finalize_running")
-                raise
-
-        session_id = await execute_with_retry(_finalize_running)
-        if session_id is None:
-            return None
+    async def finalize_running(
+        self, kernel_id: KernelId, session_id: SessionId, created_info: Mapping[str, Any]
+    ) -> None:
+        try:
+            agent_host = URL(created_info["agent_addr"]).host
+            kernel_host = created_info.get("kernel_host", agent_host)
+            service_ports = created_info.get("service_ports", [])
+            actual_allocs = self.convert_resource_spec_to_resource_slot(
+                created_info["resource_spec"]["allocations"]
+            )
+            new_status = KernelStatus.RUNNING
+            update_data = {
+                "occupied_slots": actual_allocs,
+                "scaling_group": created_info["scaling_group"],
+                "container_id": created_info["container_id"],
+                "occupied_shares": {},
+                "attached_devices": created_info.get("attached_devices", {}),
+                "kernel_host": kernel_host,
+                "repl_in_port": created_info["repl_in_port"],
+                "repl_out_port": created_info["repl_out_port"],
+                "stdin_port": created_info["stdin_port"],
+                "stdout_port": created_info["stdout_port"],
+                "service_ports": service_ports,
+                "status_history": sql_json_merge(
+                    kernels.c.status_history,
+                    (),
+                    {
+                        new_status.name: datetime.now(tzutc()).isoformat(),
+                    },
+                ),
+            }
+            self._kernel_actual_allocated_resources[kernel_id] = actual_allocs
+            kernel_did_update = await KernelRow.update_kernel(
+                self.db, kernel_id, new_status, update_data=update_data
+            )
+            if not kernel_did_update:
+                return
 
-        async def _check_session() -> None:
-            async with self.db.begin_session() as db_sess:
-                query = (
-                    sa.select(SessionRow)
-                    .where(SessionRow.id == session_id)
-                    .options(selectinload(SessionRow.kernels))
-                )
-                result = await db_sess.execute(query)
-                session: SessionRow = result.scalars().first()
-                candidate_status = determine_session_status(session.kernels)
-                if candidate_status in SESSION_STATUS_TRANSITION_MAP[session.status]:
-                    update_query = (
-                        sa.update(SessionRow)
-                        .where(SessionRow.id == session_id)
-                        .values(
-                            status=candidate_status,
-                            status_history=sql_json_merge(
-                                SessionRow.status_history,
-                                (),
-                                {
-                                    SessionStatus.RUNNING.name: datetime.now(tzutc()).isoformat(),
-                                },
-                            ),
-                        )
-                    )
-                    await db_sess.execute(update_query)
+            new_session_status = await SessionRow.transit_session_status(self.db, session_id)
+            if new_session_status is None or new_session_status != SessionStatus.RUNNING:
+                return
 
-        await execute_with_retry(_check_session)
+            updated_session = await SessionRow.get_session_to_produce_event(self.db, session_id)
 
-    async def _post_create_kernel(
-        self,
-        agent_alloc_ctx: AgentAllocationContext,
-        kernel_id: KernelId,
-    ) -> None:
-        # Wait until the kernel_started event.
-        try:
-            created_info, _ = await asyncio.gather(
-                self._post_kernel_creation_infos[kernel_id],
-                self.kernel_creation_tracker[kernel_id],
+            await self.event_producer.produce_event(
+                SessionStartedEvent(updated_session.id, updated_session.creation_id),
             )
-        except asyncio.CancelledError:
-            log.warning("post_create_kernel(k:{}) cancelled", kernel_id)
-            return
-        except Exception:
-            log.exception("post_create_kernel(k:{}) unexpected error", kernel_id)
-            return
-        else:
-            await self.finalize_running(
-                {
-                    **created_info,
-                    "scaling_group": agent_alloc_ctx.scaling_group,
-                    "agent_addr": agent_alloc_ctx.agent_addr,
-                }
+            await self.hook_plugin_ctx.notify(
+                "POST_START_SESSION",
+                (
+                    updated_session.id,
+                    updated_session.name,
+                    updated_session.access_key,
+                ),
             )
-
-        finally:
-            try:
-                await asyncio.sleep(1)
-            finally:
-                del self._post_kernel_creation_infos[kernel_id]
-                del self.kernel_creation_tracker[kernel_id]
+        except Exception:
+            log.exception("error while executing _finalize_running")
+            raise
 
     async def _create_kernels_in_one_agent(
         self,
         agent_alloc_ctx: AgentAllocationContext,
         scheduled_session: SessionRow,
         items: Sequence[KernelAgentBinding],
         image_info: Mapping[str, Any],
         cluster_info,
     ) -> None:
-        loop = asyncio.get_running_loop()
         registry_url = image_info["registry_url"]
         registry_creds = image_info["registry_creds"]
         image_infos = image_info["image_infos"]
         is_local = image_info["is_local"]
         resource_policy: KeyPairResourcePolicyRow = image_info["resource_policy"]
         auto_pull = image_info["auto_pull"]
         assert agent_alloc_ctx.agent_id is not None
         assert scheduled_session.id is not None
+
+        async def _update_kernel() -> None:
+            async with self.db.begin_session() as db_sess:
+                kernel_query = (
+                    sa.update(KernelRow)
+                    .where(KernelRow.id.in_([binding.kernel.id for binding in items]))
+                    .values(
+                        agent=agent_alloc_ctx.agent_id,
+                        agent_addr=agent_alloc_ctx.agent_addr,
+                        scaling_group=agent_alloc_ctx.scaling_group,
+                    )
+                )
+                await db_sess.execute(kernel_query)
+
+        await execute_with_retry(_update_kernel)
+
         async with RPCContext(
             agent_alloc_ctx.agent_id,
             agent_alloc_ctx.agent_addr,
             invoke_timeout=None,
             order_key=str(scheduled_session.id),
             keepalive_timeout=self.rpc_keepalive_timeout,
         ) as rpc:
-            # Prepare kernel_started event handling
-            for binding in items:
-                self.kernel_creation_tracker[binding.kernel.id] = loop.create_future()
-            # Spawn post-processing tasks
-            post_tasks = []
-            for binding in items:
-                self._post_kernel_creation_infos[binding.kernel.id] = loop.create_future()
-                post_task = asyncio.create_task(
-                    self._post_create_kernel(
-                        agent_alloc_ctx,
-                        binding.kernel.id,
-                    )
-                )
-                self._post_kernel_creation_tasks[binding.kernel.id] = post_task
-                post_tasks.append(post_task)
             try:
                 get_image_ref = lambda k: image_infos[str(k.image_ref)].image_ref
                 # Issue a batched RPC call to create kernels on this agent
-                created_infos = await rpc.call.create_kernels(
+                # created_infos = await rpc.call.create_kernels(
+                await rpc.call.create_kernels(
                     str(scheduled_session.id),
                     [str(binding.kernel.id) for binding in items],
                     [
                         {
                             "image": {
                                 # TODO: refactor registry and is_local to be specified per kernel.
                                 "registry": {
@@ -1244,70 +1171,49 @@
                 log.debug(
                     "start_session(s:{}, ak:{}, k:{}) -> created on ag:{}",
                     scheduled_session.name,
                     scheduled_session.access_key,
                     [binding.kernel.id for binding in items],
                     agent_alloc_ctx.agent_id,
                 )
-                # Pass the return value of RPC calls to post-processing tasks
-                for created_info in created_infos:
-                    kernel_id = KernelId(uuid.UUID(created_info["id"]))
-                    self._post_kernel_creation_infos[kernel_id].set_result(created_info)
-                await asyncio.gather(*post_tasks, return_exceptions=True)
-            except (asyncio.TimeoutError, asyncio.CancelledError) as e:
-                for binding in items:
-                    kernel_id = binding.kernel.kernel_id
-                    if not self.kernel_creation_tracker[kernel_id].done():
-                        self.kernel_creation_tracker[kernel_id].cancel()
-                        self._post_kernel_creation_infos[kernel_id].set_exception(e)
-                await asyncio.gather(*post_tasks, return_exceptions=True)
+            except (asyncio.TimeoutError, asyncio.CancelledError):
+                log.warning("_create_kernels_in_one_agent(s:{}) cancelled", scheduled_session.id)
             except Exception as e:
                 # The agent has already cancelled or issued the destruction lifecycle event
                 # for this batch of kernels.
+                ex = e
                 for binding in items:
                     kernel_id = binding.kernel.id
-                    if not self.kernel_creation_tracker[kernel_id].done():
-                        self.kernel_creation_tracker[kernel_id].cancel()
-                        self._post_kernel_creation_infos[kernel_id].set_exception(e)
-                    ex = e
 
                     async def _update_failure() -> None:
                         async with self.db.begin_session() as db_sess:
                             now = datetime.now(tzutc())
                             query = (
                                 sa.update(KernelRow)
                                 .where(KernelRow.id == kernel_id)
-                                .value(
+                                .values(
                                     status=KernelStatus.ERROR,
                                     status_info=f"other-error ({ex!r})",
                                     status_changed=now,
                                     terminated_at=now,
                                     status_history=sql_json_merge(
                                         KernelRow.status_history,
                                         (),
                                         {
-                                            KernelStatus.ERROR.name: now.isoformat(),  # ["PULLING", "PREPARING"]
+                                            KernelStatus.ERROR.name: (
+                                                now.isoformat()
+                                            ),  # ["PULLING", "PREPARING"]
                                         },
                                     ),
-                                    agent=binding.agent_alloc_ctx.agent_id,
-                                    agent_addr=binding.agent_alloc_ctx.agent_addr,
-                                    scaling_group=binding.agent_alloc_ctx.scaling_group,
-                                    status_data={
-                                        "error": {
-                                            "src": "other",
-                                            "name": ex.__class__.__name__,
-                                            "repr": repr(ex),
-                                        },
-                                    },
+                                    status_data=convert_to_status_data(ex, self.debug),
                                 )
                             )
                             await db_sess.execute(query)
 
                     await execute_with_retry(_update_failure)
-                await asyncio.gather(*post_tasks, return_exceptions=True)
                 raise
 
     async def create_cluster_ssh_keypair(self) -> ClusterSSHKeyPair:
         key = rsa.generate_private_key(
             backend=default_backend(),
             public_exponent=65537,
             key_size=2048,
@@ -1330,15 +1236,16 @@
     async def get_keypair_occupancy(self, access_key, *, db_sess=None):
         known_slot_types = await self.shared_config.get_resource_slots()
 
         async def _query() -> ResourceSlot:
             async with reenter_txn_session(self.db, db_sess) as _sess:
                 query = sa.select(KernelRow.occupied_slots).where(
                     (KernelRow.access_key == access_key)
-                    & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES)),
+                    & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES))
+                    & (KernelRow.role.not_in(PRIVATE_KERNEL_ROLES)),
                 )
                 zero = ResourceSlot()
                 key_occupied = sum(
                     [row.occupied_slots async for row in (await _sess.stream(query))], zero
                 )
                 # drop no-longer used slot types
                 drops = [k for k in key_occupied.keys() if k not in known_slot_types]
@@ -1352,15 +1259,16 @@
         # TODO: store domain occupied_slots in Redis?
         known_slot_types = await self.shared_config.get_resource_slots()
 
         async def _query() -> ResourceSlot:
             async with reenter_txn_session(self.db, db_sess) as _sess:
                 query = sa.select(KernelRow.occupied_slots).where(
                     (KernelRow.domain_name == domain_name)
-                    & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES)),
+                    & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES))
+                    & (KernelRow.role.not_in(PRIVATE_KERNEL_ROLES)),
                 )
                 zero = ResourceSlot()
                 key_occupied = sum(
                     [row.occupied_slots async for row in (await _sess.stream(query))],
                     zero,
                 )
                 # drop no-longer used slot types
@@ -1375,15 +1283,16 @@
         # TODO: store domain occupied_slots in Redis?
         known_slot_types = await self.shared_config.get_resource_slots()
 
         async def _query() -> ResourceSlot:
             async with reenter_txn_session(self.db, db_sess) as _sess:
                 query = sa.select(KernelRow.occupied_slots).where(
                     (KernelRow.group_id == group_id)
-                    & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES)),
+                    & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES))
+                    & (KernelRow.role.not_in(PRIVATE_KERNEL_ROLES)),
                 )
                 zero = ResourceSlot()
                 key_occupied = sum(
                     [row.occupied_slots async for row in (await _sess.stream(query))],
                     zero,
                 )
                 # drop no-longer used slot types
@@ -1470,29 +1379,34 @@
                 # Query running containers and calculate concurrency_used per AK and
                 # occupied_slots per agent.
                 query = (
                     sa.select([kernels.c.access_key, kernels.c.agent, kernels.c.occupied_slots])
                     .where(kernels.c.status.in_(AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES))
                     .order_by(sa.asc(kernels.c.access_key))
                 )
-                async for row in (await conn.stream(query)):
+                async for row in await conn.stream(query):
                     occupied_slots_per_agent[row.agent] += ResourceSlot(row.occupied_slots)
                 query = (
                     sa.select(
                         [
                             kernels.c.access_key,
                             kernels.c.session_id,
                             kernels.c.agent,
                             kernels.c.occupied_slots,
                         ]
                     )
-                    .where(kernels.c.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES))
+                    .where(
+                        (
+                            kernels.c.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES)
+                            & kernels.c.role.not_in(PRIVATE_KERNEL_ROLES)
+                        )
+                    )
                     .order_by(sa.asc(kernels.c.access_key))
                 )
-                async for row in (await conn.stream(query)):
+                async for row in await conn.stream(query):
                     concurrency_used_per_key[row.access_key].add(row.session_id)
 
                 if len(occupied_slots_per_agent) > 0:
                     # Update occupied_slots for agents with running containers.
                     for aid, slots in occupied_slots_per_agent.items():
                         query = (
                             sa.update(agents).values(occupied_slots=slots).where(agents.c.id == aid)
@@ -1581,14 +1495,15 @@
                 keepalive_timeout=self.rpc_keepalive_timeout,
             ) as rpc:
                 for kernel in destroyed_kernels:
                     # internally it enqueues a "destroy" lifecycle event.
                     rpc_coros.append(
                         rpc.call.destroy_kernel(
                             str(kernel["id"]),
+                            str(session_id),
                             KernelLifecycleEventReason.FAILED_TO_START,
                             suppress_events=True,
                         ),
                     )
                 await asyncio.gather(*rpc_coros)
 
     async def destroy_session(
@@ -1623,34 +1538,30 @@
 
         async with handle_session_exception(
             self.db,
             "destroy_session",
             session_id,
             set_error=True,
         ):
-            async with self.db.begin_readonly_session() as db_sess:
-                query = (
-                    sa.select(SessionRow)
-                    .where(SessionRow.id == session_id)
-                    .options(selectinload(SessionRow.kernels))
-                )
-                result = await db_sess.execute(query)
-                target_session = result.scalars().first()
+            target_session = await SessionRow.get_session_to_destroy(self.db, session_id)
 
             match target_session.status:
                 case SessionStatus.PENDING:
                     await SessionRow.set_session_status(
                         self.db, session_id, SessionStatus.CANCELLED
                     )
                 case SessionStatus.PULLING:
                     raise GenericForbidden("Cannot destroy sessions in pulling status")
                 case SessionStatus.SCHEDULED | SessionStatus.PREPARING | SessionStatus.TERMINATING | SessionStatus.ERROR:
                     if not forced:
                         raise GenericForbidden(
-                            "Cannot destroy sessions in scheduled/preparing/terminating/error status",
+                            (
+                                "Cannot destroy sessions in scheduled/preparing/terminating/error"
+                                " status"
+                            ),
                         )
                     log.warning(
                         "force-terminating session (s:{}, status:{})",
                         session_id,
                         target_session.status,
                     )
                     await SessionRow.set_session_status(
@@ -1680,54 +1591,49 @@
             ):
                 destroyed_kernels = []
                 grouped_kernels = [*group_iterator]
                 kernel: KernelRow
                 for kernel in grouped_kernels:
                     match kernel.status:
                         case KernelStatus.PENDING:
-
-                            async def _update() -> None:
-                                async with self.db.begin_session() as db_sess:
-                                    await db_sess.execute(
-                                        sa.update(KernelRow)
-                                        .values(
-                                            status=KernelStatus.CANCELLED,
-                                            status_info=reason,
-                                            status_changed=now,
-                                            terminated_at=now,
-                                            status_history=sql_json_merge(
-                                                KernelRow.status_history,
-                                                (),
-                                                {
-                                                    KernelStatus.CANCELLED.name: now.isoformat(),
-                                                },
-                                            ),
-                                        )
-                                        .where(KernelRow.id == kernel.id),
-                                    )
-
-                            await execute_with_retry(_update)
+                            await KernelRow.set_kernel_status(
+                                self.db,
+                                kernel.id,
+                                KernelStatus.CANCELLED,
+                                reason=reason,
+                                status_changed_at=now,
+                            )
                             await self.event_producer.produce_event(
-                                KernelCancelledEvent(kernel.id, reason),
+                                KernelCancelledEvent(kernel.id, session_id, reason),
                             )
                             if kernel.cluster_role == DEFAULT_ROLE:
                                 main_stat = {"status": "cancelled"}
+                                await SessionRow.set_session_status(
+                                    self.db,
+                                    kernel.session_id,
+                                    SessionStatus.CANCELLED,
+                                    reason=reason,
+                                    status_changed_at=now,
+                                )
                                 await self.event_producer.produce_event(
                                     SessionCancelledEvent(
                                         kernel.session_id,
                                         kernel.session_creation_id,
                                         reason,
                                     ),
                                 )
                         case KernelStatus.PULLING:
                             raise GenericForbidden("Cannot destroy kernels in pulling status")
                         case KernelStatus.SCHEDULED | KernelStatus.PREPARING | KernelStatus.TERMINATING | KernelStatus.ERROR:
                             if not forced:
                                 raise GenericForbidden(
-                                    "Cannot destroy kernels in scheduled/preparing/terminating/error status",
+                                    (
+                                        "Cannot destroy kernels in"
+                                        " scheduled/preparing/terminating/error status"
+                                    ),
                                 )
                             log.warning(
                                 "force-terminating kernel (k:{}, status:{})",
                                 kernel.id,
                                 kernel.status,
                             )
                             if kernel.container_id is not None:
@@ -1758,28 +1664,31 @@
                                         values["last_stat"] = msgpack.unpackb(kern_stat)
                                     await db_sess.execute(
                                         sa.update(KernelRow)
                                         .values(**values)
                                         .where(KernelRow.id == kernel.id),
                                     )
 
-                            if kernel.cluster_role == DEFAULT_ROLE:
+                            if (
+                                kernel.cluster_role == DEFAULT_ROLE
+                                and kernel.role not in PRIVATE_KERNEL_ROLES
+                            ):
                                 # The main session is terminated;
                                 # decrement the user's concurrency counter
                                 await redis_helper.execute(
                                     self.redis_stat,
                                     lambda r: r.incrby(
                                         f"keypair.concurrency_used.{kernel.access_key}",
                                         -1,
                                     ),
                                 )
 
                             await execute_with_retry(_update)
                             await self.event_producer.produce_event(
-                                KernelTerminatedEvent(kernel.id, reason),
+                                KernelTerminatedEvent(kernel.id, target_session.id, reason),
                             )
                         case _:
 
                             async def _update() -> None:
                                 async with self.db.begin_session() as db_sess:
                                     values = {
                                         "status": KernelStatus.TERMINATING,
@@ -1799,28 +1708,31 @@
                                     }
                                     await db_sess.execute(
                                         sa.update(KernelRow)
                                         .values(**values)
                                         .where(KernelRow.id == kernel.id),
                                     )
 
-                            if kernel.cluster_role == DEFAULT_ROLE:
+                            if (
+                                kernel.cluster_role == DEFAULT_ROLE
+                                and kernel.role not in PRIVATE_KERNEL_ROLES
+                            ):
                                 # The main session is terminated;
                                 # decrement the user's concurrency counter
                                 await redis_helper.execute(
                                     self.redis_stat,
                                     lambda r: r.incrby(
                                         f"keypair.concurrency_used.{kernel.access_key}",
                                         -1,
                                     ),
                                 )
 
                             await execute_with_retry(_update)
                             await self.event_producer.produce_event(
-                                KernelTerminatingEvent(kernel.id, reason),
+                                KernelTerminatingEvent(kernel.id, target_session.id, reason),
                             )
 
                     if kernel.agent_addr is None:
                         await self.mark_kernel_terminated(kernel.id, "missing-agent-allocation")
                         if kernel.cluster_role == DEFAULT_ROLE:
                             main_stat = {"status": "terminated"}
                     else:
@@ -1838,15 +1750,17 @@
                         keepalive_timeout=self.rpc_keepalive_timeout,
                     ) as rpc:
                         rpc_coros = []
                         for kernel in destroyed_kernels:
                             # internally it enqueues a "destroy" lifecycle event.
                             if kernel.status != KernelStatus.SCHEDULED:
                                 rpc_coros.append(
-                                    rpc.call.destroy_kernel(str(kernel.id), reason),
+                                    rpc.call.destroy_kernel(
+                                        str(kernel.id), str(session.id), reason
+                                    ),
                                 )
                         try:
                             await asyncio.gather(*rpc_coros)
                         except Exception:
                             log.exception(
                                 "destroy_kernels_in_agent(a:{}, s:{}): unexpected error",
                                 destroyed_kernels[0].agent,
@@ -1874,15 +1788,15 @@
                     per_agent_tasks.append(_destroy_kernels_in_agent(session, destroyed_kernels))
                     to_be_terminated.extend(destroyed_kernels)
 
             if per_agent_tasks:
                 await asyncio.gather(*per_agent_tasks, return_exceptions=True)
             for kernel in to_be_terminated:
                 await self.event_producer.produce_event(
-                    KernelTerminatedEvent(kernel.id, reason),
+                    KernelTerminatedEvent(kernel.id, target_session.id, reason),
                 )
             await self.hook_plugin_ctx.notify(
                 "POST_DESTROY_SESSION",
                 (session_id, session.name, session.access_key),
             )
             if forced:
                 await self.recalc_resource_usage()
@@ -1974,98 +1888,65 @@
                 await db_sess.execute(query)
 
         await execute_with_retry(_restarting_session)
 
         kernel_list = session.kernels
 
         async def _restart_kernel(kernel: KernelRow) -> None:
-            loop = asyncio.get_running_loop()
             try:
-                start_future = loop.create_future()
-                self.kernel_creation_tracker[kernel.id] = start_future
-                try:
-                    async with RPCContext(
-                        kernel.agent,  # the main-container's agent
-                        kernel.agent_addr,
-                        invoke_timeout=None,
-                        order_key=None,
-                        keepalive_timeout=self.rpc_keepalive_timeout,
-                    ) as rpc:
-                        updated_config: Dict[str, Any] = {
-                            # TODO: support resacling of sub-containers
-                        }
-                        kernel_info = await rpc.call.restart_kernel(
-                            str(kernel.session_id),
-                            str(kernel.id),
-                            updated_config,
-                        )
-                    await start_future
-
-                    async def _update_kernel() -> None:
-                        async with self.db.begin_session() as db_sess:
-                            query = (
-                                sa.update(KernelRow)
-                                .values(
-                                    status=KernelStatus.RUNNING,
-                                    container_id=kernel_info["container_id"],
-                                    repl_in_port=kernel_info["repl_in_port"],
-                                    repl_out_port=kernel_info["repl_out_port"],
-                                    stdin_port=kernel_info["stdin_port"],
-                                    stdout_port=kernel_info["stdout_port"],
-                                    service_ports=kernel_info.get("service_ports", []),
-                                    status_history=sql_json_merge(
-                                        KernelRow.status_history,
-                                        (),
-                                        {
-                                            KernelStatus.RUNNING.name: datetime.now(
-                                                tzutc()
-                                            ).isoformat(),
-                                        },
-                                    ),
-                                )
-                                .where(KernelRow.id == kernel.id)
-                            )
-                            await db_sess.execute(query)
+                async with RPCContext(
+                    kernel.agent,  # the main-container's agent
+                    kernel.agent_addr,
+                    invoke_timeout=None,
+                    order_key=None,
+                    keepalive_timeout=self.rpc_keepalive_timeout,
+                ) as rpc:
+                    updated_config: Dict[str, Any] = {
+                        # TODO: support resacling of sub-containers
+                    }
+                    kernel_info = await rpc.call.restart_kernel(
+                        str(kernel.session_id),
+                        str(kernel.id),
+                        updated_config,
+                    )
 
-                    await execute_with_retry(_update_kernel)
-                finally:
-                    del self.kernel_creation_tracker[kernel.id]
+                now = datetime.now(tzutc())
+                update_data = {
+                    "container_id": kernel_info["container_id"],
+                    "repl_in_port": kernel_info["repl_in_port"],
+                    "repl_out_port": kernel_info["repl_out_port"],
+                    "stdin_port": kernel_info["stdin_port"],
+                    "stdout_port": kernel_info["stdout_port"],
+                    "service_ports": kernel_info.get("service_ports", []),
+                    "status_history": sql_json_merge(
+                        KernelRow.status_history,
+                        (),
+                        {
+                            KernelStatus.RUNNING.name: now.isoformat(),
+                        },
+                    ),
+                }
+                await KernelRow.update_kernel(
+                    self.db, kernel.id, KernelStatus.RUNNING, update_data=update_data
+                )
             except Exception:
                 log.exception("unexpected-error in _restart_kerenl()")
 
         restart_coros = []
         for kernel in kernel_list:
             restart_coros.append(_restart_kernel(kernel))
         async with handle_session_exception(
             self.db,
             "restart_session",
             session.id,
             set_error=True,
         ):
             await asyncio.gather(*restart_coros)
 
-        async def _update_session() -> None:
-            async with self.db.begin_session() as db_sess:
-                query = (
-                    sa.update(SessionRow)
-                    .values(
-                        status=SessionStatus.RUNNING,
-                        status_history=sql_json_merge(
-                            SessionRow.status_history,
-                            (),
-                            {
-                                SessionStatus.RUNNING.name: datetime.now(tzutc()).isoformat(),
-                            },
-                        ),
-                    )
-                    .where(SessionRow.id == session.id)
-                )
-                await db_sess.execute(query)
-
-        await execute_with_retry(_update_session)
+        await SessionRow.set_session_status(self.db, session.id, SessionStatus.RUNNING)
 
         # NOTE: If the restarted session is a batch-type one, then the startup command
         #       will be executed again after restart.
         await self.event_producer.produce_event(
             SessionStartedEvent(session.id, session.creation_id),
         )
 
@@ -2309,14 +2190,15 @@
                 nonlocal instance_rejoin
                 async with self.db.begin() as conn:
                     fetch_query = (
                         sa.select(
                             [
                                 agents.c.status,
                                 agents.c.addr,
+                                agents.c.public_host,
                                 agents.c.scaling_group,
                                 agents.c.available_slots,
                                 agents.c.version,
                                 agents.c.compute_plugins,
                                 agents.c.architecture,
                             ]
                         )
@@ -2336,14 +2218,15 @@
                                 "id": agent_id,
                                 "status": AgentStatus.ALIVE,
                                 "region": agent_info["region"],
                                 "scaling_group": sgroup,
                                 "available_slots": available_slots,
                                 "occupied_slots": {},
                                 "addr": agent_info["addr"],
+                                "public_host": agent_info["public_host"],
                                 "first_contact": now,
                                 "lost_at": sa.null(),
                                 "version": agent_info["version"],
                                 "compute_plugins": agent_info["compute_plugins"],
                                 "architecture": agent_info.get("architecture", "x86_64"),
                             }
                         )
@@ -2353,14 +2236,16 @@
                         updates = {}
                         if row["available_slots"] != available_slots:
                             updates["available_slots"] = available_slots
                         if row["scaling_group"] != sgroup:
                             updates["scaling_group"] = sgroup
                         if row["addr"] != current_addr:
                             updates["addr"] = current_addr
+                        if row["public_host"] != agent_info["public_host"]:
+                            updates["public_host"] = agent_info["public_host"]
                         if row["version"] != agent_info["version"]:
                             updates["version"] = agent_info["version"]
                         if row["compute_plugins"] != agent_info["compute_plugins"]:
                             updates["compute_plugins"] = agent_info["compute_plugins"]
                         if row["architecture"] != agent_info["architecture"]:
                             updates["architecture"] = agent_info["architecture"]
                         # occupied_slots are updated when kernels starts/terminates
@@ -2377,14 +2262,15 @@
                             sa.update(agents)
                             .values(
                                 {
                                     "status": AgentStatus.ALIVE,
                                     "region": agent_info["region"],
                                     "scaling_group": sgroup,
                                     "addr": agent_info["addr"],
+                                    "public_host": agent_info["public_host"],
                                     "lost_at": sa.null(),
                                     "available_slots": available_slots,
                                     "version": agent_info["version"],
                                     "compute_plugins": agent_info["compute_plugins"],
                                     "architecture": agent_info["architecture"],
                                 }
                             )
@@ -2517,28 +2403,21 @@
         reason: str,
         exit_code: int = None,
     ) -> None:
         """
         Mark the kernel (individual worker) terminated and release
         the resource slots occupied by it.
         """
-        post_task = self._post_kernel_creation_tasks.get(kernel_id, None)
-        if post_task is not None and not post_task.done():
-            post_task.cancel()
-            try:
-                await post_task
-            except asyncio.CancelledError:
-                pass
 
         kern_stat = await redis_helper.execute(
             self.redis_stat,
             lambda r: r.get(str(kernel_id)),
         )
 
-        async def _update_kernel_status() -> Tuple[SessionId, AccessKey, AgentId] | None:
+        async def _update_kernel() -> tuple[AccessKey, AgentId] | None:
             async with self.db.begin_session() as db_sess:
                 # Check the current status.
                 select_query = (
                     sa.select(
                         KernelRow.access_key,
                         KernelRow.agent,
                         KernelRow.status,
@@ -2554,15 +2433,14 @@
                     KernelStatus.CANCELLED,
                     KernelStatus.TERMINATED,
                     KernelStatus.RESTARTING,
                 ):
                     # Skip if non-existent, already terminated, or restarting.
                     return None
 
-                session_id, access_key, agent = kernel.session_id, kernel.access_key, kernel.agent
                 # Change the status to TERMINATED.
                 # (we don't delete the row for later logging and billing)
                 now = datetime.now(tzutc())
                 values = {
                     "status": KernelStatus.TERMINATED,
                     "status_info": reason,
                     "status_changed": now,
@@ -2582,22 +2460,22 @@
                 }
                 if kern_stat:
                     values["last_stat"] = msgpack.unpackb(kern_stat)
                 update_query = (
                     sa.update(KernelRow).values(**values).where(KernelRow.id == kernel_id)
                 )
                 await db_sess.execute(update_query)
-                return session_id, access_key, agent
+                return kernel.access_key, kernel.agent
 
-        result = await execute_with_retry(_update_kernel_status)
+        result = await execute_with_retry(_update_kernel)
 
         if result is None:
             return
 
-        session_id, access_key, agent = result
+        access_key, agent = result
 
         async def _recalc() -> None:
             async with self.db.begin() as conn:
                 log.debug(
                     "recalculate concurrency used in kernel termination (ak: {})",
                     access_key,
                 )
@@ -2606,93 +2484,31 @@
                     "recalculate agent resource occupancy in kernel termination (agent: {})",
                     agent,
                 )
                 await recalc_agent_resource_occupancy(conn, agent)
 
         await execute_with_retry(_recalc)
 
-        async def _check_session() -> None:
-            async with self.db.begin_session() as db_sess:
-                query = (
-                    sa.select(SessionRow)
-                    .where(SessionRow.id == session_id)
-                    .options(selectinload(SessionRow.kernels))
-                )
-                result = await db_sess.execute(query)
-                session: SessionRow = result.scalars().first()
-                candidate_status = determine_session_status(session.kernels)
-                if candidate_status in SESSION_STATUS_TRANSITION_MAP[session.status]:
-                    now = datetime.now(tzutc())
-                    update_query = (
-                        sa.update(SessionRow)
-                        .where(SessionRow.id == session_id)
-                        .values(
-                            status=candidate_status,
-                            terminated_at=now,
-                            status_history=sql_json_merge(
-                                SessionRow.status_history,
-                                (),
-                                {
-                                    SessionStatus.TERMINATED.name: datetime.now(
-                                        tzutc()
-                                    ).isoformat(),
-                                },
-                            ),
-                        )
-                    )
-                    await db_sess.execute(update_query)
-
-        await execute_with_retry(_check_session)
-
         # Perform statistics sync in a separate transaction block, since
         # it may take a while to fetch stats from Redis.
 
         await self.sync_kernel_stats([kernel_id])
 
     async def check_session_terminated(
         self,
-        kernel_id: KernelId,
+        session_id: SessionId,
         reason: str,
     ) -> None:
-        async def _check_and_mark() -> Tuple[bool, SessionId]:
-            async with self.db.begin_session() as db_sess:
-                kernel_query = sa.select(KernelRow.session_id).where(KernelRow.id == kernel_id)
-                session_id = (await db_sess.execute(kernel_query)).scalar()
-                session = await SessionRow.get_session_with_kernels(
-                    session_id, allow_stale=True, db_session=db_sess
-                )
-                sibling_kernels = session.kernels
-                sess_status = determine_session_status(sibling_kernels)
-                now = datetime.now(tzutc())
-                if sess_status in SESSION_STATUS_TRANSITION_MAP[session.status]:
-                    values = {
-                        "status": sess_status,
-                        "status_info": reason,
-                        "terminated_at": now,
-                        "status_history": sql_json_merge(
-                            SessionRow.status_history,
-                            (),
-                            {
-                                sess_status.name: datetime.now(tzutc()).isoformat(),
-                            },
-                        ),
-                    }
-                    query = (
-                        sa.update(SessionRow).values(**values).where(SessionRow.id == session_id)
-                    )
-                    await db_sess.execute(query)
-                all_terminated = session.status in (
-                    SessionStatus.TERMINATED,
-                    SessionStatus.CANCELLED,
-                )
-                return all_terminated, session_id
-
-        do_fire_event, session_id = await execute_with_retry(_check_and_mark)
-        if session_id is None:
-            return
+        new_session_status = await SessionRow.transit_session_status(
+            self.db, session_id, status_info=reason
+        )
+        do_fire_event = new_session_status in (
+            SessionStatus.TERMINATED,
+            SessionStatus.CANCELLED,
+        )
         if do_fire_event:
             await self.event_producer.produce_event(
                 SessionTerminatedEvent(session_id, reason),
             )
 
     async def mark_session_terminating(
         self,
@@ -2742,15 +2558,16 @@
         """
         Commit a main kernel's container of the given session.
         """
 
         kernel: KernelRow = session.main_kernel
         if kernel.status != KernelStatus.RUNNING:
             raise InvalidAPIParameters(
-                f"Unable to commit since kernel(id: {kernel.id}) of session(id: {session.id}) is currently not RUNNING."
+                f"Unable to commit since kernel(id: {kernel.id}) of session(id: {session.id}) is"
+                " currently not RUNNING."
             )
         email = await self._get_user_email(kernel)
         now = datetime.now(tzutc()).strftime("%Y-%m-%dT%HH%MM%SS")
         shortend_sname = session.name[:SESSION_NAME_LEN_LIMIT]
         registry, _, filtered = kernel.image.partition("/")
         img_path, _, image_name = filtered.partition("/")
         filename = f"{now}_{shortend_sname}_{image_name}.tar.gz"
@@ -2795,24 +2612,27 @@
 async def check_scaling_group(
     conn: SAConnection,
     scaling_group: str | None,
     session_type: SessionTypes,
     access_key: AccessKey,
     domain_name: str,
     group_id: Union[uuid.UUID, str],
+    public_sgroup_only: bool = False,
 ) -> str:
     # Check scaling group availability if scaling_group parameter is given.
     # If scaling_group is not provided, it will be selected as the first one among
     # the list of allowed scaling groups.
     candidates = await query_allowed_sgroups(
         conn,
         domain_name,
         group_id,
         access_key,
     )
+    if public_sgroup_only:
+        candidates = [sgroup for sgroup in candidates if sgroup["is_public"]]
     if not candidates:
         raise ScalingGroupNotFound("You have no scaling groups allowed to use.")
 
     stype = session_type.value.lower()
     if scaling_group is None:
         for sgroup in candidates:
             allowed_session_types = sgroup["scheduler_opts"].allowed_session_types
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/dispatcher.py` & `backend.ai-manager-23.3.1/ai/backend/manager/scheduler/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 from ai.backend.plugin.entrypoint import scan_entrypoints
 
 from ..api.exceptions import GenericBadRequest, InstanceNotAvailable
 from ..defs import LockID
 from ..exceptions import convert_to_status_data
 from ..models import (
     AgentStatus,
+    KernelRole,
     KernelRow,
     KernelStatus,
     ScalingGroupRow,
     SessionRow,
     SessionStatus,
-    kernels,
     list_schedulable_agents_by_sgroup,
     recalc_agent_resource_occupancy,
     recalc_concurrency_used,
 )
 from ..models.scaling_group import ScalingGroupOpts
 from ..models.utils import ExtendedAsyncSAEngine as SAEngine
 from ..models.utils import execute_with_retry, sql_json_increment, sql_json_merge
@@ -270,33 +270,50 @@
             scheduler = await self._load_scheduler(db_sess, sgroup_name)
             existing_sessions, pending_sessions, cancelled_sessions = await _list_managed_sessions(
                 db_sess, sgroup_name, scheduler.sgroup_opts.pending_timeout
             )
 
         if cancelled_sessions:
             now = datetime.now(tzutc())
+            session_ids = [item.id for item in cancelled_sessions]
 
             async def _apply_cancellation():
                 async with self.db.begin_session() as db_sess:
+                    kernel_query = (
+                        sa.update(KernelRow)
+                        .values(
+                            status=KernelStatus.CANCELLED,
+                            status_info="pending-timeout",
+                            terminated_at=now,
+                            status_history=sql_json_merge(
+                                KernelRow.status_history,
+                                (),
+                                {
+                                    KernelStatus.CANCELLED.name: now.isoformat(),
+                                },
+                            ),
+                        )
+                        .where(KernelRow.session_id.in_(session_ids))
+                    )
+                    await db_sess.execute(kernel_query)
                     query = (
                         sa.update(SessionRow)
                         .values(
                             status=SessionStatus.CANCELLED,
-                            status_changed=now,
                             status_info="pending-timeout",
                             terminated_at=now,
                             status_history=sql_json_merge(
-                                kernels.c.status_history,
+                                SessionRow.status_history,
                                 (),
                                 {
                                     SessionStatus.CANCELLED.name: now.isoformat(),
                                 },
                             ),
                         )
-                        .where(SessionRow.id.in_([item.id for item in cancelled_sessions]))
+                        .where(SessionRow.id.in_(session_ids))
                     )
                     await db_sess.execute(query)
 
             await execute_with_retry(_apply_cancellation)
             for item in cancelled_sessions:
                 await self.event_producer.produce_event(
                     SessionCancelledEvent(
@@ -347,34 +364,37 @@
             _log_fmt.set(log_fmt)
             _log_args.set(log_args)
             log.debug(log_fmt + "try-scheduling", *log_args)
 
             async def _check_predicates() -> List[Tuple[str, Union[Exception, PredicateResult]]]:
                 check_results: List[Tuple[str, Union[Exception, PredicateResult]]] = []
                 async with self.db.begin_session() as db_sess:
-                    predicates: Sequence[Tuple[str, Awaitable[PredicateResult]]] = [
+                    predicates: list[Tuple[str, Awaitable[PredicateResult]]] = [
                         (
                             "reserved_time",
                             check_reserved_batch_session(db_sess, sched_ctx, sess_ctx),
                         ),
-                        ("concurrency", check_concurrency(db_sess, sched_ctx, sess_ctx)),
                         ("dependencies", check_dependencies(db_sess, sched_ctx, sess_ctx)),
-                        (
-                            "keypair_resource_limit",
-                            check_keypair_resource_limit(db_sess, sched_ctx, sess_ctx),
-                        ),
-                        (
-                            "user_group_resource_limit",
-                            check_group_resource_limit(db_sess, sched_ctx, sess_ctx),
-                        ),
-                        (
-                            "domain_resource_limit",
-                            check_domain_resource_limit(db_sess, sched_ctx, sess_ctx),
-                        ),
                     ]
+                    if any([kernel.role != KernelRole.SYSTEM for kernel in sess_ctx.kernels]):
+                        predicates += [
+                            ("concurrency", check_concurrency(db_sess, sched_ctx, sess_ctx)),
+                            (
+                                "keypair_resource_limit",
+                                check_keypair_resource_limit(db_sess, sched_ctx, sess_ctx),
+                            ),
+                            (
+                                "user_group_resource_limit",
+                                check_group_resource_limit(db_sess, sched_ctx, sess_ctx),
+                            ),
+                            (
+                                "domain_resource_limit",
+                                check_domain_resource_limit(db_sess, sched_ctx, sess_ctx),
+                            ),
+                        ]
                     for predicate_name, check_coro in predicates:
                         try:
                             check_results.append((predicate_name, await check_coro))
                         except DBAPIError:
                             raise
                         except Exception as e:
                             log.exception(log_fmt + "predicate-error", *log_args)
@@ -526,26 +546,25 @@
         Finds and assigns an agent having resources enough to host the entire session.
         """
         log_fmt = _log_fmt.get("")
         log_args = _log_args.get(tuple())
         requested_architectures = set(k.architecture for k in sess_ctx.kernels)
         if len(requested_architectures) > 1:
             raise GenericBadRequest(
-                "Cannot assign multiple kernels with different architecture"
-                "on single node session",
+                "Cannot assign multiple kernels with different architectureon single node session",
             )
         requested_architecture = requested_architectures.pop()
         compatible_candidate_agents = [
             ag for ag in candidate_agents if ag.architecture == requested_architecture
         ]
         try:
             if not compatible_candidate_agents:
                 raise InstanceNotAvailable(
                     extra_msg=(
-                        f"No agents found to be compatible with the image acrhitecture "
+                        "No agents found to be compatible with the image acrhitecture "
                         f"(image[0]: {sess_ctx.main_kernel.image_ref}, "
                         f"arch: {requested_architecture})"
                     ),
                 )
 
             # If sess_ctx.agent_id is already set for manual assignment by superadmin,
             # skip assign_agent_for_session().
@@ -557,16 +576,16 @@
                 # Let the scheduler check the resource availability and decide the target agent
                 cand_agent = scheduler.assign_agent_for_session(
                     compatible_candidate_agents, sess_ctx
                 )
                 if cand_agent is None:
                     raise InstanceNotAvailable(
                         extra_msg=(
-                            f"Could not find a contiguous resource region in any agent "
-                            f"big enough to host the session "
+                            "Could not find a contiguous resource region in any agent "
+                            "big enough to host the session "
                             f"({sess_ctx.id})"
                         ),
                     )
                 assert cand_agent is not None
                 agent_id = cand_agent
             async with self.db.begin_session() as agent_db_sess:
                 query = sa.select(AgentRow.available_slots).where(AgentRow.id == agent_id)
@@ -623,15 +642,15 @@
             await execute_with_retry(partial(_update_sched_failure, sched_failure))
             raise
         except Exception as e:
             log.exception(
                 log_fmt + "unexpected-error, during agent allocation",
                 *log_args,
             )
-            exc_data = convert_to_status_data(e)
+            exc_data = convert_to_status_data(e, self.local_config["debug"]["enabled"])
 
             async def _update_generic_failure() -> None:
                 async with self.db.begin_session() as kernel_db_sess:
                     await _rollback_predicate_mutations(
                         kernel_db_sess,
                         sched_ctx,
                         sess_ctx,
@@ -747,28 +766,28 @@
                         # Each kernel may have different images and different architectures
                         compatible_candidate_agents = [
                             ag for ag in candidate_agents if ag.architecture == kernel.architecture
                         ]
                         if not compatible_candidate_agents:
                             raise InstanceNotAvailable(
                                 extra_msg=(
-                                    f"No agents found to be compatible with the image acrhitecture "
+                                    "No agents found to be compatible with the image acrhitecture "
                                     f"(image: {kernel.image_ref}, "
                                     f"arch: {kernel.architecture})"
                                 ),
                             )
                         # Let the scheduler check the resource availability and decide the target agent
                         agent = scheduler.assign_agent_for_kernel(
                             compatible_candidate_agents, kernel
                         )
                         if agent is None:
                             raise InstanceNotAvailable(
                                 extra_msg=(
-                                    f"Could not find a contiguous resource region in any agent "
-                                    f"big enough to host a kernel in the session "
+                                    "Could not find a contiguous resource region in any agent "
+                                    "big enough to host a kernel in the session "
                                     f"({sess_ctx.id})"
                                 ),
                             )
                     assert agent is not None
 
                     async def _reserve() -> None:
                         nonlocal agent_alloc_ctx, candidate_agents
@@ -818,15 +837,15 @@
                     await execute_with_retry(partial(_update_sched_failure, sched_failure))
                     raise
                 except Exception as e:
                     log.exception(
                         log_fmt + "unexpected-error, during agent allocation",
                         *log_args,
                     )
-                    exc_data = convert_to_status_data(e)
+                    exc_data = convert_to_status_data(e, self.local_config["debug"]["enabled"])
 
                     async def _update_generic_failure() -> None:
                         async with self.db.begin_session() as kernel_db_sess:
                             await _rollback_predicate_mutations(
                                 kernel_db_sess,
                                 sched_ctx,
                                 sess_ctx,
@@ -1021,15 +1040,15 @@
         log_args = (session,)
         log.debug(log_fmt + "try-starting", *log_args)
         try:
             assert len(session.kernels) > 0
             await self.registry.start_session(sched_ctx, session)
         except Exception as e:
             status_data = convert_to_status_data(e, self.local_config["debug"]["enabled"])
-            log.warning(log_fmt + "failed-starting: {1!r}", *log_args, status_data)
+            log.warning(log_fmt + "failed-starting", *log_args, exc_info=True)
             # TODO: instead of instantly cancelling upon exception, we could mark it as
             #       SCHEDULED and retry within some limit using status_data.
 
             async def _mark_session_cancelled() -> None:
                 async with self.db.begin() as db_conn:
                     affected_agents = set(k.agent for k in session.kernels)
                     await _rollback_predicate_mutations(db_conn, sched_ctx, session)
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/drf.py` & `backend.ai-manager-23.3.1/ai/backend/manager/scheduler/drf.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/fifo.py` & `backend.ai-manager-23.3.1/ai/backend/manager/scheduler/fifo.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/mof.py` & `backend.ai-manager-23.3.1/ai/backend/manager/scheduler/mof.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/predicates.py` & `backend.ai-manager-23.3.1/ai/backend/manager/scheduler/predicates.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         _check_keypair_concurrency_script,
         [f"keypair.concurrency_used.{sess_ctx.access_key}"],
         [max_concurrent_sessions],
     )
     if ok == 0:
         return PredicateResult(
             False,
-            "You cannot run more than " f"{max_concurrent_sessions} concurrent sessions",
+            f"You cannot run more than {max_concurrent_sessions} concurrent sessions",
         )
     log.debug(
         "number of concurrent sessions of ak:{0} = {1} / {2}",
         sess_ctx.access_key,
         concurrency_used,
         max_concurrent_sessions,
     )
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/scheduler/types.py` & `backend.ai-manager-23.3.1/ai/backend/manager/scheduler/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/server.py` & `backend.ai-manager-23.3.1/ai/backend/manager/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,14 +414,15 @@
         root_ctx.redis_stat,
         root_ctx.redis_live,
         root_ctx.redis_image,
         root_ctx.event_dispatcher,
         root_ctx.event_producer,
         root_ctx.storage_manager,
         root_ctx.hook_plugin_ctx,
+        debug=root_ctx.local_config["debug"]["enabled"],
     )
     await root_ctx.registry.init()
     yield
     await root_ctx.registry.shutdown()
 
 
 @actxmgr
```

### Comparing `backend.ai-manager-23.3.0a4/ai/backend/manager/types.py` & `backend.ai-manager-23.3.1/ai/backend/manager/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/PKG-INFO` & `backend.ai-manager-23.3.1/backend.ai_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 Backend.AI Manager with API Gateway
 ===================================
```

### Comparing `backend.ai-manager-23.3.0a4/backend.ai_manager.egg-info/SOURCES.txt` & `backend.ai-manager-23.3.1/backend.ai_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
 ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
 ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
 ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
 ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
 ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
 ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
 ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
+ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
 ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
 ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
 ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
 ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
 ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
 ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
 ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
@@ -192,14 +193,16 @@
 ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
 ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
 ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
 ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
 ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
 ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
 ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
+ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
+ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
 ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
 ai/backend/manager/models/minilang/__init__.py
 ai/backend/manager/models/minilang/ordering.py
 ai/backend/manager/models/minilang/queryfilter.py
 ai/backend/manager/plugin/__init__.py
 ai/backend/manager/plugin/error_monitor.py
 ai/backend/manager/plugin/monitor.py
```

### Comparing `backend.ai-manager-23.3.0a4/backend_shim.py` & `backend.ai-manager-23.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.0a4/setup.py` & `backend.ai-manager-23.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI Manager',
     'entry_points': {
         'backendai_cli_v10': [
             'mgr = ai.backend.manager.cli.__main__:main',
             'mgr.start-server = ai.backend.manager.server:main',
@@ -39,24 +39,24 @@
         'PyYAML~=6.0',
         'SQLAlchemy[postgresql_asyncpg]~=1.4.40',
         'aiodataloader-ng~=0.2.1',
         'aiodocker~=0.21.0',
         'aiohttp_cors~=0.7',
         'aiohttp_sse>=2.0',
         'aiohttp~=3.8.1',
-        'aiomonitor-ng~=0.7.0',
-        'aiotools~=1.5.9',
+        'aiomonitor-ng~=0.7.2',
+        'aiotools~=1.6.1',
         'alembic~=1.8.1',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==23.03.0a4
+        """backend.ai-cli==23.03.1
 """,
-        """backend.ai-common==23.03.0a4
+        """backend.ai-common==23.03.1
 """,
-        """backend.ai-plugin==23.03.0a4
+        """backend.ai-plugin==23.03.1
 """,
         'callosum~=0.9.10',
         'click>=7.1.2',
         'cryptography>=2.8',
         'graphene~=2.1.9',
         'lark-parser~=0.11.3',
         'more-itertools~=8.13.0',
@@ -368,11 +368,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.0a4
+    'version': """23.03.1
 """,
     'zip_safe': False,
 })
```

