# Bloatware remover for | Galaxy S10e (SM-G970F)

This project can help you if

  - You don't have time to search a solution by yourself
  - Don't know how android apps works under the hood
  - Get ride of some apps quickly

# 1. Steps

1. Download and unzip [Minimal ADB and Fastboot (portable version --> zip)](https://forum.xda-developers.com/showthread.php?t=2317790)
    1. After dowloaded ***Minimal ADB and Fastboot***, unzip it where you want
    1. Double click on ***cmd-here.exe***
    1. Type inside CMD window ***adb devices***, it will launch daemon (*daemon not running; *starting now at tcp:5037 * daemon started successfully)
2. [Enable developer options](https://developer.android.com/studio/debug/dev-options#enable)
    1. Settings > About Phone > Information about software > Build Number
    2. Poque it more than 7 times
    3. It will say ***developper mode has been activated***
3. [Enable USB debugging](https://developer.android.com/studio/debug/dev-options#enable)
    1. Go back twice
    2. Inside the parameter app, at the bottom clic at ***developpers options***
    3. Find and toggle ***USB Debugging***
3. Connect your phone to your PC
    1. On your phone autorize ***Autorize phone debugging*** and check ***Always autorize this computer***
4. Check your device connectivity
    1. type ***adb devices*** ,you should see after ***List of devices attached*** your phone with random letters and numbers before the word ***device***
5. Shell
    1. Type ***adb shell*** in CMD, you should see ***beyond0:/ $***
    2. Copy and past list bellow

# 2. Easy list removal

This apps are not needed at all (unless you are using them). If you remove them nothing bad will happened.

### Facebook
pm uninstall -k --user 0 'com.facebook.services'  
pm uninstall -k --user 0 '[com.facebook.katana](https://play.google.com/store/apps/details?id=com.facebook.katana)'  
pm uninstall -k --user 0 'com.facebook.system'  
pm uninstall -k --user 0 'com.facebook.appmanager' 

### Bixby
pm uninstall -k --user 0 'com.samsung.android.app.settings.bixby'  
pm uninstall -k --user 0 'com.samsung.systemui.bixby2'  
pm uninstall -k --user 0 'com.samsung.android.bixby.service'  
pm uninstall -k --user 0 'com.samsung.android.bixby.agent'  
pm uninstall -k --user 0 'com.samsung.android.bixbyvision.framework'  
pm uninstall -k --user 0 'com.samsung.android.bixby.wakeup'  
pm uninstall -k --user 0 'com.samsung.android.bixby.agent.dummy'  
pm uninstall -k --user 0 '[com.samsung.android.app.routines](http://apps.samsung.com/appquery/appDetail.as?appId=com.samsung.android.app.routines&cId=000004770242)'  
pm uninstall -k --user 0 'com.samsung.android.visionintelligence'  
pm uninstall -k --user 0 'com.samsung.android.visionarapps'  

### Knox
pm uninstall -k --user 0 'com.samsung.android.knox.containercore'  
pm uninstall -k --user 0 'com.sec.enterprise.knox.attestation'  
pm uninstall -k --user 0 'com.samsung.android.knox.attestation'  
pm uninstall -k --user 0 'com.samsung.android.knox.containeragent'  
pm uninstall -k --user 0 'com.samsung.knox.keychain'  
pm uninstall -k --user 0 'com.samsung.knox.securefolder'  
pm uninstall -k --user 0 'com.samsung.android.knox.analytics.uploader'  
pm uninstall -k --user 0 'com.knox.vpn.proxyhandler'  
pm uninstall -k --user 0 'com.sec.enterprise.knox.cloudmdm.smdms'  
pm uninstall -k --user 0 'com.android.managedprovisioning'  
pm uninstall -k --user 0 'com.samsung.android.bbc.bbcagent'

### Dex
pm uninstall -k --user 0 'com.sec.android.app.dexonpc'  
pm uninstall -k --user 0 'com.sec.android.app.desktoplauncher'  
pm uninstall -k --user 0 'com.samsung.desktopsystemui'  
pm uninstall -k --user 0 'com.sec.android.desktopmode.uiservice'  

### Samsung Smart Switch Mobile
pm uninstall -k --user 0 'com.samsung.android.smartswitchassistant'  
pm uninstall -k --user 0 'com.sec.android.easyMover.Agent'  
pm uninstall -k --user 0 '[com.sec.android.easyMover](https://play.google.com/store/apps/details?id=com.sec.android.easyMover)'  

### Samsung Pass(word autofill)
pm uninstall -k --user 0 'com.samsung.android.samsungpassautofill'  
pm uninstall -k --user 0 'com.samsung.android.samsungpass'  
pm uninstall -k --user 0 'com.samsung.android.authfw'  

### Galaxy Theme app administrator
pm uninstall -k --user 0 'com.samsung.android.themestore'  
pm uninstall -k --user 0 'com.samsung.android.themecenter'  

### Galaxy Theme styles
pm uninstall -k --user 0 'com.android.theme.icon.square'  
pm uninstall -k --user 0 'com.android.theme.color.cinnamon'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.rounded.systemui'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.rounded.android'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.themepicker'  
pm uninstall -k --user 0 'com.android.theme.color.black'  
pm uninstall -k --user 0 'com.android.theme.color.green'  
pm uninstall -k --user 0 'com.android.theme.color.ocean'  
pm uninstall -k --user 0 'com.android.theme.color.space'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.rounded.launcher'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.settings'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.settings'  
pm uninstall -k --user 0 'com.android.theme.icon.teardrop'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.systemui'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.android'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.systemui'  
pm uninstall -k --user 0 'com.android.theme.icon.squircle'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.launcher'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.launcher'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.themepicker'  
pm uninstall -k --user 0 'com.android.theme.color.orchid'  
pm uninstall -k --user 0 'com.android.theme.color.purple'  
pm uninstall -k --user 0 'com.android.theme.icon.roundedrect'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.rounded.settings'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.android'  

### ANT +
pm uninstall -k --user 0 '[com.dsi.ant.service.socket](https://play.google.com/store/apps/details?id=com.dsi.ant.service.socket)'  
pm uninstall -k --user 0 'com.dsi.ant.sample.acquirechannels'  
pm uninstall -k --user 0 '[com.dsi.ant.plugins.antplus](https://play.google.com/store/apps/details?id=com.dsi.ant.plugins.antplus)'  
pm uninstall -k --user 0 'com.dsi.ant.server'  

### Samsung partner
pm uninstall -k --user 0 '[com.hiya.star](https://play.google.com/store/apps/details?id=com.webascender.callerid)'  
pm uninstall -k --user 0 '[de.axelspringer.yana.zeropage](https://play.google.com/store/apps/details?id=de.axelspringer.yana)'  
pm uninstall -k --user 0 'com.diotek.sec.lookup.dictionary'  

### LED cover
pm uninstall -k --user 0 'com.sec.android.cover.ledcover'  
pm uninstall -k --user 0 'com.samsung.android.app.ledbackcover'  

### Samsung Pay
pm uninstall -k --user 0 'com.samsung.android.spayfw'  
pm uninstall -k --user 0 'com.samsung.android.kgclient'  
pm uninstall -k --user 0 'com.sec.android.app.billing'  

### Samsung Clock
pm uninstall -k --user 0 'com.samsung.android.dynamiclock'  
pm uninstall -k --user 0 'com.sec.android.app.clockpackage'  

### Samsung Games
pm uninstall -k --user 0 'com.samsung.android.game.gamehome'  
pm uninstall -k --user 0 'com.samsung.android.game.gametools'  
pm uninstall -k --user 0 'com.samsung.android.game.gos'  
pm uninstall -k --user 0 'com.samsung.gamedriver.S10MaliG76'  

### Samsung AR
pm uninstall -k --user 0 'com.samsung.android.aremoji'  
pm uninstall -k --user 0 'com.samsung.android.ardrawing'  
pm uninstall -k --user 0 'com.samsung.android.app.camera.sticker.facearframe.preload'  
pm uninstall -k --user 0 'com.samsung.android.app.camera.sticker.facearavatar.preload'  
pm uninstall -k --user 0 'com.samsung.android.app.camera.sticker.facear.preload'  

# Hard list removal
You are probably using one of them. Pay attention about your actions !

### Microsoft
| Syntax      | Description |
| ----------- | ----------- |
| pm uninstall -k --user 0 '[com.microsoft.skydrive](https://play.google.com/store/apps/details?id=com.microsoft.skydrive)' | Microsoft OneDrive |
| pm uninstall -k --user 0 '[com.microsoft.appmanager](https://play.google.com/store/apps/details?id=com.microsoft.appmanager)' | Your Phone Companion - Link to Windows |

### Google
| Syntax      | Description |
| ----------- | ----------- |
| pm uninstall -k --user 0 '[com.android.chrome](https://play.google.com/store/apps/details?id=com.android.chrome)' | Google Chrome: Fast & Secure |
| pm uninstall -k --user 0 '[com.google.android.youtube](https://play.google.com/store/apps/details?id=com.google.android.youtube)' | YouTube |
| pm uninstall -k --user 0 '[com.google.android.googlequicksearchbox](https://play.google.com/store/apps/details?id=com.google.android.googlequicksearchbox)' | Google |
| pm uninstall -k --user 0 '[com.google.ar.core](https://play.google.com/store/apps/details?id=com.google.ar.core)' | Google Play Services for AR |
| pm uninstall -k --user 0 '[com.google.android.gm](https://play.google.com/store/apps/details?id=com.google.android.gm)' | Gmail |
| pm uninstall -k --user 0 '[com.google.android.music](https://play.google.com/store/apps/details?id=com.google.android.music)' | Google Play Music |
| pm uninstall -k --user 0 '[com.google.android.apps.docs](https://play.google.com/store/apps/details?id=com.google.android.apps.docs)' | Google Drive |
| pm uninstall -k --user 0 '[com.google.android.apps.maps](https://play.google.com/store/apps/details?id=com.google.android.apps.maps)' | Maps - Navigate & Explore |
| pm uninstall -k --user 0 '[com.google.android.tts](https://play.google.com/store/apps/details?id=com.google.android.tts)' | Google Text-to-Speech |
| pm uninstall -k --user 0 '[com.google.android.videos](https://play.google.com/store/apps/details?id=com.google.android.videos)' | Google Play Movies & TV |
| pm uninstall -k --user 0 '[com.google.android.apps.photos](https://play.google.com/store/apps/details?id=com.google.android.apps.photos)' | Google Photos |
| pm uninstall -k --user 0 'com.google.android.apps.turbo' | Device Health Services |
| pm uninstall -k --user 0 'com.google.android.gms.location.history' | Historique des positions Google |
| pm uninstall -k --user 0 '[com.google.android.projection.gearhead](https://play.google.com/store/apps/details?id=com.google.android.projection.gearhead)' | Android Auto - Google Maps, Media & Messaging |
| pm uninstall -k --user 0 '[com.google.android.apps.tachyon](https://play.google.com/store/apps/details?id=com.google.android.apps.tachyon)' | Google Duo - High Quality Video Calls |

### Samsung
| Syntax      | Description |
| ----------- | ----------- |
| pm uninstall -k --user 0 'com.samsung.android.app.cocktailbarservice' | Ecran latéral ✔️ |
| pm uninstall -k --user 0 'com.samsung.app.slowmotion' | Rogner ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.calendar' | Calendrier ✔️ |
| pm uninstall -k --user 0 'com.sec.android.inputmethod' | Clavier Samsung ✔️ |
| pm uninstall -k --user 0 'com.osp.app.signin' | Compte Samsung ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.app.contacts' | Contacts ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.forest' | Bien-etre numérique et controles parentaux ✔️ |
| pm uninstall -k --user 0 'com.sec.android.app.samsungapps' | Galaxy Store ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.video' | Lecteur vidéo ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.messaging' | Messages ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.wallpaper.res' | com.samsung.android.wallpaper.res ✔️ |
| pm uninstall -k --user 0 'com.samsung.app.newtrim' | Découpage de vidéos ✔️ |
| pm uninstall -k --user 0 'com.samsung.app.highlightplayer' | Créer un film ✔️ |
| pm uninstall -k --user 0 'com.samsung.storyservice' | Histoire de la Galerie ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.hmt.vrsvc' | Gear VR Service ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.service.livedrawing' | Messages animés ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.app.clipboardedge' | Presse-papiers latéral ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.kidsinstaller' | Programme d'installation Espace enfants ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.svoiceime' | Saisie vocale Samsung ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.app.reminder' | Reminder ✔️ |
| pm uninstall -k --user 0 '[com.sec.android.app.myfiles](https://play.google.com/store/apps/details?id=com.sec.android.app.myfiles)' | Samsung My Files ✔️ |
| pm uninstall -k --user 0 '[com.sec.android.gallery3d](https://play.google.com/store/apps/details?id=com.sec.android.gallery3d)' | Samsung Gallery ✔️ |
| pm uninstall -k --user 0 '[com.samsung.android.app.aodservice](https://play.google.com/store/apps/details?id=com.samsung.android.app.aodservice)' | Always On Display ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.app.sbrowseredge' | Volet Samsung Internet ✔️ |
| pm uninstall -k --user 0 '[com.samsung.android.lool](https://play.google.com/store/apps/details?id=com.samsung.android.lool)' | Device Care ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.scloud' | Samsung Cloud ✔️ |
| pm uninstall -k --user 0 'com.samsung.android.app.spage' | Samsung Daily Beta ✔️ |
| pm uninstall -k --user 0 '[com.sec.android.service.health](https://play.google.com/store/apps/details?id=com.sec.android.app.shealth)' | Samsung Health ✔️ |
| ----------- | ----------- |
| pm uninstall -k --user 0 'com.sec.android.daemonapp' | Meteo ❓ |
| pm uninstall -k --user 0 'com.sec.android.app.quicktool' | Outils ❓ |
| pm uninstall -k --user 0 'com.samsung.android.app.simplesharing' | Partage de liens ❓ |
| pm uninstall -k --user 0 'com.sec.android.sdhms' | Samsung Device Health Manager Service ❓ |
| pm uninstall -k --user 0 'com.samsung.android.mobileservice' | Samsung Experience Service ❓ |
| pm uninstall -k --user 0 'com.samsung.android.mateagent' | Samsung Galaxy Friends ❓ |
| pm uninstall -k --user 0 'com.sec.spp.push' | Samsung push service ❓ |
| pm uninstall -k --user 0 'com.samsung.android.rubin.app' | Service de personnalisation ❓ |
| pm uninstall -k --user 0 'com.sec.android.widgetapp.samsungapps' | Widget Les indisp. Galaxy ❓ |
| pm uninstall -k --user 0 'com.samsung.android.fast' | Wi-Fi sécurisé ❓ |
| pm uninstall -k --user 0 'com.samsung.android.allshare.service.fileshare' | Wi-Fi Direct ❓ |
| pm uninstall -k --user 0 'com.samsung.android.app.watchmanagerstub' | Wearable Manager Installer ❓ |
| pm uninstall -k --user 0 'com.samsung.android.dialer' | Téléphone ❓ |
| pm uninstall -k --user 0 'com.samsung.android.fmm' | Traçage du mobile ❓ |
| pm uninstall -k --user 0 'com.samsung.android.beaconmanager' | SmartThings ❓ |
| pm uninstall -k --user 0 'com.samsung.android.smartfitting' | SmartFittingService ❓ |
| pm uninstall -k --user 0 'com.samsung.android.mdx' | Service Lien avec Windows ❓ |
| pm uninstall -k --user 0 'com.samsung.android.app.mirrorlink' | Samsung MirrorLink 1.1 ❓ |
| pm uninstall -k --user 0 'com.samsung.android.easysetup' | Recherche d'appareils à proximité ❓ |
| pm uninstall -k --user 0 'com.samsung.android.sm.devicesecurity' | Protection ❓ |
| pm uninstall -k --user 0 'com.samsung.android.service.peoplestripe' | Personnes ❓ |
| pm uninstall -k --user 0 'com.samsung.android.app.telephonyui' | Paramètres d'appel ❓ |
| pm uninstall -k --user 0 'com.samsung.android.app.social' | Nouveautés ❓ |
| pm uninstall -k --user 0 'com.samsung.android.da.daagent' | Messagerie double ❓ |
| pm uninstall -k --user 0 'com.samsung.android.app.dressroom' | Fonds d'écran ❓ |
| pm uninstall -k --user 0 'com.samsung.safetyinformation' | Consignes de sécurité ❓ |
| pm uninstall -k --user 0 'com.samsung.android.drivelink.stub' | CarmodeStub ❓ |
| pm uninstall -k --user 0 'com.samsung.android.app.tips' | Astuces ❓ |
| pm uninstall -k --user 0 'com.samsung.android.app.appsedge' | Applications ❓ |
| pm uninstall -k --user 0 'com.samsung.android.mdecservice' | Appels/SMS sur autres appareils ❓ |
| pm uninstall -k --user 0 'com.samsung.android.app.taskedge' | Actions ❓ |
| pm uninstall -k --user 0 'com.samsung.android.contacts' | Contacts Migrator ❓ |
| ----------- | ----------- |
| pm uninstall -k --user 0 'com.samsung.android.app.galaxyfinder' | Finder ***WARNING without this no search bar in parameter*** |
| pm uninstall -k --user 0 '[com.sec.android.app.launcher](https://play.google.com/store/apps/details?id=com.sec.android.app.launcher)' | Samsung One UI Home ***WARNING without this no task manager*** |

### You unistalled an important app, what to do ?
You can restore any app you have 'unistall'
Use this command ***cmd package install-existing XXX*** and replace ***XXX*** by the name of the app.

### You want to submit a new app or post a problem ?
Create an issue and take your time to explain what you want
