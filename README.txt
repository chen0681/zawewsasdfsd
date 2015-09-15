cordova platform add android@3.6.4

mirrors.opencas.cn:80

#Installed Cordova plugin
cordova plugin add cordova-plugin-file
cordova plugin add cordova-plugin-file-transfer
cordova plugin add cordova-plugin-inappbrowser
cordova plugin add cordova-plugin-device
cordova plugin add cordova-plugin-console
cordova plugin add cordova-plugin-statusbar
cordova plugin add cordova-plugin-network-information
cordova plugin add cordova-plugin-splashscreen

cordova plugin add org.apache.cordova.statusbar

#require function for merge the js
node r.js -o baseUrl=js name=main out=built.js optimize=none excludeShallow=selector paths.jquery=empty:

#require function for merge css --@import url("nav.css");
node r.js -o cssIn=css/main.css out=css/built.css

#test 
npm install -g ripple-emulator
ripple emulate

http://www.runoob.com/bootstrap

http://www.bootcss.com/p/font-awesome/#