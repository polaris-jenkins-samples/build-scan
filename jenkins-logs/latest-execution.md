# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Coverity_Build_Scan/main`
- **Build Number:** #1
- **Build Status:** ⚪ **ABORTED**
- **Duration:** 5 min 32 sec and counting
- **Timestamp:** 2025-11-13 19:11:36 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from ad12b24d629720347b3da816007b5510614c9be1
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/integrations-garage/blackduck-logs-publisher
 > git init /Users/madhusud/.jenkins/workspace/_Github_Coverity_Build_Scan_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb # timeout=10
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
 > git config --add remote.origin.fetch +refs/heads/*:refs/remotes/origin/* # timeout=10
Avoid second fetch
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
First time build. Skipping changelog.
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/polaris-jenkins-samples/build-scan.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/build-scan.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/build-scan.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Avoid second fetch
Checking out Revision ad12b24d629720347b3da816007b5510614c9be1 (main)
Commit message: "Jenkins log upload - Build #4"
First time build. Skipping changelog.
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/build-scan.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f ad12b24d629720347b3da816007b5510614c9be1 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Coverity_Build_Scan/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm
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
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)

added 962 packages, and audited 1412 packages in 39s

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
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Build_Scan
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
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Build_Scan
[Security Scan] INFO: Polaris Application Name: build-scan
[Security Scan] INFO: Polaris Project Name: build-scan
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Build_Scan
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/polaris_input2053679697596456233.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 19:07:00.1580 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 19:07:00.1678 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 19:07:01.4934 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 19:07:01.4935 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 19:07:01.4935 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 19:07:01.4935 IST [Bridge CLI] INFO: network.airgap = false [polaris_input2053679697596456233.json]
2025-11-13 19:07:01.4935 IST [Bridge CLI] INFO: network.ssl.trustAll = false [polaris_input2053679697596456233.json]
2025-11-13 19:07:01.4935 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input2053679697596456233.json]
2025-11-13 19:07:01.4935 IST [Bridge CLI] INFO: polaris.application.name = build-scan [polaris_input2053679697596456233.json]
2025-11-13 19:07:01.4936 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input2053679697596456233.json]
2025-11-13 19:07:01.4936 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input2053679697596456233.json]
2025-11-13 19:07:01.4936 IST [Bridge CLI] INFO: polaris.project.name = build-scan [polaris_input2053679697596456233.json]
2025-11-13 19:07:01.4936 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input2053679697596456233.json]
2025-11-13 19:07:01.4936 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input2053679697596456233.json]
2025-11-13 19:07:01.4936 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 19:07:01.4936 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 19:07:01.4953 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 19:07:01.4953 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 19:07:01.4953 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 19:07:01.4953 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 19:07:01.5821 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 19:07:01.5853 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 19:07:01.5855 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 19:07:01.5855 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 19:07:01.5889 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 19:07:01.5891 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 19:07:01.5891 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 19:07:04.5470 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "B1S4G1B"
2025-11-13 19:07:04.6132 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "9E1ZLWZ"
2025-11-13 19:07:04.6206 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 19:07:04.6207 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 19:07:04.6209 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 19:07:04.6210 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 19:07:04.6212 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 19:07:04.6213 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 19:07:04.6214 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 19:07:04.6215 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 19:07:04.6216 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 19:07:04.6217 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 19:07:04.6220 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 19:07:04.6330 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 19:07:04.6696 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 19:07:04.6698 IST [Check pull request] INFO: Adapter finished
2025-11-13 19:07:04.7278 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 19:07:04.7282 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 19:07:05.4955 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 19:07:05.4956 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 19:07:05.4957 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 19:07:05.5316 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 19:07:05.8438 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 19:07:05.8438 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 19:07:06.1436 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 19:07:06.1437 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 19:07:06.1448 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 19:07:06.2752 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 19:07:06.5777 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 19:07:06.5778 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 19:07:06.5778 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 19:07:06.8792 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 19:07:06.8793 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 19:07:06.9694 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 19:07:06.9740 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 19:07:07.2874 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 19:07:07.3158 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 19:07:07.3159 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 19:07:07.3160 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 19:07:07.3161 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 19:07:07.3161 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 19:07:07.3161 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 19:07:07.3161 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 19:07:07.3170 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 19:07:07.3170 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 19:07:07.3170 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 19:07:07.3170 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 19:07:07.3170 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 19:07:07.3170 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 19:07:07.3174 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 19:07:07.3499 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 19:07:07.3502 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 19:07:07.3503 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 19:07:07.3583 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 19:07:07.3585 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 19:07:07.3585 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 19:07:07.3966 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 19:07:07.3973 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 19:07:07.4515 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 19:07:07.4515 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache1641659197/.authKey
2025-11-13 19:07:07.4515 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=52168e44-d2de-4aa7-a699-58314a4d1b46
2025-11-13 19:07:07.4515 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 19:07:07.4515 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 19:07:07.4516 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 19:07:07.4519 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 19:07:07.4519 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 19:07:07.4525 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 19:07:07.4829 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 19:07:07.4831 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 19:07:08.3546 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 19:07:08.3566 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 19:07:08.9049 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:07:08.9209 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 19:07:09.3911 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 19:07:09.3912 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 19:07:09.6859 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 19:07:09.9373 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 19:07:10.2291 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 19:07:10.5561 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 19:07:10.8297 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 19:07:11.1012 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 19:07:11.3751 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 19:07:11.6590 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 19:07:11.6590 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 19:07:11.6590 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 19:07:11.6641 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 19:07:12.0110 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 19:07:12.2581 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 19:07:12.4988 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 19:07:12.7428 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 19:07:12.9991 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 19:07:13.0209 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 19:07:13.0209 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 19:07:13.4929 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 19:07:13.9957 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 19:07:14.6622 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-2117350333 --record-with-source
2025-11-13 19:07:14.7070 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 19:07:14.7253 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 19:07:15.2777 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 19:07:15.2803 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 19:07:15.2803 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 19:07:15.2804 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 19:07:15.2806 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:07:15.3025 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 19:07:15.3025 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-3739158592/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 19:07:15.3441 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 19:07:15.3441 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 19:07:15.3441 IST [Polaris Coverity Capture] INFO: 
2025-11-13 19:07:19.3463 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 19:07:19.9010 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:07:19.9677 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 19:07:19.9678 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 19:07:19.9678 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 19:07:19.9679 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 19:07:19.9679 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 19:07:19.9679 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 19:07:19.9679 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32920
2025-11-13 19:07:19.9705 IST [Polaris Coverity Capture] INFO: Capture phase took 11.616s.
2025-11-13 19:07:19.9706 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 19:07:19.9706 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 19:07:19.9706 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 19:07:19.9706 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 19:07:19.9706 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 19:07:19.9983 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 19:07:20.0005 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 19:07:20.0079 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 19:07:20.0081 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 19:07:20.0082 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 19:07:20.0084 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 19:07:20.0104 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 19:07:20.0106 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 19:07:20.0106 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 19:07:20.0594 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 19:07:20.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 19:07:20.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 19:07:20.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 19:07:21.1903 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 19:07:21.1904 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 19:07:21.1904 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 19:07:21.1904 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 19:07:21.1904 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 19:07:21.1904 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 19:07:21.1904 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 19:07:21.3239 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 19:07:21.3240 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 19:07:21.3240 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge [env] 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-13-37-21-284
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm (depth 0)
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/package-lock.json
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/package.json
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 19:07:21.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 19:07:23.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-13-37-21-284/scan/components-with-locations.json
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-13-37-21-284/status/status.json
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-13-37-21-284/scan/components-with-locations.json
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 19:08:06.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 46s 566ms
2025-11-13 19:08:07.0130 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 19:08:07.0132 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 19:08:07.0134 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 19:08:07.0731 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "8681cd61-4258-45a0-aade-3219aee17f13"
2025-11-13 19:08:07.0735 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "71703663-6eac-47b8-b902-ba18f8c298cf"
2025-11-13 19:08:08.6124 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 19:08:08.6256 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 19:08:09.3127 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/385277
2025-11-13 19:08:09.3174 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208946
2025-11-13 19:08:09.5260 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/385277
2025-11-13 19:08:09.5288 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208946
2025-11-13 19:08:09.5430 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208946
2025-11-13 19:08:09.9613 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  55%  212992/385277
2025-11-13 19:08:09.9816 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208946/208946
2025-11-13 19:08:09.9848 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  80%  311296/385277
2025-11-13 19:08:10.1897 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  385277/385277
2025-11-13 19:08:10.4880 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 19:08:10.6855 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 19:08:11.0685 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "71703663-6eac-47b8-b902-ba18f8c298cf"
2025-11-13 19:08:11.1902 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "8681cd61-4258-45a0-aade-3219aee17f13"
2025-11-13 19:08:11.2141 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 19:08:11.2145 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 19:08:11.2151 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 19:08:11.2858 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "8681cd61-4258-45a0-aade-3219aee17f13"
2025-11-13 19:08:11.2863 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "71703663-6eac-47b8-b902-ba18f8c298cf"
2025-11-13 19:08:12.1235 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "71703663-6eac-47b8-b902-ba18f8c298cf" is "Queuing"
2025-11-13 19:08:12.1254 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "8681cd61-4258-45a0-aade-3219aee17f13" is "Queuing"
2025-11-13 19:08:53.4158 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "71703663-6eac-47b8-b902-ba18f8c298cf" is "Scanning & Publishing"
2025-11-13 19:08:53.4858 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "8681cd61-4258-45a0-aade-3219aee17f13" is "Scanning"
2025-11-13 19:10:36.5847 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "71703663-6eac-47b8-b902-ba18f8c298cf" completed successfully
Aborted by admin
[Security Scan] ERROR: An exception occurred while invoking bridge-cli from the plugin: null
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] ERROR: An exception occurred while deleting file: null
[Security Scan] ERROR: An exception occurred while deleting file: null
2025-11-13 19:11:28.3102 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "8681cd61-4258-45a0-aade-3219aee17f13" is "In Progress"
2025-11-13 19:11:35.5195 IST [Polaris Waiter] ERROR: Adapter failed: signal: terminated
[Security Scan] INFO: An exception occurred while processing JSON file for Issue count: null
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
Job Name: MBP_Github_Coverity_Build_Scan/main
[Pipeline] echo
Build Number: 1
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