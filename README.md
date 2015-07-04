# [Drone.io](http://Drone.io) - Android only
[Check Example](https://drone.io/github.com/HazemKhaled/Cordova-Build-with-drone.io)

## Environment Variables 
```
# Setup Android SDK
ANDROID_HOME=`pwd`/android-sdk-linux
PATH=${ANDROID_HOME}/tools:${ANDROID_HOME}/platform-tools:${PATH}
```

## Commands
```
wget -q http://dl.google.com/android/android-sdk_r24.3.3-linux.tgz
tar xf android-sdk_r24.3.3-linux.tgz
echo y | android update sdk -u -a -t 1,2,5,24

# Install Cordova
npm install -g cordova

# Let's get add Android platform there
cordova platform add android

# Build you app
cordova build android --release
```
