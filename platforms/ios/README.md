

## Mobile Foundation with Ionic
Bluemix MobileFoundation Starter for Ionic in IOS

[![](https://img.shields.io/badge/bluemix-powered-blue.svg)](https://bluemix.net)
[![Platform](https://img.shields.io/badge/platform-ios_swift-lightgrey.svg?style=flat)](https://developer.apple.com/swift/)

### Table of Contents
* [Summary](#summary)
* [Requirements](#requirements)
* [Mobile Foundation Dependency Management](#mfpdependencymanagement)
* [Mobile Foundation Configuration](#mfpconfiguration)
* [Run](#run)
* [License](#license)

### Summary
This Bluemix Mobile Starter will showcase the Ionic 3 getting started with Mobile Foundations on Bluemix.

### Requirements
* iOS 8.0+
* Xcode 8
* Node 6.0 or above
* Ionic CLI 3.10 or above

### Mobile Foundation Dependency Management
Run the below command to install all the node modules required for building the application.
```bash
$ npm install
```

### Mobile Foundation Configuration
This starter invokes an adapter in a Mobile foundation server.
##### Steps:
* Goto the project folder and find a shell scripts by name **mfpregisterapp.sh** and **mfpstartersetup.sh** and ensure that you have execute and write permissions in order to run these scripts.
* run **mfpstartersetup.sh**. This should set up the Mobile Foundation prereqs for running the starter
* Replace url in config.xml with the host of the mobile foundation provisioned for you. <mfp:server runtime="mfp" url="" />
* Add the mfp cordova plugin
```bash
$ ionic cordova plugin add cordova-plugin-mfp
```
* Build the ionic application to run ionic build scripts
```bash
$ ionic build
```

The Bluemix Mobile services SDK uses [CocoaPods](https://cocoapods.org/) to manage and configure dependencies. To use our latest SDKs you need version 1.1.0.rc.2.


Now Open the Xcode workspace: `{APP_Name}.xcworkspace`. From now on, open the `.xcworkspace` file becuase it contains all the dependencies and configurations.

If you run into any issues during the pod install, it is recommended to run a pod update by using the following commands:

```bash
$ pod update
$ pod install
```



### Run
You can now run the application on a simulator or physical device:




### License
This package contains code licensed under the Apache License, Version 2.0 (the "License"). You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0 and may also view the License in the LICENSE file within this package.
 
