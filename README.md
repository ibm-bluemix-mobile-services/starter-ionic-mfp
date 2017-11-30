

## Mobile Foundation with Ionic
Bluemix Mobile Foundation Starter with Ionic 3 in Cordova

[![](https://img.shields.io/badge/bluemix-powered-blue.svg)](https://bluemix.net)
[![Platform](https://img.shields.io/badge/platform-android-lightgrey.svg?style=flat)](https://developer.android.com/index.html)


### Table of Contents
* [Summary](#summary)
* [Requirements](#requirements)
* [Mobile Foundation Dependency Management](#mfpdependencymanagement)
* [Mobile Foundation Configuration](#mfpconfiguration)
* [Run](#run)
* [License](#license)


### Summary
This Bluemix Mobile Starter showcases the getting started steps for Ionic 3  with Mobile Foundation on Bluemix.


### Requirements
* [Android Studio](https://developer.android.com/studio/index.html)
* XCode 9.0+
* A [Bluemix Account](https://www.bluemix.net/)
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
* Go to the **platforms/android** folder and find the shell scripts by name **mfpregisterapp.sh** and **mfpstartersetup.sh**. Ensure that you have **execute** and **write** permissions in order to run these scripts.
* Run **mfpstartersetup.sh**. This should set up the Mobile Foundation prereqs for running the starter
Go to the **platforms/ios** folder and find the shell scripts by name **mfpregisterapp.sh** and **mfpstartersetup.sh**. Ensure that you have **execute** and **write** permissions in order to run these scripts.
* Run **mfpstartersetup.sh**. This should set up the Mobile Foundation prereqs for running the starter
* MFP cordova plugin requires updated cordova platforms.
```bash
$ ionic cordova platform update android ios
```
* If cordova fails in updating the ios platform, please remove and add the ios platform again.
``` bash
$ ionic cordova platform rm ios
$ ionic cordova platform add ios
```

* Add the mfp cordova plugin
```bash
$ ionic cordova plugin add cordova-plugin-mfp
```
* Replace url in config.xml with the host of the mobile foundation provisioned for you. <mfp:server runtime="mfp" url="" />

* Build the ionic application to run ionic build scripts
```bash
$ ionic build
```
* Open the project under **platforms/android** in Android Studio and perform a Gradle Sync.
* Open the project under **platforms/ios** in XCode and build it.


### Run
You can now run the application on a simulator or physical device:


### License
This package contains code licensed under the Apache License, Version 2.0 (the "License"). You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0 and may also view the License in the LICENSE file within this package.
