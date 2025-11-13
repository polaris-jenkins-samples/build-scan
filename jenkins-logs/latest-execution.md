# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Build_Scan/main`
- **Build Number:** #3
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 45 sec and counting
- **Timestamp:** 2025-11-13 11:35:01 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from bb078a1692a64eee082ce8e86cc1531a0d751fec
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/P_Github_Polaris_Build_Scan_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/.git # timeout=10
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/build-scan.git # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/build-scan.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/build-scan.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision bb078a1692a64eee082ce8e86cc1531a0d751fec (main)
Commit message: "Update Jenkinsfile"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f bb078a1692a64eee082ce8e86cc1531a0d751fec # timeout=10
 > git rev-list --no-walk 03b8cc9b537f4ebddeca68a1810a1988d187af13 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Polaris_Build_Scan/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.

up to date, audited 1412 packages in 14s

32 packages are looking for funding
  run `npm fund` for details

136 vulnerabilities (9 low, 35 moderate, 57 high, 35 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (polaris-build-scan)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Build_Scan
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [POLARIS]
[Security Scan] INFO: Parameters for polaris:
[Security Scan] INFO:  --- polaris_waitForScan = true
[Security Scan] INFO:  --- polaris_server_url = https://poc.polaris.blackduck.com
[Security Scan] INFO:  --- polaris_assessment_types = SAST,SCA
[Security Scan] INFO:  --- polaris_access_token = ******************************************************************************
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Polaris parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Build_Scan
[Security Scan] INFO: Polaris Application Name: build-scan
[Security Scan] INFO: Polaris Project Name: build-scan
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Build_Scan
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/polaris_input2097635793229381957.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 11:32:46.0981 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 11:32:46.1127 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 11:32:47.3954 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 11:32:47.3955 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 11:32:47.3955 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 11:32:47.3955 IST [Bridge CLI] INFO: network.airgap = false [polaris_input2097635793229381957.json]
2025-11-13 11:32:47.3955 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input2097635793229381957.json]
2025-11-13 11:32:47.3955 IST [Bridge CLI] INFO: polaris.application.name = build-scan [polaris_input2097635793229381957.json]
2025-11-13 11:32:47.3955 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input2097635793229381957.json]
2025-11-13 11:32:47.3955 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input2097635793229381957.json]
2025-11-13 11:32:47.3955 IST [Bridge CLI] INFO: polaris.project.name = build-scan [polaris_input2097635793229381957.json]
2025-11-13 11:32:47.3955 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input2097635793229381957.json]
2025-11-13 11:32:47.3956 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input2097635793229381957.json]
2025-11-13 11:32:47.3956 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 11:32:47.3956 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 11:32:47.3972 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 11:32:47.3972 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 11:32:47.3972 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 11:32:47.3972 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 11:32:47.4659 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 11:32:47.4690 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 11:32:47.4691 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 11:32:47.4691 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 11:32:47.4725 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 11:32:47.4726 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 11:32:47.4726 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 11:32:50.0319 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "2OTOX8D"
2025-11-13 11:32:50.0320 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "H5T8NA3"
2025-11-13 11:32:50.0607 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 11:32:50.0611 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 11:32:50.0615 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 11:32:50.0618 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 11:32:50.0621 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 11:32:50.0624 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 11:32:50.0627 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 11:32:50.0629 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 11:32:50.0631 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 11:32:50.0633 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 11:32:50.0638 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 11:32:50.0817 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 11:32:50.1269 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 11:32:50.1272 IST [Check pull request] INFO: Adapter finished
2025-11-13 11:32:50.1711 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 11:32:50.1714 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 11:32:50.5435 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 11:32:50.5436 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 11:32:50.5442 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 11:32:50.6303 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 11:32:50.9308 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 11:32:50.9310 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 11:32:51.2237 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 11:32:51.2238 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 11:32:51.2240 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 11:32:51.3176 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 11:32:51.6145 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 11:32:51.6147 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 11:32:51.6147 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 11:32:51.9769 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 11:32:51.9770 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 11:32:52.0735 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 11:32:52.0772 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 11:32:52.3917 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 11:32:52.4203 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 11:32:52.4207 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 11:32:52.4212 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 11:32:52.4213 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 11:32:52.4213 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 11:32:52.4213 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 11:32:52.4213 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 11:32:52.4225 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 11:32:52.4226 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 11:32:52.4226 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 11:32:52.4226 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 11:32:52.4226 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 11:32:52.4226 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 11:32:52.4229 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 11:32:52.4655 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 11:32:52.4666 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 11:32:52.4667 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 11:32:52.4758 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 11:32:52.4761 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 11:32:52.4761 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 11:32:52.5320 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 11:32:52.5326 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 11:32:52.5866 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 11:32:52.5866 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache2938487787/.authKey
2025-11-13 11:32:52.5867 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=52168e44-d2de-4aa7-a699-58314a4d1b46
2025-11-13 11:32:52.5867 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 11:32:52.5867 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 11:32:52.5867 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 11:32:52.5900 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir reset-host-name
2025-11-13 11:32:52.6310 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir check-compatible
2025-11-13 11:32:52.6480 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 11:32:52.6480 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 11:32:52.6503 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 11:32:52.6504 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 11:32:53.2176 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 11:32:53.2203 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 11:32:53.7537 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 11:32:53.7775 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 11:32:54.2314 IST [Polaris Coverity Capture] INFO: Executing action no-op: skipping compiler configuration
2025-11-13 11:32:54.6513 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 11:32:55.0893 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 11:32:55.6990 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-2585143417 --record-with-source
2025-11-13 11:32:55.7239 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 11:32:55.7373 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 11:32:55.8893 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 11:32:55.8909 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 11:32:55.8910 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 11:32:55.8911 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 11:32:55.8913 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 11:32:55.9098 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 11:32:55.9099 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-3868238783/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 11:32:55.9399 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 11:32:55.9399 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 11:32:55.9399 IST [Polaris Coverity Capture] INFO: 
2025-11-13 11:32:57.5704 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 11:32:58.0708 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 11:32:58.1263 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 11:32:58.1263 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 11:32:58.1263 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 11:32:58.1264 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 11:32:58.1264 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 11:32:58.1264 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 11:32:58.1264 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32920
2025-11-13 11:32:58.1284 IST [Polaris Coverity Capture] INFO: Capture phase took 4.911s.
2025-11-13 11:32:58.1285 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 11:32:58.1285 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 11:32:58.1285 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 11:32:58.1285 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 11:32:58.1285 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 11:32:58.1539 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 11:32:58.1556 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 11:32:58.1620 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 11:32:58.1621 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 11:32:58.1622 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 11:32:58.1624 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 11:32:58.1639 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 11:32:58.1640 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 11:32:58.1641 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 11:32:58.1964 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 11:32:58.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 11:32:58.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 11:32:58.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 11:32:58.9251 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 11:32:58.9251 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 11:32:58.9251 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 11:32:58.9252 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 11:32:58.9252 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 11:32:58.9252 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 11:32:58.9252 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 11:32:59.0506 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 11:32:59.0507 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 11:32:59.0507 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge [env] 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-06-02-59-007
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm (depth 0)
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/package-lock.json
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/package.json
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 11:32:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 11:33:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:33:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 11:33:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:33:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 11:33:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:33:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 11:33:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-06-02-59-007/scan/components-with-locations.json
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-06-02-59-007/status/status.json
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-06-02-59-007/scan/components-with-locations.json
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:33:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 45s 092ms
2025-11-13 11:33:43.6214 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 11:33:43.6216 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 11:33:43.6218 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 11:33:43.6589 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "90d0f5a6-690c-43c3-a121-8a2399f361be"
2025-11-13 11:33:43.6592 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "5ac8f289-32c1-438d-b17b-b3dacd936ff3"
2025-11-13 11:33:44.6396 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 11:33:44.6610 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 11:33:44.6818 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208309
2025-11-13 11:33:44.6891 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208309
2025-11-13 11:33:44.6912 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208309
2025-11-13 11:33:44.7013 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/399355
2025-11-13 11:33:44.7096 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208309/208309
2025-11-13 11:33:44.7169 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  32%  131072/399355
2025-11-13 11:33:44.7396 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  57%  229376/399355
2025-11-13 11:33:44.7478 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  82%  327680/399355
2025-11-13 11:33:44.7539 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  399355/399355
2025-11-13 11:33:45.9427 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 11:33:46.1478 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 11:33:46.5560 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "5ac8f289-32c1-438d-b17b-b3dacd936ff3"
2025-11-13 11:33:46.6369 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "90d0f5a6-690c-43c3-a121-8a2399f361be"
2025-11-13 11:33:46.6610 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 11:33:46.6616 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 11:33:46.6628 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 11:33:46.7240 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "90d0f5a6-690c-43c3-a121-8a2399f361be"
2025-11-13 11:33:46.7245 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "5ac8f289-32c1-438d-b17b-b3dacd936ff3"
2025-11-13 11:33:47.1746 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "5ac8f289-32c1-438d-b17b-b3dacd936ff3" is "Queuing"
2025-11-13 11:33:47.1747 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "90d0f5a6-690c-43c3-a121-8a2399f361be" is "Waiting for Capture"
2025-11-13 11:33:57.4999 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "5ac8f289-32c1-438d-b17b-b3dacd936ff3" is "Scanning & Publishing"
2025-11-13 11:33:57.4999 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "90d0f5a6-690c-43c3-a121-8a2399f361be" is "Scanning"
2025-11-13 11:34:18.1187 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "5ac8f289-32c1-438d-b17b-b3dacd936ff3" completed successfully
2025-11-13 11:34:59.4653 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "90d0f5a6-690c-43c3-a121-8a2399f361be" completed successfully
2025-11-13 11:34:59.4727 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 11:34:59.4729 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 11:34:59.4732 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 11:34:59.5240 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 11:34:59.5244 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 11:34:59.8962 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "90d0f5a6-690c-43c3-a121-8a2399f361be"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 11:34:59.9207 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "5ac8f289-32c1-438d-b17b-b3dacd936ff3"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 11:34:59.9499 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.informational'
2025-11-13 11:34:59.9504 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.low'
2025-11-13 11:34:59.9509 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.medium'
2025-11-13 11:34:59.9511 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.critical'
2025-11-13 11:34:59.9513 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.high'
2025-11-13 11:34:59.9515 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 11:34:59.9517 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 11:34:59.9519 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 11:34:59.9521 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 11:34:59.9523 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 11:34:59.9529 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 11:34:59.9834 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 11:34:59.9840 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 11:35:00.4012 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 11:35:00.4231 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 11:35:00.4580 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "90d0f5a6-690c-43c3-a121-8a2399f361be" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/tests/90d0f5a6-690c-43c3-a121-8a2399f361be/detected-issues
2025-11-13 11:35:00.4584 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "5ac8f289-32c1-438d-b17b-b3dacd936ff3" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/tests/5ac8f289-32c1-438d-b17b-b3dacd936ff3/detected-issues
2025-11-13 11:35:00.4584 IST [Polaris Status Provider] INFO: Polaris issues view for project "build-scan", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/issues?branchId=cadc1965-5328-45d1-8f2b-6a90ddec708f
2025-11-13 11:35:00.4666 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 11:35:00.4668 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 11:35:00.4670 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 11:35:00.4672 IST [Polaris Status Provider] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 303
[Security Scan] INFO: Security Scan execution is successful
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:polaris-jenkins-samples, repoName:build-scan, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Polaris_Build_Scan/main
[Pipeline] echo
Build Number: 3
[Pipeline] echo
GitHub Organization: polaris-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: build-scan
[Pipeline] echo
Target repository: polaris-jenkins-samples/build-scan
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*