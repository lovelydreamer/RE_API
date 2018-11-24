# RE_API
Reverse Engineer an API

Set up a proxied emulator. Here's some good instructions:
https://www.versionestabile.it/blog/ios-simulator-and-android-emulator-http-proxy/

tools > AVD Manager - follow prompts to choose device. 
after setting up the device and adding the cert, be sure to toggle off the proxy settings in the emulator. 
this is to allow yourself to sign into the play store. also turn on "wireless" in case that's a hold up. 
I had to toggle it on to continue this testing. 

then I got an error.

next was: 
https://www.geek.com/geek-pick/what-is-adb-and-how-do-i-use-it-1461697/
android SDK tools

in the emulator
/Users/{usr name}/Library/Android/sdk/platform-tools
export PATH=/Users/{usr name}/Library/Android/sdk/platform-tools:$PATH
source ~/.profile
adb shell
bam!

but wait. you can't download from the playstore the target app.
