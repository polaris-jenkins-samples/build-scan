# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Build_Scan/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 50 sec and counting
- **Timestamp:** 2025-11-13 11:28:17 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 03b8cc9b537f4ebddeca68a1810a1988d187af13
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
Checking out Revision 03b8cc9b537f4ebddeca68a1810a1988d187af13 (main)
Commit message: "Create Jenkinsfile"
First time build. Skipping changelog.
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 03b8cc9b537f4ebddeca68a1810a1988d187af13 # timeout=10
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

up to date, audited 1412 packages in 4s

32 packages are looking for funding
  run `npm fund` for details

137 vulnerabilities (9 low, 35 moderate, 57 high, 36 critical)

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
[Pipeline] { (blackduck-security-scan)
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
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/polaris_input11211808059275154540.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 11:25:44.7399 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 11:25:44.7500 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 11:25:46.0053 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 11:25:46.0054 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 11:25:46.0054 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 11:25:46.0054 IST [Bridge CLI] INFO: network.airgap = false [polaris_input11211808059275154540.json]
2025-11-13 11:25:46.0054 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input11211808059275154540.json]
2025-11-13 11:25:46.0054 IST [Bridge CLI] INFO: polaris.application.name = build-scan [polaris_input11211808059275154540.json]
2025-11-13 11:25:46.0054 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input11211808059275154540.json]
2025-11-13 11:25:46.0054 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input11211808059275154540.json]
2025-11-13 11:25:46.0054 IST [Bridge CLI] INFO: polaris.project.name = build-scan [polaris_input11211808059275154540.json]
2025-11-13 11:25:46.0054 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input11211808059275154540.json]
2025-11-13 11:25:46.0055 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input11211808059275154540.json]
2025-11-13 11:25:46.0055 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 11:25:46.0055 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 11:25:46.0071 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 11:25:46.0071 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 11:25:46.0071 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 11:25:46.0071 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 11:25:46.0909 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 11:25:46.0944 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 11:25:46.0945 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 11:25:46.0946 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 11:25:46.0976 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 11:25:46.0977 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 11:25:46.0978 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 11:25:46.9108 IST [Polaris Initializer] INFO: application doesn't exist. Will create new application as 'polaris.onboarding' is set to 'true'
2025-11-13 11:25:47.6539 IST [Polaris Initializer] INFO: project doesn't exist. Will create new project as 'polaris.onboarding' is set to 'true'
2025-11-13 11:25:48.9610 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "DT3VC16"
2025-11-13 11:25:49.2631 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "PCEMU40"
2025-11-13 11:25:49.2885 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 11:25:49.2890 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 11:25:49.2894 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 11:25:49.2898 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 11:25:49.2903 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 11:25:49.2907 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 11:25:49.2910 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 11:25:49.2913 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 11:25:49.2917 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 11:25:49.2920 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 11:25:49.2930 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 11:25:49.3147 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 11:25:49.3588 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 11:25:49.3590 IST [Check pull request] INFO: Adapter finished
2025-11-13 11:25:49.4119 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 11:25:49.4123 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 11:25:50.2912 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 11:25:50.2913 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 11:25:50.3746 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 11:25:50.3778 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 11:25:50.6751 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 11:25:50.6754 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 11:25:50.6754 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 11:25:50.9736 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 11:25:50.9737 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 11:25:50.9743 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 11:25:51.2656 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 11:25:51.5636 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 11:25:51.5637 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 11:25:51.9293 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 11:25:51.9294 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 11:25:51.9297 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 11:25:52.6897 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 11:25:52.9967 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 11:25:53.0227 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 11:25:53.0229 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 11:25:53.0231 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 11:25:53.0232 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 11:25:53.0232 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 11:25:53.0233 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 11:25:53.0233 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 11:25:53.0254 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 11:25:53.0254 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 11:25:53.0254 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 11:25:53.0255 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 11:25:53.0255 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 11:25:53.0255 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 11:25:53.0261 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 11:25:53.0641 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 11:25:53.0646 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 11:25:53.0647 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 11:25:53.0728 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 11:25:53.0729 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 11:25:53.0729 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 11:25:53.1383 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 11:25:53.1388 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 11:25:53.4482 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 11:25:53.4483 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache465252287/.authKey
2025-11-13 11:25:53.4483 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=52168e44-d2de-4aa7-a699-58314a4d1b46
2025-11-13 11:25:53.4483 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 11:25:53.4483 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 11:25:53.4483 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 11:25:53.4489 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 11:25:53.4489 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 11:25:53.4497 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 11:25:53.6111 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 11:25:53.6112 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 11:25:54.6321 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 11:25:54.6362 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 11:25:55.1611 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 11:25:55.1741 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 11:25:55.5997 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 11:25:55.5999 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 11:25:55.9953 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 11:25:56.2193 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 11:25:56.4435 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 11:25:56.6895 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 11:25:56.9307 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 11:25:57.1739 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 11:25:57.4146 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 11:25:57.6494 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 11:25:57.6494 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 11:25:57.6494 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 11:25:57.6539 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 11:25:57.9010 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 11:25:58.1242 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 11:25:58.3578 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 11:25:58.5970 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 11:25:58.8378 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 11:25:58.8584 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 11:25:58.8584 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 11:25:59.3395 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 11:25:59.7637 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 11:26:00.3184 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-2751024692 --record-with-source
2025-11-13 11:26:00.4620 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 11:26:00.4766 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 11:26:01.1785 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 11:26:01.1800 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 11:26:01.1800 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 11:26:01.1801 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 11:26:01.1803 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 11:26:01.1957 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 11:26:01.1957 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-3103587608/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 11:26:01.3327 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 11:26:01.3327 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 11:26:01.3327 IST [Polaris Coverity Capture] INFO: 
2025-11-13 11:26:02.9089 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 11:26:03.3867 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 11:26:03.4411 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 11:26:03.4412 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 11:26:03.4412 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 11:26:03.4412 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 11:26:03.4412 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 11:26:03.4412 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 11:26:03.4412 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32920
2025-11-13 11:26:03.4428 IST [Polaris Coverity Capture] INFO: Capture phase took 8.812s.
2025-11-13 11:26:03.4428 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 11:26:03.4428 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 11:26:03.4428 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 11:26:03.4428 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 11:26:03.4429 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 11:26:03.4650 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 11:26:03.4672 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 11:26:03.4741 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 11:26:03.4744 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 11:26:03.4746 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 11:26:03.4749 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 11:26:03.4763 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 11:26:03.4764 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 11:26:03.4765 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 11:26:03.5068 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 11:26:04.2284 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 11:26:04.2285 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 11:26:04.2285 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 11:26:04.2285 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 11:26:04.2285 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 11:26:04.2285 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 11:26:04.2286 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 11:26:04.3449 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 11:26:04.3450 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 11:26:04.3450 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge [env] 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-05-56-04-307
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm (depth 0)
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/package-lock.json
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/package.json
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 11:26:04.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 11:26:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-05-56-04-307/scan/components-with-locations.json
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-05-56-04-307/status/status.json
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-05-56-04-307/scan/components-with-locations.json
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:26:47.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 44s 023ms
2025-11-13 11:26:47.8534 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 11:26:47.8535 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 11:26:47.8537 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 11:26:47.9052 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "bd7241d6-9df3-4189-9ba6-1b1986eb5d53"
2025-11-13 11:26:47.9056 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "d2b319bd-3f31-4b8a-913c-2fb5c3c3c8e5"
2025-11-13 11:26:48.7997 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 11:26:48.8735 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 11:26:48.8843 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208462
2025-11-13 11:26:48.8930 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208462
2025-11-13 11:26:48.8953 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208462
2025-11-13 11:26:48.9109 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/385395
2025-11-13 11:26:48.9182 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208462/208462
2025-11-13 11:26:48.9241 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/385395
2025-11-13 11:26:48.9452 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  55%  212992/385395
2025-11-13 11:26:48.9469 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  80%  311296/385395
2025-11-13 11:26:48.9532 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  385395/385395
2025-11-13 11:26:50.1923 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 11:26:50.2836 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 11:26:50.9247 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "d2b319bd-3f31-4b8a-913c-2fb5c3c3c8e5"
2025-11-13 11:26:50.9249 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "bd7241d6-9df3-4189-9ba6-1b1986eb5d53"
2025-11-13 11:26:50.9514 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 11:26:50.9518 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 11:26:50.9524 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 11:26:51.0305 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "bd7241d6-9df3-4189-9ba6-1b1986eb5d53"
2025-11-13 11:26:51.0312 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "d2b319bd-3f31-4b8a-913c-2fb5c3c3c8e5"
2025-11-13 11:26:51.8954 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "d2b319bd-3f31-4b8a-913c-2fb5c3c3c8e5" is "Queuing"
2025-11-13 11:26:51.9233 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "bd7241d6-9df3-4189-9ba6-1b1986eb5d53" is "Queuing"
2025-11-13 11:27:02.2547 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "d2b319bd-3f31-4b8a-913c-2fb5c3c3c8e5" is "Scanning & Publishing"
2025-11-13 11:27:02.2547 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "bd7241d6-9df3-4189-9ba6-1b1986eb5d53" is "Scanning"
2025-11-13 11:27:22.9099 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "d2b319bd-3f31-4b8a-913c-2fb5c3c3c8e5" completed successfully
2025-11-13 11:28:14.7551 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "bd7241d6-9df3-4189-9ba6-1b1986eb5d53" completed successfully
2025-11-13 11:28:14.7871 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 11:28:14.7881 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 11:28:14.7886 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 11:28:14.8745 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 11:28:14.8753 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 11:28:15.8604 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 11:28:15.8849 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 11:28:15.9427 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 11:28:15.9436 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 11:28:16.3126 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "d2b319bd-3f31-4b8a-913c-2fb5c3c3c8e5"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 11:28:16.3168 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "bd7241d6-9df3-4189-9ba6-1b1986eb5d53"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 11:28:16.3450 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.informational'
2025-11-13 11:28:16.3454 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.low'
2025-11-13 11:28:16.3467 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.high'
2025-11-13 11:28:16.3471 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.medium'
2025-11-13 11:28:16.3474 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.critical'
2025-11-13 11:28:16.3476 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 11:28:16.3478 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 11:28:16.3480 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 11:28:16.3482 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 11:28:16.3484 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 11:28:16.3487 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 11:28:16.4006 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "d2b319bd-3f31-4b8a-913c-2fb5c3c3c8e5" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/tests/d2b319bd-3f31-4b8a-913c-2fb5c3c3c8e5/detected-issues
2025-11-13 11:28:16.4011 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "bd7241d6-9df3-4189-9ba6-1b1986eb5d53" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/tests/bd7241d6-9df3-4189-9ba6-1b1986eb5d53/detected-issues
2025-11-13 11:28:16.4011 IST [Polaris Status Provider] INFO: Polaris issues view for project "build-scan", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/0b228256-8d91-4452-be38-b39cb9327dad/projects/898bdc6f-5f91-45c1-a98e-6f3f243fb9ab/issues?branchId=cadc1965-5328-45d1-8f2b-6a90ddec708f
2025-11-13 11:28:16.4109 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 11:28:16.4112 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 11:28:16.4114 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 11:28:16.4116 IST [Polaris Status Provider] INFO: Adapter finished
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
Build Number: 2
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