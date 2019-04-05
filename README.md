# ReactNative (expo) Adroid Window10
This is a simple project to test reactnative on your android mobile with windows 10.

### Configure your phone
First download `Expo, Expo Project` on Google Play Store.
Then set developper mode on your phone:
`Settings -> System -> About Phone -> Clic several times on "Build Number"`
Then Enable these options:
`Settings -> System -> Developper Options -> Enable USB Debogage and, if you can, enable ADB Charger Mode Only`

### Install adb to show the result on your Android Phone
We need to install adb, configure our phone and run adb.
Full installation tutorial :
`https://www.xda-developers.com/install-adb-windows-macos-linux/`
Dowload adb link : 
`https://dl.google.com/android/repository/platform-tools-latest-darwin.zip`

To run adb with cmd:
```sh
cd C:\adb\platform-tools
adb.exe
```
Then you can start or kill the server:
```sh
adb start-server
```
```sh
adb kill-server
```
You can also verify that your phone is correctly regognised  with:
```sh
adb devices
```
When you `adb start-server` or `adb devices`, your phone may prompt you to authorize some stuff, clic Yes.
### To create the same project...
We need expo-cli to build and show the result on our android phone:
```sh
npm install -g expo-cli
```
To create a boilerplate project:
```sh
expo init ProjectName
```

### To run this project...
```sh
cd ProjectName
npm i
expo start
```
or 
```sh
cd ProjectName
npm i
npm start
```

A webpage will open...
Clic on `Run on Android device/emulator`.
Choose a connection `LAN` or `Local`.
To show the result on your phone simply modify the App.js file.

Author: Marc Leonetti & Sven Mathieu
Date: 05/04/2019