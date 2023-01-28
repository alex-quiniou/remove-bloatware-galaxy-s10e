# Bloatware remover for | Galaxy S10e Android 12 (SM-G970F/DS)

# 0. This project can help you if

  - You don't have time to search a solution by yourself.
  - Don't know how android apps works under the hood.
  - Get ride of some apps quickly.

### You want to submit a new app, update an information or post a problem ?

You can help. It's easy. Create an issue and take your time to explain what you want.  
Download this open source [App Manager](https://muntashirakon.github.io/AppManager/) then report here every information you can get on any app.  

### You unistalled an important app, what to do ?
You can restore any app you have 'unistall'  
Use this command ***cmd package install-existing XXX*** and replace ***XXX*** by the name of the app.  

### Want a listing of your apps on your phone ?
After `1.6.i` type ***pm list packages***  

# 1. Steps

1. On your PC : Download and unzip [Minimal ADB and Fastboot (portable version --> zip)](https://forum.xda-developers.com/showthread.php?t=2317790)
    1. After dowloaded ***Minimal ADB and Fastboot***, unzip it where you want
    2. Double click on ***cmd-here.exe***
    3. Type inside CMD window ***adb devices***, it will launch daemon (*daemon not running; *starting now at tcp:5037 * daemon started successfully)
2. On your Samsung SmartPhone : [Enable developer options](https://developer.android.com/studio/debug/dev-options#enable)
    1. Settings > About Phone > Information about software > Build Number
    2. Poque it more than 7 times
    3. It will say ***developper mode has been activated***
3. On your Samsung SmartPhone : [Enable USB debugging](https://developer.android.com/studio/debug/dev-options#enable)
    1. Go back twice
    2. Inside the parameter app, at the bottom clic at ***developpers options***
    3. Find and toggle ***USB Debugging***
4. Connect your phone to your PC
    1. On your phone autorize ***Autorize phone debugging*** and check ***Always autorize this computer***
5. On your PC : Check your device connectivity
    1. type ***adb devices*** ,you should see after ***List of devices attached*** your phone with random letters and numbers before the word ***device***
6. On your PC : Shell
    1. Type ***adb shell*** in CMD, you should see ***beyond0:/ $***
    2. Copy and past list bellow

# 2. Easy list removal
This apps are not needed at all (unless you are using them). If you remove them nothing bad will happened.

## Summary
1. [Facebook](https://github.com/alex-quiniou/remove-bloatware-galaxy-s10e#1-facebook)  
2. [ANT +](https://github.com/alex-quiniou/remove-bloatware-galaxy-s10e#2-ant-)  
3. [Samsung](https://github.com/alex-quiniou/remove-bloatware-galaxy-s10e#3-samsung)  
4. [Microsoft](https://github.com/alex-quiniou/remove-bloatware-galaxy-s10e#4-microsoft)  
5. [Google](https://github.com/alex-quiniou/remove-bloatware-galaxy-s10e#5-google)  

### 1. Facebook
pm uninstall -k --user 0 'com.facebook.services'  
pm uninstall -k --user 0 '[com.facebook.katana](https://play.google.com/store/apps/details?id=com.facebook.katana)'  
pm uninstall -k --user 0 'com.facebook.system'  
pm uninstall -k --user 0 'com.facebook.appmanager' 

### 2. ANT +
pm uninstall -k --user 0 '[com.dsi.ant.service.socket](https://play.google.com/store/apps/details?id=com.dsi.ant.service.socket)'  
pm uninstall -k --user 0 'com.dsi.ant.sample.acquirechannels'  
pm uninstall -k --user 0 '[com.dsi.ant.plugins.antplus](https://play.google.com/store/apps/details?id=com.dsi.ant.plugins.antplus)'  
pm uninstall -k --user 0 'com.dsi.ant.server'  

### 3. Samsung
`Bixby`  
pm uninstall -k --user 0 'com.samsung.android.app.settings.bixby'  
pm uninstall -k --user 0 'com.samsung.systemui.bixby2'  
pm uninstall -k --user 0 'com.samsung.android.bixby.service'  
pm uninstall -k --user 0 'com.samsung.android.bixby.agent'  
pm uninstall -k --user 0 'com.samsung.android.bixby.wakeup'  
pm uninstall -k --user 0 '[com.samsung.android.app.routines](http://apps.samsung.com/appquery/appDetail.as?appId=com.samsung.android.app.routines&cId=000004770242)'  
pm uninstall -k --user 0 'com.samsung.android.visionintelligence'  

`Knox`  
pm uninstall -k --user 0 'com.samsung.android.knox.containercore'  
pm uninstall -k --user 0 'com.samsung.android.knox.attestation'  
pm uninstall -k --user 0 'com.samsung.android.knox.containeragent'  
pm uninstall -k --user 0 'com.samsung.android.knox.pushmanager'  
pm uninstall -k --user 0 'com.samsung.android.knox.analytics.uploader'  
pm uninstall -k --user 0 'com.samsung.android.bbc.bbcagent'  
pm uninstall -k --user 0 'com.samsung.knox.securefolder'  
pm uninstall -k --user 0 'com.knox.vpn.proxyhandler'  
pm uninstall -k --user 0 'com.sec.enterprise.knox.cloudmdm.smdms'  
pm uninstall -k --user 0 'com.samsung.android.knox.kpecore'  

`Dex`  
pm uninstall -k --user 0 'com.sec.android.app.dexonpc'  
pm uninstall -k --user 0 'com.sec.android.app.desktoplauncher'  
pm uninstall -k --user 0 'com.samsung.desktopsystemui'  
pm uninstall -k --user 0 'com.sec.android.desktopmode.uiservice'  

`Samsung Smart Switch Mobile`  
pm uninstall -k --user 0 'com.samsung.android.smartswitchassistant'  
pm uninstall -k --user 0 'com.sec.android.easyMover.Agent'  

`Samsung Pass(word autofill)`  
pm uninstall -k --user 0 'com.samsung.android.samsungpassautofill'  
pm uninstall -k --user 0 'com.samsung.android.samsungpass'  
pm uninstall -k --user 0 'com.samsung.android.authfw'  

`Galaxy Theme app administrator`  
pm uninstall -k --user 0 'com.samsung.android.themestore'  
pm uninstall -k --user 0 'com.samsung.android.themecenter'  

`Galaxy Theme styles`  
pm uninstall -k --user 0 'com.android.theme.font.notoserifsource'  

`Samsung partner`  
pm uninstall -k --user 0 '[com.hiya.star](https://play.google.com/store/apps/details?id=com.webascender.callerid)'  
pm uninstall -k --user 0 '[de.axelspringer.yana.zeropage](https://play.google.com/store/apps/details?id=de.axelspringer.yana)'  
pm uninstall -k --user 0 'com.diotek.sec.lookup.dictionary'  

`LED cover`  
pm uninstall -k --user 0 'com.sec.android.cover.ledcover'  
pm uninstall -k --user 0 'com.samsung.android.app.ledbackcover'  

`Samsung Pay`  
pm uninstall -k --user 0 'com.samsung.android.spayfw'  
pm uninstall -k --user 0 'com.samsung.android.kgclient'  
pm uninstall -k --user 0 'com.sec.android.app.billing'  

`Samsung Games`  
pm uninstall -k --user 0 'com.samsung.android.game.gamehome'  
pm uninstall -k --user 0 'com.samsung.android.game.gametools'  
pm uninstall -k --user 0 'com.samsung.android.game.gos'  
pm uninstall -k --user 0 'com.samsung.gamedriver.ex9820'  

`Samsung AR`  
pm uninstall -k --user 0 'com.samsung.android.aremoji'  
pm uninstall -k --user 0 'com.samsung.android.ardrawing'  
pm uninstall -k --user 0 'com.samsung.android.app.camera.sticker.facearavatar.preload'  
pm uninstall -k --user 0 'com.samsung.android.arzone'  
pm uninstall -k --user 0 'com.samsung.android.livestickers'  
pm uninstall -k --user 0 'com.samsung.android.hmt.vrsvc'  

`Samsung Share apps`  
pm uninstall -k --user 0 'com.samsung.android.app.simplesharing'  
pm uninstall -k --user 0 'com.samsung.android.aware.service'  
pm uninstall -k --user 0 'com.samsung.android.app.sharelive'  
pm uninstall -k --user 0 'com.samsung.android.privateshare'  

`Lateral Panel`  
pm uninstall -k --user 0 'com.samsung.android.app.clipboardedge'  
pm uninstall -k --user 0 'com.sec.android.app.quicktool'  
pm uninstall -k --user 0 'com.samsung.android.mdx.quickboard'  
pm uninstall -k --user 0 'com.samsung.android.app.cocktailbarservice'  
pm uninstall -k --user 0 'package:com.samsung.android.app.appsedge'  
pm uninstall -k --user 0 'package:com.samsung.android.app.taskedge' 

`Samsung Clock`  
pm uninstall -k --user 0 'com.sec.android.app.clockpackage'  

`Samsung My Files`  
pm uninstall -k --user 0 'com.sec.android.app.myfiles'  

`Samsung Gallery`  
pm uninstall -k --user 0 'com.sec.android.gallery3d'  

`Always On Display`  
pm uninstall -k --user 0 'com.samsung.android.app.aodservice'  

`Device Care`  
pm uninstall -k --user 0 '[com.samsung.android.lool](https://play.google.com/store/apps/details?id=com.samsung.android.lool)'  

`Samsung Visit in` (add a banner add notification when it things you are near a samsung store)  
pm uninstall -k --user 0 'com.samsung.android.ipsgeofence'  

`Secure Wi-fi` (limited VPN offering)  
pm uninstall -k --user 0 'com.samsung.android.fast'  

`Samsung Experience Service / Group Sharing`  
pm uninstall -k --user 0 'com.samsung.android.mobileservice'  

`Calendrier`  
pm uninstall -k --user 0 'com.samsung.android.calendar'  

`Contacts`  
pm uninstall -k --user 0 'com.samsung.android.app.contacts'  

`Bien-etre numérique et controles parentaux`  
pm uninstall -k --user 0 'com.samsung.android.forest'  

`Lecteur vidéo`  
pm uninstall -k --user 0 'com.samsung.android.video'  

`Messages`  
pm uninstall -k --user 0 'com.samsung.android.messaging'  

pm uninstall -k --user 0 'com.samsung.android.wallpaper.res'  

`Découpage de vidéos`  
pm uninstall -k --user 0 'com.samsung.app.newtrim'  

`Messages animés`  
pm uninstall -k --user 0 'com.samsung.android.service.livedrawing'  

`Programme d'installation Espace enfants`  
pm uninstall -k --user 0 'com.samsung.android.kidsinstaller'  

`Saisie vocale Samsung`  
pm uninstall -k --user 0 'com.samsung.android.svoiceime'  

`Reminder`  
pm uninstall -k --user 0 'com.samsung.android.app.reminder'  

`Samsung Cloud`  
pm uninstall -k --user 0 'com.samsung.android.scloud'  

`Samsung Daily Beta`  
pm uninstall -k --user 0 'com.samsung.android.app.spage'  

`Astuces`  
pm uninstall -k --user 0 'com.samsung.android.app.tips'  

`Service Lien avec Windows`  
pm uninstall -k --user 0 'com.samsung.android.mdx'  

`Capture Samsung`  
pm uninstall -k --user 0 'com.samsung.android.app.smartcapture'  

`Clavier Samsung`  
pm uninstall -k --user 0 'com.samsung.android.honeyboard'  

`Samsung Galaxy Friends`  
pm uninstall -k --user 0 'com.samsung.android.mateagent'  

`Smart View`  
pm uninstall -k --user 0 'com.samsung.android.smartmirroring'  

`Wearable Manager Installer`  
pm uninstall -k --user 0 'com.samsung.android.app.watchmanagerstub'  

### 4. Microsoft
`Microsoft OneDrive`  
pm uninstall -k --user 0 '[com.microsoft.skydrive](https://play.google.com/store/apps/details?id=com.microsoft.skydrive)'  

`Your Phone Companion - Link to Windows`  
pm uninstall -k --user 0 '[com.microsoft.appmanager](https://play.google.com/store/apps/details?id=com.microsoft.appmanager)'   

### 5. Google
`Google Chrome: Fast & Secure`  
pm uninstall -k --user 0 '[com.android.chrome](https://play.google.com/store/apps/details?id=com.android.chrome)'  

`YouTube`  
pm uninstall -k --user 0 '[com.google.android.youtube](https://play.google.com/store/apps/details?id=com.google.android.youtube)'  

`Google`  
pm uninstall -k --user 0 '[com.google.android.googlequicksearchbox](https://play.google.com/store/apps/details?id=com.google.android.googlequicksearchbox)'  

`Google Play Services for AR`  
pm uninstall -k --user 0 '[com.google.ar.core](https://play.google.com/store/apps/details?id=com.google.ar.core)'  

`Gmail`  
pm uninstall -k --user 0 '[com.google.android.gm](https://play.google.com/store/apps/details?id=com.google.android.gm)'  

`Google Play Music`  
pm uninstall -k --user 0 '[com.google.android.music](https://play.google.com/store/apps/details?id=com.google.android.music)'  

`Google Drive`  
pm uninstall -k --user 0 '[com.google.android.apps.docs](https://play.google.com/store/apps/details?id=com.google.android.apps.docs)'  

`Maps - Navigate & Explore`  
pm uninstall -k --user 0 '[com.google.android.apps.maps](https://play.google.com/store/apps/details?id=com.google.android.apps.maps)'  

`Google Text-to-Speech`  
pm uninstall -k --user 0 '[com.google.android.tts](https://play.google.com/store/apps/details?id=com.google.android.tts)'  

`Google Play Movies & TV`  
pm uninstall -k --user 0 '[com.google.android.videos](https://play.google.com/store/apps/details?id=com.google.android.videos)'  

`Google Photos`  
pm uninstall -k --user 0 '[com.google.android.apps.photos](https://play.google.com/store/apps/details?id=com.google.android.apps.photos)'  

`Device Health Services`  
pm uninstall -k --user 0 '[com.google.android.apps.turbo](https://play.google.com/store/apps/details?id=com.google.android.apps.turbo)'  

`Services Google Play`  
pm uninstall -k --user 0 '[com.google.android.gms](https://play.google.com/store/apps/details?id=com.google.android.gms)'  

`Android System WebView`  
pm uninstall -k --user 0 '[com.google.android.webview](https://play.google.com/store/apps/details?id=com.google.android.webview)'  

`Services de personnalisation de l'appareil`  
pm uninstall -k --user 0 '[com.google.android.as](https://play.google.com/store/apps/details?id=com.google.android.as)'  

`Android Auto - Google Maps, Media & Messaging`  
pm uninstall -k --user 0 '[com.google.android.projection.gearhead](https://play.google.com/store/apps/details?id=com.google.android.projection.gearhead)'  

`Google Duo - High Quality Video Calls`  
pm uninstall -k --user 0 '[com.google.android.apps.tachyon](https://play.google.com/store/apps/details?id=com.google.android.apps.tachyon)'  

# 3. Hard list removal
All apps names are stored in the last MD file up there. Check the last `APP LIST` file created.
