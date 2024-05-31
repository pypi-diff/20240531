# Comparing `tmp/ado_wrapper-1.8.4.tar.gz` & `tmp/ado_wrapper-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.8.4.tar", max compression
+gzip compressed data, was "ado_wrapper-1.8.5.tar", max compression
```

## Comparing `ado_wrapper-1.8.4.tar` & `ado_wrapper-1.8.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.8.4/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.8.4/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.8.4/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.8.4/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.8.4/ado_wrapper/client.py
--rw-r--r--   0        0        0    21892 2024-05-07 18:26:17.266989 ado_wrapper-1.8.4/ado_wrapper/dumps.py
--rw-r--r--   0        0        0     3537 2024-05-06 10:01:09.344505 ado_wrapper-1.8.4/ado_wrapper/generate_docs.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.8.4/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.8.4/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.8.4/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.8.4/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.8.4/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.8.4/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.8.4/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3791 2024-05-06 09:59:23.335964 ado_wrapper-1.8.4/ado_wrapper/resources/agent_pools.py
--rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.8.4/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3520 2024-05-15 12:17:11.865100 ado_wrapper-1.8.4/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    15269 2024-05-06 13:26:32.155840 ado_wrapper-1.8.4/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.8.4/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.8.4/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3268 2024-05-07 17:20:44.533690 ado_wrapper-1.8.4/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    16206 2024-05-15 15:53:51.165482 ado_wrapper-1.8.4/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.8.4/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14012 2024-05-06 16:33:39.036236 ado_wrapper-1.8.4/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.8.4/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10768 2024-05-07 11:42:12.821826 ado_wrapper-1.8.4/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0    12706 2024-05-15 10:28:55.220198 ado_wrapper-1.8.4/ado_wrapper/resources/repo_user_permission.py
--rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.8.4/ado_wrapper/resources/searches.py
--rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.8.4/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.8.4/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8326 2024-05-07 18:19:31.197732 ado_wrapper-1.8.4/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.8.4/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9459 2024-05-06 09:44:07.348306 ado_wrapper-1.8.4/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.8.4/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.8.4/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2760 2024-05-15 15:54:04.641817 ado_wrapper-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.8.5/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.8.5/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.8.5/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.8.5/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.8.5/ado_wrapper/client.py
+-rw-r--r--   0        0        0    21892 2024-05-07 18:26:17.266989 ado_wrapper-1.8.5/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0     3537 2024-05-06 10:01:09.344505 ado_wrapper-1.8.5/ado_wrapper/generate_docs.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.8.5/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.8.5/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.8.5/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.8.5/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3791 2024-05-06 09:59:23.335964 ado_wrapper-1.8.5/ado_wrapper/resources/agent_pools.py
+-rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.8.5/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3520 2024-05-15 12:17:11.865100 ado_wrapper-1.8.5/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    15269 2024-05-06 13:26:32.155840 ado_wrapper-1.8.5/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.8.5/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.8.5/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3268 2024-05-07 17:20:44.533690 ado_wrapper-1.8.5/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15632 2024-05-31 16:42:45.204130 ado_wrapper-1.8.5/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.8.5/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14012 2024-05-06 16:33:39.036236 ado_wrapper-1.8.5/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.8.5/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10768 2024-05-07 11:42:12.821826 ado_wrapper-1.8.5/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0    12706 2024-05-15 10:28:55.220198 ado_wrapper-1.8.5/ado_wrapper/resources/repo_user_permission.py
+-rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.8.5/ado_wrapper/resources/searches.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.8.5/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.8.5/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8326 2024-05-07 18:19:31.197732 ado_wrapper-1.8.5/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.8.5/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9459 2024-05-06 09:44:07.348306 ado_wrapper-1.8.5/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.8.5/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.8.5/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-05-31 16:43:16.418854 ado_wrapper-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.8.5/PKG-INFO
```

### Comparing `ado_wrapper-1.8.4/LICENSE` & `ado_wrapper-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/README.md` & `ado_wrapper-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/__main__.py` & `ado_wrapper-1.8.5/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/client.py` & `ado_wrapper-1.8.5/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/dumps.py` & `ado_wrapper-1.8.5/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/generate_docs.py` & `ado_wrapper-1.8.5/ado_wrapper/generate_docs.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/agent_pools.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/agent_pools.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/branches.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/builds.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/commits.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/environment.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/groups.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/merge_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,16 @@
         return policy[0] if policy else None
 
     @staticmethod
     def set_branch_policy(ado_client: AdoClient, repo_id: str, minimum_approver_count: int,
                           creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
                           when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> None:  # fmt: skip
         """Sets the perms for a pull request, can also be used as a "update" function."""
-        existing_policy = MergePolicies.get_all_by_repo_id(ado_client, repo_id, branch_name)
-        latest_policy_id = (f"/{existing_policy[0].policy_id}") if existing_policy is not None else ""
+        existing_policy = MergePolicies.get_branch_policy(ado_client, repo_id, branch_name)
+        latest_policy_id = f"/{existing_policy.policy_id}" if existing_policy is not None else ""
         payload = {
             "settings": {
                 "minimumApproverCount": minimum_approver_count,
                 "creatorVoteCounts": creator_vote_counts,
                 "blockLastPusherVote": prohibit_last_pushers_vote,
                 "allowDownvotes": allow_completion_with_rejects,
                 "requireVoteOnEachIteration": when_new_changes_are_pushed == "require_revote_on_each_iteration",
@@ -163,24 +163,18 @@
                 "scope": [{"refName": f"refs/heads/{branch_name}", "repositoryId": repo_id, "matchKind": "Exact"}],
             },
             "type": {"id": _get_type_id(ado_client, "Minimum number of reviewers")},
             "isEnabled": True,
             "isBlocking": True,
         }
         request = ado_client.session.request(
-            "POST" if not latest_policy_id else "PUT",
+            "PUT" if latest_policy_id else "POST",
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/Configurations{latest_policy_id}?api-version=7.1",  # fmt: skip
             json=payload,
-            # headers={"Accept": "application/json;api-version=7.1"},
         )
-        if request.status_code == 400:
-            # {"$id":"1","innerException":null,"message":"A policy configuration's policy type cannot be changed once set.",
-            # "typeName":"Microsoft.TeamFoundation.Policy.Server.PolicyTypeCannotBeChangedException, Microsoft.TeamFoundation.Policy.Server",
-            # "typeKey":"PolicyTypeCannotBeChangedException","errorCode":0,"eventId":3000}
-            raise ConfigurationError("Error setting branch policy, perhaps due to permissions.")
         assert request.status_code == 200, f"Error setting branch policy: {request.text}"
 
 
 @dataclass
 class MergePolicies(StateManagedResource):
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> list[MergePolicyDefaultReviewer | MergeBranchPolicy] | None:  # type: ignore[override]
```

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/projects.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/releases.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/repo.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/repo_user_permission.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/repo_user_permission.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/searches.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/searches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/teams.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/users.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.8.5/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.8.5/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/state_manager.py` & `ado_wrapper-1.8.5/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/ado_wrapper/utils.py` & `ado_wrapper-1.8.5/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.4/pyproject.toml` & `ado_wrapper-1.8.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.8.4"
+version = "1.8.5"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.8.4/PKG-INFO` & `ado_wrapper-1.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.8.4
+Version: 1.8.5
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

