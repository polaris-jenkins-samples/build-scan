# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Async_Mode_Scan/main`
- **Build Number:** #1
- **Build Status:** 🔴 **FAILURE**
- **Duration:** 19 min and counting
- **Timestamp:** 2025-11-13 20:48:43 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 9d13fa027cb15eaa845eccf38b3f96c964aed0a9
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
 > git init /Users/madhusud/.jenkins/workspace/hub_Polaris_Async_Mode_Scan_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb # timeout=10
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
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/polaris-jenkins-samples/build-scan.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/build-scan.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/build-scan.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Avoid second fetch
Checking out Revision 9d13fa027cb15eaa845eccf38b3f96c964aed0a9 (main)
Commit message: "Jenkins log upload - Build #5"
First time build. Skipping changelog.
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/build-scan.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 9d13fa027cb15eaa845eccf38b3f96c964aed0a9 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Polaris_Async_Mode_Scan/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm
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
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options

added 962 packages, and audited 1412 packages in 22s

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
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Async_Mode_Scan
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
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Async_Mode_Scan
[Security Scan] INFO: Polaris Application Name: async-mode
[Security Scan] INFO: Polaris Project Name: async-mode
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Async_Mode_Scan
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/polaris_input17015110823949242676.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 20:29:34.8985 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 20:29:34.9087 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 20:29:36.2259 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 20:29:36.2259 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 20:29:36.2259 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 20:29:36.2259 IST [Bridge CLI] INFO: network.airgap = false [polaris_input17015110823949242676.json]
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: network.ssl.trustAll = false [polaris_input17015110823949242676.json]
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input17015110823949242676.json]
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: polaris.application.name = async-mode [polaris_input17015110823949242676.json]
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input17015110823949242676.json]
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input17015110823949242676.json]
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: polaris.project.name = async-mode [polaris_input17015110823949242676.json]
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input17015110823949242676.json]
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input17015110823949242676.json]
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 20:29:36.2260 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 20:29:36.2280 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 20:29:36.2280 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 20:29:36.2280 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 20:29:36.2280 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 20:29:36.3768 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 20:29:36.3804 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 20:29:36.3805 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 20:29:36.3806 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 20:29:36.3836 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 20:29:36.3837 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 20:29:36.3837 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 20:29:39.3303 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "GIR1YDA"
2025-11-13 20:29:39.3307 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "NOL16LL"
2025-11-13 20:29:39.3669 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 20:29:39.3671 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 20:29:39.3673 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 20:29:39.3675 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 20:29:39.3677 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 20:29:39.3678 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 20:29:39.3680 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 20:29:39.3682 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 20:29:39.3684 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 20:29:39.3686 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 20:29:39.3692 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 20:29:39.3901 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 20:29:39.4571 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 20:29:39.4574 IST [Check pull request] INFO: Adapter finished
2025-11-13 20:29:39.5043 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 20:29:39.5047 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 20:29:40.2973 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 20:29:40.2974 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 20:29:40.2992 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 20:29:40.3989 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 20:29:40.7087 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 20:29:40.7089 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 20:29:41.0068 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 20:29:41.0068 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 20:29:41.0082 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 20:29:41.0918 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 20:29:41.3960 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 20:29:41.3961 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 20:29:41.3961 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 20:29:41.6980 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 20:29:41.6981 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 20:29:41.7771 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 20:29:41.7813 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 20:29:42.0857 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 20:29:42.1222 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 20:29:42.1224 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 20:29:42.1226 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 20:29:42.1227 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 20:29:42.1227 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 20:29:42.1227 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 20:29:42.1227 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 20:29:42.1246 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 20:29:42.1246 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 20:29:42.1246 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 20:29:42.1246 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 20:29:42.1246 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 20:29:42.1280 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 20:29:42.1246 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 20:29:42.1642 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 20:29:42.1673 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 20:29:42.1673 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 20:29:42.1750 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 20:29:42.1787 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 20:29:42.1787 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 20:29:42.2702 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 20:29:42.2742 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 20:29:42.3298 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 20:29:42.3298 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache4131172216/.authKey
2025-11-13 20:29:42.3299 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=673c666f-5f9a-4514-b30a-9817bd0c02b1
2025-11-13 20:29:42.3299 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 20:29:42.3299 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 20:29:42.3299 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 20:29:42.3328 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 20:29:42.3328 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 20:29:42.3341 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 20:29:42.4157 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 20:29:42.4160 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 20:29:43.3703 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 20:29:43.3718 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 20:29:43.8840 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 20:29:43.8990 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 20:29:44.5840 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 20:29:44.5846 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 20:29:44.9848 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 20:29:45.2728 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 20:29:45.5601 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 20:29:45.8157 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 20:29:46.0718 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 20:29:46.3166 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 20:29:46.6379 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 20:29:47.0107 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 20:29:47.0108 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 20:29:47.0108 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 20:29:47.0190 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 20:29:47.3820 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 20:29:47.7030 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 20:29:48.0287 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 20:29:48.3569 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 20:29:48.6494 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 20:29:48.6663 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 20:29:48.6663 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 20:29:49.2473 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 20:29:49.6577 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 20:29:50.2101 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-384625329 --record-with-source
2025-11-13 20:29:50.2475 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 20:29:50.2630 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 20:29:50.8001 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 20:29:50.8033 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 20:29:50.8034 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 20:29:50.8036 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 20:29:50.8039 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 20:29:50.8290 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 20:29:50.8291 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-4079647080/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 20:29:50.8624 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 20:29:50.8624 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 20:29:50.8624 IST [Polaris Coverity Capture] INFO: 
2025-11-13 20:29:52.5700 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 20:29:53.0624 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 20:29:53.1182 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 20:29:53.1182 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 20:29:53.1182 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 20:29:53.1183 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 20:29:53.1183 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 20:29:53.1183 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 20:29:53.1183 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32920
2025-11-13 20:29:53.1204 IST [Polaris Coverity Capture] INFO: Capture phase took 9.75s.
2025-11-13 20:29:53.1205 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 20:29:53.1205 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 20:29:53.1205 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 20:29:53.1205 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 20:29:53.1205 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 20:29:53.1438 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 20:29:53.1456 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 20:29:53.1523 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 20:29:53.1524 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 20:29:53.1526 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 20:29:53.1528 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 20:29:53.1546 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 20:29:53.1547 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 20:29:53.1548 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 20:29:53.2015 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 20:29:53.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 20:29:53.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 20:29:53.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 20:29:54.2572 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 20:29:54.2573 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 20:29:54.2573 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 20:29:54.2573 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 20:29:54.2573 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 20:29:54.2573 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 20:29:54.2573 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 20:29:54.3910 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 20:29:54.3910 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 20:29:54.3911 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge [env] 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-14-59-54-350
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 20:29:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm (depth 0)
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/package-lock.json
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/package.json
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 20:29:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 20:29:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-14-59-54-350/scan/components-with-locations.json
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-14-59-54-350/status/status.json
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-14-59-54-350/scan/components-with-locations.json
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 46s 649ms
2025-11-13 20:30:40.1955 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 20:30:40.1957 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 20:30:40.1958 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 20:30:40.2472 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "8b24c5fd-0e64-4d73-8a36-fc427c3cc31d"
2025-11-13 20:30:40.2477 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "e17b85f3-20c4-42d7-a28b-2383b7bec74c"
2025-11-13 20:30:41.6278 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 20:30:41.7093 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 20:30:42.3240 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/385478
2025-11-13 20:30:42.3253 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208944
2025-11-13 20:30:42.5358 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/385478
2025-11-13 20:30:42.5422 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208944
2025-11-13 20:30:42.5422 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208944
2025-11-13 20:30:42.9643 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  55%  212992/385478
2025-11-13 20:30:42.9688 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208944/208944
2025-11-13 20:30:42.9689 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  80%  311296/385478
2025-11-13 20:30:43.1808 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  385478/385478
2025-11-13 20:30:43.4991 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 20:30:43.6982 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 20:30:44.0591 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "e17b85f3-20c4-42d7-a28b-2383b7bec74c"
2025-11-13 20:30:44.2001 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "8b24c5fd-0e64-4d73-8a36-fc427c3cc31d"
2025-11-13 20:30:44.2075 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 20:30:44.2082 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 20:30:44.2084 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 20:30:44.2464 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "8b24c5fd-0e64-4d73-8a36-fc427c3cc31d"
2025-11-13 20:30:44.2470 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "e17b85f3-20c4-42d7-a28b-2383b7bec74c"
2025-11-13 20:30:45.0328 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "e17b85f3-20c4-42d7-a28b-2383b7bec74c" is "Waiting for Capture"
2025-11-13 20:30:45.1240 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "8b24c5fd-0e64-4d73-8a36-fc427c3cc31d" is "Waiting for Capture"
2025-11-13 20:30:55.3909 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "e17b85f3-20c4-42d7-a28b-2383b7bec74c" is "Scanning & Publishing"
2025-11-13 20:30:55.4316 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "8b24c5fd-0e64-4d73-8a36-fc427c3cc31d" is "Scanning"
2025-11-13 20:31:26.4205 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "8b24c5fd-0e64-4d73-8a36-fc427c3cc31d" completed successfully
2025-11-13 20:48:40.1507 IST [Polaris Waiter] ERROR: error while waiting for test with assessment type "SCA(scaPackage)" and id "e17b85f3-20c4-42d7-a28b-2383b7bec74c": error while fetching test state: Get "https://poc.polaris.blackduck.com/api/tests/e17b85f3-20c4-42d7-a28b-2383b7bec74c": read tcp 10.230.18.190:51061->104.18.35.236:443: read: operation timed out
2025-11-13 20:48:40.1693 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 20:48:40.1699 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 20:48:40.1707 IST [Polaris Waiter] ERROR: Adapter failed: exit status 1
2025-11-13 20:48:40.2674 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 20:48:40.2686 IST [Polaris Policy Checker] WARNING: Skipping policy violations check for "SCA(scaPackage)" assessment with id "e17b85f3-20c4-42d7-a28b-2383b7bec74c", as the test is not completed
2025-11-13 20:48:41.6394 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 20:48:41.6737 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 20:48:41.7400 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 20:48:41.7407 IST [Polaris Issues Fetcher] WARNING: Will not fetch issues for "SCA(scaPackage)" assessment, as the test is not completed
2025-11-13 20:48:42.5339 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "8b24c5fd-0e64-4d73-8a36-fc427c3cc31d"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 20:48:42.5618 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 20:48:42.5623 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 20:48:42.5627 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 20:48:42.5631 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 20:48:42.5633 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 20:48:42.5637 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 20:48:42.6161 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "8b24c5fd-0e64-4d73-8a36-fc427c3cc31d" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f6f40d05-1268-4824-a147-bd35b7506448/projects/e684c68e-3360-40f9-8953-62fcc9d0e027/tests/8b24c5fd-0e64-4d73-8a36-fc427c3cc31d/detected-issues
2025-11-13 20:48:42.6167 IST [Polaris Status Provider] INFO: Polaris issues view for project "async-mode", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f6f40d05-1268-4824-a147-bd35b7506448/projects/e684c68e-3360-40f9-8953-62fcc9d0e027/issues?branchId=7e8ffa23-8d7b-46ec-9991-911babeaca87
2025-11-13 20:48:42.6258 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 20:48:42.6260 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 20:48:42.6264 IST [Polaris Status Provider] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 40
[Security Scan] ERROR: Workflow failed! Exit code 2: Error from adapter
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
Job Name: MBP_Github_Polaris_Async_Mode_Scan/main
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