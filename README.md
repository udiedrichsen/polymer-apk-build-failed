# polymer-apk-build-failed

Just a test repo using Polymer 1.0

meteor add-platform android

Run fine in brower but I try to build this:
meteor build ../BUILDDIR --server 192.168.178.53:3000

When I try to run it on an android-device is the app is not starting on the device (works also not in the emulator):

meteor run android-device

# Error message
meteor build ../BUILDDIR --server 192.168.178.53:3000
                                              
/Users/doedel/.meteor/packages/meteor-tool/.1.1.3.1wysac9++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/fibers/future.js:245
						throw(ex);
						      ^
Error: The APK file for the Android build was not found.
    at findApkPath (/Users/doedel/.meteor/packages/meteor-tool/.1.1.3.1wysac9++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/tools/commands.js:970:11)
    at /Users/doedel/.meteor/packages/meteor-tool/.1.1.3.1wysac9++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/tools/commands.js:950:21
    at Array.forEach (native)
    at Function._.each._.forEach (/Users/doedel/.meteor/packages/meteor-tool/.1.1.3.1wysac9++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:79:11)
    at buildCommand (/Users/doedel/.meteor/packages/meteor-tool/.1.1.3.1wysac9++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/tools/commands.js:933:29)
    at Command.main.registerCommand._.extend.name [as func] (/Users/doedel/.meteor/packages/meteor-tool/.1.1.3.1wysac9++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/tools/commands.js:746:12)
    at /Users/doedel/.meteor/packages/meteor-tool/.1.1.3.1wysac9++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/tools/main.js:1363:23

# Building the APP without android platform works.

# Building the APP for ios platform works also !
