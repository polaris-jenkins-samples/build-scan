# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Build_Scan/main`
- **Build Number:** #4
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 4 min 52 sec and counting
- **Timestamp:** 2025-11-13 15:09:10 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from ff4496e43d08672c0f0894b4ada74aa888ba3d12
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
Checking out Revision ff4496e43d08672c0f0894b4ada74aa888ba3d12 (main)
Commit message: "Delete jenkins-logs directory"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f ff4496e43d08672c0f0894b4ada74aa888ba3d12 # timeout=10
 > git rev-list --no-walk bb078a1692a64eee082ce8e86cc1531a0d751fec # timeout=10
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

up to date, audited 1412 packages in 20s

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
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/polaris_input218694576014225438.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 15:04:55.3961 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 15:04:55.4120 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 15:04:56.7614 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 15:04:56.7614 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 15:04:56.7614 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 15:04:56.7614 IST [Bridge CLI] INFO: network.airgap = false [polaris_input218694576014225438.json]
2025-11-13 15:04:56.7614 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input218694576014225438.json]
2025-11-13 15:04:56.7615 IST [Bridge CLI] INFO: polaris.application.name = build-scan [polaris_input218694576014225438.json]
2025-11-13 15:04:56.7615 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input218694576014225438.json]
2025-11-13 15:04:56.7615 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input218694576014225438.json]
2025-11-13 15:04:56.7615 IST [Bridge CLI] INFO: polaris.project.name = build-scan [polaris_input218694576014225438.json]
2025-11-13 15:04:56.7615 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input218694576014225438.json]
2025-11-13 15:04:56.7615 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input218694576014225438.json]
2025-11-13 15:04:56.7615 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 15:04:56.7615 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 15:04:56.7636 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 15:04:56.7636 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 15:04:56.7636 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 15:04:56.7636 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 15:04:56.8553 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 15:04:56.8589 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 15:04:56.8590 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 15:04:56.8591 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 15:04:56.8626 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 15:04:56.8627 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 15:04:56.8627 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 15:04:59.7385 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "7SJNR1I"
2025-11-13 15:04:59.7561 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "L8C1UJV"
2025-11-13 15:04:59.7899 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 15:04:59.7902 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 15:04:59.7903 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 15:04:59.7905 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 15:04:59.7907 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 15:04:59.7908 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 15:04:59.7910 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 15:04:59.7911 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 15:04:59.7913 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 15:04:59.7914 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 15:04:59.7920 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 15:04:59.8086 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 15:04:59.8542 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 15:04:59.8544 IST [Check pull request] INFO: Adapter finished
2025-11-13 15:04:59.9036 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 15:04:59.9039 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 15:05:00.6452 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 15:05:00.6453 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 15:05:00.6457 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 15:05:00.7508 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 15:05:01.0516 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 15:05:01.0517 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 15:05:01.3393 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 15:05:01.3393 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 15:05:01.3394 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 15:05:01.4368 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 15:05:01.7195 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 15:05:01.7197 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 15:05:01.7197 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 15:05:02.0155 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 15:05:02.0155 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 15:05:02.0848 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 15:05:02.0884 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 15:05:02.3902 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 15:05:02.4167 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 15:05:02.4168 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 15:05:02.4169 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 15:05:02.4169 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 15:05:02.4169 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 15:05:02.4169 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 15:05:02.4169 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 15:05:02.4179 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 15:05:02.4179 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 15:05:02.4179 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 15:05:02.4181 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 15:05:02.4179 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 15:05:02.4179 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 15:05:02.4179 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 15:05:02.4442 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 15:05:02.4446 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 15:05:02.4447 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 15:05:02.4510 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 15:05:02.4511 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 15:05:02.4511 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 15:05:02.5210 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 15:05:02.5223 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 15:05:02.5863 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 15:05:02.5864 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache539476777/.authKey
2025-11-13 15:05:02.5864 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=52168e44-d2de-4aa7-a699-58314a4d1b46
2025-11-13 15:05:02.5864 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 15:05:02.5865 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 15:05:02.5865 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 15:05:02.5923 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir reset-host-name
2025-11-13 15:05:02.6522 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir check-compatible
2025-11-13 15:05:02.6768 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 15:05:02.6769 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 15:05:02.6788 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 15:05:02.6792 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 15:05:03.5370 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 15:05:03.5428 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 15:05:04.7242 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 15:05:04.7540 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 15:05:05.2985 IST [Polaris Coverity Capture] INFO: Executing action no-op: skipping compiler configuration
2025-11-13 15:05:05.7337 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 15:05:06.1653 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 15:05:06.7376 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-573767963 --record-with-source
2025-11-13 15:05:06.7773 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 15:05:06.7945 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 15:05:07.0136 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 15:05:07.0159 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 15:05:07.0160 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 15:05:07.0160 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 15:05:07.0162 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 15:05:07.0350 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 15:05:07.0351 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-107103827/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 15:05:07.0665 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 15:05:07.0666 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 15:05:07.0666 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:05:08.7576 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 15:05:09.2623 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 15:05:09.3199 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 15:05:09.3199 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 15:05:09.3199 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 15:05:09.3199 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 15:05:09.3199 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 15:05:09.3199 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 15:05:09.3200 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32920
2025-11-13 15:05:09.3224 IST [Polaris Coverity Capture] INFO: Capture phase took 5.786s.
2025-11-13 15:05:09.3224 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 15:05:09.3225 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 15:05:09.3225 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 15:05:09.3225 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 15:05:09.3225 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 15:05:09.3484 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 15:05:09.3502 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 15:05:09.3569 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 15:05:09.3570 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 15:05:09.3572 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 15:05:09.3574 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 15:05:09.3593 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 15:05:09.3595 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 15:05:09.3595 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 15:05:09.4054 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 15:05:09.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 15:05:09.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 15:05:09.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 15:05:10.4538 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 15:05:10.4538 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 15:05:10.4538 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 15:05:10.4539 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 15:05:10.4539 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 15:05:10.4539 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 15:05:10.4539 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 15:05:10.5866 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 15:05:10.5866 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 15:05:10.5866 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge [env] 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-35-10-544
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 15:05:10.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm (depth 0)
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/package-lock.json
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/package.json
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 15:05:11.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 15:05:12.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-35-10-544/scan/components-with-locations.json
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-35-10-544/status/status.json
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-35-10-544/scan/components-with-locations.json
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:05:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 46s 477ms
2025-11-13 15:05:56.2191 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 15:05:56.2192 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 15:05:56.2195 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 15:05:56.2756 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "e46648a6-d94e-4952-9878-c40950b3068e"
2025-11-13 15:05:56.2761 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "0134d931-4fc5-4a6d-851b-35e5d07a3ea4"
2025-11-13 15:05:57.6837 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 15:05:57.7242 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 15:05:58.4176 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/406260
2025-11-13 15:05:58.4397 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208951
2025-11-13 15:05:58.6493 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208951
2025-11-13 15:05:58.6494 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  32%  131072/406260
2025-11-13 15:05:58.6495 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208951
2025-11-13 15:05:59.0658 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208951/208951
2025-11-13 15:05:59.0679 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  60%  245760/406260
2025-11-13 15:05:59.0808 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  88%  360448/406260
2025-11-13 15:05:59.2819 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  406260/406260
2025-11-13 15:05:59.5918 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 15:05:59.7574 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 15:06:00.1718 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "0134d931-4fc5-4a6d-851b-35e5d07a3ea4"
2025-11-13 15:06:00.1995 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "e46648a6-d94e-4952-9878-c40950b3068e"
2025-11-13 15:06:00.2419 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 15:06:00.2432 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 15:06:00.2445 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 15:06:00.3238 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "e46648a6-d94e-4952-9878-c40950b3068e"
2025-11-13 15:06:00.3246 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "0134d931-4fc5-4a6d-851b-35e5d07a3ea4"
2025-11-13 15:06:01.0984 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "0134d931-4fc5-4a6d-851b-35e5d07a3ea4" is "Queuing"
2025-11-13 15:06:01.1671 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "e46648a6-d94e-4952-9878-c40950b3068e" is "Queuing"
2025-11-13 15:06:11.4346 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "0134d931-4fc5-4a6d-851b-35e5d07a3ea4" is "Scanning & Publishing"
2025-11-13 15:06:11.4699 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "e46648a6-d94e-4952-9878-c40950b3068e" is "Scanning"
2025-11-13 15:06:32.0695 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "0134d931-4fc5-4a6d-851b-35e5d07a3ea4" completed successfully
2025-11-13 15:09:06.8381 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "e46648a6-d94e-4952-9878-c40950b3068e" completed successfully
2025-11-13 15:09:06.8601 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 15:09:06.8609 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 15:09:06.8652 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 15:09:06.9461 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 15:09:06.9468 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 15:09:07.8253 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 15:09:07.8444 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 15:09:07.9077 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 15:09:07.9083 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 15:09:08.6749 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "e46648a6-d94e-4952-9878-c40950b3068e"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 15:09:08.7585 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "0134d931-4fc5-4a6d-851b-35e5d07a3ea4"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 15:09:08.7796 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.low'
2025-11-13 15:09:08.7799 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.medium'
2025-11-13 15:09:08.7804 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.critical'
2025-11-13 15:09:08.7811 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.high'
2025-11-13 15:09:08.7813 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.informational'
2025-11-13 15:09:08.7815 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 15:09:08.7817 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 15:09:08.7819 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 15:09:08.7821 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 15:09:08.7824 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 15:09:08.7828 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 15:09:08.8420 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "e46648a6-d94e-4952-9878-c40950b3068e" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/tests/e46648a6-d94e-4952-9878-c40950b3068e/detected-issues
2025-11-13 15:09:08.8424 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "0134d931-4fc5-4a6d-851b-35e5d07a3ea4" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/tests/0134d931-4fc5-4a6d-851b-35e5d07a3ea4/detected-issues
2025-11-13 15:09:08.8424 IST [Polaris Status Provider] INFO: Polaris issues view for project "build-scan", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/issues?branchId=cadc1965-5328-45d1-8f2b-6a90ddec708f
2025-11-13 15:09:08.8500 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 15:09:08.8502 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 15:09:08.8503 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 15:09:08.8505 IST [Polaris Status Provider] INFO: Adapter finished
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
Build Number: 4
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