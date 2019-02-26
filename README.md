# demo-rn-fcm 

Demo React Native working with [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) 

## Prerequisite

- [NodeJS](https://nodejs.org/en/)
- [React Native CLI](https://facebook.github.io/react-native/)


## Create your own Firebase project

- Go to [Firebase console](https://console.firebase.google.com) and create your own project.
- Click on Android or iOS (Depend what platform you want to do) and then follow those step to register your app.

Package name : **com.demofcm**

Bundle ID : **org.reactjs.native.example.demoFCM**

***Default of this project will be this name. So if you work on other project, You need to use your own package name (Android) or bundle ID (iOS)** 

## Getting started

Clone repo and install all dependencies

```
$ git@github.com:avalond/fcm-rn-demo.git
$ cd demo-rn-fcm
$ npm install
```

## Download Firebase configuration files

When you try to register your app on Firebase project. It will ask you to download configuration file to specific path (depend on what platform you had choosed)

**Android** : _demo-rn-fcm/android/app/google-services.json_

**iOS** : _demo-rn-fcm/ios/demoFCM/GoogleService-Info.plist_

## Run

```
$ react-native run-android
```


## Test on your FCM console

Access your Firebase console project

- Go to Cloud Messaging page and start compose message
- Click on **Test on device** and put token that display on running device.
- Press **Test** Button

If setup correctly, Then notification message will shown on your running device.

_Notification will not show if your app running in Foreground. Make sure exit app or go to home screen first_
