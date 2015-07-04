# Drone.io
https://drone.io/github.com/HazemKhaled/Cordova-Build-with-drone.io

```
# Setup Android SDK
export ANDROID_HOME=`pwd`/android-sdk-linux
export PATH=${ANDROID_HOME}/tools:${ANDROID_HOME}/platform-tools:${PATH}
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
