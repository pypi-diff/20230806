# Comparing `tmp/ghast_scanner-1.5.7.tar.gz` & `tmp/ghast_scanner-1.6.7.tar.gz`

## Comparing `ghast_scanner-1.5.7.tar` & `ghast_scanner-1.6.7.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/.pylintrc
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/EXAMPLES.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/__about__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/action.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/colors.py
--rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/requirements.txt
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/.github/workflows/ghast-scan.yml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-create-or-approves-pr-using-curl.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-creates-or-approves-pr-using-gh-cli.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-creates-or-approves-pr-using-gh-script.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-using-upload-artifact-action.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-dangerous-gh-variables-2.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-dangerous-gh-variables.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-remote-script.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/analyzer/__init__.py
--rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/analyzer/analyzer.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/analyzer/analyzer_test.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/analyzer/regex.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/LICENSE
--rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/README.md
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/pyproject.toml
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 ghast_scanner-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/.pylintrc
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/EXAMPLES.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/__about__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/action.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/colors.py
+-rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/requirements.txt
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/setup.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/.github/workflows/ghast-scan.yml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-create-or-approves-pr-using-curl.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-creates-or-approves-pr-using-gh-cli.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-creates-or-approves-pr-using-gh-script.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-upload-artifact-action.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-remote-script.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/analyzer/__init__.py
+-rw-r--r--   0        0        0    17447 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/analyzer/analyzer.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/analyzer/regex.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/LICENSE
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/README.md
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/pyproject.toml
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/PKG-INFO
```

### Comparing `ghast_scanner-1.5.7/EXAMPLES.md` & `ghast_scanner-1.6.7/EXAMPLES.md`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/action.yml` & `ghast_scanner-1.6.7/action.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/colors.py` & `ghast_scanner-1.6.7/colors.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/main.py` & `ghast_scanner-1.6.7/main.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/.github/workflows/ghast-scan.yml` & `ghast_scanner-1.6.7/.github/workflows/ghast-scan.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/actions/action-create-or-approves-pr-using-curl.yml` & `ghast_scanner-1.6.7/actions/action-create-or-approves-pr-using-curl.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `ghast_scanner-1.6.7/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/analyzer/analyzer.py` & `ghast_scanner-1.6.7/analyzer/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             "_check_for_inline_script": {"level": "WARN"},
             "_check_for_pull_request_target": {"level": "FAIL"},
             "_check_for_script_injection": {"level": "FAIL"},
             "_check_for_self_hosted_runners": {"level": "WARN"},
             "_check_for_aws_configure_credentials_non_oidc": {"level": "WARN"},
             "_check_for_create_or_approve_pull_request": {"level": "FAIL"},
             "_check_for_remote_script": {"level": "WARN"},
+            "_check_for_non_github_managed_actions": {"level": "WARN"},
         }
         self.auxiliary_checks = [
             "_check_for_codeowners_file",
         ]
         self.action = {}
         self.jobs = {}
 
@@ -341,14 +342,28 @@
                 f"{Colors.LIGHT_BLUE}AUXI{Colors.END} missing CODEOWNERS file"
                 "which can provide additional protections for your workflow files"
             )
         else:
             if self.verbose:
                 print(f"{Colors.LIGHT_BLUE}AUXI{Colors.END} found CODEOWNERS file")
 
+    def _check_for_non_github_managed_actions(self) -> bool:
+        passed = True
+        for job in self.jobs:
+            for step in self.jobs[job]["steps"]:
+                if "uses" in step:
+                    action = step["uses"].strip()
+                    if not search(analyzer.regex.GITHUB_MANAGED_ACTION, action):
+                        if self.verbose:
+                            print(
+                                f"{Colors.LIGHT_GRAY}INFO{Colors.END} using non GitHub-managed action('{action}') - make sure its safe to use!"
+                            )
+                        passed = False
+        return passed
+
     def _run_aux_checks(self) -> None:
         """Runs auxiliary checks which are checks for security-related
         configurations/properties/mechanisms that contribute to more secure
         GitHub Actions workflows.
         """
         # TODO:
         # - Add check for missing SECURITY.md file
```

### Comparing `ghast_scanner-1.5.7/analyzer/analyzer_test.py` & `ghast_scanner-1.6.7/analyzer/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/analyzer/regex.py` & `ghast_scanner-1.6.7/analyzer/regex.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 CONFIGURE_AWS_CREDS_ACTION = r"aws\-actions\/configure\-aws\-credentials@(v\d+(\.\d+)?(\.\d+)?|[a-f0-9]{40})"
 GH_CLI_PR_CREATE_APPROVE = r"gh pr (review.*--approve|create.*)"
 GITHUB_SCRIPT_ACTION = r"actions\/github\-script@(v\d+(\.\d+)?(\.\d+)?|[a-f0-9]{40})"
 GITHUB_SCRIPT_CREATE_APPROVE_PR = r".*github\.rest\.pulls\.(create\(.*|reviews\(.*APPROVE.*)"
 CURL_CREATE_APPROVE_PR = (
     r".*curl.*https:\/\/api\.github\.com\/repos\/[0-9a-zA-Z-._]+\/[0-9a-zA-Z-._]+\/pulls\/[0-9]{1,}\/reviews.*"
 )
+GITHUB_MANAGED_ACTION = r"^actions\/.*"
```

### Comparing `ghast_scanner-1.5.7/.gitignore` & `ghast_scanner-1.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/LICENSE` & `ghast_scanner-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/README.md` & `ghast_scanner-1.6.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 ### See Additional Workflow Examples
 [Additional Ghast Workflow Examples](EXAMPLES.md)
 
 ### Checks Performed by `ghast`
 
 1. Name: `check_for_3p_actions_without_hash`, Level: `FAIL`
 
-    - This check identifies any third-party GitHub Actions in use that have been referenced via a version number such as `v1.1` instead of commit SHA haah. Using a hash can help mitigate supply chain threats in a scenario where a threat actor has compromised the source repository where the 3P action lives.
+    - This check identifies any third party GitHub Actions in use that have been referenced via a version number such as `v1.1` instead of commit SHA haah. Using a hash can help mitigate supply chain threats in a scenario where a threat actor has compromised the source repository where the 3P action lives.
 
 2. Name: `check_for_allow_unsecure_commands`, Level: `FAIL`
 
     - This check looks for the usage of environment variable called `ACTIONS_ALLOW_UNSECURE_COMMANDS` which allows for an Action to get access to dangerous commands (`get-env`, `add-path`) which can lead to code injection and credential thefts opportunities.
 
 3. Name: `check_for_cache_action`, Level: `WARN`
 
@@ -92,14 +92,18 @@
 
     - This check looks for a URL in an inline script of a GitHub Action which usually signals the inclusion of a remote script which can be dangerous.
   
 12. Name: `check_for_upload_download_artifact_action`, Level: `WARN`
 
     - This check is essential for identifying any usage of GitHub's upload/download artifact Action, as it can potentially expose your workflow to compromised files. For instance, an uploaded artifact might contain a compiled binary from a previous workflow, but this binary could be compromised due to the introduction of malicious dependencies during the compilation phase. Consequently, if this tainted binary is executed within another workflow, it could lead to significant security risks. To mitigate such risks, it is crucial for users to conduct integrity checks on artifacts before consumption. This check serves as a valuable reminder to reinforce this security practice.
 
+13. Name: `check_for_non_github_managed_actions`, Level: `WARN`
+
+    - This check looks for inclusion of non GitHub-managed actions and serves as a reminder to review the security posture of any third party actions you include in your workflow(s), especially if they are not developed and maintained by credible entities.
+
 #### Auxiliary Checks
 
 1. Name: `check_for_codeowners_file` - checks for existence of [CODEOWNERS](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) file.
 
 ### References
 
 - [Security hardening for GitHub Actions](https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions)
```

### Comparing `ghast_scanner-1.5.7/pyproject.toml` & `ghast_scanner-1.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.5.7/PKG-INFO` & `ghast_scanner-1.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghast-scanner
-Version: 1.5.7
+Version: 1.6.7
 Summary: Analyze the security posture of your GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/ghast#readme
 Project-URL: Issues, https://github.com/bin3xish477/ghast/issues
 Project-URL: Source, https://github.com/bin3xish477/ghast
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -73,15 +73,15 @@
 ### See Additional Workflow Examples
 [Additional Ghast Workflow Examples](EXAMPLES.md)
 
 ### Checks Performed by `ghast`
 
 1. Name: `check_for_3p_actions_without_hash`, Level: `FAIL`
 
-    - This check identifies any third-party GitHub Actions in use that have been referenced via a version number such as `v1.1` instead of commit SHA haah. Using a hash can help mitigate supply chain threats in a scenario where a threat actor has compromised the source repository where the 3P action lives.
+    - This check identifies any third party GitHub Actions in use that have been referenced via a version number such as `v1.1` instead of commit SHA haah. Using a hash can help mitigate supply chain threats in a scenario where a threat actor has compromised the source repository where the 3P action lives.
 
 2. Name: `check_for_allow_unsecure_commands`, Level: `FAIL`
 
     - This check looks for the usage of environment variable called `ACTIONS_ALLOW_UNSECURE_COMMANDS` which allows for an Action to get access to dangerous commands (`get-env`, `add-path`) which can lead to code injection and credential thefts opportunities.
 
 3. Name: `check_for_cache_action`, Level: `WARN`
 
@@ -119,14 +119,18 @@
 
     - This check looks for a URL in an inline script of a GitHub Action which usually signals the inclusion of a remote script which can be dangerous.
   
 12. Name: `check_for_upload_download_artifact_action`, Level: `WARN`
 
     - This check is essential for identifying any usage of GitHub's upload/download artifact Action, as it can potentially expose your workflow to compromised files. For instance, an uploaded artifact might contain a compiled binary from a previous workflow, but this binary could be compromised due to the introduction of malicious dependencies during the compilation phase. Consequently, if this tainted binary is executed within another workflow, it could lead to significant security risks. To mitigate such risks, it is crucial for users to conduct integrity checks on artifacts before consumption. This check serves as a valuable reminder to reinforce this security practice.
 
+13. Name: `check_for_non_github_managed_actions`, Level: `WARN`
+
+    - This check looks for inclusion of non GitHub-managed actions and serves as a reminder to review the security posture of any third party actions you include in your workflow(s), especially if they are not developed and maintained by credible entities.
+
 #### Auxiliary Checks
 
 1. Name: `check_for_codeowners_file` - checks for existence of [CODEOWNERS](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) file.
 
 ### References
 
 - [Security hardening for GitHub Actions](https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions)
```

