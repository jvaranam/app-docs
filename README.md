# app-docs
documents for creating the ios and android applications


# apk from windows

# apk from mac

adb devices / adb devices -l  --> list of the devices connected to usb

adb kill-server 9  --> kill the server  

adb start-server   --> start the server

cordova platform rm android && cordova platform add android@latest && cordova build android





# ipa from mac

error == Code signing is required for product type 'Application' in SDK 'iOS 10.2'
solution 
1. add plugins 
2. add platforms
3. open the .xcodeproj file which is there in platforms/ios/{application name}.xcodeproj
4. select the {application name} from the left side
5. select target
6. deselect "automatically manage signin"
7. signin(debug) select the provisioning profile 
8. signin(release) select the provisioning profile
..
9. clean the code by "product" "clean" on menu
10. either run the command for build app or use xcode for build the app.
