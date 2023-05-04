# Comparing `tmp/stdocker-1.0.8.tar.gz` & `tmp/stdocker-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdocker-1.0.8.tar", last modified: Thu Sep  8 09:49:19 2022, max compression
+gzip compressed data, was "stdocker-1.0.9.tar", last modified: Fri Sep  9 10:43:07 2022, max compression
```

## Comparing `stdocker-1.0.8.tar` & `stdocker-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2022-09-08 09:49:19.357488 stdocker-1.0.8/
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    21002 2022-09-08 09:49:19.357488 stdocker-1.0.8/PKG-INFO
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    14873 2022-09-08 09:42:42.000000 stdocker-1.0.8/README.md
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       38 2022-09-08 09:49:19.357488 stdocker-1.0.8/setup.cfg
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1644 2022-08-23 10:32:44.000000 stdocker-1.0.8/setup.py
-drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2022-09-08 09:49:19.353488 stdocker-1.0.8/stdocker/
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        0 2022-08-22 10:00:30.000000 stdocker-1.0.8/stdocker/__init__.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    12090 2022-09-08 05:27:16.000000 stdocker-1.0.8/stdocker/cli.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      309 2022-09-06 09:15:16.000000 stdocker-1.0.8/stdocker/config.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     5457 2022-09-08 09:39:09.000000 stdocker-1.0.8/stdocker/env_handler.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1395 2022-09-01 02:43:21.000000 stdocker-1.0.8/stdocker/env_parser.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      532 2022-09-01 03:32:56.000000 stdocker-1.0.8/stdocker/utils.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       22 2022-09-08 09:42:35.000000 stdocker-1.0.8/stdocker/version.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      748 2022-09-01 02:19:41.000000 stdocker-1.0.8/stdocker/yaml_parser.py
-drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2022-09-08 09:49:19.357488 stdocker-1.0.8/stdocker.egg-info/
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    21002 2022-09-08 09:49:19.000000 stdocker-1.0.8/stdocker.egg-info/PKG-INFO
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      408 2022-09-08 09:49:19.000000 stdocker-1.0.8/stdocker.egg-info/SOURCES.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2022-09-08 09:49:19.000000 stdocker-1.0.8/stdocker.egg-info/dependency_links.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       48 2022-09-08 09:49:19.000000 stdocker-1.0.8/stdocker.egg-info/entry_points.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2022-08-23 10:13:35.000000 stdocker-1.0.8/stdocker.egg-info/not-zip-safe
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       98 2022-09-08 09:49:19.000000 stdocker-1.0.8/stdocker.egg-info/requires.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        9 2022-09-08 09:49:19.000000 stdocker-1.0.8/stdocker.egg-info/top_level.txt
+drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2022-09-09 10:43:07.153344 stdocker-1.0.9/
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    22680 2022-09-09 10:43:07.153344 stdocker-1.0.9/PKG-INFO
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    16068 2022-09-09 10:24:53.000000 stdocker-1.0.9/README.md
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       38 2022-09-09 10:43:07.153344 stdocker-1.0.9/setup.cfg
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1644 2022-08-23 10:32:44.000000 stdocker-1.0.9/setup.py
+drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2022-09-09 10:43:07.153344 stdocker-1.0.9/stdocker/
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        0 2022-08-22 10:00:30.000000 stdocker-1.0.9/stdocker/__init__.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    13631 2022-09-09 10:23:07.000000 stdocker-1.0.9/stdocker/cli.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      328 2022-09-09 06:53:04.000000 stdocker-1.0.9/stdocker/config.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     5457 2022-09-08 09:39:09.000000 stdocker-1.0.9/stdocker/env_handler.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1395 2022-09-01 02:43:21.000000 stdocker-1.0.9/stdocker/env_parser.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      532 2022-09-01 03:32:56.000000 stdocker-1.0.9/stdocker/utils.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       22 2022-09-09 10:26:06.000000 stdocker-1.0.9/stdocker/version.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      748 2022-09-01 02:19:41.000000 stdocker-1.0.9/stdocker/yaml_parser.py
+drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2022-09-09 10:43:07.153344 stdocker-1.0.9/stdocker.egg-info/
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    22680 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/PKG-INFO
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      408 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/SOURCES.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/dependency_links.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       48 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/entry_points.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2022-09-09 10:32:04.000000 stdocker-1.0.9/stdocker.egg-info/not-zip-safe
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       98 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/requires.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        9 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/top_level.txt
```

### Comparing `stdocker-1.0.8/PKG-INFO` & `stdocker-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdocker
-Version: 1.0.8
+Version: 1.0.9
 Summary: Shinetech Docker CLI.
 Home-page: https://github.com/winds1983/stdocker
 Author: Jason Sun
 Author-email: sunf@shinetechsoftware.com
 License: MIT
 Description: # Shinetech Docker CLI
         
@@ -19,34 +19,35 @@
           * [Run docker exec command](#run-docker-exec-command)
           * [Log in to the specified server using SSH](#log-in-to-the-specified-server-using-ssh)
           * [Launch docker services](#launch-docker-services)
           * [Stop docker services](#stop-docker-services)
           * [Restart specified docker service](#restart-specified-docker-service)
           * [Configure local environment](#configure-local-environment)
           * [Build local development environment with your configuration](#build-local-development-environment-with-your-configuration)
-          * [Export or import database](#export-or-import-database)
+          * [Export and import database](#export-and-import-database)
             * [Export database](#export-database)
             * [Import database](#import-database)
           * [Show the local environment and workspace information](#show-the-local-environment-and-workspace-information)
           * [List all environments](#list-all-environments)
           * [Initial workspace](#initial-workspace)
-          * [Create project](#create-project)
-            * [Create a project based on a base template or existing code](#create-a-project-based-on-a-base-template-or-existing-code)
-            * [Create a project based on the Magento source code](#create-a-project-based-on-the-magento-source-code)
+          * [Create and setup project](#create-and-setup-project)
+            * [Create a new project based on a base template or framework skeleton](#create-a-new-project-based-on-a-base-template-or-framework-skeleton)
+            * [Create a new Magento project based on the source code or composer](#create-a-new-Magento-project-based-on-the-source-code-or-composer)
+            * [Build an existing project based on existing code and database](#build-an-existing-project-based-on-existing-code-and-database)
           * [Upgrade Shinetech Docker](#upgrade-shinetech-docker)
         
         ## Getting Started
         
         ```shell
         pip3 install stdocker
         ```
         
         If you get error `ERROR: Could not find a version that satisfies the requirement`, please use the following command to install:
         ```shell
-        python3 -m pip install stdocker==1.0.8
+        python3 -m pip install stdocker==1.0.9
         ```
         
         It based on the internal docker project `Shinetech Docker`, please install it first. If you do not have permission to use Shinetech Docker, please ignore this package.
         
         After the installation is successful, you can run the `stdocker` command in any directory and perform the operations you need.
         
         ## Use Cases
@@ -68,31 +69,42 @@
         Options:
           -d, --working-dir PATH  Location of the installation directory, defaults to
                                   /opt/shinetech/stdocker.
           --version               Show the version and exit.
           --help                  Show this message and exit.
         
         Commands:
-          about         Show the local environment and workspace information
-          bash          Bash session for running container
-          build         Build local development environment with your configuration
-          compose       Execute sudo docker-compose * command
-          configure     Configure local environment, will guide you through...
-          database      Export or import database
-          envs          List all environments
-          exec          Execute sudo docker exec * command
-          init-magento  Create a project based on the Magento source code
-          init-project  Create a project based on a base template or existing code
-          restart       Restart specified docker service
-          run           Execute sudo docker * command
-          start         Launch docker services
-          status        List all running containers
-          stop          Stop docker services
-          upgrade       Upgrade Shinetech Docker
-          workspace     Initial workspace
+          about                   Show the local environment and workspace...
+          bash                    Bash session for running container
+          build                   Build local development environment with your...
+          compose                 Execute sudo docker-compose * command
+          configure               Configure local environment, will guide you...
+          create-magento-project  Create a new Magento project based on the...
+          create-project          Create a new project based on a base template...
+          database                Export or import database
+          envs                    List all environments
+          exec                    Execute sudo docker exec * command
+          restart                 Restart specified docker service
+          run                     Execute sudo docker * command
+          setup-project           Build a existing project based on existing code...
+          start                   Launch docker services
+          status                  List all running containers
+          stop                    Stop docker services
+          upgrade                 Upgrade Shinetech Docker
+          workspace               Initial workspace
+        ```
+        
+        For the detailed usage of each command, you can use the following command to view:
+        
+        ```shell
+        stdocker [COMMAND] --help
+        ```
+        e.g:
+        ```shell
+        stdocker create-project --help
         ```
         
         ### Run docker command
         
         If you want to run `sudo docker *` command, you can use our command like this:
         ```shell
         stdocker run <DOCKER_COMMAND>
@@ -159,21 +171,21 @@
         ```shell
         sudo docker exec -it stdev_phpfpm_1 /bin/bash
         ```
         
         ### Log in to the specified server using SSH
         
         ```shell
-        stdocker ssh <SERVICE>
+        stdocker bash <SERVICE>
         ```
         
         e.g:
         ```shell
-        stdocker ssh phpfpm
-        stdocker ssh mysql
+        stdocker bash phpfpm
+        stdocker bash mysql
         ```
         This command is equivalent to:
         ```shell
         sudo docker exec -it stdev_phpfpm_1 /bin/bash
         sudo docker exec -it stdev_mysql_1 /bin/bash
         ```
         
@@ -223,15 +235,15 @@
         If `ENV` is empty, it will guide you to create your customized configuration, otherwise will base on your specified env to build services.
         
         ```shell
         stdocker build
         stdocker build --env=magento_244
         ```
         
-        ### Export or import database
+        ### Export and import database
         
         ```shell
         stdocker database <ACTION{import|export}>
         ```
         
         #### Export database:
         ```shell
@@ -248,24 +260,25 @@
         
         ```shell
         stdocker about
         ```
         You can see the following information:
         ```
         Current environment:
-         - magento_244
+         - lamp
         Your workspace information:
          - Workspace: /home/sunfeng/stdocker
          - Project Directory: /home/sunfeng/stdocker/www
          - Nginx VHosts: /home/sunfeng/stdocker/config/services/nginx/sites-enabled
          - Nginx Log: /home/sunfeng/stdocker/var/logs/nginx
          - Apache VHosts: /home/sunfeng/stdocker/config/services/apache/sites-enabled
          - Apache Log: /home/sunfeng/stdocker/var/logs/apache2
          - SSL CA: /home/sunfeng/stdocker/config/services/ca
          - php.ini: /home/sunfeng/stdocker/config/services/php/php.ini
+         - Composer auth.json: /home/sunfeng/stdocker/config/services/composer/auth.json
          - MySQL Log: /home/sunfeng/stdocker/var/logs/mysql
         ```
         
         ### List all environments
         
         ```shell
         stdocker envs
@@ -299,50 +312,65 @@
         
         It will initial your workspace to your home or specified directory, and update env config.
         
         ```shell
         stdocker workspace
         ```
         
-        ### Create project
+        ### Create and setup project
         
-        #### Create a project based on a base template or existing code
+        #### Create a new project based on a base template or framework skeleton
         
         ```shell
-        stdocker init-project [OPTIONS]
+        stdocker create-project [OPTIONS]
         ```
         
         Initial a Magento 2 project:
         ```shell
-        stdocker init-project --platform=magento --name=m2project
+        stdocker create-project --platform=magento --project-name=m2project --target-version=2.4.5
         ```
         
         Initial a Symfony project:
         ```shell
-        stdocker init-project --platform=symfony --name=sfproject
+        stdocker init-project --platform=symfony --project-name=sfproject
         ```
         
-        #### Create a project based on the Magento source code
+        #### Create a new Magento project based on the source code or composer
         
-        Please download the Magento source code from the official website first.
+        Please download the Magento source code from the official website first if use source code to create project.
         
         ```shell
-        stdocker init-magento [OPTIONS]
+        stdocker create-magento-project [OPTIONS]
         ```
         
-        Create a Magento 2.4.5 project:
+        Create a Magento 2.4.5 project with source code:
         ```shell
-        stdocker init-magento --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip
+        stdocker create-magento-project --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip
         ```
         
         Create a Magento 2.4.5 project with custom project name:
         ```shell
-        stdocker init-magento --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip --project-name=testproject
+        stdocker create-magento-project --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip --project-name=testproject
         ```
         
+        Create a Magento 2.4.5 project with composer:
+        ```shell
+        stdocker create-magento-project --target-version=2.4.5
+        ```
+        
+        #### Build an existing project based on existing code and database
+        
+        ```shell
+        stdocker setup-project [OPTIONS]
+        ```
+        
+        Setup HP project:
+        ```shell
+        stdocker setup-project --project-name=hp --db-sql-file=/home/sunfeng/Downloads/20220824201501.sql --country=id
+        ```
         
         ### Upgrade Shinetech Docker
         
         ```shell
         stdocker upgrade
         ```
         
@@ -364,14 +392,24 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
         project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
         
+        ## [1.0.9] - 2022-09-09
+        
+        ### Added
+        
+        - Rebuild create and setup project command
+        - Update project creation parameters
+        - Add composer auth.json in about command
+        - Update use cases
+        
+        
         ## [1.0.8] - 2022-09-08
         
         ### Added
         
         - Adjust platforms for init project command
         - Add MariaDB to env table
         - Add sort for env table
```

### Comparing `stdocker-1.0.8/README.md` & `stdocker-1.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,34 +11,35 @@
   * [Run docker exec command](#run-docker-exec-command)
   * [Log in to the specified server using SSH](#log-in-to-the-specified-server-using-ssh)
   * [Launch docker services](#launch-docker-services)
   * [Stop docker services](#stop-docker-services)
   * [Restart specified docker service](#restart-specified-docker-service)
   * [Configure local environment](#configure-local-environment)
   * [Build local development environment with your configuration](#build-local-development-environment-with-your-configuration)
-  * [Export or import database](#export-or-import-database)
+  * [Export and import database](#export-and-import-database)
     * [Export database](#export-database)
     * [Import database](#import-database)
   * [Show the local environment and workspace information](#show-the-local-environment-and-workspace-information)
   * [List all environments](#list-all-environments)
   * [Initial workspace](#initial-workspace)
-  * [Create project](#create-project)
-    * [Create a project based on a base template or existing code](#create-a-project-based-on-a-base-template-or-existing-code)
-    * [Create a project based on the Magento source code](#create-a-project-based-on-the-magento-source-code)
+  * [Create and setup project](#create-and-setup-project)
+    * [Create a new project based on a base template or framework skeleton](#create-a-new-project-based-on-a-base-template-or-framework-skeleton)
+    * [Create a new Magento project based on the source code or composer](#create-a-new-Magento-project-based-on-the-source-code-or-composer)
+    * [Build an existing project based on existing code and database](#build-an-existing-project-based-on-existing-code-and-database)
   * [Upgrade Shinetech Docker](#upgrade-shinetech-docker)
 
 ## Getting Started
 
 ```shell
 pip3 install stdocker
 ```
 
 If you get error `ERROR: Could not find a version that satisfies the requirement`, please use the following command to install:
 ```shell
-python3 -m pip install stdocker==1.0.8
+python3 -m pip install stdocker==1.0.9
 ```
 
 It based on the internal docker project `Shinetech Docker`, please install it first. If you do not have permission to use Shinetech Docker, please ignore this package.
 
 After the installation is successful, you can run the `stdocker` command in any directory and perform the operations you need.
 
 ## Use Cases
@@ -60,31 +61,42 @@
 Options:
   -d, --working-dir PATH  Location of the installation directory, defaults to
                           /opt/shinetech/stdocker.
   --version               Show the version and exit.
   --help                  Show this message and exit.
 
 Commands:
-  about         Show the local environment and workspace information
-  bash          Bash session for running container
-  build         Build local development environment with your configuration
-  compose       Execute sudo docker-compose * command
-  configure     Configure local environment, will guide you through...
-  database      Export or import database
-  envs          List all environments
-  exec          Execute sudo docker exec * command
-  init-magento  Create a project based on the Magento source code
-  init-project  Create a project based on a base template or existing code
-  restart       Restart specified docker service
-  run           Execute sudo docker * command
-  start         Launch docker services
-  status        List all running containers
-  stop          Stop docker services
-  upgrade       Upgrade Shinetech Docker
-  workspace     Initial workspace
+  about                   Show the local environment and workspace...
+  bash                    Bash session for running container
+  build                   Build local development environment with your...
+  compose                 Execute sudo docker-compose * command
+  configure               Configure local environment, will guide you...
+  create-magento-project  Create a new Magento project based on the...
+  create-project          Create a new project based on a base template...
+  database                Export or import database
+  envs                    List all environments
+  exec                    Execute sudo docker exec * command
+  restart                 Restart specified docker service
+  run                     Execute sudo docker * command
+  setup-project           Build a existing project based on existing code...
+  start                   Launch docker services
+  status                  List all running containers
+  stop                    Stop docker services
+  upgrade                 Upgrade Shinetech Docker
+  workspace               Initial workspace
+```
+
+For the detailed usage of each command, you can use the following command to view:
+
+```shell
+stdocker [COMMAND] --help
+```
+e.g:
+```shell
+stdocker create-project --help
 ```
 
 ### Run docker command
 
 If you want to run `sudo docker *` command, you can use our command like this:
 ```shell
 stdocker run <DOCKER_COMMAND>
@@ -151,21 +163,21 @@
 ```shell
 sudo docker exec -it stdev_phpfpm_1 /bin/bash
 ```
 
 ### Log in to the specified server using SSH
 
 ```shell
-stdocker ssh <SERVICE>
+stdocker bash <SERVICE>
 ```
 
 e.g:
 ```shell
-stdocker ssh phpfpm
-stdocker ssh mysql
+stdocker bash phpfpm
+stdocker bash mysql
 ```
 This command is equivalent to:
 ```shell
 sudo docker exec -it stdev_phpfpm_1 /bin/bash
 sudo docker exec -it stdev_mysql_1 /bin/bash
 ```
 
@@ -215,15 +227,15 @@
 If `ENV` is empty, it will guide you to create your customized configuration, otherwise will base on your specified env to build services.
 
 ```shell
 stdocker build
 stdocker build --env=magento_244
 ```
 
-### Export or import database
+### Export and import database
 
 ```shell
 stdocker database <ACTION{import|export}>
 ```
 
 #### Export database:
 ```shell
@@ -240,24 +252,25 @@
 
 ```shell
 stdocker about
 ```
 You can see the following information:
 ```
 Current environment:
- - magento_244
+ - lamp
 Your workspace information:
  - Workspace: /home/sunfeng/stdocker
  - Project Directory: /home/sunfeng/stdocker/www
  - Nginx VHosts: /home/sunfeng/stdocker/config/services/nginx/sites-enabled
  - Nginx Log: /home/sunfeng/stdocker/var/logs/nginx
  - Apache VHosts: /home/sunfeng/stdocker/config/services/apache/sites-enabled
  - Apache Log: /home/sunfeng/stdocker/var/logs/apache2
  - SSL CA: /home/sunfeng/stdocker/config/services/ca
  - php.ini: /home/sunfeng/stdocker/config/services/php/php.ini
+ - Composer auth.json: /home/sunfeng/stdocker/config/services/composer/auth.json
  - MySQL Log: /home/sunfeng/stdocker/var/logs/mysql
 ```
 
 ### List all environments
 
 ```shell
 stdocker envs
@@ -291,50 +304,65 @@
 
 It will initial your workspace to your home or specified directory, and update env config.
 
 ```shell
 stdocker workspace
 ```
 
-### Create project
+### Create and setup project
 
-#### Create a project based on a base template or existing code
+#### Create a new project based on a base template or framework skeleton
 
 ```shell
-stdocker init-project [OPTIONS]
+stdocker create-project [OPTIONS]
 ```
 
 Initial a Magento 2 project:
 ```shell
-stdocker init-project --platform=magento --name=m2project
+stdocker create-project --platform=magento --project-name=m2project --target-version=2.4.5
 ```
 
 Initial a Symfony project:
 ```shell
-stdocker init-project --platform=symfony --name=sfproject
+stdocker init-project --platform=symfony --project-name=sfproject
 ```
 
-#### Create a project based on the Magento source code
+#### Create a new Magento project based on the source code or composer
 
-Please download the Magento source code from the official website first.
+Please download the Magento source code from the official website first if use source code to create project.
 
 ```shell
-stdocker init-magento [OPTIONS]
+stdocker create-magento-project [OPTIONS]
 ```
 
-Create a Magento 2.4.5 project:
+Create a Magento 2.4.5 project with source code:
 ```shell
-stdocker init-magento --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip
+stdocker create-magento-project --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip
 ```
 
 Create a Magento 2.4.5 project with custom project name:
 ```shell
-stdocker init-magento --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip --project-name=testproject
+stdocker create-magento-project --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip --project-name=testproject
+```
+
+Create a Magento 2.4.5 project with composer:
+```shell
+stdocker create-magento-project --target-version=2.4.5
+```
+
+#### Build an existing project based on existing code and database
+
+```shell
+stdocker setup-project [OPTIONS]
 ```
 
+Setup HP project:
+```shell
+stdocker setup-project --project-name=hp --db-sql-file=/home/sunfeng/Downloads/20220824201501.sql --country=id
+```
 
 ### Upgrade Shinetech Docker
 
 ```shell
 stdocker upgrade
 ```
```

### Comparing `stdocker-1.0.8/setup.py` & `stdocker-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.0.8/stdocker/cli.py` & `stdocker-1.0.9/stdocker/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     sys.exit(1)
 
 from .version import __version__
 from .config import install_dir
 from .config import current_dir
 from .config import base_domain
 from .config import platforms
+from .config import projects
 
 
 """
 Check if project name is valid
 """
 def check_project_name(ctx, param, value):
     if not param.required and value is None:
@@ -202,14 +203,15 @@
     click.echo(click.style(f" - Nginx VHosts: {env_values['NGINX_VHOSTS_DIR']}", fg='cyan'))
     click.echo(click.style(f" - Nginx Log: {env_values['NGINX_LOG_DIR']}", fg='cyan'))
     click.echo(
         click.style(f" - Apache VHosts: {env_values['APACHE_VHOSTS_DIR']}", fg='cyan'))
     click.echo(click.style(f" - Apache Log: {env_values['APACHE_LOG_DIR']}", fg='cyan'))
     click.echo(click.style(f" - SSL CA: {env_values['SSL_CA_DIR']}", fg='cyan'))
     click.echo(click.style(f" - php.ini: {env_values['PHP_INI']}", fg='cyan'))
+    click.echo(click.style(f" - Composer auth.json: {env_values['COMPOSER_AUTH_FILE']}", fg='cyan'))
     click.echo(click.style(f" - MySQL Log: {env_values['MYSQL_LOG_DIR']}", fg='cyan'))
 
 
 @cli.command()
 @click.pass_context
 def envs(ctx: click.Context) -> None:
     """List all environments"""
@@ -217,49 +219,46 @@
     env_handler = EnvHandler(working_dir=working_dir)
     env_table = env_handler.list_env_table()
     print(env_table)
 
 
 @cli.command()
 @click.pass_context
-@click.option('--platform', required=True, default='generic',
-              type=click.Choice(platforms),
-              help="Specifies the framework used by the project.")
-@click.option('--name', required=True,
-              callback=check_project_name,
+@click.option('--project-name', required=True,
+              type=click.Choice(projects),
               help="Specify project name.")
-@click.option('--db-sql-file', required=False,
+@click.option('--db-sql-file', required=True,
               help="SQL backup file for initializing the database.")
 @click.option('--country', required=False,
               help="Build project by country, such as HP project have multiple independent countries and regions.")
 @click.option('--multiple-domain/--no-multiple-domain', default=False,
               help="Use multiple domains for multiple sites, single domain is used by default. "
                    "This option takes effect if --country is not empty. "
                    "e.g: For HP project, If No will use hp.dev.php9.cc for all country sites, "
                    "if Yes will use <country>.hp.dev.php9.cc for different sites.")
-def init_project(ctx: click.Context, platform: Any, name: Any, db_sql_file: Any, country: Any, multiple_domain: Any) -> None:
-    """Create a project based on a base template or existing code"""
+def setup_project(ctx: click.Context, project_name: Any, db_sql_file: Any, country: Any, multiple_domain: Any) -> None:
+    """Build a existing project based on existing code and database"""
     working_dir = ctx.obj['WORKING_DIR']
     env_handler = EnvHandler(working_dir=working_dir)
     env_values = env_handler.get_env_values()
     workspace_dir = env_values['WORKSPACE']
     current_env_configs = env_handler.get_current_env_configs()
     webserver = current_env_configs['services']['webserver']
 
-    domain = name + base_domain
+    domain = project_name + base_domain
     if multiple_domain and country is not None:
-        domain = name + '-' + country + base_domain
+        domain = project_name + '-' + country + base_domain
 
     project_dir = workspace_dir + '/www/' + domain
     if os.path.exists(project_dir):
         click.echo(click.style(f"NOTE: The project directory {project_dir} already exists.", fg='cyan'))
         click.confirm('Do you confirm to override and create project?', abort=True)
 
-    command = 'bash bin/init_project.sh ' \
-              + current_dir + ' ' + workspace_dir + ' ' + webserver + ' ' + platform + ' ' + name
+    command = 'bash bin/setup_project.sh ' \
+              + current_dir + ' ' + workspace_dir + ' ' + webserver + ' ' + project_name
 
     if db_sql_file is not None:
         command += ' ' + db_sql_file
     else:
         command += ' ""'
 
     if country is not None:
@@ -270,25 +269,59 @@
             command += ' n'
 
     os.system(command)
 
 
 @cli.command()
 @click.pass_context
+@click.option('--platform', required=True, default='generic',
+              type=click.Choice(platforms),
+              help="Specifies the framework used by the project.")
+@click.option('--project-name', required=True,
+              callback=check_project_name,
+              help="Specify project name.")
+@click.option('--target-version', required=False,
+              help="Specify framework version. e.g: 2.4.5, 2.4.4-p1 for Magento")
+def create_project(ctx: click.Context, platform: Any, project_name: Any, target_version: Any) -> None:
+    """Create a new project based on a base template or framework skeleton"""
+    working_dir = ctx.obj['WORKING_DIR']
+    env_handler = EnvHandler(working_dir=working_dir)
+    env_values = env_handler.get_env_values()
+    workspace_dir = env_values['WORKSPACE']
+    current_env_configs = env_handler.get_current_env_configs()
+    webserver = current_env_configs['services']['webserver']
+
+    domain = project_name + base_domain
+
+    project_dir = workspace_dir + '/www/' + domain
+    if os.path.exists(project_dir):
+        click.echo(click.style(f"NOTE: The project directory {project_dir} already exists.", fg='cyan'))
+        click.confirm('Do you confirm to override and create project?', abort=True)
+
+    command = 'bash bin/create_project.sh ' \
+              + current_dir + ' ' + workspace_dir + ' ' + webserver + ' ' + platform + ' ' + project_name
+    if target_version is not None:
+        command += ' ' + target_version
+
+    os.system(command)
+
+
+@cli.command()
+@click.pass_context
 @click.option('--target-version', required=True,
               help="Specify Magento version. e.g: 2.4.5, 2.4.4-p1")
 @click.option('--source-code-file', required=False,
               help="Specify Magento original source code file. "
                    "If not specified, composer will be used for installation, "
                    "otherwise the specified source code package will be used.")
 @click.option('--project-name', required=False,
               callback=check_project_name,
               help="Specify project name.")
-def init_magento(ctx: click.Context, target_version: Any, source_code_file: Any, project_name: Any) -> None:
-    """Create a project based on the Magento source code"""
+def create_magento_project(ctx: click.Context, target_version: Any, source_code_file: Any, project_name: Any) -> None:
+    """Create a new Magento project based on the source code or composer"""
     working_dir = ctx.obj['WORKING_DIR']
     env_handler = EnvHandler(working_dir=working_dir)
     env_values = env_handler.get_env_values()
     workspace_dir = env_values['WORKSPACE']
     current_env_configs = env_handler.get_current_env_configs()
     webserver = current_env_configs['services']['webserver']
 
@@ -300,15 +333,15 @@
     project_domain = project_name + base_domain
 
     project_dir = workspace_dir + '/www/' + project_domain
     if os.path.exists(project_dir):
         click.echo(click.style(f"NOTE: The Magento project {project_dir} already exists.", fg='cyan'))
         click.confirm('Do you confirm to override and create project?', abort=True)
 
-    command = 'bash bin/init_magento.sh ' \
+    command = 'bash bin/create_magento_project.sh ' \
               + current_dir + ' ' + workspace_dir + ' ' + webserver + ' ' + project_name + ' ' + target_version
     if source_code_file is not None:
         command += ' ' + source_code_file
 
     os.system(command)
```

### Comparing `stdocker-1.0.8/stdocker/env_handler.py` & `stdocker-1.0.9/stdocker/env_handler.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.0.8/stdocker/env_parser.py` & `stdocker-1.0.9/stdocker/env_parser.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.0.8/stdocker/utils.py` & `stdocker-1.0.9/stdocker/utils.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.0.8/stdocker/yaml_parser.py` & `stdocker-1.0.9/stdocker/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.0.8/stdocker.egg-info/PKG-INFO` & `stdocker-1.0.9/stdocker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdocker
-Version: 1.0.8
+Version: 1.0.9
 Summary: Shinetech Docker CLI.
 Home-page: https://github.com/winds1983/stdocker
 Author: Jason Sun
 Author-email: sunf@shinetechsoftware.com
 License: MIT
 Description: # Shinetech Docker CLI
         
@@ -19,34 +19,35 @@
           * [Run docker exec command](#run-docker-exec-command)
           * [Log in to the specified server using SSH](#log-in-to-the-specified-server-using-ssh)
           * [Launch docker services](#launch-docker-services)
           * [Stop docker services](#stop-docker-services)
           * [Restart specified docker service](#restart-specified-docker-service)
           * [Configure local environment](#configure-local-environment)
           * [Build local development environment with your configuration](#build-local-development-environment-with-your-configuration)
-          * [Export or import database](#export-or-import-database)
+          * [Export and import database](#export-and-import-database)
             * [Export database](#export-database)
             * [Import database](#import-database)
           * [Show the local environment and workspace information](#show-the-local-environment-and-workspace-information)
           * [List all environments](#list-all-environments)
           * [Initial workspace](#initial-workspace)
-          * [Create project](#create-project)
-            * [Create a project based on a base template or existing code](#create-a-project-based-on-a-base-template-or-existing-code)
-            * [Create a project based on the Magento source code](#create-a-project-based-on-the-magento-source-code)
+          * [Create and setup project](#create-and-setup-project)
+            * [Create a new project based on a base template or framework skeleton](#create-a-new-project-based-on-a-base-template-or-framework-skeleton)
+            * [Create a new Magento project based on the source code or composer](#create-a-new-Magento-project-based-on-the-source-code-or-composer)
+            * [Build an existing project based on existing code and database](#build-an-existing-project-based-on-existing-code-and-database)
           * [Upgrade Shinetech Docker](#upgrade-shinetech-docker)
         
         ## Getting Started
         
         ```shell
         pip3 install stdocker
         ```
         
         If you get error `ERROR: Could not find a version that satisfies the requirement`, please use the following command to install:
         ```shell
-        python3 -m pip install stdocker==1.0.8
+        python3 -m pip install stdocker==1.0.9
         ```
         
         It based on the internal docker project `Shinetech Docker`, please install it first. If you do not have permission to use Shinetech Docker, please ignore this package.
         
         After the installation is successful, you can run the `stdocker` command in any directory and perform the operations you need.
         
         ## Use Cases
@@ -68,31 +69,42 @@
         Options:
           -d, --working-dir PATH  Location of the installation directory, defaults to
                                   /opt/shinetech/stdocker.
           --version               Show the version and exit.
           --help                  Show this message and exit.
         
         Commands:
-          about         Show the local environment and workspace information
-          bash          Bash session for running container
-          build         Build local development environment with your configuration
-          compose       Execute sudo docker-compose * command
-          configure     Configure local environment, will guide you through...
-          database      Export or import database
-          envs          List all environments
-          exec          Execute sudo docker exec * command
-          init-magento  Create a project based on the Magento source code
-          init-project  Create a project based on a base template or existing code
-          restart       Restart specified docker service
-          run           Execute sudo docker * command
-          start         Launch docker services
-          status        List all running containers
-          stop          Stop docker services
-          upgrade       Upgrade Shinetech Docker
-          workspace     Initial workspace
+          about                   Show the local environment and workspace...
+          bash                    Bash session for running container
+          build                   Build local development environment with your...
+          compose                 Execute sudo docker-compose * command
+          configure               Configure local environment, will guide you...
+          create-magento-project  Create a new Magento project based on the...
+          create-project          Create a new project based on a base template...
+          database                Export or import database
+          envs                    List all environments
+          exec                    Execute sudo docker exec * command
+          restart                 Restart specified docker service
+          run                     Execute sudo docker * command
+          setup-project           Build a existing project based on existing code...
+          start                   Launch docker services
+          status                  List all running containers
+          stop                    Stop docker services
+          upgrade                 Upgrade Shinetech Docker
+          workspace               Initial workspace
+        ```
+        
+        For the detailed usage of each command, you can use the following command to view:
+        
+        ```shell
+        stdocker [COMMAND] --help
+        ```
+        e.g:
+        ```shell
+        stdocker create-project --help
         ```
         
         ### Run docker command
         
         If you want to run `sudo docker *` command, you can use our command like this:
         ```shell
         stdocker run <DOCKER_COMMAND>
@@ -159,21 +171,21 @@
         ```shell
         sudo docker exec -it stdev_phpfpm_1 /bin/bash
         ```
         
         ### Log in to the specified server using SSH
         
         ```shell
-        stdocker ssh <SERVICE>
+        stdocker bash <SERVICE>
         ```
         
         e.g:
         ```shell
-        stdocker ssh phpfpm
-        stdocker ssh mysql
+        stdocker bash phpfpm
+        stdocker bash mysql
         ```
         This command is equivalent to:
         ```shell
         sudo docker exec -it stdev_phpfpm_1 /bin/bash
         sudo docker exec -it stdev_mysql_1 /bin/bash
         ```
         
@@ -223,15 +235,15 @@
         If `ENV` is empty, it will guide you to create your customized configuration, otherwise will base on your specified env to build services.
         
         ```shell
         stdocker build
         stdocker build --env=magento_244
         ```
         
-        ### Export or import database
+        ### Export and import database
         
         ```shell
         stdocker database <ACTION{import|export}>
         ```
         
         #### Export database:
         ```shell
@@ -248,24 +260,25 @@
         
         ```shell
         stdocker about
         ```
         You can see the following information:
         ```
         Current environment:
-         - magento_244
+         - lamp
         Your workspace information:
          - Workspace: /home/sunfeng/stdocker
          - Project Directory: /home/sunfeng/stdocker/www
          - Nginx VHosts: /home/sunfeng/stdocker/config/services/nginx/sites-enabled
          - Nginx Log: /home/sunfeng/stdocker/var/logs/nginx
          - Apache VHosts: /home/sunfeng/stdocker/config/services/apache/sites-enabled
          - Apache Log: /home/sunfeng/stdocker/var/logs/apache2
          - SSL CA: /home/sunfeng/stdocker/config/services/ca
          - php.ini: /home/sunfeng/stdocker/config/services/php/php.ini
+         - Composer auth.json: /home/sunfeng/stdocker/config/services/composer/auth.json
          - MySQL Log: /home/sunfeng/stdocker/var/logs/mysql
         ```
         
         ### List all environments
         
         ```shell
         stdocker envs
@@ -299,50 +312,65 @@
         
         It will initial your workspace to your home or specified directory, and update env config.
         
         ```shell
         stdocker workspace
         ```
         
-        ### Create project
+        ### Create and setup project
         
-        #### Create a project based on a base template or existing code
+        #### Create a new project based on a base template or framework skeleton
         
         ```shell
-        stdocker init-project [OPTIONS]
+        stdocker create-project [OPTIONS]
         ```
         
         Initial a Magento 2 project:
         ```shell
-        stdocker init-project --platform=magento --name=m2project
+        stdocker create-project --platform=magento --project-name=m2project --target-version=2.4.5
         ```
         
         Initial a Symfony project:
         ```shell
-        stdocker init-project --platform=symfony --name=sfproject
+        stdocker init-project --platform=symfony --project-name=sfproject
         ```
         
-        #### Create a project based on the Magento source code
+        #### Create a new Magento project based on the source code or composer
         
-        Please download the Magento source code from the official website first.
+        Please download the Magento source code from the official website first if use source code to create project.
         
         ```shell
-        stdocker init-magento [OPTIONS]
+        stdocker create-magento-project [OPTIONS]
         ```
         
-        Create a Magento 2.4.5 project:
+        Create a Magento 2.4.5 project with source code:
         ```shell
-        stdocker init-magento --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip
+        stdocker create-magento-project --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip
         ```
         
         Create a Magento 2.4.5 project with custom project name:
         ```shell
-        stdocker init-magento --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip --project-name=testproject
+        stdocker create-magento-project --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip --project-name=testproject
         ```
         
+        Create a Magento 2.4.5 project with composer:
+        ```shell
+        stdocker create-magento-project --target-version=2.4.5
+        ```
+        
+        #### Build an existing project based on existing code and database
+        
+        ```shell
+        stdocker setup-project [OPTIONS]
+        ```
+        
+        Setup HP project:
+        ```shell
+        stdocker setup-project --project-name=hp --db-sql-file=/home/sunfeng/Downloads/20220824201501.sql --country=id
+        ```
         
         ### Upgrade Shinetech Docker
         
         ```shell
         stdocker upgrade
         ```
         
@@ -364,14 +392,24 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
         project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
         
+        ## [1.0.9] - 2022-09-09
+        
+        ### Added
+        
+        - Rebuild create and setup project command
+        - Update project creation parameters
+        - Add composer auth.json in about command
+        - Update use cases
+        
+        
         ## [1.0.8] - 2022-09-08
         
         ### Added
         
         - Adjust platforms for init project command
         - Add MariaDB to env table
         - Add sort for env table
```

