# Comparing `tmp/botocore-a-la-carte-ecs-1.34.80.tar.gz` & `tmp/botocore-a-la-carte-ecs-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ecs-1.34.80.tar", last modified: Tue Apr  9 01:00:38 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-ecs-1.34.9.tar", last modified: Thu Dec 28 01:06:49 2023, max compression
```

## Comparing `botocore-a-la-carte-ecs-1.34.80.tar` & `botocore-a-la-carte-ecs-1.34.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:38.352079 botocore-a-la-carte-ecs-1.34.80/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 01:00:38.000000 botocore-a-la-carte-ecs-1.34.80/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 01:00:38.352079 botocore-a-la-carte-ecs-1.34.80/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:38.348078 botocore-a-la-carte-ecs-1.34.80/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:38.348078 botocore-a-la-carte-ecs-1.34.80/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:38.348078 botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:38.352079 botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-09 01:00:23.000000 botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    36519 2024-04-09 01:00:23.000000 botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-09 01:00:23.000000 botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   580448 2024-04-09 01:00:23.000000 botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-09 01:00:23.000000 botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:38.352079 botocore-a-la-carte-ecs-1.34.80/botocore_a_la_carte_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 01:00:38.000000 botocore-a-la-carte-ecs-1.34.80/botocore_a_la_carte_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-09 01:00:38.000000 botocore-a-la-carte-ecs-1.34.80/botocore_a_la_carte_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:00:38.000000 botocore-a-la-carte-ecs-1.34.80/botocore_a_la_carte_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 01:00:38.000000 botocore-a-la-carte-ecs-1.34.80/botocore_a_la_carte_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:00:38.352079 botocore-a-la-carte-ecs-1.34.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 01:00:38.000000 botocore-a-la-carte-ecs-1.34.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:49.258337 botocore-a-la-carte-ecs-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:49.000000 botocore-a-la-carte-ecs-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:49.258337 botocore-a-la-carte-ecs-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:49.254337 botocore-a-la-carte-ecs-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:49.254337 botocore-a-la-carte-ecs-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:49.254337 botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:49.254337 botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2023-12-28 01:06:26.000000 botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36519 2023-12-28 01:06:26.000000 botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-28 01:06:26.000000 botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   544191 2023-12-28 01:06:26.000000 botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-12-28 01:06:26.000000 botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:49.258337 botocore-a-la-carte-ecs-1.34.9/botocore_a_la_carte_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:49.000000 botocore-a-la-carte-ecs-1.34.9/botocore_a_la_carte_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-28 01:06:49.000000 botocore-a-la-carte-ecs-1.34.9/botocore_a_la_carte_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:49.000000 botocore-a-la-carte-ecs-1.34.9/botocore_a_la_carte_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:49.000000 botocore-a-la-carte-ecs-1.34.9/botocore_a_la_carte_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:49.258337 botocore-a-la-carte-ecs-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-28 01:06:49.000000 botocore-a-la-carte-ecs-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-ecs-1.34.80/LICENSE.txt` & `botocore-a-la-carte-ecs-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.34.80/PKG-INFO` & `botocore-a-la-carte-ecs-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ecs
-Version: 1.34.80
+Version: 1.34.9
 Summary: ecs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/endpoint-rule-set-1.json` & `botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/examples-1.json` & `botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/paginators-1.json` & `botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/service-2.json` & `botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940403610023946%*

 * *Differences: {"'operations'": "{'CreateService': {'documentation': '<p>Runs and maintains your desired number "*

 * *                 'of tasks from a specified task definition. If the number of tasks running in a '*

 * *                 'service drops below the <code>desiredCount</code>, Amazon ECS runs another copy '*

 * *                 'of the task in the specified cluster. To update an existing service, see the '*

 * *                 '<a>UpdateService</a> action.</p> <note> <p>Starting April 15, 2023, Amazon Web '*

 * *                 ' […]*

```diff
@@ -69,15 +69,15 @@
             },
             "name": "CreateCluster",
             "output": {
                 "shape": "CreateClusterResponse"
             }
         },
         "CreateService": {
-            "documentation": "<p>Runs and maintains your desired number of tasks from a specified task definition. If the number of tasks running in a service drops below the <code>desiredCount</code>, Amazon ECS runs another copy of the task in the specified cluster. To update an existing service, see the <a>UpdateService</a> action.</p> <note> <p>On March 21, 2024, a change was made to resolve the task definition revision before authorization. When a task definition revision is not specified, authorization will occur using the latest revision of a task definition.</p> </note> <p>In addition to maintaining the desired count of tasks in your service, you can optionally run your service behind one or more load balancers. The load balancers distribute traffic across the tasks that are associated with the service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-load-balancing.html\">Service load balancing</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>You can attach Amazon EBS volumes to Amazon ECS tasks by configuring the volume when creating or updating a service. <code>volumeConfigurations</code> is only supported for REPLICA service and not DAEMON service. For more infomation, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ebs-volumes.html#ebs-volume-types\">Amazon EBS volumes</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Tasks for services that don't use a load balancer are considered healthy if they're in the <code>RUNNING</code> state. Tasks for services that use a load balancer are considered healthy if they're in the <code>RUNNING</code> state and are reported as healthy by the load balancer.</p> <p>There are two service scheduler strategies available:</p> <ul> <li> <p> <code>REPLICA</code> - The replica scheduling strategy places and maintains your desired number of tasks across your cluster. By default, the service scheduler spreads tasks across Availability Zones. You can use task placement strategies and constraints to customize task placement decisions. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html\">Service scheduler concepts</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> <li> <p> <code>DAEMON</code> - The daemon scheduling strategy deploys exactly one task on each active container instance that meets all of the task placement constraints that you specify in your cluster. The service scheduler also evaluates the task placement constraints for running tasks. It also stops tasks that don't meet the placement constraints. When using this strategy, you don't need to specify a desired number of tasks, a task placement strategy, or use Service Auto Scaling policies. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html\">Service scheduler concepts</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> </ul> <p>You can optionally specify a deployment configuration for your service. The deployment is initiated by changing properties. For example, the deployment might be initiated by the task definition or by your desired count of a service. This is done with an <a>UpdateService</a> operation. The default value for a replica service for <code>minimumHealthyPercent</code> is 100%. The default value for a daemon service for <code>minimumHealthyPercent</code> is 0%.</p> <p>If a service uses the <code>ECS</code> deployment controller, the minimum healthy percent represents a lower limit on the number of tasks in a service that must remain in the <code>RUNNING</code> state during a deployment. Specifically, it represents it as a percentage of your desired number of tasks (rounded up to the nearest integer). This happens when any of your container instances are in the <code>DRAINING</code> state if the service contains tasks using the EC2 launch type. Using this parameter, you can deploy without using additional cluster capacity. For example, if you set your service to have desired number of four tasks and a minimum healthy percent of 50%, the scheduler might stop two existing tasks to free up cluster capacity before starting two new tasks. If they're in the <code>RUNNING</code> state, tasks for services that don't use a load balancer are considered healthy . If they're in the <code>RUNNING</code> state and reported as healthy by the load balancer, tasks for services that <i>do</i> use a load balancer are considered healthy . The default value for minimum healthy percent is 100%.</p> <p>If a service uses the <code>ECS</code> deployment controller, the <b>maximum percent</b> parameter represents an upper limit on the number of tasks in a service that are allowed in the <code>RUNNING</code> or <code>PENDING</code> state during a deployment. Specifically, it represents it as a percentage of the desired number of tasks (rounded down to the nearest integer). This happens when any of your container instances are in the <code>DRAINING</code> state if the service contains tasks using the EC2 launch type. Using this parameter, you can define the deployment batch size. For example, if your service has a desired number of four tasks and a maximum percent value of 200%, the scheduler may start four new tasks before stopping the four older tasks (provided that the cluster resources required to do this are available). The default value for maximum percent is 200%.</p> <p>If a service uses either the <code>CODE_DEPLOY</code> or <code>EXTERNAL</code> deployment controller types and tasks that use the EC2 launch type, the <b>minimum healthy percent</b> and <b>maximum percent</b> values are used only to define the lower and upper limit on the number of the tasks in the service that remain in the <code>RUNNING</code> state. This is while the container instances are in the <code>DRAINING</code> state. If the tasks in the service use the Fargate launch type, the minimum healthy percent and maximum percent values aren't used. This is the case even if they're currently visible when describing your service.</p> <p>When creating a service that uses the <code>EXTERNAL</code> deployment controller, you can specify only parameters that aren't controlled at the task set level. The only required parameter is the service name. You control your services using the <a>CreateTaskSet</a> operation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">Amazon ECS deployment types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When the service scheduler launches new tasks, it determines task placement. For information about task placement and task placement strategies, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement.html\">Amazon ECS task placement</a> in the <i>Amazon Elastic Container Service Developer Guide</i> </p> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service. </p>",
+            "documentation": "<p>Runs and maintains your desired number of tasks from a specified task definition. If the number of tasks running in a service drops below the <code>desiredCount</code>, Amazon ECS runs another copy of the task in the specified cluster. To update an existing service, see the <a>UpdateService</a> action.</p> <note> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service. </p> </note> <p>In addition to maintaining the desired count of tasks in your service, you can optionally run your service behind one or more load balancers. The load balancers distribute traffic across the tasks that are associated with the service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-load-balancing.html\">Service load balancing</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Tasks for services that don't use a load balancer are considered healthy if they're in the <code>RUNNING</code> state. Tasks for services that use a load balancer are considered healthy if they're in the <code>RUNNING</code> state and are reported as healthy by the load balancer.</p> <p>There are two service scheduler strategies available:</p> <ul> <li> <p> <code>REPLICA</code> - The replica scheduling strategy places and maintains your desired number of tasks across your cluster. By default, the service scheduler spreads tasks across Availability Zones. You can use task placement strategies and constraints to customize task placement decisions. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html\">Service scheduler concepts</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> <li> <p> <code>DAEMON</code> - The daemon scheduling strategy deploys exactly one task on each active container instance that meets all of the task placement constraints that you specify in your cluster. The service scheduler also evaluates the task placement constraints for running tasks. It also stops tasks that don't meet the placement constraints. When using this strategy, you don't need to specify a desired number of tasks, a task placement strategy, or use Service Auto Scaling policies. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html\">Service scheduler concepts</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> </ul> <p>You can optionally specify a deployment configuration for your service. The deployment is initiated by changing properties. For example, the deployment might be initiated by the task definition or by your desired count of a service. This is done with an <a>UpdateService</a> operation. The default value for a replica service for <code>minimumHealthyPercent</code> is 100%. The default value for a daemon service for <code>minimumHealthyPercent</code> is 0%.</p> <p>If a service uses the <code>ECS</code> deployment controller, the minimum healthy percent represents a lower limit on the number of tasks in a service that must remain in the <code>RUNNING</code> state during a deployment. Specifically, it represents it as a percentage of your desired number of tasks (rounded up to the nearest integer). This happens when any of your container instances are in the <code>DRAINING</code> state if the service contains tasks using the EC2 launch type. Using this parameter, you can deploy without using additional cluster capacity. For example, if you set your service to have desired number of four tasks and a minimum healthy percent of 50%, the scheduler might stop two existing tasks to free up cluster capacity before starting two new tasks. If they're in the <code>RUNNING</code> state, tasks for services that don't use a load balancer are considered healthy . If they're in the <code>RUNNING</code> state and reported as healthy by the load balancer, tasks for services that <i>do</i> use a load balancer are considered healthy . The default value for minimum healthy percent is 100%.</p> <p>If a service uses the <code>ECS</code> deployment controller, the <b>maximum percent</b> parameter represents an upper limit on the number of tasks in a service that are allowed in the <code>RUNNING</code> or <code>PENDING</code> state during a deployment. Specifically, it represents it as a percentage of the desired number of tasks (rounded down to the nearest integer). This happens when any of your container instances are in the <code>DRAINING</code> state if the service contains tasks using the EC2 launch type. Using this parameter, you can define the deployment batch size. For example, if your service has a desired number of four tasks and a maximum percent value of 200%, the scheduler may start four new tasks before stopping the four older tasks (provided that the cluster resources required to do this are available). The default value for maximum percent is 200%.</p> <p>If a service uses either the <code>CODE_DEPLOY</code> or <code>EXTERNAL</code> deployment controller types and tasks that use the EC2 launch type, the <b>minimum healthy percent</b> and <b>maximum percent</b> values are used only to define the lower and upper limit on the number of the tasks in the service that remain in the <code>RUNNING</code> state. This is while the container instances are in the <code>DRAINING</code> state. If the tasks in the service use the Fargate launch type, the minimum healthy percent and maximum percent values aren't used. This is the case even if they're currently visible when describing your service.</p> <p>When creating a service that uses the <code>EXTERNAL</code> deployment controller, you can specify only parameters that aren't controlled at the task set level. The only required parameter is the service name. You control your services using the <a>CreateTaskSet</a> operation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">Amazon ECS deployment types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When the service scheduler launches new tasks, it determines task placement. For information about task placement and task placement strategies, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement.html\">Amazon ECS task placement</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -112,15 +112,15 @@
             },
             "name": "CreateService",
             "output": {
                 "shape": "CreateServiceResponse"
             }
         },
         "CreateTaskSet": {
-            "documentation": "<p>Create a task set in the specified cluster and service. This is used when a service uses the <code>EXTERNAL</code> deployment controller type. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">Amazon ECS deployment types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <note> <p>On March 21, 2024, a change was made to resolve the task definition revision before authorization. When a task definition revision is not specified, authorization will occur using the latest revision of a task definition.</p> </note> <p>For information about the maximum number of task sets and otther quotas, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-quotas.html\">Amazon ECS service quotas</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<p>Create a task set in the specified cluster and service. This is used when a service uses the <code>EXTERNAL</code> deployment controller type. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">Amazon ECS deployment types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -988,15 +988,15 @@
             },
             "name": "ListTasks",
             "output": {
                 "shape": "ListTasksResponse"
             }
         },
         "PutAccountSetting": {
-            "documentation": "<p>Modifies an account setting. Account settings are set on a per-Region basis.</p> <p>If you change the root user account setting, the default settings are reset for users and roles that do not have specified individual account settings. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-account-settings.html\">Account Settings</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<p>Modifies an account setting. Account settings are set on a per-Region basis.</p> <p>If you change the root user account setting, the default settings are reset for users and roles that do not have specified individual account settings. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-account-settings.html\">Account Settings</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When you specify <code>serviceLongArnFormat</code>, <code>taskLongArnFormat</code>, or <code>containerInstanceLongArnFormat</code>, the Amazon Resource Name (ARN) and resource ID format of the resource type for a specified user, role, or the root user for an account is affected. The opt-in and opt-out account setting must be set for each Amazon ECS resource separately. The ARN and resource ID format of a resource is defined by the opt-in status of the user or role that created the resource. You must turn on this setting to use Amazon ECS features such as resource tagging.</p> <p>When you specify <code>awsvpcTrunking</code>, the elastic network interface (ENI) limit for any new container instances that support the feature is changed. If <code>awsvpcTrunking</code> is turned on, any new container instances that support the feature are launched have the increased ENI limits available to them. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/container-instance-eni.html\">Elastic Network Interface Trunking</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When you specify <code>containerInsights</code>, the default setting indicating whether Amazon Web Services CloudWatch Container Insights is turned on for your clusters is changed. If <code>containerInsights</code> is turned on, any new clusters that are created will have Container Insights turned on unless you disable it during cluster creation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/cloudwatch-container-insights.html\">CloudWatch Container Insights</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Amazon ECS is introducing tagging authorization for resource creation. Users must have permissions for actions that create the resource, such as <code>ecsCreateCluster</code>. If tags are specified when you create a resource, Amazon Web Services performs additional authorization to verify if users or roles have permissions to create tags. Therefore, you must grant explicit permissions to use the <code>ecs:TagResource</code> action. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/supported-iam-actions-tagging.html\">Grant permission to tag resources on creation</a> in the <i>Amazon ECS Developer Guide</i>.</p> <p>When Amazon Web Services determines that a security or infrastructure update is needed for an Amazon ECS task hosted on Fargate, the tasks need to be stopped and new tasks launched to replace them. Use <code>fargateTaskRetirementWaitPeriod</code> to configure the wait time to retire a Fargate task. For information about the Fargate tasks maintenance, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-maintenance.html\">Amazon Web Services Fargate task maintenance</a> in the <i>Amazon ECS Developer Guide</i>.</p> <p>The <code>guardDutyActivate</code> parameter is read-only in Amazon ECS and indicates whether Amazon ECS Runtime Monitoring is enabled or disabled by your security administrator in your Amazon ECS account. Amazon GuardDuty controls this account setting on your behalf. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-guard-duty-integration.html\">Protecting Amazon ECS workloads with Amazon ECS Runtime Monitoring</a>.</p>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -1150,15 +1150,15 @@
             },
             "name": "RegisterTaskDefinition",
             "output": {
                 "shape": "RegisterTaskDefinitionResponse"
             }
         },
         "RunTask": {
-            "documentation": "<p>Starts a new task using the specified task definition.</p> <note> <p>On March 21, 2024, a change was made to resolve the task definition revision before authorization. When a task definition revision is not specified, authorization will occur using the latest revision of a task definition.</p> </note> <p>You can allow Amazon ECS to place tasks for you, or you can customize how Amazon ECS places tasks using placement constraints and placement strategies. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html\">Scheduling Tasks</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Alternatively, you can use <a>StartTask</a> to use your own scheduler or place tasks manually on specific container instances.</p> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service. </p> <p>You can attach Amazon EBS volumes to Amazon ECS tasks by configuring the volume when creating or updating a service. For more infomation, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ebs-volumes.html#ebs-volume-types\">Amazon EBS volumes</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>The Amazon ECS API follows an eventual consistency model. This is because of the distributed nature of the system supporting the API. This means that the result of an API command you run that affects your Amazon ECS resources might not be immediately visible to all subsequent commands you run. Keep this in mind when you carry out an API command that immediately follows a previous API command.</p> <p>To manage eventual consistency, you can do the following:</p> <ul> <li> <p>Confirm the state of the resource before you run a command to modify it. Run the DescribeTasks command using an exponential backoff algorithm to ensure that you allow enough time for the previous command to propagate through the system. To do this, run the DescribeTasks command repeatedly, starting with a couple of seconds of wait time and increasing gradually up to five minutes of wait time.</p> </li> <li> <p>Add wait time between subsequent commands, even if the DescribeTasks command returns an accurate response. Apply an exponential backoff algorithm starting with a couple of seconds of wait time, and increase gradually up to about five minutes of wait time.</p> </li> </ul>",
+            "documentation": "<p>Starts a new task using the specified task definition.</p> <p>You can allow Amazon ECS to place tasks for you, or you can customize how Amazon ECS places tasks using placement constraints and placement strategies. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html\">Scheduling Tasks</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Alternatively, you can use <a>StartTask</a> to use your own scheduler or place tasks manually on specific container instances.</p> <note> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service. </p> </note> <p>The Amazon ECS API follows an eventual consistency model. This is because of the distributed nature of the system supporting the API. This means that the result of an API command you run that affects your Amazon ECS resources might not be immediately visible to all subsequent commands you run. Keep this in mind when you carry out an API command that immediately follows a previous API command.</p> <p>To manage eventual consistency, you can do the following:</p> <ul> <li> <p>Confirm the state of the resource before you run a command to modify it. Run the DescribeTasks command using an exponential backoff algorithm to ensure that you allow enough time for the previous command to propagate through the system. To do this, run the DescribeTasks command repeatedly, starting with a couple of seconds of wait time and increasing gradually up to five minutes of wait time.</p> </li> <li> <p>Add wait time between subsequent commands, even if the DescribeTasks command returns an accurate response. Apply an exponential backoff algorithm starting with a couple of seconds of wait time, and increase gradually up to about five minutes of wait time.</p> </li> </ul>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -1196,30 +1196,27 @@
             },
             "name": "RunTask",
             "output": {
                 "shape": "RunTaskResponse"
             }
         },
         "StartTask": {
-            "documentation": "<p>Starts a new task from the specified task definition on the specified container instance or instances.</p> <note> <p>On March 21, 2024, a change was made to resolve the task definition revision before authorization. When a task definition revision is not specified, authorization will occur using the latest revision of a task definition.</p> </note> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service. </p> <p>Alternatively, you can use <a>RunTask</a> to place tasks for you. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html\">Scheduling Tasks</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>You can attach Amazon EBS volumes to Amazon ECS tasks by configuring the volume when creating or updating a service. For more infomation, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ebs-volumes.html#ebs-volume-types\">Amazon EBS volumes</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<p>Starts a new task from the specified task definition on the specified container instance or instances.</p> <note> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service. </p> </note> <p>Alternatively, you can use <a>RunTask</a> to place tasks for you. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html\">Scheduling Tasks</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
                 {
                     "shape": "InvalidParameterException"
                 },
                 {
                     "shape": "ClusterNotFoundException"
-                },
-                {
-                    "shape": "UnsupportedFeatureException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -1547,15 +1544,15 @@
             },
             "name": "UpdateContainerInstancesState",
             "output": {
                 "shape": "UpdateContainerInstancesStateResponse"
             }
         },
         "UpdateService": {
-            "documentation": "<p>Modifies the parameters of a service.</p> <note> <p>On March 21, 2024, a change was made to resolve the task definition revision before authorization. When a task definition revision is not specified, authorization will occur using the latest revision of a task definition.</p> </note> <p>For services using the rolling update (<code>ECS</code>) you can update the desired count, deployment configuration, network configuration, load balancers, service registries, enable ECS managed tags option, propagate tags option, task placement constraints and strategies, and task definition. When you update any of these parameters, Amazon ECS starts new tasks with the new configuration. </p> <p>You can attach Amazon EBS volumes to Amazon ECS tasks by configuring the volume when starting or running a task, or when creating or updating a service. For more infomation, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ebs-volumes.html#ebs-volume-types\">Amazon EBS volumes</a> in the <i>Amazon Elastic Container Service Developer Guide</i>. You can update your volume configurations and trigger a new deployment. <code>volumeConfigurations</code> is only supported for REPLICA service and not DAEMON service. If you leave <code>volumeConfigurations</code> <code>null</code>, it doesn't trigger a new deployment. For more infomation on volumes, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ebs-volumes.html#ebs-volume-types\">Amazon EBS volumes</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>For services using the blue/green (<code>CODE_DEPLOY</code>) deployment controller, only the desired count, deployment configuration, health check grace period, task placement constraints and strategies, enable ECS managed tags option, and propagate tags can be updated using this API. If the network configuration, platform version, task definition, or load balancer need to be updated, create a new CodeDeploy deployment. For more information, see <a href=\"https://docs.aws.amazon.com/codedeploy/latest/APIReference/API_CreateDeployment.html\">CreateDeployment</a> in the <i>CodeDeploy API Reference</i>.</p> <p>For services using an external deployment controller, you can update only the desired count, task placement constraints and strategies, health check grace period, enable ECS managed tags option, and propagate tags option, using this API. If the launch type, load balancer, network configuration, platform version, or task definition need to be updated, create a new task set For more information, see <a>CreateTaskSet</a>.</p> <p>You can add to or subtract from the number of instantiations of a task definition in a service by specifying the cluster that the service is running in and a new <code>desiredCount</code> parameter.</p> <p>You can attach Amazon EBS volumes to Amazon ECS tasks by configuring the volume when starting or running a task, or when creating or updating a service. For more infomation, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ebs-volumes.html#ebs-volume-types\">Amazon EBS volumes</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>If you have updated the container image of your application, you can create a new task definition with that image and deploy it to your service. The service scheduler uses the minimum healthy percent and maximum percent parameters (in the service's deployment configuration) to determine the deployment strategy.</p> <note> <p>If your updated Docker image uses the same tag as what is in the existing task definition for your service (for example, <code>my_image:latest</code>), you don't need to create a new revision of your task definition. You can update the service using the <code>forceNewDeployment</code> option. The new tasks launched by the deployment pull the current image/tag combination from your repository when they start.</p> </note> <p>You can also update the deployment configuration of a service. When a deployment is triggered by updating the task definition of a service, the service scheduler uses the deployment configuration parameters, <code>minimumHealthyPercent</code> and <code>maximumPercent</code>, to determine the deployment strategy.</p> <ul> <li> <p>If <code>minimumHealthyPercent</code> is below 100%, the scheduler can ignore <code>desiredCount</code> temporarily during a deployment. For example, if <code>desiredCount</code> is four tasks, a minimum of 50% allows the scheduler to stop two existing tasks before starting two new tasks. Tasks for services that don't use a load balancer are considered healthy if they're in the <code>RUNNING</code> state. Tasks for services that use a load balancer are considered healthy if they're in the <code>RUNNING</code> state and are reported as healthy by the load balancer.</p> </li> <li> <p>The <code>maximumPercent</code> parameter represents an upper limit on the number of running tasks during a deployment. You can use it to define the deployment batch size. For example, if <code>desiredCount</code> is four tasks, a maximum of 200% starts four new tasks before stopping the four older tasks (provided that the cluster resources required to do this are available).</p> </li> </ul> <p>When <a>UpdateService</a> stops a task during a deployment, the equivalent of <code>docker stop</code> is issued to the containers running in the task. This results in a <code>SIGTERM</code> and a 30-second timeout. After this, <code>SIGKILL</code> is sent and the containers are forcibly stopped. If the container handles the <code>SIGTERM</code> gracefully and exits within 30 seconds from receiving it, no <code>SIGKILL</code> is sent.</p> <p>When the service scheduler launches new tasks, it determines task placement in your cluster with the following logic.</p> <ul> <li> <p>Determine which of the container instances in your cluster can support your service's task definition. For example, they have the required CPU, memory, ports, and container instance attributes.</p> </li> <li> <p>By default, the service scheduler attempts to balance tasks across Availability Zones in this manner even though you can choose a different placement strategy.</p> <ul> <li> <p>Sort the valid container instances by the fewest number of running tasks for this service in the same Availability Zone as the instance. For example, if zone A has one running service task and zones B and C each have zero, valid container instances in either zone B or C are considered optimal for placement.</p> </li> <li> <p>Place the new service task on a valid container instance in an optimal Availability Zone (based on the previous steps), favoring container instances with the fewest number of running tasks for this service.</p> </li> </ul> </li> </ul> <p>When the service scheduler stops running tasks, it attempts to maintain balance across the Availability Zones in your cluster using the following logic: </p> <ul> <li> <p>Sort the container instances by the largest number of running tasks for this service in the same Availability Zone as the instance. For example, if zone A has one running service task and zones B and C each have two, container instances in either zone B or C are considered optimal for termination.</p> </li> <li> <p>Stop the task on a container instance in an optimal Availability Zone (based on the previous steps), favoring container instances with the largest number of running tasks for this service.</p> </li> </ul> <note> <p>You must have a service-linked role when you update any of the following service properties:</p> <ul> <li> <p> <code>loadBalancers</code>,</p> </li> <li> <p> <code>serviceRegistries</code> </p> </li> </ul> <p>For more information about the role see the <code>CreateService</code> request parameter <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html#ECS-CreateService-request-role\"> <code>role</code> </a>. </p> </note>",
+            "documentation": "<p>Modifies the parameters of a service.</p> <p>For services using the rolling update (<code>ECS</code>) you can update the desired count, deployment configuration, network configuration, load balancers, service registries, enable ECS managed tags option, propagate tags option, task placement constraints and strategies, and task definition. When you update any of these parameters, Amazon ECS starts new tasks with the new configuration. </p> <p>For services using the blue/green (<code>CODE_DEPLOY</code>) deployment controller, only the desired count, deployment configuration, health check grace period, task placement constraints and strategies, enable ECS managed tags option, and propagate tags can be updated using this API. If the network configuration, platform version, task definition, or load balancer need to be updated, create a new CodeDeploy deployment. For more information, see <a href=\"https://docs.aws.amazon.com/codedeploy/latest/APIReference/API_CreateDeployment.html\">CreateDeployment</a> in the <i>CodeDeploy API Reference</i>.</p> <p>For services using an external deployment controller, you can update only the desired count, task placement constraints and strategies, health check grace period, enable ECS managed tags option, and propagate tags option, using this API. If the launch type, load balancer, network configuration, platform version, or task definition need to be updated, create a new task set For more information, see <a>CreateTaskSet</a>.</p> <p>You can add to or subtract from the number of instantiations of a task definition in a service by specifying the cluster that the service is running in and a new <code>desiredCount</code> parameter.</p> <p>If you have updated the Docker image of your application, you can create a new task definition with that image and deploy it to your service. The service scheduler uses the minimum healthy percent and maximum percent parameters (in the service's deployment configuration) to determine the deployment strategy.</p> <note> <p>If your updated Docker image uses the same tag as what is in the existing task definition for your service (for example, <code>my_image:latest</code>), you don't need to create a new revision of your task definition. You can update the service using the <code>forceNewDeployment</code> option. The new tasks launched by the deployment pull the current image/tag combination from your repository when they start.</p> </note> <p>You can also update the deployment configuration of a service. When a deployment is triggered by updating the task definition of a service, the service scheduler uses the deployment configuration parameters, <code>minimumHealthyPercent</code> and <code>maximumPercent</code>, to determine the deployment strategy.</p> <ul> <li> <p>If <code>minimumHealthyPercent</code> is below 100%, the scheduler can ignore <code>desiredCount</code> temporarily during a deployment. For example, if <code>desiredCount</code> is four tasks, a minimum of 50% allows the scheduler to stop two existing tasks before starting two new tasks. Tasks for services that don't use a load balancer are considered healthy if they're in the <code>RUNNING</code> state. Tasks for services that use a load balancer are considered healthy if they're in the <code>RUNNING</code> state and are reported as healthy by the load balancer.</p> </li> <li> <p>The <code>maximumPercent</code> parameter represents an upper limit on the number of running tasks during a deployment. You can use it to define the deployment batch size. For example, if <code>desiredCount</code> is four tasks, a maximum of 200% starts four new tasks before stopping the four older tasks (provided that the cluster resources required to do this are available).</p> </li> </ul> <p>When <a>UpdateService</a> stops a task during a deployment, the equivalent of <code>docker stop</code> is issued to the containers running in the task. This results in a <code>SIGTERM</code> and a 30-second timeout. After this, <code>SIGKILL</code> is sent and the containers are forcibly stopped. If the container handles the <code>SIGTERM</code> gracefully and exits within 30 seconds from receiving it, no <code>SIGKILL</code> is sent.</p> <p>When the service scheduler launches new tasks, it determines task placement in your cluster with the following logic.</p> <ul> <li> <p>Determine which of the container instances in your cluster can support your service's task definition. For example, they have the required CPU, memory, ports, and container instance attributes.</p> </li> <li> <p>By default, the service scheduler attempts to balance tasks across Availability Zones in this manner even though you can choose a different placement strategy.</p> <ul> <li> <p>Sort the valid container instances by the fewest number of running tasks for this service in the same Availability Zone as the instance. For example, if zone A has one running service task and zones B and C each have zero, valid container instances in either zone B or C are considered optimal for placement.</p> </li> <li> <p>Place the new service task on a valid container instance in an optimal Availability Zone (based on the previous steps), favoring container instances with the fewest number of running tasks for this service.</p> </li> </ul> </li> </ul> <p>When the service scheduler stops running tasks, it attempts to maintain balance across the Availability Zones in your cluster using the following logic: </p> <ul> <li> <p>Sort the container instances by the largest number of running tasks for this service in the same Availability Zone as the instance. For example, if zone A has one running service task and zones B and C each have two, container instances in either zone B or C are considered optimal for termination.</p> </li> <li> <p>Stop the task on a container instance in an optimal Availability Zone (based on the previous steps), favoring container instances with the largest number of running tasks for this service.</p> </li> </ul> <note> <p>You must have a service-linked role when you update any of the following service properties:</p> <ul> <li> <p> <code>loadBalancers</code>,</p> </li> <li> <p> <code>serviceRegistries</code> </p> </li> </ul> <p>For more information about the role see the <code>CreateService</code> request parameter <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html#ECS-CreateService-request-role\"> <code>role</code> </a>. </p> </note>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -1578,17 +1575,14 @@
                     "shape": "PlatformTaskDefinitionIncompatibilityException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "NamespaceNotFoundException"
-                },
-                {
-                    "shape": "UnsupportedFeatureException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -1756,27 +1750,27 @@
             ],
             "type": "string"
         },
         "Attachment": {
             "documentation": "<p>An object representing a container instance or task attachment.</p>",
             "members": {
                 "details": {
-                    "documentation": "<p>Details of the attachment.</p> <p>For elastic network interfaces, this includes the network interface ID, the MAC address, the subnet ID, and the private IPv4 address.</p> <p>For Service Connect services, this includes <code>portName</code>, <code>clientAliases</code>, <code>discoveryName</code>, and <code>ingressPortOverride</code>.</p> <p>For Elastic Block Storage, this includes <code>roleArn</code>, <code>deleteOnTermination</code>, <code>volumeName</code>, <code>volumeId</code>, and <code>statusReason</code> (only when the attachment fails to create or attach).</p>",
+                    "documentation": "<p>Details of the attachment. For elastic network interfaces, this includes the network interface ID, the MAC address, the subnet ID, and the private IPv4 address.</p>",
                     "shape": "AttachmentDetails"
                 },
                 "id": {
                     "documentation": "<p>The unique identifier for the attachment.</p>",
                     "shape": "String"
                 },
                 "status": {
                     "documentation": "<p> The status of the attachment. Valid values are <code>PRECREATED</code>, <code>CREATED</code>, <code>ATTACHING</code>, <code>ATTACHED</code>, <code>DETACHING</code>, <code>DETACHED</code>, <code>DELETED</code>, and <code>FAILED</code>.</p>",
                     "shape": "String"
                 },
                 "type": {
-                    "documentation": "<p>The type of the attachment, such as <code>ElasticNetworkInterface</code>, <code>Service Connect</code>, and <code>AmazonElasticBlockStorage</code>.</p>",
+                    "documentation": "<p>The type of the attachment, such as <code>ElasticNetworkInterface</code>.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "AttachmentDetails": {
             "member": {
@@ -1854,18 +1848,14 @@
         "AutoScalingGroupProvider": {
             "documentation": "<p>The details of the Auto Scaling group for the capacity provider.</p>",
             "members": {
                 "autoScalingGroupArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) that identifies the Auto Scaling group, or the Auto Scaling group name.</p>",
                     "shape": "String"
                 },
-                "managedDraining": {
-                    "documentation": "<p>The managed draining option for the Auto Scaling group capacity provider. When you enable this, Amazon ECS manages and gracefully drains the EC2 container instances that are in the Auto Scaling group capacity provider.</p>",
-                    "shape": "ManagedDraining"
-                },
                 "managedScaling": {
                     "documentation": "<p>The managed scaling settings for the Auto Scaling group capacity provider.</p>",
                     "shape": "ManagedScaling"
                 },
                 "managedTerminationProtection": {
                     "documentation": "<p>The managed termination protection setting to use for the Auto Scaling group capacity provider. This determines whether the Auto Scaling group has managed termination protection. The default is off.</p> <important> <p>When using managed termination protection, managed scaling must also be used otherwise managed termination protection doesn't work.</p> </important> <p>When managed termination protection is on, Amazon ECS prevents the Amazon EC2 instances in an Auto Scaling group that contain tasks from being terminated during a scale-in action. The Auto Scaling group and each instance in the Auto Scaling group must have instance protection from scale-in actions on as well. For more information, see <a href=\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-instance-termination.html#instance-protection\">Instance Protection</a> in the <i>Auto Scaling User Guide</i>.</p> <p>When managed termination protection is off, your Amazon EC2 instances aren't protected from termination when the Auto Scaling group scales in.</p>",
                     "shape": "ManagedTerminationProtection"
@@ -1875,31 +1865,27 @@
                 "autoScalingGroupArn"
             ],
             "type": "structure"
         },
         "AutoScalingGroupProviderUpdate": {
             "documentation": "<p>The details of the Auto Scaling group capacity provider to update.</p>",
             "members": {
-                "managedDraining": {
-                    "documentation": "<p>The managed draining option for the Auto Scaling group capacity provider. When you enable this, Amazon ECS manages and gracefully drains the EC2 container instances that are in the Auto Scaling group capacity provider.</p>",
-                    "shape": "ManagedDraining"
-                },
                 "managedScaling": {
                     "documentation": "<p>The managed scaling settings for the Auto Scaling group capacity provider.</p>",
                     "shape": "ManagedScaling"
                 },
                 "managedTerminationProtection": {
                     "documentation": "<p>The managed termination protection setting to use for the Auto Scaling group capacity provider. This determines whether the Auto Scaling group has managed termination protection.</p> <important> <p>When using managed termination protection, managed scaling must also be used otherwise managed termination protection doesn't work.</p> </important> <p>When managed termination protection is on, Amazon ECS prevents the Amazon EC2 instances in an Auto Scaling group that contain tasks from being terminated during a scale-in action. The Auto Scaling group and each instance in the Auto Scaling group must have instance protection from scale-in actions on. For more information, see <a href=\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-instance-termination.html#instance-protection\">Instance Protection</a> in the <i>Auto Scaling User Guide</i>.</p> <p>When managed termination protection is off, your Amazon EC2 instances aren't protected from termination when the Auto Scaling group scales in.</p>",
                     "shape": "ManagedTerminationProtection"
                 }
             },
             "type": "structure"
         },
         "AwsVpcConfiguration": {
-            "documentation": "<p>An object representing the networking details for a task or service. For example <code>awsvpcConfiguration={subnets=[\"subnet-12344321\"],securityGroups=[\"sg-12344321\"]}</code> </p>",
+            "documentation": "<p>An object representing the networking details for a task or service.</p>",
             "members": {
                 "assignPublicIp": {
                     "documentation": "<p>Whether the task's elastic network interface receives a public IP address. The default value is <code>DISABLED</code>.</p>",
                     "shape": "AssignPublicIp"
                 },
                 "securityGroups": {
                     "documentation": "<p>The IDs of the security groups associated with the task or service. If you don't specify a security group, the default security group for the VPC is used. There's a limit of 5 security groups that can be specified per <code>AwsVpcConfiguration</code>.</p> <note> <p>All specified security groups must be from the same VPC.</p> </note>",
@@ -2047,15 +2033,14 @@
             "type": "list"
         },
         "ClientException": {
             "documentation": "<p>These errors are usually caused by a client action. This client action might be using an action or resource on behalf of a user that doesn't have permissions to use the action or resource. Or, it might be specifying an identifier that isn't valid.</p>",
             "exception": true,
             "members": {
                 "message": {
-                    "documentation": "<p> Message that describes the cause of the exception.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "Cluster": {
             "documentation": "<p>A regional grouping of one or more container instances where you can run task requests. Each account receives a default cluster the first time you use the Amazon ECS service, but you may also create other clusters. Clusters may contain more than one instance type simultaneously.</p>",
@@ -2487,19 +2472,19 @@
                     "shape": "BoxedInteger"
                 },
                 "stopTimeout": {
                     "documentation": "<p>Time duration (in seconds) to wait before the container is forcefully killed if it doesn't exit normally on its own.</p> <p>For tasks using the Fargate launch type, the task or service requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.3.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> <p>The max stop timeout value is 120 seconds and if the parameter is not specified, the default value of 30 seconds is used.</p> <p>For tasks that use the EC2 launch type, if the <code>stopTimeout</code> parameter isn't specified, the value set for the Amazon ECS container agent configuration variable <code>ECS_CONTAINER_STOP_TIMEOUT</code> is used. If neither the <code>stopTimeout</code> parameter or the <code>ECS_CONTAINER_STOP_TIMEOUT</code> agent configuration variable are set, then the default values of 30 seconds for Linux containers and 30 seconds on Windows containers are used. Your container instances require at least version 1.26.0 of the container agent to use a container stop timeout value. However, we recommend using the latest container agent version. For information about checking your agent version and updating to the latest version, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-update.html\">Updating the Amazon ECS Container Agent</a> in the <i>Amazon Elastic Container Service Developer Guide</i>. If you're using an Amazon ECS-optimized Linux AMI, your instance needs at least version 1.26.0-1 of the <code>ecs-init</code> package. If your container instances are launched from version <code>20190301</code> or later, then they contain the required versions of the container agent and <code>ecs-init</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-optimized_AMI.html\">Amazon ECS-optimized Linux AMI</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>The valid values are 2-120 seconds.</p>",
                     "shape": "BoxedInteger"
                 },
                 "systemControls": {
-                    "documentation": "<p>A list of namespaced kernel parameters to set in the container. This parameter maps to <code>Sysctls</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--sysctl</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>. For example, you can configure <code>net.ipv4.tcp_keepalive_time</code> setting to maintain longer lived connections.</p>",
+                    "documentation": "<p>A list of namespaced kernel parameters to set in the container. This parameter maps to <code>Sysctls</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--sysctl</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>. For example, you can configure <code>net.ipv4.tcp_keepalive_time</code> setting to maintain longer lived connections.</p> <note> <p>We don't recommended that you specify network-related <code>systemControls</code> parameters for multiple containers in a single task that also uses either the <code>awsvpc</code> or <code>host</code> network modes. For tasks that use the <code>awsvpc</code> network mode, the container that's started last determines which <code>systemControls</code> parameters take effect. For tasks that use the <code>host</code> network mode, it changes the container instance's namespaced kernel parameters as well as the containers.</p> </note> <note> <p>This parameter is not supported for Windows containers.</p> </note> <note> <p>This parameter is only supported for tasks that are hosted on Fargate if the tasks are using platform version <code>1.4.0</code> or later (Linux). This isn't supported for Windows containers on Fargate.</p> </note>",
                     "shape": "SystemControls"
                 },
                 "ulimits": {
-                    "documentation": "<p>A list of <code>ulimits</code> to set in the container. If a <code>ulimit</code> value is specified in a task definition, it overrides the default values set by Docker. This parameter maps to <code>Ulimits</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--ulimit</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>. Valid naming values are displayed in the <a>Ulimit</a> data type.</p> <p>Amazon ECS tasks hosted on Fargate use the default resource limit values set by the operating system with the exception of the <code>nofile</code> resource limit parameter which Fargate overrides. The <code>nofile</code> resource limit sets a restriction on the number of open files that a container can use. The default <code>nofile</code> soft limit is <code>1024</code> and the default hard limit is <code>65535</code>.</p> <p>This parameter requires version 1.18 of the Docker Remote API or greater on your container instance. To check the Docker Remote API version on your container instance, log in to your container instance and run the following command: <code>sudo docker version --format '{{.Server.APIVersion}}'</code> </p> <note> <p>This parameter is not supported for Windows containers.</p> </note>",
+                    "documentation": "<p>A list of <code>ulimits</code> to set in the container. If a <code>ulimit</code> value is specified in a task definition, it overrides the default values set by Docker. This parameter maps to <code>Ulimits</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--ulimit</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>. Valid naming values are displayed in the <a>Ulimit</a> data type.</p> <p>Amazon ECS tasks hosted on Fargate use the default resource limit values set by the operating system with the exception of the <code>nofile</code> resource limit parameter which Fargate overrides. The <code>nofile</code> resource limit sets a restriction on the number of open files that a container can use. The default <code>nofile</code> soft limit is <code>1024</code> and the default hard limit is <code>4096</code>.</p> <p>This parameter requires version 1.18 of the Docker Remote API or greater on your container instance. To check the Docker Remote API version on your container instance, log in to your container instance and run the following command: <code>sudo docker version --format '{{.Server.APIVersion}}'</code> </p> <note> <p>This parameter is not supported for Windows containers.</p> </note>",
                     "shape": "UlimitList"
                 },
                 "user": {
                     "documentation": "<p>The user to use inside the container. This parameter maps to <code>User</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--user</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <important> <p>When running tasks using the <code>host</code> network mode, don't run containers using the root user (UID 0). We recommend using a non-root user for better security.</p> </important> <p>You can specify the <code>user</code> using the following formats. If specifying a UID or GID, you must specify it as a positive integer.</p> <ul> <li> <p> <code>user</code> </p> </li> <li> <p> <code>user:group</code> </p> </li> <li> <p> <code>uid</code> </p> </li> <li> <p> <code>uid:gid</code> </p> </li> <li> <p> <code>user:gid</code> </p> </li> <li> <p> <code>uid:group</code> </p> </li> </ul> <note> <p>This parameter is not supported for Windows containers.</p> </note>",
                     "shape": "String"
                 },
                 "volumesFrom": {
@@ -2522,15 +2507,15 @@
         "ContainerDependencies": {
             "member": {
                 "shape": "ContainerDependency"
             },
             "type": "list"
         },
         "ContainerDependency": {
-            "documentation": "<p>The dependencies defined for container startup and shutdown. A container can contain multiple dependencies. When a dependency is defined for container startup, for container shutdown it is reversed.</p> <p>Your Amazon ECS container instances require at least version 1.26.0 of the container agent to use container dependencies. However, we recommend using the latest container agent version. For information about checking your agent version and updating to the latest version, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-update.html\">Updating the Amazon ECS Container Agent</a> in the <i>Amazon Elastic Container Service Developer Guide</i>. If you're using an Amazon ECS-optimized Linux AMI, your instance needs at least version 1.26.0-1 of the <code>ecs-init</code> package. If your container instances are launched from version <code>20190301</code> or later, then they contain the required versions of the container agent and <code>ecs-init</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-optimized_AMI.html\">Amazon ECS-optimized Linux AMI</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <note> <p>For tasks that use the Fargate launch type, the task or service requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.3.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> </note> <p>For more information about how to create a container dependency, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/example_task_definitions.html#example_task_definition-containerdependency\">Container dependency</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<p>The dependencies defined for container startup and shutdown. A container can contain multiple dependencies. When a dependency is defined for container startup, for container shutdown it is reversed.</p> <p>Your Amazon ECS container instances require at least version 1.26.0 of the container agent to use container dependencies. However, we recommend using the latest container agent version. For information about checking your agent version and updating to the latest version, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-update.html\">Updating the Amazon ECS Container Agent</a> in the <i>Amazon Elastic Container Service Developer Guide</i>. If you're using an Amazon ECS-optimized Linux AMI, your instance needs at least version 1.26.0-1 of the <code>ecs-init</code> package. If your container instances are launched from version <code>20190301</code> or later, then they contain the required versions of the container agent and <code>ecs-init</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-optimized_AMI.html\">Amazon ECS-optimized Linux AMI</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <note> <p>For tasks that use the Fargate launch type, the task or service requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.3.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> </note>",
             "members": {
                 "condition": {
                     "documentation": "<p>The dependency condition of the container. The following are the available conditions and their behavior:</p> <ul> <li> <p> <code>START</code> - This condition emulates the behavior of links and volumes today. It validates that a dependent container is started before permitting other containers to start.</p> </li> <li> <p> <code>COMPLETE</code> - This condition validates that a dependent container runs to completion (exits) before permitting other containers to start. This can be useful for nonessential containers that run a script and then exit. This condition can't be set on an essential container.</p> </li> <li> <p> <code>SUCCESS</code> - This condition is the same as <code>COMPLETE</code>, but it also requires that the container exits with a <code>zero</code> status. This condition can't be set on an essential container.</p> </li> <li> <p> <code>HEALTHY</code> - This condition validates that the dependent container passes its Docker health check before permitting other containers to start. This requires that the dependent container has health checks configured. This condition is confirmed only at task startup.</p> </li> </ul>",
                     "shape": "ContainerCondition"
                 },
                 "containerName": {
                     "documentation": "<p>The name of a container.</p>",
@@ -2861,15 +2846,15 @@
                     "shape": "Boolean"
                 },
                 "healthCheckGracePeriodSeconds": {
                     "documentation": "<p>The period of time, in seconds, that the Amazon ECS service scheduler ignores unhealthy Elastic Load Balancing target health checks after a task has first started. This is only used when your service is configured to use a load balancer. If your service has a load balancer defined and you don't specify a health check grace period value, the default value of <code>0</code> is used.</p> <p>If you do not use an Elastic Load Balancing, we recommend that you use the <code>startPeriod</code> in the task definition health check parameters. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_HealthCheck.html\">Health check</a>.</p> <p>If your service's tasks take a while to start and respond to Elastic Load Balancing health checks, you can specify a health check grace period of up to 2,147,483,647 seconds (about 69 years). During that time, the Amazon ECS service scheduler ignores health check status. This grace period can prevent the service scheduler from marking tasks as unhealthy and stopping them before they have time to come up.</p>",
                     "shape": "BoxedInteger"
                 },
                 "launchType": {
-                    "documentation": "<p>The infrastructure that you run your service on. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/launch_types.html\">Amazon ECS launch types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>The <code>FARGATE</code> launch type runs your tasks on Fargate On-Demand infrastructure.</p> <note> <p>Fargate Spot infrastructure is available for use but a capacity provider strategy must be used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/fargate-capacity-providers.html\">Fargate capacity providers</a> in the <i>Amazon ECS Developer Guide</i>.</p> </note> <p>The <code>EC2</code> launch type runs your tasks on Amazon EC2 instances registered to your cluster.</p> <p>The <code>EXTERNAL</code> launch type runs your tasks on your on-premises server or virtual machine (VM) capacity registered to your cluster.</p> <p>A service can use either a launch type or a capacity provider strategy. If a <code>launchType</code> is specified, the <code>capacityProviderStrategy</code> parameter must be omitted.</p>",
+                    "documentation": "<p>The infrastructure that you run your service on. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/launch_types.html\">Amazon ECS launch types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>The <code>FARGATE</code> launch type runs your tasks on Fargate On-Demand infrastructure.</p> <note> <p>Fargate Spot infrastructure is available for use but a capacity provider strategy must be used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/fargate-capacity-providers.html\">Fargate capacity providers</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> </note> <p>The <code>EC2</code> launch type runs your tasks on Amazon EC2 instances registered to your cluster.</p> <p>The <code>EXTERNAL</code> launch type runs your tasks on your on-premises server or virtual machine (VM) capacity registered to your cluster.</p> <p>A service can use either a launch type or a capacity provider strategy. If a <code>launchType</code> is specified, the <code>capacityProviderStrategy</code> parameter must be omitted.</p>",
                     "shape": "LaunchType"
                 },
                 "loadBalancers": {
                     "documentation": "<p>A load balancer object representing the load balancers to use with your service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-load-balancing.html\">Service load balancing</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>If the service uses the rolling update (<code>ECS</code>) deployment controller and using either an Application Load Balancer or Network Load Balancer, you must specify one or more target group ARNs to attach to the service. The service-linked role is required for services that use multiple target groups. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using-service-linked-roles.html\">Using service-linked roles for Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>If the service uses the <code>CODE_DEPLOY</code> deployment controller, the service is required to use either an Application Load Balancer or Network Load Balancer. When creating an CodeDeploy deployment group, you specify two target groups (referred to as a <code>targetGroupPair</code>). During a deployment, CodeDeploy determines which task set in your service has the status <code>PRIMARY</code>, and it associates one target group with it. Then, it also associates the other target group with the replacement task set. The load balancer can also have up to two listeners: a required listener for production traffic and an optional listener that you can use to perform validation tests with Lambda functions before routing production traffic to it.</p> <p>If you use the <code>CODE_DEPLOY</code> deployment controller, these values can be changed when updating the service.</p> <p>For Application Load Balancers and Network Load Balancers, this object must contain the load balancer target group ARN, the container name, and the container port to access from the load balancer. The container name must be as it appears in a container definition. The load balancer name parameter must be omitted. When a task from this service is placed on a container instance, the container instance and port combination is registered as a target in the target group that's specified here.</p> <p>For Classic Load Balancers, this object must contain the load balancer name, the container name , and the container port to access from the load balancer. The container name must be as it appears in a container definition. The target group ARN parameter must be omitted. When a task from this service is placed on a container instance, the container instance is registered with the load balancer that's specified here.</p> <p>Services with tasks that use the <code>awsvpc</code> network mode (for example, those with the Fargate launch type) only support Application Load Balancers and Network Load Balancers. Classic Load Balancers aren't supported. Also, when you create any target groups for these services, you must choose <code>ip</code> as the target type, not <code>instance</code>. This is because tasks that use the <code>awsvpc</code> network mode are associated with an elastic network interface, not an Amazon EC2 instance.</p>",
                     "shape": "LoadBalancers"
                 },
                 "networkConfiguration": {
@@ -2885,15 +2870,15 @@
                     "shape": "PlacementStrategies"
                 },
                 "platformVersion": {
                     "documentation": "<p>The platform version that your tasks in the service are running on. A platform version is specified only for tasks using the Fargate launch type. If one isn't specified, the <code>LATEST</code> platform version is used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html\">Fargate platform versions</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "String"
                 },
                 "propagateTags": {
-                    "documentation": "<p>Specifies whether to propagate the tags from the task definition to the task. If no value is specified, the tags aren't propagated. Tags can only be propagated to the task during task creation. To add tags to a task after task creation, use the <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_TagResource.html\">TagResource</a> API action.</p> <p>You must set this to a value other than <code>NONE</code> when you use Cost Explorer. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/usage-reports.html\">Amazon ECS usage reports</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>The default is <code>NONE</code>.</p>",
+                    "documentation": "<p>Specifies whether to propagate the tags from the task definition to the task. If no value is specified, the tags aren't propagated. Tags can only be propagated to the task during task creation. To add tags to a task after task creation, use the <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_TagResource.html\">TagResource</a> API action.</p> <p>The default is <code>NONE</code>.</p>",
                     "shape": "PropagateTags"
                 },
                 "role": {
                     "documentation": "<p>The name or full Amazon Resource Name (ARN) of the IAM role that allows Amazon ECS to make calls to your load balancer on your behalf. This parameter is only permitted if you are using a load balancer with your service and your task definition doesn't use the <code>awsvpc</code> network mode. If you specify the <code>role</code> parameter, you must also specify a load balancer object with the <code>loadBalancers</code> parameter.</p> <important> <p>If your account has already created the Amazon ECS service-linked role, that role is used for your service unless you specify a role here. The service-linked role is required if your task definition uses the <code>awsvpc</code> network mode or if the service is configured to use service discovery, an external deployment controller, multiple target groups, or Elastic Inference accelerators in which case you don't specify a role here. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using-service-linked-roles.html\">Using service-linked roles for Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </important> <p>If your specified role has a path other than <code>/</code>, then you must either specify the full role ARN (this is recommended) or prefix the role name with the path. For example, if a role with the name <code>bar</code> has a path of <code>/foo/</code> then you would specify <code>/foo/bar</code> as the role name. For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_identifiers.html#identifiers-friendly-names\">Friendly names and paths</a> in the <i>IAM User Guide</i>.</p>",
                     "shape": "String"
                 },
                 "schedulingStrategy": {
@@ -2915,18 +2900,14 @@
                 "tags": {
                     "documentation": "<p>The metadata that you apply to the service to help you categorize and organize them. Each tag consists of a key and an optional value, both of which you define. When a service is deleted, the tags are deleted as well.</p> <p>The following basic restrictions apply to tags:</p> <ul> <li> <p>Maximum number of tags per resource - 50</p> </li> <li> <p>For each resource, each tag key must be unique, and each tag key can have only one value.</p> </li> <li> <p>Maximum key length - 128 Unicode characters in UTF-8</p> </li> <li> <p>Maximum value length - 256 Unicode characters in UTF-8</p> </li> <li> <p>If your tagging schema is used across multiple services and resources, remember that other services may have restrictions on allowed characters. Generally allowed characters are: letters, numbers, and spaces representable in UTF-8, and the following characters: + - = . _ : / @.</p> </li> <li> <p>Tag keys and values are case-sensitive.</p> </li> <li> <p>Do not use <code>aws:</code>, <code>AWS:</code>, or any upper or lowercase combination of such as a prefix for either keys or values as it is reserved for Amazon Web Services use. You cannot edit or delete tag keys or values with this prefix. Tags with this prefix do not count against your tags per resource limit.</p> </li> </ul>",
                     "shape": "Tags"
                 },
                 "taskDefinition": {
                     "documentation": "<p>The <code>family</code> and <code>revision</code> (<code>family:revision</code>) or full ARN of the task definition to run in your service. If a <code>revision</code> isn't specified, the latest <code>ACTIVE</code> revision is used.</p> <p>A task definition must be specified if the service uses either the <code>ECS</code> or <code>CODE_DEPLOY</code> deployment controllers.</p> <p>For more information about deployment types, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">Amazon ECS deployment types</a>.</p>",
                     "shape": "String"
-                },
-                "volumeConfigurations": {
-                    "documentation": "<p>The configuration for a volume specified in the task definition as a volume that is configured at launch time. Currently, the only supported volume type is an Amazon EBS volume.</p>",
-                    "shape": "ServiceVolumeConfigurations"
                 }
             },
             "required": [
                 "serviceName"
             ],
             "type": "structure"
         },
@@ -3261,18 +3242,14 @@
                 "taskDefinition": {
                     "documentation": "<p>The most recent task definition that was specified for the tasks in the service to use.</p>",
                     "shape": "String"
                 },
                 "updatedAt": {
                     "documentation": "<p>The Unix timestamp for the time when the service deployment was last updated.</p>",
                     "shape": "Timestamp"
-                },
-                "volumeConfigurations": {
-                    "documentation": "<p>The details of the volume that was <code>configuredAtLaunch</code>. You can configure different settings like the size, throughput, volumeType, and ecryption in <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_ServiceManagedEBSVolumeConfiguration.html\">ServiceManagedEBSVolumeConfiguration</a>. The <code>name</code> of the volume must match the <code>name</code> from the task definition.</p>",
-                    "shape": "ServiceVolumeConfigurations"
                 }
             },
             "type": "structure"
         },
         "DeploymentAlarms": {
             "documentation": "<p>One of the methods which provide a way for you to quickly identify when a deployment has failed, and then to optionally roll back the failure to the last working deployment.</p> <p>When the alarms are generated, Amazon ECS sets the service deployment to failed. Set the rollback parameter to have Amazon ECS to roll back your service to the last completed deployment after a failure.</p> <p>You can only use the <code>DeploymentAlarms</code> method to detect failures when the <code>DeploymentController</code> is set to <code>ECS</code> (rolling update).</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-type-ecs.html\">Rolling update</a> in the <i> <i>Amazon Elastic Container Service Developer Guide</i> </i>.</p>",
             "members": {
@@ -3326,15 +3303,15 @@
                     "shape": "DeploymentCircuitBreaker"
                 },
                 "maximumPercent": {
                     "documentation": "<p>If a service is using the rolling update (<code>ECS</code>) deployment type, the <code>maximumPercent</code> parameter represents an upper limit on the number of your service's tasks that are allowed in the <code>RUNNING</code> or <code>PENDING</code> state during a deployment, as a percentage of the <code>desiredCount</code> (rounded down to the nearest integer). This parameter enables you to define the deployment batch size. For example, if your service is using the <code>REPLICA</code> service scheduler and has a <code>desiredCount</code> of four tasks and a <code>maximumPercent</code> value of 200%, the scheduler may start four new tasks before stopping the four older tasks (provided that the cluster resources required to do this are available). The default <code>maximumPercent</code> value for a service using the <code>REPLICA</code> service scheduler is 200%.</p> <p>If a service is using either the blue/green (<code>CODE_DEPLOY</code>) or <code>EXTERNAL</code> deployment types and tasks that use the EC2 launch type, the <b>maximum percent</b> value is set to the default value and is used to define the upper limit on the number of the tasks in the service that remain in the <code>RUNNING</code> state while the container instances are in the <code>DRAINING</code> state. If the tasks in the service use the Fargate launch type, the maximum percent value is not used, although it is returned when describing your service.</p>",
                     "shape": "BoxedInteger"
                 },
                 "minimumHealthyPercent": {
-                    "documentation": "<p>If a service is using the rolling update (<code>ECS</code>) deployment type, the <code>minimumHealthyPercent</code> represents a lower limit on the number of your service's tasks that must remain in the <code>RUNNING</code> state during a deployment, as a percentage of the <code>desiredCount</code> (rounded up to the nearest integer). This parameter enables you to deploy without using additional cluster capacity. For example, if your service has a <code>desiredCount</code> of four tasks and a <code>minimumHealthyPercent</code> of 50%, the service scheduler may stop two existing tasks to free up cluster capacity before starting two new tasks. </p> <p>For services that <i>do not</i> use a load balancer, the following should be noted:</p> <ul> <li> <p>A service is considered healthy if all essential containers within the tasks in the service pass their health checks.</p> </li> <li> <p>If a task has no essential containers with a health check defined, the service scheduler will wait for 40 seconds after a task reaches a <code>RUNNING</code> state before the task is counted towards the minimum healthy percent total.</p> </li> <li> <p>If a task has one or more essential containers with a health check defined, the service scheduler will wait for the task to reach a healthy status before counting it towards the minimum healthy percent total. A task is considered healthy when all essential containers within the task have passed their health checks. The amount of time the service scheduler can wait for is determined by the container health check settings. </p> </li> </ul> <p>For services that <i>do</i> use a load balancer, the following should be noted:</p> <ul> <li> <p>If a task has no essential containers with a health check defined, the service scheduler will wait for the load balancer target group health check to return a healthy status before counting the task towards the minimum healthy percent total.</p> </li> <li> <p>If a task has an essential container with a health check defined, the service scheduler will wait for both the task to reach a healthy status and the load balancer target group health check to return a healthy status before counting the task towards the minimum healthy percent total.</p> </li> </ul> <p>The default value for a replica service for <code>minimumHealthyPercent</code> is 100%. The default <code>minimumHealthyPercent</code> value for a service using the <code>DAEMON</code> service schedule is 0% for the CLI, the Amazon Web Services SDKs, and the APIs and 50% for the Amazon Web Services Management Console.</p> <p>The minimum number of healthy tasks during a deployment is the <code>desiredCount</code> multiplied by the <code>minimumHealthyPercent</code>/100, rounded up to the nearest integer value.</p> <p>If a service is using either the blue/green (<code>CODE_DEPLOY</code>) or <code>EXTERNAL</code> deployment types and is running tasks that use the EC2 launch type, the <b>minimum healthy percent</b> value is set to the default value and is used to define the lower limit on the number of the tasks in the service that remain in the <code>RUNNING</code> state while the container instances are in the <code>DRAINING</code> state. If a service is using either the blue/green (<code>CODE_DEPLOY</code>) or <code>EXTERNAL</code> deployment types and is running tasks that use the Fargate launch type, the minimum healthy percent value is not used, although it is returned when describing your service.</p>",
+                    "documentation": "<p>If a service is using the rolling update (<code>ECS</code>) deployment type, the <code>minimumHealthyPercent</code> represents a lower limit on the number of your service's tasks that must remain in the <code>RUNNING</code> state during a deployment, as a percentage of the <code>desiredCount</code> (rounded up to the nearest integer). This parameter enables you to deploy without using additional cluster capacity. For example, if your service has a <code>desiredCount</code> of four tasks and a <code>minimumHealthyPercent</code> of 50%, the service scheduler may stop two existing tasks to free up cluster capacity before starting two new tasks. </p> <p>For services that <i>do not</i> use a load balancer, the following should be noted:</p> <ul> <li> <p>A service is considered healthy if all essential containers within the tasks in the service pass their health checks.</p> </li> <li> <p>If a task has no essential containers with a health check defined, the service scheduler will wait for 40 seconds after a task reaches a <code>RUNNING</code> state before the task is counted towards the minimum healthy percent total.</p> </li> <li> <p>If a task has one or more essential containers with a health check defined, the service scheduler will wait for the task to reach a healthy status before counting it towards the minimum healthy percent total. A task is considered healthy when all essential containers within the task have passed their health checks. The amount of time the service scheduler can wait for is determined by the container health check settings. </p> </li> </ul> <p>For services are that <i>do</i> use a load balancer, the following should be noted:</p> <ul> <li> <p>If a task has no essential containers with a health check defined, the service scheduler will wait for the load balancer target group health check to return a healthy status before counting the task towards the minimum healthy percent total.</p> </li> <li> <p>If a task has an essential container with a health check defined, the service scheduler will wait for both the task to reach a healthy status and the load balancer target group health check to return a healthy status before counting the task towards the minimum healthy percent total.</p> </li> </ul> <p>If a service is using either the blue/green (<code>CODE_DEPLOY</code>) or <code>EXTERNAL</code> deployment types and is running tasks that use the EC2 launch type, the <b>minimum healthy percent</b> value is set to the default value and is used to define the lower limit on the number of the tasks in the service that remain in the <code>RUNNING</code> state while the container instances are in the <code>DRAINING</code> state. If a service is using either the blue/green (<code>CODE_DEPLOY</code>) or <code>EXTERNAL</code> deployment types and is running tasks that use the Fargate launch type, the minimum healthy percent value is not used, although it is returned when describing your service.</p>",
                     "shape": "BoxedInteger"
                 }
             },
             "type": "structure"
         },
         "DeploymentController": {
             "documentation": "<p>The deployment controller to use for the service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">Amazon ECS deployment types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
@@ -3764,64 +3741,14 @@
                 }
             },
             "type": "structure"
         },
         "Double": {
             "type": "double"
         },
-        "Duration": {
-            "max": 2147483647,
-            "min": 0,
-            "type": "integer"
-        },
-        "EBSKMSKeyId": {
-            "type": "string"
-        },
-        "EBSResourceType": {
-            "enum": [
-                "volume"
-            ],
-            "type": "string"
-        },
-        "EBSSnapshotId": {
-            "type": "string"
-        },
-        "EBSTagSpecification": {
-            "documentation": "<p>The tag specifications of an Amazon EBS volume.</p>",
-            "members": {
-                "propagateTags": {
-                    "documentation": "<p>Determines whether to propagate the tags from the task definition to &#x2028;the Amazon EBS volume. Tags can only propagate to a <code>SERVICE</code> specified in &#x2028;<code>ServiceVolumeConfiguration</code>. If no value is specified, the tags aren't &#x2028;propagated.</p>",
-                    "shape": "PropagateTags"
-                },
-                "resourceType": {
-                    "documentation": "<p>The type of volume resource.</p>",
-                    "shape": "EBSResourceType"
-                },
-                "tags": {
-                    "documentation": "<p>The tags applied to this Amazon EBS volume. <code>AmazonECSCreated</code> and <code>AmazonECSManaged</code> are reserved tags that can't be used.</p>",
-                    "shape": "Tags"
-                }
-            },
-            "required": [
-                "resourceType"
-            ],
-            "type": "structure"
-        },
-        "EBSTagSpecifications": {
-            "member": {
-                "shape": "EBSTagSpecification"
-            },
-            "type": "list"
-        },
-        "EBSVolumeType": {
-            "type": "string"
-        },
-        "ECSVolumeName": {
-            "type": "string"
-        },
         "EFSAuthorizationConfig": {
             "documentation": "<p>The authorization configuration details for the Amazon EFS file system.</p>",
             "members": {
                 "accessPointId": {
                     "documentation": "<p>The Amazon EFS access point ID to use. If an access point is specified, the root directory value specified in the <code>EFSVolumeConfiguration</code> must either be omitted or set to <code>/</code> which will enforce the path set on the EFS access point. If an access point is used, transit encryption must be on in the <code>EFSVolumeConfiguration</code>. For more information, see <a href=\"https://docs.aws.amazon.com/efs/latest/ug/efs-access-points.html\">Working with Amazon EFS access points</a> in the <i>Amazon Elastic File System User Guide</i>.</p>",
                     "shape": "String"
                 },
@@ -3872,18 +3799,18 @@
             },
             "required": [
                 "fileSystemId"
             ],
             "type": "structure"
         },
         "EnvironmentFile": {
-            "documentation": "<p>A list of files containing the environment variables to pass to a container. You can specify up to ten environment files. The file must have a <code>.env</code> file extension. Each line in an environment file should contain an environment variable in <code>VARIABLE=VALUE</code> format. Lines beginning with <code>#</code> are treated as comments and are ignored.</p> <p>If there are environment variables specified using the <code>environment</code> parameter in a container definition, they take precedence over the variables contained within an environment file. If multiple environment files are specified that contain the same variable, they're processed from the top down. We recommend that you use unique variable names. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/use-environment-file.html\">Use a file to pass environment variables to a container</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Environment variable files are objects in Amazon S3 and all Amazon S3 security considerations apply. </p> <p>You must use the following platforms for the Fargate launch type:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> <p>Consider the following when using the Fargate launch type:</p> <ul> <li> <p>The file is handled like a native Docker env-file.</p> </li> <li> <p>There is no support for shell escape handling.</p> </li> <li> <p>The container entry point interperts the <code>VARIABLE</code> values.</p> </li> </ul>",
+            "documentation": "<p>A list of files containing the environment variables to pass to a container. You can specify up to ten environment files. The file must have a <code>.env</code> file extension. Each line in an environment file should contain an environment variable in <code>VARIABLE=VALUE</code> format. Lines beginning with <code>#</code> are treated as comments and are ignored.</p> <p>If there are environment variables specified using the <code>environment</code> parameter in a container definition, they take precedence over the variables contained within an environment file. If multiple environment files are specified that contain the same variable, they're processed from the top down. We recommend that you use unique variable names. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/taskdef-envfiles.html\">Specifying environment variables</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>You must use the following platforms for the Fargate launch type:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> <p>Consider the following when using the Fargate launch type:</p> <ul> <li> <p>The file is handled like a native Docker env-file.</p> </li> <li> <p>There is no support for shell escape handling.</p> </li> <li> <p>The container entry point interperts the <code>VARIABLE</code> values.</p> </li> </ul>",
             "members": {
                 "type": {
-                    "documentation": "<p>The file type to use. Environment files are objects in Amazon S3. The only supported value is <code>s3</code>.</p>",
+                    "documentation": "<p>The file type to use. The only supported value is <code>s3</code>.</p>",
                     "shape": "EnvironmentFileType"
                 },
                 "value": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon S3 object containing the environment variable file.</p>",
                     "shape": "String"
                 }
             },
@@ -3908,18 +3835,18 @@
         "EnvironmentVariables": {
             "member": {
                 "shape": "KeyValuePair"
             },
             "type": "list"
         },
         "EphemeralStorage": {
-            "documentation": "<p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using_data_volumes.html\">Using data volumes in tasks</a> in the <i>Amazon ECS Developer Guide;</i>.</p> <note> <p>For tasks using the Fargate launch type, the task requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> </note>",
+            "documentation": "<p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/using_data_volumes.html\">Fargate task storage</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> <note> <p>For tasks using the Fargate launch type, the task requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> </note>",
             "members": {
                 "sizeInGiB": {
-                    "documentation": "<p>The total amount, in GiB, of ephemeral storage to set for the task. The minimum supported value is <code>20</code> GiB and the maximum supported value is <code>200</code> GiB.</p>",
+                    "documentation": "<p>The total amount, in GiB, of ephemeral storage to set for the task. The minimum supported value is <code>21</code> GiB and the maximum supported value is <code>200</code> GiB.</p>",
                     "shape": "Integer"
                 }
             },
             "required": [
                 "sizeInGiB"
             ],
             "type": "structure"
@@ -4165,15 +4092,15 @@
         "GpuIds": {
             "member": {
                 "shape": "String"
             },
             "type": "list"
         },
         "HealthCheck": {
-            "documentation": "<p>An object representing a container health check. Health check parameters that are specified in a container definition override any Docker health checks that exist in the container image (such as those specified in a parent image or from the image's Dockerfile). This configuration maps to the <code>HEALTHCHECK</code> parameter of <a href=\"https://docs.docker.com/engine/reference/run/\">docker run</a>.</p> <note> <p>The Amazon ECS container agent only monitors and reports on the health checks specified in the task definition. Amazon ECS does not monitor Docker health checks that are embedded in a container image and not specified in the container definition. Health check parameters that are specified in a container definition override any Docker health checks that exist in the container image.</p> </note> <p>You can view the health status of both individual containers and a task with the DescribeTasks API operation or when viewing the task details in the console.</p> <p>The health check is designed to make sure that your containers survive agent restarts, upgrades, or temporary unavailability.</p> <p>Amazon ECS performs health checks on containers with the default that launched the container instance or the task.</p> <p>The following describes the possible <code>healthStatus</code> values for a container:</p> <ul> <li> <p> <code>HEALTHY</code>-The container health check has passed successfully.</p> </li> <li> <p> <code>UNHEALTHY</code>-The container health check has failed.</p> </li> <li> <p> <code>UNKNOWN</code>-The container health check is being evaluated, there's no container health check defined, or Amazon ECS doesn't have the health status of the container.</p> </li> </ul> <p>The following describes the possible <code>healthStatus</code> values based on the container health checker status of essential containers in the task with the following priority order (high to low):</p> <ul> <li> <p> <code>UNHEALTHY</code>-One or more essential containers have failed their health check.</p> </li> <li> <p> <code>UNKNOWN</code>-Any essential container running within the task is in an <code>UNKNOWN</code> state and no other essential containers have an <code>UNHEALTHY</code> state.</p> </li> <li> <p> <code>HEALTHY</code>-All essential containers within the task have passed their health checks.</p> </li> </ul> <p>Consider the following task health example with 2 containers.</p> <ul> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>UNKNOWN</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>HEALTHY</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>UNKNOWN</code>, the task health is <code>UNKNOWN</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>HEALTHY</code>, the task health is <code>HEALTHY</code>.</p> </li> </ul> <p>Consider the following task health example with 3 containers.</p> <ul> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>UNKNOWN</code>, and Container3 is <code>UNKNOWN</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>UNKNOWN</code>, and Container3 is <code>HEALTHY</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>HEALTHY</code>, and Container3 is <code>HEALTHY</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>UNKNOWN</code>, and Container3 is <code>HEALTHY</code>, the task health is <code>UNKNOWN</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>UNKNOWN</code>, and Container3 is <code>UNKNOWN</code>, the task health is <code>UNKNOWN</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>HEALTHY</code>, and Container3 is <code>HEALTHY</code>, the task health is <code>HEALTHY</code>.</p> </li> </ul> <p>If a task is run manually, and not as part of a service, the task will continue its lifecycle regardless of its health status. For tasks that are part of a service, if the task reports as unhealthy then the task will be stopped and the service scheduler will replace it.</p> <p>The following are notes about container health check support:</p> <ul> <li> <p>When the Amazon ECS agent cannot connect to the Amazon ECS service, the service reports the container as <code>UNHEALTHY</code>. </p> </li> <li> <p>The health check statuses are the \"last heard from\" response from the Amazon ECS agent. There are no assumptions made about the status of the container health checks.</p> </li> <li> <p>Container health checks require version 1.17.0 or greater of the Amazon ECS container agent. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-update.html\">Updating the Amazon ECS container agent</a>.</p> </li> <li> <p>Container health checks are supported for Fargate tasks if you're using platform version <code>1.1.0</code> or greater. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html\">Fargate platform versions</a>.</p> </li> <li> <p>Container health checks aren't supported for tasks that are part of a service that's configured to use a Classic Load Balancer.</p> </li> </ul>",
+            "documentation": "<p>An object representing a container health check. Health check parameters that are specified in a container definition override any Docker health checks that exist in the container image (such as those specified in a parent image or from the image's Dockerfile). This configuration maps to the <code>HEALTHCHECK</code> parameter of <a href=\"https://docs.docker.com/engine/reference/run/\">docker run</a>.</p> <note> <p>The Amazon ECS container agent only monitors and reports on the health checks specified in the task definition. Amazon ECS does not monitor Docker health checks that are embedded in a container image and not specified in the container definition. Health check parameters that are specified in a container definition override any Docker health checks that exist in the container image.</p> </note> <p>You can view the health status of both individual containers and a task with the DescribeTasks API operation or when viewing the task details in the console.</p> <p>The health check is designed to make sure that your containers survive agent restarts, upgrades, or temporary unavailability.</p> <p>The following describes the possible <code>healthStatus</code> values for a container:</p> <ul> <li> <p> <code>HEALTHY</code>-The container health check has passed successfully.</p> </li> <li> <p> <code>UNHEALTHY</code>-The container health check has failed.</p> </li> <li> <p> <code>UNKNOWN</code>-The container health check is being evaluated, there's no container health check defined, or Amazon ECS doesn't have the health status of the container.</p> </li> </ul> <p>The following describes the possible <code>healthStatus</code> values based on the container health checker status of essential containers in the task with the following priority order (high to low):</p> <ul> <li> <p> <code>UNHEALTHY</code>-One or more essential containers have failed their health check.</p> </li> <li> <p> <code>UNKNOWN</code>-Any essential container running within the task is in an <code>UNKNOWN</code> state and no other essential containers have an <code>UNHEALTHY</code> state.</p> </li> <li> <p> <code>HEALTHY</code>-All essential containers within the task have passed their health checks.</p> </li> </ul> <p>Consider the following task health example with 2 containers.</p> <ul> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>UNKNOWN</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>HEALTHY</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>UNKNOWN</code>, the task health is <code>UNKNOWN</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>HEALTHY</code>, the task health is <code>HEALTHY</code>.</p> </li> </ul> <p>Consider the following task health example with 3 containers.</p> <ul> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>UNKNOWN</code>, and Container3 is <code>UNKNOWN</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>UNKNOWN</code>, and Container3 is <code>HEALTHY</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>UNHEALTHY</code> and Container2 is <code>HEALTHY</code>, and Container3 is <code>HEALTHY</code>, the task health is <code>UNHEALTHY</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>UNKNOWN</code>, and Container3 is <code>HEALTHY</code>, the task health is <code>UNKNOWN</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>UNKNOWN</code>, and Container3 is <code>UNKNOWN</code>, the task health is <code>UNKNOWN</code>.</p> </li> <li> <p>If Container1 is <code>HEALTHY</code> and Container2 is <code>HEALTHY</code>, and Container3 is <code>HEALTHY</code>, the task health is <code>HEALTHY</code>.</p> </li> </ul> <p>If a task is run manually, and not as part of a service, the task will continue its lifecycle regardless of its health status. For tasks that are part of a service, if the task reports as unhealthy then the task will be stopped and the service scheduler will replace it.</p> <p>The following are notes about container health check support:</p> <ul> <li> <p>When the Amazon ECS agent cannot connect to the Amazon ECS service, the service reports the container as <code>UNHEALTHY</code>. </p> </li> <li> <p>The health check statuses are the \"last heard from\" response from the Amazon ECS agent. There are no assumptions made about the status of the container health checks.</p> </li> <li> <p>Container health checks require version 1.17.0 or greater of the Amazon ECS container agent. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-update.html\">Updating the Amazon ECS container agent</a>.</p> </li> <li> <p>Container health checks are supported for Fargate tasks if you're using platform version <code>1.1.0</code> or greater. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html\">Fargate platform versions</a>.</p> </li> <li> <p>Container health checks aren't supported for tasks that are part of a service that's configured to use a Classic Load Balancer.</p> </li> </ul>",
             "members": {
                 "command": {
                     "documentation": "<p>A string array representing the command that the container runs to determine if it is healthy. The string array must start with <code>CMD</code> to run the command arguments directly, or <code>CMD-SHELL</code> to run the command with the container's default shell. </p> <p> When you use the Amazon Web Services Management Console JSON panel, the Command Line Interface, or the APIs, enclose the list of commands in double quotes and brackets.</p> <p> <code>[ \"CMD-SHELL\", \"curl -f http://localhost/ || exit 1\" ]</code> </p> <p>You don't include the double quotes and brackets when you use the Amazon Web Services Management Console.</p> <p> <code> CMD-SHELL, curl -f http://localhost/ || exit 1</code> </p> <p>An exit code of 0 indicates success, and non-zero exit code indicates failure. For more information, see <code>HealthCheck</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a>.</p>",
                     "shape": "StringList"
                 },
                 "interval": {
                     "documentation": "<p>The time period in seconds between each health check execution. You may specify between 5 and 300 seconds. The default value is 30 seconds.</p>",
@@ -4235,17 +4162,14 @@
                 "sourcePath": {
                     "documentation": "<p>When the <code>host</code> parameter is used, specify a <code>sourcePath</code> to declare the path on the host container instance that's presented to the container. If this parameter is empty, then the Docker daemon has assigned a host path for you. If the <code>host</code> parameter contains a <code>sourcePath</code> file location, then the data volume persists at the specified location on the host container instance until you delete it manually. If the <code>sourcePath</code> value doesn't exist on the host container instance, the Docker daemon creates it. If the location does exist, the contents of the source path folder are exported.</p> <p>If you're using the Fargate launch type, the <code>sourcePath</code> parameter is not supported.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
-        "IAMRoleArn": {
-            "type": "string"
-        },
         "InferenceAccelerator": {
             "documentation": "<p>Details on an Elastic Inference accelerator. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-inference.html\">Working with Amazon Elastic Inference on Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "members": {
                 "deviceName": {
                     "documentation": "<p>The Elastic Inference accelerator device name. The <code>deviceName</code> must also be referenced in a container definition as a <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_ResourceRequirement.html\">ResourceRequirement</a>.</p>",
                     "shape": "String"
                 },
@@ -4343,15 +4267,15 @@
                 "host",
                 "task",
                 "none"
             ],
             "type": "string"
         },
         "KernelCapabilities": {
-            "documentation": "<p>The Linux capabilities to add or remove from the default Docker configuration for a container defined in the task definition. For more information about the default capabilities and the non-default available capabilities, see <a href=\"https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities\">Runtime privilege and Linux capabilities</a> in the <i>Docker run reference</i>. For more detailed information about these Linux capabilities, see the <a href=\"http://man7.org/linux/man-pages/man7/capabilities.7.html\">capabilities(7)</a> Linux manual page.</p>",
+            "documentation": "<p>The Linux capabilities for the container that are added to or dropped from the default configuration provided by Docker. For more information about the default capabilities and the non-default available capabilities, see <a href=\"https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities\">Runtime privilege and Linux capabilities</a> in the <i>Docker run reference</i>. For more detailed information about these Linux capabilities, see the <a href=\"http://man7.org/linux/man-pages/man7/capabilities.7.html\">capabilities(7)</a> Linux manual page.</p>",
             "members": {
                 "add": {
                     "documentation": "<p>The Linux capabilities for the container that have been added to the default configuration provided by Docker. This parameter maps to <code>CapAdd</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--cap-add</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <note> <p>Tasks launched on Fargate only support adding the <code>SYS_PTRACE</code> kernel capability.</p> </note> <p>Valid values: <code>\"ALL\" | \"AUDIT_CONTROL\" | \"AUDIT_WRITE\" | \"BLOCK_SUSPEND\" | \"CHOWN\" | \"DAC_OVERRIDE\" | \"DAC_READ_SEARCH\" | \"FOWNER\" | \"FSETID\" | \"IPC_LOCK\" | \"IPC_OWNER\" | \"KILL\" | \"LEASE\" | \"LINUX_IMMUTABLE\" | \"MAC_ADMIN\" | \"MAC_OVERRIDE\" | \"MKNOD\" | \"NET_ADMIN\" | \"NET_BIND_SERVICE\" | \"NET_BROADCAST\" | \"NET_RAW\" | \"SETFCAP\" | \"SETGID\" | \"SETPCAP\" | \"SETUID\" | \"SYS_ADMIN\" | \"SYS_BOOT\" | \"SYS_CHROOT\" | \"SYS_MODULE\" | \"SYS_NICE\" | \"SYS_PACCT\" | \"SYS_PTRACE\" | \"SYS_RAWIO\" | \"SYS_RESOURCE\" | \"SYS_TIME\" | \"SYS_TTY_CONFIG\" | \"SYSLOG\" | \"WAKE_ALARM\"</code> </p>",
                     "shape": "StringList"
                 },
                 "drop": {
                     "documentation": "<p>The Linux capabilities for the container that have been removed from the default configuration provided by Docker. This parameter maps to <code>CapDrop</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--cap-drop</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <p>Valid values: <code>\"ALL\" | \"AUDIT_CONTROL\" | \"AUDIT_WRITE\" | \"BLOCK_SUSPEND\" | \"CHOWN\" | \"DAC_OVERRIDE\" | \"DAC_READ_SEARCH\" | \"FOWNER\" | \"FSETID\" | \"IPC_LOCK\" | \"IPC_OWNER\" | \"KILL\" | \"LEASE\" | \"LINUX_IMMUTABLE\" | \"MAC_ADMIN\" | \"MAC_OVERRIDE\" | \"MKNOD\" | \"NET_ADMIN\" | \"NET_BIND_SERVICE\" | \"NET_BROADCAST\" | \"NET_RAW\" | \"SETFCAP\" | \"SETGID\" | \"SETPCAP\" | \"SETUID\" | \"SYS_ADMIN\" | \"SYS_BOOT\" | \"SYS_CHROOT\" | \"SYS_MODULE\" | \"SYS_NICE\" | \"SYS_PACCT\" | \"SYS_PTRACE\" | \"SYS_RAWIO\" | \"SYS_RESOURCE\" | \"SYS_TIME\" | \"SYS_TTY_CONFIG\" | \"SYSLOG\" | \"WAKE_ALARM\"</code> </p>",
@@ -4791,15 +4715,15 @@
             },
             "type": "structure"
         },
         "LoadBalancer": {
             "documentation": "<p>The load balancer configuration to use with a service or task set.</p> <p>When you add, update, or remove a load balancer configuration, Amazon ECS starts a new deployment with the updated Elastic Load Balancing configuration. This causes tasks to register to and deregister from load balancers.</p> <p>We recommend that you verify this on a test environment before you update the Elastic Load Balancing configuration. </p> <p>A service-linked role is required for services that use multiple target groups. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using-service-linked-roles.html\">Using service-linked roles</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "members": {
                 "containerName": {
-                    "documentation": "<p>The name of the container (as it appears in a container definition) to associate with the load balancer.</p> <p>You need to specify the container name when configuring the target group for an Amazon ECS load balancer.</p>",
+                    "documentation": "<p>The name of the container (as it appears in a container definition) to associate with the load balancer.</p>",
                     "shape": "String"
                 },
                 "containerPort": {
                     "documentation": "<p>The port on the container to associate with the load balancer. This port must correspond to a <code>containerPort</code> in the task definition the tasks in the service are using. For tasks that use the EC2 launch type, the container instance they're launched on must allow ingress traffic on the <code>hostPort</code> of the port mapping.</p>",
                     "shape": "BoxedInteger"
                 },
                 "loadBalancerName": {
@@ -4928,21 +4852,14 @@
         },
         "ManagedAgents": {
             "member": {
                 "shape": "ManagedAgent"
             },
             "type": "list"
         },
-        "ManagedDraining": {
-            "enum": [
-                "ENABLED",
-                "DISABLED"
-            ],
-            "type": "string"
-        },
         "ManagedScaling": {
             "documentation": "<p>The managed scaling settings for the Auto Scaling group capacity provider.</p> <p>When managed scaling is turned on, Amazon ECS manages the scale-in and scale-out actions of the Auto Scaling group. Amazon ECS manages a target tracking scaling policy using an Amazon ECS managed CloudWatch metric with the specified <code>targetCapacity</code> value as the target value for the metric. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/asg-capacity-providers.html#asg-capacity-providers-managed-scaling\">Using managed scaling</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>If managed scaling is off, the user must manage the scaling of the Auto Scaling group.</p>",
             "members": {
                 "instanceWarmupPeriod": {
                     "documentation": "<p>The period of time, in seconds, after a newly launched Amazon EC2 instance can contribute to CloudWatch metrics for Auto Scaling group. If this parameter is omitted, the default value of <code>300</code> seconds is used.</p>",
                     "shape": "ManagedScalingInstanceWarmupPeriod"
                 },
@@ -5338,15 +5255,15 @@
                 "APPMESH"
             ],
             "type": "string"
         },
         "PutAccountSettingDefaultRequest": {
             "members": {
                 "name": {
-                    "documentation": "<p>The resource name for which to modify the account setting.</p> <p>The following are the valid values for the account setting name.</p> <ul> <li> <p> <code>serviceLongArnFormat</code> - When modified, the Amazon Resource Name (ARN) and resource ID format of the resource type for a specified user, role, or the root user for an account is affected. The opt-in and opt-out account setting must be set for each Amazon ECS resource separately. The ARN and resource ID format of a resource is defined by the opt-in status of the user or role that created the resource. You must turn on this setting to use Amazon ECS features such as resource tagging.</p> </li> <li> <p> <code>taskLongArnFormat</code> - When modified, the Amazon Resource Name (ARN) and resource ID format of the resource type for a specified user, role, or the root user for an account is affected. The opt-in and opt-out account setting must be set for each Amazon ECS resource separately. The ARN and resource ID format of a resource is defined by the opt-in status of the user or role that created the resource. You must turn on this setting to use Amazon ECS features such as resource tagging.</p> </li> <li> <p> <code>containerInstanceLongArnFormat</code> - When modified, the Amazon Resource Name (ARN) and resource ID format of the resource type for a specified user, role, or the root user for an account is affected. The opt-in and opt-out account setting must be set for each Amazon ECS resource separately. The ARN and resource ID format of a resource is defined by the opt-in status of the user or role that created the resource. You must turn on this setting to use Amazon ECS features such as resource tagging.</p> </li> <li> <p> <code>awsvpcTrunking</code> - When modified, the elastic network interface (ENI) limit for any new container instances that support the feature is changed. If <code>awsvpcTrunking</code> is turned on, any new container instances that support the feature are launched have the increased ENI limits available to them. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/container-instance-eni.html\">Elastic Network Interface Trunking</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> <li> <p> <code>containerInsights</code> - When modified, the default setting indicating whether Amazon Web Services CloudWatch Container Insights is turned on for your clusters is changed. If <code>containerInsights</code> is turned on, any new clusters that are created will have Container Insights turned on unless you disable it during cluster creation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/cloudwatch-container-insights.html\">CloudWatch Container Insights</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> <li> <p> <code>dualStackIPv6</code> - When turned on, when using a VPC in dual stack mode, your tasks using the <code>awsvpc</code> network mode can have an IPv6 address assigned. For more information on using IPv6 with tasks launched on Amazon EC2 instances, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-networking-awsvpc.html#task-networking-vpc-dual-stack\">Using a VPC in dual-stack mode</a>. For more information on using IPv6 with tasks launched on Fargate, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/fargate-task-networking.html#fargate-task-networking-vpc-dual-stack\">Using a VPC in dual-stack mode</a>.</p> </li> <li> <p> <code>fargateFIPSMode</code> - If you specify <code>fargateFIPSMode</code>, Fargate FIPS 140 compliance is affected.</p> </li> <li> <p> <code>fargateTaskRetirementWaitPeriod</code> - When Amazon Web Services determines that a security or infrastructure update is needed for an Amazon ECS task hosted on Fargate, the tasks need to be stopped and new tasks launched to replace them. Use <code>fargateTaskRetirementWaitPeriod</code> to configure the wait time to retire a Fargate task. For information about the Fargate tasks maintenance, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-maintenance.html\">Amazon Web Services Fargate task maintenance</a> in the <i>Amazon ECS Developer Guide</i>.</p> </li> <li> <p> <code>tagResourceAuthorization</code> - Amazon ECS is introducing tagging authorization for resource creation. Users must have permissions for actions that create the resource, such as <code>ecsCreateCluster</code>. If tags are specified when you create a resource, Amazon Web Services performs additional authorization to verify if users or roles have permissions to create tags. Therefore, you must grant explicit permissions to use the <code>ecs:TagResource</code> action. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/supported-iam-actions-tagging.html\">Grant permission to tag resources on creation</a> in the <i>Amazon ECS Developer Guide</i>.</p> </li> <li> <p> <code>guardDutyActivate</code> - The <code>guardDutyActivate</code> parameter is read-only in Amazon ECS and indicates whether Amazon ECS Runtime Monitoring is enabled or disabled by your security administrator in your Amazon ECS account. Amazon GuardDuty controls this account setting on your behalf. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-guard-duty-integration.html\">Protecting Amazon ECS workloads with Amazon ECS Runtime Monitoring</a>.</p> </li> </ul>",
+                    "documentation": "<p>The resource name for which to modify the account setting. If you specify <code>serviceLongArnFormat</code>, the ARN for your Amazon ECS services is affected. If you specify <code>taskLongArnFormat</code>, the ARN and resource ID for your Amazon ECS tasks is affected. If you specify <code>containerInstanceLongArnFormat</code>, the ARN and resource ID for your Amazon ECS container instances is affected. If you specify <code>awsvpcTrunking</code>, the ENI limit for your Amazon ECS container instances is affected. If you specify <code>containerInsights</code>, the default setting for Amazon Web Services CloudWatch Container Insights for your clusters is affected. If you specify <code>tagResourceAuthorization</code>, the opt-in option for tagging resources on creation is affected. For information about the opt-in timeline, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-account-settings.html#tag-resources\">Tagging authorization timeline</a> in the <i>Amazon ECS Developer Guide</i>. If you specify <code>fargateTaskRetirementWaitPeriod</code>, the default wait time to retire a Fargate task due to required maintenance is affected.</p> <p>When you specify <code>fargateFIPSMode</code> for the <code>name</code> and <code>enabled</code> for the <code>value</code>, Fargate uses FIPS-140 compliant cryptographic algorithms on your tasks. For more information about FIPS-140 compliance with Fargate, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-fips-compliance.html\"> Amazon Web Services Fargate Federal Information Processing Standard (FIPS) 140-2 compliance</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When Amazon Web Services determines that a security or infrastructure update is needed for an Amazon ECS task hosted on Fargate, the tasks need to be stopped and new tasks launched to replace them. Use <code>fargateTaskRetirementWaitPeriod</code> to set the wait time to retire a Fargate task to the default. For information about the Fargate tasks maintenance, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-maintenance.html\">Amazon Web Services Fargate task maintenance</a> in the <i>Amazon ECS Developer Guide</i>.</p> <p>The <code>guardDutyActivate</code> parameter is read-only in Amazon ECS and indicates whether Amazon ECS Runtime Monitoring is enabled or disabled by your security administrator in your Amazon ECS account. Amazon GuardDuty controls this account setting on your behalf. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-guard-duty-integration.html\">Protecting Amazon ECS workloads with Amazon ECS Runtime Monitoring</a>.</p>",
                     "shape": "SettingName"
                 },
                 "value": {
                     "documentation": "<p>The account setting value for the specified principal ARN. Accepted values are <code>enabled</code>, <code>disabled</code>, <code>on</code>, and <code>off</code>.</p> <p>When you specify <code>fargateTaskRetirementWaitPeriod</code> for the <code>name</code>, the following are the valid values:</p> <ul> <li> <p> <code>0</code> - Amazon Web Services sends the notification, and immediately retires the affected tasks.</p> </li> <li> <p> <code>7</code> - Amazon Web Services sends the notification, and waits 7 calendar days to retire the tasks.</p> </li> <li> <p> <code>14</code> - Amazon Web Services sends the notification, and waits 14 calendar days to retire the tasks.</p> </li> </ul>",
                     "shape": "String"
                 }
             },
@@ -5364,15 +5281,15 @@
                 }
             },
             "type": "structure"
         },
         "PutAccountSettingRequest": {
             "members": {
                 "name": {
-                    "documentation": "<p>The Amazon ECS account setting name to modify.</p> <p>The following are the valid values for the account setting name.</p> <ul> <li> <p> <code>serviceLongArnFormat</code> - When modified, the Amazon Resource Name (ARN) and resource ID format of the resource type for a specified user, role, or the root user for an account is affected. The opt-in and opt-out account setting must be set for each Amazon ECS resource separately. The ARN and resource ID format of a resource is defined by the opt-in status of the user or role that created the resource. You must turn on this setting to use Amazon ECS features such as resource tagging.</p> </li> <li> <p> <code>taskLongArnFormat</code> - When modified, the Amazon Resource Name (ARN) and resource ID format of the resource type for a specified user, role, or the root user for an account is affected. The opt-in and opt-out account setting must be set for each Amazon ECS resource separately. The ARN and resource ID format of a resource is defined by the opt-in status of the user or role that created the resource. You must turn on this setting to use Amazon ECS features such as resource tagging.</p> </li> <li> <p> <code>containerInstanceLongArnFormat</code> - When modified, the Amazon Resource Name (ARN) and resource ID format of the resource type for a specified user, role, or the root user for an account is affected. The opt-in and opt-out account setting must be set for each Amazon ECS resource separately. The ARN and resource ID format of a resource is defined by the opt-in status of the user or role that created the resource. You must turn on this setting to use Amazon ECS features such as resource tagging.</p> </li> <li> <p> <code>awsvpcTrunking</code> - When modified, the elastic network interface (ENI) limit for any new container instances that support the feature is changed. If <code>awsvpcTrunking</code> is turned on, any new container instances that support the feature are launched have the increased ENI limits available to them. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/container-instance-eni.html\">Elastic Network Interface Trunking</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> <li> <p> <code>containerInsights</code> - When modified, the default setting indicating whether Amazon Web Services CloudWatch Container Insights is turned on for your clusters is changed. If <code>containerInsights</code> is turned on, any new clusters that are created will have Container Insights turned on unless you disable it during cluster creation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/cloudwatch-container-insights.html\">CloudWatch Container Insights</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> <li> <p> <code>dualStackIPv6</code> - When turned on, when using a VPC in dual stack mode, your tasks using the <code>awsvpc</code> network mode can have an IPv6 address assigned. For more information on using IPv6 with tasks launched on Amazon EC2 instances, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-networking-awsvpc.html#task-networking-vpc-dual-stack\">Using a VPC in dual-stack mode</a>. For more information on using IPv6 with tasks launched on Fargate, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/fargate-task-networking.html#fargate-task-networking-vpc-dual-stack\">Using a VPC in dual-stack mode</a>.</p> </li> <li> <p> <code>fargateFIPSMode</code> - If you specify <code>fargateFIPSMode</code>, Fargate FIPS 140 compliance is affected.</p> </li> <li> <p> <code>fargateTaskRetirementWaitPeriod</code> - When Amazon Web Services determines that a security or infrastructure update is needed for an Amazon ECS task hosted on Fargate, the tasks need to be stopped and new tasks launched to replace them. Use <code>fargateTaskRetirementWaitPeriod</code> to configure the wait time to retire a Fargate task. For information about the Fargate tasks maintenance, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-maintenance.html\">Amazon Web Services Fargate task maintenance</a> in the <i>Amazon ECS Developer Guide</i>.</p> </li> <li> <p> <code>tagResourceAuthorization</code> - Amazon ECS is introducing tagging authorization for resource creation. Users must have permissions for actions that create the resource, such as <code>ecsCreateCluster</code>. If tags are specified when you create a resource, Amazon Web Services performs additional authorization to verify if users or roles have permissions to create tags. Therefore, you must grant explicit permissions to use the <code>ecs:TagResource</code> action. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/supported-iam-actions-tagging.html\">Grant permission to tag resources on creation</a> in the <i>Amazon ECS Developer Guide</i>.</p> </li> <li> <p> <code>guardDutyActivate</code> - The <code>guardDutyActivate</code> parameter is read-only in Amazon ECS and indicates whether Amazon ECS Runtime Monitoring is enabled or disabled by your security administrator in your Amazon ECS account. Amazon GuardDuty controls this account setting on your behalf. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-guard-duty-integration.html\">Protecting Amazon ECS workloads with Amazon ECS Runtime Monitoring</a>.</p> </li> </ul>",
+                    "documentation": "<p>The Amazon ECS resource name for which to modify the account setting. If you specify <code>serviceLongArnFormat</code>, the ARN for your Amazon ECS services is affected. If you specify <code>taskLongArnFormat</code>, the ARN and resource ID for your Amazon ECS tasks is affected. If you specify <code>containerInstanceLongArnFormat</code>, the ARN and resource ID for your Amazon ECS container instances is affected. If you specify <code>awsvpcTrunking</code>, the elastic network interface (ENI) limit for your Amazon ECS container instances is affected. If you specify <code>containerInsights</code>, the default setting for Amazon Web Services CloudWatch Container Insights for your clusters is affected. If you specify <code>fargateFIPSMode</code>, Fargate FIPS 140 compliance is affected. If you specify <code>tagResourceAuthorization</code>, the opt-in option for tagging resources on creation is affected. For information about the opt-in timeline, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-account-settings.html#tag-resources\">Tagging authorization timeline</a> in the <i>Amazon ECS Developer Guide</i>. If you specify <code>fargateTaskRetirementWaitPeriod</code>, the wait time to retire a Fargate task is affected.</p> <p>The <code>guardDutyActivate</code> parameter is read-only in Amazon ECS and indicates whether Amazon ECS Runtime Monitoring is enabled or disabled by your security administrator in your Amazon ECS account. Amazon GuardDuty controls this account setting on your behalf. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-guard-duty-integration.html\">Protecting Amazon ECS workloads with Amazon ECS Runtime Monitoring</a>.</p>",
                     "shape": "SettingName"
                 },
                 "principalArn": {
                     "documentation": "<p>The ARN of the principal, which can be a user, role, or the root user. If you specify the root user, it modifies the account setting for all users, roles, and the root user of the account unless a user or role explicitly overrides these settings. If this field is omitted, the setting is changed only for the authenticated user.</p> <note> <p>You must use the root user when you set the Fargate wait time (<code>fargateTaskRetirementWaitPeriod</code>). </p> <p>Federated users assume the account setting of the root user and can't have explicit account settings set for them.</p> </note>",
                     "shape": "String"
                 },
                 "value": {
@@ -5508,15 +5425,15 @@
                     "shape": "ContainerDefinitions"
                 },
                 "cpu": {
                     "documentation": "<p>The number of CPU units used by the task. It can be expressed as an integer using CPU units (for example, <code>1024</code>) or as a string using vCPUs (for example, <code>1 vCPU</code> or <code>1 vcpu</code>) in a task definition. String values are converted to an integer indicating the CPU units when the task definition is registered.</p> <note> <p>Task-level CPU and memory parameters are ignored for Windows containers. We recommend specifying container-level resources for Windows containers.</p> </note> <p>If you're using the EC2 launch type, this field is optional. Supported values are between <code>128</code> CPU units (<code>0.125</code> vCPUs) and <code>10240</code> CPU units (<code>10</code> vCPUs). If you do not specify a value, the parameter is ignored.</p> <p>If you're using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of supported values for the <code>memory</code> parameter:</p> <p>The CPU units cannot be less than 1 vCPU when you use Windows containers on Fargate.</p> <ul> <li> <p>256 (.25 vCPU) - Available <code>memory</code> values: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB)</p> </li> <li> <p>512 (.5 vCPU) - Available <code>memory</code> values: 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB)</p> </li> <li> <p>1024 (1 vCPU) - Available <code>memory</code> values: 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB)</p> </li> <li> <p>2048 (2 vCPU) - Available <code>memory</code> values: 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB)</p> </li> <li> <p>4096 (4 vCPU) - Available <code>memory</code> values: 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB)</p> </li> <li> <p>8192 (8 vCPU) - Available <code>memory</code> values: 16 GB and 60 GB in 4 GB increments</p> <p>This option requires Linux platform <code>1.4.0</code> or later.</p> </li> <li> <p>16384 (16vCPU) - Available <code>memory</code> values: 32GB and 120 GB in 8 GB increments</p> <p>This option requires Linux platform <code>1.4.0</code> or later.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "ephemeralStorage": {
-                    "documentation": "<p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using_data_volumes.html\">Using data volumes in tasks</a> in the <i>Amazon ECS Developer Guide</i>.</p> <note> <p>For tasks using the Fargate launch type, the task requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> </note>",
+                    "documentation": "<p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/using_data_volumes.html\">Fargate task storage</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> <note> <p>For tasks using the Fargate launch type, the task requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> </note>",
                     "shape": "EphemeralStorage"
                 },
                 "executionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the task execution role that grants the Amazon ECS container agent permission to make Amazon Web Services API calls on your behalf. The task execution IAM role is required depending on the requirements of your task. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_execution_IAM_role.html\">Amazon ECS task execution IAM role</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "String"
                 },
                 "family": {
@@ -5723,15 +5640,15 @@
                     "shape": "Boolean"
                 },
                 "group": {
                     "documentation": "<p>The name of the task group to associate with the task. The default value is the family name of the task definition (for example, <code>family:my-family-name</code>).</p>",
                     "shape": "String"
                 },
                 "launchType": {
-                    "documentation": "<p>The infrastructure to run your standalone task on. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/launch_types.html\">Amazon ECS launch types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>The <code>FARGATE</code> launch type runs your tasks on Fargate On-Demand infrastructure.</p> <note> <p>Fargate Spot infrastructure is available for use but a capacity provider strategy must be used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/fargate-capacity-providers.html\">Fargate capacity providers</a> in the <i>Amazon ECS Developer Guide</i>.</p> </note> <p>The <code>EC2</code> launch type runs your tasks on Amazon EC2 instances registered to your cluster.</p> <p>The <code>EXTERNAL</code> launch type runs your tasks on your on-premises server or virtual machine (VM) capacity registered to your cluster.</p> <p>A task can use either a launch type or a capacity provider strategy. If a <code>launchType</code> is specified, the <code>capacityProviderStrategy</code> parameter must be omitted.</p> <p>When you use cluster auto scaling, you must specify <code>capacityProviderStrategy</code> and not <code>launchType</code>. </p>",
+                    "documentation": "<p>The infrastructure to run your standalone task on. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/launch_types.html\">Amazon ECS launch types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>The <code>FARGATE</code> launch type runs your tasks on Fargate On-Demand infrastructure.</p> <note> <p>Fargate Spot infrastructure is available for use but a capacity provider strategy must be used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/fargate-capacity-providers.html\">Fargate capacity providers</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> </note> <p>The <code>EC2</code> launch type runs your tasks on Amazon EC2 instances registered to your cluster.</p> <p>The <code>EXTERNAL</code> launch type runs your tasks on your on-premises server or virtual machine (VM) capacity registered to your cluster.</p> <p>A task can use either a launch type or a capacity provider strategy. If a <code>launchType</code> is specified, the <code>capacityProviderStrategy</code> parameter must be omitted.</p> <p>When you use cluster auto scaling, you must specify <code>capacityProviderStrategy</code> and not <code>launchType</code>. </p>",
                     "shape": "LaunchType"
                 },
                 "networkConfiguration": {
                     "documentation": "<p>The network configuration for the task. This parameter is required for task definitions that use the <code>awsvpc</code> network mode to receive their own elastic network interface, and it isn't supported for other network modes. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-networking.html\">Task networking</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "NetworkConfiguration"
                 },
                 "overrides": {
@@ -5763,31 +5680,27 @@
                     "shape": "String"
                 },
                 "tags": {
                     "documentation": "<p>The metadata that you apply to the task to help you categorize and organize them. Each tag consists of a key and an optional value, both of which you define.</p> <p>The following basic restrictions apply to tags:</p> <ul> <li> <p>Maximum number of tags per resource - 50</p> </li> <li> <p>For each resource, each tag key must be unique, and each tag key can have only one value.</p> </li> <li> <p>Maximum key length - 128 Unicode characters in UTF-8</p> </li> <li> <p>Maximum value length - 256 Unicode characters in UTF-8</p> </li> <li> <p>If your tagging schema is used across multiple services and resources, remember that other services may have restrictions on allowed characters. Generally allowed characters are: letters, numbers, and spaces representable in UTF-8, and the following characters: + - = . _ : / @.</p> </li> <li> <p>Tag keys and values are case-sensitive.</p> </li> <li> <p>Do not use <code>aws:</code>, <code>AWS:</code>, or any upper or lowercase combination of such as a prefix for either keys or values as it is reserved for Amazon Web Services use. You cannot edit or delete tag keys or values with this prefix. Tags with this prefix do not count against your tags per resource limit.</p> </li> </ul>",
                     "shape": "Tags"
                 },
                 "taskDefinition": {
-                    "documentation": "<p>The <code>family</code> and <code>revision</code> (<code>family:revision</code>) or full ARN of the task definition to run. If a <code>revision</code> isn't specified, the latest <code>ACTIVE</code> revision is used.</p> <p>The full ARN value must match the value that you specified as the <code>Resource</code> of the principal's permissions policy.</p> <p>When you specify a task definition, you must either specify a specific revision, or all revisions in the ARN.</p> <p>To specify a specific revision, include the revision number in the ARN. For example, to specify revision 2, use <code>arn:aws:ecs:us-east-1:111122223333:task-definition/TaskFamilyName:2</code>.</p> <p>To specify all revisions, use the wildcard (*) in the ARN. For example, to specify all revisions, use <code>arn:aws:ecs:us-east-1:111122223333:task-definition/TaskFamilyName:*</code>.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/security_iam_service-with-iam.html#security_iam_service-with-iam-id-based-policies-resources\">Policy Resources for Amazon ECS</a> in the Amazon Elastic Container Service Developer Guide.</p>",
+                    "documentation": "<p>The <code>family</code> and <code>revision</code> (<code>family:revision</code>) or full ARN of the task definition to run. If a <code>revision</code> isn't specified, the latest <code>ACTIVE</code> revision is used.</p> <p>When you create a policy for run-task, you can set the resource to be the latest task definition revision, or a specific revision.</p> <p>The full ARN value must match the value that you specified as the <code>Resource</code> of the principal's permissions policy.</p> <p>When you specify the policy resource as the latest task definition version (by setting the <code>Resource</code> in the policy to <code>arn:aws:ecs:us-east-1:111122223333:task-definition/TaskFamilyName</code>), then set this value to <code>arn:aws:ecs:us-east-1:111122223333:task-definition/TaskFamilyName</code>.</p> <p>When you specify the policy resource as a specific task definition version (by setting the <code>Resource</code> in the policy to <code>arn:aws:ecs:us-east-1:111122223333:task-definition/TaskFamilyName:1</code> or <code>arn:aws:ecs:us-east-1:111122223333:task-definition/TaskFamilyName:*</code>), then set this value to <code>arn:aws:ecs:us-east-1:111122223333:task-definition/TaskFamilyName:1</code>.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/security_iam_service-with-iam.html#security_iam_service-with-iam-id-based-policies-resources\">Policy Resources for Amazon ECS</a> in the Amazon Elastic Container Service developer Guide.</p>",
                     "shape": "String"
-                },
-                "volumeConfigurations": {
-                    "documentation": "<p>The details of the volume that was <code>configuredAtLaunch</code>. You can configure the size, volumeType, IOPS, throughput, snapshot and encryption in in <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_TaskManagedEBSVolumeConfiguration.html\">TaskManagedEBSVolumeConfiguration</a>. The <code>name</code> of the volume must match the <code>name</code> from the task definition.</p>",
-                    "shape": "TaskVolumeConfigurations"
                 }
             },
             "required": [
                 "taskDefinition"
             ],
             "type": "structure"
         },
         "RunTaskResponse": {
             "members": {
                 "failures": {
-                    "documentation": "<p>Any failures associated with the call.</p> <p>For information about how to address failures, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-event-messages.html#service-event-messages-list\">Service event messages</a> and <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/api_failures_messages.html\">API failure reasons</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+                    "documentation": "<p>Any failures associated with the call.</p>",
                     "shape": "Failures"
                 },
                 "tasks": {
                     "documentation": "<p>A full description of the tasks that were run. The tasks that were successfully placed on your cluster are described here.</p> <p/>",
                     "shape": "Tasks"
                 }
             },
@@ -5871,15 +5784,14 @@
         },
         "ServerException": {
             "documentation": "<p>These errors are usually caused by a server issue.</p>",
             "exception": true,
             "fault": true,
             "members": {
                 "message": {
-                    "documentation": "<p> Message that describes the cause of the exception.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "Service": {
             "documentation": "<p>Details on a service within a cluster.</p>",
@@ -6072,22 +5984,14 @@
                 "ingressPortOverride": {
                     "documentation": "<p>The port number for the Service Connect proxy to listen on.</p> <p>Use the value of this field to bypass the proxy for traffic on the port number specified in the named <code>portMapping</code> in the task definition of this application, and then use it in your VPC security groups to allow traffic into the proxy for this Amazon ECS service.</p> <p>In <code>awsvpc</code> mode and Fargate, the default value is the container port number. The container port number is in the <code>portMapping</code> in the task definition. In bridge mode, the default value is the ephemeral port of the Service Connect proxy.</p>",
                     "shape": "PortNumber"
                 },
                 "portName": {
                     "documentation": "<p>The <code>portName</code> must match the name of one of the <code>portMappings</code> from all the containers in the task definition of this Amazon ECS service.</p>",
                     "shape": "String"
-                },
-                "timeout": {
-                    "documentation": "<p>A reference to an object that represents the configured timeouts for Service Connect.</p>",
-                    "shape": "TimeoutConfiguration"
-                },
-                "tls": {
-                    "documentation": "<p>A reference to an object that represents a Transport Layer Security (TLS) configuration.</p>",
-                    "shape": "ServiceConnectTlsConfiguration"
                 }
             },
             "required": [
                 "portName"
             ],
             "type": "structure"
         },
@@ -6113,45 +6017,14 @@
         },
         "ServiceConnectServiceResourceList": {
             "member": {
                 "shape": "ServiceConnectServiceResource"
             },
             "type": "list"
         },
-        "ServiceConnectTlsCertificateAuthority": {
-            "documentation": "<p>An object that represents the Amazon Web Services Private Certificate Authority certificate.</p>",
-            "members": {
-                "awsPcaAuthorityArn": {
-                    "documentation": "<p>The ARN of the Amazon Web Services Private Certificate Authority certificate.</p>",
-                    "shape": "String"
-                }
-            },
-            "type": "structure"
-        },
-        "ServiceConnectTlsConfiguration": {
-            "documentation": "<p>An object that represents the configuration for Service Connect TLS.</p>",
-            "members": {
-                "issuerCertificateAuthority": {
-                    "documentation": "<p>The signer certificate authority.</p>",
-                    "shape": "ServiceConnectTlsCertificateAuthority"
-                },
-                "kmsKey": {
-                    "documentation": "<p>The Amazon Web Services Key Management Service key.</p>",
-                    "shape": "String"
-                },
-                "roleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that's associated with the Service Connect TLS.</p>",
-                    "shape": "String"
-                }
-            },
-            "required": [
-                "issuerCertificateAuthority"
-            ],
-            "type": "structure"
-        },
         "ServiceEvent": {
             "documentation": "<p>The details for an event that's associated with a service.</p>",
             "members": {
                 "createdAt": {
                     "documentation": "<p>The Unix timestamp for the time when the event was triggered.</p>",
                     "shape": "Timestamp"
                 },
@@ -6180,63 +6053,14 @@
         },
         "ServiceFieldList": {
             "member": {
                 "shape": "ServiceField"
             },
             "type": "list"
         },
-        "ServiceManagedEBSVolumeConfiguration": {
-            "documentation": "<p>The configuration for the Amazon EBS volume that Amazon ECS creates and manages on your behalf. These settings are used to create each Amazon EBS volume, with one volume created for each task in the service.</p> <p>Many of these parameters map 1:1 with the Amazon EBS <code>CreateVolume</code> API request parameters.</p>",
-            "members": {
-                "encrypted": {
-                    "documentation": "<p>Indicates whether the volume should be encrypted. If no value is specified, encryption is turned on by default. This parameter maps 1:1 with the <code>Encrypted</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p>",
-                    "shape": "BoxedBoolean"
-                },
-                "filesystemType": {
-                    "documentation": "<p>The Linux filesystem type for the volume. For volumes created from a snapshot, you must specify the same filesystem type that the volume was using when the snapshot was created. If there is a filesystem type mismatch, the task will fail to start.</p> <p>The available filesystem types are&#x2028; <code>ext3</code>, <code>ext4</code>, and <code>xfs</code>. If no value is specified, the <code>xfs</code> filesystem type is used by default.</p>",
-                    "shape": "TaskFilesystemType"
-                },
-                "iops": {
-                    "documentation": "<p>The number of I/O operations per second (IOPS). For <code>gp3</code>, <code>io1</code>, and <code>io2</code> volumes, this represents the number of IOPS that are provisioned for the volume. For <code>gp2</code> volumes, this represents the baseline performance of the volume and the rate at which the volume accumulates I/O credits for bursting.</p> <p>The following are the supported values for each volume type.</p> <ul> <li> <p> <code>gp3</code>: 3,000 - 16,000 IOPS</p> </li> <li> <p> <code>io1</code>: 100 - 64,000 IOPS</p> </li> <li> <p> <code>io2</code>: 100 - 256,000 IOPS</p> </li> </ul> <p>This parameter is required for <code>io1</code> and <code>io2</code> volume types. The default for <code>gp3</code> volumes is <code>3,000 IOPS</code>. This parameter is not supported for <code>st1</code>, <code>sc1</code>, or <code>standard</code> volume types.</p> <p>This parameter maps 1:1 with the <code>Iops</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p>",
-                    "shape": "BoxedInteger"
-                },
-                "kmsKeyId": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) identifier of the Amazon Web Services Key Management Service key to use for Amazon EBS encryption. When encryption is turned on and no Amazon Web Services Key Management Service key is specified, the default Amazon Web Services managed key for Amazon EBS volumes is used. This parameter maps 1:1 with the <code>KmsKeyId</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p> <important> <p>Amazon Web Services authenticates the Amazon Web Services Key Management Service key asynchronously. Therefore, if you specify an ID, alias, or ARN that is invalid, the action can appear to complete, but eventually fails.</p> </important>",
-                    "shape": "EBSKMSKeyId"
-                },
-                "roleArn": {
-                    "documentation": "<p>The ARN of the IAM role to associate with this volume. This is the Amazon ECS infrastructure IAM role that is used to manage your Amazon Web Services infrastructure. We recommend using the Amazon ECS-managed <code>AmazonECSInfrastructureRolePolicyForVolumes</code> IAM policy with this role. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/infrastructure_IAM_role.html\">Amazon ECS infrastructure IAM role</a> in the <i>Amazon ECS Developer Guide</i>.</p>",
-                    "shape": "IAMRoleArn"
-                },
-                "sizeInGiB": {
-                    "documentation": "<p>The size of the volume in GiB. You must specify either a volume size or a snapshot ID. If you specify a snapshot ID, the snapshot size is used for the volume size by default. You can optionally specify a volume size greater than or equal to the snapshot size. This parameter maps 1:1 with the <code>Size</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p> <p>The following are the supported volume size values for each volume type.</p> <ul> <li> <p> <code>gp2</code> and <code>gp3</code>: 1-16,384</p> </li> <li> <p> <code>io1</code> and <code>io2</code>: 4-16,384</p> </li> <li> <p> <code>st1</code> and <code>sc1</code>: 125-16,384</p> </li> <li> <p> <code>standard</code>: 1-1,024</p> </li> </ul>",
-                    "shape": "BoxedInteger"
-                },
-                "snapshotId": {
-                    "documentation": "<p>The snapshot that Amazon ECS uses to create the volume. You must specify either a snapshot ID or a volume size. This parameter maps 1:1 with the <code>SnapshotId</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p>",
-                    "shape": "EBSSnapshotId"
-                },
-                "tagSpecifications": {
-                    "documentation": "<p>The tags to apply to the volume. Amazon ECS applies service-managed tags by default. This parameter maps 1:1 with the <code>TagSpecifications.N</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p>",
-                    "shape": "EBSTagSpecifications"
-                },
-                "throughput": {
-                    "documentation": "<p>The throughput to provision for a volume, in MiB/s, with a maximum of 1,000 MiB/s. This parameter maps 1:1 with the <code>Throughput</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p> <important> <p>This parameter is only supported for the <code>gp3</code> volume type.</p> </important>",
-                    "shape": "BoxedInteger"
-                },
-                "volumeType": {
-                    "documentation": "<p>The volume type. This parameter maps 1:1 with the <code>VolumeType</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volume-types.html\">Amazon EBS volume types</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>The following are the supported volume types.</p> <ul> <li> <p>General Purpose SSD: <code>gp2</code>|<code>gp3</code> </p> </li> <li> <p>Provisioned IOPS SSD: <code>io1</code>|<code>io2</code> </p> </li> <li> <p>Throughput Optimized HDD: <code>st1</code> </p> </li> <li> <p>Cold HDD: <code>sc1</code> </p> </li> <li> <p>Magnetic: <code>standard</code> </p> <note> <p>The magnetic volume type is not supported on Fargate.</p> </note> </li> </ul>",
-                    "shape": "EBSVolumeType"
-                }
-            },
-            "required": [
-                "roleArn"
-            ],
-            "type": "structure"
-        },
         "ServiceNotActiveException": {
             "documentation": "<p>The specified service isn't active. You can't update a service that's inactive. If you have previously deleted a service, you can re-create it with <a>CreateService</a>.</p>",
             "exception": true,
             "members": {},
             "type": "structure"
         },
         "ServiceNotFoundException": {
@@ -6269,37 +6093,14 @@
                 "registryArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the service registry. The currently supported service registry is Cloud Map. For more information, see <a href=\"https://docs.aws.amazon.com/cloud-map/latest/api/API_CreateService.html\">CreateService</a>.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
-        "ServiceVolumeConfiguration": {
-            "documentation": "<p>The configuration for a volume specified in the task definition as a volume that is configured at launch time. Currently, the only supported volume type is an Amazon EBS volume.</p>",
-            "members": {
-                "managedEBSVolume": {
-                    "documentation": "<p>The configuration for the Amazon EBS volume that Amazon ECS creates and manages on your behalf. These settings are used to create each Amazon EBS volume, with one volume created for each task in the service. The Amazon EBS volumes are visible in your account in the Amazon EC2 console once they are created.</p>",
-                    "shape": "ServiceManagedEBSVolumeConfiguration"
-                },
-                "name": {
-                    "documentation": "<p>The name of the volume. This value must match the volume name from the <code>Volume</code> object in the task definition.</p>",
-                    "shape": "ECSVolumeName"
-                }
-            },
-            "required": [
-                "name"
-            ],
-            "type": "structure"
-        },
-        "ServiceVolumeConfigurations": {
-            "member": {
-                "shape": "ServiceVolumeConfiguration"
-            },
-            "type": "list"
-        },
         "Services": {
             "member": {
                 "shape": "Service"
             },
             "type": "list"
         },
         "Session": {
@@ -6428,18 +6229,14 @@
                 "tags": {
                     "documentation": "<p>The metadata that you apply to the task to help you categorize and organize them. Each tag consists of a key and an optional value, both of which you define.</p> <p>The following basic restrictions apply to tags:</p> <ul> <li> <p>Maximum number of tags per resource - 50</p> </li> <li> <p>For each resource, each tag key must be unique, and each tag key can have only one value.</p> </li> <li> <p>Maximum key length - 128 Unicode characters in UTF-8</p> </li> <li> <p>Maximum value length - 256 Unicode characters in UTF-8</p> </li> <li> <p>If your tagging schema is used across multiple services and resources, remember that other services may have restrictions on allowed characters. Generally allowed characters are: letters, numbers, and spaces representable in UTF-8, and the following characters: + - = . _ : / @.</p> </li> <li> <p>Tag keys and values are case-sensitive.</p> </li> <li> <p>Do not use <code>aws:</code>, <code>AWS:</code>, or any upper or lowercase combination of such as a prefix for either keys or values as it is reserved for Amazon Web Services use. You cannot edit or delete tag keys or values with this prefix. Tags with this prefix do not count against your tags per resource limit.</p> </li> </ul>",
                     "shape": "Tags"
                 },
                 "taskDefinition": {
                     "documentation": "<p>The <code>family</code> and <code>revision</code> (<code>family:revision</code>) or full ARN of the task definition to start. If a <code>revision</code> isn't specified, the latest <code>ACTIVE</code> revision is used.</p>",
                     "shape": "String"
-                },
-                "volumeConfigurations": {
-                    "documentation": "<p>The details of the volume that was <code>configuredAtLaunch</code>. You can configure the size, volumeType, IOPS, throughput, snapshot and encryption in <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_TaskManagedEBSVolumeConfiguration.html\">TaskManagedEBSVolumeConfiguration</a>. The <code>name</code> of the volume must match the <code>name</code> from the task definition.</p>",
-                    "shape": "TaskVolumeConfigurations"
                 }
             },
             "required": [
                 "containerInstances",
                 "taskDefinition"
             ],
             "type": "structure"
@@ -6466,15 +6263,15 @@
         "StopTaskRequest": {
             "members": {
                 "cluster": {
                     "documentation": "<p>The short name or full Amazon Resource Name (ARN) of the cluster that hosts the task to stop. If you do not specify a cluster, the default cluster is assumed.</p>",
                     "shape": "String"
                 },
                 "reason": {
-                    "documentation": "<p>An optional message specified when a task is stopped. For example, if you're using a custom scheduler, you can use this parameter to specify the reason for stopping the task here, and the message appears in subsequent <a>DescribeTasks</a> API operations on this task.</p>",
+                    "documentation": "<p>An optional message specified when a task is stopped. For example, if you're using a custom scheduler, you can use this parameter to specify the reason for stopping the task here, and the message appears in subsequent <a>DescribeTasks</a> API operations on this task. Up to 255 characters are allowed in this message.</p>",
                     "shape": "String"
                 },
                 "task": {
                     "documentation": "<p>The task ID of the task to stop.</p>",
                     "shape": "String"
                 }
             },
@@ -6632,15 +6429,15 @@
                     "documentation": "<p>Acknowledgement of the state change.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "SystemControl": {
-            "documentation": "<p>A list of namespaced kernel parameters to set in the container. This parameter maps to <code>Sysctls</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--sysctl</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>. For example, you can configure <code>net.ipv4.tcp_keepalive_time</code> setting to maintain longer lived connections.</p> <p>We don't recommend that you specify network-related <code>systemControls</code> parameters for multiple containers in a single task that also uses either the <code>awsvpc</code> or <code>host</code> network mode. Doing this has the following disadvantages:</p> <ul> <li> <p>For tasks that use the <code>awsvpc</code> network mode including Fargate, if you set <code>systemControls</code> for any container, it applies to all containers in the task. If you set different <code>systemControls</code> for multiple containers in a single task, the container that's started last determines which <code>systemControls</code> take effect.</p> </li> <li> <p>For tasks that use the <code>host</code> network mode, the network namespace <code>systemControls</code> aren't supported.</p> </li> </ul> <p>If you're setting an IPC resource namespace to use for the containers in the task, the following conditions apply to your system controls. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definition_parameters.html#task_definition_ipcmode\">IPC mode</a>.</p> <ul> <li> <p>For tasks that use the <code>host</code> IPC mode, IPC namespace <code>systemControls</code> aren't supported.</p> </li> <li> <p>For tasks that use the <code>task</code> IPC mode, IPC namespace <code>systemControls</code> values apply to all containers within a task.</p> </li> </ul> <note> <p>This parameter is not supported for Windows containers.</p> </note> <note> <p>This parameter is only supported for tasks that are hosted on Fargate if the tasks are using platform version <code>1.4.0</code> or later (Linux). This isn't supported for Windows containers on Fargate.</p> </note>",
+            "documentation": "<p>A list of namespaced kernel parameters to set in the container. This parameter maps to <code>Sysctls</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--sysctl</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <p>We don't recommend that you specify network-related <code>systemControls</code> parameters for multiple containers in a single task. This task also uses either the <code>awsvpc</code> or <code>host</code> network mode. It does it for the following reasons.</p> <ul> <li> <p>For tasks that use the <code>awsvpc</code> network mode, if you set <code>systemControls</code> for any container, it applies to all containers in the task. If you set different <code>systemControls</code> for multiple containers in a single task, the container that's started last determines which <code>systemControls</code> take effect.</p> </li> <li> <p>For tasks that use the <code>host</code> network mode, the <code>systemControls</code> parameter applies to the container instance's kernel parameter and that of all containers of any tasks running on that container instance.</p> </li> </ul>",
             "members": {
                 "namespace": {
                     "documentation": "<p>The namespaced kernel parameter to set a <code>value</code> for.</p>",
                     "shape": "String"
                 },
                 "value": {
                     "documentation": "<p>The namespaced kernel parameter to set a <code>value</code> for.</p> <p>Valid IPC namespace values: <code>\"kernel.msgmax\" | \"kernel.msgmnb\" | \"kernel.msgmni\" | \"kernel.sem\" | \"kernel.shmall\" | \"kernel.shmmax\" | \"kernel.shmmni\" | \"kernel.shm_rmid_forced\"</code>, and <code>Sysctls</code> that start with <code>\"fs.mqueue.*\"</code> </p> <p>Valid network namespace values: <code>Sysctls</code> that start with <code>\"net.*\"</code> </p> <p>All of these values are supported by Fargate.</p>",
@@ -6846,15 +6643,15 @@
                     "shape": "Timestamp"
                 },
                 "startedBy": {
                     "documentation": "<p>The tag specified when a task is started. If an Amazon ECS service started the task, the <code>startedBy</code> parameter contains the deployment ID of that service.</p>",
                     "shape": "String"
                 },
                 "stopCode": {
-                    "documentation": "<p>The stop code indicating why a task was stopped. The <code>stoppedReason</code> might contain additional details. </p> <p>For more information about stop code, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/stopped-task-error-codes.html\">Stopped tasks error codes</a> in the <i>Amazon ECS Developer Guide</i>.</p>",
+                    "documentation": "<p>The stop code indicating why a task was stopped. The <code>stoppedReason</code> might contain additional details. </p> <p>For more information about stop code, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/stopped-task-error-codes.html\">Stopped tasks error codes</a> in the <i>Amazon ECS User Guide</i>.</p> <p>The following are valid values:</p> <ul> <li> <p> <code>TaskFailedToStart</code> </p> </li> <li> <p> <code>EssentialContainerExited</code> </p> </li> <li> <p> <code>UserInitiated</code> </p> </li> <li> <p> <code>TerminationNotice</code> </p> </li> <li> <p> <code>ServiceSchedulerInitiated</code> </p> </li> <li> <p> <code>SpotInterruption</code> </p> </li> </ul>",
                     "shape": "TaskStopCode"
                 },
                 "stoppedAt": {
                     "documentation": "<p>The Unix timestamp for the time when the task was stopped. More specifically, it's for the time when the task transitioned from the <code>RUNNING</code> state to the <code>STOPPED</code> state.</p>",
                     "shape": "Timestamp"
                 },
                 "stoppedReason": {
@@ -7054,88 +6851,14 @@
         },
         "TaskFieldList": {
             "member": {
                 "shape": "TaskField"
             },
             "type": "list"
         },
-        "TaskFilesystemType": {
-            "enum": [
-                "ext3",
-                "ext4",
-                "xfs"
-            ],
-            "type": "string"
-        },
-        "TaskManagedEBSVolumeConfiguration": {
-            "documentation": "<p>The configuration for the Amazon EBS volume that Amazon ECS creates and manages on your behalf. These settings are used to create each Amazon EBS volume, with one volume created for each task.</p>",
-            "members": {
-                "encrypted": {
-                    "documentation": "<p>Indicates whether the volume should be encrypted. If no value is specified, encryption is turned on by default. This parameter maps 1:1 with the <code>Encrypted</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p>",
-                    "shape": "BoxedBoolean"
-                },
-                "filesystemType": {
-                    "documentation": "<p>The Linux filesystem type for the volume. For volumes created from a snapshot, you must specify the same filesystem type that the volume was using when the snapshot was created. If there is a filesystem type mismatch, the task will fail to start.</p> <p>The available filesystem types are&#x2028; <code>ext3</code>, <code>ext4</code>, and <code>xfs</code>. If no value is specified, the <code>xfs</code> filesystem type is used by default.</p>",
-                    "shape": "TaskFilesystemType"
-                },
-                "iops": {
-                    "documentation": "<p>The number of I/O operations per second (IOPS). For <code>gp3</code>, <code>io1</code>, and <code>io2</code> volumes, this represents the number of IOPS that are provisioned for the volume. For <code>gp2</code> volumes, this represents the baseline performance of the volume and the rate at which the volume accumulates I/O credits for bursting.</p> <p>The following are the supported values for each volume type.</p> <ul> <li> <p> <code>gp3</code>: 3,000 - 16,000 IOPS</p> </li> <li> <p> <code>io1</code>: 100 - 64,000 IOPS</p> </li> <li> <p> <code>io2</code>: 100 - 256,000 IOPS</p> </li> </ul> <p>This parameter is required for <code>io1</code> and <code>io2</code> volume types. The default for <code>gp3</code> volumes is <code>3,000 IOPS</code>. This parameter is not supported for <code>st1</code>, <code>sc1</code>, or <code>standard</code> volume types.</p> <p>This parameter maps 1:1 with the <code>Iops</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p>",
-                    "shape": "BoxedInteger"
-                },
-                "kmsKeyId": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) identifier of the Amazon Web Services Key Management Service key to use for Amazon EBS encryption. When encryption is turned on and no Amazon Web Services Key Management Service key is specified, the default Amazon Web Services managed key for Amazon EBS volumes is used. This parameter maps 1:1 with the <code>KmsKeyId</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p> <important> <p>Amazon Web Services authenticates the Amazon Web Services Key Management Service key asynchronously. Therefore, if you specify an ID, alias, or ARN that is invalid, the action can appear to complete, but eventually fails.</p> </important>",
-                    "shape": "EBSKMSKeyId"
-                },
-                "roleArn": {
-                    "documentation": "<p>The ARN of the IAM role to associate with this volume. This is the Amazon ECS infrastructure IAM role that is used to manage your Amazon Web Services infrastructure. We recommend using the Amazon ECS-managed <code>AmazonECSInfrastructureRolePolicyForVolumes</code> IAM policy with this role. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/infrastructure_IAM_role.html\">Amazon ECS infrastructure IAM role</a> in the <i>Amazon ECS Developer Guide</i>.</p>",
-                    "shape": "IAMRoleArn"
-                },
-                "sizeInGiB": {
-                    "documentation": "<p>The size of the volume in GiB. You must specify either a volume size or a snapshot ID. If you specify a snapshot ID, the snapshot size is used for the volume size by default. You can optionally specify a volume size greater than or equal to the snapshot size. This parameter maps 1:1 with the <code>Size</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p> <p>The following are the supported volume size values for each volume type.</p> <ul> <li> <p> <code>gp2</code> and <code>gp3</code>: 1-16,384</p> </li> <li> <p> <code>io1</code> and <code>io2</code>: 4-16,384</p> </li> <li> <p> <code>st1</code> and <code>sc1</code>: 125-16,384</p> </li> <li> <p> <code>standard</code>: 1-1,024</p> </li> </ul>",
-                    "shape": "BoxedInteger"
-                },
-                "snapshotId": {
-                    "documentation": "<p>The snapshot that Amazon ECS uses to create the volume. You must specify either a snapshot ID or a volume size. This parameter maps 1:1 with the <code>SnapshotId</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p>",
-                    "shape": "EBSSnapshotId"
-                },
-                "tagSpecifications": {
-                    "documentation": "<p>The tags to apply to the volume. Amazon ECS applies service-managed tags by default. This parameter maps 1:1 with the <code>TagSpecifications.N</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p>",
-                    "shape": "EBSTagSpecifications"
-                },
-                "terminationPolicy": {
-                    "documentation": "<p>The termination policy for the volume when the task exits. This provides a way to control whether Amazon ECS terminates the Amazon EBS volume when the task stops.</p>",
-                    "shape": "TaskManagedEBSVolumeTerminationPolicy"
-                },
-                "throughput": {
-                    "documentation": "<p>The throughput to provision for a volume, in MiB/s, with a maximum of 1,000 MiB/s. This parameter maps 1:1 with the <code>Throughput</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>.</p> <important> <p>This parameter is only supported for the <code>gp3</code> volume type.</p> </important>",
-                    "shape": "BoxedInteger"
-                },
-                "volumeType": {
-                    "documentation": "<p>The volume type. This parameter maps 1:1 with the <code>VolumeType</code> parameter of the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateVolume.html\">CreateVolume API</a> in the <i>Amazon EC2 API Reference</i>. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volume-types.html\">Amazon EBS volume types</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>The following are the supported volume types.</p> <ul> <li> <p>General Purpose SSD: <code>gp2</code>|<code>gp3</code> </p> </li> <li> <p>Provisioned IOPS SSD: <code>io1</code>|<code>io2</code> </p> </li> <li> <p>Throughput Optimized HDD: <code>st1</code> </p> </li> <li> <p>Cold HDD: <code>sc1</code> </p> </li> <li> <p>Magnetic: <code>standard</code> </p> <note> <p>The magnetic volume type is not supported on Fargate.</p> </note> </li> </ul>",
-                    "shape": "EBSVolumeType"
-                }
-            },
-            "required": [
-                "roleArn"
-            ],
-            "type": "structure"
-        },
-        "TaskManagedEBSVolumeTerminationPolicy": {
-            "documentation": "<p>The termination policy for the Amazon EBS volume when the task exits. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ebs-volumes.html#ebs-volume-types\">Amazon ECS volume termination policy</a>.</p>",
-            "members": {
-                "deleteOnTermination": {
-                    "documentation": "<p>Indicates whether the volume should be deleted on when the task stops. If a value of <code>true</code> is specified, &#x2028;Amazon ECS deletes the Amazon EBS volume on your behalf when the task goes into the <code>STOPPED</code> state. If no value is specified, the &#x2028;default value is <code>true</code> is used. When set to <code>false</code>, Amazon ECS leaves the volume in your &#x2028;account.</p>",
-                    "shape": "BoxedBoolean"
-                }
-            },
-            "required": [
-                "deleteOnTermination"
-            ],
-            "type": "structure"
-        },
         "TaskOverride": {
             "documentation": "<p>The overrides that are associated with a task.</p>",
             "members": {
                 "containerOverrides": {
                     "documentation": "<p>One or more container overrides that are sent to a task.</p>",
                     "shape": "ContainerOverrides"
                 },
@@ -7299,57 +7022,20 @@
                 "UserInitiated",
                 "ServiceSchedulerInitiated",
                 "SpotInterruption",
                 "TerminationNotice"
             ],
             "type": "string"
         },
-        "TaskVolumeConfiguration": {
-            "documentation": "<p>Configuration settings for the task volume that was <code>configuredAtLaunch</code> that weren't set during <code>RegisterTaskDef</code>.</p>",
-            "members": {
-                "managedEBSVolume": {
-                    "documentation": "<p>The configuration for the Amazon EBS volume that Amazon ECS creates and manages on your behalf. These settings are used to create each Amazon EBS volume, with one volume created for each task. The Amazon EBS volumes are visible in your account in the Amazon EC2 console once they are created.</p>",
-                    "shape": "TaskManagedEBSVolumeConfiguration"
-                },
-                "name": {
-                    "documentation": "<p>The name of the volume. This value must match the volume name from the <code>Volume</code> object in the task definition.</p>",
-                    "shape": "ECSVolumeName"
-                }
-            },
-            "required": [
-                "name"
-            ],
-            "type": "structure"
-        },
-        "TaskVolumeConfigurations": {
-            "member": {
-                "shape": "TaskVolumeConfiguration"
-            },
-            "type": "list"
-        },
         "Tasks": {
             "member": {
                 "shape": "Task"
             },
             "type": "list"
         },
-        "TimeoutConfiguration": {
-            "documentation": "<p>An object that represents the timeout configurations for Service Connect.</p> <note> <p>If <code>idleTimeout</code> is set to a time that is less than <code>perRequestTimeout</code>, the connection will close when the <code>idleTimeout</code> is reached and not the <code>perRequestTimeout</code>.</p> </note>",
-            "members": {
-                "idleTimeoutSeconds": {
-                    "documentation": "<p>The amount of time in seconds a connection will stay active while idle. A value of <code>0</code> can be set to disable <code>idleTimeout</code>.</p> <p>The <code>idleTimeout</code> default for <code>HTTP</code>/<code>HTTP2</code>/<code>GRPC</code> is 5 minutes.</p> <p>The <code>idleTimeout</code> default for <code>TCP</code> is 1 hour.</p>",
-                    "shape": "Duration"
-                },
-                "perRequestTimeoutSeconds": {
-                    "documentation": "<p>The amount of time waiting for the upstream to respond with a complete response per request. A value of <code>0</code> can be set to disable <code>perRequestTimeout</code>. <code>perRequestTimeout</code> can only be set if Service Connect <code>appProtocol</code> isn't <code>TCP</code>. Only <code>idleTimeout</code> is allowed for <code>TCP</code> <code>appProtocol</code>.</p>",
-                    "shape": "Duration"
-                }
-            },
-            "type": "structure"
-        },
         "Timestamp": {
             "type": "timestamp"
         },
         "Tmpfs": {
             "documentation": "<p>The container path, mount options, and size of the tmpfs mount.</p>",
             "members": {
                 "containerPath": {
@@ -7381,15 +7067,15 @@
             "enum": [
                 "tcp",
                 "udp"
             ],
             "type": "string"
         },
         "Ulimit": {
-            "documentation": "<p>The <code>ulimit</code> settings to pass to the container.</p> <p>Amazon ECS tasks hosted on Fargate use the default resource limit values set by the operating system with the exception of the <code>nofile</code> resource limit parameter which Fargate overrides. The <code>nofile</code> resource limit sets a restriction on the number of open files that a container can use. The default <code>nofile</code> soft limit is <code>1024</code> and the default hard limit is <code>65535</code>.</p> <p>You can specify the <code>ulimit</code> settings for a container in a task definition.</p>",
+            "documentation": "<p>The <code>ulimit</code> settings to pass to the container.</p> <p>Amazon ECS tasks hosted on Fargate use the default resource limit values set by the operating system with the exception of the <code>nofile</code> resource limit parameter which Fargate overrides. The <code>nofile</code> resource limit sets a restriction on the number of open files that a container can use. The default <code>nofile</code> soft limit is <code>1024</code> and the default hard limit is <code>4096</code>.</p> <p>You can specify the <code>ulimit</code> settings for a container in a task definition.</p>",
             "members": {
                 "hardLimit": {
                     "documentation": "<p>The hard limit for the <code>ulimit</code> type.</p>",
                     "shape": "Integer"
                 },
                 "name": {
                     "documentation": "<p>The <code>type</code> of the <code>ulimit</code>.</p>",
@@ -7710,18 +7396,14 @@
                 "serviceRegistries": {
                     "documentation": "<p>The details for the service discovery registries to assign to this service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-discovery.html\">Service Discovery</a>.</p> <p>When you add, update, or remove the service registries configuration, Amazon ECS starts new tasks with the updated service registries configuration, and then stops the old tasks when the new tasks are running.</p> <p>You can remove existing <code>serviceRegistries</code> by passing an empty list.</p>",
                     "shape": "ServiceRegistries"
                 },
                 "taskDefinition": {
                     "documentation": "<p>The <code>family</code> and <code>revision</code> (<code>family:revision</code>) or full ARN of the task definition to run in your service. If a <code>revision</code> is not specified, the latest <code>ACTIVE</code> revision is used. If you modify the task definition with <code>UpdateService</code>, Amazon ECS spawns a task with the new version of the task definition and then stops an old task after the new version is running.</p>",
                     "shape": "String"
-                },
-                "volumeConfigurations": {
-                    "documentation": "<p>The details of the volume that was <code>configuredAtLaunch</code>. You can configure the size, volumeType, IOPS, throughput, snapshot and encryption in <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_ServiceManagedEBSVolumeConfiguration.html\">ServiceManagedEBSVolumeConfiguration</a>. The <code>name</code> of the volume must match the <code>name</code> from the task definition. If set to null, no new deployment is triggered. Otherwise, if this configuration differs from the existing one, it triggers a new deployment.</p>",
-                    "shape": "ServiceVolumeConfigurations"
                 }
             },
             "required": [
                 "service"
             ],
             "type": "structure"
         },
@@ -7824,20 +7506,16 @@
                     "documentation": "<p>The Docker version that's running on the container instance.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "Volume": {
-            "documentation": "<p>The data volume configuration for tasks launched using this task definition. Specifying a volume configuration in a task definition is optional. The volume configuration may contain multiple volumes but only one volume configured at launch is supported. Each volume defined in the volume configuration may only specify a <code>name</code> and one of either <code>configuredAtLaunch</code>, <code>dockerVolumeConfiguration</code>, <code>efsVolumeConfiguration</code>, <code>fsxWindowsFileServerVolumeConfiguration</code>, or <code>host</code>. If an empty volume configuration is specified, by default Amazon ECS uses a host volume. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using_data_volumes.html\">Using data volumes in tasks</a>.</p>",
+            "documentation": "<p>A data volume that's used in a task definition. For tasks that use the Amazon Elastic File System (Amazon EFS), specify an <code>efsVolumeConfiguration</code>. For Windows tasks that use Amazon FSx for Windows File Server file system, specify a <code>fsxWindowsFileServerVolumeConfiguration</code>. For tasks that use a Docker volume, specify a <code>DockerVolumeConfiguration</code>. For tasks that use a bind mount host volume, specify a <code>host</code> and optional <code>sourcePath</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using_data_volumes.html\">Using Data Volumes in Tasks</a>.</p>",
             "members": {
-                "configuredAtLaunch": {
-                    "documentation": "<p>Indicates whether the volume should be configured at launch time. This is used to create Amazon EBS volumes for standalone tasks or tasks created as part of a service. Each task definition revision may only have one volume configured at launch in the volume configuration.</p> <p>To configure a volume at launch time, use this task definition revision and specify a <code>volumeConfigurations</code> object when calling the <code>CreateService</code>, <code>UpdateService</code>, <code>RunTask</code> or <code>StartTask</code> APIs.</p>",
-                    "shape": "BoxedBoolean"
-                },
                 "dockerVolumeConfiguration": {
                     "documentation": "<p>This parameter is specified when you use Docker volumes.</p> <p>Windows containers only support the use of the <code>local</code> driver. To use bind mounts, specify the <code>host</code> parameter instead.</p> <note> <p>Docker volumes aren't supported by tasks run on Fargate.</p> </note>",
                     "shape": "DockerVolumeConfiguration"
                 },
                 "efsVolumeConfiguration": {
                     "documentation": "<p>This parameter is specified when you use an Amazon Elastic File System file system for task storage.</p>",
                     "shape": "EFSVolumeConfiguration"
@@ -7847,15 +7525,15 @@
                     "shape": "FSxWindowsFileServerVolumeConfiguration"
                 },
                 "host": {
                     "documentation": "<p>This parameter is specified when you use bind mount host volumes. The contents of the <code>host</code> parameter determine whether your bind mount host volume persists on the host container instance and where it's stored. If the <code>host</code> parameter is empty, then the Docker daemon assigns a host path for your data volume. However, the data isn't guaranteed to persist after the containers that are associated with it stop running.</p> <p>Windows containers can mount whole directories on the same drive as <code>$env:ProgramData</code>. Windows containers can't mount directories on a different drive, and mount point can't be across drives. For example, you can mount <code>C:\\my\\path:C:\\my\\path</code> and <code>D:\\:D:\\</code>, but not <code>D:\\my\\path:C:\\my\\path</code> or <code>D:\\:C:\\my\\path</code>.</p>",
                     "shape": "HostVolumeProperties"
                 },
                 "name": {
-                    "documentation": "<p>The name of the volume. Up to 255 letters (uppercase and lowercase), numbers, underscores, and hyphens are allowed.</p> <p>When using a volume configured at launch, the <code>name</code> is required and must also be specified as the volume name in the <code>ServiceVolumeConfiguration</code> or <code>TaskVolumeConfiguration</code> parameter when creating your service or standalone task.</p> <p>For all other types of volumes, this name is referenced in the <code>sourceVolume</code> parameter of the <code>mountPoints</code> object in the container definition.</p> <p>When a volume is using the <code>efsVolumeConfiguration</code>, the name is required.</p>",
+                    "documentation": "<p>The name of the volume. Up to 255 letters (uppercase and lowercase), numbers, underscores, and hyphens are allowed. This name is referenced in the <code>sourceVolume</code> parameter of container definition <code>mountPoints</code>.</p> <p>This is required wwhen you use an Amazon EFS volume.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "VolumeFrom": {
             "documentation": "<p>Details on a data volume from another container in the same task definition.</p>",
```

### Comparing `botocore-a-la-carte-ecs-1.34.80/botocore/data/ecs/2014-11-13/waiters-2.json` & `botocore-a-la-carte-ecs-1.34.9/botocore/data/ecs/2014-11-13/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.34.80/botocore_a_la_carte_ecs.egg-info/PKG-INFO` & `botocore-a-la-carte-ecs-1.34.9/botocore_a_la_carte_ecs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ecs
-Version: 1.34.80
+Version: 1.34.9
 Summary: ecs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ecs-1.34.80/setup.py` & `botocore-a-la-carte-ecs-1.34.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ecs',
-    version="1.34.80",
+    version="1.34.9",
     description='ecs data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ecs/*/*.json'],
```

