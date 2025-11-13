# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Build_Scan/main`
- **Build Number:** #5
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 20 sec and counting
- **Timestamp:** 2025-11-13 19:15:22 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 6cc77dde08f999df62791bf205b4414fbadff2a5
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
Checking out Revision 6cc77dde08f999df62791bf205b4414fbadff2a5 (main)
Commit message: "Delete jenkins-logs directory"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 6cc77dde08f999df62791bf205b4414fbadff2a5 # timeout=10
 > git rev-list --no-walk ff4496e43d08672c0f0894b4ada74aa888ba3d12 # timeout=10
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

up to date, audited 1412 packages in 21s

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
[Security Scan] INFO:  --- network_ssl_trustAll = false
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
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/polaris_input15292543998821516705.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 19:13:42.2733 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 19:13:42.2873 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 19:13:43.6101 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 19:13:43.6102 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 19:13:43.6102 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 19:13:43.6102 IST [Bridge CLI] INFO: network.airgap = false [polaris_input15292543998821516705.json]
2025-11-13 19:13:43.6102 IST [Bridge CLI] INFO: network.ssl.trustAll = false [polaris_input15292543998821516705.json]
2025-11-13 19:13:43.6102 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input15292543998821516705.json]
2025-11-13 19:13:43.6102 IST [Bridge CLI] INFO: polaris.application.name = build-scan [polaris_input15292543998821516705.json]
2025-11-13 19:13:43.6102 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input15292543998821516705.json]
2025-11-13 19:13:43.6102 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input15292543998821516705.json]
2025-11-13 19:13:43.6103 IST [Bridge CLI] INFO: polaris.project.name = build-scan [polaris_input15292543998821516705.json]
2025-11-13 19:13:43.6103 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input15292543998821516705.json]
2025-11-13 19:13:43.6103 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input15292543998821516705.json]
2025-11-13 19:13:43.6103 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 19:13:43.6103 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 19:13:43.6119 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 19:13:43.6119 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 19:13:43.6119 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 19:13:43.6119 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 19:13:43.6857 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 19:13:43.6894 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 19:13:43.6895 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 19:13:43.6896 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 19:13:43.6929 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 19:13:43.6931 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 19:13:43.6931 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 19:13:46.4706 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "S0YE8KP"
2025-11-13 19:13:46.4794 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "38FSAMA"
2025-11-13 19:13:46.5150 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 19:13:46.5152 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 19:13:46.5154 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 19:13:46.5155 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 19:13:46.5157 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 19:13:46.5158 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 19:13:46.5159 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 19:13:46.5160 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 19:13:46.5164 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 19:13:46.5167 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 19:13:46.5170 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 19:13:46.5289 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 19:13:46.5609 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 19:13:46.5612 IST [Check pull request] INFO: Adapter finished
2025-11-13 19:13:46.6020 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 19:13:46.6024 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 19:13:47.5074 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 19:13:47.5075 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 19:13:47.5079 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 19:13:47.5724 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 19:13:47.8781 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 19:13:47.8782 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 19:13:48.2009 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 19:13:48.2010 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 19:13:48.2011 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 19:13:48.3124 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 19:13:48.6249 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 19:13:48.6251 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 19:13:48.6251 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 19:13:48.9319 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 19:13:48.9320 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 19:13:48.9930 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 19:13:48.9964 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 19:13:49.3034 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 19:13:49.3288 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 19:13:49.3289 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 19:13:49.3291 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 19:13:49.3291 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 19:13:49.3291 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 19:13:49.3291 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 19:13:49.3291 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 19:13:49.3301 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 19:13:49.3301 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 19:13:49.3302 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 19:13:49.3307 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 19:13:49.3302 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 19:13:49.3302 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 19:13:49.3302 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 19:13:49.3609 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 19:13:49.3610 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 19:13:49.3611 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 19:13:49.3677 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 19:13:49.3678 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 19:13:49.3678 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 19:13:49.4299 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 19:13:49.4314 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 19:13:50.1517 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 19:13:50.1518 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache4050454374/.authKey
2025-11-13 19:13:50.1518 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=52168e44-d2de-4aa7-a699-58314a4d1b46
2025-11-13 19:13:50.1518 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 19:13:50.1518 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 19:13:50.1519 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 19:13:50.1548 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir reset-host-name
2025-11-13 19:13:50.1956 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir check-compatible
2025-11-13 19:13:50.2153 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 19:13:50.2154 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 19:13:50.2170 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 19:13:50.2171 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 19:13:52.7721 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 19:13:52.7740 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 19:13:53.7934 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:13:53.8190 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 19:13:54.3558 IST [Polaris Coverity Capture] INFO: Executing action no-op: skipping compiler configuration
2025-11-13 19:13:54.8112 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 19:13:55.3856 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 19:13:55.9577 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-2216840681 --record-with-source
2025-11-13 19:13:55.9839 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 19:13:55.9985 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 19:13:56.1721 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 19:13:56.1744 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 19:13:56.1745 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 19:13:56.1746 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 19:13:56.1748 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:13:56.1966 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 19:13:56.1967 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-907546759/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 19:13:56.2281 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 19:13:56.2282 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 19:13:56.2282 IST [Polaris Coverity Capture] INFO: 
2025-11-13 19:13:57.8547 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 19:13:58.3451 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:13:58.4014 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 19:13:58.4014 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 19:13:58.4014 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 19:13:58.4014 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 19:13:58.4014 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 19:13:58.4014 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 19:13:58.4014 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32920
2025-11-13 19:13:58.4032 IST [Polaris Coverity Capture] INFO: Capture phase took 5.631s.
2025-11-13 19:13:58.4032 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 19:13:58.4032 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 19:13:58.4032 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 19:13:58.4032 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 19:13:58.4032 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 19:13:58.4291 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 19:13:58.4311 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 19:13:58.4380 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 19:13:58.4381 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 19:13:58.4383 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 19:13:58.4385 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 19:13:58.4404 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 19:13:58.4405 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 19:13:58.4406 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 19:13:58.4727 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 19:13:59.2655 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 19:13:59.2656 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 19:13:59.2656 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 19:13:59.2656 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 19:13:59.2656 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 19:13:59.2656 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 19:13:59.2657 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 19:13:59.3890 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 19:13:59.3891 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 19:13:59.3891 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge [env] 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-13-43-59-351
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 19:13:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm (depth 0)
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/package-lock.json
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/package.json
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 19:14:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 19:14:01.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-13-43-59-351/scan/components-with-locations.json
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-13-43-59-351/status/status.json
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-13-43-59-351/scan/components-with-locations.json
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:14:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 44s 814ms
2025-11-13 19:14:43.6189 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 19:14:43.6191 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 19:14:43.6192 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 19:14:43.6590 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "94709180-0e2d-4d18-aa89-aa75cccd7e47"
2025-11-13 19:14:43.6592 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "c3d60c9c-00ba-4df7-b0fe-a5f1d4f2f0a4"
2025-11-13 19:14:45.0796 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 19:14:45.1007 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 19:14:45.7544 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208463
2025-11-13 19:14:45.7635 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   3%  16384/414068
2025-11-13 19:14:45.9739 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208463
2025-11-13 19:14:45.9760 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208463
2025-11-13 19:14:45.9792 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  31%  131072/414068
2025-11-13 19:14:46.4087 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208463/208463
2025-11-13 19:14:46.4154 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  59%  245760/414068
2025-11-13 19:14:46.4187 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  87%  360448/414068
2025-11-13 19:14:46.6311 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  414068/414068
2025-11-13 19:14:46.9497 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 19:14:47.1240 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 19:14:47.4968 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "c3d60c9c-00ba-4df7-b0fe-a5f1d4f2f0a4"
2025-11-13 19:14:47.6164 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "94709180-0e2d-4d18-aa89-aa75cccd7e47"
2025-11-13 19:14:47.6508 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 19:14:47.6533 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 19:14:47.6544 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 19:14:47.7111 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "94709180-0e2d-4d18-aa89-aa75cccd7e47"
2025-11-13 19:14:47.7114 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "c3d60c9c-00ba-4df7-b0fe-a5f1d4f2f0a4"
2025-11-13 19:14:48.4906 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "c3d60c9c-00ba-4df7-b0fe-a5f1d4f2f0a4" is "Queuing"
2025-11-13 19:14:48.4927 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "94709180-0e2d-4d18-aa89-aa75cccd7e47" is "Queuing"
2025-11-13 19:14:58.8080 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "94709180-0e2d-4d18-aa89-aa75cccd7e47" is "Scanning"
2025-11-13 19:14:58.8127 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "c3d60c9c-00ba-4df7-b0fe-a5f1d4f2f0a4" is "Scanning & Publishing"
2025-11-13 19:15:09.1293 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "94709180-0e2d-4d18-aa89-aa75cccd7e47" is "In Progress"
2025-11-13 19:15:19.4370 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "c3d60c9c-00ba-4df7-b0fe-a5f1d4f2f0a4" completed successfully
2025-11-13 19:15:19.4553 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "94709180-0e2d-4d18-aa89-aa75cccd7e47" completed successfully
2025-11-13 19:15:19.4785 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 19:15:19.4788 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 19:15:19.4793 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 19:15:19.5539 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 19:15:19.5548 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 19:15:20.5234 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 19:15:20.5585 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 19:15:20.6086 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 19:15:20.6097 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 19:15:21.4041 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "c3d60c9c-00ba-4df7-b0fe-a5f1d4f2f0a4"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 19:15:21.4124 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "94709180-0e2d-4d18-aa89-aa75cccd7e47"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 19:15:21.4422 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 19:15:21.4427 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 19:15:21.4431 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 19:15:21.4434 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 19:15:21.4438 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 19:15:21.4442 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.medium'
2025-11-13 19:15:21.4445 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.critical'
2025-11-13 19:15:21.4449 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.low'
2025-11-13 19:15:21.4453 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.high'
2025-11-13 19:15:21.4456 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.informational'
2025-11-13 19:15:21.4463 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 19:15:21.5113 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "94709180-0e2d-4d18-aa89-aa75cccd7e47" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/tests/94709180-0e2d-4d18-aa89-aa75cccd7e47/detected-issues
2025-11-13 19:15:21.5118 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "c3d60c9c-00ba-4df7-b0fe-a5f1d4f2f0a4" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/tests/c3d60c9c-00ba-4df7-b0fe-a5f1d4f2f0a4/detected-issues
2025-11-13 19:15:21.5118 IST [Polaris Status Provider] INFO: Polaris issues view for project "build-scan", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/issues?branchId=cadc1965-5328-45d1-8f2b-6a90ddec708f
2025-11-13 19:15:21.5197 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 19:15:21.5199 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 19:15:21.5201 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 19:15:21.5204 IST [Polaris Status Provider] INFO: Adapter finished
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
Build Number: 5
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